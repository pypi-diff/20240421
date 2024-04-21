# Comparing `tmp/qutip-qip-0.2.3.tar.gz` & `tmp/qutip-qip-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/qutip-qip/qutip-qip/dist/.tmp-hpepzl8h/qutip-qip-0.2.3.tar", last modified: Mon Dec 12 22:41:11 2022, max compression
+gzip compressed data, was "/home/runner/work/qutip-qip/qutip-qip/dist/.tmp-rj2kv_76/qutip-qip-0.3.0.tar", last modified: Wed Jul 19 13:11:41 2023, max compression
```

## Comparing `qutip-qip-0.2.3.tar` & `qutip-qip-0.3.0.tar`

### file list

```diff
@@ -1,85 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1538 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      130 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     6148 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      153 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)       34 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3678 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/src/qutip_qip/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/src/qutip_qip/_decompose/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/_decompose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/_decompose/_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/_decompose/decompose_single_qubit_gate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/src/qutip_qip/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/algorithms/qft.py
--rw-r--r--   0 runner    (1001) docker     (123)    85187 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/circuit_latex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/src/qutip_qip/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/compiler/cavityqedcompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7946 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/compiler/circuitqedcompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    17517 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/compiler/gatecompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/compiler/instruction.py
--rw-r--r--   0 runner    (1001) docker     (123)    23583 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/compiler/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8180 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/compiler/spinchaincompiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/src/qutip_qip/device/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/device/cavityqed.py
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/device/circuitqed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/device/modelprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/device/optpulseprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    45804 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/device/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13332 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/device/spinchain.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/gates.py
--rw-r--r--   0 runner    (1001) docker     (123)    20285 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/noise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/src/qutip_qip/operations/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59654 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/operations/gates.py
--rw-r--r--   0 runner    (1001) docker     (123)    22587 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/pulse.py
--rw-r--r--   0 runner    (1001) docker     (123)    38243 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/qasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/qubits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/src/qutip_qip/transpiler/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/transpiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/src/qutip_qip/transpiler/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/src/qutip_qip/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/src/qutip_qip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7261 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/src/qutip_qip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/src/qutip_qip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/src/qutip_qip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/src/qutip_qip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/src/qutip_qip.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/tests/decomposition_functions/
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/decomposition_functions/test_single_qubit_gate_decompositions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/decomposition_functions/test_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-12 22:41:11.000000 qutip-qip-0.2.3/tests/qasm_files/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/qasm_files/bracket_error.qasm
--rw-r--r--   0 runner    (1001) docker     (123)      167 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/qasm_files/command_error.qasm
--rw-r--r--   0 runner    (1001) docker     (123)      155 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/qasm_files/qasm_error.qasm
--rw-r--r--   0 runner    (1001) docker     (123)      232 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/qasm_files/qft.qasm
--rw-r--r--   0 runner    (1001) docker     (123)      199 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/qasm_files/teleportation.qasm
--rw-r--r--   0 runner    (1001) docker     (123)      135 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/qasm_files/test_add.qasm
--rw-r--r--   0 runner    (1001) docker     (123)      332 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/qasm_files/test_custom_gates.qasm
--rw-r--r--   0 runner    (1001) docker     (123)      329 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/qasm_files/w-state.qasm
--rw-r--r--   0 runner    (1001) docker     (123)    30347 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/test_circuit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7720 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10223 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)    15176 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/test_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/test_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9640 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/test_optpulseprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16523 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/test_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/test_pulse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/test_qasm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/test_qft.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/test_qubits.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2022-12-12 22:40:57.000000 qutip-qip-0.2.3/tests/test_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1538 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6148 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3678 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/src/qutip_qip/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/src/qutip_qip/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/algorithms/qft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/src/qutip_qip/circuit/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/circuit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19984 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/circuit/_decompose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41949 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/circuit/circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/circuit/circuit_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23944 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/circuit/circuitsimulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/src/qutip_qip/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/compiler/cavityqedcompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8007 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/compiler/circuitqedcompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17529 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/compiler/gatecompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/compiler/instruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23583 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/compiler/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8228 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/compiler/spinchaincompiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/src/qutip_qip/decompose/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/decompose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/decompose/_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/decompose/decompose_single_qubit_gate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/src/qutip_qip/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/device/cavityqed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/device/circuitqed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/device/modelprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/device/optpulseprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46017 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/device/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13332 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/device/spinchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20285 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/noise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/src/qutip_qip/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33945 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/operations/gateclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38017 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/operations/gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/operations/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/pulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38879 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/qir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/src/qutip_qip/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/qiskit/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/qiskit/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/qiskit/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/qiskit/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/qubits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/src/qutip_qip/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/transpiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/transpiler/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/src/qutip_qip/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29323 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/src/qutip_qip/vqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/src/qutip_qip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/src/qutip_qip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/src/qutip_qip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/src/qutip_qip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/src/qutip_qip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/src/qutip_qip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/tests/decomposition_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/decomposition_functions/test_single_qubit_gate_decompositions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/decomposition_functions/test_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 13:11:41.000000 qutip-qip-0.3.0/tests/qasm_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/qasm_files/bracket_error.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/qasm_files/command_error.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/qasm_files/qasm_error.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/qasm_files/qft.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/qasm_files/teleportation.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/qasm_files/test_add.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/qasm_files/test_custom_gates.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/qasm_files/w-state.qasm
+-rw-r--r--   0 runner    (1001) docker     (123)    28771 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/test_circuit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7720 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17457 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/test_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/test_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/test_optpulseprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16166 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/test_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/test_pulse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/test_qasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/test_qft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/test_qir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8748 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/test_qiskit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/test_qubits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-07-19 13:11:31.000000 qutip-qip-0.3.0/tests/test_vqa.py
```

### Comparing `qutip-qip-0.2.3/LICENSE` & `qutip-qip-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qutip-qip-0.2.3/PKG-INFO` & `qutip-qip-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qutip-qip
-Version: 0.2.3
+Version: 0.3.0
 Summary: The QuTiP quantum information processing package
 Home-page: https://github.com/qutip/qutip-qip
 Author: Alexander Pitchford, Paul D. Nation, Robert J. Johansson, Chris Granade, Arne Grimsmo, Nathan Shammah, Shahnawaz Ahmed, Neill Lambert, Eric Giguere, Boxi Li, Jake Lishman
 Author-email: qutip-admin@googlegroups.com
 License: BSD 3-Clause License
 Keywords: quantum,physics,dynamics
 Platform: Linux
@@ -21,14 +21,15 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown; variant=GFM
 Provides-Extra: graphics
 Provides-Extra: tests
 Provides-Extra: full
+Provides-Extra: qiskit
 License-File: LICENSE
 
 # qutip-qip
 
 [![build](https://github.com/qutip/qutip-qip/workflows/Tests/badge.svg)](https://github.com/qutip/qutip-qip/actions)
 [![Documentation Status](https://readthedocs.org/projects/qutip-qip/badge/?version=stable)](https://qutip-qip.readthedocs.io/en/stable/)
 [![PyPI version](https://badge.fury.io/py/qutip-qip.svg)](https://badge.fury.io/py/qutip-qip)
```

### Comparing `qutip-qip-0.2.3/README.md` & `qutip-qip-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `qutip-qip-0.2.3/setup.cfg` & `qutip-qip-0.3.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -41,12 +41,14 @@
 [options.extras_require]
 graphics = matplotlib>=1.3.0
 tests = 
 	pytest>=5.2
 full = 
 	%(graphics)s
 	%(tests)s
+qiskit = 
+	qiskit>=0.36.2
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `qutip-qip-0.2.3/setup.py` & `qutip-qip-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `qutip-qip-0.2.3/src/qutip_qip/_decompose/_utility.py` & `qutip-qip-0.3.0/src/qutip_qip/decompose/_utility.py`

 * *Files identical despite different names*

### Comparing `qutip-qip-0.2.3/src/qutip_qip/_decompose/decompose_single_qubit_gate.py` & `qutip-qip-0.3.0/src/qutip_qip/decompose/decompose_single_qubit_gate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 import cmath
 
 
-from qutip_qip._decompose._utility import (
+from qutip_qip.decompose._utility import (
     check_gate,
     MethodError,
 )
 
-from qutip_qip.circuit import Gate
+from qutip_qip.operations import Gate
 
 
 __all__ = ["decompose_one_qubit_gate"]
 
 
 def _angles_for_ZYZ(input_gate):
     """Finds and returns the angles for ZYZ rotation matrix. These are
```

### Comparing `qutip-qip-0.2.3/src/qutip_qip/algorithms/qft.py` & `qutip-qip-0.3.0/src/qutip_qip/algorithms/qft.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 This module provides the circuit implementation for Quantum Fourier Transform.
 """
 
 
 import numpy as np
-from ..operations import Gate, snot, cphase, swap
+from ..operations import Gate, snot, cphase, swap, expand_operator
 from ..circuit import QubitCircuit
 from qutip import Qobj
-from qutip_qip._decompose import decompose_one_qubit_gate
+from ..decompose import decompose_one_qubit_gate
 
 
 __all__ = ["qft", "qft_steps", "qft_gate_sequence"]
 
 
 def qft(N=1):
     """
@@ -65,21 +65,30 @@
     U_step_list = []
     if N == 1:
         U_step_list.append(snot())
     else:
         for i in range(N):
             for j in range(i):
                 U_step_list.append(
-                    cphase(np.pi / (2 ** (i - j)), N, control=i, target=j)
+                    expand_operator(
+                        cphase(np.pi / (2 ** (i - j))),
+                        dims=[2] * N,
+                        targets=[i, j],
+                    )
                 )
-            U_step_list.append(snot(N, i))
+            U_step_list.append(
+                expand_operator(snot(), dims=[2] * N, targets=i)
+            )
         if swapping:
             for i in range(N // 2):
-                U_step_list.append(swap(N, [N - i - 1, i]))
-
+                U_step_list.append(
+                    expand_operator(
+                        swap(), dims=[2] * N, targets=[N - i - 1, i]
+                    )
+                )
     return U_step_list
 
 
 def qft_gate_sequence(N=1, swapping=True, to_cnot=False):
     """
     Quantum Fourier Transform operator on N qubits returning the gate sequence.
```

### Comparing `qutip-qip-0.2.3/src/qutip_qip/circuit_latex.py` & `qutip-qip-0.3.0/src/qutip_qip/circuit/circuit_latex.py`

 * *Files identical despite different names*

### Comparing `qutip-qip-0.2.3/src/qutip_qip/compiler/cavityqedcompiler.py` & `qutip-qip-0.3.0/src/qutip_qip/compiler/cavityqedcompiler.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,18 +58,18 @@
     >>> qc.add_gate("ISWAP", targets=[0, 1])
     >>>
     >>> model = CavityQEDModel(2)
     >>> processor = ModelProcessor(model=model)
     >>> compiler = CavityQEDCompiler(2, params=model.params)
     >>> processor.load_circuit(
     ...     qc, compiler=compiler)  # doctest: +NORMALIZE_WHITESPACE
-    ({'sz0': array([   0.        , 2500.        , 2500.01315789]),
-    'sz1': array([   0.        , 2500.        , 2500.01315789]),
-    'g0': array([   0.        , 2500.        , 2500.01315789]),
-    'g1': array([   0.        , 2500.        , 2500.01315789])},
+    ({'sz0': array([   0.        , 2500.        , 2500.01316]),
+    'sz1': array([   0.        , 2500.        , 2500.01316]),
+    'g0': array([   0.        , 2500.        , 2500.01316]),
+    'g1': array([   0.        , 2500.        , 2500.01316])},
     {'sz0': array([-0.5, -9.5]),
     'sz1': array([-0.5, -9.5]),
     'g0': array([0.01, 0.  ]),
     'g1': array([0.01, 0.  ])})
 
     Notice that the above example is equivalent to using directly
     the :obj:`.DispersiveCavityQED`.
@@ -96,15 +96,15 @@
 
     def _rotation_compiler(self, gate, op_label, param_label, args):
         """
         Single qubit rotation compiler.
 
         Parameters
         ----------
-        gate : :obj:`.Gate`:
+        gate : :obj:`~.operations.Gate`:
             The quantum gate to be compiled.
         op_label : str
             Label of the corresponding control Hamiltonian.
         param_label : str
             Label of the hardware parameters saved in
             :obj:`GateCompiler.params`.
         args : dict
@@ -130,15 +130,15 @@
 
     def rz_compiler(self, gate, args):
         """
         Compiler for the RZ gate
 
         Parameters
         ----------
-        gate : :obj:`.Gate`:
+        gate : :obj:`~.operations.Gate`:
             The quantum gate to be compiled.
         args : dict
             The compilation configuration defined in the attributes
             :obj:`.GateCompiler.args` or given as a parameter in
             :obj:`.GateCompiler.compile`.
 
         Returns
@@ -150,15 +150,15 @@
 
     def rx_compiler(self, gate, args):
         """
         Compiler for the RX gate
 
         Parameters
         ----------
-        gate : :obj:`.Gate`:
+        gate : :obj:`~.operations.Gate`:
             The quantum gate to be compiled.
         args : dict
             The compilation configuration defined in the attributes
             :obj:`.GateCompiler.args` or given as a parameter in
             :obj:`.GateCompiler.compile`.
 
         Returns
@@ -208,15 +208,15 @@
 
     def sqrtiswap_compiler(self, gate, args):
         """
         Compiler for the SQRTISWAP gate.
 
         Parameters
         ----------
-        gate : :obj:`.Gate`:
+        gate : :obj:`~.operations.Gate`:
             The quantum gate to be compiled.
         args : dict
             The compilation configuration defined in the attributes
             :obj:`.GateCompiler.args` or given as a parameter in
             :obj:`.GateCompiler.compile`.
 
         Returns
@@ -236,15 +236,15 @@
 
     def iswap_compiler(self, gate, args):
         """
         Compiler for the ISWAP gate.
 
         Parameters
         ----------
-        gate : :obj:`.Gate`:
+        gate : :obj:`~.operations.Gate`:
             The quantum gate to be compiled.
         args : dict
             The compilation configuration defined in the attributes
             :obj:`.GateCompiler.args` or given as a parameter in
             :obj:`.GateCompiler.compile`.
 
         Returns
```

### Comparing `qutip-qip-0.2.3/src/qutip_qip/compiler/circuitqedcompiler.py` & `qutip-qip-0.3.0/src/qutip_qip/compiler/circuitqedcompiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from ..circuit import Gate
+from ..operations import Gate
 from ..compiler import GateCompiler, Instruction
 
 
 __all__ = ["SCQubitsCompiler"]
 
 
 class SCQubitsCompiler(GateCompiler):
@@ -29,17 +29,17 @@
 
     For single-qubit gate, we apply the DRAG correction :cite:`motzoi2013`
 
     .. math::
 
         \Omega^{x} &= \Omega_0 - \frac{\Omega_0^3}{4 \alpha^2}
 
-        \Omega^{y} &= - \dot{\Omega}_0 / \alpha
+        \Omega^{y} &= - \frac{\dot{\Omega}_0 }{\alpha}
 
-        \Omega^{z} &= - \Omega_0**2 / \alpha + \frac{2  \Omega_0^2)}{
+        \Omega^{z} &= - \frac{\Omega_0^2}{\alpha} + \frac{2 \Omega_0^2}{
             4 \alpha
         }
 
     where :math:`\Omega_0` is the original shape of the pulse.
     Notice that the :math:`\Omega_0` and its first derivative
     should be 0 from the starts and the end.
 
@@ -102,15 +102,15 @@
 
     def _rotation_compiler(self, gate, op_label, param_label, args):
         """
         Single qubit rotation compiler.
 
         Parameters
         ----------
-        gate : :obj:`.Gate`:
+        gate : :obj:`~.operations.Gate`:
             The quantum gate to be compiled.
         op_label : str
             Label of the corresponding control Hamiltonian.
         param_label : str
             Label of the hardware parameters saved in
             :obj:`GateCompiler.params`.
         args : dict
@@ -160,15 +160,15 @@
 
     def ry_compiler(self, gate, args):
         """
         Compiler for the RZ gate
 
         Parameters
         ----------
-        gate : :obj:`.Gate`:
+        gate : :obj:`~.operations.Gate`:
             The quantum gate to be compiled.
         args : dict
             The compilation configuration defined in the attributes
             :obj:`.GateCompiler.args` or given as a parameter in
             :obj:`.GateCompiler.compile`.
 
         Returns
@@ -180,15 +180,15 @@
 
     def rx_compiler(self, gate, args):
         """
         Compiler for the RX gate
 
         Parameters
         ----------
-        gate : :obj:`.Gate`:
+        gate : :obj:`~.operations.Gate`:
             The quantum gate to be compiled.
         args : dict
             The compilation configuration defined in the attributes
             :obj:`.GateCompiler.args` or given as a parameter in
             :obj:`.GateCompiler.compile`.
 
         Returns
@@ -203,15 +203,15 @@
         Compiler for CNOT gate using the cross resonance iteraction.
         See
         https://journals.aps.org/prb/abstract/10.1103/PhysRevB.81.134507
         for reference.
 
         Parameters
         ----------
-        gate : :obj:`.Gate`:
+        gate : :obj:`~.operations.Gate`:
             The quantum gate to be compiled.
         args : dict
             The compilation configuration defined in the attributes
             :obj:`.GateCompiler.args` or given as a parameter in
             :obj:`.GateCompiler.compile`.
 
         Returns
```

### Comparing `qutip-qip-0.2.3/src/qutip_qip/compiler/gatecompiler.py` & `qutip-qip-0.3.0/src/qutip_qip/compiler/gatecompiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         Compile the the native gates into control pulse sequence.
         It calls each compiling method and concatenates
         the compiled pulses.
 
         Parameters
         ----------
         circuit: :class:`.QubitCircuit` or list of
-            :class:`.Gate`
+            :class:`~.operations.Gate`
             A list of elementary gates that can be implemented in the
             corresponding hardware.
             The gate names have to be in `gate_compiler`.
 
         schedule_mode: str, optional
             ``"ASAP"`` for "as soon as possible" or
             ``"ALAP"`` for "as late as possible" or
```

### Comparing `qutip-qip-0.2.3/src/qutip_qip/compiler/instruction.py` & `qutip-qip-0.3.0/src/qutip_qip/compiler/instruction.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """
     Representation of pulses that implement a quantum gate.
     It contains the control pulse required to implement the gate
     on a particular hardware model.
 
     Parameters
     ----------
-    gate: :class:`.Gate`
+    gate: :class:`~.operations.Gate`
         The quantum gate.
     duration: list, optional
         The execution time needed for the instruction.
     tlist: array_like, optional
         A list of time at which the time-dependent coefficients are
         applied. See :class:`.Pulse` for detailed information`
     pulse_info: list, optional
```

### Comparing `qutip-qip-0.2.3/src/qutip_qip/compiler/scheduler.py` & `qutip-qip-0.3.0/src/qutip_qip/compiler/scheduler.py`

 * *Files identical despite different names*

### Comparing `qutip-qip-0.2.3/src/qutip_qip/compiler/spinchaincompiler.py` & `qutip-qip-0.3.0/src/qutip_qip/compiler/spinchaincompiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
     def _rotation_compiler(self, gate, op_label, param_label, args):
         """
         Single qubit rotation compiler.
 
         Parameters
         ----------
-        gate : :obj:`.Gate`:
+        gate : :obj:`~.operations.Gate`:
             The quantum gate to be compiled.
         op_label : str
             Label of the corresponding control Hamiltonian.
         param_label : str
             Label of the hardware parameters saved in
             :obj:`GateCompiler.params`.
         args : dict
@@ -153,15 +153,15 @@
 
     def rz_compiler(self, gate, args):
         """
         Compiler for the RZ gate
 
         Parameters
         ----------
-        gate : :obj:`.Gate`:
+        gate : :obj:`~.operations.Gate`:
             The quantum gate to be compiled.
         args : dict
             The compilation configuration defined in the attributes
             :obj:`.GateCompiler.args` or given as a parameter in
             :obj:`.GateCompiler.compile`.
 
         Returns
@@ -173,15 +173,15 @@
 
     def rx_compiler(self, gate, args):
         """
         Compiler for the RX gate
 
         Parameters
         ----------
-        gate : :obj:`.Gate`:
+        gate : :obj:`~.operations.Gate`:
             The quantum gate to be compiled.
         args : dict
             The compilation configuration defined in the attributes
             :obj:`.GateCompiler.args` or given as a parameter in
             :obj:`.GateCompiler.compile`.
 
         Returns
@@ -208,15 +208,15 @@
 
     def iswap_compiler(self, gate, args):
         """
         Compiler for the ISWAP gate.
 
         Parameters
         ----------
-        gate : :obj:`.Gate`:
+        gate : :obj:`~.operations.Gate`:
             The quantum gate to be compiled.
         args : dict
             The compilation configuration defined in the attributes
             :obj:`.GateCompiler.args` or given as a parameter in
             :obj:`.GateCompiler.compile`.
 
         Returns
```

### Comparing `qutip-qip-0.2.3/src/qutip_qip/device/cavityqed.py` & `qutip-qip-0.3.0/src/qutip_qip/device/circuitqed.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,353 +1,353 @@
-import warnings
 from copy import deepcopy
 
 import numpy as np
 
-from qutip import (
-    tensor,
-    identity,
-    destroy,
-    sigmax,
-    sigmaz,
-    basis,
-    Qobj,
-    QobjEvo,
-)
-from ..circuit import QubitCircuit
-from ..operations import Gate
-from .processor import Processor, Model
+from qutip import qeye, tensor, destroy, basis
+from .processor import Model
 from .modelprocessor import ModelProcessor, _to_array
+from ..transpiler import to_chain_structure
+from ..compiler import SCQubitsCompiler
+from ..noise import ZZCrossTalk
 from ..operations import expand_operator
-from ..pulse import Pulse
-from ..compiler import GateCompiler, CavityQEDCompiler
 
 
-__all__ = ["DispersiveCavityQED"]
+__all__ = ["SCQubits"]
 
 
-class DispersiveCavityQED(ModelProcessor):
+class SCQubits(ModelProcessor):
     """
-    The processor based on the physical implementation of
-    a dispersive cavity QED system (:obj:`.CavityQEDModel`).
-    The available Hamiltonian of the system is predefined.
-    For a given pulse amplitude matrix, the processor can
-    calculate the state evolution under the given control pulse,
-    either analytically or numerically.
-    (Only additional attributes are documented here, for others please
-    refer to the parent class :class:`.ModelProcessor`)
+    A chain of superconducting qubits with fixed frequency
+    (:obj:`SCQubitsModel`).
+    Single-qubit control is realized by rotation around the X and Y axis
+    while two-qubit gates are implemented with Cross Resonance gates.
+    A 3-level system is used to simulate the superconducting qubit system,
+    in order to simulation leakage.
+    Various types of interaction can be realized on a superconducting
+    system, as a demonstration and
+    for simplicity, we only use a ZX Hamiltonian for
+    the two-qubit interaction.
+
+    See the mathematical details in
+    :obj:`.SCQubitsCompiler` and :obj:`.SCQubitsModel`.
 
     Parameters
     ----------
     num_qubits: int
         The number of qubits in the system.
-
-    num_levels: int, optional
-        The number of energy levels in the resonator.
-
-    correct_global_phase: float, optional
-        Save the global phase, the analytical solution
-        will track the global phase.
-        It has no effect on the numerical solution.
-
+    dims: list, optional
+        The dimension of each component system.
+        Default value is a qubit system of ``dim=[2,2,2,...,2]``.
+    zz_crosstalk: bool, optional
+        If ZZ cross-talk is included.
     **params:
-        Hardware parameters. See :obj:`CavityQEDModel`.
+        Hardware parameters. See :obj:`SCQubitsModel`.
 
     Examples
     --------
 
     .. testcode::
 
         import numpy as np
         import qutip
         from qutip_qip.circuit import QubitCircuit
-        from qutip_qip.device import DispersiveCavityQED
+        from qutip_qip.device import SCQubits
 
         qc = QubitCircuit(2)
-        qc.add_gate("RX", 0, arg_value=np.pi)
+        qc.add_gate("RZ", 0, arg_value=np.pi)
         qc.add_gate("RY", 1, arg_value=np.pi)
-        qc.add_gate("ISWAP", [1, 0])
+        qc.add_gate("CNOT", targets=0, controls=1)
 
-        processor = DispersiveCavityQED(2, g=0.1)
+        processor = SCQubits(2)
         processor.load_circuit(qc)
-        result = processor.run_state(
-            qutip.basis([10, 2, 2], [0, 0, 0]),
-            options=qutip.Options(nsteps=5000))
-        final_qubit_state = result.states[-1].ptrace([1, 2])
-        print(round(qutip.fidelity(
-            final_qubit_state,
-            qc.run(qutip.basis([2, 2], [0, 0]))
-        ), 4))
-
-    .. testoutput::
-
-        0.9994
-
+        init_state = qutip.basis([3, 3], [0, 0])
+        result = processor.run_state(init_state)
     """
 
-    def __init__(
-        self, num_qubits, num_levels=10, correct_global_phase=True, **params
-    ):
-        model = CavityQEDModel(
+    def __init__(self, num_qubits, dims=None, zz_crosstalk=False, **params):
+        if dims is None:
+            dims = [3] * num_qubits
+        model = SCQubitsModel(
             num_qubits=num_qubits,
-            num_levels=num_levels,
+            dims=dims,
+            zz_crosstalk=zz_crosstalk,
             **params,
         )
-        super(DispersiveCavityQED, self).__init__(
-            model=model, correct_global_phase=correct_global_phase
-        )
-        self.correct_global_phase = correct_global_phase
-        self.num_levels = num_levels
-        self.native_gates = ["SQRTISWAP", "ISWAP", "RX", "RZ"]
-        self.spline_kind = "step_func"
+        super(SCQubits, self).__init__(model=model)
+        self.native_gates = ["RX", "RY", "CNOT"]
+        self._default_compiler = SCQubitsCompiler
+        self.pulse_mode = "continuous"
 
-    @property
-    def sx_ops(self):
-        """
-        list: A list of sigmax Hamiltonians for each qubit.
-        """
-        return self.ctrls[0 : self.num_qubits]
+    def topology_map(self, qc):
+        return to_chain_structure(qc)
 
-    @property
-    def sz_ops(self):
-        """
-        list: A list of sigmaz Hamiltonians for each qubit.
-        """
-        return self.ctrls[self.num_qubits : 2 * self.num_qubits]
 
-    @property
-    def cavityqubit_ops(self):
-        """
-        list: A list of interacting Hamiltonians between cavity and each qubit.
-        """
-        return self.ctrls[2 * self.num_qubits : 3 * self.num_qubits]
-
-    @property
-    def sx_u(self):
-        """array-like: Pulse matrix for sigmax Hamiltonians."""
-        return self.coeffs[: self.num_qubits]
-
-    @property
-    def sz_u(self):
-        """array-like: Pulse matrix for sigmaz Hamiltonians."""
-        return self.coeffs[self.num_qubits : 2 * self.num_qubits]
-
-    @property
-    def g_u(self):
-        """
-        array-like: Pulse matrix for interacting Hamiltonians
-        between cavity and each qubit.
-        """
-        return self.coeffs[2 * self.num_qubits : 3 * self.num_qubits]
-
-    def eliminate_auxillary_modes(self, U):
-        """
-        Eliminate the auxillary modes like the cavity modes in cqed.
-        """
-        psi_proj = tensor(
-            [basis(self.num_levels, 0)]
-            + [identity(2) for n in range(self.num_qubits)]
-        )
-        result = psi_proj.dag() * U * psi_proj
-        # In qutip 5 multiplication of matrices
-        # with dims [[1, 2], [2, 2]] and [[2, 2], [1, 2]]
-        # will give a result of
-        # dims [[1, 2], [1, 2]] instead of [[2], [2]].
-        if result.dims[0][0] == 1:
-            result = result.ptrace(list(range(len(self.dims)))[1:])
-        return result
-
-    def load_circuit(self, qc, schedule_mode="ASAP", compiler=None):
-        if compiler is None:
-            compiler = CavityQEDCompiler(
-                self.num_qubits, self.params, global_phase=0.0
-            )
-        tlist, coeff = super().load_circuit(
-            qc, schedule_mode=schedule_mode, compiler=compiler
-        )
-        self.global_phase = compiler.global_phase
-        return tlist, coeff
-
-
-class CavityQEDModel(Model):
+class SCQubitsModel(Model):
     """
-    The physical model for a dispersive cavity-QED processor
-    (:obj:`.DispersiveCavityQED`).
-    It is a qubit-resonator model that describes a system composed of
-    a single resonator and a few qubits connected to it.
-    The coupling is kept small so that the resonator is rarely
-    excited but acts only as a mediator for entanglement generation.
-    The single-qubit control Hamiltonians used are
-    :math:`\sigma_x` and :math:`\sigma_z`.
-    The dynamics between the resonator and the qubits is captured by
-    the Tavis-Cummings Hamiltonian,
-    :math:`\propto\sum_j a^\dagger \sigma_j^{-} + a \sigma_j^{+}`,
-    where :math:`a`, :math:`a^\dagger` are
-    the destruction and creation operators of the resonator,
-    while :math:`\sigma_j^{-}`, :math:`\sigma_j^{+}` are those of each qubit.
-    The control of the qubit-resonator coupling depends on
-    the physical implementation, but in the most general case
-    we have single and multi-qubit control in the form
+    The physical model for superconducting-qubit model processor
+    (:obj:`.SCQubits`) with fixed frequency.
+    Each qubit is simulated by a multi-level Duffing model
+    :cite:`koch2007charge`,
+    in which the qubit subspace is provided by the ground state
+    and the first excited state.
+    By default, the creation and annihilation operators are
+    truncated at the third level, which can be adjusted.
+    The multi-level representation can capture the leakage of the population
+    out of the qubit subspace during single-qubit gates.
+    The single-qubit control is generated by two orthogonal quadratures
+    :math:`a_j^{\\dagger}+a_j` and :math:`i(a_j^{\\dagger}-a_j)`.
+    The interaction is possible only between adjacent qubits.
+    Although this interaction is mediated by a resonator, for simplicity,
+    we replace the complicated dynamics among two superconducting qubits
+    and the resonator with a two-qubit effective Hamiltonian
+    derived in Ref. :cite:`magesan2020effective`.
+
+    As an example, we choose the cross resonance interaction
+    in the form of :math:`\\sigma^z_{j} \\sigma^x_{j+1}`,
+    acting only on the two-qubit levels,
+    which is widely used, e.g., in fixed-frequency superconducting qubits.
+    We can write the Hamiltonian as
 
     .. math::
 
-        H=
-        \\sum_{j=0}^{N-1}
-        \\epsilon^{\\rm{max}}_{j}(t) \\sigma^x_{j} +
-        \\Delta^{\\rm{max}}_{j}(t) \\sigma^z_{j} +
-        J_{j}(t)
-        (a^\\dagger \\sigma^{-}_{j} + a \\sigma^{+}_{j}).
+        H &= H_{\\rm{d}}
+         + \\sum_{j=0}^{N-1} \\Omega^x_{j} (a_j^{\\dagger} + a_j)
+        + \\Omega^y_{j} i(a_j^{\\dagger} - a_j) \\\\
+        &
+        + \\sum_{j=0}^{N-2} \\Omega^{\\rm{cr}1}_{j} \\sigma^z_j \\sigma^x_{j+1}
+        + \\Omega^{\\rm{cr}2}_{j} \\sigma^x_j \\sigma^z_{j+1}
 
-    The effective qubit-qubit coupling is computed by the
+    where the drift Hamiltonian is defined as
 
     .. math::
 
-        J_j = \\frac{g_j g_{j+1}}{2}(\\frac{1}{\\Delta_j} +
-        \\frac{1}{\\Delta_{j+1}}),
-
-    with :math:`\\Delta=w_q-w_0`
-    and the dressed qubit frequency :math:`w_q` defined as
-    :math:`w_q=\sqrt{\epsilon^2+\delta^2}`.
+        H_{\\rm{d}} = \\sum_{j=0}^{N-1}
+        \\frac{\\alpha_j}{2} a_j^{\\dagger}a_j^{\\dagger}a_j a_j
 
     Parameters
     ----------
-    num_qubits : int
-        The number of qubits :math:`N`.
-    num_levels : int, optional
-        The truncation level of the Hilbert space for the resonator.
-    **params :
+    num_qubits: int
+        The number of qubits.
+    dims: list, optional
+        The dimension of each component system.
+        Default value is a qubit system of ``dim=[2,2,2,...,2]``.
+    zz_crosstalk: bool, optional
+        If ZZ cross-talk is included.
+    **params:
         Keyword arguments for hardware parameters, in the unit of GHz.
-        Qubit parameters can either be a float or a list of the length
-        :math:`N`.
+        Each should be given as list:
 
-        - deltamax: float or list, optional
-            The pulse strength of sigma-x control,
-            :math:`\\Delta^{\\rm{max}}`, default ``1.0``.
-        - epsmax: float or list, optional
-            The pulse strength of sigma-z control,
-            :math:`\\epsilon^{\\rm{max}}`, default ``9.5``.
-        - eps: float or list, optional
-            The bare transition frequency for each of the qubits,
-            default ``9.5``.
-        - delta : float or list, optional
-            The coupling between qubit states, default ``0.0``.
-        - g : float or list, optional
-            The coupling strength between the resonator and the qubit,
-            default ``1.0``.
-        - w0 : float, optional
-            The bare frequency of the resonator :math:`w_0`.
-            Should only be a float, default ``0.01``.
+        - wq : list, optional
+            Qubits bare frequency, default 5.15 and 5.09
+            for each pair of superconducting qubits,
+            default ``[5.15, 5.09, 5.15, ...]``.
+        - wr : list, optional
+            Resonator bare frequency, default ``[5.96]*num_qubits``.
+        - g : list, optional
+            The coupling strength between the resonator and the qubits,
+            default ``[0.1]*(num_qubits - 1)``.
+        - alpha : list, optional
+            Anharmonicity for each superconducting qubit,
+            default ``[-0.3]*num_qubits``.
+        - omega_single : list, optional
+            The maximal control strength for single-qubit gate,
+            :math:`\\Omega^x` and :math:`\\Omega^y`,
+            default ``[0.01]*num_qubits``.
+        - omega_cr : list, optional
+            Control strength for cross resonance gate,
+            default ``[0.01]*num_qubits``.
         - t1 : float or list, optional
             Characterize the amplitude damping for each qubit.
         - t2 : list of list, optional
             Characterize the total dephasing for each qubit.
-
     """
 
-    def __init__(self, num_qubits, num_levels=10, **params):
+    def __init__(self, num_qubits, dims=None, zz_crosstalk=False, **params):
         self.num_qubits = num_qubits
-        self.num_levels = num_levels
-        self.dims = [num_levels] + [2] * num_qubits
-        self.params = {  # default parameters
-            "deltamax": 1.0,
-            "epsmax": 9.5,
-            "w0": 10,
-            "eps": 9.5,
-            "delta": 0.0,
-            "g": 0.01,
+        self.dims = dims if dims is not None else [3] * num_qubits
+        self.params = {
+            "wq": np.array(
+                ((5.15, 5.09) * int(np.ceil(self.num_qubits / 2)))[
+                    : self.num_qubits
+                ]
+            ),
+            "wr": 5.96,
+            "alpha": -0.3,
+            "g": 0.1,
+            "omega_single": 0.01,
+            "omega_cr": 0.01,
         }
         self.params.update(deepcopy(params))
+        self._compute_params()
         self._drift = []
+        self._set_up_drift()
         self._controls = self._set_up_controls()
-        self._compute_params()
         self._noise = []
+        if zz_crosstalk:
+            self._noise.append(ZZCrossTalk(self.params))
 
-    def get_all_drift(self):
-        return self._drift
+    def _set_up_drift(self):
+        for m in range(self.num_qubits):
+            destroy_op = destroy(self.dims[m])
+            coeff = 2 * np.pi * self.params["alpha"][m] / 2.0
+            self._drift.append(
+                (coeff * destroy_op.dag() ** 2 * destroy_op**2, [m])
+            )
 
     @property
     def _old_index_label_map(self):
         num_qubits = self.num_qubits
         return (
             ["sx" + str(i) for i in range(num_qubits)]
-            + ["sz" + str(i) for i in range(num_qubits)]
-            + ["g" + str(i) for i in range(num_qubits)]
+            + ["sy" + str(i) for i in range(num_qubits)]
+            + ["zx" + str(i) + str(i + 1) for i in range(num_qubits)]
+            + ["zx" + str(i + 1) + str(i) for i in range(num_qubits)]
         )
 
     def _set_up_controls(self):
         """
-        Generate the Hamiltonians for the cavity-qed model and save them in the
-        attribute `ctrls`.
-
-        Parameters
-        ----------
-        num_qubits: int
-            The number of qubits in the system.
+        Setup the operators.
+        We use 2π σ/2 as the single-qubit control Hamiltonian and
+        -2πZX/4 as the two-qubit Hamiltonian.
         """
-        controls = {}
         num_qubits = self.num_qubits
-        num_levels = self.num_levels
-        # single qubit terms
+        dims = self.dims
+        controls = {}
+
         for m in range(num_qubits):
-            controls["sx" + str(m)] = (2 * np.pi * sigmax(), [m + 1])
+            destroy_op = destroy(dims[m])
+            op = destroy_op + destroy_op.dag()
+            controls["sx" + str(m)] = (2 * np.pi / 2 * op, [m])
+
         for m in range(num_qubits):
-            controls["sz" + str(m)] = (2 * np.pi * sigmaz(), [m + 1])
-        # coupling terms
-        a = tensor(
-            [destroy(num_levels)] + [identity(2) for n in range(num_qubits)]
-        )
-        for n in range(num_qubits):
-            # FIXME expanded?
-            sm = tensor(
-                [identity(num_levels)]
-                + [
-                    destroy(2) if m == n else identity(2)
-                    for m in range(num_qubits)
-                ]
+            destroy_op = destroy(dims[m])
+            op = destroy_op * (-1.0j) + destroy_op.dag() * 1.0j
+            controls["sy" + str(m)] = (2 * np.pi / 2 * op, [m])
+
+        for m in range(num_qubits):
+            destroy_op = destroy(dims[m])
+            op = destroy_op.dag() * destroy_op
+            controls["sz" + str(m)] = (2 * np.pi * op, [m])
+
+        for m in range(num_qubits - 1):
+            # For simplicity, we neglect leakage in two-qubit gates.
+            d1 = dims[m]
+            d2 = dims[m + 1]
+            # projector to the 0 and 1 subspace
+            projector1 = (
+                basis(d1, 0) * basis(d1, 0).dag()
+                + basis(d1, 1) * basis(d1, 1).dag()
             )
-            controls["g" + str(n)] = (
-                2 * np.pi * a.dag() * sm + 2 * np.pi * a * sm.dag(),
-                list(range(num_qubits + 1)),
+            projector2 = (
+                basis(d2, 0) * basis(d2, 0).dag()
+                + basis(d2, 1) * basis(d2, 1).dag()
+            )
+            destroy_op1 = destroy(d1)
+            # Notice that this is actually 2πZX/4
+            z = (
+                projector1
+                * (-destroy_op1.dag() * destroy_op1 * 2 + qeye(d1))
+                / 2
+                * projector1
+            )
+            destroy_op2 = destroy(d2)
+            x = projector2 * (destroy_op2.dag() + destroy_op2) / 2 * projector2
+            controls["zx" + str(m) + str(m + 1)] = (
+                2 * np.pi * tensor([z, x]),
+                [m, m + 1],
+            )
+            controls["zx" + str(m + 1) + str(m)] = (
+                2 * np.pi * tensor([x, z]),
+                [m, m + 1],
             )
         return controls
 
     def _compute_params(self):
         """
-        Compute the qubit frequency and detune.
+        Compute the dressed frequency and the interaction strength.
         """
         num_qubits = self.num_qubits
-        w0 = self.params["w0"]  # only one resonator
-        # same parameters for all qubits if it is not a list
-        for name in ["epsmax", "deltamax", "eps", "delta", "g"]:
+        for name in ["alpha", "omega_single", "omega_cr"]:
             self.params[name] = _to_array(self.params[name], num_qubits)
-
-        # backward compatibility
-        self.params["sz"] = self.params["epsmax"]
-        self.params["sx"] = self.params["deltamax"]
-
-        # computed
-        wq = np.sqrt(self.params["eps"] ** 2 + self.params["delta"] ** 2)
-        self.params["wq"] = wq
-        self.params["Delta"] = wq - w0
-
-        # rwa/dispersive regime tests
-        if any(self.params["g"] / (w0 - wq) > 0.05):
-            warnings.warn("Not in the dispersive regime")
-
-        if any((w0 - wq) / (w0 + wq) > 0.05):
-            warnings.warn(
-                "The rotating-wave approximation might not be valid."
+        self.params["wr"] = _to_array(self.params["wr"], num_qubits - 1)
+        self.params["g"] = _to_array(self.params["g"], 2 * (num_qubits - 1))
+        g = self.params["g"]
+        wq = self.params["wq"]
+        wr = self.params["wr"]
+        alpha = self.params["alpha"]
+        # Dressed qubit frequency
+        wq_dr = []
+        for i in range(num_qubits):
+            tmp = wq[i]
+            if i != 0:
+                tmp += g[2 * i - 1] ** 2 / (wq[i] - wr[i - 1])
+            if i != (num_qubits - 1):
+                tmp += g[2 * i] ** 2 / (wq[i] - wr[i])
+            wq_dr.append(tmp)
+        self.params["wq_dressed"] = wq_dr
+        # Dressed resonator frequency
+        wr_dr = []
+        for i in range(num_qubits - 1):
+            tmp = wr[i]
+            tmp -= g[2 * i] ** 2 / (wq[i] - wr[i] + alpha[i])
+            tmp -= g[2 * i + 1] ** 2 / (wq[i + 1] - wr[i] + alpha[i])
+            wr_dr.append(tmp)
+        self.params["wr_dressed"] = wr_dr
+        # Effective qubit coupling strength
+        J = []
+        for i in range(num_qubits - 1):
+            tmp = (
+                g[2 * i]
+                * g[2 * i + 1]
+                * (wq[i] + wq[i + 1] - 2 * wr[i])
+                / 2
+                / (wq[i] - wr[i])
+                / (wq[i + 1] - wr[i])
             )
+            J.append(tmp)
+        self.params["J"] = J
+        # Effective ZX strength
+        zx_coeff = []
+        omega_cr = self.params["omega_cr"]
+        for i in range(num_qubits - 1):
+            tmp = (
+                J[i]
+                * omega_cr[i]
+                * (
+                    1 / (wq[i] - wq[i + 1] + alpha[i])
+                    - 1 / (wq[i] - wq[i + 1])
+                )
+            )
+            zx_coeff.append(tmp)
+        for i in range(num_qubits - 1, 0, -1):
+            tmp = (
+                J[i - 1]
+                * omega_cr[i]
+                * (
+                    1 / (wq[i] - wq[i - 1] + alpha[i])
+                    - 1 / (wq[i] - wq[i - 1])
+                )
+            )
+            zx_coeff.append(tmp)
+        # Times 2 because we use -2πZX/4 as operators
+        self.params["zx_coeff"] = np.asarray(zx_coeff) * 2
 
     def get_control_latex(self):
         """
         Get the labels for each Hamiltonian.
         It is used in the method method :meth:`.Processor.plot_pulses`.
         It is a 2-d nested list, in the plot,
         a different color will be used for each sublist.
         """
         num_qubits = self.num_qubits
-        return [
-            {f"sx{m}": r"$\sigma_x^" + f"{m}$" for m in range(num_qubits)},
-            {f"sz{m}": r"$\sigma_z^" + f"{m}$" for m in range(num_qubits)},
-            {f"g{m}": f"$g^{m}$" for m in range(num_qubits)},
+        labels = [
+            {f"sx{n}": r"$\sigma_x" + f"^{n}$" for n in range(num_qubits)},
+            {f"sy{n}": r"$\sigma_y" + f"^{n}$" for n in range(num_qubits)},
+            {f"sz{n}": r"$\sigma_z" + f"^{n}$" for n in range(num_qubits)},
         ]
+        label_zx = {}
+        for m in range(num_qubits - 1):
+            label_zx[f"zx{m}{m+1}"] = r"$ZX^{" + f"{m}{m+1}" + r"}$"
+            label_zx[f"zx{m+1}{m}"] = r"$ZX^{" + f"{m+1}{m}" + r"}$"
+
+        labels.append(label_zx)
+        return labels
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qutip-qip-0.2.3/src/qutip_qip/device/circuitqed.py` & `qutip-qip-0.3.0/src/qutip_qip/device/cavityqed.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,353 +1,404 @@
+import warnings
 from copy import deepcopy
 
 import numpy as np
 
-from qutip import qeye, tensor, destroy, basis
-from .processor import Model
+from qutip import (
+    tensor,
+    identity,
+    destroy,
+    sigmax,
+    sigmaz,
+    basis,
+    Qobj,
+    QobjEvo,
+)
+from ..circuit import QubitCircuit
+from ..operations import Gate
+from .processor import Processor, Model
 from .modelprocessor import ModelProcessor, _to_array
-from ..transpiler import to_chain_structure
-from ..compiler import SCQubitsCompiler
-from ..noise import ZZCrossTalk
-from ..operations import expand_operator
+from ..pulse import Pulse
+from ..compiler import GateCompiler, CavityQEDCompiler
 
 
-__all__ = ["SCQubits"]
+__all__ = ["DispersiveCavityQED"]
 
 
-class SCQubits(ModelProcessor):
+class DispersiveCavityQED(ModelProcessor):
     """
-    A chain of superconducting qubits with fixed frequency
-    (:obj:`SCQubitsModel`).
-    Single-qubit control is realized by rotation around the X and Y axis
-    while two-qubit gates are implemented with Cross Resonance gates.
-    A 3-level system is used to simulate the superconducting qubit system,
-    in order to simulation leakage.
-    Various types of interaction can be realized on a superconducting
-    system, as a demonstration and
-    for simplicity, we only use a ZX Hamiltonian for
-    the two-qubit interaction.
-
-    See the mathematical details in
-    :obj:`.SCQubitsCompiler` and :obj:`.SCQubitsModel`.
+    The processor based on the physical implementation of
+    a dispersive cavity QED system (:obj:`.CavityQEDModel`).
+    The available Hamiltonian of the system is predefined.
+    For a given pulse amplitude matrix, the processor can
+    calculate the state evolution under the given control pulse,
+    either analytically or numerically.
+    (Only additional attributes are documented here, for others please
+    refer to the parent class :class:`.ModelProcessor`)
 
     Parameters
     ----------
     num_qubits: int
         The number of qubits in the system.
-    dims: list, optional
-        The dimension of each component system.
-        Default value is a qubit system of ``dim=[2,2,2,...,2]``.
-    zz_crosstalk: bool, optional
-        If ZZ cross-talk is included.
+
+    num_levels: int, optional
+        The number of energy levels in the resonator.
+
+    correct_global_phase: float, optional
+        Save the global phase, the analytical solution
+        will track the global phase.
+        It has no effect on the numerical solution.
+
     **params:
-        Hardware parameters. See :obj:`SCQubitsModel`.
+        Hardware parameters. See :obj:`CavityQEDModel`.
 
     Examples
     --------
 
     .. testcode::
 
         import numpy as np
         import qutip
         from qutip_qip.circuit import QubitCircuit
-        from qutip_qip.device import SCQubits
+        from qutip_qip.device import DispersiveCavityQED
 
         qc = QubitCircuit(2)
-        qc.add_gate("RZ", 0, arg_value=np.pi)
+        qc.add_gate("RX", 0, arg_value=np.pi)
         qc.add_gate("RY", 1, arg_value=np.pi)
-        qc.add_gate("CNOT", targets=0, controls=1)
+        qc.add_gate("ISWAP", [1, 0])
 
-        processor = SCQubits(2)
+        processor = DispersiveCavityQED(2, g=0.1)
         processor.load_circuit(qc)
-        init_state = qutip.basis([3, 3], [0, 0])
-        result = processor.run_state(init_state)
+        result = processor.run_state(
+            qutip.basis([10, 2, 2], [0, 0, 0]),
+            options=qutip.Options(nsteps=5000))
+        final_qubit_state = result.states[-1].ptrace([1, 2])
+        print(round(qutip.fidelity(
+            final_qubit_state,
+            qc.run(qutip.basis([2, 2], [0, 0]))
+        ), 4))
+
+    .. testoutput::
+
+        0.9994
+
     """
 
-    def __init__(self, num_qubits, dims=None, zz_crosstalk=False, **params):
-        if dims is None:
-            dims = [3] * num_qubits
-        model = SCQubitsModel(
-            num_qubits=num_qubits,
-            dims=dims,
-            zz_crosstalk=zz_crosstalk,
-            **params,
+    def __init__(
+        self, num_qubits, num_levels=10, correct_global_phase=True, **params
+    ):
+        model = CavityQEDModel(
+            num_qubits=num_qubits, num_levels=num_levels, **params
         )
-        super(SCQubits, self).__init__(model=model)
-        self.native_gates = ["RX", "RY", "CNOT"]
-        self._default_compiler = SCQubitsCompiler
-        self.pulse_mode = "continuous"
+        super(DispersiveCavityQED, self).__init__(
+            model=model, correct_global_phase=correct_global_phase
+        )
+        self.correct_global_phase = correct_global_phase
+        self.num_levels = num_levels
+        self.native_gates = ["SQRTISWAP", "ISWAP", "RX", "RZ"]
+        self.spline_kind = "step_func"
 
-    def topology_map(self, qc):
-        return to_chain_structure(qc)
+    @property
+    def sx_ops(self):
+        """
+        list: A list of sigmax Hamiltonians for each qubit.
+        """
+        return self.ctrls[0 : self.num_qubits]
 
+    @property
+    def sz_ops(self):
+        """
+        list: A list of sigmaz Hamiltonians for each qubit.
+        """
+        return self.ctrls[self.num_qubits : 2 * self.num_qubits]
 
-class SCQubitsModel(Model):
-    """
-    The physical model for superconducting-qubit model processor
-    (:obj:`.SCQubits`) with fixed frequency.
-    Each qubit is simulated by a multi-level Duffing model
-    :cite:`koch2007charge`,
-    in which the qubit subspace is provided by the ground state
-    and the first excited state.
-    By default, the creation and annihilation operators are
-    truncated at the third level, which can be adjusted.
-    The multi-level representation can capture the leakage of the population
-    out of the qubit subspace during single-qubit gates.
-    The single-qubit control is generated by two orthogonal quadratures
-    :math:`a_j^{\\dagger}+a_j` and :math:`i(a_j^{\\dagger}-a_j)`.
-    The interaction is possible only between adjacent qubits.
-    Although this interaction is mediated by a resonator, for simplicity,
-    we replace the complicated dynamics among two superconducting qubits
-    and the resonator with a two-qubit effective Hamiltonian
-    derived in Ref. :cite:`magesan2020effective`.
-
-    As an example, we choose the cross resonance interaction
-    in the form of :math:`\\sigma^z_{j} \\sigma^x_{j+1}`,
-    acting only on the two-qubit levels,
-    which is widely used, e.g., in fixed-frequency superconducting qubits.
-    We can write the Hamiltonian as
+    @property
+    def cavityqubit_ops(self):
+        """
+        list: A list of interacting Hamiltonians between cavity and each qubit.
+        """
+        return self.ctrls[2 * self.num_qubits : 3 * self.num_qubits]
+
+    @property
+    def sx_u(self):
+        """array-like: Pulse matrix for sigmax Hamiltonians."""
+        return self.coeffs[: self.num_qubits]
+
+    @property
+    def sz_u(self):
+        """array-like: Pulse matrix for sigmaz Hamiltonians."""
+        return self.coeffs[self.num_qubits : 2 * self.num_qubits]
+
+    @property
+    def g_u(self):
+        """
+        array-like: Pulse matrix for interacting Hamiltonians
+        between cavity and each qubit.
+        """
+        return self.coeffs[2 * self.num_qubits : 3 * self.num_qubits]
+
+    def eliminate_auxillary_modes(self, U):
+        """
+        Eliminate the auxillary modes like the cavity modes in cqed.
+        """
+        psi_proj = tensor(
+            [basis(self.num_levels, 0)]
+            + [identity(2) for n in range(self.num_qubits)]
+        )
+        result = psi_proj.dag() * U * psi_proj
+        # In qutip 5 multiplication of matrices
+        # with dims [[1, 2], [2, 2]] and [[2, 2], [1, 2]]
+        # will give a result of
+        # dims [[1, 2], [1, 2]] instead of [[2], [2]].
+        if result.dims[0][0] == 1:
+            result = result.ptrace(list(range(len(self.dims)))[1:])
+        return result
+
+    def load_circuit(self, qc, schedule_mode="ASAP", compiler=None):
+        if compiler is None:
+            compiler = CavityQEDCompiler(
+                self.num_qubits, self.params, global_phase=0.0
+            )
+        tlist, coeff = super().load_circuit(
+            qc, schedule_mode=schedule_mode, compiler=compiler
+        )
+        self.global_phase = compiler.global_phase
+        return tlist, coeff
+
+    def generate_init_processor_state(
+        self, init_circuit_state: Qobj = None
+    ) -> Qobj:
+        """
+        Generate the initial state with the dimensions of the :class:`.DispersiveCavityQED` processor.
+
+        Parameters
+        ----------
+        init_circuit_state : :class:`qutip.Qobj`
+            Initial state provided with the dimensions of the circuit.
+
+        Returns
+        -------
+        :class:`qutip.Qobj`
+            Return the initial state with the dimensions of the :class:`.DispersiveCavityQED` processor model.
+            If initial_circuit_state was not provided, return the zero state.
+        """
+        if init_circuit_state is None:
+            return basis(
+                [self.num_levels] + [2] * self.num_qubits,
+                [0] + [0] * self.num_qubits,
+            )
+        return tensor(basis(self.num_levels, 0), init_circuit_state)
+
+    def get_final_circuit_state(self, final_processor_state: Qobj) -> Qobj:
+        """
+        Truncate the final processor state to get rid of the cavity subsystem.
+
+        Parameters
+        ----------
+        final_processor_state : :class:`qutip.Qobj`
+            State provided with the dimensions of the DispersiveCavityQED processor model.
+
+        Returns
+        -------
+        :class:`qutip.Qobj`
+            Return the truncated final state with the dimensions of the circuit.
+        """
+        return final_processor_state.ptrace(
+            range(1, len(final_processor_state.dims[0]))
+        )
+
+    def _get_max_step(self):
+        """
+        Define the maximal sampling step for the solver.
+        """
+        full_tlist = self.get_full_tlist()
+        if full_tlist is not None:
+            # For this model, discrete pulses are used.
+            # Hence we use half of the gate time as the step size.
+            return np.min(np.diff(full_tlist)) / 2
+        else:
+            return 0.0
+
+
+class CavityQEDModel(Model):
+    r"""
+    The physical model for a dispersive cavity-QED processor
+    (:obj:`.DispersiveCavityQED`).
+    It is a qubit-resonator model that describes a system composed of
+    a single resonator and a few qubits connected to it.
+    The coupling is kept small so that the resonator is rarely
+    excited but acts only as a mediator for entanglement generation.
+    The single-qubit control Hamiltonians used are
+    :math:`\sigma_x` and :math:`\sigma_z`.
+    The dynamics between the resonator and the qubits is captured by
+    the Tavis-Cummings Hamiltonian,
+    :math:`\propto\sum_j a^\dagger \sigma_j^{-} + a \sigma_j^{+}`,
+    where :math:`a`, :math:`a^\dagger` are
+    the destruction and creation operators of the resonator,
+    while :math:`\sigma_j^{-}`, :math:`\sigma_j^{+}` are those of each qubit.
+    The control of the qubit-resonator coupling depends on
+    the physical implementation, but in the most general case
+    we have single and multi-qubit control in the form
 
     .. math::
 
-        H &= H_{\\rm{d}}
-         + \\sum_{j=0}^{N-1} \\Omega^x_{j} (a_j^{\\dagger} + a_j)
-        + \\Omega^y_{j} i(a_j^{\\dagger} - a_j) \\\\
-        &
-        + \\sum_{j=0}^{N-2} \\Omega^{\\rm{cr}1}_{j} \\sigma^z_j \\sigma^x_{j+1}
-        + \\Omega^{\\rm{cr}2}_{j} \\sigma^x_j \\sigma^z_{j+1}
+        H=
+        \\sum_{j=0}^{N-1}
+        \\epsilon^{\\rm{max}}_{j}(t) \\sigma^x_{j} +
+        \\Delta^{\\rm{max}}_{j}(t) \\sigma^z_{j} +
+        J_{j}(t)
+        (a^\\dagger \\sigma^{-}_{j} + a \\sigma^{+}_{j}).
 
-    where the drift Hamiltonian is defined as
+    The effective qubit-qubit coupling is computed by the
 
     .. math::
 
-        H_{\\rm{d}} = \\sum_{j=0}^{N-1}
-        \\frac{\\alpha_j}{2} a_j^{\\dagger}a_j^{\\dagger}a_j a_j
+        J_j = \\frac{g_j g_{j+1}}{2}(\\frac{1}{\\Delta_j} +
+        \\frac{1}{\\Delta_{j+1}}),
+
+    with :math:`\\Delta=w_q-w_0`
+    and the dressed qubit frequency :math:`w_q` defined as
+    :math:`w_q=\sqrt{\epsilon^2+\delta^2}`.
 
     Parameters
     ----------
-    num_qubits: int
-        The number of qubits.
-    dims: list, optional
-        The dimension of each component system.
-        Default value is a qubit system of ``dim=[2,2,2,...,2]``.
-    zz_crosstalk: bool, optional
-        If ZZ cross-talk is included.
-    **params:
+    num_qubits : int
+        The number of qubits :math:`N`.
+    num_levels : int, optional
+        The truncation level of the Hilbert space for the resonator.
+    **params :
         Keyword arguments for hardware parameters, in the unit of GHz.
-        Each should be given as list:
+        Qubit parameters can either be a float or a list of the length
+        :math:`N`.
 
-        - wq : list, optional
-            Qubits bare frequency, default 5.15 and 5.09
-            for each pair of superconducting qubits,
-            default ``[5.15, 5.09, 5.15, ...]``.
-        - wr : list, optional
-            Resonator bare frequency, default ``[5.96]*num_qubits``.
-        - g : list, optional
-            The coupling strength between the resonator and the qubits,
-            default ``[0.1]*(num_qubits - 1)``.
-        - alpha : list, optional
-            Anharmonicity for each superconducting qubit,
-            default ``[-0.3]*num_qubits``.
-        - omega_single : list, optional
-            The maximal control strength for single-qubit gate,
-            :math:`\\Omega^x` and :math:`\\Omega^y`,
-            default ``[0.01]*num_qubits``.
-        - omega_cr : list, optional
-            Control strength for cross resonance gate,
-            default ``[0.01]*num_qubits``.
+        - deltamax: float or list, optional
+            The pulse strength of sigma-x control,
+            :math:`\\Delta^{\\rm{max}}`, default ``1.0``.
+        - epsmax: float or list, optional
+            The pulse strength of sigma-z control,
+            :math:`\\epsilon^{\\rm{max}}`, default ``9.5``.
+        - eps: float or list, optional
+            The bare transition frequency for each of the qubits,
+            default ``9.5``.
+        - delta : float or list, optional
+            The coupling between qubit states, default ``0.0``.
+        - g : float or list, optional
+            The coupling strength between the resonator and the qubit,
+            default ``1.0``.
+        - w0 : float, optional
+            The bare frequency of the resonator :math:`w_0`.
+            Should only be a float, default ``0.01``.
         - t1 : float or list, optional
             Characterize the amplitude damping for each qubit.
         - t2 : list of list, optional
             Characterize the total dephasing for each qubit.
+
     """
 
-    def __init__(self, num_qubits, dims=None, zz_crosstalk=False, **params):
+    def __init__(self, num_qubits, num_levels=10, **params):
         self.num_qubits = num_qubits
-        self.dims = dims if dims is not None else [3] * num_qubits
-        self.params = {
-            "wq": np.array(
-                ((5.15, 5.09) * int(np.ceil(self.num_qubits / 2)))[
-                    : self.num_qubits
-                ]
-            ),
-            "wr": 5.96,
-            "alpha": -0.3,
-            "g": 0.1,
-            "omega_single": 0.01,
-            "omega_cr": 0.01,
+        self.num_levels = num_levels
+        self.dims = [num_levels] + [2] * num_qubits
+        self.params = {  # default parameters
+            "deltamax": 1.0,
+            "epsmax": 9.5,
+            "w0": 10,
+            "eps": 9.5,
+            "delta": 0.0,
+            "g": 0.01,
         }
         self.params.update(deepcopy(params))
-        self._compute_params()
         self._drift = []
-        self._set_up_drift()
         self._controls = self._set_up_controls()
+        self._compute_params()
         self._noise = []
-        if zz_crosstalk:
-            self._noise.append(ZZCrossTalk(self.params))
 
-    def _set_up_drift(self):
-        for m in range(self.num_qubits):
-            destroy_op = destroy(self.dims[m])
-            coeff = 2 * np.pi * self.params["alpha"][m] / 2.0
-            self._drift.append(
-                (coeff * destroy_op.dag() ** 2 * destroy_op**2, [m])
-            )
+    def get_all_drift(self):
+        return self._drift
 
     @property
     def _old_index_label_map(self):
         num_qubits = self.num_qubits
         return (
             ["sx" + str(i) for i in range(num_qubits)]
-            + ["sy" + str(i) for i in range(num_qubits)]
-            + ["zx" + str(i) + str(i + 1) for i in range(num_qubits)]
-            + ["zx" + str(i + 1) + str(i) for i in range(num_qubits)]
+            + ["sz" + str(i) for i in range(num_qubits)]
+            + ["g" + str(i) for i in range(num_qubits)]
         )
 
     def _set_up_controls(self):
         """
-        Setup the operators.
-        We use 2π σ/2 as the single-qubit control Hamiltonian and
-        -2πZX/4 as the two-qubit Hamiltonian.
+        Generate the Hamiltonians for the cavity-qed model and save them in the
+        attribute `ctrls`.
+
+        Parameters
+        ----------
+        num_qubits: int
+            The number of qubits in the system.
         """
-        num_qubits = self.num_qubits
-        dims = self.dims
         controls = {}
-
-        for m in range(num_qubits):
-            destroy_op = destroy(dims[m])
-            op = destroy_op + destroy_op.dag()
-            controls["sx" + str(m)] = (2 * np.pi / 2 * op, [m])
-
+        num_qubits = self.num_qubits
+        num_levels = self.num_levels
+        # single qubit terms
         for m in range(num_qubits):
-            destroy_op = destroy(dims[m])
-            op = destroy_op * (-1.0j) + destroy_op.dag() * 1.0j
-            controls["sy" + str(m)] = (2 * np.pi / 2 * op, [m])
-
+            controls["sx" + str(m)] = (2 * np.pi * sigmax(), [m + 1])
         for m in range(num_qubits):
-            destroy_op = destroy(dims[m])
-            op = destroy_op.dag() * destroy_op
-            controls["sz" + str(m)] = (2 * np.pi * op, [m])
-
-        for m in range(num_qubits - 1):
-            # For simplicity, we neglect leakage in two-qubit gates.
-            d1 = dims[m]
-            d2 = dims[m + 1]
-            # projector to the 0 and 1 subspace
-            projector1 = (
-                basis(d1, 0) * basis(d1, 0).dag()
-                + basis(d1, 1) * basis(d1, 1).dag()
-            )
-            projector2 = (
-                basis(d2, 0) * basis(d2, 0).dag()
-                + basis(d2, 1) * basis(d2, 1).dag()
-            )
-            destroy_op1 = destroy(d1)
-            # Notice that this is actually 2πZX/4
-            z = (
-                projector1
-                * (-destroy_op1.dag() * destroy_op1 * 2 + qeye(d1))
-                / 2
-                * projector1
-            )
-            destroy_op2 = destroy(d2)
-            x = projector2 * (destroy_op2.dag() + destroy_op2) / 2 * projector2
-            controls["zx" + str(m) + str(m + 1)] = (
-                2 * np.pi * tensor([z, x]),
-                [m, m + 1],
+            controls["sz" + str(m)] = (2 * np.pi * sigmaz(), [m + 1])
+        # coupling terms
+        a = tensor(
+            [destroy(num_levels)] + [identity(2) for n in range(num_qubits)]
+        )
+        for n in range(num_qubits):
+            # FIXME expanded?
+            sm = tensor(
+                [identity(num_levels)]
+                + [
+                    destroy(2) if m == n else identity(2)
+                    for m in range(num_qubits)
+                ]
             )
-            controls["zx" + str(m + 1) + str(m)] = (
-                2 * np.pi * tensor([x, z]),
-                [m, m + 1],
+            controls["g" + str(n)] = (
+                2 * np.pi * a.dag() * sm + 2 * np.pi * a * sm.dag(),
+                list(range(num_qubits + 1)),
             )
         return controls
 
     def _compute_params(self):
         """
-        Compute the dressed frequency and the interaction strength.
+        Compute the qubit frequency and detune.
         """
         num_qubits = self.num_qubits
-        for name in ["alpha", "omega_single", "omega_cr"]:
+        w0 = self.params["w0"]  # only one resonator
+        # same parameters for all qubits if it is not a list
+        for name in ["epsmax", "deltamax", "eps", "delta", "g"]:
             self.params[name] = _to_array(self.params[name], num_qubits)
-        self.params["wr"] = _to_array(self.params["wr"], num_qubits - 1)
-        self.params["g"] = _to_array(self.params["g"], 2 * (num_qubits - 1))
-        g = self.params["g"]
-        wq = self.params["wq"]
-        wr = self.params["wr"]
-        alpha = self.params["alpha"]
-        # Dressed qubit frequency
-        wq_dr = []
-        for i in range(num_qubits):
-            tmp = wq[i]
-            if i != 0:
-                tmp += g[2 * i - 1] ** 2 / (wq[i] - wr[i - 1])
-            if i != (num_qubits - 1):
-                tmp += g[2 * i] ** 2 / (wq[i] - wr[i])
-            wq_dr.append(tmp)
-        self.params["wq_dressed"] = wq_dr
-        # Dressed resonator frequency
-        wr_dr = []
-        for i in range(num_qubits - 1):
-            tmp = wr[i]
-            tmp -= g[2 * i] ** 2 / (wq[i] - wr[i] + alpha[i])
-            tmp -= g[2 * i + 1] ** 2 / (wq[i + 1] - wr[i] + alpha[i])
-            wr_dr.append(tmp)
-        self.params["wr_dressed"] = wr_dr
-        # Effective qubit coupling strength
-        J = []
-        for i in range(num_qubits - 1):
-            tmp = (
-                g[2 * i]
-                * g[2 * i + 1]
-                * (wq[i] + wq[i + 1] - 2 * wr[i])
-                / 2
-                / (wq[i] - wr[i])
-                / (wq[i + 1] - wr[i])
-            )
-            J.append(tmp)
-        self.params["J"] = J
-        # Effective ZX strength
-        zx_coeff = []
-        omega_cr = self.params["omega_cr"]
-        for i in range(num_qubits - 1):
-            tmp = (
-                J[i]
-                * omega_cr[i]
-                * (
-                    1 / (wq[i] - wq[i + 1] + alpha[i])
-                    - 1 / (wq[i] - wq[i + 1])
-                )
-            )
-            zx_coeff.append(tmp)
-        for i in range(num_qubits - 1, 0, -1):
-            tmp = (
-                J[i - 1]
-                * omega_cr[i]
-                * (
-                    1 / (wq[i] - wq[i - 1] + alpha[i])
-                    - 1 / (wq[i] - wq[i - 1])
-                )
+
+        # backward compatibility
+        self.params["sz"] = self.params["epsmax"]
+        self.params["sx"] = self.params["deltamax"]
+
+        # computed
+        wq = np.sqrt(self.params["eps"] ** 2 + self.params["delta"] ** 2)
+        self.params["wq"] = wq
+        self.params["Delta"] = wq - w0
+
+        # rwa/dispersive regime tests
+        if any(self.params["g"] / (w0 - wq) > 0.05):
+            warnings.warn("Not in the dispersive regime")
+
+        if any((w0 - wq) / (w0 + wq) > 0.05):
+            warnings.warn(
+                "The rotating-wave approximation might not be valid."
             )
-            zx_coeff.append(tmp)
-        # Times 2 because we use -2πZX/4 as operators
-        self.params["zx_coeff"] = np.asarray(zx_coeff) * 2
 
     def get_control_latex(self):
         """
         Get the labels for each Hamiltonian.
         It is used in the method method :meth:`.Processor.plot_pulses`.
         It is a 2-d nested list, in the plot,
         a different color will be used for each sublist.
         """
         num_qubits = self.num_qubits
-        labels = [
-            {f"sx{n}": r"$\sigma_x" + f"^{n}$" for n in range(num_qubits)},
-            {f"sy{n}": r"$\sigma_y" + f"^{n}$" for n in range(num_qubits)},
-            {f"sz{n}": r"$\sigma_z" + f"^{n}$" for n in range(num_qubits)},
+        return [
+            {f"sx{m}": r"$\sigma_x^" + f"{m}$" for m in range(num_qubits)},
+            {f"sz{m}": r"$\sigma_z^" + f"{m}$" for m in range(num_qubits)},
+            {f"g{m}": f"$g^{m}$" for m in range(num_qubits)},
         ]
-        label_zx = {}
-        for m in range(num_qubits - 1):
-            label_zx[f"zx{m}{m+1}"] = r"$ZX^{" + f"{m}{m+1}" + r"}$"
-            label_zx[f"zx{m+1}{m}"] = r"$ZX^{" + f"{m+1}{m}" + r"}$"
-
-        labels.append(label_zx)
-        return labels
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `qutip-qip-0.2.3/src/qutip_qip/device/modelprocessor.py` & `qutip-qip-0.3.0/src/qutip_qip/device/modelprocessor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections.abc import Iterable
 import numbers
 
 import numpy as np
 
-from qutip import Qobj, QobjEvo, tensor, mesolve
+from qutip import Qobj, QobjEvo, tensor, mesolve, basis
 from ..operations import globalphase
 from ..circuit import QubitCircuit
 from .processor import Processor
 from ..compiler import GateCompiler
 from ..pulse import Pulse
 
 
@@ -239,14 +239,53 @@
         else:
             raise ValueError("No compiler defined.")
         # Save compiler pulses
         self.set_coeffs(coeffs)
         self.set_tlist(tlist)
         return tlist, coeffs
 
+    def generate_init_processor_state(
+        self, init_circuit_state: Qobj = None
+    ) -> Qobj:
+        """
+        Generate the initial state with the dimensions of the processor.
+
+        Parameters
+        ----------
+        init_circuit_state : :class:`qutip.Qobj`
+            Initial state provided with the dimensions of the circuit.
+
+        Returns
+        -------
+        :class:`qutip.Qobj`
+            Return the initial state with the dimensions
+            of the processor model. If initial_circuit_state
+            was not provided, return the zero state.
+        """
+        if init_circuit_state is None:
+            return basis([2] * self.num_qubits, [0] * self.num_qubits)
+        return init_circuit_state
+
+    def get_final_circuit_state(self, final_processor_state: Qobj) -> Qobj:
+        """
+        Convert the state with the dimensions of the processor model to
+        a state with the dimensions of the circuit.
+
+        Parameters
+        ----------
+        final_processor_state : :class:`qutip.Qobj`
+            State provided with the dimensions of the processor model.
+
+        Returns
+        -------
+        :class:`qutip.Qobj`
+            Return the final state with the dimensions of the circuit.
+        """
+        return final_processor_state
+
 
 def _to_array(params, num_qubits):
     """
     Transfer a parameter to an array.
     """
     if isinstance(params, numbers.Real):
         return np.asarray([params] * num_qubits)
```

### Comparing `qutip-qip-0.2.3/src/qutip_qip/device/optpulseprocessor.py` & `qutip-qip-0.3.0/src/qutip_qip/device/optpulseprocessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,24 +177,20 @@
                 kwargs.update(setting_args[gates[prop_ind]])
 
             control_labels = self.model.get_control_labels()
             full_ctrls_hams = []
             for label in control_labels:
                 qobj, targets = self.model.get_control(label)
                 full_ctrls_hams.append(
-                    expand_operator(
-                        qobj, len(self.dims), targets=targets, dims=self.dims
-                    )
+                    expand_operator(qobj, dims=self.dims, targets=targets)
                 )
 
             full_drift_ham = sum(
                 [
-                    expand_operator(
-                        qobj, len(self.dims), targets=targets, dims=self.dims
-                    )
+                    expand_operator(qobj, dims=self.dims, targets=targets)
                     for (qobj, targets) in self.model.get_all_drift()
                 ],
                 Qobj(
                     np.zeros(full_ctrls_hams[0].shape),
                     dims=[self.dims, self.dims],
                 ),
             )
```

### Comparing `qutip-qip-0.2.3/src/qutip_qip/device/processor.py` & `qutip-qip-0.3.0/src/qutip_qip/device/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     spline_kind : str, optional
         Type of the coefficient interpolation. Default is "step_func"
         Note that they have different requirements for the length of ``coeff``.
 
         -"step_func":
         The coefficient will be treated as a step function.
         E.g. ``tlist=[0,1,2]`` and ``coeff=[3,2]``, means that the coefficient
-        is 3 in t=[0,1) and 2 in t=[2,3). It requires
+        is 3 in t=[0,1) and 2 in t=[1,2). It requires
         ``len(coeff)=len(tlist)-1`` or ``len(coeff)=len(tlist)``, but
         in the second case the last element of ``coeff`` has no effect.
 
         -"cubic": Use cubic interpolation for the coefficient. It requires
         ``len(coeff)=len(tlist)``
 
     model : :obj:`Model`
@@ -309,16 +309,16 @@
         >>> processor = LinearSpinChain(1)
         >>> processor.get_control_labels()
         ['sx0', 'sz0']
         >>> processor.get_control('sz0') # doctest: +NORMALIZE_WHITESPACE
         (Quantum object: dims = [[2], [2]], shape = (2, 2),
         type = oper, isherm = True
         Qobj data =
-        [[ 6.28318531  0.        ]
-        [ 0.         -6.28318531]], 0)
+        [[ 6.28319  0.     ]
+         [ 0.      -6.28319]], 0)
         """
         return self.model.get_control(label)
 
     def get_control_labels(self):
         """
         Get a list of all available control Hamiltonians.
 
@@ -327,15 +327,15 @@
         label_list : list
             A list of hashable objects each corresponds to
             an available control Hamiltonian.
         """
         return self.model.get_control_labels()
 
     def get_control_latex(self):
-        """
+        r"""
         Get the latex string for each Hamiltonian.
         It is used in the method :meth:`.Processor.plot_pulses`.
         It is a list of dictionaries.
         In the plot, a different color will be used
         for each dictionary in the list.
 
         Returns
@@ -719,15 +719,15 @@
     def find_pulse(self, pulse_name):
         pulse_dict = self.get_pulse_dict()
         if isinstance(pulse_name, int):
             return self.pulses[pulse_name]
         else:
             try:
                 return self.pulses[pulse_dict[pulse_name]]
-            except (KeyError):
+            except KeyError:
                 raise KeyError(
                     "Pulse name {} undefined. "
                     "Please define it in the attribute "
                     "`pulse_dict`.".format(pulse_name)
                 )
 
     @property
@@ -1196,40 +1196,48 @@
             # TODO, this can be simplified further, tlist in the solver only
             # determines the time step for intermediate result.
             tlist = self.get_full_tlist()
         # Set the max step size as 1/10 of the total circuit time.
         # A better solution is to use the gate, which
         # is however, much harder to implement at this stage, see also
         # https://github.com/qutip/qutip-qip/issues/184.
-        full_tlist = self.get_full_tlist()
-        if full_tlist is not None:
-            total_circuit_time = (full_tlist)[-1]
-        else:
-            total_circuit_time = 0.0
         if is_qutip5:
-            options = kwargs.get("options", qutip.SolverOptions())
-            if options["max_step"] == 0.0:
-                options["max_step"] = total_circuit_time / 10
+            options = kwargs.get("options", qutip.Options())
+            if options.get("max_step", 0.0) == 0.0:
+                options["max_step"] = self._get_max_step()
+            options["progress_bar"] = False
         else:
             options = kwargs.get("options", qutip.Options())
             if options.max_step == 0.0:
-                options.max_step = total_circuit_time / 10
+                options.max_step = self._get_max_step()
+            options.progress_bar = False
         kwargs["options"] = options
         # choose solver:
         if solver == "mesolve":
             evo_result = mesolve(
                 H=noisy_qobjevo, rho0=init_state, tlist=tlist, **kwargs
             )
         elif solver == "mcsolve":
             evo_result = mcsolve(
-                H=noisy_qobjevo, psi0=init_state, tlist=tlist, **kwargs
+                noisy_qobjevo, init_state, tlist=tlist, **kwargs
             )
 
         return evo_result
 
+    def _get_max_step(self):
+        """
+        Define the maximal sampling step for the solver.
+        """
+        full_tlist = self.get_full_tlist()
+        if full_tlist is not None:
+            total_circuit_time = (full_tlist)[-1]
+        else:
+            total_circuit_time = 0.0
+        return total_circuit_time / 10
+
     def load_circuit(self, qc):
         """
         Translate an :class:`.QubitCircuit` to its
         corresponding Hamiltonians. (Defined in subclasses)
         """
         raise NotImplementedError("Use the function in the sub-class")
```

### Comparing `qutip-qip-0.2.3/src/qutip_qip/device/spinchain.py` & `qutip-qip-0.3.0/src/qutip_qip/device/spinchain.py`

 * *Files identical despite different names*

### Comparing `qutip-qip-0.2.3/src/qutip_qip/noise.py` & `qutip-qip-0.3.0/src/qutip_qip/noise.py`

 * *Files identical despite different names*

### Comparing `qutip-qip-0.2.3/src/qutip_qip/pulse.py` & `qutip-qip-0.3.0/src/qutip_qip/pulse.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             dims = [2] * dims
         if self.qobj is None:
             qobj = identity(dims[0]) * 0.0
             targets = 0
         else:
             qobj = self.qobj
             targets = self.targets
-        return expand_operator(qobj, len(dims), targets, dims)
+        return expand_operator(qobj, dims=dims, targets=targets)
 
     def _get_qobjevo_helper(self, spline_kind, dims):
         """
         Please refer to `_Evoelement.get_qobjevo` for documentation.
         """
         mat = self.get_qobj(dims)
         if self.tlist is None and self.coeff is None:
```

### Comparing `qutip-qip-0.2.3/src/qutip_qip/qasm.py` & `qutip-qip-0.3.0/src/qutip_qip/qasm.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,15 +130,14 @@
     tokens : list of (list of str)
         List of tokens corresponding to each QASM line taken as input.
     """
 
     processed_commands = []
 
     for line in token_cmds:
-
         # carry out some pre-processing for convenience
         for c in "[]()":
             line = line.replace(c, " " + c + " ")
         for c in "{}":
             line = line.replace(c, " ; " + c + " ; ")
         line_commands = line.split(";")
         line_commands = list(filter(lambda x: x != "", line_commands))
@@ -237,15 +236,14 @@
         additional files and insert it into previously processed list.
         """
 
         prev_index = 0
         expanded_commands = []
 
         for curr_index, command in enumerate(self.commands):
-
             if command[0] != "include":
                 continue
 
             filename = command[1].strip('"')
 
             if self.mode == "qiskit" and filename == "qelib1.inc":
                 continue
@@ -380,15 +378,14 @@
         # maps variables to supplied arguments, registers
         for i, arg in enumerate(gate.gate_args):
             args_map[arg] = eval(str(args[i]))
         for i, reg in enumerate(gate.gate_regs):
             regs_map[reg] = regs[i]
         # process all the constituent gates with supplied arguments, registers
         for call in gate.gates_inside:
-
             # create function call for the constituent gate
             name, com_args, com_regs = call
 
             for arg, real_arg in args_map.items():
                 com_args = [
                     command.replace(arg.strip(), str(real_arg))
                     for command in com_args
@@ -451,15 +448,14 @@
                 else:
                     new_regs.append(token)
             if open_bracket_mode:
                 raise SyntaxError("QASM: incorrect bracket formatting")
             regs = new_regs
 
         if reg_type == "measure":
-
             # processes register tokens of the form q[i] -> c[i]
             groups = re.match(r"(.*)\[(.*)\]->(.*)\[(.*)\]", "".join(regs))
             if groups:
                 qubit_name = groups.group(1)
                 qubit_ind = int(groups.group(2))
                 qubit_lst = self.qubit_regs[qubit_name]
                 if qubit_ind < len(qubit_lst):
@@ -522,15 +518,15 @@
     def _add_qiskit_gates(
         self,
         qc,
         name,
         regs,
         args=None,
         classical_controls=None,
-        control_value=None,
+        classical_control_value=None,
     ):
         """
         Add any gates that are pre-defined in qiskit-style exported
         qasm file with included "qelib1.inc".
 
         Parameters
         ----------
@@ -540,15 +536,15 @@
             name of gate to be added.
         regs : list of int
             list of qubit register indices to add gates to.
         args : float, optional
             value of args supplied to the gate.
         classical_controls : list of int, optional
             indices of classical bits to control gate on.
-        control_value : int, optional
+        classical_control_value : int, optional
             value of classical bits to control on, the classical controls are
             interpreted as an integer with lowest bit being the first one.
             If not specified, then the value is interpreted to be
             2 ** len(classical_controls) - 1
             (i.e. all classical controls are 1).
         """
 
@@ -572,116 +568,116 @@
 
         if name == "u3":
             qc.add_gate(
                 "QASMU",
                 targets=regs[0],
                 arg_value=args,
                 classical_controls=classical_controls,
-                control_value=control_value,
+                classical_control_value=classical_control_value,
             )
         elif name == "u2":
             qc.add_gate(
                 "u2",
                 targets=regs[0],
                 arg_value=args,
                 classical_controls=classical_controls,
-                control_value=control_value,
+                classical_control_value=classical_control_value,
             )
         elif name == "u1":
             qc.add_gate(
                 "RZ",
                 targets=regs[0],
                 arg_value=args,
                 classical_controls=classical_controls,
-                control_value=control_value,
+                classical_control_value=classical_control_value,
             )
         elif name == "cz":
             qc.add_gate(
                 "CZ",
                 targets=regs[1],
                 controls=regs[0],
                 classical_controls=classical_controls,
-                control_value=control_value,
+                classical_control_value=classical_control_value,
             )
         elif name == "cy":
             qc.add_gate(
                 "CY",
                 targets=regs[1],
                 controls=regs[0],
                 classical_controls=classical_controls,
-                control_value=control_value,
+                classical_control_value=classical_control_value,
             )
         elif name == "ch":
             qc.add_gate(
                 "ch",
                 targets=regs,
                 classical_controls=classical_controls,
-                control_value=control_value,
+                classical_control_value=classical_control_value,
             )
         elif name == "ccx":
             qc.add_gate(
                 "TOFFOLI",
                 targets=regs[2],
                 controls=regs[:2],
                 classical_controls=classical_controls,
-                control_value=control_value,
+                classical_control_value=classical_control_value,
             )
         elif name == "crz":
             qc.add_gate(
                 "CRZ",
                 targets=regs[1],
                 controls=regs[0],
                 arg_value=args,
                 classical_controls=classical_controls,
-                control_value=control_value,
+                classical_control_value=classical_control_value,
             )
         elif name == "cu1":
             qc.add_gate(
                 "CPHASE",
                 targets=regs[1],
                 controls=regs[0],
                 arg_value=args,
                 classical_controls=classical_controls,
-                control_value=control_value,
+                classical_control_value=classical_control_value,
             )
         elif name == "cu3":
             qc.add_gate(
                 "cu3",
                 targets=[regs[0], regs[1]],
                 arg_value=args,
                 classical_controls=classical_controls,
-                control_value=control_value,
+                classical_control_value=classical_control_value,
             )
         if name == "cx":
             qc.add_gate(
                 "CNOT",
                 targets=int(regs[1]),
                 controls=int(regs[0]),
                 classical_controls=classical_controls,
-                control_value=control_value,
+                classical_control_value=classical_control_value,
             )
         elif name in gate_name_map_1q:
             if args == []:
                 args = None
             qc.add_gate(
                 gate_name_map_1q[name],
                 targets=regs[0],
                 arg_value=args,
                 classical_controls=classical_controls,
-                control_value=control_value,
+                classical_control_value=classical_control_value,
             )
 
     def _add_predefined_gates(
         self,
         qc,
         name,
         com_regs,
         com_args,
         classical_controls=None,
-        control_value=None,
+        classical_control_value=None,
     ):
         """
         Add any gates that are pre-defined and/or inbuilt
         in our circuit.
 
         Parameters
         ----------
@@ -691,50 +687,55 @@
             name of gate to be added.
         regs : list of int
             list of qubit register indices to add gates to.
         args : float, optional
             value of args supplied to the gate.
         classical_controls : list of int, optional
             indices of classical bits to control gate on.
-        control_value : int, optional
+        classical_control_value : int, optional
             value of classical bits to control on, the classical controls are
             interpreted as an integer with lowest bit being the first one.
             If not specified, then the value is interpreted to be
             2 ** len(classical_controls) - 1
             (i.e. all classical controls are 1).
         """
 
         if name == "CX":
             qc.add_gate(
                 "CNOT",
                 targets=int(com_regs[1]),
                 controls=int(com_regs[0]),
                 classical_controls=classical_controls,
-                control_value=control_value,
+                classical_control_value=classical_control_value,
             )
         elif name == "U":
             qc.add_gate(
                 "QASMU",
                 targets=int(com_regs[0]),
                 arg_value=[float(arg) for arg in com_args],
                 classical_controls=classical_controls,
-                control_value=control_value,
+                classical_control_value=classical_control_value,
             )
         elif name in self.qiskitgates and self.mode == "qiskit":
             self._add_qiskit_gates(
-                qc, name, com_regs, com_args, classical_controls, control_value
+                qc,
+                name,
+                com_regs,
+                com_args,
+                classical_controls,
+                classical_control_value,
             )
 
     def _gate_add(
         self,
         qc,
         command,
         custom_gates,
         classical_controls=None,
-        control_value=None,
+        classical_control_value=None,
     ):
         """
         Add gates to :class:`.QubitCircuit` from processed tokens,
         define custom gates if necessary.
 
         Parameters
         ----------
@@ -742,15 +743,15 @@
             circuit object to which gate is added
         command: list of str
             list of tokens corresponding to gate application
         custom_gates: {gate name : gate function or unitary}
             dictionary of user gates defined for qutip
         classical_controls : int or list of int, optional
             indices of classical bits to control gate on.
-        control_value : int, optional
+        classical_control_value : int, optional
             value of classical bits to control on, the classical controls are
             interpreted as an integer with lowest bit being the first one.
             If not specified, then the value is interpreted to be
             2 ** len(classical_controls) - 1
             (i.e. all classical controls are 1).
         """
 
@@ -784,24 +785,24 @@
                 args = [eval(arg) for arg in args]
                 self._add_predefined_gates(
                     qc,
                     command[0],
                     regs,
                     args,
                     classical_controls=classical_controls,
-                    control_value=control_value,
+                    classical_control_value=classical_control_value,
                 )
             else:
                 if not isinstance(regs, list):
                     regs = [regs]
                 qc.add_gate(
                     gate_name,
                     targets=regs,
                     classical_controls=classical_controls,
-                    control_value=control_value,
+                    classical_control_value=classical_control_value,
                 )
 
     def _final_pass(self, qc):
         """
         Take a blank circuit, add all the gates and measurements specified
         by QASM.
         """
@@ -825,19 +826,23 @@
                 warnings.warn(
                     (
                         "Information about individual registers"
                         " is not preserved in QubitCircuit"
                     )
                 )
                 # adds classically controlled gates to the QubitCircuit
-                cbit_reg, control_value = command[2].split("==")
+                cbit_reg, classical_control_value = command[2].split("==")
                 cbit_inds = self.cbit_regs[cbit_reg]
-                control_value = int(control_value)
+                classical_control_value = int(classical_control_value)
                 self._gate_add(
-                    qc, command[4:], custom_gates, cbit_inds, control_value
+                    qc,
+                    command[4:],
+                    custom_gates,
+                    cbit_inds,
+                    classical_control_value,
                 )
             else:
                 err = "QASM: {} is not a valid QASM command.".format(
                     command[0]
                 )
                 raise SyntaxError(err)
 
@@ -984,17 +989,17 @@
 
     def _qasm_defn_from_resolved(self, curr_gate, gates_lst):
         """
         Resolve QASM definition of QuTiP gate in terms of component gates.
 
         Parameters
         ----------
-        curr_gate: :class:`.Gate`
+        curr_gate: :class:`~.operations.Gate`
             QuTiP gate which needs to be resolved into component gates.
-        gates_lst: list of :class:`.Gate`
+        gates_lst: list of :class:`~.operations.Gate`
             list of gate that constitute QASM definition of self.
         """
 
         forbidden_gates = ["GLOBALPHASE", "PHASEGATE"]
         reg_map = ["a", "b", "c"]
 
         q_controls = None
@@ -1039,15 +1044,15 @@
 
     def _qasm_defn_resolve(self, gate):
         """
         Resolve QASM definition of QuTiP gate if possible.
 
         Parameters
         ----------
-        gate: :class:`.Gate`
+        gate: :class:`~.operations.Gate`
             QuTiP gate which needs to be resolved into component gates.
 
         """
 
         qc = QubitCircuit(3)
         gates_lst = []
         if gate.name == "CSIGN":
@@ -1061,15 +1066,15 @@
 
     def _qasm_defns(self, gate):
         """
         Define QASM gates for QuTiP gates that do not have QASM counterparts.
 
         Parameters
         ----------
-        gate: :class:`.Gate`
+        gate: :class:`~.operations.Gate`
             QuTiP gate which needs to be defined in QASM format.
         """
 
         if gate.name == "CRY":
             gate_def = "gate cry(theta) a,b { cu3(theta,0,0) a,b; }"
         elif gate.name == "CRX":
             gate_def = "gate crx(theta) a,b { cu3(theta,-pi/2,pi/2) a,b; }"
```

### Comparing `qutip-qip-0.2.3/src/qutip_qip/qubits.py` & `qutip-qip-0.3.0/src/qutip_qip/qubits.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     ----------
     N : Integer
         Number of qubits in the register.
     states : List
         Initial state of each qubit.
 
     Returns
-    ----------
+    -------
     qstates : Qobj
         List of qubits.
 
     """
     state_list = []
     for i in range(N):
         if N > len(states) and i >= len(states):
```

### Comparing `qutip-qip-0.2.3/src/qutip_qip/transpiler/chain.py` & `qutip-qip-0.3.0/src/qutip_qip/transpiler/chain.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from copy import deepcopy
 from ..circuit import QubitCircuit
 
 
 __all__ = ["to_chain_structure"]
 
 
 def to_chain_structure(qc, setup="linear"):
@@ -23,15 +24,16 @@
     qc : :class:`.QubitCircuit`
         Returns QubitCircuit of resolved gates for the qubit circuit in the
         desired basis.
     """
     # FIXME This huge block has been here for a long time.
     # It could be moved to the new compiler section and carefully
     # splitted into smaller peaces.
-    qc_t = QubitCircuit(qc.N, qc.reverse_states)
+    qc_t = deepcopy(qc)
+    qc_t.gates = []
     swap_gates = [
         "SWAP",
         "ISWAP",
         "SQRTISWAP",
         "SQRTSWAP",
         "BERKELEY",
         "SWAPalpha",
@@ -95,15 +97,14 @@
                 mapped to a separate circuit and then copied back to the
                 original circuit.
                 """
 
                 temp = QubitCircuit(N - end + start)
                 i = 0
                 while i < (N - end + start):
-
                     if (
                         N + start - end - i - i == 1
                         and (N - end + start + 1) % 2 == 0
                     ):
                         if end == gate.controls[0]:
                             temp.add_gate(
                                 gate.name, targets=[i], controls=[i + 1]
@@ -211,15 +212,14 @@
                         )
                     i += 1
 
             else:
                 temp = QubitCircuit(N - end + start)
                 i = 0
                 while i < (N - end + start):
-
                     if (
                         N + start - end - i - i == 1
                         and (N - end + start + 1) % 2 == 0
                     ):
                         temp.add_gate(gate.name, [i, i + 1])
 
                     elif (
@@ -261,16 +261,12 @@
                                 (end + gate.targets[0]) % N,
                                 (end + gate.targets[1]) % N,
                             ],
                         )
                     j = j + 1
 
         else:
-            qc_t.add_gate(
-                gate.name,
-                gate.targets,
-                gate.controls,
-                gate.arg_value,
-                gate.arg_label,
-            )
+            # This gate can be general quantum operations
+            # such as measurement or global phase.
+            qc_t.add_gate(gate)
 
     return qc_t
```

### Comparing `qutip-qip-0.2.3/src/qutip_qip.egg-info/PKG-INFO` & `qutip-qip-0.3.0/src/qutip_qip.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qutip-qip
-Version: 0.2.3
+Version: 0.3.0
 Summary: The QuTiP quantum information processing package
 Home-page: https://github.com/qutip/qutip-qip
 Author: Alexander Pitchford, Paul D. Nation, Robert J. Johansson, Chris Granade, Arne Grimsmo, Nathan Shammah, Shahnawaz Ahmed, Neill Lambert, Eric Giguere, Boxi Li, Jake Lishman
 Author-email: qutip-admin@googlegroups.com
 License: BSD 3-Clause License
 Keywords: quantum,physics,dynamics
 Platform: Linux
@@ -21,14 +21,15 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown; variant=GFM
 Provides-Extra: graphics
 Provides-Extra: tests
 Provides-Extra: full
+Provides-Extra: qiskit
 License-File: LICENSE
 
 # qutip-qip
 
 [![build](https://github.com/qutip/qutip-qip/workflows/Tests/badge.svg)](https://github.com/qutip/qutip-qip/actions)
 [![Documentation Status](https://readthedocs.org/projects/qutip-qip/badge/?version=stable)](https://qutip-qip.readthedocs.io/en/stable/)
 [![PyPI version](https://badge.fury.io/py/qutip-qip.svg)](https://badge.fury.io/py/qutip-qip)
```

### Comparing `qutip-qip-0.2.3/src/qutip_qip.egg-info/SOURCES.txt` & `qutip-qip-0.3.0/src/qutip_qip.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -2,48 +2,60 @@
 MANIFEST.in
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 src/qutip_qip/__init__.py
-src/qutip_qip/circuit.py
-src/qutip_qip/circuit_latex.py
-src/qutip_qip/gates.py
+src/qutip_qip/compat.py
 src/qutip_qip/noise.py
 src/qutip_qip/pulse.py
 src/qutip_qip/qasm.py
+src/qutip_qip/qir.py
 src/qutip_qip/qubits.py
 src/qutip_qip/version.py
+src/qutip_qip/vqa.py
 src/qutip_qip.egg-info/PKG-INFO
 src/qutip_qip.egg-info/SOURCES.txt
 src/qutip_qip.egg-info/dependency_links.txt
 src/qutip_qip.egg-info/requires.txt
 src/qutip_qip.egg-info/top_level.txt
-src/qutip_qip/_decompose/__init__.py
-src/qutip_qip/_decompose/_utility.py
-src/qutip_qip/_decompose/decompose_single_qubit_gate.py
 src/qutip_qip/algorithms/__init__.py
 src/qutip_qip/algorithms/qft.py
+src/qutip_qip/circuit/__init__.py
+src/qutip_qip/circuit/_decompose.py
+src/qutip_qip/circuit/circuit.py
+src/qutip_qip/circuit/circuit_latex.py
+src/qutip_qip/circuit/circuitsimulator.py
 src/qutip_qip/compiler/__init__.py
 src/qutip_qip/compiler/cavityqedcompiler.py
 src/qutip_qip/compiler/circuitqedcompiler.py
 src/qutip_qip/compiler/gatecompiler.py
 src/qutip_qip/compiler/instruction.py
 src/qutip_qip/compiler/scheduler.py
 src/qutip_qip/compiler/spinchaincompiler.py
+src/qutip_qip/decompose/__init__.py
+src/qutip_qip/decompose/_utility.py
+src/qutip_qip/decompose/decompose_single_qubit_gate.py
 src/qutip_qip/device/__init__.py
 src/qutip_qip/device/cavityqed.py
 src/qutip_qip/device/circuitqed.py
 src/qutip_qip/device/modelprocessor.py
 src/qutip_qip/device/optpulseprocessor.py
 src/qutip_qip/device/processor.py
 src/qutip_qip/device/spinchain.py
 src/qutip_qip/operations/__init__.py
+src/qutip_qip/operations/gateclass.py
 src/qutip_qip/operations/gates.py
+src/qutip_qip/operations/measurement.py
+src/qutip_qip/qiskit/__init__.py
+src/qutip_qip/qiskit/backend.py
+src/qutip_qip/qiskit/converter.py
+src/qutip_qip/qiskit/job.py
+src/qutip_qip/qiskit/provider.py
 src/qutip_qip/transpiler/__init__.py
 src/qutip_qip/transpiler/chain.py
 tests/__init__.py
 tests/conftest.py
 tests/pytest.ini
 tests/test_circuit.py
 tests/test_compiler.py
@@ -53,16 +65,19 @@
 tests/test_model.py
 tests/test_noise.py
 tests/test_optpulseprocessor.py
 tests/test_processor.py
 tests/test_pulse.py
 tests/test_qasm.py
 tests/test_qft.py
+tests/test_qir.py
+tests/test_qiskit.py
 tests/test_qubits.py
 tests/test_scheduler.py
+tests/test_vqa.py
 tests/decomposition_functions/test_single_qubit_gate_decompositions.py
 tests/decomposition_functions/test_utility.py
 tests/qasm_files/bracket_error.qasm
 tests/qasm_files/command_error.qasm
 tests/qasm_files/qasm_error.qasm
 tests/qasm_files/qft.qasm
 tests/qasm_files/teleportation.qasm
```

### Comparing `qutip-qip-0.2.3/tests/conftest.py` & `qutip-qip-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `qutip-qip-0.2.3/tests/decomposition_functions/test_single_qubit_gate_decompositions.py` & `qutip-qip-0.3.0/tests/decomposition_functions/test_single_qubit_gate_decompositions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import numpy as np
 import cmath
 import pytest
 
 from qutip import (
     Qobj, average_gate_fidelity, rand_unitary, sigmax, sigmay, sigmaz
 )
-from qutip_qip._decompose.decompose_single_qubit_gate import (
+from qutip_qip.decompose.decompose_single_qubit_gate import (
     _ZYZ_rotation,
     _ZXZ_rotation,
     _ZYZ_pauli_X,
 )
-from qutip_qip._decompose import decompose_one_qubit_gate
+from qutip_qip.decompose import decompose_one_qubit_gate
 from qutip_qip.circuit import QubitCircuit
 from qutip_qip.operations.gates import snot, sqrtnot
 
 # Fidelity closer to 1 means the two states are similar to each other
-H = snot(1, 0)
+H = snot()
 sigmax = sigmax()
 sigmay = sigmay()
 sigmaz = sigmaz()
-SQRTNOT = sqrtnot(N=1, target=0)
+SQRTNOT = sqrtnot()
 T = Qobj([[1, 0], [0, cmath.rect(1, np.pi / 4)]])
 S = Qobj([[1, 0], [0, 1j]])
 target = 0
 num_qubits = 1
 
 
 # Tests for private functions
```

### Comparing `qutip-qip-0.2.3/tests/decomposition_functions/test_utility.py` & `qutip-qip-0.3.0/tests/decomposition_functions/test_utility.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pytest
 
 from qutip import Qobj, qeye
-from qutip_qip._decompose._utility import (
+from qutip_qip.decompose._utility import (
     check_gate,
 )
 
 
 # Tests for check_gate
 @pytest.mark.parametrize(
     "invalid_input",
```

### Comparing `qutip-qip-0.2.3/tests/test_circuit.py` & `qutip-qip-0.3.0/tests/test_circuit.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import pytest
 import os
 import shutil
 import numpy as np
 from pathlib import Path
 
 
-from qutip_qip.circuit import (
-    QubitCircuit, CircuitSimulator, Measurement)
+from qutip_qip.circuit import (QubitCircuit, CircuitSimulator)
 from qutip import (tensor, Qobj, ptrace, rand_ket, fock_dm, basis,
                    rand_dm, bell_state, ket2dm, identity, sigmax)
 from qutip_qip.qasm import read_qasm
 from qutip_qip.operations import (
-    Gate, gates, gate_sequence_product,
-    _ctrl_gates, _single_qubit_gates, _swap_like, _toffoli_like, _fredkin_like,
-    _para_gates
+    Gate, gates, Measurement, gate_sequence_product
 )
-
-from qutip_qip._decompose.decompose_single_qubit_gate import _ZYZ_rotation
+from qutip_qip.transpiler import to_chain_structure
+from qutip_qip.decompose.decompose_single_qubit_gate import _ZYZ_rotation
 
 import qutip as qp
 
 
 def _op_dist(A, B):
     return (A - B).norm()
 
@@ -101,54 +98,54 @@
                         pytest.param("CNOT", "SQRTISWAP",
                                         [0], [1], id="CNOTtoSQRTISWAP"),
                         pytest.param("CNOT", "ISWAP",
                                         [0], [1], id="CNOTtoISWAP")])
     def testresolve(self, gate_from, gate_to, targets, controls):
         qc1 = QubitCircuit(2)
         qc1.add_gate(gate_from, targets=targets, controls=controls)
-        U1 = gates.gate_sequence_product(qc1.propagators())
+        U1 = gate_sequence_product(qc1.propagators())
         qc2 = qc1.resolve_gates(basis=gate_to)
-        U2 = gates.gate_sequence_product(qc2.propagators())
+        U2 = gate_sequence_product(qc2.propagators())
         assert _op_dist(U1, U2) < 1e-12
 
     def testSNOTdecompose(self):
         """
         SNOT to rotation: compare unitary matrix for SNOT and product of
         resolved matrices in terms of rotation gates.
         """
         qc1 = QubitCircuit(1)
         qc1.add_gate("SNOT", targets=0)
-        U1 = gates.gate_sequence_product(qc1.propagators())
+        U1 = gate_sequence_product(qc1.propagators())
         qc2 = qc1.resolve_gates()
-        U2 = gates.gate_sequence_product(qc2.propagators())
+        U2 = gate_sequence_product(qc2.propagators())
         assert _op_dist(U1, U2) < 1e-12
 
     def testFREDKINdecompose(self):
         """
         FREDKIN to rotation and CNOT: compare unitary matrix for FREDKIN and product of
         resolved matrices in terms of rotation gates and CNOT.
         """
         qc1 = QubitCircuit(3)
         qc1.add_gate("FREDKIN", targets=[0, 1], controls=[2])
-        U1 = gates.gate_sequence_product(qc1.propagators())
+        U1 = gate_sequence_product(qc1.propagators())
         qc2 = qc1.resolve_gates()
-        U2 = gates.gate_sequence_product(qc2.propagators())
+        U2 = gate_sequence_product(qc2.propagators())
         assert _op_dist(U1, U2) < 1e-12
 
     def testadjacentgates(self):
         """
         Adjacent Gates: compare unitary matrix for ISWAP and product of
         resolved matrices in terms of adjacent gates interaction.
         """
         qc1 = QubitCircuit(3)
         qc1.add_gate("ISWAP", targets=[0, 2])
-        U1 = gates.gate_sequence_product(qc1.propagators())
+        U1 = gate_sequence_product(qc1.propagators())
         qc0 = qc1.adjacent_gates()
         qc2 = qc0.resolve_gates(basis="ISWAP")
-        U2 = gates.gate_sequence_product(qc2.propagators())
+        U2 = gate_sequence_product(qc2.propagators())
         assert _op_dist(U1, U2) < 1e-12
 
     def test_add_gate(self):
         """
         Addition of a gate object directly to a `QubitCircuit`
         """
         qc = QubitCircuit(6)
@@ -177,63 +174,14 @@
         assert qc.gates[5].name == "RY"
         assert qc.gates[5].targets == [4]
         assert qc.gates[5].arg_value == 1.570796
         assert qc.gates[6].name == "RY"
         assert qc.gates[6].targets == [5]
         assert qc.gates[5].arg_value == 1.570796
 
-        # Test Exceptions  # Global phase is not included
-        for gate in _single_qubit_gates:
-            if gate not in _para_gates:
-                # No target
-                pytest.raises(ValueError, qc.add_gate, gate, None, None)
-                # Multiple targets
-                pytest.raises(ValueError, qc.add_gate, gate, [0, 1, 2], None)
-                # With control
-                pytest.raises(ValueError, qc.add_gate, gate, [0], [1])
-            else:
-                # No target
-                pytest.raises(ValueError, qc.add_gate, gate, None, None, 1)
-                # Multiple targets
-                pytest.raises(ValueError, qc.add_gate, gate, [0, 1, 2], None, 1)
-                # With control
-                pytest.raises(ValueError, qc.add_gate, gate, [0], [1], 1)
-        for gate in _ctrl_gates:
-            if gate not in _para_gates:
-                # No target
-                pytest.raises(ValueError, qc.add_gate, gate, None, [1])
-                # No control
-                pytest.raises(ValueError, qc.add_gate, gate, [0], None)
-            else:
-                # No target
-                pytest.raises(ValueError, qc.add_gate, gate, None, [1], 1)
-                # No control
-                pytest.raises(ValueError, qc.add_gate, gate, [0], None, 1)
-        for gate in _swap_like:
-            if gate not in _para_gates:
-                # Single target
-                pytest.raises(ValueError, qc.add_gate, gate, [0], None)
-                # With control
-                pytest.raises(ValueError, qc.add_gate, gate, [0, 1], [3])
-            else:
-                # Single target
-                pytest.raises(ValueError, qc.add_gate, gate, [0], None, 1)
-                # With control
-                pytest.raises(ValueError, qc.add_gate, gate, [0, 1], [3], 1)
-        for gate in _fredkin_like:
-            # Single target
-            pytest.raises(ValueError, qc.add_gate, gate, [0], [2])
-            # No control
-            pytest.raises(ValueError, qc.add_gate, gate, [0, 1], None)
-        for gate in _toffoli_like:
-            # No target
-            pytest.raises(ValueError, qc.add_gate, gate, None, [1, 2])
-            # Single control
-            pytest.raises(ValueError, qc.add_gate, gate, [0], [1])
-
         dummy_gate1 = Gate("DUMMY1")
         inds = [1, 3, 4, 6]
         qc.add_gate(dummy_gate1, index=inds)
 
         # Test adding gates at multiple (sorted) indices at once.
         # NOTE: Every insertion shifts the indices in the original list of
         #       gates by an additional position to the right.
@@ -414,29 +362,14 @@
     def test_exceptions(self, gate):
         """
         Text exceptions are thrown correctly for inadequate inputs
         """
         qc = QubitCircuit(2)
         pytest.raises(ValueError, qc.add_gate, gate, targets=[1], controls=[0])
 
-    @pytest.mark.parametrize('gate', ['CY', 'CZ', 'CS', 'CT'])
-    def test_exceptions_controlled(self, gate):
-        """
-        Text exceptions are thrown correctly for inadequate inputs
-        """
-        qc = QubitCircuit(2)
-        '''
-        pytest.raises(ValueError, qc.add_gate, gate,
-                    targets=[1], controls=[0])
-        '''
-
-        pytest.raises(ValueError, qc.add_gate, gate,
-                      targets=[1])
-        pytest.raises(ValueError, qc.add_gate, gate)
-
     def test_globalphase_gate_propagators(self):
         qc = QubitCircuit(2)
         qc.add_gate("GLOBALPHASE", arg_value=np.pi / 2)
 
         [gate] = qc.gates
         assert gate.name == "GLOBALPHASE"
         assert gate.arg_value == np.pi / 2
@@ -588,14 +521,37 @@
         state_final = teleportation_sim_results.get_final_states(0)
 
         final_measurement = Measurement("start", targets=[2])
         _, final_probabilities = final_measurement.measurement_comp_basis(state_final)
 
         np.testing.assert_allclose(initial_probabilities, final_probabilities)
 
+    def test_classical_control(self):
+        qc = QubitCircuit(1, num_cbits=2)
+        qc.add_gate(
+            "X",
+            targets=[0],
+            classical_controls=[0, 1],
+            classical_control_value=1,
+        )
+        result = qc.run(basis(2, 0), cbits=[1, 0])
+        fid = qp.fidelity(result, basis(2, 0))
+        assert pytest.approx(fid, 1.0e-6) == 1
+
+        qc = QubitCircuit(1, num_cbits=2)
+        qc.add_gate(
+            "X",
+            targets=[0],
+            classical_controls=[0, 1],
+            classical_control_value=2,
+        )
+        result = qc.run(basis(2, 0), cbits=[1, 0])
+        fid = qp.fidelity(result, basis(2, 1))
+        assert pytest.approx(fid, 1.0e-6) == 1
+
     def test_runstatistics_teleportation(self):
         """
         Test circuit run_statistics on teleportation circuit
         """
 
         teleportation = _teleportation_circuit()
         final_measurement = Measurement("start", targets=[2])
@@ -781,23 +737,40 @@
         assert qc.latex_code() == self._latex_template % exp
 
     @pytest.mark.skipif(
                 shutil.which("pdflatex") is None,
                 reason="requires pdflatex"
                 )
     def test_export_image(self, in_temporary_directory):
-        from qutip_qip import circuit_latex
+        from qutip_qip import circuit
         qc = QubitCircuit(2, reverse_states=False)
         qc.add_gate("CSIGN", controls=[0], targets=[1])
 
-        if "png" in circuit_latex.CONVERTERS:
+        if "png" in circuit.CONVERTERS:
             file_png200 = "exported_pic_200.png"
             file_png400 = "exported_pic_400.png"
             qc.draw("png", 200, file_png200.split('.')[0], "")
             qc.draw("png", 400.5, file_png400.split('.')[0], "")
             assert file_png200 in os.listdir('.')
             assert file_png400 in os.listdir('.')
             assert os.stat(file_png200).st_size < os.stat(file_png400).st_size
-        if "svg" in circuit_latex.CONVERTERS:
+        if "svg" in circuit.CONVERTERS:
             file_svg = "exported_pic.svg"
             qc.draw("svg", file_svg.split('.')[0], "")
             assert file_svg in os.listdir('.')
+
+    def test_deprecation_warning(self):
+        # Make them available for backward compatibility.
+        with pytest.warns(DeprecationWarning):
+            from qutip_qip.circuit import Gate, Measurement
+            Gate("X", 0)
+
+    def test_circuit_chain_structure(self):
+        """
+        Test if the transpiler correctly inherit the properties of a circuit.
+        """
+        qc = QubitCircuit(3, reverse_states=True)
+        qc.add_gate("CNOT", 2, 0)
+        qc2 = to_chain_structure(qc)
+
+        assert qc2.reverse_states is True
+        assert qc2.input_states == [None] * 3
```

### Comparing `qutip-qip-0.2.3/tests/test_compiler.py` & `qutip-qip-0.3.0/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `qutip-qip-0.2.3/tests/test_device.py` & `qutip-qip-0.3.0/tests/test_device.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,15 @@
 import qutip
 from qutip_qip.circuit import QubitCircuit
 from qutip_qip.operations import Gate, gate_sequence_product
 from qutip_qip.device import (DispersiveCavityQED, LinearSpinChain,
                                 CircularSpinChain, SCQubits)
 
 from packaging.version import parse as parse_version
-if parse_version(qutip.__version__) < parse_version('5.dev'):
-    from qutip import Options as SolverOptions
-else:
-    from qutip import SolverOptions
+from qutip import Options
 
 _tol = 3.e-2
 
 _x = Gate("X", targets=[0])
 _z = Gate("Z", targets=[0])
 _y = Gate("Y", targets=[0])
 _snot = Gate("SNOT", targets=[0])
@@ -122,15 +119,15 @@
         extra = qutip.basis(device.dims[ancilla_indices], [0]*num_ancilla)
         init_state = qutip.tensor(extra, state)
     elif isinstance(device, SCQubits):
         # expand to 3-level represetnation
         init_state = _ket_expaned_dims(state, device.dims)
     else:
         init_state = state
-    options = SolverOptions(store_final_state=True, nsteps=50_000)
+    options = Options(store_final_state=True, nsteps=50_000)
     result = device.run_state(init_state=init_state,
                               analytical=False,
                               options=options)
     numerical_result = result.final_state
     if isinstance(device, DispersiveCavityQED):
         target = qutip.tensor(extra, target)
     elif isinstance(device, SCQubits):
@@ -179,33 +176,30 @@
         extra = qutip.basis(device.dims[ancilla_indices], [0]*num_ancilla)
         init_state = qutip.tensor(extra, state)
     elif isinstance(device, SCQubits):
         # expand to 3-level represetnation
         init_state = _ket_expaned_dims(state, device.dims)
     else:
         init_state = state
-    options = SolverOptions(store_final_state=True, nsteps=50_000)
+    options = Options(store_final_state=True, nsteps=50_000)
     result = device.run_state(init_state=init_state,
                               analytical=False,
                               options=options)
     if isinstance(device, DispersiveCavityQED):
         target = qutip.tensor(extra, target)
     elif isinstance(device, SCQubits):
         target = _ket_expaned_dims(target, device.dims)
     assert _tol > abs(1 - qutip.metrics.fidelity(result.final_state, target))
 
 
 @pytest.mark.parametrize(
     "processor_class",
     [DispersiveCavityQED, LinearSpinChain, CircularSpinChain, SCQubits])
 def test_pulse_plotting(processor_class):
-    try:
-        import matplotlib.pyplot as plt
-    except Exception:
-        return True
+    plt = pytest.importorskip("matplotlib.pyplot")
     qc = QubitCircuit(3)
     qc.add_gate("CNOT", 1, 0)
     qc.add_gate("X", 1)
 
     processor = processor_class(3)
     processor.load_circuit(qc)
     fig, ax = processor.plot_pulses()
```

### Comparing `qutip-qip-0.2.3/tests/test_gates.py` & `qutip-qip-0.3.0/tests/test_gates.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 from packaging.version import parse as parse_version
 import pytest
 import functools
 import itertools
 import numpy as np
 import qutip
 from qutip_qip.operations import gates
+from qutip_qip.circuit import QubitCircuit
+from qutip_qip.operations import (
+    X, Y, Z, RX, RY, RZ, H, SQRTNOT, S, T, QASMU, CNOT, CPHASE, ISWAP, SWAP,
+    CZ, SQRTSWAP, SQRTISWAP, SWAPALPHA, SWAPALPHA, MS, TOFFOLI, FREDKIN,
+    BERKELEY, R, expand_operator)
 
 
 def _permutation_id(permutation):
     return str(len(permutation)) + "-" + "".join(map(str, permutation))
 
 
 def _infidelity(a, b):
@@ -23,15 +28,15 @@
         operation = qutip.rand_unitary(8, dims=[[2] * 3] * 2)
     else:
         operation = qutip.rand_unitary([2] * 3)
 
     def gate(N=None, controls=None, target=None):
         if N is None:
             return operation
-        return gates.gate_expand_3toN(operation, N, controls, target)
+        return expand_operator(operation, dims=[2]*N, targets=controls + [target])
     return gate
 
 
 def _tensor_with_entanglement(all_qubits, entangled, entangled_locations):
     """
     Create a full tensor product when a subspace component is already in an
     entangled state.  The locations in `all_qubits` which are the entangled
@@ -95,17 +100,16 @@
         assert _infidelity(swapped, swap*start) < 1e-12
         assert _infidelity(start, swap*swap*start) < 1e-12
 
     @pytest.mark.parametrize('permutation',
                              tuple(itertools.permutations([0, 1, 2])),
                              ids=_permutation_id)
     def test_toffoli(self, permutation):
-        test = gates.toffoli(N=3,
-                             controls=permutation[:2],
-                             target=permutation[2])
+        test = expand_operator(
+            gates.toffoli(), dims=[2] * 3, targets=permutation)
         base = (qutip.tensor(1 - qutip.basis([2, 2], [1, 1]).proj(),
                              qutip.qeye(2))
                 + qutip.tensor(qutip.basis([2, 2], [1, 1]).proj(),
                                qutip.sigmax()))
         # Iterate the permutation once, equivalent to finding its inverse,
         # because for us, `permutation[n]` is where qubit `n` should be placed,
         # whereas `Qobj.permute` interprets that qubit `n` should be at the
@@ -169,14 +173,15 @@
                 # if np.allclose(gate.full(), pauli.full(), atol=1e-10):
                 if np.allclose(qutip.average_gate_fidelity(gate, pauli), 1):
                     del pauli_gates[i]
                     break
         assert len(pauli_gates) == 0
 
 
+@pytest.mark.filterwarnings('ignore::DeprecationWarning')
 class TestGateExpansion:
     """
     Test that gates act correctly when supplied with controls and targets, i.e.
     that they pick out the correct qubits to act on, the action is correct, and
     all other qubits are untouched.
     """
     n_qubits = 5
@@ -210,15 +215,15 @@
         pytest.param(gates.cy_gate, 1, id="cY"),
         pytest.param(gates.cz_gate, 1, id="cZ"),
         pytest.param(gates.cs_gate, 1, id="cS"),
         pytest.param(gates.ct_gate, 1, id="cT"),
         pytest.param(gates.swap, 0, id="swap"),
         pytest.param(gates.iswap, 0, id="iswap"),
         pytest.param(gates.sqrtswap, 0, id="sqrt(swap)"),
-        pytest.param(functools.partial(gates.molmer_sorensen, 0.5*np.pi), 0,
+        pytest.param(functools.partial(gates.molmer_sorensen, 0.5*np.pi, 0.), 0,
                      id="Molmer-Sorensen")
     ])
     def test_two_qubit(self, gate, n_controls):
         targets = [qutip.rand_ket(2) for _ in [None]*2]
         others = [qutip.rand_ket(2) for _ in [None]*self.n_qubits]
         reference = gate() * qutip.tensor(*targets)
         for q1, q2 in itertools.permutations(range(self.n_qubits), 2):
@@ -258,36 +263,40 @@
         'permutation',
         tuple(itertools.chain(*[
             itertools.permutations(range(k)) for k in [2, 3, 4]
         ])),
         ids=_permutation_id)
     def test_permutation_without_expansion(self, permutation):
         base = qutip.tensor([qutip.rand_unitary(2) for _ in permutation])
-        test = gates.expand_operator(base,
-                                     N=len(permutation), targets=permutation)
+        test = gates.expand_operator(
+            base,
+            dims=[2] * len(permutation),
+            targets=permutation)
         expected = base.permute(_apply_permutation(permutation))
         np.testing.assert_allclose(test.full(), expected.full(), atol=1e-15)
 
     @pytest.mark.parametrize('n_targets', range(1, 5))
     def test_general_qubit_expansion(self, n_targets):
         # Test all permutations with the given number of targets.
         n_qubits = 5
         if parse_version(qutip.__version__) < parse_version('5.dev'):
             operation = qutip.rand_unitary(2**n_targets, dims=[[2]*n_targets]*2)
         else:
             operation = qutip.rand_unitary([2]*n_targets)
         for targets in itertools.permutations(range(n_qubits), n_targets):
             expected = _tensor_with_entanglement([qutip.qeye(2)] * n_qubits,
                                                  operation, targets)
-            test = gates.expand_operator(operation, n_qubits, targets)
+            test = gates.expand_operator(
+                operation, dims=[2] * n_qubits, targets=targets)
             np.testing.assert_allclose(test.full(), expected.full(),
                                        atol=1e-15)
 
     def test_cnot_explicit(self):
-        test = gates.expand_operator(gates.cnot(), 3, [2, 0]).full()
+        test = gates.expand_operator(
+            gates.cnot(), dims=[2] * 3, targets=[2, 0]).full()
         expected = np.array([[1, 0, 0, 0, 0, 0, 0, 0],
                              [0, 0, 0, 0, 0, 1, 0, 0],
                              [0, 0, 1, 0, 0, 0, 0, 0],
                              [0, 0, 0, 0, 0, 0, 0, 1],
                              [0, 0, 0, 0, 1, 0, 0, 0],
                              [0, 1, 0, 0, 0, 0, 0, 0],
                              [0, 0, 0, 0, 0, 0, 1, 0],
@@ -307,35 +316,86 @@
                 [1, 1, -1, -1, -1, -1, 1, 1],
                 [1, -1, -1, 1, -1, 1, 1, -1],
             ]
         )
         expected = expected / np.sqrt(8)
         np.testing.assert_allclose(test, expected)
 
-    def test_cyclic_permutation(self):
-        operators = [qutip.sigmax(), qutip.sigmaz()]
-        test = gates.expand_operator(qutip.tensor(*operators), N=3,
-                                     targets=[0, 1], cyclic_permutation=True)
-        base_expected = qutip.tensor(*operators, qutip.qeye(2))
-        expected = [base_expected.permute(x)
-                    for x in [[0, 1, 2], [1, 2, 0], [2, 0, 1]]]
-        assert len(expected) == len(test)
-        for element in expected:
-            assert element in test
-
     @pytest.mark.parametrize('dimensions', [
         pytest.param([3, 4, 5], id="standard"),
         pytest.param([3, 3, 4, 4, 2], id="standard"),
         pytest.param([1, 2, 3], id="1D space"),
     ])
     def test_non_qubit_systems(self, dimensions):
         n_qubits = len(dimensions)
         for targets in itertools.permutations(range(n_qubits), 2):
             operators = [qutip.rand_unitary(dimension) if n in targets
                          else qutip.qeye(dimension)
                          for n, dimension in enumerate(dimensions)]
             expected = qutip.tensor(*operators)
             base_test = qutip.tensor(*[operators[x] for x in targets])
-            test = gates.expand_operator(base_test, N=n_qubits,
-                                         targets=targets, dims=dimensions)
+            test = gates.expand_operator(base_test, dims=dimensions,
+                                         targets=targets)
             assert test.dims == expected.dims
             np.testing.assert_allclose(test.full(), expected.full())
+
+def test_gates_class():
+    if parse_version(qutip.__version__) < parse_version('5.dev'):
+        init_state = qutip.rand_ket(8, dims=[[2, 2, 2], [1, 1, 1]])
+    else:
+        init_state = qutip.rand_ket([2, 2, 2])
+
+    circuit1 = QubitCircuit(3)
+    circuit1.add_gate("X", 1)
+    circuit1.add_gate("Y", 1)
+    circuit1.add_gate("Z", 2)
+    circuit1.add_gate("RX", 0, arg_value=np.pi/4)
+    circuit1.add_gate("RY", 0, arg_value=np.pi/4)
+    circuit1.add_gate("RZ", 1, arg_value=np.pi/4)
+    circuit1.add_gate("H", 0)
+    circuit1.add_gate("SQRTNOT", 0)
+    circuit1.add_gate("S", 2)
+    circuit1.add_gate("T", 1)
+    circuit1.add_gate("R", 1, arg_value=(np.pi/4, np.pi/6))
+    circuit1.add_gate("QASMU", 0, arg_value=(np.pi/4, np.pi/4, np.pi/4))
+    circuit1.add_gate("CNOT", controls=0, targets=1)
+    circuit1.add_gate("CPHASE", controls=0, targets=1, arg_value=np.pi/4)
+    circuit1.add_gate("SWAP", [0, 1])
+    circuit1.add_gate("ISWAP", [2, 1])
+    circuit1.add_gate("CZ", controls=0, targets=2)
+    circuit1.add_gate("SQRTSWAP", [2, 0])
+    circuit1.add_gate("SQRTISWAP", [0, 1])
+    circuit1.add_gate("SWAPALPHA", [1, 2], arg_value=np.pi/4)
+    circuit1.add_gate("MS", [1, 0], arg_value=(np.pi/4, np.pi/7))
+    circuit1.add_gate("TOFFOLI", [2, 0, 1])
+    circuit1.add_gate("FREDKIN", [0, 1, 2])
+    circuit1.add_gate("BERKELEY", [1, 0])
+    result1 = circuit1.run(init_state)
+
+    circuit2 = QubitCircuit(3)
+    circuit2.add_gate(X(1))
+    circuit2.add_gate(Y(1))
+    circuit2.add_gate(Z(2))
+    circuit2.add_gate(RX(0, np.pi/4))
+    circuit2.add_gate(RY(0, np.pi/4))
+    circuit2.add_gate(RZ(1, np.pi/4))
+    circuit2.add_gate(H(0))
+    circuit2.add_gate(SQRTNOT(0))
+    circuit2.add_gate(S(2))
+    circuit2.add_gate(T(1))
+    circuit2.add_gate(R(1, (np.pi/4, np.pi/6)))
+    circuit2.add_gate(QASMU(0, (np.pi/4, np.pi/4, np.pi/4)))
+    circuit2.add_gate(CNOT(0, 1))
+    circuit2.add_gate(CPHASE(0, 1, np.pi/4))
+    circuit2.add_gate(SWAP([0, 1]))
+    circuit2.add_gate(ISWAP([2, 1]))
+    circuit2.add_gate(CZ(0, 2))
+    circuit2.add_gate(SQRTSWAP([2, 0]))
+    circuit2.add_gate(SQRTISWAP([0, 1]))
+    circuit2.add_gate(SWAPALPHA([1, 2], np.pi/4))
+    circuit2.add_gate(MS([1, 0], (np.pi/4, np.pi/7)))
+    circuit2.add_gate(TOFFOLI([2, 0, 1]))
+    circuit2.add_gate(FREDKIN([0, 1, 2]))
+    circuit2.add_gate(BERKELEY([1, 0]))
+    result2 = circuit2.run(init_state)
+
+    assert pytest.approx(qutip.fidelity(result1, result2), 1.0e-6) == 1
```

### Comparing `qutip-qip-0.2.3/tests/test_measurement.py` & `qutip-qip-0.3.0/tests/test_measurement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import scipy
 import pytest
 from math import sqrt
-from qutip_qip.circuit import Measurement
+from qutip_qip.operations import Measurement
 from qutip import (Qobj, basis, ket2dm,
                     sigmax, sigmay, sigmaz, identity, tensor, rand_ket)
 from qutip.measurement import (measure_povm, measurement_statistics_povm,
                                 measure_observable,
                                 measurement_statistics_observable)
 import qutip
```

### Comparing `qutip-qip-0.2.3/tests/test_model.py` & `qutip-qip-0.3.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `qutip-qip-0.2.3/tests/test_noise.py` & `qutip-qip-0.3.0/tests/test_noise.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from numpy.testing import assert_, run_module_suite, assert_allclose
+from numpy.testing import assert_, assert_allclose
 import numpy as np
 import pytest
 
 from qutip import (
     tensor, qeye, sigmaz, sigmax, sigmay, destroy, identity, QobjEvo,
     fidelity, basis, sigmam
     )
@@ -11,18 +11,14 @@
     RelaxationNoise, DecoherenceNoise, ControlAmpNoise, RandomNoise,
     ZZCrossTalk, Noise)
 from qutip_qip.pulse import Pulse, Drift
 from qutip_qip.circuit import QubitCircuit
 
 import qutip
 from packaging.version import parse as parse_version
-if parse_version(qutip.__version__) >= parse_version('5.dev'):
-    is_qutip5 = True
-else:
-    is_qutip5 = False
 
 
 class TestNoise:
     def test_decoherence_noise(self):
         """
         Test for the decoherence noise
         """
```

### Comparing `qutip-qip-0.2.3/tests/test_optpulseprocessor.py` & `qutip-qip-0.3.0/tests/test_optpulseprocessor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 
-from numpy.testing import (assert_, run_module_suite, assert_allclose,
+from numpy.testing import (assert_, assert_allclose,
                            assert_equal)
 import numpy as np
 import pytest
 
 from qutip_qip.device import OptPulseProcessor, SpinChainModel
 from qutip_qip.circuit import QubitCircuit
 from qutip_qip.qubits import qubit_states
 import qutip
 from qutip import (fidelity, Qobj, tensor, rand_ket, basis,  sigmaz,
                     sigmax, sigmay, identity, destroy)
-from qutip_qip.operations import (cnot, gate_sequence_product,
-                                        hadamard_transform, expand_operator)
+from qutip_qip.operations import (
+    cnot, hadamard_transform, expand_operator, gate_sequence_product)
 import qutip
 from packaging.version import parse as parse_version
 if parse_version(qutip.__version__) < parse_version('5.dev'):
     from qutip import Options as SolverOptions
 else:
     from qutip import SolverOptions
```

### Comparing `qutip-qip-0.2.3/tests/test_processor.py` & `qutip-qip-0.3.0/tests/test_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 import os
 
 from packaging.version import parse as parse_version
 from numpy.testing import (
-    assert_, run_module_suite, assert_allclose, assert_equal)
+    assert_, assert_allclose, assert_equal)
 import numpy as np
 import pytest
 
 import qutip
-if parse_version(qutip.__version__) < parse_version('5.dev'):
-    from qutip import Options as SolverOptions
-else:
-    from qutip import SolverOptions
 from qutip_qip.device import Processor, LinearSpinChain
 from qutip import (
     basis, sigmaz, sigmax, sigmay, identity, destroy, tensor,
     rand_ket, rand_dm, fidelity)
 from qutip_qip.operations import hadamard_transform
 from qutip_qip.noise import (
     DecoherenceNoise, RandomNoise, ControlAmpNoise)
 from qutip_qip.qubits import qubit_states
 from qutip_qip.pulse import Pulse
 from qutip_qip.circuit import QubitCircuit
-if parse_version(qutip.__version__) < parse_version('5.dev'):
-    from qutip import Options as SolverOptions
-else:
-    from qutip import SolverOptions
+from qutip import Options
 
 
 class TestCircuitProcessor:
     def test_control_and_coeffs(self):
         processor = Processor(2)
         processor.add_control(sigmax())
         processor.add_control(sigmaz())
@@ -92,15 +85,15 @@
         """
         N = 1
         proc = Processor(N=N)
         init_state = rand_ket(2)
         tlist = [0., 1., 2.]
         proc.add_pulse(Pulse(identity(2), 0, tlist, False))
         result = proc.run_state(
-            init_state, options=SolverOptions(store_final_state=True))
+            init_state, options=Options(store_final_state=True))
         global_phase = init_state[0, 0]/result.final_state[0, 0]
         assert_allclose(
             global_phase*result.final_state.full(), init_state.full())
 
     def test_id_with_T1_T2(self):
         """
         Test for identity evolution with relaxation t1 and t2
@@ -146,18 +139,16 @@
             err_msg="Error in t1 & t2 simulation, "
                     "with t1={} and t2={}".format(t1, t2))
 
     def test_plot(self):
         """
         Test for plotting functions
         """
-        try:
-            import matplotlib.pyplot as plt
-        except Exception:
-            return True
+        plt = pytest.importorskip("matplotlib.pyplot")
+
         # step_func
         tlist = np.linspace(0., 2*np.pi, 20)
         processor = Processor(N=1, spline_kind="step_func")
         processor.add_control(sigmaz(), label="sz")
         processor.set_all_coeffs({"sz": np.array([np.sin(t) for t in tlist])})
         processor.set_all_tlist(tlist)
         fig, _ = processor.plot_pulses(use_control_latex=False)
@@ -403,15 +394,15 @@
         qc.add_gate("X", targets=[0])
         processor = LinearSpinChain(num_qubits)
         processor.load_circuit(qc)
 
         # No max_step
         final_state = processor.run_state(
             init_state,
-            options=SolverOptions(max_step=10000)  # too large max_step
+            options=Options(max_step=10000)  # too large max_step
         ).states[-1]
         expected_state = tensor([basis(2, 0), basis(2, 1)])
         assert pytest.approx(fidelity(final_state, expected_state), 0.001) == 0
 
         # With default max_step
         final_state = processor.run_state(init_state).states[-1]
         expected_state = tensor([basis(2, 0), basis(2, 1)])
```

### Comparing `qutip-qip-0.2.3/tests/test_pulse.py` & `qutip-qip-0.3.0/tests/test_pulse.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from packaging.version import parse as parse_version
 import numpy as np
-from numpy.testing import assert_, run_module_suite, assert_allclose
+from numpy.testing import assert_, assert_allclose
 import pytest
 
 import qutip
 from qutip import (
     Qobj, sigmax, sigmay, sigmaz, identity, tensor, QobjEvo
 )
 from qutip_qip.pulse import Pulse, Drift
```

### Comparing `qutip-qip-0.2.3/tests/test_qasm.py` & `qutip-qip-0.3.0/tests/test_qasm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 import numpy as np
 from pathlib import Path
 
 from qutip_qip.qasm import read_qasm, circuit_to_qasm_str
-from qutip_qip.circuit import Measurement, QubitCircuit
+from qutip_qip.circuit import QubitCircuit
 from qutip import tensor, rand_ket, basis, rand_dm, identity
-from qutip_qip.operations import cnot, ry
+from qutip_qip.operations import cnot, ry, Measurement
 
 
 @pytest.mark.parametrize(["filename", "error", "error_message"], [
     pytest.param("command_error.qasm", SyntaxError,
                  "QASM: post is not a valid QASM command."),
     pytest.param("bracket_error.qasm", SyntaxError,
                  "QASM: incorrect bracket formatting"),
@@ -19,20 +19,20 @@
     filepath = Path(__file__).parent / 'qasm_files' / filename
     with pytest.raises(error) as exc_info:
         read_qasm(filepath)
     assert error_message in str(exc_info.value)
 
 
 def check_gate_defn(gate, gate_name, targets, controls=None,
-                    classical_controls=None, control_value=None):
+                    classical_controls=None, classical_control_value=None):
     assert gate.name == gate_name
     assert gate.targets == targets
     assert gate.controls == controls
     assert gate.classical_controls == classical_controls
-    assert gate.control_value == control_value
+    assert gate.classical_control_value == classical_control_value
 
 
 def check_measurement_defn(gate, gate_name, targets, classical_store):
     assert gate.name == gate_name
     assert gate.targets == targets
     assert gate.classical_store == classical_store
```

### Comparing `qutip-qip-0.2.3/tests/test_qft.py` & `qutip-qip-0.3.0/tests/test_qft.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from numpy.testing import assert_, assert_equal, assert_string_equal, run_module_suite
+from numpy.testing import assert_, assert_equal, assert_string_equal
 from qutip_qip.algorithms.qft import qft, qft_steps, qft_gate_sequence
 from qutip_qip.operations import gate_sequence_product
 
 
 class TestQFT:
     """
     A test class for the QuTiP functions for QFT
@@ -55,10 +55,7 @@
         qft: Inspect swap gates added to gate sequences if
         it is decomposed into cnot.
         """
         for N in range(1, 6):
             circuit = qft_gate_sequence(N, swapping=False, to_cnot=True)
 
         assert not any([gate.name == "CPHASE" for gate in circuit.gates])
-
-if __name__ == "__main__":
-    run_module_suite()
```

### Comparing `qutip-qip-0.2.3/tests/test_qubits.py` & `qutip-qip-0.3.0/tests/test_qubits.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from numpy.testing import assert_, run_module_suite
+from numpy.testing import assert_
 from qutip_qip.qubits import qubit_states
 from qutip import (tensor,  basis) 
 
 
 class TestQubits:
     """
     A test class for the QuTiP functions for qubits.
@@ -18,11 +18,7 @@
         psi1_a = basis(2, 1)
         psi1_b = qubit_states(states=[1])
         assert_(psi1_a == psi1_b)
 
         psi01_a = tensor(psi0_a, psi1_a)
         psi01_b = qubit_states(N=2, states=[0, 1])
         assert_(psi01_a == psi01_b)
-
-
-if __name__ == "__main__":
-    run_module_suite()
```

### Comparing `qutip-qip-0.2.3/tests/test_scheduler.py` & `qutip-qip-0.3.0/tests/test_scheduler.py`

 * *Files identical despite different names*

