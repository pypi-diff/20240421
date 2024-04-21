# Comparing `tmp/spicelib-1.0.4.tar.gz` & `tmp/spicelib-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spicelib-1.0.4.tar", last modified: Sun Mar 10 15:39:02 2024, max compression
+gzip compressed data, was "spicelib-1.1.1.tar", last modified: Sun Apr 21 14:58:07 2024, max compression
```

## Comparing `spicelib-1.0.4.tar` & `spicelib-1.1.1.tar`

### file list

```diff
@@ -1,100 +1,105 @@
-drwxrwxrwx   0        0        0        0 2024-03-10 15:39:02.362154 spicelib-1.0.4/
--rw-rw-rw-   0        0        0    35823 2023-09-01 13:27:07.000000 spicelib-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      132 2024-03-10 15:30:59.000000 spicelib-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0    66231 2024-03-10 15:39:02.360150 spicelib-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    24120 2024-03-10 15:36:25.000000 spicelib-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-03-10 15:39:02.224198 spicelib-1.0.4/examples/
--rw-rw-rw-   0        0        0      798 2023-09-01 13:57:48.000000 spicelib-1.0.4/examples/ltsteps_example.py
--rw-rw-rw-   0        0        0     1142 2023-09-08 09:39:40.000000 spicelib-1.0.4/examples/ngspice_batch.py
--rw-rw-rw-   0        0        0     1708 2024-02-23 21:06:01.000000 spicelib-1.0.4/examples/qspice_example.py
--rw-rw-rw-   0        0        0     3151 2023-09-18 15:59:31.000000 spicelib-1.0.4/examples/raw_plotting.py
--rw-rw-rw-   0        0        0      486 2024-02-25 16:29:46.000000 spicelib-1.0.4/examples/raw_read_example.py
--rw-rw-rw-   0        0        0     4276 2024-02-25 14:48:43.000000 spicelib-1.0.4/examples/raw_write_example.py
--rw-rw-rw-   0        0        0     1833 2024-02-10 22:37:40.000000 spicelib-1.0.4/examples/run_fast_worst_case.py
--rw-rw-rw-   0        0        0     2693 2024-02-23 21:48:40.000000 spicelib-1.0.4/examples/run_montecarlo.py
--rw-rw-rw-   0        0        0     1910 2024-02-02 12:19:23.000000 spicelib-1.0.4/examples/run_sensitivity.py
--rw-rw-rw-   0        0        0     2794 2024-02-23 21:48:40.000000 spicelib-1.0.4/examples/run_worst_case.py
--rw-rw-rw-   0        0        0     2467 2024-02-24 15:52:27.000000 spicelib-1.0.4/examples/sim_client_example.py
--rw-rw-rw-   0        0        0     1470 2023-10-10 21:01:06.000000 spicelib-1.0.4/examples/sim_runner_asc_example.py
--rw-rw-rw-   0        0        0     2775 2023-09-08 09:39:40.000000 spicelib-1.0.4/examples/sim_runner_callback_example.py
--rw-rw-rw-   0        0        0     2732 2023-09-08 09:39:40.000000 spicelib-1.0.4/examples/sim_runner_callback_process_example.py
--rw-rw-rw-   0        0        0     1696 2023-09-08 09:39:40.000000 spicelib-1.0.4/examples/sim_runner_example.py
--rw-rw-rw-   0        0        0     2010 2023-09-08 09:39:40.000000 spicelib-1.0.4/examples/sim_server_example.py
--rw-rw-rw-   0        0        0     1253 2024-02-23 21:30:13.000000 spicelib-1.0.4/examples/sim_stepper_example.py
--rw-rw-rw-   0        0        0      379 2023-09-08 09:39:40.000000 spicelib-1.0.4/examples/spice_editor_example.py
--rw-rw-rw-   0        0        0     1714 2024-03-10 15:27:28.000000 spicelib-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-10 15:39:02.362154 spicelib-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-10 15:39:02.225197 spicelib-1.0.4/spicelib/
--rw-rw-rw-   0        0        0     1770 2023-10-10 21:31:05.000000 spicelib-1.0.4/spicelib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-10 15:39:02.257880 spicelib-1.0.4/spicelib/client_server/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.0.4/spicelib/client_server/__init__.py
--rw-rw-rw-   0        0        0    10097 2024-02-15 17:23:09.000000 spicelib-1.0.4/spicelib/client_server/sim_client.py
--rw-rw-rw-   0        0        0     8378 2024-02-16 14:22:36.000000 spicelib-1.0.4/spicelib/client_server/sim_server.py
--rw-rw-rw-   0        0        0     6097 2024-02-15 19:28:40.000000 spicelib-1.0.4/spicelib/client_server/srv_sim_runner.py
-drwxrwxrwx   0        0        0        0 2024-03-10 15:39:02.270927 spicelib-1.0.4/spicelib/editor/
--rw-rw-rw-   0        0        0      123 2023-10-15 17:22:56.000000 spicelib-1.0.4/spicelib/editor/__init__.py
--rw-rw-rw-   0        0        0    19861 2024-03-03 09:48:47.000000 spicelib-1.0.4/spicelib/editor/asc_editor.py
--rw-rw-rw-   0        0        0     9372 2024-03-09 12:38:17.000000 spicelib-1.0.4/spicelib/editor/asy_reader.py
--rw-rw-rw-   0        0        0    18608 2024-02-25 18:03:13.000000 spicelib-1.0.4/spicelib/editor/base_editor.py
--rw-rw-rw-   0        0        0    11263 2024-03-08 21:52:03.000000 spicelib-1.0.4/spicelib/editor/base_schematic.py
--rw-rw-rw-   0        0        0    26749 2024-03-09 16:54:16.000000 spicelib-1.0.4/spicelib/editor/qsch_editor.py
--rw-rw-rw-   0        0        0    47894 2024-02-25 16:04:50.000000 spicelib-1.0.4/spicelib/editor/spice_editor.py
-drwxrwxrwx   0        0        0        0 2024-03-10 15:39:02.283117 spicelib-1.0.4/spicelib/log/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.0.4/spicelib/log/__init__.py
--rw-rw-rw-   0        0        0    20952 2024-03-02 20:08:05.000000 spicelib-1.0.4/spicelib/log/logfile_data.py
--rw-rw-rw-   0        0        0    25632 2024-02-16 14:36:38.000000 spicelib-1.0.4/spicelib/log/ltsteps.py
--rw-rw-rw-   0        0        0     8183 2024-03-02 20:02:43.000000 spicelib-1.0.4/spicelib/log/qspice_log_reader.py
--rw-rw-rw-   0        0        0     6664 2023-09-01 14:14:09.000000 spicelib-1.0.4/spicelib/log/semi_dev_op_reader.py
-drwxrwxrwx   0        0        0        0 2024-03-10 15:39:02.292210 spicelib-1.0.4/spicelib/raw/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.0.4/spicelib/raw/__init__.py
--rw-rw-rw-   0        0        0    14833 2023-10-16 19:39:04.000000 spicelib-1.0.4/spicelib/raw/raw_classes.py
--rw-rw-rw-   0        0        0     6197 2023-09-01 23:08:42.000000 spicelib-1.0.4/spicelib/raw/raw_convert.py
--rw-rw-rw-   0        0        0    42506 2024-02-10 22:37:40.000000 spicelib-1.0.4/spicelib/raw/raw_read.py
--rw-rw-rw-   0        0        0    17368 2023-09-01 14:14:09.000000 spicelib-1.0.4/spicelib/raw/raw_write.py
-drwxrwxrwx   0        0        0        0 2024-03-10 15:39:02.305351 spicelib-1.0.4/spicelib/scripts/
--rw-rw-rw-   0        0        0     9136 2024-03-09 16:05:05.000000 spicelib-1.0.4/spicelib/scripts/asc_to_qsch.py
--rw-rw-rw-   0        0        0     5654 2024-03-09 13:11:41.000000 spicelib-1.0.4/spicelib/scripts/asc_to_qsch_data.xml
--rw-rw-rw-   0        0        0    12540 2024-02-23 01:33:50.000000 spicelib-1.0.4/spicelib/scripts/histogram.py
--rw-rw-rw-   0        0        0     7460 2024-02-16 14:36:38.000000 spicelib-1.0.4/spicelib/scripts/ltsteps.py
--rw-rw-rw-   0        0        0     4479 2023-09-01 22:58:58.000000 spicelib-1.0.4/spicelib/scripts/rawplot.py
--rw-rw-rw-   0        0        0     3025 2024-02-24 16:53:21.000000 spicelib-1.0.4/spicelib/scripts/readme_update.py
--rw-rw-rw-   0        0        0     4295 2024-02-15 10:43:01.000000 spicelib-1.0.4/spicelib/scripts/run_server.py
-drwxrwxrwx   0        0        0        0 2024-03-10 15:39:02.315802 spicelib-1.0.4/spicelib/sim/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.0.4/spicelib/sim/__init__.py
--rw-rw-rw-   0        0        0     2205 2023-09-08 09:39:40.000000 spicelib-1.0.4/spicelib/sim/process_callback.py
--rw-rw-rw-   0        0        0     8337 2024-02-10 22:37:40.000000 spicelib-1.0.4/spicelib/sim/run_task.py
--rw-rw-rw-   0        0        0    28813 2024-02-16 14:36:38.000000 spicelib-1.0.4/spicelib/sim/sim_runner.py
--rw-rw-rw-   0        0        0    10216 2023-10-19 12:50:05.000000 spicelib-1.0.4/spicelib/sim/sim_stepping.py
--rw-rw-rw-   0        0        0     5757 2023-11-03 11:50:22.000000 spicelib-1.0.4/spicelib/sim/simulator.py
-drwxrwxrwx   0        0        0        0 2024-03-10 15:39:02.331809 spicelib-1.0.4/spicelib/sim/tookit/
--rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.0.4/spicelib/sim/tookit/__init__.py
--rw-rw-rw-   0        0        0     4800 2023-10-19 16:51:29.000000 spicelib-1.0.4/spicelib/sim/tookit/failure_modes.py
--rw-rw-rw-   0        0        0    14582 2024-02-15 19:51:50.000000 spicelib-1.0.4/spicelib/sim/tookit/fast_worst_case.py
--rw-rw-rw-   0        0        0    12645 2024-03-09 16:55:25.000000 spicelib-1.0.4/spicelib/sim/tookit/montecarlo.py
--rw-rw-rw-   0        0        0    10260 2024-02-15 19:49:53.000000 spicelib-1.0.4/spicelib/sim/tookit/quick_sensitivity_analysis.py
--rw-rw-rw-   0        0        0     9616 2024-02-15 09:14:53.000000 spicelib-1.0.4/spicelib/sim/tookit/sim_analysis.py
--rw-rw-rw-   0        0        0    13777 2024-02-15 19:48:44.000000 spicelib-1.0.4/spicelib/sim/tookit/tolerance_deviations.py
--rw-rw-rw-   0        0        0    13523 2024-02-15 19:49:32.000000 spicelib-1.0.4/spicelib/sim/tookit/worst_case.py
-drwxrwxrwx   0        0        0        0 2024-03-10 15:39:02.342067 spicelib-1.0.4/spicelib/simulators/
--rw-rw-rw-   0        0        0        0 2023-09-08 09:39:40.000000 spicelib-1.0.4/spicelib/simulators/__init__.py
--rw-rw-rw-   0        0        0    10327 2024-02-10 22:37:40.000000 spicelib-1.0.4/spicelib/simulators/ltspice_simulator.py
--rw-rw-rw-   0        0        0     5355 2023-10-08 21:40:06.000000 spicelib-1.0.4/spicelib/simulators/ngspice_simulator.py
--rw-rw-rw-   0        0        0     6026 2023-11-03 11:49:49.000000 spicelib-1.0.4/spicelib/simulators/qspice_simulator.py
--rw-rw-rw-   0        0        0     8073 2023-10-08 21:40:06.000000 spicelib-1.0.4/spicelib/simulators/xyce_simulator.py
-drwxrwxrwx   0        0        0        0 2024-03-10 15:39:02.345548 spicelib-1.0.4/spicelib/utils/
--rw-rw-rw-   0        0        0     3811 2024-02-10 22:37:40.000000 spicelib-1.0.4/spicelib/utils/detect_encoding.py
--rw-rw-rw-   0        0        0     8101 2023-10-01 12:37:22.000000 spicelib-1.0.4/spicelib/utils/sweep_iterators.py
-drwxrwxrwx   0        0        0        0 2024-03-10 15:39:02.359149 spicelib-1.0.4/spicelib.egg-info/
--rw-rw-rw-   0        0        0    66231 2024-03-10 15:39:02.000000 spicelib-1.0.4/spicelib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2604 2024-03-10 15:39:02.000000 spicelib-1.0.4/spicelib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-10 15:39:02.000000 spicelib-1.0.4/spicelib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      330 2024-03-10 15:39:02.000000 spicelib-1.0.4/spicelib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2024-03-10 15:39:02.000000 spicelib-1.0.4/spicelib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       43 2024-03-10 15:39:02.000000 spicelib-1.0.4/spicelib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-10 15:39:02.356144 spicelib-1.0.4/unittests/
--rw-rw-rw-   0        0        0     4093 2023-09-01 21:04:13.000000 spicelib-1.0.4/unittests/sweep_iterators_unittest.py
--rw-rw-rw-   0        0        0     4856 2024-02-11 08:24:38.000000 spicelib-1.0.4/unittests/test_asc_editor.py
--rw-rw-rw-   0        0        0     6051 2024-02-11 22:28:55.000000 spicelib-1.0.4/unittests/test_qsch_editor.py
--rw-rw-rw-   0        0        0    20949 2023-10-19 22:15:33.000000 spicelib-1.0.4/unittests/test_qspice_rawread.py
--rw-rw-rw-   0        0        0     4865 2023-10-19 13:29:57.000000 spicelib-1.0.4/unittests/test_spice_editor.py
--rw-rw-rw-   0        0        0    22921 2024-02-10 22:37:40.000000 spicelib-1.0.4/unittests/test_spicelib.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.469311 spicelib-1.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-09-01 13:27:07.000000 spicelib-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      132 2024-03-10 15:30:59.000000 spicelib-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    67351 2024-04-21 14:58:07.469311 spicelib-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    25240 2024-04-21 13:17:00.000000 spicelib-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.212540 spicelib-1.1.1/examples/
+-rw-rw-rw-   0        0        0      798 2023-09-01 13:57:48.000000 spicelib-1.1.1/examples/ltsteps_example.py
+-rw-rw-rw-   0        0        0     1142 2023-09-08 09:39:40.000000 spicelib-1.1.1/examples/ngspice_batch.py
+-rw-rw-rw-   0        0        0     1708 2024-02-23 21:06:01.000000 spicelib-1.1.1/examples/qspice_example.py
+-rw-rw-rw-   0        0        0     3151 2023-09-18 15:59:31.000000 spicelib-1.1.1/examples/raw_plotting.py
+-rw-rw-rw-   0        0        0      486 2024-02-25 16:29:46.000000 spicelib-1.1.1/examples/raw_read_example.py
+-rw-rw-rw-   0        0        0     4276 2024-02-25 14:48:43.000000 spicelib-1.1.1/examples/raw_write_example.py
+-rw-rw-rw-   0        0        0     1833 2024-02-10 22:37:40.000000 spicelib-1.1.1/examples/run_fast_worst_case.py
+-rw-rw-rw-   0        0        0     2673 2024-03-16 10:43:35.000000 spicelib-1.1.1/examples/run_montecarlo.py
+-rw-rw-rw-   0        0        0     1910 2024-02-02 12:19:23.000000 spicelib-1.1.1/examples/run_sensitivity.py
+-rw-rw-rw-   0        0        0     2812 2024-04-21 13:17:00.000000 spicelib-1.1.1/examples/run_worst_case.py
+-rw-rw-rw-   0        0        0     2464 2024-03-16 10:41:24.000000 spicelib-1.1.1/examples/sim_client_example.py
+-rw-rw-rw-   0        0        0     1479 2024-03-16 10:24:39.000000 spicelib-1.1.1/examples/sim_runner_asc_example.py
+-rw-rw-rw-   0        0        0     2867 2024-04-21 13:16:18.000000 spicelib-1.1.1/examples/sim_runner_callback_example.py
+-rw-rw-rw-   0        0        0     2732 2023-09-08 09:39:40.000000 spicelib-1.1.1/examples/sim_runner_callback_process_example.py
+-rw-rw-rw-   0        0        0     1705 2024-03-16 10:24:39.000000 spicelib-1.1.1/examples/sim_runner_example.py
+-rw-rw-rw-   0        0        0     2010 2023-09-08 09:39:40.000000 spicelib-1.1.1/examples/sim_server_example.py
+-rw-rw-rw-   0        0        0     1253 2024-02-23 21:30:13.000000 spicelib-1.1.1/examples/sim_stepper_example.py
+-rw-rw-rw-   0        0        0      379 2023-09-08 09:39:40.000000 spicelib-1.1.1/examples/spice_editor_example.py
+-rw-rw-rw-   0        0        0     1280 2024-04-21 13:16:18.000000 spicelib-1.1.1/examples/sub_circuit_asc_edits.py
+-rw-rw-rw-   0        0        0     1302 2024-04-21 13:16:18.000000 spicelib-1.1.1/examples/sub_circuit_edits.py
+-rw-rw-rw-   0        0        0     1184 2024-04-21 13:16:18.000000 spicelib-1.1.1/examples/sub_circuit_qsch_edits.py
+-rw-rw-rw-   0        0        0     1714 2024-04-21 13:16:18.000000 spicelib-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-21 14:58:07.470644 spicelib-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.221051 spicelib-1.1.1/spicelib/
+-rw-rw-rw-   0        0        0     1741 2024-03-16 10:24:39.000000 spicelib-1.1.1/spicelib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.271704 spicelib-1.1.1/spicelib/client_server/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.1/spicelib/client_server/__init__.py
+-rw-rw-rw-   0        0        0    10097 2024-02-15 17:23:09.000000 spicelib-1.1.1/spicelib/client_server/sim_client.py
+-rw-rw-rw-   0        0        0     8378 2024-02-16 14:22:36.000000 spicelib-1.1.1/spicelib/client_server/sim_server.py
+-rw-rw-rw-   0        0        0     6097 2024-02-15 19:28:40.000000 spicelib-1.1.1/spicelib/client_server/srv_sim_runner.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.288114 spicelib-1.1.1/spicelib/editor/
+-rw-rw-rw-   0        0        0      123 2023-10-15 17:22:56.000000 spicelib-1.1.1/spicelib/editor/__init__.py
+-rw-rw-rw-   0        0        0    23214 2024-04-21 13:17:00.000000 spicelib-1.1.1/spicelib/editor/asc_editor.py
+-rw-rw-rw-   0        0        0    11781 2024-04-21 13:16:18.000000 spicelib-1.1.1/spicelib/editor/asy_reader.py
+-rw-rw-rw-   0        0        0    19713 2024-04-21 13:17:00.000000 spicelib-1.1.1/spicelib/editor/base_editor.py
+-rw-rw-rw-   0        0        0    13201 2024-04-21 13:20:57.000000 spicelib-1.1.1/spicelib/editor/base_schematic.py
+-rw-rw-rw-   0        0        0    36329 2024-04-21 13:30:43.000000 spicelib-1.1.1/spicelib/editor/qsch_editor.py
+-rw-rw-rw-   0        0        0    47480 2024-04-21 13:17:00.000000 spicelib-1.1.1/spicelib/editor/spice_editor.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.299648 spicelib-1.1.1/spicelib/log/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.1/spicelib/log/__init__.py
+-rw-rw-rw-   0        0        0    20952 2024-03-02 20:08:05.000000 spicelib-1.1.1/spicelib/log/logfile_data.py
+-rw-rw-rw-   0        0        0    25636 2024-03-16 10:24:39.000000 spicelib-1.1.1/spicelib/log/ltsteps.py
+-rw-rw-rw-   0        0        0     8183 2024-03-02 20:02:43.000000 spicelib-1.1.1/spicelib/log/qspice_log_reader.py
+-rw-rw-rw-   0        0        0     6664 2023-09-01 14:14:09.000000 spicelib-1.1.1/spicelib/log/semi_dev_op_reader.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.312352 spicelib-1.1.1/spicelib/raw/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.1/spicelib/raw/__init__.py
+-rw-rw-rw-   0        0        0    14833 2023-10-16 19:39:04.000000 spicelib-1.1.1/spicelib/raw/raw_classes.py
+-rw-rw-rw-   0        0        0     6197 2023-09-01 23:08:42.000000 spicelib-1.1.1/spicelib/raw/raw_convert.py
+-rw-rw-rw-   0        0        0    42506 2024-02-10 22:37:40.000000 spicelib-1.1.1/spicelib/raw/raw_read.py
+-rw-rw-rw-   0        0        0    17368 2023-09-01 14:14:09.000000 spicelib-1.1.1/spicelib/raw/raw_write.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.354181 spicelib-1.1.1/spicelib/scripts/
+-rw-rw-rw-   0        0        0     9237 2024-04-21 13:16:18.000000 spicelib-1.1.1/spicelib/scripts/asc_to_qsch.py
+-rw-rw-rw-   0        0        0     5654 2024-03-09 13:11:41.000000 spicelib-1.1.1/spicelib/scripts/asc_to_qsch_data.xml
+-rw-rw-rw-   0        0        0    12544 2024-03-16 10:24:39.000000 spicelib-1.1.1/spicelib/scripts/histogram.py
+-rw-rw-rw-   0        0        0     7464 2024-03-16 10:24:39.000000 spicelib-1.1.1/spicelib/scripts/ltsteps.py
+-rw-rw-rw-   0        0        0     4479 2023-09-01 22:58:58.000000 spicelib-1.1.1/spicelib/scripts/rawplot.py
+-rw-rw-rw-   0        0        0     3502 2024-04-21 13:17:00.000000 spicelib-1.1.1/spicelib/scripts/readme_update.py
+-rw-rw-rw-   0        0        0     4295 2024-02-15 10:43:01.000000 spicelib-1.1.1/spicelib/scripts/run_server.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.371041 spicelib-1.1.1/spicelib/sim/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.1/spicelib/sim/__init__.py
+-rw-rw-rw-   0        0        0     2205 2023-09-08 09:39:40.000000 spicelib-1.1.1/spicelib/sim/process_callback.py
+-rw-rw-rw-   0        0        0     8337 2024-02-10 22:37:40.000000 spicelib-1.1.1/spicelib/sim/run_task.py
+-rw-rw-rw-   0        0        0    28813 2024-02-16 14:36:38.000000 spicelib-1.1.1/spicelib/sim/sim_runner.py
+-rw-rw-rw-   0        0        0    10216 2023-10-19 12:50:05.000000 spicelib-1.1.1/spicelib/sim/sim_stepping.py
+-rw-rw-rw-   0        0        0     5757 2023-11-03 11:50:22.000000 spicelib-1.1.1/spicelib/sim/simulator.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.416155 spicelib-1.1.1/spicelib/sim/tookit/
+-rw-rw-rw-   0        0        0        0 2023-09-01 13:34:50.000000 spicelib-1.1.1/spicelib/sim/tookit/__init__.py
+-rw-rw-rw-   0        0        0     4800 2023-10-19 16:51:29.000000 spicelib-1.1.1/spicelib/sim/tookit/failure_modes.py
+-rw-rw-rw-   0        0        0    14582 2024-02-15 19:51:50.000000 spicelib-1.1.1/spicelib/sim/tookit/fast_worst_case.py
+-rw-rw-rw-   0        0        0    12645 2024-03-09 16:55:25.000000 spicelib-1.1.1/spicelib/sim/tookit/montecarlo.py
+-rw-rw-rw-   0        0        0    10260 2024-02-15 19:49:53.000000 spicelib-1.1.1/spicelib/sim/tookit/quick_sensitivity_analysis.py
+-rw-rw-rw-   0        0        0     9616 2024-02-15 09:14:53.000000 spicelib-1.1.1/spicelib/sim/tookit/sim_analysis.py
+-rw-rw-rw-   0        0        0    13777 2024-02-15 19:48:44.000000 spicelib-1.1.1/spicelib/sim/tookit/tolerance_deviations.py
+-rw-rw-rw-   0        0        0    13523 2024-02-15 19:49:32.000000 spicelib-1.1.1/spicelib/sim/tookit/worst_case.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.422392 spicelib-1.1.1/spicelib/simulators/
+-rw-rw-rw-   0        0        0        0 2023-09-08 09:39:40.000000 spicelib-1.1.1/spicelib/simulators/__init__.py
+-rw-rw-rw-   0        0        0    10327 2024-02-10 22:37:40.000000 spicelib-1.1.1/spicelib/simulators/ltspice_simulator.py
+-rw-rw-rw-   0        0        0     5355 2023-10-08 21:40:06.000000 spicelib-1.1.1/spicelib/simulators/ngspice_simulator.py
+-rw-rw-rw-   0        0        0     6026 2023-11-03 11:49:49.000000 spicelib-1.1.1/spicelib/simulators/qspice_simulator.py
+-rw-rw-rw-   0        0        0     8073 2023-10-08 21:40:06.000000 spicelib-1.1.1/spicelib/simulators/xyce_simulator.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.435370 spicelib-1.1.1/spicelib/utils/
+-rw-rw-rw-   0        0        0     3811 2024-02-10 22:37:40.000000 spicelib-1.1.1/spicelib/utils/detect_encoding.py
+-rw-rw-rw-   0        0        0     1886 2024-04-21 13:16:18.000000 spicelib-1.1.1/spicelib/utils/file_search.py
+-rw-rw-rw-   0        0        0     8101 2023-10-01 12:37:22.000000 spicelib-1.1.1/spicelib/utils/sweep_iterators.py
+-rw-rw-rw-   0        0        0     1133 2024-04-21 13:16:18.000000 spicelib-1.1.1/spicelib/utils/windows_short_names.py
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.467834 spicelib-1.1.1/spicelib.egg-info/
+-rw-rw-rw-   0        0        0    67351 2024-04-21 14:58:06.000000 spicelib-1.1.1/spicelib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2771 2024-04-21 14:58:07.000000 spicelib-1.1.1/spicelib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 14:58:06.000000 spicelib-1.1.1/spicelib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      330 2024-04-21 14:58:06.000000 spicelib-1.1.1/spicelib.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2024-04-21 14:58:06.000000 spicelib-1.1.1/spicelib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       53 2024-04-21 14:58:06.000000 spicelib-1.1.1/spicelib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-21 14:58:07.465827 spicelib-1.1.1/unittests/
+-rw-rw-rw-   0        0        0     4093 2023-09-01 21:04:13.000000 spicelib-1.1.1/unittests/sweep_iterators_unittest.py
+-rw-rw-rw-   0        0        0     4856 2024-02-11 08:24:38.000000 spicelib-1.1.1/unittests/test_asc_editor.py
+-rw-rw-rw-   0        0        0     6573 2024-04-21 13:16:18.000000 spicelib-1.1.1/unittests/test_qsch_editor.py
+-rw-rw-rw-   0        0        0    20957 2024-03-16 10:24:39.000000 spicelib-1.1.1/unittests/test_qspice_rawread.py
+-rw-rw-rw-   0        0        0     4865 2023-10-19 13:29:57.000000 spicelib-1.1.1/unittests/test_spice_editor.py
+-rw-rw-rw-   0        0        0    22930 2024-03-16 10:24:39.000000 spicelib-1.1.1/unittests/test_spicelib.py
```

### Comparing `spicelib-1.0.4/LICENSE` & `spicelib-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/PKG-INFO` & `spicelib-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spicelib
-Version: 1.0.4
+Version: 1.1.1
 Summary: A set of tools to Automate Spice simulations
 Author-email: Nuno Brum <me@nunobrum.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -702,15 +702,15 @@
   * LTspice
   * NGSpice
   * QSPICE
   * Xyce
 
 ## What is contained in this repository ##
 
-* __LTSteps.py__
+* __ltsteps.exe__
   An utility that extracts from LTSpice output files data, and formats it for import in a spreadsheet, such like Excel
   or Calc.
 
 * __raw_read.py__
   A pure python class that serves to read raw files into a python class.
 
 * __raw_write.py__
@@ -731,25 +731,25 @@
 * __sim_runner.py__
   A python script that can be used to run LTSpice simulations in batch mode without having to open the LTSpice GUI.
   This in cooperation with the classes defined in spice_editor.py or asc_editor.py is useful because:
 
     - Can overcome the limitation of only stepping 3 parameters
     - Different types of simulations .TRAN .AC .NOISE can be run in a single batch
     - The RAW Files are smaller and easier to treat
-    - When used with the RawRead.py and LTSteps.py, validation of the circuit can be done automatically.
+    - When used with the RawRead.py and ltsteps.py, validation of the circuit can be done automatically.
     - Different models can be simulated in a single batch, by using the following instructions:
 
   Note: It was only tested with Windows based installations.
 
 * __Analysis Toolkit__
   A set of tools that prepare an LTSpice netlist for a Montecarlo or Worst Case Analysis. The device tolerances are set
   by the user and the netlist is updated accordingly. The netlist can then be used with the sim_runner.py to run a 
   batch of simulations or with the LTSpice GUI.
 
-* __Histogram.py__
+* __histogram.exe__
   A python script that uses numpy and matplotlib to create a histogram and calculate the sigma deviations. This is
   useful for Monte-Carlo analysis.
 
 ## How to Install ##
 
 `pip install spicelib`
 
@@ -783,15 +783,15 @@
 "TRAN - STEP.raw" and displays all steps of the "I(R1)" trace in a matplotlib plot
 
  ```python
 from spicelib import RawRead
 
 from matplotlib import pyplot as plt
 
-rawfile = RawRead("TRAN - STEP.raw")
+rawfile = RawRead("./testfiles/TRAN - STEP.raw")
 
 print(rawfile.get_trace_names())
 print(rawfile.get_raw_property())
 
 IR1 = rawfile.get_trace("I(R1)")
 x = rawfile.get_trace('time')  # Gets the time axis
 steps = rawfile.get_steps()
@@ -807,30 +807,30 @@
 ### RawWrite ###
 
 The following example writes a RAW file with a 3 milliseconds transient simulation sine with a 10kHz and a cosine with
 9.997kHz
 
  ```python
 import numpy as np
-from spicelib import RawRead, Trace, RawWrite
+from spicelib import Trace, RawWrite
 LW = RawWrite(fastacces=False)
 tx = Trace('time', np.arange(0.0, 3e-3, 997E-11))
 vy = Trace('N001', np.sin(2 * np.pi * tx.data * 10000))
 vz = Trace('N002', np.cos(2 * np.pi * tx.data * 9970))
 LW.add_trace(tx)
 LW.add_trace(vy)
 LW.add_trace(vz)
 LW.save("./testfiles/teste_snippet1.raw")
  ```
 -- in examples/raw_write_example.py [Example 1]
 
 ### SpiceEditor, AscEditor and SimRunner.py ###
 
 This module is used to launch LTSPice simulations. Results then can be processed with either the RawRead or with the
-LTSteps module to read the log file which can contain .MEAS results.
+LTSpiceLogReader module to read the log file which can contain .MEAS results.
 
 The script will firstly invoke the LTSpice in command line to generate a netlist, and then this netlist can be updated
 directly by the script, in order to change component values, parameters or simulation commands.
 
 Here follows an example of operation.
 
 ```python
@@ -862,15 +862,15 @@
         print("simulating OpAmp", opamp, "Voltage", supply_voltage)
         LTC.run(netlist)
 
 for raw, log in LTC:
     print("Raw file: %s, Log file: %s" % (raw, log))
     # do something with the data
     # raw_data = RawRead(raw)
-    # log_data = LTSteps(log)
+    # log_data = LTSpiceLogReader(log)
     # ...
 
 netlist.reset_netlist()
 netlist.add_instructions(
     "; Simulation settings",
     ".ac dec 30 10 1Meg",
     ".meas AC Gain MAX mag(V(out)) ; find the peak response and call it ""Gain""",
@@ -900,15 +900,14 @@
 ![Sallen-Key Amplifier](./doc/modules/sallenkey.png "Sallen-Key Amplifier")
 
 When performing a Monte Carlo simulation on this circuit, we need to manually modify the value of each component, 
 and then add the .step command for making several runs on the same circuit. 
 To simplify this process, the AscEditor class can be used as exemplified below:
 
 ```python
-import numpy as np
 from spicelib import AscEditor, SimRunner  # Imports the class that manipulates the asc file
 from spicelib.sim.tookit.montecarlo import Montecarlo  # Imports the Montecarlo toolkit class
 from spicelib.simulators.ltspice_simulator import LTspice
 
 sallenkey = AscEditor("./testfiles/sallenkey.asc")  # Reads the asc file into memory
 runner = SimRunner(simulator=LTspice, output_folder='./temp_mc',
                    verbose=True)  # Instantiates the runner with a temp folder set
@@ -969,15 +968,15 @@
 # wca.set_tolerance('V', 0.1)  # 10% tolerance. For Worst Case analysis, the distribution is irrelevant
 wca.set_tolerance('I', 0.1)  # 10% tolerance. For Worst Case analysis, the distribution is irrelevant
 # Some components can have a different tolerance
 wca.set_tolerance('R1', 0.05)  # 5% tolerance for R1 only. This only overrides the default tolerance for R1
 wca.set_tolerance('R4', 0.0)  # 5% tolerance for R1 only. This only overrides the default tolerance for R1
 
 # Tolerances can be set for parameters as well.
-# wca.set_parameter_deviation('Vos', 3e-4, 5e-3)
+wca.set_parameter_deviation('Vos', 3e-4, 5e-3)
 
 # Finally the netlist is saved to a file
 wca.save_netlist('./testfiles/sallenkey_wc.asc')
 ```
 -- in examples/run_worst_case.py [Example 1]
 
 When opening the created sallenkey_wc.net file, we can see that the following circuit.
@@ -996,15 +995,15 @@
 - A default value for the run parameter was added. This is useful if the .step param run is commented out.
 - The R1 tolerance is different from the other resistors. This is because the tolerance was explicitly set for R1.
 - The wc() function is added to the circuit. This function is used to calculate the worst case value for each component,
 given a tolerance value and its respective index.
 - The wc1() function is added to the circuit. This function is used to calculate the worst case value for each component,
 given a minimum and maximum value and its respective index.
 
-### LTSteps.py ###
+### ltsteps.py ###
 
 This module defines a class that can be used to parse LTSpice log files where the information about .STEP information is
 written. There are two possible usages of this module, either programmatically by importing the module and then
 accessing data through the class as exemplified here:
 
 ```python
 #!/usr/bin/env python
@@ -1096,27 +1095,39 @@
 
 This module is used to run a server that can be used to run simulations in a remote machine. The server will run in the
 background and will wait for a client to connect. The client will send a netlist to the server and the server will run
 the simulation and return the results to the client. The client on the remote machine is a script instancing the
 SimClient class. An example of its usage is shown below:
 
 ```python
+import os
+import zipfile
+import logging
+
+# In order for this, to work, you need to have a server running. To start a server, run the following command:
+# python -m spicelib.run_server --port 9000 --parallel 4 --output ./temp
+
+_logger = logging.getLogger("spicelib.SimClient")
+_logger.setLevel(logging.DEBUG)
+
 from spicelib.client_server.sim_client import SimClient
 
 server = SimClient('http://localhost', 9000)
 print(server.session_id)
 runid = server.run("./testfiles/testfile.net")
 print("Got Job id", runid)
 for runid in server:  # Ma
     zip_filename = server.get_runno_data(runid)
     print(f"Received {zip_filename} from runid {runid}")
     with zipfile.ZipFile(zip_filename, 'r') as zipf:  # Extract the contents of the zip file
         print(zipf.namelist())  # Debug printing the contents of the zip file
         zipf.extract(zipf.namelist()[0])  # Normally the raw file comes first
     os.remove(zip_filename)  # Remove the zip file
+
+server.close_session()
 ```
 -- in examples/sim_client_example.py [SimClient Example]
 
 ```bash
 usage: run_server [-h] [-p PORT] [-o OUTPUT] [-l PARALLEL] simulator
 
 Run the LTSpice Server. This is a command line interface to the SimServer class.The SimServer class is used to run
@@ -1174,14 +1185,27 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 1.1.1
+  * Supporting hierarchical edits on both QSpice and LTspice schematics
+  * Skipping the need of the rich library on examples
+  * Giving feedback on the search for symbols on the ASC to QSCH conversion
+  * Improvement on Documentation
+  * Adding examples and unittests on hiearchical edits
+  * Giving access to hidden properties (asc_file_path in AscEditor and qsch_file_path in QschEditor)
+  * Refactoring save_netlist() method in QschEditor class
+  * Supporting arcs and rectangles on AsyReader
+  * Adding file_search.py containing utility functions for searching files
+  * Adding windows_short_names.py containing a code to get the 8.3 Windows short names.
+* Version 1.1.0
+  * First usable version of a LTspice to Qspice schematic converter.
 * Version 1.0.4
   * Adding the missing the asc_to_qsch_data.xml to the package
   * Adding a MANIFEST.in to the project
   * Adding keywords to the project.toml
 * Version 1.0.3
   * Correcting the generation of a .net from the QschEditor.
 * Version 1.0.2
```

### Comparing `spicelib-1.0.4/README.md` & `spicelib-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   * LTspice
   * NGSpice
   * QSPICE
   * Xyce
 
 ## What is contained in this repository ##
 
-* __LTSteps.py__
+* __ltsteps.exe__
   An utility that extracts from LTSpice output files data, and formats it for import in a spreadsheet, such like Excel
   or Calc.
 
 * __raw_read.py__
   A pure python class that serves to read raw files into a python class.
 
 * __raw_write.py__
@@ -33,25 +33,25 @@
 * __sim_runner.py__
   A python script that can be used to run LTSpice simulations in batch mode without having to open the LTSpice GUI.
   This in cooperation with the classes defined in spice_editor.py or asc_editor.py is useful because:
 
     - Can overcome the limitation of only stepping 3 parameters
     - Different types of simulations .TRAN .AC .NOISE can be run in a single batch
     - The RAW Files are smaller and easier to treat
-    - When used with the RawRead.py and LTSteps.py, validation of the circuit can be done automatically.
+    - When used with the RawRead.py and ltsteps.py, validation of the circuit can be done automatically.
     - Different models can be simulated in a single batch, by using the following instructions:
 
   Note: It was only tested with Windows based installations.
 
 * __Analysis Toolkit__
   A set of tools that prepare an LTSpice netlist for a Montecarlo or Worst Case Analysis. The device tolerances are set
   by the user and the netlist is updated accordingly. The netlist can then be used with the sim_runner.py to run a 
   batch of simulations or with the LTSpice GUI.
 
-* __Histogram.py__
+* __histogram.exe__
   A python script that uses numpy and matplotlib to create a histogram and calculate the sigma deviations. This is
   useful for Monte-Carlo analysis.
 
 ## How to Install ##
 
 `pip install spicelib`
 
@@ -85,15 +85,15 @@
 "TRAN - STEP.raw" and displays all steps of the "I(R1)" trace in a matplotlib plot
 
  ```python
 from spicelib import RawRead
 
 from matplotlib import pyplot as plt
 
-rawfile = RawRead("TRAN - STEP.raw")
+rawfile = RawRead("./testfiles/TRAN - STEP.raw")
 
 print(rawfile.get_trace_names())
 print(rawfile.get_raw_property())
 
 IR1 = rawfile.get_trace("I(R1)")
 x = rawfile.get_trace('time')  # Gets the time axis
 steps = rawfile.get_steps()
@@ -109,30 +109,30 @@
 ### RawWrite ###
 
 The following example writes a RAW file with a 3 milliseconds transient simulation sine with a 10kHz and a cosine with
 9.997kHz
 
  ```python
 import numpy as np
-from spicelib import RawRead, Trace, RawWrite
+from spicelib import Trace, RawWrite
 LW = RawWrite(fastacces=False)
 tx = Trace('time', np.arange(0.0, 3e-3, 997E-11))
 vy = Trace('N001', np.sin(2 * np.pi * tx.data * 10000))
 vz = Trace('N002', np.cos(2 * np.pi * tx.data * 9970))
 LW.add_trace(tx)
 LW.add_trace(vy)
 LW.add_trace(vz)
 LW.save("./testfiles/teste_snippet1.raw")
  ```
 -- in examples/raw_write_example.py [Example 1]
 
 ### SpiceEditor, AscEditor and SimRunner.py ###
 
 This module is used to launch LTSPice simulations. Results then can be processed with either the RawRead or with the
-LTSteps module to read the log file which can contain .MEAS results.
+LTSpiceLogReader module to read the log file which can contain .MEAS results.
 
 The script will firstly invoke the LTSpice in command line to generate a netlist, and then this netlist can be updated
 directly by the script, in order to change component values, parameters or simulation commands.
 
 Here follows an example of operation.
 
 ```python
@@ -164,15 +164,15 @@
         print("simulating OpAmp", opamp, "Voltage", supply_voltage)
         LTC.run(netlist)
 
 for raw, log in LTC:
     print("Raw file: %s, Log file: %s" % (raw, log))
     # do something with the data
     # raw_data = RawRead(raw)
-    # log_data = LTSteps(log)
+    # log_data = LTSpiceLogReader(log)
     # ...
 
 netlist.reset_netlist()
 netlist.add_instructions(
     "; Simulation settings",
     ".ac dec 30 10 1Meg",
     ".meas AC Gain MAX mag(V(out)) ; find the peak response and call it ""Gain""",
@@ -202,15 +202,14 @@
 ![Sallen-Key Amplifier](./doc/modules/sallenkey.png "Sallen-Key Amplifier")
 
 When performing a Monte Carlo simulation on this circuit, we need to manually modify the value of each component, 
 and then add the .step command for making several runs on the same circuit. 
 To simplify this process, the AscEditor class can be used as exemplified below:
 
 ```python
-import numpy as np
 from spicelib import AscEditor, SimRunner  # Imports the class that manipulates the asc file
 from spicelib.sim.tookit.montecarlo import Montecarlo  # Imports the Montecarlo toolkit class
 from spicelib.simulators.ltspice_simulator import LTspice
 
 sallenkey = AscEditor("./testfiles/sallenkey.asc")  # Reads the asc file into memory
 runner = SimRunner(simulator=LTspice, output_folder='./temp_mc',
                    verbose=True)  # Instantiates the runner with a temp folder set
@@ -271,15 +270,15 @@
 # wca.set_tolerance('V', 0.1)  # 10% tolerance. For Worst Case analysis, the distribution is irrelevant
 wca.set_tolerance('I', 0.1)  # 10% tolerance. For Worst Case analysis, the distribution is irrelevant
 # Some components can have a different tolerance
 wca.set_tolerance('R1', 0.05)  # 5% tolerance for R1 only. This only overrides the default tolerance for R1
 wca.set_tolerance('R4', 0.0)  # 5% tolerance for R1 only. This only overrides the default tolerance for R1
 
 # Tolerances can be set for parameters as well.
-# wca.set_parameter_deviation('Vos', 3e-4, 5e-3)
+wca.set_parameter_deviation('Vos', 3e-4, 5e-3)
 
 # Finally the netlist is saved to a file
 wca.save_netlist('./testfiles/sallenkey_wc.asc')
 ```
 -- in examples/run_worst_case.py [Example 1]
 
 When opening the created sallenkey_wc.net file, we can see that the following circuit.
@@ -298,15 +297,15 @@
 - A default value for the run parameter was added. This is useful if the .step param run is commented out.
 - The R1 tolerance is different from the other resistors. This is because the tolerance was explicitly set for R1.
 - The wc() function is added to the circuit. This function is used to calculate the worst case value for each component,
 given a tolerance value and its respective index.
 - The wc1() function is added to the circuit. This function is used to calculate the worst case value for each component,
 given a minimum and maximum value and its respective index.
 
-### LTSteps.py ###
+### ltsteps.py ###
 
 This module defines a class that can be used to parse LTSpice log files where the information about .STEP information is
 written. There are two possible usages of this module, either programmatically by importing the module and then
 accessing data through the class as exemplified here:
 
 ```python
 #!/usr/bin/env python
@@ -398,27 +397,39 @@
 
 This module is used to run a server that can be used to run simulations in a remote machine. The server will run in the
 background and will wait for a client to connect. The client will send a netlist to the server and the server will run
 the simulation and return the results to the client. The client on the remote machine is a script instancing the
 SimClient class. An example of its usage is shown below:
 
 ```python
+import os
+import zipfile
+import logging
+
+# In order for this, to work, you need to have a server running. To start a server, run the following command:
+# python -m spicelib.run_server --port 9000 --parallel 4 --output ./temp
+
+_logger = logging.getLogger("spicelib.SimClient")
+_logger.setLevel(logging.DEBUG)
+
 from spicelib.client_server.sim_client import SimClient
 
 server = SimClient('http://localhost', 9000)
 print(server.session_id)
 runid = server.run("./testfiles/testfile.net")
 print("Got Job id", runid)
 for runid in server:  # Ma
     zip_filename = server.get_runno_data(runid)
     print(f"Received {zip_filename} from runid {runid}")
     with zipfile.ZipFile(zip_filename, 'r') as zipf:  # Extract the contents of the zip file
         print(zipf.namelist())  # Debug printing the contents of the zip file
         zipf.extract(zipf.namelist()[0])  # Normally the raw file comes first
     os.remove(zip_filename)  # Remove the zip file
+
+server.close_session()
 ```
 -- in examples/sim_client_example.py [SimClient Example]
 
 ```bash
 usage: run_server [-h] [-p PORT] [-o OUTPUT] [-l PARALLEL] simulator
 
 Run the LTSpice Server. This is a command line interface to the SimServer class.The SimServer class is used to run
@@ -476,14 +487,27 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 1.1.1
+  * Supporting hierarchical edits on both QSpice and LTspice schematics
+  * Skipping the need of the rich library on examples
+  * Giving feedback on the search for symbols on the ASC to QSCH conversion
+  * Improvement on Documentation
+  * Adding examples and unittests on hiearchical edits
+  * Giving access to hidden properties (asc_file_path in AscEditor and qsch_file_path in QschEditor)
+  * Refactoring save_netlist() method in QschEditor class
+  * Supporting arcs and rectangles on AsyReader
+  * Adding file_search.py containing utility functions for searching files
+  * Adding windows_short_names.py containing a code to get the 8.3 Windows short names.
+* Version 1.1.0
+  * First usable version of a LTspice to Qspice schematic converter.
 * Version 1.0.4
   * Adding the missing the asc_to_qsch_data.xml to the package
   * Adding a MANIFEST.in to the project
   * Adding keywords to the project.toml
 * Version 1.0.3
   * Correcting the generation of a .net from the QschEditor.
 * Version 1.0.2
```

### Comparing `spicelib-1.0.4/examples/ltsteps_example.py` & `spicelib-1.1.1/examples/ltsteps_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/examples/ngspice_batch.py` & `spicelib-1.1.1/examples/ngspice_batch.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/examples/qspice_example.py` & `spicelib-1.1.1/examples/qspice_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/examples/raw_plotting.py` & `spicelib-1.1.1/examples/raw_plotting.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/examples/raw_write_example.py` & `spicelib-1.1.1/examples/raw_write_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/examples/run_fast_worst_case.py` & `spicelib-1.1.1/examples/run_fast_worst_case.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/examples/run_montecarlo.py` & `spicelib-1.1.1/examples/run_montecarlo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -- Start of Example 1 --
-import numpy as np
 from spicelib import AscEditor, SimRunner  # Imports the class that manipulates the asc file
 from spicelib.sim.tookit.montecarlo import Montecarlo  # Imports the Montecarlo toolkit class
 from spicelib.simulators.ltspice_simulator import LTspice
 
 sallenkey = AscEditor("./testfiles/sallenkey.asc")  # Reads the asc file into memory
 runner = SimRunner(simulator=LTspice, output_folder='./temp_mc',
                    verbose=True)  # Instantiates the runner with a temp folder set
```

### Comparing `spicelib-1.0.4/examples/run_sensitivity.py` & `spicelib-1.1.1/examples/run_sensitivity.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/examples/run_worst_case.py` & `spicelib-1.1.1/examples/run_worst_case.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,41 +18,42 @@
 # wca.set_tolerance('V', 0.1)  # 10% tolerance. For Worst Case analysis, the distribution is irrelevant
 wca.set_tolerance('I', 0.1)  # 10% tolerance. For Worst Case analysis, the distribution is irrelevant
 # Some components can have a different tolerance
 wca.set_tolerance('R1', 0.05)  # 5% tolerance for R1 only. This only overrides the default tolerance for R1
 wca.set_tolerance('R4', 0.0)  # 5% tolerance for R1 only. This only overrides the default tolerance for R1
 
 # Tolerances can be set for parameters as well.
-# wca.set_parameter_deviation('Vos', 3e-4, 5e-3)
+wca.set_parameter_deviation('Vos', 3e-4, 5e-3)
 
 # Finally the netlist is saved to a file
 wca.save_netlist('./testfiles/sallenkey_wc.asc')
 # -- End of Example 1 --
 
 wca.run_testbench()  # Runs the simulation with splits of 100 runs each
 
 logs = wca.read_logfiles()   # Reads the log files and stores the results in the results attribute
 logs.export_data('./temp_wca/data.csv')  # Exports the data to a csv file
 
 print("Worst case results:")
 for param in ('fcut', 'fcut_FROM'):
     print(f"{param}: min:{logs.min_measure_value(param)} max:{logs.max_measure_value(param)}")
 
-## All components sensitivity
+# All components sensitivity
 sens = wca.make_sensitivity_analysis('fcut', '*')  # Makes the sensitivity analysis for all components
 print(sens)
 
 wca.cleanup_files()  # Deletes the temporary files
 
 print("=====================================")
 # Now using the second method, where the simulations are ran one by one
 wca.clear_simulation_data()  # Clears the simulation data
 wca.reset_netlist()  # Resets the netlist to the original
 wca.run_analysis()  # Makes the Worst Case Analysis
-min, max = wca.get_min_max_measure_value('fcut')
-print(f"fcut: min:{min} max:{max}")
+min_fcut, max_fcut = wca.get_min_max_measure_value('fcut')
+print(f"fcut: min:{min_fcut} max:{max_fcut}")
 sens = wca.make_sensitivity_analysis('fcut', 'R1')  # Makes the sensitivity analysis for R1
 print(sens)
-## All components sensitivity
+
+# All components sensitivity
 sens = wca.make_sensitivity_analysis('fcut', '*')  # Makes the sensitivity analysis for all components
 print(sens)
 wca.cleanup_files()  # Deletes the temporary files
```

### Comparing `spicelib-1.0.4/examples/sim_client_example.py` & `spicelib-1.1.1/examples/sim_client_example.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,35 +14,36 @@
 # Purpose:     Example of a client to the SimServer
 #
 # Author:      Nuno Brum (nuno.brum@gmail.com)
 #
 # Created:     23-02-2023
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
-import os.path
+# -- Start of SimClient Example --
+import os
 import zipfile
 import logging
 
 # In order for this, to work, you need to have a server running. To start a server, run the following command:
 # python -m spicelib.run_server --port 9000 --parallel 4 --output ./temp
 
 _logger = logging.getLogger("spicelib.SimClient")
 _logger.setLevel(logging.DEBUG)
-# -- Start of SimClient Example --
+
 from spicelib.client_server.sim_client import SimClient
 
 server = SimClient('http://localhost', 9000)
 print(server.session_id)
 runid = server.run("./testfiles/testfile.net")
 print("Got Job id", runid)
 for runid in server:  # Ma
     zip_filename = server.get_runno_data(runid)
     print(f"Received {zip_filename} from runid {runid}")
     with zipfile.ZipFile(zip_filename, 'r') as zipf:  # Extract the contents of the zip file
         print(zipf.namelist())  # Debug printing the contents of the zip file
         zipf.extract(zipf.namelist()[0])  # Normally the raw file comes first
     os.remove(zip_filename)  # Remove the zip file
-# -- End of SimClient Example --
 
 server.close_session()
+# -- End of SimClient Example --
 print("Finished")
 # server.server.stop_server()  # This will terminate the server
```

### Comparing `spicelib-1.0.4/examples/sim_runner_asc_example.py` & `spicelib-1.1.1/examples/sim_runner_asc_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         print("simulating OpAmp", opamp, "Voltage", supply_voltage)
         LTC.run(netlist)
 
 for raw, log in LTC:
     print("Raw file: %s, Log file: %s" % (raw, log))
     # do something with the data
     # raw_data = RawRead(raw)
-    # log_data = LTSteps(log)
+    # log_data = LTSpiceLogReader(log)
     # ...
 
 # Sim Statistics
 print('Successful/Total Simulations: ' + str(LTC.okSim) + '/' + str(LTC.runno))
 
 enter = input("Press enter to delete created files")
 if enter == '':
```

### Comparing `spicelib-1.0.4/examples/sim_runner_callback_example.py` & `spicelib-1.1.1/examples/sim_runner_callback_example.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 # coding=utf-8
 import logging
-from rich.logging import RichHandler
+
+try:
+    from rich.logging import RichHandler
+except ImportError:
+    RichHandler = None
+
 import spicelib
 
 from spicelib import SimRunner, SpiceEditor
 from time import sleep
 from random import random
 
 spicelib.set_log_level(logging.DEBUG)
-spicelib.add_log_handler(RichHandler())
+if RichHandler is not None:
+    spicelib.add_log_handler(RichHandler())
 
 
 from spicelib.simulators.ltspice_simulator import LTspice
 
 
 def processing_data(raw_file, log_file, supply_voltage, opamp):
     print("Handling the simulation data of ""%s"", log file ""%s""" % (raw_file, log_file))
```

### Comparing `spicelib-1.0.4/examples/sim_runner_callback_process_example.py` & `spicelib-1.1.1/examples/sim_runner_callback_process_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/examples/sim_runner_example.py` & `spicelib-1.1.1/examples/sim_runner_example.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         print("simulating OpAmp", opamp, "Voltage", supply_voltage)
         LTC.run(netlist)
 
 for raw, log in LTC:
     print("Raw file: %s, Log file: %s" % (raw, log))
     # do something with the data
     # raw_data = RawRead(raw)
-    # log_data = LTSteps(log)
+    # log_data = LTSpiceLogReader(log)
     # ...
 
 netlist.reset_netlist()
 netlist.add_instructions(
     "; Simulation settings",
     ".ac dec 30 10 1Meg",
     ".meas AC Gain MAX mag(V(out)) ; find the peak response and call it ""Gain""",
```

### Comparing `spicelib-1.0.4/examples/sim_server_example.py` & `spicelib-1.1.1/examples/sim_server_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/examples/sim_stepper_example.py` & `spicelib-1.1.1/examples/sim_stepper_example.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/pyproject.toml` & `spicelib-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 [project]
 name = "spicelib"
-version = "1.0.4"
+version = "1.1.1"
 authors = [
   { name="Nuno Brum", email="me@nunobrum.com" },
 ]
 description = "A set of tools to Automate Spice simulations"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `spicelib-1.0.4/spicelib/__init__.py` & `spicelib-1.1.1/spicelib/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     Returns all the name strings used as logger identifiers.
 
     :return: A List of strings which contains all the logger's names used in this library.
     :rtype: list[str]
     """
     return [
         "spicelib.RunTask",
-        "spicelib.LTSteps",
         "spicelib.SimClient",
         "spicelib.SimServer",
         "spicelib.ServerSimRunner",
         "spicelib.LTSteps",
         "spicelib.RawRead",
         "spicelib.LTSpiceSimulator",
         "spicelib.NGSpiceSimulator",
```

### Comparing `spicelib-1.0.4/spicelib/client_server/sim_client.py` & `spicelib-1.1.1/spicelib/client_server/sim_client.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/client_server/sim_server.py` & `spicelib-1.1.1/spicelib/client_server/sim_server.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/client_server/srv_sim_runner.py` & `spicelib-1.1.1/spicelib/client_server/srv_sim_runner.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/editor/asc_editor.py` & `spicelib-1.1.1/spicelib/editor/asc_editor.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 # Name:        asc_editor.py
 # Purpose:     Class made to update directly the LTspice ASC files
 #
 # Author:      Nuno Brum (nuno.brum@gmail.com)
 #
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
+import os.path
 from pathlib import Path
-from typing import Union, Tuple, List
+from typing import Union, Optional
 import re
 import logging
+from ..utils.file_search import find_file_in_directory
 from .base_editor import BaseEditor, format_eng, ComponentNotFoundError, ParameterNotFoundError, PARAM_REGEX, \
     UNIQUE_SIMULATION_DOT_INSTRUCTIONS, Component
 from .base_schematic import (BaseSchematic, Point, Line, Text, SchematicComponent, ERotation, HorAlign, VerAlign,
-                             TextTypeEnum)
+                             TextTypeEnum, Port)
 
 _logger = logging.getLogger("spicelib.AscEditor")
 
 TEXT_REGEX = re.compile(r"TEXT (-?\d+)\s+(-?\d+)\s+(Left|Right|Top|Bottom)\s(\d+)\s*(?P<type>[!;])(?P<text>.*)",
                         re.IGNORECASE)
 TEXT_REGEX_X = 1
 TEXT_REGEX_Y = 2
@@ -112,28 +114,29 @@
             return 'VBottom'
         else:
             return 'Left'
 
 
 class AscEditor(BaseSchematic):
     """Class made to update directly the LTspice ASC files"""
+    lib_paths = []  # This is a class variable, so it can be shared between all instances.
 
     def __init__(self, asc_file: str):
         super().__init__()
         self.version = 4
         self.sheet = "1 0 0"  # Three values are present on the SHEET clause
-        self._asc_file_path = Path(asc_file)
-        if not self._asc_file_path.exists():
+        self.asc_file_path = Path(asc_file)
+        if not self.asc_file_path.exists():
             raise FileNotFoundError(f"File {asc_file} not found")
         # read the file into memory
         self.reset_netlist()
 
     @property
     def circuit_file(self) -> Path:
-        return self._asc_file_path
+        return self.asc_file_path
 
     def save_netlist(self, run_netlist_file: Union[str, Path]) -> None:
         if isinstance(run_netlist_file, str):
             run_netlist_file = Path(run_netlist_file)
         run_netlist_file = run_netlist_file.with_suffix(".asc")
         with open(run_netlist_file, 'w') as asc:
             _logger.info(f"Writing ASC file {run_netlist_file}")
@@ -147,39 +150,45 @@
             for component in self.components.values():
                 symbol = component.symbol
                 posX = component.position.X
                 posY = component.position.Y
                 rotation = ASC_INV_ROTATION_DICT[component.rotation]
                 asc.write(f"SYMBOL {symbol} {posX} {posY} {rotation}" + END_LINE_TERM)
                 for attr, value in component.attributes.items():
-                    if attr.startswith('WINDOW') and isinstance(value, Text):
+                    if attr.startswith('_WINDOW') and isinstance(value, Text):
+                        num_ref = attr[len("_WINDOW_"):]
                         posX = value.coord.X
                         posY = value.coord.Y
                         alignment = asc_text_align_get(value)
                         size = value.size
-                        asc.write(f"{attr} {posX} {posY} {alignment} {size}" + END_LINE_TERM)
+                        asc.write(f"WINDOW {num_ref} {posX} {posY} {alignment} {size}" + END_LINE_TERM)
                 asc.write(f"SYMATTR InstName {component.reference}" + END_LINE_TERM)
+                if component.reference.startswith('X') and "_SUBCKT" in component.attributes:
+                    # writing the sub-circuit if it was updated
+                    sub_circuit: AscEditor = component.attributes["_SUBCKT"]
+                    if sub_circuit.updated:
+                        sub_circuit.save_netlist(sub_circuit.asc_file_path)
                 for attr, value in component.attributes.items():
-                    if not attr.startswith('WINDOW'):
+                    if not attr.startswith('_'):  # All these are not exported since they are only used internally
                         asc.write(f"SYMATTR {attr} {value}" + END_LINE_TERM)
             for directive in self.directives:
                 posX = directive.coord.X
                 posY = directive.coord.Y
                 alignment = asc_text_align_get(directive)
                 size = directive.size
                 if directive.type == TextTypeEnum.DIRECTIVE:
                     directive_type = '!'
                 else:
                     directive_type = ';'  # Otherwise assume it is a comment
                 asc.write(f"TEXT {posX} {posY} {alignment} {size} {directive_type}{directive.text}" + END_LINE_TERM)
 
     def reset_netlist(self, create_blank: bool = False) -> None:
         super().reset_netlist()
-        with open(self._asc_file_path, 'r') as asc_file:
-            _logger.info(f"Parsing ASC file {self._asc_file_path}")
+        with open(self.asc_file_path, 'r') as asc_file:
+            _logger.info(f"Parsing ASC file {self.asc_file_path}")
             component = None
             for line in asc_file:
                 if line.startswith("SYMBOL"):
                     tag, symbol, posX, posY, rotation = line.split()
                     if component is not None:
                         assert component.reference is not None, "Component InstName was not given"
                         self.components[component.reference] = component
@@ -193,22 +202,25 @@
                         raise ValueError(f"Invalid Rotation value: {rotation}")
                 elif line.startswith("WINDOW"):
                     assert component is not None, "Syntax Error: WINDOW clause without SYMBOL"
                     tag, num_ref, posX, posY, alignment, size = line.split()
                     coord = Point(int(posX), int(posY))
                     text = Text(coord=coord, text=num_ref, size=size, type=TextTypeEnum.ATTRIBUTE)
                     text = asc_text_align_set(text, alignment)
-                    component.attributes['WINDOW ' + num_ref] = text
+                    component.attributes['_WINDOW ' + num_ref] = text
 
                 elif line.startswith("SYMATTR"):
                     assert component is not None, "Syntax Error: SYMATTR clause without SYMBOL"
                     tag, ref, text = line.split(maxsplit=2)
                     text = text.strip()  # Gets rid of the \n terminator
                     if ref == "InstName":
                         component.reference = text
+                        if component.reference.startswith('X'):  # This is a subcircuit
+                            # then create the attribute "SUBCKT"
+                            component.attributes["_SUBCKT"] = self._get_symbol_circuit(component.symbol)
                     else:
                         component.attributes[ref] = text
                 elif line.startswith("TEXT"):
                     match = TEXT_REGEX.match(line)
                     if match:
                         text = match.group(TEXT_REGEX_TEXT)
                         X = int(match.group(TEXT_REGEX_X))
@@ -237,25 +249,42 @@
                     self.labels.append(flag)
                 elif line.startswith("Version"):
                     tag, version = line.split()
                     assert version in ["4"], f"Unsupported version : {version}"
                     self.version = version
                 elif line.startswith("SHEET "):
                     self.sheet = line[len("SHEET "):].strip()
+                elif line.startswith("IOPIN "):
+                    tag, posX, posY, direction = line.split()
+                    text = self.labels[-1]  # Assuming it is the last FLAG parsed
+                    assert text.coord.X == int(posX) and text.coord.Y == int(posY), "Syntax Error, getting a IOPIN withou an associated label"
+                    port = Port(text, direction)
+                    self.ports.append(port)
                 else:
                     raise NotImplementedError("Primitive not supported for ASC file\n" 
                                               f'"{line}"')
             if component is not None:
                 assert component.reference is not None, "Component InstName was not given"
                 self.components[component.reference] = component
 
+    def _get_symbol_circuit(self, symbol: str):
+        asc_filename = symbol + os.path.extsep + "asc"
+        asc_path = self._lib_file_find(asc_filename)
+        answer = AscEditor(asc_path)
+        return answer
+
+    def get_subcircuit(self, reference: str) -> 'AscEditor':
+        """Returns an AscEditor file corresponding to the symbol"""
+        sub = self.get_component(reference)
+        return sub.attributes["_SUBCKT"]
+
     def get_component_info(self, reference) -> dict:
         """Returns the reference information as a dictionary"""
         component = self.get_component(reference)
-        info = {name: value for name, value in component.attributes if not name.startswith("WINDOW ")}
+        info = {name: value for name, value in component.attributes.items() if not name.startswith("WINDOW ")}
         info["InstName"] = reference  # For legacy purposes
         return info
 
     def get_component_position(self, reference: str) -> (Point, ERotation):
         component = self.get_component(reference)
         return component.position, component.rotation
 
@@ -299,47 +328,52 @@
             _logger.debug(f"Parameter {param} not found in ASC file, adding it")
             x, y = self._get_text_space()
             coord = Point(x, y)
             text = f".param {param}={value}"
             directive = Text(coord=coord, text=text, size=2, type=TextTypeEnum.DIRECTIVE)
             _logger.info(f"Parameter {param} added with value {value}")
             self.directives.append(directive)
+        self.updated = True
 
     def set_component_value(self, device: str, value: Union[str, int, float]) -> None:
         component = self.get_component(device)
         if "Value" in component.attributes:
             if isinstance(value, str):
                 value_str = value
             else:
                 value_str = format_eng(value)
             component.attributes["Value"] = value_str
             _logger.info(f"Component {device} updated to {value_str}")
+            self.set_updated(device)
         else:
             _logger.error(f"Component {device} does not have a Value attribute")
             raise ComponentNotFoundError(f"Component {device} does not have a Value attribute")
 
     def set_element_model(self, element: str, model: str) -> None:
         component = self.get_component(element)
         component.symbol = model
         _logger.info(f"Component {element} updated to {model}")
+        self.set_updated(element)
 
     def get_component_value(self, element: str) -> str:
         component = self.get_component(element)
         if "Value" not in component.attributes:
             _logger.error(f"Component {element} does not have a Value attribute")
             raise ComponentNotFoundError(f"Component {element} does not have a Value attribute")
         return component.attributes["Value"]
 
     def get_components(self, prefixes='*') -> list:
         if prefixes == '*':
             return list(self.components.keys())
         return [k for k in self.components.keys() if k[0] in prefixes]
 
     def remove_component(self, designator: str):
-        del self.components[designator]
+        sub_circuit, ref = self._get_parent(designator)
+        del sub_circuit.components[ref]
+        sub_circuit.updated = True
 
     def _get_text_space(self):
         """
         Returns the coordinate on the Schematic File canvas where a text can be appended.
         """
         min_x = 100000  # High enough to be sure it will be replaced
         max_x = -100000
@@ -367,45 +401,73 @@
             min_x = min(min_x, component.position.X)
             max_x = max(max_x, component.position.X)
             min_y = min(min_y, component.position.Y)
             max_y = max(max_y, component.position.Y)
 
         return min_x, max_y + 24  # Setting the text in the bottom left corner of the canvas
 
+    def add_library_paths(self, *paths):
+        """Adding paths for searching for symbols and libraries"""
+        self.lib_paths.extend(*paths)
+
+    def _lib_file_find(self, filename) -> Optional[str]:
+        for sym_root in self.lib_paths + [
+            # os.path.curdir,  # The current script directory
+            os.path.split(self.asc_file_path)[0],  # The directory where the script is located
+            os.path.expanduser(r"~\AppData\Local\LTspice\lib\sym"),
+            os.path.expanduser(r"~\Documents\LtspiceXVII\lib\sym"),
+            # os.path.expanduser(r"~\AppData\Local\Programs\ADI\LTspice\lib.zip"), # TODO: implement this
+        ]:
+            print(f"   {os.path.abspath(sym_root)}")
+            if not os.path.exists(sym_root):  # Skipping invalid paths
+                continue
+            if sym_root.endswith('.zip'):
+                pass
+                # TODO: Using an IO buffer to pass the file to the AsyEditor
+            else:
+                file_found = find_file_in_directory(sym_root, filename)
+                if file_found is not None:
+                    return file_found
+        return None
+
     def add_instruction(self, instruction: str) -> None:
+        # docstring inherited from BaseEditor
         instruction = instruction.strip()  # Clean any end of line terminators
         set_command = instruction.split()[0].upper()
 
         if set_command in UNIQUE_SIMULATION_DOT_INSTRUCTIONS:
             # Before adding new instruction, if it is a unique instruction, we just replace it
             i = 0
             while i < len(self.directives):
                 directive = self.directives[i]
                 if directive.type == TextTypeEnum.COMMENT:
                     continue  # this is a comment
                 directive_command = directive.text.split()[0].upper()
                 if directive_command in UNIQUE_SIMULATION_DOT_INSTRUCTIONS:
                     directive.text = instruction
+                    self.updated = True
                     return  # Job done, can exit this method
                 i += 1
         elif set_command.startswith('.PARAM'):
             raise RuntimeError('The .PARAM instruction should be added using the "set_parameter" method')
         # If we get here, then the instruction was not found, so we need to add it
         x, y = self._get_text_space()
         coord = Point(x, y)
         directive = Text(coord=coord, text=instruction, size=2, type=TextTypeEnum.DIRECTIVE)
         self.directives.append(directive)
+        self.updated = True
 
     def remove_instruction(self, instruction: str) -> None:
         i = 0
         while i < len(self.directives):
             if instruction in self.directives[i].text:
                 text = self.directives[i].text
                 del self.directives[i]
                 _logger.info(f"Instruction {text} removed")
+                self.updated = True
                 return  # Job done, can exit this method
             i += 1
 
         msg = f'Instruction "{instruction}" not found'
         _logger.error(msg)
         raise RuntimeError(msg)
 
@@ -417,10 +479,12 @@
             instruction = self.directives[i].text
             if regex.match(instruction) is not None:
                 instr_removed = True
                 del self.directives[i]
                 _logger.info(f"Instruction {instruction} removed")
             else:
                 i += 1
-        if not instr_removed:
+        if instr_removed:
+            self.updated = True
+        else:
             msg = f'Instructions matching "{search_pattern}" not found'
             _logger.error(msg)
```

### Comparing `spicelib-1.0.4/spicelib/editor/asy_reader.py` & `spicelib-1.1.1/spicelib/editor/asy_reader.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -------------------------------------------------------------------------------
 
 import logging
 from collections import OrderedDict
 from pathlib import Path
 from typing import Union
 
-from .base_schematic import Point, Text, TextTypeEnum, Line, HorAlign, ERotation, VerAlign
+from .base_schematic import Point, Text, TextTypeEnum, Line, Circle, Rectangle, Arc, HorAlign, ERotation, VerAlign
 from .asc_editor import asc_text_align_set, TEXT_REGEX, LT_ATTRIBUTE_NUMBERS, LT_ATTRIBUTE_NUMBERS_INV, \
     WEIGHT_CONVERSION_TABLE
 
 from .qsch_editor import QschTag
 
 _logger = logging.getLogger("spicelib.AsyReader")
 SCALE_X = 6.25
@@ -38,15 +38,17 @@
 
     def __init__(self, asy_file: Union[Path, str]):
         super().__init__()
         self.version = 4
         self.symbol_type = None
         self.pins = []
         self.lines = []
+        self.arcs = []
         self.circles = []
+        self.rectangles = []
         self.attributes = OrderedDict()
         self._asy_file_path = Path(asy_file)
         self.windows = []
         pin = None
         if not self._asy_file_path.exists():
             raise FileNotFoundError(f"File {asy_file} not found")
         with open(self._asy_file_path, 'r') as asc_file:
@@ -82,15 +84,15 @@
                     x1 = int(x1)
                     x2 = int(x2)
                     y1 = int(y1)
                     y2 = int(y2)
                     # distance = (x2-x1)  # Always assuming a circle
                     # circle = Arc(Point((x1+x2)/2, (y1+y2)/2), radius=distance/2, start_angle=0, stop_angle=360,
                     #              style=f"{{style:1, weight:{weight}}}")
-                    circle = Line(Point(x1, y1), Point(x2, y2))
+                    circle = Circle(Point(x1, y1), Point(x2, y2))
                     self.circles.append(circle)
                 elif line.startswith("Version"):
                     tag, version = line.split()
                     assert version in ["4"], f"Unsupported version : {version}"
                     self.version = version
                 elif line.startswith("SymbolType "):
                     self.symbol_type = line[len("SymbolType "):].strip()
@@ -126,46 +128,97 @@
                             #     vertical_alignment = VerAlign.BOTTOM (default)
                             elif justification == "RIGHT":
                                 text_alignment = HorAlign.RIGHT
                             # else: justification == "LEFT" (default)
 
                     pin = Text(coord, "", type=TextTypeEnum.PIN, size=int(offset),
                                textAlignment=text_alignment, verticalAlignment=vertical_alignment, angle=angle)
+                elif line.startswith("ARC"):
+                    tag, weight, x1, y1, x2, y2, x3, y3, x4, y4  = line.split()
+                    x1 = int(x1)
+                    x2 = int(x2)
+                    x3 = int(x3)
+                    x4 = int(x4)
+                    y1 = int(y1)
+                    y2 = int(y2)
+                    y3 = int(y3)
+                    y4 = int(y4)
+
+                    center = Point((x1+x2)//2, (y1+y2)//2)
+                    radius = abs(x2-x1)/2  # Using only the X axis. Assuming a circle not an elipse
+                    start = Point((x3-center.X)/radius, (y3-center.Y)/radius)
+                    stop = Point((x4-center.X)/radius, (y4-center.Y)/radius)
+                    arc = Arc(center, radius=radius, start=start, stop=stop)
+                    self.arcs.append(arc)
+                elif line.startswith("RECTANGLE"):
+                    tag, weight, x1, y1, x2, y2 = line.split()
+                    x1 = int(x1)
+                    x2 = int(x2)
+                    y1 = int(y1)
+                    y2 = int(y2)
+                    rect = Rectangle(Point(x1, y1), Point(x2, y2))
+                    self.rectangles.append(rect)
                 else:
-                    raise NotImplementedError("Primitive not supported for ASC file\n"
+                    print("Primitive not supported for ASC file\n"
                                               f'"{line}"')
             if pin is not None:
                 self.pins.append(pin)
 
     def to_qsch(self, *args):
         """Create a QschTag representing a component symbol."""
         spice_prefix = self.attributes['Prefix']
         symbol = QschTag("symbol", spice_prefix[0])
         symbol.items.append(QschTag("type:", spice_prefix))
         symbol.items.append(QschTag("description:", self.attributes["Description"]))
         symbol.items.append(QschTag("shorted pins:", "false"))
         for line in self.lines:
+            x1 = int(line.V1.X * SCALE_X)
+            y1 = int(line.V1.Y * SCALE_Y)
+            x2 = int(line.V2.X * SCALE_X)
+            y2 = int(line.V2.Y * SCALE_Y)
             segment, _ = QschTag.parse(
-                f"«line ({line.V1.X * SCALE_X:.0f},{line.V1.Y * SCALE_Y:.0f}) "
-                f"({line.V2.X * SCALE_X:.0f},{line.V2.Y * SCALE_Y:.0f})"
-                f" 0 0 0x1000000 -1 -1»")
+                f"«line ({x1},{y1}) ({x2},{y2}) 0 0 0x1000000 -1 -1»")
             symbol.items.append(segment)
 
-        for arc in self.circles:
+        for circle in self.circles:
             # x1 = int((arc.center.X - arc.radius) * SCALE_X)
             # y1 = int((arc.center.Y - arc.radius) * SCALE_Y)
             # x2 = int((arc.center.X + arc.radius) * SCALE_X)
             # y2 = int((arc.center.Y + arc.radius) * SCALE_Y)
-            x1 = int(arc.V1.X * SCALE_X)
-            y1 = int(arc.V1.Y * SCALE_Y)
-            x2 = int(arc.V2.X * SCALE_X)
-            y2 = int(arc.V2.Y * SCALE_Y)
-            elipse_tag, _ = QschTag.parse(f"«ellipse ({x1},{y1}) ({x2},{y2}) 0 0 0 0x1000000 0x1000000 -1 -1»")
+            x1 = int(circle.V1.X * SCALE_X)
+            y1 = int(circle.V1.Y * SCALE_Y)
+            x2 = int(circle.V2.X * SCALE_X)
+            y2 = int(circle.V2.Y * SCALE_Y)
+            elipse_tag, _ = QschTag.parse(
+                f"«ellipse ({x1},{y1}) ({x2},{y2}) 0 0 0 0x1000000 0x1000000 -1 -1»"
+            )
             symbol.items.append(elipse_tag)
 
+        for rectangle in self.rectangles:
+            x1 = int(rectangle.V1.X * SCALE_X)
+            y1 = int(rectangle.V1.Y * SCALE_Y)
+            x2 = int(rectangle.V2.X * SCALE_X)
+            y2 = int(rectangle.V2.Y * SCALE_Y)
+            rectangle_tag, _ = QschTag.parse(
+                f"«rect ({x1},{y1}) ({x2},{y2}) 0 0 0 0x4000000 0x1000000 -1 0 -1»"
+            )
+            symbol.items.append(rectangle_tag)
+
+        for arc in self.arcs:
+            cx = int(arc.center.X * SCALE_X)
+            cy = int(arc.center.Y * SCALE_Y)
+            x1 = int((arc.center.X + arc.start.X * arc.radius) * SCALE_X)
+            y1 = int((arc.center.Y + arc.start.Y * arc.radius) * SCALE_Y)
+            x2 = int((arc.center.X + arc.stop.X * arc.radius) * SCALE_X)
+            y2 = int((arc.center.Y + arc.stop.Y * arc.radius) * SCALE_Y)
+
+            elipse_tag, _ = QschTag.parse(
+                f"«arc3p ({x1},{y1}) ({x2},{y2}) ({cx},{cy}) 0 0 0xff0000 -1 -1»"
+            )
+            symbol.items.append(elipse_tag)
         for i, attr in enumerate(self.windows):
             coord = attr.coord
             x = coord.X * SCALE_X
             y = coord.Y * SCALE_Y
             text, _ = QschTag.parse(f'«text ({x :.0f},{y :.0f})'
                                     f' 1 7 0 0x1000000 -1 -1 "{args[i]}"»')
             symbol.items.append(text)
```

### Comparing `spicelib-1.0.4/spicelib/editor/base_editor.py` & `spicelib-1.1.1/spicelib/editor/base_editor.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 from math import floor, log
 from pathlib import Path
 from typing import Union
 import logging
 
 _logger = logging.getLogger("spicelib.BaseEditor")
 
+SUBCKT_DIVIDER = ':'  #: This controls the sub-circuit divider when setting component values inside sub-circuits.
+# Ex: Editor.set_component_value('XU1:R1', '1k')
+
 UNIQUE_SIMULATION_DOT_INSTRUCTIONS = ('.AC', '.DC', '.TRAN', '.NOISE', '.DC', '.TF')
 SPICE_DOT_INSTRUCTIONS = (
     '.BACKANNO',
     '.END',
     '.ENDS',
     '.FERRET',  # Downloads a File from a given URL
     '.FOUR',  # Compute a Fourier Component after a .TRAN Analysis
@@ -165,44 +168,55 @@
     This defines the primitives (protocol) to be used for both SpiceEditor and AscEditor
     classes.
     """
 
     @property
     @abstractmethod
     def circuit_file(self) -> Path:
-        """Returns the netlist as a string"""
+        """Returns the path of the circuit file."""
         ...
 
     @abstractmethod
     def reset_netlist(self, create_blank: bool = False) -> None:
         """
-        Resets the netlist to the original state.
+        Reverts all changes done to the netlist. If create_blank is set to True, then the netlist is blanked.
 
-        :param create_blank: If True, the netlist will be reset to a new empty netlist. If False, the netlist will be reset to
-        the original state.
+        :param create_blank: If True, the netlist will be reset to a new empty netlist. If False, the netlist will be
+                             reset to the original state.
         """
         ...
 
     @abstractmethod
     def save_netlist(self, run_netlist_file: Union[str, Path]) -> None:
-        """Writes the netlist to a file"""
+        """
+        Saves the current state of the netlist to a file.
+
+        :param run_netlist_file: File name of the netlist file.
+        :type run_netlist_file: Path or str
+        :returns: Nothing
+        """
         ...
 
     def write_netlist(self, run_netlist_file: Union[str, Path]) -> None:
         """
         (Deprecated)
 
         Writes the netlist to a file. This is an alias to save_netlist."""
         self.save_netlist(run_netlist_file)
 
     @abstractmethod
     def get_component(self, reference: str) -> Component:
         """Returns the Component object representing the given reference in the netlist."""
         ...
 
+    @abstractmethod
+    def get_subcircuit(self, reference: str) -> 'BaseEditor':
+        """Returns a hierarchical subdesign"""
+        ...
+
     def get_component_attribute(self, reference: str, attribute: str) -> str:
         """Returns the value of the attribute of the component.
         :param reference: Reference of the component
         :type reference: str
         :param attribute: Name of the attribute to be retrieved
         :type attribute: str
         :return: Value of the attribute being sought
@@ -442,64 +456,80 @@
         :return: Nothing
         :raises: ComponentNotFoundError - When the component doesn't exist on the netlist.
         """
         ...
 
     @abstractmethod
     def add_instruction(self, instruction: str) -> None:
-        """Serves to add SPICE instructions to the simulation netlist. For example:
+        """
+        Adds a SPICE instruction to the netlist.
+
+        For example:
+
+            .. code-block:: text
 
-        .. code-block:: text
+                .tran 10m ; makes a transient simulation
+                .meas TRAN Icurr AVG I(Rs1) TRIG time=1.5ms TARG time=2.5ms" ; Establishes a measuring
+                .step run 1 100, 1 ; makes the simulation run 100 times
 
-                  .tran 10m ; makes a transient simulation
-                  .meas TRAN Icurr AVG I(Rs1) TRIG time=1.5ms TARG time=2.5ms" ; Establishes a measuring
-                  .step run 1 100, 1 ; makes the simulation run 100 times
 
         :param instruction:
             Spice instruction to add to the netlist. This instruction will be added at the end of the netlist,
             typically just before the .BACKANNO statement
         :type instruction: str
         :return: Nothing
         """
         ...
 
     @abstractmethod
     def remove_instruction(self, instruction) -> None:
-        """Usage a previously added instructions.
-        Example: ::
+        """
+        Removes a SPICE instruction from the netlist.
+
+        Example:
+
+        .. code-block:: python
 
             editor.remove_instruction(".STEP run -1 1023 1")
 
         This only works if the instruction exactly matches the line on the netlist. This means that space characters,
         and upper case and lower case differences will not match the line.
 
         :param instruction: The list of instructions to remove. Each instruction is of the type 'str'
         :type instruction: str
         :returns: Nothing
         """
         ...
 
     @abstractmethod
     def remove_Xinstruction(self, search_pattern: str) -> None:
-        """Removes a list of instructions from the SPICE NETLIST.
-        Example:
-        ::
+        """
+        Removes a SPICE instruction from the netlist based on a search pattern. This is a more flexible way to remove
+        instructions from the netlist. The search pattern is a regular expression that will be used to match the
+        instructions to be removed. The search pattern will be applied to each line of the netlist and if the pattern
+        matches, the line will be removed.
+
+        Example: The code below will remove all AC analysis instructions from the netlist.
+
+        .. code-block:: python
 
             editor.remove_Xinstruction("\.AC.*")
 
         :param search_pattern: The list of instructions to remove. Each instruction is of the type 'str'
         :type search_pattern: str
         :returns: Nothing
         """
         ...
 
     def add_instructions(self, *instructions) -> None:
-        """Adds a list of instructions to the SPICE NETLIST.
+        """
+        Adds a list of instructions to the SPICE NETLIST.
+
         Example:
-        ::
+        .. code-block:: python
 
             editor.add_instructions(
                 ".STEP run -1 1023 1",
                 ".dc V1 -5 5"
             )
 
         :param instructions: Argument list of instructions to add
```

### Comparing `spicelib-1.0.4/spicelib/editor/base_schematic.py` & `spicelib-1.1.1/spicelib/editor/base_schematic.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 
 
 from typing import List, Callable, Union
 from collections import OrderedDict
 import logging
-from .base_editor import BaseEditor, Component, ComponentNotFoundError
+from .base_editor import BaseEditor, Component, ComponentNotFoundError, SUBCKT_DIVIDER
 
 _logger = logging.getLogger("spicelib.BaseSchematic")
 
 
 class ERotation(enum.IntEnum):
     """Component Rotation Enum"""
     R0 = 0  # 0 Rotation
@@ -182,36 +182,50 @@
             return True
         # We also have to check if the given line touches any of the vertices of this line
         if line.touches(self.V1) or line.touches(self.V2):
             return True
         return False
 
 
-# @dataclasses.dataclass
-# class Arc:
-#     """X1, Y1, X2, Y2 coordinates"""
-#     center: Point
-#     radius: float
-#     start_angle: float
-#     stop_angle: float
-#     style: str = ""
-#     # The Arcs are decorative, they don't have associated nets
+Rectangle = Line  # Rectangles have the same properties as Line: Defined as the line that crosses two opposing vertices
+Circle = Line  # Circles are defined by the rectangle that touches 4 points of a circle.
+
+
+@dataclasses.dataclass
+class Arc:
+    """Opting for a non-native representation of the arc as LTspice and Qspice have different
+    ways of storing Arc information. Start and Stop points are calculated as a fraction of the radius
+    for X and Y. This avoids having to deal with the calculation of sines and cosines and their inverse
+    into radians."""
+    center: Point
+    radius: float
+    start: Point
+    stop: Point
+    style: str = ""
+    # The Arcs are decorative, they don't have associated nets
+
 
 @dataclasses.dataclass
 class Text:
     """Text object"""
     coord: Point
     text: str
     size: int = 1
     type: TextTypeEnum = TextTypeEnum.NULL
     textAlignment: HorAlign = HorAlign.LEFT
     verticalAlignment: VerAlign = VerAlign.CENTER
     angle: ERotation = ERotation.R0
 
 
+@dataclasses.dataclass
+class Port:
+    text: Text
+    direction: str
+
+
 class SchematicComponent(Component):
     """Hols component information"""
 
     def __init__(self):
         super().__init__()
         self.position: Point = Point(0, 0)
         self.rotation: ERotation = ERotation.R0
@@ -225,56 +239,92 @@
     """
 
     def __init__(self):
         self.components: OrderedDict[str, SchematicComponent] = OrderedDict()
         self.wires: List[Line] = []
         self.labels: List[Text] = []
         self.directives: List[Text] = []
+        self.ports: List[Port] = []
+        self.updated = False  # indicates if an edit was done and the file has to be written back to disk
 
     def reset_netlist(self, create_blank: bool = False) -> None:
         """Resets the netlist to the original state"""
         self.components.clear()
         self.wires.clear()
         self.labels.clear()
         self.directives.clear()
+        self.updated = False
 
     def copy_from(self, editor: 'BaseSchematic') -> None:
-        """Copies the contents of the given editor"""
+        """Clones the contents of the given editor"""
         from copy import deepcopy
         self.components = deepcopy(editor.components)
         self.wires = deepcopy(editor.wires)
         self.labels = deepcopy(editor.labels)
         self.directives = deepcopy(editor.directives)
+        self.updated = True
+
+    def _get_parent(self, reference) -> ("BaseSchematic", str):
+        if SUBCKT_DIVIDER in reference:
+            sub_ref, sub_comp = reference.split(SUBCKT_DIVIDER, 1)
+
+            subckt = self.get_component(sub_ref)
+            subcircuit = subckt.attributes['_SUBCKT']
+            return subcircuit, sub_comp
+        else:
+            return self, reference
+
+    def set_updated(self, reference):
+        sub_circuit, _ = self._get_parent(reference)
+        sub_circuit.updated = True
 
     def get_component(self, reference: str) -> SchematicComponent:
-        """Returns the SchematicComponent object representing the given reference in the schematic file"""
-        if reference not in self.components:
+        """
+        Returns the SchematicComponent object representing the given reference in the schematic file.
+
+        :param reference: The reference of the component
+        :return: The SchematicComponent object
+        :raises ComponentNotFoundError: If the component is not found.
+        """
+        sub_circuit, ref = self._get_parent(reference)
+
+        if ref not in sub_circuit.components:
             _logger.error(f"Component {reference} not found")
-            raise ComponentNotFoundError(f"Component {reference} not found in ASC file")
-        return self.components[reference]
+            raise ComponentNotFoundError(f"Component {reference} not found in Schematic file")
+        return sub_circuit.components[ref]
 
     def get_component_position(self, reference: str) -> (Point, ERotation):
         """Returns the position and rotation of the component"""
         comp = self.get_component(reference)
         return comp.position, comp.rotation
 
     def set_component_position(self, reference: str, position: Point, rotation: ERotation) -> None:
-        """Sets the position of the component"""
+        """Sets the position and rotation of the component.
+
+        :param reference: The reference of the component
+        :type reference: str
+        :param position: The new position of the component
+        :type position: Point
+        :param rotation: The new rotation of the component
+        :type rotation: ERotation
+        """
         comp = self.get_component(reference)
         comp.position = position
         comp.rotation = rotation
+        self.set_updated(reference)
 
     def add_component(self, component: SchematicComponent, **kwargs) -> None:
         if component.reference in self.components:
             # The component is already in the list, so we need to update it
             comp = self.components[component.reference]
         else:
             comp = SchematicComponent()
             comp.reference = component.reference
         self.components[component.reference] = comp
+        self.updated = True
 
     def scale(self, offset_x, offset_y, scale_x, scale_y: float,
               round_fun: Callable[[float], Union[int, float]] = None) -> None:
         """Scales the schematic"""
         if round_fun is None:
             round_fun = int
         for comp in self.components.values():
@@ -287,7 +337,8 @@
             wire.V2.Y = round_fun(wire.V2.Y * scale_y + offset_y)
         for label in self.labels:
             label.coord.X = round_fun(label.coord.X * scale_x + offset_x)
             label.coord.Y = round_fun(label.coord.Y * scale_y + offset_y)
         for directive in self.directives:
             directive.coord.X = round_fun(directive.coord.X * scale_x + offset_x)
             directive.coord.Y = round_fun(directive.coord.Y * scale_y + offset_y)
+        self.updated = True
```

### Comparing `spicelib-1.0.4/spicelib/editor/spice_editor.py` & `spicelib-1.1.1/spicelib/editor/spice_editor.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,26 +18,25 @@
 # -------------------------------------------------------------------------------
 import os
 from pathlib import Path
 import re
 import logging
 
 from .base_editor import BaseEditor, format_eng, ComponentNotFoundError, ParameterNotFoundError, PARAM_REGEX, \
-    UNIQUE_SIMULATION_DOT_INSTRUCTIONS, Component
+    UNIQUE_SIMULATION_DOT_INSTRUCTIONS, Component, SUBCKT_DIVIDER
 
-_logger = logging.getLogger("spicelib.SpiceEditor")
 from typing import Union, List, Callable, Any, Tuple, Optional
 from ..utils.detect_encoding import detect_encoding, EncodingDetectError
 
+_logger = logging.getLogger("spicelib.SpiceEditor")
+
 __author__ = "Nuno Canto Brum <nuno.brum@gmail.com>"
 __copyright__ = "Copyright 2021, Fribourg Switzerland"
 
 END_LINE_TERM = '\n'  #: This controls the end of line terminator used
-SUBCKT_DIVIDER = ':'  #: This controls the sub-circuit divider when setting component values inside sub-circuits.
-# Ex: Editor.set_component_value('XU1:R1', '1k')
 
 # A Spice netlist can only have one of the instructions below, otherwise an error will be raised
 
 REPLACE_REGXES = {
     'A': r"",  # LTSPice Only : Special Functions, Parameter substitution not supported
     'B': r"^(?P<designator>B§?[VI]?\w+)(?P<nodes>(\s+\S+){2})\s+(?P<value>.*)$",  # Behavioral source
     'C': r"^(?P<designator>C§?\w+)(?P<nodes>(\s+\S+){2})(?P<model>\s+\w+)?\s+(?P<value>({)?(?(6).*}|([0-9\.E+-]+(Meg|[kmuµnpf])?F?))).*$",
@@ -161,23 +160,17 @@
 
 class MissingExpectedClauseError(Exception):
     """Missing expected clause in Spice netlist"""
 
 
 class SpiceCircuit(BaseEditor):
     """
-    The Spice Circuit represents sub-circuits within a SPICE circuit and since sub-circuits can have sub-circuits inside
-    them, it serves as base for the top level netlist. See class SpiceEditor
-    This hierarchical approach helps to encapsulate and protect parameters and components from edits made at a higher
-    level.
-
-    The netlist information is stored in a list, each element of the list corresponds to a SPICE instruction.
-    If an instruction spawns more than a line with the '+' operator, it is contained in the same element.
-
-    This class serves as subclass to the SpiceEditor class.
+    Represents sub-circuits within a SPICE circuit. Since sub-circuits can have sub-circuits inside
+    them, it serves as base for the top level netlist. This hierarchical approach helps to encapsulate
+    and protect parameters and components from edits made at a higher level.
     """
 
     def __init__(self):
         super().__init__()
         self.netlist = []
 
     def _get_line_starting_with(self, substr: str) -> int:
@@ -211,15 +204,15 @@
                     return False
             elif cmd == '+':
                 assert len(self.netlist) > 0, "ERROR: The first line cannot be starting with a +"
                 self.netlist[-1] += line  # Appends to the last line
             else:
                 self.netlist.append(line)
                 if cmd[:4] == '.END':  # True for either .END and .ENDS primitives
-                    return True  # If an sub-circuit is ended correctly, returns True
+                    return True  # If a sub-circuit is ended correctly, returns True
         return False  # If a sub-circuit ends abruptly, returns False
 
     def write_lines(self, f):
         """Internal function. Do not use."""
         # This helper function writes the contents of sub-circuit to the file f
         for command in self.netlist:
             if isinstance(command, SpiceCircuit):
@@ -242,16 +235,24 @@
             if cmd == command:
                 match = search_expression.search(line)
                 if match:
                     return line_no, match
             line_no += 1
         return -1, None  # If it fails, it returns an invalid line number and No match
 
-    def _get_subckt(self, instance_name: str) -> 'SpiceCircuit':
-        """Internal function. Do not use."""
+    def get_subcircuit(self, instance_name: str) -> 'SpiceCircuit':
+        """
+        Returns an object representing a Subcircuit. This object can manipulate elements such as the SpiceEditor does.
+        :param instance_name: Reference of the subcircuit
+        :type instance_name: str
+        :returns: SpiceCircuit instance
+        :rtype: SpiceCircuit
+        :raises UnrecognizedSyntaxError: when an spice command is not recognized by spicelib
+        :raises ComponentNotFoundError: When the reference was not found
+        """
         global LibSearchPaths
         if SUBCKT_DIVIDER in instance_name:
             subckt_ref, sub_subckts = instance_name.split(SUBCKT_DIVIDER, 1)
         else:
             subckt_ref = instance_name
 
         line_no = self._get_line_starting_with(subckt_ref)
@@ -298,15 +299,15 @@
             # If it reached here, we have a valid lib_filename
             for lib_path in libs_list_full_path:
                 sub_circuit = SpiceEditor.find_subckt_in_lib(lib_path, subcircuit_name)
                 if sub_circuit:
                     break
         if sub_circuit:
             if SUBCKT_DIVIDER in instance_name:
-                return sub_circuit._get_subckt(sub_subckts)
+                return sub_circuit.get_subcircuit(sub_subckts)
             else:
                 return sub_circuit
         else:
             # The search was not successful
             raise ComponentNotFoundError(f'Sub-circuit "{subcircuit_name}" not found')
 
     def _set_model_and_value(self, component, value):
@@ -331,19 +332,26 @@
             raise UnrecognizedSyntaxError(line, REPLACE_REGXES[prefix])
         else:
             start = m.start('value')
             end = m.end('value')
             self.netlist[line_no] = line[:start] + value + line[end:]
 
     def reset_netlist(self, create_blank: bool = False) -> None:
+        """
+        Reverts all changes done to the netlist. If create_blank is set to True, then the netlist is blanked.
+
+        :param create_blank: If True, the netlist is blanked. That is, all primitives and components are erased.
+        :type create_blank: bool
+        :returns: None
+        """
         self.netlist.clear()
 
     def clone(self, **kwargs) -> 'SpiceCircuit':
         """
-        Creates a new copy of the SpiceCircuit. Change done at the new copy are not affecting the original
+        Creates a new copy of the SpiceCircuit. Changes done at the new copy do not affect the original.
 
         :key new_name: The new name to be given to the circuit
         :key type new_name: str
         :return: The new replica of the SpiceCircuit object
         :rtype: SpiceCircuit
         """
         clone = SpiceCircuit()
@@ -353,15 +361,15 @@
         new_name = kwargs.get('new_name', None)
         if new_name:  # If it is different from None
             clone.setname(new_name)
         return clone
 
     def name(self) -> str:
         """
-        Returns the name of the Sub-Circuit -> str.
+        Returns the name of the Sub-Circuit.
 
         :rtype: str
         """
         if len(self.netlist):
             for line in self.netlist:
                 m = subckt_regex.search(line)
                 if m:
@@ -369,16 +377,16 @@
             else:
                 raise RuntimeError("Unable to find .SUBCKT clause in subcircuit")
         else:
             raise RuntimeError("Empty Subcircuit")
 
     def setname(self, new_name: str):
         """
-        Renames the sub-circuit to a new name. No check is done to the new game give. It is up to the user to make sure
-        that the new name is valid.
+        Renames the sub-circuit to a new name. No check is done to the new name.
+        It is up to the user to make sure that the new name is valid.
 
         :param new_name: The new Name.
         :type new_name: str
         :return: Nothing
         :rtype: None
         """
         if len(self.netlist):
@@ -408,55 +416,58 @@
                 raise MissingExpectedClauseError("Unable to find .SUBCKT clause in subcircuit")
         else:
             # Avoiding exception by creating an empty sub-circuit
             self.netlist.append("* SpiceEditor Created this sub-circuit")
             self.netlist.append('.SUBCKT %s%s' % (new_name, END_LINE_TERM))
             self.netlist.append('.ENDS %s%s' % (new_name, END_LINE_TERM))
 
-    def get_component_info(self, component) -> dict:
+    def get_component_info(self, reference) -> dict:
         """
         Retrieves the component information as defined in the corresponding REGEX. The line number is also added.
 
-        :param component: Reference of the component
-        :type component: str
+        :param reference: Reference of the component
+        :type reference: str
         :return: Dictionary with the component information
         :rtype: dict
         :raises: ComponentNotFoundError - In case the component is not found
         :raises: UnrecognizedSyntaxError when the line doesn't match the expected REGEX.
         :raises: NotImplementedError if there isn't an associated regular expression for the component prefix.
         """
-        prefix = component[0]  # Using the first letter of the component to identify what is it
+        if SUBCKT_DIVIDER in reference:
+            raise NotImplementedError("This method doesn't support hierarchical access. "
+                                      "Please use set_component_value() and get_component_value() methods.")
+        prefix = reference[0]  # Using the first letter of the component to identify what is it
         regex = component_replace_regexs.get(prefix, None)  # Obtain RegX to make the update
 
         if regex is None:
             error_msg = f"Component must start with one of these letters: {','.join(REPLACE_REGXES.keys())}\n" \
-                        f"Got {component}"
+                        f"Got {reference}"
             _logger.warning(error_msg)
             raise NotImplementedError("Unsuported prefix {}".format(prefix))
 
-        line_no = self._get_line_starting_with(component)
+        line_no = self._get_line_starting_with(reference)
         line = self.netlist[line_no]
         m = regex.match(line)
         if m is None:
             error_msg = 'Unsupported line "{}"\nExpected format is "{}"'.format(line, REPLACE_REGXES[prefix])
             _logger.error(error_msg)
             raise UnrecognizedSyntaxError(line, REPLACE_REGXES[prefix])
 
         info = m.groupdict()
         info['line'] = line_no  # adding the line number to the component information
         return info
 
-    def get_component(self, reference: str) -> Component:
+    def get_component(self, reference: str) -> Union[Component, 'SpiceCircuit']:
         """
-        Returns an object representing the given reference in the schematic file
+        Returns an object representing the given reference in the schematic file.
 
         :param reference: Reference of the component
         :type reference: str
-        :return: The SchematicComponent object
-        :rtype: SchematicComponent
+        :return: The Component object or a SpiceSubcircuit in case of hierarchical design
+        :rtype: Component or SpiceSubcircuit
         :raises: ComponentNotFoundError - In case the component is not found
         :raises: UnrecognizedSyntaxError when the line doesn't match the expected REGEX.
         :raises: NotImplementedError if there isn't an associated regular expression for the component prefix.
         """
         component_info = self.get_component_info(reference)
         component = Component()
         component.reference = reference
@@ -464,15 +475,15 @@
         for attr in component_info:
             if attr not in ('designator', 'nodes'):
                 component.attributes[attr] = component_info[attr]
         return component
 
     def get_component_attribute(self, reference: str, attribute: str) -> Optional[str]:
         """
-        Retrieves the value of the attribute for the given component.
+        Returns the attribute of a component retrieved from the netlist.
 
         :param reference: Reference of the component
         :type reference: str
         :param attribute: Name of the attribute to be retrieved
         :type attribute: str
         :return: Value of the attribute
         :rtype: str
@@ -481,15 +492,15 @@
         :raises: NotImplementedError if there isn't an associated regular expression for the component prefix.
         """
         component_info = self.get_component_info(reference)
         return component_info.get(attribute, None)
 
     def get_parameter(self, param: str) -> str:
         """
-        Retrieves a Parameter from the Netlist
+        Returns the value of a parameter retrieved from the netlist.
 
         :param param: Name of the parameter to be retrieved
         :type param: str
         :return: Value of the parameter being sought
         :rtype: str
         :raises: ParameterNotFoundError - In case the component is not found
         """
@@ -497,25 +508,25 @@
         line_no, match = self._get_line_matching('.PARAM', regx)
         if match:
             return match.group('value')
         else:
             raise ParameterNotFoundError(param)
 
     def set_parameter(self, param: str, value: Union[str, int, float]) -> None:
-        """Adds a parameter to the SPICE netlist.
+        """Sets the value of a parameter in the netlist. If the parameter is not found, it is added to the netlist.
 
         Usage: ::
 
          LTC.set_parameter("TEMP", 80)
 
         This adds onto the netlist the following line: ::
 
          .PARAM TEMP=80
 
-        This is an alternative to the set_parameters which is more pythonic in it's usage,
+        This is an alternative to the set_parameters which is more pythonic in its usage
         and allows setting more than one parameter at once.
 
         :param param: Spice Parameter name to be added or updated.
         :type param: str
 
         :param value: Parameter Value to be set.
         :type value: str, int or float
@@ -531,16 +542,17 @@
         else:
             # Was not found
             # the last two lines are typically (.backano and .end)
             insert_line = len(self.netlist) - 2
             self.netlist.insert(insert_line, '.PARAM {}={}  ; Batch instruction'.format(param, value) + END_LINE_TERM)
 
     def set_component_value(self, device: str, value: Union[str, int, float]) -> None:
-        """Changes the value of a component, such as a Resistor, Capacitor or Inductor. For components inside
-        sub-circuits, use the sub-circuit designator prefix with ':' as separator (Example X1:R1)
+        """
+        Changes the value of a component, such as a Resistor, Capacitor or Inductor.
+        For components inside sub-circuits, use the sub-circuit designator prefix with ':' as separator (Example X1:R1)
         Usage: ::
 
             LTC.set_component_value('R1', '3.3k')
             LTC.set_component_value('X1:C1', '10u')
 
         :param device: Reference of the circuit element to be updated.
         :type device: str
@@ -640,16 +652,16 @@
                     answer.append(tokens[0])  # Appends only the designators
             except IndexError or TypeError:
                 pass
         return answer
 
     def add_component(self, component: Component, **kwargs) -> None:
         """
-        Adds a component to the netlist. The component is added to the end of the netlist, just before the .END statement.
-        If the component already exists, it will be replaced by the new one.
+        Adds a component to the netlist. The component is added to the end of the netlist,
+        just before the .END statement. If the component already exists, it will be replaced by the new one.
 
         :param component: The component to be added to the netlist
         :type component: Component
         :param kwargs:
             The following keyword arguments are supported:
 
             * **insert_before** (str) - The reference of the component before which the new component should be inserted.
@@ -672,30 +684,30 @@
         model = component.attributes.get('model', 'no_model')
         parameters = " ".join([f"{k}={v}" for k, v in component.attributes.items() if k != 'model'])
         component_line = f"{component.reference} {nodes} {model} {parameters}{END_LINE_TERM}"
         self.netlist.insert(line_no, component_line)
 
     def remove_component(self, designator: str) -> None:
         """
-        Removes a component from  the design.
-        Note: Current implementation only allows removal of a component from the main netlist, not from a sub-circuit.
+        Removes a component from  the design. Current implementation only allows removal of a component
+        from the main netlist, not from a sub-circuit.
 
         :param designator: Component reference in the design. Ex: V1, C1, R1, etc...
         :type designator: str
 
         :return: Nothing
         :raises: ComponentNotFoundError - When the component doesn't exist on the netlist.
         """
         line = self._get_line_starting_with(designator)
         self.netlist[line] = ''  # Blanks the line
 
     @staticmethod
     def add_library_search_paths(paths: Union[str, List[str]]) -> None:
         """
-        Adding search paths for libraries. By default, the local directory and the
+        Adds search paths for libraries. By default, the local directory and the
         ~username/"Documents/LTspiceXVII/lib/sub will be searched forehand. Only when a library is not found in these
         paths then the paths added by this method will be searched.
         Alternatively spicelib.SpiceEditor.LibSearchPaths.append(paths) can be used."
 
         :param paths: Path to add to the Search path
         :type paths: str
         :return: Nothing
@@ -705,15 +717,15 @@
         if isinstance(paths, str):
             LibSearchPaths.append(paths)
         elif isinstance(paths, list):
             LibSearchPaths += paths
 
     def get_all_nodes(self) -> List[str]:
         """
-        A function that retrieves all nodes existing on a Netlist
+        Retrieves all nodes existing on a Netlist.
 
         :returns: Circuit Nodes
         :rtype: list[str]
         """
         circuit_nodes = []
         for line in self.netlist:
             prefix = get_line_command(line)
@@ -723,78 +735,104 @@
                     nodes = match.group('nodes').split()  # This separates by all space characters including \t
                     for node in nodes:
                         if node not in circuit_nodes:
                             circuit_nodes.append(node)
         return circuit_nodes
 
     def save_netlist(self, run_netlist_file: Union[str, Path]) -> None:
+        # docstring is in the parent class
         pass
 
     def add_instruction(self, instruction: str) -> None:
+        # docstring is in the parent class
         pass
 
     def remove_instruction(self, instruction: str) -> None:
+        # docstring is in the parent class
         pass
 
     def remove_Xinstruction(self, search_pattern: str) -> None:
+        # docstring is in the parent class
         pass
 
     @property
     def circuit_file(self) -> Path:
-        """This is only here to avoid breaking compatibility with the BaseEditor superclass. It will always return ''"""
+        """
+        Returns the path of the circuit file. Always returns an empty Path for SpiceCircuit.
+        """
         return Path('')
 
 
 class SpiceEditor(SpiceCircuit):
     """
-    This class implements interfaces to manipulate SPICE netlist files. The class doesn't update the netlist file
+    Provides interfaces to manipulate SPICE netlist files. The class doesn't update the netlist file
     itself. After implementing the modifications the user should call the "save_netlist" method to write a new
     netlist file.
 
     :param netlist_file: Name of the .NET file to parse
     :type netlist_file: str or Path
     :param encoding: Forcing the encoding to be used on the circuit netlile read. Defaults to 'autodetect' which will
-        call a function that tries to detect the encoding automatically. This however is not 100% fool proof.
+        call a function that tries to detect the encoding automatically. This however is not 100% foolproof.
     :param create_blank: Create a blank '.net' file when 'netlist_file' not exist.
     :type encoding: str, optional
     """
 
     def __init__(self, netlist_file: Union[str, Path], encoding='autodetect', create_blank=False):
         super().__init__()
         self.netlist_file = Path(netlist_file)
         self.modified_subcircuits = {}
         if create_blank:
             self.encoding = 'utf-8'  # when user want to create a blank netlist file, and didn't set encoding.
         else:
             if encoding == 'autodetect':
                 try:
-                    self.encoding = detect_encoding(self.netlist_file, '^\* ')  # Normally the file will start with a '*'
+                    self.encoding = detect_encoding(self.netlist_file, r'^\* ')  # Normally the file will start with a '*'
                 except EncodingDetectError as err:
                     raise err
             else:
                 self.encoding = encoding
         self.reset_netlist(create_blank)
 
     @property
     def circuit_file(self) -> Path:
         return self.netlist_file
 
+    def get_component_info(self, component) -> dict:
+        prefix = component[0]
+        if prefix == 'X' and SUBCKT_DIVIDER in component:  # Replaces a component inside of a subciruit
+            # In this case the sub-circuit needs to be copied so that is copy is modified. A copy is created for each
+            # instance of a sub-circuit.
+            component_split = component.split(SUBCKT_DIVIDER)
+            modified_path = SUBCKT_DIVIDER.join(component_split[:-1])  # excludes last component
+            component = component_split[-1]  # This is the last component to modify
+
+            if modified_path in self.modified_subcircuits:  # See if this was already a modified sub-circuit instance
+                subcircuit = self.modified_subcircuits[modified_path]
+            else:
+                subcircuit = self.get_subcircuit(component)
+            return subcircuit.get_component_info(component)
+
+        return super().get_component_info(component)
+
     def _set_model_and_value(self, component, value):
+        """
+        Internal method to set the model and value of a component.
+        """
         prefix = component[0]  # Using the first letter of the component to identify what is it
         if prefix == 'X' and SUBCKT_DIVIDER in component:  # Relaces a component inside of a subciruit
             # In this case the sub-circuit needs to be copied so that is copy is modified. A copy is created for each
             # instance of a sub-circuit.
             component_split = component.split(SUBCKT_DIVIDER)
             modified_path = SUBCKT_DIVIDER.join(component_split[:-1])  # excludes last component
             component = component_split[-1]  # This is the last component to modify
 
             if modified_path in self.modified_subcircuits:  # See if this was already a modified sub-circuit instance
                 sub_circuit = self.modified_subcircuits[modified_path]
             else:
-                sub_circuit_original = self._get_subckt(modified_path)  # If not will look for it.
+                sub_circuit_original = self.get_subcircuit(modified_path)  # If not will look for it.
                 if sub_circuit_original:
                     new_name = sub_circuit_original.name() + '_' + '_'.join(
                         component_split[:-1])  # Creates a new name with the path appended
                     sub_circuit = sub_circuit_original.clone(new_name=new_name)
                     # Memorize that the copy is relative to that particular instance
                     self.modified_subcircuits[modified_path] = sub_circuit
                     # Change the call to the sub-circuit
@@ -804,20 +842,22 @@
             #  Change the copy of the sub-circuit related to that particular instance.
             sub_circuit._set_model_and_value(component, value)
             return
         # else: This is the generic case where the sub-circuit is changed
         super()._set_model_and_value(component, value)
 
     def add_instruction(self, instruction: str) -> None:
-        """Serves to add SPICE instructions to the simulation netlist. For example:
+        """Adds a SPICE instruction to the netlist.
+
+        For example:
 
         .. code-block:: text
 
                   .tran 10m ; makes a transient simulation
-                  .meas TRAN Icurr AVG I(Rs1) TRIG time=1.5ms TARG time=2.5ms" ; Establishes a measuring
+                  .meas TRAN Icurr AVG I(Rs1) TRIG time=1.5ms TARG time=2.5ms ; Establishes a measuring
                   .step run 1 100, 1 ; makes the simulation run 100 times
 
         :param instruction:
             Spice instruction to add to the netlist. This instruction will be added at the end of the netlist,
             typically just before the .BACKANNO statement
         :type instruction: str
         :return: Nothing
@@ -845,44 +885,29 @@
                 line = self.netlist.index(
                     '.backanno\n')  # TODO: Improve this. END of line termination could be differnt and case as well
             except ValueError:
                 line = len(self.netlist) - 2  # This is where typically the .backanno instruction is
             self.netlist.insert(line, instruction)
 
     def remove_instruction(self, instruction) -> None:
-        """Usage a previously added instructions.
-        Example: ::
-
-            LTC.remove_instruction(".STEP run -1 1023 1")
-
-        This only works if the instruction exactly matches the line on the netlist. This means that space characters,
-        and upper case and lower case differences will not match the line.
+        # docstring is in the parent class
 
-        :param instruction: The list of instructions to remove. Each instruction is of the type 'str'
-        :type instruction: str
-        :returns: Nothing
-        """
         # TODO: Make it more intelligent so it recognizes .models, .param and .subckt
         # Because the netlist is stored containing the end of line terminations and because they are added when they
         # they are added to the netlist.
         if not instruction.endswith(END_LINE_TERM):
             instruction += END_LINE_TERM
         if instruction in self.netlist:
             self.netlist.remove(instruction)
             _logger.info(f'Instruction "{instruction}" removed')
         else:
             _logger.error(f'Instruction "{instruction}" not found.')
 
     def remove_Xinstruction(self, search_pattern: str) -> None:
-        """
-        Removes all instructions that match the search pattern.
-        :param search_pattern: The search pattern to be used
-        :type search_pattern: str
-        :return: Nothing
-        """
+        # docstring is in the parent class
         regex = re.compile(search_pattern, re.IGNORECASE)
         i = 0
         instr_removed = False
         while i < len(self.netlist):
             line = self.netlist[i]
             if isinstance(line, str) and regex.match(line):
                 del self.netlist[i]
@@ -890,21 +915,15 @@
                 _logger.info(f'Instruction "{line}" removed')
             else:
                 i += 1
         if not instr_removed:
             _logger.error(f'No instruction matching pattern "{search_pattern}" was found')
 
     def save_netlist(self, run_netlist_file: Union[str, Path]) -> None:
-        """
-        Writes the netlist will all the requested updates into a file named <run_netlist_file>.
-
-        :param run_netlist_file: File name of the netlist file.
-        :type run_netlist_file: Path or str
-        :returns: Nothing
-        """
+        # docstring is in the parent class
         if isinstance(run_netlist_file, str):
             run_netlist_file = Path(run_netlist_file)
         run_netlist_file = run_netlist_file.with_suffix('.net')
         with open(run_netlist_file, 'w', encoding=self.encoding) as f:
             lines = iter(self.netlist)
             for line in lines:
                 if isinstance(line, SpiceCircuit):
@@ -941,15 +960,15 @@
                 #         pass  # print("Ignoring %s" % _)
         else:
             _logger.error("Netlist file not found: {}".format(self.netlist_file))
 
     @staticmethod
     def find_subckt_in_lib(library, subckt_name) -> Union['SpiceCircuit', None]:
         """
-        Finds returns a Subckt from a library file.
+        Finds a sub-circuit in a library. The search is case-insensitive.
 
         :param library: path to the library to search
         :type library: str
         :param subckt_name: sub-circuit to search for
         :type subckt_name: str
         :return: Returns a SpiceCircuit instance with the sub-circuit found or None if not found
         :rtype: SpiceCircuit
@@ -973,50 +992,12 @@
         return None
 
     def run(self, wait_resource: bool = True,
             callback: Callable[[str, str], Any] = None, timeout: float = None, run_filename: str = None, simulator=None):
         """
         *(Deprecated)*
 
-        Convenience function for maintaining legacy with legacy code.
+        Convenience function for maintaining legacy with legacy code. Runs the SPICE simulation.
         """
         from ..sim.sim_runner import SimRunner
         Sim = SimRunner(simulator=simulator)
         return Sim.run(self, wait_resource=wait_resource, callback=callback, timeout=timeout, run_filename=run_filename)
-
-
-if __name__ == '__main__':
-    E = SpiceEditor(os.path.abspath('..\\tests\\PI_Filter_resampled.net'))
-    E.add_instruction(".nodeset V(N001)=0")
-    E.save_netlist('..\\tests\\PI_Filter_resampled_mod.net')
-    E = SpiceEditor('..\\tests\\Editor_Test.net')
-    print("Circuit Nodes", E.get_all_nodes())
-    E.add_library_search_paths([r"C:\SVN\Electronic_Libraries\LTSpice\lib"])
-    E.set_element_model("XU2", 324)
-    E.set_component_value("XU1:XDUT:R77", 200)
-    print(E.get_component_value('R1'))
-    print("Setting R1 to 10k")
-    E.set_component_value('R1', 10000)
-    print("Setting parameter I1 1.23k")
-    E.set_parameter("I1", "1.23k")
-    print(E.get_parameter('I1'))
-    print("Setting {freq*(10/5.0})")
-    E.set_parameters(I2="{freq*(10/5.0})")
-    print(E.get_parameter('I2'))
-    print(E.get_components())
-    print(E.get_components('RC'))
-    print("Setting C1 to 1µF")
-    E.set_component_value("C1", '1µF')
-    print("Setting C4 to 22nF")
-    E.set_component_value("C4", 22e-9)
-    print("Setting C3 to 120nF")
-    E.set_component_value("C3", '120n')
-    print(E.get_component_floatvalue("C1"))
-    print(E.get_component_floatvalue("C3"))
-    print(E.get_component_floatvalue("C4"))
-    E.set_parameters(
-        test_exiting_param_set1=24,
-        test_exiting_param_set2=25,
-        test_exiting_param_set3=26,
-        test_exiting_param_set4=27,
-        test_add_parameter=34.45, )
-    E.save_netlist("..\\tests\\test_spice_editor.net")
```

### Comparing `spicelib-1.0.4/spicelib/log/logfile_data.py` & `spicelib-1.1.1/spicelib/log/logfile_data.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/log/ltsteps.py` & `spicelib-1.1.1/spicelib/log/ltsteps.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,19 +58,20 @@
 
             Measurement: gain
               step	Vout_rms/Vin_rms
                  1	1.99809
                  2	1.99689
 
 
-The ltsteps.py can be used directly from a command line by invoking python with the -m option as exemplified below.
+The ltsteps.exe can be used directly from a command line if the Python's Scripts folder is included in the PATH
+environment variable.
 
 .. code-block:: text
 
-    $ python -m spicelib.LTSteps <path_to_filename>
+    $ ltsteps.exe <path_to_filename>
 
 If `<path_to_filename>` is a log file, it will create a file with the same name, but with extension .tout that is a
 tab separated value (tsv) file, which contains the .STEP and .MEAS information collected.
 
 If `<path_to_filename>` is a txt exported file, it will create a file with the same name, but with extension .tsv a
 tab separated value (tsv) file, which contains data reformatted with the step number as one of the columns. Please
 consult the reformat_LTSpice_export() function for more information.
```

### Comparing `spicelib-1.0.4/spicelib/log/qspice_log_reader.py` & `spicelib-1.1.1/spicelib/log/qspice_log_reader.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/log/semi_dev_op_reader.py` & `spicelib-1.1.1/spicelib/log/semi_dev_op_reader.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/raw/raw_classes.py` & `spicelib-1.1.1/spicelib/raw/raw_classes.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/raw/raw_convert.py` & `spicelib-1.1.1/spicelib/raw/raw_convert.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/raw/raw_read.py` & `spicelib-1.1.1/spicelib/raw/raw_read.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/raw/raw_write.py` & `spicelib-1.1.1/spicelib/raw/raw_write.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/scripts/asc_to_qsch.py` & `spicelib-1.1.1/spicelib/scripts/asc_to_qsch.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 #!/usr/bin/env python
 # coding=utf-8
-import logging
 # -------------------------------------------------------------------------------
 #
 #  ███████╗██████╗ ██╗ ██████╗███████╗██╗     ██╗██████╗
 #  ██╔════╝██╔══██╗██║██╔════╝██╔════╝██║     ██║██╔══██╗
 #  ███████╗██████╔╝██║██║     █████╗  ██║     ██║██████╔╝
 #  ╚════██║██╔═══╝ ██║██║     ██╔══╝  ██║     ██║██╔══██╗
 #  ███████║██║     ██║╚██████╗███████╗███████╗██║██████╔╝
@@ -15,54 +14,52 @@
 #
 # Author:      Nuno Brum (nuno.brum@gmail.com)
 #
 # Created:     16-02-2024
 # Licence:     refer to the LICENSE file
 # -------------------------------------------------------------------------------
 import os
+import logging
 import xml.etree.ElementTree as ET
 
 from spicelib.editor.asy_reader import AsyReader
-from spicelib.editor.base_schematic import ERotation
 from spicelib.editor.asc_editor import AscEditor
-from spicelib.editor.qsch_editor import QschEditor, QschTag
+from spicelib.editor.qsch_editor import QschEditor
+from spicelib.utils.file_search import find_file_in_directory
 
 _logger = logging.getLogger()
 
 
-def find_file_in_directory(directory, filename):
-    """
-    Searches for a file with the given filename in the specified directory and its subdirectories.
-    Returns the path to the file if found, or None if not found.
-    """
-    # First check whether there is a path tagged to the filename
-    path, filename = os.path.split(filename)
-    if path != '':
-        directory = os.path.join(directory, path)
-    for root, dirs, files in os.walk(directory):
-        if filename in files:
-            return os.path.join(root, filename)
-    return None
-
-
 def main():
     """Converts an ASC file to a QSCH schematic"""
-    import sys
     import os.path
+    from optparse import OptionParser
+
+    opts = OptionParser(
+        usage="usage: %prog [options] ASC_FILE [QSCH_FILE]",
+        version="%prog 0.1")
 
-    if len(sys.argv) < 2:
-        print("Usage: asc_to_qsch ASC_FILE [QSCH_FILE]")
-        sys.exit(-1)
-
-    asc_file = sys.argv[1]
-    if len(sys.argv) > 2:
-        qsch_file = sys.argv[2]
+    opts.add_option('-a', "--add", action="append", type="string", dest="path",
+                    help="Add a path for searching for symbols")
+
+    (options, args) = opts.parse_args()
+
+    if len(args) < 1:
+        opts.print_help()
+        exit(-1)
+
+    asc_file = args[0]
+    if len(args) > 1:
+        qsch_file = args[1]
     else:
         qsch_file = os.path.splitext(asc_file)[0] + ".qsch"
 
+    search_paths = [] if options.path is None else options.path
+    symbol_stock = {}
+
     print(f"Using {qsch_file} as output file")
 
     # Open the ASC file
     asc_editor = AscEditor(asc_file)
 
     # import the conversion data from xml file
     # need first to find the file. It is in the same directory as the script
@@ -85,37 +82,40 @@
     asc_editor.scale(offset_x=offset_x, offset_y=offset_y, scale_x=scale_x, scale_y=scale_y)
 
     # Adding symbols to components
     # symbol_stock = {sym.find('LT_name').text: sym for sym in root.findall('component_symbols/symbol')}
     # The symbol_stock has native QSpice symbols and information on how to replace the LTSpice symbols by
     # QSpice ones. For now this is not operational
     for comp in asc_editor.components.values():
-        # TODO: symbol_tree = symbol_stock.get(comp.symbol)
-        symbol_tag = None
-        # if symbol_tree is None:
-        # Will try to get it from the sym folder
-        for sym_root in (
-            os.path.curdir,  # The current script directory
-            os.path.split(asc_file)[0],  # The directory where the scrip is located
-            os.path.expanduser(r"~\AppData\Local\LTspice\lib\sym"),
-            os.path.expanduser(r"~\AppData\Local\Programs\ADI\LTspice\lib.zip"),
-            "A stupid test directory that doesn't exist and that should be skipped"
-        ):
-            if not os.path.exists(sym_root):  # Skipping invalid paths
-                continue
-            if sym_root.endswith('.zip'):  # TODO: test if it is a file
-                pass  # TODO: implement this
-                # Using an IO buffer to pass the file to the AsyEditor
-            else:
-                symbol_asc_file = find_file_in_directory(sym_root, comp.symbol + '.asy')
-            if symbol_asc_file is not None:
-                symbol_asc = AsyReader(symbol_asc_file)
-                value = comp.attributes.get('Value', '<val>')
-                symbol_tag = symbol_asc.to_qsch(comp.reference, value)
-                break
+        symbol_tag = symbol_stock.get(comp.symbol, None)
+        if symbol_tag is None:
+            # Will try to get it from the sym folder
+            print(f"Searching for symbol {comp.symbol}...")
+            for sym_root in search_paths + [
+                # os.path.curdir,  # The current script directory
+                os.path.split(asc_file)[0],  # The directory where the scrip is located
+                os.path.expanduser(r"~\AppData\Local\LTspice\lib\sym"),
+                os.path.expanduser(r"~\Documents\LtspiceXVII\lib\sym"),
+                # os.path.expanduser(r"~\AppData\Local\Programs\ADI\LTspice\lib.zip"), # TODO: implement this
+            ]:
+                print(f"   {os.path.abspath(sym_root)}")
+                if not os.path.exists(sym_root):  # Skipping invalid paths
+                    continue
+                if sym_root.endswith('.zip'):  # TODO: test if it is a file
+                    pass
+                    # Using an IO buffer to pass the file to the AsyEditor
+                else:
+                    symbol_asc_file = find_file_in_directory(sym_root, comp.symbol + '.asy')
+                    if symbol_asc_file is not None:
+                        print(f"Found {symbol_asc_file}")
+                        symbol_asc = AsyReader(symbol_asc_file)
+                        value = comp.attributes.get('Value', '<val>')
+                        symbol_tag = symbol_asc.to_qsch(comp.reference, value)
+                        symbol_stock[comp.symbol] = symbol_tag
+                        break
 
         # if symbol_tree:
         #     name = symbol_tree.find("name").text
         #     offset = symbol_tree.find('LT_origin')
         #     offset_x = int(offset.get('x'))
         #     offset_y = int(offset.get('y'))
         #
@@ -151,19 +151,19 @@
         #     elif rotation == 'R180':
         #         comp.rotation = comp.rotation + ERotation.R180
         #     elif rotation == 'R270':
         #         comp.rotation = comp.rotation + ERotation.R270
         #     elif rotation == 'M0':
         #         comp.rotation = comp.rotation.mirror_x_axis()
         #     elif rotation == 'M90':
-        #         comp.rotation = comp.rotation  # TODO
+        #         comp.rotation = comp.rotation
         #     elif rotation == 'M180':
         #         comp.rotation = comp.rotation.M180
         #     elif rotation == 'M270':
-        #         comp.rotation = comp.rotation  # TODO
+        #         comp.rotation = comp.rotation
         #
         #     # typ = symbol_tree.find("type").text
         #     # description = symbol_tree.find("description").text
         #
         #     symbol_tag = QschTag("symbol", name)
         #     # symbol_tag.items.append(QschTag("type", typ))
         #     # symbol_tag.items.append(QschTag("description:", description))
```

### Comparing `spicelib-1.0.4/spicelib/scripts/asc_to_qsch_data.xml` & `spicelib-1.1.1/spicelib/scripts/asc_to_qsch_data.xml`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/scripts/histogram.py` & `spicelib-1.1.1/spicelib/scripts/histogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
         if logfile.endswith(".log"):
             # Maybe it is a LTSpice log file
             from spicelib.log.ltsteps import LTSpiceLogReader
             try:
                 log = LTSpiceLogReader(logfile)
             except EncodingDetectError:
-                print("Failed to load file '%s'. Use LTSteps first to convert to tlog format" % logfile)
+                print("Failed to load file '%s'. Use ltsteps.exe first to convert to tlog format" % logfile)
                 exit(-1)
             else:
                 if options.filters is None:
                     values = log.get_measure_values_at_steps(TRACE, None)
                 else:
                     # This implementation only allows equal operators
                     filters = {}
```

### Comparing `spicelib-1.0.4/spicelib/scripts/ltsteps.py` & `spicelib-1.1.1/spicelib/scripts/ltsteps.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,19 +57,20 @@
 
             Measurement: gain
               step	Vout_rms/Vin_rms
                  1	1.99809
                  2	1.99689
 
 
-The ltsteps.py can be used directly from a command line by invoking python with the -m option as exemplified below.
+The ltsteps.exe can be used directly from a command line if the Python's Scripts folder is included in the PATH
+environment variable.
 
 .. code-block:: text
 
-    $ python -m spicelib.LTSteps <path_to_filename>
+    $ ltsteps.exe <path_to_filename>
 
 If `<path_to_filename>` is a log file, it will create a file with the same name, but with extension .tout that is a
 tab separated value (tsv) file, which contains the .STEP and .MEAS information collected.
 
 If `<path_to_filename>` is a txt exported file, it will create a file with the same name, but with extension .tsv a
 tab separated value (tsv) file, which contains data reformatted with the step number as one of the columns. Please
 consult the reformat_LTSpice_export() function for more information.
```

### Comparing `spicelib-1.0.4/spicelib/scripts/rawplot.py` & `spicelib-1.1.1/spicelib/scripts/rawplot.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/scripts/readme_update.py` & `spicelib-1.1.1/spicelib/scripts/readme_update.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,17 +5,24 @@
 import os
 import sys
 import re
 from shutil import copyfile
 
 # Read the README.md on the path indicated on the command line arguments
 filename = sys.argv[1]
-
-readme_md = open(filename).readlines()
-
+print(f"Reading \"{filename}\"", end="...")
+try:
+    readme_md = open(filename).readlines()
+except FileNotFoundError:
+    print("File not found")
+    exit(1)
+except Exception as e:
+    print(f"Error reading file: {e}")
+    exit(1)
+print(f"{len(readme_md)} lines read")
 in_statement_regex = re.compile(r"-- in (?P<path>.*?)(?P<loc>\s\[.*\])?$")
 
 block_start = -1
 line_no = 0
 # detect python code blocks
 while line_no < len(readme_md):
     line = readme_md[line_no]
@@ -23,14 +30,15 @@
         block_start = line_no
     elif "```" in line and block_start != -1:
         # check whether the next line has the -- in statement
         if line_no + 1 < len(readme_md):
             m = in_statement_regex.search(readme_md[line_no + 1])
             # find the file to include
             if m:
+                print(f"Updating code on lines {block_start+1}:{line_no + 1}")
                 include_relpath = m.group("path")
                 include_path = os.path.abspath(os.path.join(os.curdir, include_relpath))
                 include_text = open(include_path, "r", encoding="utf-8").readlines()
                 # if there is a localization, isolate only the part identified by loc
                 # the part starts with "# -- Start of <loc> --" and ends with "# -- End of <loc> --"
                 # where <loc> is the text within the square brackets [] in the readme.md
                 if (loc := m.group("loc")) is not None:
@@ -52,13 +60,17 @@
                                     lines_to_plug.append(line1[include_ident:])
                 else:
                     lines_to_plug = include_text
                 existing_lines = line_no - (block_start + 1)  # This accounts for the start and finish ``` line
                 new_lines = len(lines_to_plug)
                 readme_md[block_start + 1:line_no] = lines_to_plug
                 line_no += new_lines - existing_lines
+        block_start = -1
     line_no += 1
 
 # Finally write back the readme.md but first create a backup
-copyfile(filename, filename.replace(".md", ".bak"))
+backup_filename = filename.replace(".md", ".bak")
+print(f"Creating backup {backup_filename}")
+copyfile(filename, backup_filename)
+print(f"Writing {len(readme_md)} lines to {filename}")
 open(filename, 'w').writelines(readme_md)
 exit(0)
```

### Comparing `spicelib-1.0.4/spicelib/scripts/run_server.py` & `spicelib-1.1.1/spicelib/scripts/run_server.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/sim/process_callback.py` & `spicelib-1.1.1/spicelib/sim/process_callback.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/sim/run_task.py` & `spicelib-1.1.1/spicelib/sim/run_task.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/sim/sim_runner.py` & `spicelib-1.1.1/spicelib/sim/sim_runner.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/sim/sim_stepping.py` & `spicelib-1.1.1/spicelib/sim/sim_stepping.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/sim/simulator.py` & `spicelib-1.1.1/spicelib/sim/simulator.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/sim/tookit/failure_modes.py` & `spicelib-1.1.1/spicelib/sim/tookit/failure_modes.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/sim/tookit/fast_worst_case.py` & `spicelib-1.1.1/spicelib/sim/tookit/fast_worst_case.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/sim/tookit/montecarlo.py` & `spicelib-1.1.1/spicelib/sim/tookit/montecarlo.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/sim/tookit/quick_sensitivity_analysis.py` & `spicelib-1.1.1/spicelib/sim/tookit/quick_sensitivity_analysis.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/sim/tookit/sim_analysis.py` & `spicelib-1.1.1/spicelib/sim/tookit/sim_analysis.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/sim/tookit/tolerance_deviations.py` & `spicelib-1.1.1/spicelib/sim/tookit/tolerance_deviations.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/sim/tookit/worst_case.py` & `spicelib-1.1.1/spicelib/sim/tookit/worst_case.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/simulators/ltspice_simulator.py` & `spicelib-1.1.1/spicelib/simulators/ltspice_simulator.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/simulators/ngspice_simulator.py` & `spicelib-1.1.1/spicelib/simulators/ngspice_simulator.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/simulators/qspice_simulator.py` & `spicelib-1.1.1/spicelib/simulators/qspice_simulator.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/simulators/xyce_simulator.py` & `spicelib-1.1.1/spicelib/simulators/xyce_simulator.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/utils/detect_encoding.py` & `spicelib-1.1.1/spicelib/utils/detect_encoding.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib/utils/sweep_iterators.py` & `spicelib-1.1.1/spicelib/utils/sweep_iterators.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/spicelib.egg-info/PKG-INFO` & `spicelib-1.1.1/spicelib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spicelib
-Version: 1.0.4
+Version: 1.1.1
 Summary: A set of tools to Automate Spice simulations
 Author-email: Nuno Brum <me@nunobrum.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -702,15 +702,15 @@
   * LTspice
   * NGSpice
   * QSPICE
   * Xyce
 
 ## What is contained in this repository ##
 
-* __LTSteps.py__
+* __ltsteps.exe__
   An utility that extracts from LTSpice output files data, and formats it for import in a spreadsheet, such like Excel
   or Calc.
 
 * __raw_read.py__
   A pure python class that serves to read raw files into a python class.
 
 * __raw_write.py__
@@ -731,25 +731,25 @@
 * __sim_runner.py__
   A python script that can be used to run LTSpice simulations in batch mode without having to open the LTSpice GUI.
   This in cooperation with the classes defined in spice_editor.py or asc_editor.py is useful because:
 
     - Can overcome the limitation of only stepping 3 parameters
     - Different types of simulations .TRAN .AC .NOISE can be run in a single batch
     - The RAW Files are smaller and easier to treat
-    - When used with the RawRead.py and LTSteps.py, validation of the circuit can be done automatically.
+    - When used with the RawRead.py and ltsteps.py, validation of the circuit can be done automatically.
     - Different models can be simulated in a single batch, by using the following instructions:
 
   Note: It was only tested with Windows based installations.
 
 * __Analysis Toolkit__
   A set of tools that prepare an LTSpice netlist for a Montecarlo or Worst Case Analysis. The device tolerances are set
   by the user and the netlist is updated accordingly. The netlist can then be used with the sim_runner.py to run a 
   batch of simulations or with the LTSpice GUI.
 
-* __Histogram.py__
+* __histogram.exe__
   A python script that uses numpy and matplotlib to create a histogram and calculate the sigma deviations. This is
   useful for Monte-Carlo analysis.
 
 ## How to Install ##
 
 `pip install spicelib`
 
@@ -783,15 +783,15 @@
 "TRAN - STEP.raw" and displays all steps of the "I(R1)" trace in a matplotlib plot
 
  ```python
 from spicelib import RawRead
 
 from matplotlib import pyplot as plt
 
-rawfile = RawRead("TRAN - STEP.raw")
+rawfile = RawRead("./testfiles/TRAN - STEP.raw")
 
 print(rawfile.get_trace_names())
 print(rawfile.get_raw_property())
 
 IR1 = rawfile.get_trace("I(R1)")
 x = rawfile.get_trace('time')  # Gets the time axis
 steps = rawfile.get_steps()
@@ -807,30 +807,30 @@
 ### RawWrite ###
 
 The following example writes a RAW file with a 3 milliseconds transient simulation sine with a 10kHz and a cosine with
 9.997kHz
 
  ```python
 import numpy as np
-from spicelib import RawRead, Trace, RawWrite
+from spicelib import Trace, RawWrite
 LW = RawWrite(fastacces=False)
 tx = Trace('time', np.arange(0.0, 3e-3, 997E-11))
 vy = Trace('N001', np.sin(2 * np.pi * tx.data * 10000))
 vz = Trace('N002', np.cos(2 * np.pi * tx.data * 9970))
 LW.add_trace(tx)
 LW.add_trace(vy)
 LW.add_trace(vz)
 LW.save("./testfiles/teste_snippet1.raw")
  ```
 -- in examples/raw_write_example.py [Example 1]
 
 ### SpiceEditor, AscEditor and SimRunner.py ###
 
 This module is used to launch LTSPice simulations. Results then can be processed with either the RawRead or with the
-LTSteps module to read the log file which can contain .MEAS results.
+LTSpiceLogReader module to read the log file which can contain .MEAS results.
 
 The script will firstly invoke the LTSpice in command line to generate a netlist, and then this netlist can be updated
 directly by the script, in order to change component values, parameters or simulation commands.
 
 Here follows an example of operation.
 
 ```python
@@ -862,15 +862,15 @@
         print("simulating OpAmp", opamp, "Voltage", supply_voltage)
         LTC.run(netlist)
 
 for raw, log in LTC:
     print("Raw file: %s, Log file: %s" % (raw, log))
     # do something with the data
     # raw_data = RawRead(raw)
-    # log_data = LTSteps(log)
+    # log_data = LTSpiceLogReader(log)
     # ...
 
 netlist.reset_netlist()
 netlist.add_instructions(
     "; Simulation settings",
     ".ac dec 30 10 1Meg",
     ".meas AC Gain MAX mag(V(out)) ; find the peak response and call it ""Gain""",
@@ -900,15 +900,14 @@
 ![Sallen-Key Amplifier](./doc/modules/sallenkey.png "Sallen-Key Amplifier")
 
 When performing a Monte Carlo simulation on this circuit, we need to manually modify the value of each component, 
 and then add the .step command for making several runs on the same circuit. 
 To simplify this process, the AscEditor class can be used as exemplified below:
 
 ```python
-import numpy as np
 from spicelib import AscEditor, SimRunner  # Imports the class that manipulates the asc file
 from spicelib.sim.tookit.montecarlo import Montecarlo  # Imports the Montecarlo toolkit class
 from spicelib.simulators.ltspice_simulator import LTspice
 
 sallenkey = AscEditor("./testfiles/sallenkey.asc")  # Reads the asc file into memory
 runner = SimRunner(simulator=LTspice, output_folder='./temp_mc',
                    verbose=True)  # Instantiates the runner with a temp folder set
@@ -969,15 +968,15 @@
 # wca.set_tolerance('V', 0.1)  # 10% tolerance. For Worst Case analysis, the distribution is irrelevant
 wca.set_tolerance('I', 0.1)  # 10% tolerance. For Worst Case analysis, the distribution is irrelevant
 # Some components can have a different tolerance
 wca.set_tolerance('R1', 0.05)  # 5% tolerance for R1 only. This only overrides the default tolerance for R1
 wca.set_tolerance('R4', 0.0)  # 5% tolerance for R1 only. This only overrides the default tolerance for R1
 
 # Tolerances can be set for parameters as well.
-# wca.set_parameter_deviation('Vos', 3e-4, 5e-3)
+wca.set_parameter_deviation('Vos', 3e-4, 5e-3)
 
 # Finally the netlist is saved to a file
 wca.save_netlist('./testfiles/sallenkey_wc.asc')
 ```
 -- in examples/run_worst_case.py [Example 1]
 
 When opening the created sallenkey_wc.net file, we can see that the following circuit.
@@ -996,15 +995,15 @@
 - A default value for the run parameter was added. This is useful if the .step param run is commented out.
 - The R1 tolerance is different from the other resistors. This is because the tolerance was explicitly set for R1.
 - The wc() function is added to the circuit. This function is used to calculate the worst case value for each component,
 given a tolerance value and its respective index.
 - The wc1() function is added to the circuit. This function is used to calculate the worst case value for each component,
 given a minimum and maximum value and its respective index.
 
-### LTSteps.py ###
+### ltsteps.py ###
 
 This module defines a class that can be used to parse LTSpice log files where the information about .STEP information is
 written. There are two possible usages of this module, either programmatically by importing the module and then
 accessing data through the class as exemplified here:
 
 ```python
 #!/usr/bin/env python
@@ -1096,27 +1095,39 @@
 
 This module is used to run a server that can be used to run simulations in a remote machine. The server will run in the
 background and will wait for a client to connect. The client will send a netlist to the server and the server will run
 the simulation and return the results to the client. The client on the remote machine is a script instancing the
 SimClient class. An example of its usage is shown below:
 
 ```python
+import os
+import zipfile
+import logging
+
+# In order for this, to work, you need to have a server running. To start a server, run the following command:
+# python -m spicelib.run_server --port 9000 --parallel 4 --output ./temp
+
+_logger = logging.getLogger("spicelib.SimClient")
+_logger.setLevel(logging.DEBUG)
+
 from spicelib.client_server.sim_client import SimClient
 
 server = SimClient('http://localhost', 9000)
 print(server.session_id)
 runid = server.run("./testfiles/testfile.net")
 print("Got Job id", runid)
 for runid in server:  # Ma
     zip_filename = server.get_runno_data(runid)
     print(f"Received {zip_filename} from runid {runid}")
     with zipfile.ZipFile(zip_filename, 'r') as zipf:  # Extract the contents of the zip file
         print(zipf.namelist())  # Debug printing the contents of the zip file
         zipf.extract(zipf.namelist()[0])  # Normally the raw file comes first
     os.remove(zip_filename)  # Remove the zip file
+
+server.close_session()
 ```
 -- in examples/sim_client_example.py [SimClient Example]
 
 ```bash
 usage: run_server [-h] [-p PORT] [-o OUTPUT] [-l PARALLEL] simulator
 
 Run the LTSpice Server. This is a command line interface to the SimServer class.The SimServer class is used to run
@@ -1174,14 +1185,27 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 1.1.1
+  * Supporting hierarchical edits on both QSpice and LTspice schematics
+  * Skipping the need of the rich library on examples
+  * Giving feedback on the search for symbols on the ASC to QSCH conversion
+  * Improvement on Documentation
+  * Adding examples and unittests on hiearchical edits
+  * Giving access to hidden properties (asc_file_path in AscEditor and qsch_file_path in QschEditor)
+  * Refactoring save_netlist() method in QschEditor class
+  * Supporting arcs and rectangles on AsyReader
+  * Adding file_search.py containing utility functions for searching files
+  * Adding windows_short_names.py containing a code to get the 8.3 Windows short names.
+* Version 1.1.0
+  * First usable version of a LTspice to Qspice schematic converter.
 * Version 1.0.4
   * Adding the missing the asc_to_qsch_data.xml to the package
   * Adding a MANIFEST.in to the project
   * Adding keywords to the project.toml
 * Version 1.0.3
   * Correcting the generation of a .net from the QschEditor.
 * Version 1.0.2
```

### Comparing `spicelib-1.0.4/spicelib.egg-info/SOURCES.txt` & `spicelib-1.1.1/spicelib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 examples/sim_runner_asc_example.py
 examples/sim_runner_callback_example.py
 examples/sim_runner_callback_process_example.py
 examples/sim_runner_example.py
 examples/sim_server_example.py
 examples/sim_stepper_example.py
 examples/spice_editor_example.py
+examples/sub_circuit_asc_edits.py
+examples/sub_circuit_edits.py
+examples/sub_circuit_qsch_edits.py
 spicelib/__init__.py
 spicelib.egg-info/PKG-INFO
 spicelib.egg-info/SOURCES.txt
 spicelib.egg-info/dependency_links.txt
 spicelib.egg-info/entry_points.txt
 spicelib.egg-info/requires.txt
 spicelib.egg-info/top_level.txt
@@ -71,14 +74,16 @@
 spicelib/sim/tookit/worst_case.py
 spicelib/simulators/__init__.py
 spicelib/simulators/ltspice_simulator.py
 spicelib/simulators/ngspice_simulator.py
 spicelib/simulators/qspice_simulator.py
 spicelib/simulators/xyce_simulator.py
 spicelib/utils/detect_encoding.py
+spicelib/utils/file_search.py
 spicelib/utils/sweep_iterators.py
+spicelib/utils/windows_short_names.py
 unittests/sweep_iterators_unittest.py
 unittests/test_asc_editor.py
 unittests/test_qsch_editor.py
 unittests/test_qspice_rawread.py
 unittests/test_spice_editor.py
 unittests/test_spicelib.py
```

### Comparing `spicelib-1.0.4/unittests/sweep_iterators_unittest.py` & `spicelib-1.1.1/unittests/sweep_iterators_unittest.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/unittests/test_asc_editor.py` & `spicelib-1.1.1/unittests/test_asc_editor.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/unittests/test_qsch_editor.py` & `spicelib-1.1.1/unittests/test_qsch_editor.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         lines2 = f2.readlines()
     testcase.assertEqual(len(lines1), len(lines2), "Files have different number of lines")
     for i in range(len(lines1)):
         data1 = lines1[i].strip()  # Remove white spaces and line terminators
         data2 = lines2[i].strip()
         if data1.startswith('*') and data2.startswith('*'):
             continue  # Skip comments
-        testcase.assertEqual(data1, data2, "Files are not equal")
+        testcase.assertEqual(data1, data2, f"Files \"{file1}\" and \"{file2}\" are not equal")
     
 
 class ASC_Editor_Test(unittest.TestCase):
 
     def setUp(self):
         self.edt = spicelib.editor.qsch_editor.QschEditor(test_dir + "DC sweep.qsch")
 
@@ -99,9 +99,20 @@
         self.qsch = spicelib.editor.qsch_editor.QschEditor(test_dir + 'qsch_rotation_set_test.qsch')
         for rotation in range(0, 360, 45):
             self.qsch.set_component_position('R1', (0, 0), rotation)
             self.qsch.save_netlist(temp_dir + f'qsch_rotation_set_{rotation}.qsch')
             equalFiles(self, temp_dir + f'qsch_rotation_set_{rotation}.qsch', golden_dir + f"qsch_rotation_set_{rotation}.qsch")
 
 
+class QschEditorSpiceGeneration(unittest.TestCase):
+
+    def test_hierarchical(self):
+        self.edt = spicelib.editor.qsch_editor.QschEditor(test_dir + "top_circuit.qsch")
+        self.edt.save_netlist(temp_dir + "top_circuit.net")
+        if sys.platform.startswith("win"):
+            equalFiles(self, temp_dir + 'top_circuit.net', golden_dir + "top_circuit_win32.net")
+        else:
+            equalFiles(self, temp_dir + 'top_circuit.net', golden_dir + "top_circuit.net")
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `spicelib-1.0.4/unittests/test_qspice_rawread.py` & `spicelib-1.1.1/unittests/test_qspice_rawread.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         SE.set_component_value('V1', 'AC 1 0')
         runner.run(SE, callback=callback_function)
         runner.wait_completion()
         self.assertEqual(runner.okSim, 5)  # Simulation done with success
 
     @unittest.skipIf(skip_qspice_editor_tests, "Execute All")
     def test_ltsteps_measures(self):
-        """LTSteps Measures from Batch_Test.asc"""
+        """QspiceLogReader Measures from Batch_Test.asc"""
         print("Starting test_ltsteps_measures")
         assert_data = {
             'vout1m'   : [
                 -0.0186257,
                 -1.04378,
                 -1.64283,
                 -0.622014,
```

### Comparing `spicelib-1.0.4/unittests/test_spice_editor.py` & `spicelib-1.1.1/unittests/test_spice_editor.py`

 * *Files identical despite different names*

### Comparing `spicelib-1.0.4/unittests/test_spicelib.py` & `spicelib-1.1.1/unittests/test_spicelib.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,15 +201,15 @@
         SE.add_instruction('.ac dec 40 1m 1G')
         SE.set_component_value('V1', 'AC 1 0')
         LTC.run(SE, callback=callback_function)
         LTC.wait_completion()
 
     @unittest.skipIf(False, "Execute All")
     def test_ltsteps_measures(self):
-        """LTSteps Measures from Batch_Test.asc"""
+        """LTSpiceLogReader Measures from Batch_Test.asc"""
         print("Starting test_ltsteps_measures")
         assert_data = {
             'vout1m'   : [
                 -0.0186257,
                 -1.04378,
                 -1.64283,
                 -0.622014,
```

