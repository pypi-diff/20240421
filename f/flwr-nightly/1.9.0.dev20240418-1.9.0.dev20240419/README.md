# Comparing `tmp/flwr_nightly-1.9.0.dev20240418.tar.gz` & `tmp/flwr_nightly-1.9.0.dev20240419.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.9.0.dev20240418.tar", max compression
+gzip compressed data, was "flwr_nightly-1.9.0.dev20240419.tar", max compression
```

## Comparing `flwr_nightly-1.9.0.dev20240418.tar` & `flwr_nightly-1.9.0.dev20240419.tar`

### file list

```diff
@@ -1,210 +1,212 @@
--rw-r--r--   0        0        0    11358 2024-04-18 23:05:56.600567 flwr_nightly-1.9.0.dev20240418/LICENSE
--rw-r--r--   0        0        0    12916 2024-04-18 23:05:56.600567 flwr_nightly-1.9.0.dev20240418/README.md
--rw-r--r--   0        0        0     5836 2024-04-18 23:06:14.592406 flwr_nightly-1.9.0.dev20240418/pyproject.toml
--rw-r--r--   0        0        0      937 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/__init__.py
--rw-r--r--   0        0        0      720 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/app.py
--rw-r--r--   0        0        0     4696 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/config_utils.py
--rw-r--r--   0        0        0     2215 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/example.py
--rw-r--r--   0        0        0      789 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/__init__.py
--rw-r--r--   0        0        0     5380 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/new.py
--rw-r--r--   0        0        0      725 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/__init__.py
--rw-r--r--   0        0        0     3078 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/.gitignore.tpl
--rw-r--r--   0        0        0      668 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/README.md.tpl
--rw-r--r--   0        0        0      729 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/__init__.py
--rw-r--r--   0        0        0      736 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/__init__.py
--rw-r--r--   0        0        0       21 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
--rw-r--r--   0        0        0      521 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
--rw-r--r--   0        0        0     1173 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
--rw-r--r--   0        0        0       48 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
--rw-r--r--   0        0        0      248 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
--rw-r--r--   0        0        0      594 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
--rw-r--r--   0        0        0       48 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
--rw-r--r--   0        0        0     3684 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
--rw-r--r--   0        0        0      489 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
--rw-r--r--   0        0        0      558 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
--rw-r--r--   0        0        0      537 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
--rw-r--r--   0        0        0      789 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/run/__init__.py
--rw-r--r--   0        0        0     2331 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/run/run.py
--rw-r--r--   0        0        0     4153 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/utils.py
--rw-r--r--   0        0        0     1187 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    26193 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     8183 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     8636 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/client_app.py
--rw-r--r--   0        0        0     7435 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      735 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     8717 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      752 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     8560 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0     2404 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/heartbeat.py
--rw-r--r--   0        0        0      719 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     6553 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1824 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     1143 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/__init__.py
--rw-r--r--   0        0        0     5397 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/centraldp_mods.py
--rw-r--r--   0        0        0     2623 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/comms_mods.py
--rw-r--r--   0        0        0     4918 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/localdp_mod.py
--rw-r--r--   0        0        0      849 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     1095 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
--rw-r--r--   0        0        0    19699 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
--rw-r--r--   0        0        0     1226 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/utils.py
--rw-r--r--   0        0        0     1778 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/node_state.py
--rw-r--r--   0        0        0     2195 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/node_state_tests.py
--rw-r--r--   0        0        0    10283 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      735 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0    14456 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     1006 2024-04-18 23:05:57.020564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/typing.py
--rw-r--r--   0        0        0     3721 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1882 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     2424 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0     1313 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/context.py
--rw-r--r--   0        0        0      891 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     6113 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/differential_privacy.py
--rw-r--r--   0        0        0     1074 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/differential_privacy_constants.py
--rw-r--r--   0        0        0     2004 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     2812 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/exit_handlers.py
--rw-r--r--   0        0        0     2273 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     6096 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0    12385 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/message.py
--rw-r--r--   0        0        0     4961 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/object_ref.py
--rw-r--r--   0        0        0     2095 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0     1385 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/pyproject.py
--rw-r--r--   0        0        0     1054 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/__init__.py
--rw-r--r--   0        0        0     4652 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/configsrecord.py
--rw-r--r--   0        0        0     1393 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/conversion_utils.py
--rw-r--r--   0        0        0     3923 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/metricsrecord.py
--rw-r--r--   0        0        0     4849 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/parametersrecord.py
--rw-r--r--   0        0        0     4553 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/recordset.py
--rw-r--r--   0        0        0     3879 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/typeddict.py
--rw-r--r--   0        0        0    13798 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/recordset_compat.py
--rw-r--r--   0        0        0    11707 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/retry_invoker.py
--rw-r--r--   0        0        0      731 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/__init__.py
--rw-r--r--   0        0        0      738 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/crypto/__init__.py
--rw-r--r--   0        0        0     2792 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/crypto/shamir.py
--rw-r--r--   0        0        0     3546 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
--rw-r--r--   0        0        0     3026 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
--rw-r--r--   0        0        0     2310 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/quantization.py
--rw-r--r--   0        0        0     2183 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
--rw-r--r--   0        0        0     3221 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
--rw-r--r--   0        0        0    22250 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7782 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     4382 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      666 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      683 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     3207 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     5016 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     7304 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     2022 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     1084 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/error_pb2.py
--rw-r--r--   0        0        0      734 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/error_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/error_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/error_pb2_grpc.pyi
--rw-r--r--   0        0        0     5018 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     9161 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0    10605 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2811 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1081 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     6009 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/recordset_pb2.py
--rw-r--r--   0        0        0    14161 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/recordset_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/recordset_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/recordset_pb2_grpc.pyi
--rw-r--r--   0        0        0     2472 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4320 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0     9781 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1785 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    24302 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6127 2024-04-18 23:05:57.024564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2399 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0      892 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/__init__.py
--rw-r--r--   0        0        0     5271 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/app.py
--rw-r--r--   0        0        0     3496 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/app_utils.py
--rw-r--r--   0        0        0     7344 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/driver_client_proxy.py
--rw-r--r--   0        0        0     1766 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/legacy_context.py
--rw-r--r--   0        0        0     1061 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      820 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     5090 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/driver/abc_driver.py
--rw-r--r--   0        0        0    10106 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/driver/driver.py
--rw-r--r--   0        0        0     4586 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/driver/grpc_driver.py
--rw-r--r--   0        0        0     5121 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/history.py
--rw-r--r--   0        0        0     5592 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/run_serverapp.py
--rw-r--r--   0        0        0    17664 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/server.py
--rw-r--r--   0        0        0     4402 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/server_app.py
--rw-r--r--   0        0        0     1349 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/server_config.py
--rw-r--r--   0        0        0     2836 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0    13468 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     6532 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/bulyan.py
--rw-r--r--   0        0        0    17458 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/dp_adaptive_clipping.py
--rw-r--r--   0        0        0    12904 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/dp_fixed_clipping.py
--rw-r--r--   0        0        0     4877 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     7219 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5900 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6505 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     6763 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11799 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9784 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8132 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2704 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5242 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     6862 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5890 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     6080 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedxgb_bagging.py
--rw-r--r--   0        0        0     5607 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedxgb_cyclic.py
--rw-r--r--   0        0        0     4047 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     6801 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6285 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10150 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7543 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      707 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/__init__.py
--rw-r--r--   0        0        0      712 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/driver/__init__.py
--rw-r--r--   0        0        0     1932 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/driver/driver_grpc.py
--rw-r--r--   0        0        0     4780 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/driver/driver_servicer.py
--rw-r--r--   0        0        0      711 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/__init__.py
--rw-r--r--   0        0        0      735 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     5993 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6458 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4887 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11818 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0      758 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     3387 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      731 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     3473 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      735 2024-04-18 23:05:57.028564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     7621 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0      783 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/__init__.py
--rw-r--r--   0        0        0     1466 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
--rw-r--r--   0        0        0     2260 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
--rw-r--r--   0        0        0     6375 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
--rw-r--r--   0        0        0    12454 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/vce_api.py
--rw-r--r--   0        0        0     1003 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/__init__.py
--rw-r--r--   0        0        0    10083 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/in_memory_state.py
--rw-r--r--   0        0        0    24580 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/sqlite_state.py
--rw-r--r--   0        0        0     6762 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/state.py
--rw-r--r--   0        0        0     1654 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/state_factory.py
--rw-r--r--   0        0        0     2207 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/utils.py
--rw-r--r--   0        0        0      913 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/typing.py
--rw-r--r--   0        0        0      908 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5485 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     5301 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0      902 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/__init__.py
--rw-r--r--   0        0        0     1082 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/constant.py
--rw-r--r--   0        0        0    12547 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/default_workflows.py
--rw-r--r--   0        0        0      880 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     5838 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
--rw-r--r--   0        0        0    29038 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
--rw-r--r--   0        0        0     1400 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0    13904 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      734 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0    19367 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/ray_transport/ray_actor.py
--rw-r--r--   0        0        0     6738 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0     2392 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/ray_transport/utils.py
--rw-r--r--   0        0        0    15685 2024-04-18 23:05:57.032564 flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/run_simulation.py
--rw-r--r--   0        0        0    15260 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240418/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-19 23:05:27.660393 flwr_nightly-1.9.0.dev20240419/LICENSE
+-rw-r--r--   0        0        0    12916 2024-04-19 23:05:27.660393 flwr_nightly-1.9.0.dev20240419/README.md
+-rw-r--r--   0        0        0     5883 2024-04-19 23:05:41.312365 flwr_nightly-1.9.0.dev20240419/pyproject.toml
+-rw-r--r--   0        0        0      937 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0      720 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/app.py
+-rw-r--r--   0        0        0     5597 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/config_utils.py
+-rw-r--r--   0        0        0     2215 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/example.py
+-rw-r--r--   0        0        0      789 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/__init__.py
+-rw-r--r--   0        0        0     5380 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/new.py
+-rw-r--r--   0        0        0      725 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/__init__.py
+-rw-r--r--   0        0        0     3078 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/.gitignore.tpl
+-rw-r--r--   0        0        0      668 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/README.md.tpl
+-rw-r--r--   0        0        0      729 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/__init__.py
+-rw-r--r--   0        0        0      736 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/code/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
+-rw-r--r--   0        0        0      521 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
+-rw-r--r--   0        0        0     1173 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
+-rw-r--r--   0        0        0     1911 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
+-rw-r--r--   0        0        0      248 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
+-rw-r--r--   0        0        0      594 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
+-rw-r--r--   0        0        0      371 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
+-rw-r--r--   0        0        0     3684 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
+-rw-r--r--   0        0        0      489 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
+-rw-r--r--   0        0        0      558 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
+-rw-r--r--   0        0        0      537 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
+-rw-r--r--   0        0        0      789 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/run/__init__.py
+-rw-r--r--   0        0        0     2331 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/run/run.py
+-rw-r--r--   0        0        0     4153 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/utils.py
+-rw-r--r--   0        0        0     1262 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    24670 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     8183 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     8636 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/client_app.py
+-rw-r--r--   0        0        0     7435 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     8775 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      752 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     9052 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0     2404 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/heartbeat.py
+-rw-r--r--   0        0        0      719 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6553 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1824 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     1143 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/mod/__init__.py
+-rw-r--r--   0        0        0     5397 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/mod/centraldp_mods.py
+-rw-r--r--   0        0        0     2623 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/mod/comms_mods.py
+-rw-r--r--   0        0        0     4918 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/mod/localdp_mod.py
+-rw-r--r--   0        0        0      849 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/mod/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-19 23:05:28.076392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
+-rw-r--r--   0        0        0    19699 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
+-rw-r--r--   0        0        0     1226 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/mod/utils.py
+-rw-r--r--   0        0        0     1778 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/node_state.py
+-rw-r--r--   0        0        0     2195 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/node_state_tests.py
+-rw-r--r--   0        0        0    10283 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0    11302 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0      793 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/supernode/__init__.py
+-rw-r--r--   0        0        0     3436 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/supernode/app.py
+-rw-r--r--   0        0        0     1006 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/typing.py
+-rw-r--r--   0        0        0     3721 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1882 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     2424 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0     1313 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/context.py
+-rw-r--r--   0        0        0      891 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     6113 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/differential_privacy.py
+-rw-r--r--   0        0        0     1074 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/differential_privacy_constants.py
+-rw-r--r--   0        0        0     2004 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     2812 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/exit_handlers.py
+-rw-r--r--   0        0        0     2273 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     6096 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0    12385 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/message.py
+-rw-r--r--   0        0        0     4961 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/object_ref.py
+-rw-r--r--   0        0        0     2095 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0     1385 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/pyproject.py
+-rw-r--r--   0        0        0     1054 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/record/__init__.py
+-rw-r--r--   0        0        0     4652 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/record/configsrecord.py
+-rw-r--r--   0        0        0     1393 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/record/conversion_utils.py
+-rw-r--r--   0        0        0     3923 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/record/metricsrecord.py
+-rw-r--r--   0        0        0     4849 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/record/parametersrecord.py
+-rw-r--r--   0        0        0     4553 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/record/recordset.py
+-rw-r--r--   0        0        0     3879 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/record/typeddict.py
+-rw-r--r--   0        0        0    13798 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/recordset_compat.py
+-rw-r--r--   0        0        0    11707 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/retry_invoker.py
+-rw-r--r--   0        0        0      731 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/secure_aggregation/crypto/__init__.py
+-rw-r--r--   0        0        0     2792 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/secure_aggregation/crypto/shamir.py
+-rw-r--r--   0        0        0     3546 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
+-rw-r--r--   0        0        0     3026 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
+-rw-r--r--   0        0        0     2310 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/secure_aggregation/quantization.py
+-rw-r--r--   0        0        0     2183 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
+-rw-r--r--   0        0        0     3221 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
+-rw-r--r--   0        0        0    22250 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7865 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     4382 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      666 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      683 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     3207 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     5016 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     7304 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     2022 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1084 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/error_pb2.py
+-rw-r--r--   0        0        0      734 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/error_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/error_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/error_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5018 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     9161 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0    10605 2024-04-19 23:05:28.080392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2811 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1081 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6009 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/recordset_pb2.py
+-rw-r--r--   0        0        0    14161 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/recordset_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/recordset_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/recordset_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2472 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4320 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9781 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1785 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    24199 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6127 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2399 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0      892 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/compat/__init__.py
+-rw-r--r--   0        0        0     5271 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/compat/app.py
+-rw-r--r--   0        0        0     3496 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/compat/app_utils.py
+-rw-r--r--   0        0        0     7344 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/compat/driver_client_proxy.py
+-rw-r--r--   0        0        0     1766 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/compat/legacy_context.py
+-rw-r--r--   0        0        0     1061 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      820 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     5090 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/driver/abc_driver.py
+-rw-r--r--   0        0        0    10106 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/driver/driver.py
+-rw-r--r--   0        0        0     4586 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/driver/grpc_driver.py
+-rw-r--r--   0        0        0     5121 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0     5592 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/run_serverapp.py
+-rw-r--r--   0        0        0    17664 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0     4402 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/server_app.py
+-rw-r--r--   0        0        0     1349 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/server_config.py
+-rw-r--r--   0        0        0     2836 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0    13468 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     6532 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/bulyan.py
+-rw-r--r--   0        0        0    17458 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/dp_adaptive_clipping.py
+-rw-r--r--   0        0        0    12904 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/dp_fixed_clipping.py
+-rw-r--r--   0        0        0     4877 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     7219 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5900 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6505 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     6763 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11799 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9784 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8132 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2704 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5242 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     6862 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5890 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     6080 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedxgb_bagging.py
+-rw-r--r--   0        0        0     5607 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedxgb_cyclic.py
+-rw-r--r--   0        0        0     4047 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     6801 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6285 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10150 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7543 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      707 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/driver/__init__.py
+-rw-r--r--   0        0        0     1932 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/driver/driver_grpc.py
+-rw-r--r--   0        0        0     4780 2024-04-19 23:05:28.084392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/driver/driver_servicer.py
+-rw-r--r--   0        0        0      711 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/__init__.py
+-rw-r--r--   0        0        0      735 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     5993 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6458 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4887 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11818 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0      758 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     3387 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      731 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     3622 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      735 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     7621 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0      783 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/vce/__init__.py
+-rw-r--r--   0        0        0     1466 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
+-rw-r--r--   0        0        0     2260 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
+-rw-r--r--   0        0        0     6375 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
+-rw-r--r--   0        0        0    12454 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/vce/vce_api.py
+-rw-r--r--   0        0        0     1003 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/state/__init__.py
+-rw-r--r--   0        0        0    10083 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/state/in_memory_state.py
+-rw-r--r--   0        0        0    24580 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/state/sqlite_state.py
+-rw-r--r--   0        0        0     6762 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/state/state.py
+-rw-r--r--   0        0        0     1654 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/state/state_factory.py
+-rw-r--r--   0        0        0     2207 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/state/utils.py
+-rw-r--r--   0        0        0      913 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/typing.py
+-rw-r--r--   0        0        0      908 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5485 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     5301 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0      902 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/workflow/__init__.py
+-rw-r--r--   0        0        0     1082 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/workflow/constant.py
+-rw-r--r--   0        0        0    12547 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/workflow/default_workflows.py
+-rw-r--r--   0        0        0      880 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/workflow/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     5838 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
+-rw-r--r--   0        0        0    29038 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
+-rw-r--r--   0        0        0     1400 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0    13904 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      734 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0    19367 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/simulation/ray_transport/ray_actor.py
+-rw-r--r--   0        0        0     6738 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0     2392 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/simulation/ray_transport/utils.py
+-rw-r--r--   0        0        0    15685 2024-04-19 23:05:28.088392 flwr_nightly-1.9.0.dev20240419/src/py/flwr/simulation/run_simulation.py
+-rw-r--r--   0        0        0    15260 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240419/PKG-INFO
```

### Comparing `flwr_nightly-1.9.0.dev20240418/LICENSE` & `flwr_nightly-1.9.0.dev20240419/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/README.md` & `flwr_nightly-1.9.0.dev20240419/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/pyproject.toml` & `flwr_nightly-1.9.0.dev20240419/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.9.0.dev20240418"
+version = "1.9.0.dev20240419"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.ai>"]
 readme = "README.md"
 homepage = "https://flower.ai"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.ai"
@@ -52,14 +52,15 @@
 ]
 
 [tool.poetry.scripts]
 flwr = "flwr.cli.app:app"
 flower-driver-api = "flwr.server:run_driver_api"
 flower-fleet-api = "flwr.server:run_fleet_api"
 flower-superlink = "flwr.server:run_superlink"
+flower-supernode = "flwr.client:run_supernode"
 flower-client-app = "flwr.client:run_client_app"
 flower-server-app = "flwr.server:run_server_app"
 flower-simulation = "flwr.simulation:run_simulation_from_cli"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 # Mandatory dependencies
```

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/app.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/config_utils.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/config_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,21 +11,54 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Utility to validate the `pyproject.toml` file."""
 
 import os
+from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple
 
 import tomli
+import typer
 
 from flwr.common import object_ref
 
 
+def validate_project_dir(project_dir: Path) -> Optional[Dict[str, Any]]:
+    """Check if a Flower App directory is valid."""
+    config = load(str(project_dir / "pyproject.toml"))
+    if config is None:
+        typer.secho(
+            "❌ Project configuration could not be loaded. "
+            "`pyproject.toml` does not exist.",
+            fg=typer.colors.RED,
+            bold=True,
+        )
+        return None
+
+    if not validate(config):
+        typer.secho(
+            "❌ Project configuration is invalid.",
+            fg=typer.colors.RED,
+            bold=True,
+        )
+        return None
+
+    if "publisher" not in config["flower"]:
+        typer.secho(
+            "❌ Project configuration is missing required `publisher` field.",
+            fg=typer.colors.RED,
+            bold=True,
+        )
+        return None
+
+    return config
+
+
 def load_and_validate_with_defaults(
     path: Optional[str] = None,
 ) -> Tuple[Optional[Dict[str, Any]], List[str], List[str]]:
     """Load and validate pyproject.toml as dict.
 
     Returns
     -------
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/example.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/example.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/new.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/new.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/.gitignore.tpl` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/.gitignore.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/README.md.tpl` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/README.md.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/code/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/run/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/run/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/run/run.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/run/run.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/cli/utils.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/cli/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/app.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,22 +43,23 @@
 from flwr.common.retry_invoker import RetryInvoker, exponential
 
 from .grpc_client.connection import grpc_connection
 from .grpc_rere_client.connection import grpc_request_response
 from .message_handler.message_handler import handle_control_message
 from .node_state import NodeState
 from .numpy_client import NumPyClient
+from .supernode.app import parse_args_run_client_app
 
 
 def run_client_app() -> None:
     """Run Flower client app."""
-    event(EventType.RUN_CLIENT_APP_ENTER)
-
     log(INFO, "Long-running Flower client starting")
 
+    event(EventType.RUN_CLIENT_APP_ENTER)
+
     args = _parse_args_run_client_app().parse_args()
 
     # Obtain certificates
     if args.insecure:
         if args.root_certificates is not None:
             sys.exit(
                 "Conflicting options: The '--insecure' flag disables HTTPS, "
@@ -127,64 +128,15 @@
 
 def _parse_args_run_client_app() -> argparse.ArgumentParser:
     """Parse flower-client-app command line arguments."""
     parser = argparse.ArgumentParser(
         description="Start a Flower client app",
     )
 
-    parser.add_argument(
-        "client-app",
-        help="For example: `client:app` or `project.package.module:wrapper.app`",
-    )
-    parser.add_argument(
-        "--insecure",
-        action="store_true",
-        help="Run the client without HTTPS. By default, the client runs with "
-        "HTTPS enabled. Use this flag only if you understand the risks.",
-    )
-    parser.add_argument(
-        "--rest",
-        action="store_true",
-        help="Use REST as a transport layer for the client.",
-    )
-    parser.add_argument(
-        "--root-certificates",
-        metavar="ROOT_CERT",
-        type=str,
-        help="Specifies the path to the PEM-encoded root certificate file for "
-        "establishing secure HTTPS connections.",
-    )
-    parser.add_argument(
-        "--server",
-        default="0.0.0.0:9092",
-        help="Server address",
-    )
-    parser.add_argument(
-        "--max-retries",
-        type=int,
-        default=None,
-        help="The maximum number of times the client will try to connect to the"
-        "server before giving up in case of a connection error. By default,"
-        "it is set to None, meaning there is no limit to the number of tries.",
-    )
-    parser.add_argument(
-        "--max-wait-time",
-        type=float,
-        default=None,
-        help="The maximum duration before the client stops trying to"
-        "connect to the server in case of connection error. By default, it"
-        "is set to None, meaning there is no limit to the total time.",
-    )
-    parser.add_argument(
-        "--dir",
-        default="",
-        help="Add specified directory to the PYTHONPATH and load Flower "
-        "app from there."
-        " Default: current working directory.",
-    )
+    parse_args_run_client_app(parser=parser)
 
     return parser
 
 
 def _check_actionable_client(
     client: Optional[Client], client_fn: Optional[ClientFn]
 ) -> None:
@@ -438,15 +390,16 @@
         with connection(
             address,
             insecure,
             retry_invoker,
             grpc_max_message_length,
             root_certificates,
         ) as conn:
-            receive, send, create_node, delete_node = conn
+            # pylint: disable-next=W0612
+            receive, send, create_node, delete_node, get_run = conn
 
             # Register node
             if create_node is not None:
                 create_node()  # pylint: disable=not-callable
 
             while True:
                 # Receive
@@ -656,14 +609,15 @@
         [str, bool, RetryInvoker, int, Union[bytes, str, None]],
         ContextManager[
             Tuple[
                 Callable[[], Optional[Message]],
                 Callable[[Message], None],
                 Optional[Callable[[], None]],
                 Optional[Callable[[], None]],
+                Optional[Callable[[int], Tuple[str, str]]],
             ]
         ],
     ],
     str,
     Type[Exception],
 ]:
     # Parse IP address
```

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/client.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/client_app.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/client_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/grpc_client/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     root_certificates: Optional[Union[bytes, str]] = None,
 ) -> Iterator[
     Tuple[
         Callable[[], Optional[Message]],
         Callable[[Message], None],
         Optional[Callable[[], None]],
         Optional[Callable[[], None]],
+        Optional[Callable[[int], Tuple[str, str]]],
     ]
 ]:
     """Establish a gRPC connection to a gRPC server.
 
     Parameters
     ----------
     server_address : str
@@ -220,12 +221,12 @@
             raise ValueError(f"Invalid message type: {message_type}")
 
         # Send ClientMessage proto
         return queue.put(msg_proto, block=False)
 
     try:
         # Yield methods
-        yield (receive, send, None, None)
+        yield (receive, send, None, None, None)
     finally:
         # Make sure to have a final
         channel.close()
         log(DEBUG, "gRPC channel closed")
```

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,16 @@
 from flwr.common.logger import log
 from flwr.common.message import Message, Metadata
 from flwr.common.retry_invoker import RetryInvoker
 from flwr.common.serde import message_from_taskins, message_to_taskres
 from flwr.proto.fleet_pb2 import (  # pylint: disable=E0611
     CreateNodeRequest,
     DeleteNodeRequest,
+    GetRunRequest,
+    GetRunResponse,
     PingRequest,
     PingResponse,
     PullTaskInsRequest,
     PushTaskResRequest,
 )
 from flwr.proto.fleet_pb2_grpc import FleetStub  # pylint: disable=E0611
 from flwr.proto.node_pb2 import Node  # pylint: disable=E0611
@@ -65,14 +67,15 @@
     root_certificates: Optional[Union[bytes, str]] = None,
 ) -> Iterator[
     Tuple[
         Callable[[], Optional[Message]],
         Callable[[Message], None],
         Optional[Callable[[], None]],
         Optional[Callable[[], None]],
+        Optional[Callable[[int], Tuple[str, str]]],
     ]
 ]:
     """Primitives for request/response-based interaction with a server.
 
     One notable difference to the grpc_connection context manager is that
     `receive` can return `None`.
 
@@ -118,15 +121,15 @@
     stub = FleetStub(channel)
     metadata: Optional[Metadata] = None
     node: Optional[Node] = None
     ping_thread: Optional[threading.Thread] = None
     ping_stop_event = threading.Event()
 
     ###########################################################################
-    # ping/create_node/delete_node/receive/send functions
+    # ping/create_node/delete_node/receive/send/get_run functions
     ###########################################################################
 
     def ping() -> None:
         # Get Node
         if node is None:
             log(ERROR, "Node instance missing")
             return
@@ -237,12 +240,23 @@
         # Serialize ProtoBuf to bytes
         request = PushTaskResRequest(task_res_list=[task_res])
         _ = retry_invoker.invoke(stub.PushTaskRes, request)
 
         # Cleanup
         metadata = None
 
+    def get_run(run_id: int) -> Tuple[str, str]:
+        # Call FleetAPI
+        get_run_request = GetRunRequest(run_id=run_id)
+        get_run_response: GetRunResponse = retry_invoker.invoke(
+            stub.GetRun,
+            request=get_run_request,
+        )
+
+        # Return fab_id and fab_version
+        return get_run_response.run.fab_id, get_run_response.run.fab_version
+
     try:
         # Yield methods
-        yield (receive, send, create_node, delete_node)
+        yield (receive, send, create_node, delete_node, get_run)
     except Exception as exc:  # pylint: disable=broad-except
         log(ERROR, exc)
```

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/heartbeat.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/heartbeat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/centraldp_mods.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/mod/centraldp_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/comms_mods.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/mod/comms_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/localdp_mod.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/mod/localdp_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/mod/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/mod/utils.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/mod/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/node_state.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/node_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/node_state_tests.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/node_state_tests.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/client/typing.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/client/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/address.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/constant.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/context.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/date.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/differential_privacy.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/differential_privacy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/differential_privacy_constants.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/differential_privacy_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/dp.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/exit_handlers.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/exit_handlers.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/grpc.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/logger.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/message.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/message.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/object_ref.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/object_ref.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/parameter.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/pyproject.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/pyproject.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/record/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/configsrecord.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/record/configsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/conversion_utils.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/record/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/metricsrecord.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/record/metricsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/parametersrecord.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/record/parametersrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/recordset.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/record/recordset.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/record/typeddict.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/record/typeddict.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/recordset_compat.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/recordset_compat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/retry_invoker.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/retry_invoker.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/crypto/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/secure_aggregation/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/crypto/shamir.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/secure_aggregation/crypto/shamir.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/quantization.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/secure_aggregation/quantization.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/secaggplus_constants.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/secure_aggregation/secaggplus_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/secure_aggregation/secaggplus_utils.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/secure_aggregation/secaggplus_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/serde.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,14 +156,18 @@
     RUN_CLIENT_APP_ENTER = auto()
     RUN_CLIENT_APP_LEAVE = auto()
 
     # flower-server-app
     RUN_SERVER_APP_ENTER = auto()
     RUN_SERVER_APP_LEAVE = auto()
 
+    # SuperNode
+    RUN_SUPERNODE_ENTER = auto()
+    RUN_SUPERNODE_LEAVE = auto()
+
 
 # Use the ThreadPoolExecutor with max_workers=1 to have a queue
 # and also ensure that telemetry calls are not blocking.
 state: Dict[str, Union[Optional[str], Optional[ThreadPoolExecutor]]] = {
     # Will be assigned ThreadPoolExecutor(max_workers=1)
     # in event() the first time it's required
     "executor": None,
```

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/typing.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/common/version.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/error_pb2.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/error_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/error_pb2.pyi` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/recordset_pb2.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/recordset_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/recordset_pb2.pyi` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/recordset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/app.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,17 +287,19 @@
         grpc_servers[0].wait_for_termination()
     elif len(bckg_threads) > 0:
         bckg_threads[0].join()
 
 
 # pylint: disable=too-many-branches, too-many-locals, too-many-statements
 def run_superlink() -> None:
-    """Run Flower server (Driver API and Fleet API)."""
-    log(INFO, "Starting Flower server")
+    """Run Flower SuperLink (Driver API and Fleet API)."""
+    log(INFO, "Starting Flower SuperLink")
+
     event(EventType.RUN_SUPERLINK_ENTER)
+
     args = _parse_args_run_superlink().parse_args()
 
     # Parse IP address
     parsed_address = parse_address(args.driver_api_address)
     if not parsed_address:
         sys.exit(f"Driver IP address ({args.driver_api_address}) cannot be parsed.")
     host, port, is_v6 = parsed_address
@@ -564,17 +566,15 @@
 
     return parser
 
 
 def _parse_args_run_superlink() -> argparse.ArgumentParser:
     """Parse command line arguments for both Driver API and Fleet API."""
     parser = argparse.ArgumentParser(
-        description="This will start a Flower server "
-        "(meaning, a Driver API and a Fleet API), "
-        "that clients will be able to connect to.",
+        description="Start a Flower SuperLink",
     )
 
     _add_args_common(parser=parser)
     _add_args_driver_api(parser=parser)
     _add_args_fleet_api(parser=parser)
 
     return parser
```

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/app.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/compat/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/app_utils.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/compat/app_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/driver_client_proxy.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/compat/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/compat/legacy_context.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/compat/legacy_context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/criterion.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/driver/abc_driver.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/driver/abc_driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/driver/driver.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/driver/grpc_driver.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/driver/grpc_driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/history.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/run_serverapp.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/run_serverapp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/server.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/server_app.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/server_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/server_config.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/server_config.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/bulyan.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/bulyan.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/dp_adaptive_clipping.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/dp_adaptive_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/dp_fixed_clipping.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/dp_fixed_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedxgb_bagging.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedxgb_bagging.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedxgb_cyclic.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedxgb_cyclic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/driver/driver_grpc.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/driver/driver_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/driver/driver_servicer.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     PingRequest,
     PingResponse,
     PullTaskInsRequest,
     PullTaskInsResponse,
     PushTaskResRequest,
     PushTaskResResponse,
     Reconnect,
+    Run,
 )
 from flwr.proto.node_pb2 import Node  # pylint: disable=E0611
 from flwr.proto.task_pb2 import TaskIns, TaskRes  # pylint: disable=E0611
 from flwr.server.superlink.state import State
 
 
 def create_node(
@@ -105,8 +106,10 @@
     return response
 
 
 def get_run(
     request: GetRunRequest, state: State  # pylint: disable=W0613
 ) -> GetRunResponse:
     """Get run information."""
-    return GetRunResponse()
+    run_id, fab_id, fab_version = state.get_run(request.run_id)
+    run = Run(run_id=run_id, fab_id=fab_id, fab_version=fab_version)
+    return GetRunResponse(run=run)
```

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/vce/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/backend/backend.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/vce/backend/backend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/fleet/vce/vce_api.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/fleet/vce/vce_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/in_memory_state.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/sqlite_state.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/state.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/state_factory.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/superlink/state/utils.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/superlink/state/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/typing.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/constant.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/workflow/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/default_workflows.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/workflow/default_workflows.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/workflow/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/app.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/ray_transport/ray_actor.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/simulation/ray_transport/ray_actor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/ray_transport/utils.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/simulation/ray_transport/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/src/py/flwr/simulation/run_simulation.py` & `flwr_nightly-1.9.0.dev20240419/src/py/flwr/simulation/run_simulation.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240418/PKG-INFO` & `flwr_nightly-1.9.0.dev20240419/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.9.0.dev20240418
+Version: 1.9.0.dev20240419
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.ai
 License: Apache-2.0
 Keywords: flower,fl,federated learning,federated analytics,federated evaluation,machine learning
 Author: The Flower Authors
 Author-email: hello@flower.ai
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240418 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240419 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.ai
 License: Apache-2.0 Keywords: flower,fl,federated learning,federated
 analytics,federated evaluation,machine learning Author: The Flower Authors
 Author-email: hello@flower.ai Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
```

