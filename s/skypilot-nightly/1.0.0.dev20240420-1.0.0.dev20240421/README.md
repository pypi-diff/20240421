# Comparing `tmp/skypilot_nightly-1.0.0.dev20240420.tar.gz` & `tmp/skypilot_nightly-1.0.0.dev20240421.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot_nightly-1.0.0.dev20240420.tar", last modified: Sat Apr 20 10:38:07 2024, max compression
+gzip compressed data, was "skypilot_nightly-1.0.0.dev20240421.tar", last modified: Sun Apr 21 10:38:08 2024, max compression
```

## Comparing `skypilot_nightly-1.0.0.dev20240420.tar` & `skypilot_nightly-1.0.0.dev20240421.tar`

### file list

```diff
@@ -1,335 +1,338 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.376599 skypilot_nightly-1.0.0.dev20240420/
--rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-20 10:38:07.376599 skypilot_nightly-1.0.0.dev20240420/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 10:38:07.376599 skypilot_nightly-1.0.0.dev20240420/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-20 10:38:04.000000 skypilot_nightly-1.0.0.dev20240420/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.316599 skypilot_nightly-1.0.0.dev20240420/sky/
--rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-20 10:38:07.000000 skypilot_nightly-1.0.0.dev20240420/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.316599 skypilot_nightly-1.0.0.dev20240420/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/adaptors/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/adaptors/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/adaptors/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/adaptors/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/adaptors/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    21410 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.320599 skypilot_nightly-1.0.0.dev20240420/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)   118820 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   221923 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.320599 skypilot_nightly-1.0.0.dev20240420/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.320599 skypilot_nightly-1.0.0.dev20240420/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    26440 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (127)   186846 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.320599 skypilot_nightly-1.0.0.dev20240420/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43129 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    31006 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    30816 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/cloud_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)    12508 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    46901 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    21044 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16680 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/paperspace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/runpod.py
--rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.324599 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/cudo_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.324599 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
--rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/fluidstack_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/kubernetes_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/paperspace_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/runpod_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/vsphere_catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.328599 skypilot_nightly-1.0.0.dev20240420/sky/clouds/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/utils/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/utils/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/utils/oci_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/utils/scp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/clouds/vsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.328599 skypilot_nightly-1.0.0.dev20240420/sky/data/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   119221 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    24916 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    54049 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.328599 skypilot_nightly-1.0.0.dev20240420/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.328599 skypilot_nightly-1.0.0.dev20240420/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    36603 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/aws/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.328599 skypilot_nightly-1.0.0.dev20240420/sky/provision/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/azure/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.332599 skypilot_nightly-1.0.0.dev20240420/sky/provision/cudo/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/cudo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/cudo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/cudo/cudo_machine_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/cudo/cudo_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/cudo/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/docker_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.332599 skypilot_nightly-1.0.0.dev20240420/sky/provision/fluidstack/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/fluidstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/fluidstack/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/fluidstack/fluidstack_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14870 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/fluidstack/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.332599 skypilot_nightly-1.0.0.dev20240420/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    24482 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22258 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/instance_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.332599 skypilot_nightly-1.0.0.dev20240420/sky/provision/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    32523 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/kubernetes/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/kubernetes/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/kubernetes/network_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    53819 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/kubernetes/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/metadata_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.336599 skypilot_nightly-1.0.0.dev20240420/sky/provision/paperspace/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/paperspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/paperspace/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/paperspace/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/paperspace/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/paperspace/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25255 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/provisioner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.336599 skypilot_nightly-1.0.0.dev20240420/sky/provision/runpod/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/runpod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/runpod/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/runpod/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/runpod/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.336599 skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.336599 skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/cls_api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/cls_api_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/custom_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/metadata_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/service_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/service_manager_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/ssl_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/vapiconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/vim_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    24476 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/vsphere_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    60100 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.340599 skypilot_nightly-1.0.0.dev20240420/sky/serve/
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30137 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/serve/autoscalers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/serve/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/serve/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    29231 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/serve/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/serve/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/serve/load_balancing_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    55738 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/serve/replica_managers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/serve/serve_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    36837 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/serve/serve_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/serve/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/serve/service_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.340599 skypilot_nightly-1.0.0.dev20240420/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-20 10:38:04.000000 skypilot_nightly-1.0.0.dev20240420/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.344599 skypilot_nightly-1.0.0.dev20240420/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    11542 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    35113 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18788 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/log_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/log_lib.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.344599 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.344599 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    18603 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/azure/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/command_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.344599 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.344599 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.348599 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.348599 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/scp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.348599 skypilot_nightly-1.0.0.dev20240420/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/skypilot_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.348599 skypilot_nightly-1.0.0.dev20240420/sky/spot/
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/spot/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    25830 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/spot/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    13074 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/spot/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.348599 skypilot_nightly-1.0.0.dev20240420/sky/spot/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/spot/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.352599 skypilot_nightly-1.0.0.dev20240420/sky/spot/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/spot/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.352599 skypilot_nightly-1.0.0.dev20240420/sky/spot/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/spot/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/spot/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    22487 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/spot/spot_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    31559 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/spot/spot_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    46443 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.356599 skypilot_nightly-1.0.0.dev20240420/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/cudo-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/fluidstack-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/kubernetes-ingress.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/kubernetes-loadbalancer.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)     9851 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/kubernetes-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/kubernetes-ssh-jump.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/paperspace-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/runpod-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/sky-serve-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/spot-controller.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/templates/vsphere-ray.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.356599 skypilot_nightly-1.0.0.dev20240420/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.360599 skypilot_nightly-1.0.0.dev20240420/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.360599 skypilot_nightly-1.0.0.dev20240420/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/cluster_yaml_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/command_runner.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    22349 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25413 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/controller_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/env_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.360599 skypilot_nightly-1.0.0.dev20240420/sky/utils/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/kubernetes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9667 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/kubernetes/create_cluster.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/kubernetes/delete_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/kubernetes/generate_kind_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/kubernetes/gpu_labeler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/kubernetes_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/resources_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/rich_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20387 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.364599 skypilot_nightly-1.0.0.dev20240420/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-20 10:38:07.000000 skypilot_nightly-1.0.0.dev20240420/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9162 2024-04-20 10:38:07.000000 skypilot_nightly-1.0.0.dev20240420/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 10:38:07.000000 skypilot_nightly-1.0.0.dev20240420/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-20 10:38:07.000000 skypilot_nightly-1.0.0.dev20240420/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-20 10:38:07.000000 skypilot_nightly-1.0.0.dev20240420/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-20 10:38:07.000000 skypilot_nightly-1.0.0.dev20240420/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 10:38:07.364599 skypilot_nightly-1.0.0.dev20240420/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/tests/test_serve_autoscaler.py
--rw-r--r--   0 runner    (1001) docker     (127)   211236 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/tests/test_spot_serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/tests/test_wheels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-20 10:38:01.000000 skypilot_nightly-1.0.0.dev20240420/tests/test_yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.347398 skypilot_nightly-1.0.0.dev20240421/
+-rw-r--r--   0 runner    (1001) docker     (127)    12170 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-21 10:38:08.347398 skypilot_nightly-1.0.0.dev20240421/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 10:38:08.347398 skypilot_nightly-1.0.0.dev20240421/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-21 10:38:05.000000 skypilot_nightly-1.0.0.dev20240421/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.283399 skypilot_nightly-1.0.0.dev20240421/sky/
+-rw-r--r--   0 runner    (1001) docker     (127)     5588 2024-04-21 10:38:08.000000 skypilot_nightly-1.0.0.dev20240421/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.283399 skypilot_nightly-1.0.0.dev20240421/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6863 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/adaptors/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/adaptors/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/adaptors/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/adaptors/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/adaptors/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21410 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.287399 skypilot_nightly-1.0.0.dev20240421/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)   118820 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   222702 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16741 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.287399 skypilot_nightly-1.0.0.dev20240421/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7297 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.287399 skypilot_nightly-1.0.0.dev20240421/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26440 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)   186846 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11806 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.291399 skypilot_nightly-1.0.0.dev20240421/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43129 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31006 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30816 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/cloud_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12508 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46901 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21044 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17186 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12045 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25299 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/paperspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/runpod.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15546 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.295399 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)    12771 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7289 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26837 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/cudo_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.295399 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22424 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11477 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22243 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21462 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/fluidstack_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24120 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4472 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4240 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/kubernetes_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/paperspace_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/runpod_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/vsphere_catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.295399 skypilot_nightly-1.0.0.dev20240421/sky/clouds/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/utils/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9991 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/utils/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/utils/oci_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/utils/scp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/clouds/vsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.299399 skypilot_nightly-1.0.0.dev20240421/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21664 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8226 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119221 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24916 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54049 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.299399 skypilot_nightly-1.0.0.dev20240421/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.299399 skypilot_nightly-1.0.0.dev20240421/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22092 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36603 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/aws/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.299399 skypilot_nightly-1.0.0.dev20240421/sky/provision/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/azure/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8561 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.303398 skypilot_nightly-1.0.0.dev20240421/sky/provision/cudo/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/cudo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/cudo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/cudo/cudo_machine_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/cudo/cudo_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8202 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/cudo/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/docker_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.303398 skypilot_nightly-1.0.0.dev20240421/sky/provision/fluidstack/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/fluidstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/fluidstack/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/fluidstack/fluidstack_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14870 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/fluidstack/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.303398 skypilot_nightly-1.0.0.dev20240421/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32964 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7234 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24482 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59069 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22258 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/instance_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.303398 skypilot_nightly-1.0.0.dev20240421/sky/provision/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17388 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32523 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/kubernetes/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.307399 skypilot_nightly-1.0.0.dev20240421/sky/provision/kubernetes/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/kubernetes/manifests/smarter-device-manager-configmap.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9457 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/kubernetes/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8635 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/kubernetes/network_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54541 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/kubernetes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/metadata_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.307399 skypilot_nightly-1.0.0.dev20240421/sky/provision/paperspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/paperspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/paperspace/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/paperspace/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/paperspace/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9428 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/paperspace/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25255 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/provisioner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.307399 skypilot_nightly-1.0.0.dev20240421/sky/provision/runpod/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/runpod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/runpod/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/runpod/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/runpod/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.307399 skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.311399 skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/cls_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14096 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/cls_api_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/custom_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/metadata_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/service_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/service_manager_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/ssl_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/vapiconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/vim_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24476 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/vsphere_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61778 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.311399 skypilot_nightly-1.0.0.dev20240421/sky/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30137 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/serve/autoscalers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/serve/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7571 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/serve/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29231 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/serve/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/serve/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/serve/load_balancing_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55738 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/serve/replica_managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18830 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/serve/serve_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36837 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/serve/serve_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/serve/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13803 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/serve/service_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.311399 skypilot_nightly-1.0.0.dev20240421/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-21 10:38:05.000000 skypilot_nightly-1.0.0.dev20240421/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4000 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.315399 skypilot_nightly-1.0.0.dev20240421/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9964 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11542 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35113 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18788 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/log_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/log_lib.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.315399 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.315399 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)    10901 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18603 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/azure/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15645 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/command_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.315399 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34630 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.315399 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13992 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.319398 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20492 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17202 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.319398 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22411 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/scp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.319398 skypilot_nightly-1.0.0.dev20240421/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/skypilot_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.319398 skypilot_nightly-1.0.0.dev20240421/sky/spot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/spot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25830 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/spot/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13074 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/spot/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.319398 skypilot_nightly-1.0.0.dev20240421/sky/spot/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/spot/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.323398 skypilot_nightly-1.0.0.dev20240421/sky/spot/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/spot/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.323398 skypilot_nightly-1.0.0.dev20240421/sky/spot/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/spot/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/spot/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22487 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/spot/spot_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31559 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/spot/spot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47182 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.323398 skypilot_nightly-1.0.0.dev20240421/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     9037 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/cudo-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/fluidstack-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8872 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/kubernetes-ingress.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/kubernetes-loadbalancer.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/kubernetes-port-forward-proxy-command.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/kubernetes-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/kubernetes-ssh-jump.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5676 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3898 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/paperspace-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/runpod-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/sky-serve-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/spot-controller.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/templates/vsphere-ray.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.327398 skypilot_nightly-1.0.0.dev20240421/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17601 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.327398 skypilot_nightly-1.0.0.dev20240421/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.327398 skypilot_nightly-1.0.0.dev20240421/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11032 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/cluster_yaml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18805 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/command_runner.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    22349 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25413 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/controller_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6260 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/env_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.331398 skypilot_nightly-1.0.0.dev20240421/sky/utils/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/kubernetes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9667 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/kubernetes/create_cluster.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      927 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/kubernetes/delete_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/kubernetes/generate_kind_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6960 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/kubernetes/gpu_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6560 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/kubernetes_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/resources_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/rich_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20387 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.335398 skypilot_nightly-1.0.0.dev20240421/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17869 2024-04-21 10:38:08.000000 skypilot_nightly-1.0.0.dev20240421/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9308 2024-04-21 10:38:08.000000 skypilot_nightly-1.0.0.dev20240421/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 10:38:08.000000 skypilot_nightly-1.0.0.dev20240421/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-21 10:38:08.000000 skypilot_nightly-1.0.0.dev20240421/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-21 10:38:08.000000 skypilot_nightly-1.0.0.dev20240421/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-21 10:38:08.000000 skypilot_nightly-1.0.0.dev20240421/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:38:08.335398 skypilot_nightly-1.0.0.dev20240421/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8789 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/tests/test_serve_autoscaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)   211236 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17581 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/tests/test_spot_serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/tests/test_wheels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-04-21 10:38:03.000000 skypilot_nightly-1.0.0.dev20240421/tests/test_yaml_parser.py
```

### Comparing `skypilot_nightly-1.0.0.dev20240420/LICENSE` & `skypilot_nightly-1.0.0.dev20240421/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/MANIFEST.in` & `skypilot_nightly-1.0.0.dev20240421/MANIFEST.in`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 include sky/backends/monkey_patches/*.py
 exclude sky/clouds/service_catalog/data_fetchers/analyze.py
+include sky/provision/kubernetes/manifests/*
 include sky/setup_files/*
 include sky/skylet/*.sh
 include sky/skylet/LICENSE
 include sky/skylet/providers/azure/*
 include sky/skylet/providers/gcp/*
 include sky/skylet/providers/ibm/*
 include sky/skylet/providers/kubernetes/*
```

### Comparing `skypilot_nightly-1.0.0.dev20240420/PKG-INFO` & `skypilot_nightly-1.0.0.dev20240421/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240420
+Version: 1.0.0.dev20240421
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot_nightly-1.0.0.dev20240420/README.md` & `skypilot_nightly-1.0.0.dev20240421/README.md`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/pyproject.toml` & `skypilot_nightly-1.0.0.dev20240421/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/setup.py` & `skypilot_nightly-1.0.0.dev20240421/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/__init__.py` & `skypilot_nightly-1.0.0.dev20240421/sky/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """The SkyPilot package."""
 import os
 import subprocess
 from typing import Optional
 import urllib.request
 
 # Replaced with the current commit when building the wheels.
-_SKYPILOT_COMMIT_SHA = '6eb1d97addc26916de9c6314f1deee04fae8d7c3'
+_SKYPILOT_COMMIT_SHA = '118fc79b98b974ae10ccdeebb0ab6cc7f9792795'
 
 
 def _get_git_commit():
     if 'SKYPILOT_COMMIT_SHA' not in _SKYPILOT_COMMIT_SHA:
         # This is a release build, so we don't need to get the commit hash from
         # git, as it's already been set.
         return _SKYPILOT_COMMIT_SHA
@@ -31,15 +31,15 @@
             commit_hash += '-dirty'
         return commit_hash
     except Exception:  # pylint: disable=broad-except
         return _SKYPILOT_COMMIT_SHA
 
 
 __commit__ = _get_git_commit()
-__version__ = '1.0.0.dev20240420'
+__version__ = '1.0.0.dev20240421'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 
 # ---------------------- Proxy Configuration ---------------------- #
 def _set_http_proxy_env_vars() -> None:
     urllib_proxies = dict(urllib.request.getproxies())
```

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/adaptors/aws.py` & `skypilot_nightly-1.0.0.dev20240421/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/adaptors/azure.py` & `skypilot_nightly-1.0.0.dev20240421/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/adaptors/cloudflare.py` & `skypilot_nightly-1.0.0.dev20240421/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/adaptors/common.py` & `skypilot_nightly-1.0.0.dev20240421/sky/adaptors/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/adaptors/gcp.py` & `skypilot_nightly-1.0.0.dev20240421/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/adaptors/ibm.py` & `skypilot_nightly-1.0.0.dev20240421/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/adaptors/kubernetes.py` & `skypilot_nightly-1.0.0.dev20240421/sky/adaptors/kubernetes.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 _configured = False
 _core_api = None
 _auth_api = None
 _networking_api = None
 _custom_objects_api = None
 _node_api = None
+_apps_api = None
 
 # Timeout to use for API calls
 API_TIMEOUT = 5
 
 
 def _load_config():
     global _configured
@@ -104,14 +105,23 @@
     if _node_api is None:
         _load_config()
         _node_api = kubernetes.client.NodeV1Api()
 
     return _node_api
 
 
+def apps_api():
+    global _apps_api
+    if _apps_api is None:
+        _load_config()
+        _apps_api = kubernetes.client.AppsV1Api()
+
+    return _apps_api
+
+
 def api_exception():
     return kubernetes.client.rest.ApiException
 
 
 def config_exception():
     return kubernetes.config.config_exception.ConfigException
```

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/adaptors/oci.py` & `skypilot_nightly-1.0.0.dev20240421/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/adaptors/vsphere.py` & `skypilot_nightly-1.0.0.dev20240421/sky/adaptors/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/authentication.py` & `skypilot_nightly-1.0.0.dev20240421/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/backends/__init__.py` & `skypilot_nightly-1.0.0.dev20240421/sky/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/backends/backend.py` & `skypilot_nightly-1.0.0.dev20240421/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/backends/backend_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/backends/backend_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/backends/cloud_vm_ray_backend.py` & `skypilot_nightly-1.0.0.dev20240421/sky/backends/cloud_vm_ray_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -2557,14 +2557,25 @@
                                 'does not have zone specified.')
                     with ux_utils.print_exception_no_traceback():
                         raise exceptions.ResourcesMismatchError(
                             f'Task requested resources {example_resource} in zone '  # pylint: disable=line-too-long
                             f'{example_resource.zone!r},'
                             'but the existing cluster '
                             f'{zone_str}')
+                if (example_resource.requires_fuse and
+                        not launched_resources.requires_fuse):
+                    # Will not be reached for non-k8s case since the
+                    # less_demanding_than only fails fuse requirement when
+                    # the cloud is Kubernetes AND the cluster doesn't have fuse.
+                    with ux_utils.print_exception_no_traceback():
+                        raise exceptions.ResourcesMismatchError(
+                            'Task requires FUSE support for mounting object '
+                            'stores, but the existing cluster with '
+                            f'{launched_resources!r} does not support FUSE '
+                            f'mounting. Launch a new cluster to run this task.')
             requested_resource_str = ', '.join(requested_resource_list)
             if isinstance(task.resources, list):
                 requested_resource_str = f'[{requested_resource_str}]'
             elif isinstance(task.resources, set):
                 requested_resource_str = f'{{{requested_resource_str}}}'
             with ux_utils.print_exception_no_traceback():
                 raise exceptions.ResourcesMismatchError(
```

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/backends/docker_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/backends/local_docker_backend.py` & `skypilot_nightly-1.0.0.dev20240421/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot_nightly-1.0.0.dev20240421/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/backends/wheel_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/benchmark/benchmark_state.py` & `skypilot_nightly-1.0.0.dev20240421/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/benchmark/benchmark_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/check.py` & `skypilot_nightly-1.0.0.dev20240421/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/cli.py` & `skypilot_nightly-1.0.0.dev20240421/sky/cli.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/cloud_stores.py` & `skypilot_nightly-1.0.0.dev20240421/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/__init__.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/aws.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/azure.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/cloud.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/cloud_registry.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/cloud_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/cudo.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/fluidstack.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/gcp.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/ibm.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/kubernetes.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/kubernetes.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,19 @@
 
 logger = sky_logging.init_logger(__name__)
 
 # Check if KUBECONFIG is set, and use it if it is.
 DEFAULT_KUBECONFIG_PATH = '~/.kube/config'
 CREDENTIAL_PATH = os.environ.get('KUBECONFIG', DEFAULT_KUBECONFIG_PATH)
 
+# Namespace for SkyPilot resources shared across multiple tenants on the
+# same cluster (even if they might be running in different namespaces).
+# E.g., FUSE device manager daemonset is run in this namespace.
+_SKY_SYSTEM_NAMESPACE = 'skypilot-system'
+
 
 @clouds.CLOUD_REGISTRY.register
 class Kubernetes(clouds.Cloud):
     """Kubernetes."""
 
     SKY_SSH_KEY_SECRET_NAME = 'sky-ssh-keys'
     SKY_SSH_KEY_SECRET_FIELD_NAME = \
@@ -251,14 +256,16 @@
         # If GPUs are requested, set node label to match the GPU type.
         if acc_count > 0 and acc_type is not None:
             k8s_acc_label_key, k8s_acc_label_value = \
                 kubernetes_utils.get_gpu_label_key_value(acc_type)
 
         port_mode = network_utils.get_port_mode(None)
 
+        fuse_device_required = bool(resources.requires_fuse)
+
         deploy_vars = {
             'instance_type': resources.instance_type,
             'custom_resources': custom_resources,
             'region': region.name,
             'cpus': str(cpus),
             'memory': str(mem),
             'accelerator_count': str(acc_count),
@@ -267,14 +274,17 @@
                 kubernetes_utils.get_current_kube_config_context_namespace(),
             'k8s_port_mode': port_mode.value,
             'k8s_ssh_key_secret_name': self.SKY_SSH_KEY_SECRET_NAME,
             'k8s_acc_label_key': k8s_acc_label_key,
             'k8s_acc_label_value': k8s_acc_label_value,
             'k8s_ssh_jump_name': self.SKY_SSH_JUMP_NAME,
             'k8s_ssh_jump_image': ssh_jump_image,
+            'k8s_fuse_device_required': fuse_device_required,
+            # Namespace to run the FUSE device manager in
+            'k8s_fuse_device_manager_namespace': _SKY_SYSTEM_NAMESPACE,
             'image_id': image_id,
         }
 
         return deploy_vars
 
     def _get_feasible_launchable_resources(
         self, resources: 'resources_lib.Resources'
```

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/lambda_cloud.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/oci.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/paperspace.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/paperspace.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/runpod.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/runpod.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/scp.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/scp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/__init__.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/aws_catalog.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/azure_catalog.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/common.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/config.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/cudo_catalog.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/cudo_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/data_fetchers/fetch_cudo.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/data_fetchers/fetch_fluidstack.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/data_fetchers/fetch_vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/fluidstack_catalog.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/fluidstack_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/kubernetes_catalog.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/kubernetes_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/oci_catalog.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/paperspace_catalog.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/paperspace_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/runpod_catalog.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/runpod_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/scp_catalog.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/service_catalog/vsphere_catalog.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/service_catalog/vsphere_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/utils/gcp_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/utils/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/utils/lambda_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/utils/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/utils/oci_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/utils/oci_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/utils/scp_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/utils/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/clouds/vsphere.py` & `skypilot_nightly-1.0.0.dev20240421/sky/clouds/vsphere.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/core.py` & `skypilot_nightly-1.0.0.dev20240421/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/dag.py` & `skypilot_nightly-1.0.0.dev20240421/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/data/data_transfer.py` & `skypilot_nightly-1.0.0.dev20240421/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/data/data_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/data/mounting_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/data/storage.py` & `skypilot_nightly-1.0.0.dev20240421/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/data/storage_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/exceptions.py` & `skypilot_nightly-1.0.0.dev20240421/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/execution.py` & `skypilot_nightly-1.0.0.dev20240421/sky/execution.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/global_user_state.py` & `skypilot_nightly-1.0.0.dev20240421/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/optimizer.py` & `skypilot_nightly-1.0.0.dev20240421/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/__init__.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/aws/__init__.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/aws/config.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/aws/instance.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/aws/utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/azure/instance.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/azure/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/common.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/common.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/cudo/__init__.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/cudo/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/cudo/cudo_machine_type.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/cudo/cudo_machine_type.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/cudo/cudo_wrapper.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/cudo/cudo_wrapper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/cudo/instance.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/cudo/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/docker_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/fluidstack/__init__.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/fluidstack/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/fluidstack/fluidstack_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/fluidstack/fluidstack_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/fluidstack/instance.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/fluidstack/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/gcp/__init__.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/gcp/config.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/gcp/constants.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/gcp/instance.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/gcp/instance_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/instance_setup.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/instance_setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/kubernetes/__init__.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/kubernetes/config.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/kubernetes/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Kubernetes-specific configuration for the provisioner."""
 import copy
 import logging
 import math
+import os
 from typing import Any, Dict, Union
 
+import yaml
+
 from sky.adaptors import kubernetes
 from sky.provision import common
 from sky.provision.kubernetes import utils as kubernetes_utils
 
 logger = logging.getLogger(__name__)
 
 # Timeout for deleting a Kubernetes resource (in seconds).
@@ -20,14 +23,17 @@
     del region, cluster_name  # unused
     namespace = kubernetes_utils.get_current_kube_config_context_namespace()
 
     _configure_services(namespace, config.provider_config)
 
     config = _configure_ssh_jump(namespace, config)
 
+    if config.provider_config.get('fuse_device_required', False):
+        _configure_fuse_mounting(config.provider_config)
+
     if not config.provider_config.get('_operator'):
         # These steps are unecessary when using the Operator.
         _configure_autoscaler_service_account(namespace, config.provider_config)
         _configure_autoscaler_role(namespace, config.provider_config)
         _configure_autoscaler_role_binding(namespace, config.provider_config)
 
     return config
@@ -307,14 +313,81 @@
     #  service is missing, we should raise an error.
 
     kubernetes_utils.setup_ssh_jump_pod(ssh_jump_name, ssh_jump_image,
                                         ssh_key_secret_name, namespace)
     return config
 
 
+def _configure_fuse_mounting(provider_config: Dict[str, Any]) -> None:
+    """Creates sidecars required for FUSE mounting.
+
+    FUSE mounting in Kubernetes without privileged containers requires us to
+    run a sidecar container with the necessary capabilities. We run a daemonset
+    which exposes the host /dev/fuse device as a Kubernetes resource. The
+    SkyPilot pod requests this resource to mount the FUSE filesystem.
+
+    We create this daemonset in a common namespace, which is configurable in the
+    provider config. This allows the FUSE mounting sidecar to be shared across
+    multiple tenants. The default namespace is 'sky-system' (populated in
+    clouds.Kubernetes)
+    """
+
+    logger.info('_configure_fuse_mounting: Setting up FUSE device manager.')
+
+    fuse_device_manager_namespace = provider_config.get(
+        'fuse_device_manager_namespace', 'default')
+    kubernetes_utils.create_namespace(fuse_device_manager_namespace)
+
+    # Read the device manager YAMLs from the manifests directory
+    root_dir = os.path.dirname(os.path.dirname(__file__))
+
+    # Load and create the ConfigMap
+    logger.info('_configure_fuse_mounting: Creating configmap.')
+    config_map_path = os.path.join(
+        root_dir, 'kubernetes/manifests/smarter-device-manager-configmap.yaml')
+    with open(config_map_path, 'r', encoding='utf-8') as file:
+        config_map = yaml.safe_load(file)
+    kubernetes_utils.merge_custom_metadata(config_map['metadata'])
+    try:
+        kubernetes.core_api().create_namespaced_config_map(
+            fuse_device_manager_namespace, config_map)
+    except kubernetes.api_exception() as e:
+        if e.status == 409:
+            logger.info('_configure_fuse_mounting: ConfigMap already exists '
+                        f'in namespace {fuse_device_manager_namespace!r}')
+        else:
+            raise
+    else:
+        logger.info('_configure_fuse_mounting: ConfigMap created '
+                    f'in namespace {fuse_device_manager_namespace!r}')
+
+    # Load and create the DaemonSet
+    logger.info('_configure_fuse_mounting: Creating daemonset.')
+    daemonset_path = os.path.join(
+        root_dir, 'kubernetes/manifests/smarter-device-manager-daemonset.yaml')
+    with open(daemonset_path, 'r', encoding='utf-8') as file:
+        daemonset = yaml.safe_load(file)
+    kubernetes_utils.merge_custom_metadata(daemonset['metadata'])
+    try:
+        kubernetes.apps_api().create_namespaced_daemon_set(
+            fuse_device_manager_namespace, daemonset)
+    except kubernetes.api_exception() as e:
+        if e.status == 409:
+            logger.info('_configure_fuse_mounting: DaemonSet already exists '
+                        f'in namespace {fuse_device_manager_namespace!r}')
+        else:
+            raise
+    else:
+        logger.info('_configure_fuse_mounting: DaemonSet created '
+                    f'in namespace {fuse_device_manager_namespace!r}')
+
+    logger.info('FUSE device manager setup complete '
+                f'in namespace {fuse_device_manager_namespace!r}')
+
+
 def _configure_services(namespace: str, provider_config: Dict[str,
                                                               Any]) -> None:
     service_field = 'services'
     if service_field not in provider_config:
         logger.info(f'_configure_services: {not_provided_msg(service_field)}')
         return
```

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/kubernetes/instance.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/kubernetes/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/kubernetes/network.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/kubernetes/network.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/kubernetes/network_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/kubernetes/network_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/kubernetes/utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/kubernetes/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1267,7 +1267,28 @@
             secret_name, namespace, _request_timeout=kubernetes.API_TIMEOUT)
     except kubernetes.api_exception() as e:
         if e.status == 404:
             return False
         raise
     else:
         return True
+
+
+def create_namespace(namespace: str) -> None:
+    """Creates a namespace in the cluster.
+
+    If the namespace already exists, logs a message and does nothing.
+
+    Args:
+        namespace: Name of the namespace to create
+    """
+    kubernetes_client = kubernetes.kubernetes.client
+    ns_metadata = dict(name=namespace, labels={'parent': 'skypilot'})
+    merge_custom_metadata(ns_metadata)
+    namespace_obj = kubernetes_client.V1Namespace(metadata=ns_metadata)
+    try:
+        kubernetes.core_api().create_namespace(namespace_obj)
+    except kubernetes.api_exception() as e:
+        if e.status == 409:
+            logger.info(f'Namespace {namespace} already exists in the cluster.')
+        else:
+            raise
```

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/logging.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/logging.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/metadata_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/paperspace/__init__.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/paperspace/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/paperspace/config.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/paperspace/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/paperspace/constants.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/paperspace/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/paperspace/instance.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/paperspace/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/paperspace/utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/paperspace/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/provisioner.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/provisioner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/runpod/instance.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/runpod/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/runpod/utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/runpod/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/__init__.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/cls_api_client.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/cls_api_client.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/cls_api_helper.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/cls_api_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/metadata_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/metadata_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/service_manager.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/service_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/service_manager_factory.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/service_manager_factory.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/ssl_helper.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/ssl_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/vapiconnect.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/vapiconnect.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/common/vim_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/common/vim_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/instance.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/provision/vsphere/vsphere_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/provision/vsphere/vsphere_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/resources.py` & `skypilot_nightly-1.0.0.dev20240421/sky/resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     * as a "filter" to get concrete launchable instances
     * for calculating billing
     * for provisioning on a cloud
 
     """
     # If any fields changed, increment the version. For backward compatibility,
     # modify the __setstate__ method to handle the old version.
-    _VERSION = 15
+    _VERSION = 16
 
     def __init__(
         self,
         cloud: Optional[clouds.Cloud] = None,
         instance_type: Optional[str] = None,
         cpus: Union[None, int, float, str] = None,
         memory: Union[None, int, float, str] = None,
@@ -61,14 +61,15 @@
         disk_size: Optional[int] = None,
         disk_tier: Optional[Union[str, resources_utils.DiskTier]] = None,
         ports: Optional[Union[int, str, List[str], Tuple[str]]] = None,
         # Internal use only.
         # pylint: disable=invalid-name
         _docker_login_config: Optional[docker_utils.DockerLoginConfig] = None,
         _is_image_managed: Optional[bool] = None,
+        _requires_fuse: Optional[bool] = None,
     ):
         """Initialize a Resources object.
 
         All fields are optional.  ``Resources.is_launchable`` decides whether
         the Resources is fully specified to launch an instance.
 
         Examples:
@@ -127,14 +128,19 @@
           disk_size: the size of the OS disk in GiB.
           disk_tier: the disk performance tier to use. If None, defaults to
             ``'medium'``.
           ports: the ports to open on the instance.
           _docker_login_config: the docker configuration to use. This include
             the docker username, password, and registry server. If None, skip
             docker login.
+          _requires_fuse: whether the task requires FUSE mounting support. This
+            is used internally by certain cloud implementations to do additional
+            setup for FUSE mounting. This flag also safeguards against using
+            FUSE mounting on existing clusters that do not support it. If None,
+            defaults to False.
 
         Raises:
             ValueError: if some attributes are invalid.
             exceptions.NoCloudAccessError: if no public cloud is enabled.
         """
         self._version = self._VERSION
         self._cloud = cloud
@@ -196,14 +202,17 @@
                 # Set to None if empty. This is mainly for resources from
                 # cli, which will comes in as an empty tuple.
                 ports = None
         self._ports = ports
 
         self._docker_login_config = _docker_login_config
 
+        self._requires_fuse = (_requires_fuse
+                               if _requires_fuse is not None else False)
+
         self._set_cpus(cpus)
         self._set_memory(memory)
         self._set_accelerators(accelerators, accelerator_args)
 
         self._try_validate_instance_type()
         self._try_validate_cpus_mem()
         self._try_validate_spot()
@@ -408,14 +417,22 @@
     def ports(self) -> Optional[List[str]]:
         return self._ports
 
     @property
     def is_image_managed(self) -> Optional[bool]:
         return self._is_image_managed
 
+    @property
+    def requires_fuse(self) -> Optional[bool]:
+        return self._requires_fuse
+
+    @requires_fuse.setter
+    def requires_fuse(self, value: Optional[bool]) -> None:
+        self._requires_fuse = value
+
     def _set_cpus(
         self,
         cpus: Union[None, int, float, str],
     ) -> None:
         if cpus is None:
             self._cpus = None
             return
@@ -1067,14 +1084,21 @@
                 if other.ports is None:
                     return False
                 self_ports = resources_utils.port_ranges_to_set(self.ports)
                 other_ports = resources_utils.port_ranges_to_set(other.ports)
                 if not self_ports <= other_ports:
                     return False
 
+        if self.requires_fuse and not other.requires_fuse:
+            # On Kubernetes, we can't launch a task that requires FUSE on a pod
+            # that wasn't initialized with FUSE support at the start.
+            # Other clouds don't have this limitation.
+            if other.cloud.is_same_cloud(clouds.Kubernetes()):
+                return False
+
         # self <= other
         return True
 
     def should_be_blocked_by(self, blocked: 'Resources') -> bool:
         """Whether this Resources matches the blocked Resources.
 
         If a field in `blocked` is None, it should be considered as a wildcard
@@ -1132,14 +1156,15 @@
             image_id=override.pop('image_id', self.image_id),
             disk_tier=override.pop('disk_tier', self.disk_tier),
             ports=override.pop('ports', self.ports),
             _docker_login_config=override.pop('_docker_login_config',
                                               self._docker_login_config),
             _is_image_managed=override.pop('_is_image_managed',
                                            self._is_image_managed),
+            _requires_fuse=override.pop('_requires_fuse', self._requires_fuse),
         )
         assert len(override) == 0
         return resources
 
     def valid_on_region_zones(self, region: str, zones: List[str]) -> bool:
         """Returns whether this Resources is valid on given region and zones"""
         if self.region is not None and self.region != region:
@@ -1270,14 +1295,15 @@
         resources_fields['image_id'] = config.pop('image_id', None)
         resources_fields['disk_tier'] = config.pop('disk_tier', None)
         resources_fields['ports'] = config.pop('ports', None)
         resources_fields['_docker_login_config'] = config.pop(
             '_docker_login_config', None)
         resources_fields['_is_image_managed'] = config.pop(
             '_is_image_managed', None)
+        resources_fields['_requires_fuse'] = config.pop('_requires_fuse', None)
 
         if resources_fields['cpus'] is not None:
             resources_fields['cpus'] = str(resources_fields['cpus'])
         if resources_fields['memory'] is not None:
             resources_fields['memory'] = str(resources_fields['memory'])
         if resources_fields['accelerator_args'] is not None:
             resources_fields['accelerator_args'] = dict(
@@ -1311,14 +1337,16 @@
         add_if_not_none('zone', self.zone)
         add_if_not_none('image_id', self.image_id)
         if self.disk_tier is not None:
             config['disk_tier'] = self.disk_tier.value
         add_if_not_none('ports', self.ports)
         if self._is_image_managed is not None:
             config['_is_image_managed'] = self._is_image_managed
+        if self._requires_fuse is not None:
+            config['_requires_fuse'] = self._requires_fuse
         return config
 
     def __setstate__(self, state):
         """Set state from pickled state, for backward compatibility."""
         self._version = self._VERSION
 
         # TODO (zhwu): Design our persistent state format with `__getstate__`,
@@ -1408,8 +1436,14 @@
 
         if version < 15:
             original_disk_tier = state.get('_disk_tier', None)
             if original_disk_tier is not None:
                 state['_disk_tier'] = resources_utils.DiskTier(
                     original_disk_tier)
 
+        if version < 16:
+            # Kubernetes clusters launched prior to version 16 run in privileged
+            # mode and have FUSE support enabled by default. As a result, we
+            # set the default to True for backward compatibility.
+            state['_requires_fuse'] = state.get('_requires_fuse', True)
+
         self.__dict__.update(state)
```

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/serve/__init__.py` & `skypilot_nightly-1.0.0.dev20240421/sky/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/serve/autoscalers.py` & `skypilot_nightly-1.0.0.dev20240421/sky/serve/autoscalers.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/serve/constants.py` & `skypilot_nightly-1.0.0.dev20240421/sky/serve/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/serve/controller.py` & `skypilot_nightly-1.0.0.dev20240421/sky/serve/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/serve/core.py` & `skypilot_nightly-1.0.0.dev20240421/sky/serve/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/serve/load_balancer.py` & `skypilot_nightly-1.0.0.dev20240421/sky/serve/load_balancer.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/serve/load_balancing_policies.py` & `skypilot_nightly-1.0.0.dev20240421/sky/serve/load_balancing_policies.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/serve/replica_managers.py` & `skypilot_nightly-1.0.0.dev20240421/sky/serve/replica_managers.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/serve/serve_state.py` & `skypilot_nightly-1.0.0.dev20240421/sky/serve/serve_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/serve/serve_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/serve/serve_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/serve/service.py` & `skypilot_nightly-1.0.0.dev20240421/sky/serve/service.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/serve/service_spec.py` & `skypilot_nightly-1.0.0.dev20240421/sky/serve/service_spec.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/setup_files/MANIFEST.in` & `skypilot_nightly-1.0.0.dev20240421/sky/setup_files/MANIFEST.in`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 include sky/backends/monkey_patches/*.py
 exclude sky/clouds/service_catalog/data_fetchers/analyze.py
+include sky/provision/kubernetes/manifests/*
 include sky/setup_files/*
 include sky/skylet/*.sh
 include sky/skylet/LICENSE
 include sky/skylet/providers/azure/*
 include sky/skylet/providers/gcp/*
 include sky/skylet/providers/ibm/*
 include sky/skylet/providers/kubernetes/*
```

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/setup_files/setup.py` & `skypilot_nightly-1.0.0.dev20240421/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/sky_logging.py` & `skypilot_nightly-1.0.0.dev20240421/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/LICENSE` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/attempt_skylet.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/autostop_lib.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/configs.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/constants.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/events.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/job_lib.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/log_lib.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/log_lib.pyi` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/log_lib.pyi`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/azure/azure-config-template.json` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/azure/config.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/azure/node_provider.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/command_runner.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/ibm/node_provider.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/ibm/utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/oci/node_provider.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/oci/query_helper.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/scp/config.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/providers/scp/node_provider.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/ray_patches/__init__.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/ray_patches/worker.py.patch` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/skylet.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skylet/subprocess_daemon.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/skypilot_config.py` & `skypilot_nightly-1.0.0.dev20240421/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/spot/__init__.py` & `skypilot_nightly-1.0.0.dev20240421/sky/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/spot/constants.py` & `skypilot_nightly-1.0.0.dev20240421/sky/spot/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/spot/controller.py` & `skypilot_nightly-1.0.0.dev20240421/sky/spot/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/spot/core.py` & `skypilot_nightly-1.0.0.dev20240421/sky/spot/core.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/spot/dashboard/dashboard.py` & `skypilot_nightly-1.0.0.dev20240421/sky/spot/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/spot/dashboard/static/favicon.ico` & `skypilot_nightly-1.0.0.dev20240421/sky/spot/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/spot/dashboard/templates/index.html` & `skypilot_nightly-1.0.0.dev20240421/sky/spot/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/spot/recovery_strategy.py` & `skypilot_nightly-1.0.0.dev20240421/sky/spot/recovery_strategy.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/spot/spot_state.py` & `skypilot_nightly-1.0.0.dev20240421/sky/spot/spot_state.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/spot/spot_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/spot/spot_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/status_lib.py` & `skypilot_nightly-1.0.0.dev20240421/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/task.py` & `skypilot_nightly-1.0.0.dev20240421/sky/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 logger = sky_logging.init_logger(__name__)
 
 # A lambda generating commands (node rank_i, node addrs -> cmd_i).
 CommandGen = Callable[[int, List[str]], Optional[str]]
 CommandOrCommandGen = Union[str, CommandGen]
 
-_VALID_NAME_REGEX = '[a-z0-9]+(?:[._-]{1,2}[a-z0-9]+)*'
+_VALID_NAME_REGEX = '[a-zA-Z0-9]+(?:[._-]{1,2}[a-zA-Z0-9]+)*'
 _VALID_NAME_DESCR = ('ASCII characters and may contain lowercase and'
                      ' uppercase letters, digits, underscores, periods,'
                      ' and dashes. Must start and end with alphanumeric'
                      ' characters. No triple dashes or underscores.')
 
 _RUN_FN_CHECK_FAIL_MSG = (
     'run command generator must take exactly 2 arguments: node_rank (int) and'
@@ -612,14 +612,22 @@
         Returns:
           self: The current task, with resources set.
         """
         if isinstance(resources, sky.Resources):
             resources = {resources}
         # TODO(woosuk): Check if the resources are None.
         self.resources = _with_docker_login_config(resources, self.envs)
+
+        # Evaluate if the task requires FUSE and set the requires_fuse flag
+        for _, storage_obj in self.storage_mounts.items():
+            if storage_obj.mode == storage_lib.StorageMode.MOUNT:
+                for r in self.resources:
+                    r.requires_fuse = True
+                break
+
         return self
 
     def set_resources_override(self, override_params: Dict[str, Any]) -> 'Task':
         """Sets the override parameters for the resources."""
         new_resources_list = []
         for res in list(self.resources):
             new_resources = res.copy(**override_params)
@@ -801,16 +809,19 @@
           self: The current task, with storage mounts set.
 
         Raises:
           ValueError: if input paths are invalid.
         """
         if storage_mounts is None:
             self.storage_mounts = {}
+            # Clear the requires_fuse flag if no storage mounts are set.
+            for r in self.resources:
+                r.requires_fuse = False
             return self
-        for target, _ in storage_mounts.items():
+        for target, storage_obj in storage_mounts.items():
             # TODO(zhwu): /home/username/sky_workdir as the target path need
             # to be filtered out as well.
             if (target == constants.SKY_REMOTE_WORKDIR and
                     self.workdir is not None):
                 with ux_utils.print_exception_no_traceback():
                     raise ValueError(
                         f'Cannot use {constants.SKY_REMOTE_WORKDIR!r} as a '
@@ -820,14 +831,20 @@
                         'the file/folder.')
 
             if data_utils.is_cloud_store_url(target):
                 with ux_utils.print_exception_no_traceback():
                     raise ValueError(
                         'Storage mount destination path cannot be cloud storage'
                     )
+
+            if storage_obj.mode == storage_lib.StorageMode.MOUNT:
+                # If any storage is using MOUNT mode, we need to enable FUSE in
+                # the resources.
+                for r in self.resources:
+                    r.requires_fuse = True
         # Storage source validation is done in Storage object
         self.storage_mounts = storage_mounts
         return self
 
     def update_storage_mounts(
             self, storage_mounts: Dict[str, storage_lib.Storage]) -> 'Task':
         """Updates the storage mounts for this task.
```

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/aws-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/azure-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/cudo-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/cudo-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/fluidstack-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/fluidstack-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/gcp-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/gcp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/ibm-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/kubernetes-ingress.yml.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/kubernetes-ingress.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/kubernetes-port-forward-proxy-command.sh.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/kubernetes-port-forward-proxy-command.sh.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/kubernetes-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/kubernetes-ray.yml.j2`

 * *Files 18% similar despite different names*

```diff
@@ -29,14 +29,19 @@
     # head node.
     use_internal_ips: true
 
     timeout: {{timeout}}
 
     ssh_jump_image: {{k8s_ssh_jump_image}}
 
+    # Boolean flag to indicate if the cluster requires FUSE mounting.
+    # Used to set up the necessary permissions and sidecars.
+    fuse_device_required: {{k8s_fuse_device_required}}
+    fuse_device_manager_namespace: {{k8s_fuse_device_manager_namespace}}
+
     # ServiceAccount created by the autoscaler for the head node pod that it
     # runs in. If this field isn't provided, the head pod config below must
     # contain a user-created service account with the proper permissions.
     autoscaler_service_account:
         apiVersion: v1
         kind: ServiceAccount
         metadata:
@@ -135,14 +140,19 @@
         # service is required.
         labels:
             parent: skypilot
             # component will be set for the head node pod to be the same as the head node service selector above if a 
             skypilot-cluster: {{cluster_name_on_cloud}}
             # Identifies the SSH jump pod used by this pod. Used in life cycle management of the ssh jump pod.
             skypilot-ssh-jump: {{k8s_ssh_jump_name}}
+        {% if k8s_fuse_device_required %}
+        annotations:
+            # Required for FUSE mounting to access /dev/fuse
+            container.apparmor.security.beta.kubernetes.io/ray-node: unconfined
+        {% endif %}
       spec:
         # Change this if you altered the autoscaler_service_account above
         # or want to provide your own.
         serviceAccountName: skypilot-service-account
 
         restartPolicy: Never
 
@@ -182,27 +192,40 @@
           # This volume allocates shared memory for Ray to use for its plasma
           # object store. If you do not provide this, Ray will fall back to
           # /tmp which cause slowdowns if is not a shared memory volume.
           volumeMounts:
           - name: secret-volume
             readOnly: true
             mountPath: "/etc/secret-volume"
+          # This volume allocates shared memory for Ray to use for its plasma
+          # object store. If you do not provide this, Ray will fall back to
+          # /tmp which cause slowdowns if is not a shared memory volume.
           - mountPath: /dev/shm
             name: dshm
-          - mountPath: /dev/fuse    # Required for FUSE mounting
-            name: dev-fuse
-          securityContext:          # Required for FUSE mounting. TODO(romilb): See if we can grant a reduced set of privileges.
-            privileged: true
+          {% if k8s_fuse_device_required %}
+          securityContext:
+            capabilities:
+              add:
+                - "SYS_ADMIN"
+          {% endif %}
           resources:
             requests:
               cpu: {{cpus}}
               memory: {{memory}}G
               nvidia.com/gpu: {{accelerator_count}}
+              {% if k8s_fuse_device_required %}
+              # Kubernetes resource exposed by the fuse device manager
+              # https://gitlab.com/arm-research/smarter/smarter-device-manager
+              smarter-devices/fuse: "1"
+              {% endif %}
             limits:
               nvidia.com/gpu: {{accelerator_count}} # Limits need to be defined for GPU requests
+              {% if k8s_fuse_device_required %}
+              smarter-devices/fuse: "1"
+              {% endif %}
 
 setup_commands:
   # Disable `unattended-upgrades` to prevent apt-get from hanging. It should be called at the beginning before the process started to avoid being blocked. (This is a temporary fix.)
   # Create ~/.ssh/config file in case the file does not exist in the image.
   # Line 'sudo bash ..': set the ulimit as suggested by ray docs for performance. https://docs.ray.io/en/latest/cluster/vms/user-guides/large-cluster-best-practices.html#system-configuration
   # Line 'sudo grep ..': set the number of threads per process to unlimited to avoid ray job submit stucking issue when the number of running ray jobs increase.
   # Line 'mkdir -p ..': disable host key check
```

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/kubernetes-ssh-jump.yml.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/kubernetes-ssh-jump.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/lambda-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/local-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/oci-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/paperspace-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/paperspace-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/runpod-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/runpod-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/scp-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/sky-serve-controller.yaml.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/sky-serve-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/spot-controller.yaml.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/spot-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/templates/vsphere-ray.yml.j2` & `skypilot_nightly-1.0.0.dev20240421/sky/templates/vsphere-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/usage/constants.py` & `skypilot_nightly-1.0.0.dev20240421/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/usage/usage_lib.py` & `skypilot_nightly-1.0.0.dev20240421/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/accelerator_registry.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/cli_utils/status_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/cluster_yaml_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/cluster_yaml_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/command_runner.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/command_runner.pyi` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/command_runner.pyi`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/common_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/controller_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/controller_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/dag_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/db_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/env_options.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/kubernetes/create_cluster.sh` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/kubernetes/create_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/kubernetes/delete_cluster.sh` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/kubernetes/delete_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/kubernetes/generate_kind_config.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/kubernetes/generate_kind_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/kubernetes/gpu_labeler.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/kubernetes/gpu_labeler.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/kubernetes/k8s_gpu_labeler_job.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/kubernetes/k8s_gpu_labeler_setup.yaml`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/kubernetes/ssh_jump_lifecycle_manager.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/kubernetes_enums.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/kubernetes_enums.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/log_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/resources_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/resources_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/rich_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/rich_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/schemas.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/subprocess_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/timeline.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/ux_utils.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/sky/utils/validator.py` & `skypilot_nightly-1.0.0.dev20240421/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/skypilot_nightly.egg-info/PKG-INFO` & `skypilot_nightly-1.0.0.dev20240421/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20240420
+Version: 1.0.0.dev20240421
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

### Comparing `skypilot_nightly-1.0.0.dev20240420/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot_nightly-1.0.0.dev20240421/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,16 @@
 sky/provision/gcp/instance_utils.py
 sky/provision/kubernetes/__init__.py
 sky/provision/kubernetes/config.py
 sky/provision/kubernetes/instance.py
 sky/provision/kubernetes/network.py
 sky/provision/kubernetes/network_utils.py
 sky/provision/kubernetes/utils.py
+sky/provision/kubernetes/manifests/smarter-device-manager-configmap.yaml
+sky/provision/kubernetes/manifests/smarter-device-manager-daemonset.yaml
 sky/provision/paperspace/__init__.py
 sky/provision/paperspace/config.py
 sky/provision/paperspace/constants.py
 sky/provision/paperspace/instance.py
 sky/provision/paperspace/utils.py
 sky/provision/runpod/__init__.py
 sky/provision/runpod/config.py
```

### Comparing `skypilot_nightly-1.0.0.dev20240420/skypilot_nightly.egg-info/requires.txt` & `skypilot_nightly-1.0.0.dev20240421/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/tests/test_cli.py` & `skypilot_nightly-1.0.0.dev20240421/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/tests/test_config.py` & `skypilot_nightly-1.0.0.dev20240421/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/tests/test_jobs.py` & `skypilot_nightly-1.0.0.dev20240421/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/tests/test_list_accelerators.py` & `skypilot_nightly-1.0.0.dev20240421/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/tests/test_optimizer_dryruns.py` & `skypilot_nightly-1.0.0.dev20240421/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/tests/test_optimizer_random_dag.py` & `skypilot_nightly-1.0.0.dev20240421/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/tests/test_serve_autoscaler.py` & `skypilot_nightly-1.0.0.dev20240421/tests/test_serve_autoscaler.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/tests/test_smoke.py` & `skypilot_nightly-1.0.0.dev20240421/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/tests/test_spot_serve.py` & `skypilot_nightly-1.0.0.dev20240421/tests/test_spot_serve.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/tests/test_storage.py` & `skypilot_nightly-1.0.0.dev20240421/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/tests/test_wheels.py` & `skypilot_nightly-1.0.0.dev20240421/tests/test_wheels.py`

 * *Files identical despite different names*

### Comparing `skypilot_nightly-1.0.0.dev20240420/tests/test_yaml_parser.py` & `skypilot_nightly-1.0.0.dev20240421/tests/test_yaml_parser.py`

 * *Files identical despite different names*

