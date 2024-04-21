# Comparing `tmp/PyLTSpice-5.2.2.tar.gz` & `tmp/pyltspice-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLTSpice-5.2.2.tar", last modified: Sat Mar 16 09:47:55 2024, max compression
+gzip compressed data, was "pyltspice-5.3.0.tar", last modified: Sun Apr 21 15:06:40 2024, max compression
```

## Comparing `PyLTSpice-5.2.2.tar` & `pyltspice-5.3.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxrwx   0        0        0        0 2024-03-16 09:47:55.885569 PyLTSpice-5.2.2/
--rw-rw-rw-   0        0        0    35823 2023-08-06 15:17:19.000000 PyLTSpice-5.2.2/LICENSE
--rw-rw-rw-   0        0        0    69082 2024-03-16 09:47:55.884296 PyLTSpice-5.2.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-16 09:47:55.824026 PyLTSpice-5.2.2/PyLTSpice/
--rw-rw-rw-   0        0        0      789 2023-10-16 16:04:02.000000 PyLTSpice-5.2.2/PyLTSpice/Histogram.py
--rw-rw-rw-   0        0        0      809 2023-10-16 16:04:02.000000 PyLTSpice-5.2.2/PyLTSpice/LTSteps.py
--rw-rw-rw-   0        0        0     1856 2024-03-16 09:47:29.000000 PyLTSpice-5.2.2/PyLTSpice/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-16 09:47:55.835055 PyLTSpice-5.2.2/PyLTSpice/editor/
--rw-rw-rw-   0        0        0        0 2023-10-16 16:04:02.000000 PyLTSpice-5.2.2/PyLTSpice/editor/__init__.py
--rw-rw-rw-   0        0        0      904 2024-03-16 09:13:46.000000 PyLTSpice-5.2.2/PyLTSpice/editor/asc_editor.py
--rw-rw-rw-   0        0        0     1797 2024-03-16 09:13:46.000000 PyLTSpice-5.2.2/PyLTSpice/editor/spice_editor.py
-drwxrwxrwx   0        0        0        0 2024-03-16 09:47:55.840850 PyLTSpice-5.2.2/PyLTSpice/log/
--rw-rw-rw-   0        0        0        0 2023-08-06 15:17:19.000000 PyLTSpice-5.2.2/PyLTSpice/log/__init__.py
--rw-rw-rw-   0        0        0      638 2024-03-16 09:16:16.000000 PyLTSpice-5.2.2/PyLTSpice/log/logfile_data.py
--rw-rw-rw-   0        0        0      728 2024-03-16 09:13:46.000000 PyLTSpice-5.2.2/PyLTSpice/log/ltsteps.py
--rw-rw-rw-   0        0        0      788 2023-10-16 16:04:02.000000 PyLTSpice-5.2.2/PyLTSpice/log/semi_dev_op_reader.py
-drwxrwxrwx   0        0        0        0 2024-03-16 09:47:55.845372 PyLTSpice-5.2.2/PyLTSpice/raw/
--rw-rw-rw-   0        0        0        0 2023-08-06 15:17:19.000000 PyLTSpice-5.2.2/PyLTSpice/raw/__init__.py
--rw-rw-rw-   0        0        0      813 2023-10-16 16:04:02.000000 PyLTSpice-5.2.2/PyLTSpice/raw/raw_classes.py
--rw-rw-rw-   0        0        0     9473 2024-03-16 09:14:55.000000 PyLTSpice-5.2.2/PyLTSpice/raw/raw_read.py
--rw-rw-rw-   0        0        0      870 2023-10-16 16:04:02.000000 PyLTSpice-5.2.2/PyLTSpice/raw/raw_write.py
--rw-rw-rw-   0        0        0      775 2023-10-16 16:10:21.000000 PyLTSpice-5.2.2/PyLTSpice/rawplot.py
--rw-rw-rw-   0        0        0      775 2023-10-16 16:04:02.000000 PyLTSpice-5.2.2/PyLTSpice/run_server.py
-drwxrwxrwx   0        0        0        0 2024-03-16 09:47:55.851466 PyLTSpice-5.2.2/PyLTSpice/sim/
--rw-rw-rw-   0        0        0        0 2023-08-06 15:17:19.000000 PyLTSpice-5.2.2/PyLTSpice/sim/__init__.py
--rw-rw-rw-   0        0        0     1096 2024-03-16 09:16:49.000000 PyLTSpice-5.2.2/PyLTSpice/sim/ltspice_simulator.py
--rw-rw-rw-   0        0        0      797 2023-10-16 16:04:02.000000 PyLTSpice-5.2.2/PyLTSpice/sim/process_callback.py
--rw-rw-rw-   0        0        0    10830 2024-03-16 09:18:04.000000 PyLTSpice-5.2.2/PyLTSpice/sim/sim_batch.py
--rw-rw-rw-   0        0        0     7807 2024-03-16 09:18:04.000000 PyLTSpice-5.2.2/PyLTSpice/sim/sim_runner.py
--rw-rw-rw-   0        0        0     1618 2024-03-16 09:18:04.000000 PyLTSpice-5.2.2/PyLTSpice/sim/sim_stepping.py
-drwxrwxrwx   0        0        0        0 2024-03-16 09:47:55.855370 PyLTSpice-5.2.2/PyLTSpice/sim/tookit/
--rw-rw-rw-   0        0        0      766 2023-10-16 16:04:02.000000 PyLTSpice-5.2.2/PyLTSpice/sim/tookit/montecarlo.py
--rw-rw-rw-   0        0        0      771 2023-10-16 16:04:02.000000 PyLTSpice-5.2.2/PyLTSpice/sim/tookit/worst_case.py
-drwxrwxrwx   0        0        0        0 2024-03-16 09:47:55.857526 PyLTSpice-5.2.2/PyLTSpice/utils/
--rw-rw-rw-   0        0        0     1067 2023-10-16 16:04:02.000000 PyLTSpice-5.2.2/PyLTSpice/utils/detect_encoding.py
--rw-rw-rw-   0        0        0     4387 2023-10-16 16:04:02.000000 PyLTSpice-5.2.2/PyLTSpice/utils/sweep_iterators.py
-drwxrwxrwx   0        0        0        0 2024-03-16 09:47:55.881823 PyLTSpice-5.2.2/PyLTSpice.egg-info/
--rw-rw-rw-   0        0        0    69082 2024-03-16 09:47:55.000000 PyLTSpice-5.2.2/PyLTSpice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1396 2024-03-16 09:47:55.000000 PyLTSpice-5.2.2/PyLTSpice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-16 09:47:55.000000 PyLTSpice-5.2.2/PyLTSpice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-03-16 09:47:55.000000 PyLTSpice-5.2.2/PyLTSpice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       48 2024-03-16 09:47:55.000000 PyLTSpice-5.2.2/PyLTSpice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    27153 2024-03-16 09:34:23.000000 PyLTSpice-5.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-16 09:47:55.876427 PyLTSpice-5.2.2/examples/
--rw-rw-rw-   0        0        0      799 2023-09-02 12:26:10.000000 PyLTSpice-5.2.2/examples/ltsteps_example.py
--rw-rw-rw-   0        0        0     3152 2023-09-02 12:26:10.000000 PyLTSpice-5.2.2/examples/raw_plotting.py
--rw-rw-rw-   0        0        0     3939 2023-09-02 12:26:10.000000 PyLTSpice-5.2.2/examples/raw_write_example.py
--rw-rw-rw-   0        0        0     2449 2024-02-23 21:07:51.000000 PyLTSpice-5.2.2/examples/run_montecarlo.py
--rw-rw-rw-   0        0        0     1544 2024-02-15 09:12:22.000000 PyLTSpice-5.2.2/examples/run_worst_case.py
--rw-rw-rw-   0        0        0     1354 2023-09-02 12:26:10.000000 PyLTSpice-5.2.2/examples/sim_runner_asc_example.py
--rw-rw-rw-   0        0        0     2535 2023-09-02 12:26:10.000000 PyLTSpice-5.2.2/examples/sim_runner_callback_example.py
--rw-rw-rw-   0        0        0     2740 2023-09-02 12:26:10.000000 PyLTSpice-5.2.2/examples/sim_runner_callback_process_example.py
--rw-rw-rw-   0        0        0     1759 2023-09-02 12:26:10.000000 PyLTSpice-5.2.2/examples/sim_runner_example.py
--rw-rw-rw-   0        0        0     1175 2023-09-02 12:26:10.000000 PyLTSpice-5.2.2/examples/sim_stepper_example.py
--rw-rw-rw-   0        0        0      251 2024-02-15 09:34:35.000000 PyLTSpice-5.2.2/examples/spice_editor_example.py
--rw-rw-rw-   0        0        0     1095 2024-03-16 09:19:19.000000 PyLTSpice-5.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-16 09:47:55.885569 PyLTSpice-5.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-16 09:47:55.880815 PyLTSpice-5.2.2/unittests/
--rw-rw-rw-   0        0        0     6054 2023-09-02 12:26:10.000000 PyLTSpice-5.2.2/unittests/sweep_iterators_unittest.py
--rw-rw-rw-   0        0        0     3164 2024-03-10 16:16:13.000000 PyLTSpice-5.2.2/unittests/test_asc_editor.py
--rw-rw-rw-   0        0        0    19390 2024-03-10 16:30:27.000000 PyLTSpice-5.2.2/unittests/test_pyltspice.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.839309 pyltspice-5.3.0/
+-rw-rw-rw-   0        0        0    35823 2023-08-06 15:17:19.000000 pyltspice-5.3.0/LICENSE
+-rw-rw-rw-   0        0        0    69160 2024-04-21 15:06:40.839309 pyltspice-5.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.786970 pyltspice-5.3.0/PyLTSpice/
+-rw-rw-rw-   0        0        0      789 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/Histogram.py
+-rw-rw-rw-   0        0        0      809 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/LTSteps.py
+-rw-rw-rw-   0        0        0     1856 2024-03-16 09:47:29.000000 pyltspice-5.3.0/PyLTSpice/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.795539 pyltspice-5.3.0/PyLTSpice/editor/
+-rw-rw-rw-   0        0        0        0 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/editor/__init__.py
+-rw-rw-rw-   0        0        0      904 2024-03-16 09:13:46.000000 pyltspice-5.3.0/PyLTSpice/editor/asc_editor.py
+-rw-rw-rw-   0        0        0     1797 2024-03-16 09:13:46.000000 pyltspice-5.3.0/PyLTSpice/editor/spice_editor.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.800124 pyltspice-5.3.0/PyLTSpice/log/
+-rw-rw-rw-   0        0        0        0 2023-08-06 15:17:19.000000 pyltspice-5.3.0/PyLTSpice/log/__init__.py
+-rw-rw-rw-   0        0        0      638 2024-03-16 09:16:16.000000 pyltspice-5.3.0/PyLTSpice/log/logfile_data.py
+-rw-rw-rw-   0        0        0      728 2024-03-16 09:13:46.000000 pyltspice-5.3.0/PyLTSpice/log/ltsteps.py
+-rw-rw-rw-   0        0        0      788 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/log/semi_dev_op_reader.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.804375 pyltspice-5.3.0/PyLTSpice/raw/
+-rw-rw-rw-   0        0        0        0 2023-08-06 15:17:19.000000 pyltspice-5.3.0/PyLTSpice/raw/__init__.py
+-rw-rw-rw-   0        0        0      813 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/raw/raw_classes.py
+-rw-rw-rw-   0        0        0     9473 2024-03-16 09:14:55.000000 pyltspice-5.3.0/PyLTSpice/raw/raw_read.py
+-rw-rw-rw-   0        0        0      870 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/raw/raw_write.py
+-rw-rw-rw-   0        0        0      775 2023-10-16 16:10:21.000000 pyltspice-5.3.0/PyLTSpice/rawplot.py
+-rw-rw-rw-   0        0        0      775 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/run_server.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.811574 pyltspice-5.3.0/PyLTSpice/sim/
+-rw-rw-rw-   0        0        0        0 2023-08-06 15:17:19.000000 pyltspice-5.3.0/PyLTSpice/sim/__init__.py
+-rw-rw-rw-   0        0        0     1096 2024-03-16 09:16:49.000000 pyltspice-5.3.0/PyLTSpice/sim/ltspice_simulator.py
+-rw-rw-rw-   0        0        0      797 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/sim/process_callback.py
+-rw-rw-rw-   0        0        0    10830 2024-03-16 09:18:04.000000 pyltspice-5.3.0/PyLTSpice/sim/sim_batch.py
+-rw-rw-rw-   0        0        0     7807 2024-03-16 09:18:04.000000 pyltspice-5.3.0/PyLTSpice/sim/sim_runner.py
+-rw-rw-rw-   0        0        0     1618 2024-03-16 09:18:04.000000 pyltspice-5.3.0/PyLTSpice/sim/sim_stepping.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.814899 pyltspice-5.3.0/PyLTSpice/sim/tookit/
+-rw-rw-rw-   0        0        0      766 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/sim/tookit/montecarlo.py
+-rw-rw-rw-   0        0        0      771 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/sim/tookit/worst_case.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.818113 pyltspice-5.3.0/PyLTSpice/utils/
+-rw-rw-rw-   0        0        0     1067 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/utils/detect_encoding.py
+-rw-rw-rw-   0        0        0     4387 2023-10-16 16:04:02.000000 pyltspice-5.3.0/PyLTSpice/utils/sweep_iterators.py
+drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.837193 pyltspice-5.3.0/PyLTSpice.egg-info/
+-rw-rw-rw-   0        0        0    69160 2024-04-21 15:06:40.000000 pyltspice-5.3.0/PyLTSpice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1396 2024-04-21 15:06:40.000000 pyltspice-5.3.0/PyLTSpice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 15:06:40.000000 pyltspice-5.3.0/PyLTSpice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-21 15:06:40.000000 pyltspice-5.3.0/PyLTSpice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       48 2024-04-21 15:06:40.000000 pyltspice-5.3.0/PyLTSpice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    27231 2024-04-21 15:05:37.000000 pyltspice-5.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.831531 pyltspice-5.3.0/examples/
+-rw-rw-rw-   0        0        0      799 2023-09-02 12:26:10.000000 pyltspice-5.3.0/examples/ltsteps_example.py
+-rw-rw-rw-   0        0        0     3152 2023-09-02 12:26:10.000000 pyltspice-5.3.0/examples/raw_plotting.py
+-rw-rw-rw-   0        0        0     3939 2023-09-02 12:26:10.000000 pyltspice-5.3.0/examples/raw_write_example.py
+-rw-rw-rw-   0        0        0     2449 2024-02-23 21:07:51.000000 pyltspice-5.3.0/examples/run_montecarlo.py
+-rw-rw-rw-   0        0        0     1544 2024-02-15 09:12:22.000000 pyltspice-5.3.0/examples/run_worst_case.py
+-rw-rw-rw-   0        0        0     1354 2023-09-02 12:26:10.000000 pyltspice-5.3.0/examples/sim_runner_asc_example.py
+-rw-rw-rw-   0        0        0     2535 2023-09-02 12:26:10.000000 pyltspice-5.3.0/examples/sim_runner_callback_example.py
+-rw-rw-rw-   0        0        0     2740 2023-09-02 12:26:10.000000 pyltspice-5.3.0/examples/sim_runner_callback_process_example.py
+-rw-rw-rw-   0        0        0     1759 2023-09-02 12:26:10.000000 pyltspice-5.3.0/examples/sim_runner_example.py
+-rw-rw-rw-   0        0        0     1175 2023-09-02 12:26:10.000000 pyltspice-5.3.0/examples/sim_stepper_example.py
+-rw-rw-rw-   0        0        0      251 2024-02-15 09:34:35.000000 pyltspice-5.3.0/examples/spice_editor_example.py
+-rw-rw-rw-   0        0        0     1095 2024-04-21 15:05:37.000000 pyltspice-5.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-21 15:06:40.840317 pyltspice-5.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-21 15:06:40.835547 pyltspice-5.3.0/unittests/
+-rw-rw-rw-   0        0        0     6054 2023-09-02 12:26:10.000000 pyltspice-5.3.0/unittests/sweep_iterators_unittest.py
+-rw-rw-rw-   0        0        0     3178 2024-04-21 15:05:37.000000 pyltspice-5.3.0/unittests/test_asc_editor.py
+-rw-rw-rw-   0        0        0    19390 2024-03-10 16:30:27.000000 pyltspice-5.3.0/unittests/test_pyltspice.py
```

### Comparing `PyLTSpice-5.2.2/LICENSE` & `pyltspice-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PKG-INFO` & `pyltspice-5.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2050 794c  : 2.1..Name: PyL
 00000020: 5453 7069 6365 0d0a 5665 7273 696f 6e3a  TSpice..Version:
-00000030: 2035 2e32 2e32 0d0a 5375 6d6d 6172 793a   5.2.2..Summary:
+00000030: 2035 2e33 2e30 0d0a 5375 6d6d 6172 793a   5.3.0..Summary:
 00000040: 2041 2073 6574 206f 6620 746f 6f6c 7320   A set of tools 
 00000050: 746f 2041 7574 6f6d 6174 6520 4c54 5370  to Automate LTSp
 00000060: 6963 6520 7369 6d75 6c61 7469 6f6e 730d  ice simulations.
 00000070: 0a41 7574 686f 722d 656d 6169 6c3a 204e  .Author-email: N
 00000080: 756e 6f20 4272 756d 203c 6d65 406e 756e  uno Brum <me@nun
 00000090: 6f62 7275 6d2e 636f 6d3e 0d0a 4c69 6365  obrum.com>..Lice
 000000a0: 6e73 653a 2020 2020 2020 2020 2020 2020  nse:            
@@ -2614,15 +2614,15 @@
 0000a350: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
 0000a360: 3e3d 332e 380d 0a44 6573 6372 6970 7469  >=3.8..Descripti
 0000a370: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
 0000a380: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
 0000a390: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
 0000a3a0: 4345 4e53 450d 0a52 6571 7569 7265 732d  CENSE..Requires-
 0000a3b0: 4469 7374 3a20 7370 6963 656c 6962 3e3d  Dist: spicelib>=
-0000a3c0: 312e 302e 340d 0a0d 0a23 2052 4541 444d  1.0.4....# READM
+0000a3c0: 312e 312e 310d 0a0d 0a23 2052 4541 444d  1.1.1....# READM
 0000a3d0: 4520 230d 0a0d 0a50 794c 5453 7069 6365  E #....PyLTSpice
 0000a3e0: 2069 7320 6120 746f 6f6c 6368 6169 6e20   is a toolchain 
 0000a3f0: 6f66 2070 7974 686f 6e20 7574 696c 6974  of python utilit
 0000a400: 6965 7320 6465 7369 676e 2074 6f20 696e  ies design to in
 0000a410: 7465 7261 6374 2077 6974 6820 4c54 5370  teract with LTSp
 0000a420: 6963 6520 456c 6563 7472 6f6e 6963 2053  ice Electronic S
 0000a430: 696d 756c 6174 6f72 2e0d 0a49 7420 6973  imulator...It is
@@ -3821,498 +3821,503 @@
 0000eec0: 6d2e 636f 6d29 0d0a 2a20 416c 7465 726e  m.com)..* Altern
 0000eed0: 6174 6976 6520 636f 6e74 6163 7420 3a20  ative contact : 
 0000eee0: 5b6e 756e 6f2e 6272 756d 4067 6d61 696c  [nuno.brum@gmail
 0000eef0: 2e63 6f6d 5d28 6d61 696c 746f 3a6e 756e  .com](mailto:nun
 0000ef00: 6f2e 6272 756d 4067 6d61 696c 2e63 6f6d  o.brum@gmail.com
 0000ef10: 290d 0a0d 0a23 2320 4869 7374 6f72 7920  )....## History 
 0000ef20: 2323 0d0a 2a20 5665 7273 696f 6e20 352e  ##..* Version 5.
-0000ef30: 322e 330d 0a20 202a 2055 7064 6174 696e  2.3..  * Updatin
-0000ef40: 6720 6c6f 6767 6572 7320 746f 2075 7365  g loggers to use
-0000ef50: 2074 6865 2022 7370 6963 656c 6962 2220   the "spicelib" 
-0000ef60: 4944 732e 0d0a 2020 2a20 4669 7869 6e67  IDs...  * Fixing
-0000ef70: 2061 7574 6f64 6f63 2065 7272 6f72 730d   autodoc errors.
-0000ef80: 0a20 202a 2043 6f72 7265 6374 696e 6720  .  * Correcting 
-0000ef90: 5665 7273 696f 6e20 7265 6665 7265 6e63  Version referenc
-0000efa0: 6573 0d0a 0d0a 2a20 5665 7273 696f 6e20  es....* Version 
-0000efb0: 352e 322e 320d 0a20 202a 2046 6978 6573  5.2.2..  * Fixes
-0000efc0: 206f 6e20 7468 6520 756e 6974 7465 7374   on the unittest
-0000efd0: 7320 6166 7465 7220 7468 6520 7370 6963  s after the spic
-0000efe0: 656c 6962 2075 7064 6174 6520 746f 2031  elib update to 1
-0000eff0: 2e30 2e34 0d0a 0d0a 2a20 5665 7273 696f  .0.4....* Versio
-0000f000: 6e20 352e 322e 310d 0a20 202a 2043 6f72  n 5.2.1..  * Cor
-0000f010: 7265 6374 696f 6e20 6f6e 2074 6865 2072  rection on the r
-0000f020: 756e 5f6d 6f6e 7465 6361 726c 6f2e 7079  un_montecarlo.py
-0000f030: 2061 6e64 2072 756e 5f77 6f72 7374 5f63   and run_worst_c
-0000f040: 6173 652e 7079 2065 7861 6d70 6c65 732e  ase.py examples.
-0000f050: 0d0a 2020 2a20 4669 7865 7320 6f6e 2074  ..  * Fixes on t
-0000f060: 6865 2073 7069 6365 6c69 6220 2856 6572  he spicelib (Ver
-0000f070: 7369 6f6e 2031 2e30 2e33 290d 0a0d 0a2a  sion 1.0.3)....*
-0000f080: 2056 6572 7369 6f6e 2035 2e32 0d0a 2020   Version 5.2..  
-0000f090: 2a20 5369 6d41 6e61 6c79 7369 7320 7375  * SimAnalysis su
-0000f0a0: 7070 6f72 7469 6e67 2062 6f74 6820 5173  pporting both Qs
-0000f0b0: 7069 6365 2061 6e64 204c 5453 7069 6365  pice and LTSpice
-0000f0c0: 206c 6f67 6669 6c65 732e 0d0a 2020 2a20   logfiles...  * 
-0000f0d0: 4661 7374 576f 7273 7443 6173 6541 6e61  FastWorstCaseAna
-0000f0e0: 6c79 7369 7320 616c 676f 7269 7468 6d20  lysis algorithm 
-0000f0f0: 696d 706c 656d 656e 7465 640d 0a20 202a  implemented..  *
-0000f100: 2046 6978 206f 6e20 7468 6520 6c6f 6720   Fix on the log 
-0000f110: 7265 6164 696e 6720 6f66 2066 6f75 7269  reading of fouri
-0000f120: 6572 2064 6174 612e 0d0a 0d0a 2a20 5665  er data.....* Ve
-0000f130: 7273 696f 6e20 352e 310d 0a20 202a 2049  rsion 5.1..  * I
-0000f140: 6d70 6f72 7461 6e74 2042 7567 6669 7820  mportant Bugfix 
-0000f150: 6f6e 2074 6865 204c 5443 6f6d 706c 6578  on the LTComplex
-0000f160: 2063 6c61 7373 2e0d 0a20 202a 2046 6978   class...  * Fix
-0000f170: 6573 2061 6e64 2065 6e68 616e 6369 6e67  es and enhancing
-0000f180: 2074 6865 2061 6e61 6c79 7369 7320 746f   the analysis to
-0000f190: 6f6c 6b69 742e 0d0a 2020 2a20 4465 7072  olkit...  * Depr
-0000f1a0: 6563 6174 696e 6720 5370 6963 6545 6469  ecating SpiceEdi
-0000f1b0: 746f 722e 7772 6974 655f 6e65 746c 6973  tor.write_netlis
-0000f1c0: 7420 696e 2066 6176 6f75 7220 6f66 2073  t in favour of s
-0000f1d0: 6176 655f 6e65 746c 6973 7428 290d 0a0d  ave_netlist()...
-0000f1e0: 0a2a 2056 6572 7369 6f6e 2035 2e30 0d0a  .* Version 5.0..
-0000f1f0: 2020 2a20 4d61 6b69 6e67 2074 6869 7320    * Making this 
-0000f200: 6c69 6272 6172 7920 6465 7065 6e64 656e  library dependen
-0000f210: 7420 6f6e 2073 7069 6365 6c69 6220 7768  t on spicelib wh
-0000f220: 696c 6520 7472 7969 6e67 2074 6f20 6d61  ile trying to ma
-0000f230: 696e 7461 696e 2062 6163 6b77 6172 6420  intain backward 
-0000f240: 636f 6d70 6174 6962 696c 6974 7920 6173  compatibility as
-0000f250: 206d 7563 6820 6173 2070 6f73 7369 626c   much as possibl
-0000f260: 652e 200d 0a20 2050 794c 5473 7069 6365  e. ..  PyLTspice
-0000f270: 2077 696c 6c20 6265 206b 6570 7420 616c   will be kept al
-0000f280: 6976 6520 616e 6420 6974 7320 7570 6461  ive and its upda
-0000f290: 7465 2077 696c 6c20 6265 206c 696e 6b65  te will be linke
-0000f2a0: 6420 746f 2074 6865 2073 7069 6365 6c69  d to the spiceli
-0000f2b0: 622e 2054 6865 206d 6169 6e20 6469 6666  b. The main diff
-0000f2c0: 6572 656e 6365 2069 7320 7468 6174 2075  erence is that u
-0000f2d0: 7369 6e67 0d0a 2020 5079 4c54 7370 6963  sing..  PyLTspic
-0000f2e0: 6520 7769 6c6c 2061 7665 7274 2074 6865  e will avert the
-0000f2f0: 206e 6565 6420 6f66 2068 6176 696e 6720   need of having 
-0000f300: 746f 2073 656c 6563 7420 6120 7369 6d75  to select a simu
-0000f310: 6c61 746f 7220 696e 2061 6c6c 2072 756e  lator in all run
-0000f320: 2063 6f6d 6d61 6e64 732e 0d0a 0d0a 2a20   commands.....* 
-0000f330: 5665 7273 696f 6e20 342e 312e 320d 0a20  Version 4.1.2.. 
-0000f340: 202a 2041 6464 696e 6720 7375 7070 6f72   * Adding suppor
-0000f350: 7420 666f 7220 7468 6520 6e65 7720 5153  t for the new QS
-0000f360: 5049 4345 2073 696d 756c 6174 6f72 0d0a  PICE simulator..
-0000f370: 2020 2a20 496d 7072 6f76 696e 6720 7468    * Improving th
-0000f380: 6520 7469 6d65 6f75 7420 6d65 6368 616e  e timeout mechan
-0000f390: 6973 6d20 6f6e 2074 6865 2053 696d 5275  ism on the SimRu
-0000f3a0: 6e6e 6572 2063 6c61 7373 0d0a 2020 2a20  nner class..  * 
-0000f3b0: 4d69 6e6f 7220 6275 6720 6669 7865 730d  Minor bug fixes.
-0000f3c0: 0a0d 0a2a 2056 6572 7369 6f6e 2034 2e31  ...* Version 4.1
-0000f3d0: 2e31 0d0a 2020 2a20 436f 6d70 6c65 7469  .1..  * Completi
-0000f3e0: 6e67 2074 6865 2057 6f72 7374 2d43 6173  ng the Worst-Cas
-0000f3f0: 6520 416e 616c 7973 6973 2066 756e 6374  e Analysis funct
-0000f400: 696f 6e73 2e20 4164 6469 6e67 2061 2064  ions. Adding a d
-0000f410: 6564 6963 6174 6564 2065 7861 6d70 6c65  edicated example
-0000f420: 2066 6f72 2069 742e 0d0a 2020 2a20 5265   for it...  * Re
-0000f430: 6661 6374 6f72 696e 6720 7468 6520 4c54  factoring the LT
-0000f440: 5370 6963 654c 6f67 5265 6164 6572 2063  SpiceLogReader c
-0000f450: 6c61 7373 2069 6e20 6f72 6465 7220 746f  lass in order to
-0000f460: 2075 7365 2069 7420 6f6e 2074 6865 2041   use it on the A
-0000f470: 6e61 6c79 7369 7320 746f 6f6c 6b69 740d  nalysis toolkit.
-0000f480: 0a0d 0a2a 2056 6572 7369 6f6e 2034 2e31  ...* Version 4.1
-0000f490: 2e30 202a 2872 6571 7569 7265 7320 5079  .0 *(requires Py
-0000f4a0: 7468 6f6e 2033 2e38 206f 7220 6869 6768  thon 3.8 or high
-0000f4b0: 6572 292a 0d0a 2020 2020 2a20 4164 6469  er)*..    * Addi
-0000f4c0: 6e67 2061 206e 6577 2063 6c61 7373 2074  ng a new class t
-0000f4d0: 6f20 6d61 6e69 7075 6c61 7465 2064 6972  o manipulate dir
-0000f4e0: 6563 746c 7920 7468 6520 2e61 7363 2066  ectly the .asc f
-0000f4f0: 696c 6573 2e0d 0a20 2020 202a 204d 6f64  iles...    * Mod
-0000f500: 6966 7969 6e67 2061 6c6c 2074 6865 206f  ifying all the o
-0000f510: 7468 6572 2063 6c61 7373 6573 2069 6e20  ther classes in 
-0000f520: 6f72 6465 7220 746f 2075 7365 2074 6865  order to use the
-0000f530: 206e 6577 2063 6c61 7373 2e0d 0a20 2020   new class...   
-0000f540: 202a 2041 6464 696e 6720 636c 6173 7365   * Adding classe
-0000f550: 7320 746f 2070 6572 666f 726d 204d 6f6e  s to perform Mon
-0000f560: 7465 6361 726c 6f20 616e 6420 776f 7273  tecarlo and wors
-0000f570: 7420 6361 7365 2061 6e61 6c79 7369 7320  t case analysis 
-0000f580: 2854 6861 6e6b 7320 746f 2040 6d76 616e  (Thanks to @mvan
-0000f590: 7269 6574 2066 6f72 2068 6973 2073 7461  riet for his sta
-0000f5a0: 7274 696e 6720 7468 6973 292e 0d0a 2020  rting this)...  
-0000f5b0: 2020 2a20 5265 6d6f 7669 6e67 2074 6865    * Removing the
-0000f5c0: 2064 6570 7265 6361 7465 6420 4c54 5370   deprecated LTSp
-0000f5d0: 6963 655f 5261 7752 6561 642e 7079 2c20  ice_RawRead.py, 
-0000f5e0: 4c54 5370 6963 655f 5261 7757 7269 7465  LTSpice_RawWrite
-0000f5f0: 2e70 7920 616e 6420 4c54 5370 6963 6542  .py and LTSpiceB
-0000f600: 6174 6368 2e70 7920 6669 6c65 7320 616e  atch.py files an
-0000f610: 6420 7265 7370 6563 7469 7665 2063 6c61  d respective cla
-0000f620: 7373 6573 2e0d 0a20 2020 202a 2052 6573  sses...    * Res
-0000f630: 7472 7563 7475 7265 6420 7468 6520 666f  tructured the fo
-0000f640: 6c64 6572 2073 7472 7563 7475 7265 2074  lder structure t
-0000f650: 6f20 6265 206d 6f72 6520 696e 206c 696e  o be more in lin
-0000f660: 6520 7769 7468 2074 6865 2050 7974 686f  e with the Pytho
-0000f670: 6e20 7374 616e 6461 7264 732e 0d0a 2020  n standards...  
-0000f680: 2020 2a20 4164 6465 6420 616e 2045 7861    * Added an Exa
-0000f690: 6d70 6c65 7320 666f 6c64 6572 2077 6974  mples folder wit
-0000f6a0: 6820 736f 6d65 2065 7861 6d70 6c65 7320  h some examples 
-0000f6b0: 6f6e 2068 6f77 2074 6f20 7573 6520 7468  on how to use th
-0000f6c0: 6520 6c69 6272 6172 792e 0d0a 0d0a 2a20  e library.....* 
-0000f6d0: 5665 7273 696f 6e20 342e 302e 360d 0a20  Version 4.0.6.. 
-0000f6e0: 2020 202a 2046 6978 696e 6720 6973 7375     * Fixing issu
-0000f6f0: 6520 7769 7468 2074 6865 2077 7269 7465  e with the write
-0000f700: 5f6e 6574 6c69 7374 2829 2066 756e 6374  _netlist() funct
-0000f710: 696f 6e20 7768 656e 2072 6563 6569 7669  ion when receivi
-0000f720: 6e67 2061 2073 7472 696e 6720 696e 7374  ng a string inst
-0000f730: 6561 6420 6f66 2061 2070 6174 686c 6962  ead of a pathlib
-0000f740: 2e50 6174 6820 6f62 6a65 6374 2e0d 0a20  .Path object... 
-0000f750: 2020 202a 2043 6861 6e67 696e 6720 7468     * Changing th
-0000f760: 6520 7265 6775 6c61 7220 6578 7072 6573  e regular expres
-0000f770: 7369 6f6e 2066 6f72 2074 6865 2072 6573  sion for the res
-0000f780: 6973 746f 7220 696e 206f 7264 6572 2074  istor in order t
-0000f790: 6f20 6163 6365 7074 2074 6865 2052 3d20  o accept the R= 
-0000f7a0: 7072 6566 6978 206f 6e20 7468 6520 7661  prefix on the va
-0000f7b0: 6c75 6573 2e0d 0a0d 0a2a 2056 6572 7369  lues.....* Versi
-0000f7c0: 6f6e 2034 2e30 2e35 0d0a 2020 2020 2a20  on 4.0.5..    * 
-0000f7d0: 4163 6365 7074 696e 6720 6669 7865 7320  Accepting fixes 
-0000f7e0: 6672 6f6d 2061 616e 6173 2d73 6179 6564  from aanas-sayed
-0000f7f0: 4047 6974 4875 6220 7468 6174 2066 6978  @GitHub that fix
-0000f800: 6573 2069 7373 7565 7320 7769 7468 2072  es issues with r
-0000f810: 756e 6e69 6e67 2074 6865 204c 5453 7069  unning the LTSpi
-0000f820: 6365 2069 6e20 4c69 6e75 782e 0d0a 0d0a  ce in Linux.....
-0000f830: 2a20 5665 7273 696f 6e20 342e 302e 340d  * Version 4.0.4.
-0000f840: 0a20 2020 202a 2049 6d70 726f 7665 6420  .    * Improved 
-0000f850: 7573 6167 6520 6f66 2074 6865 206c 6f67  usage of the log
-0000f860: 6769 6e67 206c 6962 7261 7279 2e20 2854  ging library. (T
-0000f870: 6861 6e6b 7320 4054 5370 7265 6368 2066  hanks @TSprech f
-0000f880: 6f72 2076 6173 746c 7920 696d 7072 6f76  or vastly improv
-0000f890: 696e 6720 7468 6520 6c6f 6767 696e 6729  ing the logging)
-0000f8a0: 0d0a 2020 2020 2a20 496e 636c 7564 6564  ..    * Included
-0000f8b0: 2052 756e 5461 736b 206e 756d 6265 7220   RunTask number 
-0000f8c0: 696e 2074 6865 206c 6f67 206d 6573 7361  in the log messa
-0000f8d0: 6765 732e 0d0a 2020 2020 2a20 496e 636c  ges...    * Incl
-0000f8e0: 7564 6564 206d 696c 6c69 7365 636f 6e64  uded millisecond
-0000f8f0: 7320 696e 2074 6865 2074 696d 6520 656c  s in the time el
-0000f900: 6170 7365 6420 6361 6c63 756c 6174 696f  apsed calculatio
-0000f910: 6e2e 0d0a 0d0a 2a20 5665 7273 696f 6e20  n.....* Version 
-0000f920: 342e 302e 330d 0a20 2020 202a 2046 6978  4.0.3..    * Fix
-0000f930: 696e 6720 6973 7375 6520 696e 2065 6c61  ing issue in ela
-0000f940: 7073 6564 2074 696d 6520 6361 6c63 756c  psed time calcul
-0000f950: 6174 696f 6e2e 0d0a 2020 2020 2a20 4669  ation...    * Fi
-0000f960: 7869 6e67 2069 7373 7565 2077 6974 6820  xing issue with 
-0000f970: 7468 6520 696d 706f 7274 206f 6620 4c54  the import of LT
-0000f980: 5370 6963 654c 6f67 5265 6164 6572 2066  SpiceLogReader f
-0000f990: 726f 6d20 4c54 5374 6570 732e 7079 0d0a  rom LTSteps.py..
-0000f9a0: 0d0a 2a20 5665 7273 696f 6e20 342e 302e  ..* Version 4.0.
-0000f9b0: 320d 0a20 2020 202a 2043 6861 6e67 696e  2..    * Changin
-0000f9c0: 6720 6c69 7374 206f 6620 4c69 6272 6172  g list of Librar
-0000f9d0: 7920 6465 7065 6e64 656e 6369 6573 2e0d  y dependencies..
-0000f9e0: 0a0d 0a2a 2056 6572 7369 6f6e 2034 2e30  ...* Version 4.0
-0000f9f0: 2e31 0d0a 2020 2020 2a20 4275 6720 6669  .1..    * Bug fi
-0000fa00: 7820 6f6e 2043 4c49 2066 6f72 2074 6865  x on CLI for the
-0000fa10: 2048 6973 746f 6772 616d 2e70 7920 616e   Histogram.py an
-0000fa20: 6420 4c54 5374 6570 732e 7079 0d0a 0d0a  d LTSteps.py....
-0000fa30: 2a20 5665 7273 696f 6e20 342e 302e 300d  * Version 4.0.0.
-0000fa40: 0a20 2020 202a 2053 6570 6172 6174 696e  .    * Separatin
-0000fa50: 6720 7468 6520 5369 6d43 6f6d 6d61 6e64  g the SimCommand
-0000fa60: 6572 2069 6e74 6f20 7477 6f20 7365 7061  er into two sepa
-0000fa70: 7261 7465 2063 6c61 7373 6573 2c20 6f6e  rate classes, on
-0000fa80: 6520 666f 7220 7468 6520 7370 6963 6520  e for the spice 
-0000fa90: 6e65 746c 6973 7420 6564 6974 696e 6720  netlist editing 
-0000faa0: 2853 7069 6365 4564 6974 6f72 2920 616e  (SpiceEditor) an
-0000fab0: 6420 616e 6f74 6865 720d 0a20 2020 2020  d another..     
-0000fac0: 2066 6f72 2074 6865 2073 696d 756c 6174   for the simulat
-0000fad0: 696f 6e20 6578 6563 7574 696f 6e20 2853  ion execution (S
-0000fae0: 696d 5275 6e6e 6572 292e 0d0a 2020 2020  imRunner)...    
-0000faf0: 2a20 496d 706c 656d 656e 7469 6e67 2073  * Implementing s
-0000fb00: 696d 756c 6174 696f 6e20 7365 7276 6572  imulation server
-0000fb10: 2074 6f20 616c 6c6f 7720 666f 7220 7265   to allow for re
-0000fb20: 6d6f 7465 2073 696d 756c 6174 696f 6e20  mote simulation 
-0000fb30: 6578 6563 7574 696f 6e20 616e 6420 7468  execution and th
-0000fb40: 6520 7265 7370 6563 7469 7665 2063 6c69  e respective cli
-0000fb50: 656e 742e 0d0a 2020 2020 2a20 5375 7070  ent...    * Supp
-0000fb60: 6f72 7469 6e67 2057 6967 676c 6572 2065  orting Wiggler e
-0000fb70: 6c65 6d65 6e74 2069 6e20 7468 6520 6e65  lement in the ne
-0000fb80: 7720 4c54 5370 6963 6558 5649 492e 0d0a  w LTSpiceXVII...
-0000fb90: 2020 2020 2a20 5265 6e61 6d69 6e67 2061      * Renaming a
-0000fba0: 6c6c 2066 696c 6573 2069 6e74 6f20 6c6f  ll files into lo
-0000fbb0: 7765 7263 6173 652e 0d0a 2020 2020 2a20  wercase...    * 
-0000fbc0: 4372 6561 7469 6e67 2045 7272 6f72 2063  Creating Error c
-0000fbd0: 6c61 7373 6573 2066 6f72 2062 6574 7465  lasses for bette
-0000fbe0: 7220 6572 726f 7220 6861 6e64 6c69 6e67  r error handling
-0000fbf0: 2e0d 0a20 2020 202a 2041 6464 696e 6720  ...    * Adding 
-0000fc00: 7375 7070 6f72 7420 666f 7220 6f74 6865  support for othe
-0000fc10: 7220 7369 6d75 6c61 746f 7273 2028 6578  r simulators (ex
-0000fc20: 3a20 6e67 7370 6963 6529 2077 6865 7265  : ngspice) where
-0000fc30: 2074 6865 2073 696d 756c 6174 6f72 2069   the simulator i
-0000fc40: 7320 6465 6669 6e65 6420 6279 2061 2063  s defined by a c
-0000fc50: 6c61 7373 2e20 5468 6973 0d0a 2020 2020  lass. This..    
-0000fc60: 2020 7375 7070 6f72 7420 636c 6173 7320    support class 
-0000fc70: 6e65 6564 7320 746f 2062 6520 6120 7375  needs to be a su
-0000fc80: 6263 6c61 7373 206f 6620 7468 6520 6162  bclass of the ab
-0000fc90: 7374 7261 6374 2063 6c61 7373 2053 696d  stract class Sim
-0000fca0: 756c 6174 6f72 2e0d 0a20 2020 202a 2045  ulator...    * E
-0000fcb0: 6e6f 726d 6f75 7320 696d 7072 6f76 656d  normous improvem
-0000fcc0: 656e 7420 696e 2074 6865 2064 6f63 756d  ent in the docum
-0000fcd0: 656e 7461 7469 6f6e 206f 6620 7468 6520  entation of the 
-0000fce0: 636f 6465 2e0d 0a0d 0a2a 2056 6572 7369  code.....* Versi
-0000fcf0: 6f6e 2033 2e30 0d0a 2020 2020 2a20 456c  on 3.0..    * El
-0000fd00: 696d 696e 6174 696e 6720 7468 6520 4c54  iminating the LT
-0000fd10: 5370 6963 6520 7072 6566 6978 6573 2066  Spice prefixes f
-0000fd20: 726f 6d20 6669 6c65 7320 616e 6420 636c  rom files and cl
-0000fd30: 6173 7365 732e 0d0a 2020 2020 2a20 4164  asses...    * Ad
-0000fd40: 6f70 7469 6e67 2074 6865 206c 6f77 6572  opting the lower
-0000fd50: 6361 7365 2063 6f6e 7665 6e74 696f 6e20  case convention 
-0000fd60: 666f 7220 6669 6c65 6e61 6d65 732e 0d0a  for filenames...
-0000fd70: 0d0a 2a20 5665 7273 696f 6e20 322e 332e  ..* Version 2.3.
-0000fd80: 310d 0a20 2020 202a 2042 7567 2066 6978  1..    * Bug fix
-0000fd90: 206f 6e20 7468 6520 7061 7261 6d65 7465   on the paramete
-0000fda0: 7220 7265 706c 6163 656d 656e 742e 0d0a  r replacement...
-0000fdb0: 0d0a 2a20 5665 7273 696f 6e20 322e 330d  ..* Version 2.3.
-0000fdc0: 0a20 2020 202a 2053 7570 706f 7274 696e  .    * Supportin
-0000fdd0: 6720 7468 6520 6372 6561 7469 6f6e 206f  g the creation o
-0000fde0: 6620 5241 5720 4e6f 6973 6520 416e 616c  f RAW Noise Anal
-0000fdf0: 7973 6973 0d0a 2020 2020 2a20 4275 6720  ysis..    * Bug 
-0000fe00: 4669 7865 7320 2853 6565 2047 6974 4875  Fixes (See GitHu
-0000fe10: 6220 4c6f 6729 0d0a 0d0a 2a20 5665 7273  b Log)....* Vers
-0000fe20: 696f 6e20 322e 320d 0a20 2020 202a 204d  ion 2.2..    * M
-0000fe30: 616b 696e 6720 6e75 6d70 7920 6173 2061  aking numpy as a
-0000fe40: 2072 6571 7569 7265 6d65 6e74 2061 6e64   requirement and
-0000fe50: 2065 6c69 6d69 6e61 7469 6e67 2061 6c6c   eliminating all
-0000fe60: 2063 6f64 6520 7468 6174 2061 766f 6964   code that avoid
-0000fe70: 6564 2074 6865 2075 7365 206f 6620 6e75  ed the use of nu
-0000fe80: 6d70 790d 0a20 2020 202a 2055 7369 6e67  mpy..    * Using
-0000fe90: 206e 6577 2070 6163 6b61 6769 6e67 2074   new packaging t
-0000fea0: 6f6f 6c0d 0a20 2020 202a 2046 6978 6573  ool..    * Fixes
-0000feb0: 206f 6e20 7468 6520 4c54 5370 6963 655f   on the LTSpice_
-0000fec0: 5261 7757 7269 7465 0d0a 2020 2020 2a20  RawWrite..    * 
-0000fed0: 4669 7865 7320 696e 2074 6865 2068 616e  Fixes in the han
-0000fee0: 646c 696e 6720 6f66 2073 7465 7070 6564  dling of stepped
-0000fef0: 206f 7065 7261 7469 6e67 2070 6f69 6e74   operating point
-0000ff00: 2073 696d 756c 6174 696f 6e73 0d0a 0d0a   simulations....
-0000ff10: 2a20 5665 7273 696f 6e20 322e 310d 0a20  * Version 2.1.. 
-0000ff20: 2020 202a 2041 646f 7074 696e 6720 6d69     * Adopting mi
-0000ff30: 6e69 6d75 6d20 7079 7468 6f6e 2076 6572  nimum python ver
-0000ff40: 7369 6f6e 2033 2e37 0d0a 2020 2020 2a20  sion 3.7..    * 
-0000ff50: 5374 6172 7469 6e67 2074 6f20 7573 6520  Starting to use 
-0000ff60: 756e 6974 2074 6573 7473 2074 6f20 7661  unit tests to va
-0000ff70: 6c69 6461 7465 2061 6c6c 206d 6f64 756c  lidate all modul
-0000ff80: 6573 2061 6e64 2069 6d70 726f 7669 6e67  es and improving
-0000ff90: 2074 6573 7462 656e 6368 6573 0d0a 2020   testbenches..  
-0000ffa0: 2020 2a20 436f 6d70 6174 6962 696c 6974    * Compatibilit
-0000ffb0: 7920 7769 7468 204e 4753 7069 6365 0d0a  y with NGSpice..
-0000ffc0: 2020 2020 2a20 4176 6f69 6469 6e67 2074      * Avoiding t
-0000ffd0: 6865 2075 7365 206f 6620 7365 7475 702e  he use of setup.
-0000ffe0: 7079 2061 7320 7065 7220 5045 5035 3137  py as per PEP517
-0000fff0: 2061 6e64 2050 4550 3531 380d 0a20 2020   and PEP518..   
-00010000: 202a 2042 7567 2046 6978 6573 2028 5365   * Bug Fixes (Se
-00010010: 6520 4769 7448 7562 206c 6f67 2066 6f72  e GitHub log for
-00010020: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-00010030: 6e29 0d0a 2020 2020 2a20 496d 7072 6f76  n)..    * Improv
-00010040: 656d 656e 7473 206f 6e20 7468 6520 6d61  ements on the ma
-00010050: 6e61 6765 6d65 6e74 206f 6620 7374 6570  nagement of step
-00010060: 7065 6420 6461 7461 2069 6e20 7468 6520  ped data in the 
-00010070: 4c54 5370 6963 655f 5261 7752 6561 642e  LTSpice_RawRead.
-00010080: 7079 0d0a 0d0a 2a20 5665 7273 696f 6e20  py....* Version 
-00010090: 322e 302e 320d 0a20 2020 202a 2049 6d70  2.0.2..    * Imp
-000100a0: 726f 7665 6d65 6e74 7320 6f6e 2045 6e63  rovements on Enc
-000100b0: 6f64 696e 6720 6465 7465 6374 696f 6e0d  oding detection.
-000100c0: 0a0d 0a2a 2056 6572 7369 6f6e 2032 2e30  ...* Version 2.0
-000100d0: 0d0a 2020 2020 2a20 496e 7465 726e 6174  ..    * Internat
-000100e0: 696f 6e61 6c20 5375 7070 6f72 7420 7573  ional Support us
-000100f0: 696e 6720 7468 6520 636f 7272 6563 7420  ing the correct 
-00010100: 656e 636f 6469 6e67 2077 6865 6e20 6c6f  encoding when lo
-00010110: 6164 696e 6720 6c6f 6720 6669 6c65 732e  ading log files.
-00010120: 0d0a 2020 2020 2a20 436f 6465 204f 7074  ..    * Code Opt
-00010130: 696d 697a 6174 696f 6e73 206f 6e20 7468  imizations on th
-00010140: 6520 4c54 5370 6963 655f 5261 7752 6561  e LTSpice_RawRea
-00010150: 6465 7220 7468 6174 2061 6c6c 6f77 2066  der that allow f
-00010160: 6173 7465 7220 6461 7461 206c 6f61 6469  aster data loadi
-00010170: 6e67 2e0d 0a20 2020 202a 2049 6d70 726f  ng...    * Impro
-00010180: 7669 6e67 2074 6865 2066 756e 6374 696f  ving the functio
-00010190: 6e61 6c69 7479 206f 6e20 7468 6520 4c54  nality on the LT
-000101a0: 5370 6963 655f 5261 7757 7269 7465 722e  Spice_RawWriter.
-000101b0: 7079 0d0a 2020 2020 2a20 4164 6469 6e67  py..    * Adding
-000101c0: 2073 7570 706f 7274 2074 6f20 6564 6974   support to edit
-000101d0: 696e 6720 636f 6d70 6f6e 656e 7473 2069  ing components i
-000101e0: 6e73 6964 6520 7375 6263 6972 6375 6974  nside subcircuit
-000101f0: 7320 282e 7375 6263 6b74 290d 0a20 2020  s (.subckt)..   
-00010200: 202a 2053 7570 706f 7274 696e 6720 7265   * Supporting re
-00010210: 7369 7374 6f72 7320 7769 7468 204d 6f64  sistors with Mod
-00010220: 656c 2044 6566 696e 6974 696f 6e73 0d0a  el Definitions..
-00010230: 2020 2020 2a20 4669 7869 6e67 2070 726f      * Fixing pro
-00010240: 626c 656d 2077 6974 6820 4c54 5370 6963  blem with LTSpic
-00010250: 654c 6f67 5265 6164 6572 2074 6861 7420  eLogReader that 
-00010260: 776f 756c 6420 7265 7475 726e 206d 6573  would return mes
-00010270: 7365 6420 7570 2064 6174 610d 0a20 2020  sed up data..   
-00010280: 202a 2046 6978 696e 6720 7072 6f62 6c65   * Fixing proble
-00010290: 6d20 7769 7468 2072 6570 6c61 6369 6e67  m with replacing
-000102a0: 2074 6865 2066 696c 6520 6578 7465 6e73   the file extens
-000102b0: 696f 6e20 696e 2063 6572 7461 696e 206e  ion in certain n
-000102c0: 616d 6573 0d0a 2020 2020 2a20 436f 7272  ames..    * Corr
-000102d0: 6563 7469 6e67 2070 726f 626c 656d 2077  ecting problem w
-000102e0: 6974 6820 6465 7072 6563 6174 696f 6e73  ith deprecations
-000102f0: 206f 6e20 7468 6520 6e75 6d70 7920 6675   on the numpy fu
-00010300: 6e63 7469 6f6e 7320 7573 6564 2062 7920  nctions used by 
-00010310: 7468 6520 4869 7374 6f67 7261 6d2e 7079  the Histogram.py
-00010320: 0d0a 2020 2020 2a20 4164 6469 6e67 2062  ..    * Adding b
-00010330: 6163 6b20 7468 6520 5245 4144 4d45 2e6d  ack the README.m
-00010340: 6420 7468 6174 2073 6f6d 6568 6f77 2077  d that somehow w
-00010350: 6173 2064 656c 6574 6564 0d0a 0d0a 2a20  as deleted....* 
-00010360: 5665 7273 696f 6e20 312e 390d 0a20 2020  Version 1.9..   
-00010370: 202a 2041 6464 696e 6720 7375 7070 6f72   * Adding suppor
-00010380: 7420 666f 7220 c2b5 2063 6861 7261 6374  t for .. charact
-00010390: 6572 2069 6e20 7468 6520 5370 6963 6545  er in the SpiceE
-000103a0: 6469 746f 722e 0d0a 2020 2020 2a20 4164  ditor...    * Ad
-000103b0: 6469 6e67 2067 6574 5f63 6f6d 706f 6e65  ding get_compone
-000103c0: 6e74 5f66 6c6f 6174 7661 6c75 6528 2920  nt_floatvalue() 
-000103d0: 6d65 7468 6f64 2069 6e20 7468 6520 6e65  method in the ne
-000103e0: 746c 6973 7420 6d61 6e69 7075 6c61 7469  tlist manipulati
-000103f0: 6e67 2063 6c61 7373 2074 6861 7420 6861  ng class that ha
-00010400: 6e64 6c65 7320 7468 6520 636f 6e76 6572  ndles the conver
-00010410: 7369 6f6e 206f 6620 6e75 6d65 7269 630d  sion of numeric.
-00010420: 0a20 2020 2020 2066 6965 6c64 7320 696e  .      fields in
-00010430: 746f 2061 2066 6c6f 6174 2e20 5468 6973  to a float. This
-00010440: 2066 756e 6374 696f 6e20 7461 6b65 7320   function takes 
-00010450: 696e 746f 2061 6363 6f75 6e74 2074 6865  into account the
-00010460: 2065 6e67 696e 6565 7269 6e67 2071 7561   engineering qua
-00010470: 6c69 6669 6572 7320 276b 2720 666f 7220  lifiers 'k' for 
-00010480: 6b69 6c6f 732c 2027 6d27 206f 7220 6d69  kilos, 'm' or mi
-00010490: 6c69 732c 0d0a 2020 2020 2020 2775 2720  lis,..      'u' 
-000104a0: 6f72 2027 c2b5 2720 666f 7220 6d69 6372  or '..' for micr
-000104b0: 6f6e 732c 2027 6e27 2066 6f72 206e 616e  ons, 'n' for nan
-000104c0: 6f73 2c20 2766 2720 666f 7220 6665 6d74  os, 'f' for femt
-000104d0: 6f73 2061 6e64 2027 4d65 6727 2066 6f72  os and 'Meg' for
-000104e0: 204d 6567 6173 2e0d 0a0d 0a2a 2056 6572   Megas.....* Ver
-000104f0: 7369 6f6e 2031 2e38 0d0a 2020 2020 2a20  sion 1.8..    * 
-00010500: 556e 6966 6f72 6d69 6e67 204c 6963 656e  Uniforming Licen
-00010510: 7365 2072 6566 6572 656e 6365 2061 6372  se reference acr
-00010520: 6f73 7320 6669 6c65 7320 616e 6420 696d  oss files and im
-00010530: 7072 6f76 656d 656e 7473 206f 6e20 7468  provements on th
-00010540: 6520 646f 6375 6d65 6e74 6174 696f 6e0d  e documentation.
-00010550: 0a20 2020 202a 2041 6e20 656e 6f72 6d6f  .    * An enormo
-00010560: 7573 2061 6e64 2077 686f 6c65 6865 6172  us and wholehear
-00010570: 7465 6420 7468 616e 6b73 2074 6f20 406c  ted thanks to @l
-00010580: 7068 6572 7220 666f 7220 7468 6520 696d  pherr for the im
-00010590: 7072 6f76 656d 656e 7473 2069 6e20 7468  provements in th
-000105a0: 6520 646f 6375 6d65 6e74 6174 696f 6e2e  e documentation.
-000105b0: 0d0a 2020 2020 2a20 4275 6766 6978 206f  ..    * Bugfix o
-000105c0: 6e20 7468 6520 6164 645f 4c54 7370 6963  n the add_LTspic
-000105d0: 6552 756e 436d 644c 696e 6553 7769 7463  eRunCmdLineSwitc
-000105e0: 6865 7328 2920 3b20 5375 7070 6f72 7469  hes() ; Supporti
-000105f0: 6e67 202e 7061 7261 6d20 6e61 6d65 2076  ng .param name v
-00010600: 616c 7565 2066 6f72 6d61 740d 0a20 2020  alue format..   
-00010610: 202a 2041 6c6c 6f77 696e 6720 7468 6520   * Allowing the 
-00010620: 4c54 5370 6963 6552 6177 5265 6164 2074  LTSpiceRawRead t
-00010630: 6f20 7072 6f63 6565 6420 7768 656e 2074  o proceed when t
-00010640: 6865 206c 6f67 2066 696c 6520 6361 6e27  he log file can'
-00010650: 7420 6265 2066 6f75 6e64 206f 7220 7768  t be found or wh
-00010660: 656e 2074 6865 7265 2061 7265 2070 726f  en there are pro
-00010670: 626c 656d 7320 7265 6164 696e 6720 6974  blems reading it
-00010680: 2e0d 0a2a 2056 6572 7369 6f6e 2031 2e37  ...* Version 1.7
-00010690: 0d0a 2020 2020 2a20 5275 6e6e 696e 6720  ..    * Running 
-000106a0: 696e 204c 696e 7578 2075 6e64 6572 2077  in Linux under w
-000106b0: 696e 6520 6973 206e 6f77 2070 6f73 7369  ine is now possi
-000106c0: 626c 650d 0a0d 0a2a 2056 6572 7369 6f6e  ble....* Version
-000106d0: 2031 2e36 0d0a 2020 2020 2a20 4164 6469   1.6..    * Addi
-000106e0: 6e67 204c 5453 7069 6365 5f52 6177 5772  ng LTSpice_RawWr
-000106f0: 6974 652e 2041 6464 696e 6720 646f 6375  ite. Adding docu
-00010700: 6d65 6e74 6174 696f 6e2e 0d0a 0d0a 2a20  mentation.....* 
-00010710: 5665 7273 696f 6e20 312e 350d 0a20 2020  Version 1.5..   
-00010720: 202a 2053 6d61 6c6c 2066 6978 6573 2061   * Small fixes a
-00010730: 6e64 2069 6d70 726f 7665 6d65 6e74 7320  nd improvements 
-00010740: 6f6e 2074 6865 2063 6c61 7373 2075 7361  on the class usa
-00010750: 6765 2e20 4e6f 2061 6464 6564 2066 6561  ge. No added fea
-00010760: 7475 7265 730d 0a0d 0a2a 2056 6572 7369  tures....* Versi
-00010770: 6f6e 2031 2e34 0d0a 2020 2020 2a20 4164  on 1.4..    * Ad
-00010780: 6469 6e67 2074 6865 204c 5453 7069 6365  ding the LTSpice
-00010790: 5f53 656d 6944 6576 4f70 5265 6164 6572  _SemiDevOpReader
-000107a0: 206d 6f64 756c 650d 0a20 2020 202a 2052   module..    * R
-000107b0: 652d 656e 6162 6c69 6e67 2074 6865 2048  e-enabling the H
-000107c0: 6973 746f 6772 616d 2066 756e 6374 696f  istogram functio
-000107d0: 6e73 2077 6869 6368 2077 6865 7265 2064  ns which where d
-000107e0: 6973 6162 6c65 6420 6279 206d 6973 7461  isabled by mista
-000107f0: 6b65 2e0d 0a0d 0a2a 2056 6572 7369 6f6e  ke.....* Version
-00010800: 2031 2e33 0d0a 2020 2020 2a20 4275 6720   1.3..    * Bug 
-00010810: 6669 7865 7320 6f6e 2074 6865 2053 7069  fixes on the Spi
-00010820: 6365 4564 6974 6f72 2043 6c61 7373 0d0a  ceEditor Class..
-00010830: 0d0a 2a20 5665 7273 696f 6e20 312e 320d  ..* Version 1.2.
-00010840: 0a20 2020 202a 2052 4541 444d 452e 6d64  .    * README.md
-00010850: 3a0d 0a20 2020 2020 2041 6464 696e 6720  :..      Adding 
-00010860: 6c69 6e6b 2074 6f20 7265 6164 7468 6564  link to readthed
-00010870: 6f63 7320 646f 6375 6d65 6e74 6174 696f  ocs documentatio
-00010880: 6e0d 0a20 2020 202a 2041 6c6c 2066 696c  n..    * All fil
-00010890: 6573 3a0d 0a20 2020 2020 2043 6f6d 7072  es:..      Compr
-000108a0: 6568 656e 7369 7665 2064 6f63 756d 656e  ehensive documen
-000108b0: 7461 7469 6f6e 206f 6e20 686f 7720 746f  tation on how to
-000108c0: 2075 7365 2065 6163 6820 6d6f 6475 6c65   use each module
-000108d0: 0d0a 0d0a 2a20 5665 7273 696f 6e20 312e  ....* Version 1.
-000108e0: 310d 0a20 2020 202a 2052 4541 444d 452e  1..    * README.
-000108f0: 6d64 3a0d 0a20 2020 2020 2055 7064 6174  md:..      Updat
-00010900: 6564 2074 6865 2064 6573 6372 6970 7469  ed the descripti
-00010910: 6f6e 0d0a 2020 2020 2a20 4c54 5370 6963  on..    * LTSpic
-00010920: 6542 6174 6368 2e70 793a 0d0a 2020 2020  eBatch.py:..    
-00010930: 2020 436f 7272 6563 7465 6420 7468 6520    Corrected the 
-00010940: 6e61 6d65 206f 6620 7468 6520 7265 7475  name of the retu
-00010950: 726e 6564 2072 6177 2066 696c 652e 0d0a  rned raw file...
-00010960: 2020 2020 2a20 4164 6465 6420 636f 6d6d      * Added comm
-00010970: 656e 7473 2074 6872 6f75 6768 6f75 7420  ents throughout 
-00010980: 7468 6520 636f 6465 2061 6e64 2063 6c65  the code and cle
-00010990: 616e 7570 0d0a 0d0a 2a20 5665 7273 696f  anup....* Versio
-000109a0: 6e20 312e 300d 0a20 2020 202a 204c 5453  n 1.0..    * LTS
-000109b0: 7069 6365 4261 7463 682e 7079 3a5c 0d0a  piceBatch.py:\..
-000109c0: 2020 2020 2020 496d 706c 656d 656e 7465        Implemente
-000109d0: 6420 6120 6e65 7720 6170 7072 6f61 6368  d a new approach
-000109e0: 2028 4e4f 5420 4241 434b 5741 5244 5320   (NOT BACKWARDS 
-000109f0: 434f 4d50 4154 4942 4c45 292c 2074 6861  COMPATIBLE), tha
-00010a00: 7420 6176 6f69 6473 2074 6865 2075 7361  t avoids the usa
-00010a10: 6765 206f 6620 7468 6520 7369 6d5f 7365  ge of the sim_se
-00010a20: 7474 696e 6773 2e69 6e63 2066 696c 652e  ttings.inc file.
-00010a30: 0d0a 2020 2020 2020 416e 6420 616c 6c6f  ..      And allo
-00010a40: 7773 2074 6f20 6d6f 6469 6679 206e 6f74  ws to modify not
-00010a50: 206f 6e6c 7920 7061 7261 6d65 7465 7273   only parameters
-00010a60: 2c20 6275 7420 616c 736f 206d 6f64 656c  , but also model
-00010a70: 7320 616e 6420 6576 656e 2074 6865 2073  s and even the s
-00010a80: 696d 756c 6174 696f 6e20 636f 6d6d 616e  imulation comman
-00010a90: 6473 2e0d 0a20 2020 202a 204c 5453 7069  ds...    * LTSpi
-00010aa0: 6365 5f52 6177 5265 6164 2e70 793a 5c0d  ce_RawRead.py:\.
-00010ab0: 0a20 2020 2020 2041 6464 6564 2074 6865  .      Added the
-00010ac0: 2067 6574 5f74 696d 655f 6178 6973 206d   get_time_axis m
-00010ad0: 6574 686f 6420 746f 2074 6865 2052 6177  ethod to the Raw
-00010ae0: 5265 6164 2063 6c61 7373 2074 6f20 6176  Read class to av
-00010af0: 6f69 6420 7468 6520 7072 6f62 6c65 6d73  oid the problems
-00010b00: 2077 6974 6820 6e65 6761 7469 7665 2076   with negative v
-00010b10: 616c 7565 7320 6f6e 2074 696d 6520 6178  alues on time ax
-00010b20: 6973 2c0d 0a20 2020 2020 2077 6865 6e20  is,..      when 
-00010b30: 326e 6420 6f72 6465 7220 636f 6d70 7265  2nd order compre
-00010b40: 7373 696f 6e20 6973 2065 6e61 626c 6564  ssion is enabled
-00010b50: 2069 6e20 4c54 5370 6963 652e 0d0a 2020   in LTSpice...  
-00010b60: 2020 2a20 4c54 5374 6570 732e 7079 3a5c    * LTSteps.py:\
-00010b70: 0d0a 2020 2020 2020 4d6f 6469 6669 6564  ..      Modified
-00010b80: 2074 6865 204c 5453 7465 7073 2c20 736f   the LTSteps, so
-00010b90: 2069 7420 6361 6e20 616c 736f 2072 6561   it can also rea
-00010ba0: 6420 6d65 6173 7572 656d 656e 7473 206f  d measurements o
-00010bb0: 6e20 6c6f 6720 6669 6c65 7320 7769 7468  n log files with
-00010bc0: 6f75 7420 616e 7920 7374 6570 7320 646f  out any steps do
-00010bd0: 6e65 2e0d 0a0d 0a2a 2056 6572 7369 6f6e  ne.....* Version
-00010be0: 2030 2e36 0d0a 2020 2a20 4869 7374 6f67   0.6..  * Histog
-00010bf0: 7261 6d2e 7079 206e 6f77 2068 6173 2061  ram.py now has a
-00010c00: 6e20 6f70 7469 6f6e 2074 6f20 6d61 6b65  n option to make
-00010c10: 2074 6865 2068 6973 746f 6772 616d 2064   the histogram d
-00010c20: 6972 6563 746c 7920 6672 6f6d 2076 616c  irectly from val
-00010c30: 7565 7320 7374 6f72 6564 2069 6e20 7468  ues stored in th
-00010c40: 6520 636c 6970 626f 6172 640d 0a0d 0a2a  e clipboard....*
-00010c50: 2056 6572 7369 6f6e 2030 2e35 0d0a 2020   Version 0.5..  
-00010c60: 2a20 5468 6520 4c54 5370 6963 655f 5261  * The LTSpice_Ra
-00010c70: 7752 6561 6465 722e 7079 206e 6f77 2075  wReader.py now u
-00010c80: 7365 7320 7468 6520 6073 7472 7563 742e  ses the `struct.
-00010c90: 756e 7061 636b 6020 6675 6e63 7469 6f6e  unpack` function
-00010ca0: 2066 6f72 2061 2066 6173 7465 7220 6578   for a faster ex
-00010cb0: 6563 7574 696f 6e0d 0a0d 0a2a 2056 6572  ecution....* Ver
-00010cc0: 7369 6f6e 2030 2e34 0d0a 2020 2a20 4164  sion 0.4..  * Ad
-00010cd0: 6465 6420 4c54 5370 6963 6542 6174 6368  ded LTSpiceBatch
-00010ce0: 2e70 7920 746f 2074 6865 2063 6f6c 6c65  .py to the colle
-00010cf0: 6374 696f 6e20 6f66 2074 6f6f 6c73 0d0a  ction of tools..
-00010d00: 0d0a 2a20 5665 7273 696f 6e20 302e 330d  ..* Version 0.3.
-00010d10: 0a20 202a 2041 2076 6572 7369 6f6e 206f  .  * A version o
-00010d20: 6620 4c54 5374 6570 7320 7468 6174 2063  f LTSteps that c
-00010d30: 616e 2062 6520 696d 706f 7274 6564 2074  an be imported t
-00010d40: 6f20 7573 6520 696e 2061 2068 6967 6865  o use in a highe
-00010d50: 7220 6c65 7665 6c20 7363 7269 7074 0d0a  r level script..
-00010d60: 0d0a 2a20 5665 7273 696f 6e20 302e 320d  ..* Version 0.2.
-00010d70: 0a20 202a 2041 6464 696e 6720 4c54 5374  .  * Adding LTSt
-00010d80: 6570 732e 7079 2061 6e64 2048 6973 746f  eps.py and Histo
-00010d90: 6772 616d 2e70 790d 0a0d 0a2a 2056 6572  gram.py....* Ver
-00010da0: 7369 6f6e 2030 2e31 200d 0a20 202a 2046  sion 0.1 ..  * F
-00010db0: 6972 7374 2063 6f6d 6d69 7420 746f 2074  irst commit to t
-00010dc0: 6865 2062 6974 6275 636b 6574 2072 6570  he bitbucket rep
-00010dd0: 6f73 6974 6f72 792e 0d0a                 ository...
+0000ef30: 332e 300d 0a20 202a 2048 6965 7261 7263  3.0..  * Hierarc
+0000ef40: 6869 6361 6c20 5375 7070 6f72 7420 2841  hical Support (A
+0000ef50: 6c69 676e 696e 6720 7769 7468 2074 6865  ligning with the
+0000ef60: 2073 7069 6365 6c69 6220 312e 312e 3129   spicelib 1.1.1)
+0000ef70: 0d0a 2a20 5665 7273 696f 6e20 352e 322e  ..* Version 5.2.
+0000ef80: 330d 0a20 202a 2055 7064 6174 696e 6720  3..  * Updating 
+0000ef90: 6c6f 6767 6572 7320 746f 2075 7365 2074  loggers to use t
+0000efa0: 6865 2022 7370 6963 656c 6962 2220 4944  he "spicelib" ID
+0000efb0: 732e 0d0a 2020 2a20 4669 7869 6e67 2061  s...  * Fixing a
+0000efc0: 7574 6f64 6f63 2065 7272 6f72 730d 0a20  utodoc errors.. 
+0000efd0: 202a 2043 6f72 7265 6374 696e 6720 5665   * Correcting Ve
+0000efe0: 7273 696f 6e20 7265 6665 7265 6e63 6573  rsion references
+0000eff0: 0d0a 0d0a 2a20 5665 7273 696f 6e20 352e  ....* Version 5.
+0000f000: 322e 320d 0a20 202a 2046 6978 6573 206f  2.2..  * Fixes o
+0000f010: 6e20 7468 6520 756e 6974 7465 7374 7320  n the unittests 
+0000f020: 6166 7465 7220 7468 6520 7370 6963 656c  after the spicel
+0000f030: 6962 2075 7064 6174 6520 746f 2031 2e30  ib update to 1.0
+0000f040: 2e34 0d0a 0d0a 2a20 5665 7273 696f 6e20  .4....* Version 
+0000f050: 352e 322e 310d 0a20 202a 2043 6f72 7265  5.2.1..  * Corre
+0000f060: 6374 696f 6e20 6f6e 2074 6865 2072 756e  ction on the run
+0000f070: 5f6d 6f6e 7465 6361 726c 6f2e 7079 2061  _montecarlo.py a
+0000f080: 6e64 2072 756e 5f77 6f72 7374 5f63 6173  nd run_worst_cas
+0000f090: 652e 7079 2065 7861 6d70 6c65 732e 0d0a  e.py examples...
+0000f0a0: 2020 2a20 4669 7865 7320 6f6e 2074 6865    * Fixes on the
+0000f0b0: 2073 7069 6365 6c69 6220 2856 6572 7369   spicelib (Versi
+0000f0c0: 6f6e 2031 2e30 2e33 290d 0a0d 0a2a 2056  on 1.0.3)....* V
+0000f0d0: 6572 7369 6f6e 2035 2e32 0d0a 2020 2a20  ersion 5.2..  * 
+0000f0e0: 5369 6d41 6e61 6c79 7369 7320 7375 7070  SimAnalysis supp
+0000f0f0: 6f72 7469 6e67 2062 6f74 6820 5173 7069  orting both Qspi
+0000f100: 6365 2061 6e64 204c 5453 7069 6365 206c  ce and LTSpice l
+0000f110: 6f67 6669 6c65 732e 0d0a 2020 2a20 4661  ogfiles...  * Fa
+0000f120: 7374 576f 7273 7443 6173 6541 6e61 6c79  stWorstCaseAnaly
+0000f130: 7369 7320 616c 676f 7269 7468 6d20 696d  sis algorithm im
+0000f140: 706c 656d 656e 7465 640d 0a20 202a 2046  plemented..  * F
+0000f150: 6978 206f 6e20 7468 6520 6c6f 6720 7265  ix on the log re
+0000f160: 6164 696e 6720 6f66 2066 6f75 7269 6572  ading of fourier
+0000f170: 2064 6174 612e 0d0a 0d0a 2a20 5665 7273   data.....* Vers
+0000f180: 696f 6e20 352e 310d 0a20 202a 2049 6d70  ion 5.1..  * Imp
+0000f190: 6f72 7461 6e74 2042 7567 6669 7820 6f6e  ortant Bugfix on
+0000f1a0: 2074 6865 204c 5443 6f6d 706c 6578 2063   the LTComplex c
+0000f1b0: 6c61 7373 2e0d 0a20 202a 2046 6978 6573  lass...  * Fixes
+0000f1c0: 2061 6e64 2065 6e68 616e 6369 6e67 2074   and enhancing t
+0000f1d0: 6865 2061 6e61 6c79 7369 7320 746f 6f6c  he analysis tool
+0000f1e0: 6b69 742e 0d0a 2020 2a20 4465 7072 6563  kit...  * Deprec
+0000f1f0: 6174 696e 6720 5370 6963 6545 6469 746f  ating SpiceEdito
+0000f200: 722e 7772 6974 655f 6e65 746c 6973 7420  r.write_netlist 
+0000f210: 696e 2066 6176 6f75 7220 6f66 2073 6176  in favour of sav
+0000f220: 655f 6e65 746c 6973 7428 290d 0a0d 0a2a  e_netlist()....*
+0000f230: 2056 6572 7369 6f6e 2035 2e30 0d0a 2020   Version 5.0..  
+0000f240: 2a20 4d61 6b69 6e67 2074 6869 7320 6c69  * Making this li
+0000f250: 6272 6172 7920 6465 7065 6e64 656e 7420  brary dependent 
+0000f260: 6f6e 2073 7069 6365 6c69 6220 7768 696c  on spicelib whil
+0000f270: 6520 7472 7969 6e67 2074 6f20 6d61 696e  e trying to main
+0000f280: 7461 696e 2062 6163 6b77 6172 6420 636f  tain backward co
+0000f290: 6d70 6174 6962 696c 6974 7920 6173 206d  mpatibility as m
+0000f2a0: 7563 6820 6173 2070 6f73 7369 626c 652e  uch as possible.
+0000f2b0: 200d 0a20 2050 794c 5473 7069 6365 2077   ..  PyLTspice w
+0000f2c0: 696c 6c20 6265 206b 6570 7420 616c 6976  ill be kept aliv
+0000f2d0: 6520 616e 6420 6974 7320 7570 6461 7465  e and its update
+0000f2e0: 2077 696c 6c20 6265 206c 696e 6b65 6420   will be linked 
+0000f2f0: 746f 2074 6865 2073 7069 6365 6c69 622e  to the spicelib.
+0000f300: 2054 6865 206d 6169 6e20 6469 6666 6572   The main differ
+0000f310: 656e 6365 2069 7320 7468 6174 2075 7369  ence is that usi
+0000f320: 6e67 0d0a 2020 5079 4c54 7370 6963 6520  ng..  PyLTspice 
+0000f330: 7769 6c6c 2061 7665 7274 2074 6865 206e  will avert the n
+0000f340: 6565 6420 6f66 2068 6176 696e 6720 746f  eed of having to
+0000f350: 2073 656c 6563 7420 6120 7369 6d75 6c61   select a simula
+0000f360: 746f 7220 696e 2061 6c6c 2072 756e 2063  tor in all run c
+0000f370: 6f6d 6d61 6e64 732e 0d0a 0d0a 2a20 5665  ommands.....* Ve
+0000f380: 7273 696f 6e20 342e 312e 320d 0a20 202a  rsion 4.1.2..  *
+0000f390: 2041 6464 696e 6720 7375 7070 6f72 7420   Adding support 
+0000f3a0: 666f 7220 7468 6520 6e65 7720 5153 5049  for the new QSPI
+0000f3b0: 4345 2073 696d 756c 6174 6f72 0d0a 2020  CE simulator..  
+0000f3c0: 2a20 496d 7072 6f76 696e 6720 7468 6520  * Improving the 
+0000f3d0: 7469 6d65 6f75 7420 6d65 6368 616e 6973  timeout mechanis
+0000f3e0: 6d20 6f6e 2074 6865 2053 696d 5275 6e6e  m on the SimRunn
+0000f3f0: 6572 2063 6c61 7373 0d0a 2020 2a20 4d69  er class..  * Mi
+0000f400: 6e6f 7220 6275 6720 6669 7865 730d 0a0d  nor bug fixes...
+0000f410: 0a2a 2056 6572 7369 6f6e 2034 2e31 2e31  .* Version 4.1.1
+0000f420: 0d0a 2020 2a20 436f 6d70 6c65 7469 6e67  ..  * Completing
+0000f430: 2074 6865 2057 6f72 7374 2d43 6173 6520   the Worst-Case 
+0000f440: 416e 616c 7973 6973 2066 756e 6374 696f  Analysis functio
+0000f450: 6e73 2e20 4164 6469 6e67 2061 2064 6564  ns. Adding a ded
+0000f460: 6963 6174 6564 2065 7861 6d70 6c65 2066  icated example f
+0000f470: 6f72 2069 742e 0d0a 2020 2a20 5265 6661  or it...  * Refa
+0000f480: 6374 6f72 696e 6720 7468 6520 4c54 5370  ctoring the LTSp
+0000f490: 6963 654c 6f67 5265 6164 6572 2063 6c61  iceLogReader cla
+0000f4a0: 7373 2069 6e20 6f72 6465 7220 746f 2075  ss in order to u
+0000f4b0: 7365 2069 7420 6f6e 2074 6865 2041 6e61  se it on the Ana
+0000f4c0: 6c79 7369 7320 746f 6f6c 6b69 740d 0a0d  lysis toolkit...
+0000f4d0: 0a2a 2056 6572 7369 6f6e 2034 2e31 2e30  .* Version 4.1.0
+0000f4e0: 202a 2872 6571 7569 7265 7320 5079 7468   *(requires Pyth
+0000f4f0: 6f6e 2033 2e38 206f 7220 6869 6768 6572  on 3.8 or higher
+0000f500: 292a 0d0a 2020 2020 2a20 4164 6469 6e67  )*..    * Adding
+0000f510: 2061 206e 6577 2063 6c61 7373 2074 6f20   a new class to 
+0000f520: 6d61 6e69 7075 6c61 7465 2064 6972 6563  manipulate direc
+0000f530: 746c 7920 7468 6520 2e61 7363 2066 696c  tly the .asc fil
+0000f540: 6573 2e0d 0a20 2020 202a 204d 6f64 6966  es...    * Modif
+0000f550: 7969 6e67 2061 6c6c 2074 6865 206f 7468  ying all the oth
+0000f560: 6572 2063 6c61 7373 6573 2069 6e20 6f72  er classes in or
+0000f570: 6465 7220 746f 2075 7365 2074 6865 206e  der to use the n
+0000f580: 6577 2063 6c61 7373 2e0d 0a20 2020 202a  ew class...    *
+0000f590: 2041 6464 696e 6720 636c 6173 7365 7320   Adding classes 
+0000f5a0: 746f 2070 6572 666f 726d 204d 6f6e 7465  to perform Monte
+0000f5b0: 6361 726c 6f20 616e 6420 776f 7273 7420  carlo and worst 
+0000f5c0: 6361 7365 2061 6e61 6c79 7369 7320 2854  case analysis (T
+0000f5d0: 6861 6e6b 7320 746f 2040 6d76 616e 7269  hanks to @mvanri
+0000f5e0: 6574 2066 6f72 2068 6973 2073 7461 7274  et for his start
+0000f5f0: 696e 6720 7468 6973 292e 0d0a 2020 2020  ing this)...    
+0000f600: 2a20 5265 6d6f 7669 6e67 2074 6865 2064  * Removing the d
+0000f610: 6570 7265 6361 7465 6420 4c54 5370 6963  eprecated LTSpic
+0000f620: 655f 5261 7752 6561 642e 7079 2c20 4c54  e_RawRead.py, LT
+0000f630: 5370 6963 655f 5261 7757 7269 7465 2e70  Spice_RawWrite.p
+0000f640: 7920 616e 6420 4c54 5370 6963 6542 6174  y and LTSpiceBat
+0000f650: 6368 2e70 7920 6669 6c65 7320 616e 6420  ch.py files and 
+0000f660: 7265 7370 6563 7469 7665 2063 6c61 7373  respective class
+0000f670: 6573 2e0d 0a20 2020 202a 2052 6573 7472  es...    * Restr
+0000f680: 7563 7475 7265 6420 7468 6520 666f 6c64  uctured the fold
+0000f690: 6572 2073 7472 7563 7475 7265 2074 6f20  er structure to 
+0000f6a0: 6265 206d 6f72 6520 696e 206c 696e 6520  be more in line 
+0000f6b0: 7769 7468 2074 6865 2050 7974 686f 6e20  with the Python 
+0000f6c0: 7374 616e 6461 7264 732e 0d0a 2020 2020  standards...    
+0000f6d0: 2a20 4164 6465 6420 616e 2045 7861 6d70  * Added an Examp
+0000f6e0: 6c65 7320 666f 6c64 6572 2077 6974 6820  les folder with 
+0000f6f0: 736f 6d65 2065 7861 6d70 6c65 7320 6f6e  some examples on
+0000f700: 2068 6f77 2074 6f20 7573 6520 7468 6520   how to use the 
+0000f710: 6c69 6272 6172 792e 0d0a 0d0a 2a20 5665  library.....* Ve
+0000f720: 7273 696f 6e20 342e 302e 360d 0a20 2020  rsion 4.0.6..   
+0000f730: 202a 2046 6978 696e 6720 6973 7375 6520   * Fixing issue 
+0000f740: 7769 7468 2074 6865 2077 7269 7465 5f6e  with the write_n
+0000f750: 6574 6c69 7374 2829 2066 756e 6374 696f  etlist() functio
+0000f760: 6e20 7768 656e 2072 6563 6569 7669 6e67  n when receiving
+0000f770: 2061 2073 7472 696e 6720 696e 7374 6561   a string instea
+0000f780: 6420 6f66 2061 2070 6174 686c 6962 2e50  d of a pathlib.P
+0000f790: 6174 6820 6f62 6a65 6374 2e0d 0a20 2020  ath object...   
+0000f7a0: 202a 2043 6861 6e67 696e 6720 7468 6520   * Changing the 
+0000f7b0: 7265 6775 6c61 7220 6578 7072 6573 7369  regular expressi
+0000f7c0: 6f6e 2066 6f72 2074 6865 2072 6573 6973  on for the resis
+0000f7d0: 746f 7220 696e 206f 7264 6572 2074 6f20  tor in order to 
+0000f7e0: 6163 6365 7074 2074 6865 2052 3d20 7072  accept the R= pr
+0000f7f0: 6566 6978 206f 6e20 7468 6520 7661 6c75  efix on the valu
+0000f800: 6573 2e0d 0a0d 0a2a 2056 6572 7369 6f6e  es.....* Version
+0000f810: 2034 2e30 2e35 0d0a 2020 2020 2a20 4163   4.0.5..    * Ac
+0000f820: 6365 7074 696e 6720 6669 7865 7320 6672  cepting fixes fr
+0000f830: 6f6d 2061 616e 6173 2d73 6179 6564 4047  om aanas-sayed@G
+0000f840: 6974 4875 6220 7468 6174 2066 6978 6573  itHub that fixes
+0000f850: 2069 7373 7565 7320 7769 7468 2072 756e   issues with run
+0000f860: 6e69 6e67 2074 6865 204c 5453 7069 6365  ning the LTSpice
+0000f870: 2069 6e20 4c69 6e75 782e 0d0a 0d0a 2a20   in Linux.....* 
+0000f880: 5665 7273 696f 6e20 342e 302e 340d 0a20  Version 4.0.4.. 
+0000f890: 2020 202a 2049 6d70 726f 7665 6420 7573     * Improved us
+0000f8a0: 6167 6520 6f66 2074 6865 206c 6f67 6769  age of the loggi
+0000f8b0: 6e67 206c 6962 7261 7279 2e20 2854 6861  ng library. (Tha
+0000f8c0: 6e6b 7320 4054 5370 7265 6368 2066 6f72  nks @TSprech for
+0000f8d0: 2076 6173 746c 7920 696d 7072 6f76 696e   vastly improvin
+0000f8e0: 6720 7468 6520 6c6f 6767 696e 6729 0d0a  g the logging)..
+0000f8f0: 2020 2020 2a20 496e 636c 7564 6564 2052      * Included R
+0000f900: 756e 5461 736b 206e 756d 6265 7220 696e  unTask number in
+0000f910: 2074 6865 206c 6f67 206d 6573 7361 6765   the log message
+0000f920: 732e 0d0a 2020 2020 2a20 496e 636c 7564  s...    * Includ
+0000f930: 6564 206d 696c 6c69 7365 636f 6e64 7320  ed milliseconds 
+0000f940: 696e 2074 6865 2074 696d 6520 656c 6170  in the time elap
+0000f950: 7365 6420 6361 6c63 756c 6174 696f 6e2e  sed calculation.
+0000f960: 0d0a 0d0a 2a20 5665 7273 696f 6e20 342e  ....* Version 4.
+0000f970: 302e 330d 0a20 2020 202a 2046 6978 696e  0.3..    * Fixin
+0000f980: 6720 6973 7375 6520 696e 2065 6c61 7073  g issue in elaps
+0000f990: 6564 2074 696d 6520 6361 6c63 756c 6174  ed time calculat
+0000f9a0: 696f 6e2e 0d0a 2020 2020 2a20 4669 7869  ion...    * Fixi
+0000f9b0: 6e67 2069 7373 7565 2077 6974 6820 7468  ng issue with th
+0000f9c0: 6520 696d 706f 7274 206f 6620 4c54 5370  e import of LTSp
+0000f9d0: 6963 654c 6f67 5265 6164 6572 2066 726f  iceLogReader fro
+0000f9e0: 6d20 4c54 5374 6570 732e 7079 0d0a 0d0a  m LTSteps.py....
+0000f9f0: 2a20 5665 7273 696f 6e20 342e 302e 320d  * Version 4.0.2.
+0000fa00: 0a20 2020 202a 2043 6861 6e67 696e 6720  .    * Changing 
+0000fa10: 6c69 7374 206f 6620 4c69 6272 6172 7920  list of Library 
+0000fa20: 6465 7065 6e64 656e 6369 6573 2e0d 0a0d  dependencies....
+0000fa30: 0a2a 2056 6572 7369 6f6e 2034 2e30 2e31  .* Version 4.0.1
+0000fa40: 0d0a 2020 2020 2a20 4275 6720 6669 7820  ..    * Bug fix 
+0000fa50: 6f6e 2043 4c49 2066 6f72 2074 6865 2048  on CLI for the H
+0000fa60: 6973 746f 6772 616d 2e70 7920 616e 6420  istogram.py and 
+0000fa70: 4c54 5374 6570 732e 7079 0d0a 0d0a 2a20  LTSteps.py....* 
+0000fa80: 5665 7273 696f 6e20 342e 302e 300d 0a20  Version 4.0.0.. 
+0000fa90: 2020 202a 2053 6570 6172 6174 696e 6720     * Separating 
+0000faa0: 7468 6520 5369 6d43 6f6d 6d61 6e64 6572  the SimCommander
+0000fab0: 2069 6e74 6f20 7477 6f20 7365 7061 7261   into two separa
+0000fac0: 7465 2063 6c61 7373 6573 2c20 6f6e 6520  te classes, one 
+0000fad0: 666f 7220 7468 6520 7370 6963 6520 6e65  for the spice ne
+0000fae0: 746c 6973 7420 6564 6974 696e 6720 2853  tlist editing (S
+0000faf0: 7069 6365 4564 6974 6f72 2920 616e 6420  piceEditor) and 
+0000fb00: 616e 6f74 6865 720d 0a20 2020 2020 2066  another..      f
+0000fb10: 6f72 2074 6865 2073 696d 756c 6174 696f  or the simulatio
+0000fb20: 6e20 6578 6563 7574 696f 6e20 2853 696d  n execution (Sim
+0000fb30: 5275 6e6e 6572 292e 0d0a 2020 2020 2a20  Runner)...    * 
+0000fb40: 496d 706c 656d 656e 7469 6e67 2073 696d  Implementing sim
+0000fb50: 756c 6174 696f 6e20 7365 7276 6572 2074  ulation server t
+0000fb60: 6f20 616c 6c6f 7720 666f 7220 7265 6d6f  o allow for remo
+0000fb70: 7465 2073 696d 756c 6174 696f 6e20 6578  te simulation ex
+0000fb80: 6563 7574 696f 6e20 616e 6420 7468 6520  ecution and the 
+0000fb90: 7265 7370 6563 7469 7665 2063 6c69 656e  respective clien
+0000fba0: 742e 0d0a 2020 2020 2a20 5375 7070 6f72  t...    * Suppor
+0000fbb0: 7469 6e67 2057 6967 676c 6572 2065 6c65  ting Wiggler ele
+0000fbc0: 6d65 6e74 2069 6e20 7468 6520 6e65 7720  ment in the new 
+0000fbd0: 4c54 5370 6963 6558 5649 492e 0d0a 2020  LTSpiceXVII...  
+0000fbe0: 2020 2a20 5265 6e61 6d69 6e67 2061 6c6c    * Renaming all
+0000fbf0: 2066 696c 6573 2069 6e74 6f20 6c6f 7765   files into lowe
+0000fc00: 7263 6173 652e 0d0a 2020 2020 2a20 4372  rcase...    * Cr
+0000fc10: 6561 7469 6e67 2045 7272 6f72 2063 6c61  eating Error cla
+0000fc20: 7373 6573 2066 6f72 2062 6574 7465 7220  sses for better 
+0000fc30: 6572 726f 7220 6861 6e64 6c69 6e67 2e0d  error handling..
+0000fc40: 0a20 2020 202a 2041 6464 696e 6720 7375  .    * Adding su
+0000fc50: 7070 6f72 7420 666f 7220 6f74 6865 7220  pport for other 
+0000fc60: 7369 6d75 6c61 746f 7273 2028 6578 3a20  simulators (ex: 
+0000fc70: 6e67 7370 6963 6529 2077 6865 7265 2074  ngspice) where t
+0000fc80: 6865 2073 696d 756c 6174 6f72 2069 7320  he simulator is 
+0000fc90: 6465 6669 6e65 6420 6279 2061 2063 6c61  defined by a cla
+0000fca0: 7373 2e20 5468 6973 0d0a 2020 2020 2020  ss. This..      
+0000fcb0: 7375 7070 6f72 7420 636c 6173 7320 6e65  support class ne
+0000fcc0: 6564 7320 746f 2062 6520 6120 7375 6263  eds to be a subc
+0000fcd0: 6c61 7373 206f 6620 7468 6520 6162 7374  lass of the abst
+0000fce0: 7261 6374 2063 6c61 7373 2053 696d 756c  ract class Simul
+0000fcf0: 6174 6f72 2e0d 0a20 2020 202a 2045 6e6f  ator...    * Eno
+0000fd00: 726d 6f75 7320 696d 7072 6f76 656d 656e  rmous improvemen
+0000fd10: 7420 696e 2074 6865 2064 6f63 756d 656e  t in the documen
+0000fd20: 7461 7469 6f6e 206f 6620 7468 6520 636f  tation of the co
+0000fd30: 6465 2e0d 0a0d 0a2a 2056 6572 7369 6f6e  de.....* Version
+0000fd40: 2033 2e30 0d0a 2020 2020 2a20 456c 696d   3.0..    * Elim
+0000fd50: 696e 6174 696e 6720 7468 6520 4c54 5370  inating the LTSp
+0000fd60: 6963 6520 7072 6566 6978 6573 2066 726f  ice prefixes fro
+0000fd70: 6d20 6669 6c65 7320 616e 6420 636c 6173  m files and clas
+0000fd80: 7365 732e 0d0a 2020 2020 2a20 4164 6f70  ses...    * Adop
+0000fd90: 7469 6e67 2074 6865 206c 6f77 6572 6361  ting the lowerca
+0000fda0: 7365 2063 6f6e 7665 6e74 696f 6e20 666f  se convention fo
+0000fdb0: 7220 6669 6c65 6e61 6d65 732e 0d0a 0d0a  r filenames.....
+0000fdc0: 2a20 5665 7273 696f 6e20 322e 332e 310d  * Version 2.3.1.
+0000fdd0: 0a20 2020 202a 2042 7567 2066 6978 206f  .    * Bug fix o
+0000fde0: 6e20 7468 6520 7061 7261 6d65 7465 7220  n the parameter 
+0000fdf0: 7265 706c 6163 656d 656e 742e 0d0a 0d0a  replacement.....
+0000fe00: 2a20 5665 7273 696f 6e20 322e 330d 0a20  * Version 2.3.. 
+0000fe10: 2020 202a 2053 7570 706f 7274 696e 6720     * Supporting 
+0000fe20: 7468 6520 6372 6561 7469 6f6e 206f 6620  the creation of 
+0000fe30: 5241 5720 4e6f 6973 6520 416e 616c 7973  RAW Noise Analys
+0000fe40: 6973 0d0a 2020 2020 2a20 4275 6720 4669  is..    * Bug Fi
+0000fe50: 7865 7320 2853 6565 2047 6974 4875 6220  xes (See GitHub 
+0000fe60: 4c6f 6729 0d0a 0d0a 2a20 5665 7273 696f  Log)....* Versio
+0000fe70: 6e20 322e 320d 0a20 2020 202a 204d 616b  n 2.2..    * Mak
+0000fe80: 696e 6720 6e75 6d70 7920 6173 2061 2072  ing numpy as a r
+0000fe90: 6571 7569 7265 6d65 6e74 2061 6e64 2065  equirement and e
+0000fea0: 6c69 6d69 6e61 7469 6e67 2061 6c6c 2063  liminating all c
+0000feb0: 6f64 6520 7468 6174 2061 766f 6964 6564  ode that avoided
+0000fec0: 2074 6865 2075 7365 206f 6620 6e75 6d70   the use of nump
+0000fed0: 790d 0a20 2020 202a 2055 7369 6e67 206e  y..    * Using n
+0000fee0: 6577 2070 6163 6b61 6769 6e67 2074 6f6f  ew packaging too
+0000fef0: 6c0d 0a20 2020 202a 2046 6978 6573 206f  l..    * Fixes o
+0000ff00: 6e20 7468 6520 4c54 5370 6963 655f 5261  n the LTSpice_Ra
+0000ff10: 7757 7269 7465 0d0a 2020 2020 2a20 4669  wWrite..    * Fi
+0000ff20: 7865 7320 696e 2074 6865 2068 616e 646c  xes in the handl
+0000ff30: 696e 6720 6f66 2073 7465 7070 6564 206f  ing of stepped o
+0000ff40: 7065 7261 7469 6e67 2070 6f69 6e74 2073  perating point s
+0000ff50: 696d 756c 6174 696f 6e73 0d0a 0d0a 2a20  imulations....* 
+0000ff60: 5665 7273 696f 6e20 322e 310d 0a20 2020  Version 2.1..   
+0000ff70: 202a 2041 646f 7074 696e 6720 6d69 6e69   * Adopting mini
+0000ff80: 6d75 6d20 7079 7468 6f6e 2076 6572 7369  mum python versi
+0000ff90: 6f6e 2033 2e37 0d0a 2020 2020 2a20 5374  on 3.7..    * St
+0000ffa0: 6172 7469 6e67 2074 6f20 7573 6520 756e  arting to use un
+0000ffb0: 6974 2074 6573 7473 2074 6f20 7661 6c69  it tests to vali
+0000ffc0: 6461 7465 2061 6c6c 206d 6f64 756c 6573  date all modules
+0000ffd0: 2061 6e64 2069 6d70 726f 7669 6e67 2074   and improving t
+0000ffe0: 6573 7462 656e 6368 6573 0d0a 2020 2020  estbenches..    
+0000fff0: 2a20 436f 6d70 6174 6962 696c 6974 7920  * Compatibility 
+00010000: 7769 7468 204e 4753 7069 6365 0d0a 2020  with NGSpice..  
+00010010: 2020 2a20 4176 6f69 6469 6e67 2074 6865    * Avoiding the
+00010020: 2075 7365 206f 6620 7365 7475 702e 7079   use of setup.py
+00010030: 2061 7320 7065 7220 5045 5035 3137 2061   as per PEP517 a
+00010040: 6e64 2050 4550 3531 380d 0a20 2020 202a  nd PEP518..    *
+00010050: 2042 7567 2046 6978 6573 2028 5365 6520   Bug Fixes (See 
+00010060: 4769 7448 7562 206c 6f67 2066 6f72 206d  GitHub log for m
+00010070: 6f72 6520 696e 666f 726d 6174 696f 6e29  ore information)
+00010080: 0d0a 2020 2020 2a20 496d 7072 6f76 656d  ..    * Improvem
+00010090: 656e 7473 206f 6e20 7468 6520 6d61 6e61  ents on the mana
+000100a0: 6765 6d65 6e74 206f 6620 7374 6570 7065  gement of steppe
+000100b0: 6420 6461 7461 2069 6e20 7468 6520 4c54  d data in the LT
+000100c0: 5370 6963 655f 5261 7752 6561 642e 7079  Spice_RawRead.py
+000100d0: 0d0a 0d0a 2a20 5665 7273 696f 6e20 322e  ....* Version 2.
+000100e0: 302e 320d 0a20 2020 202a 2049 6d70 726f  0.2..    * Impro
+000100f0: 7665 6d65 6e74 7320 6f6e 2045 6e63 6f64  vements on Encod
+00010100: 696e 6720 6465 7465 6374 696f 6e0d 0a0d  ing detection...
+00010110: 0a2a 2056 6572 7369 6f6e 2032 2e30 0d0a  .* Version 2.0..
+00010120: 2020 2020 2a20 496e 7465 726e 6174 696f      * Internatio
+00010130: 6e61 6c20 5375 7070 6f72 7420 7573 696e  nal Support usin
+00010140: 6720 7468 6520 636f 7272 6563 7420 656e  g the correct en
+00010150: 636f 6469 6e67 2077 6865 6e20 6c6f 6164  coding when load
+00010160: 696e 6720 6c6f 6720 6669 6c65 732e 0d0a  ing log files...
+00010170: 2020 2020 2a20 436f 6465 204f 7074 696d      * Code Optim
+00010180: 697a 6174 696f 6e73 206f 6e20 7468 6520  izations on the 
+00010190: 4c54 5370 6963 655f 5261 7752 6561 6465  LTSpice_RawReade
+000101a0: 7220 7468 6174 2061 6c6c 6f77 2066 6173  r that allow fas
+000101b0: 7465 7220 6461 7461 206c 6f61 6469 6e67  ter data loading
+000101c0: 2e0d 0a20 2020 202a 2049 6d70 726f 7669  ...    * Improvi
+000101d0: 6e67 2074 6865 2066 756e 6374 696f 6e61  ng the functiona
+000101e0: 6c69 7479 206f 6e20 7468 6520 4c54 5370  lity on the LTSp
+000101f0: 6963 655f 5261 7757 7269 7465 722e 7079  ice_RawWriter.py
+00010200: 0d0a 2020 2020 2a20 4164 6469 6e67 2073  ..    * Adding s
+00010210: 7570 706f 7274 2074 6f20 6564 6974 696e  upport to editin
+00010220: 6720 636f 6d70 6f6e 656e 7473 2069 6e73  g components ins
+00010230: 6964 6520 7375 6263 6972 6375 6974 7320  ide subcircuits 
+00010240: 282e 7375 6263 6b74 290d 0a20 2020 202a  (.subckt)..    *
+00010250: 2053 7570 706f 7274 696e 6720 7265 7369   Supporting resi
+00010260: 7374 6f72 7320 7769 7468 204d 6f64 656c  stors with Model
+00010270: 2044 6566 696e 6974 696f 6e73 0d0a 2020   Definitions..  
+00010280: 2020 2a20 4669 7869 6e67 2070 726f 626c    * Fixing probl
+00010290: 656d 2077 6974 6820 4c54 5370 6963 654c  em with LTSpiceL
+000102a0: 6f67 5265 6164 6572 2074 6861 7420 776f  ogReader that wo
+000102b0: 756c 6420 7265 7475 726e 206d 6573 7365  uld return messe
+000102c0: 6420 7570 2064 6174 610d 0a20 2020 202a  d up data..    *
+000102d0: 2046 6978 696e 6720 7072 6f62 6c65 6d20   Fixing problem 
+000102e0: 7769 7468 2072 6570 6c61 6369 6e67 2074  with replacing t
+000102f0: 6865 2066 696c 6520 6578 7465 6e73 696f  he file extensio
+00010300: 6e20 696e 2063 6572 7461 696e 206e 616d  n in certain nam
+00010310: 6573 0d0a 2020 2020 2a20 436f 7272 6563  es..    * Correc
+00010320: 7469 6e67 2070 726f 626c 656d 2077 6974  ting problem wit
+00010330: 6820 6465 7072 6563 6174 696f 6e73 206f  h deprecations o
+00010340: 6e20 7468 6520 6e75 6d70 7920 6675 6e63  n the numpy func
+00010350: 7469 6f6e 7320 7573 6564 2062 7920 7468  tions used by th
+00010360: 6520 4869 7374 6f67 7261 6d2e 7079 0d0a  e Histogram.py..
+00010370: 2020 2020 2a20 4164 6469 6e67 2062 6163      * Adding bac
+00010380: 6b20 7468 6520 5245 4144 4d45 2e6d 6420  k the README.md 
+00010390: 7468 6174 2073 6f6d 6568 6f77 2077 6173  that somehow was
+000103a0: 2064 656c 6574 6564 0d0a 0d0a 2a20 5665   deleted....* Ve
+000103b0: 7273 696f 6e20 312e 390d 0a20 2020 202a  rsion 1.9..    *
+000103c0: 2041 6464 696e 6720 7375 7070 6f72 7420   Adding support 
+000103d0: 666f 7220 c2b5 2063 6861 7261 6374 6572  for .. character
+000103e0: 2069 6e20 7468 6520 5370 6963 6545 6469   in the SpiceEdi
+000103f0: 746f 722e 0d0a 2020 2020 2a20 4164 6469  tor...    * Addi
+00010400: 6e67 2067 6574 5f63 6f6d 706f 6e65 6e74  ng get_component
+00010410: 5f66 6c6f 6174 7661 6c75 6528 2920 6d65  _floatvalue() me
+00010420: 7468 6f64 2069 6e20 7468 6520 6e65 746c  thod in the netl
+00010430: 6973 7420 6d61 6e69 7075 6c61 7469 6e67  ist manipulating
+00010440: 2063 6c61 7373 2074 6861 7420 6861 6e64   class that hand
+00010450: 6c65 7320 7468 6520 636f 6e76 6572 7369  les the conversi
+00010460: 6f6e 206f 6620 6e75 6d65 7269 630d 0a20  on of numeric.. 
+00010470: 2020 2020 2066 6965 6c64 7320 696e 746f       fields into
+00010480: 2061 2066 6c6f 6174 2e20 5468 6973 2066   a float. This f
+00010490: 756e 6374 696f 6e20 7461 6b65 7320 696e  unction takes in
+000104a0: 746f 2061 6363 6f75 6e74 2074 6865 2065  to account the e
+000104b0: 6e67 696e 6565 7269 6e67 2071 7561 6c69  ngineering quali
+000104c0: 6669 6572 7320 276b 2720 666f 7220 6b69  fiers 'k' for ki
+000104d0: 6c6f 732c 2027 6d27 206f 7220 6d69 6c69  los, 'm' or mili
+000104e0: 732c 0d0a 2020 2020 2020 2775 2720 6f72  s,..      'u' or
+000104f0: 2027 c2b5 2720 666f 7220 6d69 6372 6f6e   '..' for micron
+00010500: 732c 2027 6e27 2066 6f72 206e 616e 6f73  s, 'n' for nanos
+00010510: 2c20 2766 2720 666f 7220 6665 6d74 6f73  , 'f' for femtos
+00010520: 2061 6e64 2027 4d65 6727 2066 6f72 204d   and 'Meg' for M
+00010530: 6567 6173 2e0d 0a0d 0a2a 2056 6572 7369  egas.....* Versi
+00010540: 6f6e 2031 2e38 0d0a 2020 2020 2a20 556e  on 1.8..    * Un
+00010550: 6966 6f72 6d69 6e67 204c 6963 656e 7365  iforming License
+00010560: 2072 6566 6572 656e 6365 2061 6372 6f73   reference acros
+00010570: 7320 6669 6c65 7320 616e 6420 696d 7072  s files and impr
+00010580: 6f76 656d 656e 7473 206f 6e20 7468 6520  ovements on the 
+00010590: 646f 6375 6d65 6e74 6174 696f 6e0d 0a20  documentation.. 
+000105a0: 2020 202a 2041 6e20 656e 6f72 6d6f 7573     * An enormous
+000105b0: 2061 6e64 2077 686f 6c65 6865 6172 7465   and wholehearte
+000105c0: 6420 7468 616e 6b73 2074 6f20 406c 7068  d thanks to @lph
+000105d0: 6572 7220 666f 7220 7468 6520 696d 7072  err for the impr
+000105e0: 6f76 656d 656e 7473 2069 6e20 7468 6520  ovements in the 
+000105f0: 646f 6375 6d65 6e74 6174 696f 6e2e 0d0a  documentation...
+00010600: 2020 2020 2a20 4275 6766 6978 206f 6e20      * Bugfix on 
+00010610: 7468 6520 6164 645f 4c54 7370 6963 6552  the add_LTspiceR
+00010620: 756e 436d 644c 696e 6553 7769 7463 6865  unCmdLineSwitche
+00010630: 7328 2920 3b20 5375 7070 6f72 7469 6e67  s() ; Supporting
+00010640: 202e 7061 7261 6d20 6e61 6d65 2076 616c   .param name val
+00010650: 7565 2066 6f72 6d61 740d 0a20 2020 202a  ue format..    *
+00010660: 2041 6c6c 6f77 696e 6720 7468 6520 4c54   Allowing the LT
+00010670: 5370 6963 6552 6177 5265 6164 2074 6f20  SpiceRawRead to 
+00010680: 7072 6f63 6565 6420 7768 656e 2074 6865  proceed when the
+00010690: 206c 6f67 2066 696c 6520 6361 6e27 7420   log file can't 
+000106a0: 6265 2066 6f75 6e64 206f 7220 7768 656e  be found or when
+000106b0: 2074 6865 7265 2061 7265 2070 726f 626c   there are probl
+000106c0: 656d 7320 7265 6164 696e 6720 6974 2e0d  ems reading it..
+000106d0: 0a2a 2056 6572 7369 6f6e 2031 2e37 0d0a  .* Version 1.7..
+000106e0: 2020 2020 2a20 5275 6e6e 696e 6720 696e      * Running in
+000106f0: 204c 696e 7578 2075 6e64 6572 2077 696e   Linux under win
+00010700: 6520 6973 206e 6f77 2070 6f73 7369 626c  e is now possibl
+00010710: 650d 0a0d 0a2a 2056 6572 7369 6f6e 2031  e....* Version 1
+00010720: 2e36 0d0a 2020 2020 2a20 4164 6469 6e67  .6..    * Adding
+00010730: 204c 5453 7069 6365 5f52 6177 5772 6974   LTSpice_RawWrit
+00010740: 652e 2041 6464 696e 6720 646f 6375 6d65  e. Adding docume
+00010750: 6e74 6174 696f 6e2e 0d0a 0d0a 2a20 5665  ntation.....* Ve
+00010760: 7273 696f 6e20 312e 350d 0a20 2020 202a  rsion 1.5..    *
+00010770: 2053 6d61 6c6c 2066 6978 6573 2061 6e64   Small fixes and
+00010780: 2069 6d70 726f 7665 6d65 6e74 7320 6f6e   improvements on
+00010790: 2074 6865 2063 6c61 7373 2075 7361 6765   the class usage
+000107a0: 2e20 4e6f 2061 6464 6564 2066 6561 7475  . No added featu
+000107b0: 7265 730d 0a0d 0a2a 2056 6572 7369 6f6e  res....* Version
+000107c0: 2031 2e34 0d0a 2020 2020 2a20 4164 6469   1.4..    * Addi
+000107d0: 6e67 2074 6865 204c 5453 7069 6365 5f53  ng the LTSpice_S
+000107e0: 656d 6944 6576 4f70 5265 6164 6572 206d  emiDevOpReader m
+000107f0: 6f64 756c 650d 0a20 2020 202a 2052 652d  odule..    * Re-
+00010800: 656e 6162 6c69 6e67 2074 6865 2048 6973  enabling the His
+00010810: 746f 6772 616d 2066 756e 6374 696f 6e73  togram functions
+00010820: 2077 6869 6368 2077 6865 7265 2064 6973   which where dis
+00010830: 6162 6c65 6420 6279 206d 6973 7461 6b65  abled by mistake
+00010840: 2e0d 0a0d 0a2a 2056 6572 7369 6f6e 2031  .....* Version 1
+00010850: 2e33 0d0a 2020 2020 2a20 4275 6720 6669  .3..    * Bug fi
+00010860: 7865 7320 6f6e 2074 6865 2053 7069 6365  xes on the Spice
+00010870: 4564 6974 6f72 2043 6c61 7373 0d0a 0d0a  Editor Class....
+00010880: 2a20 5665 7273 696f 6e20 312e 320d 0a20  * Version 1.2.. 
+00010890: 2020 202a 2052 4541 444d 452e 6d64 3a0d     * README.md:.
+000108a0: 0a20 2020 2020 2041 6464 696e 6720 6c69  .      Adding li
+000108b0: 6e6b 2074 6f20 7265 6164 7468 6564 6f63  nk to readthedoc
+000108c0: 7320 646f 6375 6d65 6e74 6174 696f 6e0d  s documentation.
+000108d0: 0a20 2020 202a 2041 6c6c 2066 696c 6573  .    * All files
+000108e0: 3a0d 0a20 2020 2020 2043 6f6d 7072 6568  :..      Compreh
+000108f0: 656e 7369 7665 2064 6f63 756d 656e 7461  ensive documenta
+00010900: 7469 6f6e 206f 6e20 686f 7720 746f 2075  tion on how to u
+00010910: 7365 2065 6163 6820 6d6f 6475 6c65 0d0a  se each module..
+00010920: 0d0a 2a20 5665 7273 696f 6e20 312e 310d  ..* Version 1.1.
+00010930: 0a20 2020 202a 2052 4541 444d 452e 6d64  .    * README.md
+00010940: 3a0d 0a20 2020 2020 2055 7064 6174 6564  :..      Updated
+00010950: 2074 6865 2064 6573 6372 6970 7469 6f6e   the description
+00010960: 0d0a 2020 2020 2a20 4c54 5370 6963 6542  ..    * LTSpiceB
+00010970: 6174 6368 2e70 793a 0d0a 2020 2020 2020  atch.py:..      
+00010980: 436f 7272 6563 7465 6420 7468 6520 6e61  Corrected the na
+00010990: 6d65 206f 6620 7468 6520 7265 7475 726e  me of the return
+000109a0: 6564 2072 6177 2066 696c 652e 0d0a 2020  ed raw file...  
+000109b0: 2020 2a20 4164 6465 6420 636f 6d6d 656e    * Added commen
+000109c0: 7473 2074 6872 6f75 6768 6f75 7420 7468  ts throughout th
+000109d0: 6520 636f 6465 2061 6e64 2063 6c65 616e  e code and clean
+000109e0: 7570 0d0a 0d0a 2a20 5665 7273 696f 6e20  up....* Version 
+000109f0: 312e 300d 0a20 2020 202a 204c 5453 7069  1.0..    * LTSpi
+00010a00: 6365 4261 7463 682e 7079 3a5c 0d0a 2020  ceBatch.py:\..  
+00010a10: 2020 2020 496d 706c 656d 656e 7465 6420      Implemented 
+00010a20: 6120 6e65 7720 6170 7072 6f61 6368 2028  a new approach (
+00010a30: 4e4f 5420 4241 434b 5741 5244 5320 434f  NOT BACKWARDS CO
+00010a40: 4d50 4154 4942 4c45 292c 2074 6861 7420  MPATIBLE), that 
+00010a50: 6176 6f69 6473 2074 6865 2075 7361 6765  avoids the usage
+00010a60: 206f 6620 7468 6520 7369 6d5f 7365 7474   of the sim_sett
+00010a70: 696e 6773 2e69 6e63 2066 696c 652e 0d0a  ings.inc file...
+00010a80: 2020 2020 2020 416e 6420 616c 6c6f 7773        And allows
+00010a90: 2074 6f20 6d6f 6469 6679 206e 6f74 206f   to modify not o
+00010aa0: 6e6c 7920 7061 7261 6d65 7465 7273 2c20  nly parameters, 
+00010ab0: 6275 7420 616c 736f 206d 6f64 656c 7320  but also models 
+00010ac0: 616e 6420 6576 656e 2074 6865 2073 696d  and even the sim
+00010ad0: 756c 6174 696f 6e20 636f 6d6d 616e 6473  ulation commands
+00010ae0: 2e0d 0a20 2020 202a 204c 5453 7069 6365  ...    * LTSpice
+00010af0: 5f52 6177 5265 6164 2e70 793a 5c0d 0a20  _RawRead.py:\.. 
+00010b00: 2020 2020 2041 6464 6564 2074 6865 2067       Added the g
+00010b10: 6574 5f74 696d 655f 6178 6973 206d 6574  et_time_axis met
+00010b20: 686f 6420 746f 2074 6865 2052 6177 5265  hod to the RawRe
+00010b30: 6164 2063 6c61 7373 2074 6f20 6176 6f69  ad class to avoi
+00010b40: 6420 7468 6520 7072 6f62 6c65 6d73 2077  d the problems w
+00010b50: 6974 6820 6e65 6761 7469 7665 2076 616c  ith negative val
+00010b60: 7565 7320 6f6e 2074 696d 6520 6178 6973  ues on time axis
+00010b70: 2c0d 0a20 2020 2020 2077 6865 6e20 326e  ,..      when 2n
+00010b80: 6420 6f72 6465 7220 636f 6d70 7265 7373  d order compress
+00010b90: 696f 6e20 6973 2065 6e61 626c 6564 2069  ion is enabled i
+00010ba0: 6e20 4c54 5370 6963 652e 0d0a 2020 2020  n LTSpice...    
+00010bb0: 2a20 4c54 5374 6570 732e 7079 3a5c 0d0a  * LTSteps.py:\..
+00010bc0: 2020 2020 2020 4d6f 6469 6669 6564 2074        Modified t
+00010bd0: 6865 204c 5453 7465 7073 2c20 736f 2069  he LTSteps, so i
+00010be0: 7420 6361 6e20 616c 736f 2072 6561 6420  t can also read 
+00010bf0: 6d65 6173 7572 656d 656e 7473 206f 6e20  measurements on 
+00010c00: 6c6f 6720 6669 6c65 7320 7769 7468 6f75  log files withou
+00010c10: 7420 616e 7920 7374 6570 7320 646f 6e65  t any steps done
+00010c20: 2e0d 0a0d 0a2a 2056 6572 7369 6f6e 2030  .....* Version 0
+00010c30: 2e36 0d0a 2020 2a20 4869 7374 6f67 7261  .6..  * Histogra
+00010c40: 6d2e 7079 206e 6f77 2068 6173 2061 6e20  m.py now has an 
+00010c50: 6f70 7469 6f6e 2074 6f20 6d61 6b65 2074  option to make t
+00010c60: 6865 2068 6973 746f 6772 616d 2064 6972  he histogram dir
+00010c70: 6563 746c 7920 6672 6f6d 2076 616c 7565  ectly from value
+00010c80: 7320 7374 6f72 6564 2069 6e20 7468 6520  s stored in the 
+00010c90: 636c 6970 626f 6172 640d 0a0d 0a2a 2056  clipboard....* V
+00010ca0: 6572 7369 6f6e 2030 2e35 0d0a 2020 2a20  ersion 0.5..  * 
+00010cb0: 5468 6520 4c54 5370 6963 655f 5261 7752  The LTSpice_RawR
+00010cc0: 6561 6465 722e 7079 206e 6f77 2075 7365  eader.py now use
+00010cd0: 7320 7468 6520 6073 7472 7563 742e 756e  s the `struct.un
+00010ce0: 7061 636b 6020 6675 6e63 7469 6f6e 2066  pack` function f
+00010cf0: 6f72 2061 2066 6173 7465 7220 6578 6563  or a faster exec
+00010d00: 7574 696f 6e0d 0a0d 0a2a 2056 6572 7369  ution....* Versi
+00010d10: 6f6e 2030 2e34 0d0a 2020 2a20 4164 6465  on 0.4..  * Adde
+00010d20: 6420 4c54 5370 6963 6542 6174 6368 2e70  d LTSpiceBatch.p
+00010d30: 7920 746f 2074 6865 2063 6f6c 6c65 6374  y to the collect
+00010d40: 696f 6e20 6f66 2074 6f6f 6c73 0d0a 0d0a  ion of tools....
+00010d50: 2a20 5665 7273 696f 6e20 302e 330d 0a20  * Version 0.3.. 
+00010d60: 202a 2041 2076 6572 7369 6f6e 206f 6620   * A version of 
+00010d70: 4c54 5374 6570 7320 7468 6174 2063 616e  LTSteps that can
+00010d80: 2062 6520 696d 706f 7274 6564 2074 6f20   be imported to 
+00010d90: 7573 6520 696e 2061 2068 6967 6865 7220  use in a higher 
+00010da0: 6c65 7665 6c20 7363 7269 7074 0d0a 0d0a  level script....
+00010db0: 2a20 5665 7273 696f 6e20 302e 320d 0a20  * Version 0.2.. 
+00010dc0: 202a 2041 6464 696e 6720 4c54 5374 6570   * Adding LTStep
+00010dd0: 732e 7079 2061 6e64 2048 6973 746f 6772  s.py and Histogr
+00010de0: 616d 2e70 790d 0a0d 0a2a 2056 6572 7369  am.py....* Versi
+00010df0: 6f6e 2030 2e31 200d 0a20 202a 2046 6972  on 0.1 ..  * Fir
+00010e00: 7374 2063 6f6d 6d69 7420 746f 2074 6865  st commit to the
+00010e10: 2062 6974 6275 636b 6574 2072 6570 6f73   bitbucket repos
+00010e20: 6974 6f72 792e 0d0a                      itory...
```

### Comparing `PyLTSpice-5.2.2/PyLTSpice/Histogram.py` & `pyltspice-5.3.0/PyLTSpice/Histogram.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/LTSteps.py` & `pyltspice-5.3.0/PyLTSpice/LTSteps.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/__init__.py` & `pyltspice-5.3.0/PyLTSpice/__init__.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/editor/asc_editor.py` & `pyltspice-5.3.0/PyLTSpice/editor/asc_editor.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/editor/spice_editor.py` & `pyltspice-5.3.0/PyLTSpice/editor/spice_editor.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/log/logfile_data.py` & `pyltspice-5.3.0/PyLTSpice/log/logfile_data.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/log/ltsteps.py` & `pyltspice-5.3.0/PyLTSpice/log/ltsteps.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/log/semi_dev_op_reader.py` & `pyltspice-5.3.0/PyLTSpice/log/semi_dev_op_reader.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/raw/raw_classes.py` & `pyltspice-5.3.0/PyLTSpice/raw/raw_classes.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/raw/raw_read.py` & `pyltspice-5.3.0/PyLTSpice/raw/raw_read.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/raw/raw_write.py` & `pyltspice-5.3.0/PyLTSpice/raw/raw_write.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/rawplot.py` & `pyltspice-5.3.0/PyLTSpice/rawplot.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/run_server.py` & `pyltspice-5.3.0/PyLTSpice/run_server.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/sim/ltspice_simulator.py` & `pyltspice-5.3.0/PyLTSpice/sim/ltspice_simulator.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/sim/process_callback.py` & `pyltspice-5.3.0/PyLTSpice/sim/process_callback.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/sim/sim_batch.py` & `pyltspice-5.3.0/PyLTSpice/sim/sim_batch.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/sim/sim_runner.py` & `pyltspice-5.3.0/PyLTSpice/sim/sim_runner.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/sim/sim_stepping.py` & `pyltspice-5.3.0/PyLTSpice/sim/sim_stepping.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/sim/tookit/montecarlo.py` & `pyltspice-5.3.0/PyLTSpice/sim/tookit/montecarlo.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/sim/tookit/worst_case.py` & `pyltspice-5.3.0/PyLTSpice/sim/tookit/worst_case.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/utils/detect_encoding.py` & `pyltspice-5.3.0/PyLTSpice/utils/detect_encoding.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice/utils/sweep_iterators.py` & `pyltspice-5.3.0/PyLTSpice/utils/sweep_iterators.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/PyLTSpice.egg-info/PKG-INFO` & `pyltspice-5.3.0/PyLTSpice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2050 794c  : 2.1..Name: PyL
 00000020: 5453 7069 6365 0d0a 5665 7273 696f 6e3a  TSpice..Version:
-00000030: 2035 2e32 2e32 0d0a 5375 6d6d 6172 793a   5.2.2..Summary:
+00000030: 2035 2e33 2e30 0d0a 5375 6d6d 6172 793a   5.3.0..Summary:
 00000040: 2041 2073 6574 206f 6620 746f 6f6c 7320   A set of tools 
 00000050: 746f 2041 7574 6f6d 6174 6520 4c54 5370  to Automate LTSp
 00000060: 6963 6520 7369 6d75 6c61 7469 6f6e 730d  ice simulations.
 00000070: 0a41 7574 686f 722d 656d 6169 6c3a 204e  .Author-email: N
 00000080: 756e 6f20 4272 756d 203c 6d65 406e 756e  uno Brum <me@nun
 00000090: 6f62 7275 6d2e 636f 6d3e 0d0a 4c69 6365  obrum.com>..Lice
 000000a0: 6e73 653a 2020 2020 2020 2020 2020 2020  nse:            
@@ -2614,15 +2614,15 @@
 0000a350: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
 0000a360: 3e3d 332e 380d 0a44 6573 6372 6970 7469  >=3.8..Descripti
 0000a370: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
 0000a380: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
 0000a390: 4c69 6365 6e73 652d 4669 6c65 3a20 4c49  License-File: LI
 0000a3a0: 4345 4e53 450d 0a52 6571 7569 7265 732d  CENSE..Requires-
 0000a3b0: 4469 7374 3a20 7370 6963 656c 6962 3e3d  Dist: spicelib>=
-0000a3c0: 312e 302e 340d 0a0d 0a23 2052 4541 444d  1.0.4....# READM
+0000a3c0: 312e 312e 310d 0a0d 0a23 2052 4541 444d  1.1.1....# READM
 0000a3d0: 4520 230d 0a0d 0a50 794c 5453 7069 6365  E #....PyLTSpice
 0000a3e0: 2069 7320 6120 746f 6f6c 6368 6169 6e20   is a toolchain 
 0000a3f0: 6f66 2070 7974 686f 6e20 7574 696c 6974  of python utilit
 0000a400: 6965 7320 6465 7369 676e 2074 6f20 696e  ies design to in
 0000a410: 7465 7261 6374 2077 6974 6820 4c54 5370  teract with LTSp
 0000a420: 6963 6520 456c 6563 7472 6f6e 6963 2053  ice Electronic S
 0000a430: 696d 756c 6174 6f72 2e0d 0a49 7420 6973  imulator...It is
@@ -3821,498 +3821,503 @@
 0000eec0: 6d2e 636f 6d29 0d0a 2a20 416c 7465 726e  m.com)..* Altern
 0000eed0: 6174 6976 6520 636f 6e74 6163 7420 3a20  ative contact : 
 0000eee0: 5b6e 756e 6f2e 6272 756d 4067 6d61 696c  [nuno.brum@gmail
 0000eef0: 2e63 6f6d 5d28 6d61 696c 746f 3a6e 756e  .com](mailto:nun
 0000ef00: 6f2e 6272 756d 4067 6d61 696c 2e63 6f6d  o.brum@gmail.com
 0000ef10: 290d 0a0d 0a23 2320 4869 7374 6f72 7920  )....## History 
 0000ef20: 2323 0d0a 2a20 5665 7273 696f 6e20 352e  ##..* Version 5.
-0000ef30: 322e 330d 0a20 202a 2055 7064 6174 696e  2.3..  * Updatin
-0000ef40: 6720 6c6f 6767 6572 7320 746f 2075 7365  g loggers to use
-0000ef50: 2074 6865 2022 7370 6963 656c 6962 2220   the "spicelib" 
-0000ef60: 4944 732e 0d0a 2020 2a20 4669 7869 6e67  IDs...  * Fixing
-0000ef70: 2061 7574 6f64 6f63 2065 7272 6f72 730d   autodoc errors.
-0000ef80: 0a20 202a 2043 6f72 7265 6374 696e 6720  .  * Correcting 
-0000ef90: 5665 7273 696f 6e20 7265 6665 7265 6e63  Version referenc
-0000efa0: 6573 0d0a 0d0a 2a20 5665 7273 696f 6e20  es....* Version 
-0000efb0: 352e 322e 320d 0a20 202a 2046 6978 6573  5.2.2..  * Fixes
-0000efc0: 206f 6e20 7468 6520 756e 6974 7465 7374   on the unittest
-0000efd0: 7320 6166 7465 7220 7468 6520 7370 6963  s after the spic
-0000efe0: 656c 6962 2075 7064 6174 6520 746f 2031  elib update to 1
-0000eff0: 2e30 2e34 0d0a 0d0a 2a20 5665 7273 696f  .0.4....* Versio
-0000f000: 6e20 352e 322e 310d 0a20 202a 2043 6f72  n 5.2.1..  * Cor
-0000f010: 7265 6374 696f 6e20 6f6e 2074 6865 2072  rection on the r
-0000f020: 756e 5f6d 6f6e 7465 6361 726c 6f2e 7079  un_montecarlo.py
-0000f030: 2061 6e64 2072 756e 5f77 6f72 7374 5f63   and run_worst_c
-0000f040: 6173 652e 7079 2065 7861 6d70 6c65 732e  ase.py examples.
-0000f050: 0d0a 2020 2a20 4669 7865 7320 6f6e 2074  ..  * Fixes on t
-0000f060: 6865 2073 7069 6365 6c69 6220 2856 6572  he spicelib (Ver
-0000f070: 7369 6f6e 2031 2e30 2e33 290d 0a0d 0a2a  sion 1.0.3)....*
-0000f080: 2056 6572 7369 6f6e 2035 2e32 0d0a 2020   Version 5.2..  
-0000f090: 2a20 5369 6d41 6e61 6c79 7369 7320 7375  * SimAnalysis su
-0000f0a0: 7070 6f72 7469 6e67 2062 6f74 6820 5173  pporting both Qs
-0000f0b0: 7069 6365 2061 6e64 204c 5453 7069 6365  pice and LTSpice
-0000f0c0: 206c 6f67 6669 6c65 732e 0d0a 2020 2a20   logfiles...  * 
-0000f0d0: 4661 7374 576f 7273 7443 6173 6541 6e61  FastWorstCaseAna
-0000f0e0: 6c79 7369 7320 616c 676f 7269 7468 6d20  lysis algorithm 
-0000f0f0: 696d 706c 656d 656e 7465 640d 0a20 202a  implemented..  *
-0000f100: 2046 6978 206f 6e20 7468 6520 6c6f 6720   Fix on the log 
-0000f110: 7265 6164 696e 6720 6f66 2066 6f75 7269  reading of fouri
-0000f120: 6572 2064 6174 612e 0d0a 0d0a 2a20 5665  er data.....* Ve
-0000f130: 7273 696f 6e20 352e 310d 0a20 202a 2049  rsion 5.1..  * I
-0000f140: 6d70 6f72 7461 6e74 2042 7567 6669 7820  mportant Bugfix 
-0000f150: 6f6e 2074 6865 204c 5443 6f6d 706c 6578  on the LTComplex
-0000f160: 2063 6c61 7373 2e0d 0a20 202a 2046 6978   class...  * Fix
-0000f170: 6573 2061 6e64 2065 6e68 616e 6369 6e67  es and enhancing
-0000f180: 2074 6865 2061 6e61 6c79 7369 7320 746f   the analysis to
-0000f190: 6f6c 6b69 742e 0d0a 2020 2a20 4465 7072  olkit...  * Depr
-0000f1a0: 6563 6174 696e 6720 5370 6963 6545 6469  ecating SpiceEdi
-0000f1b0: 746f 722e 7772 6974 655f 6e65 746c 6973  tor.write_netlis
-0000f1c0: 7420 696e 2066 6176 6f75 7220 6f66 2073  t in favour of s
-0000f1d0: 6176 655f 6e65 746c 6973 7428 290d 0a0d  ave_netlist()...
-0000f1e0: 0a2a 2056 6572 7369 6f6e 2035 2e30 0d0a  .* Version 5.0..
-0000f1f0: 2020 2a20 4d61 6b69 6e67 2074 6869 7320    * Making this 
-0000f200: 6c69 6272 6172 7920 6465 7065 6e64 656e  library dependen
-0000f210: 7420 6f6e 2073 7069 6365 6c69 6220 7768  t on spicelib wh
-0000f220: 696c 6520 7472 7969 6e67 2074 6f20 6d61  ile trying to ma
-0000f230: 696e 7461 696e 2062 6163 6b77 6172 6420  intain backward 
-0000f240: 636f 6d70 6174 6962 696c 6974 7920 6173  compatibility as
-0000f250: 206d 7563 6820 6173 2070 6f73 7369 626c   much as possibl
-0000f260: 652e 200d 0a20 2050 794c 5473 7069 6365  e. ..  PyLTspice
-0000f270: 2077 696c 6c20 6265 206b 6570 7420 616c   will be kept al
-0000f280: 6976 6520 616e 6420 6974 7320 7570 6461  ive and its upda
-0000f290: 7465 2077 696c 6c20 6265 206c 696e 6b65  te will be linke
-0000f2a0: 6420 746f 2074 6865 2073 7069 6365 6c69  d to the spiceli
-0000f2b0: 622e 2054 6865 206d 6169 6e20 6469 6666  b. The main diff
-0000f2c0: 6572 656e 6365 2069 7320 7468 6174 2075  erence is that u
-0000f2d0: 7369 6e67 0d0a 2020 5079 4c54 7370 6963  sing..  PyLTspic
-0000f2e0: 6520 7769 6c6c 2061 7665 7274 2074 6865  e will avert the
-0000f2f0: 206e 6565 6420 6f66 2068 6176 696e 6720   need of having 
-0000f300: 746f 2073 656c 6563 7420 6120 7369 6d75  to select a simu
-0000f310: 6c61 746f 7220 696e 2061 6c6c 2072 756e  lator in all run
-0000f320: 2063 6f6d 6d61 6e64 732e 0d0a 0d0a 2a20   commands.....* 
-0000f330: 5665 7273 696f 6e20 342e 312e 320d 0a20  Version 4.1.2.. 
-0000f340: 202a 2041 6464 696e 6720 7375 7070 6f72   * Adding suppor
-0000f350: 7420 666f 7220 7468 6520 6e65 7720 5153  t for the new QS
-0000f360: 5049 4345 2073 696d 756c 6174 6f72 0d0a  PICE simulator..
-0000f370: 2020 2a20 496d 7072 6f76 696e 6720 7468    * Improving th
-0000f380: 6520 7469 6d65 6f75 7420 6d65 6368 616e  e timeout mechan
-0000f390: 6973 6d20 6f6e 2074 6865 2053 696d 5275  ism on the SimRu
-0000f3a0: 6e6e 6572 2063 6c61 7373 0d0a 2020 2a20  nner class..  * 
-0000f3b0: 4d69 6e6f 7220 6275 6720 6669 7865 730d  Minor bug fixes.
-0000f3c0: 0a0d 0a2a 2056 6572 7369 6f6e 2034 2e31  ...* Version 4.1
-0000f3d0: 2e31 0d0a 2020 2a20 436f 6d70 6c65 7469  .1..  * Completi
-0000f3e0: 6e67 2074 6865 2057 6f72 7374 2d43 6173  ng the Worst-Cas
-0000f3f0: 6520 416e 616c 7973 6973 2066 756e 6374  e Analysis funct
-0000f400: 696f 6e73 2e20 4164 6469 6e67 2061 2064  ions. Adding a d
-0000f410: 6564 6963 6174 6564 2065 7861 6d70 6c65  edicated example
-0000f420: 2066 6f72 2069 742e 0d0a 2020 2a20 5265   for it...  * Re
-0000f430: 6661 6374 6f72 696e 6720 7468 6520 4c54  factoring the LT
-0000f440: 5370 6963 654c 6f67 5265 6164 6572 2063  SpiceLogReader c
-0000f450: 6c61 7373 2069 6e20 6f72 6465 7220 746f  lass in order to
-0000f460: 2075 7365 2069 7420 6f6e 2074 6865 2041   use it on the A
-0000f470: 6e61 6c79 7369 7320 746f 6f6c 6b69 740d  nalysis toolkit.
-0000f480: 0a0d 0a2a 2056 6572 7369 6f6e 2034 2e31  ...* Version 4.1
-0000f490: 2e30 202a 2872 6571 7569 7265 7320 5079  .0 *(requires Py
-0000f4a0: 7468 6f6e 2033 2e38 206f 7220 6869 6768  thon 3.8 or high
-0000f4b0: 6572 292a 0d0a 2020 2020 2a20 4164 6469  er)*..    * Addi
-0000f4c0: 6e67 2061 206e 6577 2063 6c61 7373 2074  ng a new class t
-0000f4d0: 6f20 6d61 6e69 7075 6c61 7465 2064 6972  o manipulate dir
-0000f4e0: 6563 746c 7920 7468 6520 2e61 7363 2066  ectly the .asc f
-0000f4f0: 696c 6573 2e0d 0a20 2020 202a 204d 6f64  iles...    * Mod
-0000f500: 6966 7969 6e67 2061 6c6c 2074 6865 206f  ifying all the o
-0000f510: 7468 6572 2063 6c61 7373 6573 2069 6e20  ther classes in 
-0000f520: 6f72 6465 7220 746f 2075 7365 2074 6865  order to use the
-0000f530: 206e 6577 2063 6c61 7373 2e0d 0a20 2020   new class...   
-0000f540: 202a 2041 6464 696e 6720 636c 6173 7365   * Adding classe
-0000f550: 7320 746f 2070 6572 666f 726d 204d 6f6e  s to perform Mon
-0000f560: 7465 6361 726c 6f20 616e 6420 776f 7273  tecarlo and wors
-0000f570: 7420 6361 7365 2061 6e61 6c79 7369 7320  t case analysis 
-0000f580: 2854 6861 6e6b 7320 746f 2040 6d76 616e  (Thanks to @mvan
-0000f590: 7269 6574 2066 6f72 2068 6973 2073 7461  riet for his sta
-0000f5a0: 7274 696e 6720 7468 6973 292e 0d0a 2020  rting this)...  
-0000f5b0: 2020 2a20 5265 6d6f 7669 6e67 2074 6865    * Removing the
-0000f5c0: 2064 6570 7265 6361 7465 6420 4c54 5370   deprecated LTSp
-0000f5d0: 6963 655f 5261 7752 6561 642e 7079 2c20  ice_RawRead.py, 
-0000f5e0: 4c54 5370 6963 655f 5261 7757 7269 7465  LTSpice_RawWrite
-0000f5f0: 2e70 7920 616e 6420 4c54 5370 6963 6542  .py and LTSpiceB
-0000f600: 6174 6368 2e70 7920 6669 6c65 7320 616e  atch.py files an
-0000f610: 6420 7265 7370 6563 7469 7665 2063 6c61  d respective cla
-0000f620: 7373 6573 2e0d 0a20 2020 202a 2052 6573  sses...    * Res
-0000f630: 7472 7563 7475 7265 6420 7468 6520 666f  tructured the fo
-0000f640: 6c64 6572 2073 7472 7563 7475 7265 2074  lder structure t
-0000f650: 6f20 6265 206d 6f72 6520 696e 206c 696e  o be more in lin
-0000f660: 6520 7769 7468 2074 6865 2050 7974 686f  e with the Pytho
-0000f670: 6e20 7374 616e 6461 7264 732e 0d0a 2020  n standards...  
-0000f680: 2020 2a20 4164 6465 6420 616e 2045 7861    * Added an Exa
-0000f690: 6d70 6c65 7320 666f 6c64 6572 2077 6974  mples folder wit
-0000f6a0: 6820 736f 6d65 2065 7861 6d70 6c65 7320  h some examples 
-0000f6b0: 6f6e 2068 6f77 2074 6f20 7573 6520 7468  on how to use th
-0000f6c0: 6520 6c69 6272 6172 792e 0d0a 0d0a 2a20  e library.....* 
-0000f6d0: 5665 7273 696f 6e20 342e 302e 360d 0a20  Version 4.0.6.. 
-0000f6e0: 2020 202a 2046 6978 696e 6720 6973 7375     * Fixing issu
-0000f6f0: 6520 7769 7468 2074 6865 2077 7269 7465  e with the write
-0000f700: 5f6e 6574 6c69 7374 2829 2066 756e 6374  _netlist() funct
-0000f710: 696f 6e20 7768 656e 2072 6563 6569 7669  ion when receivi
-0000f720: 6e67 2061 2073 7472 696e 6720 696e 7374  ng a string inst
-0000f730: 6561 6420 6f66 2061 2070 6174 686c 6962  ead of a pathlib
-0000f740: 2e50 6174 6820 6f62 6a65 6374 2e0d 0a20  .Path object... 
-0000f750: 2020 202a 2043 6861 6e67 696e 6720 7468     * Changing th
-0000f760: 6520 7265 6775 6c61 7220 6578 7072 6573  e regular expres
-0000f770: 7369 6f6e 2066 6f72 2074 6865 2072 6573  sion for the res
-0000f780: 6973 746f 7220 696e 206f 7264 6572 2074  istor in order t
-0000f790: 6f20 6163 6365 7074 2074 6865 2052 3d20  o accept the R= 
-0000f7a0: 7072 6566 6978 206f 6e20 7468 6520 7661  prefix on the va
-0000f7b0: 6c75 6573 2e0d 0a0d 0a2a 2056 6572 7369  lues.....* Versi
-0000f7c0: 6f6e 2034 2e30 2e35 0d0a 2020 2020 2a20  on 4.0.5..    * 
-0000f7d0: 4163 6365 7074 696e 6720 6669 7865 7320  Accepting fixes 
-0000f7e0: 6672 6f6d 2061 616e 6173 2d73 6179 6564  from aanas-sayed
-0000f7f0: 4047 6974 4875 6220 7468 6174 2066 6978  @GitHub that fix
-0000f800: 6573 2069 7373 7565 7320 7769 7468 2072  es issues with r
-0000f810: 756e 6e69 6e67 2074 6865 204c 5453 7069  unning the LTSpi
-0000f820: 6365 2069 6e20 4c69 6e75 782e 0d0a 0d0a  ce in Linux.....
-0000f830: 2a20 5665 7273 696f 6e20 342e 302e 340d  * Version 4.0.4.
-0000f840: 0a20 2020 202a 2049 6d70 726f 7665 6420  .    * Improved 
-0000f850: 7573 6167 6520 6f66 2074 6865 206c 6f67  usage of the log
-0000f860: 6769 6e67 206c 6962 7261 7279 2e20 2854  ging library. (T
-0000f870: 6861 6e6b 7320 4054 5370 7265 6368 2066  hanks @TSprech f
-0000f880: 6f72 2076 6173 746c 7920 696d 7072 6f76  or vastly improv
-0000f890: 696e 6720 7468 6520 6c6f 6767 696e 6729  ing the logging)
-0000f8a0: 0d0a 2020 2020 2a20 496e 636c 7564 6564  ..    * Included
-0000f8b0: 2052 756e 5461 736b 206e 756d 6265 7220   RunTask number 
-0000f8c0: 696e 2074 6865 206c 6f67 206d 6573 7361  in the log messa
-0000f8d0: 6765 732e 0d0a 2020 2020 2a20 496e 636c  ges...    * Incl
-0000f8e0: 7564 6564 206d 696c 6c69 7365 636f 6e64  uded millisecond
-0000f8f0: 7320 696e 2074 6865 2074 696d 6520 656c  s in the time el
-0000f900: 6170 7365 6420 6361 6c63 756c 6174 696f  apsed calculatio
-0000f910: 6e2e 0d0a 0d0a 2a20 5665 7273 696f 6e20  n.....* Version 
-0000f920: 342e 302e 330d 0a20 2020 202a 2046 6978  4.0.3..    * Fix
-0000f930: 696e 6720 6973 7375 6520 696e 2065 6c61  ing issue in ela
-0000f940: 7073 6564 2074 696d 6520 6361 6c63 756c  psed time calcul
-0000f950: 6174 696f 6e2e 0d0a 2020 2020 2a20 4669  ation...    * Fi
-0000f960: 7869 6e67 2069 7373 7565 2077 6974 6820  xing issue with 
-0000f970: 7468 6520 696d 706f 7274 206f 6620 4c54  the import of LT
-0000f980: 5370 6963 654c 6f67 5265 6164 6572 2066  SpiceLogReader f
-0000f990: 726f 6d20 4c54 5374 6570 732e 7079 0d0a  rom LTSteps.py..
-0000f9a0: 0d0a 2a20 5665 7273 696f 6e20 342e 302e  ..* Version 4.0.
-0000f9b0: 320d 0a20 2020 202a 2043 6861 6e67 696e  2..    * Changin
-0000f9c0: 6720 6c69 7374 206f 6620 4c69 6272 6172  g list of Librar
-0000f9d0: 7920 6465 7065 6e64 656e 6369 6573 2e0d  y dependencies..
-0000f9e0: 0a0d 0a2a 2056 6572 7369 6f6e 2034 2e30  ...* Version 4.0
-0000f9f0: 2e31 0d0a 2020 2020 2a20 4275 6720 6669  .1..    * Bug fi
-0000fa00: 7820 6f6e 2043 4c49 2066 6f72 2074 6865  x on CLI for the
-0000fa10: 2048 6973 746f 6772 616d 2e70 7920 616e   Histogram.py an
-0000fa20: 6420 4c54 5374 6570 732e 7079 0d0a 0d0a  d LTSteps.py....
-0000fa30: 2a20 5665 7273 696f 6e20 342e 302e 300d  * Version 4.0.0.
-0000fa40: 0a20 2020 202a 2053 6570 6172 6174 696e  .    * Separatin
-0000fa50: 6720 7468 6520 5369 6d43 6f6d 6d61 6e64  g the SimCommand
-0000fa60: 6572 2069 6e74 6f20 7477 6f20 7365 7061  er into two sepa
-0000fa70: 7261 7465 2063 6c61 7373 6573 2c20 6f6e  rate classes, on
-0000fa80: 6520 666f 7220 7468 6520 7370 6963 6520  e for the spice 
-0000fa90: 6e65 746c 6973 7420 6564 6974 696e 6720  netlist editing 
-0000faa0: 2853 7069 6365 4564 6974 6f72 2920 616e  (SpiceEditor) an
-0000fab0: 6420 616e 6f74 6865 720d 0a20 2020 2020  d another..     
-0000fac0: 2066 6f72 2074 6865 2073 696d 756c 6174   for the simulat
-0000fad0: 696f 6e20 6578 6563 7574 696f 6e20 2853  ion execution (S
-0000fae0: 696d 5275 6e6e 6572 292e 0d0a 2020 2020  imRunner)...    
-0000faf0: 2a20 496d 706c 656d 656e 7469 6e67 2073  * Implementing s
-0000fb00: 696d 756c 6174 696f 6e20 7365 7276 6572  imulation server
-0000fb10: 2074 6f20 616c 6c6f 7720 666f 7220 7265   to allow for re
-0000fb20: 6d6f 7465 2073 696d 756c 6174 696f 6e20  mote simulation 
-0000fb30: 6578 6563 7574 696f 6e20 616e 6420 7468  execution and th
-0000fb40: 6520 7265 7370 6563 7469 7665 2063 6c69  e respective cli
-0000fb50: 656e 742e 0d0a 2020 2020 2a20 5375 7070  ent...    * Supp
-0000fb60: 6f72 7469 6e67 2057 6967 676c 6572 2065  orting Wiggler e
-0000fb70: 6c65 6d65 6e74 2069 6e20 7468 6520 6e65  lement in the ne
-0000fb80: 7720 4c54 5370 6963 6558 5649 492e 0d0a  w LTSpiceXVII...
-0000fb90: 2020 2020 2a20 5265 6e61 6d69 6e67 2061      * Renaming a
-0000fba0: 6c6c 2066 696c 6573 2069 6e74 6f20 6c6f  ll files into lo
-0000fbb0: 7765 7263 6173 652e 0d0a 2020 2020 2a20  wercase...    * 
-0000fbc0: 4372 6561 7469 6e67 2045 7272 6f72 2063  Creating Error c
-0000fbd0: 6c61 7373 6573 2066 6f72 2062 6574 7465  lasses for bette
-0000fbe0: 7220 6572 726f 7220 6861 6e64 6c69 6e67  r error handling
-0000fbf0: 2e0d 0a20 2020 202a 2041 6464 696e 6720  ...    * Adding 
-0000fc00: 7375 7070 6f72 7420 666f 7220 6f74 6865  support for othe
-0000fc10: 7220 7369 6d75 6c61 746f 7273 2028 6578  r simulators (ex
-0000fc20: 3a20 6e67 7370 6963 6529 2077 6865 7265  : ngspice) where
-0000fc30: 2074 6865 2073 696d 756c 6174 6f72 2069   the simulator i
-0000fc40: 7320 6465 6669 6e65 6420 6279 2061 2063  s defined by a c
-0000fc50: 6c61 7373 2e20 5468 6973 0d0a 2020 2020  lass. This..    
-0000fc60: 2020 7375 7070 6f72 7420 636c 6173 7320    support class 
-0000fc70: 6e65 6564 7320 746f 2062 6520 6120 7375  needs to be a su
-0000fc80: 6263 6c61 7373 206f 6620 7468 6520 6162  bclass of the ab
-0000fc90: 7374 7261 6374 2063 6c61 7373 2053 696d  stract class Sim
-0000fca0: 756c 6174 6f72 2e0d 0a20 2020 202a 2045  ulator...    * E
-0000fcb0: 6e6f 726d 6f75 7320 696d 7072 6f76 656d  normous improvem
-0000fcc0: 656e 7420 696e 2074 6865 2064 6f63 756d  ent in the docum
-0000fcd0: 656e 7461 7469 6f6e 206f 6620 7468 6520  entation of the 
-0000fce0: 636f 6465 2e0d 0a0d 0a2a 2056 6572 7369  code.....* Versi
-0000fcf0: 6f6e 2033 2e30 0d0a 2020 2020 2a20 456c  on 3.0..    * El
-0000fd00: 696d 696e 6174 696e 6720 7468 6520 4c54  iminating the LT
-0000fd10: 5370 6963 6520 7072 6566 6978 6573 2066  Spice prefixes f
-0000fd20: 726f 6d20 6669 6c65 7320 616e 6420 636c  rom files and cl
-0000fd30: 6173 7365 732e 0d0a 2020 2020 2a20 4164  asses...    * Ad
-0000fd40: 6f70 7469 6e67 2074 6865 206c 6f77 6572  opting the lower
-0000fd50: 6361 7365 2063 6f6e 7665 6e74 696f 6e20  case convention 
-0000fd60: 666f 7220 6669 6c65 6e61 6d65 732e 0d0a  for filenames...
-0000fd70: 0d0a 2a20 5665 7273 696f 6e20 322e 332e  ..* Version 2.3.
-0000fd80: 310d 0a20 2020 202a 2042 7567 2066 6978  1..    * Bug fix
-0000fd90: 206f 6e20 7468 6520 7061 7261 6d65 7465   on the paramete
-0000fda0: 7220 7265 706c 6163 656d 656e 742e 0d0a  r replacement...
-0000fdb0: 0d0a 2a20 5665 7273 696f 6e20 322e 330d  ..* Version 2.3.
-0000fdc0: 0a20 2020 202a 2053 7570 706f 7274 696e  .    * Supportin
-0000fdd0: 6720 7468 6520 6372 6561 7469 6f6e 206f  g the creation o
-0000fde0: 6620 5241 5720 4e6f 6973 6520 416e 616c  f RAW Noise Anal
-0000fdf0: 7973 6973 0d0a 2020 2020 2a20 4275 6720  ysis..    * Bug 
-0000fe00: 4669 7865 7320 2853 6565 2047 6974 4875  Fixes (See GitHu
-0000fe10: 6220 4c6f 6729 0d0a 0d0a 2a20 5665 7273  b Log)....* Vers
-0000fe20: 696f 6e20 322e 320d 0a20 2020 202a 204d  ion 2.2..    * M
-0000fe30: 616b 696e 6720 6e75 6d70 7920 6173 2061  aking numpy as a
-0000fe40: 2072 6571 7569 7265 6d65 6e74 2061 6e64   requirement and
-0000fe50: 2065 6c69 6d69 6e61 7469 6e67 2061 6c6c   eliminating all
-0000fe60: 2063 6f64 6520 7468 6174 2061 766f 6964   code that avoid
-0000fe70: 6564 2074 6865 2075 7365 206f 6620 6e75  ed the use of nu
-0000fe80: 6d70 790d 0a20 2020 202a 2055 7369 6e67  mpy..    * Using
-0000fe90: 206e 6577 2070 6163 6b61 6769 6e67 2074   new packaging t
-0000fea0: 6f6f 6c0d 0a20 2020 202a 2046 6978 6573  ool..    * Fixes
-0000feb0: 206f 6e20 7468 6520 4c54 5370 6963 655f   on the LTSpice_
-0000fec0: 5261 7757 7269 7465 0d0a 2020 2020 2a20  RawWrite..    * 
-0000fed0: 4669 7865 7320 696e 2074 6865 2068 616e  Fixes in the han
-0000fee0: 646c 696e 6720 6f66 2073 7465 7070 6564  dling of stepped
-0000fef0: 206f 7065 7261 7469 6e67 2070 6f69 6e74   operating point
-0000ff00: 2073 696d 756c 6174 696f 6e73 0d0a 0d0a   simulations....
-0000ff10: 2a20 5665 7273 696f 6e20 322e 310d 0a20  * Version 2.1.. 
-0000ff20: 2020 202a 2041 646f 7074 696e 6720 6d69     * Adopting mi
-0000ff30: 6e69 6d75 6d20 7079 7468 6f6e 2076 6572  nimum python ver
-0000ff40: 7369 6f6e 2033 2e37 0d0a 2020 2020 2a20  sion 3.7..    * 
-0000ff50: 5374 6172 7469 6e67 2074 6f20 7573 6520  Starting to use 
-0000ff60: 756e 6974 2074 6573 7473 2074 6f20 7661  unit tests to va
-0000ff70: 6c69 6461 7465 2061 6c6c 206d 6f64 756c  lidate all modul
-0000ff80: 6573 2061 6e64 2069 6d70 726f 7669 6e67  es and improving
-0000ff90: 2074 6573 7462 656e 6368 6573 0d0a 2020   testbenches..  
-0000ffa0: 2020 2a20 436f 6d70 6174 6962 696c 6974    * Compatibilit
-0000ffb0: 7920 7769 7468 204e 4753 7069 6365 0d0a  y with NGSpice..
-0000ffc0: 2020 2020 2a20 4176 6f69 6469 6e67 2074      * Avoiding t
-0000ffd0: 6865 2075 7365 206f 6620 7365 7475 702e  he use of setup.
-0000ffe0: 7079 2061 7320 7065 7220 5045 5035 3137  py as per PEP517
-0000fff0: 2061 6e64 2050 4550 3531 380d 0a20 2020   and PEP518..   
-00010000: 202a 2042 7567 2046 6978 6573 2028 5365   * Bug Fixes (Se
-00010010: 6520 4769 7448 7562 206c 6f67 2066 6f72  e GitHub log for
-00010020: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-00010030: 6e29 0d0a 2020 2020 2a20 496d 7072 6f76  n)..    * Improv
-00010040: 656d 656e 7473 206f 6e20 7468 6520 6d61  ements on the ma
-00010050: 6e61 6765 6d65 6e74 206f 6620 7374 6570  nagement of step
-00010060: 7065 6420 6461 7461 2069 6e20 7468 6520  ped data in the 
-00010070: 4c54 5370 6963 655f 5261 7752 6561 642e  LTSpice_RawRead.
-00010080: 7079 0d0a 0d0a 2a20 5665 7273 696f 6e20  py....* Version 
-00010090: 322e 302e 320d 0a20 2020 202a 2049 6d70  2.0.2..    * Imp
-000100a0: 726f 7665 6d65 6e74 7320 6f6e 2045 6e63  rovements on Enc
-000100b0: 6f64 696e 6720 6465 7465 6374 696f 6e0d  oding detection.
-000100c0: 0a0d 0a2a 2056 6572 7369 6f6e 2032 2e30  ...* Version 2.0
-000100d0: 0d0a 2020 2020 2a20 496e 7465 726e 6174  ..    * Internat
-000100e0: 696f 6e61 6c20 5375 7070 6f72 7420 7573  ional Support us
-000100f0: 696e 6720 7468 6520 636f 7272 6563 7420  ing the correct 
-00010100: 656e 636f 6469 6e67 2077 6865 6e20 6c6f  encoding when lo
-00010110: 6164 696e 6720 6c6f 6720 6669 6c65 732e  ading log files.
-00010120: 0d0a 2020 2020 2a20 436f 6465 204f 7074  ..    * Code Opt
-00010130: 696d 697a 6174 696f 6e73 206f 6e20 7468  imizations on th
-00010140: 6520 4c54 5370 6963 655f 5261 7752 6561  e LTSpice_RawRea
-00010150: 6465 7220 7468 6174 2061 6c6c 6f77 2066  der that allow f
-00010160: 6173 7465 7220 6461 7461 206c 6f61 6469  aster data loadi
-00010170: 6e67 2e0d 0a20 2020 202a 2049 6d70 726f  ng...    * Impro
-00010180: 7669 6e67 2074 6865 2066 756e 6374 696f  ving the functio
-00010190: 6e61 6c69 7479 206f 6e20 7468 6520 4c54  nality on the LT
-000101a0: 5370 6963 655f 5261 7757 7269 7465 722e  Spice_RawWriter.
-000101b0: 7079 0d0a 2020 2020 2a20 4164 6469 6e67  py..    * Adding
-000101c0: 2073 7570 706f 7274 2074 6f20 6564 6974   support to edit
-000101d0: 696e 6720 636f 6d70 6f6e 656e 7473 2069  ing components i
-000101e0: 6e73 6964 6520 7375 6263 6972 6375 6974  nside subcircuit
-000101f0: 7320 282e 7375 6263 6b74 290d 0a20 2020  s (.subckt)..   
-00010200: 202a 2053 7570 706f 7274 696e 6720 7265   * Supporting re
-00010210: 7369 7374 6f72 7320 7769 7468 204d 6f64  sistors with Mod
-00010220: 656c 2044 6566 696e 6974 696f 6e73 0d0a  el Definitions..
-00010230: 2020 2020 2a20 4669 7869 6e67 2070 726f      * Fixing pro
-00010240: 626c 656d 2077 6974 6820 4c54 5370 6963  blem with LTSpic
-00010250: 654c 6f67 5265 6164 6572 2074 6861 7420  eLogReader that 
-00010260: 776f 756c 6420 7265 7475 726e 206d 6573  would return mes
-00010270: 7365 6420 7570 2064 6174 610d 0a20 2020  sed up data..   
-00010280: 202a 2046 6978 696e 6720 7072 6f62 6c65   * Fixing proble
-00010290: 6d20 7769 7468 2072 6570 6c61 6369 6e67  m with replacing
-000102a0: 2074 6865 2066 696c 6520 6578 7465 6e73   the file extens
-000102b0: 696f 6e20 696e 2063 6572 7461 696e 206e  ion in certain n
-000102c0: 616d 6573 0d0a 2020 2020 2a20 436f 7272  ames..    * Corr
-000102d0: 6563 7469 6e67 2070 726f 626c 656d 2077  ecting problem w
-000102e0: 6974 6820 6465 7072 6563 6174 696f 6e73  ith deprecations
-000102f0: 206f 6e20 7468 6520 6e75 6d70 7920 6675   on the numpy fu
-00010300: 6e63 7469 6f6e 7320 7573 6564 2062 7920  nctions used by 
-00010310: 7468 6520 4869 7374 6f67 7261 6d2e 7079  the Histogram.py
-00010320: 0d0a 2020 2020 2a20 4164 6469 6e67 2062  ..    * Adding b
-00010330: 6163 6b20 7468 6520 5245 4144 4d45 2e6d  ack the README.m
-00010340: 6420 7468 6174 2073 6f6d 6568 6f77 2077  d that somehow w
-00010350: 6173 2064 656c 6574 6564 0d0a 0d0a 2a20  as deleted....* 
-00010360: 5665 7273 696f 6e20 312e 390d 0a20 2020  Version 1.9..   
-00010370: 202a 2041 6464 696e 6720 7375 7070 6f72   * Adding suppor
-00010380: 7420 666f 7220 c2b5 2063 6861 7261 6374  t for .. charact
-00010390: 6572 2069 6e20 7468 6520 5370 6963 6545  er in the SpiceE
-000103a0: 6469 746f 722e 0d0a 2020 2020 2a20 4164  ditor...    * Ad
-000103b0: 6469 6e67 2067 6574 5f63 6f6d 706f 6e65  ding get_compone
-000103c0: 6e74 5f66 6c6f 6174 7661 6c75 6528 2920  nt_floatvalue() 
-000103d0: 6d65 7468 6f64 2069 6e20 7468 6520 6e65  method in the ne
-000103e0: 746c 6973 7420 6d61 6e69 7075 6c61 7469  tlist manipulati
-000103f0: 6e67 2063 6c61 7373 2074 6861 7420 6861  ng class that ha
-00010400: 6e64 6c65 7320 7468 6520 636f 6e76 6572  ndles the conver
-00010410: 7369 6f6e 206f 6620 6e75 6d65 7269 630d  sion of numeric.
-00010420: 0a20 2020 2020 2066 6965 6c64 7320 696e  .      fields in
-00010430: 746f 2061 2066 6c6f 6174 2e20 5468 6973  to a float. This
-00010440: 2066 756e 6374 696f 6e20 7461 6b65 7320   function takes 
-00010450: 696e 746f 2061 6363 6f75 6e74 2074 6865  into account the
-00010460: 2065 6e67 696e 6565 7269 6e67 2071 7561   engineering qua
-00010470: 6c69 6669 6572 7320 276b 2720 666f 7220  lifiers 'k' for 
-00010480: 6b69 6c6f 732c 2027 6d27 206f 7220 6d69  kilos, 'm' or mi
-00010490: 6c69 732c 0d0a 2020 2020 2020 2775 2720  lis,..      'u' 
-000104a0: 6f72 2027 c2b5 2720 666f 7220 6d69 6372  or '..' for micr
-000104b0: 6f6e 732c 2027 6e27 2066 6f72 206e 616e  ons, 'n' for nan
-000104c0: 6f73 2c20 2766 2720 666f 7220 6665 6d74  os, 'f' for femt
-000104d0: 6f73 2061 6e64 2027 4d65 6727 2066 6f72  os and 'Meg' for
-000104e0: 204d 6567 6173 2e0d 0a0d 0a2a 2056 6572   Megas.....* Ver
-000104f0: 7369 6f6e 2031 2e38 0d0a 2020 2020 2a20  sion 1.8..    * 
-00010500: 556e 6966 6f72 6d69 6e67 204c 6963 656e  Uniforming Licen
-00010510: 7365 2072 6566 6572 656e 6365 2061 6372  se reference acr
-00010520: 6f73 7320 6669 6c65 7320 616e 6420 696d  oss files and im
-00010530: 7072 6f76 656d 656e 7473 206f 6e20 7468  provements on th
-00010540: 6520 646f 6375 6d65 6e74 6174 696f 6e0d  e documentation.
-00010550: 0a20 2020 202a 2041 6e20 656e 6f72 6d6f  .    * An enormo
-00010560: 7573 2061 6e64 2077 686f 6c65 6865 6172  us and wholehear
-00010570: 7465 6420 7468 616e 6b73 2074 6f20 406c  ted thanks to @l
-00010580: 7068 6572 7220 666f 7220 7468 6520 696d  pherr for the im
-00010590: 7072 6f76 656d 656e 7473 2069 6e20 7468  provements in th
-000105a0: 6520 646f 6375 6d65 6e74 6174 696f 6e2e  e documentation.
-000105b0: 0d0a 2020 2020 2a20 4275 6766 6978 206f  ..    * Bugfix o
-000105c0: 6e20 7468 6520 6164 645f 4c54 7370 6963  n the add_LTspic
-000105d0: 6552 756e 436d 644c 696e 6553 7769 7463  eRunCmdLineSwitc
-000105e0: 6865 7328 2920 3b20 5375 7070 6f72 7469  hes() ; Supporti
-000105f0: 6e67 202e 7061 7261 6d20 6e61 6d65 2076  ng .param name v
-00010600: 616c 7565 2066 6f72 6d61 740d 0a20 2020  alue format..   
-00010610: 202a 2041 6c6c 6f77 696e 6720 7468 6520   * Allowing the 
-00010620: 4c54 5370 6963 6552 6177 5265 6164 2074  LTSpiceRawRead t
-00010630: 6f20 7072 6f63 6565 6420 7768 656e 2074  o proceed when t
-00010640: 6865 206c 6f67 2066 696c 6520 6361 6e27  he log file can'
-00010650: 7420 6265 2066 6f75 6e64 206f 7220 7768  t be found or wh
-00010660: 656e 2074 6865 7265 2061 7265 2070 726f  en there are pro
-00010670: 626c 656d 7320 7265 6164 696e 6720 6974  blems reading it
-00010680: 2e0d 0a2a 2056 6572 7369 6f6e 2031 2e37  ...* Version 1.7
-00010690: 0d0a 2020 2020 2a20 5275 6e6e 696e 6720  ..    * Running 
-000106a0: 696e 204c 696e 7578 2075 6e64 6572 2077  in Linux under w
-000106b0: 696e 6520 6973 206e 6f77 2070 6f73 7369  ine is now possi
-000106c0: 626c 650d 0a0d 0a2a 2056 6572 7369 6f6e  ble....* Version
-000106d0: 2031 2e36 0d0a 2020 2020 2a20 4164 6469   1.6..    * Addi
-000106e0: 6e67 204c 5453 7069 6365 5f52 6177 5772  ng LTSpice_RawWr
-000106f0: 6974 652e 2041 6464 696e 6720 646f 6375  ite. Adding docu
-00010700: 6d65 6e74 6174 696f 6e2e 0d0a 0d0a 2a20  mentation.....* 
-00010710: 5665 7273 696f 6e20 312e 350d 0a20 2020  Version 1.5..   
-00010720: 202a 2053 6d61 6c6c 2066 6978 6573 2061   * Small fixes a
-00010730: 6e64 2069 6d70 726f 7665 6d65 6e74 7320  nd improvements 
-00010740: 6f6e 2074 6865 2063 6c61 7373 2075 7361  on the class usa
-00010750: 6765 2e20 4e6f 2061 6464 6564 2066 6561  ge. No added fea
-00010760: 7475 7265 730d 0a0d 0a2a 2056 6572 7369  tures....* Versi
-00010770: 6f6e 2031 2e34 0d0a 2020 2020 2a20 4164  on 1.4..    * Ad
-00010780: 6469 6e67 2074 6865 204c 5453 7069 6365  ding the LTSpice
-00010790: 5f53 656d 6944 6576 4f70 5265 6164 6572  _SemiDevOpReader
-000107a0: 206d 6f64 756c 650d 0a20 2020 202a 2052   module..    * R
-000107b0: 652d 656e 6162 6c69 6e67 2074 6865 2048  e-enabling the H
-000107c0: 6973 746f 6772 616d 2066 756e 6374 696f  istogram functio
-000107d0: 6e73 2077 6869 6368 2077 6865 7265 2064  ns which where d
-000107e0: 6973 6162 6c65 6420 6279 206d 6973 7461  isabled by mista
-000107f0: 6b65 2e0d 0a0d 0a2a 2056 6572 7369 6f6e  ke.....* Version
-00010800: 2031 2e33 0d0a 2020 2020 2a20 4275 6720   1.3..    * Bug 
-00010810: 6669 7865 7320 6f6e 2074 6865 2053 7069  fixes on the Spi
-00010820: 6365 4564 6974 6f72 2043 6c61 7373 0d0a  ceEditor Class..
-00010830: 0d0a 2a20 5665 7273 696f 6e20 312e 320d  ..* Version 1.2.
-00010840: 0a20 2020 202a 2052 4541 444d 452e 6d64  .    * README.md
-00010850: 3a0d 0a20 2020 2020 2041 6464 696e 6720  :..      Adding 
-00010860: 6c69 6e6b 2074 6f20 7265 6164 7468 6564  link to readthed
-00010870: 6f63 7320 646f 6375 6d65 6e74 6174 696f  ocs documentatio
-00010880: 6e0d 0a20 2020 202a 2041 6c6c 2066 696c  n..    * All fil
-00010890: 6573 3a0d 0a20 2020 2020 2043 6f6d 7072  es:..      Compr
-000108a0: 6568 656e 7369 7665 2064 6f63 756d 656e  ehensive documen
-000108b0: 7461 7469 6f6e 206f 6e20 686f 7720 746f  tation on how to
-000108c0: 2075 7365 2065 6163 6820 6d6f 6475 6c65   use each module
-000108d0: 0d0a 0d0a 2a20 5665 7273 696f 6e20 312e  ....* Version 1.
-000108e0: 310d 0a20 2020 202a 2052 4541 444d 452e  1..    * README.
-000108f0: 6d64 3a0d 0a20 2020 2020 2055 7064 6174  md:..      Updat
-00010900: 6564 2074 6865 2064 6573 6372 6970 7469  ed the descripti
-00010910: 6f6e 0d0a 2020 2020 2a20 4c54 5370 6963  on..    * LTSpic
-00010920: 6542 6174 6368 2e70 793a 0d0a 2020 2020  eBatch.py:..    
-00010930: 2020 436f 7272 6563 7465 6420 7468 6520    Corrected the 
-00010940: 6e61 6d65 206f 6620 7468 6520 7265 7475  name of the retu
-00010950: 726e 6564 2072 6177 2066 696c 652e 0d0a  rned raw file...
-00010960: 2020 2020 2a20 4164 6465 6420 636f 6d6d      * Added comm
-00010970: 656e 7473 2074 6872 6f75 6768 6f75 7420  ents throughout 
-00010980: 7468 6520 636f 6465 2061 6e64 2063 6c65  the code and cle
-00010990: 616e 7570 0d0a 0d0a 2a20 5665 7273 696f  anup....* Versio
-000109a0: 6e20 312e 300d 0a20 2020 202a 204c 5453  n 1.0..    * LTS
-000109b0: 7069 6365 4261 7463 682e 7079 3a5c 0d0a  piceBatch.py:\..
-000109c0: 2020 2020 2020 496d 706c 656d 656e 7465        Implemente
-000109d0: 6420 6120 6e65 7720 6170 7072 6f61 6368  d a new approach
-000109e0: 2028 4e4f 5420 4241 434b 5741 5244 5320   (NOT BACKWARDS 
-000109f0: 434f 4d50 4154 4942 4c45 292c 2074 6861  COMPATIBLE), tha
-00010a00: 7420 6176 6f69 6473 2074 6865 2075 7361  t avoids the usa
-00010a10: 6765 206f 6620 7468 6520 7369 6d5f 7365  ge of the sim_se
-00010a20: 7474 696e 6773 2e69 6e63 2066 696c 652e  ttings.inc file.
-00010a30: 0d0a 2020 2020 2020 416e 6420 616c 6c6f  ..      And allo
-00010a40: 7773 2074 6f20 6d6f 6469 6679 206e 6f74  ws to modify not
-00010a50: 206f 6e6c 7920 7061 7261 6d65 7465 7273   only parameters
-00010a60: 2c20 6275 7420 616c 736f 206d 6f64 656c  , but also model
-00010a70: 7320 616e 6420 6576 656e 2074 6865 2073  s and even the s
-00010a80: 696d 756c 6174 696f 6e20 636f 6d6d 616e  imulation comman
-00010a90: 6473 2e0d 0a20 2020 202a 204c 5453 7069  ds...    * LTSpi
-00010aa0: 6365 5f52 6177 5265 6164 2e70 793a 5c0d  ce_RawRead.py:\.
-00010ab0: 0a20 2020 2020 2041 6464 6564 2074 6865  .      Added the
-00010ac0: 2067 6574 5f74 696d 655f 6178 6973 206d   get_time_axis m
-00010ad0: 6574 686f 6420 746f 2074 6865 2052 6177  ethod to the Raw
-00010ae0: 5265 6164 2063 6c61 7373 2074 6f20 6176  Read class to av
-00010af0: 6f69 6420 7468 6520 7072 6f62 6c65 6d73  oid the problems
-00010b00: 2077 6974 6820 6e65 6761 7469 7665 2076   with negative v
-00010b10: 616c 7565 7320 6f6e 2074 696d 6520 6178  alues on time ax
-00010b20: 6973 2c0d 0a20 2020 2020 2077 6865 6e20  is,..      when 
-00010b30: 326e 6420 6f72 6465 7220 636f 6d70 7265  2nd order compre
-00010b40: 7373 696f 6e20 6973 2065 6e61 626c 6564  ssion is enabled
-00010b50: 2069 6e20 4c54 5370 6963 652e 0d0a 2020   in LTSpice...  
-00010b60: 2020 2a20 4c54 5374 6570 732e 7079 3a5c    * LTSteps.py:\
-00010b70: 0d0a 2020 2020 2020 4d6f 6469 6669 6564  ..      Modified
-00010b80: 2074 6865 204c 5453 7465 7073 2c20 736f   the LTSteps, so
-00010b90: 2069 7420 6361 6e20 616c 736f 2072 6561   it can also rea
-00010ba0: 6420 6d65 6173 7572 656d 656e 7473 206f  d measurements o
-00010bb0: 6e20 6c6f 6720 6669 6c65 7320 7769 7468  n log files with
-00010bc0: 6f75 7420 616e 7920 7374 6570 7320 646f  out any steps do
-00010bd0: 6e65 2e0d 0a0d 0a2a 2056 6572 7369 6f6e  ne.....* Version
-00010be0: 2030 2e36 0d0a 2020 2a20 4869 7374 6f67   0.6..  * Histog
-00010bf0: 7261 6d2e 7079 206e 6f77 2068 6173 2061  ram.py now has a
-00010c00: 6e20 6f70 7469 6f6e 2074 6f20 6d61 6b65  n option to make
-00010c10: 2074 6865 2068 6973 746f 6772 616d 2064   the histogram d
-00010c20: 6972 6563 746c 7920 6672 6f6d 2076 616c  irectly from val
-00010c30: 7565 7320 7374 6f72 6564 2069 6e20 7468  ues stored in th
-00010c40: 6520 636c 6970 626f 6172 640d 0a0d 0a2a  e clipboard....*
-00010c50: 2056 6572 7369 6f6e 2030 2e35 0d0a 2020   Version 0.5..  
-00010c60: 2a20 5468 6520 4c54 5370 6963 655f 5261  * The LTSpice_Ra
-00010c70: 7752 6561 6465 722e 7079 206e 6f77 2075  wReader.py now u
-00010c80: 7365 7320 7468 6520 6073 7472 7563 742e  ses the `struct.
-00010c90: 756e 7061 636b 6020 6675 6e63 7469 6f6e  unpack` function
-00010ca0: 2066 6f72 2061 2066 6173 7465 7220 6578   for a faster ex
-00010cb0: 6563 7574 696f 6e0d 0a0d 0a2a 2056 6572  ecution....* Ver
-00010cc0: 7369 6f6e 2030 2e34 0d0a 2020 2a20 4164  sion 0.4..  * Ad
-00010cd0: 6465 6420 4c54 5370 6963 6542 6174 6368  ded LTSpiceBatch
-00010ce0: 2e70 7920 746f 2074 6865 2063 6f6c 6c65  .py to the colle
-00010cf0: 6374 696f 6e20 6f66 2074 6f6f 6c73 0d0a  ction of tools..
-00010d00: 0d0a 2a20 5665 7273 696f 6e20 302e 330d  ..* Version 0.3.
-00010d10: 0a20 202a 2041 2076 6572 7369 6f6e 206f  .  * A version o
-00010d20: 6620 4c54 5374 6570 7320 7468 6174 2063  f LTSteps that c
-00010d30: 616e 2062 6520 696d 706f 7274 6564 2074  an be imported t
-00010d40: 6f20 7573 6520 696e 2061 2068 6967 6865  o use in a highe
-00010d50: 7220 6c65 7665 6c20 7363 7269 7074 0d0a  r level script..
-00010d60: 0d0a 2a20 5665 7273 696f 6e20 302e 320d  ..* Version 0.2.
-00010d70: 0a20 202a 2041 6464 696e 6720 4c54 5374  .  * Adding LTSt
-00010d80: 6570 732e 7079 2061 6e64 2048 6973 746f  eps.py and Histo
-00010d90: 6772 616d 2e70 790d 0a0d 0a2a 2056 6572  gram.py....* Ver
-00010da0: 7369 6f6e 2030 2e31 200d 0a20 202a 2046  sion 0.1 ..  * F
-00010db0: 6972 7374 2063 6f6d 6d69 7420 746f 2074  irst commit to t
-00010dc0: 6865 2062 6974 6275 636b 6574 2072 6570  he bitbucket rep
-00010dd0: 6f73 6974 6f72 792e 0d0a                 ository...
+0000ef30: 332e 300d 0a20 202a 2048 6965 7261 7263  3.0..  * Hierarc
+0000ef40: 6869 6361 6c20 5375 7070 6f72 7420 2841  hical Support (A
+0000ef50: 6c69 676e 696e 6720 7769 7468 2074 6865  ligning with the
+0000ef60: 2073 7069 6365 6c69 6220 312e 312e 3129   spicelib 1.1.1)
+0000ef70: 0d0a 2a20 5665 7273 696f 6e20 352e 322e  ..* Version 5.2.
+0000ef80: 330d 0a20 202a 2055 7064 6174 696e 6720  3..  * Updating 
+0000ef90: 6c6f 6767 6572 7320 746f 2075 7365 2074  loggers to use t
+0000efa0: 6865 2022 7370 6963 656c 6962 2220 4944  he "spicelib" ID
+0000efb0: 732e 0d0a 2020 2a20 4669 7869 6e67 2061  s...  * Fixing a
+0000efc0: 7574 6f64 6f63 2065 7272 6f72 730d 0a20  utodoc errors.. 
+0000efd0: 202a 2043 6f72 7265 6374 696e 6720 5665   * Correcting Ve
+0000efe0: 7273 696f 6e20 7265 6665 7265 6e63 6573  rsion references
+0000eff0: 0d0a 0d0a 2a20 5665 7273 696f 6e20 352e  ....* Version 5.
+0000f000: 322e 320d 0a20 202a 2046 6978 6573 206f  2.2..  * Fixes o
+0000f010: 6e20 7468 6520 756e 6974 7465 7374 7320  n the unittests 
+0000f020: 6166 7465 7220 7468 6520 7370 6963 656c  after the spicel
+0000f030: 6962 2075 7064 6174 6520 746f 2031 2e30  ib update to 1.0
+0000f040: 2e34 0d0a 0d0a 2a20 5665 7273 696f 6e20  .4....* Version 
+0000f050: 352e 322e 310d 0a20 202a 2043 6f72 7265  5.2.1..  * Corre
+0000f060: 6374 696f 6e20 6f6e 2074 6865 2072 756e  ction on the run
+0000f070: 5f6d 6f6e 7465 6361 726c 6f2e 7079 2061  _montecarlo.py a
+0000f080: 6e64 2072 756e 5f77 6f72 7374 5f63 6173  nd run_worst_cas
+0000f090: 652e 7079 2065 7861 6d70 6c65 732e 0d0a  e.py examples...
+0000f0a0: 2020 2a20 4669 7865 7320 6f6e 2074 6865    * Fixes on the
+0000f0b0: 2073 7069 6365 6c69 6220 2856 6572 7369   spicelib (Versi
+0000f0c0: 6f6e 2031 2e30 2e33 290d 0a0d 0a2a 2056  on 1.0.3)....* V
+0000f0d0: 6572 7369 6f6e 2035 2e32 0d0a 2020 2a20  ersion 5.2..  * 
+0000f0e0: 5369 6d41 6e61 6c79 7369 7320 7375 7070  SimAnalysis supp
+0000f0f0: 6f72 7469 6e67 2062 6f74 6820 5173 7069  orting both Qspi
+0000f100: 6365 2061 6e64 204c 5453 7069 6365 206c  ce and LTSpice l
+0000f110: 6f67 6669 6c65 732e 0d0a 2020 2a20 4661  ogfiles...  * Fa
+0000f120: 7374 576f 7273 7443 6173 6541 6e61 6c79  stWorstCaseAnaly
+0000f130: 7369 7320 616c 676f 7269 7468 6d20 696d  sis algorithm im
+0000f140: 706c 656d 656e 7465 640d 0a20 202a 2046  plemented..  * F
+0000f150: 6978 206f 6e20 7468 6520 6c6f 6720 7265  ix on the log re
+0000f160: 6164 696e 6720 6f66 2066 6f75 7269 6572  ading of fourier
+0000f170: 2064 6174 612e 0d0a 0d0a 2a20 5665 7273   data.....* Vers
+0000f180: 696f 6e20 352e 310d 0a20 202a 2049 6d70  ion 5.1..  * Imp
+0000f190: 6f72 7461 6e74 2042 7567 6669 7820 6f6e  ortant Bugfix on
+0000f1a0: 2074 6865 204c 5443 6f6d 706c 6578 2063   the LTComplex c
+0000f1b0: 6c61 7373 2e0d 0a20 202a 2046 6978 6573  lass...  * Fixes
+0000f1c0: 2061 6e64 2065 6e68 616e 6369 6e67 2074   and enhancing t
+0000f1d0: 6865 2061 6e61 6c79 7369 7320 746f 6f6c  he analysis tool
+0000f1e0: 6b69 742e 0d0a 2020 2a20 4465 7072 6563  kit...  * Deprec
+0000f1f0: 6174 696e 6720 5370 6963 6545 6469 746f  ating SpiceEdito
+0000f200: 722e 7772 6974 655f 6e65 746c 6973 7420  r.write_netlist 
+0000f210: 696e 2066 6176 6f75 7220 6f66 2073 6176  in favour of sav
+0000f220: 655f 6e65 746c 6973 7428 290d 0a0d 0a2a  e_netlist()....*
+0000f230: 2056 6572 7369 6f6e 2035 2e30 0d0a 2020   Version 5.0..  
+0000f240: 2a20 4d61 6b69 6e67 2074 6869 7320 6c69  * Making this li
+0000f250: 6272 6172 7920 6465 7065 6e64 656e 7420  brary dependent 
+0000f260: 6f6e 2073 7069 6365 6c69 6220 7768 696c  on spicelib whil
+0000f270: 6520 7472 7969 6e67 2074 6f20 6d61 696e  e trying to main
+0000f280: 7461 696e 2062 6163 6b77 6172 6420 636f  tain backward co
+0000f290: 6d70 6174 6962 696c 6974 7920 6173 206d  mpatibility as m
+0000f2a0: 7563 6820 6173 2070 6f73 7369 626c 652e  uch as possible.
+0000f2b0: 200d 0a20 2050 794c 5473 7069 6365 2077   ..  PyLTspice w
+0000f2c0: 696c 6c20 6265 206b 6570 7420 616c 6976  ill be kept aliv
+0000f2d0: 6520 616e 6420 6974 7320 7570 6461 7465  e and its update
+0000f2e0: 2077 696c 6c20 6265 206c 696e 6b65 6420   will be linked 
+0000f2f0: 746f 2074 6865 2073 7069 6365 6c69 622e  to the spicelib.
+0000f300: 2054 6865 206d 6169 6e20 6469 6666 6572   The main differ
+0000f310: 656e 6365 2069 7320 7468 6174 2075 7369  ence is that usi
+0000f320: 6e67 0d0a 2020 5079 4c54 7370 6963 6520  ng..  PyLTspice 
+0000f330: 7769 6c6c 2061 7665 7274 2074 6865 206e  will avert the n
+0000f340: 6565 6420 6f66 2068 6176 696e 6720 746f  eed of having to
+0000f350: 2073 656c 6563 7420 6120 7369 6d75 6c61   select a simula
+0000f360: 746f 7220 696e 2061 6c6c 2072 756e 2063  tor in all run c
+0000f370: 6f6d 6d61 6e64 732e 0d0a 0d0a 2a20 5665  ommands.....* Ve
+0000f380: 7273 696f 6e20 342e 312e 320d 0a20 202a  rsion 4.1.2..  *
+0000f390: 2041 6464 696e 6720 7375 7070 6f72 7420   Adding support 
+0000f3a0: 666f 7220 7468 6520 6e65 7720 5153 5049  for the new QSPI
+0000f3b0: 4345 2073 696d 756c 6174 6f72 0d0a 2020  CE simulator..  
+0000f3c0: 2a20 496d 7072 6f76 696e 6720 7468 6520  * Improving the 
+0000f3d0: 7469 6d65 6f75 7420 6d65 6368 616e 6973  timeout mechanis
+0000f3e0: 6d20 6f6e 2074 6865 2053 696d 5275 6e6e  m on the SimRunn
+0000f3f0: 6572 2063 6c61 7373 0d0a 2020 2a20 4d69  er class..  * Mi
+0000f400: 6e6f 7220 6275 6720 6669 7865 730d 0a0d  nor bug fixes...
+0000f410: 0a2a 2056 6572 7369 6f6e 2034 2e31 2e31  .* Version 4.1.1
+0000f420: 0d0a 2020 2a20 436f 6d70 6c65 7469 6e67  ..  * Completing
+0000f430: 2074 6865 2057 6f72 7374 2d43 6173 6520   the Worst-Case 
+0000f440: 416e 616c 7973 6973 2066 756e 6374 696f  Analysis functio
+0000f450: 6e73 2e20 4164 6469 6e67 2061 2064 6564  ns. Adding a ded
+0000f460: 6963 6174 6564 2065 7861 6d70 6c65 2066  icated example f
+0000f470: 6f72 2069 742e 0d0a 2020 2a20 5265 6661  or it...  * Refa
+0000f480: 6374 6f72 696e 6720 7468 6520 4c54 5370  ctoring the LTSp
+0000f490: 6963 654c 6f67 5265 6164 6572 2063 6c61  iceLogReader cla
+0000f4a0: 7373 2069 6e20 6f72 6465 7220 746f 2075  ss in order to u
+0000f4b0: 7365 2069 7420 6f6e 2074 6865 2041 6e61  se it on the Ana
+0000f4c0: 6c79 7369 7320 746f 6f6c 6b69 740d 0a0d  lysis toolkit...
+0000f4d0: 0a2a 2056 6572 7369 6f6e 2034 2e31 2e30  .* Version 4.1.0
+0000f4e0: 202a 2872 6571 7569 7265 7320 5079 7468   *(requires Pyth
+0000f4f0: 6f6e 2033 2e38 206f 7220 6869 6768 6572  on 3.8 or higher
+0000f500: 292a 0d0a 2020 2020 2a20 4164 6469 6e67  )*..    * Adding
+0000f510: 2061 206e 6577 2063 6c61 7373 2074 6f20   a new class to 
+0000f520: 6d61 6e69 7075 6c61 7465 2064 6972 6563  manipulate direc
+0000f530: 746c 7920 7468 6520 2e61 7363 2066 696c  tly the .asc fil
+0000f540: 6573 2e0d 0a20 2020 202a 204d 6f64 6966  es...    * Modif
+0000f550: 7969 6e67 2061 6c6c 2074 6865 206f 7468  ying all the oth
+0000f560: 6572 2063 6c61 7373 6573 2069 6e20 6f72  er classes in or
+0000f570: 6465 7220 746f 2075 7365 2074 6865 206e  der to use the n
+0000f580: 6577 2063 6c61 7373 2e0d 0a20 2020 202a  ew class...    *
+0000f590: 2041 6464 696e 6720 636c 6173 7365 7320   Adding classes 
+0000f5a0: 746f 2070 6572 666f 726d 204d 6f6e 7465  to perform Monte
+0000f5b0: 6361 726c 6f20 616e 6420 776f 7273 7420  carlo and worst 
+0000f5c0: 6361 7365 2061 6e61 6c79 7369 7320 2854  case analysis (T
+0000f5d0: 6861 6e6b 7320 746f 2040 6d76 616e 7269  hanks to @mvanri
+0000f5e0: 6574 2066 6f72 2068 6973 2073 7461 7274  et for his start
+0000f5f0: 696e 6720 7468 6973 292e 0d0a 2020 2020  ing this)...    
+0000f600: 2a20 5265 6d6f 7669 6e67 2074 6865 2064  * Removing the d
+0000f610: 6570 7265 6361 7465 6420 4c54 5370 6963  eprecated LTSpic
+0000f620: 655f 5261 7752 6561 642e 7079 2c20 4c54  e_RawRead.py, LT
+0000f630: 5370 6963 655f 5261 7757 7269 7465 2e70  Spice_RawWrite.p
+0000f640: 7920 616e 6420 4c54 5370 6963 6542 6174  y and LTSpiceBat
+0000f650: 6368 2e70 7920 6669 6c65 7320 616e 6420  ch.py files and 
+0000f660: 7265 7370 6563 7469 7665 2063 6c61 7373  respective class
+0000f670: 6573 2e0d 0a20 2020 202a 2052 6573 7472  es...    * Restr
+0000f680: 7563 7475 7265 6420 7468 6520 666f 6c64  uctured the fold
+0000f690: 6572 2073 7472 7563 7475 7265 2074 6f20  er structure to 
+0000f6a0: 6265 206d 6f72 6520 696e 206c 696e 6520  be more in line 
+0000f6b0: 7769 7468 2074 6865 2050 7974 686f 6e20  with the Python 
+0000f6c0: 7374 616e 6461 7264 732e 0d0a 2020 2020  standards...    
+0000f6d0: 2a20 4164 6465 6420 616e 2045 7861 6d70  * Added an Examp
+0000f6e0: 6c65 7320 666f 6c64 6572 2077 6974 6820  les folder with 
+0000f6f0: 736f 6d65 2065 7861 6d70 6c65 7320 6f6e  some examples on
+0000f700: 2068 6f77 2074 6f20 7573 6520 7468 6520   how to use the 
+0000f710: 6c69 6272 6172 792e 0d0a 0d0a 2a20 5665  library.....* Ve
+0000f720: 7273 696f 6e20 342e 302e 360d 0a20 2020  rsion 4.0.6..   
+0000f730: 202a 2046 6978 696e 6720 6973 7375 6520   * Fixing issue 
+0000f740: 7769 7468 2074 6865 2077 7269 7465 5f6e  with the write_n
+0000f750: 6574 6c69 7374 2829 2066 756e 6374 696f  etlist() functio
+0000f760: 6e20 7768 656e 2072 6563 6569 7669 6e67  n when receiving
+0000f770: 2061 2073 7472 696e 6720 696e 7374 6561   a string instea
+0000f780: 6420 6f66 2061 2070 6174 686c 6962 2e50  d of a pathlib.P
+0000f790: 6174 6820 6f62 6a65 6374 2e0d 0a20 2020  ath object...   
+0000f7a0: 202a 2043 6861 6e67 696e 6720 7468 6520   * Changing the 
+0000f7b0: 7265 6775 6c61 7220 6578 7072 6573 7369  regular expressi
+0000f7c0: 6f6e 2066 6f72 2074 6865 2072 6573 6973  on for the resis
+0000f7d0: 746f 7220 696e 206f 7264 6572 2074 6f20  tor in order to 
+0000f7e0: 6163 6365 7074 2074 6865 2052 3d20 7072  accept the R= pr
+0000f7f0: 6566 6978 206f 6e20 7468 6520 7661 6c75  efix on the valu
+0000f800: 6573 2e0d 0a0d 0a2a 2056 6572 7369 6f6e  es.....* Version
+0000f810: 2034 2e30 2e35 0d0a 2020 2020 2a20 4163   4.0.5..    * Ac
+0000f820: 6365 7074 696e 6720 6669 7865 7320 6672  cepting fixes fr
+0000f830: 6f6d 2061 616e 6173 2d73 6179 6564 4047  om aanas-sayed@G
+0000f840: 6974 4875 6220 7468 6174 2066 6978 6573  itHub that fixes
+0000f850: 2069 7373 7565 7320 7769 7468 2072 756e   issues with run
+0000f860: 6e69 6e67 2074 6865 204c 5453 7069 6365  ning the LTSpice
+0000f870: 2069 6e20 4c69 6e75 782e 0d0a 0d0a 2a20   in Linux.....* 
+0000f880: 5665 7273 696f 6e20 342e 302e 340d 0a20  Version 4.0.4.. 
+0000f890: 2020 202a 2049 6d70 726f 7665 6420 7573     * Improved us
+0000f8a0: 6167 6520 6f66 2074 6865 206c 6f67 6769  age of the loggi
+0000f8b0: 6e67 206c 6962 7261 7279 2e20 2854 6861  ng library. (Tha
+0000f8c0: 6e6b 7320 4054 5370 7265 6368 2066 6f72  nks @TSprech for
+0000f8d0: 2076 6173 746c 7920 696d 7072 6f76 696e   vastly improvin
+0000f8e0: 6720 7468 6520 6c6f 6767 696e 6729 0d0a  g the logging)..
+0000f8f0: 2020 2020 2a20 496e 636c 7564 6564 2052      * Included R
+0000f900: 756e 5461 736b 206e 756d 6265 7220 696e  unTask number in
+0000f910: 2074 6865 206c 6f67 206d 6573 7361 6765   the log message
+0000f920: 732e 0d0a 2020 2020 2a20 496e 636c 7564  s...    * Includ
+0000f930: 6564 206d 696c 6c69 7365 636f 6e64 7320  ed milliseconds 
+0000f940: 696e 2074 6865 2074 696d 6520 656c 6170  in the time elap
+0000f950: 7365 6420 6361 6c63 756c 6174 696f 6e2e  sed calculation.
+0000f960: 0d0a 0d0a 2a20 5665 7273 696f 6e20 342e  ....* Version 4.
+0000f970: 302e 330d 0a20 2020 202a 2046 6978 696e  0.3..    * Fixin
+0000f980: 6720 6973 7375 6520 696e 2065 6c61 7073  g issue in elaps
+0000f990: 6564 2074 696d 6520 6361 6c63 756c 6174  ed time calculat
+0000f9a0: 696f 6e2e 0d0a 2020 2020 2a20 4669 7869  ion...    * Fixi
+0000f9b0: 6e67 2069 7373 7565 2077 6974 6820 7468  ng issue with th
+0000f9c0: 6520 696d 706f 7274 206f 6620 4c54 5370  e import of LTSp
+0000f9d0: 6963 654c 6f67 5265 6164 6572 2066 726f  iceLogReader fro
+0000f9e0: 6d20 4c54 5374 6570 732e 7079 0d0a 0d0a  m LTSteps.py....
+0000f9f0: 2a20 5665 7273 696f 6e20 342e 302e 320d  * Version 4.0.2.
+0000fa00: 0a20 2020 202a 2043 6861 6e67 696e 6720  .    * Changing 
+0000fa10: 6c69 7374 206f 6620 4c69 6272 6172 7920  list of Library 
+0000fa20: 6465 7065 6e64 656e 6369 6573 2e0d 0a0d  dependencies....
+0000fa30: 0a2a 2056 6572 7369 6f6e 2034 2e30 2e31  .* Version 4.0.1
+0000fa40: 0d0a 2020 2020 2a20 4275 6720 6669 7820  ..    * Bug fix 
+0000fa50: 6f6e 2043 4c49 2066 6f72 2074 6865 2048  on CLI for the H
+0000fa60: 6973 746f 6772 616d 2e70 7920 616e 6420  istogram.py and 
+0000fa70: 4c54 5374 6570 732e 7079 0d0a 0d0a 2a20  LTSteps.py....* 
+0000fa80: 5665 7273 696f 6e20 342e 302e 300d 0a20  Version 4.0.0.. 
+0000fa90: 2020 202a 2053 6570 6172 6174 696e 6720     * Separating 
+0000faa0: 7468 6520 5369 6d43 6f6d 6d61 6e64 6572  the SimCommander
+0000fab0: 2069 6e74 6f20 7477 6f20 7365 7061 7261   into two separa
+0000fac0: 7465 2063 6c61 7373 6573 2c20 6f6e 6520  te classes, one 
+0000fad0: 666f 7220 7468 6520 7370 6963 6520 6e65  for the spice ne
+0000fae0: 746c 6973 7420 6564 6974 696e 6720 2853  tlist editing (S
+0000faf0: 7069 6365 4564 6974 6f72 2920 616e 6420  piceEditor) and 
+0000fb00: 616e 6f74 6865 720d 0a20 2020 2020 2066  another..      f
+0000fb10: 6f72 2074 6865 2073 696d 756c 6174 696f  or the simulatio
+0000fb20: 6e20 6578 6563 7574 696f 6e20 2853 696d  n execution (Sim
+0000fb30: 5275 6e6e 6572 292e 0d0a 2020 2020 2a20  Runner)...    * 
+0000fb40: 496d 706c 656d 656e 7469 6e67 2073 696d  Implementing sim
+0000fb50: 756c 6174 696f 6e20 7365 7276 6572 2074  ulation server t
+0000fb60: 6f20 616c 6c6f 7720 666f 7220 7265 6d6f  o allow for remo
+0000fb70: 7465 2073 696d 756c 6174 696f 6e20 6578  te simulation ex
+0000fb80: 6563 7574 696f 6e20 616e 6420 7468 6520  ecution and the 
+0000fb90: 7265 7370 6563 7469 7665 2063 6c69 656e  respective clien
+0000fba0: 742e 0d0a 2020 2020 2a20 5375 7070 6f72  t...    * Suppor
+0000fbb0: 7469 6e67 2057 6967 676c 6572 2065 6c65  ting Wiggler ele
+0000fbc0: 6d65 6e74 2069 6e20 7468 6520 6e65 7720  ment in the new 
+0000fbd0: 4c54 5370 6963 6558 5649 492e 0d0a 2020  LTSpiceXVII...  
+0000fbe0: 2020 2a20 5265 6e61 6d69 6e67 2061 6c6c    * Renaming all
+0000fbf0: 2066 696c 6573 2069 6e74 6f20 6c6f 7765   files into lowe
+0000fc00: 7263 6173 652e 0d0a 2020 2020 2a20 4372  rcase...    * Cr
+0000fc10: 6561 7469 6e67 2045 7272 6f72 2063 6c61  eating Error cla
+0000fc20: 7373 6573 2066 6f72 2062 6574 7465 7220  sses for better 
+0000fc30: 6572 726f 7220 6861 6e64 6c69 6e67 2e0d  error handling..
+0000fc40: 0a20 2020 202a 2041 6464 696e 6720 7375  .    * Adding su
+0000fc50: 7070 6f72 7420 666f 7220 6f74 6865 7220  pport for other 
+0000fc60: 7369 6d75 6c61 746f 7273 2028 6578 3a20  simulators (ex: 
+0000fc70: 6e67 7370 6963 6529 2077 6865 7265 2074  ngspice) where t
+0000fc80: 6865 2073 696d 756c 6174 6f72 2069 7320  he simulator is 
+0000fc90: 6465 6669 6e65 6420 6279 2061 2063 6c61  defined by a cla
+0000fca0: 7373 2e20 5468 6973 0d0a 2020 2020 2020  ss. This..      
+0000fcb0: 7375 7070 6f72 7420 636c 6173 7320 6e65  support class ne
+0000fcc0: 6564 7320 746f 2062 6520 6120 7375 6263  eds to be a subc
+0000fcd0: 6c61 7373 206f 6620 7468 6520 6162 7374  lass of the abst
+0000fce0: 7261 6374 2063 6c61 7373 2053 696d 756c  ract class Simul
+0000fcf0: 6174 6f72 2e0d 0a20 2020 202a 2045 6e6f  ator...    * Eno
+0000fd00: 726d 6f75 7320 696d 7072 6f76 656d 656e  rmous improvemen
+0000fd10: 7420 696e 2074 6865 2064 6f63 756d 656e  t in the documen
+0000fd20: 7461 7469 6f6e 206f 6620 7468 6520 636f  tation of the co
+0000fd30: 6465 2e0d 0a0d 0a2a 2056 6572 7369 6f6e  de.....* Version
+0000fd40: 2033 2e30 0d0a 2020 2020 2a20 456c 696d   3.0..    * Elim
+0000fd50: 696e 6174 696e 6720 7468 6520 4c54 5370  inating the LTSp
+0000fd60: 6963 6520 7072 6566 6978 6573 2066 726f  ice prefixes fro
+0000fd70: 6d20 6669 6c65 7320 616e 6420 636c 6173  m files and clas
+0000fd80: 7365 732e 0d0a 2020 2020 2a20 4164 6f70  ses...    * Adop
+0000fd90: 7469 6e67 2074 6865 206c 6f77 6572 6361  ting the lowerca
+0000fda0: 7365 2063 6f6e 7665 6e74 696f 6e20 666f  se convention fo
+0000fdb0: 7220 6669 6c65 6e61 6d65 732e 0d0a 0d0a  r filenames.....
+0000fdc0: 2a20 5665 7273 696f 6e20 322e 332e 310d  * Version 2.3.1.
+0000fdd0: 0a20 2020 202a 2042 7567 2066 6978 206f  .    * Bug fix o
+0000fde0: 6e20 7468 6520 7061 7261 6d65 7465 7220  n the parameter 
+0000fdf0: 7265 706c 6163 656d 656e 742e 0d0a 0d0a  replacement.....
+0000fe00: 2a20 5665 7273 696f 6e20 322e 330d 0a20  * Version 2.3.. 
+0000fe10: 2020 202a 2053 7570 706f 7274 696e 6720     * Supporting 
+0000fe20: 7468 6520 6372 6561 7469 6f6e 206f 6620  the creation of 
+0000fe30: 5241 5720 4e6f 6973 6520 416e 616c 7973  RAW Noise Analys
+0000fe40: 6973 0d0a 2020 2020 2a20 4275 6720 4669  is..    * Bug Fi
+0000fe50: 7865 7320 2853 6565 2047 6974 4875 6220  xes (See GitHub 
+0000fe60: 4c6f 6729 0d0a 0d0a 2a20 5665 7273 696f  Log)....* Versio
+0000fe70: 6e20 322e 320d 0a20 2020 202a 204d 616b  n 2.2..    * Mak
+0000fe80: 696e 6720 6e75 6d70 7920 6173 2061 2072  ing numpy as a r
+0000fe90: 6571 7569 7265 6d65 6e74 2061 6e64 2065  equirement and e
+0000fea0: 6c69 6d69 6e61 7469 6e67 2061 6c6c 2063  liminating all c
+0000feb0: 6f64 6520 7468 6174 2061 766f 6964 6564  ode that avoided
+0000fec0: 2074 6865 2075 7365 206f 6620 6e75 6d70   the use of nump
+0000fed0: 790d 0a20 2020 202a 2055 7369 6e67 206e  y..    * Using n
+0000fee0: 6577 2070 6163 6b61 6769 6e67 2074 6f6f  ew packaging too
+0000fef0: 6c0d 0a20 2020 202a 2046 6978 6573 206f  l..    * Fixes o
+0000ff00: 6e20 7468 6520 4c54 5370 6963 655f 5261  n the LTSpice_Ra
+0000ff10: 7757 7269 7465 0d0a 2020 2020 2a20 4669  wWrite..    * Fi
+0000ff20: 7865 7320 696e 2074 6865 2068 616e 646c  xes in the handl
+0000ff30: 696e 6720 6f66 2073 7465 7070 6564 206f  ing of stepped o
+0000ff40: 7065 7261 7469 6e67 2070 6f69 6e74 2073  perating point s
+0000ff50: 696d 756c 6174 696f 6e73 0d0a 0d0a 2a20  imulations....* 
+0000ff60: 5665 7273 696f 6e20 322e 310d 0a20 2020  Version 2.1..   
+0000ff70: 202a 2041 646f 7074 696e 6720 6d69 6e69   * Adopting mini
+0000ff80: 6d75 6d20 7079 7468 6f6e 2076 6572 7369  mum python versi
+0000ff90: 6f6e 2033 2e37 0d0a 2020 2020 2a20 5374  on 3.7..    * St
+0000ffa0: 6172 7469 6e67 2074 6f20 7573 6520 756e  arting to use un
+0000ffb0: 6974 2074 6573 7473 2074 6f20 7661 6c69  it tests to vali
+0000ffc0: 6461 7465 2061 6c6c 206d 6f64 756c 6573  date all modules
+0000ffd0: 2061 6e64 2069 6d70 726f 7669 6e67 2074   and improving t
+0000ffe0: 6573 7462 656e 6368 6573 0d0a 2020 2020  estbenches..    
+0000fff0: 2a20 436f 6d70 6174 6962 696c 6974 7920  * Compatibility 
+00010000: 7769 7468 204e 4753 7069 6365 0d0a 2020  with NGSpice..  
+00010010: 2020 2a20 4176 6f69 6469 6e67 2074 6865    * Avoiding the
+00010020: 2075 7365 206f 6620 7365 7475 702e 7079   use of setup.py
+00010030: 2061 7320 7065 7220 5045 5035 3137 2061   as per PEP517 a
+00010040: 6e64 2050 4550 3531 380d 0a20 2020 202a  nd PEP518..    *
+00010050: 2042 7567 2046 6978 6573 2028 5365 6520   Bug Fixes (See 
+00010060: 4769 7448 7562 206c 6f67 2066 6f72 206d  GitHub log for m
+00010070: 6f72 6520 696e 666f 726d 6174 696f 6e29  ore information)
+00010080: 0d0a 2020 2020 2a20 496d 7072 6f76 656d  ..    * Improvem
+00010090: 656e 7473 206f 6e20 7468 6520 6d61 6e61  ents on the mana
+000100a0: 6765 6d65 6e74 206f 6620 7374 6570 7065  gement of steppe
+000100b0: 6420 6461 7461 2069 6e20 7468 6520 4c54  d data in the LT
+000100c0: 5370 6963 655f 5261 7752 6561 642e 7079  Spice_RawRead.py
+000100d0: 0d0a 0d0a 2a20 5665 7273 696f 6e20 322e  ....* Version 2.
+000100e0: 302e 320d 0a20 2020 202a 2049 6d70 726f  0.2..    * Impro
+000100f0: 7665 6d65 6e74 7320 6f6e 2045 6e63 6f64  vements on Encod
+00010100: 696e 6720 6465 7465 6374 696f 6e0d 0a0d  ing detection...
+00010110: 0a2a 2056 6572 7369 6f6e 2032 2e30 0d0a  .* Version 2.0..
+00010120: 2020 2020 2a20 496e 7465 726e 6174 696f      * Internatio
+00010130: 6e61 6c20 5375 7070 6f72 7420 7573 696e  nal Support usin
+00010140: 6720 7468 6520 636f 7272 6563 7420 656e  g the correct en
+00010150: 636f 6469 6e67 2077 6865 6e20 6c6f 6164  coding when load
+00010160: 696e 6720 6c6f 6720 6669 6c65 732e 0d0a  ing log files...
+00010170: 2020 2020 2a20 436f 6465 204f 7074 696d      * Code Optim
+00010180: 697a 6174 696f 6e73 206f 6e20 7468 6520  izations on the 
+00010190: 4c54 5370 6963 655f 5261 7752 6561 6465  LTSpice_RawReade
+000101a0: 7220 7468 6174 2061 6c6c 6f77 2066 6173  r that allow fas
+000101b0: 7465 7220 6461 7461 206c 6f61 6469 6e67  ter data loading
+000101c0: 2e0d 0a20 2020 202a 2049 6d70 726f 7669  ...    * Improvi
+000101d0: 6e67 2074 6865 2066 756e 6374 696f 6e61  ng the functiona
+000101e0: 6c69 7479 206f 6e20 7468 6520 4c54 5370  lity on the LTSp
+000101f0: 6963 655f 5261 7757 7269 7465 722e 7079  ice_RawWriter.py
+00010200: 0d0a 2020 2020 2a20 4164 6469 6e67 2073  ..    * Adding s
+00010210: 7570 706f 7274 2074 6f20 6564 6974 696e  upport to editin
+00010220: 6720 636f 6d70 6f6e 656e 7473 2069 6e73  g components ins
+00010230: 6964 6520 7375 6263 6972 6375 6974 7320  ide subcircuits 
+00010240: 282e 7375 6263 6b74 290d 0a20 2020 202a  (.subckt)..    *
+00010250: 2053 7570 706f 7274 696e 6720 7265 7369   Supporting resi
+00010260: 7374 6f72 7320 7769 7468 204d 6f64 656c  stors with Model
+00010270: 2044 6566 696e 6974 696f 6e73 0d0a 2020   Definitions..  
+00010280: 2020 2a20 4669 7869 6e67 2070 726f 626c    * Fixing probl
+00010290: 656d 2077 6974 6820 4c54 5370 6963 654c  em with LTSpiceL
+000102a0: 6f67 5265 6164 6572 2074 6861 7420 776f  ogReader that wo
+000102b0: 756c 6420 7265 7475 726e 206d 6573 7365  uld return messe
+000102c0: 6420 7570 2064 6174 610d 0a20 2020 202a  d up data..    *
+000102d0: 2046 6978 696e 6720 7072 6f62 6c65 6d20   Fixing problem 
+000102e0: 7769 7468 2072 6570 6c61 6369 6e67 2074  with replacing t
+000102f0: 6865 2066 696c 6520 6578 7465 6e73 696f  he file extensio
+00010300: 6e20 696e 2063 6572 7461 696e 206e 616d  n in certain nam
+00010310: 6573 0d0a 2020 2020 2a20 436f 7272 6563  es..    * Correc
+00010320: 7469 6e67 2070 726f 626c 656d 2077 6974  ting problem wit
+00010330: 6820 6465 7072 6563 6174 696f 6e73 206f  h deprecations o
+00010340: 6e20 7468 6520 6e75 6d70 7920 6675 6e63  n the numpy func
+00010350: 7469 6f6e 7320 7573 6564 2062 7920 7468  tions used by th
+00010360: 6520 4869 7374 6f67 7261 6d2e 7079 0d0a  e Histogram.py..
+00010370: 2020 2020 2a20 4164 6469 6e67 2062 6163      * Adding bac
+00010380: 6b20 7468 6520 5245 4144 4d45 2e6d 6420  k the README.md 
+00010390: 7468 6174 2073 6f6d 6568 6f77 2077 6173  that somehow was
+000103a0: 2064 656c 6574 6564 0d0a 0d0a 2a20 5665   deleted....* Ve
+000103b0: 7273 696f 6e20 312e 390d 0a20 2020 202a  rsion 1.9..    *
+000103c0: 2041 6464 696e 6720 7375 7070 6f72 7420   Adding support 
+000103d0: 666f 7220 c2b5 2063 6861 7261 6374 6572  for .. character
+000103e0: 2069 6e20 7468 6520 5370 6963 6545 6469   in the SpiceEdi
+000103f0: 746f 722e 0d0a 2020 2020 2a20 4164 6469  tor...    * Addi
+00010400: 6e67 2067 6574 5f63 6f6d 706f 6e65 6e74  ng get_component
+00010410: 5f66 6c6f 6174 7661 6c75 6528 2920 6d65  _floatvalue() me
+00010420: 7468 6f64 2069 6e20 7468 6520 6e65 746c  thod in the netl
+00010430: 6973 7420 6d61 6e69 7075 6c61 7469 6e67  ist manipulating
+00010440: 2063 6c61 7373 2074 6861 7420 6861 6e64   class that hand
+00010450: 6c65 7320 7468 6520 636f 6e76 6572 7369  les the conversi
+00010460: 6f6e 206f 6620 6e75 6d65 7269 630d 0a20  on of numeric.. 
+00010470: 2020 2020 2066 6965 6c64 7320 696e 746f       fields into
+00010480: 2061 2066 6c6f 6174 2e20 5468 6973 2066   a float. This f
+00010490: 756e 6374 696f 6e20 7461 6b65 7320 696e  unction takes in
+000104a0: 746f 2061 6363 6f75 6e74 2074 6865 2065  to account the e
+000104b0: 6e67 696e 6565 7269 6e67 2071 7561 6c69  ngineering quali
+000104c0: 6669 6572 7320 276b 2720 666f 7220 6b69  fiers 'k' for ki
+000104d0: 6c6f 732c 2027 6d27 206f 7220 6d69 6c69  los, 'm' or mili
+000104e0: 732c 0d0a 2020 2020 2020 2775 2720 6f72  s,..      'u' or
+000104f0: 2027 c2b5 2720 666f 7220 6d69 6372 6f6e   '..' for micron
+00010500: 732c 2027 6e27 2066 6f72 206e 616e 6f73  s, 'n' for nanos
+00010510: 2c20 2766 2720 666f 7220 6665 6d74 6f73  , 'f' for femtos
+00010520: 2061 6e64 2027 4d65 6727 2066 6f72 204d   and 'Meg' for M
+00010530: 6567 6173 2e0d 0a0d 0a2a 2056 6572 7369  egas.....* Versi
+00010540: 6f6e 2031 2e38 0d0a 2020 2020 2a20 556e  on 1.8..    * Un
+00010550: 6966 6f72 6d69 6e67 204c 6963 656e 7365  iforming License
+00010560: 2072 6566 6572 656e 6365 2061 6372 6f73   reference acros
+00010570: 7320 6669 6c65 7320 616e 6420 696d 7072  s files and impr
+00010580: 6f76 656d 656e 7473 206f 6e20 7468 6520  ovements on the 
+00010590: 646f 6375 6d65 6e74 6174 696f 6e0d 0a20  documentation.. 
+000105a0: 2020 202a 2041 6e20 656e 6f72 6d6f 7573     * An enormous
+000105b0: 2061 6e64 2077 686f 6c65 6865 6172 7465   and wholehearte
+000105c0: 6420 7468 616e 6b73 2074 6f20 406c 7068  d thanks to @lph
+000105d0: 6572 7220 666f 7220 7468 6520 696d 7072  err for the impr
+000105e0: 6f76 656d 656e 7473 2069 6e20 7468 6520  ovements in the 
+000105f0: 646f 6375 6d65 6e74 6174 696f 6e2e 0d0a  documentation...
+00010600: 2020 2020 2a20 4275 6766 6978 206f 6e20      * Bugfix on 
+00010610: 7468 6520 6164 645f 4c54 7370 6963 6552  the add_LTspiceR
+00010620: 756e 436d 644c 696e 6553 7769 7463 6865  unCmdLineSwitche
+00010630: 7328 2920 3b20 5375 7070 6f72 7469 6e67  s() ; Supporting
+00010640: 202e 7061 7261 6d20 6e61 6d65 2076 616c   .param name val
+00010650: 7565 2066 6f72 6d61 740d 0a20 2020 202a  ue format..    *
+00010660: 2041 6c6c 6f77 696e 6720 7468 6520 4c54   Allowing the LT
+00010670: 5370 6963 6552 6177 5265 6164 2074 6f20  SpiceRawRead to 
+00010680: 7072 6f63 6565 6420 7768 656e 2074 6865  proceed when the
+00010690: 206c 6f67 2066 696c 6520 6361 6e27 7420   log file can't 
+000106a0: 6265 2066 6f75 6e64 206f 7220 7768 656e  be found or when
+000106b0: 2074 6865 7265 2061 7265 2070 726f 626c   there are probl
+000106c0: 656d 7320 7265 6164 696e 6720 6974 2e0d  ems reading it..
+000106d0: 0a2a 2056 6572 7369 6f6e 2031 2e37 0d0a  .* Version 1.7..
+000106e0: 2020 2020 2a20 5275 6e6e 696e 6720 696e      * Running in
+000106f0: 204c 696e 7578 2075 6e64 6572 2077 696e   Linux under win
+00010700: 6520 6973 206e 6f77 2070 6f73 7369 626c  e is now possibl
+00010710: 650d 0a0d 0a2a 2056 6572 7369 6f6e 2031  e....* Version 1
+00010720: 2e36 0d0a 2020 2020 2a20 4164 6469 6e67  .6..    * Adding
+00010730: 204c 5453 7069 6365 5f52 6177 5772 6974   LTSpice_RawWrit
+00010740: 652e 2041 6464 696e 6720 646f 6375 6d65  e. Adding docume
+00010750: 6e74 6174 696f 6e2e 0d0a 0d0a 2a20 5665  ntation.....* Ve
+00010760: 7273 696f 6e20 312e 350d 0a20 2020 202a  rsion 1.5..    *
+00010770: 2053 6d61 6c6c 2066 6978 6573 2061 6e64   Small fixes and
+00010780: 2069 6d70 726f 7665 6d65 6e74 7320 6f6e   improvements on
+00010790: 2074 6865 2063 6c61 7373 2075 7361 6765   the class usage
+000107a0: 2e20 4e6f 2061 6464 6564 2066 6561 7475  . No added featu
+000107b0: 7265 730d 0a0d 0a2a 2056 6572 7369 6f6e  res....* Version
+000107c0: 2031 2e34 0d0a 2020 2020 2a20 4164 6469   1.4..    * Addi
+000107d0: 6e67 2074 6865 204c 5453 7069 6365 5f53  ng the LTSpice_S
+000107e0: 656d 6944 6576 4f70 5265 6164 6572 206d  emiDevOpReader m
+000107f0: 6f64 756c 650d 0a20 2020 202a 2052 652d  odule..    * Re-
+00010800: 656e 6162 6c69 6e67 2074 6865 2048 6973  enabling the His
+00010810: 746f 6772 616d 2066 756e 6374 696f 6e73  togram functions
+00010820: 2077 6869 6368 2077 6865 7265 2064 6973   which where dis
+00010830: 6162 6c65 6420 6279 206d 6973 7461 6b65  abled by mistake
+00010840: 2e0d 0a0d 0a2a 2056 6572 7369 6f6e 2031  .....* Version 1
+00010850: 2e33 0d0a 2020 2020 2a20 4275 6720 6669  .3..    * Bug fi
+00010860: 7865 7320 6f6e 2074 6865 2053 7069 6365  xes on the Spice
+00010870: 4564 6974 6f72 2043 6c61 7373 0d0a 0d0a  Editor Class....
+00010880: 2a20 5665 7273 696f 6e20 312e 320d 0a20  * Version 1.2.. 
+00010890: 2020 202a 2052 4541 444d 452e 6d64 3a0d     * README.md:.
+000108a0: 0a20 2020 2020 2041 6464 696e 6720 6c69  .      Adding li
+000108b0: 6e6b 2074 6f20 7265 6164 7468 6564 6f63  nk to readthedoc
+000108c0: 7320 646f 6375 6d65 6e74 6174 696f 6e0d  s documentation.
+000108d0: 0a20 2020 202a 2041 6c6c 2066 696c 6573  .    * All files
+000108e0: 3a0d 0a20 2020 2020 2043 6f6d 7072 6568  :..      Compreh
+000108f0: 656e 7369 7665 2064 6f63 756d 656e 7461  ensive documenta
+00010900: 7469 6f6e 206f 6e20 686f 7720 746f 2075  tion on how to u
+00010910: 7365 2065 6163 6820 6d6f 6475 6c65 0d0a  se each module..
+00010920: 0d0a 2a20 5665 7273 696f 6e20 312e 310d  ..* Version 1.1.
+00010930: 0a20 2020 202a 2052 4541 444d 452e 6d64  .    * README.md
+00010940: 3a0d 0a20 2020 2020 2055 7064 6174 6564  :..      Updated
+00010950: 2074 6865 2064 6573 6372 6970 7469 6f6e   the description
+00010960: 0d0a 2020 2020 2a20 4c54 5370 6963 6542  ..    * LTSpiceB
+00010970: 6174 6368 2e70 793a 0d0a 2020 2020 2020  atch.py:..      
+00010980: 436f 7272 6563 7465 6420 7468 6520 6e61  Corrected the na
+00010990: 6d65 206f 6620 7468 6520 7265 7475 726e  me of the return
+000109a0: 6564 2072 6177 2066 696c 652e 0d0a 2020  ed raw file...  
+000109b0: 2020 2a20 4164 6465 6420 636f 6d6d 656e    * Added commen
+000109c0: 7473 2074 6872 6f75 6768 6f75 7420 7468  ts throughout th
+000109d0: 6520 636f 6465 2061 6e64 2063 6c65 616e  e code and clean
+000109e0: 7570 0d0a 0d0a 2a20 5665 7273 696f 6e20  up....* Version 
+000109f0: 312e 300d 0a20 2020 202a 204c 5453 7069  1.0..    * LTSpi
+00010a00: 6365 4261 7463 682e 7079 3a5c 0d0a 2020  ceBatch.py:\..  
+00010a10: 2020 2020 496d 706c 656d 656e 7465 6420      Implemented 
+00010a20: 6120 6e65 7720 6170 7072 6f61 6368 2028  a new approach (
+00010a30: 4e4f 5420 4241 434b 5741 5244 5320 434f  NOT BACKWARDS CO
+00010a40: 4d50 4154 4942 4c45 292c 2074 6861 7420  MPATIBLE), that 
+00010a50: 6176 6f69 6473 2074 6865 2075 7361 6765  avoids the usage
+00010a60: 206f 6620 7468 6520 7369 6d5f 7365 7474   of the sim_sett
+00010a70: 696e 6773 2e69 6e63 2066 696c 652e 0d0a  ings.inc file...
+00010a80: 2020 2020 2020 416e 6420 616c 6c6f 7773        And allows
+00010a90: 2074 6f20 6d6f 6469 6679 206e 6f74 206f   to modify not o
+00010aa0: 6e6c 7920 7061 7261 6d65 7465 7273 2c20  nly parameters, 
+00010ab0: 6275 7420 616c 736f 206d 6f64 656c 7320  but also models 
+00010ac0: 616e 6420 6576 656e 2074 6865 2073 696d  and even the sim
+00010ad0: 756c 6174 696f 6e20 636f 6d6d 616e 6473  ulation commands
+00010ae0: 2e0d 0a20 2020 202a 204c 5453 7069 6365  ...    * LTSpice
+00010af0: 5f52 6177 5265 6164 2e70 793a 5c0d 0a20  _RawRead.py:\.. 
+00010b00: 2020 2020 2041 6464 6564 2074 6865 2067       Added the g
+00010b10: 6574 5f74 696d 655f 6178 6973 206d 6574  et_time_axis met
+00010b20: 686f 6420 746f 2074 6865 2052 6177 5265  hod to the RawRe
+00010b30: 6164 2063 6c61 7373 2074 6f20 6176 6f69  ad class to avoi
+00010b40: 6420 7468 6520 7072 6f62 6c65 6d73 2077  d the problems w
+00010b50: 6974 6820 6e65 6761 7469 7665 2076 616c  ith negative val
+00010b60: 7565 7320 6f6e 2074 696d 6520 6178 6973  ues on time axis
+00010b70: 2c0d 0a20 2020 2020 2077 6865 6e20 326e  ,..      when 2n
+00010b80: 6420 6f72 6465 7220 636f 6d70 7265 7373  d order compress
+00010b90: 696f 6e20 6973 2065 6e61 626c 6564 2069  ion is enabled i
+00010ba0: 6e20 4c54 5370 6963 652e 0d0a 2020 2020  n LTSpice...    
+00010bb0: 2a20 4c54 5374 6570 732e 7079 3a5c 0d0a  * LTSteps.py:\..
+00010bc0: 2020 2020 2020 4d6f 6469 6669 6564 2074        Modified t
+00010bd0: 6865 204c 5453 7465 7073 2c20 736f 2069  he LTSteps, so i
+00010be0: 7420 6361 6e20 616c 736f 2072 6561 6420  t can also read 
+00010bf0: 6d65 6173 7572 656d 656e 7473 206f 6e20  measurements on 
+00010c00: 6c6f 6720 6669 6c65 7320 7769 7468 6f75  log files withou
+00010c10: 7420 616e 7920 7374 6570 7320 646f 6e65  t any steps done
+00010c20: 2e0d 0a0d 0a2a 2056 6572 7369 6f6e 2030  .....* Version 0
+00010c30: 2e36 0d0a 2020 2a20 4869 7374 6f67 7261  .6..  * Histogra
+00010c40: 6d2e 7079 206e 6f77 2068 6173 2061 6e20  m.py now has an 
+00010c50: 6f70 7469 6f6e 2074 6f20 6d61 6b65 2074  option to make t
+00010c60: 6865 2068 6973 746f 6772 616d 2064 6972  he histogram dir
+00010c70: 6563 746c 7920 6672 6f6d 2076 616c 7565  ectly from value
+00010c80: 7320 7374 6f72 6564 2069 6e20 7468 6520  s stored in the 
+00010c90: 636c 6970 626f 6172 640d 0a0d 0a2a 2056  clipboard....* V
+00010ca0: 6572 7369 6f6e 2030 2e35 0d0a 2020 2a20  ersion 0.5..  * 
+00010cb0: 5468 6520 4c54 5370 6963 655f 5261 7752  The LTSpice_RawR
+00010cc0: 6561 6465 722e 7079 206e 6f77 2075 7365  eader.py now use
+00010cd0: 7320 7468 6520 6073 7472 7563 742e 756e  s the `struct.un
+00010ce0: 7061 636b 6020 6675 6e63 7469 6f6e 2066  pack` function f
+00010cf0: 6f72 2061 2066 6173 7465 7220 6578 6563  or a faster exec
+00010d00: 7574 696f 6e0d 0a0d 0a2a 2056 6572 7369  ution....* Versi
+00010d10: 6f6e 2030 2e34 0d0a 2020 2a20 4164 6465  on 0.4..  * Adde
+00010d20: 6420 4c54 5370 6963 6542 6174 6368 2e70  d LTSpiceBatch.p
+00010d30: 7920 746f 2074 6865 2063 6f6c 6c65 6374  y to the collect
+00010d40: 696f 6e20 6f66 2074 6f6f 6c73 0d0a 0d0a  ion of tools....
+00010d50: 2a20 5665 7273 696f 6e20 302e 330d 0a20  * Version 0.3.. 
+00010d60: 202a 2041 2076 6572 7369 6f6e 206f 6620   * A version of 
+00010d70: 4c54 5374 6570 7320 7468 6174 2063 616e  LTSteps that can
+00010d80: 2062 6520 696d 706f 7274 6564 2074 6f20   be imported to 
+00010d90: 7573 6520 696e 2061 2068 6967 6865 7220  use in a higher 
+00010da0: 6c65 7665 6c20 7363 7269 7074 0d0a 0d0a  level script....
+00010db0: 2a20 5665 7273 696f 6e20 302e 320d 0a20  * Version 0.2.. 
+00010dc0: 202a 2041 6464 696e 6720 4c54 5374 6570   * Adding LTStep
+00010dd0: 732e 7079 2061 6e64 2048 6973 746f 6772  s.py and Histogr
+00010de0: 616d 2e70 790d 0a0d 0a2a 2056 6572 7369  am.py....* Versi
+00010df0: 6f6e 2030 2e31 200d 0a20 202a 2046 6972  on 0.1 ..  * Fir
+00010e00: 7374 2063 6f6d 6d69 7420 746f 2074 6865  st commit to the
+00010e10: 2062 6974 6275 636b 6574 2072 6570 6f73   bitbucket repos
+00010e20: 6974 6f72 792e 0d0a                      itory...
```

### Comparing `PyLTSpice-5.2.2/PyLTSpice.egg-info/SOURCES.txt` & `pyltspice-5.3.0/PyLTSpice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/README.md` & `pyltspice-5.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -428,14 +428,16 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](mailto:me@nunobrum.com)
 * Alternative contact : [nuno.brum@gmail.com](mailto:nuno.brum@gmail.com)
 
 ## History ##
+* Version 5.3.0
+  * Hierarchical Support (Aligning with the spicelib 1.1.1)
 * Version 5.2.3
   * Updating loggers to use the "spicelib" IDs.
   * Fixing autodoc errors
   * Correcting Version references
 
 * Version 5.2.2
   * Fixes on the unittests after the spicelib update to 1.0.4
```

### Comparing `PyLTSpice-5.2.2/examples/ltsteps_example.py` & `pyltspice-5.3.0/examples/ltsteps_example.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/examples/raw_plotting.py` & `pyltspice-5.3.0/examples/raw_plotting.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/examples/raw_write_example.py` & `pyltspice-5.3.0/examples/raw_write_example.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/examples/run_montecarlo.py` & `pyltspice-5.3.0/examples/run_montecarlo.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/examples/run_worst_case.py` & `pyltspice-5.3.0/examples/run_worst_case.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/examples/sim_runner_asc_example.py` & `pyltspice-5.3.0/examples/sim_runner_asc_example.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/examples/sim_runner_callback_example.py` & `pyltspice-5.3.0/examples/sim_runner_callback_example.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/examples/sim_runner_callback_process_example.py` & `pyltspice-5.3.0/examples/sim_runner_callback_process_example.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/examples/sim_runner_example.py` & `pyltspice-5.3.0/examples/sim_runner_example.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/examples/sim_stepper_example.py` & `pyltspice-5.3.0/examples/sim_stepper_example.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/pyproject.toml` & `pyltspice-5.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 requires = [
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 [project]
 name = "PyLTSpice"
-version = "5.2.2"
+version = "5.3.0"
 authors = [
   { name="Nuno Brum", email="me@nunobrum.com" },
 ]
 description = "A set of tools to Automate LTSpice simulations"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
 dependencies = [
-    "spicelib>=1.0.4",
+    "spicelib>=1.1.1",
 ]
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
```

### Comparing `PyLTSpice-5.2.2/unittests/sweep_iterators_unittest.py` & `pyltspice-5.3.0/unittests/sweep_iterators_unittest.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-5.2.2/unittests/test_asc_editor.py` & `pyltspice-5.3.0/unittests/test_asc_editor.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,24 @@
     os.path.abspath((os.path.dirname(os.path.abspath(__file__)) + "/../")))  # add project root to lib search path
 
 import PyLTSpice
 
 test_dir = '../examples/testfiles/' if os.path.abspath(os.curdir).endswith('unittests') else './examples/testfiles/'
 golden_dir = './golden/' if os.path.abspath(os.curdir).endswith('unittests') else './unittests/golden/'
 
+
 class ASC_Editor_Test(unittest.TestCase):
 
     def setUp(self):
-        self.edt = PyLTSpice.editor.asc_editor.AscEditor(test_dir + "DC sweep.asc")
+        self.edt = PyLTSpice.AscEditor(test_dir + "DC sweep.asc")
 
     def test_component_editing(self):
         self.assertEqual(self.edt.get_component_value('R1'), '10k', "Tested R1 Value")  # add assertion here
-        self.assertListEqual(self.edt.get_components(), ['Vin', 'R1', 'R2', 'D1'], "Tested get_components")  # add assertion here
+        self.assertListEqual(self.edt.get_components(), ['Vin', 'R1', 'R2', 'D1'],
+                             "Tested get_components")  # add assertion here
         self.edt.set_component_value('R1', '33k')
         self.edt.save_netlist(test_dir + 'test_components_output.asc')
         self.equalFiles(test_dir + 'test_components_output.asc', golden_dir + 'test_components_output.asc')
         self.assertEqual(self.edt.get_component_value('R1'), '33k', "Tested R1 Value")  # add assertion here
         self.edt.remove_component('R1')
         self.edt.save_netlist(test_dir + 'test_components_output_1.asc')
         self.equalFiles(test_dir + 'test_components_output_1.asc', golden_dir + 'test_components_output_1.asc')
```

### Comparing `PyLTSpice-5.2.2/unittests/test_pyltspice.py` & `pyltspice-5.3.0/unittests/test_pyltspice.py`

 * *Files identical despite different names*

