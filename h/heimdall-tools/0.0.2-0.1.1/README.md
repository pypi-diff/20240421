# Comparing `tmp/heimdall_tools-0.0.2.tar.gz` & `tmp/heimdall_tools-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heimdall_tools-0.0.2.tar", last modified: Mon Apr  8 15:40:50 2024, max compression
+gzip compressed data, was "heimdall_tools-0.1.1.tar", last modified: Sun Apr 21 16:47:51 2024, max compression
```

## Comparing `heimdall_tools-0.0.2.tar` & `heimdall_tools-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 pediashops  (1000) pediashops  (1000)        0 2024-04-08 15:40:50.541019 heimdall_tools-0.0.2/
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)      188 2024-04-08 15:40:50.541019 heimdall_tools-0.0.2/PKG-INFO
-drwxr-xr-x   0 pediashops  (1000) pediashops  (1000)        0 2024-04-08 15:40:50.529957 heimdall_tools-0.0.2/heimdall_tools/
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)      121 2024-04-08 13:34:54.000000 heimdall_tools-0.0.2/heimdall_tools/__init__.py
--rwxr-xr-x   0 pediashops  (1000) pediashops  (1000)      806 2024-04-08 11:55:43.000000 heimdall_tools-0.0.2/heimdall_tools/sns.py
--rwxrwxrwx   0 pediashops  (1000) pediashops  (1000)     1252 2024-04-08 15:38:34.000000 heimdall_tools-0.0.2/heimdall_tools/sqs.py
-drwxr-xr-x   0 pediashops  (1000) pediashops  (1000)        0 2024-04-08 15:40:50.541019 heimdall_tools-0.0.2/heimdall_tools.egg-info/
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)      188 2024-04-08 15:40:49.000000 heimdall_tools-0.0.2/heimdall_tools.egg-info/PKG-INFO
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)      268 2024-04-08 15:40:50.000000 heimdall_tools-0.0.2/heimdall_tools.egg-info/SOURCES.txt
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)        1 2024-04-08 15:40:49.000000 heimdall_tools-0.0.2/heimdall_tools.egg-info/dependency_links.txt
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)        6 2024-04-08 15:40:49.000000 heimdall_tools-0.0.2/heimdall_tools.egg-info/requires.txt
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)       15 2024-04-08 15:40:49.000000 heimdall_tools-0.0.2/heimdall_tools.egg-info/top_level.txt
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)       38 2024-04-08 15:40:50.541019 heimdall_tools-0.0.2/setup.cfg
--rw-r--r--   0 pediashops  (1000) pediashops  (1000)      321 2024-04-08 15:39:07.000000 heimdall_tools-0.0.2/setup.py
+drwxr-xr-x   0 pediashops  (1000) pediashops  (1000)        0 2024-04-21 16:47:51.724446 heimdall_tools-0.1.1/
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)     1143 2024-04-21 16:47:51.724446 heimdall_tools-0.1.1/PKG-INFO
+-rwxrwxrwx   0 pediashops  (1000) pediashops  (1000)      556 2024-04-21 16:39:40.000000 heimdall_tools-0.1.1/README.md
+drwxr-xr-x   0 pediashops  (1000) pediashops  (1000)        0 2024-04-21 16:47:51.700622 heimdall_tools-0.1.1/heimdall_tools/
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)      121 2024-04-08 13:34:54.000000 heimdall_tools-0.1.1/heimdall_tools/__init__.py
+-rwxr-xr-x   0 pediashops  (1000) pediashops  (1000)     2483 2024-04-21 15:43:23.000000 heimdall_tools-0.1.1/heimdall_tools/mysql_client.py
+-rwxr-xr-x   0 pediashops  (1000) pediashops  (1000)      806 2024-04-08 11:55:43.000000 heimdall_tools-0.1.1/heimdall_tools/sns.py
+-rwxrwxrwx   0 pediashops  (1000) pediashops  (1000)     1208 2024-04-11 13:49:12.000000 heimdall_tools-0.1.1/heimdall_tools/sqs.py
+drwxr-xr-x   0 pediashops  (1000) pediashops  (1000)        0 2024-04-21 16:47:51.720373 heimdall_tools-0.1.1/heimdall_tools.egg-info/
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)     1143 2024-04-21 16:47:49.000000 heimdall_tools-0.1.1/heimdall_tools.egg-info/PKG-INFO
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)      309 2024-04-21 16:47:50.000000 heimdall_tools-0.1.1/heimdall_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)        1 2024-04-21 16:47:49.000000 heimdall_tools-0.1.1/heimdall_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)       29 2024-04-21 16:47:49.000000 heimdall_tools-0.1.1/heimdall_tools.egg-info/requires.txt
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)       15 2024-04-21 16:47:49.000000 heimdall_tools-0.1.1/heimdall_tools.egg-info/top_level.txt
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)       38 2024-04-21 16:47:51.724446 heimdall_tools-0.1.1/setup.cfg
+-rw-r--r--   0 pediashops  (1000) pediashops  (1000)      861 2024-04-21 16:47:33.000000 heimdall_tools-0.1.1/setup.py
```

### Comparing `heimdall_tools-0.0.2/heimdall_tools/sns.py` & `heimdall_tools-0.1.1/heimdall_tools/sns.py`

 * *Files identical despite different names*

### Comparing `heimdall_tools-0.0.2/heimdall_tools/sqs.py` & `heimdall_tools-0.1.1/heimdall_tools/sqs.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SQS queue subscribe to this SNS topic to queue the messages for further processing.
 # In the architecture, an HTTP endpoint shall read data from SQS for further processing in most of the cases.
 
 import json
 import boto3
 
 def read_from_sqs_queue(region, queue_url, max_number_messages = 10, timeout_secs = 20, delete_on_read = True):
-    sqs_client = boto3.client('sqs', region_name = region)  # Replace 'your_region' with your AWS region
+    sqs_client = boto3.client('sqs', region_name = region)  
 
     # Receive messages from the queue
     response = sqs_client.receive_message(
         QueueUrl=queue_url,
         MaxNumberOfMessages = max_number_messages,  # Maximum number of messages to retrieve
         WaitTimeSeconds = timeout_secs,      # Long polling: Wait up to 20 seconds for messages
     )
```

