# Comparing `tmp/IPFS-Toolkit-0.5.8.tar.gz` & `tmp/IPFS-Toolkit-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IPFS-Toolkit-0.5.8.tar", last modified: Tue May  2 15:09:45 2023, max compression
+gzip compressed data, was "IPFS-Toolkit-0.5.9.tar", last modified: Tue May  2 15:43:48 2023, max compression
```

## Comparing `IPFS-Toolkit-0.5.8.tar` & `IPFS-Toolkit-0.5.9.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-02 15:09:45.704021 IPFS-Toolkit-0.5.8/
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7983 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.8/IPFS_API.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    12925 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.8/IPFS_DataTransmission.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1368 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.8/IPFS_LNS.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-02 15:09:45.692021 IPFS-Toolkit-0.5.8/IPFS_Toolkit.egg-info/
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)    12580 2023-05-02 15:09:44.000000 IPFS-Toolkit-0.5.8/IPFS_Toolkit.egg-info/PKG-INFO
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)     1357 2023-05-02 15:09:45.000000 IPFS-Toolkit-0.5.8/IPFS_Toolkit.egg-info/SOURCES.txt
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)        1 2023-05-02 15:09:44.000000 IPFS-Toolkit-0.5.8/IPFS_Toolkit.egg-info/dependency_links.txt
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)       64 2023-05-02 15:09:45.000000 IPFS-Toolkit-0.5.8/IPFS_Toolkit.egg-info/requires.txt
--rwxrwxrwx   0 llearuin  (1000) llearuin  (1000)      115 2023-05-02 15:09:45.000000 IPFS-Toolkit-0.5.8/IPFS_Toolkit.egg-info/top_level.txt
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    12580 2023-05-02 15:09:45.704021 IPFS-Toolkit-0.5.8/PKG-INFO
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)    19979 2023-05-02 10:39:20.000000 IPFS-Toolkit-0.5.8/ipfs_api.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    14844 2023-04-29 06:24:24.000000 IPFS-Toolkit-0.5.8/ipfs_cli.py
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)    74398 2023-04-29 06:24:24.000000 IPFS-Toolkit-0.5.8/ipfs_datatransmission.py
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     5291 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.8/ipfs_lns.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-02 15:09:45.696020 IPFS-Toolkit-0.5.8/ipfshttpclient2/
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      417 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/__init__.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-02 15:09:45.700021 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    10097 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/__init__.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    12665 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/base.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1755 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/bitswap.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2045 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/block.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1783 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/bootstrap.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2159 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/config.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4665 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/dag.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6294 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/dht.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    14839 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/files.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     3431 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/key.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6230 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/miscellaneous.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4125 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/name.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    11246 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/object.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     3400 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/p2p.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     8698 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/pin.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    10038 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/pubsub.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2366 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/repo.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7484 2023-04-30 17:51:07.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/swarm.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     5684 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/client/unstable.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     7884 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/encoding.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     5622 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/exceptions.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    25493 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/filescanner.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1361 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/http.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    19985 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/http_common.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6139 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/http_httpx.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6600 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/http_requests.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    19796 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/multipart.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     9483 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/requests_wrapper.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4749 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/utils.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      551 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/ipfshttpclient2/version.py
--rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      104 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.8/pyproject.toml
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2023-05-02 15:09:45.704021 IPFS-Toolkit-0.5.8/setup.cfg
--rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     1512 2023-05-02 15:07:02.000000 IPFS-Toolkit-0.5.8/setup.py
-drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-02 15:09:45.704021 IPFS-Toolkit-0.5.8/tests/
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     5311 2023-05-02 10:39:20.000000 IPFS-Toolkit-0.5.8/tests/test_peers.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     5345 2023-04-30 17:45:34.000000 IPFS-Toolkit-0.5.8/tests/test_with_docker.py
--rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1547 2023-04-30 17:46:18.000000 IPFS-Toolkit-0.5.8/tests/test_without_docker.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-02 15:43:48.647237 IPFS-Toolkit-0.5.9/
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7983 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.9/IPFS_API.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    12925 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.9/IPFS_DataTransmission.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1368 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.9/IPFS_LNS.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-02 15:43:48.639237 IPFS-Toolkit-0.5.9/IPFS_Toolkit.egg-info/
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    12580 2023-05-02 15:43:47.000000 IPFS-Toolkit-0.5.9/IPFS_Toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1371 2023-05-02 15:43:48.000000 IPFS-Toolkit-0.5.9/IPFS_Toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)        1 2023-05-02 15:43:47.000000 IPFS-Toolkit-0.5.9/IPFS_Toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       64 2023-05-02 15:43:48.000000 IPFS-Toolkit-0.5.9/IPFS_Toolkit.egg-info/requires.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)      116 2023-05-02 15:43:48.000000 IPFS-Toolkit-0.5.9/IPFS_Toolkit.egg-info/top_level.txt
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    12580 2023-05-02 15:43:48.647237 IPFS-Toolkit-0.5.9/PKG-INFO
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)    19979 2023-05-02 10:39:20.000000 IPFS-Toolkit-0.5.9/ipfs_api.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    14844 2023-04-29 06:24:24.000000 IPFS-Toolkit-0.5.9/ipfs_cli.py
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)    74398 2023-04-29 06:24:24.000000 IPFS-Toolkit-0.5.9/ipfs_datatransmission.py
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     5291 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.9/ipfs_lns.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7638 2023-05-02 15:12:04.000000 IPFS-Toolkit-0.5.9/ipfs_peers.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-02 15:43:48.643236 IPFS-Toolkit-0.5.9/ipfshttpclient2/
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      417 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/__init__.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-02 15:43:48.647237 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    10097 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/__init__.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    12665 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/base.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1755 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/bitswap.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2045 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/block.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1783 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/bootstrap.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2159 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/config.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4665 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/dag.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6294 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/dht.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    14839 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/files.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     3431 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/key.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6230 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/miscellaneous.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4125 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/name.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    11246 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/object.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     3400 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/p2p.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     8698 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/pin.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    10038 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/pubsub.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     2366 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/repo.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     7484 2023-04-30 17:51:07.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/swarm.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     5684 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/client/unstable.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     7884 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/encoding.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     5622 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/exceptions.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    25493 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/filescanner.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     1361 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/http.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)    19985 2023-03-12 08:16:08.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/http_common.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6139 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/http_httpx.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     6600 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/http_requests.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)    19796 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/multipart.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     9483 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/requests_wrapper.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)     4749 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/utils.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      551 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/ipfshttpclient2/version.py
+-rw-rw-rw-   0 llearuin  (1000) llearuin  (1000)      104 2022-08-06 05:04:59.000000 IPFS-Toolkit-0.5.9/pyproject.toml
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)       38 2023-05-02 15:43:48.647237 IPFS-Toolkit-0.5.9/setup.cfg
+-rwxrwxr-x   0 llearuin  (1000) llearuin  (1000)     1513 2023-05-02 15:41:55.000000 IPFS-Toolkit-0.5.9/setup.py
+drwxrwxr-x   0 llearuin  (1000) llearuin  (1000)        0 2023-05-02 15:43:48.647237 IPFS-Toolkit-0.5.9/tests/
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     5311 2023-05-02 10:39:20.000000 IPFS-Toolkit-0.5.9/tests/test_peers.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     5345 2023-04-30 17:45:34.000000 IPFS-Toolkit-0.5.9/tests/test_with_docker.py
+-rw-rw-r--   0 llearuin  (1000) llearuin  (1000)     1547 2023-04-30 17:46:18.000000 IPFS-Toolkit-0.5.9/tests/test_without_docker.py
```

### Comparing `IPFS-Toolkit-0.5.8/IPFS_API.py` & `IPFS-Toolkit-0.5.9/IPFS_API.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/IPFS_DataTransmission.py` & `IPFS-Toolkit-0.5.9/IPFS_DataTransmission.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/IPFS_LNS.py` & `IPFS-Toolkit-0.5.9/IPFS_LNS.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/IPFS_Toolkit.egg-info/PKG-INFO` & `IPFS-Toolkit-0.5.9/IPFS_Toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IPFS-Toolkit
-Version: 0.5.8
+Version: 0.5.9
 Summary: A set of tools  for working with IPFS in Python: a programmer-friendly API wrapper, P2P data-transmission machinery, and accelerated connections to known peers
 Home-page: https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup#IPFS-Toolkit
 Author: emendir
 License: UNKNOWN
 Project-URL: Github, https://github.com/emendir/IPFS-Toolkit-Python
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IPFS-Toolkit-0.5.8/IPFS_Toolkit.egg-info/SOURCES.txt` & `IPFS-Toolkit-0.5.9/IPFS_Toolkit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 IPFS_API.py
 IPFS_DataTransmission.py
 IPFS_LNS.py
 ipfs_api.py
 ipfs_cli.py
 ipfs_datatransmission.py
 ipfs_lns.py
+ipfs_peers.py
 pyproject.toml
 setup.py
 IPFS_Toolkit.egg-info/PKG-INFO
 IPFS_Toolkit.egg-info/SOURCES.txt
 IPFS_Toolkit.egg-info/dependency_links.txt
 IPFS_Toolkit.egg-info/requires.txt
 IPFS_Toolkit.egg-info/top_level.txt
```

### Comparing `IPFS-Toolkit-0.5.8/PKG-INFO` & `IPFS-Toolkit-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IPFS-Toolkit
-Version: 0.5.8
+Version: 0.5.9
 Summary: A set of tools  for working with IPFS in Python: a programmer-friendly API wrapper, P2P data-transmission machinery, and accelerated connections to known peers
 Home-page: https://ipfs.io/ipns/k2k4r8nismm5mmgrox2fci816xvj4l4cudnuc55gkfoealjuiaexbsup#IPFS-Toolkit
 Author: emendir
 License: UNKNOWN
 Project-URL: Github, https://github.com/emendir/IPFS-Toolkit-Python
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `IPFS-Toolkit-0.5.8/ipfs_api.py` & `IPFS-Toolkit-0.5.9/ipfs_api.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfs_cli.py` & `IPFS-Toolkit-0.5.9/ipfs_cli.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfs_datatransmission.py` & `IPFS-Toolkit-0.5.9/ipfs_datatransmission.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfs_lns.py` & `IPFS-Toolkit-0.5.9/ipfs_lns.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/__init__.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/__init__.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/base.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/base.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/bitswap.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/bitswap.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/block.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/block.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/bootstrap.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/bootstrap.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/config.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/config.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/dag.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/dag.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/dht.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/dht.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/files.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/files.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/key.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/key.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/miscellaneous.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/name.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/name.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/object.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/object.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/p2p.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/p2p.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/pin.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/pin.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/pubsub.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/pubsub.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/repo.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/repo.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/swarm.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/swarm.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/client/unstable.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/client/unstable.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/encoding.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/encoding.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/exceptions.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/exceptions.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/filescanner.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/filescanner.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/http.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/http.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/http_common.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/http_common.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/http_httpx.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/http_httpx.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/http_requests.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/http_requests.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/multipart.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/multipart.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/requests_wrapper.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/requests_wrapper.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/utils.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/utils.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/ipfshttpclient2/version.py` & `IPFS-Toolkit-0.5.9/ipfshttpclient2/version.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/setup.py` & `IPFS-Toolkit-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,13 +23,13 @@
         "Github": "https://github.com/emendir/IPFS-Toolkit-Python",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     py_modules=['ipfs_api', 'ipfs_datatransmission', 'ipfs_lns',
-                'ipfs_cli', 'ipfs_peers' 'IPFS_API', 'IPFS_LNS', 'IPFS_DataTransmission'],
+                'ipfs_cli', 'ipfs_peers', 'IPFS_API', 'IPFS_LNS', 'IPFS_DataTransmission'],
     packages=setuptools.find_packages(),
     python_requires=">=3.6",
     install_requires=['multiaddr', 'appdirs', 'idna',
                       'httpcore', 'httpx', 'requests', 'varint', 'termcolor'],
 )
```

### Comparing `IPFS-Toolkit-0.5.8/tests/test_peers.py` & `IPFS-Toolkit-0.5.9/tests/test_peers.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/tests/test_with_docker.py` & `IPFS-Toolkit-0.5.9/tests/test_with_docker.py`

 * *Files identical despite different names*

### Comparing `IPFS-Toolkit-0.5.8/tests/test_without_docker.py` & `IPFS-Toolkit-0.5.9/tests/test_without_docker.py`

 * *Files identical despite different names*

