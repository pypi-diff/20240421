# Comparing `tmp/syft-0.8.7b1.tar.gz` & `tmp/syft-0.8.7b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.7b1.tar", last modified: Sun Apr  7 12:41:40 2024, max compression
+gzip compressed data, was "syft-0.8.7b2.tar", last modified: Sun Apr 21 12:50:56 2024, max compression
```

## Comparing `syft-0.8.7b1.tar` & `syft-0.8.7b2.tar`

### file list

```diff
@@ -1,305 +1,307 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.201675 syft-0.8.7b1/
--rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-04-07 12:37:49.000000 syft-0.8.7b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-07 12:37:49.000000 syft-0.8.7b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-04-07 12:41:40.201675 syft-0.8.7b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18678 2024-04-07 12:39:28.000000 syft-0.8.7b1/PYPI.md
--rw-r--r--   0 runner    (1001) docker     (127)    17508 2024-04-07 12:37:49.000000 syft-0.8.7b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-07 12:37:49.000000 syft-0.8.7b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-07 12:41:40.201675 syft-0.8.7b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-07 12:37:49.000000 syft-0.8.7b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.141673 syft-0.8.7b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.149673 syft-0.8.7b1/src/syft/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-07 12:38:47.000000 syft-0.8.7b1/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-07 12:38:47.000000 syft-0.8.7b1/src/syft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/abstract_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.149673 syft-0.8.7b1/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.153673 syft-0.8.7b1/src/syft/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41720 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46245 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18511 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/domain_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7793 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/enclave_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/gateway_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    16212 2024-04-07 12:40:41.000000 syft-0.8.7b1/src/syft/client/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/search.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/sync_decision.py
--rw-r--r--   0 runner    (1001) docker     (127)    12864 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/syncing.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/client/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.153673 syft-0.8.7b1/src/syft/custom_worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/custom_worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/custom_worker/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/custom_worker/builder_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/custom_worker/builder_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/custom_worker/builder_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/custom_worker/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/custom_worker/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/custom_worker/runner_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/custom_worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.153673 syft-0.8.7b1/src/syft/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/exceptions/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/exceptions/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/gevent_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.153673 syft-0.8.7b1/src/syft/img/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/img/base64.py
--rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    41764 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/img/small-grid-symbol-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.157673 syft-0.8.7b1/src/syft/node/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/enclave.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    59372 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/node/worker_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.157673 syft-0.8.7b1/src/syft/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)    24381 2024-04-07 12:40:41.000000 syft-0.8.7b1/src/syft/protocol/data_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/protocol/protocol_version.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.157673 syft-0.8.7b1/src/syft/protocol/releases/
--rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/protocol/releases/0.8.2.json
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/protocol/releases/0.8.3.json
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/protocol/releases/0.8.4.json
--rw-r--r--   0 runner    (1001) docker     (127)    50490 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/protocol/releases/0.8.6.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.161673 syft-0.8.7b1/src/syft/serde/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/capnp.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/lib_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/recursive.py
--rw-r--r--   0 runner    (1001) docker     (127)    11583 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/serializable.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/serde/third_party.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.161673 syft-0.8.7b1/src/syft/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.165674 syft-0.8.7b1/src/syft/service/action/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/action_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/action_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    72779 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/action_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    39060 2024-04-07 12:40:41.000000 syft-0.8.7b1/src/syft/service/action/action_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    14084 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/action_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/action_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/action/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.165674 syft-0.8.7b1/src/syft/service/api/
--rw-r--r--   0 runner    (1001) docker     (127)    19755 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/api/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12425 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/api/api_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/api/api_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.165674 syft-0.8.7b1/src/syft/service/blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/blob_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/blob_storage/remote_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12511 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/blob_storage/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/blob_storage/stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.165674 syft-0.8.7b1/src/syft/service/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code/status_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code/unparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    55843 2024-04-07 12:40:41.000000 syft-0.8.7b1/src/syft/service/code/user_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    25074 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.169674 syft-0.8.7b1/src/syft/service/code_history/
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code_history/code_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code_history/code_history_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/code_history/code_history_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.169674 syft-0.8.7b1/src/syft/service/data_subject/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.169674 syft-0.8.7b1/src/syft/service/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28880 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.169674 syft-0.8.7b1/src/syft/service/enclave/
--rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/enclave/enclave_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.169674 syft-0.8.7b1/src/syft/service/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/job/job_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    24816 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/job/job_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.169674 syft-0.8.7b1/src/syft/service/log/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/log/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/log/log_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/log/log_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.173674 syft-0.8.7b1/src/syft/service/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/metadata/metadata_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/metadata/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.173674 syft-0.8.7b1/src/syft/service/network/
--rw-r--r--   0 runner    (1001) docker     (127)    18970 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/network/network_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/network/node_peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/network/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.173674 syft-0.8.7b1/src/syft/service/notification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14281 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notification/email_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     9667 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notification/notification_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notification/notification_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notification/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.173674 syft-0.8.7b1/src/syft/service/notifier/
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notifier/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notifier/notifier_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notifier/notifier_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notifier/notifier_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/notifier/smtp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.173674 syft-0.8.7b1/src/syft/service/object_search/
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/object_search/migration_state_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/object_search/object_migration_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.173674 syft-0.8.7b1/src/syft/service/output/
--rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/output/output_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.177674 syft-0.8.7b1/src/syft/service/policy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27118 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/policy/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/policy/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.177674 syft-0.8.7b1/src/syft/service/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49644 2024-04-07 12:40:41.000000 syft-0.8.7b1/src/syft/service/project/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    15401 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/project/project_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.177674 syft-0.8.7b1/src/syft/service/queue/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/queue/base_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/queue/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/queue/queue_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    33929 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.177674 syft-0.8.7b1/src/syft/service/request/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49704 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/request/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11273 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/request/request_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/request/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17295 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.181674 syft-0.8.7b1/src/syft/service/settings/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/settings/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/settings/settings_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/settings/settings_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.181674 syft-0.8.7b1/src/syft/service/sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    48845 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/sync/diff_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    21598 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/sync/resolve_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)    13157 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/sync/sync_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/sync/sync_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/sync/sync_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.181674 syft-0.8.7b1/src/syft/service/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/user/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/user/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/user/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    20579 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/user/user_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/user/user_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.185674 syft-0.8.7b1/src/syft/service/veilid/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/veilid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/veilid/veilid_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/veilid/veilid_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.185674 syft-0.8.7b1/src/syft/service/worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/image_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/image_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/image_registry_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/image_registry_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    22317 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/worker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/worker_image_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/worker_image_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/worker_pool_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/worker_pool_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/worker_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/service/worker/worker_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/stable_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.189674 syft-0.8.7b1/src/syft/store/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.189674 syft-0.8.7b1/src/syft/store/blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/blob_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/blob_storage/on_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/blob_storage/seaweedfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    26359 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    25265 2024-04-07 12:40:41.000000 syft-0.8.7b1/src/syft/store/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/locks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)    35722 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/store/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-04-07 12:40:41.000000 syft-0.8.7b1/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.193674 syft-0.8.7b1/src/syft/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/cache_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/dicttuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/syft_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/syft_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)    36866 2024-04-07 12:40:41.000000 syft-0.8.7b1/src/syft/types/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/syncable_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/types/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.197674 syft-0.8.7b1/src/syft/util/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/_std_stream_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/experimental_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/fonts.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.197674 syft-0.8.7b1/src/syft/util/notebook_ui/
--rw-r--r--   0 runner    (1001) docker     (127)    32438 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/notebook_ui/notebook_addons.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-07 12:37:49.000000 syft-0.8.7b1/src/syft/util/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:41:40.197674 syft-0.8.7b1/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-04-07 12:41:40.000000 syft-0.8.7b1/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-07 12:41:40.000000 syft-0.8.7b1/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:41:40.000000 syft-0.8.7b1/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-07 12:41:40.000000 syft-0.8.7b1/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:38:48.000000 syft-0.8.7b1/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-07 12:41:40.000000 syft-0.8.7b1/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 12:41:40.000000 syft-0.8.7b1/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.808075 syft-0.8.7b2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-04-21 12:47:35.000000 syft-0.8.7b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-21 12:47:35.000000 syft-0.8.7b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-04-21 12:50:56.808075 syft-0.8.7b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18678 2024-04-21 12:48:43.000000 syft-0.8.7b2/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17508 2024-04-21 12:47:35.000000 syft-0.8.7b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-21 12:47:35.000000 syft-0.8.7b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-04-21 12:50:56.808075 syft-0.8.7b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-21 12:47:35.000000 syft-0.8.7b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.748079 syft-0.8.7b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.752079 syft-0.8.7b2/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-21 12:48:08.000000 syft-0.8.7b2/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     6371 2024-04-21 12:48:08.000000 syft-0.8.7b2/src/syft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/abstract_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.756079 syft-0.8.7b2/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.760079 syft-0.8.7b2/src/syft/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41860 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37060 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18538 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/domain_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7814 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/enclave_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/gateway_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16329 2024-04-21 12:49:56.000000 syft-0.8.7b2/src/syft/client/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/sync_decision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12864 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/syncing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/client/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.760079 syft-0.8.7b2/src/syft/custom_worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/custom_worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/custom_worker/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/custom_worker/builder_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/custom_worker/builder_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/custom_worker/builder_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/custom_worker/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/custom_worker/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/custom_worker/runner_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/custom_worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.760079 syft-0.8.7b2/src/syft/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/exceptions/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/exceptions/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/gevent_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.760079 syft-0.8.7b2/src/syft/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/img/base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41764 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/img/small-grid-symbol-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.764078 syft-0.8.7b2/src/syft/node/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/enclave.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59989 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/node/worker_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.764078 syft-0.8.7b2/src/syft/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)    24381 2024-04-21 12:49:56.000000 syft-0.8.7b2/src/syft/protocol/data_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/protocol/protocol_version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.764078 syft-0.8.7b2/src/syft/protocol/releases/
+-rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/protocol/releases/0.8.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/protocol/releases/0.8.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/protocol/releases/0.8.4.json
+-rw-r--r--   0 runner    (1001) docker     (127)    50490 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/protocol/releases/0.8.6.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.768078 syft-0.8.7b2/src/syft/serde/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12236 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12186 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/third_party.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/serde/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.768078 syft-0.8.7b2/src/syft/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.772078 syft-0.8.7b2/src/syft/service/action/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/action_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/action_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74031 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3164 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38799 2024-04-21 12:49:57.000000 syft-0.8.7b2/src/syft/service/action/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/action/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.772078 syft-0.8.7b2/src/syft/service/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    20448 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13237 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/api/api_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/api/api_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.772078 syft-0.8.7b2/src/syft/service/blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/blob_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/blob_storage/remote_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12511 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/blob_storage/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/blob_storage/stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.776077 syft-0.8.7b2/src/syft/service/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code/status_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55843 2024-04-21 12:49:57.000000 syft-0.8.7b2/src/syft/service/code/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25113 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.776077 syft-0.8.7b2/src/syft/service/code_history/
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code_history/code_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8832 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code_history/code_history_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/code_history/code_history_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.776077 syft-0.8.7b2/src/syft/service/data_subject/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.776077 syft-0.8.7b2/src/syft/service/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28880 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.776077 syft-0.8.7b2/src/syft/service/enclave/
+-rw-r--r--   0 runner    (1001) docker     (127)     5324 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/enclave/enclave_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.776077 syft-0.8.7b2/src/syft/service/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9408 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/job/job_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24949 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/job/job_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.780077 syft-0.8.7b2/src/syft/service/log/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/log/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4876 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/log/log_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/log/log_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.780077 syft-0.8.7b2/src/syft/service/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/metadata/metadata_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/metadata/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.780077 syft-0.8.7b2/src/syft/service/network/
+-rw-r--r--   0 runner    (1001) docker     (127)    30351 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/network/network_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10813 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/network/node_peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/network/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.780077 syft-0.8.7b2/src/syft/service/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14281 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notification/email_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notification/notification_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notification/notification_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notification/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.780077 syft-0.8.7b2/src/syft/service/notifier/
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notifier/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notifier/notifier_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notifier/notifier_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notifier/notifier_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/notifier/smtp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.784077 syft-0.8.7b2/src/syft/service/object_search/
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/object_search/migration_state_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/object_search/object_migration_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.784077 syft-0.8.7b2/src/syft/service/output/
+-rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/output/output_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.784077 syft-0.8.7b2/src/syft/service/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27131 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/policy/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.784077 syft-0.8.7b2/src/syft/service/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49644 2024-04-21 12:49:56.000000 syft-0.8.7b2/src/syft/service/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15758 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/project/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.784077 syft-0.8.7b2/src/syft/service/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/queue/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/queue/queue_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33929 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.784077 syft-0.8.7b2/src/syft/service/request/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49867 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/request/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11273 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/request/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/request/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16874 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.788076 syft-0.8.7b2/src/syft/service/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/settings/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.788076 syft-0.8.7b2/src/syft/service/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50919 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/sync/diff_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22083 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/sync/resolve_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/sync/sync_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/sync/sync_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/sync/sync_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.788076 syft-0.8.7b2/src/syft/service/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/user/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/user/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20579 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/user/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/user/user_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.792076 syft-0.8.7b2/src/syft/service/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/image_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/image_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/image_registry_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/image_registry_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22317 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/worker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10135 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/worker_image_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/worker_image_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9698 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25273 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/worker_pool_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/worker_pool_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/worker_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/service/worker/worker_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/stable_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.792076 syft-0.8.7b2/src/syft/store/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.796076 syft-0.8.7b2/src/syft/store/blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/blob_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/blob_storage/on_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10835 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/blob_storage/seaweedfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26587 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-04-21 12:49:56.000000 syft-0.8.7b2/src/syft/store/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37008 2024-04-21 12:49:57.000000 syft-0.8.7b2/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-04-21 12:49:56.000000 syft-0.8.7b2/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.796076 syft-0.8.7b2/src/syft/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11929 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/cache_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/dicttuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/syft_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36866 2024-04-21 12:49:56.000000 syft-0.8.7b2/src/syft/types/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/syncable_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/types/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.800076 syft-0.8.7b2/src/syft/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/_std_stream_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/experimental_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/jax_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.800076 syft-0.8.7b2/src/syft/util/notebook_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/notebook_ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.800076 syft-0.8.7b2/src/syft/util/notebook_ui/components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/notebook_ui/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/notebook_ui/components/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7837 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/notebook_ui/components/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33088 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/notebook_ui/notebook_addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-21 12:47:35.000000 syft-0.8.7b2/src/syft/util/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:50:56.800076 syft-0.8.7b2/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-04-21 12:50:56.000000 syft-0.8.7b2/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-04-21 12:50:56.000000 syft-0.8.7b2/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 12:50:56.000000 syft-0.8.7b2/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-21 12:50:56.000000 syft-0.8.7b2/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 12:48:09.000000 syft-0.8.7b2/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-21 12:50:56.000000 syft-0.8.7b2/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-21 12:50:56.000000 syft-0.8.7b2/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.7b1/LICENSE` & `syft-0.8.7b2/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/PKG-INFO` & `syft-0.8.7b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.7b1
+Version: 0.8.7b2
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
@@ -50,15 +50,15 @@
 Requires-Dist: pandas==2.2.1
 Requires-Dist: docker==6.1.3
 Requires-Dist: kr8s==0.13.5
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: azure-storage-blob==12.19.1
 Requires-Dist: ipywidgets==8.1.2
 Provides-Extra: data-science
-Requires-Dist: transformers==4.38.2; extra == "data-science"
+Requires-Dist: transformers==4.39.3; extra == "data-science"
 Requires-Dist: opendp==0.9.2; extra == "data-science"
 Requires-Dist: evaluate==0.4.1; extra == "data-science"
 Requires-Dist: recordlinkage==0.16; extra == "data-science"
 Requires-Dist: dm-haiku==0.0.10; extra == "data-science"
 Requires-Dist: torch[cpu]==2.2.1; extra == "data-science"
 Provides-Extra: dev
 Requires-Dist: pytest<8; extra == "dev"
```

### Comparing `syft-0.8.7b1/PYPI.md` & `syft-0.8.7b2/PYPI.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/README.md` & `syft-0.8.7b2/README.md`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/setup.cfg` & `syft-0.8.7b2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.7-beta.1"
+version = attr: "0.8.7-beta.2"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: PYPI.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
@@ -69,15 +69,15 @@
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
 data_science = 
-	transformers==4.38.2
+	transformers==4.39.3
 	opendp==0.9.2
 	evaluate==0.4.1
 	recordlinkage==0.16
 	dm-haiku==0.0.10
 	torch[cpu]==2.2.1
 dev = 
 	%(test_plugins)s
```

### Comparing `syft-0.8.7b1/src/syft/VERSION` & `syft-0.8.7b2/src/syft/VERSION`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.7-beta.1"
+__version__ = "0.8.7-beta.2"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.7b1/src/syft/__init__.py` & `syft-0.8.7b2/src/syft/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.7-beta.1"
+__version__ = "0.8.7-beta.2"
 
 # stdlib
 from collections.abc import Callable
 import pathlib
 from pathlib import Path
 import sys
 from typing import Any
```

### Comparing `syft-0.8.7b1/src/syft/abstract_node.py` & `syft-0.8.7b2/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/client/api.py` & `syft-0.8.7b2/src/syft/client/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,27 +308,27 @@
     def private(self, *args: Any, **kwargs: Any) -> Any:
         if self.custom_function:
             return self.__function_call("api.call_private", *args, **kwargs)
         return SyftError(
             message="This function doesn't support public/private calls as it's not custom."
         )
 
-    def custom_function_id(self) -> UID | SyftError:
+    def custom_function_actionobject_id(self) -> UID | SyftError:
         if self.custom_function and self.pre_kwargs is not None:
             custom_path = self.pre_kwargs.get("path", "")
             api_call = SyftAPICall(
                 node_uid=self.node_uid,
                 path="api.view",
                 args=[custom_path],
                 kwargs={},
             )
             endpoint = self.make_call(api_call=api_call)
             if isinstance(endpoint, SyftError):
                 return endpoint
-            return endpoint.id
+            return endpoint.action_object_id
         return SyftError(message="This function is not a custom function")
 
     def _repr_markdown_(self, wrap_as_python: bool = False, indent: int = 0) -> str:
         if self.custom_function and self.pre_kwargs is not None:
             custom_path = self.pre_kwargs.get("path", "")
             api_call = SyftAPICall(
                 node_uid=self.node_uid,
@@ -385,15 +385,15 @@
         # We can recover the function/method pointer by its UID in server side.
         for i in range(len(args)):
             if isinstance(args[i], RemoteFunction) and args[i].custom_function:
                 args[i] = args[i].custom_function_id()
 
         for k, v in kwargs.items():
             if isinstance(v, RemoteFunction) and v.custom_function:
-                kwargs[k] = v.custom_function_id()
+                kwargs[k] = v.custom_function_actionobject_id()
 
         args, kwargs = convert_to_pointers(
             api=self.api,
             node_uid=self.node_uid,
             args=args,
             kwargs=kwargs,
         )
@@ -569,15 +569,16 @@
 
     def __getattribute__(self, name: str) -> Any:
         try:
             return object.__getattribute__(self, name)
         except AttributeError:
             raise SyftAttributeError(
                 f"'APIModule' api{self.path} object has no submodule or method '{name}', "
-                "you may not have permission to access the module you are trying to access"
+                "you may not have permission to access the module you are trying to access."
+                "If you think this is an error, try calling `client.refresh()` to update the API."
             )
 
     def __getitem__(self, key: str | int) -> Any:
         if hasattr(self, "get_all"):
             return self.get_all()[key]
         raise NotImplementedError
```

### Comparing `syft-0.8.7b1/src/syft/client/client.py` & `syft-0.8.7b2/src/syft/client/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # future
 from __future__ import annotations
 
 # stdlib
-import base64
 from collections.abc import Callable
 from copy import deepcopy
 from enum import Enum
 from getpass import getpass
 import json
 import os
 from typing import Any
 from typing import TYPE_CHECKING
 from typing import cast
 
 # third party
 from argon2 import PasswordHasher
-from pydantic import Field
 from pydantic import field_validator
 import requests
 from requests import Response
 from requests import Session
 from requests.adapters import HTTPAdapter
 from requests.packages.urllib3.util.retry import Retry  # type: ignore[import-untyped]
 from typing_extensions import Self
@@ -44,19 +42,15 @@
 from ..service.response import SyftError
 from ..service.response import SyftSuccess
 from ..service.user.user import UserCreate
 from ..service.user.user import UserPrivateKey
 from ..service.user.user import UserView
 from ..service.user.user_roles import ServiceRole
 from ..service.user.user_service import UserService
-from ..service.veilid.veilid_endpoints import VEILID_PROXY_PATH
-from ..service.veilid.veilid_endpoints import VEILID_SERVICE_URL
-from ..service.veilid.veilid_endpoints import VEILID_SYFT_PROXY_URL
 from ..types.grid_url import GridURL
-from ..types.syft_object import SYFT_OBJECT_VERSION_1
 from ..types.syft_object import SYFT_OBJECT_VERSION_2
 from ..types.uid import UID
 from ..util.logger import debug
 from ..util.telemetry import instrument
 from ..util.util import prompt_warning_message
 from ..util.util import thread_ident
 from ..util.util import verify_tls
@@ -69,14 +63,15 @@
 from .connection import NodeConnection
 from .protocol import SyftProtocol
 
 if TYPE_CHECKING:
     # relative
     from ..service.network.node_peer import NodePeer
 
+
 # use to enable mitm proxy
 # from syft.grid.connections.http_connection import HTTPConnection
 # HTTPConnection.proxies = {"http": "http://127.0.0.1:8080"}
 
 
 def upgrade_tls(url: GridURL, response: Response) -> GridURL:
     try:
@@ -108,15 +103,15 @@
         blocking=True,
     )
 
     if credentials is None:
         # generate a random signing key
         credentials = SyftSigningKey.generate()
 
-    signed_message = call.sign(credentials=credentials)
+    signed_message: SignedSyftAPICall = call.sign(credentials=credentials)
     signed_result = make_call(signed_message)
     response = debox_signed_syftapicall_response(signed_result)
     return response
 
 
 API_PATH = "/api/v2"
 DEFAULT_PYGRID_PORT = 80
@@ -207,15 +202,17 @@
             )
 
         # upgrade to tls if available
         self.url = upgrade_tls(self.url, response)
 
         return response.content
 
-    def get_node_metadata(self, credentials: SyftSigningKey) -> NodeMetadataJSON:
+    def get_node_metadata(
+        self, credentials: SyftSigningKey
+    ) -> NodeMetadataJSON | SyftError:
         if self.proxy_target_uid:
             response = forward_message_to_proxy(
                 make_call=self.make_call,
                 proxy_target_uid=self.proxy_target_uid,
                 path="metadata",
                 credentials=credentials,
             )
@@ -306,227 +303,15 @@
 
     def __str__(self) -> str:
         return f"{type(self).__name__}: {self.url}"
 
     def __hash__(self) -> int:
         return hash(self.proxy_target_uid) + hash(self.url)
 
-    def get_client_type(self) -> type[SyftClient]:
-        # TODO: Rasswanth, should remove passing in credentials
-        # when metadata are proxy forwarded in the grid routes
-        # in the gateway fixes PR
-        # relative
-        from .domain_client import DomainClient
-        from .enclave_client import EnclaveClient
-        from .gateway_client import GatewayClient
-
-        metadata = self.get_node_metadata(credentials=SyftSigningKey.generate())
-        if metadata.node_type == NodeType.DOMAIN.value:
-            return DomainClient
-        elif metadata.node_type == NodeType.GATEWAY.value:
-            return GatewayClient
-        elif metadata.node_type == NodeType.ENCLAVE.value:
-            return EnclaveClient
-        else:
-            return SyftError(message=f"Unknown node type {metadata.node_type}")
-
-
-@serializable(
-    attrs=["proxy_target_uid", "vld_key", "vld_forward_proxy", "vld_reverse_proxy"]
-)
-class VeilidConnection(NodeConnection):
-    __canonical_name__ = "VeilidConnection"
-    __version__ = SYFT_OBJECT_VERSION_1
-
-    vld_forward_proxy: GridURL = Field(default=GridURL.from_url(VEILID_SERVICE_URL))
-    vld_reverse_proxy: GridURL = Field(default=GridURL.from_url(VEILID_SYFT_PROXY_URL))
-    vld_key: str
-    proxy_target_uid: UID | None = None
-    routes: type[Routes] = Field(default=Routes)
-    session_cache: Session | None = None
-
-    @field_validator("vld_forward_proxy", mode="before")
-    def make_forward_proxy_url(cls, v: GridURL | str) -> GridURL:
-        if isinstance(v, str):
-            return GridURL.from_url(v)
-        else:
-            return v
-
-    # TODO: Remove this once when we remove reverse proxy in Veilid Connection
-    @field_validator("vld_reverse_proxy", mode="before")
-    def make_reverse_proxy_url(cls, v: GridURL | str) -> GridURL:
-        if isinstance(v, str):
-            return GridURL.from_url(v)
-        else:
-            return v
-
-    def with_proxy(self, proxy_target_uid: UID) -> Self:
-        raise NotImplementedError("VeilidConnection does not support with_proxy")
-
-    def get_cache_key(self) -> str:
-        return str(self.vld_key)
-
-    # def to_blob_route(self, path: str, **kwargs) -> GridURL:
-    #     _path = self.routes.ROUTE_BLOB_STORE.value + path
-    #     return self.url.with_path(_path)
-
-    @property
-    def session(self) -> Session:
-        if self.session_cache is None:
-            session = requests.Session()
-            retry = Retry(total=3, backoff_factor=0.5)
-            adapter = HTTPAdapter(max_retries=retry)
-            session.mount("http://", adapter)
-            session.mount("https://", adapter)
-            self.session_cache = session
-        return self.session_cache
-
-    def _make_get(self, path: str, params: dict | None = None) -> bytes:
-        rev_proxy_url = self.vld_reverse_proxy.with_path(path)
-        forward_proxy_url = self.vld_forward_proxy.with_path(VEILID_PROXY_PATH)
-
-        json_data = {
-            "url": str(rev_proxy_url),
-            "method": "GET",
-            "vld_key": self.vld_key,
-            "params": params,
-        }
-        response = self.session.get(str(forward_proxy_url), json=json_data)
-        if response.status_code != 200:
-            raise requests.ConnectionError(
-                f"Failed to fetch {forward_proxy_url}. Response returned with code {response.status_code}"
-            )
-
-        return response.content
-
-    def _make_post(
-        self,
-        path: str,
-        json: dict[str, Any] | None = None,
-        data: bytes | None = None,
-    ) -> bytes:
-        rev_proxy_url = self.vld_reverse_proxy.with_path(path)
-        forward_proxy_url = self.vld_forward_proxy.with_path(VEILID_PROXY_PATH)
-
-        # Since JSON expects strings, we need to encode the bytes to base64
-        # as some bytes may not be valid utf-8
-        # TODO: Can we optimize this?
-        data_base64 = base64.b64encode(data).decode() if data else None
-
-        json_data = {
-            "url": str(rev_proxy_url),
-            "method": "POST",
-            "vld_key": self.vld_key,
-            "json": json,
-            "data": data_base64,
-        }
-
-        response = self.session.post(str(forward_proxy_url), json=json_data)
-        if response.status_code != 200:
-            raise requests.ConnectionError(
-                f"Failed to fetch {forward_proxy_url}. Response returned with code {response.status_code}"
-            )
-
-        return response.content
-
-    def get_node_metadata(self, credentials: SyftSigningKey) -> NodeMetadataJSON:
-        # TODO: Implement message proxy forwarding for gateway
-
-        response = self._make_get(self.routes.ROUTE_METADATA.value)
-        metadata_json = json.loads(response)
-        return NodeMetadataJSON(**metadata_json)
-
-    def get_api(
-        self, credentials: SyftSigningKey, communication_protocol: int
-    ) -> SyftAPI:
-        # TODO: Implement message proxy forwarding for gateway
-
-        params = {
-            "verify_key": str(credentials.verify_key),
-            "communication_protocol": communication_protocol,
-        }
-        content = self._make_get(self.routes.ROUTE_API.value, params=params)
-        obj = _deserialize(content, from_bytes=True)
-        obj.connection = self
-        obj.signing_key = credentials
-        obj.communication_protocol = communication_protocol
-        if self.proxy_target_uid:
-            obj.node_uid = self.proxy_target_uid
-        return cast(SyftAPI, obj)
-
-    def login(
-        self,
-        email: str,
-        password: str,
-    ) -> SyftSigningKey | None:
-        # TODO: Implement message proxy forwarding for gateway
-
-        credentials = {"email": email, "password": password}
-        response = self._make_post(self.routes.ROUTE_LOGIN.value, credentials)
-        obj = _deserialize(response, from_bytes=True)
-
-        return obj
-
-    def register(self, new_user: UserCreate) -> Any:
-        # TODO: Implement message proxy forwarding for gateway
-
-        data = _serialize(new_user, to_bytes=True)
-        response = self._make_post(self.routes.ROUTE_REGISTER.value, data=data)
-        response = _deserialize(response, from_bytes=True)
-        return response
-
-    def make_call(self, signed_call: SignedSyftAPICall) -> Any:
-        msg_bytes: bytes = _serialize(obj=signed_call, to_bytes=True)
-        # Since JSON expects strings, we need to encode the bytes to base64
-        # as some bytes may not be valid utf-8
-        # TODO: Can we optimize this?
-        msg_base64 = base64.b64encode(msg_bytes).decode()
-
-        rev_proxy_url = self.vld_reverse_proxy.with_path(
-            self.routes.ROUTE_API_CALL.value
-        )
-        forward_proxy_url = self.vld_forward_proxy.with_path(VEILID_PROXY_PATH)
-        json_data = {
-            "url": str(rev_proxy_url),
-            "method": "POST",
-            "vld_key": self.vld_key,
-            "data": msg_base64,
-        }
-        response = requests.post(  # nosec
-            url=str(forward_proxy_url),
-            json=json_data,
-        )
-
-        if response.status_code != 200:
-            raise requests.ConnectionError(
-                f"Failed to fetch metadata. Response returned with code {response.status_code}"
-            )
-
-        result = _deserialize(response.content, from_bytes=True)
-        return result
-
-    def __repr__(self) -> str:
-        return self.__str__()
-
-    def __str__(self) -> str:
-        res = f"{type(self).__name__}:"
-        res += f"\n DHT Key: {self.vld_key}"
-        res += f"\n Forward Proxy: {self.vld_forward_proxy}"
-        res += f"\n Reverse Proxy: {self.vld_reverse_proxy}"
-        return res
-
-    def __hash__(self) -> int:
-        return (
-            hash(self.proxy_target_uid)
-            + hash(self.vld_key)
-            + hash(self.vld_forward_proxy)
-            + hash(self.vld_reverse_proxy)
-        )
-
-    def get_client_type(self) -> type[SyftClient]:
+    def get_client_type(self) -> type[SyftClient] | SyftError:
         # TODO: Rasswanth, should remove passing in credentials
         # when metadata are proxy forwarded in the grid routes
         # in the gateway fixes PR
         # relative
         from .domain_client import DomainClient
         from .enclave_client import EnclaveClient
         from .gateway_client import GatewayClient
@@ -549,15 +334,17 @@
 
     node: AbstractNode
     proxy_target_uid: UID | None = None
 
     def with_proxy(self, proxy_target_uid: UID) -> Self:
         return PythonConnection(node=self.node, proxy_target_uid=proxy_target_uid)
 
-    def get_node_metadata(self, credentials: SyftSigningKey) -> NodeMetadataJSON:
+    def get_node_metadata(
+        self, credentials: SyftSigningKey
+    ) -> NodeMetadataJSON | SyftError:
         if self.proxy_target_uid:
             response = forward_message_to_proxy(
                 make_call=self.make_call,
                 proxy_target_uid=self.proxy_target_uid,
                 path="metadata",
                 credentials=credentials,
             )
@@ -648,15 +435,15 @@
 
     def __repr__(self) -> str:
         return f"{type(self).__name__}"
 
     def __str__(self) -> str:
         return f"{type(self).__name__}"
 
-    def get_client_type(self) -> type[SyftClient]:
+    def get_client_type(self) -> type[SyftClient] | SyftError:
         # relative
         from .domain_client import DomainClient
         from .enclave_client import EnclaveClient
         from .gateway_client import GatewayClient
 
         metadata = self.get_node_metadata(credentials=SyftSigningKey.generate())
         if metadata.node_type == NodeType.DOMAIN.value:
@@ -878,21 +665,14 @@
                 return SyftError(f"client {client}'s metadata is None!")
 
             result = self.api.services.network.exchange_credentials_with(
                 self_node_route=self_node_route,
                 remote_node_route=remote_node_route,
                 remote_node_verify_key=client.metadata.to(NodeMetadataV3).verify_key,
             )
-
-        elif protocol == SyftProtocol.VEILID:
-            remote_node_route = connection_to_route(client.connection)
-
-            result = self.api.services.network.exchange_veilid_route(
-                remote_node_route=remote_node_route,
-            )
         else:
             raise ValueError(
                 f"Invalid Route Exchange SyftProtocol: {protocol}.Supported protocols are {SyftProtocol.all()}"
             )
 
         return result
 
@@ -1162,26 +942,17 @@
 
 
 @instrument
 def connect(
     url: str | GridURL = DEFAULT_PYGRID_ADDRESS,
     node: AbstractNode | None = None,
     port: int | None = None,
-    vld_forward_proxy: str | GridURL | None = None,
-    vld_reverse_proxy: str | GridURL | None = None,
-    vld_key: str | None = None,
 ) -> SyftClient:
     if node:
         connection = PythonConnection(node=node)
-    elif vld_key and vld_forward_proxy and vld_reverse_proxy:
-        connection = VeilidConnection(
-            vld_forward_proxy=vld_forward_proxy,
-            vld_reverse_proxy=vld_reverse_proxy,
-            vld_key=vld_key,
-        )
     else:
         url = GridURL.from_url(url)
         if isinstance(port, int | str):
             url.set_port(int(port))
         connection = HTTPConnection(url=url)
 
     client_type = connection.get_client_type()
@@ -1215,27 +986,20 @@
 @instrument
 def login_as_guest(
     # HTTPConnection
     url: str | GridURL = DEFAULT_PYGRID_ADDRESS,
     port: int | None = None,
     # PythonConnection
     node: AbstractNode | None = None,
-    # Veilid Connection
-    vld_forward_proxy: str | GridURL | None = None,
-    vld_reverse_proxy: str | GridURL | None = None,
-    vld_key: str | None = None,
     verbose: bool = True,
 ) -> SyftClient:
     _client = connect(
         url=url,
         node=node,
         port=port,
-        vld_forward_proxy=vld_forward_proxy,
-        vld_reverse_proxy=vld_reverse_proxy,
-        vld_key=vld_key,
     )
 
     if isinstance(_client, SyftError):
         return _client
 
     if verbose and _client.metadata is not None:
         print(
@@ -1250,28 +1014,21 @@
 def login(
     email: str,
     # HTTPConnection
     url: str | GridURL = DEFAULT_PYGRID_ADDRESS,
     port: int | None = None,
     # PythonConnection
     node: AbstractNode | None = None,
-    # Veilid Connection
-    vld_forward_proxy: str | GridURL | None = None,
-    vld_reverse_proxy: str | GridURL | None = None,
-    vld_key: str | None = None,
     password: str | None = None,
     cache: bool = True,
 ) -> SyftClient:
     _client = connect(
         url=url,
         node=node,
         port=port,
-        vld_forward_proxy=vld_forward_proxy,
-        vld_reverse_proxy=vld_reverse_proxy,
-        vld_key=vld_key,
     )
 
     if isinstance(_client, SyftError):
         return _client
 
     connection = _client.connection
```

### Comparing `syft-0.8.7b1/src/syft/client/connection.py` & `syft-0.8.7b2/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/client/deploy.py` & `syft-0.8.7b2/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/client/domain_client.py` & `syft-0.8.7b2/src/syft/client/domain_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -302,18 +302,18 @@
             if isinstance(client, SyftError):
                 return client
 
         res = self.exchange_route(client, protocol=protocol)
         if isinstance(res, SyftSuccess):
             if self.metadata:
                 return SyftSuccess(
-                    message=f"Connected {self.metadata.node_type} to {client.name} gateway"
+                    message=f"Connected {self.metadata.node_type} '{self.metadata.name}' to gateway '{client.name}'"
                 )
             else:
-                return SyftSuccess(message=f"Connected to {client.name} gateway")
+                return SyftSuccess(message=f"Connected to '{client.name}' gateway")
         return res
 
     @property
     def data_subject_registry(self) -> APIModule | None:
         if self.api.has_service("data_subject"):
             return self.api.services.data_subject
         return None
```

### Comparing `syft-0.8.7b1/src/syft/client/enclave_client.py` & `syft-0.8.7b2/src/syft/client/enclave_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from ..client.api import APIRegistry
 from ..img.base64 import base64read
 from ..serde.serializable import serializable
 from ..service.metadata.node_metadata import NodeMetadataJSON
 from ..service.network.routes import NodeRouteType
 from ..service.response import SyftError
 from ..service.response import SyftSuccess
-from ..types.syft_object import SYFT_OBJECT_VERSION_2
+from ..types.syft_object import SYFT_OBJECT_VERSION_3
 from ..types.syft_object import SyftObject
 from ..types.uid import UID
 from ..util.fonts import FONT_CSS
 from .api import APIModule
 from .client import SyftClient
 from .client import login
 from .client import login_as_guest
@@ -31,15 +31,15 @@
     # relative
     from ..service.code.user_code import SubmitUserCode
 
 
 @serializable()
 class EnclaveMetadata(SyftObject):
     __canonical_name__ = "EnclaveMetadata"
-    __version__ = SYFT_OBJECT_VERSION_2
+    __version__ = SYFT_OBJECT_VERSION_3
 
     route: NodeRouteType
 
 
 @serializable()
 class EnclaveClient(SyftClient):
     # TODO: add widget repr for enclave client
@@ -92,15 +92,15 @@
                 return client
 
         self.metadata: NodeMetadataJSON = self.metadata
         res = self.exchange_route(client, protocol=protocol)
 
         if isinstance(res, SyftSuccess):
             return SyftSuccess(
-                message=f"Connected {self.metadata.node_type} to {client.name} gateway"
+                message=f"Connected {self.metadata.node_type} {self.metadata.name} to {client.name} gateway"
             )
 
         return res
 
     def get_enclave_metadata(self) -> EnclaveMetadata:
         return EnclaveMetadata(route=self.connection.route)
```

### Comparing `syft-0.8.7b1/src/syft/client/gateway_client.py` & `syft-0.8.7b2/src/syft/client/gateway_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,34 +3,40 @@
 
 # relative
 from ..abstract_node import NodeSideType
 from ..abstract_node import NodeType
 from ..img.base64 import base64read
 from ..node.credentials import SyftSigningKey
 from ..serde.serializable import serializable
+from ..service.metadata.node_metadata import NodeMetadataJSON
 from ..service.network.node_peer import NodePeer
 from ..service.response import SyftError
 from ..service.response import SyftException
 from ..types.syft_object import SYFT_OBJECT_VERSION_2
 from ..types.syft_object import SyftObject
 from ..util.fonts import FONT_CSS
 from .client import SyftClient
+from .connection import NodeConnection
 
 
 @serializable()
 class GatewayClient(SyftClient):
     # TODO: add widget repr for gateway client
 
     def proxy_to(self, peer: Any) -> SyftClient:
         # relative
         from .domain_client import DomainClient
         from .enclave_client import EnclaveClient
 
-        connection = self.connection.with_proxy(peer.id)
-        metadata = connection.get_node_metadata(credentials=SyftSigningKey.generate())
+        connection: type[NodeConnection] = self.connection.with_proxy(peer.id)
+        metadata: NodeMetadataJSON | SyftError = connection.get_node_metadata(
+            credentials=SyftSigningKey.generate()
+        )
+        if isinstance(metadata, SyftError):
+            return metadata
         if metadata.node_type == NodeType.DOMAIN.value:
             client_type: type[SyftClient] = DomainClient
         elif metadata.node_type == NodeType.ENCLAVE.value:
             client_type = EnclaveClient
         else:
             raise SyftException(
                 f"Unknown node type {metadata.node_type} to create proxy client"
```

### Comparing `syft-0.8.7b1/src/syft/client/registry.py` & `syft-0.8.7b2/src/syft/client/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,28 +46,29 @@
                 f"Failed to get Network Registry, go checkout: {NETWORK_REGISTRY_REPO}. Exception: {e}"
             )
 
     @staticmethod
     def load_network_registry_json() -> dict:
         try:
             # Get the environment variable
-            network_registry_json = os.getenv("NETWORK_REGISTRY_JSON")
+            network_registry_json: str | None = os.getenv("NETWORK_REGISTRY_JSON")
             # If the environment variable exists, use it
             if network_registry_json is not None:
                 network_json: dict = json.loads(network_registry_json)
             else:
                 # Load the network registry from the NETWORK_REGISTRY_URL
-                response = requests.get(NETWORK_REGISTRY_URL, timeout=10)  # nosec
+                response = requests.get(NETWORK_REGISTRY_URL, timeout=30)  # nosec
+                response.raise_for_status()  # raise an exception if the HTTP request returns an error
                 network_json = response.json()
 
             return network_json
 
         except Exception as e:
             warning(
-                f"Failed to get Network Registry, go checkout: {NETWORK_REGISTRY_REPO}. {e}"
+                f"Failed to get Network Registry from {NETWORK_REGISTRY_REPO}. Exception: {e}"
             )
             return {}
 
     @property
     def online_networks(self) -> list[dict]:
         networks = self.all_networks
```

### Comparing `syft-0.8.7b1/src/syft/client/search.py` & `syft-0.8.7b2/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/client/syncing.py` & `syft-0.8.7b2/src/syft/client/syncing.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/client/user_settings.py` & `syft-0.8.7b2/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/custom_worker/builder.py` & `syft-0.8.7b2/src/syft/custom_worker/builder.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/custom_worker/builder_docker.py` & `syft-0.8.7b2/src/syft/custom_worker/builder_docker.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/custom_worker/builder_k8s.py` & `syft-0.8.7b2/src/syft/custom_worker/builder_k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/custom_worker/builder_types.py` & `syft-0.8.7b2/src/syft/custom_worker/builder_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/custom_worker/config.py` & `syft-0.8.7b2/src/syft/custom_worker/config.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/custom_worker/k8s.py` & `syft-0.8.7b2/src/syft/custom_worker/k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/custom_worker/runner_k8s.py` & `syft-0.8.7b2/src/syft/custom_worker/runner_k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/custom_worker/utils.py` & `syft-0.8.7b2/src/syft/custom_worker/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/exceptions/exception.py` & `syft-0.8.7b2/src/syft/exceptions/exception.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/gevent_patch.py` & `syft-0.8.7b2/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/img/logo.png` & `syft-0.8.7b2/src/syft/img/logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/img/small-grid-symbol-logo.png` & `syft-0.8.7b2/src/syft/img/small-grid-symbol-logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/node/credentials.py` & `syft-0.8.7b2/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/node/node.py` & `syft-0.8.7b2/src/syft/node/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import subprocess  # nosec
 import tempfile
 from time import sleep
 import traceback
 from typing import Any
 
 # third party
+from loguru import logger
 from nacl.signing import SigningKey
 from result import Err
 from result import Result
 from typing_extensions import Self
 
 # relative
 from .. import __version__
@@ -92,15 +93,14 @@
 from ..service.settings.settings_stash import SettingsStash
 from ..service.sync.sync_service import SyncService
 from ..service.user.user import User
 from ..service.user.user import UserCreate
 from ..service.user.user_roles import ServiceRole
 from ..service.user.user_service import UserService
 from ..service.user.user_stash import UserStash
-from ..service.veilid import VeilidServiceProvider
 from ..service.worker.image_registry_service import SyftImageRegistryService
 from ..service.worker.utils import DEFAULT_WORKER_IMAGE_TAG
 from ..service.worker.utils import DEFAULT_WORKER_POOL_NAME
 from ..service.worker.utils import create_default_image
 from ..service.worker.worker_image_service import SyftWorkerImageService
 from ..service.worker.worker_pool import WorkerPool
 from ..service.worker.worker_pool_service import SyftWorkerPoolService
@@ -191,14 +191,20 @@
     return get_env("DEFAULT_WORKER_POOL_IMAGE")
 
 
 def get_default_worker_pool_name() -> str | None:
     return get_env("DEFAULT_WORKER_POOL_NAME", DEFAULT_WORKER_POOL_NAME)
 
 
+def get_default_bucket_name() -> str:
+    env = get_env("DEFAULT_BUCKET_NAME")
+    node_id = get_node_uid_env() or "syft-bucket"
+    return env or node_id or "syft-bucket"
+
+
 def get_default_worker_pool_count(node: Node) -> int:
     return int(
         get_env(
             "DEFAULT_WORKER_POOL_COUNT", node.queue_config.client_config.n_consumers
         )
     )
 
@@ -870,16 +876,15 @@
             {"svc": BlobStorageService},
             {"svc": MigrateStateService},
             {"svc": SyftWorkerImageService},
             {"svc": SyftWorkerPoolService},
             {"svc": SyftImageRegistryService},
             {"svc": SyncService},
             {"svc": OutputService},
-            {"svc": UserCodeStatusService},
-            {"svc": VeilidServiceProvider},  # this is lazy
+            {"svc": UserCodeStatusService},  # this is lazy
         ]
 
         for svc_kwargs in default_services:
             ServiceCls = svc_kwargs.pop("svc")
             svc_kwargs.setdefault("store", self.document_store)
 
             svc_instance = ServiceCls(**svc_kwargs)
@@ -1028,15 +1033,15 @@
                 credentials=credentials,
             )
             return queue_obj
         return result.err()
 
     def forward_message(
         self, api_call: SyftAPICall | SignedSyftAPICall
-    ) -> Result[QueueItem | SyftObject, Err]:
+    ) -> Result | QueueItem | SyftObject | SyftError | Any:
         node_uid = api_call.message.node_uid
         if "networkservice" not in self.service_path_map:
             return SyftError(
                 message=(
                     "Node has no network service so we can't "
                     f"forward this message to {node_uid}"
                 )
@@ -1049,22 +1054,29 @@
 
         if peer.is_ok() and peer.ok():
             peer = peer.ok()
 
             # Since we have several routes to a peer
             # we need to cache the client for a given node_uid along with the route
             peer_cache_key = hash(node_uid) + hash(peer.pick_highest_priority_route())
-
             if peer_cache_key in self.peer_client_cache:
                 client = self.peer_client_cache[peer_cache_key]
             else:
                 context = AuthedServiceContext(
                     node=self, credentials=api_call.credentials
                 )
+
                 client = peer.client_with_context(context=context)
+                if client.is_err():
+                    return SyftError(
+                        message=f"Failed to create remote client for peer: "
+                        f"{peer.id}. Error: {client.err()}"
+                    )
+                client = client.ok()
+
                 self.peer_client_cache[peer_cache_key] = client
 
         if client:
             message: SyftAPICall = api_call.message
             if message.path == "metadata":
                 result = client.metadata
             elif message.path == "login":
@@ -1127,14 +1139,15 @@
             )
         else:
             if not api_call.is_valid:
                 return SyftError(message="Your message signature is invalid")
 
         if api_call.message.node_uid != self.id and check_call_location:
             return self.forward_message(api_call=api_call)
+
         if api_call.message.path == "queue":
             return self.resolve_future(
                 credentials=api_call.credentials, uid=api_call.message.kwargs["uid"]
             )
 
         if api_call.message.path == "metadata":
             return self.metadata
@@ -1548,14 +1561,20 @@
     worker_count = get_default_worker_pool_count(node)
     context = AuthedServiceContext(
         node=node,
         credentials=credentials,
         role=ServiceRole.ADMIN,
     )
 
+    if isinstance(default_worker_pool, SyftError):
+        logger.error(
+            f"Failed to get default worker pool {default_pool_name}. Error: {default_worker_pool.message}"
+        )
+        return default_worker_pool
+
     print(f"Creating default worker image with tag='{default_worker_tag}'")
     # Get/Create a default worker SyftWorkerImage
     default_image = create_default_image(
         credentials=credentials,
         image_stash=image_stash,
         tag=default_worker_tag,
         in_kubernetes=in_kubernetes(),
```

### Comparing `syft-0.8.7b1/src/syft/node/routes.py` & `syft-0.8.7b2/src/syft/node/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/node/run.py` & `syft-0.8.7b2/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/node/server.py` & `syft-0.8.7b2/src/syft/node/server.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/node/worker_settings.py` & `syft-0.8.7b2/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/protocol/data_protocol.py` & `syft-0.8.7b2/src/syft/protocol/data_protocol.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/protocol/protocol_version.json` & `syft-0.8.7b2/src/syft/protocol/protocol_version.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9863888888888889%*

 * *Differences: {"'dev'": "{'object_versions': {'CustomAPIView': {'1': {'hash': "*

 * *          "'5cdfaea6b5af235d0f9ab8e6f01d6cebcde7c8bf4efd00aec26c343965ef865e'}}, "*

 * *          "'TwinAPIEndpoint': {'1': {'hash': "*

 * *          "'03a0244c6b322e72032c5c33c1db09b913f83d72cfad1cc51ac4ec90506afcf5'}}, "*

 * *          "'EnclaveMetadata': OrderedDict([('2', OrderedDict([('version', 2), ('hash', "*

 * *          "'6dcc26695abc6a9ecd9d7d1e6507a9f1a92cc5ccd10987e92419bf984245f9a1'), ('action', "*

 * *          "'remove')])), ('3', OrderedDict([('versi […]*

```diff
@@ -19,37 +19,56 @@
                     "hash": "98021128a9be0a9a135b43b50cb08f141faed72bc39999a9cedd162bc8814f62",
                     "version": 1
                 }
             },
             "CustomAPIView": {
                 "1": {
                     "action": "add",
-                    "hash": "21cada3f8b8609e91e4f01f3bfdbdab3f8b96003163e09dba1c4b31041598ca2",
+                    "hash": "5cdfaea6b5af235d0f9ab8e6f01d6cebcde7c8bf4efd00aec26c343965ef865e",
                     "version": 1
                 }
             },
             "CustomEndpointActionObject": {
                 "1": {
                     "action": "add",
                     "hash": "642facc6cafbaad4de030a33cd619bd68ac31a32b0db07ddc1c1d5d7f914503e",
                     "version": 1
                 }
             },
+            "EnclaveMetadata": {
+                "2": {
+                    "action": "remove",
+                    "hash": "6dcc26695abc6a9ecd9d7d1e6507a9f1a92cc5ccd10987e92419bf984245f9a1",
+                    "version": 2
+                },
+                "3": {
+                    "action": "add",
+                    "hash": "d2f23411927c68e2307a84d180ad053b3e4ba12d74aba64d34dac224c90e815d",
+                    "version": 3
+                }
+            },
             "ExecutionOutput": {
                 "1": {
                     "action": "remove",
                     "hash": "c2337099eba14767ead75fcc1b1fa265c1898461ede0b5e7758a0e8d11d1757d",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
                     "hash": "854fe9df5bcbb5c7e5b7c467bac423cd98c32f93d6876fea7b8eb6c08f6596da",
                     "version": 2
                 }
             },
+            "NodePeer": {
+                "3": {
+                    "action": "add",
+                    "hash": "dababb03d2463b6218ae22d55293a60580f5a14bebd0c664d71da104e2f0b835",
+                    "version": 3
+                }
+            },
             "PrivateAPIEndpoint": {
                 "1": {
                     "action": "add",
                     "hash": "004ec19753263440e2896b4e35d7a6305322934512f473f37d54043af5726fe6",
                     "version": 1
                 }
             },
@@ -87,31 +106,31 @@
             "SyncStateItem": {
                 "1": {
                     "action": "remove",
                     "hash": "4dbfa0813f5a3f7be0b36249ff2d67e395ad7c9e138c5a122fc7342b8dcc4b92",
                     "version": 1
                 }
             },
-            "SyncView": {
+            "TwinAPIEndpoint": {
                 "1": {
                     "action": "add",
-                    "hash": "4e87744e86cd7781e3d5cf4618e63516f3d26309a4da919033dacc5ed338d76d",
+                    "hash": "03a0244c6b322e72032c5c33c1db09b913f83d72cfad1cc51ac4ec90506afcf5",
                     "version": 1
                 }
             },
-            "TwinAPIEndpoint": {
+            "UpdateTwinAPIEndpoint": {
                 "1": {
                     "action": "add",
-                    "hash": "edcd67ab41edfae56deb23d9ef838edc442f587bdb16b8e8c46efa20c04e3c25",
+                    "hash": "6c0c6bc042391e60d5c78893f859c8bdec4b45f0bdc7749957a425e041a4096c",
                     "version": 1
                 }
             },
-            "UpdateTwinAPIEndpoint": {
+            "VeilidConnection": {
                 "1": {
-                    "action": "add",
-                    "hash": "6c0c6bc042391e60d5c78893f859c8bdec4b45f0bdc7749957a425e041a4096c",
+                    "action": "remove",
+                    "hash": "c1796e7b01c9eae0dbf59cfd5c2c2f0e7eba593e0cea615717246572b27aae4b",
                     "version": 1
                 }
             }
         }
     }
 }
```

### Comparing `syft-0.8.7b1/src/syft/protocol/releases/0.8.2.json` & `syft-0.8.7b2/src/syft/protocol/releases/0.8.2.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/protocol/releases/0.8.3.json` & `syft-0.8.7b2/src/syft/protocol/releases/0.8.3.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/protocol/releases/0.8.4.json` & `syft-0.8.7b2/src/syft/protocol/releases/0.8.4.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/protocol/releases/0.8.6.json` & `syft-0.8.7b2/src/syft/protocol/releases/0.8.6.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/serde/array.py` & `syft-0.8.7b2/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/serde/arrow.py` & `syft-0.8.7b2/src/syft/serde/arrow.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,28 +9,32 @@
 from ..util.experimental_flags import ApacheArrowCompression
 from ..util.experimental_flags import flags
 from .deserialize import _deserialize
 from .serialize import _serialize
 
 
 def arrow_serialize(obj: np.ndarray) -> bytes:
-    original_dtype = obj.dtype
-    apache_arrow = pa.Tensor.from_numpy(obj=obj)
-    sink = pa.BufferOutputStream()
-    pa.ipc.write_tensor(apache_arrow, sink)
-    buffer = sink.getvalue()
-    if flags.APACHE_ARROW_COMPRESSION is ApacheArrowCompression.NONE:
-        numpy_bytes = buffer.to_pybytes()
-    else:
-        numpy_bytes = pa.compress(
-            buffer, asbytes=True, codec=flags.APACHE_ARROW_COMPRESSION.value
-        )
-    dtype = original_dtype.name
+    # inner function to make sure variables go out of scope after this
+    def inner(obj: np.ndarray) -> tuple:
+        original_dtype = obj.dtype
+        apache_arrow = pa.Tensor.from_numpy(obj=obj)
+        sink = pa.BufferOutputStream()
+        pa.ipc.write_tensor(apache_arrow, sink)
+        buffer = sink.getvalue()
+        if flags.APACHE_ARROW_COMPRESSION is ApacheArrowCompression.NONE:
+            numpy_bytes = buffer.to_pybytes()
+        else:
+            numpy_bytes = pa.compress(
+                buffer, asbytes=True, codec=flags.APACHE_ARROW_COMPRESSION.value
+            )
+        dtype = original_dtype.name
+        return (numpy_bytes, buffer.size, dtype)
 
-    return cast(bytes, _serialize((numpy_bytes, buffer.size, dtype), to_bytes=True))
+    m = inner(obj)
+    return cast(bytes, _serialize(m, to_bytes=True))
 
 
 def arrow_deserialize(
     numpy_bytes: bytes, decompressed_size: int, dtype: str
 ) -> np.ndarray:
     original_dtype = np.dtype(dtype)
     if flags.APACHE_ARROW_COMPRESSION is ApacheArrowCompression.NONE:
```

### Comparing `syft-0.8.7b1/src/syft/serde/deserialize.py` & `syft-0.8.7b2/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/serde/lib_permissions.py` & `syft-0.8.7b2/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/serde/lib_service_registry.py` & `syft-0.8.7b2/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/serde/mock.py` & `syft-0.8.7b2/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/serde/recursive.py` & `syft-0.8.7b2/src/syft/serde/recursive.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # stdlib
 from collections.abc import Callable
 from enum import Enum
 from enum import EnumMeta
 import sys
+import tempfile
 import types
 from typing import Any
 
 # third party
 from capnp.lib.capnp import _DynamicStructBuilder
 from pydantic import BaseModel
 
@@ -18,14 +19,16 @@
 from ..util.util import index_syft_by_module_name
 from .capnp import get_capnp_schema
 
 TYPE_BANK = {}
 
 recursive_scheme = get_capnp_schema("recursive_serde.capnp").RecursiveSerde
 
+SPOOLED_FILE_MAX_SIZE_SERDE = 50 * (1024**2)  # 50MB
+
 
 def get_types(cls: type, keys: list[str] | None = None) -> list[type] | None:
     if keys is None:
         return None
     types = []
     for key in keys:
         _type = None
@@ -157,24 +160,36 @@
 
     if isinstance(alias_fqn, tuple):
         for alias in alias_fqn:
             TYPE_BANK[alias] = serde_attributes
 
 
 def chunk_bytes(
-    data: bytes, field_name: str | int, builder: _DynamicStructBuilder
+    field_obj: Any,
+    ser_func: Callable,
+    field_name: str | int,
+    builder: _DynamicStructBuilder,
 ) -> None:
-    CHUNK_SIZE = int(5.12e8)  # capnp max for a List(Data) field
-    list_size = len(data) // CHUNK_SIZE + 1
-    data_lst = builder.init(field_name, list_size)
-    END_INDEX = CHUNK_SIZE
-    for idx in range(list_size):
-        START_INDEX = idx * CHUNK_SIZE
-        END_INDEX = min(START_INDEX + CHUNK_SIZE, len(data))
-        data_lst[idx] = data[START_INDEX:END_INDEX]
+    data = ser_func(field_obj)
+    size_of_data = len(data)
+    with tempfile.SpooledTemporaryFile(
+        max_size=SPOOLED_FILE_MAX_SIZE_SERDE
+    ) as tmp_file:
+        # Write data to a file to save RAM
+        tmp_file.write(data)
+        tmp_file.seek(0)
+        del data
+
+        CHUNK_SIZE = int(5.12e8)  # capnp max for a List(Data) field
+        list_size = size_of_data // CHUNK_SIZE + 1
+        data_lst = builder.init(field_name, list_size)
+        for idx in range(list_size):
+            bytes_to_read = min(CHUNK_SIZE, size_of_data)
+            data_lst[idx] = tmp_file.read(bytes_to_read)
+            size_of_data -= CHUNK_SIZE
 
 
 def combine_bytes(capnp_list: list[bytes]) -> bytes:
     # TODO: make sure this doesn't copy, perhaps allocate a fixed size buffer
     # and move the bytes into it as we go
     bytes_value = b""
     for value in capnp_list:
@@ -191,15 +206,14 @@
         is_type = True
 
     msg = recursive_scheme.new_message()
     fqn = get_fully_qualified_name(self)
     if fqn not in TYPE_BANK:
         # third party
         raise Exception(f"{fqn} not in TYPE_BANK")
-
     msg.fullyQualifiedName = fqn
     (
         nonrecursive,
         serialize,
         deserialize,
         attribute_list,
         exclude_attrs_list,
@@ -211,15 +225,15 @@
     ) = TYPE_BANK[fqn]
 
     if nonrecursive or is_type:
         if serialize is None:
             raise Exception(
                 f"Cant serialize {type(self)} nonrecursive without serialize."
             )
-        chunk_bytes(serialize(self), "nonrecursiveBlob", msg)
+        chunk_bytes(self, serialize, "nonrecursiveBlob", msg)
         return msg
 
     if attribute_list is None:
         attribute_list = self.__dict__.keys()
 
     hash_exclude_attrs_set = (
         set(hash_exclude_attrs).union(set(DYNAMIC_SYFT_ATTRIBUTES))
@@ -244,17 +258,21 @@
 
         if transforms is not None:
             field_obj = transforms[0](field_obj)
 
         if isinstance(field_obj, types.FunctionType):
             continue
 
-        serialized = sy.serialize(field_obj, to_bytes=True, for_hashing=for_hashing)
         msg.fieldsName[idx] = attr_name
-        chunk_bytes(serialized, idx, msg.fieldsData)
+        chunk_bytes(
+            field_obj,
+            lambda x: sy.serialize(x, to_bytes=True, for_hashing=for_hashing),
+            idx,
+            msg.fieldsData,
+        )
 
     return msg
 
 
 def rs_bytes2object(blob: bytes) -> Any:
     MAX_TRAVERSAL_LIMIT = 2**64 - 1
```

### Comparing `syft-0.8.7b1/src/syft/serde/recursive_primitives.py` & `syft-0.8.7b2/src/syft/serde/recursive_primitives.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from collections.abc import Mapping
 from enum import Enum
 from enum import EnumMeta
 import functools
 import pathlib
 from pathlib import PurePath
 import sys
+import tempfile
 from types import MappingProxyType
 from types import UnionType
 from typing import Any
 from typing import GenericAlias
 from typing import Optional
 from typing import TypeVar
 from typing import Union
@@ -22,35 +23,50 @@
 from typing import _SpecialGenericAlias
 from typing import _UnionGenericAlias
 from typing import cast
 import weakref
 
 # relative
 from .capnp import get_capnp_schema
+from .recursive import SPOOLED_FILE_MAX_SIZE_SERDE
 from .recursive import chunk_bytes
 from .recursive import combine_bytes
 from .recursive import recursive_serde_register
+from .util import compatible_with_large_file_writes_capnp
 
 iterable_schema = get_capnp_schema("iterable.capnp").Iterable
 kv_iterable_schema = get_capnp_schema("kv_iterable.capnp").KVIterable
 
 
 def serialize_iterable(iterable: Collection) -> bytes:
     # relative
     from .serialize import _serialize
 
     message = iterable_schema.new_message()
 
     message.init("values", len(iterable))
 
     for idx, it in enumerate(iterable):
-        serialized = _serialize(it, to_bytes=True)
-        chunk_bytes(serialized, idx, message.values)
+        # serialized = _serialize(it, to_bytes=True)
+        chunk_bytes(it, lambda x: _serialize(x, to_bytes=True), idx, message.values)
 
-    return message.to_bytes()
+    if compatible_with_large_file_writes_capnp():
+        with tempfile.SpooledTemporaryFile(
+            max_size=SPOOLED_FILE_MAX_SIZE_SERDE
+        ) as tmp_file:
+            # Write data to a file to save RAM
+            message.write(tmp_file)
+            del message
+            tmp_file.seek(0)
+            res = tmp_file.read()
+            return res
+    else:
+        res = message.to_bytes()
+        del message
+        return res
 
 
 def deserialize_iterable(iterable_type: type, blob: bytes) -> Collection:
     # relative
     from .deserialize import _deserialize
 
     MAX_TRAVERSAL_LIMIT = 2**64 - 1
@@ -76,16 +92,16 @@
     message = kv_iterable_schema.new_message()
 
     message.init("keys", size)
     message.init("values", size)
 
     for index, (k, v) in enumerate(kv_pairs):
         message.keys[index] = _serialize(k, to_bytes=True)
-        serialized = _serialize(v, to_bytes=True)
-        chunk_bytes(serialized, index, message.values)
+        # serialized = _serialize(v, to_bytes=True)
+        chunk_bytes(v, lambda x: _serialize(x, to_bytes=True), index, message.values)
 
     return message.to_bytes()
 
 
 def serialize_kv(map: Mapping) -> bytes:
     return _serialize_kv_pairs(len(map), map.items())
```

### Comparing `syft-0.8.7b1/src/syft/serde/serializable.py` & `syft-0.8.7b2/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/serde/signature.py` & `syft-0.8.7b2/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/serde/third_party.py` & `syft-0.8.7b2/src/syft/serde/third_party.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/action/action_data_empty.py` & `syft-0.8.7b2/src/syft/service/action/action_data_empty.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/action/action_endpoint.py` & `syft-0.8.7b2/src/syft/service/action/action_endpoint.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/action/action_graph.py` & `syft-0.8.7b2/src/syft/service/action/action_graph.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/action/action_graph_service.py` & `syft-0.8.7b2/src/syft/service/action/action_graph_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/action/action_object.py` & `syft-0.8.7b2/src/syft/service/action/action_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # future
 from __future__ import annotations
 
 # stdlib
 from collections.abc import Callable
+from collections.abc import Iterable
 from enum import Enum
 import inspect
 from io import BytesIO
 from pathlib import Path
+import sys
 import threading
 import time
 import traceback
 import types
 from typing import Any
 from typing import ClassVar
 from typing import TYPE_CHECKING
@@ -299,14 +301,15 @@
     "__sha256__",  # syft
     "__hash_exclude_attrs__",  # syft
     "__private_sync_attr_mocks__",  # syft
     "__exclude_sync_diff_attrs__",  # syft
     "__repr_attrs__",  # syft
     "get_sync_dependencies",
     "_data_repr",
+    "syft_eq",  # syft
 ]
 dont_wrap_output_attrs = [
     "__repr__",
     "__str__",
     "__repr_attrs__",
     "_repr_html_",
     "_repr_markdown_",
@@ -320,14 +323,15 @@
     "node_uid",
     "syft_action_data_node_id",
     "__sha256__",
     "__hash_exclude_attrs__",
     "__exclude_sync_diff_attrs__",  # syft
     "__repr_attrs__",  # syft
     "get_sync_dependencies",  # syft
+    "syft_eq",  # syft
 ]
 dont_make_side_effects = [
     "__repr_attrs__",
     "_repr_html_",
     "_repr_markdown_",
     "_repr_latex_",
     "__repr__",
@@ -339,20 +343,36 @@
     "node_uid",
     "syft_action_data_node_id",
     "__sha256__",
     "__hash_exclude_attrs__",
     "__exclude_sync_diff_attrs__",  # syft
     "__repr_attrs__",
     "get_sync_dependencies",
+    "syft_eq",  # syft
 ]
 action_data_empty_must_run = [
     "__repr__",
     "__str__",
 ]
 
+methods_to_check_in_cache = [
+    "_ipython_display_",
+    "_repr_mimebundle_",
+    "_repr_latex_",
+    "_repr_javascript_",
+    "_repr_html_",
+    "_repr_jpeg_",
+    "_repr_png_",
+    "_repr_svg_",
+    "_repr_pretty_",
+    "_repr_pdf_",
+    "_repr_json_",
+    "_repr_markdown_",
+]
+
 
 class PreHookContext(SyftBaseObject):
     __canonical_name__ = "PreHookContext"
     __version__ = SYFT_OBJECT_VERSION_2
 
     """Hook context
 
@@ -621,14 +641,15 @@
     "__hash__",
     "create_shareable_sync_copy",
     "_has_private_sync_attrs",
     "__exclude_sync_diff_attrs__",
     "__repr_attrs__",
     "get_sync_dependencies",
     "_data_repr",
+    "syft_eq",
 ]
 
 
 @serializable(without=["syft_pre_hooks__", "syft_post_hooks__"])
 class ActionObject(SyncableSyftObject):
     """Action object for remote execution."""
 
@@ -674,15 +695,23 @@
 
         # Sanity check
         if ext_obj.id != self.id:
             raise Exception("Not the same id for low side and high side requests")
 
         low_data = ext_obj.syft_action_data
         high_data = self.syft_action_data
-        if low_data != high_data:
+
+        try:
+            cmp = low_data != high_data
+            if isinstance(cmp, Iterable):
+                cmp = all(cmp)
+        except Exception:
+            cmp = False
+
+        if cmp:
             diff_attr = AttrDiff(
                 attr_name="syft_action_data", low_attr=low_data, high_attr=high_data
             )
             diff_attrs.append(diff_attr)
         return diff_attrs
 
     def _set_obj_location_(self, node_uid: UID, credentials: SyftVerifyKey) -> None:
@@ -752,32 +781,35 @@
         if not isinstance(data, ActionDataEmpty):
             if isinstance(data, BlobFile) and not data.uploaded:
                 api = APIRegistry.api_for(
                     self.syft_node_location, self.syft_client_verify_key
                 )
                 data.upload_to_blobstorage_from_api(api)
             else:
-                storage_entry = CreateBlobStorageEntry.from_obj(data)
+                serialized = serialize(data, to_bytes=True)
+                size = sys.getsizeof(serialized)
+                storage_entry = CreateBlobStorageEntry.from_obj(data, file_size=size)
+
+                if not TraceResultRegistry.current_thread_is_tracing():
+                    self.syft_action_data_cache = self.as_empty_data()
                 if self.syft_blob_storage_entry_id is not None:
                     # TODO: check if it already exists
                     storage_entry.id = self.syft_blob_storage_entry_id
                 allocate_method = from_api_or_context(
                     func_or_path="blob_storage.allocate",
                     syft_node_location=self.syft_node_location,
                     syft_client_verify_key=self.syft_client_verify_key,
                 )
                 if allocate_method is not None:
                     blob_deposit_object = allocate_method(storage_entry)
 
                     if isinstance(blob_deposit_object, SyftError):
                         return blob_deposit_object
 
-                    result = blob_deposit_object.write(
-                        BytesIO(serialize(data, to_bytes=True))
-                    )
+                    result = blob_deposit_object.write(BytesIO(serialized))
                     if isinstance(result, SyftError):
                         return result
                     self.syft_blob_storage_entry_id = (
                         blob_deposit_object.blob_storage_entry_id
                     )
                 else:
                     print("cannot save to blob storage")
@@ -869,14 +901,19 @@
 
     def syft_is_property(self, obj: Any, method: str) -> bool:
         klass_method = getattr(type(obj), method, None)
         return isinstance(klass_method, property) or inspect.isdatadescriptor(
             klass_method
         )
 
+    def syft_eq(self, ext_obj: Self | None) -> bool:
+        if ext_obj is None:
+            return False
+        return self.id.id == ext_obj.id.id
+
     def syft_execute_action(
         self, action: Action, sync: bool = True
     ) -> ActionObjectPointer:
         """Execute a remote action
 
         Parameters:
             action: Action
@@ -1551,16 +1588,14 @@
         """The results from these attributes are ignored from UID patching."""
         return dont_wrap_output_attrs + getattr(self, "syft_dont_wrap_attrs", [])
 
     def _syft_get_attr_context(self, name: str) -> Any:
         """Find which instance - Syft ActionObject or the original object - has the requested attribute."""
         defined_on_self = name in self.__dict__ or name in self.__private_attributes__
 
-        debug(">> ", name, ", defined_on_self = ", defined_on_self)
-
         # use the custom defined version
         context_self = self
         if not defined_on_self:
             context_self = self.syft_action_data
 
         return context_self
 
@@ -1781,41 +1816,49 @@
          * use the syft/_syft prefix for internal methods.
          * add the method name to the passthrough_attrs.
 
         Parameters:
             name: str
                 The name of the attribute to access.
         """
+        # bypass ipython canary verification
+        if name == "_ipython_canary_method_should_not_exist_":
+            return None
+
         # bypass certain attrs to prevent recursion issues
         if name.startswith("_syft") or name.startswith("syft"):
             return object.__getattribute__(self, name)
 
         if name in passthrough_attrs:
             return object.__getattribute__(self, name)
 
         # third party
         if name in self._syft_passthrough_attrs():
             return object.__getattribute__(self, name)
-        context_self = self._syft_get_attr_context(name)
 
         # Handle bool operator on nonbools
         if name == "__bool__" and not self.syft_has_bool_attr:
             return self._syft_wrap_attribute_for_bool_on_nonbools(name)
 
+        # check cache first
+        if name in methods_to_check_in_cache:
+            return getattr(self.syft_action_data_cache, name, None)
+
         # Handle Properties
+        context_self = self._syft_get_attr_context(name)
         if self.syft_is_property(context_self, name):
             return self._syft_wrap_attribute_for_properties(name)
 
         # Handle anything else
         res = self._syft_wrap_attribute_for_methods(name)
         return res
 
     @property
     def is_link(self) -> bool:
-        return isinstance(self.syft_action_data, ActionDataLink)
+        return self.syft_action_data_type is ActionDataLink
 
     def __setattr__(self, name: str, value: Any) -> Any:
         defined_on_self = name in self.__dict__ or name in self.__private_attributes__
 
         debug(">> ", name, ", defined_on_self = ", defined_on_self)
 
         # use the custom defined version
@@ -1854,15 +1897,15 @@
                     if (
                         self.syft_action_data_cache is not None
                         and hasattr(self.syft_action_data_cache, "_repr_markdown_")
                     )
                     else self.syft_action_data_cache.__repr__()
                 )
 
-        return f"```python\n{res}\n```\n{data_repr_}"
+        return f"```python\n{res}\n{data_repr_}```\n"
 
     def _data_repr(self) -> str | None:
         if isinstance(self.syft_action_data_cache, ActionDataEmpty):
             data_repr = self.syft_action_data_repr_
         elif inspect.isclass(self.syft_action_data_cache):
             data_repr = repr_cls(self.syft_action_data_cache)
         else:
@@ -2037,14 +2080,19 @@
 
     def __rrshift__(self, other: Any) -> Any:
         return self._syft_output_action_object(self.__rrshift__(other))
 
 
 @serializable()
 class AnyActionObject(ActionObject):
+    """
+    This is a catch-all class for all objects that are not
+    defined in the `action_types` dictionary.
+    """
+
     __canonical_name__ = "AnyActionObject"
     __version__ = SYFT_OBJECT_VERSION_3
 
     syft_internal_type: ClassVar[type[Any]] = NoneType  # type: ignore
     # syft_passthrough_attrs: List[str] = []
     syft_dont_wrap_attrs: list[str] = ["__str__", "__repr__", "syft_action_data_str_"]
     syft_action_data_str_: str = ""
```

### Comparing `syft-0.8.7b1/src/syft/service/action/action_permissions.py` & `syft-0.8.7b2/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/action/action_service.py` & `syft-0.8.7b2/src/syft/service/action/action_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,20 +136,19 @@
     def is_resolved(
         self,
         context: AuthedServiceContext,
         uid: UID,
     ) -> Result[Ok[bool], Err[str]]:
         """Get an object from the action store"""
         # relative
-        from .action_data_empty import ActionDataLink
 
         result = self._get(context, uid)
         if result.is_ok():
             obj = result.ok()
-            if isinstance(obj.syft_action_data, ActionDataLink):
+            if obj.is_link:
                 result = self.resolve_links(
                     context, obj.syft_action_data.action_object_id.id
                 )
 
                 # Checking in case any error occurred
                 if result.is_err():
                     return result
@@ -173,23 +172,22 @@
         self,
         context: AuthedServiceContext,
         uid: UID,
         twin_mode: TwinMode = TwinMode.PRIVATE,
     ) -> Result[Ok[ActionObject], Err[str]]:
         """Get an object from the action store"""
         # relative
-        from .action_data_empty import ActionDataLink
 
         result = self.store.get(uid=uid, credentials=context.credentials)
         # If user has permission to get the object / object exists
         if result.is_ok():
             obj = result.ok()
 
             # If it's not a leaf
-            if isinstance(obj.syft_action_data, ActionDataLink):
+            if obj.is_link:
                 nested_result = self.resolve_links(
                     context, obj.syft_action_data.action_object_id.id, twin_mode
                 )
                 return nested_result
 
             # If it's a leaf
             return result
@@ -215,30 +213,29 @@
         has_permission: bool = False,
         resolve_nested: bool = True,
     ) -> Result[ActionObject, str]:
         """Get an object from the action store"""
         # stdlib
 
         # relative
-        from .action_data_empty import ActionDataLink
 
         result = self.store.get(
             uid=uid, credentials=context.credentials, has_permission=has_permission
         )
         if result.is_ok() and context.node is not None:
             obj: TwinObject | ActionObject = result.ok()
             obj._set_obj_location_(
                 context.node.id,
                 context.credentials,
             )
             # Resolve graph links
             if (
                 not isinstance(obj, TwinObject)  # type: ignore[unreachable]
                 and resolve_nested
-                and isinstance(obj.syft_action_data, ActionDataLink)
+                and obj.is_link
             ):
                 if not self.is_resolved(  # type: ignore[unreachable]
                     context, obj.syft_action_data.action_object_id.id
                 ).ok():
                     return SyftError(message="This object is not resolved yet.")
                 result = self.resolve_links(
                     context, obj.syft_action_data.action_object_id.id, twin_mode
@@ -311,15 +308,15 @@
             user_code_service = context.node.get_service("usercodeservice")
 
         input_policy = code_item.get_input_policy(context)
         output_policy = code_item.get_output_policy(context)
 
         if not override_execution_permission:
             if input_policy is None:
-                if not code_item.output_policy_approved:
+                if not code_item.is_output_policy_approved(context):
                     return Err("Execution denied: Your code is waiting for approval")
                 return Err(f"No input policy defined for user code: {code_item.id}")
 
             # Filter input kwargs based on policy
             filtered_kwargs = input_policy.filter_kwargs(
                 kwargs=kwargs, context=context, code_item_id=code_item.id
             )
```

### Comparing `syft-0.8.7b1/src/syft/service/action/action_store.py` & `syft-0.8.7b2/src/syft/service/action/action_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,14 +265,19 @@
         permissions.remove(permission.permission_string)
         self.permissions[permission.uid] = permissions
 
     def add_permissions(self, permissions: list[ActionObjectPermission]) -> None:
         for permission in permissions:
             self.add_permission(permission)
 
+    def _get_permissions_for_uid(self, uid: UID) -> Result[set[str], str]:
+        if uid in self.permissions:
+            return Ok(self.permissions[uid])
+        return Err(f"No permissions found for uid: {uid}")
+
     def add_storage_permission(self, permission: StoragePermission) -> None:
         permissions = self.storage_permissions[permission.uid]
         permissions.add(permission.node_uid)
         self.storage_permissions[permission.uid] = permissions
 
     def add_storage_permissions(self, permissions: list[StoragePermission]) -> None:
         for permission in permissions:
@@ -287,14 +292,19 @@
         if isinstance(permission, UID):
             permission = StoragePermission(uid=permission, node_uid=self.node_uid)
 
         if permission.uid in self.storage_permissions:
             return permission.node_uid in self.storage_permissions[permission.uid]
         return False
 
+    def _get_storage_permissions_for_uid(self, uid: UID) -> Result[set[UID], str]:
+        if uid in self.storage_permissions:
+            return Ok(self.storage_permissions[uid])
+        return Err(f"No storage permissions found for uid: {uid}")
+
     def migrate_data(
         self, to_klass: SyftObject, credentials: SyftVerifyKey
     ) -> Result[bool, str]:
         has_root_permission = credentials == self.root_verify_key
 
         if has_root_permission:
             for key, value in self.data.items():
```

### Comparing `syft-0.8.7b1/src/syft/service/action/action_types.py` & `syft-0.8.7b2/src/syft/service/action/action_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,25 +11,23 @@
 def action_type_for_type(obj_or_type: Any) -> type:
     """Convert standard type to Syft types
 
     Parameters:
         obj_or_type: Union[object, type]
             Can be an object or a class
     """
+    if isinstance(obj_or_type, ActionDataEmpty):
+        obj_or_type = obj_or_type.syft_internal_type
     if type(obj_or_type) != type:
-        if isinstance(obj_or_type, ActionDataEmpty):
-            obj_or_type = obj_or_type.syft_internal_type
-        else:
-            obj_or_type = type(obj_or_type)
+        obj_or_type = type(obj_or_type)
 
     if obj_or_type not in action_types:
         debug(f"WARNING: No Type for {obj_or_type}, returning {action_types[Any]}")
-        return action_types[Any]
 
-    return action_types[obj_or_type]
+    return action_types.get(obj_or_type, action_types[Any])
 
 
 def action_type_for_object(obj: Any) -> type:
     """Convert standard type to Syft types
 
     Parameters:
         obj_or_type: Union[object, type]
```

### Comparing `syft-0.8.7b1/src/syft/service/action/numpy.py` & `syft-0.8.7b2/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/action/pandas.py` & `syft-0.8.7b2/src/syft/service/action/pandas.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,19 @@
 
     def syft_is_property(self, obj: Any, method: str) -> bool:
         cols = self.syft_action_data.columns.values.tolist()
         if method in cols:
             return True
         return super().syft_is_property(obj, method)
 
+    def __bool__(self) -> bool:
+        if self.syft_action_data_cache is None:
+            return False
+        return bool(self.syft_action_data_cache.empty)
+
 
 @serializable()
 class PandasSeriesObject(ActionObject):
     __canonical_name__ = "PandasSeriesObject"
     __version__ = SYFT_OBJECT_VERSION_3
 
     syft_internal_type = Series
```

### Comparing `syft-0.8.7b1/src/syft/service/action/plan.py` & `syft-0.8.7b2/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/action/verification.py` & `syft-0.8.7b2/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/api/api.py` & `syft-0.8.7b2/src/syft/service/api/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # stdlib
 import ast
 from collections.abc import Callable
 import inspect
 from inspect import Signature
 import keyword
 import re
+import textwrap
 from typing import Any
 from typing import cast
 
 # third party
 from pydantic import ValidationError
 from pydantic import field_validator
 from pydantic import model_validator
@@ -19,17 +20,20 @@
 # relative
 from ...abstract_node import AbstractNode
 from ...serde.serializable import serializable
 from ...serde.signature import signature_remove_context
 from ...types.syft_object import PartialSyftObject
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SyftObject
+from ...types.syncable_object import SyncableSyftObject
 from ...types.transforms import TransformContext
+from ...types.transforms import generate_action_object_id
 from ...types.transforms import generate_id
 from ...types.transforms import transform
+from ...types.uid import UID
 from ..context import AuthedServiceContext
 from ..response import SyftError
 
 NOT_ACCESSIBLE_STRING = "N / A"
 
 
 class HelperFunctionSet:
@@ -57,14 +61,15 @@
 @serializable()
 class TwinAPIEndpointView(SyftObject):
     # version
     __canonical_name__ = "CustomAPIView"
     __version__ = SYFT_OBJECT_VERSION_1
 
     path: str
+    action_object_id: UID
     signature: Signature
     access: str = "Public"
     mock_function: str | None = None
     private_function: str | None = None
     description: str | None = None
     mock_helper_functions: list[str] | None = None
     private_helper_functions: list[str] | None = None
@@ -109,14 +114,24 @@
     func_name: str
     settings: dict[str, Any] | None = None
     view_access: bool = True
     helper_functions: dict[str, str] | None = None
     state: dict[Any, Any] | None = None
     signature: Signature
 
+    __exclude_sync_diff_attrs__ = ["state"]
+
+    def __repr__(self) -> str:
+        type_name = type(self).__name__
+        repr_str = f"""<{type_name}: {self.func_name}>
+
+        {self.api_code}
+        """
+        return textwrap.dedent(repr_str)
+
     @field_validator("api_code", check_fields=False)
     @classmethod
     def validate_api_code(cls, api_code: str) -> str:
         valid_code = True
         try:
             ast.parse(api_code)
         except SyntaxError:
@@ -230,30 +245,40 @@
     private_function: PrivateAPIEndpoint | None = None
     mock_function: PublicAPIEndpoint
     signature: Signature
     description: str | None = None
 
 
 @serializable()
-class TwinAPIEndpoint(SyftObject):
+class TwinAPIEndpoint(SyncableSyftObject):
     # version
     __canonical_name__ = "TwinAPIEndpoint"
     __version__ = SYFT_OBJECT_VERSION_1
 
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(**kwargs)
 
     path: str
     private_function: PrivateAPIEndpoint | None = None
     mock_function: PublicAPIEndpoint
     signature: Signature
     description: str | None = None
+    action_object_id: UID
+    __private_sync_attr_mocks__ = {
+        "private_function": None,
+    }
 
     __attr_searchable__ = ["path"]
     __attr_unique__ = ["path"]
+    __repr_attrs__ = [
+        "path",
+        "description",
+        "private_function",
+        "mock_function",
+    ]
 
     def has_mock(self) -> bool:
         return self.api_mock_code is not None
 
     def has_permission(self, context: AuthedServiceContext) -> bool:
         """Check if the user has permission to access the endpoint.
 
@@ -457,15 +482,15 @@
         return context
 
     return code_string
 
 
 @transform(CreateTwinAPIEndpoint, TwinAPIEndpoint)
 def endpoint_create_to_twin_endpoint() -> list[Callable]:
-    return [generate_id, check_and_cleanup_signature]
+    return [generate_id, generate_action_object_id, check_and_cleanup_signature]
 
 
 @transform(TwinAPIEndpoint, TwinAPIEndpointView)
 def twin_endpoint_to_view() -> list[Callable]:
     return [
         set_access_type,
         extract_code_string("private_function"),
```

### Comparing `syft-0.8.7b1/src/syft/service/api/api_service.py` & `syft-0.8.7b2/src/syft/service/api/api_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ...store.document_store import DocumentStore
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..context import AuthedServiceContext
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..service import AbstractService
+from ..service import TYPE_TO_SERVICE
 from ..service import service_method
 from ..user.user_roles import ADMIN_ROLE_LEVEL
 from ..user.user_roles import DATA_SCIENTIST_ROLE_LEVEL
 from ..user.user_roles import GUEST_ROLE_LEVEL
 from .api import CreateTwinAPIEndpoint
 from .api import PrivateAPIEndpoint
 from .api import PublicAPIEndpoint
@@ -40,19 +41,26 @@
 
     @service_method(
         path="api.add",
         name="add",
         roles=ADMIN_ROLE_LEVEL,
     )
     def set(
-        self, context: AuthedServiceContext, endpoint: CreateTwinAPIEndpoint
+        self,
+        context: AuthedServiceContext,
+        endpoint: CreateTwinAPIEndpoint | TwinAPIEndpoint,
     ) -> SyftSuccess | SyftError:
         """Register an CustomAPIEndpoint."""
         try:
-            new_endpoint = endpoint.to(TwinAPIEndpoint)
+            if isinstance(endpoint, CreateTwinAPIEndpoint):  # type: ignore
+                new_endpoint = endpoint.to(TwinAPIEndpoint)
+            elif isinstance(endpoint, TwinAPIEndpoint):  # type: ignore
+                new_endpoint = endpoint
+            else:
+                return SyftError(message="Invalid endpoint type.")
         except ValueError as e:
             return SyftError(message=str(e))
 
         endpoint_exists = self.stash.path_exists(context.credentials, new_endpoint.path)
 
         if endpoint_exists.is_err():
             return SyftError(message=endpoint_exists.err())
@@ -64,15 +72,15 @@
 
         result = self.stash.upsert(context.credentials, endpoint=new_endpoint)
         if result.is_err():
             return SyftError(message=result.err())
 
         result = result.ok()
         action_obj = ActionObject.from_obj(
-            id=result.id,
+            id=new_endpoint.action_object_id,
             syft_action_data=CustomEndpointActionObject(endpoint_id=result.id),
             syft_node_location=context.node.id,
             syft_client_verify_key=context.credentials,
         )
         action_service = context.node.get_service("actionservice")
         res = action_service.set(context=context, action_object=action_obj)
         if res.is_err():
@@ -209,14 +217,25 @@
         for api_endpoint in all_api_endpoints:
             api_endpoint_view.append(
                 api_endpoint.to(TwinAPIEndpointView, context=context)
             )
 
         return api_endpoint_view
 
+    @service_method(path="api.get_all", name="get_all", roles=ADMIN_ROLE_LEVEL)
+    def get_all(
+        self,
+        context: AuthedServiceContext,
+    ) -> list[TwinAPIEndpoint] | SyftError:
+        """Get all API endpoints."""
+        result = self.stash.get_all(context.credentials)
+        if result.is_ok():
+            return result.ok()
+        return SyftError(message=result.err())
+
     @service_method(path="api.call", name="call", roles=GUEST_ROLE_LEVEL)
     def call(
         self,
         context: AuthedServiceContext,
         path: str,
         *args: Any,
         **kwargs: Any,
@@ -353,7 +372,10 @@
                 message=f"CustomAPIEndpoint: {endpoint_path} does not exist"
             )
 
         if result.is_ok():
             return result.ok()
 
         return SyftError(message=f"Unable to get {endpoint_path} CustomAPIEndpoint")
+
+
+TYPE_TO_SERVICE[TwinAPIEndpoint] = APIService
```

### Comparing `syft-0.8.7b1/src/syft/service/api/api_stash.py` & `syft-0.8.7b2/src/syft/service/api/api_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/blob_storage/remote_profile.py` & `syft-0.8.7b2/src/syft/service/blob_storage/remote_profile.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/blob_storage/service.py` & `syft-0.8.7b2/src/syft/service/blob_storage/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/blob_storage/stash.py` & `syft-0.8.7b2/src/syft/service/blob_storage/stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/code/code_parse.py` & `syft-0.8.7b2/src/syft/service/code/code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/code/status_service.py` & `syft-0.8.7b2/src/syft/service/code/status_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/code/user_code.py` & `syft-0.8.7b2/src/syft/service/code/user_code.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/code/user_code_parse.py` & `syft-0.8.7b2/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/code/user_code_service.py` & `syft-0.8.7b2/src/syft/service/code/user_code_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,15 +380,17 @@
             ):
                 mock_kwargs[k] = v
         return mock_kwargs
 
     def is_execution_on_owned_args(
         self, kwargs: dict[str, Any], context: AuthedServiceContext
     ) -> bool:
-        return len(self.keep_owned_kwargs(kwargs, context)) == len(kwargs)
+        return bool(kwargs) and len(self.keep_owned_kwargs(kwargs, context)) == len(
+            kwargs
+        )
 
     @service_method(path="code.call", name="call", roles=GUEST_ROLE_LEVEL)
     def call(
         self, context: AuthedServiceContext, uid: UID, **kwargs: Any
     ) -> CachedSyftObject | ActionObject | SyftSuccess | SyftError:
         """Call a User Code Function"""
         kwargs.pop("result_id", None)
```

### Comparing `syft-0.8.7b1/src/syft/service/code/user_code_stash.py` & `syft-0.8.7b2/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/code/utils.py` & `syft-0.8.7b2/src/syft/service/code/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/code_history/code_history.py` & `syft-0.8.7b2/src/syft/service/code_history/code_history.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/code_history/code_history_service.py` & `syft-0.8.7b2/src/syft/service/code_history/code_history_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/code_history/code_history_stash.py` & `syft-0.8.7b2/src/syft/service/code_history/code_history_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/context.py` & `syft-0.8.7b2/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/data_subject/data_subject.py` & `syft-0.8.7b2/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.7b2/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.7b2/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.7b2/src/syft/service/data_subject/data_subject_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,28 +70,36 @@
     ) -> SyftSuccess | SyftError:
         """Register a data subject."""
 
         member_relationship_add = context.node.get_service_method(
             DataSubjectMemberService.add
         )
 
-        member_relationships = data_subject.member_relationships
-        for member_relationship in member_relationships:
-            parent_ds, child_ds = member_relationship
-            for ds in [parent_ds, child_ds]:
-                result = self.stash.set(
-                    context.credentials,
-                    ds.to(DataSubject, context=context),
-                    ignore_duplicates=True,
-                )
-                if result.is_err():
-                    return SyftError(message=str(result.err()))
-            result = member_relationship_add(context, parent_ds.name, child_ds.name)
-            if isinstance(result, SyftError):
-                return result
+        member_relationships: set[tuple[str, str]] = data_subject.member_relationships
+        if len(member_relationships) == 0:
+            result = self.stash.set(
+                context.credentials,
+                data_subject.to(DataSubject, context=context),
+            )
+            if result.is_err():
+                return SyftError(message=str(result.err()))
+        else:
+            for member_relationship in member_relationships:
+                parent_ds, child_ds = member_relationship
+                for ds in [parent_ds, child_ds]:
+                    result = self.stash.set(
+                        context.credentials,
+                        ds.to(DataSubject, context=context),
+                        ignore_duplicates=True,
+                    )
+                    if result.is_err():
+                        return SyftError(message=str(result.err()))
+                result = member_relationship_add(context, parent_ds.name, child_ds.name)
+                if isinstance(result, SyftError):
+                    return result
 
         return SyftSuccess(
             message=f"{len(member_relationships)+1} Data Subjects Registered"
         )
 
     @service_method(path="data_subject.get_all", name="get_all")
     def get_all(self, context: AuthedServiceContext) -> list[DataSubject] | SyftError:
```

### Comparing `syft-0.8.7b1/src/syft/service/dataset/dataset.py` & `syft-0.8.7b2/src/syft/service/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/dataset/dataset_service.py` & `syft-0.8.7b2/src/syft/service/dataset/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.7b2/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/enclave/enclave_service.py` & `syft-0.8.7b2/src/syft/service/enclave/enclave_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/job/job_service.py` & `syft-0.8.7b2/src/syft/service/job/job_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/job/job_stash.py` & `syft-0.8.7b2/src/syft/service/job/job_stash.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 from ...types.syncable_object import SyncableSyftObject
 from ...types.uid import UID
 from ...util import options
 from ...util.colors import SURFACE
 from ...util.markdown import as_markdown_code
 from ...util.telemetry import instrument
 from ...util.util import prompt_warning_message
-from ..action.action_data_empty import ActionDataLink
 from ..action.action_object import Action
 from ..action.action_object import ActionObject
 from ..action.action_permissions import ActionObjectPermission
 from ..response import SyftError
 from ..response import SyftNotReady
 from ..response import SyftSuccess
 from ..user.user import UserView
@@ -82,15 +81,15 @@
         "id",
         "result",
         "resolved",
         "progress",
         "creation_time",
         "user_code_name",
     ]
-    __exclude_sync_diff_attrs__ = ["action"]
+    __exclude_sync_diff_attrs__ = ["action", "node_uid"]
 
     @field_validator("creation_time")
     @classmethod
     def check_time(cls, time: Any) -> Any:
         return str(datetime.now()) if time is None else time
 
     @model_validator(mode="after")
@@ -322,14 +321,18 @@
         )
         if api is None:
             return SyftError(
                 message=f"Can't access Syft API. You must login to {self.syft_node_location}"
             )
         return api.services.job.get_subjobs(self.id)
 
+    def get_subjobs(self, context: AuthedServiceContext) -> list["Job"] | SyftError:
+        job_service = context.node.get_service("jobservice")
+        return job_service.get_subjobs(context, self.id)
+
     @property
     def owner(self) -> UserView | SyftError:
         api = APIRegistry.api_for(
             node_uid=self.syft_node_location,
             user_verify_key=self.syft_client_verify_key,
         )
         if api is None:
@@ -479,15 +482,15 @@
         counter = 0
         while True:
             self.fetch()
             if print_warning and self.result is not None:
                 result_obj = api.services.action.get(
                     self.result.id, resolve_nested=False
                 )
-                if isinstance(result_obj.syft_action_data, ActionDataLink) and job_only:
+                if result_obj.is_link and job_only:
                     print(
                         "You're trying to wait on a job that has a link as a result."
                         "This means that the job may be ready but the linked result may not."
                         "Use job.wait().get() instead to wait for the linked result."
                     )
                     print_warning = False
             sleep(1)
@@ -513,19 +516,19 @@
         dependencies = []
         if self.result is not None:
             dependencies.append(self.result.id.id)
 
         if self.log_id:
             dependencies.append(self.log_id)
 
-        subjobs = self.subjobs
+        subjobs = self.get_subjobs(context)
         if isinstance(subjobs, SyftError):
             return subjobs
 
-        subjob_ids = [subjob.id for subjob in self.subjobs]
+        subjob_ids = [subjob.id for subjob in subjobs]
         dependencies.extend(subjob_ids)
 
         if self.user_code_id is not None:
             dependencies.append(self.user_code_id)
 
         output = context.node.get_service("outputservice").get_by_job_id(  # type: ignore
             context, self.id
```

### Comparing `syft-0.8.7b1/src/syft/service/log/log.py` & `syft-0.8.7b2/src/syft/service/log/log.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/log/log_service.py` & `syft-0.8.7b2/src/syft/service/log/log_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/log/log_stash.py` & `syft-0.8.7b2/src/syft/service/log/log_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/metadata/metadata_service.py` & `syft-0.8.7b2/src/syft/service/metadata/metadata_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/metadata/migrations.py` & `syft-0.8.7b2/src/syft/service/metadata/migrations.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/metadata/node_metadata.py` & `syft-0.8.7b2/src/syft/service/metadata/node_metadata.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/network/node_peer.py` & `syft-0.8.7b2/src/syft/service/network/routes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,162 +1,204 @@
+# future
+from __future__ import annotations
+
 # stdlib
+import secrets
+from typing import Any
+from typing import TYPE_CHECKING
+
+# third party
+from typing_extensions import Self
 
 # relative
-from ...abstract_node import NodeType
+from ...abstract_node import AbstractNode
+from ...client.client import HTTPConnection
+from ...client.client import NodeConnection
+from ...client.client import PythonConnection
 from ...client.client import SyftClient
-from ...node.credentials import SyftSigningKey
-from ...node.credentials import SyftVerifyKey
+from ...node.worker_settings import WorkerSettings
 from ...serde.serializable import serializable
-from ...service.response import SyftError
+from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SYFT_OBJECT_VERSION_2
 from ...types.syft_object import SyftObject
+from ...types.transforms import TransformContext
 from ...types.uid import UID
+from ..context import AuthedServiceContext
 from ..context import NodeServiceContext
-from ..metadata.node_metadata import NodeMetadataV3
-from .routes import HTTPNodeRoute
-from .routes import NodeRoute
-from .routes import NodeRouteType
-from .routes import PythonNodeRoute
-from .routes import VeilidNodeRoute
-from .routes import connection_to_route
-from .routes import route_to_connection
+from ..response import SyftError
 
+if TYPE_CHECKING:
+    # relative
+    from .node_peer import NodePeer
 
-@serializable()
-class NodePeer(SyftObject):
-    # version
-    __canonical_name__ = "NodePeer"
-    __version__ = SYFT_OBJECT_VERSION_2
 
-    __attr_searchable__ = ["name", "node_type"]
-    __attr_unique__ = ["verify_key"]
-    __repr_attrs__ = ["name", "node_type", "admin_email"]
-
-    id: UID | None = None  # type: ignore[assignment]
-    name: str
-    verify_key: SyftVerifyKey
-    node_routes: list[NodeRouteType] = []
-    node_type: NodeType
-    admin_email: str
-
-    def update_routes(self, new_routes: list[NodeRoute]) -> None:
-        add_routes = []
-        new_routes = self.update_route_priorities(new_routes)
-        for new_route in new_routes:
-            existed, index = self.existed_route(new_route)
-            if existed and index is not None:
-                # if the route already exists, we do not append it to self.new_route,
-                # but update its priority
-                self.node_routes[index].priority = new_route.priority
-            else:
-                add_routes.append(new_route)
-
-        self.node_routes += add_routes
-
-    def update_route_priorities(self, new_routes: list[NodeRoute]) -> list[NodeRoute]:
-        """
-        Since we pick the newest route has the highest priority, we
-        update the priority of the newly added routes here to be increments of
-        current routes' highest priority.
+class NodeRoute:
+    def client_with_context(
+        self, context: NodeServiceContext
+    ) -> SyftClient | SyftError:
         """
-        current_max_priority = max(route.priority for route in self.node_routes)
-        for route in new_routes:
-            route.priority = current_max_priority + 1
-            current_max_priority += 1
-        return new_routes
-
-    def existed_route(self, route: NodeRoute) -> tuple[bool, int | None]:
-        """Check if a route exists in self.node_routes
-        - For HTTPNodeRoute: check based on protocol, host_or_ip (url) and port
-        - For PythonNodeRoute: check if the route exists in the set of all node_routes
+        Convert the current route (self) to a connection (either HTTP, Veilid or Python)
+        and create a SyftClient from the connection.
+
         Args:
-            route: the route to be checked
+            context (NodeServiceContext): The NodeServiceContext containing the node information.
+
         Returns:
-            if the route exists, returns (True, index of the existed route in self.node_routes)
-            if the route does not exist returns (False, None)
+            SyftClient | SyftError: Returns the created SyftClient, or SyftError
+                if the client type is not valid or if the context's node is None.
         """
-        if isinstance(route, HTTPNodeRoute):
-            for i, r in enumerate(self.node_routes):
-                if (
-                    (route.host_or_ip == r.host_or_ip)
-                    and (route.port == r.port)
-                    and (route.protocol == r.protocol)
-                ):
-                    return (True, i)
-            return (False, None)
-        elif isinstance(route, PythonNodeRoute):  # PythonNodeRoute
-            for i, r in enumerate(self.node_routes):  # something went wrong here
-                if (
-                    (route.worker_settings.id == r.worker_settings.id)
-                    and (route.worker_settings.name == r.worker_settings.name)
-                    and (route.worker_settings.node_type == r.worker_settings.node_type)
-                    and (
-                        route.worker_settings.node_side_type
-                        == r.worker_settings.node_side_type
-                    )
-                    and (
-                        route.worker_settings.signing_key
-                        == r.worker_settings.signing_key
-                    )
-                ):
-                    return (True, i)
-            return (False, None)
-        elif isinstance(route, VeilidNodeRoute):
-            for i, r in enumerate(self.node_routes):
-                if (
-                    route.vld_key == r.vld_key
-                    and route.proxy_target_uid == r.proxy_target_uid
-                ):
-                    return (True, i)
-
-            return (False, None)
-        else:
-            raise ValueError(f"Unsupported route type: {type(route)}")
-
-    @staticmethod
-    def from_client(client: SyftClient) -> "NodePeer":
-        if not client.metadata:
-            raise Exception("Client has to have metadata first")
-
-        peer = client.metadata.to(NodeMetadataV3).to(NodePeer)
-        route = connection_to_route(client.connection)
-        peer.node_routes.append(route)
-        return peer
-
-    def client_with_context(self, context: NodeServiceContext) -> SyftClient:
-        if len(self.node_routes) < 1:
-            raise Exception(f"No routes to peer: {self}")
-        # select the latest added route
-        final_route = self.pick_highest_priority_route()
-        connection = route_to_connection(route=final_route)
-
+        connection = route_to_connection(route=self, context=context)
         client_type = connection.get_client_type()
         if isinstance(client_type, SyftError):
             return client_type
         return client_type(connection=connection, credentials=context.node.signing_key)
 
-    def client_with_key(self, credentials: SyftSigningKey) -> SyftClient:
-        if len(self.node_routes) < 1:
-            raise Exception(f"No routes to peer: {self}")
-        # select the latest added route
-        final_route = self.pick_highest_priority_route()
-        connection = route_to_connection(route=final_route)
-        client_type = connection.get_client_type()
-        if isinstance(client_type, SyftError):
-            return client_type
+    def validate_with_context(
+        self, context: AuthedServiceContext
+    ) -> NodePeer | SyftError:
+        # relative
+        from .node_peer import NodePeer
+
+        # Step 1: Check if the given route is able to reach the given node
+        # As we allow the user to give custom routes, we need to check the reachability of the route
+        self_client = self.client_with_context(context=context)
+
+        # generating a random challenge
+        random_challenge = secrets.token_bytes(16)
+        challenge_signature = self_client.api.services.network.ping(random_challenge)
+
+        if isinstance(challenge_signature, SyftError):
+            return challenge_signature
+
+        try:
+            # Verifying if the challenge is valid
+            context.node.verify_key.verify_key.verify(
+                random_challenge, challenge_signature
+            )
+        except Exception:
+            return SyftError(message="Signature Verification Failed in ping")
+
+        # Step 2: Create a Node Peer with the given route
+        self_node_peer: NodePeer = context.node.settings.to(NodePeer)
+        self_node_peer.node_routes.append(self)
+
+        return self_node_peer
 
-        return client_type(connection=connection, credentials=credentials)
+
+@serializable()
+class HTTPNodeRoute(SyftObject, NodeRoute):
+    __canonical_name__ = "HTTPNodeRoute"
+    __version__ = SYFT_OBJECT_VERSION_2
+
+    host_or_ip: str
+    private: bool = False
+    protocol: str = "http"
+    port: int = 80
+    proxy_target_uid: UID | None = None
+    priority: int = 1
+
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, HTTPNodeRoute):
+            return False
+        return hash(self) == hash(other)
+
+    def __hash__(self) -> int:
+        return (
+            hash(self.host_or_ip)
+            + hash(self.port)
+            + hash(self.protocol)
+            + hash(self.proxy_target_uid)
+        )
+
+    def __str__(self) -> str:
+        return f"{self.protocol}://{self.host_or_ip}:{self.port}"
+
+
+@serializable()
+class PythonNodeRoute(SyftObject, NodeRoute):
+    __canonical_name__ = "PythonNodeRoute"
+    __version__ = SYFT_OBJECT_VERSION_2
+
+    worker_settings: WorkerSettings
+    proxy_target_uid: UID | None = None
+    priority: int = 1
 
     @property
-    def guest_client(self) -> SyftClient:
-        guest_key = SyftSigningKey.generate()
-        return self.client_with_key(credentials=guest_key)
-
-    def proxy_from(self, client: SyftClient) -> SyftClient:
-        return client.proxy_to(self)
-
-    def pick_highest_priority_route(self) -> NodeRoute:
-        final_route: NodeRoute = self.node_routes[-1]
-        for route in self.node_routes:
-            if route.priority > final_route.priority:
-                final_route = route
-        return final_route
+    def node(self) -> AbstractNode | None:
+        # relative
+        from ...node.worker import Worker
+
+        node = Worker(
+            id=self.worker_settings.id,
+            name=self.worker_settings.name,
+            node_type=self.worker_settings.node_type,
+            node_side_type=self.worker_settings.node_side_type,
+            signing_key=self.worker_settings.signing_key,
+            document_store_config=self.worker_settings.document_store_config,
+            action_store_config=self.worker_settings.action_store_config,
+            processes=1,
+        )
+        return node
+
+    @classmethod
+    def with_node(cls, node: AbstractNode) -> Self:
+        worker_settings = WorkerSettings.from_node(node)
+        return cls(id=worker_settings.id, worker_settings=worker_settings)
+
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, PythonNodeRoute):
+            return False
+        return hash(self) == hash(other)
+
+    def __hash__(self) -> int:
+        return (
+            hash(self.worker_settings.id)
+            + hash(self.worker_settings.name)
+            + hash(self.worker_settings.node_type)
+            + hash(self.worker_settings.node_side_type)
+            + hash(self.worker_settings.signing_key)
+        )
+
+    def __str__(self) -> str:
+        return "PythonNodeRoute"
+
+
+@serializable()
+class VeilidNodeRoute(SyftObject, NodeRoute):
+    __canonical_name__ = "VeilidNodeRoute"
+    __version__ = SYFT_OBJECT_VERSION_1
+
+    vld_key: str
+    proxy_target_uid: UID | None = None
+    priority: int = 1
+
+    def __eq__(self, other: Any) -> bool:
+        if not isinstance(other, VeilidNodeRoute):
+            return False
+        return hash(self) == hash(other)
+
+    def __hash__(self) -> int:
+        return hash(self.vld_key) + hash(self.proxy_target_uid)
+
+
+NodeRouteTypeV1 = HTTPNodeRoute | PythonNodeRoute | VeilidNodeRoute
+NodeRouteType = HTTPNodeRoute | PythonNodeRoute
+
+
+def route_to_connection(
+    route: NodeRoute, context: TransformContext | None = None
+) -> NodeConnection:
+    if isinstance(route, HTTPNodeRoute):
+        return route.to(HTTPConnection, context=context)
+    elif isinstance(route, PythonNodeRoute):
+        return route.to(PythonConnection, context=context)
+    else:
+        raise ValueError(f"Route {route} is not supported.")
+
+
+def connection_to_route(connection: NodeConnection) -> NodeRoute:
+    if isinstance(connection, HTTPConnection):
+        return connection.to(HTTPNodeRoute)
+    elif isinstance(connection, PythonConnection):  # type: ignore[unreachable]
+        return connection.to(PythonNodeRoute)
+    else:
+        raise ValueError(f"Connection {connection} is not supported.")
```

### Comparing `syft-0.8.7b1/src/syft/service/notification/email_templates.py` & `syft-0.8.7b2/src/syft/service/notification/email_templates.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/notification/notification_service.py` & `syft-0.8.7b2/src/syft/service/notification/notification_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,15 @@
         if result.is_err():
             return SyftError(message=str(result.err()))
         return result.ok()
 
     @service_method(
         path="notifications.resolve_object",
         name="resolve_object",
-        roles=DATA_SCIENTIST_ROLE_LEVEL,
+        roles=GUEST_ROLE_LEVEL,
     )
     def resolve_object(
         self, context: AuthedServiceContext, linked_obj: LinkedObject
     ) -> Notification | SyftError:
         service = context.node.get_service(linked_obj.service_type)
         result = service.resolve_link(context=context, linked_obj=linked_obj)
         if result.is_err():
```

### Comparing `syft-0.8.7b1/src/syft/service/notification/notification_stash.py` & `syft-0.8.7b2/src/syft/service/notification/notification_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/notification/notifications.py` & `syft-0.8.7b2/src/syft/service/notification/notifications.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/notifier/notifier.py` & `syft-0.8.7b2/src/syft/service/notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/notifier/notifier_service.py` & `syft-0.8.7b2/src/syft/service/notifier/notifier_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/notifier/notifier_stash.py` & `syft-0.8.7b2/src/syft/service/notifier/notifier_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/notifier/smtp_client.py` & `syft-0.8.7b2/src/syft/service/notifier/smtp_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/object_search/migration_state_service.py` & `syft-0.8.7b2/src/syft/service/object_search/migration_state_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/object_search/object_migration_state.py` & `syft-0.8.7b2/src/syft/service/object_search/object_migration_state.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/output/output_service.py` & `syft-0.8.7b2/src/syft/service/output/output_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/policy/policy.py` & `syft-0.8.7b2/src/syft/service/policy/policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     for k, v in kwargs.items():
         uid = v
         if isinstance(v, ActionObject):
             uid = v.id
         if isinstance(v, TwinObject):
             uid = v.id
         if isinstance(v, RemoteFunction):
-            uid = v.custom_function_id()
+            uid = v.custom_function_actionobject_id()
         if isinstance(v, Asset):
             uid = v.action_id
         if not isinstance(uid, UID):
             raise Exception(f"Input {k} must have a UID not {type(v)}")
 
         _obj_exists = False
         for api in api_list:
```

### Comparing `syft-0.8.7b1/src/syft/service/policy/policy_service.py` & `syft-0.8.7b2/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.7b2/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/project/project.py` & `syft-0.8.7b2/src/syft/service/project/project.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/project/project_service.py` & `syft-0.8.7b2/src/syft/service/project/project_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             # They would raise as error
             leader_node = project_obj.state_sync_leader
 
             # If the current node is a follower
             # For followers the leader node route is retrieved from its peer
             if leader_node.verify_key != context.node.verify_key:
                 network_service = context.node.get_service("networkservice")
-                peer = network_service.stash.get_for_verify_key(
+                peer = network_service.stash.get_by_verify_key(
                     credentials=context.node.verify_key,
                     verify_key=leader_node.verify_key,
                 )
                 if peer.is_err():
                     this_node_id = context.node.id.short() if context.node.id else ""
                     return SyftError(
                         message=(
@@ -224,27 +224,36 @@
             return message_result
 
         # Broadcast the event to all the members of the project
         network_service = context.node.get_service("networkservice")
         for member in project.members:
             if member.verify_key != context.node.verify_key:
                 # Retrieving the NodePeer Object to communicate with the node
-                peer = network_service.stash.get_for_verify_key(
+                peer = network_service.stash.get_by_verify_key(
                     credentials=context.node.verify_key,
                     verify_key=member.verify_key,
                 )
 
                 if peer.is_err():
                     return SyftError(
                         message=f"Leader node does not have peer {member.name}-{member.id.short()}"
                         + " Kindly exchange routes with the peer"
                     )
                 peer = peer.ok()
-                client = peer.client_with_context(context)
-                event_result = client.api.services.project.add_event(project_event)
+                remote_client = peer.client_with_context(context=context)
+                if remote_client.is_err():
+                    return SyftError(
+                        message=f"Failed to create remote client for peer: "
+                        f"{peer.id}. Error: {remote_client.err()}"
+                    )
+                remote_client = remote_client.ok()
+
+                event_result = remote_client.api.services.project.add_event(
+                    project_event
+                )
                 if isinstance(event_result, SyftError):
                     return event_result
 
         result = self.stash.update(context.node.verify_key, project)
 
         if result.is_err():
             return SyftError(message=str(result.err()))
```

### Comparing `syft-0.8.7b1/src/syft/service/project/project_stash.py` & `syft-0.8.7b2/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/queue/base_queue.py` & `syft-0.8.7b2/src/syft/service/queue/base_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/queue/queue.py` & `syft-0.8.7b2/src/syft/service/queue/queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/queue/queue_service.py` & `syft-0.8.7b2/src/syft/service/queue/queue_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/queue/queue_stash.py` & `syft-0.8.7b2/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/queue/zmq_queue.py` & `syft-0.8.7b2/src/syft/service/queue/zmq_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/request/request.py` & `syft-0.8.7b2/src/syft/service/request/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -656,15 +656,15 @@
             res = job_service.add_read_permission_log_for_code_owner(
                 job.log_id, self.code
             )
             print(res)
 
         return job
 
-    def _is_action_object_from_job(self, action_object: ActionObject) -> Job | None:  # type: ignore
+    def _get_job_from_action_object(self, action_object: ActionObject) -> Job | None:  # type: ignore
         api = APIRegistry.api_for(self.node_uid, self.syft_client_verify_key)
         if api is None:
             raise ValueError(f"Can't access the api. You must login to {self.node_uid}")
         job_service = api.services.job
         existing_jobs = job_service.get_by_user_code_id(self.code.id)
         for job in existing_jobs:
             if job.result and job.result.id == action_object.id:
@@ -683,21 +683,27 @@
                 return SyftError(
                     message="JobInfo should not include result. Use sync_job instead."
                 )
             result = job_info.result
         elif isinstance(result, ActionObject):
             # Do not allow accepting a result produced by a Job,
             # This can cause an inconsistent Job state
-            if self._is_action_object_from_job(result):
-                action_object_job = self._is_action_object_from_job(result)
-                if action_object_job is not None:
-                    return SyftError(
-                        message=f"This ActionObject is the result of Job {action_object_job.id}, "
-                        f"please use the `Job.info` instead."
-                    )
+            action_object_job = self._get_job_from_action_object(result)
+            if action_object_job is not None:
+                return SyftError(
+                    message=f"This ActionObject is the result of Job {action_object_job.id}, "
+                    f"please use the `Job.info` instead."
+                )
+            else:
+                job_info = JobInfo(
+                    includes_metadata=True,
+                    includes_result=True,
+                    status=JobStatus.COMPLETED,
+                    resolved=True,
+                )
         else:
             # NOTE result is added at the end of function (once ActionObject is created)
             job_info = JobInfo(
                 includes_metadata=True,
                 includes_result=True,
                 status=JobStatus.COMPLETED,
                 resolved=True,
```

### Comparing `syft-0.8.7b1/src/syft/service/request/request_service.py` & `syft-0.8.7b2/src/syft/service/request/request_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/request/request_stash.py` & `syft-0.8.7b2/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/response.py` & `syft-0.8.7b2/src/syft/service/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/service.py` & `syft-0.8.7b2/src/syft/service/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 from ..types.syft_object import attach_attribute_to_syft_object
 from ..types.uid import UID
 from .context import AuthedServiceContext
 from .context import ChangeContext
 from .response import SyftError
 from .user.user_roles import DATA_OWNER_ROLE_LEVEL
 from .user.user_roles import ServiceRole
-from .veilid import VEILID_ENABLED
 from .warnings import APIEndpointWarning
 
 if TYPE_CHECKING:
     # relative
     from ..client.api import APIModule
 
 TYPE_TO_SERVICE: dict = {}
@@ -224,27 +223,22 @@
                 permissions={lib_obj.permissions},
                 is_from_lib=True,
             )
 
             LibConfigRegistry.register(lib_config)
 
 
-# NOTE: Currently we disable adding library enpoints like numpy, torch when veilid is enabled
-# This is because the /api endpoint which return SyftAPI along with the lib enpoints exceeds
-# 2 MB . But veilid has a limit of 32 KB for sending and receiving message.
-# This would be fixed, when chunking is implemented at veilid core.
-if not VEILID_ENABLED:
-    # hacky, prevent circular imports
-    for lib_obj in action_execute_registry_libs.flatten():
-        # # for functions
-        # func_name = func.__name__
-        # # for classes
-        # func_name = path.split(".")[-1]
-        if isinstance(lib_obj, CMPFunction) or isinstance(lib_obj, CMPClass):
-            register_lib_obj(lib_obj)
+# hacky, prevent circular imports
+for lib_obj in action_execute_registry_libs.flatten():
+    # # for functions
+    # func_name = func.__name__
+    # # for classes
+    # func_name = path.split(".")[-1]
+    if isinstance(lib_obj, CMPFunction) or isinstance(lib_obj, CMPClass):
+        register_lib_obj(lib_obj)
 
 
 def deconstruct_param(param: inspect.Parameter) -> dict[str, Any]:
     # Gets the init signature form pydantic object
     param_type = param.annotation
     if not hasattr(param_type, "__signature__"):
         raise Exception(
```

### Comparing `syft-0.8.7b1/src/syft/service/settings/settings.py` & `syft-0.8.7b2/src/syft/service/settings/settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/settings/settings_service.py` & `syft-0.8.7b2/src/syft/service/settings/settings_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/settings/settings_stash.py` & `syft-0.8.7b2/src/syft/service/settings/settings_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/sync/diff_state.py` & `syft-0.8.7b2/src/syft/service/sync/diff_state.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 import html
 import textwrap
 from typing import Any
 from typing import ClassVar
 from typing import Literal
 
 # third party
+import pandas as pd
 from pydantic import model_validator
 from rich import box
 from rich.console import Console
 from rich.console import Group
 from rich.markdown import Markdown
 from rich.padding import Padding
 from rich.panel import Panel
 from typing_extensions import Self
 
 # relative
+from ...client.api import APIRegistry
 from ...client.client import SyftClient
 from ...client.sync_decision import SyncDecision
 from ...client.sync_decision import SyncDirection
 from ...node.credentials import SyftVerifyKey
 from ...types.datetime import DateTime
 from ...types.syft_object import SYFT_OBJECT_VERSION_1
 from ...types.syft_object import SYFT_OBJECT_VERSION_2
@@ -28,28 +30,29 @@
 from ...types.syncable_object import SyncableSyftObject
 from ...types.uid import LineageID
 from ...types.uid import UID
 from ...util import options
 from ...util.colors import SURFACE
 from ...util.fonts import FONT_CSS
 from ...util.fonts import ITABLES_CSS
+from ...util.notebook_ui.components.sync import SyncTableObject
 from ...util.notebook_ui.notebook_addons import ARROW_ICON
 from ..action.action_object import ActionObject
 from ..action.action_permissions import ActionObjectPermission
 from ..action.action_permissions import ActionPermission
 from ..action.action_permissions import StoragePermission
+from ..api.api import TwinAPIEndpoint
 from ..code.user_code import UserCode
 from ..code.user_code import UserCodeStatusCollection
 from ..job.job_stash import Job
 from ..log.log import SyftLog
 from ..output.output_service import ExecutionOutput
 from ..request.request import Request
 from ..response import SyftError
 from .sync_state import SyncState
-from .sync_state import SyncView
 
 sketchy_tab = "‎ " * 4
 
 
 class AttrDiff(SyftObject):
     # version
     __canonical_name__ = "AttrDiff"
@@ -178,14 +181,15 @@
     obj_type: type
     diff_list: list[AttrDiff] = []
 
     __repr_attrs__ = [
         "low_state",
         "high_state",
     ]
+    __syft_include_id_coll_repr__ = False
 
     def is_mock(self, side: str) -> bool:
         # An object is a mock object if it exists on both sides,
         # and has no storage permissions on `side`
         # NOTE both sides must have the objects, else it is a new object.
         # New+mock objects do not appear naturally, but if they do we
         # want them to show up.
@@ -319,14 +323,22 @@
         res = {}
         for attr in all_attrs:
             value_low = low_attrs.get(attr, None)
             value_high = high_attrs.get(attr, None)
 
             if value_low is None or value_high is None:
                 res[attr] = DiffStatus.NEW
+            elif isinstance(value_low, pd.DataFrame) and isinstance(
+                value_high, pd.DataFrame
+            ):
+                res[attr] = (
+                    DiffStatus.MODIFIED
+                    if not value_low.equals(value_high)
+                    else DiffStatus.SAME
+                )
             elif value_low != value_high:
                 res[attr] = DiffStatus.MODIFIED
             else:
                 res[attr] = DiffStatus.SAME
         return res
 
     def repr_attr_dict(self, side: str) -> dict[str, Any]:
@@ -571,22 +583,60 @@
             raise ValueError("no direction specified")
         if self.sync_direction == SyncDirection.LOW_TO_HIGH:
             return self.high_node_uid
         else:
             return self.low_node_uid
 
     @property
+    def source_node_uid(self) -> UID:
+        if self.sync_direction is None:
+            raise ValueError("no direction specified")
+        if self.sync_direction == SyncDirection.LOW_TO_HIGH:
+            return self.low_node_uid
+        else:
+            return self.high_node_uid
+
+    @property
     def target_verify_key(self) -> SyftVerifyKey:
         if self.sync_direction is None:
             raise ValueError("no direction specified")
         if self.sync_direction == SyncDirection.LOW_TO_HIGH:
             return self.user_verify_key_high
         else:
             return self.user_verify_key_low
 
+    @property
+    def source_verify_key(self) -> SyftVerifyKey:
+        if self.sync_direction is None:
+            raise ValueError("no direction specified")
+        if self.sync_direction == SyncDirection.LOW_TO_HIGH:
+            return self.user_verify_key_low
+        else:
+            return self.user_verify_key_high
+
+    @property
+    def source_client(self) -> SyftClient:
+        return self.build(self.source_node_uid, self.source_verify_key)
+
+    @property
+    def target_client(self) -> SyftClient:
+        return self.build(self.target_node_uid, self.target_verify_key)
+
+    def build(self, node_uid: UID, syft_client_verify_key: SyftVerifyKey):  # type: ignore
+        # relative
+        from ...client.domain_client import DomainClient
+
+        api = APIRegistry.api_for(node_uid, syft_client_verify_key)
+        client = DomainClient(
+            api=api,
+            connection=api.connection,  # type: ignore
+            credentials=api.signing_key,  # type: ignore
+        )
+        return client
+
     def get_dependencies(
         self,
         include_roots: bool = False,
         include_batch_root: bool = True,
     ) -> list[ObjectDiff]:
         return self.walk_graph(
             deps=self.dependencies,
@@ -738,20 +788,20 @@
         return {"value": status.upper(), "type": badge_color}
 
     def _coll_repr_(self) -> dict[str, Any]:
         no_obj_html = "<p class='diff-state-no-obj'>No object detected</p>"
         if self.root_diff.low_obj is None:
             low_html = no_obj_html
         else:
-            low_html = SyncView(object=self.root_diff.low_obj).summary_html()
+            low_html = SyncTableObject(object=self.root_diff.low_obj).to_html()
 
         if self.root_diff.high_obj is None:
             high_html = no_obj_html
         else:
-            high_html = SyncView(object=self.root_diff.high_obj).summary_html()
+            high_html = SyncTableObject(object=self.root_diff.high_obj).to_html()
 
         return {
             "Merge status": self.status_badge(),
             "Public Sync State": low_html,
             "Private sync state": high_html,
         }
 
@@ -771,14 +821,18 @@
             }
         elif isinstance(root_obj, Job):
             return UserCode, {  # type: ignore
                 UserCode: [ExecutionOutput, UserCode],
                 ExecutionOutput: [Job],
                 Job: [ActionObject, SyftLog, Job],
             }
+        elif isinstance(root_obj, TwinAPIEndpoint):
+            return TwinAPIEndpoint, {  # type: ignore
+                TwinAPIEndpoint: [],
+            }
         else:
             raise ValueError(f"Unknown root type: {self.root.obj_type}")
 
     @model_validator(mode="after")
     def make_dependents(self) -> Self:
         dependents: dict = {}
         for parent, children in self.dependencies.items():
@@ -1103,15 +1157,16 @@
         <p style="margin-bottom:16px;"></p>
         <div class="diff-state-header"><span>{name1}</span> {ARROW_ICON} <span>{name2}</span></div>
         <p style="margin-bottom:16px;"></p>
         <div class="diff-state-sub-header"> This would sync <span class="diff-state-orange-text">{n} batches</span> from <i>{name1}</i> to <i>{name2}</i></div>
         """  # noqa: E501
         repr_html = repr_html.replace("\n", "")
 
-        return repr_html + self.batches._repr_html_()
+        res = repr_html + self.batches._repr_html_()
+        return res
 
     @staticmethod
     def _sort_batches(hierarchies: list[ObjectDiffBatch]) -> list[ObjectDiffBatch]:
         without_usercode = []
         grouped_by_usercode: dict[UID, list[ObjectDiffBatch]] = {}
         for hierarchy in hierarchies:
             has_usercode = False
@@ -1154,20 +1209,19 @@
         direction: SyncDirection,
     ) -> list[ObjectDiffBatch]:
         batches = []
         root_ids = []
 
         for diff in obj_uid_to_diff.values():
             diff_obj = diff.low_obj if diff.low_obj is not None else diff.high_obj
-            if isinstance(diff_obj, Request):
-                root_ids.append(diff.object_id)
-            elif isinstance(diff_obj, Job) and diff_obj.parent_job_id is None:  # type: ignore
-                root_ids.append(diff.object_id)  # type: ignore
-            elif isinstance(diff_obj, UserCode):
+            if isinstance(diff_obj, Request | UserCode | TwinAPIEndpoint):
                 # TODO: Figure out nested user codes, do we even need that?
+
+                root_ids.append(diff.object_id)  # type: ignore
+            elif isinstance(diff_obj, Job) and diff_obj.parent_job_id is None:  # type: ignore
                 root_ids.append(diff.object_id)  # type: ignore
 
         for root_uid in root_ids:
             batch = ObjectDiffBatch.from_dependencies(
                 root_uid,
                 obj_dependencies,
                 obj_uid_to_diff,
@@ -1212,25 +1266,27 @@
         diff = widget.diff
         new_permissions_low_side = []
 
         # read permissions
         if sync_direction == SyncDirection.HIGH_TO_LOW:
             if widget.share_private_data or diff.object_type == "Job":
                 if share_to_user is None:
-                    raise ValueError("empty to user to share with")
-                new_permissions_low_side = [
-                    ActionObjectPermission(
-                        uid=widget.diff.object_id,
-                        permission=ActionPermission.READ,
-                        credentials=share_to_user,  # type: ignore
-                    )
-                ]
+                    raise ValueError("share_to_user is required for private data")
+                else:
+                    new_permissions_low_side = [
+                        ActionObjectPermission(
+                            uid=widget.diff.object_id,
+                            permission=ActionPermission.READ,
+                            credentials=share_to_user,  # type: ignore
+                        )
+                    ]
 
-        # mockify
         mockify = widget.mockify
+        if widget.has_unused_share_button:
+            print("Share button was not used, so we will mockify the object")
 
         # storage permissions
         new_storage_permissions = []
 
         if sync_direction == SyncDirection.HIGH_TO_LOW:
             # TODO: apply storage permissions on both ends
             if not mockify:
```

### Comparing `syft-0.8.7b1/src/syft/service/sync/resolve_widget.py` & `syft-0.8.7b2/src/syft/service/sync/resolve_widget.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 # stdlib
 from enum import Enum
 from enum import auto
 import html
-import json
 from typing import Any
+from uuid import uuid4
 
 # third party
-from IPython.display import Javascript
-from IPython.display import display
 import ipywidgets as widgets
 from ipywidgets import Button
+from ipywidgets import Checkbox
 from ipywidgets import HBox
 from ipywidgets import HTML
 from ipywidgets import Layout
 from ipywidgets import VBox
-from typing_extensions import Self
 
 # relative
-from ...client.api import APIRegistry
 from ...client.sync_decision import SyncDecision
 from ...client.sync_decision import SyncDirection
 from ...node.credentials import SyftVerifyKey
 from ...types.uid import UID
+from ...util.notebook_ui.components.sync import Badge
+from ...util.notebook_ui.components.sync import CopyIDButton
+from ...util.notebook_ui.components.sync import MainDescription
+from ...util.notebook_ui.components.sync import SyncWidgetHeader
 from ...util.notebook_ui.notebook_addons import CSS_CODE
 from ..action.action_object import ActionObject
+from ..api.api import TwinAPIEndpoint
 from ..log.log import SyftLog
 from ..response import SyftError
 from ..response import SyftSuccess
 from .diff_state import ObjectDiff
 from .diff_state import ObjectDiffBatch
 from .diff_state import ResolvedSyncState
 from .diff_state import SyncInstruction
-from .sync_state import SyncView
 
 # Standard div Jupyter Lab uses for notebook outputs
 # This is needed to use alert styles from SyftSuccess and SyftError
 NOTEBOOK_OUTPUT_DIV = """
 <div class="lm-Widget
             jp-RenderedHTMLCommon
             jp-RenderedHTML
@@ -66,294 +67,318 @@
     DiffStatus.NEW: "#256B24;",
     DiffStatus.SAME: "#353243",
     DiffStatus.MODIFIED: "#B8520A;",
     DiffStatus.DELETED: "#353243",
 }
 
 
-class HeaderWidget:
+def create_diff_html(
+    title: str,
+    properties: dict[str, str],
+    statuses: dict[str, DiffStatus],
+) -> str:
+    html_str = f"<div style='width: 100%;'>{title}<br>"
+    html_str += "<div style='font-family: monospace; border-left: 1px solid #B4B0BF; padding-left: 10px;'>"
+
+    for attr, val in properties.items():
+        status = statuses[attr]
+        val = val if val is not None else ""
+        style = f"background-color: {background_colors[status]}; color: {colors[status]}; display: block; white-space: pre-wrap; margin-bottom: 5px;"  # noqa: E501
+        content = html.escape(f"{attr}: {val}")
+        html_str += f"<div style='{style}'>{content}</div>"
+
+    html_str += "</div></div>"
+
+    return html_str
+
+
+# TODO move CSS/HTML/JS outside function
+
+
+class MainObjectDiffWidget:
     def __init__(
         self,
-        item_type: str,
-        item_name: str,
-        item_id: str,
-        num_diffs: int,
-        source_side: str,
-        target_side: str,
+        diff: ObjectDiff,
+        direction: SyncDirection,
+        with_box: bool = True,
     ):
-        self.item_type = item_type
-        self.item_name = item_name
-        self.item_id = item_id
-        self.num_diffs = num_diffs
-        self.source_side = source_side
-        self.target_side = target_side
-        self.widget = self.create_widget()
+        self.low_properties = diff.repr_attr_dict("low")
+        self.high_properties = diff.repr_attr_dict("high")
+        self.statuses = diff.repr_attr_diffstatus_dict()
+        self.direction = direction
+        self.diff: ObjectDiff = diff
+        self.with_box = with_box
+        self.widget = self.build()
+        self.sync = True
+        self.is_main_widget: bool = True
 
-    @classmethod
-    def from_object_diff_batch(cls, obj_diff_batch: ObjectDiffBatch) -> Self:
-        """
-        (
-            diff=self.obj_diff_batch.root_diff,
-            item_type=self.obj_diff_batch.root_type_name,
-            item_name="compute_mean",
-            item_id=self.obj_diff_batch.root_id,
-            num_diffs=2,
-            source_side="Low",
-            target_side="High",
-        )
+    def set_share_private_data(self) -> None:
+        # No-op for main widget
+        pass
 
-        """
-        if obj_diff_batch.sync_direction == SyncDirection.LOW_TO_HIGH:
+    @property
+    def mockify(self) -> bool:
+        return not self.share_private_data
+
+    @property
+    def has_unused_share_button(self) -> bool:
+        # does not have share button
+        return False
+
+    @property
+    def share_private_data(self) -> bool:
+        # there are TwinAPIEndpoint.__private_sync_attr_mocks__
+        return not isinstance(self.diff.non_empty_object, TwinAPIEndpoint)
+
+    def build(self) -> widgets.HBox:
+        all_keys = list(self.low_properties.keys()) + list(self.high_properties.keys())
+        low_properties = {}
+        high_properties = {}
+        for k in all_keys:
+            low_properties[k] = self.low_properties.get(k, None)
+            high_properties[k] = self.high_properties.get(k, None)
+
+        if self.direction == SyncDirection.LOW_TO_HIGH:
+            from_properties = low_properties
+            to_properties = high_properties
             source_side = "Low side"
             target_side = "High side"
         else:
+            from_properties = high_properties
+            to_properties = low_properties
             source_side = "High side"
             target_side = "Low side"
 
-        root_diff = obj_diff_batch.root_diff
-        root_obj = (
-            root_diff.low_obj if root_diff.low_obj is not None else root_diff.high_obj
-        )
-        obj_view = SyncView(object=root_obj)
-        return cls(
-            item_type=obj_view.object_type_name,
-            item_name=obj_view.main_object_description_str(),
-            item_id=str(root_obj.id.id),  # type: ignore
-            num_diffs=len(obj_diff_batch.get_dependencies(include_roots=True)),
-            source_side=source_side,
-            target_side=target_side,
-        )
-
-    def copy_text_button(self, text: str) -> widgets.Widget:
-        button = widgets.Button(
-            icon="clone",
-            layout=widgets.Layout(width="25px", height="25px", margin="0", padding="0"),
-        )
-        output = widgets.Output(layout=widgets.Layout(display="none"))
-        copy_js = Javascript(f"navigator.clipboard.writeText({json.dumps(text)})")
-
-        def on_click(_: widgets.Button) -> None:
-            output.clear_output()
-            with output:
-                display(copy_js)
-
-        button.on_click(on_click)
-
-        return widgets.Box(
-            (button, output),
-            layout=widgets.Layout(display="flex", align_items="center"),
-        )
-
-    def create_item_type_label(self, item_type: str) -> HTML:
-        # TODO different bg for different types (levels?)
-        style = (
-            "background-color: #C2DEF0; "
-            "border-radius: 4px; "
-            "padding: 4px 6px; "
-            "color: #373B7B;"
-        )
-        return HTML(
-            value=f"<span style='{style}'>{item_type.upper()}</span>",
-            layout=Layout(margin="0 5px 0 0"),
-        )
-
-    def create_name_id_label(self, item_name: str, item_id: str) -> HTML:
-        item_id_short = item_id[:4] + "..." if len(item_id) > 4 else item_id
-        return HTML(
-            value=(
-                f"<span style='margin-left: 5px; font-weight: bold; color: #373B7B;'>{item_name}</span> "
-                f"<span style='margin-left: 5px; color: #B4B0BF;'>#{item_id_short}</span>"
-            )
+        html_from = create_diff_html(
+            f"From <i>{source_side}</i> (new values)", from_properties, self.statuses
+        )
+        html_to = create_diff_html(
+            f"To <i>{target_side}</i> (old values)", to_properties, self.statuses
         )
 
-    def create_widget(self) -> VBox:
-        type_box = self.create_item_type_label(self.item_type)
-        name_id_label = self.create_name_id_label(self.item_name, self.item_id)
-        copy_button = self.copy_text_button(self.item_id)
-
-        first_line = HTML(
-            value="<span style='color: #B4B0BF;'>Syncing changes on</span>"
+        widget_from = widgets.HTML(
+            value=html_from, layout=widgets.Layout(width="50%", overflow="auto")
         )
-        second_line = HBox(
-            [type_box, name_id_label, copy_button], layout=Layout(align_items="center")
+        widget_to = widgets.HTML(
+            value=html_to, layout=widgets.Layout(width="50%", overflow="auto")
         )
-        third_line = HTML(
-            value=f"<span style='color: #5E5A72;'>This would sync <span style='color: #B8520A'>{self.num_diffs} changes </span> from <i>{self.source_side} Node</i> to <i>{self.target_side} Node</i></span>"  # noqa: E501
+        css_accordion = """
+            <style>
+            .diff-container {
+                border: 0.5px solid #B4B0BF;
+            }
+            </style>
+        """
+        dom_classes = []
+        if self.with_box:
+            dom_classes.append("diff-container")
+
+        return widgets.HBox(
+            [HTML(css_accordion), widget_from, widget_to], _dom_classes=dom_classes
         )
-        fourth_line = HTML(value="<div style='height: 16px;'></div>")
-        header = VBox([first_line, second_line, third_line, fourth_line])
-        return header
 
 
-# TODO use ObjectDiff instead
-class ObjectDiffWidget:
+class CollapsableObjectDiffWidget:
     def __init__(
         self,
         diff: ObjectDiff,
-        low_properties: list[str],
-        high_properties: list[str],
-        statuses: list[DiffStatus],
         direction: SyncDirection,
-        is_main_widget: bool = False,
     ):
-        self.low_properties = low_properties
-        self.high_properties = high_properties
-        self.statuses = statuses
         self.direction = direction
         self.share_private_data = False
         self.diff: ObjectDiff = diff
-
         self.sync: bool = False
-
-        self.is_main_widget = is_main_widget
+        self.is_main_widget: bool = False
         self.widget = self.build()
         self.set_and_disable_sync()
 
     @property
     def mockify(self) -> bool:
-        if self.show_share_button and not self.share_private_data:
+        if isinstance(self.diff.non_empty_object, TwinAPIEndpoint):
+            return True
+        if self.has_unused_share_button:
             return True
         else:
             return False
 
-    @classmethod
-    def from_diff(
-        cls, diff: ObjectDiff, direction: SyncDirection, is_main_widget: bool
-    ) -> Self:
-        return cls(
-            low_properties=diff.repr_attr_dict("low"),
-            high_properties=diff.repr_attr_dict("high"),
-            statuses=diff.repr_attr_diffstatus_dict(),
-            is_main_widget=is_main_widget,
-            diff=diff,
-            direction=direction,
-        )
+    @property
+    def has_unused_share_button(self) -> bool:
+        return self.show_share_button and not self.share_private_data
 
     @property
     def show_share_button(self) -> bool:
         return isinstance(self.diff.non_empty_object, SyftLog | ActionObject)
 
     @property
-    def show_sync_button(self) -> bool:
-        return not self.is_main_widget
-
-    @property
-    def num_changes(self) -> int:
-        return len([x for x in self.statuses.values() if x != DiffStatus.SAME])
-
-    @property
     def title(self) -> str:
-        return f"{self.diff.object_type} ({self.num_changes} changes)"
+        object = self.diff.non_empty_object
+        if object is None:
+            return "n/a"
+        type_html = Badge(object=object).to_html()
+        description_html = MainDescription(object=object).to_html()
+        copy_id_button = CopyIDButton(copy_text=str(object.id.id), max_width=60)
+
+        second_line_html = f"""
+            <div class="widget-header2">
+            <div class="widget-header2-2">
+            {type_html} {description_html}
+            </div>
+            {copy_id_button.to_html()}
+            </div>
+        """  # noqa: E501
+        return second_line_html
 
     def set_and_disable_sync(self) -> None:
-        if self.show_sync_button:
-            self._sync_checkbox.disabled = True
-            self._sync_checkbox.value = True
+        self._sync_checkbox.disabled = True
+        self._sync_checkbox.value = True
 
     def enable_sync(self) -> None:
         if self.show_sync_button:
             self._sync_checkbox.disabled = False
 
     def set_share_private_data(self) -> None:
         if self.show_share_button:
             self._share_private_checkbox.value = True
 
-    def create_diff_html(
-        self,
-        title: str,
-        properties: dict[str, str],
-        statuses: dict[str, DiffStatus],
-    ) -> str:
-        html_str = f"<div style='width: 100%;'>{title}<br>"
-        html_str += "<div style='font-family: monospace; border-left: 1px solid #B4B0BF; padding-left: 10px;'>"
+    def build(self) -> widgets.VBox:
+        content = MainObjectDiffWidget(self.diff, self.direction, with_box=False).widget
 
-        for attr, val in properties.items():
-            status = statuses[attr]
-            val = val if val is not None else ""
-            style = f"background-color: {background_colors[status]}; color: {colors[status]}; display: block; white-space: pre-wrap; margin-bottom: 5px;"  # noqa: E501
-            content = html.escape(f"{attr}: {val}")
-            html_str += f"<div style='{style}'>{content}</div>"
+        accordion, share_private_checkbox, sync_checkbox = self.build_accordion(
+            accordion_body=content,
+            show_sync_checkbox=True,
+            show_share_private_checkbox=self.show_share_button,
+        )
 
-        html_str += "</div></div>"
+        self._sync_checkbox = sync_checkbox
+        self._sync_checkbox.observe(self._on_sync_change, "value")
 
-        return html_str
+        self._share_private_checkbox = share_private_checkbox
+        self._share_private_checkbox.observe(
+            self._on_share_private_data_change, "value"
+        )
 
-    def build(self) -> widgets.VBox:
-        all_keys = list(self.low_properties.keys()) + list(self.high_properties.keys())
-        low_properties = {}
-        high_properties = {}
-        for k in all_keys:
-            low_properties[k] = self.low_properties.get(k, None)
-            high_properties[k] = self.high_properties.get(k, None)
+        return accordion
 
-        if self.direction == SyncDirection.LOW_TO_HIGH:
-            from_properties = low_properties
-            to_properties = high_properties
-            source_side = "Low side"
-            target_side = "High side"
-        else:
-            from_properties = high_properties
-            to_properties = low_properties
-            source_side = "High side"
-            target_side = "Low side"
+    def create_accordion_css(
+        self, header_id: str, body_id: str, class_name: str
+    ) -> str:
+        css_accordion = f"""
+            <style>
+            .accordion {{
+                padding: 0 10px;
+            }}
+
+            .body-hidden {{
+                display: none;
+            }}
+
+            .body-visible {{
+                display: flex;
+            }}
+
+            .{header_id}{{
+                display: flex;
+                align-items: center;
+            }}
+
+
+            .{class_name}-folded {{
+                background: #F4F3F6;
+                border: 0.5px solid #B4B0BF;
+            }}
+            .{class_name}-unfolded {{
+                background: white;
+                border: 0.5px solid #B4B0BF;
+            }}
+            </style>
+        """
+        return css_accordion
 
-        html_from = self.create_diff_html(
-            f"From <i>{source_side}</i> (new values)", from_properties, self.statuses
-        )
-        html_to = self.create_diff_html(
-            f"To <i>{target_side}</i> (old values)", to_properties, self.statuses
+    def build_accordion(
+        self,
+        accordion_body: widgets.Widget,
+        show_sync_checkbox: bool = True,
+        show_share_private_checkbox: bool = True,
+    ) -> VBox:
+        uid = str(uuid4())
+        body_id = f"accordion-body-{uid}"
+        header_id = f"accordion-header-{uid}"
+        class_name = f"accordion-{uid}"
+        caret_id = f"caret-{uid}"
+
+        toggle_hide_body_js = f"""
+            var body = document.getElementsByClassName('{body_id}')[0];
+            var caret = document.getElementById('{caret_id}');
+            if (body.classList.contains('body-hidden')) {{
+                var vbox = document.getElementsByClassName('{class_name}-folded')[0];
+                body.classList.remove('body-hidden');
+                body.classList.add('body-visible');
+                vbox.classList.remove('{class_name}-folded');
+                vbox.classList.add('{class_name}-unfolded');
+                caret.classList.remove('fa-caret-right');
+                caret.classList.add('fa-caret-down');
+            }} else {{
+                var vbox = document.getElementsByClassName('{class_name}-unfolded')[0];
+                body.classList.remove('body-visible');
+                body.classList.add('body-hidden');
+                vbox.classList.remove('{class_name}-unfolded');
+                vbox.classList.add('{class_name}-folded');
+                caret.classList.remove('fa-caret-down');
+                caret.classList.add('fa-caret-right');
+            }}
+        """
+        caret = f'<i id="{caret_id}" class="fa fa-fw fa-caret-right"></i>'
+        title_html = HTML(
+            value=f"<div class='{header_id}' onclick=\"{toggle_hide_body_js}\" style='cursor: pointer; flex-grow: 1; user-select: none; '>{caret} {self.title}</div>",  # noqa: E501
+            layout=Layout(flex="1"),
         )
 
-        widget_from = widgets.HTML(
-            value=html_from, layout=widgets.Layout(width="50%", overflow="auto")
+        share_private_data_checkbox = Checkbox(
+            description="Sync Real Data",
+            layout=Layout(width="auto", margin="0 2px 0 0"),
         )
-        widget_to = widgets.HTML(
-            value=html_to, layout=widgets.Layout(width="50%", overflow="auto")
+        sync_checkbox = Checkbox(
+            description="Sync", layout=Layout(width="auto", margin="0 2px 0 0")
         )
-        content = widgets.HBox([widget_from, widget_to])
 
         checkboxes = []
+        if show_share_private_checkbox:
+            checkboxes.append(share_private_data_checkbox)
+        if show_sync_checkbox:
+            checkboxes.append(sync_checkbox)
 
-        if self.show_sync_button:
-            self._sync_checkbox = widgets.Checkbox(
-                value=self.sync,
-                description="Sync",
-            )
-            self._sync_checkbox.observe(self._on_sync_change, "value")
-            checkboxes.append(self._sync_checkbox)
+        accordion_header = HBox(
+            [title_html] + checkboxes,
+            layout=Layout(width="100%", justify_content="space-between"),
+        )
 
-        if self.show_share_button:
-            self._share_private_checkbox = widgets.Checkbox(
-                value=self.share_private_data,
-                description="Share private data",
-            )
-            self._share_private_checkbox.observe(
-                self._on_share_private_data_change, "value"
-            )
-            checkboxes = [self._share_private_checkbox] + checkboxes
+        accordion_body.add_class(body_id)
+        accordion_body.add_class("body-hidden")
 
-        checkboxes_widget = widgets.HBox(checkboxes)
-        kwargs = {}
-        if self.is_main_widget:
-            kwargs["layout"] = Layout(border="#353243 solid 0.5px", padding="16px")
+        style = HTML(value=self.create_accordion_css(header_id, body_id, class_name))
 
-        widget = widgets.VBox([checkboxes_widget, content], **kwargs)
-        return widget
+        accordion = VBox(
+            [style, accordion_header, accordion_body],
+            _dom_classes=(f"accordion-{uid}-folded", "accordion"),
+        )
+        return accordion, share_private_data_checkbox, sync_checkbox
 
     def _on_sync_change(self, change: Any) -> None:
         self.sync = change["new"]
 
     def _on_share_private_data_change(self, change: Any) -> None:
         self.share_private_data = change["new"]
 
 
 class ResolveWidget:
     def __init__(self, obj_diff_batch: ObjectDiffBatch):
         self.obj_diff_batch: ObjectDiffBatch = obj_diff_batch
-        self.id2widget: dict[UID, ObjectDiffWidget] = {}
+        self.id2widget: dict[
+            UID, CollapsableObjectDiffWidget | MainObjectDiffWidget
+        ] = {}
         self.main_widget = self.build()
         self.result_widget = VBox()  # Placeholder for SyftSuccess / SyftError
         self.widget = VBox(
             [self.build_css_widget(), self.main_widget, self.result_widget]
         )
         self.is_synced = False
         self.hide_result_widget()
@@ -396,16 +421,20 @@
 
         # previously_ignored_batches = state.low_state.ignored_batches
         previously_ignored_batches: dict = {}
         # TODO: only add permissions for objects where we manually give permission
         # Maybe default read permission for some objects (high -> low)
 
         # TODO: UID
-        resolved_state_low = ResolvedSyncState(node_uid=UID(), alias="low")
-        resolved_state_high = ResolvedSyncState(node_uid=UID(), alias="high")
+        resolved_state_low = ResolvedSyncState(
+            node_uid=self.obj_diff_batch.low_node_uid, alias="low"
+        )
+        resolved_state_high = ResolvedSyncState(
+            node_uid=self.obj_diff_batch.high_node_uid, alias="high"
+        )
 
         batch_diff = self.obj_diff_batch
         if batch_diff.is_unchanged:
             # Hierarchy has no diffs
             return SyftSuccess(message="No changes to sync")
 
         if batch_diff.decision is not None:
@@ -465,76 +494,72 @@
 
         print(f"Decision: Syncing {len(sync_instructions)} objects")
 
         for sync_instruction in sync_instructions:
             resolved_state_low.add_sync_instruction(sync_instruction)
             resolved_state_high.add_sync_instruction(sync_instruction)
 
-        # TODO: ONLY WORKS FOR LOW TO HIGH
-        # relative
-        from ...client.domain_client import DomainClient
-
-        api = APIRegistry.api_for(
-            self.obj_diff_batch.target_node_uid, self.obj_diff_batch.target_verify_key
-        )
-        client = DomainClient(
-            api=api,
-            connection=api.connection,  # type: ignore
-            credentials=api.signing_key,  # type: ignore
-        )
-
         if self.obj_diff_batch.sync_direction is None:
             raise ValueError("no direction specified")
-        if self.obj_diff_batch.sync_direction == SyncDirection.LOW_TO_HIGH:
-            res = client.apply_state(resolved_state_high)
-        else:
-            res = client.apply_state(resolved_state_low)
+        sync_direction = self.obj_diff_batch.sync_direction
+        resolved_state = (
+            resolved_state_high
+            if sync_direction == SyncDirection.LOW_TO_HIGH
+            else resolved_state_low
+        )
+        res = self.obj_diff_batch.target_client.apply_state(resolved_state)
+
+        if sync_direction == SyncDirection.HIGH_TO_LOW:
+            # apply empty state to generete a new state
+            resolved_state_high = ResolvedSyncState(
+                node_uid=self.obj_diff_batch.high_node_uid, alias="high"
+            )
+            high_client = self.obj_diff_batch.source_client
+            res = high_client.apply_state(resolved_state_high)
 
         self.is_synced = True
         self.set_result_state(res)
         self.hide_main_widget()
         self.show_result_widget()
         return res
 
     @property
-    def batch_diff_widgets(self) -> list[ObjectDiffWidget]:
+    def batch_diff_widgets(self) -> list[CollapsableObjectDiffWidget]:
         dependents = self.obj_diff_batch.get_dependents(
             include_roots=False, include_batch_root=False
         )
         dependent_diff_widgets = [
-            ObjectDiffWidget.from_diff(
+            CollapsableObjectDiffWidget(
                 diff,
-                is_main_widget=False,
                 direction=self.obj_diff_batch.sync_direction,
             )
             for diff in dependents
         ]
         return dependent_diff_widgets
 
     @property
-    def dependent_batch_diff_widgets(self) -> list[ObjectDiffWidget]:
+    def dependent_batch_diff_widgets(self) -> list[CollapsableObjectDiffWidget]:
         dependencies = self.obj_diff_batch.get_dependencies(
             include_roots=True, include_batch_root=False
         )
         other_roots = [
             d for d in dependencies if d.object_id in self.obj_diff_batch.global_roots
         ]
         dependent_root_diff_widgets = [
-            ObjectDiffWidget.from_diff(
-                diff, is_main_widget=False, direction=self.obj_diff_batch.sync_direction
+            CollapsableObjectDiffWidget(
+                diff, direction=self.obj_diff_batch.sync_direction
             )
             for diff in other_roots
         ]
         return dependent_root_diff_widgets
 
     @property
-    def main_object_diff_widget(self) -> ObjectDiffWidget:
-        obj_diff_widget = ObjectDiffWidget.from_diff(
+    def main_object_diff_widget(self) -> MainObjectDiffWidget:
+        obj_diff_widget = MainObjectDiffWidget(
             self.obj_diff_batch.root_diff,
-            is_main_widget=True,
             direction=self.obj_diff_batch.sync_direction,
         )
         return obj_diff_widget
 
     def set_result_state(self, result: SyftSuccess | SyftError) -> None:
         result_html = result._repr_html_()
         # Wrap in div to match Jupyter Lab output styling
@@ -564,26 +589,25 @@
 
         for widget in batch_diff_widgets:
             self.id2widget[widget.diff.object_id] = widget
 
         for widget in dependent_batch_diff_widgets:
             self.id2widget[widget.diff.object_id] = widget
 
-        main_batch_items = widgets.Accordion(
+        main_batch_items = widgets.VBox(
             children=[d.widget for d in batch_diff_widgets],
-            titles=[d.title for d in batch_diff_widgets],
         )
-        dependency_items = widgets.Accordion(
+
+        dependency_items = widgets.VBox(
             children=[d.widget for d in dependent_batch_diff_widgets],
-            titles=[d.title for d in dependent_batch_diff_widgets],
         )
 
         full_widget = widgets.VBox(
             [
-                self.build_header().widget,
+                self.build_header(),
                 self.main_object_diff_widget.widget,
                 self.spacer(16),
                 main_batch_items,
                 self.separator(),
                 dependency_items,
                 self.spacer(16),
                 self.sync_button(),
@@ -609,9 +633,10 @@
 
     def separator(self) -> widgets.HTML:
         return widgets.HTML(
             value='<div style="text-align: center; margin: 10px 0; border: 1px dashed #B4B0BF;"></div>',
             layout=Layout(width="100%"),
         )
 
-    def build_header(self) -> HeaderWidget:
-        return HeaderWidget.from_object_diff_batch(self.obj_diff_batch)
+    def build_header(self) -> HTML:
+        header_html = SyncWidgetHeader(diff_batch=self.obj_diff_batch).to_html()
+        return HTML(value=header_html)
```

### Comparing `syft-0.8.7b1/src/syft/service/sync/sync_service.py` & `syft-0.8.7b2/src/syft/service/sync/sync_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from ...types.syncable_object import SyncableSyftObject
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..action.action_object import ActionObject
 from ..action.action_permissions import ActionObjectPermission
 from ..action.action_permissions import ActionPermission
 from ..action.action_permissions import StoragePermission
+from ..api.api import TwinAPIEndpoint
 from ..code.user_code import UserCodeStatusCollection
 from ..context import AuthedServiceContext
 from ..job.job_stash import Job
 from ..output.output_service import ExecutionOutput
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..service import AbstractService
@@ -146,14 +147,26 @@
     def set_object(
         self, context: AuthedServiceContext, item: SyncableSyftObject
     ) -> Result[SyftObject, str]:
         stash = self.get_stash_for_item(context, item)
         creds = context.credentials
 
         exists = stash.get_by_uid(context.credentials, item.id).ok() is not None
+
+        if isinstance(item, TwinAPIEndpoint):
+            # we need the side effect of set function
+            # to create an action object
+            res = context.node.get_service("apiservice").set(
+                context=context, endpoint=item
+            )
+            if isinstance(res, SyftError):
+                return res
+            else:
+                return Ok(item)
+
         if exists:
             res = stash.update(creds, item)
         else:
             # Storage permissions are added separately
             res = stash.set(
                 creds,
                 item,
@@ -233,41 +246,44 @@
     ) -> tuple[dict[UID, set[str]], dict[UID, set[str]]]:
         permissions = {}
         storage_permissions = {}
 
         for item in items:
             store = get_store(context, item)
             if store is not None:
-                _id = item.id.id
-                permissions[_id] = store.permissions[_id]
-                storage_permissions[_id] = store.storage_permissions[_id]
+                # TODO fix error handling
+                uid = item.id.id
+                permissions[uid] = store._get_permissions_for_uid(uid).ok()
+                storage_permissions[uid] = store._get_storage_permissions_for_uid(
+                    uid
+                ).ok()
         return permissions, storage_permissions
 
     def get_all_syncable_items(
         self, context: AuthedServiceContext
     ) -> Result[list[SyncableSyftObject], str]:
         all_items = []
 
         services_to_sync = [
             "requestservice",
             "usercodeservice",
             "jobservice",
             "logservice",
             "outputservice",
             "usercodestatusservice",
+            "apiservice",
         ]
 
         for service_name in services_to_sync:
             service = context.node.get_service(service_name)
             items = service.get_all(context)
             if isinstance(items, SyftError):
                 return items
             all_items.extend(items)
 
-        # NOTE we only need action objects from outputs for now
         action_object_ids = set()
         for obj in all_items:
             if isinstance(obj, ExecutionOutput):
                 action_object_ids |= set(obj.output_id_list)
             elif isinstance(obj, Job) and obj.result is not None:
                 if isinstance(obj.result, ActionObject):
                     obj.result = obj.result.as_empty()
```

### Comparing `syft-0.8.7b1/src/syft/service/sync/sync_stash.py` & `syft-0.8.7b2/src/syft/service/sync/sync_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/sync/sync_state.py` & `syft-0.8.7b2/src/syft/service/sync/sync_state.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,99 +17,25 @@
 from ...types.syncable_object import SyncableSyftObject
 from ...types.uid import LineageID
 from ...types.uid import UID
 from ...util import options
 from ...util.colors import SURFACE
 from ...util.fonts import FONT_CSS
 from ...util.fonts import ITABLES_CSS
-from ..code.user_code import UserCode
+from ...util.notebook_ui.components.sync import SyncTableObject
 from ..context import AuthedServiceContext
-from ..job.job_stash import Job
-from ..request.request import Request
 
 
 def get_hierarchy_level_prefix(level: int) -> str:
     if level == 0:
         return ""
     else:
         return "--" * level + " "
 
 
-@serializable()
-class SyncView(SyftObject):
-    __canonical_name__ = "SyncView"
-    __version__ = SYFT_OBJECT_VERSION_1
-
-    object: SyftObject
-
-    def main_object_description_str(self) -> str:
-        if isinstance(self.object, UserCode):
-            return self.object.service_func_name
-        elif isinstance(self.object, Job):  # type: ignore
-            return self.object.user_code_name
-        elif isinstance(self.object, Request):  # type: ignore
-            # TODO: handle other requests
-            return f"Execute {self.object.code.service_func_name}"
-        else:
-            return ""
-
-    @property
-    def object_type_name(self) -> str:
-        return type(self.object).__name__
-
-    def type_badge_class(self) -> str:
-        if isinstance(self.object, UserCode):
-            return "label-light-blue"
-        elif isinstance(self.object, Job):  # type: ignore
-            return "label-light-blue"
-        elif isinstance(self.object, Request):  # type: ignore
-            # TODO: handle other requests
-            return "label-light-purple"
-        else:
-            return ""
-
-    def get_status_str(self) -> str:
-        if isinstance(self.object, UserCode):
-            return ""
-        elif isinstance(self.object, Job):  # type: ignore
-            return f"Status: {self.object.status.value}"
-        elif isinstance(self.object, Request):
-            code = self.object.code
-            statusses = list(code.status.status_dict.values())
-            if len(statusses) != 1:
-                raise ValueError("Request code should have exactly one status")
-            status_tuple = statusses[0]
-            status, _ = status_tuple
-            return status.value
-        else:
-            return ""
-
-    def summary_html(self) -> str:
-        try:
-            type_html = f'<div class="label {self.type_badge_class()}">{self.object_type_name.upper()}</div>'
-            description_html = f"<span class='syncstate-description'>{self.main_object_description_str()}</span>"
-            updated_delta_str = "29m ago"
-            updated_by = "john@doe.org"
-            status_str = self.get_status_str()
-            status_seperator = " • " if len(status_str) else ""
-            summary_html = f"""
-    <div style="display: flex; gap: 8px; justify-content: start; width: 100%;">
-    {type_html} {description_html}
-    </div>
-    <div style="display: table-row">
-    <span class='syncstate-col-footer'>{status_str}{status_seperator}Updated by {updated_by} {updated_delta_str}</span>
-    </div>
-    """
-            summary_html = summary_html.replace("\n", "")
-        except Exception as e:
-            print("Failed to build table", e)
-            raise
-        return summary_html
-
-
 class SyncStateRow(SyftObject):
     """A row in the SyncState table"""
 
     __canonical_name__ = "SyncStateItem"
     __version__ = SYFT_OBJECT_VERSION_1
 
     object: SyftObject
@@ -135,30 +61,30 @@
         elif status == "SAME":
             badge_color = "label-gray"
         else:
             badge_color = "label-orange"
         return {"value": status.upper(), "type": badge_color}
 
     def _coll_repr_(self) -> dict[str, Any]:
-        obj_view = SyncView(object=self.object)
+        obj_view = SyncTableObject(object=self.object)
 
         if self.last_sync_date is not None:
             last_sync_date = self.last_sync_date
             last_sync_delta = timedelta(
                 seconds=DateTime.now().utc_timestamp - last_sync_date.utc_timestamp
             )
             last_sync_delta_str = td_format(last_sync_delta)
             last_sync_html = (
                 f"<p class='diff-state-no-obj'>{last_sync_delta_str} ago</p>"
             )
         else:
             last_sync_html = "<p class='diff-state-no-obj'>n/a</p>"
         return {
             "Status": self.status_badge(),
-            "Summary": obj_view.summary_html(),
+            "Summary": obj_view.to_html(),
             "Last Sync": last_sync_html,
         }
 
     @property
     def object_type(self) -> str:
         prefix = get_hierarchy_level_prefix(self.level)
         return f"{prefix}{type(self.object).__name__}"
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `syft-0.8.7b1/src/syft/service/user/user.py` & `syft-0.8.7b2/src/syft/service/user/user.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/user/user_roles.py` & `syft-0.8.7b2/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/user/user_service.py` & `syft-0.8.7b2/src/syft/service/user/user_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/user/user_stash.py` & `syft-0.8.7b2/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/warnings.py` & `syft-0.8.7b2/src/syft/service/warnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/worker/image_identifier.py` & `syft-0.8.7b2/src/syft/service/worker/image_identifier.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/worker/image_registry.py` & `syft-0.8.7b2/src/syft/service/worker/image_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/worker/image_registry_service.py` & `syft-0.8.7b2/src/syft/service/worker/image_registry_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/worker/image_registry_stash.py` & `syft-0.8.7b2/src/syft/service/worker/image_registry_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/worker/utils.py` & `syft-0.8.7b2/src/syft/service/worker/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/worker/worker.py` & `syft-0.8.7b2/src/syft/service/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/worker/worker_image.py` & `syft-0.8.7b2/src/syft/service/worker/worker_image.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/worker/worker_image_service.py` & `syft-0.8.7b2/src/syft/service/worker/worker_image_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/worker/worker_image_stash.py` & `syft-0.8.7b2/src/syft/service/worker/worker_image_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/worker/worker_pool.py` & `syft-0.8.7b2/src/syft/service/worker/worker_pool.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/worker/worker_pool_service.py` & `syft-0.8.7b2/src/syft/service/worker/worker_pool_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/worker/worker_pool_stash.py` & `syft-0.8.7b2/src/syft/service/worker/worker_pool_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/worker/worker_service.py` & `syft-0.8.7b2/src/syft/service/worker/worker_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/service/worker/worker_stash.py` & `syft-0.8.7b2/src/syft/service/worker/worker_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/store/blob_storage/__init__.py` & `syft-0.8.7b2/src/syft/store/blob_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/store/blob_storage/on_disk.py` & `syft-0.8.7b2/src/syft/store/blob_storage/on_disk.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/store/blob_storage/seaweedfs.py` & `syft-0.8.7b2/src/syft/store/blob_storage/seaweedfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,18 @@
 from ...types.blob_storage import CreateBlobStorageEntry
 from ...types.blob_storage import SeaweedSecureFilePathLocation
 from ...types.blob_storage import SecureFilePathLocation
 from ...types.grid_url import GridURL
 from ...types.syft_object import SYFT_OBJECT_VERSION_3
 from ...util.constants import DEFAULT_TIMEOUT
 
+MAX_QUEUE_SIZE = 100
 WRITE_EXPIRATION_TIME = 900  # seconds
-DEFAULT_FILE_PART_SIZE = (1024**3) * 5  # 5GB
-DEFAULT_UPLOAD_CHUNK_SIZE = 819200
+DEFAULT_FILE_PART_SIZE = 1024**3  # 1GB
+DEFAULT_UPLOAD_CHUNK_SIZE = 1024 * 800  # 800KB
 
 
 @serializable()
 class SeaweedFSBlobDeposit(BlobDeposit):
     __canonical_name__ = "SeaweedFSBlobDeposit"
     __version__ = SYFT_OBJECT_VERSION_3
 
@@ -90,15 +91,15 @@
                     class PartGenerator:
                         def __init__(self) -> None:
                             self.no_lines = 0
 
                         def async_generator(
                             self, chunk_size: int = DEFAULT_UPLOAD_CHUNK_SIZE
                         ) -> Generator:
-                            item_queue: Queue = Queue()
+                            item_queue: Queue = Queue(maxsize=MAX_QUEUE_SIZE)
                             threading.Thread(
                                 target=self.add_chunks_to_queue,
                                 kwargs={"queue": item_queue, "chunk_size": chunk_size},
                                 daemon=True,
                             ).start()
                             item = item_queue.get()
                             while item != 0:
```

### Comparing `syft-0.8.7b1/src/syft/store/dict_document_store.py` & `syft-0.8.7b2/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/store/document_store.py` & `syft-0.8.7b2/src/syft/store/document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -517,26 +517,32 @@
 
     def remove_permission(self, permission: ActionObjectPermission) -> None:
         raise NotImplementedError
 
     def has_permission(self, permission: ActionObjectPermission) -> bool:
         raise NotImplementedError
 
+    def _get_permissions_for_uid(self, uid: UID) -> Result[set[str], str]:
+        raise NotImplementedError
+
     def add_storage_permission(self, permission: StoragePermission) -> None:
         raise NotImplementedError
 
     def add_storage_permissions(self, permissions: list[StoragePermission]) -> None:
         raise NotImplementedError
 
     def remove_storage_permission(self, permission: StoragePermission) -> None:
         raise NotImplementedError
 
     def has_storage_permission(self, permission: StoragePermission | UID) -> bool:
         raise NotImplementedError
 
+    def _get_storage_permissions_for_uid(self, uid: UID) -> Result[set[UID], str]:
+        raise NotImplementedError
+
     def _migrate_data(
         self,
         to_klass: SyftObject,
         context: AuthedServiceContext,
         has_permission: bool,
     ) -> Result[bool, str]:
         raise NotImplementedError
```

### Comparing `syft-0.8.7b1/src/syft/store/kv_document_store.py` & `syft-0.8.7b2/src/syft/store/kv_document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,14 +298,19 @@
         elif permission.permission == ActionPermission.WRITE:
             pass
         elif permission.permission == ActionPermission.EXECUTE:
             pass
 
         return False
 
+    def _get_permissions_for_uid(self, uid: UID) -> Result[set[str], Err]:
+        if uid in self.permissions:
+            return Ok(self.permissions[uid])
+        return Err(f"No permissions found for uid: {uid}")
+
     def add_storage_permission(self, permission: StoragePermission) -> None:
         permissions = self.storage_permissions[permission.uid]
         permissions.add(permission.node_uid)
         self.storage_permissions[permission.uid] = permissions
 
     def add_storage_permissions(self, permissions: list[StoragePermission]) -> None:
         for permission in permissions:
@@ -333,14 +338,19 @@
         # this checks permissions
         res = [self._get(uid, credentials, has_permission) for uid in self.data.keys()]
         result = [x.ok() for x in res if x.is_ok()]
         if order_by is not None:
             result = sorted(result, key=lambda x: getattr(x, order_by.key, ""))
         return Ok(result)
 
+    def _get_storage_permissions_for_uid(self, uid: UID) -> Result[set[UID], Err]:
+        if uid in self.storage_permissions:
+            return Ok(self.storage_permissions[uid])
+        return Err(f"No storage permissions found for uid: {uid}")
+
     def _remove_keys(
         self,
         store_key: QueryKey,
         unique_query_keys: QueryKeys,
         searchable_query_keys: QueryKeys,
     ) -> None:
         uqks = unique_query_keys.all
```

### Comparing `syft-0.8.7b1/src/syft/store/linked_obj.py` & `syft-0.8.7b2/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/store/locks.py` & `syft-0.8.7b2/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/store/mongo_client.py` & `syft-0.8.7b2/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/store/mongo_codecs.py` & `syft-0.8.7b2/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/store/mongo_document_store.py` & `syft-0.8.7b2/src/syft/store/mongo_document_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # stdlib
 from collections.abc import Callable
 from typing import Any
+from typing import Set  # noqa: UP035
 
 # third party
 from pydantic import Field
 from pymongo import ASCENDING
 from pymongo.collection import Collection as MongoCollection
 from result import Err
 from result import Ok
@@ -496,14 +497,27 @@
             ).permission_string
             in permissions["permissions"]
         ):
             return True
 
         return False
 
+    def _get_permissions_for_uid(self, uid: UID) -> Result[Set[str], Err]:  # noqa: UP006
+        collection_permissions_status = self.permissions
+        if collection_permissions_status.is_err():
+            return collection_permissions_status
+        collection_permissions: MongoCollection = collection_permissions_status.ok()
+
+        permissions: dict | None = collection_permissions.find_one({"_id": uid})
+
+        if permissions is None:
+            return Err(f"Permissions for object with UID {uid} not found!")
+
+        return Ok(set(permissions["permissions"]))
+
     def add_permission(self, permission: ActionObjectPermission) -> Result[None, Err]:
         collection_permissions_status = self.permissions
         if collection_permissions_status.is_err():
             return collection_permissions_status
         collection_permissions: MongoCollection = collection_permissions_status.ok()
 
         # find the permissions for the given permission.uid
@@ -629,14 +643,31 @@
                 {"$set": {"node_uids": node_uids}},
             )
         else:
             return Err(
                 f"the node_uid {storage_permission.node_uid} does not exist in the storage permission!"
             )
 
+    def _get_storage_permissions_for_uid(self, uid: UID) -> Result[Set[UID], Err]:  # noqa: UP006
+        storage_permissions_or_err = self.storage_permissions
+        if storage_permissions_or_err.is_err():
+            return storage_permissions_or_err
+        storage_permissions_collection: MongoCollection = (
+            storage_permissions_or_err.ok()
+        )
+
+        storage_permissions: dict | None = storage_permissions_collection.find_one(
+            {"_id": uid}
+        )
+
+        if storage_permissions is None:
+            return Err(f"Storage permissions for object with UID {uid} not found!")
+
+        return Ok(set(storage_permissions["node_uids"]))
+
     def take_ownership(
         self, uid: UID, credentials: SyftVerifyKey
     ) -> Result[SyftSuccess, str]:
         collection_permissions_status = self.permissions
         if collection_permissions_status.is_err():
             return collection_permissions_status
         collection_permissions: MongoCollection = collection_permissions_status.ok()
```

### Comparing `syft-0.8.7b1/src/syft/store/sqlite_document_store.py` & `syft-0.8.7b2/src/syft/store/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/types/blob_storage.py` & `syft-0.8.7b2/src/syft/types/blob_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,16 +323,17 @@
     id: UID
     type_: type | None = None
     mimetype: str = "bytes"
     file_size: int
     extensions: list[str] = []
 
     @classmethod
-    def from_obj(cls, obj: SyftObject) -> Self:
-        file_size = sys.getsizeof(serialize._serialize(obj=obj, to_bytes=True))
+    def from_obj(cls, obj: SyftObject, file_size: int | None = None) -> Self:
+        if file_size is None:
+            file_size = sys.getsizeof(serialize._serialize(obj=obj, to_bytes=True))
         return cls(file_size=file_size, type_=type(obj))
 
     @classmethod
     def from_path(cls, fp: str | Path, mimetype: str | None = None) -> Self:
         path = Path(fp)
         if not path.exists():
             raise SyftException(f"{fp} does not exist.")
```

### Comparing `syft-0.8.7b1/src/syft/types/datetime.py` & `syft-0.8.7b2/src/syft/types/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/types/dicttuple.py` & `syft-0.8.7b2/src/syft/types/dicttuple.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/types/grid_url.py` & `syft-0.8.7b2/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/types/identity.py` & `syft-0.8.7b2/src/syft/types/identity.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/types/syft_metaclass.py` & `syft-0.8.7b2/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/types/syft_migration.py` & `syft-0.8.7b2/src/syft/types/syft_migration.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/types/syft_object.py` & `syft-0.8.7b2/src/syft/types/syft_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/types/syncable_object.py` & `syft-0.8.7b2/src/syft/types/syncable_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/types/transforms.py` & `syft-0.8.7b2/src/syft/types/transforms.py`

 * *Files 3% similar despite different names*

```diff
@@ -139,14 +139,24 @@
     if context.output is None:
         return context
     if "id" not in context.output or not isinstance(context.output["id"], UID):
         context.output["id"] = UID()
     return context
 
 
+def generate_action_object_id(context: TransformContext) -> TransformContext:
+    if context.output is None:
+        return context
+    if "action_object_id" not in context.output or not isinstance(
+        context.output["action_object_id"], UID
+    ):
+        context.output["action_object_id"] = UID()
+    return context
+
+
 def validate_url(context: TransformContext) -> TransformContext:
     if context.output and context.output["url"] is not None:
         context.output["url"] = GridURL.from_url(context.output["url"]).url_no_port
     return context
 
 
 def validate_email(context: TransformContext) -> TransformContext:
```

### Comparing `syft-0.8.7b1/src/syft/types/twin_object.py` & `syft-0.8.7b2/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/types/uid.py` & `syft-0.8.7b2/src/syft/types/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/util/_std_stream_capture.py` & `syft-0.8.7b2/src/syft/util/_std_stream_capture.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/util/autoreload.py` & `syft-0.8.7b2/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/util/decorators.py` & `syft-0.8.7b2/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/util/experimental_flags.py` & `syft-0.8.7b2/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/util/filterwarnings.py` & `syft-0.8.7b2/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/util/fonts.py` & `syft-0.8.7b2/src/syft/util/fonts.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/util/logger.py` & `syft-0.8.7b2/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/util/markdown.py` & `syft-0.8.7b2/src/syft/util/markdown.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/util/notebook_ui/notebook_addons.py` & `syft-0.8.7b2/src/syft/util/notebook_ui/notebook_addons.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,14 +270,32 @@
 
     .syncstate-description {
         font-family: Open Sans;
         font-size: 14px;
         font-weight: 600;
         line-height: 19.6px;
         text-align: left;
+        white-space: nowrap;
+        flex-grow: 1;
+    }
+
+    .widget-header2{
+        display: flex;
+        gap: 8px;
+        justify-content: start;
+        width: 100%;
+        overflow: hidden;
+        align-items: center;
+    }
+
+    .widget-header2-2{
+        display: flex;
+        gap: 8px;
+        justify-content: start;
+        align-items: center;
     }
 
     .diff-state-orange-text{
         color: #B8520A;
     }
 
     .diff-state-no-obj{
@@ -321,16 +339,19 @@
         code-text;
         border-radius: 30px;
     }
 
     .label {
         code-text;
         border-radius: 4px;
-        padding: 0px 4px;
-
+        padding: 6px 4px;
+        white-space: nowrap;
+        overflow: hidden;
+        line-height: 1.2;
+        font-family: monospace;
     }
 
     .label-light-purple {
         label;
         background-color: #C9CFE8;
         color: #373B7B;
     }
@@ -397,14 +418,22 @@
         display: flex;
         justify-content: center;
         gap: 8px;
         padding: 5px;
         color: var(--tertiary-color);
     }
 
+    .widget-label-basic{
+        display:flex;
+    }
+
+    .widget-label-basic input[type='checkbox'][disabled] {
+        filter: sepia(0.3) hue-rotate(67deg) saturate(3);
+    }
+
     .page{
         color: black;
         font-weight: bold;
         color: var(--tertiary-color);
     }
     .page:hover {
       color: #38bdf8;
```

### Comparing `syft-0.8.7b1/src/syft/util/schema.py` & `syft-0.8.7b2/src/syft/util/schema.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/util/telemetry.py` & `syft-0.8.7b2/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/util/trace_decorator.py` & `syft-0.8.7b2/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/util/util.py` & `syft-0.8.7b2/src/syft/util/util.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft/util/version_compare.py` & `syft-0.8.7b2/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.7b1/src/syft.egg-info/PKG-INFO` & `syft-0.8.7b2/src/syft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.7b1
+Version: 0.8.7b2
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
@@ -50,15 +50,15 @@
 Requires-Dist: pandas==2.2.1
 Requires-Dist: docker==6.1.3
 Requires-Dist: kr8s==0.13.5
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: azure-storage-blob==12.19.1
 Requires-Dist: ipywidgets==8.1.2
 Provides-Extra: data-science
-Requires-Dist: transformers==4.38.2; extra == "data-science"
+Requires-Dist: transformers==4.39.3; extra == "data-science"
 Requires-Dist: opendp==0.9.2; extra == "data-science"
 Requires-Dist: evaluate==0.4.1; extra == "data-science"
 Requires-Dist: recordlinkage==0.16; extra == "data-science"
 Requires-Dist: dm-haiku==0.0.10; extra == "data-science"
 Requires-Dist: torch[cpu]==2.2.1; extra == "data-science"
 Provides-Extra: dev
 Requires-Dist: pytest<8; extra == "dev"
```

### Comparing `syft-0.8.7b1/src/syft.egg-info/SOURCES.txt` & `syft-0.8.7b2/src/syft.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
 src/syft/serde/mock.py
 src/syft/serde/recursive.py
 src/syft/serde/recursive_primitives.py
 src/syft/serde/serializable.py
 src/syft/serde/serialize.py
 src/syft/serde/signature.py
 src/syft/serde/third_party.py
+src/syft/serde/util.py
 src/syft/service/__init__.py
 src/syft/service/context.py
 src/syft/service/response.py
 src/syft/service/service.py
 src/syft/service/warnings.py
 src/syft/service/action/__init__.py
 src/syft/service/action/action_data_empty.py
@@ -188,17 +189,14 @@
 src/syft/service/sync/sync_state.py
 src/syft/service/user/__init__.py
 src/syft/service/user/roles.py
 src/syft/service/user/user.py
 src/syft/service/user/user_roles.py
 src/syft/service/user/user_service.py
 src/syft/service/user/user_stash.py
-src/syft/service/veilid/__init__.py
-src/syft/service/veilid/veilid_endpoints.py
-src/syft/service/veilid/veilid_service.py
 src/syft/service/worker/__init__.py
 src/syft/service/worker/image_identifier.py
 src/syft/service/worker/image_registry.py
 src/syft/service/worker/image_registry_service.py
 src/syft/service/worker/image_registry_stash.py
 src/syft/service/worker/utils.py
 src/syft/service/worker/worker.py
@@ -253,8 +251,12 @@
 src/syft/util/markdown.py
 src/syft/util/options.py
 src/syft/util/schema.py
 src/syft/util/telemetry.py
 src/syft/util/trace_decorator.py
 src/syft/util/util.py
 src/syft/util/version_compare.py
-src/syft/util/notebook_ui/notebook_addons.py
+src/syft/util/notebook_ui/__init__.py
+src/syft/util/notebook_ui/notebook_addons.py
+src/syft/util/notebook_ui/components/__init__.py
+src/syft/util/notebook_ui/components/base.py
+src/syft/util/notebook_ui/components/sync.py
```

### Comparing `syft-0.8.7b1/src/syft.egg-info/requires.txt` & `syft-0.8.7b2/src/syft.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 [:python_version < "3.12"]
 numpy<=1.24.4,>=1.23.5
 
 [:python_version >= "3.12"]
 numpy<1.27,>=1.26.4
 
 [data_science]
-transformers==4.38.2
+transformers==4.39.3
 opendp==0.9.2
 evaluate==0.4.1
 recordlinkage==0.16
 dm-haiku==0.0.10
 torch[cpu]==2.2.1
 
 [dev]
```

