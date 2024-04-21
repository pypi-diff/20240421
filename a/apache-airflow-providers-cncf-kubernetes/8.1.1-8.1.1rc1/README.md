# Comparing `tmp/apache_airflow_providers_cncf_kubernetes-8.1.1.tar.gz` & `tmp/apache_airflow_providers_cncf_kubernetes-8.1.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache_airflow_providers_cncf_kubernetes-8.1.1.tar", last modified: Tue Apr 16 07:37:35 2024, max compression
+gzip compressed data, was "apache_airflow_providers_cncf_kubernetes-8.1.1rc1.tar", last modified: Tue Apr 16 07:37:35 2024, max compression
```

## Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1.tar` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     3337 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/README.rst
--rw-r--r--   0        0        0    13569 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/LICENSE
--rw-r--r--   0        0        0     1590 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/__init__.py
--rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
--rw-r--r--   0        0        0     3967 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
--rw-r--r--   0        0        0     4094 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/callbacks.py
--rw-r--r--   0        0        0      787 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/decorators/__init__.py
--rw-r--r--   0        0        0     5780 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
--rw-r--r--   0        0        0      787 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/executors/__init__.py
--rw-r--r--   0        0        0    34132 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py
--rw-r--r--   0        0        0     1673 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py
--rw-r--r--   0        0        0    23564 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py
--rw-r--r--   0        0        0    10014 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py
--rw-r--r--   0        0        0    17754 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/get_provider_info.py
--rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/hooks/__init__.py
--rw-r--r--   0        0        0    31558 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
--rw-r--r--   0        0        0     2101 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/k8s_model.py
--rw-r--r--   0        0        0     5329 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/kube_client.py
--rw-r--r--   0        0        0     5225 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/kube_config.py
--rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py
--rw-r--r--   0        0        0     2567 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/basic_template.yaml
--rw-r--r--   0        0        0     6410 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py
--rw-r--r--   0        0        0      787 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/operators/__init__.py
--rw-r--r--   0        0        0    15370 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/operators/custom_object_launcher.py
--rw-r--r--   0        0        0    21432 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/operators/job.py
--rw-r--r--   0        0        0     1269 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
--rw-r--r--   0        0        0    50268 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/operators/pod.py
--rw-r--r--   0        0        0     7151 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/operators/resource.py
--rw-r--r--   0        0        0    13262 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
--rw-r--r--   0        0        0    24490 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/pod_generator.py
--rw-r--r--   0        0        0    11994 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py
--rw-r--r--   0        0        0    12009 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py
--rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py
--rw-r--r--   0        0        0     2256 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_image_template.yaml
--rw-r--r--   0        0        0     2442 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_volume_template.yaml
--rw-r--r--   0        0        0     3020 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/pod_template_file_examples/git_sync_template.yaml
--rw-r--r--   0        0        0     1741 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
--rw-r--r--   0        0        0     3460 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
--rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/resource_convert/__init__.py
--rw-r--r--   0        0        0     1873 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/resource_convert/configmap.py
--rw-r--r--   0        0        0     1464 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/resource_convert/env_variable.py
--rw-r--r--   0        0        0     1494 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/resource_convert/secret.py
--rw-r--r--   0        0        0     5209 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/secret.py
--rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/sensors/__init__.py
--rw-r--r--   0        0        0     5552 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
--rw-r--r--   0        0        0     2968 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/template_rendering.py
--rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/triggers/__init__.py
--rw-r--r--   0        0        0     4060 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/triggers/job.py
--rw-r--r--   0        0        0     1266 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
--rw-r--r--   0        0        0    13519 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/triggers/pod.py
--rw-r--r--   0        0        0      863 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/utils/__init__.py
--rw-r--r--   0        0        0     5195 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/utils/delete_from.py
--rw-r--r--   0        0        0     1928 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/utils/k8s_resource_iterator.py
--rw-r--r--   0        0        0    33444 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
--rw-r--r--   0        0        0     2519 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
--rw-r--r--   0        0        0     3171 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/pyproject.toml
--rw-r--r--   0        0        0     5258 1970-01-01 00:00:00.000000 apache_airflow_providers_cncf_kubernetes-8.1.1/PKG-INFO
+-rw-r--r--   0        0        0     3341 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/README.rst
+-rw-r--r--   0        0        0    13569 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/LICENSE
+-rw-r--r--   0        0        0     1590 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/__init__.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py
+-rw-r--r--   0        0        0     3967 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py
+-rw-r--r--   0        0        0     4094 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/callbacks.py
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py
+-rw-r--r--   0        0        0     5780 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/__init__.py
+-rw-r--r--   0        0        0    34132 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py
+-rw-r--r--   0        0        0     1673 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py
+-rw-r--r--   0        0        0    23564 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py
+-rw-r--r--   0        0        0    10014 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py
+-rw-r--r--   0        0        0    17754 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/get_provider_info.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py
+-rw-r--r--   0        0        0    31558 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py
+-rw-r--r--   0        0        0     2101 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/k8s_model.py
+-rw-r--r--   0        0        0     5329 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kube_client.py
+-rw-r--r--   0        0        0     5225 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kube_config.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py
+-rw-r--r--   0        0        0     2567 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/basic_template.yaml
+-rw-r--r--   0        0        0     6410 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py
+-rw-r--r--   0        0        0      787 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/__init__.py
+-rw-r--r--   0        0        0    15370 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/custom_object_launcher.py
+-rw-r--r--   0        0        0    21432 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/job.py
+-rw-r--r--   0        0        0     1269 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py
+-rw-r--r--   0        0        0    50268 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/pod.py
+-rw-r--r--   0        0        0     7151 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/resource.py
+-rw-r--r--   0        0        0    13262 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py
+-rw-r--r--   0        0        0    24490 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_generator.py
+-rw-r--r--   0        0        0    11994 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py
+-rw-r--r--   0        0        0    12009 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py
+-rw-r--r--   0        0        0     2256 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_image_template.yaml
+-rw-r--r--   0        0        0     2442 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_volume_template.yaml
+-rw-r--r--   0        0        0     3020 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/git_sync_template.yaml
+-rw-r--r--   0        0        0     1741 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2
+-rw-r--r--   0        0        0     3460 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/resource_convert/__init__.py
+-rw-r--r--   0        0        0     1873 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/resource_convert/configmap.py
+-rw-r--r--   0        0        0     1464 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/resource_convert/env_variable.py
+-rw-r--r--   0        0        0     1494 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/resource_convert/secret.py
+-rw-r--r--   0        0        0     5209 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/secret.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py
+-rw-r--r--   0        0        0     5552 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py
+-rw-r--r--   0        0        0     2968 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/template_rendering.py
+-rw-r--r--   0        0        0      785 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py
+-rw-r--r--   0        0        0     4060 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/triggers/job.py
+-rw-r--r--   0        0        0     1266 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py
+-rw-r--r--   0        0        0    13519 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/triggers/pod.py
+-rw-r--r--   0        0        0      863 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/__init__.py
+-rw-r--r--   0        0        0     5195 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py
+-rw-r--r--   0        0        0     1928 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/k8s_resource_iterator.py
+-rw-r--r--   0        0        0    33444 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py
+-rw-r--r--   0        0        0     2519 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py
+-rw-r--r--   0        0        0     3178 2024-04-16 07:37:35.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/pyproject.toml
+-rw-r--r--   0        0        0     5268 1970-01-01 00:00:00.000000 apache_airflow_providers_cncf_kubernetes-8.1.1rc1/PKG-INFO
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/README.rst` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``8.1.1``
+Release: ``8.1.1.rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/LICENSE` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/LICENSE`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/backcompat/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/backcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/backcompat/backwards_compat_converters.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/callbacks.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/callbacks.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/decorators/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/decorators/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/executors/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_types.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/kubernetes_executor_utils.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/executors/local_kubernetes_executor.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/get_provider_info.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/hooks/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/hooks/kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/k8s_model.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/k8s_model.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/kube_client.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kube_client.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/kube_config.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kube_config.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/basic_template.yaml` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kubernetes_executor_templates/basic_template.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/kubernetes_helper_functions.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/operators/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/operators/custom_object_launcher.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/custom_object_launcher.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/operators/job.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/job.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/operators/pod.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/pod.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/operators/resource.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/resource.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/operators/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/pod_generator.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_generator.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_generator_deprecated.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_launcher_deprecated.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_image_template.yaml` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_image_template.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_volume_template.yaml` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/dags_in_volume_template.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/pod_template_file_examples/git_sync_template.yaml` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/pod_template_file_examples/git_sync_template.yaml`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.jinja2`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/python_kubernetes_script.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/resource_convert/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/resource_convert/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/resource_convert/configmap.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/resource_convert/configmap.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/resource_convert/env_variable.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/resource_convert/env_variable.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/resource_convert/secret.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/resource_convert/secret.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/secret.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/secret.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/sensors/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/sensors/spark_kubernetes.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/template_rendering.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/template_rendering.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/triggers/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/triggers/job.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/triggers/job.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/triggers/kubernetes_pod.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/triggers/pod.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/triggers/pod.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/utils/__init__.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/utils/delete_from.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/delete_from.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/utils/k8s_resource_iterator.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/k8s_resource_iterator.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/utils/pod_manager.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/pod_manager.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/airflow/providers/cncf/kubernetes/utils/xcom_sidecar.py`

 * *Files identical despite different names*

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/pyproject.toml` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 #
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "apache-airflow-providers-cncf-kubernetes"
-version = "8.1.1"
+version = "8.1.1.rc1"
 description = "Provider package apache-airflow-providers-cncf-kubernetes for Apache Airflow"
 readme = "README.rst"
 authors = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
 ]
 maintainers = [
     {name="Apache Software Foundation", email="dev@airflow.apache.org"},
@@ -53,15 +53,15 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: System :: Monitoring",
 ]
 requires-python = "~=3.8"
 dependencies = [
     "aiofiles>=23.2.0",
-    "apache-airflow>=2.6.0",
+    "apache-airflow>=2.6.0rc0",
     "asgiref>=3.5.2",
     "cryptography>=2.0.0",
     "google-re2>=1.0",
     "kubernetes>=28.1.0,<=29.0.0",
     "kubernetes_asyncio>=28.1.0,<=29.0.0",
 ]
```

### Comparing `apache_airflow_providers_cncf_kubernetes-8.1.1/PKG-INFO` & `apache_airflow_providers_cncf_kubernetes-8.1.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-cncf-kubernetes
-Version: 8.1.1
+Version: 8.1.1rc1
 Summary: Provider package apache-airflow-providers-cncf-kubernetes for Apache Airflow
 Keywords: airflow-provider,cncf.kubernetes,airflow,integration
 Author-email: Apache Software Foundation <dev@airflow.apache.org>
 Maintainer-email: Apache Software Foundation <dev@airflow.apache.org>
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: System :: Monitoring
 Requires-Dist: aiofiles>=23.2.0
-Requires-Dist: apache-airflow>=2.6.0
+Requires-Dist: apache-airflow>=2.6.0rc0
 Requires-Dist: asgiref>=3.5.2
 Requires-Dist: cryptography>=2.0.0
 Requires-Dist: google-re2>=1.0
 Requires-Dist: kubernetes>=28.1.0,<=29.0.0
 Requires-Dist: kubernetes_asyncio>=28.1.0,<=29.0.0
 Project-URL: Bug Tracker, https://github.com/apache/airflow/issues
 Project-URL: Changelog, https://airflow.apache.org/docs/apache-airflow-providers-cncf-kubernetes/8.1.1/changelog.html
@@ -76,15 +76,15 @@
 
  .. IF YOU WANT TO MODIFY TEMPLATE FOR THIS FILE, YOU SHOULD MODIFY THE TEMPLATE
     `PROVIDER_README_TEMPLATE.rst.jinja2` IN the `dev/breeze/src/airflow_breeze/templates` DIRECTORY
 
 
 Package ``apache-airflow-providers-cncf-kubernetes``
 
-Release: ``8.1.1``
+Release: ``8.1.1.rc1``
 
 
 `Kubernetes <https://kubernetes.io/>`__
 
 
 Provider package
 ----------------
```

