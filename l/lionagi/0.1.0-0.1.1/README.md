# Comparing `tmp/lionagi-0.1.0.tar.gz` & `tmp/lionagi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lionagi-0.1.0.tar", last modified: Wed Apr 10 04:41:42 2024, max compression
+gzip compressed data, was "lionagi-0.1.1.tar", last modified: Sun Apr 21 00:58:00 2024, max compression
```

## Comparing `lionagi-0.1.0.tar` & `lionagi-0.1.1.tar`

### file list

```diff
@@ -1,175 +1,243 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.672225 lionagi-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-10 04:41:26.000000 lionagi-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-04-10 04:41:42.672225 lionagi-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-10 04:41:26.000000 lionagi-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-10 04:41:26.000000 lionagi-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.648225 lionagi-0.1.0/lionagi/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.648225 lionagi-0.1.0/lionagi/core/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.648225 lionagi-0.1.0/lionagi/core/agent/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/agent/base_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.652225 lionagi-0.1.0/lionagi/core/branch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/branch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22168 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/branch/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17989 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/branch/branch.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/branch/executable_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/branch/flow_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11812 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/branch/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.652225 lionagi-0.1.0/lionagi/core/direct/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/cot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/predict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/react.py
--rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/score.py
--rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/select.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/sentiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/direct/vote.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.652225 lionagi-0.1.0/lionagi/core/execute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/execute/base_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8298 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/execute/branch_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/execute/instruction_map_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/execute/structure_executor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.652225 lionagi-0.1.0/lionagi/core/flow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/baseflow.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/mono_chat_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.652225 lionagi-0.1.0/lionagi/core/flow/monoflow/
--rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/monoflow/ReAct.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/monoflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/monoflow/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/monoflow/chat_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     8948 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/monoflow/followup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.656225 lionagi-0.1.0/lionagi/core/flow/polyflow/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/polyflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/flow/polyflow/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.656225 lionagi-0.1.0/lionagi/core/form/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/form/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/form/action_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/form/field_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/form/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/form/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/form/scored_form.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.656225 lionagi-0.1.0/lionagi/core/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    11236 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/data_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/mailbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/signal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11972 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/structure.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/generic/work.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.656225 lionagi-0.1.0/lionagi/core/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/graph/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/core/mail/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/mail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/mail/mail_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/mail/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/core/messages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/messages/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/core/session/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38110 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/session/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/core/tool/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/tool/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)    10667 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/core/tool/tool_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/integrations/bridge/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/integrations/bridge/langchain_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/langchain_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/langchain_/documents.py
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/langchain_/langchain_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/llama_index_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/node_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/textnode.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/integrations/bridge/pydantic_/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/pydantic_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/bridge/pydantic_/pydantic_bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.660225 lionagi-0.1.0/lionagi/integrations/chunker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/chunker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/chunker/chunk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.664225 lionagi-0.1.0/lionagi/integrations/config/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/config/mlx_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/config/oai_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/config/ollama_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/config/openrouter_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.664225 lionagi-0.1.0/lionagi/integrations/loader/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/loader/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/loader/load_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.664225 lionagi-0.1.0/lionagi/integrations/provider/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/provider/litellm.py
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/provider/mistralai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/provider/mlx_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/provider/oai.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/provider/ollama.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/provider/openrouter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/provider/services.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/integrations/provider/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.668225 lionagi-0.1.0/lionagi/libs/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34577 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/ln_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/ln_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    23535 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/ln_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/ln_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    49096 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/ln_func_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    29640 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/ln_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)    25007 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/ln_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/ln_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    17351 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/libs/sys_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.668225 lionagi-0.1.0/lionagi/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.668225 lionagi-0.1.0/lionagi/tests/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.668225 lionagi-0.1.0/lionagi/tests/libs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/libs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/libs/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/libs/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/libs/test_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/libs/test_field_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)    20782 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/libs/test_func_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/libs/test_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/libs/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/libs/test_sys_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.668225 lionagi-0.1.0/lionagi/tests/test_core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/test_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18628 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/test_core/test_base_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/test_core/test_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/test_core/test_chat_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/test_core/test_mail_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/test_core/test_prompts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/test_core/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/test_core/test_session_base_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/tests/test_core/test_tool_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 04:41:26.000000 lionagi-0.1.0/lionagi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 04:41:42.668225 lionagi-0.1.0/lionagi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-04-10 04:41:42.000000 lionagi-0.1.0/lionagi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-10 04:41:42.000000 lionagi-0.1.0/lionagi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 04:41:42.000000 lionagi-0.1.0/lionagi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-10 04:41:42.000000 lionagi-0.1.0/lionagi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-10 04:41:42.000000 lionagi-0.1.0/lionagi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-10 04:41:26.000000 lionagi-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 04:41:42.672225 lionagi-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-10 04:41:26.000000 lionagi-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.141428 lionagi-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-21 00:57:39.000000 lionagi-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-04-21 00:58:00.141428 lionagi-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-21 00:57:39.000000 lionagi-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-21 00:57:39.000000 lionagi-0.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.113428 lionagi-0.1.1/lionagi/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.113428 lionagi-0.1.1/lionagi/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.113428 lionagi-0.1.1/lionagi/core/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/agent/base_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.113428 lionagi-0.1.1/lionagi/core/branch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/branch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22169 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/branch/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18010 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/branch/branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/branch/executable_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/branch/flow_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11813 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/branch/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.117428 lionagi-0.1.1/lionagi/core/direct/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/cot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/predict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4321 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/react.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10332 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6131 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/direct/vote.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.117428 lionagi-0.1.1/lionagi/core/execute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/execute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/execute/base_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/execute/branch_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/execute/instruction_map_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15254 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/execute/neo4j_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12151 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/execute/structure_executor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.117428 lionagi-0.1.1/lionagi/core/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/baseflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/mono_chat_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.117428 lionagi-0.1.1/lionagi/core/flow/monoflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     9585 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/monoflow/ReAct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/monoflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/monoflow/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/monoflow/chat_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8886 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/monoflow/followup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.117428 lionagi-0.1.1/lionagi/core/flow/polyflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/polyflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/flow/polyflow/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.121428 lionagi-0.1.1/lionagi/core/form/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/form/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/form/action_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/form/field_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9926 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/form/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6921 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/form/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/form/scored_form.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.121428 lionagi-0.1.1/lionagi/core/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14011 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11236 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/data_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11972 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/generic/work.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.121428 lionagi-0.1.1/lionagi/core/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/graph/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.121428 lionagi-0.1.1/lionagi/core/mail/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/mail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/mail/mail_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/mail/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.121428 lionagi-0.1.1/lionagi/core/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10577 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/messages/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.125428 lionagi-0.1.1/lionagi/core/session/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38111 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/session/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.125428 lionagi-0.1.1/lionagi/core/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/tool/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10667 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/core/tool/tool_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.125428 lionagi-0.1.1/lionagi/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.125428 lionagi-0.1.1/lionagi/experimental/directive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.125428 lionagi-0.1.1/lionagi/experimental/directive/evaluator/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/evaluator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/evaluator/ast_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8062 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/evaluator/base_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/evaluator/sandbox_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/evaluator/script_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.125428 lionagi-0.1.1/lionagi/experimental/directive/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/parser/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.125428 lionagi-0.1.1/lionagi/experimental/directive/template_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/template_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/directive/template_/base_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.125428 lionagi-0.1.1/lionagi/experimental/tool/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/tool/function_calling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/tool/manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/tool/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/tool/tool_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/tool/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.129428 lionagi-0.1.1/lionagi/experimental/work/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/work/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/work/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/work/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/work/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/work/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/work/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/work/work_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/experimental/work/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.129428 lionagi-0.1.1/lionagi/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.129428 lionagi-0.1.1/lionagi/integrations/bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.129428 lionagi-0.1.1/lionagi/integrations/bridge/autogen_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/autogen_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4055 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/autogen_/autogen_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.129428 lionagi-0.1.1/lionagi/integrations/bridge/langchain_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/langchain_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/langchain_/documents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/langchain_/langchain_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.129428 lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11826 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/get_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/llama_index_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/llama_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/node_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/textnode.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.129428 lionagi-0.1.1/lionagi/integrations/bridge/pydantic_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/pydantic_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/pydantic_/pydantic_bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.129428 lionagi-0.1.1/lionagi/integrations/bridge/transformers_/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/transformers_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/bridge/transformers_/install_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.129428 lionagi-0.1.1/lionagi/integrations/chunker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/chunker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/chunker/chunk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.133428 lionagi-0.1.1/lionagi/integrations/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/config/mlx_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/config/oai_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/config/ollama_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/config/openrouter_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.133428 lionagi-0.1.1/lionagi/integrations/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4559 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/loader/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8338 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/loader/load_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.133428 lionagi-0.1.1/lionagi/integrations/provider/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/provider/litellm.py
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/provider/mistralai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/provider/mlx_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/provider/oai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/provider/ollama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/provider/openrouter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5388 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/provider/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/provider/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.133428 lionagi-0.1.1/lionagi/integrations/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25785 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/storage/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10593 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/storage/storage_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/storage/to_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/integrations/storage/to_excel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.137428 lionagi-0.1.1/lionagi/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34577 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23535 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49096 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_func_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14930 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_knowledge_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29640 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25007 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8404 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/ln_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17353 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/libs/sys_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.137428 lionagi-0.1.1/lionagi/lions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.137428 lionagi-0.1.1/lionagi/lions/coder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/coder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/coder/add_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/coder/base_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/coder/coder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/coder/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.137428 lionagi-0.1.1/lionagi/lions/researcher/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/researcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.137428 lionagi-0.1.1/lionagi/lions/researcher/data_source/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/researcher/data_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/researcher/data_source/finhub_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/researcher/data_source/google_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/researcher/data_source/wiki_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/lions/researcher/data_source/yfinance_.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.137428 lionagi-0.1.1/lionagi/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.137428 lionagi-0.1.1/lionagi/tests/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.141428 lionagi-0.1.1/lionagi/tests/libs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11901 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/test_field_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20782 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/test_func_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13106 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/test_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/libs/test_sys_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.141428 lionagi-0.1.1/lionagi/tests/test_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/test_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18628 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/test_core/test_base_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11712 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/test_core/test_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/test_core/test_chat_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/test_core/test_mail_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/test_core/test_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/test_core/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10619 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/test_core/test_session_base_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/tests/test_core/test_tool_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-21 00:57:39.000000 lionagi-0.1.1/lionagi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 00:58:00.141428 lionagi-0.1.1/lionagi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7926 2024-04-21 00:58:00.000000 lionagi-0.1.1/lionagi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7184 2024-04-21 00:58:00.000000 lionagi-0.1.1/lionagi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 00:58:00.000000 lionagi-0.1.1/lionagi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-21 00:58:00.000000 lionagi-0.1.1/lionagi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-21 00:58:00.000000 lionagi-0.1.1/lionagi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-21 00:57:39.000000 lionagi-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 00:58:00.141428 lionagi-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-21 00:57:39.000000 lionagi-0.1.1/setup.py
```

### Comparing `lionagi-0.1.0/LICENSE` & `lionagi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/PKG-INFO` & `lionagi-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lionagi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Towards automated general intelligence.
 Author: HaiyangLi
 Author-email: Haiyang Li <ocean@lionagi.ai>
 License: MIT License
         
         Copyright (c) 2023 HaiyangLi quantocean.li@gmail.com
```

### Comparing `lionagi-0.1.0/README.md` & `lionagi-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/agent/base_agent.py` & `lionagi-0.1.1/lionagi/core/agent/base_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,29 +15,29 @@
 from lionagi.core.execute.structure_executor import StructureExecutor
 
 
 class BaseAgent(Node):
 
     def __init__(
         self,
-        structure: StructureExecutor,
+        structure: BaseExecutor,
         executable: BaseExecutor,
         output_parser=None,
         **kwargs,
     ) -> None:
         """
         Initializes the BaseAgent instance.
 
         Args:
             structure: The structure of the agent.
             executable_obj: The executable object of the agent.
             output_parser: A function for parsing the agent's output (optional).
         """
         super().__init__()
-        self.structure: StructureExecutor = structure
+        self.structure: BaseExecutor = structure
         self.executable: BaseExecutor = executable
         for v, k in kwargs.items():
             executable.__setattr__(v, k)
         self.start: StartMail = StartMail()
         self.mailManager: MailManager = MailManager(
             [self.structure, self.executable, self.start]
         )
@@ -83,8 +83,7 @@
 
         self.structure.execute_stop = False
         self.executable.execute_stop = False
         self.mailManager.execute_stop = False
 
         if self.output_parser:
             return self.output_parser(self)
-
```

### Comparing `lionagi-0.1.0/lionagi/core/branch/base.py` & `lionagi-0.1.1/lionagi/core/branch/base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -646,8 +646,8 @@
         Returns:
                 A dictionary summarizing the count of messages either by role or sender.
         """
 
         messages = self.messages["sender"] if use_sender else self.messages["role"]
         result = messages.value_counts().to_dict()
         result["total"] = len(self.messages)
-        return result
+        return result
```

### Comparing `lionagi-0.1.0/lionagi/core/branch/branch.py` & `lionagi-0.1.1/lionagi/core/branch/branch.py`

 * *Files 0% similar despite different names*

```diff
@@ -466,8 +466,9 @@
             if convert.to_dict(content)["action_response"].keys() >= {
                 "function",
                 "arguments",
                 "output",
             }:
                 return True
         except Exception:
-            return False
+            return False
+        return False
```

### Comparing `lionagi-0.1.0/lionagi/core/branch/flow_mixin.py` & `lionagi-0.1.1/lionagi/core/branch/flow_mixin.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -89,8 +89,8 @@
             tools=tools,
             max_followup=max_followup,
             auto=auto,
             followup_prompt=followup_prompt,
             output_prompt=output_prompt,
             out=out,
             **kwargs,
-        )
+        )
```

### Comparing `lionagi-0.1.0/lionagi/core/branch/util.py` & `lionagi-0.1.1/lionagi/core/branch/util.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -316,8 +316,8 @@
                         answers.append(nested.nget(content, ["assistant_response"]))
             elif i.role == "user":
                 with contextlib.suppress(Exception):
                     answers.append(nested.nget(content, ["instruction"]))
             else:
                 with contextlib.suppress(Exception):
                     answers.append(nested.nget(content, ["system_info"]))
-        return "\n".join(answers)
+        return "\n".join(answers)
```

### Comparing `lionagi-0.1.0/lionagi/core/direct/cot.py` & `lionagi-0.1.1/lionagi/core/direct/cot.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/direct/plan.py` & `lionagi-0.1.1/lionagi/core/direct/plan.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/direct/predict.py` & `lionagi-0.1.1/lionagi/core/direct/predict.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/direct/react.py` & `lionagi-0.1.1/lionagi/core/direct/react.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/direct/score.py` & `lionagi-0.1.1/lionagi/core/direct/score.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/direct/select.py` & `lionagi-0.1.1/lionagi/core/direct/select.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/direct/utils.py` & `lionagi-0.1.1/lionagi/core/direct/utils.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/direct/vote.py` & `lionagi-0.1.1/lionagi/core/direct/vote.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/execute/base_executor.py` & `lionagi-0.1.1/lionagi/core/execute/base_executor.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,27 +14,24 @@
     )
     pending_outs: deque = Field(
         default_factory=deque, description="The pending outgoing mails."
     )
     execute_stop: bool = Field(
         False, description="A flag indicating whether to stop execution."
     )
-    context: dict | str | None = Field(
+    context: dict | str | list | None = Field(
         None, description="The context buffer for the next instruction."
     )
     execution_responses: list = Field(
         default_factory=list, description="The list of responses."
     )
     context_log: list = Field(default_factory=list, description="The context log.")
     verbose: bool = Field(
         True, description="A flag indicating whether to provide verbose output."
     )
-    execute_stop: bool = Field(
-        False, description="A flag indicating whether to stop execution."
-    )
 
     def send(self, recipient_id: str, category: str, package: Any) -> None:
         """
         Sends a mail to a recipient.
 
         Args:
             recipient_id (str): The ID of the recipient.
```

### Comparing `lionagi-0.1.0/lionagi/core/execute/branch_executor.py` & `lionagi-0.1.1/lionagi/core/execute/branch_executor.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 from lionagi.core.branch.branch import Branch
 from lionagi.core.execute.base_executor import BaseExecutor
 
 
 class BranchExecutor(Branch, BaseExecutor):
 
     async def forward(self) -> None:
+        """
+        Forwards the execution by processing all pending incoming mails in each branch. Depending on the category of the mail,
+        it processes starts, nodes, node lists, conditions, or ends, accordingly executing different functions.
+        """
         for key in list(self.pending_ins.keys()):
             while self.pending_ins[key]:
                 mail = self.pending_ins[key].popleft()
                 if mail.category == "start":
                     self._process_start(mail)
                 elif mail.category == "node":
                     await self._process_node(mail)
@@ -22,19 +26,35 @@
                     self._process_node_list(mail)
                 elif mail.category == "condition":
                     self._process_condition(mail)
                 elif mail.category == "end":
                     self._process_end(mail)
 
     async def execute(self, refresh_time=1) -> None:
+        """
+        Executes the forward process repeatedly at specified time intervals until execution is instructed to stop.
+
+        Args:
+            refresh_time (int): The interval, in seconds, at which the forward method is called repeatedly.
+        """
         while not self.execute_stop:
             await self.forward()
             await AsyncUtil.sleep(refresh_time)
 
     async def _process_node(self, mail: BaseMail):
+        """
+        Processes a single node based on the node type specified in the mail's package. It handles different types of nodes such as System,
+        Instruction, ActionNode, and generic nodes through separate processes.
+
+        Args:
+            mail (BaseMail): The mail containing the node to be processed along with associated details.
+
+        Raises:
+            ValueError: If an invalid mail is encountered or the process encounters errors.
+        """
         if isinstance(mail.package["package"], System):
             self._system_process(mail.package["package"], verbose=self.verbose)
             self.send(
                 mail.sender_id,
                 "node_id",
                 {"request_source": self.id_, "package": mail.package["package"].id_},
             )
@@ -70,33 +90,56 @@
                         "package": mail.package["package"].id_,
                     },
                 )
             except:
                 raise ValueError(f"Invalid mail to process. Mail:{mail}")
 
     def _process_node_list(self, mail: BaseMail):
+        """
+        Processes a list of nodes provided in the mail, but currently only sends an end signal as multiple path selection is not supported.
+
+        Args:
+            mail (BaseMail): The mail containing a list of nodes to be processed.
+
+        Raises:
+            ValueError: When trying to process multiple paths which is currently unsupported.
+        """
         self.send(mail.sender_id, "end", {"request_source": self.id_, "package": "end"})
         self.execute_stop = True
         raise ValueError("Multiple path selection is currently not supported")
 
     def _process_condition(self, mail: BaseMail):
+        """
+        Processes a condition associated with an edge based on the mail's package, setting up the result of the condition check.
+
+        Args:
+            mail (BaseMail): The mail containing the condition to be processed.
+        """
         relationship: Edge = mail.package["package"]
         check_result = relationship.condition(self)
         back_mail = {
             "from": self.id_,
             "edge_id": mail.package["package"].id_,
             "check_result": check_result,
         }
         self.send(
             mail.sender_id,
             "condition",
             {"request_source": self.id_, "package": back_mail},
         )
 
     def _system_process(self, system: System, verbose=True, context_verbose=False):
+        """
+        Processes a system node, possibly displaying its content and context if verbose is enabled.
+
+        Args:
+            system (System): The system node to process.
+            verbose (bool): Flag to enable verbose output.
+            context_verbose (bool): Flag to enable verbose output specifically for context.
+        """
         from lionagi.libs import SysUtil
 
         SysUtil.check_import("IPython")
         from IPython.display import Markdown, display
 
         if verbose:
             print(f"------------------Welcome: {system.sender}--------------------")
@@ -107,14 +150,22 @@
                 display(Markdown(f"context: {convert.to_str(self.context)}"))
 
         self.add_message(system=system)
 
     async def _instruction_process(
         self, instruction: Instruction, verbose=True, **kwargs
     ):
+        """
+        Processes an instruction node, possibly displaying its content if verbose is enabled, and handling any additional keyword arguments.
+
+        Args:
+            instruction (Instruction): The instruction node to process.
+            verbose (bool): Flag to enable verbose output.
+            **kwargs: Additional keyword arguments that might affect how instructions are processed.
+        """
         from lionagi.libs import SysUtil
 
         SysUtil.check_import("IPython")
         from IPython.display import Markdown, display
 
         if verbose:
             with contextlib.suppress(Exception):
@@ -142,14 +193,21 @@
                 )
             )
             print("-----------------------------------------------------")
 
         self.execution_responses.append(result)
 
     async def _action_process(self, action: ActionNode, verbose=True):
+        """
+        Processes an action node, executing the defined action along with any tools specified within the node.
+
+        Args:
+            action (ActionNode): The action node to process.
+            verbose (bool): Flag to enable verbose output of the action results.
+        """
         from lionagi.libs import SysUtil
 
         SysUtil.check_import("IPython")
         from IPython.display import Markdown, display
 
         try:
             func = getattr(self, action.action)
@@ -192,24 +250,29 @@
         """
         Processes an agent.
 
         Args:
             agent: The agent to process.
             verbose (bool): A flag indicating whether to provide verbose output (default: True).
         """
-        context = self.responses
+        context = list(self.messages["content"])
         if verbose:
             print("*****************************************************")
         result = await agent.execute(context)
 
         if verbose:
             print("*****************************************************")
 
-        self.context = result
-        self.responses.append(result)
+        from pandas import DataFrame
+
+        if isinstance(result, DataFrame):
+            self.context = list(result["content"])
+        else:
+            self.context = result
+        self.execution_responses.append(result)
 
     def _process_start(self, mail):
         """
         Processes a start mail.
 
         Args:
             mail (BaseMail): The start mail to process.
```

### Comparing `lionagi-0.1.0/lionagi/core/execute/structure_executor.py` & `lionagi-0.1.1/lionagi/core/execute/structure_executor.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,18 +15,40 @@
 from lionagi.core.tool import Tool
 
 from lionagi.core.mail.schema import BaseMail
 from lionagi.core.graph.graph import Graph
 
 
 class StructureExecutor(BaseExecutor, Graph):
+    """
+    Executes tasks within a graph structure, handling dynamic node flows and conditional edge logic.
+
+    Attributes:
+        condition_check_result (bool | None): Result of the last condition check performed during execution,
+            used to control flow based on dynamic conditions.
+    """
 
     condition_check_result: bool | None = None
 
     async def check_edge_condition(self, edge: Edge, executable_id, request_source):
+        """
+        Evaluates the condition associated with an edge, determining if execution should proceed along that edge based
+        on the condition's source type.
+
+        Args:
+            edge (Edge): The edge whose condition needs to be checked.
+            executable_id (str): ID of the executor handling this edge's condition.
+            request_source (str): Origin of the request prompting this condition check.
+
+        Returns:
+            bool: Result of the condition evaluation.
+
+        Raises:
+            ValueError: If the source_type of the condition is invalid.
+        """
         if edge.condition.source_type == "structure":
             return edge.condition(self)
 
         elif edge.condition.source_type == "executable":
             return await self._check_executable_condition(
                 edge, executable_id, request_source
             )
@@ -55,49 +77,87 @@
                 else:
                     skipped_requests.append(mail)
             self.pending_ins[key] = skipped_requests
 
     async def _check_executable_condition(
         self, edge: Edge, executable_id, request_source
     ):
+        """
+        Sends the edge's condition to an external executable for evaluation and waits for the result.
+
+        Args:
+            edge (Edge): The edge containing the condition to be checked.
+            executable_id (str): ID of the executable that will evaluate the condition.
+            request_source (str): Source of the request for condition evaluation.
+
+        Returns:
+            bool: The result of the condition check.
+        """
         self.send(
             recipient_id=executable_id,
             category="condition",
             package={"request_source": request_source, "package": edge},
         )
         while self.condition_check_result is None:
             await AsyncUtil.sleep(0.1)
             self._process_edge_condition(edge.id_)
             continue
         check_result = self.condition_check_result
         self.condition_check_result = None
         return check_result
 
     async def _handle_node_id(self, mail: BaseMail):
+        """
+        Processes the node identified by its ID in the mail's package, ensuring it exists and retrieving the next set of
+        nodes based on the current node.
+
+        Args:
+            mail (BaseMail): The mail containing the node ID and related execution details.
+
+        Raises:
+            ValueError: If the node does not exist within the structure.
+        """
         if mail.package["package"] not in self.internal_nodes:
             raise ValueError(
                 f"Node {mail.package} does not exist in the structure {self.id_}"
             )
         return await self._next_node(
             self.internal_nodes[mail.package["package"]],
             mail.sender_id,
             mail.package["request_source"],
         )
 
     async def _handle_node(self, mail: BaseMail):
+        """
+        Processes the node specified in the mail's package, ensuring it exists within the structure.
+
+        Args:
+            mail (BaseMail): The mail containing the node details to be processed.
+
+        Raises:
+            ValueError: If the node does not exist within the structure.
+        """
         if not self.node_exist(mail.package["package"]):
             raise ValueError(
                 f"Node {mail.package} does not exist in the structure {self.id_}"
             )
         return await self._next_node(
             mail.package["package"], mail.sender_id, mail.package["request_source"]
         )
 
     async def _handle_mail(self, mail: BaseMail):
+        """
+        Processes incoming mail based on its category, initiating node execution or structure operations accordingly.
+
+        Args:
+            mail (BaseMail): The mail to be processed, containing category and package information.
 
+        Raises:
+            ValueError: If the mail type is invalid for the current structure or an error occurs in handling the node ID.
+        """
         if mail.category == "start":
             return self.get_heads()
 
         elif mail.category == "end":
             self.execute_stop = True
             return None
 
@@ -112,48 +172,55 @@
                 return await self._handle_node(mail)
             except Exception as e:
                 raise ValueError(f"Error handling node: {e}") from e
 
         else:
             raise ValueError(f"Invalid mail type for structure")
 
-    async def _next_node(self, current_node: BaseNode, executable_id, request_source):
+    async def _next_node(self, current_node: Node, executable_id, request_source):
         """
         Get the next step nodes based on the current node.
 
         Args:
             current_node (Node): The current node.
             executable_id (str): The ID of the executable.
 
         Returns:
             list[Node]: The next step nodes.
         """
         next_nodes = []
-        next_edges: dict[Edge] = self.get_node_edges(current_node, node_as="out")
+        next_edges = self.get_node_edges(current_node, node_as="out")
         for edge in convert.to_list(list(next_edges.values())):
             if edge.bundle:
                 continue
             if edge.condition:
                 check = await self.check_edge_condition(
                     edge, executable_id, request_source
                 )
                 if not check:
                     continue
             node = self.internal_nodes[edge.tail]
-            further_edges: dict[Edge] = self.get_node_edges(node, node_as="out")
+            further_edges = self.get_node_edges(node, node_as="out")
             bundled_nodes = deque()
             for f_edge in convert.to_list(list(further_edges.values())):
                 if f_edge.bundle:
                     bundled_nodes.append(self.internal_nodes[f_edge.tail])
             if bundled_nodes:
                 node = self.parse_bundled_to_action(node, bundled_nodes)
             next_nodes.append(node)
         return next_nodes
 
     def _send_mail(self, next_nodes: list | None, mail: BaseMail):
+        """
+        Sends mails to the next nodes or signals the end of execution if no next nodes exist.
+
+        Args:
+            next_nodes (list | None): List of next nodes to process or None if no further nodes are available.
+            mail (BaseMail): The base mail used for sending follow-up actions.
+        """
         if not next_nodes:  # tail
             self.send(
                 recipient_id=mail.sender_id,
                 category="end",
                 package={
                     "request_source": mail.package["request_source"],
                     "package": "end",
@@ -177,14 +244,34 @@
                         "request_source": mail.package["request_source"],
                         "package": next_nodes,
                     },
                 )
 
     @staticmethod
     def parse_bundled_to_action(instruction: Node, bundled_nodes: deque):
+        """
+        Constructs an action node from a bundle of nodes, combining various types of nodes like ActionSelection or Tool
+        into a single actionable unit.
+
+        This method takes a bundle of nodes and systematically integrates their functionalities into a single `ActionNode`.
+        This is crucial in scenarios where multiple actions or tools need to be executed sequentially or in a coordinated
+        manner as part of a larger instruction flow.
+
+        Args:
+            instruction (Node): The initial instruction node leading to this action.
+            bundled_nodes (deque): A deque containing nodes to be bundled into the action. These nodes typically represent
+                either actions to be taken or tools to be utilized.
+
+        Returns:
+            ActionNode: An `ActionNode` that encapsulates the combined functionality of the bundled nodes, ready for execution.
+
+        Raises:
+            ValueError: If an unrecognized node type is encountered within the bundled nodes. Only `ActionSelection` and
+                `Tool` nodes are valid for bundling into an `ActionNode`.
+        """
         action_node = ActionNode(instruction=instruction)
         while bundled_nodes:
             node = bundled_nodes.popleft()
             if isinstance(node, ActionSelection):
                 action_node.action = node.action
                 action_node.action_kwargs = node.action_kwargs
             elif isinstance(node, Tool):
@@ -206,13 +293,22 @@
                         return
                     next_nodes = await self._handle_mail(mail)
                     self._send_mail(next_nodes, mail)
                 except Exception as e:
                     raise ValueError(f"Error handling mail: {e}") from e
 
     async def execute(self, refresh_time=1):
+        """
+        Executes the forward processing loop, checking conditions and processing nodes at defined intervals.
+
+        Args:
+            refresh_time (int): The delay between execution cycles, allowing for asynchronous operations to complete.
+
+        Raises:
+            ValueError: If the graph structure is found to be cyclic, which is unsupported.
+        """
         if not self.acyclic:
             raise ValueError("Structure is not acyclic")
 
         while not self.execute_stop:
             await self.forward()
             await AsyncUtil.sleep(refresh_time)
```

### Comparing `lionagi-0.1.0/lionagi/core/flow/monoflow/ReAct.py` & `lionagi-0.1.1/lionagi/core/flow/monoflow/ReAct.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,16 +42,15 @@
 
     REASON_PROMPT = """
     You have {num_steps} steps left in the current task. If available, integrate previous tool responses.
     Perform reasoning and prepare an action plan according to available tools only. Apply divide and conquer technique.
     """
 
     ACTION_PROMPT = """
-    You have {num_steps} steps left in the current task. If further actions are needed, invoke tool usage.
-    If you are done, present the final result to the user without further tool usage.
+    You have {num_steps} steps left in the current task. invoke tool usage.
     """
 
     OUTPUT_PROMPT = "Notice: Present the final output to the user. Original user instruction: {instruction}"
 
     async def ReAct(
         self,
         instruction: Instruction | str | dict[str, dict | str],
@@ -123,23 +122,23 @@
         except (KeyError, ValueError):
             pass
 
         return default
 
     def _create_followup_config(self, tools, tool_choice="auto", **kwargs):
         """
-        Creates the configuration for the followup steps based on the provided tools and parameters.
+        Creates the configuration for the followup chat based on the provided tools and parameters.
 
         Args:
-            tools (Optional[Any]): Specifies tools to be invoked during the followup steps.
+            tools (Optional[Any]): Specifies tools to be invoked during the followup chat.
             tool_choice (str): The choice of tools to use (default: "auto").
-            **kwargs: Additional keyword arguments for the followup configuration.
+            **kwargs: Additional keyword arguments for the followup chat configuration.
 
         Returns:
-            dict: The configuration for the followup steps.
+            dict: The configuration for the followup chat.
 
         Raises:
             ValueError: If no tools are found and registered.
         """
         if tools and isinstance(tools, list) and isinstance(tools[0], (Callable, Tool)):
             self.branch.tool_manager.register_tools(tools)
 
@@ -155,15 +154,15 @@
         self,
         instruction: Instruction | str | dict[str, dict | str],
         context=None,
         sender=None,
         system=None,
         tools=None,
         num_rounds: int = 1,
-        auto=False,
+        auto=True,
         reason_prompt=None,
         action_prompt=None,
         output_prompt=None,
         out=True,
         **kwargs,
     ):
         """
@@ -184,14 +183,15 @@
             out (bool): Flag indicating whether to return the output of the task (default: True).
             **kwargs: Additional keyword arguments for the task.
 
         Returns:
             The result of the reasoning and action steps.
         """
         config = self._create_followup_config(tools, **kwargs)
+        kwargs.pop("tools", None)
 
         i = 0
         _out = ""
 
         while i < num_rounds:
             _prompt = self._get_prompt(
                 prompt=reason_prompt,
@@ -216,23 +216,23 @@
                 prompt=action_prompt,
                 default=self.ACTION_PROMPT,
                 num_steps=(num_rounds - i) * 2 - 1,
             )
 
             _out = await self.chat(_prompt, sender=sender, **config)
 
-            if auto and not self.branch._is_invoked():
+            if not self.branch._is_invoked():
                 return _out if out else None
 
             i += 1
 
-        if auto:
-            if not self.branch._is_invoked():
-                return _out if out else None
 
-            _prompt = self._get_prompt(
-                prompt=output_prompt,
-                default=self.OUTPUT_PROMPT,
-                instruction=instruction,
-            )
-            _out = await self.chat(_prompt, sender=sender, **kwargs)
-            return _out if out else None
+        if not self.branch._is_invoked():
+            return _out if out else None
+
+        _prompt = self._get_prompt(
+            prompt=output_prompt,
+            default=self.OUTPUT_PROMPT,
+            instruction=instruction,
+        )
+        _out = await self.chat(_prompt, sender=sender, **kwargs)
+        return _out if out else None
```

### Comparing `lionagi-0.1.0/lionagi/core/flow/monoflow/chat.py` & `lionagi-0.1.1/lionagi/core/flow/monoflow/chat.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/flow/monoflow/chat_mixin.py` & `lionagi-0.1.1/lionagi/core/flow/monoflow/chat_mixin.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -246,8 +246,8 @@
 
 
 class MonoChatMixin(MonoChatConfigMixin, MonoChatInvokeMixin, ABC):
     """
     Mixin class that combines MonoChatConfigMixin and MonoChatInvokeMixin.
     """
 
-    pass
+    pass
```

### Comparing `lionagi-0.1.0/lionagi/core/flow/monoflow/followup.py` & `lionagi-0.1.1/lionagi/core/flow/monoflow/followup.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         self,
         instruction: Instruction | str | dict[str, dict | str],
         context=None,
         sender=None,
         system=None,
         tools=None,
         max_followup: int = 1,
-        auto=False,
+        auto=True,
         followup_prompt=None,
         output_prompt=None,
         out=True,
         **kwargs,
     ) -> None:
         """
         Performs the actual followup chats with the LLM, processing instructions and system messages,
@@ -192,23 +192,22 @@
                 _prompt = {"NOTICE": _prompt, "TASK": instruction}
                 _out = await self.chat(
                     _prompt, context=context, sender=sender, system=system, **config
                 )
             else:
                 _out = await self.chat(_prompt, sender=sender, **config)
 
-            if auto and not self.branch._is_invoked():
+            if not self.branch._is_invoked():
                 return _out if out else None
 
             i += 1
 
-        if auto:
-            if not self.branch._is_invoked():
-                return _out if out else None
+        if not self.branch._is_invoked():
+            return _out if out else None
 
-            _prompt = self._get_prompt(
-                prompt=output_prompt,
-                default=self.OUTPUT_PROMPT,
-                instruction=instruction,
-            )
-            _out = await self.chat(_prompt, sender=sender, **kwargs)
-            return _out if out else None
+        _prompt = self._get_prompt(
+            prompt=output_prompt,
+            default=self.OUTPUT_PROMPT,
+            instruction=instruction,
+        )
+        _out = await self.chat(_prompt, sender=sender, **kwargs)
+        return _out if out else None
```

### Comparing `lionagi-0.1.0/lionagi/core/flow/polyflow/chat.py` & `lionagi-0.1.1/lionagi/core/flow/polyflow/chat.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/form/action_form.py` & `lionagi-0.1.1/lionagi/core/form/action_form.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/form/field_validator.py` & `lionagi-0.1.1/lionagi/core/form/field_validator.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/form/form.py` & `lionagi-0.1.1/lionagi/core/form/form.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/form/mixin.py` & `lionagi-0.1.1/lionagi/core/form/mixin.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/generic/__init__.py` & `lionagi-0.1.1/lionagi/core/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/generic/action.py` & `lionagi-0.1.1/lionagi/core/generic/action.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/generic/component.py` & `lionagi-0.1.1/lionagi/core/generic/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,14 @@
                 annotations.
         """
         dict_ = {}
         for i in field_name:
             dict_.update(self._get_field_annotation(i))
         return dict_
 
-
     @_get_field_annotation.register(tuple)
     def _(self, field_name) -> dict[str, Any]:
         """
         Get the annotations for multiple fields as a dictionary.
 
         Args:
             field_name (tuple): A list or tuple of field names.
@@ -164,15 +163,14 @@
                 annotations.
         """
         dict_ = {}
         for i in field_name:
             dict_.update(self._get_field_annotation(i))
         return dict_
 
-
     def _field_has_attr(self, k: str, attr: str) -> bool:
         """
         Check if a field has a specific attribute.
 
         Args:
             k (str): The field name.
             attr (str): The attribute name.
```

### Comparing `lionagi-0.1.0/lionagi/core/generic/condition.py` & `lionagi-0.1.1/lionagi/core/generic/condition.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,14 @@
 
     class Config:
         """Model configuration settings."""
 
         extra = "allow"
 
     @abstractmethod
-    def __call__(self, *args, **kwargs) -> bool:
+    def __call__(self, executable) -> bool:
         """Evaluates the condition based on implemented logic.
 
         Returns:
             bool: The boolean result of the condition evaluation.
         """
         pass
```

### Comparing `lionagi-0.1.0/lionagi/core/generic/data_logger.py` & `lionagi-0.1.1/lionagi/core/generic/data_logger.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/generic/mail.py` & `lionagi-0.1.1/lionagi/core/generic/mail.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/generic/mailbox.py` & `lionagi-0.1.1/lionagi/core/generic/mailbox.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/generic/node.py` & `lionagi-0.1.1/lionagi/core/generic/node.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/generic/relation.py` & `lionagi-0.1.1/lionagi/core/generic/relation.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/generic/signal.py` & `lionagi-0.1.1/lionagi/core/generic/signal.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/generic/structure.py` & `lionagi-0.1.1/lionagi/core/generic/structure.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/generic/transfer.py` & `lionagi-0.1.1/lionagi/core/generic/transfer.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/generic/work.py` & `lionagi-0.1.1/lionagi/core/generic/work.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/graph/graph.py` & `lionagi-0.1.1/lionagi/core/graph/graph.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/graph/tree.py` & `lionagi-0.1.1/lionagi/core/graph/tree.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/mail/mail_manager.py` & `lionagi-0.1.1/lionagi/core/mail/mail_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 
     Attributes:
             sources (Dict[str, Any]): A dictionary mapping source identifiers to their attributes.
             mails (Dict[str, Dict[str, deque]]): A nested dictionary storing queued mail items, organized by recipient
                     and sender.
     """
 
-    def __init__(self, sources):
+    def __init__(self, sources=None):
         self.sources = {}
         self.mails = {}
-        self.add_sources(sources)
+        if sources:
+            self.add_sources(sources)
         self.execute_stop = False
 
     def add_sources(self, sources):
         if isinstance(sources, dict):
             for _, v in sources.items():
                 if v.id_ not in self.sources:
                     self.sources[v.id_] = v
```

### Comparing `lionagi-0.1.0/lionagi/core/mail/schema.py` & `lionagi-0.1.1/lionagi/core/mail/schema.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/messages/schema.py` & `lionagi-0.1.1/lionagi/core/messages/schema.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/session/session.py` & `lionagi-0.1.1/lionagi/core/session/session.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -978,8 +978,8 @@
         )
 
         self.default_branch = branch
         self.default_branch_name = default_branch_name or "main"
         if system:
             self.default_branch.add_message(system=system, sender=sender)
 
-        self.llmconfig = self.default_branch.llmconfig
+        self.llmconfig = self.default_branch.llmconfig
```

### Comparing `lionagi-0.1.0/lionagi/core/tool/tool.py` & `lionagi-0.1.1/lionagi/core/tool/tool.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/core/tool/tool_manager.py` & `lionagi-0.1.1/lionagi/core/tool/tool_manager.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/integrations/bridge/langchain_/documents.py` & `lionagi-0.1.1/lionagi/integrations/bridge/langchain_/documents.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/integrations/bridge/langchain_/langchain_bridge.py` & `lionagi-0.1.1/lionagi/integrations/bridge/langchain_/langchain_bridge.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/llama_index_bridge.py` & `lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/llama_index_bridge.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/node_parser.py` & `lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/node_parser.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/reader.py` & `lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/reader.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/integrations/bridge/llamaindex_/textnode.py` & `lionagi-0.1.1/lionagi/integrations/bridge/llamaindex_/textnode.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/integrations/chunker/chunk.py` & `lionagi-0.1.1/lionagi/integrations/chunker/chunk.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/integrations/config/oai_configs.py` & `lionagi-0.1.1/lionagi/integrations/config/oai_configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Default configs for the OpenAI API
 
 # ChatCompletion
 oai_chat_llmconfig = {
-    "model": "gpt-4-turbo-preview",
+    "model": "gpt-4-turbo",
     "frequency_penalty": 0,
     "max_tokens": None,
     "n": 1,
     "presence_penalty": 0,
     "response_format": {"type": "text"},
     "seed": None,
     "stop": None,
```

### Comparing `lionagi-0.1.0/lionagi/integrations/config/openrouter_configs.py` & `lionagi-0.1.1/lionagi/integrations/config/openrouter_configs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 openrouter_chat_llmconfig = {
-    "model": "gpt-4-turbo-preview",
+    "model": "gpt-4-turbo",
     "frequency_penalty": 0,
     "max_tokens": None,
     "num": 1,
     "presence_penalty": 0,
     "response_format": {"type": "text"},
     "seed": None,
     "stop": None,
```

### Comparing `lionagi-0.1.0/lionagi/integrations/loader/load.py` & `lionagi-0.1.1/lionagi/integrations/loader/load.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/integrations/loader/load_util.py` & `lionagi-0.1.1/lionagi/integrations/loader/load_util.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/integrations/provider/litellm.py` & `lionagi-0.1.1/lionagi/integrations/provider/litellm.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/integrations/provider/mlx_service.py` & `lionagi-0.1.1/lionagi/integrations/provider/mlx_service.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/integrations/provider/oai.py` & `lionagi-0.1.1/lionagi/integrations/provider/oai.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/integrations/provider/ollama.py` & `lionagi-0.1.1/lionagi/integrations/provider/ollama.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/integrations/provider/openrouter.py` & `lionagi-0.1.1/lionagi/integrations/provider/openrouter.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/integrations/provider/services.py` & `lionagi-0.1.1/lionagi/integrations/provider/services.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/integrations/provider/transformers.py` & `lionagi-0.1.1/lionagi/integrations/provider/transformers.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/libs/__init__.py` & `lionagi-0.1.1/lionagi/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/libs/ln_api.py` & `lionagi-0.1.1/lionagi/libs/ln_api.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/libs/ln_async.py` & `lionagi-0.1.1/lionagi/libs/ln_async.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/libs/ln_convert.py` & `lionagi-0.1.1/lionagi/libs/ln_convert.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/libs/ln_dataframe.py` & `lionagi-0.1.1/lionagi/libs/ln_dataframe.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/libs/ln_func_call.py` & `lionagi-0.1.1/lionagi/libs/ln_func_call.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/libs/ln_nested.py` & `lionagi-0.1.1/lionagi/libs/ln_nested.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/libs/ln_parse.py` & `lionagi-0.1.1/lionagi/libs/ln_parse.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/libs/ln_validate.py` & `lionagi-0.1.1/lionagi/libs/ln_validate.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/libs/sys_util.py` & `lionagi-0.1.1/lionagi/libs/sys_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,15 +268,15 @@
                 import_name: The specific name to import from the module or package. Defaults to None.
                 pip_name: The pip package name if different from `package_name`. Defaults to None.
                 attempt_install: If attempt to install the package if uninstalled. Defaults to True.
                 error_message: Error message when the package is not installed and not attempt to install.
         """
         try:
             if not SysUtil.is_package_installed(package_name):
-                print("check")
+                # print("check")
                 if attempt_install:
                     logging.info(
                         f"Package {package_name} not found. Attempting to install."
                     )
                     SysUtil.install_import(
                         package_name, module_name, import_name, pip_name
                     )
```

### Comparing `lionagi-0.1.0/lionagi/tests/libs/test_api.py` & `lionagi-0.1.1/lionagi/tests/libs/test_api.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/tests/libs/test_convert.py` & `lionagi-0.1.1/lionagi/tests/libs/test_convert.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/tests/libs/test_field_validators.py` & `lionagi-0.1.1/lionagi/tests/libs/test_field_validators.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/tests/libs/test_func_call.py` & `lionagi-0.1.1/lionagi/tests/libs/test_func_call.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/tests/libs/test_nested.py` & `lionagi-0.1.1/lionagi/tests/libs/test_nested.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/tests/libs/test_parse.py` & `lionagi-0.1.1/lionagi/tests/libs/test_parse.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/tests/libs/test_sys_util.py` & `lionagi-0.1.1/lionagi/tests/libs/test_sys_util.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/tests/test_core/test_base_branch.py` & `lionagi-0.1.1/lionagi/tests/test_core/test_base_branch.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/tests/test_core/test_branch.py` & `lionagi-0.1.1/lionagi/tests/test_core/test_branch.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # import unittest
 # from unittest.mock import patch, MagicMock
 # import pandas as pd
 # import json
 # from collections import deque
 
 
-
 # class TestBranch(unittest.TestCase):
 #     def setUp(self):
 #         # Assuming no need for actual files or external services for initialization
 #         self.test_messages = [
 #             {
 #                 "node_id": "1",
 #                 "timestamp": "2021-01-01 00:00:00",
```

### Comparing `lionagi-0.1.0/lionagi/tests/test_core/test_chat_flow.py` & `lionagi-0.1.1/lionagi/tests/test_core/test_chat_flow.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/tests/test_core/test_mail_manager.py` & `lionagi-0.1.1/lionagi/tests/test_core/test_mail_manager.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/tests/test_core/test_prompts.py` & `lionagi-0.1.1/lionagi/tests/test_core/test_prompts.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/tests/test_core/test_session.py` & `lionagi-0.1.1/lionagi/tests/test_core/test_session.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/tests/test_core/test_session_base_util.py` & `lionagi-0.1.1/lionagi/tests/test_core/test_session_base_util.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi/tests/test_core/test_tool_manager.py` & `lionagi-0.1.1/lionagi/tests/test_core/test_tool_manager.py`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/lionagi.egg-info/PKG-INFO` & `lionagi-0.1.1/lionagi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lionagi
-Version: 0.1.0
+Version: 0.1.1
 Summary: Towards automated general intelligence.
 Author: HaiyangLi
 Author-email: Haiyang Li <ocean@lionagi.ai>
 License: MIT License
         
         Copyright (c) 2023 HaiyangLi quantocean.li@gmail.com
```

### Comparing `lionagi-0.1.0/pyproject.toml` & `lionagi-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lionagi-0.1.0/setup.py` & `lionagi-0.1.1/setup.py`

 * *Files identical despite different names*

