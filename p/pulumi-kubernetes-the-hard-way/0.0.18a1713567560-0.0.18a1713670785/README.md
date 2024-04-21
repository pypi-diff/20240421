# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.18a1713567560.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.18a1713670785.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.18a1713567560.tar", last modified: Fri Apr 19 23:01:38 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.18a1713670785.tar", last modified: Sun Apr 21 03:42:14 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560.tar` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785.tar`

### file list

```diff
@@ -1,75 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:01:38.119175 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-19 23:01:38.119175 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:01:38.107175 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     4080 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:01:38.107175 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      418 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    21101 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     8728 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)    23922 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    29159 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:01:38.115175 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)      940 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1095 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    15965 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8426 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    12377 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
--rw-------   0 runner    (1001) docker     (127)    14905 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)    14696 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)    15536 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    13390 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     5113 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)    10944 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:01:38.115175 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     3019 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    30597 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     2983 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27130 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:01:38.119175 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      545 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     3166 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)    22577 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    97822 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/curl.py
--rw-------   0 runner    (1001) docker     (127)    14986 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    24623 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
--rw-------   0 runner    (1001) docker     (127)    14032 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    16572 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    25981 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    16828 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    30857 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/sed.py
--rw-------   0 runner    (1001) docker     (127)    13649 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    19232 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    17062 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    19599 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 23:01:38.119175 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-19 23:01:38.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-19 23:01:38.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 23:01:38.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-19 23:01:38.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-19 23:01:38.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      899 2024-04-19 23:01:28.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 23:01:38.119175 pulumi_kubernetes_the_hard_way-0.0.18a1713567560/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:42:14.265900 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-21 03:42:14.261900 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:42:14.249900 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     4080 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:42:14.253900 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      418 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      427 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    21101 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     8728 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)     3426 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+-rw-------   0 runner    (1001) docker     (127)    23922 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)    29159 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:42:14.257900 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)      940 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1095 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    15965 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    19229 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)    10255 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)    10159 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8328 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    12377 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
+-rw-------   0 runner    (1001) docker     (127)    14905 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10651 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14696 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
+-rw-------   0 runner    (1001) docker     (127)     7339 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     9822 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     9652 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)    15536 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    13390 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     9580 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)     5113 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     7429 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/static_pod.py
+-rw-------   0 runner    (1001) docker     (127)    10944 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:42:14.257900 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      425 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1000 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     3019 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    30597 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    15919 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4450 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)     2983 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tls/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    27130 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:42:14.261900 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      590 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     3166 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)   108421 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    14165 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    14181 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/curl.py
+-rw-------   0 runner    (1001) docker     (127)    14263 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    14415 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
+-rw-------   0 runner    (1001) docker     (127)    14165 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    14203 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    14051 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    91760 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    14051 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    14089 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/sed.py
+-rw-------   0 runner    (1001) docker     (127)    14339 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    14089 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    14109 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    14127 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 03:42:14.261900 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-21 03:42:14.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-04-21 03:42:14.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 03:42:14.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-21 03:42:14.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-21 03:42:14.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      899 2024-04-21 03:42:05.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 03:42:14.265900 pulumi_kubernetes_the_hard_way-0.0.18a1713670785/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.18a1713567560
+Version: 0.0.18a1713670785
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/README.md` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 
 @pulumi.input_type
 class DownloadArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  destination: pulumi.Input[str],
                  url: pulumi.Input[str],
-                 remove_on_delete: Optional[pulumi.Input[bool]] = None):
+                 remove_on_delete: Optional[bool] = None):
         """
         The set of arguments for constructing a Download resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: The parameters with which to connect to the remote host.
         :param pulumi.Input[str] destination: The fully qualified path on the remote system where the file should be downloaded to.
         :param pulumi.Input[str] url: The URL of the file to be downloaded.
-        :param pulumi.Input[bool] remove_on_delete: Remove the downloaded fiel when the resource is deleted.
+        :param bool remove_on_delete: Remove the downloaded fiel when the resource is deleted.
         """
         pulumi.set(__self__, "connection", connection)
         pulumi.set(__self__, "destination", destination)
         pulumi.set(__self__, "url", url)
         if remove_on_delete is not None:
             pulumi.set(__self__, "remove_on_delete", remove_on_delete)
 
@@ -67,43 +67,43 @@
 
     @url.setter
     def url(self, value: pulumi.Input[str]):
         pulumi.set(self, "url", value)
 
     @property
     @pulumi.getter(name="removeOnDelete")
-    def remove_on_delete(self) -> Optional[pulumi.Input[bool]]:
+    def remove_on_delete(self) -> Optional[bool]:
         """
         Remove the downloaded fiel when the resource is deleted.
         """
         return pulumi.get(self, "remove_on_delete")
 
     @remove_on_delete.setter
-    def remove_on_delete(self, value: Optional[pulumi.Input[bool]]):
+    def remove_on_delete(self, value: Optional[bool]):
         pulumi.set(self, "remove_on_delete", value)
 
 
 class Download(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  destination: Optional[pulumi.Input[str]] = None,
-                 remove_on_delete: Optional[pulumi.Input[bool]] = None,
+                 remove_on_delete: Optional[bool] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Downloads the file specified by `url` onto a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: The parameters with which to connect to the remote host.
         :param pulumi.Input[str] destination: The fully qualified path on the remote system where the file should be downloaded to.
-        :param pulumi.Input[bool] remove_on_delete: Remove the downloaded fiel when the resource is deleted.
+        :param bool remove_on_delete: Remove the downloaded fiel when the resource is deleted.
         :param pulumi.Input[str] url: The URL of the file to be downloaded.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: DownloadArgs,
@@ -124,15 +124,15 @@
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
                  destination: Optional[pulumi.Input[str]] = None,
-                 remove_on_delete: Optional[pulumi.Input[bool]] = None,
+                 remove_on_delete: Optional[bool] = None,
                  url: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/etcd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/etcd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/start_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/start_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/static_pod.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tls/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,7 +15,9 @@
 from .mv import *
 from .rm import *
 from .sed import *
 from .systemctl import *
 from .tar import *
 from .tee import *
 from .wget import *
+from ._inputs import *
+from . import outputs
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,258 +4,125 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from . import outputs
 from ._enums import *
+from ._inputs import *
 import pulumi_command
 
-__all__ = ['ChmodArgs', 'Chmod']
+__all__ = ['TeeArgs', 'Tee']
 
 @pulumi.input_type
-class ChmodArgs:
+class TeeArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 files: pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]],
-                 mode: pulumi.Input[str],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 changes: Optional[pulumi.Input[bool]] = None,
+                 create: Optional['TeeOptsArgs'] = None,
+                 delete: Optional['TeeOptsArgs'] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 help: Optional[pulumi.Input[bool]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 no_preserve_root: Optional[pulumi.Input[bool]] = None,
-                 preserve_root: Optional[pulumi.Input[bool]] = None,
-                 quiet: Optional[pulumi.Input[bool]] = None,
-                 recursive: Optional[pulumi.Input[bool]] = None,
-                 reference: Optional[pulumi.Input[str]] = None,
-                 silent: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 version: Optional[pulumi.Input[bool]] = None):
+                 update: Optional['TeeOptsArgs'] = None):
         """
-        The set of arguments for constructing a Chmod resource.
+        The set of arguments for constructing a Tee resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
-        :param pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]] files: Corresponds to the [FILE] argument.
-        :param pulumi.Input[str] mode: Modes may be absolute or symbolic. An absolute mode is an octal number...
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param pulumi.Input[bool] changes: Like verbose but report only when a change is made.
+        :param 'TeeOptsArgs' create: The command to run on create.
+        :param 'TeeOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+               and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+               Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
-        :param pulumi.Input[bool] help: Display help and exit.
-        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
-        :param pulumi.Input[bool] no_preserve_root: Do not treat '/' specially (the default).
-        :param pulumi.Input[bool] preserve_root: Fail to operate recursively on '/'.
-        :param pulumi.Input[bool] quiet: Suppress most error messages. Same as `silent`.
-        :param pulumi.Input[bool] recursive: Change files and directories recursively.
-        :param pulumi.Input[str] reference: Use RFILE's mode instead of specifying MODE values. RFILE is always dereferenced if a symbolic link.
-        :param pulumi.Input[bool] silent: Suppress most error messages. Same as `quiet`.
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.Input[bool] version: Output version information and exit.
+        :param 'TeeOptsArgs' update: The command to run on update, if empty, create will 
+               run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+               are set to the stdout and stderr properties of the Command resource from previous 
+               create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
-        pulumi.set(__self__, "files", files)
-        pulumi.set(__self__, "mode", mode)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
-        if changes is not None:
-            pulumi.set(__self__, "changes", changes)
+        if create is not None:
+            pulumi.set(__self__, "create", create)
+        if delete is not None:
+            pulumi.set(__self__, "delete", delete)
         if environment is not None:
             pulumi.set(__self__, "environment", environment)
-        if help is not None:
-            pulumi.set(__self__, "help", help)
-        if lifecycle is not None:
-            pulumi.set(__self__, "lifecycle", lifecycle)
-        if no_preserve_root is not None:
-            pulumi.set(__self__, "no_preserve_root", no_preserve_root)
-        if preserve_root is not None:
-            pulumi.set(__self__, "preserve_root", preserve_root)
-        if quiet is not None:
-            pulumi.set(__self__, "quiet", quiet)
-        if recursive is not None:
-            pulumi.set(__self__, "recursive", recursive)
-        if reference is not None:
-            pulumi.set(__self__, "reference", reference)
-        if silent is not None:
-            pulumi.set(__self__, "silent", silent)
         if stdin is not None:
             pulumi.set(__self__, "stdin", stdin)
         if triggers is not None:
             pulumi.set(__self__, "triggers", triggers)
-        if version is not None:
-            pulumi.set(__self__, "version", version)
+        if update is not None:
+            pulumi.set(__self__, "update", update)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
-    @pulumi.getter
-    def files(self) -> pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]:
-        """
-        Corresponds to the [FILE] argument.
-        """
-        return pulumi.get(self, "files")
-
-    @files.setter
-    def files(self, value: pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "files", value)
-
-    @property
-    @pulumi.getter
-    def mode(self) -> pulumi.Input[str]:
-        """
-        Modes may be absolute or symbolic. An absolute mode is an octal number...
-        """
-        return pulumi.get(self, "mode")
-
-    @mode.setter
-    def mode(self, value: pulumi.Input[str]):
-        pulumi.set(self, "mode", value)
-
-    @property
     @pulumi.getter(name="binaryPath")
     def binary_path(self) -> Optional[pulumi.Input[str]]:
         """
         Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         """
         return pulumi.get(self, "binary_path")
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def changes(self) -> Optional[pulumi.Input[bool]]:
+    def create(self) -> Optional['TeeOptsArgs']:
         """
-        Like verbose but report only when a change is made.
+        The command to run on create.
         """
-        return pulumi.get(self, "changes")
+        return pulumi.get(self, "create")
 
-    @changes.setter
-    def changes(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "changes", value)
+    @create.setter
+    def create(self, value: Optional['TeeOptsArgs']):
+        pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+    def delete(self) -> Optional['TeeOptsArgs']:
         """
-        Environment variables
+        The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+        Command resource from previous create or update steps.
         """
-        return pulumi.get(self, "environment")
+        return pulumi.get(self, "delete")
 
-    @environment.setter
-    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
-        pulumi.set(self, "environment", value)
-
-    @property
-    @pulumi.getter
-    def help(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Display help and exit.
-        """
-        return pulumi.get(self, "help")
-
-    @help.setter
-    def help(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "help", value)
+    @delete.setter
+    def delete(self, value: Optional['TeeOptsArgs']):
+        pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
-    def lifecycle(self) -> Optional['CommandLifecycle']:
-        """
-        At what stage(s) in the resource lifecycle should the command be run
-        """
-        return pulumi.get(self, "lifecycle")
-
-    @lifecycle.setter
-    def lifecycle(self, value: Optional['CommandLifecycle']):
-        pulumi.set(self, "lifecycle", value)
-
-    @property
-    @pulumi.getter(name="noPreserveRoot")
-    def no_preserve_root(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Do not treat '/' specially (the default).
-        """
-        return pulumi.get(self, "no_preserve_root")
-
-    @no_preserve_root.setter
-    def no_preserve_root(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "no_preserve_root", value)
-
-    @property
-    @pulumi.getter(name="preserveRoot")
-    def preserve_root(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Fail to operate recursively on '/'.
-        """
-        return pulumi.get(self, "preserve_root")
-
-    @preserve_root.setter
-    def preserve_root(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "preserve_root", value)
-
-    @property
-    @pulumi.getter
-    def quiet(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Suppress most error messages. Same as `silent`.
-        """
-        return pulumi.get(self, "quiet")
-
-    @quiet.setter
-    def quiet(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "quiet", value)
-
-    @property
-    @pulumi.getter
-    def recursive(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Change files and directories recursively.
-        """
-        return pulumi.get(self, "recursive")
-
-    @recursive.setter
-    def recursive(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "recursive", value)
-
-    @property
-    @pulumi.getter
-    def reference(self) -> Optional[pulumi.Input[str]]:
-        """
-        Use RFILE's mode instead of specifying MODE values. RFILE is always dereferenced if a symbolic link.
-        """
-        return pulumi.get(self, "reference")
-
-    @reference.setter
-    def reference(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "reference", value)
-
-    @property
-    @pulumi.getter
-    def silent(self) -> Optional[pulumi.Input[bool]]:
+    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Suppress most error messages. Same as `quiet`.
+        Environment variables
         """
-        return pulumi.get(self, "silent")
+        return pulumi.get(self, "environment")
 
-    @silent.setter
-    def silent(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "silent", value)
+    @environment.setter
+    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "environment", value)
 
     @property
     @pulumi.getter
     def stdin(self) -> Optional[pulumi.Input[str]]:
         """
         TODO
         """
@@ -275,151 +142,119 @@
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def version(self) -> Optional[pulumi.Input[bool]]:
+    def update(self) -> Optional['TeeOptsArgs']:
         """
-        Output version information and exit.
+        The command to run on update, if empty, create will 
+        run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+        are set to the stdout and stderr properties of the Command resource from previous 
+        create or update steps.
         """
-        return pulumi.get(self, "version")
+        return pulumi.get(self, "update")
 
-    @version.setter
-    def version(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "version", value)
+    @update.setter
+    def update(self, value: Optional['TeeOptsArgs']):
+        pulumi.set(self, "update", value)
 
 
-class Chmod(pulumi.ComponentResource):
+class Tee(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 changes: Optional[pulumi.Input[bool]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
+                 create: Optional[pulumi.InputType['TeeOptsArgs']] = None,
+                 delete: Optional[pulumi.InputType['TeeOptsArgs']] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 files: Optional[pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]] = None,
-                 help: Optional[pulumi.Input[bool]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 mode: Optional[pulumi.Input[str]] = None,
-                 no_preserve_root: Optional[pulumi.Input[bool]] = None,
-                 preserve_root: Optional[pulumi.Input[bool]] = None,
-                 quiet: Optional[pulumi.Input[bool]] = None,
-                 recursive: Optional[pulumi.Input[bool]] = None,
-                 reference: Optional[pulumi.Input[str]] = None,
-                 silent: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 version: Optional[pulumi.Input[bool]] = None,
+                 update: Optional[pulumi.InputType['TeeOptsArgs']] = None,
                  __props__=None):
         """
-        Abstraction over the `chmod` utility on a remote system.
+        Abstraction over the `rm` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param pulumi.Input[bool] changes: Like verbose but report only when a change is made.
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
+        :param pulumi.InputType['TeeOptsArgs'] create: The command to run on create.
+        :param pulumi.InputType['TeeOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+               and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+               Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
-        :param pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]] files: Corresponds to the [FILE] argument.
-        :param pulumi.Input[bool] help: Display help and exit.
-        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
-        :param pulumi.Input[str] mode: Modes may be absolute or symbolic. An absolute mode is an octal number...
-        :param pulumi.Input[bool] no_preserve_root: Do not treat '/' specially (the default).
-        :param pulumi.Input[bool] preserve_root: Fail to operate recursively on '/'.
-        :param pulumi.Input[bool] quiet: Suppress most error messages. Same as `silent`.
-        :param pulumi.Input[bool] recursive: Change files and directories recursively.
-        :param pulumi.Input[str] reference: Use RFILE's mode instead of specifying MODE values. RFILE is always dereferenced if a symbolic link.
-        :param pulumi.Input[bool] silent: Suppress most error messages. Same as `quiet`.
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.Input[bool] version: Output version information and exit.
+        :param pulumi.InputType['TeeOptsArgs'] update: The command to run on update, if empty, create will 
+               run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+               are set to the stdout and stderr properties of the Command resource from previous 
+               create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ChmodArgs,
+                 args: TeeArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `chmod` utility on a remote system.
+        Abstraction over the `rm` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param ChmodArgs args: The arguments to use to populate this resource's properties.
+        :param TeeArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ChmodArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(TeeArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 changes: Optional[pulumi.Input[bool]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
+                 create: Optional[pulumi.InputType['TeeOptsArgs']] = None,
+                 delete: Optional[pulumi.InputType['TeeOptsArgs']] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 files: Optional[pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]] = None,
-                 help: Optional[pulumi.Input[bool]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 mode: Optional[pulumi.Input[str]] = None,
-                 no_preserve_root: Optional[pulumi.Input[bool]] = None,
-                 preserve_root: Optional[pulumi.Input[bool]] = None,
-                 quiet: Optional[pulumi.Input[bool]] = None,
-                 recursive: Optional[pulumi.Input[bool]] = None,
-                 reference: Optional[pulumi.Input[str]] = None,
-                 silent: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 version: Optional[pulumi.Input[bool]] = None,
+                 update: Optional[pulumi.InputType['TeeOptsArgs']] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ChmodArgs.__new__(ChmodArgs)
+            __props__ = TeeArgs.__new__(TeeArgs)
 
             __props__.__dict__["binary_path"] = binary_path
-            __props__.__dict__["changes"] = changes
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
+            __props__.__dict__["create"] = create
+            __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
-            if files is None and not opts.urn:
-                raise TypeError("Missing required property 'files'")
-            __props__.__dict__["files"] = files
-            __props__.__dict__["help"] = help
-            __props__.__dict__["lifecycle"] = lifecycle
-            if mode is None and not opts.urn:
-                raise TypeError("Missing required property 'mode'")
-            __props__.__dict__["mode"] = mode
-            __props__.__dict__["no_preserve_root"] = no_preserve_root
-            __props__.__dict__["preserve_root"] = preserve_root
-            __props__.__dict__["quiet"] = quiet
-            __props__.__dict__["recursive"] = recursive
-            __props__.__dict__["reference"] = reference
-            __props__.__dict__["silent"] = silent
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
-            __props__.__dict__["version"] = version
+            __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Chmod, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Chmod',
+        super(Tee, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Tee',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -427,22 +262,14 @@
         """
         Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         """
         return pulumi.get(self, "binary_path")
 
     @property
     @pulumi.getter
-    def changes(self) -> pulumi.Output[bool]:
-        """
-        Like verbose but report only when a change is made.
-        """
-        return pulumi.get(self, "changes")
-
-    @property
-    @pulumi.getter
     def command(self) -> pulumi.Output['pulumi_command.remote.Command']:
         """
         The underlying command
         """
         return pulumi.get(self, "command")
 
     @property
@@ -451,99 +278,37 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def environment(self) -> pulumi.Output[Mapping[str, str]]:
-        """
-        Environment variables
-        """
-        return pulumi.get(self, "environment")
-
-    @property
-    @pulumi.getter
-    def files(self) -> pulumi.Output[Any]:
-        """
-        Corresponds to the [FILE] argument.
-        """
-        return pulumi.get(self, "files")
-
-    @property
-    @pulumi.getter
-    def help(self) -> pulumi.Output[bool]:
-        """
-        Display help and exit.
-        """
-        return pulumi.get(self, "help")
-
-    @property
-    @pulumi.getter
-    def lifecycle(self) -> pulumi.Output[Optional['CommandLifecycle']]:
-        """
-        At what stage(s) in the resource lifecycle should the command be run
-        """
-        return pulumi.get(self, "lifecycle")
-
-    @property
-    @pulumi.getter
-    def mode(self) -> pulumi.Output[str]:
-        """
-        Modes may be absolute or symbolic. An absolute mode is an octal number...
-        """
-        return pulumi.get(self, "mode")
-
-    @property
-    @pulumi.getter(name="noPreserveRoot")
-    def no_preserve_root(self) -> pulumi.Output[bool]:
-        """
-        Do not treat '/' specially (the default).
-        """
-        return pulumi.get(self, "no_preserve_root")
-
-    @property
-    @pulumi.getter(name="preserveRoot")
-    def preserve_root(self) -> pulumi.Output[bool]:
-        """
-        Fail to operate recursively on '/'.
-        """
-        return pulumi.get(self, "preserve_root")
-
-    @property
-    @pulumi.getter
-    def quiet(self) -> pulumi.Output[bool]:
-        """
-        Suppress most error messages. Same as `silent`.
-        """
-        return pulumi.get(self, "quiet")
-
-    @property
-    @pulumi.getter
-    def recursive(self) -> pulumi.Output[bool]:
+    def create(self) -> pulumi.Output[Optional['outputs.TeeOpts']]:
         """
-        Change files and directories recursively.
+        The command to run on create.
         """
-        return pulumi.get(self, "recursive")
+        return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def reference(self) -> pulumi.Output[Optional[str]]:
+    def delete(self) -> pulumi.Output[Optional['outputs.TeeOpts']]:
         """
-        Use RFILE's mode instead of specifying MODE values. RFILE is always dereferenced if a symbolic link.
+        The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+        Command resource from previous create or update steps.
         """
-        return pulumi.get(self, "reference")
+        return pulumi.get(self, "delete")
 
     @property
     @pulumi.getter
-    def silent(self) -> pulumi.Output[bool]:
+    def environment(self) -> pulumi.Output[Mapping[str, str]]:
         """
-        Suppress most error messages. Same as `quiet`.
+        Environment variables
         """
-        return pulumi.get(self, "silent")
+        return pulumi.get(self, "environment")
 
     @property
     @pulumi.getter
     def stderr(self) -> pulumi.Output[str]:
         """
         TODO
         """
@@ -571,13 +336,16 @@
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def version(self) -> pulumi.Output[bool]:
+    def update(self) -> pulumi.Output[Optional['outputs.TeeOpts']]:
         """
-        Output version information and exit.
+        The command to run on update, if empty, create will 
+        run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+        are set to the stdout and stderr properties of the Command resource from previous 
+        create or update steps.
         """
-        return pulumi.get(self, "version")
+        return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/curl.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/_inputs.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,30 +5,223 @@
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
 from ._enums import *
-import pulumi_command
 
-__all__ = ['CurlArgs', 'Curl']
+__all__ = [
+    'ChmodOptsArgs',
+    'CurlOptsArgs',
+    'EtcdctlOptsArgs',
+    'HostnamectlOptsArgs',
+    'MkdirOptsArgs',
+    'MktempOptsArgs',
+    'MvOptsArgs',
+    'RmOptsArgs',
+    'SedOptsArgs',
+    'SystemctlOptsArgs',
+    'TarOptsArgs',
+    'TeeOptsArgs',
+    'WgetOptsArgs',
+]
 
 @pulumi.input_type
-class CurlArgs:
+class ChmodOptsArgs:
     def __init__(__self__, *,
-                 connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 urls: pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]],
+                 files: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 mode: pulumi.Input[str],
+                 changes: Optional[pulumi.Input[bool]] = None,
+                 help: Optional[pulumi.Input[bool]] = None,
+                 no_preserve_root: Optional[pulumi.Input[bool]] = None,
+                 preserve_root: Optional[pulumi.Input[bool]] = None,
+                 quiet: Optional[pulumi.Input[bool]] = None,
+                 recursive: Optional[pulumi.Input[bool]] = None,
+                 reference: Optional[pulumi.Input[str]] = None,
+                 silent: Optional[pulumi.Input[bool]] = None,
+                 version: Optional[pulumi.Input[bool]] = None):
+        """
+        Abstraction over the `chmod` utility on a remote system.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] files: Corresponds to the [FILE] argument.
+        :param pulumi.Input[str] mode: Modes may be absolute or symbolic. An absolute mode is an octal number...
+        :param pulumi.Input[bool] changes: Like verbose but report only when a change is made.
+        :param pulumi.Input[bool] help: Display help and exit.
+        :param pulumi.Input[bool] no_preserve_root: Do not treat '/' specially (the default).
+        :param pulumi.Input[bool] preserve_root: Fail to operate recursively on '/'.
+        :param pulumi.Input[bool] quiet: Suppress most error messages. Same as `silent`.
+        :param pulumi.Input[bool] recursive: Change files and directories recursively.
+        :param pulumi.Input[str] reference: Use RFILE's mode instead of specifying MODE values. RFILE is always dereferenced if a symbolic link.
+        :param pulumi.Input[bool] silent: Suppress most error messages. Same as `quiet`.
+        :param pulumi.Input[bool] version: Output version information and exit.
+        """
+        pulumi.set(__self__, "files", files)
+        pulumi.set(__self__, "mode", mode)
+        if changes is not None:
+            pulumi.set(__self__, "changes", changes)
+        if help is not None:
+            pulumi.set(__self__, "help", help)
+        if no_preserve_root is not None:
+            pulumi.set(__self__, "no_preserve_root", no_preserve_root)
+        if preserve_root is not None:
+            pulumi.set(__self__, "preserve_root", preserve_root)
+        if quiet is not None:
+            pulumi.set(__self__, "quiet", quiet)
+        if recursive is not None:
+            pulumi.set(__self__, "recursive", recursive)
+        if reference is not None:
+            pulumi.set(__self__, "reference", reference)
+        if silent is not None:
+            pulumi.set(__self__, "silent", silent)
+        if version is not None:
+            pulumi.set(__self__, "version", version)
+
+    @property
+    @pulumi.getter
+    def files(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
+        """
+        Corresponds to the [FILE] argument.
+        """
+        return pulumi.get(self, "files")
+
+    @files.setter
+    def files(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "files", value)
+
+    @property
+    @pulumi.getter
+    def mode(self) -> pulumi.Input[str]:
+        """
+        Modes may be absolute or symbolic. An absolute mode is an octal number...
+        """
+        return pulumi.get(self, "mode")
+
+    @mode.setter
+    def mode(self, value: pulumi.Input[str]):
+        pulumi.set(self, "mode", value)
+
+    @property
+    @pulumi.getter
+    def changes(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Like verbose but report only when a change is made.
+        """
+        return pulumi.get(self, "changes")
+
+    @changes.setter
+    def changes(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "changes", value)
+
+    @property
+    @pulumi.getter
+    def help(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Display help and exit.
+        """
+        return pulumi.get(self, "help")
+
+    @help.setter
+    def help(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "help", value)
+
+    @property
+    @pulumi.getter(name="noPreserveRoot")
+    def no_preserve_root(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Do not treat '/' specially (the default).
+        """
+        return pulumi.get(self, "no_preserve_root")
+
+    @no_preserve_root.setter
+    def no_preserve_root(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "no_preserve_root", value)
+
+    @property
+    @pulumi.getter(name="preserveRoot")
+    def preserve_root(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Fail to operate recursively on '/'.
+        """
+        return pulumi.get(self, "preserve_root")
+
+    @preserve_root.setter
+    def preserve_root(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "preserve_root", value)
+
+    @property
+    @pulumi.getter
+    def quiet(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Suppress most error messages. Same as `silent`.
+        """
+        return pulumi.get(self, "quiet")
+
+    @quiet.setter
+    def quiet(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "quiet", value)
+
+    @property
+    @pulumi.getter
+    def recursive(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Change files and directories recursively.
+        """
+        return pulumi.get(self, "recursive")
+
+    @recursive.setter
+    def recursive(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "recursive", value)
+
+    @property
+    @pulumi.getter
+    def reference(self) -> Optional[pulumi.Input[str]]:
+        """
+        Use RFILE's mode instead of specifying MODE values. RFILE is always dereferenced if a symbolic link.
+        """
+        return pulumi.get(self, "reference")
+
+    @reference.setter
+    def reference(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "reference", value)
+
+    @property
+    @pulumi.getter
+    def silent(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Suppress most error messages. Same as `quiet`.
+        """
+        return pulumi.get(self, "silent")
+
+    @silent.setter
+    def silent(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "silent", value)
+
+    @property
+    @pulumi.getter
+    def version(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Output version information and exit.
+        """
+        return pulumi.get(self, "version")
+
+    @version.setter
+    def version(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "version", value)
+
+
+@pulumi.input_type
+class CurlOptsArgs:
+    def __init__(__self__, *,
+                 urls: pulumi.Input[Sequence[pulumi.Input[str]]],
                  abstract_unix_socket: Optional[pulumi.Input[str]] = None,
                  alt_svc: Optional[pulumi.Input[str]] = None,
                  any_auth: Optional[pulumi.Input[bool]] = None,
                  append: Optional[pulumi.Input[bool]] = None,
                  aws_sigv4: Optional[pulumi.Input[str]] = None,
                  basic: Optional[pulumi.Input[bool]] = None,
-                 binary_path: Optional[pulumi.Input[str]] = None,
                  cacert: Optional[pulumi.Input[str]] = None,
                  capath: Optional[pulumi.Input[str]] = None,
                  cert: Optional[pulumi.Input[str]] = None,
                  cert_status: Optional[pulumi.Input[bool]] = None,
                  cert_type: Optional[pulumi.Input['CurlCertType']] = None,
                  ciphers: Optional[pulumi.Input[str]] = None,
                  compressed: Optional[pulumi.Input[bool]] = None,
@@ -61,15 +254,14 @@
                  dns_servers: Optional[pulumi.Input[str]] = None,
                  doh_cert_status: Optional[pulumi.Input[bool]] = None,
                  doh_insecure: Optional[pulumi.Input[bool]] = None,
                  doh_url: Optional[pulumi.Input[str]] = None,
                  dump_header: Optional[pulumi.Input[str]] = None,
                  egd_file: Optional[pulumi.Input[str]] = None,
                  engine: Optional[pulumi.Input[str]] = None,
-                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  etag_compare: Optional[pulumi.Input[str]] = None,
                  etag_save: Optional[pulumi.Input[str]] = None,
                  expect100_timeout: Optional[pulumi.Input[int]] = None,
                  fail: Optional[pulumi.Input[bool]] = None,
                  fail_early: Optional[pulumi.Input[bool]] = None,
                  fail_with_body: Optional[pulumi.Input[bool]] = None,
                  false_start: Optional[pulumi.Input[bool]] = None,
@@ -80,29 +272,24 @@
                  ftp_alternative_user: Optional[pulumi.Input[str]] = None,
                  ftp_create_dirs: Optional[pulumi.Input[bool]] = None,
                  ftp_method: Optional[pulumi.Input[str]] = None,
                  ftp_pasv: Optional[pulumi.Input[bool]] = None,
                  ftp_port: Optional[pulumi.Input[str]] = None,
                  ftp_pret: Optional[pulumi.Input[bool]] = None,
                  ftp_skip_pasv_ip: Optional[pulumi.Input[bool]] = None,
-                 ftp_ssl_ccc_mode: Optional[pulumi.Input[str]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 stdin: Optional[pulumi.Input[str]] = None,
-                 triggers: Optional[pulumi.Input[Sequence[Any]]] = None):
-        """
-        The set of arguments for constructing a Curl resource.
-        :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
-        :param pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]] urls: Corresponds to the URLs argument.
+                 ftp_ssl_ccc_mode: Optional[pulumi.Input[str]] = None):
+        """
+        Abstraction over the `curl` utility on a remote system. Transfer a URL.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] urls: Corresponds to the URLs argument.
         :param pulumi.Input[str] abstract_unix_socket: (HTTP) Connect through an abstract Unix domain socket, instead of using the network.
         :param pulumi.Input[str] alt_svc: (HTTPS)  This  option enables the alt-svc parser in curl.
         :param pulumi.Input[bool] any_auth: (HTTP) Tells curl to figure out authentication method by itself, and use the most secure one the remote site claims to support.
         :param pulumi.Input[bool] append: (FTP SFTP) When used in an upload, this makes curl append to the target file instead of overwriting it.
         :param pulumi.Input[str] aws_sigv4: Use AWS V4 signature authentication in the transfer.
         :param pulumi.Input[bool] basic: (HTTP) Tells curl to use HTTP Basic authentication with the remote host.
-        :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[str] cacert: (TLS)  Tells curl to use the specified certificate file to verify the peer.
         :param pulumi.Input[str] capath: (TLS) Tells curl to use the specified certificate directory to verify the peer.
         :param pulumi.Input[str] cert: (TLS)  Tells  curl to use the specified client certificate file when getting a file with HTTPS, FTPS or another SSL-based protocol.
         :param pulumi.Input[bool] cert_status: (TLS) Tells curl to verify the status of the server certificate by using the Certificate Status Request (aka. OCSP stapling) TLS extension.
         :param pulumi.Input['CurlCertType'] cert_type: (TLS) Tells curl what type the provided client certificate is using.
         :param pulumi.Input[str] ciphers: (TLS) Specifies which ciphers to use in the connection.
         :param pulumi.Input[bool] compressed: (HTTP) Request a compressed response using one of the algorithms curl supports, and automatically decompress the content.
@@ -135,15 +322,14 @@
         :param pulumi.Input[str] dns_servers: Set the list of DNS servers to be used instead of the system default.
         :param pulumi.Input[bool] doh_cert_status: Same as --cert-status but used for DoH (DNS-over-HTTPS).
         :param pulumi.Input[bool] doh_insecure: Same as -k, --insecure but used for DoH (DNS-over-HTTPS).
         :param pulumi.Input[str] doh_url: Specifies which DNS-over-HTTPS (DoH) server to use to resolve hostnames, instead of using the default name resolver mechanism.
         :param pulumi.Input[str] dump_header: (HTTP FTP) Write the received protocol headers to the specified file.
         :param pulumi.Input[str] egd_file: (TLS) Specify the path name to the Entropy Gathering Daemon socket.
         :param pulumi.Input[str] engine: (TLS) Select the OpenSSL crypto engine to use for cipher operations.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
         :param pulumi.Input[str] etag_compare: (HTTP) This option makes a conditional HTTP request for the specific ETag read from the given file by sending a custom If-None-Match header using the stored ETag.
         :param pulumi.Input[str] etag_save: (HTTP) This option saves an HTTP ETag to the specified file.
         :param pulumi.Input[int] expect100_timeout: (HTTP)  Maximum  time in seconds that you allow curl to wait for a 100-continue response when curl emits an Expects: 100-continue header in its request.
         :param pulumi.Input[bool] fail: (HTTP) Fail silently (no output at all) on server errors.
         :param pulumi.Input[bool] fail_early: Fail and exit on the first detected transfer error.
         :param pulumi.Input[bool] fail_with_body: (HTTP)  Return an error on server errors where the HTTP response code is 400 or greater).
         :param pulumi.Input[bool] false_start: (TLS) Tells curl to use false start during the TLS handshake.
@@ -155,34 +341,28 @@
         :param pulumi.Input[bool] ftp_create_dirs: (FTP  SFTP) When an FTP or SFTP URL/operation uses a path that does not currently exist on the server, the standard behavior of curl is to fail.
         :param pulumi.Input[str] ftp_method: (FTP) Control what method curl should use to reach a file on an FTP(S) server.
         :param pulumi.Input[bool] ftp_pasv: (FTP) Use passive mode for the data connection.
         :param pulumi.Input[str] ftp_port: (FTP)  Reverses  the  default  initiator/listener  roles  when connecting with FTP.
         :param pulumi.Input[bool] ftp_pret: (FTP) Tell curl to send a PRET command before PASV (and EPSV).
         :param pulumi.Input[bool] ftp_skip_pasv_ip: (FTP)  Tell  curl  to  not use the IP address the server suggests in its response to curl's PASV command when curl connects the data connection.
         :param pulumi.Input[str] ftp_ssl_ccc_mode: (FTP) Sets the CCC mode. The passive mode will not initiate the shutdown, but instead wait for the server to do it, and will not reply to the shutdown from the  server.
-        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
-        :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
         """
-        pulumi.set(__self__, "connection", connection)
         pulumi.set(__self__, "urls", urls)
         if abstract_unix_socket is not None:
             pulumi.set(__self__, "abstract_unix_socket", abstract_unix_socket)
         if alt_svc is not None:
             pulumi.set(__self__, "alt_svc", alt_svc)
         if any_auth is not None:
             pulumi.set(__self__, "any_auth", any_auth)
         if append is not None:
             pulumi.set(__self__, "append", append)
         if aws_sigv4 is not None:
             pulumi.set(__self__, "aws_sigv4", aws_sigv4)
         if basic is not None:
             pulumi.set(__self__, "basic", basic)
-        if binary_path is not None:
-            pulumi.set(__self__, "binary_path", binary_path)
         if cacert is not None:
             pulumi.set(__self__, "cacert", cacert)
         if capath is not None:
             pulumi.set(__self__, "capath", capath)
         if cert is not None:
             pulumi.set(__self__, "cert", cert)
         if cert_status is not None:
@@ -255,16 +435,14 @@
             pulumi.set(__self__, "doh_url", doh_url)
         if dump_header is not None:
             pulumi.set(__self__, "dump_header", dump_header)
         if egd_file is not None:
             pulumi.set(__self__, "egd_file", egd_file)
         if engine is not None:
             pulumi.set(__self__, "engine", engine)
-        if environment is not None:
-            pulumi.set(__self__, "environment", environment)
         if etag_compare is not None:
             pulumi.set(__self__, "etag_compare", etag_compare)
         if etag_save is not None:
             pulumi.set(__self__, "etag_save", etag_save)
         if expect100_timeout is not None:
             pulumi.set(__self__, "expect100_timeout", expect100_timeout)
         if fail is not None:
@@ -295,43 +473,25 @@
             pulumi.set(__self__, "ftp_port", ftp_port)
         if ftp_pret is not None:
             pulumi.set(__self__, "ftp_pret", ftp_pret)
         if ftp_skip_pasv_ip is not None:
             pulumi.set(__self__, "ftp_skip_pasv_ip", ftp_skip_pasv_ip)
         if ftp_ssl_ccc_mode is not None:
             pulumi.set(__self__, "ftp_ssl_ccc_mode", ftp_ssl_ccc_mode)
-        if lifecycle is not None:
-            pulumi.set(__self__, "lifecycle", lifecycle)
-        if stdin is not None:
-            pulumi.set(__self__, "stdin", stdin)
-        if triggers is not None:
-            pulumi.set(__self__, "triggers", triggers)
-
-    @property
-    @pulumi.getter
-    def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
-        """
-        Connection details for the remote system
-        """
-        return pulumi.get(self, "connection")
-
-    @connection.setter
-    def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
-        pulumi.set(self, "connection", value)
 
     @property
     @pulumi.getter
-    def urls(self) -> pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]:
+    def urls(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
         Corresponds to the URLs argument.
         """
         return pulumi.get(self, "urls")
 
     @urls.setter
-    def urls(self, value: pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]):
+    def urls(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "urls", value)
 
     @property
     @pulumi.getter(name="abstractUnixSocket")
     def abstract_unix_socket(self) -> Optional[pulumi.Input[str]]:
         """
         (HTTP) Connect through an abstract Unix domain socket, instead of using the network.
@@ -399,26 +559,14 @@
         return pulumi.get(self, "basic")
 
     @basic.setter
     def basic(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "basic", value)
 
     @property
-    @pulumi.getter(name="binaryPath")
-    def binary_path(self) -> Optional[pulumi.Input[str]]:
-        """
-        Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        """
-        return pulumi.get(self, "binary_path")
-
-    @binary_path.setter
-    def binary_path(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "binary_path", value)
-
-    @property
     @pulumi.getter
     def cacert(self) -> Optional[pulumi.Input[str]]:
         """
         (TLS)  Tells curl to use the specified certificate file to verify the peer.
         """
         return pulumi.get(self, "cacert")
 
@@ -891,26 +1039,14 @@
         return pulumi.get(self, "engine")
 
     @engine.setter
     def engine(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "engine", value)
 
     @property
-    @pulumi.getter
-    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
-        """
-        Environment variables
-        """
-        return pulumi.get(self, "environment")
-
-    @environment.setter
-    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
-        pulumi.set(self, "environment", value)
-
-    @property
     @pulumi.getter(name="etagCompare")
     def etag_compare(self) -> Optional[pulumi.Input[str]]:
         """
         (HTTP) This option makes a conditional HTTP request for the specific ETag read from the given file by sending a custom If-None-Match header using the stored ETag.
         """
         return pulumi.get(self, "etag_compare")
 
@@ -1130,993 +1266,1478 @@
         """
         return pulumi.get(self, "ftp_ssl_ccc_mode")
 
     @ftp_ssl_ccc_mode.setter
     def ftp_ssl_ccc_mode(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ftp_ssl_ccc_mode", value)
 
+
+@pulumi.input_type
+class EtcdctlOptsArgs:
+    def __init__(__self__, *,
+                 commands: pulumi.Input['EtcdctlCommand'],
+                 ca_cert: Optional[pulumi.Input[str]] = None,
+                 cert: Optional[pulumi.Input[str]] = None,
+                 endpoints: Optional[pulumi.Input[str]] = None,
+                 key: Optional[pulumi.Input[str]] = None):
+        """
+        Abstraction over the `etcdctl` utility on a remote system.
+        :param pulumi.Input['EtcdctlCommand'] commands: TODO
+        :param pulumi.Input[str] ca_cert: TODO
+        :param pulumi.Input[str] cert: TODO
+        :param pulumi.Input[str] endpoints: TODO
+        :param pulumi.Input[str] key: TODO
+        """
+        pulumi.set(__self__, "commands", commands)
+        if ca_cert is not None:
+            pulumi.set(__self__, "ca_cert", ca_cert)
+        if cert is not None:
+            pulumi.set(__self__, "cert", cert)
+        if endpoints is not None:
+            pulumi.set(__self__, "endpoints", endpoints)
+        if key is not None:
+            pulumi.set(__self__, "key", key)
+
     @property
     @pulumi.getter
-    def lifecycle(self) -> Optional['CommandLifecycle']:
+    def commands(self) -> pulumi.Input['EtcdctlCommand']:
+        """
+        TODO
         """
-        At what stage(s) in the resource lifecycle should the command be run
+        return pulumi.get(self, "commands")
+
+    @commands.setter
+    def commands(self, value: pulumi.Input['EtcdctlCommand']):
+        pulumi.set(self, "commands", value)
+
+    @property
+    @pulumi.getter(name="caCert")
+    def ca_cert(self) -> Optional[pulumi.Input[str]]:
         """
-        return pulumi.get(self, "lifecycle")
+        TODO
+        """
+        return pulumi.get(self, "ca_cert")
 
-    @lifecycle.setter
-    def lifecycle(self, value: Optional['CommandLifecycle']):
-        pulumi.set(self, "lifecycle", value)
+    @ca_cert.setter
+    def ca_cert(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ca_cert", value)
 
     @property
     @pulumi.getter
-    def stdin(self) -> Optional[pulumi.Input[str]]:
+    def cert(self) -> Optional[pulumi.Input[str]]:
         """
         TODO
         """
-        return pulumi.get(self, "stdin")
+        return pulumi.get(self, "cert")
 
-    @stdin.setter
-    def stdin(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "stdin", value)
+    @cert.setter
+    def cert(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cert", value)
 
     @property
     @pulumi.getter
-    def triggers(self) -> Optional[pulumi.Input[Sequence[Any]]]:
+    def endpoints(self) -> Optional[pulumi.Input[str]]:
         """
         TODO
         """
-        return pulumi.get(self, "triggers")
+        return pulumi.get(self, "endpoints")
 
-    @triggers.setter
-    def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
-        pulumi.set(self, "triggers", value)
+    @endpoints.setter
+    def endpoints(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "endpoints", value)
 
+    @property
+    @pulumi.getter
+    def key(self) -> Optional[pulumi.Input[str]]:
+        """
+        TODO
+        """
+        return pulumi.get(self, "key")
 
-class Curl(pulumi.ComponentResource):
-    @overload
-    def __init__(__self__,
-                 resource_name: str,
-                 opts: Optional[pulumi.ResourceOptions] = None,
-                 abstract_unix_socket: Optional[pulumi.Input[str]] = None,
-                 alt_svc: Optional[pulumi.Input[str]] = None,
-                 any_auth: Optional[pulumi.Input[bool]] = None,
-                 append: Optional[pulumi.Input[bool]] = None,
-                 aws_sigv4: Optional[pulumi.Input[str]] = None,
-                 basic: Optional[pulumi.Input[bool]] = None,
-                 binary_path: Optional[pulumi.Input[str]] = None,
-                 cacert: Optional[pulumi.Input[str]] = None,
-                 capath: Optional[pulumi.Input[str]] = None,
-                 cert: Optional[pulumi.Input[str]] = None,
-                 cert_status: Optional[pulumi.Input[bool]] = None,
-                 cert_type: Optional[pulumi.Input['CurlCertType']] = None,
-                 ciphers: Optional[pulumi.Input[str]] = None,
-                 compressed: Optional[pulumi.Input[bool]] = None,
-                 compressed_ssh: Optional[pulumi.Input[bool]] = None,
-                 config: Optional[pulumi.Input[str]] = None,
-                 connect_timeout: Optional[pulumi.Input[int]] = None,
-                 connect_to: Optional[pulumi.Input[str]] = None,
-                 connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 continue_at: Optional[pulumi.Input[str]] = None,
-                 cookie: Optional[pulumi.Input[str]] = None,
-                 cookie_jar: Optional[pulumi.Input[str]] = None,
-                 create_dirs: Optional[pulumi.Input[bool]] = None,
-                 create_file_mode: Optional[pulumi.Input[str]] = None,
-                 crlf: Optional[pulumi.Input[bool]] = None,
-                 crlf_file: Optional[pulumi.Input[str]] = None,
-                 curves: Optional[pulumi.Input[str]] = None,
-                 data: Optional[pulumi.Input[str]] = None,
-                 data_ascii: Optional[pulumi.Input[str]] = None,
-                 data_binary: Optional[pulumi.Input[str]] = None,
-                 data_raw: Optional[pulumi.Input[str]] = None,
-                 data_url_encode: Optional[pulumi.Input[str]] = None,
-                 delegation: Optional[pulumi.Input['CurlDelegationLevel']] = None,
-                 digest: Optional[pulumi.Input[bool]] = None,
-                 disable: Optional[pulumi.Input[bool]] = None,
-                 disable_eprt: Optional[pulumi.Input[bool]] = None,
-                 disable_epsv: Optional[pulumi.Input[bool]] = None,
-                 disallow_username_in_url: Optional[pulumi.Input[bool]] = None,
-                 dns_interface: Optional[pulumi.Input[str]] = None,
-                 dns_ipv4_addr: Optional[pulumi.Input[str]] = None,
-                 dns_ipv6_addr: Optional[pulumi.Input[str]] = None,
-                 dns_servers: Optional[pulumi.Input[str]] = None,
-                 doh_cert_status: Optional[pulumi.Input[bool]] = None,
-                 doh_insecure: Optional[pulumi.Input[bool]] = None,
-                 doh_url: Optional[pulumi.Input[str]] = None,
-                 dump_header: Optional[pulumi.Input[str]] = None,
-                 egd_file: Optional[pulumi.Input[str]] = None,
-                 engine: Optional[pulumi.Input[str]] = None,
-                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 etag_compare: Optional[pulumi.Input[str]] = None,
-                 etag_save: Optional[pulumi.Input[str]] = None,
-                 expect100_timeout: Optional[pulumi.Input[int]] = None,
-                 fail: Optional[pulumi.Input[bool]] = None,
-                 fail_early: Optional[pulumi.Input[bool]] = None,
-                 fail_with_body: Optional[pulumi.Input[bool]] = None,
-                 false_start: Optional[pulumi.Input[bool]] = None,
-                 form: Optional[pulumi.Input[str]] = None,
-                 form_escape: Optional[pulumi.Input[bool]] = None,
-                 form_name: Optional[pulumi.Input[str]] = None,
-                 ftp_account: Optional[pulumi.Input[str]] = None,
-                 ftp_alternative_user: Optional[pulumi.Input[str]] = None,
-                 ftp_create_dirs: Optional[pulumi.Input[bool]] = None,
-                 ftp_method: Optional[pulumi.Input[str]] = None,
-                 ftp_pasv: Optional[pulumi.Input[bool]] = None,
-                 ftp_port: Optional[pulumi.Input[str]] = None,
-                 ftp_pret: Optional[pulumi.Input[bool]] = None,
-                 ftp_skip_pasv_ip: Optional[pulumi.Input[bool]] = None,
-                 ftp_ssl_ccc_mode: Optional[pulumi.Input[str]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 stdin: Optional[pulumi.Input[str]] = None,
-                 triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 urls: Optional[pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]] = None,
-                 __props__=None):
+    @key.setter
+    def key(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "key", value)
+
+
+@pulumi.input_type
+class HostnamectlOptsArgs:
+    def __init__(__self__, *,
+                 command: pulumi.Input['HostnamectlCommand'],
+                 arg: Optional[pulumi.Input[str]] = None,
+                 help: Optional[pulumi.Input[bool]] = None,
+                 host: Optional[pulumi.Input[str]] = None,
+                 json: Optional[pulumi.Input['HostnamectlJsonMode']] = None,
+                 machine: Optional[pulumi.Input[str]] = None,
+                 no_ask_password: Optional[pulumi.Input[bool]] = None,
+                 pretty: Optional[pulumi.Input[bool]] = None,
+                 static: Optional[pulumi.Input[bool]] = None,
+                 transient: Optional[pulumi.Input[bool]] = None,
+                 version: Optional[pulumi.Input[bool]] = None):
+        """
+        Abstraction over the `hostnamectl` utility on a remote system.
+        :param pulumi.Input['HostnamectlCommand'] command: Corresponds to the {COMMAND} argument.
+        :param pulumi.Input[str] arg: The argument for the specified `command`.
+        :param pulumi.Input[bool] help: Print a short help text and exit.
+        :param pulumi.Input[str] host: Execute the operation remotely. Specify a hostname, or a username and hostname separated by '@', to connect to.
+        :param pulumi.Input['HostnamectlJsonMode'] json: Shows output formatted as JSON.
+        :param pulumi.Input[str] machine: Execute operation on a local container. Specify a container name to connect to, optionally prefixed by a user name to connect as and a separating '@' character.
+        :param pulumi.Input[bool] no_ask_password: Do not query the user for authentication for privileged operations.
+        :param pulumi.Input[bool] pretty: If status is invoked (or no explicit command is given) and one of these switches is specified, hostnamectl will print out just this selected hostname. Same as `static` and `transient`.
+        :param pulumi.Input[bool] static: If status is invoked (or no explicit command is given) and one of these switches is specified, hostnamectl will print out just this selected hostname. Same as `transient` and `pretty`.
+        :param pulumi.Input[bool] transient: If status is invoked (or no explicit command is given) and one of these switches is specified, hostnamectl will print out just this selected hostname. Same as `static` and `pretty`.
+        :param pulumi.Input[bool] version: Print a short version string and exit.
+        """
+        pulumi.set(__self__, "command", command)
+        if arg is not None:
+            pulumi.set(__self__, "arg", arg)
+        if help is not None:
+            pulumi.set(__self__, "help", help)
+        if host is not None:
+            pulumi.set(__self__, "host", host)
+        if json is not None:
+            pulumi.set(__self__, "json", json)
+        if machine is not None:
+            pulumi.set(__self__, "machine", machine)
+        if no_ask_password is not None:
+            pulumi.set(__self__, "no_ask_password", no_ask_password)
+        if pretty is not None:
+            pulumi.set(__self__, "pretty", pretty)
+        if static is not None:
+            pulumi.set(__self__, "static", static)
+        if transient is not None:
+            pulumi.set(__self__, "transient", transient)
+        if version is not None:
+            pulumi.set(__self__, "version", version)
+
+    @property
+    @pulumi.getter
+    def command(self) -> pulumi.Input['HostnamectlCommand']:
         """
-        Abstraction over the `curl` utility on a remote system. Transfer a URL.
+        Corresponds to the {COMMAND} argument.
+        """
+        return pulumi.get(self, "command")
 
-        :param str resource_name: The name of the resource.
-        :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] abstract_unix_socket: (HTTP) Connect through an abstract Unix domain socket, instead of using the network.
-        :param pulumi.Input[str] alt_svc: (HTTPS)  This  option enables the alt-svc parser in curl.
-        :param pulumi.Input[bool] any_auth: (HTTP) Tells curl to figure out authentication method by itself, and use the most secure one the remote site claims to support.
-        :param pulumi.Input[bool] append: (FTP SFTP) When used in an upload, this makes curl append to the target file instead of overwriting it.
-        :param pulumi.Input[str] aws_sigv4: Use AWS V4 signature authentication in the transfer.
-        :param pulumi.Input[bool] basic: (HTTP) Tells curl to use HTTP Basic authentication with the remote host.
-        :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param pulumi.Input[str] cacert: (TLS)  Tells curl to use the specified certificate file to verify the peer.
-        :param pulumi.Input[str] capath: (TLS) Tells curl to use the specified certificate directory to verify the peer.
-        :param pulumi.Input[str] cert: (TLS)  Tells  curl to use the specified client certificate file when getting a file with HTTPS, FTPS or another SSL-based protocol.
-        :param pulumi.Input[bool] cert_status: (TLS) Tells curl to verify the status of the server certificate by using the Certificate Status Request (aka. OCSP stapling) TLS extension.
-        :param pulumi.Input['CurlCertType'] cert_type: (TLS) Tells curl what type the provided client certificate is using.
-        :param pulumi.Input[str] ciphers: (TLS) Specifies which ciphers to use in the connection.
-        :param pulumi.Input[bool] compressed: (HTTP) Request a compressed response using one of the algorithms curl supports, and automatically decompress the content.
-        :param pulumi.Input[bool] compressed_ssh: (SCP SFTP) Enables built-in SSH compression.
-        :param pulumi.Input[str] config: Specify a text file to read curl arguments from.
-        :param pulumi.Input[int] connect_timeout: Maximum  time  in seconds that you allow curl's connection to take.
-        :param pulumi.Input[str] connect_to: For a request to the given HOST1:PORT1 pair, connect to HOST2:PORT2 instead.
-        :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.Input[str] continue_at: Continue/Resume a previous file transfer at the given offset.
-        :param pulumi.Input[str] cookie: (HTTP) Pass the data to the HTTP server in the Cookie header.
-        :param pulumi.Input[str] cookie_jar: (HTTP)  Specify  to which file you want curl to write all cookies after a completed operation.
-        :param pulumi.Input[bool] create_dirs: When used in conjunction with the -o, --output option, curl will create the necessary local directory hierarchy as needed.
-        :param pulumi.Input[str] create_file_mode: (SFTP SCP FILE) When curl is used to create files remotely using one of the supported protocols, this option allows the user to set which 'mode' to set on the file at creation time, instead of the default 0644.
-        :param pulumi.Input[bool] crlf: (FTP SMTP) Convert LF to CRLF in upload. Useful for MVS (OS/390).
-        :param pulumi.Input[str] crlf_file: (TLS) Provide a file using PEM format with a Certificate Revocation List that may specify peer certificates that are to be considered revoked.
-        :param pulumi.Input[str] curves: (TLS)  Tells curl to request specific curves to use during SSL session establishment according to RFC 8422, 5.1.
-        :param pulumi.Input[str] data: (HTTP  MQTT) Sends the specified data in a POST request to the HTTP server, in the same way that a browser does when a user has filled in an HTML form and presses the submit button.
-        :param pulumi.Input[str] data_ascii: (HTTP) This is just an alias for -d, --data.
-        :param pulumi.Input[str] data_binary: (HTTP) This posts data exactly as specified with no extra processing whatsoever.
-        :param pulumi.Input[str] data_raw: (HTTP) This posts data similarly to -d, --data but without the special interpretation of the @ character.
-        :param pulumi.Input[str] data_url_encode: (HTTP) This posts data, similar to the other -d, --data options with the exception that this performs URL-encoding.
-        :param pulumi.Input['CurlDelegationLevel'] delegation: (GSS/kerberos) Set LEVEL to tell the server what it is allowed to delegate when it comes to user credentials.
-        :param pulumi.Input[bool] digest: (HTTP) Enables HTTP Digest authentication.
-        :param pulumi.Input[bool] disable: If used as the first parameter on the command line, the curlrc config file will not be read and used.
-        :param pulumi.Input[bool] disable_eprt: (FTP) Tell curl to disable the use of the EPRT and LPRT commands when doing active FTP transfers
-        :param pulumi.Input[bool] disable_epsv: (FTP)  Tell  curl to disable the use of the EPSV command when doing passive FTP transfers
-        :param pulumi.Input[bool] disallow_username_in_url: (HTTP) This tells curl to exit if passed a url containing a username.
-        :param pulumi.Input[str] dns_interface: (DNS)  Tell  curl  to send outgoing DNS requests through <interface>.
-        :param pulumi.Input[str] dns_ipv4_addr: (DNS) Tell curl to bind to <ip-address> when making IPv4 DNS requests, so that the DNS requests originate from this address.
-        :param pulumi.Input[str] dns_ipv6_addr: (DNS) Tell curl to bind to <ip-address> when making IPv6 DNS requests, so that the DNS requests originate from this address.
-        :param pulumi.Input[str] dns_servers: Set the list of DNS servers to be used instead of the system default.
-        :param pulumi.Input[bool] doh_cert_status: Same as --cert-status but used for DoH (DNS-over-HTTPS).
-        :param pulumi.Input[bool] doh_insecure: Same as -k, --insecure but used for DoH (DNS-over-HTTPS).
-        :param pulumi.Input[str] doh_url: Specifies which DNS-over-HTTPS (DoH) server to use to resolve hostnames, instead of using the default name resolver mechanism.
-        :param pulumi.Input[str] dump_header: (HTTP FTP) Write the received protocol headers to the specified file.
-        :param pulumi.Input[str] egd_file: (TLS) Specify the path name to the Entropy Gathering Daemon socket.
-        :param pulumi.Input[str] engine: (TLS) Select the OpenSSL crypto engine to use for cipher operations.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
-        :param pulumi.Input[str] etag_compare: (HTTP) This option makes a conditional HTTP request for the specific ETag read from the given file by sending a custom If-None-Match header using the stored ETag.
-        :param pulumi.Input[str] etag_save: (HTTP) This option saves an HTTP ETag to the specified file.
-        :param pulumi.Input[int] expect100_timeout: (HTTP)  Maximum  time in seconds that you allow curl to wait for a 100-continue response when curl emits an Expects: 100-continue header in its request.
-        :param pulumi.Input[bool] fail: (HTTP) Fail silently (no output at all) on server errors.
-        :param pulumi.Input[bool] fail_early: Fail and exit on the first detected transfer error.
-        :param pulumi.Input[bool] fail_with_body: (HTTP)  Return an error on server errors where the HTTP response code is 400 or greater).
-        :param pulumi.Input[bool] false_start: (TLS) Tells curl to use false start during the TLS handshake.
-        :param pulumi.Input[str] form: (HTTP SMTP IMAP) For HTTP protocol family, this lets curl emulate a filled-in form in which a user has pressed the submit button.
-        :param pulumi.Input[bool] form_escape: (HTTP) Tells curl to pass on names of multipart form fields and files using backslash-escaping instead of percent-encoding.
-        :param pulumi.Input[str] form_name: (HTTP SMTP IMAP) Similar to -F, --form except that the value string for the named parameter is used literally.
-        :param pulumi.Input[str] ftp_account: (FTP) When an FTP server asks for 'account data' after user name and password has been provided, this data is sent off using the ACCT command.
-        :param pulumi.Input[str] ftp_alternative_user: (FTP) If authenticating with the USER and PASS commands fails, send this command.
-        :param pulumi.Input[bool] ftp_create_dirs: (FTP  SFTP) When an FTP or SFTP URL/operation uses a path that does not currently exist on the server, the standard behavior of curl is to fail.
-        :param pulumi.Input[str] ftp_method: (FTP) Control what method curl should use to reach a file on an FTP(S) server.
-        :param pulumi.Input[bool] ftp_pasv: (FTP) Use passive mode for the data connection.
-        :param pulumi.Input[str] ftp_port: (FTP)  Reverses  the  default  initiator/listener  roles  when connecting with FTP.
-        :param pulumi.Input[bool] ftp_pret: (FTP) Tell curl to send a PRET command before PASV (and EPSV).
-        :param pulumi.Input[bool] ftp_skip_pasv_ip: (FTP)  Tell  curl  to  not use the IP address the server suggests in its response to curl's PASV command when curl connects the data connection.
-        :param pulumi.Input[str] ftp_ssl_ccc_mode: (FTP) Sets the CCC mode. The passive mode will not initiate the shutdown, but instead wait for the server to do it, and will not reply to the shutdown from the  server.
-        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
-        :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]] urls: Corresponds to the URLs argument.
-        """
-        ...
-    @overload
-    def __init__(__self__,
-                 resource_name: str,
-                 args: CurlArgs,
-                 opts: Optional[pulumi.ResourceOptions] = None):
+    @command.setter
+    def command(self, value: pulumi.Input['HostnamectlCommand']):
+        pulumi.set(self, "command", value)
+
+    @property
+    @pulumi.getter
+    def arg(self) -> Optional[pulumi.Input[str]]:
         """
-        Abstraction over the `curl` utility on a remote system. Transfer a URL.
+        The argument for the specified `command`.
+        """
+        return pulumi.get(self, "arg")
 
-        :param str resource_name: The name of the resource.
-        :param CurlArgs args: The arguments to use to populate this resource's properties.
-        :param pulumi.ResourceOptions opts: Options for the resource.
-        """
-        ...
-    def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(CurlArgs, pulumi.ResourceOptions, *args, **kwargs)
-        if resource_args is not None:
-            __self__._internal_init(resource_name, opts, **resource_args.__dict__)
-        else:
-            __self__._internal_init(resource_name, *args, **kwargs)
-
-    def _internal_init(__self__,
-                 resource_name: str,
-                 opts: Optional[pulumi.ResourceOptions] = None,
-                 abstract_unix_socket: Optional[pulumi.Input[str]] = None,
-                 alt_svc: Optional[pulumi.Input[str]] = None,
-                 any_auth: Optional[pulumi.Input[bool]] = None,
-                 append: Optional[pulumi.Input[bool]] = None,
-                 aws_sigv4: Optional[pulumi.Input[str]] = None,
-                 basic: Optional[pulumi.Input[bool]] = None,
-                 binary_path: Optional[pulumi.Input[str]] = None,
-                 cacert: Optional[pulumi.Input[str]] = None,
-                 capath: Optional[pulumi.Input[str]] = None,
-                 cert: Optional[pulumi.Input[str]] = None,
-                 cert_status: Optional[pulumi.Input[bool]] = None,
-                 cert_type: Optional[pulumi.Input['CurlCertType']] = None,
-                 ciphers: Optional[pulumi.Input[str]] = None,
-                 compressed: Optional[pulumi.Input[bool]] = None,
-                 compressed_ssh: Optional[pulumi.Input[bool]] = None,
-                 config: Optional[pulumi.Input[str]] = None,
-                 connect_timeout: Optional[pulumi.Input[int]] = None,
-                 connect_to: Optional[pulumi.Input[str]] = None,
-                 connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 continue_at: Optional[pulumi.Input[str]] = None,
-                 cookie: Optional[pulumi.Input[str]] = None,
-                 cookie_jar: Optional[pulumi.Input[str]] = None,
-                 create_dirs: Optional[pulumi.Input[bool]] = None,
-                 create_file_mode: Optional[pulumi.Input[str]] = None,
-                 crlf: Optional[pulumi.Input[bool]] = None,
-                 crlf_file: Optional[pulumi.Input[str]] = None,
-                 curves: Optional[pulumi.Input[str]] = None,
-                 data: Optional[pulumi.Input[str]] = None,
-                 data_ascii: Optional[pulumi.Input[str]] = None,
-                 data_binary: Optional[pulumi.Input[str]] = None,
-                 data_raw: Optional[pulumi.Input[str]] = None,
-                 data_url_encode: Optional[pulumi.Input[str]] = None,
-                 delegation: Optional[pulumi.Input['CurlDelegationLevel']] = None,
-                 digest: Optional[pulumi.Input[bool]] = None,
-                 disable: Optional[pulumi.Input[bool]] = None,
-                 disable_eprt: Optional[pulumi.Input[bool]] = None,
-                 disable_epsv: Optional[pulumi.Input[bool]] = None,
-                 disallow_username_in_url: Optional[pulumi.Input[bool]] = None,
-                 dns_interface: Optional[pulumi.Input[str]] = None,
-                 dns_ipv4_addr: Optional[pulumi.Input[str]] = None,
-                 dns_ipv6_addr: Optional[pulumi.Input[str]] = None,
-                 dns_servers: Optional[pulumi.Input[str]] = None,
-                 doh_cert_status: Optional[pulumi.Input[bool]] = None,
-                 doh_insecure: Optional[pulumi.Input[bool]] = None,
-                 doh_url: Optional[pulumi.Input[str]] = None,
-                 dump_header: Optional[pulumi.Input[str]] = None,
-                 egd_file: Optional[pulumi.Input[str]] = None,
-                 engine: Optional[pulumi.Input[str]] = None,
-                 environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 etag_compare: Optional[pulumi.Input[str]] = None,
-                 etag_save: Optional[pulumi.Input[str]] = None,
-                 expect100_timeout: Optional[pulumi.Input[int]] = None,
-                 fail: Optional[pulumi.Input[bool]] = None,
-                 fail_early: Optional[pulumi.Input[bool]] = None,
-                 fail_with_body: Optional[pulumi.Input[bool]] = None,
-                 false_start: Optional[pulumi.Input[bool]] = None,
-                 form: Optional[pulumi.Input[str]] = None,
-                 form_escape: Optional[pulumi.Input[bool]] = None,
-                 form_name: Optional[pulumi.Input[str]] = None,
-                 ftp_account: Optional[pulumi.Input[str]] = None,
-                 ftp_alternative_user: Optional[pulumi.Input[str]] = None,
-                 ftp_create_dirs: Optional[pulumi.Input[bool]] = None,
-                 ftp_method: Optional[pulumi.Input[str]] = None,
-                 ftp_pasv: Optional[pulumi.Input[bool]] = None,
-                 ftp_port: Optional[pulumi.Input[str]] = None,
-                 ftp_pret: Optional[pulumi.Input[bool]] = None,
-                 ftp_skip_pasv_ip: Optional[pulumi.Input[bool]] = None,
-                 ftp_ssl_ccc_mode: Optional[pulumi.Input[str]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 stdin: Optional[pulumi.Input[str]] = None,
-                 triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 urls: Optional[pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]] = None,
-                 __props__=None):
-        opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
-        if not isinstance(opts, pulumi.ResourceOptions):
-            raise TypeError('Expected resource options to be a ResourceOptions instance')
-        if opts.id is not None:
-            raise ValueError('ComponentResource classes do not support opts.id')
-        else:
-            if __props__ is not None:
-                raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = CurlArgs.__new__(CurlArgs)
-
-            __props__.__dict__["abstract_unix_socket"] = abstract_unix_socket
-            __props__.__dict__["alt_svc"] = alt_svc
-            __props__.__dict__["any_auth"] = any_auth
-            __props__.__dict__["append"] = append
-            __props__.__dict__["aws_sigv4"] = aws_sigv4
-            __props__.__dict__["basic"] = basic
-            __props__.__dict__["binary_path"] = binary_path
-            __props__.__dict__["cacert"] = cacert
-            __props__.__dict__["capath"] = capath
-            __props__.__dict__["cert"] = cert
-            __props__.__dict__["cert_status"] = cert_status
-            __props__.__dict__["cert_type"] = cert_type
-            __props__.__dict__["ciphers"] = ciphers
-            __props__.__dict__["compressed"] = compressed
-            __props__.__dict__["compressed_ssh"] = compressed_ssh
-            __props__.__dict__["config"] = config
-            __props__.__dict__["connect_timeout"] = connect_timeout
-            __props__.__dict__["connect_to"] = connect_to
-            if connection is None and not opts.urn:
-                raise TypeError("Missing required property 'connection'")
-            __props__.__dict__["connection"] = connection
-            __props__.__dict__["continue_at"] = continue_at
-            __props__.__dict__["cookie"] = cookie
-            __props__.__dict__["cookie_jar"] = cookie_jar
-            __props__.__dict__["create_dirs"] = create_dirs
-            __props__.__dict__["create_file_mode"] = create_file_mode
-            __props__.__dict__["crlf"] = crlf
-            __props__.__dict__["crlf_file"] = crlf_file
-            __props__.__dict__["curves"] = curves
-            __props__.__dict__["data"] = data
-            __props__.__dict__["data_ascii"] = data_ascii
-            __props__.__dict__["data_binary"] = data_binary
-            __props__.__dict__["data_raw"] = data_raw
-            __props__.__dict__["data_url_encode"] = data_url_encode
-            __props__.__dict__["delegation"] = delegation
-            __props__.__dict__["digest"] = digest
-            __props__.__dict__["disable"] = disable
-            __props__.__dict__["disable_eprt"] = disable_eprt
-            __props__.__dict__["disable_epsv"] = disable_epsv
-            __props__.__dict__["disallow_username_in_url"] = disallow_username_in_url
-            __props__.__dict__["dns_interface"] = dns_interface
-            __props__.__dict__["dns_ipv4_addr"] = dns_ipv4_addr
-            __props__.__dict__["dns_ipv6_addr"] = dns_ipv6_addr
-            __props__.__dict__["dns_servers"] = dns_servers
-            __props__.__dict__["doh_cert_status"] = doh_cert_status
-            __props__.__dict__["doh_insecure"] = doh_insecure
-            __props__.__dict__["doh_url"] = doh_url
-            __props__.__dict__["dump_header"] = dump_header
-            __props__.__dict__["egd_file"] = egd_file
-            __props__.__dict__["engine"] = engine
-            __props__.__dict__["environment"] = environment
-            __props__.__dict__["etag_compare"] = etag_compare
-            __props__.__dict__["etag_save"] = etag_save
-            __props__.__dict__["expect100_timeout"] = expect100_timeout
-            __props__.__dict__["fail"] = fail
-            __props__.__dict__["fail_early"] = fail_early
-            __props__.__dict__["fail_with_body"] = fail_with_body
-            __props__.__dict__["false_start"] = false_start
-            __props__.__dict__["form"] = form
-            __props__.__dict__["form_escape"] = form_escape
-            __props__.__dict__["form_name"] = form_name
-            __props__.__dict__["ftp_account"] = ftp_account
-            __props__.__dict__["ftp_alternative_user"] = ftp_alternative_user
-            __props__.__dict__["ftp_create_dirs"] = ftp_create_dirs
-            __props__.__dict__["ftp_method"] = ftp_method
-            __props__.__dict__["ftp_pasv"] = ftp_pasv
-            __props__.__dict__["ftp_port"] = ftp_port
-            __props__.__dict__["ftp_pret"] = ftp_pret
-            __props__.__dict__["ftp_skip_pasv_ip"] = ftp_skip_pasv_ip
-            __props__.__dict__["ftp_ssl_ccc_mode"] = ftp_ssl_ccc_mode
-            __props__.__dict__["lifecycle"] = lifecycle
-            __props__.__dict__["stdin"] = stdin
-            __props__.__dict__["triggers"] = triggers
-            if urls is None and not opts.urn:
-                raise TypeError("Missing required property 'urls'")
-            __props__.__dict__["urls"] = urls
-            __props__.__dict__["command"] = None
-            __props__.__dict__["stderr"] = None
-            __props__.__dict__["stdout"] = None
-        super(Curl, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Curl',
-            resource_name,
-            __props__,
-            opts,
-            remote=True)
+    @arg.setter
+    def arg(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "arg", value)
 
     @property
-    @pulumi.getter(name="abstractUnixSocket")
-    def abstract_unix_socket(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def help(self) -> Optional[pulumi.Input[bool]]:
         """
-        (HTTP) Connect through an abstract Unix domain socket, instead of using the network.
+        Print a short help text and exit.
         """
-        return pulumi.get(self, "abstract_unix_socket")
+        return pulumi.get(self, "help")
+
+    @help.setter
+    def help(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "help", value)
 
     @property
-    @pulumi.getter(name="altSvc")
-    def alt_svc(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def host(self) -> Optional[pulumi.Input[str]]:
         """
-        (HTTPS)  This  option enables the alt-svc parser in curl.
+        Execute the operation remotely. Specify a hostname, or a username and hostname separated by '@', to connect to.
         """
-        return pulumi.get(self, "alt_svc")
+        return pulumi.get(self, "host")
+
+    @host.setter
+    def host(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "host", value)
 
     @property
-    @pulumi.getter(name="anyAuth")
-    def any_auth(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter
+    def json(self) -> Optional[pulumi.Input['HostnamectlJsonMode']]:
         """
-        (HTTP) Tells curl to figure out authentication method by itself, and use the most secure one the remote site claims to support.
+        Shows output formatted as JSON.
         """
-        return pulumi.get(self, "any_auth")
+        return pulumi.get(self, "json")
+
+    @json.setter
+    def json(self, value: Optional[pulumi.Input['HostnamectlJsonMode']]):
+        pulumi.set(self, "json", value)
 
     @property
     @pulumi.getter
-    def append(self) -> pulumi.Output[Optional[bool]]:
+    def machine(self) -> Optional[pulumi.Input[str]]:
         """
-        (FTP SFTP) When used in an upload, this makes curl append to the target file instead of overwriting it.
+        Execute operation on a local container. Specify a container name to connect to, optionally prefixed by a user name to connect as and a separating '@' character.
         """
-        return pulumi.get(self, "append")
+        return pulumi.get(self, "machine")
+
+    @machine.setter
+    def machine(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "machine", value)
 
     @property
-    @pulumi.getter(name="awsSigv4")
-    def aws_sigv4(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="noAskPassword")
+    def no_ask_password(self) -> Optional[pulumi.Input[bool]]:
         """
-        Use AWS V4 signature authentication in the transfer.
+        Do not query the user for authentication for privileged operations.
         """
-        return pulumi.get(self, "aws_sigv4")
+        return pulumi.get(self, "no_ask_password")
+
+    @no_ask_password.setter
+    def no_ask_password(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "no_ask_password", value)
 
     @property
     @pulumi.getter
-    def basic(self) -> pulumi.Output[Optional[bool]]:
+    def pretty(self) -> Optional[pulumi.Input[bool]]:
         """
-        (HTTP) Tells curl to use HTTP Basic authentication with the remote host.
+        If status is invoked (or no explicit command is given) and one of these switches is specified, hostnamectl will print out just this selected hostname. Same as `static` and `transient`.
         """
-        return pulumi.get(self, "basic")
+        return pulumi.get(self, "pretty")
+
+    @pretty.setter
+    def pretty(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "pretty", value)
 
     @property
-    @pulumi.getter(name="binaryPath")
-    def binary_path(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def static(self) -> Optional[pulumi.Input[bool]]:
         """
-        Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
+        If status is invoked (or no explicit command is given) and one of these switches is specified, hostnamectl will print out just this selected hostname. Same as `transient` and `pretty`.
         """
-        return pulumi.get(self, "binary_path")
+        return pulumi.get(self, "static")
+
+    @static.setter
+    def static(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "static", value)
 
     @property
     @pulumi.getter
-    def cacert(self) -> pulumi.Output[Optional[str]]:
+    def transient(self) -> Optional[pulumi.Input[bool]]:
         """
-        (TLS)  Tells curl to use the specified certificate file to verify the peer.
+        If status is invoked (or no explicit command is given) and one of these switches is specified, hostnamectl will print out just this selected hostname. Same as `static` and `pretty`.
         """
-        return pulumi.get(self, "cacert")
+        return pulumi.get(self, "transient")
+
+    @transient.setter
+    def transient(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "transient", value)
 
     @property
     @pulumi.getter
-    def capath(self) -> pulumi.Output[Optional[str]]:
+    def version(self) -> Optional[pulumi.Input[bool]]:
         """
-        (TLS) Tells curl to use the specified certificate directory to verify the peer.
+        Print a short version string and exit.
         """
-        return pulumi.get(self, "capath")
+        return pulumi.get(self, "version")
+
+    @version.setter
+    def version(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "version", value)
+
+
+@pulumi.input_type
+class MkdirOptsArgs:
+    def __init__(__self__, *,
+                 directory: pulumi.Input[str],
+                 parents: Optional[pulumi.Input[bool]] = None,
+                 remove_on_delete: Optional[pulumi.Input[bool]] = None):
+        """
+        Abstraction over the `mkdir` utility on a remote system.
+        :param pulumi.Input[str] directory: The fully qualified path of the directory on the remote system.
+        :param pulumi.Input[bool] parents: Corresponds to the `--parents` option.
+        :param pulumi.Input[bool] remove_on_delete: Remove the created directory when the `Mkdir` resource is deleted or updated.
+        """
+        pulumi.set(__self__, "directory", directory)
+        if parents is not None:
+            pulumi.set(__self__, "parents", parents)
+        if remove_on_delete is not None:
+            pulumi.set(__self__, "remove_on_delete", remove_on_delete)
 
     @property
     @pulumi.getter
-    def cert(self) -> pulumi.Output[Optional[str]]:
+    def directory(self) -> pulumi.Input[str]:
         """
-        (TLS)  Tells  curl to use the specified client certificate file when getting a file with HTTPS, FTPS or another SSL-based protocol.
+        The fully qualified path of the directory on the remote system.
         """
-        return pulumi.get(self, "cert")
+        return pulumi.get(self, "directory")
+
+    @directory.setter
+    def directory(self, value: pulumi.Input[str]):
+        pulumi.set(self, "directory", value)
 
     @property
-    @pulumi.getter(name="certStatus")
-    def cert_status(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter
+    def parents(self) -> Optional[pulumi.Input[bool]]:
         """
-        (TLS) Tells curl to verify the status of the server certificate by using the Certificate Status Request (aka. OCSP stapling) TLS extension.
+        Corresponds to the `--parents` option.
         """
-        return pulumi.get(self, "cert_status")
+        return pulumi.get(self, "parents")
+
+    @parents.setter
+    def parents(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "parents", value)
 
     @property
-    @pulumi.getter(name="certType")
-    def cert_type(self) -> pulumi.Output[Optional['CurlCertType']]:
+    @pulumi.getter(name="removeOnDelete")
+    def remove_on_delete(self) -> Optional[pulumi.Input[bool]]:
         """
-        (TLS) Tells curl what type the provided client certificate is using.
+        Remove the created directory when the `Mkdir` resource is deleted or updated.
         """
-        return pulumi.get(self, "cert_type")
+        return pulumi.get(self, "remove_on_delete")
+
+    @remove_on_delete.setter
+    def remove_on_delete(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "remove_on_delete", value)
+
+
+@pulumi.input_type
+class MktempOptsArgs:
+    def __init__(__self__, *,
+                 directory: Optional[pulumi.Input[bool]] = None,
+                 dry_run: Optional[pulumi.Input[bool]] = None,
+                 quiet: Optional[pulumi.Input[bool]] = None,
+                 suffix: Optional[pulumi.Input[str]] = None,
+                 template: Optional[pulumi.Input[str]] = None,
+                 tmpdir: Optional[pulumi.Input[str]] = None):
+        """
+        Abstraction over the `mktemp` utility on a remote system.
+        :param pulumi.Input[bool] directory: Corresponds to the `--directory` option.
+        :param pulumi.Input[bool] dry_run: Corresponds to the `--dry-run` option.
+        :param pulumi.Input[bool] quiet: Corresponds to the `--quiet` option.
+        :param pulumi.Input[str] suffix: Corresponds to the `--suffix` option.
+        :param pulumi.Input[str] template: Corresponds to the [TEMPLATE] argument.
+        :param pulumi.Input[str] tmpdir: Corresponds to the `--tmpdir` option.
+        """
+        if directory is not None:
+            pulumi.set(__self__, "directory", directory)
+        if dry_run is not None:
+            pulumi.set(__self__, "dry_run", dry_run)
+        if quiet is not None:
+            pulumi.set(__self__, "quiet", quiet)
+        if suffix is not None:
+            pulumi.set(__self__, "suffix", suffix)
+        if template is not None:
+            pulumi.set(__self__, "template", template)
+        if tmpdir is not None:
+            pulumi.set(__self__, "tmpdir", tmpdir)
 
     @property
     @pulumi.getter
-    def ciphers(self) -> pulumi.Output[Optional[str]]:
+    def directory(self) -> Optional[pulumi.Input[bool]]:
         """
-        (TLS) Specifies which ciphers to use in the connection.
+        Corresponds to the `--directory` option.
         """
-        return pulumi.get(self, "ciphers")
+        return pulumi.get(self, "directory")
+
+    @directory.setter
+    def directory(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "directory", value)
+
+    @property
+    @pulumi.getter(name="dryRun")
+    def dry_run(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Corresponds to the `--dry-run` option.
+        """
+        return pulumi.get(self, "dry_run")
+
+    @dry_run.setter
+    def dry_run(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "dry_run", value)
 
     @property
     @pulumi.getter
-    def command(self) -> pulumi.Output['pulumi_command.remote.Command']:
+    def quiet(self) -> Optional[pulumi.Input[bool]]:
         """
-        The underlying command
+        Corresponds to the `--quiet` option.
         """
-        return pulumi.get(self, "command")
+        return pulumi.get(self, "quiet")
+
+    @quiet.setter
+    def quiet(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "quiet", value)
 
     @property
     @pulumi.getter
-    def compressed(self) -> pulumi.Output[Optional[bool]]:
+    def suffix(self) -> Optional[pulumi.Input[str]]:
         """
-        (HTTP) Request a compressed response using one of the algorithms curl supports, and automatically decompress the content.
+        Corresponds to the `--suffix` option.
         """
-        return pulumi.get(self, "compressed")
+        return pulumi.get(self, "suffix")
+
+    @suffix.setter
+    def suffix(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "suffix", value)
 
     @property
-    @pulumi.getter(name="compressedSsh")
-    def compressed_ssh(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter
+    def template(self) -> Optional[pulumi.Input[str]]:
         """
-        (SCP SFTP) Enables built-in SSH compression.
+        Corresponds to the [TEMPLATE] argument.
         """
-        return pulumi.get(self, "compressed_ssh")
+        return pulumi.get(self, "template")
+
+    @template.setter
+    def template(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "template", value)
 
     @property
     @pulumi.getter
-    def config(self) -> pulumi.Output[Optional[str]]:
+    def tmpdir(self) -> Optional[pulumi.Input[str]]:
         """
-        Specify a text file to read curl arguments from.
+        Corresponds to the `--tmpdir` option.
         """
-        return pulumi.get(self, "config")
+        return pulumi.get(self, "tmpdir")
+
+    @tmpdir.setter
+    def tmpdir(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "tmpdir", value)
+
+
+@pulumi.input_type
+class MvOptsArgs:
+    def __init__(__self__, *,
+                 source: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 backup: Optional[bool] = None,
+                 context: Optional[pulumi.Input[bool]] = None,
+                 control: Optional[pulumi.Input[bool]] = None,
+                 dest: Optional[pulumi.Input[str]] = None,
+                 directory: Optional[pulumi.Input[str]] = None,
+                 force: Optional[pulumi.Input[bool]] = None,
+                 no_clobber: Optional[pulumi.Input[bool]] = None,
+                 no_target_directory: Optional[pulumi.Input[bool]] = None,
+                 strip_trailing_slashes: Optional[pulumi.Input[bool]] = None,
+                 suffix: Optional[pulumi.Input[str]] = None,
+                 target_directory: Optional[pulumi.Input[bool]] = None,
+                 update: Optional[pulumi.Input[bool]] = None,
+                 verbose: Optional[pulumi.Input[bool]] = None):
+        """
+        Abstraction over the `mv` utility on a remote system.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] source: Corresponds to the [SOURCE] argument.
+        :param bool backup: Corresponds to the `-b` and `--backup` options depending on whether [CONTROL] is supplied.
+        :param pulumi.Input[bool] context: Corresponds to the `--context` option.
+        :param pulumi.Input[bool] control: Corresponds to the [CONTROL] argument for the `--backup` option.
+        :param pulumi.Input[str] dest: Corresponds to the [DEST] argument.
+        :param pulumi.Input[str] directory: Corresponds to the [DIRECTORY] argument.
+        :param pulumi.Input[bool] force: Corresponds to the `--force` option.
+        :param pulumi.Input[bool] no_clobber: Corresponds to the `--no-clobber` option.
+        :param pulumi.Input[bool] no_target_directory: Corresponds to the `--no-target-directory` option.
+        :param pulumi.Input[bool] strip_trailing_slashes: Corresponds to the `--strip-trailing-slashes` option.
+        :param pulumi.Input[str] suffix: Corresponds to the `--suffix` option.
+        :param pulumi.Input[bool] target_directory: Corresponds to the `--target-directory` option.
+        :param pulumi.Input[bool] update: Corresponds to the `--update` option.
+        :param pulumi.Input[bool] verbose: Corresponds to the `--verbose` option.
+        """
+        pulumi.set(__self__, "source", source)
+        if backup is not None:
+            pulumi.set(__self__, "backup", backup)
+        if context is not None:
+            pulumi.set(__self__, "context", context)
+        if control is not None:
+            pulumi.set(__self__, "control", control)
+        if dest is not None:
+            pulumi.set(__self__, "dest", dest)
+        if directory is not None:
+            pulumi.set(__self__, "directory", directory)
+        if force is not None:
+            pulumi.set(__self__, "force", force)
+        if no_clobber is not None:
+            pulumi.set(__self__, "no_clobber", no_clobber)
+        if no_target_directory is not None:
+            pulumi.set(__self__, "no_target_directory", no_target_directory)
+        if strip_trailing_slashes is not None:
+            pulumi.set(__self__, "strip_trailing_slashes", strip_trailing_slashes)
+        if suffix is not None:
+            pulumi.set(__self__, "suffix", suffix)
+        if target_directory is not None:
+            pulumi.set(__self__, "target_directory", target_directory)
+        if update is not None:
+            pulumi.set(__self__, "update", update)
+        if verbose is not None:
+            pulumi.set(__self__, "verbose", verbose)
 
     @property
-    @pulumi.getter(name="connectTimeout")
-    def connect_timeout(self) -> pulumi.Output[Optional[int]]:
+    @pulumi.getter
+    def source(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        Maximum  time  in seconds that you allow curl's connection to take.
+        Corresponds to the [SOURCE] argument.
         """
-        return pulumi.get(self, "connect_timeout")
+        return pulumi.get(self, "source")
+
+    @source.setter
+    def source(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "source", value)
 
     @property
-    @pulumi.getter(name="connectTo")
-    def connect_to(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def backup(self) -> Optional[bool]:
         """
-        For a request to the given HOST1:PORT1 pair, connect to HOST2:PORT2 instead.
+        Corresponds to the `-b` and `--backup` options depending on whether [CONTROL] is supplied.
         """
-        return pulumi.get(self, "connect_to")
+        return pulumi.get(self, "backup")
+
+    @backup.setter
+    def backup(self, value: Optional[bool]):
+        pulumi.set(self, "backup", value)
 
     @property
     @pulumi.getter
-    def connection(self) -> pulumi.Output['pulumi_command.remote.outputs.Connection']:
+    def context(self) -> Optional[pulumi.Input[bool]]:
         """
-        Connection details for the remote system
+        Corresponds to the `--context` option.
         """
-        return pulumi.get(self, "connection")
+        return pulumi.get(self, "context")
+
+    @context.setter
+    def context(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "context", value)
 
     @property
-    @pulumi.getter(name="continueAt")
-    def continue_at(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def control(self) -> Optional[pulumi.Input[bool]]:
         """
-        Continue/Resume a previous file transfer at the given offset.
+        Corresponds to the [CONTROL] argument for the `--backup` option.
         """
-        return pulumi.get(self, "continue_at")
+        return pulumi.get(self, "control")
+
+    @control.setter
+    def control(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "control", value)
 
     @property
     @pulumi.getter
-    def cookie(self) -> pulumi.Output[Optional[str]]:
+    def dest(self) -> Optional[pulumi.Input[str]]:
         """
-        (HTTP) Pass the data to the HTTP server in the Cookie header.
+        Corresponds to the [DEST] argument.
         """
-        return pulumi.get(self, "cookie")
+        return pulumi.get(self, "dest")
+
+    @dest.setter
+    def dest(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "dest", value)
 
     @property
-    @pulumi.getter(name="cookieJar")
-    def cookie_jar(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def directory(self) -> Optional[pulumi.Input[str]]:
         """
-        (HTTP)  Specify  to which file you want curl to write all cookies after a completed operation.
+        Corresponds to the [DIRECTORY] argument.
         """
-        return pulumi.get(self, "cookie_jar")
+        return pulumi.get(self, "directory")
+
+    @directory.setter
+    def directory(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "directory", value)
 
     @property
-    @pulumi.getter(name="createDirs")
-    def create_dirs(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter
+    def force(self) -> Optional[pulumi.Input[bool]]:
         """
-        When used in conjunction with the -o, --output option, curl will create the necessary local directory hierarchy as needed.
+        Corresponds to the `--force` option.
         """
-        return pulumi.get(self, "create_dirs")
+        return pulumi.get(self, "force")
+
+    @force.setter
+    def force(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "force", value)
 
     @property
-    @pulumi.getter(name="createFileMode")
-    def create_file_mode(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="noClobber")
+    def no_clobber(self) -> Optional[pulumi.Input[bool]]:
         """
-        (SFTP SCP FILE) When curl is used to create files remotely using one of the supported protocols, this option allows the user to set which 'mode' to set on the file at creation time, instead of the default 0644.
+        Corresponds to the `--no-clobber` option.
         """
-        return pulumi.get(self, "create_file_mode")
+        return pulumi.get(self, "no_clobber")
+
+    @no_clobber.setter
+    def no_clobber(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "no_clobber", value)
+
+    @property
+    @pulumi.getter(name="noTargetDirectory")
+    def no_target_directory(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Corresponds to the `--no-target-directory` option.
+        """
+        return pulumi.get(self, "no_target_directory")
+
+    @no_target_directory.setter
+    def no_target_directory(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "no_target_directory", value)
+
+    @property
+    @pulumi.getter(name="stripTrailingSlashes")
+    def strip_trailing_slashes(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Corresponds to the `--strip-trailing-slashes` option.
+        """
+        return pulumi.get(self, "strip_trailing_slashes")
+
+    @strip_trailing_slashes.setter
+    def strip_trailing_slashes(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "strip_trailing_slashes", value)
 
     @property
     @pulumi.getter
-    def crlf(self) -> pulumi.Output[Optional[bool]]:
+    def suffix(self) -> Optional[pulumi.Input[str]]:
         """
-        (FTP SMTP) Convert LF to CRLF in upload. Useful for MVS (OS/390).
+        Corresponds to the `--suffix` option.
         """
-        return pulumi.get(self, "crlf")
+        return pulumi.get(self, "suffix")
+
+    @suffix.setter
+    def suffix(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "suffix", value)
 
     @property
-    @pulumi.getter(name="crlfFile")
-    def crlf_file(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="targetDirectory")
+    def target_directory(self) -> Optional[pulumi.Input[bool]]:
         """
-        (TLS) Provide a file using PEM format with a Certificate Revocation List that may specify peer certificates that are to be considered revoked.
+        Corresponds to the `--target-directory` option.
         """
-        return pulumi.get(self, "crlf_file")
+        return pulumi.get(self, "target_directory")
+
+    @target_directory.setter
+    def target_directory(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "target_directory", value)
 
     @property
     @pulumi.getter
-    def curves(self) -> pulumi.Output[Optional[str]]:
+    def update(self) -> Optional[pulumi.Input[bool]]:
         """
-        (TLS)  Tells curl to request specific curves to use during SSL session establishment according to RFC 8422, 5.1.
+        Corresponds to the `--update` option.
         """
-        return pulumi.get(self, "curves")
+        return pulumi.get(self, "update")
+
+    @update.setter
+    def update(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "update", value)
 
     @property
     @pulumi.getter
-    def data(self) -> pulumi.Output[Optional[str]]:
+    def verbose(self) -> Optional[pulumi.Input[bool]]:
         """
-        (HTTP  MQTT) Sends the specified data in a POST request to the HTTP server, in the same way that a browser does when a user has filled in an HTML form and presses the submit button.
+        Corresponds to the `--verbose` option.
         """
-        return pulumi.get(self, "data")
+        return pulumi.get(self, "verbose")
+
+    @verbose.setter
+    def verbose(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "verbose", value)
+
+
+@pulumi.input_type
+class RmOptsArgs:
+    def __init__(__self__, *,
+                 files: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 dir: Optional[pulumi.Input[bool]] = None,
+                 force: Optional[pulumi.Input[bool]] = None,
+                 on_delete: Optional[pulumi.Input[bool]] = None,
+                 recursive: Optional[pulumi.Input[bool]] = None,
+                 verbose: Optional[pulumi.Input[bool]] = None):
+        """
+        Abstraction over the `rm` utility on a remote system.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] files: Corresponds to the [FILE] argument.
+        :param pulumi.Input[bool] dir: Corresponds to the `--dir` option.
+        :param pulumi.Input[bool] force: Corresponds to the `--force` option.
+        :param pulumi.Input[bool] on_delete: Whether rm should be run when the resource is created or deleted.
+        :param pulumi.Input[bool] recursive: Corresponds to the `--recursive` option.
+        :param pulumi.Input[bool] verbose: Corresponds to the `--verbose` option.
+        """
+        pulumi.set(__self__, "files", files)
+        if dir is not None:
+            pulumi.set(__self__, "dir", dir)
+        if force is not None:
+            pulumi.set(__self__, "force", force)
+        if on_delete is not None:
+            pulumi.set(__self__, "on_delete", on_delete)
+        if recursive is not None:
+            pulumi.set(__self__, "recursive", recursive)
+        if verbose is not None:
+            pulumi.set(__self__, "verbose", verbose)
 
     @property
-    @pulumi.getter(name="dataAscii")
-    def data_ascii(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def files(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        (HTTP) This is just an alias for -d, --data.
+        Corresponds to the [FILE] argument.
         """
-        return pulumi.get(self, "data_ascii")
+        return pulumi.get(self, "files")
+
+    @files.setter
+    def files(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "files", value)
 
     @property
-    @pulumi.getter(name="dataBinary")
-    def data_binary(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def dir(self) -> Optional[pulumi.Input[bool]]:
         """
-        (HTTP) This posts data exactly as specified with no extra processing whatsoever.
+        Corresponds to the `--dir` option.
         """
-        return pulumi.get(self, "data_binary")
+        return pulumi.get(self, "dir")
+
+    @dir.setter
+    def dir(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "dir", value)
 
     @property
-    @pulumi.getter(name="dataRaw")
-    def data_raw(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def force(self) -> Optional[pulumi.Input[bool]]:
         """
-        (HTTP) This posts data similarly to -d, --data but without the special interpretation of the @ character.
+        Corresponds to the `--force` option.
         """
-        return pulumi.get(self, "data_raw")
+        return pulumi.get(self, "force")
+
+    @force.setter
+    def force(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "force", value)
 
     @property
-    @pulumi.getter(name="dataUrlEncode")
-    def data_url_encode(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="onDelete")
+    def on_delete(self) -> Optional[pulumi.Input[bool]]:
         """
-        (HTTP) This posts data, similar to the other -d, --data options with the exception that this performs URL-encoding.
+        Whether rm should be run when the resource is created or deleted.
         """
-        return pulumi.get(self, "data_url_encode")
+        return pulumi.get(self, "on_delete")
+
+    @on_delete.setter
+    def on_delete(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "on_delete", value)
 
     @property
     @pulumi.getter
-    def delegation(self) -> pulumi.Output[Optional['CurlDelegationLevel']]:
+    def recursive(self) -> Optional[pulumi.Input[bool]]:
         """
-        (GSS/kerberos) Set LEVEL to tell the server what it is allowed to delegate when it comes to user credentials.
+        Corresponds to the `--recursive` option.
         """
-        return pulumi.get(self, "delegation")
+        return pulumi.get(self, "recursive")
+
+    @recursive.setter
+    def recursive(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "recursive", value)
 
     @property
     @pulumi.getter
-    def digest(self) -> pulumi.Output[Optional[bool]]:
+    def verbose(self) -> Optional[pulumi.Input[bool]]:
         """
-        (HTTP) Enables HTTP Digest authentication.
+        Corresponds to the `--verbose` option.
         """
-        return pulumi.get(self, "digest")
+        return pulumi.get(self, "verbose")
+
+    @verbose.setter
+    def verbose(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "verbose", value)
+
+
+@pulumi.input_type
+class SedOptsArgs:
+    def __init__(__self__, *,
+                 debug: Optional[pulumi.Input[bool]] = None,
+                 expressions: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 files: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 follow_symlinks: Optional[pulumi.Input[bool]] = None,
+                 help: Optional[pulumi.Input[bool]] = None,
+                 in_place: Optional[pulumi.Input[str]] = None,
+                 input_files: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 line_length: Optional[pulumi.Input[int]] = None,
+                 null_data: Optional[pulumi.Input[bool]] = None,
+                 posix: Optional[pulumi.Input[bool]] = None,
+                 quiet: Optional[pulumi.Input[bool]] = None,
+                 regexp_extended: Optional[pulumi.Input[bool]] = None,
+                 sandbox: Optional[pulumi.Input[bool]] = None,
+                 script: Optional[pulumi.Input[str]] = None,
+                 separate: Optional[pulumi.Input[bool]] = None,
+                 silent: Optional[pulumi.Input[bool]] = None,
+                 unbuffered: Optional[pulumi.Input[bool]] = None,
+                 version: Optional[pulumi.Input[bool]] = None):
+        """
+        Abstraction over the `sed` utility on a remote system.
+        :param pulumi.Input[bool] debug: annotate program execution.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] expressions: add the script to the commands to be executed.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] files: add the contents of script-file to the commands to be executed.
+        :param pulumi.Input[bool] follow_symlinks: follow symlinks when processing in place
+        :param pulumi.Input[bool] help: display this help and exit.
+        :param pulumi.Input[str] in_place: edit files in place (makes backup if SUFFIX supplied)
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] input_files: corresponds to the [input-file]... argument(s).
+        :param pulumi.Input[int] line_length: specify the desired line-wrap length for the `l' command
+        :param pulumi.Input[bool] null_data: separate lines by NUL characters
+        :param pulumi.Input[bool] posix: disable all GNU extensions.
+        :param pulumi.Input[bool] quiet: suppress automatic printing of pattern space. Same as `silent`.
+        :param pulumi.Input[bool] regexp_extended: use extended regular expressions in the script (for portability use POSIX -E).
+        :param pulumi.Input[bool] sandbox: operate in sandbox mode (disable e/r/w commands).
+        :param pulumi.Input[str] script: script only if no other script.
+        :param pulumi.Input[bool] separate: consider files as separate rather than as a single, continuous long stream.
+        :param pulumi.Input[bool] silent: suppress automatic printing of pattern space. Same as `quiet`.
+        :param pulumi.Input[bool] unbuffered: load minimal amounts of data from the input files and flush the output buffers more often.
+        :param pulumi.Input[bool] version: output version information and exit.
+        """
+        if debug is not None:
+            pulumi.set(__self__, "debug", debug)
+        if expressions is not None:
+            pulumi.set(__self__, "expressions", expressions)
+        if files is not None:
+            pulumi.set(__self__, "files", files)
+        if follow_symlinks is not None:
+            pulumi.set(__self__, "follow_symlinks", follow_symlinks)
+        if help is not None:
+            pulumi.set(__self__, "help", help)
+        if in_place is not None:
+            pulumi.set(__self__, "in_place", in_place)
+        if input_files is not None:
+            pulumi.set(__self__, "input_files", input_files)
+        if line_length is not None:
+            pulumi.set(__self__, "line_length", line_length)
+        if null_data is not None:
+            pulumi.set(__self__, "null_data", null_data)
+        if posix is not None:
+            pulumi.set(__self__, "posix", posix)
+        if quiet is not None:
+            pulumi.set(__self__, "quiet", quiet)
+        if regexp_extended is not None:
+            pulumi.set(__self__, "regexp_extended", regexp_extended)
+        if sandbox is not None:
+            pulumi.set(__self__, "sandbox", sandbox)
+        if script is not None:
+            pulumi.set(__self__, "script", script)
+        if separate is not None:
+            pulumi.set(__self__, "separate", separate)
+        if silent is not None:
+            pulumi.set(__self__, "silent", silent)
+        if unbuffered is not None:
+            pulumi.set(__self__, "unbuffered", unbuffered)
+        if version is not None:
+            pulumi.set(__self__, "version", version)
 
     @property
     @pulumi.getter
-    def disable(self) -> pulumi.Output[Optional[bool]]:
+    def debug(self) -> Optional[pulumi.Input[bool]]:
         """
-        If used as the first parameter on the command line, the curlrc config file will not be read and used.
+        annotate program execution.
         """
-        return pulumi.get(self, "disable")
+        return pulumi.get(self, "debug")
+
+    @debug.setter
+    def debug(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "debug", value)
 
     @property
-    @pulumi.getter(name="disableEprt")
-    def disable_eprt(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter
+    def expressions(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        (FTP) Tell curl to disable the use of the EPRT and LPRT commands when doing active FTP transfers
+        add the script to the commands to be executed.
         """
-        return pulumi.get(self, "disable_eprt")
+        return pulumi.get(self, "expressions")
+
+    @expressions.setter
+    def expressions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "expressions", value)
 
     @property
-    @pulumi.getter(name="disableEpsv")
-    def disable_epsv(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter
+    def files(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        (FTP)  Tell  curl to disable the use of the EPSV command when doing passive FTP transfers
+        add the contents of script-file to the commands to be executed.
         """
-        return pulumi.get(self, "disable_epsv")
+        return pulumi.get(self, "files")
+
+    @files.setter
+    def files(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "files", value)
 
     @property
-    @pulumi.getter(name="disallowUsernameInUrl")
-    def disallow_username_in_url(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="followSymlinks")
+    def follow_symlinks(self) -> Optional[pulumi.Input[bool]]:
         """
-        (HTTP) This tells curl to exit if passed a url containing a username.
+        follow symlinks when processing in place
         """
-        return pulumi.get(self, "disallow_username_in_url")
+        return pulumi.get(self, "follow_symlinks")
+
+    @follow_symlinks.setter
+    def follow_symlinks(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "follow_symlinks", value)
 
     @property
-    @pulumi.getter(name="dnsInterface")
-    def dns_interface(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def help(self) -> Optional[pulumi.Input[bool]]:
         """
-        (DNS)  Tell  curl  to send outgoing DNS requests through <interface>.
+        display this help and exit.
         """
-        return pulumi.get(self, "dns_interface")
+        return pulumi.get(self, "help")
+
+    @help.setter
+    def help(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "help", value)
 
     @property
-    @pulumi.getter(name="dnsIpv4Addr")
-    def dns_ipv4_addr(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="inPlace")
+    def in_place(self) -> Optional[pulumi.Input[str]]:
         """
-        (DNS) Tell curl to bind to <ip-address> when making IPv4 DNS requests, so that the DNS requests originate from this address.
+        edit files in place (makes backup if SUFFIX supplied)
         """
-        return pulumi.get(self, "dns_ipv4_addr")
+        return pulumi.get(self, "in_place")
+
+    @in_place.setter
+    def in_place(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "in_place", value)
 
     @property
-    @pulumi.getter(name="dnsIpv6Addr")
-    def dns_ipv6_addr(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="inputFiles")
+    def input_files(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        (DNS) Tell curl to bind to <ip-address> when making IPv6 DNS requests, so that the DNS requests originate from this address.
+        corresponds to the [input-file]... argument(s).
         """
-        return pulumi.get(self, "dns_ipv6_addr")
+        return pulumi.get(self, "input_files")
+
+    @input_files.setter
+    def input_files(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "input_files", value)
 
     @property
-    @pulumi.getter(name="dnsServers")
-    def dns_servers(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="lineLength")
+    def line_length(self) -> Optional[pulumi.Input[int]]:
         """
-        Set the list of DNS servers to be used instead of the system default.
+        specify the desired line-wrap length for the `l' command
         """
-        return pulumi.get(self, "dns_servers")
+        return pulumi.get(self, "line_length")
+
+    @line_length.setter
+    def line_length(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "line_length", value)
 
     @property
-    @pulumi.getter(name="dohCertStatus")
-    def doh_cert_status(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="nullData")
+    def null_data(self) -> Optional[pulumi.Input[bool]]:
         """
-        Same as --cert-status but used for DoH (DNS-over-HTTPS).
+        separate lines by NUL characters
         """
-        return pulumi.get(self, "doh_cert_status")
+        return pulumi.get(self, "null_data")
+
+    @null_data.setter
+    def null_data(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "null_data", value)
 
     @property
-    @pulumi.getter(name="dohInsecure")
-    def doh_insecure(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter
+    def posix(self) -> Optional[pulumi.Input[bool]]:
         """
-        Same as -k, --insecure but used for DoH (DNS-over-HTTPS).
+        disable all GNU extensions.
         """
-        return pulumi.get(self, "doh_insecure")
+        return pulumi.get(self, "posix")
+
+    @posix.setter
+    def posix(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "posix", value)
 
     @property
-    @pulumi.getter(name="dohUrl")
-    def doh_url(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def quiet(self) -> Optional[pulumi.Input[bool]]:
         """
-        Specifies which DNS-over-HTTPS (DoH) server to use to resolve hostnames, instead of using the default name resolver mechanism.
+        suppress automatic printing of pattern space. Same as `silent`.
         """
-        return pulumi.get(self, "doh_url")
+        return pulumi.get(self, "quiet")
+
+    @quiet.setter
+    def quiet(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "quiet", value)
 
     @property
-    @pulumi.getter(name="dumpHeader")
-    def dump_header(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="regexpExtended")
+    def regexp_extended(self) -> Optional[pulumi.Input[bool]]:
         """
-        (HTTP FTP) Write the received protocol headers to the specified file.
+        use extended regular expressions in the script (for portability use POSIX -E).
         """
-        return pulumi.get(self, "dump_header")
+        return pulumi.get(self, "regexp_extended")
+
+    @regexp_extended.setter
+    def regexp_extended(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "regexp_extended", value)
 
     @property
-    @pulumi.getter(name="egdFile")
-    def egd_file(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def sandbox(self) -> Optional[pulumi.Input[bool]]:
         """
-        (TLS) Specify the path name to the Entropy Gathering Daemon socket.
+        operate in sandbox mode (disable e/r/w commands).
         """
-        return pulumi.get(self, "egd_file")
+        return pulumi.get(self, "sandbox")
+
+    @sandbox.setter
+    def sandbox(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "sandbox", value)
 
     @property
     @pulumi.getter
-    def engine(self) -> pulumi.Output[Optional[str]]:
+    def script(self) -> Optional[pulumi.Input[str]]:
         """
-        (TLS) Select the OpenSSL crypto engine to use for cipher operations.
+        script only if no other script.
         """
-        return pulumi.get(self, "engine")
+        return pulumi.get(self, "script")
+
+    @script.setter
+    def script(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "script", value)
 
     @property
     @pulumi.getter
-    def environment(self) -> pulumi.Output[Mapping[str, str]]:
+    def separate(self) -> Optional[pulumi.Input[bool]]:
         """
-        Environment variables
+        consider files as separate rather than as a single, continuous long stream.
         """
-        return pulumi.get(self, "environment")
+        return pulumi.get(self, "separate")
+
+    @separate.setter
+    def separate(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "separate", value)
 
     @property
-    @pulumi.getter(name="etagCompare")
-    def etag_compare(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def silent(self) -> Optional[pulumi.Input[bool]]:
         """
-        (HTTP) This option makes a conditional HTTP request for the specific ETag read from the given file by sending a custom If-None-Match header using the stored ETag.
+        suppress automatic printing of pattern space. Same as `quiet`.
         """
-        return pulumi.get(self, "etag_compare")
+        return pulumi.get(self, "silent")
+
+    @silent.setter
+    def silent(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "silent", value)
 
     @property
-    @pulumi.getter(name="etagSave")
-    def etag_save(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def unbuffered(self) -> Optional[pulumi.Input[bool]]:
         """
-        (HTTP) This option saves an HTTP ETag to the specified file.
+        load minimal amounts of data from the input files and flush the output buffers more often.
         """
-        return pulumi.get(self, "etag_save")
+        return pulumi.get(self, "unbuffered")
+
+    @unbuffered.setter
+    def unbuffered(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "unbuffered", value)
 
     @property
-    @pulumi.getter(name="expect100Timeout")
-    def expect100_timeout(self) -> pulumi.Output[Optional[int]]:
+    @pulumi.getter
+    def version(self) -> Optional[pulumi.Input[bool]]:
         """
-        (HTTP)  Maximum  time in seconds that you allow curl to wait for a 100-continue response when curl emits an Expects: 100-continue header in its request.
+        output version information and exit.
         """
-        return pulumi.get(self, "expect100_timeout")
+        return pulumi.get(self, "version")
+
+    @version.setter
+    def version(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "version", value)
+
+
+@pulumi.input_type
+class SystemctlOptsArgs:
+    def __init__(__self__, *,
+                 command: 'SystemctlCommand',
+                 unit: pulumi.Input[str],
+                 pattern: Optional[pulumi.Input[str]] = None):
+        """
+        Abstraction over the `systemctl` utility on a remote system.
+        :param 'SystemctlCommand' command: Corresponds to the COMMAND argument.
+        :param pulumi.Input[str] unit: Corresponds to the [UNIT...] argument.
+        :param pulumi.Input[str] pattern: Corresponds to the [PATTERN] argument
+        """
+        pulumi.set(__self__, "command", command)
+        pulumi.set(__self__, "unit", unit)
+        if pattern is not None:
+            pulumi.set(__self__, "pattern", pattern)
 
     @property
     @pulumi.getter
-    def fail(self) -> pulumi.Output[Optional[bool]]:
+    def command(self) -> 'SystemctlCommand':
         """
-        (HTTP) Fail silently (no output at all) on server errors.
+        Corresponds to the COMMAND argument.
         """
-        return pulumi.get(self, "fail")
+        return pulumi.get(self, "command")
+
+    @command.setter
+    def command(self, value: 'SystemctlCommand'):
+        pulumi.set(self, "command", value)
 
     @property
-    @pulumi.getter(name="failEarly")
-    def fail_early(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter
+    def unit(self) -> pulumi.Input[str]:
         """
-        Fail and exit on the first detected transfer error.
+        Corresponds to the [UNIT...] argument.
         """
-        return pulumi.get(self, "fail_early")
+        return pulumi.get(self, "unit")
+
+    @unit.setter
+    def unit(self, value: pulumi.Input[str]):
+        pulumi.set(self, "unit", value)
 
     @property
-    @pulumi.getter(name="failWithBody")
-    def fail_with_body(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter
+    def pattern(self) -> Optional[pulumi.Input[str]]:
         """
-        (HTTP)  Return an error on server errors where the HTTP response code is 400 or greater).
+        Corresponds to the [PATTERN] argument
         """
-        return pulumi.get(self, "fail_with_body")
+        return pulumi.get(self, "pattern")
 
-    @property
-    @pulumi.getter(name="falseStart")
-    def false_start(self) -> pulumi.Output[Optional[bool]]:
+    @pattern.setter
+    def pattern(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "pattern", value)
+
+
+@pulumi.input_type
+class TarOptsArgs:
+    def __init__(__self__, *,
+                 archive: pulumi.Input[str],
+                 directory: Optional[pulumi.Input[str]] = None,
+                 extract: Optional[pulumi.Input[bool]] = None,
+                 files: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 gzip: Optional[pulumi.Input[bool]] = None,
+                 on_delete: Optional[pulumi.Input[bool]] = None,
+                 recursive: Optional[pulumi.Input[bool]] = None,
+                 strip_components: Optional[pulumi.Input[int]] = None):
         """
-        (TLS) Tells curl to use false start during the TLS handshake.
+        Abstraction over the `tar` utility on a remote system.
+        :param pulumi.Input[str] archive: Corresponds to the [ARCHIVE] argument.
+        :param pulumi.Input[str] directory: Corresponds to the `--directory` option.
+        :param pulumi.Input[bool] extract: Corresponds to the `--extract` option.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] files: Corresponds to the [FILE] argument.
+        :param pulumi.Input[bool] gzip: Corresponds to the `--gzip` option.
+        :param pulumi.Input[bool] on_delete: Whether rm should be run when the resource is created or deleted.
+        :param pulumi.Input[bool] recursive: Corresponds to the `--recursive` option.
+        :param pulumi.Input[int] strip_components: Corresponds to the `--strip-components` option.
         """
-        return pulumi.get(self, "false_start")
+        pulumi.set(__self__, "archive", archive)
+        if directory is not None:
+            pulumi.set(__self__, "directory", directory)
+        if extract is not None:
+            pulumi.set(__self__, "extract", extract)
+        if files is not None:
+            pulumi.set(__self__, "files", files)
+        if gzip is not None:
+            pulumi.set(__self__, "gzip", gzip)
+        if on_delete is not None:
+            pulumi.set(__self__, "on_delete", on_delete)
+        if recursive is not None:
+            pulumi.set(__self__, "recursive", recursive)
+        if strip_components is not None:
+            pulumi.set(__self__, "strip_components", strip_components)
 
     @property
     @pulumi.getter
-    def form(self) -> pulumi.Output[Optional[str]]:
+    def archive(self) -> pulumi.Input[str]:
         """
-        (HTTP SMTP IMAP) For HTTP protocol family, this lets curl emulate a filled-in form in which a user has pressed the submit button.
+        Corresponds to the [ARCHIVE] argument.
         """
-        return pulumi.get(self, "form")
+        return pulumi.get(self, "archive")
+
+    @archive.setter
+    def archive(self, value: pulumi.Input[str]):
+        pulumi.set(self, "archive", value)
 
     @property
-    @pulumi.getter(name="formEscape")
-    def form_escape(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter
+    def directory(self) -> Optional[pulumi.Input[str]]:
         """
-        (HTTP) Tells curl to pass on names of multipart form fields and files using backslash-escaping instead of percent-encoding.
+        Corresponds to the `--directory` option.
         """
-        return pulumi.get(self, "form_escape")
+        return pulumi.get(self, "directory")
+
+    @directory.setter
+    def directory(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "directory", value)
 
     @property
-    @pulumi.getter(name="formName")
-    def form_name(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def extract(self) -> Optional[pulumi.Input[bool]]:
         """
-        (HTTP SMTP IMAP) Similar to -F, --form except that the value string for the named parameter is used literally.
+        Corresponds to the `--extract` option.
         """
-        return pulumi.get(self, "form_name")
+        return pulumi.get(self, "extract")
+
+    @extract.setter
+    def extract(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "extract", value)
 
     @property
-    @pulumi.getter(name="ftpAccount")
-    def ftp_account(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def files(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        (FTP) When an FTP server asks for 'account data' after user name and password has been provided, this data is sent off using the ACCT command.
+        Corresponds to the [FILE] argument.
         """
-        return pulumi.get(self, "ftp_account")
+        return pulumi.get(self, "files")
+
+    @files.setter
+    def files(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "files", value)
 
     @property
-    @pulumi.getter(name="ftpAlternativeUser")
-    def ftp_alternative_user(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def gzip(self) -> Optional[pulumi.Input[bool]]:
         """
-        (FTP) If authenticating with the USER and PASS commands fails, send this command.
+        Corresponds to the `--gzip` option.
         """
-        return pulumi.get(self, "ftp_alternative_user")
+        return pulumi.get(self, "gzip")
+
+    @gzip.setter
+    def gzip(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "gzip", value)
 
     @property
-    @pulumi.getter(name="ftpCreateDirs")
-    def ftp_create_dirs(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="onDelete")
+    def on_delete(self) -> Optional[pulumi.Input[bool]]:
         """
-        (FTP  SFTP) When an FTP or SFTP URL/operation uses a path that does not currently exist on the server, the standard behavior of curl is to fail.
+        Whether rm should be run when the resource is created or deleted.
         """
-        return pulumi.get(self, "ftp_create_dirs")
+        return pulumi.get(self, "on_delete")
+
+    @on_delete.setter
+    def on_delete(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "on_delete", value)
 
     @property
-    @pulumi.getter(name="ftpMethod")
-    def ftp_method(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def recursive(self) -> Optional[pulumi.Input[bool]]:
         """
-        (FTP) Control what method curl should use to reach a file on an FTP(S) server.
+        Corresponds to the `--recursive` option.
         """
-        return pulumi.get(self, "ftp_method")
+        return pulumi.get(self, "recursive")
+
+    @recursive.setter
+    def recursive(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "recursive", value)
 
     @property
-    @pulumi.getter(name="ftpPasv")
-    def ftp_pasv(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="stripComponents")
+    def strip_components(self) -> Optional[pulumi.Input[int]]:
         """
-        (FTP) Use passive mode for the data connection.
+        Corresponds to the `--strip-components` option.
         """
-        return pulumi.get(self, "ftp_pasv")
+        return pulumi.get(self, "strip_components")
+
+    @strip_components.setter
+    def strip_components(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "strip_components", value)
+
+
+@pulumi.input_type
+class TeeOptsArgs:
+    def __init__(__self__, *,
+                 files: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 append: Optional[pulumi.Input[bool]] = None,
+                 ignore_interrupts: Optional[pulumi.Input[bool]] = None,
+                 output_error: Optional[pulumi.Input['TeeMode']] = None,
+                 pipe: Optional[pulumi.Input[bool]] = None,
+                 version: Optional[pulumi.Input[bool]] = None):
+        """
+        Abstraction over the `rm` utility on a remote system.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] files: Corresponds to the [FILE] argument.
+        :param pulumi.Input[bool] append: Append to the given FILEs, do not overwrite
+        :param pulumi.Input[bool] ignore_interrupts: Ignore interrupt signals.
+        :param pulumi.Input['TeeMode'] output_error: Set behavior on write error.
+        :param pulumi.Input[bool] pipe: Operate in a more appropriate MODE with pipes.
+        :param pulumi.Input[bool] version: Output version information and exit.
+        """
+        pulumi.set(__self__, "files", files)
+        if append is not None:
+            pulumi.set(__self__, "append", append)
+        if ignore_interrupts is not None:
+            pulumi.set(__self__, "ignore_interrupts", ignore_interrupts)
+        if output_error is not None:
+            pulumi.set(__self__, "output_error", output_error)
+        if pipe is not None:
+            pulumi.set(__self__, "pipe", pipe)
+        if version is not None:
+            pulumi.set(__self__, "version", version)
 
     @property
-    @pulumi.getter(name="ftpPort")
-    def ftp_port(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter
+    def files(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        (FTP)  Reverses  the  default  initiator/listener  roles  when connecting with FTP.
+        Corresponds to the [FILE] argument.
         """
-        return pulumi.get(self, "ftp_port")
+        return pulumi.get(self, "files")
+
+    @files.setter
+    def files(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "files", value)
 
     @property
-    @pulumi.getter(name="ftpPret")
-    def ftp_pret(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter
+    def append(self) -> Optional[pulumi.Input[bool]]:
         """
-        (FTP) Tell curl to send a PRET command before PASV (and EPSV).
+        Append to the given FILEs, do not overwrite
         """
-        return pulumi.get(self, "ftp_pret")
+        return pulumi.get(self, "append")
+
+    @append.setter
+    def append(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "append", value)
 
     @property
-    @pulumi.getter(name="ftpSkipPasvIp")
-    def ftp_skip_pasv_ip(self) -> pulumi.Output[Optional[bool]]:
+    @pulumi.getter(name="ignoreInterrupts")
+    def ignore_interrupts(self) -> Optional[pulumi.Input[bool]]:
         """
-        (FTP)  Tell  curl  to  not use the IP address the server suggests in its response to curl's PASV command when curl connects the data connection.
+        Ignore interrupt signals.
         """
-        return pulumi.get(self, "ftp_skip_pasv_ip")
+        return pulumi.get(self, "ignore_interrupts")
+
+    @ignore_interrupts.setter
+    def ignore_interrupts(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "ignore_interrupts", value)
 
     @property
-    @pulumi.getter(name="ftpSslCccMode")
-    def ftp_ssl_ccc_mode(self) -> pulumi.Output[Optional[str]]:
+    @pulumi.getter(name="outputError")
+    def output_error(self) -> Optional[pulumi.Input['TeeMode']]:
         """
-        (FTP) Sets the CCC mode. The passive mode will not initiate the shutdown, but instead wait for the server to do it, and will not reply to the shutdown from the  server.
+        Set behavior on write error.
         """
-        return pulumi.get(self, "ftp_ssl_ccc_mode")
+        return pulumi.get(self, "output_error")
+
+    @output_error.setter
+    def output_error(self, value: Optional[pulumi.Input['TeeMode']]):
+        pulumi.set(self, "output_error", value)
 
     @property
     @pulumi.getter
-    def lifecycle(self) -> pulumi.Output[Optional['CommandLifecycle']]:
+    def pipe(self) -> Optional[pulumi.Input[bool]]:
         """
-        At what stage(s) in the resource lifecycle should the command be run
+        Operate in a more appropriate MODE with pipes.
         """
-        return pulumi.get(self, "lifecycle")
+        return pulumi.get(self, "pipe")
+
+    @pipe.setter
+    def pipe(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "pipe", value)
 
     @property
     @pulumi.getter
-    def stderr(self) -> pulumi.Output[str]:
+    def version(self) -> Optional[pulumi.Input[bool]]:
         """
-        TODO
+        Output version information and exit.
         """
-        return pulumi.get(self, "stderr")
+        return pulumi.get(self, "version")
+
+    @version.setter
+    def version(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "version", value)
+
+
+@pulumi.input_type
+class WgetOptsArgs:
+    def __init__(__self__, *,
+                 url: pulumi.Input[Sequence[pulumi.Input[str]]],
+                 directory_prefix: Optional[pulumi.Input[str]] = None,
+                 https_only: Optional[pulumi.Input[bool]] = None,
+                 no_verbose: Optional[pulumi.Input[bool]] = None,
+                 output_document: Optional[pulumi.Input[str]] = None,
+                 quiet: Optional[pulumi.Input[bool]] = None,
+                 timestamping: Optional[pulumi.Input[bool]] = None):
+        """
+        Abstraction over the `wget` utility on a remote system.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] url: Corresponds to the [URL...] argument.
+        :param pulumi.Input[str] directory_prefix: The  directory prefix is the directory where all other files and subdirectories will be saved to, i.e. the top of the retrieval tree.  The default is . (the current directory).
+        :param pulumi.Input[bool] https_only: When in recursive mode, only HTTPS links are followed.
+        :param pulumi.Input[bool] no_verbose: Turn off verbose without being completely quiet (use -q for that), which means that error messages and basic information still get printed.
+        :param pulumi.Input[str] output_document: The  documents  will  not  be  written  to the appropriate files, but all will be concatenated together and written to file.
+        :param pulumi.Input[bool] quiet: Turn off Wget's output.
+        :param pulumi.Input[bool] timestamping: Turn on time-stamping.
+        """
+        pulumi.set(__self__, "url", url)
+        if directory_prefix is not None:
+            pulumi.set(__self__, "directory_prefix", directory_prefix)
+        if https_only is not None:
+            pulumi.set(__self__, "https_only", https_only)
+        if no_verbose is not None:
+            pulumi.set(__self__, "no_verbose", no_verbose)
+        if output_document is not None:
+            pulumi.set(__self__, "output_document", output_document)
+        if quiet is not None:
+            pulumi.set(__self__, "quiet", quiet)
+        if timestamping is not None:
+            pulumi.set(__self__, "timestamping", timestamping)
 
     @property
     @pulumi.getter
-    def stdin(self) -> pulumi.Output[Optional[str]]:
+    def url(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        TODO
+        Corresponds to the [URL...] argument.
         """
-        return pulumi.get(self, "stdin")
+        return pulumi.get(self, "url")
+
+    @url.setter
+    def url(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
+        pulumi.set(self, "url", value)
 
     @property
-    @pulumi.getter
-    def stdout(self) -> pulumi.Output[str]:
+    @pulumi.getter(name="directoryPrefix")
+    def directory_prefix(self) -> Optional[pulumi.Input[str]]:
         """
-        TODO
+        The  directory prefix is the directory where all other files and subdirectories will be saved to, i.e. the top of the retrieval tree.  The default is . (the current directory).
         """
-        return pulumi.get(self, "stdout")
+        return pulumi.get(self, "directory_prefix")
+
+    @directory_prefix.setter
+    def directory_prefix(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "directory_prefix", value)
+
+    @property
+    @pulumi.getter(name="httpsOnly")
+    def https_only(self) -> Optional[pulumi.Input[bool]]:
+        """
+        When in recursive mode, only HTTPS links are followed.
+        """
+        return pulumi.get(self, "https_only")
+
+    @https_only.setter
+    def https_only(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "https_only", value)
+
+    @property
+    @pulumi.getter(name="noVerbose")
+    def no_verbose(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Turn off verbose without being completely quiet (use -q for that), which means that error messages and basic information still get printed.
+        """
+        return pulumi.get(self, "no_verbose")
+
+    @no_verbose.setter
+    def no_verbose(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "no_verbose", value)
+
+    @property
+    @pulumi.getter(name="outputDocument")
+    def output_document(self) -> Optional[pulumi.Input[str]]:
+        """
+        The  documents  will  not  be  written  to the appropriate files, but all will be concatenated together and written to file.
+        """
+        return pulumi.get(self, "output_document")
+
+    @output_document.setter
+    def output_document(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "output_document", value)
 
     @property
     @pulumi.getter
-    def triggers(self) -> pulumi.Output[Sequence[Any]]:
+    def quiet(self) -> Optional[pulumi.Input[bool]]:
         """
-        TODO
+        Turn off Wget's output.
         """
-        return pulumi.get(self, "triggers")
+        return pulumi.get(self, "quiet")
+
+    @quiet.setter
+    def quiet(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "quiet", value)
 
     @property
     @pulumi.getter
-    def urls(self) -> pulumi.Output[Any]:
+    def timestamping(self) -> Optional[pulumi.Input[bool]]:
         """
-        Corresponds to the URLs argument.
+        Turn on time-stamping.
         """
-        return pulumi.get(self, "urls")
+        return pulumi.get(self, "timestamping")
+
+    @timestamping.setter
+    def timestamping(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "timestamping", value)
+
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,143 +4,124 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from ._enums import *
+from . import outputs
+from ._inputs import *
 import pulumi_command
 
-__all__ = ['MkdirArgs', 'Mkdir']
+__all__ = ['TarArgs', 'Tar']
 
 @pulumi.input_type
-class MkdirArgs:
+class TarArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 directory: pulumi.Input[str],
                  binary_path: Optional[pulumi.Input[str]] = None,
+                 create: Optional['TarOptsArgs'] = None,
+                 delete: Optional['TarOptsArgs'] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 parents: Optional[pulumi.Input[bool]] = None,
-                 remove_on_delete: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
-                 triggers: Optional[pulumi.Input[Sequence[Any]]] = None):
+                 triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
+                 update: Optional['TarOptsArgs'] = None):
         """
-        The set of arguments for constructing a Mkdir resource.
+        The set of arguments for constructing a Tar resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
-        :param pulumi.Input[str] directory: The fully qualified path of the directory on the remote system.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
+        :param 'TarOptsArgs' create: The command to run on create.
+        :param 'TarOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+               and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+               Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
-        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
-        :param pulumi.Input[bool] parents: Corresponds to the `--parents` option.
-        :param pulumi.Input[bool] remove_on_delete: Remove the created directory when the `Mkdir` resource is deleted or updated.
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param 'TarOptsArgs' update: The command to run on update, if empty, create will 
+               run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+               are set to the stdout and stderr properties of the Command resource from previous 
+               create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
-        pulumi.set(__self__, "directory", directory)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
+        if create is not None:
+            pulumi.set(__self__, "create", create)
+        if delete is not None:
+            pulumi.set(__self__, "delete", delete)
         if environment is not None:
             pulumi.set(__self__, "environment", environment)
-        if lifecycle is not None:
-            pulumi.set(__self__, "lifecycle", lifecycle)
-        if parents is not None:
-            pulumi.set(__self__, "parents", parents)
-        if remove_on_delete is not None:
-            pulumi.set(__self__, "remove_on_delete", remove_on_delete)
         if stdin is not None:
             pulumi.set(__self__, "stdin", stdin)
         if triggers is not None:
             pulumi.set(__self__, "triggers", triggers)
+        if update is not None:
+            pulumi.set(__self__, "update", update)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
-    @pulumi.getter
-    def directory(self) -> pulumi.Input[str]:
-        """
-        The fully qualified path of the directory on the remote system.
-        """
-        return pulumi.get(self, "directory")
-
-    @directory.setter
-    def directory(self, value: pulumi.Input[str]):
-        pulumi.set(self, "directory", value)
-
-    @property
     @pulumi.getter(name="binaryPath")
     def binary_path(self) -> Optional[pulumi.Input[str]]:
         """
         Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         """
         return pulumi.get(self, "binary_path")
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+    def create(self) -> Optional['TarOptsArgs']:
         """
-        Environment variables
+        The command to run on create.
         """
-        return pulumi.get(self, "environment")
+        return pulumi.get(self, "create")
 
-    @environment.setter
-    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
-        pulumi.set(self, "environment", value)
+    @create.setter
+    def create(self, value: Optional['TarOptsArgs']):
+        pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def lifecycle(self) -> Optional['CommandLifecycle']:
+    def delete(self) -> Optional['TarOptsArgs']:
         """
-        At what stage(s) in the resource lifecycle should the command be run
+        The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+        Command resource from previous create or update steps.
         """
-        return pulumi.get(self, "lifecycle")
+        return pulumi.get(self, "delete")
 
-    @lifecycle.setter
-    def lifecycle(self, value: Optional['CommandLifecycle']):
-        pulumi.set(self, "lifecycle", value)
+    @delete.setter
+    def delete(self, value: Optional['TarOptsArgs']):
+        pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
-    def parents(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Corresponds to the `--parents` option.
-        """
-        return pulumi.get(self, "parents")
-
-    @parents.setter
-    def parents(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "parents", value)
-
-    @property
-    @pulumi.getter(name="removeOnDelete")
-    def remove_on_delete(self) -> Optional[pulumi.Input[bool]]:
+    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Remove the created directory when the `Mkdir` resource is deleted or updated.
+        Environment variables
         """
-        return pulumi.get(self, "remove_on_delete")
+        return pulumi.get(self, "environment")
 
-    @remove_on_delete.setter
-    def remove_on_delete(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "remove_on_delete", value)
+    @environment.setter
+    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "environment", value)
 
     @property
     @pulumi.getter
     def stdin(self) -> Optional[pulumi.Input[str]]:
         """
         TODO
         """
@@ -158,107 +139,121 @@
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
+    @property
+    @pulumi.getter
+    def update(self) -> Optional['TarOptsArgs']:
+        """
+        The command to run on update, if empty, create will 
+        run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+        are set to the stdout and stderr properties of the Command resource from previous 
+        create or update steps.
+        """
+        return pulumi.get(self, "update")
+
+    @update.setter
+    def update(self, value: Optional['TarOptsArgs']):
+        pulumi.set(self, "update", value)
 
-class Mkdir(pulumi.ComponentResource):
+
+class Tar(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 directory: Optional[pulumi.Input[str]] = None,
+                 create: Optional[pulumi.InputType['TarOptsArgs']] = None,
+                 delete: Optional[pulumi.InputType['TarOptsArgs']] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 parents: Optional[pulumi.Input[bool]] = None,
-                 remove_on_delete: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
+                 update: Optional[pulumi.InputType['TarOptsArgs']] = None,
                  __props__=None):
         """
-        Abstraction over the `mkdir` utility on a remote system.
+        Abstraction over the `tar` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.Input[str] directory: The fully qualified path of the directory on the remote system.
+        :param pulumi.InputType['TarOptsArgs'] create: The command to run on create.
+        :param pulumi.InputType['TarOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+               and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+               Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
-        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
-        :param pulumi.Input[bool] parents: Corresponds to the `--parents` option.
-        :param pulumi.Input[bool] remove_on_delete: Remove the created directory when the `Mkdir` resource is deleted or updated.
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param pulumi.InputType['TarOptsArgs'] update: The command to run on update, if empty, create will 
+               run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+               are set to the stdout and stderr properties of the Command resource from previous 
+               create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: MkdirArgs,
+                 args: TarArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `mkdir` utility on a remote system.
+        Abstraction over the `tar` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param MkdirArgs args: The arguments to use to populate this resource's properties.
+        :param TarArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(MkdirArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(TarArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 directory: Optional[pulumi.Input[str]] = None,
+                 create: Optional[pulumi.InputType['TarOptsArgs']] = None,
+                 delete: Optional[pulumi.InputType['TarOptsArgs']] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 parents: Optional[pulumi.Input[bool]] = None,
-                 remove_on_delete: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
+                 update: Optional[pulumi.InputType['TarOptsArgs']] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = MkdirArgs.__new__(MkdirArgs)
+            __props__ = TarArgs.__new__(TarArgs)
 
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            if directory is None and not opts.urn:
-                raise TypeError("Missing required property 'directory'")
-            __props__.__dict__["directory"] = directory
+            __props__.__dict__["create"] = create
+            __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
-            __props__.__dict__["lifecycle"] = lifecycle
-            __props__.__dict__["parents"] = parents
-            __props__.__dict__["remove_on_delete"] = remove_on_delete
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
+            __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Mkdir, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Mkdir',
+        super(Tar, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Tar',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -282,51 +277,37 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def directory(self) -> pulumi.Output[str]:
+    def create(self) -> pulumi.Output[Optional['outputs.TarOpts']]:
         """
-        The fully qualified path of the directory on the remote system.
+        The command to run on create.
         """
-        return pulumi.get(self, "directory")
-
-    @property
-    @pulumi.getter
-    def environment(self) -> pulumi.Output[Mapping[str, str]]:
-        """
-        Environment variables
-        """
-        return pulumi.get(self, "environment")
+        return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def lifecycle(self) -> pulumi.Output[Optional['CommandLifecycle']]:
+    def delete(self) -> pulumi.Output[Optional['outputs.TarOpts']]:
         """
-        At what stage(s) in the resource lifecycle should the command be run
+        The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+        Command resource from previous create or update steps.
         """
-        return pulumi.get(self, "lifecycle")
+        return pulumi.get(self, "delete")
 
     @property
     @pulumi.getter
-    def parents(self) -> pulumi.Output[bool]:
-        """
-        Corresponds to the `--parents` option.
-        """
-        return pulumi.get(self, "parents")
-
-    @property
-    @pulumi.getter(name="removeOnDelete")
-    def remove_on_delete(self) -> pulumi.Output[bool]:
+    def environment(self) -> pulumi.Output[Mapping[str, str]]:
         """
-        Remove the created directory when the `Mkdir` resource is deleted or updated.
+        Environment variables
         """
-        return pulumi.get(self, "remove_on_delete")
+        return pulumi.get(self, "environment")
 
     @property
     @pulumi.getter
     def stderr(self) -> pulumi.Output[str]:
         """
         TODO
         """
@@ -352,7 +333,18 @@
     @pulumi.getter
     def triggers(self) -> pulumi.Output[Sequence[Any]]:
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
+    @property
+    @pulumi.getter
+    def update(self) -> pulumi.Output[Optional['outputs.TarOpts']]:
+        """
+        The command to run on update, if empty, create will 
+        run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+        are set to the stdout and stderr properties of the Command resource from previous 
+        create or update steps.
+        """
+        return pulumi.get(self, "update")
+
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,72 +4,62 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from ._enums import *
+from . import outputs
+from ._inputs import *
 import pulumi_command
 
-__all__ = ['MktempArgs', 'Mktemp']
+__all__ = ['MkdirArgs', 'Mkdir']
 
 @pulumi.input_type
-class MktempArgs:
+class MkdirArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 directory: Optional[pulumi.Input[bool]] = None,
-                 dry_run: Optional[pulumi.Input[bool]] = None,
+                 create: Optional['MkdirOptsArgs'] = None,
+                 delete: Optional['MkdirOptsArgs'] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 quiet: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
-                 suffix: Optional[pulumi.Input[str]] = None,
-                 template: Optional[pulumi.Input[str]] = None,
-                 tmpdir: Optional[pulumi.Input[str]] = None,
-                 triggers: Optional[pulumi.Input[Sequence[Any]]] = None):
+                 triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
+                 update: Optional['MkdirOptsArgs'] = None):
         """
-        The set of arguments for constructing a Mktemp resource.
+        The set of arguments for constructing a Mkdir resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param pulumi.Input[bool] directory: Corresponds to the `--directory` option.
-        :param pulumi.Input[bool] dry_run: Corresponds to the `--dry-run` option.
+        :param 'MkdirOptsArgs' create: The command to run on create.
+        :param 'MkdirOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+               and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+               Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
-        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
-        :param pulumi.Input[bool] quiet: Corresponds to the `--quiet` option.
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[str] suffix: Corresponds to the `--suffix` option.
-        :param pulumi.Input[str] template: Corresponds to the [TEMPLATE] argument.
-        :param pulumi.Input[str] tmpdir: Corresponds to the `--tmpdir` option.
         :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param 'MkdirOptsArgs' update: The command to run on update, if empty, create will 
+               run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+               are set to the stdout and stderr properties of the Command resource from previous 
+               create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
-        if directory is not None:
-            pulumi.set(__self__, "directory", directory)
-        if dry_run is not None:
-            pulumi.set(__self__, "dry_run", dry_run)
+        if create is not None:
+            pulumi.set(__self__, "create", create)
+        if delete is not None:
+            pulumi.set(__self__, "delete", delete)
         if environment is not None:
             pulumi.set(__self__, "environment", environment)
-        if lifecycle is not None:
-            pulumi.set(__self__, "lifecycle", lifecycle)
-        if quiet is not None:
-            pulumi.set(__self__, "quiet", quiet)
         if stdin is not None:
             pulumi.set(__self__, "stdin", stdin)
-        if suffix is not None:
-            pulumi.set(__self__, "suffix", suffix)
-        if template is not None:
-            pulumi.set(__self__, "template", template)
-        if tmpdir is not None:
-            pulumi.set(__self__, "tmpdir", tmpdir)
         if triggers is not None:
             pulumi.set(__self__, "triggers", triggers)
+        if update is not None:
+            pulumi.set(__self__, "update", update)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
         Connection details for the remote system
         """
@@ -89,35 +79,37 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def directory(self) -> Optional[pulumi.Input[bool]]:
+    def create(self) -> Optional['MkdirOptsArgs']:
         """
-        Corresponds to the `--directory` option.
+        The command to run on create.
         """
-        return pulumi.get(self, "directory")
+        return pulumi.get(self, "create")
 
-    @directory.setter
-    def directory(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "directory", value)
+    @create.setter
+    def create(self, value: Optional['MkdirOptsArgs']):
+        pulumi.set(self, "create", value)
 
     @property
-    @pulumi.getter(name="dryRun")
-    def dry_run(self) -> Optional[pulumi.Input[bool]]:
+    @pulumi.getter
+    def delete(self) -> Optional['MkdirOptsArgs']:
         """
-        Corresponds to the `--dry-run` option.
+        The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+        Command resource from previous create or update steps.
         """
-        return pulumi.get(self, "dry_run")
+        return pulumi.get(self, "delete")
 
-    @dry_run.setter
-    def dry_run(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "dry_run", value)
+    @delete.setter
+    def delete(self, value: Optional['MkdirOptsArgs']):
+        pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
     def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
         Environment variables
         """
@@ -125,199 +117,143 @@
 
     @environment.setter
     def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "environment", value)
 
     @property
     @pulumi.getter
-    def lifecycle(self) -> Optional['CommandLifecycle']:
-        """
-        At what stage(s) in the resource lifecycle should the command be run
-        """
-        return pulumi.get(self, "lifecycle")
-
-    @lifecycle.setter
-    def lifecycle(self, value: Optional['CommandLifecycle']):
-        pulumi.set(self, "lifecycle", value)
-
-    @property
-    @pulumi.getter
-    def quiet(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Corresponds to the `--quiet` option.
-        """
-        return pulumi.get(self, "quiet")
-
-    @quiet.setter
-    def quiet(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "quiet", value)
-
-    @property
-    @pulumi.getter
     def stdin(self) -> Optional[pulumi.Input[str]]:
         """
         TODO
         """
         return pulumi.get(self, "stdin")
 
     @stdin.setter
     def stdin(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "stdin", value)
 
     @property
     @pulumi.getter
-    def suffix(self) -> Optional[pulumi.Input[str]]:
-        """
-        Corresponds to the `--suffix` option.
-        """
-        return pulumi.get(self, "suffix")
-
-    @suffix.setter
-    def suffix(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "suffix", value)
-
-    @property
-    @pulumi.getter
-    def template(self) -> Optional[pulumi.Input[str]]:
-        """
-        Corresponds to the [TEMPLATE] argument.
-        """
-        return pulumi.get(self, "template")
-
-    @template.setter
-    def template(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "template", value)
-
-    @property
-    @pulumi.getter
-    def tmpdir(self) -> Optional[pulumi.Input[str]]:
-        """
-        Corresponds to the `--tmpdir` option.
-        """
-        return pulumi.get(self, "tmpdir")
-
-    @tmpdir.setter
-    def tmpdir(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "tmpdir", value)
-
-    @property
-    @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Sequence[Any]]]:
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
+    @property
+    @pulumi.getter
+    def update(self) -> Optional['MkdirOptsArgs']:
+        """
+        The command to run on update, if empty, create will 
+        run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+        are set to the stdout and stderr properties of the Command resource from previous 
+        create or update steps.
+        """
+        return pulumi.get(self, "update")
+
+    @update.setter
+    def update(self, value: Optional['MkdirOptsArgs']):
+        pulumi.set(self, "update", value)
 
-class Mktemp(pulumi.ComponentResource):
+
+class Mkdir(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 directory: Optional[pulumi.Input[bool]] = None,
-                 dry_run: Optional[pulumi.Input[bool]] = None,
+                 create: Optional[pulumi.InputType['MkdirOptsArgs']] = None,
+                 delete: Optional[pulumi.InputType['MkdirOptsArgs']] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 quiet: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
-                 suffix: Optional[pulumi.Input[str]] = None,
-                 template: Optional[pulumi.Input[str]] = None,
-                 tmpdir: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
+                 update: Optional[pulumi.InputType['MkdirOptsArgs']] = None,
                  __props__=None):
         """
         Abstraction over the `mkdir` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.Input[bool] directory: Corresponds to the `--directory` option.
-        :param pulumi.Input[bool] dry_run: Corresponds to the `--dry-run` option.
+        :param pulumi.InputType['MkdirOptsArgs'] create: The command to run on create.
+        :param pulumi.InputType['MkdirOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+               and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+               Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
-        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
-        :param pulumi.Input[bool] quiet: Corresponds to the `--quiet` option.
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[str] suffix: Corresponds to the `--suffix` option.
-        :param pulumi.Input[str] template: Corresponds to the [TEMPLATE] argument.
-        :param pulumi.Input[str] tmpdir: Corresponds to the `--tmpdir` option.
         :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param pulumi.InputType['MkdirOptsArgs'] update: The command to run on update, if empty, create will 
+               run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+               are set to the stdout and stderr properties of the Command resource from previous 
+               create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: MktempArgs,
+                 args: MkdirArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Abstraction over the `mkdir` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param MktempArgs args: The arguments to use to populate this resource's properties.
+        :param MkdirArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(MktempArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(MkdirArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 directory: Optional[pulumi.Input[bool]] = None,
-                 dry_run: Optional[pulumi.Input[bool]] = None,
+                 create: Optional[pulumi.InputType['MkdirOptsArgs']] = None,
+                 delete: Optional[pulumi.InputType['MkdirOptsArgs']] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 quiet: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
-                 suffix: Optional[pulumi.Input[str]] = None,
-                 template: Optional[pulumi.Input[str]] = None,
-                 tmpdir: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
+                 update: Optional[pulumi.InputType['MkdirOptsArgs']] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = MktempArgs.__new__(MktempArgs)
+            __props__ = MkdirArgs.__new__(MkdirArgs)
 
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            __props__.__dict__["directory"] = directory
-            __props__.__dict__["dry_run"] = dry_run
+            __props__.__dict__["create"] = create
+            __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
-            __props__.__dict__["lifecycle"] = lifecycle
-            __props__.__dict__["quiet"] = quiet
             __props__.__dict__["stdin"] = stdin
-            __props__.__dict__["suffix"] = suffix
-            __props__.__dict__["template"] = template
-            __props__.__dict__["tmpdir"] = tmpdir
             __props__.__dict__["triggers"] = triggers
+            __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Mktemp, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Mktemp',
+        super(Mkdir, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Mkdir',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -341,54 +277,40 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def directory(self) -> pulumi.Output[Optional[bool]]:
+    def create(self) -> pulumi.Output[Optional['outputs.MkdirOpts']]:
         """
-        Corresponds to the `--directory` option.
+        The command to run on create.
         """
-        return pulumi.get(self, "directory")
+        return pulumi.get(self, "create")
 
     @property
-    @pulumi.getter(name="dryRun")
-    def dry_run(self) -> pulumi.Output[bool]:
+    @pulumi.getter
+    def delete(self) -> pulumi.Output[Optional['outputs.MkdirOpts']]:
         """
-        Corresponds to the `--dry-run` option.
+        The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+        Command resource from previous create or update steps.
         """
-        return pulumi.get(self, "dry_run")
+        return pulumi.get(self, "delete")
 
     @property
     @pulumi.getter
     def environment(self) -> pulumi.Output[Mapping[str, str]]:
         """
         Environment variables
         """
         return pulumi.get(self, "environment")
 
     @property
     @pulumi.getter
-    def lifecycle(self) -> pulumi.Output[Optional['CommandLifecycle']]:
-        """
-        At what stage(s) in the resource lifecycle should the command be run
-        """
-        return pulumi.get(self, "lifecycle")
-
-    @property
-    @pulumi.getter
-    def quiet(self) -> pulumi.Output[bool]:
-        """
-        Corresponds to the `--quiet` option.
-        """
-        return pulumi.get(self, "quiet")
-
-    @property
-    @pulumi.getter
     def stderr(self) -> pulumi.Output[str]:
         """
         TODO
         """
         return pulumi.get(self, "stderr")
 
     @property
@@ -405,37 +327,24 @@
         """
         TODO
         """
         return pulumi.get(self, "stdout")
 
     @property
     @pulumi.getter
-    def suffix(self) -> pulumi.Output[Optional[str]]:
-        """
-        Corresponds to the `--suffix` option.
-        """
-        return pulumi.get(self, "suffix")
-
-    @property
-    @pulumi.getter
-    def template(self) -> pulumi.Output[Optional[str]]:
-        """
-        Corresponds to the [TEMPLATE] argument.
-        """
-        return pulumi.get(self, "template")
-
-    @property
-    @pulumi.getter
-    def tmpdir(self) -> pulumi.Output[Optional[str]]:
+    def triggers(self) -> pulumi.Output[Sequence[Any]]:
         """
-        Corresponds to the `--tmpdir` option.
+        TODO
         """
-        return pulumi.get(self, "tmpdir")
+        return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def triggers(self) -> pulumi.Output[Sequence[Any]]:
+    def update(self) -> pulumi.Output[Optional['outputs.MkdirOpts']]:
         """
-        TODO
+        The command to run on update, if empty, create will 
+        run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+        are set to the stdout and stderr properties of the Command resource from previous 
+        create or update steps.
         """
-        return pulumi.get(self, "triggers")
+        return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/curl.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,179 +4,125 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from . import outputs
 from ._enums import *
+from ._inputs import *
 import pulumi_command
 
-__all__ = ['RmArgs', 'Rm']
+__all__ = ['CurlArgs', 'Curl']
 
 @pulumi.input_type
-class RmArgs:
+class CurlArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 files: pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 dir: Optional[pulumi.Input[bool]] = None,
+                 create: Optional['CurlOptsArgs'] = None,
+                 delete: Optional['CurlOptsArgs'] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 force: Optional[pulumi.Input[bool]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 on_delete: Optional[pulumi.Input[bool]] = None,
-                 recursive: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 verbose: Optional[pulumi.Input[bool]] = None):
+                 update: Optional['CurlOptsArgs'] = None):
         """
-        The set of arguments for constructing a Rm resource.
+        The set of arguments for constructing a Curl resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
-        :param pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]] files: Corresponds to the [FILE] argument.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param pulumi.Input[bool] dir: Corresponds to the `--dir` option.
+        :param 'CurlOptsArgs' create: The command to run on create.
+        :param 'CurlOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+               and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+               Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
-        :param pulumi.Input[bool] force: Corresponds to the `--force` option.
-        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
-        :param pulumi.Input[bool] on_delete: Whether rm should be run when the resource is created or deleted.
-        :param pulumi.Input[bool] recursive: Corresponds to the `--recursive` option.
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.Input[bool] verbose: Corresponds to the `--verbose` option.
+        :param 'CurlOptsArgs' update: The command to run on update, if empty, create will 
+               run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+               are set to the stdout and stderr properties of the Command resource from previous 
+               create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
-        pulumi.set(__self__, "files", files)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
-        if dir is not None:
-            pulumi.set(__self__, "dir", dir)
+        if create is not None:
+            pulumi.set(__self__, "create", create)
+        if delete is not None:
+            pulumi.set(__self__, "delete", delete)
         if environment is not None:
             pulumi.set(__self__, "environment", environment)
-        if force is not None:
-            pulumi.set(__self__, "force", force)
-        if lifecycle is not None:
-            pulumi.set(__self__, "lifecycle", lifecycle)
-        if on_delete is not None:
-            pulumi.set(__self__, "on_delete", on_delete)
-        if recursive is not None:
-            pulumi.set(__self__, "recursive", recursive)
         if stdin is not None:
             pulumi.set(__self__, "stdin", stdin)
         if triggers is not None:
             pulumi.set(__self__, "triggers", triggers)
-        if verbose is not None:
-            pulumi.set(__self__, "verbose", verbose)
+        if update is not None:
+            pulumi.set(__self__, "update", update)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
-    @pulumi.getter
-    def files(self) -> pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]:
-        """
-        Corresponds to the [FILE] argument.
-        """
-        return pulumi.get(self, "files")
-
-    @files.setter
-    def files(self, value: pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "files", value)
-
-    @property
     @pulumi.getter(name="binaryPath")
     def binary_path(self) -> Optional[pulumi.Input[str]]:
         """
         Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         """
         return pulumi.get(self, "binary_path")
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def dir(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Corresponds to the `--dir` option.
-        """
-        return pulumi.get(self, "dir")
-
-    @dir.setter
-    def dir(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "dir", value)
-
-    @property
-    @pulumi.getter
-    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
-        """
-        Environment variables
-        """
-        return pulumi.get(self, "environment")
-
-    @environment.setter
-    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
-        pulumi.set(self, "environment", value)
-
-    @property
-    @pulumi.getter
-    def force(self) -> Optional[pulumi.Input[bool]]:
+    def create(self) -> Optional['CurlOptsArgs']:
         """
-        Corresponds to the `--force` option.
+        The command to run on create.
         """
-        return pulumi.get(self, "force")
+        return pulumi.get(self, "create")
 
-    @force.setter
-    def force(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "force", value)
+    @create.setter
+    def create(self, value: Optional['CurlOptsArgs']):
+        pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def lifecycle(self) -> Optional['CommandLifecycle']:
+    def delete(self) -> Optional['CurlOptsArgs']:
         """
-        At what stage(s) in the resource lifecycle should the command be run
+        The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+        Command resource from previous create or update steps.
         """
-        return pulumi.get(self, "lifecycle")
+        return pulumi.get(self, "delete")
 
-    @lifecycle.setter
-    def lifecycle(self, value: Optional['CommandLifecycle']):
-        pulumi.set(self, "lifecycle", value)
-
-    @property
-    @pulumi.getter(name="onDelete")
-    def on_delete(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Whether rm should be run when the resource is created or deleted.
-        """
-        return pulumi.get(self, "on_delete")
-
-    @on_delete.setter
-    def on_delete(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "on_delete", value)
+    @delete.setter
+    def delete(self, value: Optional['CurlOptsArgs']):
+        pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
-    def recursive(self) -> Optional[pulumi.Input[bool]]:
+    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Corresponds to the `--recursive` option.
+        Environment variables
         """
-        return pulumi.get(self, "recursive")
+        return pulumi.get(self, "environment")
 
-    @recursive.setter
-    def recursive(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "recursive", value)
+    @environment.setter
+    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "environment", value)
 
     @property
     @pulumi.getter
     def stdin(self) -> Optional[pulumi.Input[str]]:
         """
         TODO
         """
@@ -196,129 +142,119 @@
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def verbose(self) -> Optional[pulumi.Input[bool]]:
+    def update(self) -> Optional['CurlOptsArgs']:
         """
-        Corresponds to the `--verbose` option.
+        The command to run on update, if empty, create will 
+        run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+        are set to the stdout and stderr properties of the Command resource from previous 
+        create or update steps.
         """
-        return pulumi.get(self, "verbose")
+        return pulumi.get(self, "update")
 
-    @verbose.setter
-    def verbose(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "verbose", value)
+    @update.setter
+    def update(self, value: Optional['CurlOptsArgs']):
+        pulumi.set(self, "update", value)
 
 
-class Rm(pulumi.ComponentResource):
+class Curl(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 dir: Optional[pulumi.Input[bool]] = None,
+                 create: Optional[pulumi.InputType['CurlOptsArgs']] = None,
+                 delete: Optional[pulumi.InputType['CurlOptsArgs']] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 files: Optional[pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]] = None,
-                 force: Optional[pulumi.Input[bool]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 on_delete: Optional[pulumi.Input[bool]] = None,
-                 recursive: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 verbose: Optional[pulumi.Input[bool]] = None,
+                 update: Optional[pulumi.InputType['CurlOptsArgs']] = None,
                  __props__=None):
         """
-        Abstraction over the `rm` utility on a remote system.
+        Abstraction over the `curl` utility on a remote system. Transfer a URL.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.Input[bool] dir: Corresponds to the `--dir` option.
+        :param pulumi.InputType['CurlOptsArgs'] create: The command to run on create.
+        :param pulumi.InputType['CurlOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+               and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+               Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
-        :param pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]] files: Corresponds to the [FILE] argument.
-        :param pulumi.Input[bool] force: Corresponds to the `--force` option.
-        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
-        :param pulumi.Input[bool] on_delete: Whether rm should be run when the resource is created or deleted.
-        :param pulumi.Input[bool] recursive: Corresponds to the `--recursive` option.
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.Input[bool] verbose: Corresponds to the `--verbose` option.
+        :param pulumi.InputType['CurlOptsArgs'] update: The command to run on update, if empty, create will 
+               run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+               are set to the stdout and stderr properties of the Command resource from previous 
+               create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: RmArgs,
+                 args: CurlArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `rm` utility on a remote system.
+        Abstraction over the `curl` utility on a remote system. Transfer a URL.
 
         :param str resource_name: The name of the resource.
-        :param RmArgs args: The arguments to use to populate this resource's properties.
+        :param CurlArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(RmArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(CurlArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 dir: Optional[pulumi.Input[bool]] = None,
+                 create: Optional[pulumi.InputType['CurlOptsArgs']] = None,
+                 delete: Optional[pulumi.InputType['CurlOptsArgs']] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 files: Optional[pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]] = None,
-                 force: Optional[pulumi.Input[bool]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 on_delete: Optional[pulumi.Input[bool]] = None,
-                 recursive: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 verbose: Optional[pulumi.Input[bool]] = None,
+                 update: Optional[pulumi.InputType['CurlOptsArgs']] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = RmArgs.__new__(RmArgs)
+            __props__ = CurlArgs.__new__(CurlArgs)
 
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            __props__.__dict__["dir"] = dir
+            __props__.__dict__["create"] = create
+            __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
-            if files is None and not opts.urn:
-                raise TypeError("Missing required property 'files'")
-            __props__.__dict__["files"] = files
-            __props__.__dict__["force"] = force
-            __props__.__dict__["lifecycle"] = lifecycle
-            __props__.__dict__["on_delete"] = on_delete
-            __props__.__dict__["recursive"] = recursive
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
-            __props__.__dict__["verbose"] = verbose
+            __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Rm, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Rm',
+        super(Curl, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Curl',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -342,67 +278,37 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def dir(self) -> pulumi.Output[bool]:
-        """
-        Corresponds to the `--dir` option.
-        """
-        return pulumi.get(self, "dir")
-
-    @property
-    @pulumi.getter
-    def environment(self) -> pulumi.Output[Mapping[str, str]]:
-        """
-        Environment variables
-        """
-        return pulumi.get(self, "environment")
-
-    @property
-    @pulumi.getter
-    def files(self) -> pulumi.Output[Any]:
+    def create(self) -> pulumi.Output[Optional['outputs.CurlOpts']]:
         """
-        Corresponds to the [FILE] argument.
+        The command to run on create.
         """
-        return pulumi.get(self, "files")
+        return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def force(self) -> pulumi.Output[bool]:
+    def delete(self) -> pulumi.Output[Optional['outputs.CurlOpts']]:
         """
-        Corresponds to the `--force` option.
+        The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+        Command resource from previous create or update steps.
         """
-        return pulumi.get(self, "force")
+        return pulumi.get(self, "delete")
 
     @property
     @pulumi.getter
-    def lifecycle(self) -> pulumi.Output[Optional['CommandLifecycle']]:
-        """
-        At what stage(s) in the resource lifecycle should the command be run
-        """
-        return pulumi.get(self, "lifecycle")
-
-    @property
-    @pulumi.getter(name="onDelete")
-    def on_delete(self) -> pulumi.Output[bool]:
-        """
-        Whether rm should be run when the resource is created or deleted.
-        """
-        return pulumi.get(self, "on_delete")
-
-    @property
-    @pulumi.getter
-    def recursive(self) -> pulumi.Output[bool]:
+    def environment(self) -> pulumi.Output[Mapping[str, str]]:
         """
-        Corresponds to the `--recursive` option.
+        Environment variables
         """
-        return pulumi.get(self, "recursive")
+        return pulumi.get(self, "environment")
 
     @property
     @pulumi.getter
     def stderr(self) -> pulumi.Output[str]:
         """
         TODO
         """
@@ -430,13 +336,16 @@
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def verbose(self) -> pulumi.Output[bool]:
+    def update(self) -> pulumi.Output[Optional['outputs.CurlOpts']]:
         """
-        Corresponds to the `--verbose` option.
+        The command to run on update, if empty, create will 
+        run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+        are set to the stdout and stderr properties of the Command resource from previous 
+        create or update steps.
         """
-        return pulumi.get(self, "verbose")
+        return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,142 +4,124 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from ._enums import *
+from . import outputs
+from ._inputs import *
 import pulumi_command
 
-__all__ = ['SystemctlArgs', 'Systemctl']
+__all__ = ['MktempArgs', 'Mktemp']
 
 @pulumi.input_type
-class SystemctlArgs:
+class MktempArgs:
     def __init__(__self__, *,
-                 command: 'SystemctlCommand',
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 unit: pulumi.Input[str],
                  binary_path: Optional[pulumi.Input[str]] = None,
+                 create: Optional['MktempOptsArgs'] = None,
+                 delete: Optional['MktempOptsArgs'] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 pattern: Optional[pulumi.Input[str]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
-                 triggers: Optional[pulumi.Input[Sequence[Any]]] = None):
+                 triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
+                 update: Optional['MktempOptsArgs'] = None):
         """
-        The set of arguments for constructing a Systemctl resource.
-        :param 'SystemctlCommand' command: Corresponds to the COMMAND argument.
+        The set of arguments for constructing a Mktemp resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
-        :param pulumi.Input[str] unit: Corresponds to the [UNIT...] argument.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
+        :param 'MktempOptsArgs' create: The command to run on create.
+        :param 'MktempOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+               and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+               Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
-        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
-        :param pulumi.Input[str] pattern: Corresponds to the [PATTERN] argument
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param 'MktempOptsArgs' update: The command to run on update, if empty, create will 
+               run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+               are set to the stdout and stderr properties of the Command resource from previous 
+               create or update steps.
         """
-        pulumi.set(__self__, "command", command)
         pulumi.set(__self__, "connection", connection)
-        pulumi.set(__self__, "unit", unit)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
+        if create is not None:
+            pulumi.set(__self__, "create", create)
+        if delete is not None:
+            pulumi.set(__self__, "delete", delete)
         if environment is not None:
             pulumi.set(__self__, "environment", environment)
-        if lifecycle is not None:
-            pulumi.set(__self__, "lifecycle", lifecycle)
-        if pattern is not None:
-            pulumi.set(__self__, "pattern", pattern)
         if stdin is not None:
             pulumi.set(__self__, "stdin", stdin)
         if triggers is not None:
             pulumi.set(__self__, "triggers", triggers)
-
-    @property
-    @pulumi.getter
-    def command(self) -> 'SystemctlCommand':
-        """
-        Corresponds to the COMMAND argument.
-        """
-        return pulumi.get(self, "command")
-
-    @command.setter
-    def command(self, value: 'SystemctlCommand'):
-        pulumi.set(self, "command", value)
+        if update is not None:
+            pulumi.set(__self__, "update", update)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
-    @pulumi.getter
-    def unit(self) -> pulumi.Input[str]:
-        """
-        Corresponds to the [UNIT...] argument.
-        """
-        return pulumi.get(self, "unit")
-
-    @unit.setter
-    def unit(self, value: pulumi.Input[str]):
-        pulumi.set(self, "unit", value)
-
-    @property
     @pulumi.getter(name="binaryPath")
     def binary_path(self) -> Optional[pulumi.Input[str]]:
         """
         Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         """
         return pulumi.get(self, "binary_path")
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+    def create(self) -> Optional['MktempOptsArgs']:
         """
-        Environment variables
+        The command to run on create.
         """
-        return pulumi.get(self, "environment")
+        return pulumi.get(self, "create")
 
-    @environment.setter
-    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
-        pulumi.set(self, "environment", value)
+    @create.setter
+    def create(self, value: Optional['MktempOptsArgs']):
+        pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def lifecycle(self) -> Optional['CommandLifecycle']:
+    def delete(self) -> Optional['MktempOptsArgs']:
         """
-        At what stage(s) in the resource lifecycle should the command be run
+        The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+        Command resource from previous create or update steps.
         """
-        return pulumi.get(self, "lifecycle")
+        return pulumi.get(self, "delete")
 
-    @lifecycle.setter
-    def lifecycle(self, value: Optional['CommandLifecycle']):
-        pulumi.set(self, "lifecycle", value)
+    @delete.setter
+    def delete(self, value: Optional['MktempOptsArgs']):
+        pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
-    def pattern(self) -> Optional[pulumi.Input[str]]:
+    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Corresponds to the [PATTERN] argument
+        Environment variables
         """
-        return pulumi.get(self, "pattern")
+        return pulumi.get(self, "environment")
 
-    @pattern.setter
-    def pattern(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "pattern", value)
+    @environment.setter
+    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "environment", value)
 
     @property
     @pulumi.getter
     def stdin(self) -> Optional[pulumi.Input[str]]:
         """
         TODO
         """
@@ -157,109 +139,121 @@
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
+    @property
+    @pulumi.getter
+    def update(self) -> Optional['MktempOptsArgs']:
+        """
+        The command to run on update, if empty, create will 
+        run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+        are set to the stdout and stderr properties of the Command resource from previous 
+        create or update steps.
+        """
+        return pulumi.get(self, "update")
+
+    @update.setter
+    def update(self, value: Optional['MktempOptsArgs']):
+        pulumi.set(self, "update", value)
+
 
-class Systemctl(pulumi.ComponentResource):
+class Mktemp(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 command: Optional['SystemctlCommand'] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
+                 create: Optional[pulumi.InputType['MktempOptsArgs']] = None,
+                 delete: Optional[pulumi.InputType['MktempOptsArgs']] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 pattern: Optional[pulumi.Input[str]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 unit: Optional[pulumi.Input[str]] = None,
+                 update: Optional[pulumi.InputType['MktempOptsArgs']] = None,
                  __props__=None):
         """
-        Abstraction over the `systemctl` utility on a remote system.
+        Abstraction over the `mktemp` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param 'SystemctlCommand' command: Corresponds to the COMMAND argument.
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
+        :param pulumi.InputType['MktempOptsArgs'] create: The command to run on create.
+        :param pulumi.InputType['MktempOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+               and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+               Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
-        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
-        :param pulumi.Input[str] pattern: Corresponds to the [PATTERN] argument
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.Input[str] unit: Corresponds to the [UNIT...] argument.
+        :param pulumi.InputType['MktempOptsArgs'] update: The command to run on update, if empty, create will 
+               run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+               are set to the stdout and stderr properties of the Command resource from previous 
+               create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: SystemctlArgs,
+                 args: MktempArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `systemctl` utility on a remote system.
+        Abstraction over the `mktemp` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param SystemctlArgs args: The arguments to use to populate this resource's properties.
+        :param MktempArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(SystemctlArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(MktempArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 command: Optional['SystemctlCommand'] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
+                 create: Optional[pulumi.InputType['MktempOptsArgs']] = None,
+                 delete: Optional[pulumi.InputType['MktempOptsArgs']] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 pattern: Optional[pulumi.Input[str]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 unit: Optional[pulumi.Input[str]] = None,
+                 update: Optional[pulumi.InputType['MktempOptsArgs']] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = SystemctlArgs.__new__(SystemctlArgs)
+            __props__ = MktempArgs.__new__(MktempArgs)
 
             __props__.__dict__["binary_path"] = binary_path
-            if command is None and not opts.urn:
-                raise TypeError("Missing required property 'command'")
-            __props__.__dict__["command"] = command
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
+            __props__.__dict__["create"] = create
+            __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
-            __props__.__dict__["lifecycle"] = lifecycle
-            __props__.__dict__["pattern"] = pattern
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
-            if unit is None and not opts.urn:
-                raise TypeError("Missing required property 'unit'")
-            __props__.__dict__["unit"] = unit
+            __props__.__dict__["update"] = update
+            __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-            __props__.__dict__["systemctl_command"] = None
-        super(Systemctl, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Systemctl',
+        super(Mktemp, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Mktemp',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -283,35 +277,37 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def environment(self) -> pulumi.Output[Mapping[str, str]]:
+    def create(self) -> pulumi.Output[Optional['outputs.MktempOpts']]:
         """
-        Environment variables
+        The command to run on create.
         """
-        return pulumi.get(self, "environment")
+        return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def lifecycle(self) -> pulumi.Output[Optional['CommandLifecycle']]:
+    def delete(self) -> pulumi.Output[Optional['outputs.MktempOpts']]:
         """
-        At what stage(s) in the resource lifecycle should the command be run
+        The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+        Command resource from previous create or update steps.
         """
-        return pulumi.get(self, "lifecycle")
+        return pulumi.get(self, "delete")
 
     @property
     @pulumi.getter
-    def pattern(self) -> pulumi.Output[Optional[str]]:
+    def environment(self) -> pulumi.Output[Mapping[str, str]]:
         """
-        Corresponds to the [PATTERN] argument
+        Environment variables
         """
-        return pulumi.get(self, "pattern")
+        return pulumi.get(self, "environment")
 
     @property
     @pulumi.getter
     def stderr(self) -> pulumi.Output[str]:
         """
         TODO
         """
@@ -330,30 +326,25 @@
     def stdout(self) -> pulumi.Output[str]:
         """
         TODO
         """
         return pulumi.get(self, "stdout")
 
     @property
-    @pulumi.getter(name="systemctlCommand")
-    def systemctl_command(self) -> pulumi.Output['SystemctlCommand']:
-        """
-        Corresponds to the COMMAND argument.
-        """
-        return pulumi.get(self, "systemctl_command")
-
-    @property
     @pulumi.getter
     def triggers(self) -> pulumi.Output[Sequence[Any]]:
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def unit(self) -> pulumi.Output[str]:
+    def update(self) -> pulumi.Output[Optional['outputs.MktempOpts']]:
         """
-        Corresponds to the [UNIT...] argument.
+        The command to run on update, if empty, create will 
+        run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+        are set to the stdout and stderr properties of the Command resource from previous 
+        create or update steps.
         """
-        return pulumi.get(self, "unit")
+        return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,91 +4,63 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from . import outputs
 from ._enums import *
+from ._inputs import *
 import pulumi_command
 
-__all__ = ['TarArgs', 'Tar']
+__all__ = ['SystemctlArgs', 'Systemctl']
 
 @pulumi.input_type
-class TarArgs:
+class SystemctlArgs:
     def __init__(__self__, *,
-                 archive: pulumi.Input[str],
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 directory: Optional[pulumi.Input[str]] = None,
+                 create: Optional['SystemctlOptsArgs'] = None,
+                 delete: Optional['SystemctlOptsArgs'] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 extract: Optional[pulumi.Input[bool]] = None,
-                 files: Optional[pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]] = None,
-                 gzip: Optional[pulumi.Input[bool]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 on_delete: Optional[pulumi.Input[bool]] = None,
-                 recursive: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
-                 strip_components: Optional[pulumi.Input[int]] = None,
-                 triggers: Optional[pulumi.Input[Sequence[Any]]] = None):
+                 triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
+                 update: Optional['SystemctlOptsArgs'] = None):
         """
-        The set of arguments for constructing a Tar resource.
-        :param pulumi.Input[str] archive: Corresponds to the [ARCHIVE] argument.
+        The set of arguments for constructing a Systemctl resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param pulumi.Input[str] directory: Corresponds to the `--directory` option.
+        :param 'SystemctlOptsArgs' create: The command to run on create.
+        :param 'SystemctlOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+               and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+               Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
-        :param pulumi.Input[bool] extract: Corresponds to the `--extract` option.
-        :param pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]] files: Corresponds to the [FILE] argument.
-        :param pulumi.Input[bool] gzip: Corresponds to the `--gzip` option.
-        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
-        :param pulumi.Input[bool] on_delete: Whether rm should be run when the resource is created or deleted.
-        :param pulumi.Input[bool] recursive: Corresponds to the `--recursive` option.
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[int] strip_components: Corresponds to the `--strip-components` option.
         :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param 'SystemctlOptsArgs' update: The command to run on update, if empty, create will 
+               run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+               are set to the stdout and stderr properties of the Command resource from previous 
+               create or update steps.
         """
-        pulumi.set(__self__, "archive", archive)
         pulumi.set(__self__, "connection", connection)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
-        if directory is not None:
-            pulumi.set(__self__, "directory", directory)
+        if create is not None:
+            pulumi.set(__self__, "create", create)
+        if delete is not None:
+            pulumi.set(__self__, "delete", delete)
         if environment is not None:
             pulumi.set(__self__, "environment", environment)
-        if extract is not None:
-            pulumi.set(__self__, "extract", extract)
-        if files is not None:
-            pulumi.set(__self__, "files", files)
-        if gzip is not None:
-            pulumi.set(__self__, "gzip", gzip)
-        if lifecycle is not None:
-            pulumi.set(__self__, "lifecycle", lifecycle)
-        if on_delete is not None:
-            pulumi.set(__self__, "on_delete", on_delete)
-        if recursive is not None:
-            pulumi.set(__self__, "recursive", recursive)
         if stdin is not None:
             pulumi.set(__self__, "stdin", stdin)
-        if strip_components is not None:
-            pulumi.set(__self__, "strip_components", strip_components)
         if triggers is not None:
             pulumi.set(__self__, "triggers", triggers)
-
-    @property
-    @pulumi.getter
-    def archive(self) -> pulumi.Input[str]:
-        """
-        Corresponds to the [ARCHIVE] argument.
-        """
-        return pulumi.get(self, "archive")
-
-    @archive.setter
-    def archive(self, value: pulumi.Input[str]):
-        pulumi.set(self, "archive", value)
+        if update is not None:
+            pulumi.set(__self__, "update", update)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
         Connection details for the remote system
         """
@@ -108,271 +80,187 @@
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def directory(self) -> Optional[pulumi.Input[str]]:
-        """
-        Corresponds to the `--directory` option.
-        """
-        return pulumi.get(self, "directory")
-
-    @directory.setter
-    def directory(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "directory", value)
-
-    @property
-    @pulumi.getter
-    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+    def create(self) -> Optional['SystemctlOptsArgs']:
         """
-        Environment variables
+        The command to run on create.
         """
-        return pulumi.get(self, "environment")
+        return pulumi.get(self, "create")
 
-    @environment.setter
-    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
-        pulumi.set(self, "environment", value)
+    @create.setter
+    def create(self, value: Optional['SystemctlOptsArgs']):
+        pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def extract(self) -> Optional[pulumi.Input[bool]]:
+    def delete(self) -> Optional['SystemctlOptsArgs']:
         """
-        Corresponds to the `--extract` option.
+        The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+        Command resource from previous create or update steps.
         """
-        return pulumi.get(self, "extract")
+        return pulumi.get(self, "delete")
 
-    @extract.setter
-    def extract(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "extract", value)
+    @delete.setter
+    def delete(self, value: Optional['SystemctlOptsArgs']):
+        pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
-    def files(self) -> Optional[pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]]:
-        """
-        Corresponds to the [FILE] argument.
-        """
-        return pulumi.get(self, "files")
-
-    @files.setter
-    def files(self, value: Optional[pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]]):
-        pulumi.set(self, "files", value)
-
-    @property
-    @pulumi.getter
-    def gzip(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Corresponds to the `--gzip` option.
-        """
-        return pulumi.get(self, "gzip")
-
-    @gzip.setter
-    def gzip(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "gzip", value)
-
-    @property
-    @pulumi.getter
-    def lifecycle(self) -> Optional['CommandLifecycle']:
-        """
-        At what stage(s) in the resource lifecycle should the command be run
-        """
-        return pulumi.get(self, "lifecycle")
-
-    @lifecycle.setter
-    def lifecycle(self, value: Optional['CommandLifecycle']):
-        pulumi.set(self, "lifecycle", value)
-
-    @property
-    @pulumi.getter(name="onDelete")
-    def on_delete(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Whether rm should be run when the resource is created or deleted.
-        """
-        return pulumi.get(self, "on_delete")
-
-    @on_delete.setter
-    def on_delete(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "on_delete", value)
-
-    @property
-    @pulumi.getter
-    def recursive(self) -> Optional[pulumi.Input[bool]]:
+    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Corresponds to the `--recursive` option.
+        Environment variables
         """
-        return pulumi.get(self, "recursive")
+        return pulumi.get(self, "environment")
 
-    @recursive.setter
-    def recursive(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "recursive", value)
+    @environment.setter
+    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "environment", value)
 
     @property
     @pulumi.getter
     def stdin(self) -> Optional[pulumi.Input[str]]:
         """
         TODO
         """
         return pulumi.get(self, "stdin")
 
     @stdin.setter
     def stdin(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "stdin", value)
 
     @property
-    @pulumi.getter(name="stripComponents")
-    def strip_components(self) -> Optional[pulumi.Input[int]]:
-        """
-        Corresponds to the `--strip-components` option.
-        """
-        return pulumi.get(self, "strip_components")
-
-    @strip_components.setter
-    def strip_components(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "strip_components", value)
-
-    @property
     @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Sequence[Any]]]:
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
+    @property
+    @pulumi.getter
+    def update(self) -> Optional['SystemctlOptsArgs']:
+        """
+        The command to run on update, if empty, create will 
+        run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+        are set to the stdout and stderr properties of the Command resource from previous 
+        create or update steps.
+        """
+        return pulumi.get(self, "update")
+
+    @update.setter
+    def update(self, value: Optional['SystemctlOptsArgs']):
+        pulumi.set(self, "update", value)
 
-class Tar(pulumi.ComponentResource):
+
+class Systemctl(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 archive: Optional[pulumi.Input[str]] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 directory: Optional[pulumi.Input[str]] = None,
+                 create: Optional[pulumi.InputType['SystemctlOptsArgs']] = None,
+                 delete: Optional[pulumi.InputType['SystemctlOptsArgs']] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 extract: Optional[pulumi.Input[bool]] = None,
-                 files: Optional[pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]] = None,
-                 gzip: Optional[pulumi.Input[bool]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 on_delete: Optional[pulumi.Input[bool]] = None,
-                 recursive: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
-                 strip_components: Optional[pulumi.Input[int]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
+                 update: Optional[pulumi.InputType['SystemctlOptsArgs']] = None,
                  __props__=None):
         """
-        Abstraction over the `rm` utility on a remote system.
+        Abstraction over the `systemctl` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] archive: Corresponds to the [ARCHIVE] argument.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.Input[str] directory: Corresponds to the `--directory` option.
+        :param pulumi.InputType['SystemctlOptsArgs'] create: The command to run on create.
+        :param pulumi.InputType['SystemctlOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+               and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+               Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
-        :param pulumi.Input[bool] extract: Corresponds to the `--extract` option.
-        :param pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]] files: Corresponds to the [FILE] argument.
-        :param pulumi.Input[bool] gzip: Corresponds to the `--gzip` option.
-        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
-        :param pulumi.Input[bool] on_delete: Whether rm should be run when the resource is created or deleted.
-        :param pulumi.Input[bool] recursive: Corresponds to the `--recursive` option.
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[int] strip_components: Corresponds to the `--strip-components` option.
         :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param pulumi.InputType['SystemctlOptsArgs'] update: The command to run on update, if empty, create will 
+               run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+               are set to the stdout and stderr properties of the Command resource from previous 
+               create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: TarArgs,
+                 args: SystemctlArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `rm` utility on a remote system.
+        Abstraction over the `systemctl` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param TarArgs args: The arguments to use to populate this resource's properties.
+        :param SystemctlArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(TarArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(SystemctlArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 archive: Optional[pulumi.Input[str]] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 directory: Optional[pulumi.Input[str]] = None,
+                 create: Optional[pulumi.InputType['SystemctlOptsArgs']] = None,
+                 delete: Optional[pulumi.InputType['SystemctlOptsArgs']] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 extract: Optional[pulumi.Input[bool]] = None,
-                 files: Optional[pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]] = None,
-                 gzip: Optional[pulumi.Input[bool]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 on_delete: Optional[pulumi.Input[bool]] = None,
-                 recursive: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
-                 strip_components: Optional[pulumi.Input[int]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
+                 update: Optional[pulumi.InputType['SystemctlOptsArgs']] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = TarArgs.__new__(TarArgs)
+            __props__ = SystemctlArgs.__new__(SystemctlArgs)
 
-            if archive is None and not opts.urn:
-                raise TypeError("Missing required property 'archive'")
-            __props__.__dict__["archive"] = archive
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            __props__.__dict__["directory"] = directory
+            __props__.__dict__["create"] = create
+            __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
-            __props__.__dict__["extract"] = extract
-            __props__.__dict__["files"] = files
-            __props__.__dict__["gzip"] = gzip
-            __props__.__dict__["lifecycle"] = lifecycle
-            __props__.__dict__["on_delete"] = on_delete
-            __props__.__dict__["recursive"] = recursive
             __props__.__dict__["stdin"] = stdin
-            __props__.__dict__["strip_components"] = strip_components
             __props__.__dict__["triggers"] = triggers
+            __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Tar, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Tar',
+        super(Systemctl, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Systemctl',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
-    @pulumi.getter
-    def archive(self) -> pulumi.Output[str]:
-        """
-        Corresponds to the [ARCHIVE] argument.
-        """
-        return pulumi.get(self, "archive")
-
-    @property
     @pulumi.getter(name="binaryPath")
     def binary_path(self) -> pulumi.Output[str]:
         """
         Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         """
         return pulumi.get(self, "binary_path")
 
@@ -390,75 +278,37 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def directory(self) -> pulumi.Output[Optional[str]]:
-        """
-        Corresponds to the `--directory` option.
-        """
-        return pulumi.get(self, "directory")
-
-    @property
-    @pulumi.getter
-    def environment(self) -> pulumi.Output[Mapping[str, str]]:
-        """
-        Environment variables
-        """
-        return pulumi.get(self, "environment")
-
-    @property
-    @pulumi.getter
-    def extract(self) -> pulumi.Output[bool]:
+    def create(self) -> pulumi.Output[Optional['outputs.SystemctlOpts']]:
         """
-        Corresponds to the `--extract` option.
+        The command to run on create.
         """
-        return pulumi.get(self, "extract")
+        return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def files(self) -> pulumi.Output[Any]:
+    def delete(self) -> pulumi.Output[Optional['outputs.SystemctlOpts']]:
         """
-        Corresponds to the [FILE] argument.
+        The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+        Command resource from previous create or update steps.
         """
-        return pulumi.get(self, "files")
+        return pulumi.get(self, "delete")
 
     @property
     @pulumi.getter
-    def gzip(self) -> pulumi.Output[Optional[bool]]:
-        """
-        Corresponds to the `--gzip` option.
-        """
-        return pulumi.get(self, "gzip")
-
-    @property
-    @pulumi.getter
-    def lifecycle(self) -> pulumi.Output[Optional['CommandLifecycle']]:
-        """
-        At what stage(s) in the resource lifecycle should the command be run
-        """
-        return pulumi.get(self, "lifecycle")
-
-    @property
-    @pulumi.getter(name="onDelete")
-    def on_delete(self) -> pulumi.Output[Optional[bool]]:
-        """
-        Whether rm should be run when the resource is created or deleted.
-        """
-        return pulumi.get(self, "on_delete")
-
-    @property
-    @pulumi.getter
-    def recursive(self) -> pulumi.Output[Optional[bool]]:
+    def environment(self) -> pulumi.Output[Mapping[str, str]]:
         """
-        Corresponds to the `--recursive` option.
+        Environment variables
         """
-        return pulumi.get(self, "recursive")
+        return pulumi.get(self, "environment")
 
     @property
     @pulumi.getter
     def stderr(self) -> pulumi.Output[str]:
         """
         TODO
         """
@@ -477,22 +327,25 @@
     def stdout(self) -> pulumi.Output[str]:
         """
         TODO
         """
         return pulumi.get(self, "stdout")
 
     @property
-    @pulumi.getter(name="stripComponents")
-    def strip_components(self) -> pulumi.Output[Optional[int]]:
+    @pulumi.getter
+    def triggers(self) -> pulumi.Output[Sequence[Any]]:
         """
-        Corresponds to the `--strip-components` option.
+        TODO
         """
-        return pulumi.get(self, "strip_components")
+        return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def triggers(self) -> pulumi.Output[Sequence[Any]]:
+    def update(self) -> pulumi.Output[Optional['outputs.SystemctlOpts']]:
         """
-        TODO
+        The command to run on update, if empty, create will 
+        run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+        are set to the stdout and stderr properties of the Command resource from previous 
+        create or update steps.
         """
-        return pulumi.get(self, "triggers")
+        return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,190 +4,137 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
+from . import outputs
 from ._enums import *
+from ._inputs import *
 import pulumi_command
 
-__all__ = ['TeeArgs', 'Tee']
+__all__ = ['EtcdctlArgs', 'Etcdctl']
 
 @pulumi.input_type
-class TeeArgs:
+class EtcdctlArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 files: pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]],
-                 stdin: pulumi.Input[str],
-                 append: Optional[pulumi.Input[bool]] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
+                 create: Optional['EtcdctlOptsArgs'] = None,
+                 delete: Optional['EtcdctlOptsArgs'] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 ignore_interrupts: Optional[pulumi.Input[bool]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 output_error: Optional[pulumi.Input['TeeMode']] = None,
-                 pipe: Optional[pulumi.Input[bool]] = None,
+                 stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 version: Optional[pulumi.Input[bool]] = None):
+                 update: Optional['EtcdctlOptsArgs'] = None):
         """
-        The set of arguments for constructing a Tee resource.
+        The set of arguments for constructing a Etcdctl resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
-        :param pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]] files: Corresponds to the [FILE] argument.
-        :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[bool] append: Append to the given FILEs, do not overwrite
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
+        :param 'EtcdctlOptsArgs' create: The command to run on create.
+        :param 'EtcdctlOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+               and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+               Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
-        :param pulumi.Input[bool] ignore_interrupts: Ignore interrupt signals.
-        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
-        :param pulumi.Input['TeeMode'] output_error: Set behavior on write error.
-        :param pulumi.Input[bool] pipe: Operate in a more appropriate MODE with pipes.
+        :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.Input[bool] version: Output version information and exit.
+        :param 'EtcdctlOptsArgs' update: The command to run on update, if empty, create will 
+               run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+               are set to the stdout and stderr properties of the Command resource from previous 
+               create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
-        pulumi.set(__self__, "files", files)
-        pulumi.set(__self__, "stdin", stdin)
-        if append is not None:
-            pulumi.set(__self__, "append", append)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
+        if create is not None:
+            pulumi.set(__self__, "create", create)
+        if delete is not None:
+            pulumi.set(__self__, "delete", delete)
         if environment is not None:
             pulumi.set(__self__, "environment", environment)
-        if ignore_interrupts is not None:
-            pulumi.set(__self__, "ignore_interrupts", ignore_interrupts)
-        if lifecycle is not None:
-            pulumi.set(__self__, "lifecycle", lifecycle)
-        if output_error is not None:
-            pulumi.set(__self__, "output_error", output_error)
-        if pipe is not None:
-            pulumi.set(__self__, "pipe", pipe)
+        if stdin is not None:
+            pulumi.set(__self__, "stdin", stdin)
         if triggers is not None:
             pulumi.set(__self__, "triggers", triggers)
-        if version is not None:
-            pulumi.set(__self__, "version", version)
+        if update is not None:
+            pulumi.set(__self__, "update", update)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
-    @pulumi.getter
-    def files(self) -> pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]:
-        """
-        Corresponds to the [FILE] argument.
-        """
-        return pulumi.get(self, "files")
-
-    @files.setter
-    def files(self, value: pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "files", value)
-
-    @property
-    @pulumi.getter
-    def stdin(self) -> pulumi.Input[str]:
-        """
-        TODO
-        """
-        return pulumi.get(self, "stdin")
-
-    @stdin.setter
-    def stdin(self, value: pulumi.Input[str]):
-        pulumi.set(self, "stdin", value)
-
-    @property
-    @pulumi.getter
-    def append(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Append to the given FILEs, do not overwrite
-        """
-        return pulumi.get(self, "append")
-
-    @append.setter
-    def append(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "append", value)
-
-    @property
     @pulumi.getter(name="binaryPath")
     def binary_path(self) -> Optional[pulumi.Input[str]]:
         """
         Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         """
         return pulumi.get(self, "binary_path")
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
     @pulumi.getter
-    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
-        """
-        Environment variables
-        """
-        return pulumi.get(self, "environment")
-
-    @environment.setter
-    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
-        pulumi.set(self, "environment", value)
-
-    @property
-    @pulumi.getter(name="ignoreInterrupts")
-    def ignore_interrupts(self) -> Optional[pulumi.Input[bool]]:
+    def create(self) -> Optional['EtcdctlOptsArgs']:
         """
-        Ignore interrupt signals.
+        The command to run on create.
         """
-        return pulumi.get(self, "ignore_interrupts")
+        return pulumi.get(self, "create")
 
-    @ignore_interrupts.setter
-    def ignore_interrupts(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "ignore_interrupts", value)
+    @create.setter
+    def create(self, value: Optional['EtcdctlOptsArgs']):
+        pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def lifecycle(self) -> Optional['CommandLifecycle']:
+    def delete(self) -> Optional['EtcdctlOptsArgs']:
         """
-        At what stage(s) in the resource lifecycle should the command be run
+        The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+        Command resource from previous create or update steps.
         """
-        return pulumi.get(self, "lifecycle")
+        return pulumi.get(self, "delete")
 
-    @lifecycle.setter
-    def lifecycle(self, value: Optional['CommandLifecycle']):
-        pulumi.set(self, "lifecycle", value)
+    @delete.setter
+    def delete(self, value: Optional['EtcdctlOptsArgs']):
+        pulumi.set(self, "delete", value)
 
     @property
-    @pulumi.getter(name="outputError")
-    def output_error(self) -> Optional[pulumi.Input['TeeMode']]:
+    @pulumi.getter
+    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Set behavior on write error.
+        Environment variables
         """
-        return pulumi.get(self, "output_error")
+        return pulumi.get(self, "environment")
 
-    @output_error.setter
-    def output_error(self, value: Optional[pulumi.Input['TeeMode']]):
-        pulumi.set(self, "output_error", value)
+    @environment.setter
+    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "environment", value)
 
     @property
     @pulumi.getter
-    def pipe(self) -> Optional[pulumi.Input[bool]]:
+    def stdin(self) -> Optional[pulumi.Input[str]]:
         """
-        Operate in a more appropriate MODE with pipes.
+        TODO
         """
-        return pulumi.get(self, "pipe")
+        return pulumi.get(self, "stdin")
 
-    @pipe.setter
-    def pipe(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "pipe", value)
+    @stdin.setter
+    def stdin(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "stdin", value)
 
     @property
     @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Sequence[Any]]]:
         """
         TODO
         """
@@ -195,145 +142,125 @@
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
     @property
     @pulumi.getter
-    def version(self) -> Optional[pulumi.Input[bool]]:
+    def update(self) -> Optional['EtcdctlOptsArgs']:
         """
-        Output version information and exit.
+        The command to run on update, if empty, create will 
+        run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+        are set to the stdout and stderr properties of the Command resource from previous 
+        create or update steps.
         """
-        return pulumi.get(self, "version")
+        return pulumi.get(self, "update")
 
-    @version.setter
-    def version(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "version", value)
+    @update.setter
+    def update(self, value: Optional['EtcdctlOptsArgs']):
+        pulumi.set(self, "update", value)
 
 
-class Tee(pulumi.ComponentResource):
+class Etcdctl(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 append: Optional[pulumi.Input[bool]] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
+                 create: Optional[pulumi.InputType['EtcdctlOptsArgs']] = None,
+                 delete: Optional[pulumi.InputType['EtcdctlOptsArgs']] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 files: Optional[pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]] = None,
-                 ignore_interrupts: Optional[pulumi.Input[bool]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 output_error: Optional[pulumi.Input['TeeMode']] = None,
-                 pipe: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 version: Optional[pulumi.Input[bool]] = None,
+                 update: Optional[pulumi.InputType['EtcdctlOptsArgs']] = None,
                  __props__=None):
         """
-        Abstraction over the `rm` utility on a remote system.
+        Abstraction over the `etcdctl` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[bool] append: Append to the given FILEs, do not overwrite
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
+        :param pulumi.InputType['EtcdctlOptsArgs'] create: The command to run on create.
+        :param pulumi.InputType['EtcdctlOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+               and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+               Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
-        :param pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]] files: Corresponds to the [FILE] argument.
-        :param pulumi.Input[bool] ignore_interrupts: Ignore interrupt signals.
-        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
-        :param pulumi.Input['TeeMode'] output_error: Set behavior on write error.
-        :param pulumi.Input[bool] pipe: Operate in a more appropriate MODE with pipes.
         :param pulumi.Input[str] stdin: TODO
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.Input[bool] version: Output version information and exit.
+        :param pulumi.InputType['EtcdctlOptsArgs'] update: The command to run on update, if empty, create will 
+               run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+               are set to the stdout and stderr properties of the Command resource from previous 
+               create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: TeeArgs,
+                 args: EtcdctlArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `rm` utility on a remote system.
+        Abstraction over the `etcdctl` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param TeeArgs args: The arguments to use to populate this resource's properties.
+        :param EtcdctlArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(TeeArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(EtcdctlArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 append: Optional[pulumi.Input[bool]] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
+                 create: Optional[pulumi.InputType['EtcdctlOptsArgs']] = None,
+                 delete: Optional[pulumi.InputType['EtcdctlOptsArgs']] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 files: Optional[pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]] = None,
-                 ignore_interrupts: Optional[pulumi.Input[bool]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 output_error: Optional[pulumi.Input['TeeMode']] = None,
-                 pipe: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 version: Optional[pulumi.Input[bool]] = None,
+                 update: Optional[pulumi.InputType['EtcdctlOptsArgs']] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = TeeArgs.__new__(TeeArgs)
+            __props__ = EtcdctlArgs.__new__(EtcdctlArgs)
 
-            __props__.__dict__["append"] = append
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
+            __props__.__dict__["create"] = create
+            __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
-            if files is None and not opts.urn:
-                raise TypeError("Missing required property 'files'")
-            __props__.__dict__["files"] = files
-            __props__.__dict__["ignore_interrupts"] = ignore_interrupts
-            __props__.__dict__["lifecycle"] = lifecycle
-            __props__.__dict__["output_error"] = output_error
-            __props__.__dict__["pipe"] = pipe
-            if stdin is None and not opts.urn:
-                raise TypeError("Missing required property 'stdin'")
             __props__.__dict__["stdin"] = stdin
             __props__.__dict__["triggers"] = triggers
-            __props__.__dict__["version"] = version
+            __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Tee, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Tee',
+        super(Etcdctl, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Etcdctl',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
-    @pulumi.getter
-    def append(self) -> pulumi.Output[bool]:
-        """
-        Append to the given FILEs, do not overwrite
-        """
-        return pulumi.get(self, "append")
-
-    @property
     @pulumi.getter(name="binaryPath")
     def binary_path(self) -> pulumi.Output[str]:
         """
         Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         """
         return pulumi.get(self, "binary_path")
 
@@ -351,71 +278,49 @@
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
     @pulumi.getter
-    def environment(self) -> pulumi.Output[Mapping[str, str]]:
+    def create(self) -> pulumi.Output[Optional['outputs.EtcdctlOpts']]:
         """
-        Environment variables
+        The command to run on create.
         """
-        return pulumi.get(self, "environment")
+        return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def files(self) -> pulumi.Output[Any]:
-        """
-        Corresponds to the [FILE] argument.
-        """
-        return pulumi.get(self, "files")
-
-    @property
-    @pulumi.getter(name="ignoreInterrupts")
-    def ignore_interrupts(self) -> pulumi.Output[bool]:
+    def delete(self) -> pulumi.Output[Optional['outputs.EtcdctlOpts']]:
         """
-        Ignore interrupt signals.
+        The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+        Command resource from previous create or update steps.
         """
-        return pulumi.get(self, "ignore_interrupts")
+        return pulumi.get(self, "delete")
 
     @property
     @pulumi.getter
-    def lifecycle(self) -> pulumi.Output[Optional['CommandLifecycle']]:
-        """
-        At what stage(s) in the resource lifecycle should the command be run
-        """
-        return pulumi.get(self, "lifecycle")
-
-    @property
-    @pulumi.getter(name="outputError")
-    def output_error(self) -> pulumi.Output[Optional['TeeMode']]:
-        """
-        Set behavior on write error.
-        """
-        return pulumi.get(self, "output_error")
-
-    @property
-    @pulumi.getter
-    def pipe(self) -> pulumi.Output[bool]:
+    def environment(self) -> pulumi.Output[Mapping[str, str]]:
         """
-        Operate in a more appropriate MODE with pipes.
+        Environment variables
         """
-        return pulumi.get(self, "pipe")
+        return pulumi.get(self, "environment")
 
     @property
     @pulumi.getter
     def stderr(self) -> pulumi.Output[str]:
         """
         TODO
         """
         return pulumi.get(self, "stderr")
 
     @property
     @pulumi.getter
-    def stdin(self) -> pulumi.Output[str]:
+    def stdin(self) -> pulumi.Output[Optional[str]]:
         """
         TODO
         """
         return pulumi.get(self, "stdin")
 
     @property
     @pulumi.getter
@@ -431,13 +336,16 @@
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def version(self) -> pulumi.Output[bool]:
+    def update(self) -> pulumi.Output[Optional['outputs.EtcdctlOpts']]:
         """
-        Output version information and exit.
+        The command to run on update, if empty, create will 
+        run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+        are set to the stdout and stderr properties of the Command resource from previous 
+        create or update steps.
         """
-        return pulumi.get(self, "version")
+        return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way/tools/sed.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,195 +4,124 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from .. import _utilities
-from ._enums import *
+from . import outputs
+from ._inputs import *
 import pulumi_command
 
-__all__ = ['WgetArgs', 'Wget']
+__all__ = ['SedArgs', 'Sed']
 
 @pulumi.input_type
-class WgetArgs:
+class SedArgs:
     def __init__(__self__, *,
                  connection: pulumi.Input['pulumi_command.remote.ConnectionArgs'],
-                 url: pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]],
                  binary_path: Optional[pulumi.Input[str]] = None,
-                 directory_prefix: Optional[pulumi.Input[str]] = None,
+                 create: Optional['SedOptsArgs'] = None,
+                 delete: Optional['SedOptsArgs'] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 https_only: Optional[pulumi.Input[bool]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 no_verbose: Optional[pulumi.Input[bool]] = None,
-                 output_document: Optional[pulumi.Input[str]] = None,
-                 quiet: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
-                 timestamping: Optional[pulumi.Input[bool]] = None,
-                 triggers: Optional[pulumi.Input[Sequence[Any]]] = None):
+                 triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
+                 update: Optional['SedOptsArgs'] = None):
         """
-        The set of arguments for constructing a Wget resource.
+        The set of arguments for constructing a Sed resource.
         :param pulumi.Input['pulumi_command.remote.ConnectionArgs'] connection: Connection details for the remote system
-        :param pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]] url: Corresponds to the [URL...] argument.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
-        :param pulumi.Input[str] directory_prefix: The  directory prefix is the directory where all other files and subdirectories will be saved to, i.e. the top of the retrieval tree.  The default is . (the current directory).
+        :param 'SedOptsArgs' create: The command to run on create.
+        :param 'SedOptsArgs' delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+               and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+               Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
-        :param pulumi.Input[bool] https_only: When in recursive mode, only HTTPS links are followed.
-        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
-        :param pulumi.Input[bool] no_verbose: Turn off verbose without being completely quiet (use -q for that), which means that error messages and basic information still get printed.
-        :param pulumi.Input[str] output_document: The  documents  will  not  be  written  to the appropriate files, but all will be concatenated together and written to file.
-        :param pulumi.Input[bool] quiet: Turn off Wget's output.
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[bool] timestamping: Turn on time-stamping.
         :param pulumi.Input[Sequence[Any]] triggers: TODO
+        :param 'SedOptsArgs' update: The command to run on update, if empty, create will 
+               run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+               are set to the stdout and stderr properties of the Command resource from previous 
+               create or update steps.
         """
         pulumi.set(__self__, "connection", connection)
-        pulumi.set(__self__, "url", url)
         if binary_path is not None:
             pulumi.set(__self__, "binary_path", binary_path)
-        if directory_prefix is not None:
-            pulumi.set(__self__, "directory_prefix", directory_prefix)
+        if create is not None:
+            pulumi.set(__self__, "create", create)
+        if delete is not None:
+            pulumi.set(__self__, "delete", delete)
         if environment is not None:
             pulumi.set(__self__, "environment", environment)
-        if https_only is not None:
-            pulumi.set(__self__, "https_only", https_only)
-        if lifecycle is not None:
-            pulumi.set(__self__, "lifecycle", lifecycle)
-        if no_verbose is not None:
-            pulumi.set(__self__, "no_verbose", no_verbose)
-        if output_document is not None:
-            pulumi.set(__self__, "output_document", output_document)
-        if quiet is not None:
-            pulumi.set(__self__, "quiet", quiet)
         if stdin is not None:
             pulumi.set(__self__, "stdin", stdin)
-        if timestamping is not None:
-            pulumi.set(__self__, "timestamping", timestamping)
         if triggers is not None:
             pulumi.set(__self__, "triggers", triggers)
+        if update is not None:
+            pulumi.set(__self__, "update", update)
 
     @property
     @pulumi.getter
     def connection(self) -> pulumi.Input['pulumi_command.remote.ConnectionArgs']:
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @connection.setter
     def connection(self, value: pulumi.Input['pulumi_command.remote.ConnectionArgs']):
         pulumi.set(self, "connection", value)
 
     @property
-    @pulumi.getter
-    def url(self) -> pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]:
-        """
-        Corresponds to the [URL...] argument.
-        """
-        return pulumi.get(self, "url")
-
-    @url.setter
-    def url(self, value: pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]):
-        pulumi.set(self, "url", value)
-
-    @property
     @pulumi.getter(name="binaryPath")
     def binary_path(self) -> Optional[pulumi.Input[str]]:
         """
         Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         """
         return pulumi.get(self, "binary_path")
 
     @binary_path.setter
     def binary_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "binary_path", value)
 
     @property
-    @pulumi.getter(name="directoryPrefix")
-    def directory_prefix(self) -> Optional[pulumi.Input[str]]:
-        """
-        The  directory prefix is the directory where all other files and subdirectories will be saved to, i.e. the top of the retrieval tree.  The default is . (the current directory).
-        """
-        return pulumi.get(self, "directory_prefix")
-
-    @directory_prefix.setter
-    def directory_prefix(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "directory_prefix", value)
-
-    @property
     @pulumi.getter
-    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+    def create(self) -> Optional['SedOptsArgs']:
         """
-        Environment variables
+        The command to run on create.
         """
-        return pulumi.get(self, "environment")
+        return pulumi.get(self, "create")
 
-    @environment.setter
-    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
-        pulumi.set(self, "environment", value)
-
-    @property
-    @pulumi.getter(name="httpsOnly")
-    def https_only(self) -> Optional[pulumi.Input[bool]]:
-        """
-        When in recursive mode, only HTTPS links are followed.
-        """
-        return pulumi.get(self, "https_only")
-
-    @https_only.setter
-    def https_only(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "https_only", value)
+    @create.setter
+    def create(self, value: Optional['SedOptsArgs']):
+        pulumi.set(self, "create", value)
 
     @property
     @pulumi.getter
-    def lifecycle(self) -> Optional['CommandLifecycle']:
-        """
-        At what stage(s) in the resource lifecycle should the command be run
-        """
-        return pulumi.get(self, "lifecycle")
-
-    @lifecycle.setter
-    def lifecycle(self, value: Optional['CommandLifecycle']):
-        pulumi.set(self, "lifecycle", value)
-
-    @property
-    @pulumi.getter(name="noVerbose")
-    def no_verbose(self) -> Optional[pulumi.Input[bool]]:
+    def delete(self) -> Optional['SedOptsArgs']:
         """
-        Turn off verbose without being completely quiet (use -q for that), which means that error messages and basic information still get printed.
+        The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+        Command resource from previous create or update steps.
         """
-        return pulumi.get(self, "no_verbose")
+        return pulumi.get(self, "delete")
 
-    @no_verbose.setter
-    def no_verbose(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "no_verbose", value)
-
-    @property
-    @pulumi.getter(name="outputDocument")
-    def output_document(self) -> Optional[pulumi.Input[str]]:
-        """
-        The  documents  will  not  be  written  to the appropriate files, but all will be concatenated together and written to file.
-        """
-        return pulumi.get(self, "output_document")
-
-    @output_document.setter
-    def output_document(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "output_document", value)
+    @delete.setter
+    def delete(self, value: Optional['SedOptsArgs']):
+        pulumi.set(self, "delete", value)
 
     @property
     @pulumi.getter
-    def quiet(self) -> Optional[pulumi.Input[bool]]:
+    def environment(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Turn off Wget's output.
+        Environment variables
         """
-        return pulumi.get(self, "quiet")
+        return pulumi.get(self, "environment")
 
-    @quiet.setter
-    def quiet(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "quiet", value)
+    @environment.setter
+    def environment(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "environment", value)
 
     @property
     @pulumi.getter
     def stdin(self) -> Optional[pulumi.Input[str]]:
         """
         TODO
         """
@@ -200,145 +129,131 @@
 
     @stdin.setter
     def stdin(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "stdin", value)
 
     @property
     @pulumi.getter
-    def timestamping(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Turn on time-stamping.
-        """
-        return pulumi.get(self, "timestamping")
-
-    @timestamping.setter
-    def timestamping(self, value: Optional[pulumi.Input[bool]]):
-        pulumi.set(self, "timestamping", value)
-
-    @property
-    @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Sequence[Any]]]:
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Sequence[Any]]]):
         pulumi.set(self, "triggers", value)
 
+    @property
+    @pulumi.getter
+    def update(self) -> Optional['SedOptsArgs']:
+        """
+        The command to run on update, if empty, create will 
+        run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+        are set to the stdout and stderr properties of the Command resource from previous 
+        create or update steps.
+        """
+        return pulumi.get(self, "update")
+
+    @update.setter
+    def update(self, value: Optional['SedOptsArgs']):
+        pulumi.set(self, "update", value)
+
 
-class Wget(pulumi.ComponentResource):
+class Sed(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 directory_prefix: Optional[pulumi.Input[str]] = None,
+                 create: Optional[pulumi.InputType['SedOptsArgs']] = None,
+                 delete: Optional[pulumi.InputType['SedOptsArgs']] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 https_only: Optional[pulumi.Input[bool]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 no_verbose: Optional[pulumi.Input[bool]] = None,
-                 output_document: Optional[pulumi.Input[str]] = None,
-                 quiet: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
-                 timestamping: Optional[pulumi.Input[bool]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 url: Optional[pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]] = None,
+                 update: Optional[pulumi.InputType['SedOptsArgs']] = None,
                  __props__=None):
         """
-        Abstraction over the `wget` utility on a remote system.
+        Abstraction over the `sed` utility on a remote system.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] binary_path: Path to the binary on the remote system. If omitted, the tool is assumed to be on $PATH
         :param pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']] connection: Connection details for the remote system
-        :param pulumi.Input[str] directory_prefix: The  directory prefix is the directory where all other files and subdirectories will be saved to, i.e. the top of the retrieval tree.  The default is . (the current directory).
+        :param pulumi.InputType['SedOptsArgs'] create: The command to run on create.
+        :param pulumi.InputType['SedOptsArgs'] delete: The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+               and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+               Command resource from previous create or update steps.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] environment: Environment variables
-        :param pulumi.Input[bool] https_only: When in recursive mode, only HTTPS links are followed.
-        :param 'CommandLifecycle' lifecycle: At what stage(s) in the resource lifecycle should the command be run
-        :param pulumi.Input[bool] no_verbose: Turn off verbose without being completely quiet (use -q for that), which means that error messages and basic information still get printed.
-        :param pulumi.Input[str] output_document: The  documents  will  not  be  written  to the appropriate files, but all will be concatenated together and written to file.
-        :param pulumi.Input[bool] quiet: Turn off Wget's output.
         :param pulumi.Input[str] stdin: TODO
-        :param pulumi.Input[bool] timestamping: Turn on time-stamping.
         :param pulumi.Input[Sequence[Any]] triggers: TODO
-        :param pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]] url: Corresponds to the [URL...] argument.
+        :param pulumi.InputType['SedOptsArgs'] update: The command to run on update, if empty, create will 
+               run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+               are set to the stdout and stderr properties of the Command resource from previous 
+               create or update steps.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: WgetArgs,
+                 args: SedArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        Abstraction over the `wget` utility on a remote system.
+        Abstraction over the `sed` utility on a remote system.
 
         :param str resource_name: The name of the resource.
-        :param WgetArgs args: The arguments to use to populate this resource's properties.
+        :param SedArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(WgetArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(SedArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  binary_path: Optional[pulumi.Input[str]] = None,
                  connection: Optional[pulumi.Input[pulumi.InputType['pulumi_command.remote.ConnectionArgs']]] = None,
-                 directory_prefix: Optional[pulumi.Input[str]] = None,
+                 create: Optional[pulumi.InputType['SedOptsArgs']] = None,
+                 delete: Optional[pulumi.InputType['SedOptsArgs']] = None,
                  environment: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
-                 https_only: Optional[pulumi.Input[bool]] = None,
-                 lifecycle: Optional['CommandLifecycle'] = None,
-                 no_verbose: Optional[pulumi.Input[bool]] = None,
-                 output_document: Optional[pulumi.Input[str]] = None,
-                 quiet: Optional[pulumi.Input[bool]] = None,
                  stdin: Optional[pulumi.Input[str]] = None,
-                 timestamping: Optional[pulumi.Input[bool]] = None,
                  triggers: Optional[pulumi.Input[Sequence[Any]]] = None,
-                 url: Optional[pulumi.Input[Union[str, Sequence[pulumi.Input[str]]]]] = None,
+                 update: Optional[pulumi.InputType['SedOptsArgs']] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = WgetArgs.__new__(WgetArgs)
+            __props__ = SedArgs.__new__(SedArgs)
 
             __props__.__dict__["binary_path"] = binary_path
             if connection is None and not opts.urn:
                 raise TypeError("Missing required property 'connection'")
             __props__.__dict__["connection"] = connection
-            __props__.__dict__["directory_prefix"] = directory_prefix
+            __props__.__dict__["create"] = create
+            __props__.__dict__["delete"] = delete
             __props__.__dict__["environment"] = environment
-            __props__.__dict__["https_only"] = https_only
-            __props__.__dict__["lifecycle"] = lifecycle
-            __props__.__dict__["no_verbose"] = no_verbose
-            __props__.__dict__["output_document"] = output_document
-            __props__.__dict__["quiet"] = quiet
             __props__.__dict__["stdin"] = stdin
-            __props__.__dict__["timestamping"] = timestamping
             __props__.__dict__["triggers"] = triggers
-            if url is None and not opts.urn:
-                raise TypeError("Missing required property 'url'")
-            __props__.__dict__["url"] = url
+            __props__.__dict__["update"] = update
             __props__.__dict__["command"] = None
             __props__.__dict__["stderr"] = None
             __props__.__dict__["stdout"] = None
-        super(Wget, __self__).__init__(
-            'kubernetes-the-hard-way:tools:Wget',
+        super(Sed, __self__).__init__(
+            'kubernetes-the-hard-way:tools:Sed',
             resource_name,
             __props__,
             opts,
             remote=True)
 
     @property
     @pulumi.getter(name="binaryPath")
@@ -361,68 +276,38 @@
     def connection(self) -> pulumi.Output['pulumi_command.remote.outputs.Connection']:
         """
         Connection details for the remote system
         """
         return pulumi.get(self, "connection")
 
     @property
-    @pulumi.getter(name="directoryPrefix")
-    def directory_prefix(self) -> pulumi.Output[Optional[str]]:
-        """
-        The  directory prefix is the directory where all other files and subdirectories will be saved to, i.e. the top of the retrieval tree.  The default is . (the current directory).
-        """
-        return pulumi.get(self, "directory_prefix")
-
-    @property
     @pulumi.getter
-    def environment(self) -> pulumi.Output[Mapping[str, str]]:
+    def create(self) -> pulumi.Output[Optional['outputs.SedOpts']]:
         """
-        Environment variables
+        The command to run on create.
         """
-        return pulumi.get(self, "environment")
-
-    @property
-    @pulumi.getter(name="httpsOnly")
-    def https_only(self) -> pulumi.Output[bool]:
-        """
-        When in recursive mode, only HTTPS links are followed.
-        """
-        return pulumi.get(self, "https_only")
+        return pulumi.get(self, "create")
 
     @property
     @pulumi.getter
-    def lifecycle(self) -> pulumi.Output[Optional['CommandLifecycle']]:
-        """
-        At what stage(s) in the resource lifecycle should the command be run
-        """
-        return pulumi.get(self, "lifecycle")
-
-    @property
-    @pulumi.getter(name="noVerbose")
-    def no_verbose(self) -> pulumi.Output[bool]:
+    def delete(self) -> pulumi.Output[Optional['outputs.SedOpts']]:
         """
-        Turn off verbose without being completely quiet (use -q for that), which means that error messages and basic information still get printed.
+        The command to run on delete. The environment variables PULUMI_COMMAND_STDOUT
+        and PULUMI_COMMAND_STDERR are set to the stdout and stderr properties of the
+        Command resource from previous create or update steps.
         """
-        return pulumi.get(self, "no_verbose")
-
-    @property
-    @pulumi.getter(name="outputDocument")
-    def output_document(self) -> pulumi.Output[Optional[str]]:
-        """
-        The  documents  will  not  be  written  to the appropriate files, but all will be concatenated together and written to file.
-        """
-        return pulumi.get(self, "output_document")
+        return pulumi.get(self, "delete")
 
     @property
     @pulumi.getter
-    def quiet(self) -> pulumi.Output[bool]:
+    def environment(self) -> pulumi.Output[Mapping[str, str]]:
         """
-        Turn off Wget's output.
+        Environment variables
         """
-        return pulumi.get(self, "quiet")
+        return pulumi.get(self, "environment")
 
     @property
     @pulumi.getter
     def stderr(self) -> pulumi.Output[str]:
         """
         TODO
         """
@@ -442,29 +327,24 @@
         """
         TODO
         """
         return pulumi.get(self, "stdout")
 
     @property
     @pulumi.getter
-    def timestamping(self) -> pulumi.Output[bool]:
-        """
-        Turn on time-stamping.
-        """
-        return pulumi.get(self, "timestamping")
-
-    @property
-    @pulumi.getter
     def triggers(self) -> pulumi.Output[Sequence[Any]]:
         """
         TODO
         """
         return pulumi.get(self, "triggers")
 
     @property
     @pulumi.getter
-    def url(self) -> pulumi.Output[Any]:
+    def update(self) -> pulumi.Output[Optional['outputs.SedOpts']]:
         """
-        Corresponds to the [URL...] argument.
+        The command to run on update, if empty, create will 
+        run again. The environment variables PULUMI_COMMAND_STDOUT and PULUMI_COMMAND_STDERR 
+        are set to the stdout and stderr properties of the Command resource from previous 
+        create or update steps.
         """
-        return pulumi.get(self, "url")
+        return pulumi.get(self, "update")
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.18a1713567560
+Version: 0.0.18a1713670785
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -47,20 +47,22 @@
 pulumi_kubernetes_the_hard_way/tls/certificate.py
 pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
 pulumi_kubernetes_the_hard_way/tls/encryption_key.py
 pulumi_kubernetes_the_hard_way/tls/outputs.py
 pulumi_kubernetes_the_hard_way/tls/root_ca.py
 pulumi_kubernetes_the_hard_way/tools/__init__.py
 pulumi_kubernetes_the_hard_way/tools/_enums.py
+pulumi_kubernetes_the_hard_way/tools/_inputs.py
 pulumi_kubernetes_the_hard_way/tools/chmod.py
 pulumi_kubernetes_the_hard_way/tools/curl.py
 pulumi_kubernetes_the_hard_way/tools/etcdctl.py
 pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
 pulumi_kubernetes_the_hard_way/tools/mkdir.py
 pulumi_kubernetes_the_hard_way/tools/mktemp.py
 pulumi_kubernetes_the_hard_way/tools/mv.py
+pulumi_kubernetes_the_hard_way/tools/outputs.py
 pulumi_kubernetes_the_hard_way/tools/rm.py
 pulumi_kubernetes_the_hard_way/tools/sed.py
 pulumi_kubernetes_the_hard_way/tools/systemctl.py
 pulumi_kubernetes_the_hard_way/tools/tar.py
 pulumi_kubernetes_the_hard_way/tools/tee.py
 pulumi_kubernetes_the_hard_way/tools/wget.py
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713567560/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.18a1713670785/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.10.0,<1.0.0", "pulumi-kubernetes>=4.11.0,<5.0.0", "pulumi-random>=4.16.1,<5.0.0", "pulumi-tls>=5.0.2,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.18a1713567560"
+  version = "0.0.18a1713670785"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

