# Comparing `tmp/graphlit_client-1.0.20240420004.tar.gz` & `tmp/graphlit_client-1.0.20240420005.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphlit_client-1.0.20240420004.tar", last modified: Sat Apr 20 20:10:35 2024, max compression
+gzip compressed data, was "graphlit_client-1.0.20240420005.tar", last modified: Sat Apr 20 20:58:03 2024, max compression
```

## Comparing `graphlit_client-1.0.20240420004.tar` & `graphlit_client-1.0.20240420005.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 20:10:35.079753 graphlit_client-1.0.20240420004/
--rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-20 20:10:35.079753 graphlit_client-1.0.20240420004/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 20:10:35.063752 graphlit_client-1.0.20240420004/graphlit/
--rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1796 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit/graphlit.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 20:10:35.079753 graphlit_client-1.0.20240420004/graphlit_api/
--rw-r--r--   0 vsts      (1001) docker     (127)    59598 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/add_contents_to_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/async_base_client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/base_model.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/clear_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)    42057 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/client.py
--rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/close_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/create_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/create_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/create_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/create_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/create_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/create_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      984 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/delete_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/delete_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/delete_all_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/delete_all_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/delete_all_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/delete_all_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/delete_all_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/delete_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/delete_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/delete_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/delete_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/delete_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/delete_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/delete_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/delete_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/delete_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/delete_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/delete_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/disable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/disable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/enable_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/enable_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16585 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/enums.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/extract_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/get_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/get_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7230 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/get_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4014 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/get_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7138 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/get_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/get_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4461 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/get_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7887 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/get_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)      677 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/ingest_encoded_file.py
--rw-r--r--   0 vsts      (1001) docker     (127)      606 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/ingest_text.py
--rw-r--r--   0 vsts      (1001) docker     (127)      598 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/ingest_uri.py
--rw-r--r--   0 vsts      (1001) docker     (127)    68146 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/input_types.py
--rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/is_content_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/is_feed_done.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/lookup_credits.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1568 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/lookup_usage.py
--rw-r--r--   0 vsts      (1001) docker     (127)    39275 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/operations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3242 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/prompt_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2055 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/prompt_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/publish_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/publish_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/query_alerts.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/query_collections.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1112 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/query_content_facets.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7934 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/query_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4623 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/query_conversations.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7942 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/query_feeds.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4912 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/query_specifications.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8865 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/query_workflows.py
--rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/remove_contents_from_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/suggest_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/summarize_contents.py
--rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/update_alert.py
--rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/update_collection.py
--rw-r--r--   0 vsts      (1001) docker     (127)      644 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/update_content.py
--rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/update_conversation.py
--rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/update_feed.py
--rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/update_project.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/update_specification.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/update_workflow.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1482 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/graphlit_api/usage.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 20:10:35.079753 graphlit_client-1.0.20240420004/graphlit_client.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-20 20:10:35.000000 graphlit_client-1.0.20240420004/graphlit_client.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     2831 2024-04-20 20:10:35.000000 graphlit_client-1.0.20240420004/graphlit_client.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-20 20:10:35.000000 graphlit_client-1.0.20240420004/graphlit_client.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-20 20:10:35.000000 graphlit_client-1.0.20240420004/graphlit_client.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-20 20:10:35.000000 graphlit_client-1.0.20240420004/graphlit_client.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      299 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-20 20:10:35.079753 graphlit_client-1.0.20240420004/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-04-20 20:10:16.000000 graphlit_client-1.0.20240420004/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 20:58:03.178585 graphlit_client-1.0.20240420005/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1095 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-20 20:58:03.178585 graphlit_client-1.0.20240420005/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2321 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 20:58:03.162585 graphlit_client-1.0.20240420005/graphlit/
+-rw-r--r--   0 vsts      (1001) docker     (127)       32 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1796 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit/graphlit.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 20:58:03.178585 graphlit_client-1.0.20240420005/graphlit_api/
+-rw-r--r--   0 vsts      (1001) docker     (127)    59598 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      888 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/add_contents_to_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12578 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/async_base_client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      620 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/base_model.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/clear_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    42432 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/client.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      531 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/close_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/create_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/create_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/create_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/create_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/create_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/create_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      984 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/delete_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      442 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/delete_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      469 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/delete_all_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/delete_all_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      523 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/delete_all_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/delete_all_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      491 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/delete_all_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      452 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/delete_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      482 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/delete_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      428 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/delete_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/delete_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/delete_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      498 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/delete_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/delete_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      434 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/delete_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      476 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/delete_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      436 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/delete_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      468 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/delete_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      406 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/disable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/disable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      398 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/enable_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/enable_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16585 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/enums.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2411 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      957 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/extract_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3609 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/get_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      799 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/get_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7230 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/get_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4014 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/get_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7138 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/get_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1269 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/get_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4461 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/get_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7887 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/get_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      677 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/ingest_encoded_file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      606 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/ingest_text.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      598 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/ingest_uri.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    68146 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/input_types.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      390 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/is_content_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      352 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/is_feed_done.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/lookup_credits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1568 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/lookup_usage.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    39482 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/operations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3242 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/prompt_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2055 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/prompt_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      796 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/publish_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      828 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/publish_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4196 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/query_alerts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1044 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/query_collections.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1112 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/query_content_facets.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7934 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/query_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4623 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/query_conversations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7942 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/query_feeds.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4912 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/query_specifications.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8865 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/query_workflows.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      950 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/remove_contents_from_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      459 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/suggest_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1096 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/summarize_contents.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      445 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/update_alert.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      519 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/update_collection.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      644 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/update_content.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      539 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/update_conversation.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      435 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/update_feed.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      388 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/update_project.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/update_specification.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8453 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/update_workflow.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1482 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/graphlit_api/usage.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-20 20:58:03.178585 graphlit_client-1.0.20240420005/graphlit_client.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2675 2024-04-20 20:58:03.000000 graphlit_client-1.0.20240420005/graphlit_client.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     2831 2024-04-20 20:58:03.000000 graphlit_client-1.0.20240420005/graphlit_client.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-20 20:58:03.000000 graphlit_client-1.0.20240420005/graphlit_client.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       46 2024-04-20 20:58:03.000000 graphlit_client-1.0.20240420005/graphlit_client.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       22 2024-04-20 20:58:03.000000 graphlit_client-1.0.20240420005/graphlit_client.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      299 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-20 20:58:03.178585 graphlit_client-1.0.20240420005/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      766 2024-04-20 20:57:48.000000 graphlit_client-1.0.20240420005/setup.py
```

### Comparing `graphlit_client-1.0.20240420004/LICENSE` & `graphlit_client-1.0.20240420005/LICENSE`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/PKG-INFO` & `graphlit_client-1.0.20240420005/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240420004
+Version: 1.0.20240420005
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240420004/README.md` & `graphlit_client-1.0.20240420005/README.md`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit/graphlit.py` & `graphlit_client-1.0.20240420005/graphlit/graphlit.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/__init__.py` & `graphlit_client-1.0.20240420005/graphlit_api/__init__.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/add_contents_to_collections.py` & `graphlit_client-1.0.20240420005/graphlit_api/add_contents_to_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/async_base_client.py` & `graphlit_client-1.0.20240420005/graphlit_api/async_base_client.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/base_model.py` & `graphlit_client-1.0.20240420005/graphlit_api/base_model.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/clear_conversation.py` & `graphlit_client-1.0.20240420005/graphlit_api/clear_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/client.py` & `graphlit_client-1.0.20240420005/graphlit_api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -473,24 +473,26 @@
     async def ingest_encoded_file(
         self,
         name: str,
         data: str,
         mime_type: str,
         id: Union[Optional[str], UnsetType] = UNSET,
         is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        collections: Union[Optional[List[EntityReferenceInput]], UnsetType] = UNSET,
         workflow: Union[Optional[EntityReferenceInput], UnsetType] = UNSET,
         correlation_id: Union[Optional[str], UnsetType] = UNSET,
         **kwargs: Any
     ) -> IngestEncodedFile:
         variables: Dict[str, object] = {
             "name": name,
             "data": data,
             "mimeType": mime_type,
             "id": id,
             "isSynchronous": is_synchronous,
+            "collections": collections,
             "workflow": workflow,
             "correlationId": correlation_id,
         }
         response = await self.execute(
             query=INGEST_ENCODED_FILE_GQL,
             operation_name="IngestEncodedFile",
             variables=variables,
@@ -503,25 +505,27 @@
         self,
         name: str,
         text: str,
         text_type: Union[Optional[TextTypes], UnsetType] = UNSET,
         uri: Union[Optional[Any], UnsetType] = UNSET,
         id: Union[Optional[str], UnsetType] = UNSET,
         is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        collections: Union[Optional[List[EntityReferenceInput]], UnsetType] = UNSET,
         workflow: Union[Optional[EntityReferenceInput], UnsetType] = UNSET,
         correlation_id: Union[Optional[str], UnsetType] = UNSET,
         **kwargs: Any
     ) -> IngestText:
         variables: Dict[str, object] = {
             "name": name,
             "text": text,
             "textType": text_type,
             "uri": uri,
             "id": id,
             "isSynchronous": is_synchronous,
+            "collections": collections,
             "workflow": workflow,
             "correlationId": correlation_id,
         }
         response = await self.execute(
             query=INGEST_TEXT_GQL,
             operation_name="IngestText",
             variables=variables,
@@ -532,23 +536,25 @@
 
     async def ingest_uri(
         self,
         uri: Any,
         name: Union[Optional[str], UnsetType] = UNSET,
         id: Union[Optional[str], UnsetType] = UNSET,
         is_synchronous: Union[Optional[bool], UnsetType] = UNSET,
+        collections: Union[Optional[List[EntityReferenceInput]], UnsetType] = UNSET,
         workflow: Union[Optional[EntityReferenceInput], UnsetType] = UNSET,
         correlation_id: Union[Optional[str], UnsetType] = UNSET,
         **kwargs: Any
     ) -> IngestUri:
         variables: Dict[str, object] = {
             "name": name,
             "uri": uri,
             "id": id,
             "isSynchronous": is_synchronous,
+            "collections": collections,
             "workflow": workflow,
             "correlationId": correlation_id,
         }
         response = await self.execute(
             query=INGEST_URI_GQL,
             operation_name="IngestUri",
             variables=variables,
```

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/close_conversation.py` & `graphlit_client-1.0.20240420005/graphlit_api/close_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/create_collection.py` & `graphlit_client-1.0.20240420005/graphlit_api/create_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/create_conversation.py` & `graphlit_client-1.0.20240420005/graphlit_api/create_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/create_specification.py` & `graphlit_client-1.0.20240420005/graphlit_api/create_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/create_workflow.py` & `graphlit_client-1.0.20240420005/graphlit_api/create_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/credits.py` & `graphlit_client-1.0.20240420005/graphlit_api/credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/delete_all_conversations.py` & `graphlit_client-1.0.20240420005/graphlit_api/delete_all_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/enums.py` & `graphlit_client-1.0.20240420005/graphlit_api/enums.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/exceptions.py` & `graphlit_client-1.0.20240420005/graphlit_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/extract_contents.py` & `graphlit_client-1.0.20240420005/graphlit_api/extract_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/get_alert.py` & `graphlit_client-1.0.20240420005/graphlit_api/get_alert.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/get_collection.py` & `graphlit_client-1.0.20240420005/graphlit_api/get_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/get_content.py` & `graphlit_client-1.0.20240420005/graphlit_api/get_content.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/get_conversation.py` & `graphlit_client-1.0.20240420005/graphlit_api/get_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/get_feed.py` & `graphlit_client-1.0.20240420005/graphlit_api/get_feed.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/get_project.py` & `graphlit_client-1.0.20240420005/graphlit_api/get_project.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/get_specification.py` & `graphlit_client-1.0.20240420005/graphlit_api/get_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/get_workflow.py` & `graphlit_client-1.0.20240420005/graphlit_api/get_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/ingest_encoded_file.py` & `graphlit_client-1.0.20240420005/graphlit_api/ingest_encoded_file.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/ingest_text.py` & `graphlit_client-1.0.20240420005/graphlit_api/ingest_text.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/ingest_uri.py` & `graphlit_client-1.0.20240420005/graphlit_api/ingest_uri.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/input_types.py` & `graphlit_client-1.0.20240420005/graphlit_api/input_types.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/lookup_credits.py` & `graphlit_client-1.0.20240420005/graphlit_api/lookup_credits.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/lookup_usage.py` & `graphlit_client-1.0.20240420005/graphlit_api/lookup_usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/operations.py` & `graphlit_client-1.0.20240420005/graphlit_api/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -609,21 +609,22 @@
     }
     error
   }
 }
 """
 
 INGEST_ENCODED_FILE_GQL = """
-mutation IngestEncodedFile($name: String!, $data: String!, $mimeType: String!, $id: ID, $isSynchronous: Boolean, $workflow: EntityReferenceInput, $correlationId: String) {
+mutation IngestEncodedFile($name: String!, $data: String!, $mimeType: String!, $id: ID, $isSynchronous: Boolean, $collections: [EntityReferenceInput!], $workflow: EntityReferenceInput, $correlationId: String) {
   ingestEncodedFile(
     name: $name
     data: $data
     mimeType: $mimeType
     id: $id
     isSynchronous: $isSynchronous
+    collections: $collections
     workflow: $workflow
     correlationId: $correlationId
   ) {
     id
     name
     state
     type
@@ -631,22 +632,23 @@
     mimeType
     uri
   }
 }
 """
 
 INGEST_TEXT_GQL = """
-mutation IngestText($name: String!, $text: String!, $textType: TextTypes, $uri: URL, $id: ID, $isSynchronous: Boolean, $workflow: EntityReferenceInput, $correlationId: String) {
+mutation IngestText($name: String!, $text: String!, $textType: TextTypes, $uri: URL, $id: ID, $isSynchronous: Boolean, $collections: [EntityReferenceInput!], $workflow: EntityReferenceInput, $correlationId: String) {
   ingestText(
     name: $name
     text: $text
     textType: $textType
     uri: $uri
     id: $id
     isSynchronous: $isSynchronous
+    collections: $collections
     workflow: $workflow
     correlationId: $correlationId
   ) {
     id
     name
     state
     type
@@ -654,19 +656,20 @@
     mimeType
     uri
   }
 }
 """
 
 INGEST_URI_GQL = """
-mutation IngestUri($name: String, $uri: URL!, $id: ID, $isSynchronous: Boolean, $workflow: EntityReferenceInput, $correlationId: String) {
+mutation IngestUri($name: String, $uri: URL!, $id: ID, $isSynchronous: Boolean, $collections: [EntityReferenceInput!], $workflow: EntityReferenceInput, $correlationId: String) {
   ingestUri(
     name: $name
     uri: $uri
     id: $id
+    collections: $collections
     workflow: $workflow
     isSynchronous: $isSynchronous
     correlationId: $correlationId
   ) {
     id
     name
     state
```

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/prompt_conversation.py` & `graphlit_client-1.0.20240420005/graphlit_api/prompt_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/prompt_specifications.py` & `graphlit_client-1.0.20240420005/graphlit_api/prompt_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/publish_contents.py` & `graphlit_client-1.0.20240420005/graphlit_api/publish_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/publish_conversation.py` & `graphlit_client-1.0.20240420005/graphlit_api/publish_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/query_alerts.py` & `graphlit_client-1.0.20240420005/graphlit_api/query_alerts.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/query_collections.py` & `graphlit_client-1.0.20240420005/graphlit_api/query_collections.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/query_content_facets.py` & `graphlit_client-1.0.20240420005/graphlit_api/query_content_facets.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/query_contents.py` & `graphlit_client-1.0.20240420005/graphlit_api/query_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/query_conversations.py` & `graphlit_client-1.0.20240420005/graphlit_api/query_conversations.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/query_feeds.py` & `graphlit_client-1.0.20240420005/graphlit_api/query_feeds.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/query_specifications.py` & `graphlit_client-1.0.20240420005/graphlit_api/query_specifications.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/query_workflows.py` & `graphlit_client-1.0.20240420005/graphlit_api/query_workflows.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/remove_contents_from_collection.py` & `graphlit_client-1.0.20240420005/graphlit_api/remove_contents_from_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/summarize_contents.py` & `graphlit_client-1.0.20240420005/graphlit_api/summarize_contents.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/update_collection.py` & `graphlit_client-1.0.20240420005/graphlit_api/update_collection.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/update_content.py` & `graphlit_client-1.0.20240420005/graphlit_api/update_content.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/update_conversation.py` & `graphlit_client-1.0.20240420005/graphlit_api/update_conversation.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/update_specification.py` & `graphlit_client-1.0.20240420005/graphlit_api/update_specification.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/update_workflow.py` & `graphlit_client-1.0.20240420005/graphlit_api/update_workflow.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_api/usage.py` & `graphlit_client-1.0.20240420005/graphlit_api/usage.py`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/graphlit_client.egg-info/PKG-INFO` & `graphlit_client-1.0.20240420005/graphlit_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlit-client
-Version: 1.0.20240420004
+Version: 1.0.20240420005
 Summary: Graphlit API Python Client
 Home-page: https://github.com/graphlit/graphlit-client-python
 Author: Unstruk Data Inc.
 Author-email: questions@graphlit.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `graphlit_client-1.0.20240420004/graphlit_client.egg-info/SOURCES.txt` & `graphlit_client-1.0.20240420005/graphlit_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphlit_client-1.0.20240420004/setup.py` & `graphlit_client-1.0.20240420005/setup.py`

 * *Files identical despite different names*

