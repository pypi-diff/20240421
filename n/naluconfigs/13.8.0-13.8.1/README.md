# Comparing `tmp/naluconfigs-13.8.0.tar.gz` & `tmp/naluconfigs-13.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naluconfigs-13.8.0.tar", last modified: Fri Apr  5 23:36:54 2024, max compression
+gzip compressed data, was "naluconfigs-13.8.1.tar", last modified: Sun Apr 21 16:04:33 2024, max compression
```

## Comparing `naluconfigs-13.8.0.tar` & `naluconfigs-13.8.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:36:54.733826 naluconfigs-13.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-05 23:36:54.733826 naluconfigs-13.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 23:36:54.733826 naluconfigs-13.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:36:54.717826 naluconfigs-13.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:36:54.717826 naluconfigs-13.8.0/src/naluconfigs/
--rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/_constructors.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:36:54.717826 naluconfigs-13.8.0/src/naluconfigs/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:36:54.721826 naluconfigs-13.8.0/src/naluconfigs/data/chips/
--rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/chips/aardvarcv3.yml
--rw-r--r--   0 runner    (1001) docker     (127)    21891 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/chips/aardvarcv4.yml
--rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/chips/aodsv1.yml
--rw-r--r--   0 runner    (1001) docker     (127)    15860 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/chips/aodsv2.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/chips/asocv3.yml
--rw-r--r--   0 runner    (1001) docker     (127)    51581 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/chips/hdsocv1.yml
--rw-r--r--   0 runner    (1001) docker     (127)    15092 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/chips/hiper.yml
--rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/chips/udc16.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:36:54.725826 naluconfigs-13.8.0/src/naluconfigs/data/clocks/
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/AODS_300GCC.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/AODS_8M.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv3S_GCC400M_1xSysClk_v32andup_PLL80M-AARDVARC-Registers.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:36:54.729826 naluconfigs-13.8.0/src/naluconfigs/data/registers/
--rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/aardvarcv2.yml
--rw-r--r--   0 runner    (1001) docker     (127)    13589 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/aardvarcv3.yml
--rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/aardvarcv4.yml
--rw-r--r--   0 runner    (1001) docker     (127)    15940 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/aodsoc_aods.yml
--rw-r--r--   0 runner    (1001) docker     (127)    15787 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/aodsoc_asoc.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/aodsv1.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11559 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/aodsv2_eval.yml
--rw-r--r--   0 runner    (1001) docker     (127)    17672 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/asoc.yml
--rw-r--r--   0 runner    (1001) docker     (127)    21823 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/asocv2.yml
--rw-r--r--   0 runner    (1001) docker     (127)    14340 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/asocv3.yml
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/asocv3s.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
--rw-r--r--   0 runner    (1001) docker     (127)    19910 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/hiper.yml
--rw-r--r--   0 runner    (1001) docker     (127)    32887 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/hiper_fmc.yml
--rw-r--r--   0 runner    (1001) docker     (127)    25199 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/oleas_box2.yml
--rw-r--r--   0 runner    (1001) docker     (127)    19218 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/siread.yml
--rw-r--r--   0 runner    (1001) docker     (127)    15673 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/trbhm.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11733 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/udc16.yml
--rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/upac32.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/upac96.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16851 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/upaci.yml
--rw-r--r--   0 runner    (1001) docker     (127)    16884 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/data/registers/zdigitizer.yml
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/src/naluconfigs/postprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:36:54.729826 naluconfigs-13.8.0/src/naluconfigs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-05 23:36:54.000000 naluconfigs-13.8.0/src/naluconfigs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-05 23:36:54.000000 naluconfigs-13.8.0/src/naluconfigs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 23:36:54.000000 naluconfigs-13.8.0/src/naluconfigs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-05 23:36:54.000000 naluconfigs-13.8.0/src/naluconfigs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-05 23:36:54.000000 naluconfigs-13.8.0/src/naluconfigs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 23:36:54.729826 naluconfigs-13.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/tests/test_hex_addr_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/tests/test_i2c_registers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/tests/test_multichip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/tests/test_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-05 23:36:42.000000 naluconfigs-13.8.0/tests/test_range_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:04:33.554392 naluconfigs-13.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-21 16:04:33.550392 naluconfigs-13.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 16:04:33.554392 naluconfigs-13.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:04:33.534392 naluconfigs-13.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:04:33.538392 naluconfigs-13.8.1/src/naluconfigs/
+-rw-r--r--   0 runner    (1001) docker     (127)     8408 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:04:33.534392 naluconfigs-13.8.1/src/naluconfigs/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:04:33.542392 naluconfigs-13.8.1/src/naluconfigs/data/chips/
+-rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/chips/aardvarcv3.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    21891 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/chips/aardvarcv4.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    14649 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/chips/aodsv1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    15860 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/chips/aodsv2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/chips/asocv3.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    51581 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/chips/hdsocv1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    15092 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/chips/hiper.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/chips/udc16.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:04:33.546392 naluconfigs-13.8.1/src/naluconfigs/data/clocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/AODS_300GCC.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/AODS_8M.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5430 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5433 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5455 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5440 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5443 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341_ASoCv3S_GCC400M_1xSysClk_v32andup_PLL80M-AARDVARC-Registers.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5413 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:04:33.550392 naluconfigs-13.8.1/src/naluconfigs/data/registers/
+-rw-r--r--   0 runner    (1001) docker     (127)    21676 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/aardvarcv2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13589 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/aardvarcv3.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/aardvarcv4.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    15940 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/aodsoc_aods.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    15787 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/aodsoc_asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/aodsv1.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11559 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/aodsv2_eval.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    17672 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/asoc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    21823 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/asocv2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    14340 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/asocv3.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/asocv3s.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16214 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/hdsocv1_evalr2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    19910 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/hiper.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    32887 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/hiper_fmc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    25199 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/oleas_box2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    19218 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/siread.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    15673 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/trbhm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11733 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/udc16.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/upac32.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11664 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/upac96.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16851 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/upaci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    16884 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/data/registers/zdigitizer.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5940 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/src/naluconfigs/postprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:04:33.550392 naluconfigs-13.8.1/src/naluconfigs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-04-21 16:04:33.000000 naluconfigs-13.8.1/src/naluconfigs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-04-21 16:04:33.000000 naluconfigs-13.8.1/src/naluconfigs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 16:04:33.000000 naluconfigs-13.8.1/src/naluconfigs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-21 16:04:33.000000 naluconfigs-13.8.1/src/naluconfigs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 16:04:33.000000 naluconfigs-13.8.1/src/naluconfigs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 16:04:33.550392 naluconfigs-13.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/tests/test_hex_addr_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/tests/test_i2c_registers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/tests/test_multichip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/tests/test_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-21 16:04:24.000000 naluconfigs-13.8.1/tests/test_range_keys.py
```

### Comparing `naluconfigs-13.8.0/PKG-INFO` & `naluconfigs-13.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 13.8.0
+Version: 13.8.1
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-13.8.0/README.md` & `naluconfigs-13.8.1/README.md`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/pyproject.toml` & `naluconfigs-13.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/setup.py` & `naluconfigs-13.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/__init__.py` & `naluconfigs-13.8.1/src/naluconfigs/__init__.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/_constructors.py` & `naluconfigs-13.8.1/src/naluconfigs/_constructors.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/chips/aardvarcv3.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/chips/aardvarcv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/chips/aardvarcv4.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/chips/aardvarcv4.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/chips/aodsv1.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/chips/aodsv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/chips/aodsv2.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/chips/aodsv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/chips/asocv3.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/chips/asocv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/chips/hdsocv1.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/chips/hdsocv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/chips/hiper.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/chips/hiper.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/chips/udc16.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/chips/udc16.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/AODS_300GCC.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/AODS_300GCC.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/AODS_8M.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/AODS_8M.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2-13GSa_711MGCC-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv2_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv3_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-AARDVARCv4_GCC781_DebugSE-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-ASoC_lambchop-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_15_625SysClk_400GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GCCclk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-HDSoC_31_25SYSclk_15_625SSTclk_400GccClk_156_25TxClk_31_25TxDivClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR-NexysFMC_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-HIPeR_78_125SysClk_312_5GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-Lambchop-Registers_compSysclk.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-TR-BHM_78_125SysClk_781_25GccClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD-UDC_78_125SlowClk_78_125IntermediateClk_312_5FastClk-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_GCC450M_debugse3125-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341-RevD_ASoCv2_simple_GCC300M_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC123M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341_ASoCv2_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv3S_GCC400M_1xSysClk_v32andup_PLL80M-AARDVARC-Registers.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341_ASoCv3S_GCC400M_1xSysClk_v32andup_PLL80M-AARDVARC-Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC420M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341_ASoCv3_GCC450M_1xSysClk_v32andup_6250ksed.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt` & `naluconfigs-13.8.1/src/naluconfigs/data/clocks/Si5341_TRBHM_10GSaps_GCCsstx2_Registers.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/aardvarcv2.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/aardvarcv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/aardvarcv3.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/aardvarcv3.yml`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     stepsize: 5
     units: counts
   ext_dac:
     chip: dac7578
     max_mv: 1200
     max_counts: 4095
     channels:
-      0..3: 2048
+      0..3: 2730
     address_mapping:
       0..3: 0x4E
     channel_mapping:
       0: 2
       1: 6
       2: 3
       3: 7
```

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/aardvarcv4.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/aardvarcv4.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/aodsoc_aods.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/aodsoc_aods.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/aodsoc_asoc.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/aodsoc_asoc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/aodsv1.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/aodsv1.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/aodsv2_eval.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/aodsv2_eval.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/asoc.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/asoc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/asocv2.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/asocv2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/asocv3.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/asocv3.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/asocv3s.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/asocv3s.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/hdsocv1_evalr2.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/hdsocv1_evalr2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/hiper.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/hiper.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/hiper_fmc.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/hiper_fmc.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/oleas_box2.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/oleas_box2.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/siread.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/siread.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/trbhm.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/trbhm.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/udc16.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/udc16.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/upac32.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/upac32.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/upac96.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/upac96.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/upaci.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/upaci.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/data/registers/zdigitizer.yml` & `naluconfigs-13.8.1/src/naluconfigs/data/registers/zdigitizer.yml`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/exceptions.py` & `naluconfigs-13.8.1/src/naluconfigs/exceptions.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/helpers.py` & `naluconfigs-13.8.1/src/naluconfigs/helpers.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs/postprocess.py` & `naluconfigs-13.8.1/src/naluconfigs/postprocess.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/src/naluconfigs.egg-info/PKG-INFO` & `naluconfigs-13.8.1/src/naluconfigs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naluconfigs
-Version: 13.8.0
+Version: 13.8.1
 Summary: Home for board configs
 Home-page: 
 Author: Thomas Yang, Emily Lum
 Author-email: Marcus Luck <marcus@naluscientific.com>, Mitchell Matsumori-Kelly <mitchell@naluscientific.com>, Alvin Yang <alvin@naluscientific.com>, Kenneth Lauritzen <kenneth@naluscientific.com>, Ben Rotter <ben@naluscientific.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

### Comparing `naluconfigs-13.8.0/src/naluconfigs.egg-info/SOURCES.txt` & `naluconfigs-13.8.1/src/naluconfigs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/tests/test_hex_addr_converter.py` & `naluconfigs-13.8.1/tests/test_hex_addr_converter.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/tests/test_i2c_registers.py` & `naluconfigs-13.8.1/tests/test_i2c_registers.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/tests/test_multichip.py` & `naluconfigs-13.8.1/tests/test_multichip.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/tests/test_post_processing.py` & `naluconfigs-13.8.1/tests/test_post_processing.py`

 * *Files identical despite different names*

### Comparing `naluconfigs-13.8.0/tests/test_range_keys.py` & `naluconfigs-13.8.1/tests/test_range_keys.py`

 * *Files identical despite different names*

