# Comparing `tmp/llmtuner-0.6.2.tar.gz` & `tmp/llmtuner-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmtuner-0.6.2.tar", last modified: Thu Apr 11 12:07:25 2024, max compression
+gzip compressed data, was "llmtuner-0.6.3.tar", last modified: Sun Apr 21 15:13:38 2024, max compression
```

## Comparing `llmtuner-0.6.2.tar` & `llmtuner-0.6.3.tar`

### file list

```diff
@@ -1,119 +1,121 @@
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:24.949448 llmtuner-0.6.2/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2024-04-11 12:07:00.000000 llmtuner-0.6.2/LICENSE
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    32281 2024-04-11 12:07:24.913448 llmtuner-0.6.2/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    29705 2024-04-11 12:07:00.000000 llmtuner-0.6.2/README.md
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      641 2024-04-11 12:07:00.000000 llmtuner-0.6.2/pyproject.toml
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2024-04-11 12:07:24.949448 llmtuner-0.6.2/setup.cfg
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2572 2024-04-11 12:07:00.000000 llmtuner-0.6.2/setup.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:20.641434 llmtuner-0.6.2/src/
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:20.765434 llmtuner-0.6.2/src/llmtuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      389 2024-04-11 12:06:59.000000 llmtuner-0.6.2/src/llmtuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:21.153435 llmtuner-0.6.2/src/llmtuner/api/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       55 2024-04-11 12:06:50.000000 llmtuner-0.6.2/src/llmtuner/api/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8717 2024-04-11 12:06:50.000000 llmtuner-0.6.2/src/llmtuner/api/app.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3127 2024-04-11 12:06:50.000000 llmtuner-0.6.2/src/llmtuner/api/protocol.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:21.389436 llmtuner-0.6.2/src/llmtuner/chat/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      110 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/chat/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1858 2024-04-11 12:06:50.000000 llmtuner-0.6.2/src/llmtuner/chat/base_engine.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3334 2024-04-11 12:06:50.000000 llmtuner-0.6.2/src/llmtuner/chat/chat_model.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    10056 2024-04-11 12:06:50.000000 llmtuner-0.6.2/src/llmtuner/chat/hf_engine.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5974 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/chat/vllm_engine.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:21.869438 llmtuner-0.6.2/src/llmtuner/data/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      377 2024-04-11 12:06:52.000000 llmtuner-0.6.2/src/llmtuner/data/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5505 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/data/aligner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2140 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/data/collator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6528 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/data/formatter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7364 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/data/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4989 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/data/parser.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    11328 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/data/preprocess.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    29041 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/data/template.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3698 2024-04-11 12:06:51.000000 llmtuner-0.6.2/src/llmtuner/data/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:22.049438 llmtuner-0.6.2/src/llmtuner/eval/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       59 2024-04-11 12:06:52.000000 llmtuner-0.6.2/src/llmtuner/eval/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5763 2024-04-11 12:06:52.000000 llmtuner-0.6.2/src/llmtuner/eval/evaluator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2419 2024-04-11 12:06:52.000000 llmtuner-0.6.2/src/llmtuner/eval/template.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:22.361440 llmtuner-0.6.2/src/llmtuner/extras/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/extras/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6495 2024-04-11 12:06:52.000000 llmtuner-0.6.2/src/llmtuner/extras/callbacks.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    32324 2024-04-11 12:06:52.000000 llmtuner-0.6.2/src/llmtuner/extras/constants.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1117 2024-04-11 12:06:52.000000 llmtuner-0.6.2/src/llmtuner/extras/logging.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7411 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/extras/misc.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1316 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/extras/packages.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:22.409440 llmtuner-0.6.2/src/llmtuner/extras/patches/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/extras/patches/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8841 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/extras/patches/llama_patch.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1824 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/extras/ploting.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:22.729441 llmtuner-0.6.2/src/llmtuner/hparams/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      494 2024-04-11 12:06:54.000000 llmtuner-0.6.2/src/llmtuner/hparams/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3871 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/hparams/data_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1462 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/hparams/evaluation_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    10631 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/hparams/finetuning_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1915 2024-04-11 12:06:53.000000 llmtuner-0.6.2/src/llmtuner/hparams/generating_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7154 2024-04-11 12:06:54.000000 llmtuner-0.6.2/src/llmtuner/hparams/model_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    12665 2024-04-11 12:06:54.000000 llmtuner-0.6.2/src/llmtuner/hparams/parser.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:22.909441 llmtuner-0.6.2/src/llmtuner/model/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      229 2024-04-11 12:06:54.000000 llmtuner-0.6.2/src/llmtuner/model/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7413 2024-04-11 12:06:54.000000 llmtuner-0.6.2/src/llmtuner/model/adapter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4780 2024-04-11 12:06:54.000000 llmtuner-0.6.2/src/llmtuner/model/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    18170 2024-04-11 12:06:54.000000 llmtuner-0.6.2/src/llmtuner/model/patcher.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5277 2024-04-11 12:06:54.000000 llmtuner-0.6.2/src/llmtuner/model/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:23.053442 llmtuner-0.6.2/src/llmtuner/train/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       81 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/train/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:23.169442 llmtuner-0.6.2/src/llmtuner/train/dpo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-04-11 12:06:55.000000 llmtuner-0.6.2/src/llmtuner/train/dpo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7335 2024-04-11 12:06:55.000000 llmtuner-0.6.2/src/llmtuner/train/dpo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3090 2024-04-11 12:06:55.000000 llmtuner-0.6.2/src/llmtuner/train/dpo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:23.289443 llmtuner-0.6.2/src/llmtuner/train/orpo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       60 2024-04-11 12:06:55.000000 llmtuner-0.6.2/src/llmtuner/train/orpo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5517 2024-04-11 12:06:55.000000 llmtuner-0.6.2/src/llmtuner/train/orpo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2654 2024-04-11 12:06:55.000000 llmtuner-0.6.2/src/llmtuner/train/orpo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:23.445443 llmtuner-0.6.2/src/llmtuner/train/ppo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/ppo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    20565 2024-04-11 12:06:55.000000 llmtuner-0.6.2/src/llmtuner/train/ppo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2380 2024-04-11 12:06:55.000000 llmtuner-0.6.2/src/llmtuner/train/ppo/utils.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2634 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/ppo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:23.673444 llmtuner-0.6.2/src/llmtuner/train/pt/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       52 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/pt/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1107 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/pt/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2439 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/pt/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:23.905445 llmtuner-0.6.2/src/llmtuner/train/rm/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       52 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/rm/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      267 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/rm/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5077 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/rm/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3041 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/rm/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:24.085446 llmtuner-0.6.2/src/llmtuner/train/sft/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/train/sft/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2504 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/sft/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5073 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/sft/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4300 2024-04-11 12:06:56.000000 llmtuner-0.6.2/src/llmtuner/train/sft/workflow.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3969 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/train/tuner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    14011 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/train/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:24.401446 llmtuner-0.6.2/src/llmtuner/webui/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       95 2024-04-11 12:06:59.000000 llmtuner-0.6.2/src/llmtuner/webui/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4997 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/webui/chatter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4799 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/webui/common.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:24.713448 llmtuner-0.6.2/src/llmtuner/webui/components/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      362 2024-04-11 12:06:58.000000 llmtuner-0.6.2/src/llmtuner/webui/components/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2021 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/webui/components/chatbot.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3393 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/webui/components/data.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2719 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/webui/components/eval.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3671 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/webui/components/export.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1274 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/webui/components/infer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2313 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/webui/components/top.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     9869 2024-04-11 12:06:58.000000 llmtuner-0.6.2/src/llmtuner/webui/components/train.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      567 2024-04-11 12:06:57.000000 llmtuner-0.6.2/src/llmtuner/webui/css.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2784 2024-04-11 12:06:58.000000 llmtuner-0.6.2/src/llmtuner/webui/engine.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2519 2024-04-11 12:06:58.000000 llmtuner-0.6.2/src/llmtuner/webui/interface.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    42316 2024-04-11 12:06:58.000000 llmtuner-0.6.2/src/llmtuner/webui/locales.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2004 2024-04-11 12:06:58.000000 llmtuner-0.6.2/src/llmtuner/webui/manager.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    16024 2024-04-11 12:06:58.000000 llmtuner-0.6.2/src/llmtuner/webui/runner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3260 2024-04-11 12:06:58.000000 llmtuner-0.6.2/src/llmtuner/webui/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:20.977435 llmtuner-0.6.2/src/llmtuner.egg-info/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    32281 2024-04-11 12:07:19.000000 llmtuner-0.6.2/src/llmtuner.egg-info/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3007 2024-04-11 12:07:19.000000 llmtuner-0.6.2/src/llmtuner.egg-info/SOURCES.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2024-04-11 12:07:19.000000 llmtuner-0.6.2/src/llmtuner.egg-info/dependency_links.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      580 2024-04-11 12:07:19.000000 llmtuner-0.6.2/src/llmtuner.egg-info/requires.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2024-04-11 12:07:19.000000 llmtuner-0.6.2/src/llmtuner.egg-info/top_level.txt
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-11 12:07:24.829448 llmtuner-0.6.2/tests/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      933 2024-04-11 12:06:59.000000 llmtuner-0.6.2/tests/test_throughput.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2566 2024-04-11 12:06:59.000000 llmtuner-0.6.2/tests/test_toolcall.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:38.024641 llmtuner-0.6.3/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2024-04-21 15:12:38.000000 llmtuner-0.6.3/LICENSE
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    34527 2024-04-21 15:13:37.988640 llmtuner-0.6.3/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    31899 2024-04-21 15:12:38.000000 llmtuner-0.6.3/README.md
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      641 2024-04-21 15:12:38.000000 llmtuner-0.6.3/pyproject.toml
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2024-04-21 15:13:38.024641 llmtuner-0.6.3/setup.cfg
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2596 2024-04-21 15:12:39.000000 llmtuner-0.6.3/setup.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:32.364621 llmtuner-0.6.3/src/
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:32.552622 llmtuner-0.6.3/src/llmtuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      389 2024-04-21 15:12:37.000000 llmtuner-0.6.3/src/llmtuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:32.880623 llmtuner-0.6.3/src/llmtuner/api/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       55 2024-04-21 15:12:28.000000 llmtuner-0.6.3/src/llmtuner/api/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8717 2024-04-21 15:12:28.000000 llmtuner-0.6.3/src/llmtuner/api/app.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3127 2024-04-21 15:12:28.000000 llmtuner-0.6.3/src/llmtuner/api/protocol.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:33.148624 llmtuner-0.6.3/src/llmtuner/chat/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      110 2024-04-21 15:12:29.000000 llmtuner-0.6.3/src/llmtuner/chat/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1770 2024-04-21 15:12:28.000000 llmtuner-0.6.3/src/llmtuner/chat/base_engine.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3334 2024-04-21 15:12:29.000000 llmtuner-0.6.3/src/llmtuner/chat/chat_model.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    10056 2024-04-21 15:12:29.000000 llmtuner-0.6.3/src/llmtuner/chat/hf_engine.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5840 2024-04-21 15:12:29.000000 llmtuner-0.6.3/src/llmtuner/chat/vllm_engine.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:33.584625 llmtuner-0.6.3/src/llmtuner/data/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      377 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/data/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5505 2024-04-21 15:12:29.000000 llmtuner-0.6.3/src/llmtuner/data/aligner.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2140 2024-04-21 15:12:29.000000 llmtuner-0.6.3/src/llmtuner/data/collator.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6528 2024-04-21 15:12:29.000000 llmtuner-0.6.3/src/llmtuner/data/formatter.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7364 2024-04-21 15:12:29.000000 llmtuner-0.6.3/src/llmtuner/data/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4989 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/data/parser.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    11328 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/data/preprocess.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    30113 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/data/template.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3698 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/data/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:33.692626 llmtuner-0.6.3/src/llmtuner/eval/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       59 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/eval/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5763 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/eval/evaluator.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2419 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/eval/template.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:34.232627 llmtuner-0.6.3/src/llmtuner/extras/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/extras/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6495 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/extras/callbacks.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    34840 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/extras/constants.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1117 2024-04-21 15:12:30.000000 llmtuner-0.6.3/src/llmtuner/extras/logging.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7450 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/extras/misc.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1314 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/extras/packages.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:34.468628 llmtuner-0.6.3/src/llmtuner/extras/patches/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/extras/patches/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8841 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/extras/patches/llama_patch.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1824 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/extras/ploting.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:34.884630 llmtuner-0.6.3/src/llmtuner/hparams/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      494 2024-04-21 15:12:32.000000 llmtuner-0.6.3/src/llmtuner/hparams/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3871 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/hparams/data_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1462 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/hparams/evaluation_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    12586 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/hparams/finetuning_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1915 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/hparams/generating_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7468 2024-04-21 15:12:31.000000 llmtuner-0.6.3/src/llmtuner/hparams/model_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    14439 2024-04-21 15:12:32.000000 llmtuner-0.6.3/src/llmtuner/hparams/parser.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:35.380632 llmtuner-0.6.3/src/llmtuner/model/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      229 2024-04-21 15:12:32.000000 llmtuner-0.6.3/src/llmtuner/model/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7992 2024-04-21 15:12:32.000000 llmtuner-0.6.3/src/llmtuner/model/adapter.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5786 2024-04-21 15:12:32.000000 llmtuner-0.6.3/src/llmtuner/model/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    18372 2024-04-21 15:12:32.000000 llmtuner-0.6.3/src/llmtuner/model/patcher.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6956 2024-04-21 15:12:32.000000 llmtuner-0.6.3/src/llmtuner/model/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:35.520632 llmtuner-0.6.3/src/llmtuner/train/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       81 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/train/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:35.664632 llmtuner-0.6.3/src/llmtuner/train/dpo/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/dpo/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7577 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/dpo/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3090 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/dpo/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:35.792633 llmtuner-0.6.3/src/llmtuner/train/orpo/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       60 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/orpo/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5763 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/orpo/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2654 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/orpo/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:36.032634 llmtuner-0.6.3/src/llmtuner/train/ppo/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/ppo/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    20807 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/ppo/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2380 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/ppo/utils.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2634 2024-04-21 15:12:33.000000 llmtuner-0.6.3/src/llmtuner/train/ppo/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:36.240634 llmtuner-0.6.3/src/llmtuner/train/pt/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       52 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/pt/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1348 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/pt/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2439 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/pt/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:36.452635 llmtuner-0.6.3/src/llmtuner/train/rm/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       52 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/rm/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      267 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/rm/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5318 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/rm/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3041 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/rm/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:36.840637 llmtuner-0.6.3/src/llmtuner/train/sft/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       54 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/sft/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2247 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/sft/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5314 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/sft/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4300 2024-04-21 15:12:34.000000 llmtuner-0.6.3/src/llmtuner/train/sft/workflow.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3914 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/train/tuner.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    16450 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/train/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:37.216638 llmtuner-0.6.3/src/llmtuner/webui/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       95 2024-04-21 15:12:37.000000 llmtuner-0.6.3/src/llmtuner/webui/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4956 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/webui/chatter.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4881 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/webui/common.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:37.648639 llmtuner-0.6.3/src/llmtuner/webui/components/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      362 2024-04-21 15:12:36.000000 llmtuner-0.6.3/src/llmtuner/webui/components/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2103 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/webui/components/chatbot.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3839 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/webui/components/data.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2776 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/webui/components/eval.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3753 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/webui/components/export.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1356 2024-04-21 15:12:36.000000 llmtuner-0.6.3/src/llmtuner/webui/components/infer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2395 2024-04-21 15:12:36.000000 llmtuner-0.6.3/src/llmtuner/webui/components/top.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     9927 2024-04-21 15:12:36.000000 llmtuner-0.6.3/src/llmtuner/webui/components/train.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      567 2024-04-21 15:12:35.000000 llmtuner-0.6.3/src/llmtuner/webui/css.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2695 2024-04-21 15:12:36.000000 llmtuner-0.6.3/src/llmtuner/webui/engine.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2600 2024-04-21 15:12:36.000000 llmtuner-0.6.3/src/llmtuner/webui/interface.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    42316 2024-04-21 15:12:36.000000 llmtuner-0.6.3/src/llmtuner/webui/locales.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2004 2024-04-21 15:12:36.000000 llmtuner-0.6.3/src/llmtuner/webui/manager.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    15689 2024-04-21 15:12:36.000000 llmtuner-0.6.3/src/llmtuner/webui/runner.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3313 2024-04-21 15:12:37.000000 llmtuner-0.6.3/src/llmtuner/webui/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:32.780622 llmtuner-0.6.3/src/llmtuner.egg-info/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    34527 2024-04-21 15:13:30.000000 llmtuner-0.6.3/src/llmtuner.egg-info/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3047 2024-04-21 15:13:31.000000 llmtuner-0.6.3/src/llmtuner.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2024-04-21 15:13:30.000000 llmtuner-0.6.3/src/llmtuner.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      586 2024-04-21 15:13:30.000000 llmtuner-0.6.3/src/llmtuner.egg-info/requires.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2024-04-21 15:13:30.000000 llmtuner-0.6.3/src/llmtuner.egg-info/top_level.txt
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2024-04-21 15:13:37.952640 llmtuner-0.6.3/tests/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2311 2024-04-21 15:12:37.000000 llmtuner-0.6.3/tests/test_attn.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1691 2024-04-21 15:12:37.000000 llmtuner-0.6.3/tests/test_galore.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      933 2024-04-21 15:12:37.000000 llmtuner-0.6.3/tests/test_throughput.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2566 2024-04-21 15:12:37.000000 llmtuner-0.6.3/tests/test_toolcall.py
```

### Comparing `llmtuner-0.6.2/LICENSE` & `llmtuner-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/PKG-INFO` & `llmtuner-0.6.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.6.2
+Version: 0.6.3
 Summary: Easy-to-use LLM fine-tuning framework
 Home-page: https://github.com/hiyouga/LLaMA-Factory
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -24,15 +24,15 @@
 License-File: LICENSE
 Requires-Dist: torch>=1.13.1
 Requires-Dist: transformers>=4.37.2
 Requires-Dist: datasets>=2.14.3
 Requires-Dist: accelerate>=0.27.2
 Requires-Dist: peft>=0.10.0
 Requires-Dist: trl>=0.8.1
-Requires-Dist: gradio<=4.21.0,>=4.0.0
+Requires-Dist: gradio>=4.0.0
 Requires-Dist: scipy
 Requires-Dist: einops
 Requires-Dist: sentencepiece
 Requires-Dist: protobuf
 Requires-Dist: uvicorn
 Requires-Dist: pydantic
 Requires-Dist: fastapi
@@ -46,14 +46,16 @@
 Requires-Dist: jieba; extra == "metrics"
 Requires-Dist: rouge-chinese; extra == "metrics"
 Provides-Extra: unsloth
 Requires-Dist: torch==2.2.0; extra == "unsloth"
 Requires-Dist: unsloth[cu121-ampere-torch220]; extra == "unsloth"
 Provides-Extra: galore
 Requires-Dist: galore-torch; extra == "galore"
+Provides-Extra: badam
+Requires-Dist: badam; extra == "badam"
 Provides-Extra: vllm
 Requires-Dist: vllm>=0.3.3; extra == "vllm"
 Provides-Extra: bitsandbytes
 Requires-Dist: bitsandbytes>=0.39.0; extra == "bitsandbytes"
 Provides-Extra: gptq
 Requires-Dist: optimum>=1.16.0; extra == "gptq"
 Requires-Dist: auto-gptq>=0.5.0; extra == "gptq"
@@ -72,15 +74,15 @@
 ![# LLaMA Factory](assets/logo.png)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Factory?style=social)](https://github.com/hiyouga/LLaMA-Factory/stargazers)
 [![GitHub Code License](https://img.shields.io/github/license/hiyouga/LLaMA-Factory)](LICENSE)
 [![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Factory)](https://github.com/hiyouga/LLaMA-Factory/commits/main)
 [![PyPI](https://img.shields.io/pypi/v/llmtuner)](https://pypi.org/project/llmtuner/)
 [![Downloads](https://static.pepy.tech/badge/llmtuner)](https://pypi.org/project/llmtuner/)
-[![Citation](https://img.shields.io/badge/citation-28-green)](#projects-using-llama-factory)
+[![Citation](https://img.shields.io/badge/citation-34-green)](#projects-using-llama-factory)
 [![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/LLaMA-Factory/pulls)
 [![Discord](https://dcbadge.vercel.app/api/server/rKfvV9r9FK?compact=true&style=flat)](https://discord.gg/rKfvV9r9FK)
 [![Twitter](https://img.shields.io/twitter/follow/llamafactory_ai)](https://twitter.com/llamafactory_ai)
 [![Spaces](https://img.shields.io/badge/🤗-Open%20in%20Spaces-blue)](https://huggingface.co/spaces/hiyouga/LLaMA-Board)
 [![Studios](https://img.shields.io/badge/ModelScope-Open%20in%20Studios-blue)](https://modelscope.cn/studios/hiyouga/LLaMA-Board)
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eRTPn37ltBbYsISy9Aw2NuI2Aq5CQrD9?usp=sharing)
 
@@ -113,15 +115,15 @@
 - [Acknowledgement](#acknowledgement)
 
 ## Features
 
 - **Various models**: LLaMA, Mistral, Mixtral-MoE, Qwen, Yi, Gemma, Baichuan, ChatGLM, Phi, etc.
 - **Integrated methods**: (Continuous) pre-training, supervised fine-tuning, reward modeling, PPO, DPO and ORPO.
 - **Scalable resources**: 32-bit full-tuning, 16-bit freeze-tuning, 16-bit LoRA and 2/4/8-bit QLoRA via AQLM/AWQ/GPTQ/LLM.int8.
-- **Advanced algorithms**: GaLore, DoRA, LongLoRA, LLaMA Pro, LoRA+, LoftQ and Agent tuning.
+- **Advanced algorithms**: GaLore, BAdam, DoRA, LongLoRA, LLaMA Pro, Mixture-of-Depths, LoRA+, LoftQ and Agent tuning.
 - **Practical tricks**: FlashAttention-2, Unsloth, RoPE scaling, NEFTune and rsLoRA.
 - **Experiment monitors**: LlamaBoard, TensorBoard, Wandb, MLflow, etc.
 - **Faster inference**: OpenAI-style API, Gradio UI and CLI with vLLM worker.
 
 ## Benchmark
 
 Compared to ChatGLM's [P-Tuning](https://github.com/THUDM/ChatGLM2-6B/tree/main/ptuning), LLaMA Factory's LoRA tuning offers up to **3.7 times faster** training speed with a better Rouge score on the advertising text generation task. By leveraging 4-bit quantization technique, LLaMA Factory's QLoRA further improves the efficiency regarding the GPU memory.
@@ -135,22 +137,30 @@
 - **GPU Memory**: Peak GPU memory usage in 4-bit quantized training. (bs=1, cutoff_len=1024)
 - We adopt `pre_seq_len=128` for ChatGLM's P-Tuning and `lora_rank=32` for LLaMA Factory's LoRA tuning.
 
 </details>
 
 ## Changelog
 
+[24/04/21] We supported **[Mixture-of-Depths](https://arxiv.org/abs/2404.02258)** according to [AstraMindAI's implementation](https://github.com/astramind-ai/Mixture-of-depths). See `examples/extras/mod` for usage.
+
+[24/04/19] We supported **Meta Llama 3** model series.
+
+[24/04/16] We supported **[BAdam](https://arxiv.org/abs/2404.02827)**. See `examples/extras/badam` for usage.
+
+[24/04/16] We supported **[unsloth](https://github.com/unslothai/unsloth)**'s long-sequence training (Llama-2-7B-56k within 24GB). It achieves **117%** speed and **50%** memory compared with FlashAttention-2, more benchmarks can be found in [this page](https://github.com/hiyouga/LLaMA-Factory/wiki/Performance-comparison).
+
+<details><summary>Full Changelog</summary>
+
 [24/03/31] We supported **[ORPO](https://arxiv.org/abs/2403.07691)**. See `examples/lora_single_gpu` for usage.
 
 [24/03/21] Our paper "[LlamaFactory: Unified Efficient Fine-Tuning of 100+ Language Models](https://arxiv.org/abs/2403.13372)" is available at arXiv!
 
 [24/03/20] We supported **FSDP+QLoRA** that fine-tunes a 70B model on 2x24GB GPUs. See `examples/extras/fsdp_qlora` for usage.
 
-<details><summary>Full Changelog</summary>
-
 [24/03/13] We supported **[LoRA+](https://arxiv.org/abs/2402.12354)**. See `examples/extras/loraplus` for usage.
 
 [24/03/07] We supported gradient low-rank projection (**[GaLore](https://arxiv.org/abs/2403.03507)**) algorithm. See `examples/extras/galore` for usage.
 
 [24/03/07] We integrated **[vLLM](https://github.com/vllm-project/vllm)** for faster and concurrent inference. Try `--infer_backend vllm` to enjoy **270%** inference speed. (LoRA is not yet supported, merge it first.)
 
 [24/02/28] We supported weight-decomposed LoRA (**[DoRA](https://arxiv.org/abs/2402.09353)**). Try `--use_dora` to activate DoRA training.
@@ -196,28 +206,30 @@
 </details>
 
 ## Supported Models
 
 | Model                                                    | Model size                  | Default module    | Template  |
 | -------------------------------------------------------- | --------------------------- | ----------------- | --------- |
 | [Baichuan2](https://huggingface.co/baichuan-inc)         | 7B/13B                      | W_pack            | baichuan2 |
-| [BLOOM](https://huggingface.co/bigscience/bloom)         | 560M/1.1B/1.7B/3B/7.1B/176B | query_key_value   | -         |
-| [BLOOMZ](https://huggingface.co/bigscience/bloomz)       | 560M/1.1B/1.7B/3B/7.1B/176B | query_key_value   | -         |
-| [ChatGLM3](https://huggingface.co/THUDM/chatglm3-6b)     | 6B                          | query_key_value   | chatglm3  |
+| [BLOOM](https://huggingface.co/bigscience)               | 560M/1.1B/1.7B/3B/7.1B/176B | query_key_value   | -         |
+| [BLOOMZ](https://huggingface.co/bigscience)              | 560M/1.1B/1.7B/3B/7.1B/176B | query_key_value   | -         |
+| [ChatGLM3](https://huggingface.co/THUDM)                 | 6B                          | query_key_value   | chatglm3  |
+| [Command-R](https://huggingface.co/CohereForAI)          | 35B/104B                    | q_proj,v_proj     | cohere    |
 | [DeepSeek (MoE)](https://huggingface.co/deepseek-ai)     | 7B/16B/67B                  | q_proj,v_proj     | deepseek  |
 | [Falcon](https://huggingface.co/tiiuae)                  | 7B/40B/180B                 | query_key_value   | falcon    |
-| [Gemma](https://huggingface.co/google)                   | 2B/7B                       | q_proj,v_proj     | gemma     |
+| [Gemma/CodeGemma](https://huggingface.co/google)         | 2B/7B                       | q_proj,v_proj     | gemma     |
 | [InternLM2](https://huggingface.co/internlm)             | 7B/20B                      | wqkv              | intern2   |
 | [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B              | q_proj,v_proj     | -         |
 | [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B                  | q_proj,v_proj     | llama2    |
-| [Mistral/Mixtral](https://huggingface.co/mistralai)      | 7B/8x7B                     | q_proj,v_proj     | mistral   |
+| [LLaMA-3](https://huggingface.co/meta-llama)             | 8B/70B                      | q_proj,v_proj     | llama3    |
+| [Mistral/Mixtral](https://huggingface.co/mistralai)      | 7B/8x7B/8x22B               | q_proj,v_proj     | mistral   |
 | [OLMo](https://huggingface.co/allenai)                   | 1B/7B                       | att_proj          | olmo      |
 | [Phi-1.5/2](https://huggingface.co/microsoft)            | 1.3B/2.7B                   | q_proj,v_proj     | -         |
 | [Qwen](https://huggingface.co/Qwen)                      | 1.8B/7B/14B/72B             | c_attn            | qwen      |
-| [Qwen1.5 (MoE)](https://huggingface.co/Qwen)             | 0.5B/1.8B/4B/7B/14B/32B/72B | q_proj,v_proj     | qwen      |
+| [Qwen1.5 (Code/MoE)](https://huggingface.co/Qwen)        | 0.5B/1.8B/4B/7B/14B/32B/72B | q_proj,v_proj     | qwen      |
 | [StarCoder2](https://huggingface.co/bigcode)             | 3B/7B/15B                   | q_proj,v_proj     | -         |
 | [XVERSE](https://huggingface.co/xverse)                  | 7B/13B/65B                  | q_proj,v_proj     | xverse    |
 | [Yi](https://huggingface.co/01-ai)                       | 6B/9B/34B                   | q_proj,v_proj     | yi        |
 | [Yuan](https://huggingface.co/IEITYuan)                  | 2B/51B/102B                 | q_proj,v_proj     | yuan      |
 
 > [!NOTE]
 > **Default module** is used for the `--lora_target` argument, you can use `--lora_target all` to specify all the available modules.
@@ -308,14 +320,15 @@
 <details><summary>Preference datasets</summary>
 
 - [HH-RLHF (en)](https://huggingface.co/datasets/Anthropic/hh-rlhf)
 - [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
 - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
 - [Orca DPO (en)](https://huggingface.co/datasets/Intel/orca_dpo_pairs)
 - [Nectar (en)](https://huggingface.co/datasets/berkeley-nest/Nectar)
+- [DPO mix (en&zh)](https://huggingface.co/datasets/hiyouga/DPO-En-Zh-20k)
 - [Orca DPO (de)](https://huggingface.co/datasets/mayflowergmbh/intel_orca_dpo_pairs_de)
 
 </details>
 
 Some datasets require confirmation before using them, so we recommend logging in with your Hugging Face account using these commands.
 
 ```bash
@@ -342,24 +355,23 @@
 | bitsandbytes | 0.39.0  | 0.43.0    |
 | flash-attn   | 2.3.0   | 2.5.6     |
 
 ### Hardware Requirement
 
 \* *estimated*
 
-| Method | Bits |   7B  |  13B  |  30B  |   70B  |   8x7B |
-| ------ | ---- | ----- | ----- | ----- | ------ | ------ |
-| Full   | AMP  | 120GB | 240GB | 600GB | 1200GB |  900GB |
-| Full   |  16  |  60GB | 120GB | 300GB |  600GB |  400GB |
-| GaLore |  16  |  16GB |  32GB |  64GB |  160GB |  120GB |
-| Freeze |  16  |  20GB |  40GB |  80GB |  200GB |  160GB |
-| LoRA   |  16  |  16GB |  32GB |  64GB |  160GB |  120GB |
-| QLoRA  |   8  |  10GB |  20GB |  40GB |   80GB |   60GB |
-| QLoRA  |   4  |   6GB |  12GB |  24GB |   48GB |   30GB |
-| QLoRA  |   2  |   4GB |   8GB |  16GB |   24GB |   18GB |
+| Method            | Bits |   7B  |  13B  |  30B  |   70B  |  8x7B |  8x22B |
+| ----------------- | ---- | ----- | ----- | ----- | ------ | ----- | ------ |
+| Full              | AMP  | 120GB | 240GB | 600GB | 1200GB | 900GB | 2400GB |
+| Full              |  16  |  60GB | 120GB | 300GB |  600GB | 400GB | 1200GB |
+| Freeze            |  16  |  20GB |  40GB |  80GB |  200GB | 160GB |  400GB |
+| LoRA/GaLore/BAdam |  16  |  16GB |  32GB |  64GB |  160GB | 120GB |  320GB |
+| QLoRA             |   8  |  10GB |  20GB |  40GB |   80GB |  60GB |  160GB |
+| QLoRA             |   4  |   6GB |  12GB |  24GB |   48GB |  30GB |   96GB |
+| QLoRA             |   2  |   4GB |   8GB |  16GB |   24GB |  18GB |   48GB |
 
 ## Getting Started
 
 ### Data Preparation
 
 Please refer to [data/README.md](data/README.md) for checking the details about the format of dataset files. You can either use datasets on HuggingFace / ModelScope hub or load the dataset in local disk.
 
@@ -372,15 +384,15 @@
 git clone https://github.com/hiyouga/LLaMA-Factory.git
 conda create -n llama_factory python=3.10
 conda activate llama_factory
 cd LLaMA-Factory
 pip install -e .[metrics]
 ```
 
-Extra dependencies available: deepspeed, metrics, unsloth, galore, vllm, bitsandbytes, gptq, awq, aqlm, qwen, modelscope, quality
+Extra dependencies available: deepspeed, metrics, unsloth, galore, badam, vllm, bitsandbytes, gptq, awq, aqlm, qwen, modelscope, quality
 
 <details><summary>For Windows users</summary>
 
 If you want to enable the quantized LoRA (QLoRA) on the Windows platform, you will be required to install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.2, please select the appropriate [release version](https://github.com/jllllll/bitsandbytes-windows-webui/releases/tag/wheels) based on your CUDA version.
 
 ```bash
 pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.41.2.post2-py3-none-win_amd64.whl
@@ -395,14 +407,15 @@
 > [!IMPORTANT]
 > LLaMA Board GUI only supports training on a single GPU, please use [CLI](#command-line-interface) for distributed training.
 
 #### Use local environment
 
 ```bash
 export CUDA_VISIBLE_DEVICES=0 # `set CUDA_VISIBLE_DEVICES=0` for Windows
+export GRADIO_SERVER_PORT=7860 # `set GRADIO_SERVER_PORT=7860` for Windows
 python src/train_web.py # or python -m llmtuner.webui.interface
 ```
 
 #### Use Docker
 
 ```bash
 docker build -f ./Dockerfile -t llama-factory:latest .
@@ -480,29 +493,35 @@
 1. Cao et al. Head-wise Shareable Attention for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.11819)
 1. Zhang et al. Enhancing Multilingual Capabilities of Large Language Models through Self-Distillation from Resource-Rich Languages. 2024. [[arxiv]](https://arxiv.org/abs/2402.12204)
 1. Kim et al. Efficient and Effective Vocabulary Expansion Towards Multilingual Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.14714)
 1. Yu et al. KIEval: A Knowledge-grounded Interactive Evaluation Framework for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.15043)
 1. Huang et al. Key-Point-Driven Data Synthesis with its Enhancement on Mathematical Reasoning. 2024. [[arxiv]](https://arxiv.org/abs/2403.02333)
 1. Duan et al. Negating Negatives: Alignment without Human Positive Samples via Distributional Dispreference Optimization. 2024. [[arxiv]](https://arxiv.org/abs/2403.03419)
 1. Xie and Schwertfeger. Empowering Robotics with Large Language Models: osmAG Map Comprehension with LLMs. 2024. [[arxiv]](https://arxiv.org/abs/2403.08228)
+1. Zhang et al. EDT: Improving Large Language Models' Generation by Entropy-based Dynamic Temperature Sampling. 2024. [[arxiv]](https://arxiv.org/abs/2403.14541)
 1. Weller et al. FollowIR: Evaluating and Teaching Information Retrieval Models to Follow Instructions. 2024. [[arxiv]](https://arxiv.org/abs/2403.15246)
 1. Hongbin Na. CBT-LLM: A Chinese Large Language Model for Cognitive Behavioral Therapy-based Mental Health Question Answering. 2024. [[arxiv]](https://arxiv.org/abs/2403.16008)
+1. Zan et al. CodeS: Natural Language to Code Repository via Multi-Layer Sketch. 2024. [[arxiv]](https://arxiv.org/abs/2403.16443)
+1. Liu et al. Extensive Self-Contrast Enables Feedback-Free Language Model Alignment. 2024. [[arxiv]](https://arxiv.org/abs/2404.00604)
+1. Luo et al. BAdam: A Memory Efficient Full Parameter Training Method for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2404.02827)
+1. Du et al. Chinese Tiny LLM: Pretraining a Chinese-Centric Large Language Model. 2024. [[arxiv]](https://arxiv.org/abs/2404.04167)
+1. Liu et al. Dynamic Generation of Personalities with Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2404.07084)
 1. **[StarWhisper](https://github.com/Yu-Yang-Li/StarWhisper)**: A large language model for Astronomy, based on ChatGLM2-6B and Qwen-14B.
 1. **[DISC-LawLLM](https://github.com/FudanDISC/DISC-LawLLM)**: A large language model specialized in Chinese legal domain, based on Baichuan-13B, is capable of retrieving and reasoning on legal knowledge.
 1. **[Sunsimiao](https://github.com/thomas-yanxin/Sunsimiao)**: A large language model specialized in Chinese medical domain, based on Baichuan-7B and ChatGLM-6B.
 1. **[CareGPT](https://github.com/WangRongsheng/CareGPT)**: A series of large language models for Chinese medical domain, based on LLaMA2-7B and Baichuan-13B.
 1. **[MachineMindset](https://github.com/PKU-YuanGroup/Machine-Mindset/)**: A series of MBTI Personality large language models, capable of giving any LLM 16 different personality types based on different datasets and training methods.
 
 </details>
 
 ## License
 
 This repository is licensed under the [Apache-2.0 License](LICENSE).
 
-Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2](https://ai.meta.com/llama/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
+Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [Command-R](https://cohere.com/c4ai-cc-by-nc-license) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2](https://ai.meta.com/llama/license/) / [LLaMA-3](https://llama.meta.com/llama3/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
 
 ## Citation
 
 If this work is helpful, please kindly cite as:
 
 ```bibtex
 @article{zheng2024llamafactory,
```

### Comparing `llmtuner-0.6.2/README.md` & `llmtuner-0.6.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ![# LLaMA Factory](assets/logo.png)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Factory?style=social)](https://github.com/hiyouga/LLaMA-Factory/stargazers)
 [![GitHub Code License](https://img.shields.io/github/license/hiyouga/LLaMA-Factory)](LICENSE)
 [![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Factory)](https://github.com/hiyouga/LLaMA-Factory/commits/main)
 [![PyPI](https://img.shields.io/pypi/v/llmtuner)](https://pypi.org/project/llmtuner/)
 [![Downloads](https://static.pepy.tech/badge/llmtuner)](https://pypi.org/project/llmtuner/)
-[![Citation](https://img.shields.io/badge/citation-28-green)](#projects-using-llama-factory)
+[![Citation](https://img.shields.io/badge/citation-34-green)](#projects-using-llama-factory)
 [![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/LLaMA-Factory/pulls)
 [![Discord](https://dcbadge.vercel.app/api/server/rKfvV9r9FK?compact=true&style=flat)](https://discord.gg/rKfvV9r9FK)
 [![Twitter](https://img.shields.io/twitter/follow/llamafactory_ai)](https://twitter.com/llamafactory_ai)
 [![Spaces](https://img.shields.io/badge/🤗-Open%20in%20Spaces-blue)](https://huggingface.co/spaces/hiyouga/LLaMA-Board)
 [![Studios](https://img.shields.io/badge/ModelScope-Open%20in%20Studios-blue)](https://modelscope.cn/studios/hiyouga/LLaMA-Board)
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eRTPn37ltBbYsISy9Aw2NuI2Aq5CQrD9?usp=sharing)
 
@@ -42,15 +42,15 @@
 - [Acknowledgement](#acknowledgement)
 
 ## Features
 
 - **Various models**: LLaMA, Mistral, Mixtral-MoE, Qwen, Yi, Gemma, Baichuan, ChatGLM, Phi, etc.
 - **Integrated methods**: (Continuous) pre-training, supervised fine-tuning, reward modeling, PPO, DPO and ORPO.
 - **Scalable resources**: 32-bit full-tuning, 16-bit freeze-tuning, 16-bit LoRA and 2/4/8-bit QLoRA via AQLM/AWQ/GPTQ/LLM.int8.
-- **Advanced algorithms**: GaLore, DoRA, LongLoRA, LLaMA Pro, LoRA+, LoftQ and Agent tuning.
+- **Advanced algorithms**: GaLore, BAdam, DoRA, LongLoRA, LLaMA Pro, Mixture-of-Depths, LoRA+, LoftQ and Agent tuning.
 - **Practical tricks**: FlashAttention-2, Unsloth, RoPE scaling, NEFTune and rsLoRA.
 - **Experiment monitors**: LlamaBoard, TensorBoard, Wandb, MLflow, etc.
 - **Faster inference**: OpenAI-style API, Gradio UI and CLI with vLLM worker.
 
 ## Benchmark
 
 Compared to ChatGLM's [P-Tuning](https://github.com/THUDM/ChatGLM2-6B/tree/main/ptuning), LLaMA Factory's LoRA tuning offers up to **3.7 times faster** training speed with a better Rouge score on the advertising text generation task. By leveraging 4-bit quantization technique, LLaMA Factory's QLoRA further improves the efficiency regarding the GPU memory.
@@ -64,22 +64,30 @@
 - **GPU Memory**: Peak GPU memory usage in 4-bit quantized training. (bs=1, cutoff_len=1024)
 - We adopt `pre_seq_len=128` for ChatGLM's P-Tuning and `lora_rank=32` for LLaMA Factory's LoRA tuning.
 
 </details>
 
 ## Changelog
 
+[24/04/21] We supported **[Mixture-of-Depths](https://arxiv.org/abs/2404.02258)** according to [AstraMindAI's implementation](https://github.com/astramind-ai/Mixture-of-depths). See `examples/extras/mod` for usage.
+
+[24/04/19] We supported **Meta Llama 3** model series.
+
+[24/04/16] We supported **[BAdam](https://arxiv.org/abs/2404.02827)**. See `examples/extras/badam` for usage.
+
+[24/04/16] We supported **[unsloth](https://github.com/unslothai/unsloth)**'s long-sequence training (Llama-2-7B-56k within 24GB). It achieves **117%** speed and **50%** memory compared with FlashAttention-2, more benchmarks can be found in [this page](https://github.com/hiyouga/LLaMA-Factory/wiki/Performance-comparison).
+
+<details><summary>Full Changelog</summary>
+
 [24/03/31] We supported **[ORPO](https://arxiv.org/abs/2403.07691)**. See `examples/lora_single_gpu` for usage.
 
 [24/03/21] Our paper "[LlamaFactory: Unified Efficient Fine-Tuning of 100+ Language Models](https://arxiv.org/abs/2403.13372)" is available at arXiv!
 
 [24/03/20] We supported **FSDP+QLoRA** that fine-tunes a 70B model on 2x24GB GPUs. See `examples/extras/fsdp_qlora` for usage.
 
-<details><summary>Full Changelog</summary>
-
 [24/03/13] We supported **[LoRA+](https://arxiv.org/abs/2402.12354)**. See `examples/extras/loraplus` for usage.
 
 [24/03/07] We supported gradient low-rank projection (**[GaLore](https://arxiv.org/abs/2403.03507)**) algorithm. See `examples/extras/galore` for usage.
 
 [24/03/07] We integrated **[vLLM](https://github.com/vllm-project/vllm)** for faster and concurrent inference. Try `--infer_backend vllm` to enjoy **270%** inference speed. (LoRA is not yet supported, merge it first.)
 
 [24/02/28] We supported weight-decomposed LoRA (**[DoRA](https://arxiv.org/abs/2402.09353)**). Try `--use_dora` to activate DoRA training.
@@ -125,28 +133,30 @@
 </details>
 
 ## Supported Models
 
 | Model                                                    | Model size                  | Default module    | Template  |
 | -------------------------------------------------------- | --------------------------- | ----------------- | --------- |
 | [Baichuan2](https://huggingface.co/baichuan-inc)         | 7B/13B                      | W_pack            | baichuan2 |
-| [BLOOM](https://huggingface.co/bigscience/bloom)         | 560M/1.1B/1.7B/3B/7.1B/176B | query_key_value   | -         |
-| [BLOOMZ](https://huggingface.co/bigscience/bloomz)       | 560M/1.1B/1.7B/3B/7.1B/176B | query_key_value   | -         |
-| [ChatGLM3](https://huggingface.co/THUDM/chatglm3-6b)     | 6B                          | query_key_value   | chatglm3  |
+| [BLOOM](https://huggingface.co/bigscience)               | 560M/1.1B/1.7B/3B/7.1B/176B | query_key_value   | -         |
+| [BLOOMZ](https://huggingface.co/bigscience)              | 560M/1.1B/1.7B/3B/7.1B/176B | query_key_value   | -         |
+| [ChatGLM3](https://huggingface.co/THUDM)                 | 6B                          | query_key_value   | chatglm3  |
+| [Command-R](https://huggingface.co/CohereForAI)          | 35B/104B                    | q_proj,v_proj     | cohere    |
 | [DeepSeek (MoE)](https://huggingface.co/deepseek-ai)     | 7B/16B/67B                  | q_proj,v_proj     | deepseek  |
 | [Falcon](https://huggingface.co/tiiuae)                  | 7B/40B/180B                 | query_key_value   | falcon    |
-| [Gemma](https://huggingface.co/google)                   | 2B/7B                       | q_proj,v_proj     | gemma     |
+| [Gemma/CodeGemma](https://huggingface.co/google)         | 2B/7B                       | q_proj,v_proj     | gemma     |
 | [InternLM2](https://huggingface.co/internlm)             | 7B/20B                      | wqkv              | intern2   |
 | [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B              | q_proj,v_proj     | -         |
 | [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B                  | q_proj,v_proj     | llama2    |
-| [Mistral/Mixtral](https://huggingface.co/mistralai)      | 7B/8x7B                     | q_proj,v_proj     | mistral   |
+| [LLaMA-3](https://huggingface.co/meta-llama)             | 8B/70B                      | q_proj,v_proj     | llama3    |
+| [Mistral/Mixtral](https://huggingface.co/mistralai)      | 7B/8x7B/8x22B               | q_proj,v_proj     | mistral   |
 | [OLMo](https://huggingface.co/allenai)                   | 1B/7B                       | att_proj          | olmo      |
 | [Phi-1.5/2](https://huggingface.co/microsoft)            | 1.3B/2.7B                   | q_proj,v_proj     | -         |
 | [Qwen](https://huggingface.co/Qwen)                      | 1.8B/7B/14B/72B             | c_attn            | qwen      |
-| [Qwen1.5 (MoE)](https://huggingface.co/Qwen)             | 0.5B/1.8B/4B/7B/14B/32B/72B | q_proj,v_proj     | qwen      |
+| [Qwen1.5 (Code/MoE)](https://huggingface.co/Qwen)        | 0.5B/1.8B/4B/7B/14B/32B/72B | q_proj,v_proj     | qwen      |
 | [StarCoder2](https://huggingface.co/bigcode)             | 3B/7B/15B                   | q_proj,v_proj     | -         |
 | [XVERSE](https://huggingface.co/xverse)                  | 7B/13B/65B                  | q_proj,v_proj     | xverse    |
 | [Yi](https://huggingface.co/01-ai)                       | 6B/9B/34B                   | q_proj,v_proj     | yi        |
 | [Yuan](https://huggingface.co/IEITYuan)                  | 2B/51B/102B                 | q_proj,v_proj     | yuan      |
 
 > [!NOTE]
 > **Default module** is used for the `--lora_target` argument, you can use `--lora_target all` to specify all the available modules.
@@ -237,14 +247,15 @@
 <details><summary>Preference datasets</summary>
 
 - [HH-RLHF (en)](https://huggingface.co/datasets/Anthropic/hh-rlhf)
 - [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
 - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
 - [Orca DPO (en)](https://huggingface.co/datasets/Intel/orca_dpo_pairs)
 - [Nectar (en)](https://huggingface.co/datasets/berkeley-nest/Nectar)
+- [DPO mix (en&zh)](https://huggingface.co/datasets/hiyouga/DPO-En-Zh-20k)
 - [Orca DPO (de)](https://huggingface.co/datasets/mayflowergmbh/intel_orca_dpo_pairs_de)
 
 </details>
 
 Some datasets require confirmation before using them, so we recommend logging in with your Hugging Face account using these commands.
 
 ```bash
@@ -271,24 +282,23 @@
 | bitsandbytes | 0.39.0  | 0.43.0    |
 | flash-attn   | 2.3.0   | 2.5.6     |
 
 ### Hardware Requirement
 
 \* *estimated*
 
-| Method | Bits |   7B  |  13B  |  30B  |   70B  |   8x7B |
-| ------ | ---- | ----- | ----- | ----- | ------ | ------ |
-| Full   | AMP  | 120GB | 240GB | 600GB | 1200GB |  900GB |
-| Full   |  16  |  60GB | 120GB | 300GB |  600GB |  400GB |
-| GaLore |  16  |  16GB |  32GB |  64GB |  160GB |  120GB |
-| Freeze |  16  |  20GB |  40GB |  80GB |  200GB |  160GB |
-| LoRA   |  16  |  16GB |  32GB |  64GB |  160GB |  120GB |
-| QLoRA  |   8  |  10GB |  20GB |  40GB |   80GB |   60GB |
-| QLoRA  |   4  |   6GB |  12GB |  24GB |   48GB |   30GB |
-| QLoRA  |   2  |   4GB |   8GB |  16GB |   24GB |   18GB |
+| Method            | Bits |   7B  |  13B  |  30B  |   70B  |  8x7B |  8x22B |
+| ----------------- | ---- | ----- | ----- | ----- | ------ | ----- | ------ |
+| Full              | AMP  | 120GB | 240GB | 600GB | 1200GB | 900GB | 2400GB |
+| Full              |  16  |  60GB | 120GB | 300GB |  600GB | 400GB | 1200GB |
+| Freeze            |  16  |  20GB |  40GB |  80GB |  200GB | 160GB |  400GB |
+| LoRA/GaLore/BAdam |  16  |  16GB |  32GB |  64GB |  160GB | 120GB |  320GB |
+| QLoRA             |   8  |  10GB |  20GB |  40GB |   80GB |  60GB |  160GB |
+| QLoRA             |   4  |   6GB |  12GB |  24GB |   48GB |  30GB |   96GB |
+| QLoRA             |   2  |   4GB |   8GB |  16GB |   24GB |  18GB |   48GB |
 
 ## Getting Started
 
 ### Data Preparation
 
 Please refer to [data/README.md](data/README.md) for checking the details about the format of dataset files. You can either use datasets on HuggingFace / ModelScope hub or load the dataset in local disk.
 
@@ -301,15 +311,15 @@
 git clone https://github.com/hiyouga/LLaMA-Factory.git
 conda create -n llama_factory python=3.10
 conda activate llama_factory
 cd LLaMA-Factory
 pip install -e .[metrics]
 ```
 
-Extra dependencies available: deepspeed, metrics, unsloth, galore, vllm, bitsandbytes, gptq, awq, aqlm, qwen, modelscope, quality
+Extra dependencies available: deepspeed, metrics, unsloth, galore, badam, vllm, bitsandbytes, gptq, awq, aqlm, qwen, modelscope, quality
 
 <details><summary>For Windows users</summary>
 
 If you want to enable the quantized LoRA (QLoRA) on the Windows platform, you will be required to install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.2, please select the appropriate [release version](https://github.com/jllllll/bitsandbytes-windows-webui/releases/tag/wheels) based on your CUDA version.
 
 ```bash
 pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.41.2.post2-py3-none-win_amd64.whl
@@ -324,14 +334,15 @@
 > [!IMPORTANT]
 > LLaMA Board GUI only supports training on a single GPU, please use [CLI](#command-line-interface) for distributed training.
 
 #### Use local environment
 
 ```bash
 export CUDA_VISIBLE_DEVICES=0 # `set CUDA_VISIBLE_DEVICES=0` for Windows
+export GRADIO_SERVER_PORT=7860 # `set GRADIO_SERVER_PORT=7860` for Windows
 python src/train_web.py # or python -m llmtuner.webui.interface
 ```
 
 #### Use Docker
 
 ```bash
 docker build -f ./Dockerfile -t llama-factory:latest .
@@ -409,29 +420,35 @@
 1. Cao et al. Head-wise Shareable Attention for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.11819)
 1. Zhang et al. Enhancing Multilingual Capabilities of Large Language Models through Self-Distillation from Resource-Rich Languages. 2024. [[arxiv]](https://arxiv.org/abs/2402.12204)
 1. Kim et al. Efficient and Effective Vocabulary Expansion Towards Multilingual Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.14714)
 1. Yu et al. KIEval: A Knowledge-grounded Interactive Evaluation Framework for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.15043)
 1. Huang et al. Key-Point-Driven Data Synthesis with its Enhancement on Mathematical Reasoning. 2024. [[arxiv]](https://arxiv.org/abs/2403.02333)
 1. Duan et al. Negating Negatives: Alignment without Human Positive Samples via Distributional Dispreference Optimization. 2024. [[arxiv]](https://arxiv.org/abs/2403.03419)
 1. Xie and Schwertfeger. Empowering Robotics with Large Language Models: osmAG Map Comprehension with LLMs. 2024. [[arxiv]](https://arxiv.org/abs/2403.08228)
+1. Zhang et al. EDT: Improving Large Language Models' Generation by Entropy-based Dynamic Temperature Sampling. 2024. [[arxiv]](https://arxiv.org/abs/2403.14541)
 1. Weller et al. FollowIR: Evaluating and Teaching Information Retrieval Models to Follow Instructions. 2024. [[arxiv]](https://arxiv.org/abs/2403.15246)
 1. Hongbin Na. CBT-LLM: A Chinese Large Language Model for Cognitive Behavioral Therapy-based Mental Health Question Answering. 2024. [[arxiv]](https://arxiv.org/abs/2403.16008)
+1. Zan et al. CodeS: Natural Language to Code Repository via Multi-Layer Sketch. 2024. [[arxiv]](https://arxiv.org/abs/2403.16443)
+1. Liu et al. Extensive Self-Contrast Enables Feedback-Free Language Model Alignment. 2024. [[arxiv]](https://arxiv.org/abs/2404.00604)
+1. Luo et al. BAdam: A Memory Efficient Full Parameter Training Method for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2404.02827)
+1. Du et al. Chinese Tiny LLM: Pretraining a Chinese-Centric Large Language Model. 2024. [[arxiv]](https://arxiv.org/abs/2404.04167)
+1. Liu et al. Dynamic Generation of Personalities with Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2404.07084)
 1. **[StarWhisper](https://github.com/Yu-Yang-Li/StarWhisper)**: A large language model for Astronomy, based on ChatGLM2-6B and Qwen-14B.
 1. **[DISC-LawLLM](https://github.com/FudanDISC/DISC-LawLLM)**: A large language model specialized in Chinese legal domain, based on Baichuan-13B, is capable of retrieving and reasoning on legal knowledge.
 1. **[Sunsimiao](https://github.com/thomas-yanxin/Sunsimiao)**: A large language model specialized in Chinese medical domain, based on Baichuan-7B and ChatGLM-6B.
 1. **[CareGPT](https://github.com/WangRongsheng/CareGPT)**: A series of large language models for Chinese medical domain, based on LLaMA2-7B and Baichuan-13B.
 1. **[MachineMindset](https://github.com/PKU-YuanGroup/Machine-Mindset/)**: A series of MBTI Personality large language models, capable of giving any LLM 16 different personality types based on different datasets and training methods.
 
 </details>
 
 ## License
 
 This repository is licensed under the [Apache-2.0 License](LICENSE).
 
-Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2](https://ai.meta.com/llama/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
+Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [Command-R](https://cohere.com/c4ai-cc-by-nc-license) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2](https://ai.meta.com/llama/license/) / [LLaMA-3](https://llama.meta.com/llama3/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
 
 ## Citation
 
 If this work is helpful, please kindly cite as:
 
 ```bibtex
 @article{zheng2024llamafactory,
```

### Comparing `llmtuner-0.6.2/pyproject.toml` & `llmtuner-0.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/setup.py` & `llmtuner-0.6.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 
 extra_require = {
     "deepspeed": ["deepspeed>=0.10.0"],
     "metrics": ["nltk", "jieba", "rouge-chinese"],
     "unsloth": ["torch==2.2.0", "unsloth[cu121-ampere-torch220]"],
     "galore": ["galore-torch"],
+    "badam": ["badam"],
     "vllm": ["vllm>=0.3.3"],
     "bitsandbytes": ["bitsandbytes>=0.39.0"],
     "gptq": ["optimum>=1.16.0", "auto-gptq>=0.5.0"],
     "awq": ["autoawq"],
     "aqlm": ["aqlm[gpu]>=1.1.0"],
     "qwen": ["tiktoken", "transformers_stream_generator"],
     "modelscope": ["modelscope"],
```

### Comparing `llmtuner-0.6.2/src/llmtuner/api/app.py` & `llmtuner-0.6.3/src/llmtuner/api/app.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/api/protocol.py` & `llmtuner-0.6.3/src/llmtuner/api/protocol.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/chat/base_engine.py` & `llmtuner-0.6.3/src/llmtuner/chat/base_engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, AsyncGenerator, Dict, List, Literal, Optional, Sequence, Union
 
 
 if TYPE_CHECKING:
     from transformers import PreTrainedModel, PreTrainedTokenizer
+    from vllm import AsyncLLMEngine
 
     from ..data import Template
-    from ..extras.packages import is_vllm_available
     from ..hparams import DataArguments, FinetuningArguments, GeneratingArguments, ModelArguments
 
-    if is_vllm_available():
-        from vllm import AsyncLLMEngine
-
 
 @dataclass
 class Response:
     response_text: str
     response_length: int
     prompt_length: int
     finish_reason: Literal["stop", "length"]
```

### Comparing `llmtuner-0.6.2/src/llmtuner/chat/chat_model.py` & `llmtuner-0.6.3/src/llmtuner/chat/chat_model.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/chat/hf_engine.py` & `llmtuner-0.6.3/src/llmtuner/chat/hf_engine.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/chat/vllm_engine.py` & `llmtuner-0.6.3/src/llmtuner/chat/vllm_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import uuid
 from typing import TYPE_CHECKING, AsyncGenerator, AsyncIterator, Dict, List, Optional, Sequence
 
-from transformers.utils.versions import require_version
-
 from ..data import get_template_and_fix_tokenizer
 from ..extras.misc import get_device_count
 from ..extras.packages import is_vllm_available
 from ..model import load_tokenizer
 from .base_engine import BaseEngine, Response
 
 
@@ -21,15 +19,14 @@
     def __init__(
         self,
         model_args: "ModelArguments",
         data_args: "DataArguments",
         finetuning_args: "FinetuningArguments",
         generating_args: "GeneratingArguments",
     ) -> None:
-        require_version("vllm>=0.3.3", "To fix: pip install vllm>=0.3.3")
         self.can_generate = finetuning_args.stage == "sft"
         engine_args = AsyncEngineArgs(
             model=model_args.model_name_or_path,
             trust_remote_code=True,
             max_model_len=model_args.vllm_maxlen,
             tensor_parallel_size=get_device_count() or 1,
             gpu_memory_utilization=model_args.vllm_gpu_util,
```

### Comparing `llmtuner-0.6.2/src/llmtuner/data/aligner.py` & `llmtuner-0.6.3/src/llmtuner/data/aligner.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/data/collator.py` & `llmtuner-0.6.3/src/llmtuner/data/collator.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/data/formatter.py` & `llmtuner-0.6.3/src/llmtuner/data/formatter.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/data/loader.py` & `llmtuner-0.6.3/src/llmtuner/data/loader.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/data/parser.py` & `llmtuner-0.6.3/src/llmtuner/data/parser.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/data/preprocess.py` & `llmtuner-0.6.3/src/llmtuner/data/preprocess.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/data/template.py` & `llmtuner-0.6.3/src/llmtuner/data/template.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,15 +339,15 @@
 
 
 def get_template_and_fix_tokenizer(
     tokenizer: "PreTrainedTokenizer",
     name: Optional[str] = None,
 ) -> Template:
     if name is None:
-        template = templates["vanilla"]  # placeholder
+        template = templates["empty"]  # placeholder
     else:
         template = templates.get(name, None)
         if template is None:
             raise ValueError("Template {} does not exist.".format(name))
 
     stop_words = template.stop_words
     if template.replace_eos:
@@ -381,15 +381,16 @@
 
 
 _register_template(
     name="alpaca",
     format_user=StringFormatter(slots=["### Instruction:\n{{content}}\n\n### Response:\n"]),
     format_separator=EmptyFormatter(slots=["\n\n"]),
     default_system=(
-        "Below is an instruction that describes a task. " "Write a response that appropriately completes the request."
+        "Below is an instruction that describes a task. "
+        "Write a response that appropriately completes the request.\n\n"
     ),
 )
 
 
 _register_template(
     name="aquila",
     format_user=StringFormatter(slots=["Human: {{content}}###Assistant:"]),
@@ -523,14 +524,29 @@
     name="codegeex2",
     format_system=StringFormatter(slots=[{"token": "[gMASK]"}, {"token": "sop"}, "{{content}}"]),
     force_system=True,
 )
 
 
 _register_template(
+    name="cohere",
+    format_user=StringFormatter(
+        slots=[
+            (
+                "<|START_OF_TURN_TOKEN|><|USER_TOKEN|>{{content}}<|END_OF_TURN_TOKEN|>"
+                "<|START_OF_TURN_TOKEN|><|CHATBOT_TOKEN|>"
+            )
+        ]
+    ),
+    format_system=EmptyFormatter(slots=[{"bos_token"}]),
+    force_system=True,
+)
+
+
+_register_template(
     name="cpm",
     format_user=StringFormatter(slots=["<用户>{{content}}<AI>"]),
     format_system=StringFormatter(slots=[{"bos_token"}, "{{content}}"]),
     force_system=True,
 )
 
 
@@ -563,22 +579,36 @@
     format_user=StringFormatter(slots=["Human: {{content}}\nAssistant: "]),
     format_system=StringFormatter(slots=["{{content}}\n"]),
     format_separator=EmptyFormatter(slots=["\n"]),
 )
 
 
 _register_template(
+    name="empty",
+    format_user=StringFormatter(slots=["{{content}}"]),
+    format_assistant=StringFormatter(slots=["{{content}}"]),
+)
+
+
+_register_template(
     name="falcon",
     format_user=StringFormatter(slots=["User: {{content}}\nFalcon:"]),
     format_separator=EmptyFormatter(slots=["\n"]),
     efficient_eos=True,
 )
 
 
 _register_template(
+    name="fewshot",
+    format_separator=EmptyFormatter(slots=["\n\n"]),
+    efficient_eos=True,
+)
+
+
+_register_template(
     name="gemma",
     format_user=StringFormatter(slots=["<start_of_turn>user\n{{content}}<end_of_turn>\n<start_of_turn>model\n"]),
     format_system=StringFormatter(slots=[{"bos_token"}, "{{content}}"]),
     format_separator=EmptyFormatter(slots=["<end_of_turn>\n"]),
     efficient_eos=True,
     force_system=True,
 )
@@ -632,16 +662,35 @@
     format_user=StringFormatter(slots=[{"bos_token"}, "[INST] {{content}} [/INST]"]),
     format_system=StringFormatter(slots=["<<SYS>>\n{{content}}\n<</SYS>>\n\n"]),
     default_system="You are a helpful assistant. 你是一个乐于助人的助手。",
 )
 
 
 _register_template(
+    name="llama3",
+    format_user=StringFormatter(
+        slots=[
+            (
+                "<|start_header_id|>user<|end_header_id|>\n\n{{content}}<|eot_id|>"
+                "<|start_header_id|>assistant<|end_header_id|>\n\n"
+            )
+        ]
+    ),
+    format_system=StringFormatter(
+        slots=[{"bos_token"}, "<|start_header_id|>system<|end_header_id|>\n\n{{content}}<|eot_id|>"]
+    ),
+    default_system="You are a helpful assistant.",
+    stop_words=["<|eot_id|>"],
+    replace_eos=True,
+)
+
+
+_register_template(
     name="mistral",
-    format_user=StringFormatter(slots=["[INST] {{content}} [/INST]"]),
+    format_user=StringFormatter(slots=[" [INST] {{content}} [/INST]"]),
     format_system=StringFormatter(slots=[{"bos_token"}, "{{content}}"]),
     force_system=True,
 )
 
 
 _register_template(
     name="olmo",
@@ -696,21 +745,14 @@
     stop_words=["<|end|>"],
     replace_eos=True,
     force_system=True,
 )
 
 
 _register_template(
-    name="vanilla",
-    format_separator=EmptyFormatter(slots=["\n"]),
-    efficient_eos=True,
-)
-
-
-_register_template(
     name="vicuna",
     format_user=StringFormatter(slots=["USER: {{content}} ASSISTANT:"]),
     default_system=(
         "A chat between a curious user and an artificial intelligence assistant. "
         "The assistant gives helpful, detailed, and polite answers to the user's questions."
     ),
 )
```

### Comparing `llmtuner-0.6.2/src/llmtuner/data/utils.py` & `llmtuner-0.6.3/src/llmtuner/data/utils.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/eval/evaluator.py` & `llmtuner-0.6.3/src/llmtuner/eval/evaluator.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/eval/template.py` & `llmtuner-0.6.3/src/llmtuner/eval/template.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/extras/callbacks.py` & `llmtuner-0.6.3/src/llmtuner/extras/callbacks.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/extras/constants.py` & `llmtuner-0.6.3/src/llmtuner/extras/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 
 LAYERNORM_NAMES = {"norm", "ln"}
 
 LOG_FILE_NAME = "trainer_log.jsonl"
 
 METHODS = ["full", "freeze", "lora"]
 
+MOD_SUPPORTED_MODELS = ["bloom", "falcon", "gemma", "llama", "mistral", "mixtral", "phi", "starcoder2"]
+
 PEFT_METHODS = ["lora"]
 
 SUBJECTS = ["Average", "STEM", "Social Sciences", "Humanities", "Other"]
 
 SUPPORTED_MODELS = OrderedDict()
 
 TRAINING_STAGES = {
@@ -240,14 +242,36 @@
     },
     template="llama2_zh",
 )
 
 
 register_model_group(
     models={
+        "CommandR-35B-Chat": {
+            DownloadSource.DEFAULT: "CohereForAI/c4ai-command-r-v01",
+            DownloadSource.MODELSCOPE: "AI-ModelScope/c4ai-command-r-v01",
+        },
+        "CommandR-Plus-104B-Chat": {
+            DownloadSource.DEFAULT: "CohereForAI/c4ai-command-r-plus",
+            DownloadSource.MODELSCOPE: "AI-ModelScope/c4ai-command-r-plus",
+        },
+        "CommandR-35B-4bit-Chat": {
+            DownloadSource.DEFAULT: "CohereForAI/c4ai-command-r-v01-4bit",
+            DownloadSource.MODELSCOPE: "mirror013/c4ai-command-r-v01-4bit",
+        },
+        "CommandR-Plus-104B-4bit-Chat": {
+            DownloadSource.DEFAULT: "CohereForAI/c4ai-command-r-plus-4bit",
+        },
+    },
+    template="cohere",
+)
+
+
+register_model_group(
+    models={
         "DeepSeek-LLM-7B-Base": {
             DownloadSource.DEFAULT: "deepseek-ai/deepseek-llm-7b-base",
             DownloadSource.MODELSCOPE: "deepseek-ai/deepseek-llm-7b-base",
         },
         "DeepSeek-LLM-67B-Base": {
             DownloadSource.DEFAULT: "deepseek-ai/deepseek-llm-67b-base",
             DownloadSource.MODELSCOPE: "deepseek-ai/deepseek-llm-67b-base",
@@ -361,14 +385,31 @@
     },
     template="gemma",
 )
 
 
 register_model_group(
     models={
+        "CodeGemma-2B": {
+            DownloadSource.DEFAULT: "google/codegemma-2b",
+        },
+        "CodeGemma-7B": {
+            DownloadSource.DEFAULT: "google/codegemma-7b",
+        },
+        "CodeGemma-7B-Chat": {
+            DownloadSource.DEFAULT: "google/codegemma-7b-it",
+            DownloadSource.MODELSCOPE: "AI-ModelScope/codegemma-7b-it",
+        },
+    },
+    template="gemma",
+)
+
+
+register_model_group(
+    models={
         "InternLM-7B": {
             DownloadSource.DEFAULT: "internlm/internlm-7b",
             DownloadSource.MODELSCOPE: "Shanghai_AI_Laboratory/internlm-7b",
         },
         "InternLM-20B": {
             DownloadSource.DEFAULT: "internlm/internlm-20b",
             DownloadSource.MODELSCOPE: "Shanghai_AI_Laboratory/internlm-20b",
@@ -472,14 +513,37 @@
     },
     template="llama2",
 )
 
 
 register_model_group(
     models={
+        "LLaMA3-8B": {
+            DownloadSource.DEFAULT: "meta-llama/Meta-Llama-3-8B",
+            DownloadSource.MODELSCOPE: "LLM-Research/Meta-Llama-3-8B",
+        },
+        "LLaMA3-70B": {
+            DownloadSource.DEFAULT: "meta-llama/Meta-Llama-3-70B",
+            DownloadSource.MODELSCOPE: "LLM-Research/Meta-Llama-3-70B",
+        },
+        "LLaMA3-8B-Chat": {
+            DownloadSource.DEFAULT: "meta-llama/Meta-Llama-3-8B-Instruct",
+            DownloadSource.MODELSCOPE: "LLM-Research/Meta-Llama-3-8B-Instruct",
+        },
+        "LLaMA3-70B-Chat": {
+            DownloadSource.DEFAULT: "meta-llama/Meta-Llama-3-70B-Instruct",
+            DownloadSource.MODELSCOPE: "LLM-Research/Meta-Llama-3-70B-Instruct",
+        },
+    },
+    template="llama3",
+)
+
+
+register_model_group(
+    models={
         "Mistral-7B-v0.1": {
             DownloadSource.DEFAULT: "mistralai/Mistral-7B-v0.1",
             DownloadSource.MODELSCOPE: "AI-ModelScope/Mistral-7B-v0.1",
         },
         "Mistral-7B-v0.1-Chat": {
             DownloadSource.DEFAULT: "mistralai/Mistral-7B-Instruct-v0.1",
             DownloadSource.MODELSCOPE: "AI-ModelScope/Mistral-7B-Instruct-v0.1",
@@ -495,22 +559,28 @@
     },
     template="mistral",
 )
 
 
 register_model_group(
     models={
-        "Mixtral-8x7B": {
+        "Mixtral-8x7B-v0.1": {
             DownloadSource.DEFAULT: "mistralai/Mixtral-8x7B-v0.1",
             DownloadSource.MODELSCOPE: "AI-ModelScope/Mixtral-8x7B-v0.1",
         },
-        "Mixtral-8x7B-Chat": {
+        "Mixtral-8x7B-v0.1-Chat": {
             DownloadSource.DEFAULT: "mistralai/Mixtral-8x7B-Instruct-v0.1",
             DownloadSource.MODELSCOPE: "AI-ModelScope/Mixtral-8x7B-Instruct-v0.1",
         },
+        "Mixtral-8x22B-v0.1": {
+            DownloadSource.DEFAULT: "mistralai/Mixtral-8x22B-v0.1",
+        },
+        "Mixtral-8x22B-v0.1-Chat": {
+            DownloadSource.DEFAULT: "mistralai/Mixtral-8x22B-Instruct-v0.1",
+        },
     },
     template="mistral",
 )
 
 
 register_model_group(
     models={
@@ -684,14 +754,18 @@
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-72B",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-72B",
         },
         "Qwen1.5-MoE-A2.7B": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-MoE-A2.7B",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-MoE-A2.7B",
         },
+        "Qwen1.5-Code-7B": {
+            DownloadSource.DEFAULT: "Qwen/CodeQwen1.5-7B",
+            DownloadSource.MODELSCOPE: "qwen/CodeQwen1.5-7B",
+        },
         "Qwen1.5-0.5B-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-0.5B-Chat",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-0.5B-Chat",
         },
         "Qwen1.5-1.8B-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-1.8B-Chat",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-1.8B-Chat",
@@ -716,14 +790,18 @@
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-72B-Chat",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-72B-Chat",
         },
         "Qwen1.5-MoE-A2.7B-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-MoE-A2.7B-Chat",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-MoE-A2.7B-Chat",
         },
+        "Qwen1.5-Code-7B-Chat": {
+            DownloadSource.DEFAULT: "Qwen/CodeQwen1.5-7B-Chat",
+            DownloadSource.MODELSCOPE: "qwen/CodeQwen1.5-7B-Chat",
+        },
         "Qwen1.5-0.5B-int8-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-0.5B-Chat-GPTQ-Int8",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-0.5B-Chat-GPTQ-Int8",
         },
         "Qwen1.5-0.5B-int4-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-0.5B-Chat-AWQ",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-0.5B-Chat-AWQ",
@@ -772,14 +850,18 @@
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-72B-Chat-AWQ",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-72B-Chat-AWQ",
         },
         "Qwen1.5-MoE-A2.7B-int4-Chat": {
             DownloadSource.DEFAULT: "Qwen/Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4",
             DownloadSource.MODELSCOPE: "qwen/Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4",
         },
+        "Qwen1.5-Code-7B-int4-Chat": {
+            DownloadSource.DEFAULT: "Qwen/CodeQwen1.5-7B-Chat-AWQ",
+            DownloadSource.MODELSCOPE: "qwen/CodeQwen1.5-7B-Chat-AWQ",
+        },
     },
     template="qwen",
 )
 
 
 register_model_group(
     models={
@@ -975,22 +1057,7 @@
         "Zephyr-7B-Beta-Chat": {
             DownloadSource.DEFAULT: "HuggingFaceH4/zephyr-7b-beta",
             DownloadSource.MODELSCOPE: "modelscope/zephyr-7b-beta",
         },
     },
     template="zephyr",
 )
-
-
-register_model_group(
-    models={
-        "Atom-7B": {
-            DownloadSource.DEFAULT: "FlagAlpha/Atom-7B",
-            DownloadSource.MODELSCOPE: "FlagAlpha/Atom-7B",
-        },
-        "Atom-7B-Chat": {
-            DownloadSource.DEFAULT: "FlagAlpha/Atom-7B-Chat",
-            DownloadSource.MODELSCOPE: "FlagAlpha/Atom-7B-Chat",
-        },
-    },
-    template="atom",
-)
```

### Comparing `llmtuner-0.6.2/src/llmtuner/extras/logging.py` & `llmtuner-0.6.3/src/llmtuner/extras/logging.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/extras/misc.py` & `llmtuner-0.6.3/src/llmtuner/extras/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,14 @@
         logger.warning("Version checking has been disabled, may lead to unexpected behaviors.")
     else:
         require_version("transformers>=4.37.2", "To fix: pip install transformers>=4.37.2")
         require_version("datasets>=2.14.3", "To fix: pip install datasets>=2.14.3")
         require_version("accelerate>=0.27.2", "To fix: pip install accelerate>=0.27.2")
         require_version("peft>=0.10.0", "To fix: pip install peft>=0.10.0")
         require_version("trl>=0.8.1", "To fix: pip install trl>=0.8.1")
-        require_version("gradio>=4.0.0,<=4.21.0", "To fix: pip install gradio==4.21.0")
 
 
 def count_parameters(model: torch.nn.Module) -> Tuple[int, int]:
     r"""
     Returns the number of trainable parameters and number of all parameters in the model.
     """
     trainable_params, all_param = 0, 0
@@ -80,14 +79,16 @@
         if num_params == 0 and hasattr(param, "ds_numel"):
             num_params = param.ds_numel
 
         # Due to the design of 4bit linear layers from bitsandbytes, multiply the number of parameters by 2
         if param.__class__.__name__ == "Params4bit":
             if hasattr(param, "quant_storage") and hasattr(param.quant_storage, "itemsize"):
                 num_bytes = param.quant_storage.itemsize
+            elif hasattr(param, "element_size"):  # for older pytorch version
+                num_bytes = param.element_size()
             else:
                 num_bytes = 1
 
             num_params = num_params * 2 * num_bytes
 
         all_param += num_params
         if param.requires_grad:
```

### Comparing `llmtuner-0.6.2/src/llmtuner/extras/packages.py` & `llmtuner-0.6.3/src/llmtuner/extras/packages.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     return _is_package_available("flash_attn") and _get_package_version("flash_attn").startswith("2")
 
 
 def is_galore_available():
     return _is_package_available("galore_torch")
 
 
+def is_gradio_available():
+    return _is_package_available("gradio")
+
+
 def is_jieba_available():
     return _is_package_available("jieba")
 
 
 def is_matplotlib_available():
     return _is_package_available("matplotlib")
 
@@ -45,17 +49,13 @@
     return _is_package_available("rouge_chinese")
 
 
 def is_starlette_available():
     return _is_package_available("sse_starlette")
 
 
-def is_unsloth_available():
-    return _is_package_available("unsloth")
-
-
 def is_uvicorn_available():
     return _is_package_available("uvicorn")
 
 
 def is_vllm_available():
     return _is_package_available("vllm")
```

### Comparing `llmtuner-0.6.2/src/llmtuner/extras/patches/llama_patch.py` & `llmtuner-0.6.3/src/llmtuner/extras/patches/llama_patch.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/extras/ploting.py` & `llmtuner-0.6.3/src/llmtuner/extras/ploting.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/hparams/data_args.py` & `llmtuner-0.6.3/src/llmtuner/hparams/data_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/hparams/evaluation_args.py` & `llmtuner-0.6.3/src/llmtuner/hparams/evaluation_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/hparams/finetuning_args.py` & `llmtuner-0.6.3/src/llmtuner/hparams/finetuning_args.py`

 * *Files 18% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 class GaloreArguments:
     r"""
     Arguments pertaining to the GaLore algorithm.
     """
 
     use_galore: bool = field(
         default=False,
-        metadata={"help": "Whether or not to use gradient low-Rank projection."},
+        metadata={"help": "Whether or not to use the gradient low-Rank projection (GaLore)."},
     )
     galore_target: str = field(
         default="all",
         metadata={
             "help": """Name(s) of modules to apply GaLore. Use commas to separate multiple modules. \
                     Use "all" to specify all the linear modules."""
         },
@@ -200,15 +200,62 @@
     galore_layerwise: bool = field(
         default=False,
         metadata={"help": "Whether or not to enable layer-wise update to further save memory."},
     )
 
 
 @dataclass
-class FinetuningArguments(FreezeArguments, LoraArguments, RLHFArguments, GaloreArguments):
+class BAdamArgument:
+    r"""
+    Arguments pertaining to the BAdam optimizer.
+    """
+
+    use_badam: bool = field(
+        default=False,
+        metadata={"help": "Whether or not to use the BAdam optimizer."},
+    )
+    badam_mode: Literal["layer", "ratio"] = field(
+        default="layer",
+        metadata={"help": "Whether to use layer-wise or ratio-wise BAdam optimizer."},
+    )
+    badam_start_block: Optional[int] = field(
+        default=None,
+        metadata={"help": "The starting block index for layer-wise BAdam."},
+    )
+    badam_switch_block_every: Optional[int] = field(
+        default=50,
+        metadata={"help": "How often to switch model's block update. Set to -1 to disable the block update."},
+    )
+    badam_switch_mode: Optional[Literal["ascending", "descending", "random", "fixed"]] = field(
+        default="ascending",
+        metadata={"help": "the strategy of picking block to update for layer-wise BAdam."},
+    )
+    badam_update_ratio: float = field(
+        default=0.0,
+        metadata={"help": "The ratio of the update for ratio-wise BAdam."},
+    )
+    badam_mask_mode: Literal["adjacent", "scatter"] = field(
+        default="adjacent",
+        metadata={
+            "help": """The mode of the mask for BAdam optimizer. \
+                    `adjacent` means that the trainable parameters are adjacent to each other, \
+                    `scatter` means that trainable parameters are randomly choosed from the weight."""
+        },
+    )
+    badam_verbose: int = field(
+        default=0,
+        metadata={
+            "help": """The verbosity level of BAdam optimizer. \
+                    0 for no print, 1 for print the block prefix, 2 for print trainable parameters"""
+        },
+    )
+
+
+@dataclass
+class FinetuningArguments(FreezeArguments, LoraArguments, RLHFArguments, GaloreArguments, BAdamArgument):
     r"""
     Arguments pertaining to which techniques we are going to fine-tuning with.
     """
 
     pure_bf16: bool = field(
         default=False,
         metadata={"help": "Whether or not to train model in purely bf16 precision (without AMP)."},
@@ -252,19 +299,22 @@
         if self.stage == "ppo" and self.reward_model_type == "lora" and self.finetuning_type != "lora":
             raise ValueError("`reward_model_type` cannot be lora for Freeze/Full PPO training.")
 
         if self.stage == "dpo" and self.dpo_loss != "sigmoid" and self.dpo_label_smoothing > 1e-6:
             raise ValueError("`dpo_label_smoothing` is only valid for sigmoid loss function.")
 
         if self.use_llama_pro and self.finetuning_type == "full":
-            raise ValueError("`use_llama_pro` is only valid for the Freeze or LoRA method.")
+            raise ValueError("`use_llama_pro` is only valid for the Freeze or LoRA training.")
 
         if self.use_galore and self.finetuning_type == "lora":
             raise ValueError("Cannot use LoRA with GaLore together.")
 
+        if self.loraplus_lr_ratio is not None and self.finetuning_type != "lora":
+            raise ValueError("`loraplus_lr_ratio` is only valid for the LoRA training.")
+
     def save_to_json(self, json_path: str):
         r"""Saves the content of this instance in JSON format inside `json_path`."""
         json_string = json.dumps(asdict(self), indent=2, sort_keys=True) + "\n"
         with open(json_path, "w", encoding="utf-8") as f:
             f.write(json_string)
 
     @classmethod
```

### Comparing `llmtuner-0.6.2/src/llmtuner/hparams/generating_args.py` & `llmtuner-0.6.3/src/llmtuner/hparams/generating_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/hparams/model_args.py` & `llmtuner-0.6.3/src/llmtuner/hparams/model_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,28 +51,32 @@
     )
     double_quantization: bool = field(
         default=True,
         metadata={"help": "Whether or not to use double quantization in int4 training."},
     )
     quantization_device_map: Optional[Literal["auto"]] = field(
         default=None,
-        metadata={"help": "Device map used for loading the 4-bit quantized model, needs bitsandbytes>=0.43.0."},
+        metadata={"help": "Device map used to infer the 4-bit quantized model, needs bitsandbytes>=0.43.0."},
     )
     rope_scaling: Optional[Literal["linear", "dynamic"]] = field(
         default=None,
         metadata={"help": "Which scaling strategy should be adopted for the RoPE embeddings."},
     )
     flash_attn: bool = field(
         default=False,
-        metadata={"help": "Enable FlashAttention-2 for faster training."},
+        metadata={"help": "Enable FlashAttention for faster training."},
     )
     shift_attn: bool = field(
         default=False,
         metadata={"help": "Enable shift short attention (S^2-Attn) proposed by LongLoRA."},
     )
+    mixture_of_depths: Optional[Literal["convert", "load"]] = field(
+        default=None,
+        metadata={"help": "Convert the model to mixture-of-depths (MoD) or load the MoD model."},
+    )
     use_unsloth: bool = field(
         default=False,
         metadata={"help": "Whether or not to use unsloth's optimization for the LoRA training."},
     )
     moe_aux_loss_coef: Optional[float] = field(
         default=None,
         metadata={"help": "Coefficient of the auxiliary router loss in mixture-of-experts model."},
@@ -125,14 +129,18 @@
         default=None,
         metadata={"help": "Path to the directory to save the exported model."},
     )
     export_size: int = field(
         default=1,
         metadata={"help": "The file shard size (in GB) of the exported model."},
     )
+    export_device: str = field(
+        default="cpu",
+        metadata={"help": "The device used in model export."},
+    )
     export_quantization_bit: Optional[int] = field(
         default=None,
         metadata={"help": "The number of bits to quantize the exported model."},
     )
     export_quantization_dataset: Optional[str] = field(
         default=None,
         metadata={"help": "Path to the dataset or dataset name to use in quantizing the exported model."},
```

### Comparing `llmtuner-0.6.2/src/llmtuner/hparams/parser.py` & `llmtuner-0.6.3/src/llmtuner/hparams/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 from typing import Any, Dict, Optional, Tuple
 
 import torch
 import transformers
 from transformers import HfArgumentParser, Seq2SeqTrainingArguments
 from transformers.trainer_utils import get_last_checkpoint
 from transformers.utils import is_torch_bf16_gpu_available
+from transformers.utils.versions import require_version
 
 from ..extras.logging import get_logger
-from ..extras.misc import check_dependencies
-from ..extras.packages import is_unsloth_available
+from ..extras.misc import check_dependencies, get_current_device
 from .data_args import DataArguments
 from .evaluation_args import EvaluationArguments
 from .finetuning_args import FinetuningArguments
 from .generating_args import GeneratingArguments
 from .model_args import ModelArguments
 
 
@@ -70,14 +70,40 @@
         if model_args.adapter_name_or_path is not None and finetuning_args.create_new_adapter:
             raise ValueError("Cannot create new adapter upon a quantized model.")
 
         if model_args.adapter_name_or_path is not None and len(model_args.adapter_name_or_path) != 1:
             raise ValueError("Quantized model only accepts a single adapter. Merge them first.")
 
 
+def _check_extra_dependencies(
+    model_args: "ModelArguments",
+    finetuning_args: "FinetuningArguments",
+    training_args: Optional["Seq2SeqTrainingArguments"] = None,
+) -> None:
+    if model_args.use_unsloth:
+        require_version("unsloth", "Please install unsloth: https://github.com/unslothai/unsloth")
+
+    if model_args.mixture_of_depths is not None:
+        require_version("mixture-of-depth>=1.1.6", "To fix: pip install mixture-of-depth>=1.1.6")
+
+    if model_args.infer_backend == "vllm":
+        require_version("vllm>=0.3.3", "To fix: pip install vllm>=0.3.3")
+
+    if finetuning_args.use_galore:
+        require_version("galore_torch", "To fix: pip install galore_torch")
+
+    if finetuning_args.use_badam:
+        require_version("badam", "To fix: pip install badam")
+
+    if training_args is not None and training_args.predict_with_generate:
+        require_version("jieba", "To fix: pip install jieba")
+        require_version("nltk", "To fix: pip install nltk")
+        require_version("rouge_chinese", "To fix: pip install rouge-chinese")
+
+
 def _parse_train_args(args: Optional[Dict[str, Any]] = None) -> _TRAIN_CLS:
     parser = HfArgumentParser(_TRAIN_ARGS)
     return _parse_args(parser, args)
 
 
 def _parse_infer_args(args: Optional[Dict[str, Any]] = None) -> _INFER_CLS:
     parser = HfArgumentParser(_INFER_ARGS)
@@ -127,16 +153,16 @@
 
     if training_args.max_steps == -1 and data_args.streaming:
         raise ValueError("Please specify `max_steps` in streaming mode.")
 
     if training_args.do_train and training_args.predict_with_generate:
         raise ValueError("`predict_with_generate` cannot be set as True while training.")
 
-    if training_args.do_train and model_args.use_unsloth and not is_unsloth_available():
-        raise ValueError("Unsloth was not installed: https://github.com/unslothai/unsloth")
+    if training_args.do_train and model_args.quantization_device_map == "auto":
+        raise ValueError("Cannot use device map for quantized models in training.")
 
     if finetuning_args.use_dora and model_args.use_unsloth:
         raise ValueError("Unsloth does not support DoRA.")
 
     if finetuning_args.pure_bf16:
         if not is_torch_bf16_gpu_available():
             raise ValueError("This device does not support `pure_bf16`.")
@@ -147,21 +173,29 @@
     if (
         finetuning_args.use_galore
         and finetuning_args.galore_layerwise
         and training_args.parallel_mode.value == "distributed"
     ):
         raise ValueError("Distributed training does not support layer-wise GaLore.")
 
-    if finetuning_args.use_galore and training_args.deepspeed is not None:
-        raise ValueError("GaLore is incompatible with DeepSpeed.")
+    if (
+        finetuning_args.use_badam
+        and finetuning_args.badam_mode == "layer"
+        and training_args.parallel_mode.value == "distributed"
+    ):
+        raise ValueError("Layer-wise BAdam does not yet support distributed training, use ratio-wise BAdam.")
+
+    if (finetuning_args.use_galore or finetuning_args.use_badam) and training_args.deepspeed is not None:
+        raise ValueError("GaLore and BAdam are incompatible with DeepSpeed yet.")
 
     if model_args.infer_backend == "vllm":
         raise ValueError("vLLM backend is only available for API, CLI and Web.")
 
     _verify_model_args(model_args, finetuning_args)
+    _check_extra_dependencies(model_args, finetuning_args, training_args)
 
     if (
         training_args.do_train
         and finetuning_args.finetuning_type == "lora"
         and model_args.resize_vocab
         and finetuning_args.additional_target is None
     ):
@@ -231,14 +265,15 @@
 
     # Post-process model arguments
     if training_args.bf16 or finetuning_args.pure_bf16:
         model_args.compute_dtype = torch.bfloat16
     elif training_args.fp16:
         model_args.compute_dtype = torch.float16
 
+    model_args.device_map = {"": get_current_device()}
     model_args.model_max_length = data_args.cutoff_len
     data_args.packing = data_args.packing if data_args.packing is not None else finetuning_args.stage == "pt"
 
     # Log on each process the small summary:
     logger.info(
         "Process rank: {}, device: {}, n_gpu: {}, distributed training: {}, compute dtype: {}".format(
             training_args.local_rank,
@@ -272,16 +307,20 @@
         if model_args.quantization_bit is not None:
             raise ValueError("vLLM engine does not support quantization.")
 
         if model_args.rope_scaling is not None:
             raise ValueError("vLLM engine does not support RoPE scaling.")
 
     _verify_model_args(model_args, finetuning_args)
+    _check_extra_dependencies(model_args, finetuning_args)
 
-    model_args.device_map = "auto"
+    if model_args.export_dir is not None:
+        model_args.device_map = {"": torch.device(model_args.export_device)}
+    else:
+        model_args.device_map = "auto"
 
     return model_args, data_args, finetuning_args, generating_args
 
 
 def get_eval_args(args: Optional[Dict[str, Any]] = None) -> _EVAL_CLS:
     model_args, data_args, eval_args, finetuning_args = _parse_eval_args(args)
 
@@ -290,13 +329,14 @@
     if data_args.template is None:
         raise ValueError("Please specify which `template` to use.")
 
     if model_args.infer_backend == "vllm":
         raise ValueError("vLLM backend is only available for API, CLI and Web.")
 
     _verify_model_args(model_args, finetuning_args)
+    _check_extra_dependencies(model_args, finetuning_args)
 
     model_args.device_map = "auto"
 
     transformers.set_seed(eval_args.seed)
 
     return model_args, data_args, eval_args, finetuning_args
```

### Comparing `llmtuner-0.6.2/src/llmtuner/model/adapter.py` & `llmtuner-0.6.3/src/llmtuner/model/adapter.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,17 +28,20 @@
     Note that the trainable parameters must be cast to float32.
     """
 
     if (not is_trainable) and model_args.adapter_name_or_path is None:
         logger.info("Adapter is not found at evaluation, load the base model.")
         return model
 
+    if finetuning_args.finetuning_type != "lora" and getattr(model, "quantization_method", None):
+        raise ValueError("You can only use lora for quantized models.")
+
     if finetuning_args.finetuning_type == "full" and is_trainable:
         logger.info("Fine-tuning method: Full")
-        if not finetuning_args.pure_bf16:
+        if (not finetuning_args.pure_bf16) and (not finetuning_args.use_badam):
             model = model.float()
 
     if finetuning_args.finetuning_type == "freeze" and is_trainable:
         logger.info("Fine-tuning method: Freeze")
         num_layers = (
             getattr(model.config, "num_hidden_layers", None)
             or getattr(model.config, "num_layers", None)
@@ -62,28 +65,30 @@
         else:  # fine-tuning the first n layers if num_layer_trainable < 0
             trainable_layer_ids = range(-finetuning_args.num_layer_trainable)
 
         freeze_modules = {"all"}
         for name, _ in model.named_modules():
             if ".0." in name:
                 freeze_modules.add(name.split(".0.")[-1].split(".")[0])
+            elif ".1." in name:  # MoD starts from layer 1
+                freeze_modules.add(name.split(".1.")[-1].split(".")[0])
 
         trainable_layers = []
         for module_name in finetuning_args.name_module_trainable:
             if module_name not in freeze_modules:
                 raise ValueError(
                     "Module {} is not found, please choose from {}".format(module_name, ", ".join(freeze_modules))
                 )
 
             for idx in trainable_layer_ids:
                 trainable_layers.append(".{:d}.{}".format(idx, module_name if module_name != "all" else ""))
 
         for name, param in model.named_parameters():
             if any(trainable_layer in name for trainable_layer in trainable_layers):
-                if not finetuning_args.pure_bf16:
+                if (not finetuning_args.pure_bf16) and (not finetuning_args.use_badam):
                     param.data = param.data.to(torch.float32)
             else:
                 param.requires_grad_(False)
 
         logger.info("Set trainable layers: {}".format(",".join(map(str, trainable_layer_ids))))
 
     if finetuning_args.finetuning_type == "lora":
@@ -125,42 +130,49 @@
                 target_modules = find_all_linear_modules(model)
             else:
                 target_modules = finetuning_args.lora_target
 
             if finetuning_args.use_llama_pro:
                 target_modules = find_expanded_modules(model, target_modules, finetuning_args.num_layer_trainable)
 
-            if finetuning_args.use_dora and getattr(model, "quantization_method", None) is not None:
-                if getattr(model, "quantization_method", None) != QuantizationMethod.BITS_AND_BYTES:
-                    raise ValueError("DoRA is not compatible with PTQ-quantized models.")
+            if (
+                finetuning_args.use_dora
+                and getattr(model, "quantization_method", None) is not None
+                and getattr(model, "quantization_method", None) != QuantizationMethod.BITS_AND_BYTES
+            ):
+                raise ValueError("DoRA is not compatible with PTQ-quantized models.")
 
             peft_kwargs = {
                 "r": finetuning_args.lora_rank,
                 "target_modules": target_modules,
                 "lora_alpha": finetuning_args.lora_alpha,
                 "lora_dropout": finetuning_args.lora_dropout,
                 "use_rslora": finetuning_args.use_rslora,
+                "modules_to_save": finetuning_args.additional_target,
             }
 
             if model_args.use_unsloth:
                 from unsloth import FastLanguageModel  # type: ignore
 
-                unsloth_peft_kwargs = {"model": model, "max_seq_length": model_args.model_max_length}
+                unsloth_peft_kwargs = {
+                    "model": model,
+                    "max_seq_length": model_args.model_max_length,
+                    "use_gradient_checkpointing": "unsloth",
+                }
                 model = FastLanguageModel.get_peft_model(**peft_kwargs, **unsloth_peft_kwargs)
             else:
                 lora_config = LoraConfig(
                     task_type=TaskType.CAUSAL_LM,
                     inference_mode=False,
-                    modules_to_save=finetuning_args.additional_target,
                     use_dora=finetuning_args.use_dora,
                     **peft_kwargs,
                 )
                 model = get_peft_model(model, lora_config)
 
-        if not finetuning_args.pure_bf16:
+        if (not finetuning_args.pure_bf16) and (not finetuning_args.use_badam):
             for param in filter(lambda p: p.requires_grad, model.parameters()):
                 param.data = param.data.to(torch.float32)
 
         if model_args.adapter_name_or_path is not None:
             logger.info("Loaded adapter(s): {}".format(",".join(model_args.adapter_name_or_path)))
 
     return model
```

### Comparing `llmtuner-0.6.2/src/llmtuner/model/loader.py` & `llmtuner-0.6.3/src/llmtuner/model/loader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import TYPE_CHECKING, Any, Dict
 
 from transformers import AutoConfig, AutoModelForCausalLM, AutoTokenizer
 from trl import AutoModelForCausalLMWithValueHead
 
+from ..extras.constants import MOD_SUPPORTED_MODELS
 from ..extras.logging import get_logger
 from ..extras.misc import count_parameters, get_current_device, try_download_model_from_ms
 from .adapter import init_adapter
 from .patcher import patch_config, patch_model, patch_tokenizer, patch_valuehead_model
 from .utils import load_valuehead_params, register_autoclass
 
 
@@ -32,21 +33,30 @@
 def load_tokenizer(model_args: "ModelArguments") -> "PreTrainedTokenizer":
     r"""
     Loads pretrained tokenizer. Must before load_model.
 
     Note: including inplace operation of model_args.
     """
     init_kwargs = _get_init_kwargs(model_args)
-    tokenizer = AutoTokenizer.from_pretrained(
-        model_args.model_name_or_path,
-        use_fast=model_args.use_fast_tokenizer,
-        split_special_tokens=model_args.split_special_tokens,
-        padding_side="right",
-        **init_kwargs,
-    )
+    try:
+        tokenizer = AutoTokenizer.from_pretrained(
+            model_args.model_name_or_path,
+            use_fast=model_args.use_fast_tokenizer,
+            split_special_tokens=model_args.split_special_tokens,
+            padding_side="right",
+            **init_kwargs,
+        )
+    except ValueError:  # try the fast one
+        tokenizer = AutoTokenizer.from_pretrained(
+            model_args.model_name_or_path,
+            use_fast=True,
+            padding_side="right",
+            **init_kwargs,
+        )
+
     patch_tokenizer(tokenizer)
     return tokenizer
 
 
 def load_model(
     tokenizer: "PreTrainedTokenizer",
     model_args: "ModelArguments",
@@ -69,35 +79,54 @@
             "model_name": model_args.model_name_or_path,
             "max_seq_length": model_args.model_max_length,
             "dtype": model_args.compute_dtype,
             "load_in_4bit": model_args.quantization_bit == 4,
             "token": model_args.hf_hub_token,
             "device_map": {"": get_current_device()},
             "rope_scaling": getattr(config, "rope_scaling", None),
+            "fix_tokenizer": False,
+            "trust_remote_code": True,
         }
         try:
             model, _ = FastLanguageModel.from_pretrained(**unsloth_kwargs)
         except NotImplementedError:
             logger.warning("Unsloth does not support model type {}.".format(getattr(config, "model_type", None)))
             model_args.use_unsloth = False
 
         if model_args.adapter_name_or_path:
             model_args.adapter_name_or_path = None
             logger.warning("Unsloth does not support loading adapters.")
 
     if model is None:
-        model = AutoModelForCausalLM.from_pretrained(model_args.model_name_or_path, config=config, **init_kwargs)
+        init_kwargs["config"] = config
+        init_kwargs["pretrained_model_name_or_path"] = model_args.model_name_or_path
+
+        if model_args.mixture_of_depths == "load":
+            from MoD import AutoMoDModelForCausalLM
+
+            model = AutoMoDModelForCausalLM.from_pretrained(**init_kwargs)
+        else:
+            model = AutoModelForCausalLM.from_pretrained(**init_kwargs)
+
+        if model_args.mixture_of_depths == "convert":
+            from MoD import apply_mod_to_hf
+
+            if getattr(config, "model_type", None) not in MOD_SUPPORTED_MODELS:
+                raise ValueError("Current model is not supported by mixture-of-depth.")
+
+            model = apply_mod_to_hf(model)
+            model = model.to(model_args.compute_dtype)
 
     patch_model(model, tokenizer, model_args, is_trainable)
     register_autoclass(config, model, tokenizer)
 
     model = init_adapter(model, model_args, finetuning_args, is_trainable)
 
     if add_valuehead:
-        model: "AutoModelForCausalLMWithValueHead" = AutoModelForCausalLMWithValueHead.from_pretrained(model)
+        model = AutoModelForCausalLMWithValueHead.from_pretrained(model)
         patch_valuehead_model(model)
 
         if model_args.adapter_name_or_path is not None:
             vhead_path = model_args.adapter_name_or_path[-1]
         else:
             vhead_path = model_args.model_name_or_path
```

### Comparing `llmtuner-0.6.2/src/llmtuner/model/patcher.py` & `llmtuner-0.6.3/src/llmtuner/model/patcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from transformers.utils.versions import require_version
 
 from ..extras.constants import FILEEXT2TYPE, LAYERNORM_NAMES
 from ..extras.logging import get_logger
 from ..extras.misc import get_current_device, infer_optim_dtype
 from ..extras.packages import is_flash_attn2_available
 from ..extras.patches.llama_patch import apply_llama_patch
-from .utils import QuantizationMethod, add_z3_leaf_module
+from .utils import QuantizationMethod, add_z3_leaf_module, gradient_checkpointing_enable
 
 
 if TYPE_CHECKING:
     from transformers import PretrainedConfig, PreTrainedTokenizer
     from trl import AutoModelForCausalLMWithValueHead
 
     from ..hparams import ModelArguments
@@ -57,29 +57,27 @@
         word_idx = random.randint(0, sample["input_ids"].size(1) - maxlen - 1)
         input_ids = sample["input_ids"][:, word_idx : word_idx + maxlen]
         samples.append(tokenizer.decode(input_ids[0].tolist(), skip_special_tokens=True))
 
     return samples
 
 
-def _configure_attn_implementation(
-    config: "PretrainedConfig", model_args: "ModelArguments", init_kwargs: Dict[str, Any]
-) -> None:
+def _configure_attn_implementation(config: "PretrainedConfig", model_args: "ModelArguments") -> None:
     if model_args.flash_attn:
         if not is_flash_attn2_available():
             logger.warning("FlashAttention2 is not installed.")
             return
 
         logger.info("Using FlashAttention-2 for faster training and inference.")
         if getattr(config, "model_type", None) == "internlm2":  # special case for custom models
             setattr(config, "attn_implementation", "flash_attention_2")
         else:
-            init_kwargs["attn_implementation"] = "flash_attention_2"
+            setattr(config, "_attn_implementation", "flash_attention_2")
     else:
-        init_kwargs["attn_implementation"] = "eager"
+        setattr(config, "_attn_implementation", "eager")
 
 
 def _configure_rope(config: "PretrainedConfig", model_args: "ModelArguments", is_trainable: bool) -> None:
     if model_args.rope_scaling is None:
         return
 
     if not hasattr(config, "rope_scaling"):
@@ -129,20 +127,23 @@
     r"""
     Priority: PTQ-quantized (training) > AutoGPTQ (export) > Bitsandbytes (training)
     """
     if getattr(config, "quantization_config", None):  # ptq
         if is_deepspeed_zero3_enabled():
             raise ValueError("DeepSpeed ZeRO-3 is incompatible with quantized models.")
 
-        init_kwargs["device_map"] = {"": get_current_device()}
+        if model_args.quantization_device_map != "auto":
+            init_kwargs["device_map"] = {"": get_current_device()}
+
         quantization_config: Dict[str, Any] = getattr(config, "quantization_config", None)
         quant_method = quantization_config.get("quant_method", "")
 
         if quant_method == QuantizationMethod.GPTQ:
             require_version("auto_gptq>=0.5.0", "To fix: pip install auto_gptq>=0.5.0")
+            quantization_config.pop("disable_exllama", None)  # remove deprecated args
             quantization_config["use_exllama"] = False  # disable exllama
 
         if quant_method == QuantizationMethod.AWQ:
             require_version("autoawq", "To fix: pip install autoawq")
 
         if quant_method == QuantizationMethod.AQLM:
             require_version("transformers>=4.39.0", "To fix: pip install transformers>=4.39.0")
@@ -262,16 +263,16 @@
 
     if not model_args.disable_gradient_checkpointing:
         if not getattr(model, "supports_gradient_checkpointing", False):
             logger.warning("Current model does not support gradient checkpointing.")
         else:
             # use_reentrant=False might increase VRAM usage (have not been empirically verified yet)
             # According to: https://github.com/huggingface/transformers/issues/28339
+            model.gradient_checkpointing_enable = MethodType(gradient_checkpointing_enable, model)
             model.gradient_checkpointing_enable(gradient_checkpointing_kwargs={"use_reentrant": True})
-            model.enable_input_require_grads()
             setattr(model.config, "use_cache", False)  # turn off when gradient checkpointing is enabled
             logger.info("Gradient checkpointing enabled.")
 
     if hasattr(model, output_layer_name) and model_args.upcast_lmhead_output:
         logger.info("Upcasting lm_head outputs in float32.")
         output_layer = getattr(model, output_layer_name)
         if isinstance(output_layer, torch.nn.Linear) and output_layer.weight.dtype != torch.float32:
@@ -289,15 +290,15 @@
     model_args: "ModelArguments",
     init_kwargs: Dict[str, Any],
     is_trainable: bool,
 ) -> None:
     if model_args.compute_dtype is None:  # priority: bf16 > fp16 > fp32
         model_args.compute_dtype = infer_optim_dtype(model_dtype=getattr(config, "torch_dtype", None))
 
-    _configure_attn_implementation(config, model_args, init_kwargs)
+    _configure_attn_implementation(config, model_args)
     _configure_rope(config, model_args, is_trainable)
     _configure_longlora(config, model_args, is_trainable)
     _configure_quantization(config, tokenizer, model_args, init_kwargs)
 
     if model_args.use_cache and not is_trainable:
         setattr(config, "use_cache", True)
         logger.info("Using KV cache for faster generation.")
@@ -312,23 +313,23 @@
         setattr(config, "use_flash_attn", model_args.flash_attn)
         for dtype_name, dtype in [("fp16", torch.float16), ("bf16", torch.bfloat16), ("fp32", torch.float32)]:
             setattr(config, dtype_name, model_args.compute_dtype == dtype)
 
     if getattr(config, "model_type", None) == "qwen2" and is_trainable and model_args.flash_attn:
         setattr(config, "use_cache", False)  # qwen2 does not support use_cache when using flashattn
 
-    if getattr(config, "model_type", None) == "qwen2_moe" and is_trainable:
+    if getattr(config, "model_type", None) in ["mixtral", "qwen2_moe"] and is_trainable:
         setattr(config, "output_router_logits", True)
 
     init_kwargs["torch_dtype"] = model_args.compute_dtype
     if not is_deepspeed_zero3_enabled():
         init_kwargs["low_cpu_mem_usage"] = model_args.low_cpu_mem_usage
         if init_kwargs["low_cpu_mem_usage"]:
-            if "device_map" not in init_kwargs:
-                init_kwargs["device_map"] = model_args.device_map or {"": get_current_device()}
+            if "device_map" not in init_kwargs and model_args.device_map:
+                init_kwargs["device_map"] = model_args.device_map
 
             if init_kwargs["device_map"] == "auto":
                 init_kwargs["offload_folder"] = model_args.offload_folder
 
 
 def patch_model(
     model: "PreTrainedModel", tokenizer: "PreTrainedTokenizer", model_args: "ModelArguments", is_trainable: bool
```

### Comparing `llmtuner-0.6.2/src/llmtuner/model/utils.py` & `llmtuner-0.6.3/src/llmtuner/model/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import inspect
 from enum import Enum, unique
-from typing import TYPE_CHECKING, Dict, List
+from functools import partial
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 import torch
 from transformers import PreTrainedModel
 from transformers.integrations import is_deepspeed_zero3_enabled
 from transformers.utils import cached_file
 from transformers.utils.versions import require_version
 
@@ -96,14 +98,50 @@
         ):
             module_names.append(name)
 
     logger.info("Apply lora to layers: {}".format(",".join(map(str, trainable_layer_ids))))
     return module_names
 
 
+def gradient_checkpointing_enable(
+    self: "PreTrainedModel", gradient_checkpointing_kwargs: Optional[Dict[str, Any]] = None
+) -> None:
+    r"""
+    Activates gradient checkpointing for the current model.
+
+    Modification of the original method to enable gradient checkpointing for block-wise optimizer.
+    """
+    from torch.utils.checkpoint import checkpoint
+
+    if not self.supports_gradient_checkpointing:
+        raise ValueError("{} does not support gradient checkpointing.".format(self.__class__.__name__))
+
+    if gradient_checkpointing_kwargs is None:
+        gradient_checkpointing_kwargs = {"use_reentrant": True}
+
+    gradient_checkpointing_func = partial(checkpoint, **gradient_checkpointing_kwargs)
+
+    def custom_gradient_checkpointing_func(func, *args, **kwargs):
+        module: "torch.nn.Module" = func.__self__
+
+        if any(param.requires_grad for param in module.parameters()):
+            for arg in args:
+                if torch.is_tensor(arg) and torch.is_floating_point(arg):
+                    arg.requires_grad_(True)
+
+        return gradient_checkpointing_func(func, *args, **kwargs)
+
+    if "value" in inspect.signature(self._set_gradient_checkpointing).parameters:  # old GC format
+        self.apply(partial(self._set_gradient_checkpointing, value=True))
+        self.enable_input_require_grads()
+        logger.warning("You are using the old GC format, some features (e.g. BAdam) will be invalid.")
+    else:  # have already enabled input require gradients
+        self._set_gradient_checkpointing(enable=True, gradient_checkpointing_func=custom_gradient_checkpointing_func)
+
+
 def load_valuehead_params(path_or_repo_id: str, model_args: "ModelArguments") -> Dict[str, torch.Tensor]:
     r"""
     Loads value head parameters from Hugging Face Hub or local disk.
 
     Returns: dict with keys `v_head.summary.weight` and `v_head.summary.bias`.
     """
     kwargs = {"path_or_repo_id": path_or_repo_id, "cache_dir": model_args.cache_dir, "token": model_args.hf_hub_token}
```

### Comparing `llmtuner-0.6.2/src/llmtuner/train/dpo/trainer.py` & `llmtuner-0.6.3/src/llmtuner/train/dpo/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import defaultdict
 from contextlib import nullcontext
+from types import MethodType
 from typing import TYPE_CHECKING, Dict, Literal, Optional, Tuple, Union
 
 import torch
 from transformers import BatchEncoding, Trainer
 from trl import DPOTrainer
 from trl.trainer.utils import disable_dropout_in_model
 
@@ -59,14 +60,19 @@
                 if not (
                     getattr(ref_model, "is_loaded_in_8bit", False) or getattr(ref_model, "is_loaded_in_4bit", False)
                 ):  # quantized models are already set on the correct device
                     self.ref_model = self._prepare_deepspeed(self.ref_model)
             else:
                 self.ref_model = self.accelerator.prepare_model(self.ref_model, evaluation_mode=True)
 
+        if finetuning_args.use_badam:
+            from badam import clip_grad_norm_for_sparse_tensor
+
+            self.accelerator.clip_grad_norm_ = MethodType(clip_grad_norm_for_sparse_tensor, self.accelerator)
+
     def create_optimizer(self) -> "torch.optim.Optimizer":
         if self.optimizer is None:
             self.optimizer = create_custom_optimzer(self.model, self.args, self.finetuning_args)
         return super().create_optimizer()
 
     def create_scheduler(
         self, num_training_steps: int, optimizer: Optional["torch.optim.Optimizer"] = None
```

### Comparing `llmtuner-0.6.2/src/llmtuner/train/dpo/workflow.py` & `llmtuner-0.6.3/src/llmtuner/train/dpo/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/train/orpo/trainer.py` & `llmtuner-0.6.3/src/llmtuner/train/orpo/trainer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections import defaultdict
+from types import MethodType
 from typing import TYPE_CHECKING, Dict, Literal, Optional, Tuple, Union
 
 import torch
 import torch.nn.functional as F
 from transformers import Trainer
 from trl import DPOTrainer
 from trl.trainer.utils import disable_dropout_in_model
@@ -40,14 +41,18 @@
         self._precomputed_eval_ref_log_probs = False
         self._peft_has_been_casted_to_bf16 = False
 
         self.beta = finetuning_args.orpo_beta
         self._stored_metrics = defaultdict(lambda: defaultdict(list))
 
         Trainer.__init__(self, model=model, **kwargs)
+        if finetuning_args.use_badam:
+            from badam import clip_grad_norm_for_sparse_tensor
+
+            self.accelerator.clip_grad_norm_ = MethodType(clip_grad_norm_for_sparse_tensor, self.accelerator)
 
     def create_optimizer(self) -> "torch.optim.Optimizer":
         if self.optimizer is None:
             self.optimizer = create_custom_optimzer(self.model, self.args, self.finetuning_args)
         return super().create_optimizer()
 
     def create_scheduler(
```

### Comparing `llmtuner-0.6.2/src/llmtuner/train/orpo/workflow.py` & `llmtuner-0.6.3/src/llmtuner/train/orpo/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/train/ppo/trainer.py` & `llmtuner-0.6.3/src/llmtuner/train/ppo/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import math
 import os
 import sys
+from types import MethodType
 from typing import TYPE_CHECKING, Dict, List, Optional, Tuple
 
 import torch
 from tqdm import tqdm
 from transformers import GenerationConfig, Trainer, TrainerControl, TrainerState
 from transformers.optimization import get_scheduler
 from transformers.trainer_pt_utils import remove_dummy_checkpoint
@@ -120,14 +121,19 @@
                     getattr(reward_model.pretrained_model, "is_loaded_in_8bit", False)
                     or getattr(reward_model.pretrained_model, "is_loaded_in_4bit", False)
                 ):  # quantized models are already set on the correct device
                     self.reward_model = self._prepare_deepspeed(self.reward_model)
             else:
                 self.reward_model = self.accelerator.prepare_model(self.reward_model, evaluation_mode=True)
 
+        if finetuning_args.use_badam:
+            from badam import clip_grad_norm_for_sparse_tensor
+
+            self.accelerator.clip_grad_norm_ = MethodType(clip_grad_norm_for_sparse_tensor, self.accelerator)
+
     def ppo_train(self, resume_from_checkpoint: Optional[str] = None) -> None:
         r"""
         Implements training loop for the PPO stage, like _inner_training_loop() in Huggingface's Trainer.
         """
         if resume_from_checkpoint is not None:
             raise ValueError("`resume_from_checkpoint` will be supported in the future version.")
```

### Comparing `llmtuner-0.6.2/src/llmtuner/train/ppo/utils.py` & `llmtuner-0.6.3/src/llmtuner/train/ppo/utils.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/train/ppo/workflow.py` & `llmtuner-0.6.3/src/llmtuner/train/ppo/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/train/pt/trainer.py` & `llmtuner-0.6.3/src/llmtuner/train/pt/trainer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from types import MethodType
 from typing import TYPE_CHECKING, Optional
 
 from transformers import Trainer
 
 from ...extras.logging import get_logger
 from ..utils import create_custom_optimzer, create_custom_scheduler
 
@@ -19,14 +20,18 @@
     r"""
     Inherits Trainer for custom optimizer.
     """
 
     def __init__(self, finetuning_args: "FinetuningArguments", **kwargs) -> None:
         super().__init__(**kwargs)
         self.finetuning_args = finetuning_args
+        if finetuning_args.use_badam:
+            from badam import clip_grad_norm_for_sparse_tensor
+
+            self.accelerator.clip_grad_norm_ = MethodType(clip_grad_norm_for_sparse_tensor, self.accelerator)
 
     def create_optimizer(self) -> "torch.optim.Optimizer":
         if self.optimizer is None:
             self.optimizer = create_custom_optimzer(self.model, self.args, self.finetuning_args)
         return super().create_optimizer()
 
     def create_scheduler(
```

### Comparing `llmtuner-0.6.2/src/llmtuner/train/pt/workflow.py` & `llmtuner-0.6.3/src/llmtuner/train/pt/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/train/rm/trainer.py` & `llmtuner-0.6.3/src/llmtuner/train/rm/trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+from types import MethodType
 from typing import TYPE_CHECKING, Dict, List, Optional, Tuple, Union
 
 import torch
 from transformers import Trainer
 
 from ...extras.logging import get_logger
 from ..utils import create_custom_optimzer, create_custom_scheduler
@@ -24,14 +25,18 @@
     Inherits Trainer to compute pairwise loss.
     """
 
     def __init__(self, finetuning_args: "FinetuningArguments", **kwargs) -> None:
         super().__init__(**kwargs)
         self.finetuning_args = finetuning_args
         self.can_return_loss = True  # override property to return eval_loss
+        if finetuning_args.use_badam:
+            from badam import clip_grad_norm_for_sparse_tensor
+
+            self.accelerator.clip_grad_norm_ = MethodType(clip_grad_norm_for_sparse_tensor, self.accelerator)
 
     def create_optimizer(self) -> "torch.optim.Optimizer":
         if self.optimizer is None:
             self.optimizer = create_custom_optimzer(self.model, self.args, self.finetuning_args)
         return super().create_optimizer()
 
     def create_scheduler(
```

### Comparing `llmtuner-0.6.2/src/llmtuner/train/rm/workflow.py` & `llmtuner-0.6.3/src/llmtuner/train/rm/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/train/sft/metric.py` & `llmtuner-0.6.3/src/llmtuner/train/sft/metric.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Dict, Sequence, Tuple, Union
 
 import numpy as np
-from transformers.utils.versions import require_version
 
 from ...extras.constants import IGNORE_INDEX
 from ...extras.packages import is_jieba_available, is_nltk_available, is_rouge_available
 
 
 if TYPE_CHECKING:
     from transformers.tokenization_utils import PreTrainedTokenizer
@@ -29,18 +28,14 @@
 
     tokenizer: "PreTrainedTokenizer"
 
     def __call__(self, eval_preds: Sequence[Union[np.ndarray, Tuple[np.ndarray]]]) -> Dict[str, float]:
         r"""
         Uses the model predictions to compute metrics.
         """
-        require_version("jieba", "To fix: pip install jieba")
-        require_version("nltk", "To fix: pip install nltk")
-        require_version("rouge_chinese", "To fix: pip install rouge-chinese")
-
         preds, labels = eval_preds
         score_dict = {"rouge-1": [], "rouge-2": [], "rouge-l": [], "bleu-4": []}
 
         preds = np.where(preds != IGNORE_INDEX, preds, self.tokenizer.pad_token_id)
         labels = np.where(labels != IGNORE_INDEX, labels, self.tokenizer.pad_token_id)
 
         decoded_preds = self.tokenizer.batch_decode(preds, skip_special_tokens=True)
```

### Comparing `llmtuner-0.6.2/src/llmtuner/train/sft/trainer.py` & `llmtuner-0.6.3/src/llmtuner/train/sft/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import os
+from types import MethodType
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import torch
 from transformers import Seq2SeqTrainer
 
 from ...extras.constants import IGNORE_INDEX
@@ -24,14 +25,18 @@
     r"""
     Inherits Seq2SeqTrainer to compute generative metrics such as BLEU and ROUGE.
     """
 
     def __init__(self, finetuning_args: "FinetuningArguments", **kwargs) -> None:
         super().__init__(**kwargs)
         self.finetuning_args = finetuning_args
+        if finetuning_args.use_badam:
+            from badam import clip_grad_norm_for_sparse_tensor
+
+            self.accelerator.clip_grad_norm_ = MethodType(clip_grad_norm_for_sparse_tensor, self.accelerator)
 
     def create_optimizer(self) -> "torch.optim.Optimizer":
         if self.optimizer is None:
             self.optimizer = create_custom_optimzer(self.model, self.args, self.finetuning_args)
         return super().create_optimizer()
 
     def create_scheduler(
```

### Comparing `llmtuner-0.6.2/src/llmtuner/train/sft/workflow.py` & `llmtuner-0.6.3/src/llmtuner/train/sft/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/train/tuner.py` & `llmtuner-0.6.3/src/llmtuner/train/tuner.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,16 +61,15 @@
 
     if not isinstance(model, PreTrainedModel):
         raise ValueError("The model is not a `PreTrainedModel`, export aborted.")
 
     if getattr(model, "quantization_method", None) is None:  # cannot convert dtype of a quantized model
         output_dtype = getattr(model.config, "torch_dtype", torch.float16)
         setattr(model.config, "torch_dtype", output_dtype)
-        for param in model.parameters():
-            param.data = param.data.to(output_dtype)
+        model = model.to(output_dtype)
 
     model.save_pretrained(
         save_directory=model_args.export_dir,
         max_shard_size="{}GB".format(model_args.export_size),
         safe_serialization=(not model_args.export_legacy_format),
     )
     if model_args.export_hub_model_id is not None:
```

### Comparing `llmtuner-0.6.2/src/llmtuner/train/utils.py` & `llmtuner-0.6.3/src/llmtuner/train/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import TYPE_CHECKING, Callable, Dict, List, Optional, Union
 
 import torch
 from transformers import Trainer
 from transformers.optimization import get_scheduler
 from transformers.pytorch_utils import ALL_LAYERNORM_LAYERS
 from transformers.trainer_pt_utils import get_parameter_names
-from transformers.utils.versions import require_version
 
 from ..extras.logging import get_logger
 from ..extras.packages import is_galore_available
 from ..hparams import FinetuningArguments, ModelArguments
 from ..model import find_all_linear_modules, load_model, load_tokenizer, load_valuehead_params
 
 
@@ -53,17 +52,19 @@
     data_args: "DataArguments",
     training_args: "Seq2SeqTrainingArguments",
     finetuning_args: "FinetuningArguments",
 ) -> None:
     kwargs = {
         "tasks": "text-generation",
         "finetuned_from": model_args.model_name_or_path,
-        "dataset": [dataset.strip() for dataset in data_args.dataset.split(",")],
         "tags": ["llama-factory", finetuning_args.finetuning_type],
     }
+    if data_args.dataset is not None:
+        kwargs["dataset"] = [dataset.strip() for dataset in data_args.dataset.split(",")]
+
     if not training_args.do_train:
         pass
     elif training_args.push_to_hub:
         trainer.push_to_hub(**kwargs)
     else:
         trainer.create_model_card(license="other", **kwargs)  # prevent from connecting to hub
 
@@ -162,16 +163,14 @@
 
 
 def _create_galore_optimizer(
     model: "PreTrainedModel",
     training_args: "Seq2SeqTrainingArguments",
     finetuning_args: "FinetuningArguments",
 ) -> "torch.optim.Optimizer":
-    require_version("galore_torch", "To fix: pip install galore_torch")
-
     if len(finetuning_args.galore_target) == 1 and finetuning_args.galore_target[0] == "all":
         galore_targets = find_all_linear_modules(model)
     else:
         galore_targets = finetuning_args.galore_target
 
     galore_params: List["torch.nn.Parameter"] = []
     for name, module in model.named_modules():
@@ -213,15 +212,15 @@
 
     if finetuning_args.galore_layerwise:
         if training_args.gradient_accumulation_steps != 1:
             raise ValueError("Per-layer GaLore does not support gradient accumulation.")
 
         optimizer_dict: Dict["torch.Tensor", "torch.optim.Optimizer"] = {}
         for param in nodecay_params:
-            param_groups = [dict(params=[param])]
+            param_groups = [dict(params=[param], weight_decay=0.0)]
             optimizer_dict[param] = optim_class(param_groups, **optim_kwargs)
         for param in decay_params:
             param_groups = [dict(params=[param], weight_decay=training_args.weight_decay)]
             optimizer_dict[param] = optim_class(param_groups, **optim_kwargs)
         for param in galore_params:  # galore params have weight decay
             param_groups = [dict(params=[param], weight_decay=training_args.weight_decay, **galore_kwargs)]
             optimizer_dict[param] = optim_class(param_groups, **optim_kwargs)
@@ -233,34 +232,32 @@
 
         for param in trainable_params:
             param.register_post_accumulate_grad_hook(optimizer_hook)
 
         optimizer = DummyOptimizer(lr=training_args.learning_rate, optimizer_dict=optimizer_dict)
     else:
         param_groups = [
-            dict(params=nodecay_params),
+            dict(params=nodecay_params, weight_decay=0.0),
             dict(params=decay_params, weight_decay=training_args.weight_decay),
             dict(params=galore_params, weight_decay=training_args.weight_decay, **galore_kwargs),
         ]
         optimizer = optim_class(param_groups, **optim_kwargs)
 
     logger.info("Using GaLore optimizer, may cause hanging at the start of training, wait patiently.")
     return optimizer
 
 
 def _create_loraplus_optimizer(
     model: "PreTrainedModel",
     training_args: "Seq2SeqTrainingArguments",
     finetuning_args: "FinetuningArguments",
 ) -> "torch.optim.Optimizer":
-    if finetuning_args.finetuning_type != "lora":
-        raise ValueError("You should use LoRA tuning to activate LoRA+.")
-
+    default_lr = training_args.learning_rate
     loraplus_lr = training_args.learning_rate * finetuning_args.loraplus_lr_ratio
-    decay_args = {"weight_decay": training_args.weight_decay}
+    embedding_lr = finetuning_args.loraplus_lr_embedding
 
     decay_param_names = _get_decay_parameter_names(model)
     param_dict: Dict[str, List["torch.nn.Parameter"]] = {
         "lora_a": [],
         "lora_b": [],
         "lora_b_nodecay": [],
         "embedding": [],
@@ -275,52 +272,114 @@
                 else:
                     param_dict["lora_b_nodecay"].append(param)
             else:
                 param_dict["lora_a"].append(param)
 
     optim_class, optim_kwargs = Trainer.get_optimizer_cls_and_kwargs(training_args)
     param_groups = [
-        dict(params=param_dict["lora_a"], **decay_args),
-        dict(params=param_dict["lora_b"], lr=loraplus_lr, **decay_args),
-        dict(params=param_dict["lora_b_nodecay"], lr=loraplus_lr),
-        dict(params=param_dict["embedding"], lr=finetuning_args.loraplus_lr_embedding, **decay_args),
+        dict(params=param_dict["lora_a"], lr=default_lr, weight_decay=training_args.weight_decay),
+        dict(params=param_dict["lora_b"], lr=loraplus_lr, weight_decay=training_args.weight_decay),
+        dict(params=param_dict["lora_b_nodecay"], lr=loraplus_lr, weight_decay=0.0),
+        dict(params=param_dict["embedding"], lr=embedding_lr, weight_decay=training_args.weight_decay),
     ]
     optimizer = optim_class(param_groups, **optim_kwargs)
     logger.info("Using LoRA+ optimizer with loraplus lr ratio {:.2f}.".format(finetuning_args.loraplus_lr_ratio))
     return optimizer
 
 
+def _create_badam_optimizer(
+    model: "PreTrainedModel",
+    training_args: "Seq2SeqTrainingArguments",
+    finetuning_args: "FinetuningArguments",
+) -> "torch.optim.Optimizer":
+    decay_params, nodecay_params = [], []
+    decay_param_names = _get_decay_parameter_names(model)
+    for name, param in model.named_parameters():
+        if param.requires_grad:
+            if name in decay_param_names:
+                decay_params.append(param)
+            else:
+                nodecay_params.append(param)
+
+    optim_class, optim_kwargs = Trainer.get_optimizer_cls_and_kwargs(training_args)
+    param_groups = [
+        dict(params=nodecay_params, weight_decay=0.0),
+        dict(params=decay_params, weight_decay=training_args.weight_decay),
+    ]
+
+    if finetuning_args.badam_mode == "layer":
+        from badam import BlockOptimizer
+
+        base_optimizer = optim_class(param_groups, **optim_kwargs)
+        optimizer = BlockOptimizer(
+            base_optimizer=base_optimizer,
+            named_parameters_list=list(model.named_parameters()),
+            block_prefix_list=None,
+            switch_block_every=finetuning_args.badam_switch_block_every,
+            start_block=finetuning_args.badam_start_block,
+            switch_mode=finetuning_args.badam_switch_mode,
+            verbose=finetuning_args.badam_verbose,
+        )
+        logger.info(
+            f"Using BAdam optimizer with layer-wise update, switch mode is {finetuning_args.badam_switch_mode}, "
+            f"switch block every {finetuning_args.badam_switch_block_every} steps, "
+            f"default start block is {finetuning_args.badam_start_block}"
+        )
+
+    elif finetuning_args.badam_mode == "ratio":
+        from badam import BlockOptimizerRatio
+
+        assert finetuning_args.badam_update_ratio > 1e-6
+        optimizer = BlockOptimizerRatio(
+            param_groups=param_groups,
+            named_parameters_list=list(model.named_parameters()),
+            update_ratio=finetuning_args.badam_update_ratio,
+            mask_mode=finetuning_args.badam_mask_mode,
+            verbose=finetuning_args.badam_verbose,
+            include_embedding=False,
+            **optim_kwargs,
+        )
+        logger.info(
+            f"Using BAdam optimizer with ratio-wise update, update ratio is {finetuning_args.badam_update_ratio}, "
+            f"mask mode is {finetuning_args.badam_mask_mode}"
+        )
+
+    return optimizer
+
+
 def create_custom_optimzer(
     model: "PreTrainedModel",
     training_args: "Seq2SeqTrainingArguments",
     finetuning_args: "FinetuningArguments",
 ) -> Optional["torch.optim.Optimizer"]:
     if finetuning_args.use_galore:
         return _create_galore_optimizer(model, training_args, finetuning_args)
 
     if finetuning_args.loraplus_lr_ratio is not None:
         return _create_loraplus_optimizer(model, training_args, finetuning_args)
 
+    if finetuning_args.use_badam:
+        return _create_badam_optimizer(model, training_args, finetuning_args)
+
 
 def create_custom_scheduler(
     training_args: "Seq2SeqTrainingArguments",
     num_training_steps: int,
     optimizer: Optional["torch.optim.Optimizer"] = None,
 ) -> None:
     if optimizer is not None and isinstance(optimizer, DummyOptimizer):
         optimizer_dict = optimizer.optimizer_dict
         scheduler_dict: Dict["torch.nn.Parameter", "torch.optim.lr_scheduler.LRScheduler"] = {}
 
         for param in optimizer_dict.keys():
             scheduler_dict[param] = get_scheduler(
                 training_args.lr_scheduler_type,
                 optimizer=optimizer_dict[param],
-                num_warmup_steps=training_args.get_warmup_steps(num_training_steps) * 2,
-                num_training_steps=num_training_steps * 2,
+                num_warmup_steps=training_args.get_warmup_steps(num_training_steps),
+                num_training_steps=num_training_steps,
             )
 
         def scheduler_hook(param: "torch.nn.Parameter"):
-            if param.grad is not None:
-                scheduler_dict[param].step()
+            scheduler_dict[param].step()
 
         for param in optimizer_dict.keys():
             param.register_post_accumulate_grad_hook(scheduler_hook)
```

### Comparing `llmtuner-0.6.2/src/llmtuner/webui/chatter.py` & `llmtuner-0.6.3/src/llmtuner/webui/chatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import json
 import os
-from typing import TYPE_CHECKING, Any, Dict, Generator, List, Optional, Sequence, Tuple
-
-import gradio as gr
-from gradio.components import Component  # cannot use TYPE_CHECKING here
+from typing import TYPE_CHECKING, Dict, Generator, List, Optional, Sequence, Tuple
 
 from ..chat import ChatModel
 from ..data import Role
 from ..extras.misc import torch_gc
+from ..extras.packages import is_gradio_available
 from .common import get_save_dir
 from .locales import ALERTS
 
 
 if TYPE_CHECKING:
     from ..chat import BaseEngine
     from .manager import Manager
 
 
+if is_gradio_available():
+    import gradio as gr
+
+
 class WebChatModel(ChatModel):
     def __init__(self, manager: "Manager", demo_mode: bool = False, lazy_init: bool = True) -> None:
         self.manager = manager
         self.demo_mode = demo_mode
         self.engine: Optional["BaseEngine"] = None
 
         if not lazy_init:  # read arguments from command line
@@ -31,15 +33,15 @@
             template = os.environ.get("DEMO_TEMPLATE")
             super().__init__(dict(model_name_or_path=model_name_or_path, template=template))
 
     @property
     def loaded(self) -> bool:
         return self.engine is not None
 
-    def load_model(self, data: Dict[Component, Any]) -> Generator[str, None, None]:
+    def load_model(self, data) -> Generator[str, None, None]:
         get = lambda elem_id: data[self.manager.get_elem_by_id(elem_id)]
         lang = get("top.lang")
         error = ""
         if self.loaded:
             error = ALERTS["err_exists"][lang]
         elif not get("top.model_name"):
             error = ALERTS["err_no_model"][lang]
@@ -75,15 +77,15 @@
             rope_scaling=get("top.rope_scaling") if get("top.rope_scaling") in ["linear", "dynamic"] else None,
             infer_backend=get("infer.infer_backend"),
         )
         super().__init__(args)
 
         yield ALERTS["info_loaded"][lang]
 
-    def unload_model(self, data: Dict[Component, Any]) -> Generator[str, None, None]:
+    def unload_model(self, data) -> Generator[str, None, None]:
         lang = data[self.manager.get_elem_by_id("top.lang")]
 
         if self.demo_mode:
             gr.Warning(ALERTS["err_demo"][lang])
             yield ALERTS["err_demo"][lang]
             return
```

### Comparing `llmtuner-0.6.2/src/llmtuner/webui/common.py` & `llmtuner-0.6.3/src/llmtuner/webui/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import json
 import os
 from collections import defaultdict
 from typing import Any, Dict, Optional
 
-import gradio as gr
 from peft.utils import SAFETENSORS_WEIGHTS_NAME, WEIGHTS_NAME
 
 from ..extras.constants import (
     DATA_CONFIG,
     DEFAULT_MODULE,
     DEFAULT_TEMPLATE,
     PEFT_METHODS,
     STAGES_USE_PAIR_DATA,
     SUPPORTED_MODELS,
     TRAINING_STAGES,
     DownloadSource,
 )
 from ..extras.misc import use_modelscope
+from ..extras.packages import is_gradio_available
+
+
+if is_gradio_available():
+    import gradio as gr
 
 
 ADAPTER_NAMES = {WEIGHTS_NAME, SAFETENSORS_WEIGHTS_NAME}
 DEFAULT_CACHE_DIR = "cache"
 DEFAULT_CONFIG_DIR = "config"
 DEFAULT_DATA_DIR = "data"
 DEFAULT_SAVE_DIR = "saves"
```

### Comparing `llmtuner-0.6.2/src/llmtuner/webui/components/chatbot.py` & `llmtuner-0.6.3/src/llmtuner/webui/components/chatbot.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from typing import TYPE_CHECKING, Dict, Tuple
 
-import gradio as gr
-
 from ...data import Role
+from ...extras.packages import is_gradio_available
 from ..utils import check_json_schema
 
 
+if is_gradio_available():
+    import gradio as gr
+
+
 if TYPE_CHECKING:
     from gradio.components import Component
 
     from ..engine import Engine
 
 
 def create_chat_box(
```

### Comparing `llmtuner-0.6.2/src/llmtuner/webui/components/data.py` & `llmtuner-0.6.3/src/llmtuner/webui/components/data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import json
 import os
-from typing import TYPE_CHECKING, Dict, Tuple
-
-import gradio as gr
+from typing import TYPE_CHECKING, Any, Dict, List, Tuple
 
 from ...extras.constants import DATA_CONFIG
+from ...extras.packages import is_gradio_available
+
+
+if is_gradio_available():
+    import gradio as gr
 
 
 if TYPE_CHECKING:
     from gradio.components import Component
 
 
 PAGE_SIZE = 2
@@ -25,36 +28,46 @@
 def can_preview(dataset_dir: str, dataset: list) -> "gr.Button":
     try:
         with open(os.path.join(dataset_dir, DATA_CONFIG), "r", encoding="utf-8") as f:
             dataset_info = json.load(f)
     except Exception:
         return gr.Button(interactive=False)
 
-    if (
-        len(dataset) > 0
-        and "file_name" in dataset_info[dataset[0]]
-        and os.path.isfile(os.path.join(dataset_dir, dataset_info[dataset[0]]["file_name"]))
-    ):
+    if len(dataset) == 0 or "file_name" not in dataset_info[dataset[0]]:
+        return gr.Button(interactive=False)
+
+    data_path = os.path.join(dataset_dir, dataset_info[dataset[0]]["file_name"])
+    if os.path.isfile(data_path) or (os.path.isdir(data_path) and os.listdir(data_path)):
         return gr.Button(interactive=True)
     else:
         return gr.Button(interactive=False)
 
 
+def _load_data_file(file_path: str) -> List[Any]:
+    with open(file_path, "r", encoding="utf-8") as f:
+        if file_path.endswith(".json"):
+            return json.load(f)
+        elif file_path.endswith(".jsonl"):
+            return [json.loads(line) for line in f]
+        else:
+            return list(f)
+
+
 def get_preview(dataset_dir: str, dataset: list, page_index: int) -> Tuple[int, list, "gr.Column"]:
     with open(os.path.join(dataset_dir, DATA_CONFIG), "r", encoding="utf-8") as f:
         dataset_info = json.load(f)
 
-    data_file: str = dataset_info[dataset[0]]["file_name"]
-    with open(os.path.join(dataset_dir, data_file), "r", encoding="utf-8") as f:
-        if data_file.endswith(".json"):
-            data = json.load(f)
-        elif data_file.endswith(".jsonl"):
-            data = [json.loads(line) for line in f]
-        else:
-            data = [line for line in f]  # noqa: C416
+    data_path = os.path.join(dataset_dir, dataset_info[dataset[0]]["file_name"])
+    if os.path.isfile(data_path):
+        data = _load_data_file(data_path)
+    else:
+        data = []
+        for file_name in os.listdir(data_path):
+            data.extend(_load_data_file(os.path.join(data_path, file_name)))
+
     return len(data), data[PAGE_SIZE * page_index : PAGE_SIZE * (page_index + 1)], gr.Column(visible=True)
 
 
 def create_preview_box(dataset_dir: "gr.Textbox", dataset: "gr.Dropdown") -> Dict[str, "Component"]:
     data_preview_btn = gr.Button(interactive=False, scale=1)
     with gr.Column(visible=False, elem_classes="modal-box") as preview_box:
         with gr.Row():
```

### Comparing `llmtuner-0.6.2/src/llmtuner/webui/components/eval.py` & `llmtuner-0.6.3/src/llmtuner/webui/components/eval.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from typing import TYPE_CHECKING, Dict
 
-import gradio as gr
-
+from ...extras.packages import is_gradio_available
 from ..common import DEFAULT_DATA_DIR, list_dataset
 from .data import create_preview_box
 
 
+if is_gradio_available():
+    import gradio as gr
+
+
 if TYPE_CHECKING:
     from gradio.components import Component
 
     from ..engine import Engine
 
 
 def create_eval_tab(engine: "Engine") -> Dict[str, "Component"]:
     input_elems = engine.manager.get_base_elems()
     elem_dict = dict()
 
     with gr.Row():
         dataset_dir = gr.Textbox(value=DEFAULT_DATA_DIR, scale=2)
-        dataset = gr.Dropdown(multiselect=True, allow_custom_value=True, scale=4)
+        dataset = gr.Dropdown(multiselect=True, scale=4)
         preview_elems = create_preview_box(dataset_dir, dataset)
 
     input_elems.update({dataset_dir, dataset})
     elem_dict.update(dict(dataset_dir=dataset_dir, dataset=dataset, **preview_elems))
 
     with gr.Row():
         cutoff_len = gr.Slider(value=1024, minimum=4, maximum=8192, step=1)
```

### Comparing `llmtuner-0.6.2/src/llmtuner/webui/components/export.py` & `llmtuner-0.6.3/src/llmtuner/webui/components/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from typing import TYPE_CHECKING, Dict, Generator, List
 
-import gradio as gr
-
+from ...extras.packages import is_gradio_available
 from ...train import export_model
 from ..common import get_save_dir
 from ..locales import ALERTS
 
 
+if is_gradio_available():
+    import gradio as gr
+
+
 if TYPE_CHECKING:
     from gradio.components import Component
 
     from ..engine import Engine
 
 
 GPTQ_BITS = ["8", "4", "3", "2"]
```

### Comparing `llmtuner-0.6.2/src/llmtuner/webui/components/infer.py` & `llmtuner-0.6.3/src/llmtuner/webui/components/infer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from typing import TYPE_CHECKING, Dict
 
-import gradio as gr
-
+from ...extras.packages import is_gradio_available
 from .chatbot import create_chat_box
 
 
+if is_gradio_available():
+    import gradio as gr
+
+
 if TYPE_CHECKING:
     from gradio.components import Component
 
     from ..engine import Engine
 
 
 def create_infer_tab(engine: "Engine") -> Dict[str, "Component"]:
```

### Comparing `llmtuner-0.6.2/src/llmtuner/webui/components/top.py` & `llmtuner-0.6.3/src/llmtuner/webui/components/top.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from typing import TYPE_CHECKING, Dict
 
-import gradio as gr
-
 from ...data import templates
 from ...extras.constants import METHODS, SUPPORTED_MODELS
+from ...extras.packages import is_gradio_available
 from ..common import get_model_path, get_template, list_adapters, save_config
 from ..utils import can_quantize
 
 
+if is_gradio_available():
+    import gradio as gr
+
+
 if TYPE_CHECKING:
     from gradio.components import Component
 
 
 def create_top() -> Dict[str, "Component"]:
     available_models = list(SUPPORTED_MODELS.keys()) + ["Custom"]
```

### Comparing `llmtuner-0.6.2/src/llmtuner/webui/components/train.py` & `llmtuner-0.6.3/src/llmtuner/webui/components/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from typing import TYPE_CHECKING, Dict
 
-import gradio as gr
 from transformers.trainer_utils import SchedulerType
 
 from ...extras.constants import TRAINING_STAGES
+from ...extras.packages import is_gradio_available
 from ..common import DEFAULT_DATA_DIR, autoset_packing, list_adapters, list_dataset
 from ..components.data import create_preview_box
 
 
+if is_gradio_available():
+    import gradio as gr
+
+
 if TYPE_CHECKING:
     from gradio.components import Component
 
     from ..engine import Engine
 
 
 def create_train_tab(engine: "Engine") -> Dict[str, "Component"]:
@@ -19,15 +23,15 @@
     elem_dict = dict()
 
     with gr.Row():
         training_stage = gr.Dropdown(
             choices=list(TRAINING_STAGES.keys()), value=list(TRAINING_STAGES.keys())[0], scale=1
         )
         dataset_dir = gr.Textbox(value=DEFAULT_DATA_DIR, scale=1)
-        dataset = gr.Dropdown(multiselect=True, allow_custom_value=True, scale=4)
+        dataset = gr.Dropdown(multiselect=True, scale=4)
         preview_elems = create_preview_box(dataset_dir, dataset)
 
     input_elems.update({training_stage, dataset_dir, dataset})
     elem_dict.update(dict(training_stage=training_stage, dataset_dir=dataset_dir, dataset=dataset, **preview_elems))
 
     with gr.Row():
         learning_rate = gr.Textbox(value="5e-5")
```

### Comparing `llmtuner-0.6.2/src/llmtuner/webui/css.py` & `llmtuner-0.6.3/src/llmtuner/webui/css.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/webui/engine.py` & `llmtuner-0.6.3/src/llmtuner/webui/engine.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
-from typing import Any, Dict, Generator
-
-from gradio.components import Component  # cannot use TYPE_CHECKING here
+from typing import TYPE_CHECKING, Any, Dict
 
 from .chatter import WebChatModel
 from .common import get_model_path, list_dataset, load_config
 from .locales import LOCALES
 from .manager import Manager
 from .runner import Runner
 from .utils import get_time
 
 
+if TYPE_CHECKING:
+    from gradio.components import Component
+
+
 class Engine:
     def __init__(self, demo_mode: bool = False, pure_chat: bool = False) -> None:
         self.demo_mode = demo_mode
         self.pure_chat = pure_chat
         self.manager = Manager()
         self.runner = Runner(self.manager, demo_mode)
         self.chatter = WebChatModel(self.manager, demo_mode, lazy_init=(not pure_chat))
@@ -25,15 +27,15 @@
         output_dict: Dict["Component", "Component"] = {}
         for elem_id, elem_attr in input_dict.items():
             elem = self.manager.get_elem_by_id(elem_id)
             output_dict[elem] = elem.__class__(**elem_attr)
 
         return output_dict
 
-    def resume(self) -> Generator[Dict[Component, Component], None, None]:
+    def resume(self):
         user_config = load_config() if not self.demo_mode else {}
         lang = user_config.get("lang", None) or "en"
 
         init_dict = {"top.lang": {"value": lang}, "infer.chat_box": {"visible": self.chatter.loaded}}
 
         if not self.pure_chat:
             init_dict["train.dataset"] = {"choices": list_dataset().choices}
@@ -51,13 +53,13 @@
         if self.runner.alive and not self.demo_mode and not self.pure_chat:
             yield {elem: elem.__class__(value=value) for elem, value in self.runner.running_data.items()}
             if self.runner.do_train:
                 yield self._update_component({"train.resume_btn": {"value": True}})
             else:
                 yield self._update_component({"eval.resume_btn": {"value": True}})
 
-    def change_lang(self, lang: str) -> Dict[Component, Component]:
+    def change_lang(self, lang: str):
         return {
             elem: elem.__class__(**LOCALES[elem_name][lang])
             for elem_name, elem in self.manager.get_elem_iter()
             if elem_name in LOCALES
         }
```

### Comparing `llmtuner-0.6.2/src/llmtuner/webui/interface.py` & `llmtuner-0.6.3/src/llmtuner/webui/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-import gradio as gr
-
+from ..extras.packages import is_gradio_available
 from .common import save_config
 from .components import (
     create_chat_box,
     create_eval_tab,
     create_export_tab,
     create_infer_tab,
     create_top,
     create_train_tab,
 )
 from .css import CSS
 from .engine import Engine
 
 
+if is_gradio_available():
+    import gradio as gr
+
+
 def create_ui(demo_mode: bool = False) -> gr.Blocks:
     engine = Engine(demo_mode=demo_mode, pure_chat=False)
 
     with gr.Blocks(title="LLaMA Board", css=CSS) as demo:
         if demo_mode:
             gr.HTML("<h1><center>LLaMA Board: A One-stop Web UI for Getting Started with LLaMA Factory</center></h1>")
             gr.HTML(
```

### Comparing `llmtuner-0.6.2/src/llmtuner/webui/locales.py` & `llmtuner-0.6.3/src/llmtuner/webui/locales.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/webui/manager.py` & `llmtuner-0.6.3/src/llmtuner/webui/manager.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/src/llmtuner/webui/runner.py` & `llmtuner-0.6.3/src/llmtuner/webui/runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 import logging
 import os
 import time
 from threading import Thread
 from typing import TYPE_CHECKING, Any, Dict, Generator
 
-import gradio as gr
 import transformers
-from gradio.components import Component  # cannot use TYPE_CHECKING here
 from transformers.trainer import TRAINING_ARGS_NAME
 from transformers.utils import is_torch_cuda_available
 
 from ..extras.callbacks import LogCallback
 from ..extras.constants import TRAINING_STAGES
 from ..extras.logging import LoggerHandler
 from ..extras.misc import get_device_count, torch_gc
+from ..extras.packages import is_gradio_available
 from ..train import run_exp
 from .common import get_module, get_save_dir, load_args, load_config, save_args
 from .locales import ALERTS
 from .utils import gen_cmd, gen_plot, get_eval_results, update_process_bar
 
 
+if is_gradio_available():
+    import gradio as gr
+
+
 if TYPE_CHECKING:
+    from gradio.components import Component
+
     from .manager import Manager
 
 
 class Runner:
     def __init__(self, manager: "Manager", demo_mode: bool = False) -> None:
         self.manager = manager
         self.demo_mode = demo_mode
@@ -235,51 +240,51 @@
         if get("eval.predict"):
             args["do_predict"] = True
         else:
             args["do_eval"] = True
 
         return args
 
-    def _preview(self, data: Dict["Component", Any], do_train: bool) -> Generator[Dict[Component, str], None, None]:
+    def _preview(self, data: Dict["Component", Any], do_train: bool) -> Generator[Dict["Component", str], None, None]:
         output_box = self.manager.get_elem_by_id("{}.output_box".format("train" if do_train else "eval"))
         error = self._initialize(data, do_train, from_preview=True)
         if error:
             gr.Warning(error)
             yield {output_box: error}
         else:
             args = self._parse_train_args(data) if do_train else self._parse_eval_args(data)
             yield {output_box: gen_cmd(args)}
 
-    def _launch(self, data: Dict["Component", Any], do_train: bool) -> Generator[Dict[Component, Any], None, None]:
+    def _launch(self, data: Dict["Component", Any], do_train: bool) -> Generator[Dict["Component", Any], None, None]:
         output_box = self.manager.get_elem_by_id("{}.output_box".format("train" if do_train else "eval"))
         error = self._initialize(data, do_train, from_preview=False)
         if error:
             gr.Warning(error)
             yield {output_box: error}
         else:
             args = self._parse_train_args(data) if do_train else self._parse_eval_args(data)
             run_kwargs = dict(args=args, callbacks=[self.trainer_callback])
             self.do_train, self.running_data = do_train, data
             self.thread = Thread(target=run_exp, kwargs=run_kwargs)
             self.thread.start()
             yield from self.monitor()
 
-    def preview_train(self, data: Dict[Component, Any]) -> Generator[Dict[Component, str], None, None]:
+    def preview_train(self, data):
         yield from self._preview(data, do_train=True)
 
-    def preview_eval(self, data: Dict[Component, Any]) -> Generator[Dict[Component, str], None, None]:
+    def preview_eval(self, data):
         yield from self._preview(data, do_train=False)
 
-    def run_train(self, data: Dict[Component, Any]) -> Generator[Dict[Component, Any], None, None]:
+    def run_train(self, data):
         yield from self._launch(data, do_train=True)
 
-    def run_eval(self, data: Dict[Component, Any]) -> Generator[Dict[Component, Any], None, None]:
+    def run_eval(self, data):
         yield from self._launch(data, do_train=False)
 
-    def monitor(self) -> Generator[Dict[Component, Any], None, None]:
+    def monitor(self):
         get = lambda elem_id: self.running_data[self.manager.get_elem_by_id(elem_id)]
         self.aborted = False
         self.running = True
 
         lang = get("top.lang")
         model_name = get("top.model_name")
         finetuning_type = get("top.finetuning_type")
@@ -328,15 +333,15 @@
         if self.do_train:
             plot = gen_plot(output_path)
             if plot is not None:
                 return_dict[loss_viewer] = plot
 
         yield return_dict
 
-    def save_args(self, data: Dict[Component, Any]) -> Dict[Component, str]:
+    def save_args(self, data):
         output_box = self.manager.get_elem_by_id("train.output_box")
         error = self._initialize(data, do_train=True, from_preview=True)
         if error:
             gr.Warning(error)
             return {output_box: error}
 
         config_dict: Dict[str, Any] = {}
@@ -347,15 +352,15 @@
             elem_id = self.manager.get_id_by_elem(elem)
             if elem_id not in skip_ids:
                 config_dict[elem_id] = value
 
         save_path = save_args(config_path, config_dict)
         return {output_box: ALERTS["info_config_saved"][lang] + save_path}
 
-    def load_args(self, lang: str, config_path: str) -> Dict[Component, Any]:
+    def load_args(self, lang: str, config_path: str):
         output_box = self.manager.get_elem_by_id("train.output_box")
         config_dict = load_args(config_path)
         if config_dict is None:
             gr.Warning(ALERTS["err_config_not_found"][lang])
             return {output_box: ALERTS["err_config_not_found"][lang]}
 
         output_dict: Dict["Component", Any] = {output_box: ALERTS["info_config_loaded"][lang]}
```

### Comparing `llmtuner-0.6.2/src/llmtuner/webui/utils.py` & `llmtuner-0.6.3/src/llmtuner/webui/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import json
 import os
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, Dict, Optional
 
-import gradio as gr
-
-from ..extras.packages import is_matplotlib_available
+from ..extras.packages import is_gradio_available, is_matplotlib_available
 from ..extras.ploting import smooth
 from .locales import ALERTS
 
 
-if TYPE_CHECKING:
-    from ..extras.callbacks import LogCallback
+if is_gradio_available():
+    import gradio as gr
+
 
 if is_matplotlib_available():
     import matplotlib.figure
     import matplotlib.pyplot as plt
 
 
+if TYPE_CHECKING:
+    from ..extras.callbacks import LogCallback
+
+
 def update_process_bar(callback: "LogCallback") -> "gr.Slider":
     if not callback.max_steps:
         return gr.Slider(visible=False)
 
     percentage = round(100 * callback.cur_steps / callback.max_steps, 0) if callback.max_steps != 0 else 100.0
     label = "Running {:d}/{:d}: {} < {}".format(
         callback.cur_steps, callback.max_steps, callback.elapsed_time, callback.remaining_time
```

### Comparing `llmtuner-0.6.2/src/llmtuner.egg-info/PKG-INFO` & `llmtuner-0.6.3/src/llmtuner.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.6.2
+Version: 0.6.3
 Summary: Easy-to-use LLM fine-tuning framework
 Home-page: https://github.com/hiyouga/LLaMA-Factory
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -24,15 +24,15 @@
 License-File: LICENSE
 Requires-Dist: torch>=1.13.1
 Requires-Dist: transformers>=4.37.2
 Requires-Dist: datasets>=2.14.3
 Requires-Dist: accelerate>=0.27.2
 Requires-Dist: peft>=0.10.0
 Requires-Dist: trl>=0.8.1
-Requires-Dist: gradio<=4.21.0,>=4.0.0
+Requires-Dist: gradio>=4.0.0
 Requires-Dist: scipy
 Requires-Dist: einops
 Requires-Dist: sentencepiece
 Requires-Dist: protobuf
 Requires-Dist: uvicorn
 Requires-Dist: pydantic
 Requires-Dist: fastapi
@@ -46,14 +46,16 @@
 Requires-Dist: jieba; extra == "metrics"
 Requires-Dist: rouge-chinese; extra == "metrics"
 Provides-Extra: unsloth
 Requires-Dist: torch==2.2.0; extra == "unsloth"
 Requires-Dist: unsloth[cu121-ampere-torch220]; extra == "unsloth"
 Provides-Extra: galore
 Requires-Dist: galore-torch; extra == "galore"
+Provides-Extra: badam
+Requires-Dist: badam; extra == "badam"
 Provides-Extra: vllm
 Requires-Dist: vllm>=0.3.3; extra == "vllm"
 Provides-Extra: bitsandbytes
 Requires-Dist: bitsandbytes>=0.39.0; extra == "bitsandbytes"
 Provides-Extra: gptq
 Requires-Dist: optimum>=1.16.0; extra == "gptq"
 Requires-Dist: auto-gptq>=0.5.0; extra == "gptq"
@@ -72,15 +74,15 @@
 ![# LLaMA Factory](assets/logo.png)
 
 [![GitHub Repo stars](https://img.shields.io/github/stars/hiyouga/LLaMA-Factory?style=social)](https://github.com/hiyouga/LLaMA-Factory/stargazers)
 [![GitHub Code License](https://img.shields.io/github/license/hiyouga/LLaMA-Factory)](LICENSE)
 [![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Factory)](https://github.com/hiyouga/LLaMA-Factory/commits/main)
 [![PyPI](https://img.shields.io/pypi/v/llmtuner)](https://pypi.org/project/llmtuner/)
 [![Downloads](https://static.pepy.tech/badge/llmtuner)](https://pypi.org/project/llmtuner/)
-[![Citation](https://img.shields.io/badge/citation-28-green)](#projects-using-llama-factory)
+[![Citation](https://img.shields.io/badge/citation-34-green)](#projects-using-llama-factory)
 [![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/LLaMA-Factory/pulls)
 [![Discord](https://dcbadge.vercel.app/api/server/rKfvV9r9FK?compact=true&style=flat)](https://discord.gg/rKfvV9r9FK)
 [![Twitter](https://img.shields.io/twitter/follow/llamafactory_ai)](https://twitter.com/llamafactory_ai)
 [![Spaces](https://img.shields.io/badge/🤗-Open%20in%20Spaces-blue)](https://huggingface.co/spaces/hiyouga/LLaMA-Board)
 [![Studios](https://img.shields.io/badge/ModelScope-Open%20in%20Studios-blue)](https://modelscope.cn/studios/hiyouga/LLaMA-Board)
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1eRTPn37ltBbYsISy9Aw2NuI2Aq5CQrD9?usp=sharing)
 
@@ -113,15 +115,15 @@
 - [Acknowledgement](#acknowledgement)
 
 ## Features
 
 - **Various models**: LLaMA, Mistral, Mixtral-MoE, Qwen, Yi, Gemma, Baichuan, ChatGLM, Phi, etc.
 - **Integrated methods**: (Continuous) pre-training, supervised fine-tuning, reward modeling, PPO, DPO and ORPO.
 - **Scalable resources**: 32-bit full-tuning, 16-bit freeze-tuning, 16-bit LoRA and 2/4/8-bit QLoRA via AQLM/AWQ/GPTQ/LLM.int8.
-- **Advanced algorithms**: GaLore, DoRA, LongLoRA, LLaMA Pro, LoRA+, LoftQ and Agent tuning.
+- **Advanced algorithms**: GaLore, BAdam, DoRA, LongLoRA, LLaMA Pro, Mixture-of-Depths, LoRA+, LoftQ and Agent tuning.
 - **Practical tricks**: FlashAttention-2, Unsloth, RoPE scaling, NEFTune and rsLoRA.
 - **Experiment monitors**: LlamaBoard, TensorBoard, Wandb, MLflow, etc.
 - **Faster inference**: OpenAI-style API, Gradio UI and CLI with vLLM worker.
 
 ## Benchmark
 
 Compared to ChatGLM's [P-Tuning](https://github.com/THUDM/ChatGLM2-6B/tree/main/ptuning), LLaMA Factory's LoRA tuning offers up to **3.7 times faster** training speed with a better Rouge score on the advertising text generation task. By leveraging 4-bit quantization technique, LLaMA Factory's QLoRA further improves the efficiency regarding the GPU memory.
@@ -135,22 +137,30 @@
 - **GPU Memory**: Peak GPU memory usage in 4-bit quantized training. (bs=1, cutoff_len=1024)
 - We adopt `pre_seq_len=128` for ChatGLM's P-Tuning and `lora_rank=32` for LLaMA Factory's LoRA tuning.
 
 </details>
 
 ## Changelog
 
+[24/04/21] We supported **[Mixture-of-Depths](https://arxiv.org/abs/2404.02258)** according to [AstraMindAI's implementation](https://github.com/astramind-ai/Mixture-of-depths). See `examples/extras/mod` for usage.
+
+[24/04/19] We supported **Meta Llama 3** model series.
+
+[24/04/16] We supported **[BAdam](https://arxiv.org/abs/2404.02827)**. See `examples/extras/badam` for usage.
+
+[24/04/16] We supported **[unsloth](https://github.com/unslothai/unsloth)**'s long-sequence training (Llama-2-7B-56k within 24GB). It achieves **117%** speed and **50%** memory compared with FlashAttention-2, more benchmarks can be found in [this page](https://github.com/hiyouga/LLaMA-Factory/wiki/Performance-comparison).
+
+<details><summary>Full Changelog</summary>
+
 [24/03/31] We supported **[ORPO](https://arxiv.org/abs/2403.07691)**. See `examples/lora_single_gpu` for usage.
 
 [24/03/21] Our paper "[LlamaFactory: Unified Efficient Fine-Tuning of 100+ Language Models](https://arxiv.org/abs/2403.13372)" is available at arXiv!
 
 [24/03/20] We supported **FSDP+QLoRA** that fine-tunes a 70B model on 2x24GB GPUs. See `examples/extras/fsdp_qlora` for usage.
 
-<details><summary>Full Changelog</summary>
-
 [24/03/13] We supported **[LoRA+](https://arxiv.org/abs/2402.12354)**. See `examples/extras/loraplus` for usage.
 
 [24/03/07] We supported gradient low-rank projection (**[GaLore](https://arxiv.org/abs/2403.03507)**) algorithm. See `examples/extras/galore` for usage.
 
 [24/03/07] We integrated **[vLLM](https://github.com/vllm-project/vllm)** for faster and concurrent inference. Try `--infer_backend vllm` to enjoy **270%** inference speed. (LoRA is not yet supported, merge it first.)
 
 [24/02/28] We supported weight-decomposed LoRA (**[DoRA](https://arxiv.org/abs/2402.09353)**). Try `--use_dora` to activate DoRA training.
@@ -196,28 +206,30 @@
 </details>
 
 ## Supported Models
 
 | Model                                                    | Model size                  | Default module    | Template  |
 | -------------------------------------------------------- | --------------------------- | ----------------- | --------- |
 | [Baichuan2](https://huggingface.co/baichuan-inc)         | 7B/13B                      | W_pack            | baichuan2 |
-| [BLOOM](https://huggingface.co/bigscience/bloom)         | 560M/1.1B/1.7B/3B/7.1B/176B | query_key_value   | -         |
-| [BLOOMZ](https://huggingface.co/bigscience/bloomz)       | 560M/1.1B/1.7B/3B/7.1B/176B | query_key_value   | -         |
-| [ChatGLM3](https://huggingface.co/THUDM/chatglm3-6b)     | 6B                          | query_key_value   | chatglm3  |
+| [BLOOM](https://huggingface.co/bigscience)               | 560M/1.1B/1.7B/3B/7.1B/176B | query_key_value   | -         |
+| [BLOOMZ](https://huggingface.co/bigscience)              | 560M/1.1B/1.7B/3B/7.1B/176B | query_key_value   | -         |
+| [ChatGLM3](https://huggingface.co/THUDM)                 | 6B                          | query_key_value   | chatglm3  |
+| [Command-R](https://huggingface.co/CohereForAI)          | 35B/104B                    | q_proj,v_proj     | cohere    |
 | [DeepSeek (MoE)](https://huggingface.co/deepseek-ai)     | 7B/16B/67B                  | q_proj,v_proj     | deepseek  |
 | [Falcon](https://huggingface.co/tiiuae)                  | 7B/40B/180B                 | query_key_value   | falcon    |
-| [Gemma](https://huggingface.co/google)                   | 2B/7B                       | q_proj,v_proj     | gemma     |
+| [Gemma/CodeGemma](https://huggingface.co/google)         | 2B/7B                       | q_proj,v_proj     | gemma     |
 | [InternLM2](https://huggingface.co/internlm)             | 7B/20B                      | wqkv              | intern2   |
 | [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B              | q_proj,v_proj     | -         |
 | [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B                  | q_proj,v_proj     | llama2    |
-| [Mistral/Mixtral](https://huggingface.co/mistralai)      | 7B/8x7B                     | q_proj,v_proj     | mistral   |
+| [LLaMA-3](https://huggingface.co/meta-llama)             | 8B/70B                      | q_proj,v_proj     | llama3    |
+| [Mistral/Mixtral](https://huggingface.co/mistralai)      | 7B/8x7B/8x22B               | q_proj,v_proj     | mistral   |
 | [OLMo](https://huggingface.co/allenai)                   | 1B/7B                       | att_proj          | olmo      |
 | [Phi-1.5/2](https://huggingface.co/microsoft)            | 1.3B/2.7B                   | q_proj,v_proj     | -         |
 | [Qwen](https://huggingface.co/Qwen)                      | 1.8B/7B/14B/72B             | c_attn            | qwen      |
-| [Qwen1.5 (MoE)](https://huggingface.co/Qwen)             | 0.5B/1.8B/4B/7B/14B/32B/72B | q_proj,v_proj     | qwen      |
+| [Qwen1.5 (Code/MoE)](https://huggingface.co/Qwen)        | 0.5B/1.8B/4B/7B/14B/32B/72B | q_proj,v_proj     | qwen      |
 | [StarCoder2](https://huggingface.co/bigcode)             | 3B/7B/15B                   | q_proj,v_proj     | -         |
 | [XVERSE](https://huggingface.co/xverse)                  | 7B/13B/65B                  | q_proj,v_proj     | xverse    |
 | [Yi](https://huggingface.co/01-ai)                       | 6B/9B/34B                   | q_proj,v_proj     | yi        |
 | [Yuan](https://huggingface.co/IEITYuan)                  | 2B/51B/102B                 | q_proj,v_proj     | yuan      |
 
 > [!NOTE]
 > **Default module** is used for the `--lora_target` argument, you can use `--lora_target all` to specify all the available modules.
@@ -308,14 +320,15 @@
 <details><summary>Preference datasets</summary>
 
 - [HH-RLHF (en)](https://huggingface.co/datasets/Anthropic/hh-rlhf)
 - [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
 - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
 - [Orca DPO (en)](https://huggingface.co/datasets/Intel/orca_dpo_pairs)
 - [Nectar (en)](https://huggingface.co/datasets/berkeley-nest/Nectar)
+- [DPO mix (en&zh)](https://huggingface.co/datasets/hiyouga/DPO-En-Zh-20k)
 - [Orca DPO (de)](https://huggingface.co/datasets/mayflowergmbh/intel_orca_dpo_pairs_de)
 
 </details>
 
 Some datasets require confirmation before using them, so we recommend logging in with your Hugging Face account using these commands.
 
 ```bash
@@ -342,24 +355,23 @@
 | bitsandbytes | 0.39.0  | 0.43.0    |
 | flash-attn   | 2.3.0   | 2.5.6     |
 
 ### Hardware Requirement
 
 \* *estimated*
 
-| Method | Bits |   7B  |  13B  |  30B  |   70B  |   8x7B |
-| ------ | ---- | ----- | ----- | ----- | ------ | ------ |
-| Full   | AMP  | 120GB | 240GB | 600GB | 1200GB |  900GB |
-| Full   |  16  |  60GB | 120GB | 300GB |  600GB |  400GB |
-| GaLore |  16  |  16GB |  32GB |  64GB |  160GB |  120GB |
-| Freeze |  16  |  20GB |  40GB |  80GB |  200GB |  160GB |
-| LoRA   |  16  |  16GB |  32GB |  64GB |  160GB |  120GB |
-| QLoRA  |   8  |  10GB |  20GB |  40GB |   80GB |   60GB |
-| QLoRA  |   4  |   6GB |  12GB |  24GB |   48GB |   30GB |
-| QLoRA  |   2  |   4GB |   8GB |  16GB |   24GB |   18GB |
+| Method            | Bits |   7B  |  13B  |  30B  |   70B  |  8x7B |  8x22B |
+| ----------------- | ---- | ----- | ----- | ----- | ------ | ----- | ------ |
+| Full              | AMP  | 120GB | 240GB | 600GB | 1200GB | 900GB | 2400GB |
+| Full              |  16  |  60GB | 120GB | 300GB |  600GB | 400GB | 1200GB |
+| Freeze            |  16  |  20GB |  40GB |  80GB |  200GB | 160GB |  400GB |
+| LoRA/GaLore/BAdam |  16  |  16GB |  32GB |  64GB |  160GB | 120GB |  320GB |
+| QLoRA             |   8  |  10GB |  20GB |  40GB |   80GB |  60GB |  160GB |
+| QLoRA             |   4  |   6GB |  12GB |  24GB |   48GB |  30GB |   96GB |
+| QLoRA             |   2  |   4GB |   8GB |  16GB |   24GB |  18GB |   48GB |
 
 ## Getting Started
 
 ### Data Preparation
 
 Please refer to [data/README.md](data/README.md) for checking the details about the format of dataset files. You can either use datasets on HuggingFace / ModelScope hub or load the dataset in local disk.
 
@@ -372,15 +384,15 @@
 git clone https://github.com/hiyouga/LLaMA-Factory.git
 conda create -n llama_factory python=3.10
 conda activate llama_factory
 cd LLaMA-Factory
 pip install -e .[metrics]
 ```
 
-Extra dependencies available: deepspeed, metrics, unsloth, galore, vllm, bitsandbytes, gptq, awq, aqlm, qwen, modelscope, quality
+Extra dependencies available: deepspeed, metrics, unsloth, galore, badam, vllm, bitsandbytes, gptq, awq, aqlm, qwen, modelscope, quality
 
 <details><summary>For Windows users</summary>
 
 If you want to enable the quantized LoRA (QLoRA) on the Windows platform, you will be required to install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.2, please select the appropriate [release version](https://github.com/jllllll/bitsandbytes-windows-webui/releases/tag/wheels) based on your CUDA version.
 
 ```bash
 pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.41.2.post2-py3-none-win_amd64.whl
@@ -395,14 +407,15 @@
 > [!IMPORTANT]
 > LLaMA Board GUI only supports training on a single GPU, please use [CLI](#command-line-interface) for distributed training.
 
 #### Use local environment
 
 ```bash
 export CUDA_VISIBLE_DEVICES=0 # `set CUDA_VISIBLE_DEVICES=0` for Windows
+export GRADIO_SERVER_PORT=7860 # `set GRADIO_SERVER_PORT=7860` for Windows
 python src/train_web.py # or python -m llmtuner.webui.interface
 ```
 
 #### Use Docker
 
 ```bash
 docker build -f ./Dockerfile -t llama-factory:latest .
@@ -480,29 +493,35 @@
 1. Cao et al. Head-wise Shareable Attention for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.11819)
 1. Zhang et al. Enhancing Multilingual Capabilities of Large Language Models through Self-Distillation from Resource-Rich Languages. 2024. [[arxiv]](https://arxiv.org/abs/2402.12204)
 1. Kim et al. Efficient and Effective Vocabulary Expansion Towards Multilingual Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.14714)
 1. Yu et al. KIEval: A Knowledge-grounded Interactive Evaluation Framework for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2402.15043)
 1. Huang et al. Key-Point-Driven Data Synthesis with its Enhancement on Mathematical Reasoning. 2024. [[arxiv]](https://arxiv.org/abs/2403.02333)
 1. Duan et al. Negating Negatives: Alignment without Human Positive Samples via Distributional Dispreference Optimization. 2024. [[arxiv]](https://arxiv.org/abs/2403.03419)
 1. Xie and Schwertfeger. Empowering Robotics with Large Language Models: osmAG Map Comprehension with LLMs. 2024. [[arxiv]](https://arxiv.org/abs/2403.08228)
+1. Zhang et al. EDT: Improving Large Language Models' Generation by Entropy-based Dynamic Temperature Sampling. 2024. [[arxiv]](https://arxiv.org/abs/2403.14541)
 1. Weller et al. FollowIR: Evaluating and Teaching Information Retrieval Models to Follow Instructions. 2024. [[arxiv]](https://arxiv.org/abs/2403.15246)
 1. Hongbin Na. CBT-LLM: A Chinese Large Language Model for Cognitive Behavioral Therapy-based Mental Health Question Answering. 2024. [[arxiv]](https://arxiv.org/abs/2403.16008)
+1. Zan et al. CodeS: Natural Language to Code Repository via Multi-Layer Sketch. 2024. [[arxiv]](https://arxiv.org/abs/2403.16443)
+1. Liu et al. Extensive Self-Contrast Enables Feedback-Free Language Model Alignment. 2024. [[arxiv]](https://arxiv.org/abs/2404.00604)
+1. Luo et al. BAdam: A Memory Efficient Full Parameter Training Method for Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2404.02827)
+1. Du et al. Chinese Tiny LLM: Pretraining a Chinese-Centric Large Language Model. 2024. [[arxiv]](https://arxiv.org/abs/2404.04167)
+1. Liu et al. Dynamic Generation of Personalities with Large Language Models. 2024. [[arxiv]](https://arxiv.org/abs/2404.07084)
 1. **[StarWhisper](https://github.com/Yu-Yang-Li/StarWhisper)**: A large language model for Astronomy, based on ChatGLM2-6B and Qwen-14B.
 1. **[DISC-LawLLM](https://github.com/FudanDISC/DISC-LawLLM)**: A large language model specialized in Chinese legal domain, based on Baichuan-13B, is capable of retrieving and reasoning on legal knowledge.
 1. **[Sunsimiao](https://github.com/thomas-yanxin/Sunsimiao)**: A large language model specialized in Chinese medical domain, based on Baichuan-7B and ChatGLM-6B.
 1. **[CareGPT](https://github.com/WangRongsheng/CareGPT)**: A series of large language models for Chinese medical domain, based on LLaMA2-7B and Baichuan-13B.
 1. **[MachineMindset](https://github.com/PKU-YuanGroup/Machine-Mindset/)**: A series of MBTI Personality large language models, capable of giving any LLM 16 different personality types based on different datasets and training methods.
 
 </details>
 
 ## License
 
 This repository is licensed under the [Apache-2.0 License](LICENSE).
 
-Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2](https://ai.meta.com/llama/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
+Please follow the model licenses to use the corresponding model weights: [Baichuan2](https://huggingface.co/baichuan-inc/Baichuan2-7B-Base/blob/main/Community%20License%20for%20Baichuan%202%20Model.pdf) / [BLOOM](https://huggingface.co/spaces/bigscience/license) / [ChatGLM3](https://github.com/THUDM/ChatGLM3/blob/main/MODEL_LICENSE) / [Command-R](https://cohere.com/c4ai-cc-by-nc-license) / [DeepSeek](https://github.com/deepseek-ai/DeepSeek-LLM/blob/main/LICENSE-MODEL) / [Falcon](https://huggingface.co/tiiuae/falcon-180B/blob/main/LICENSE.txt) / [Gemma](https://ai.google.dev/gemma/terms) / [InternLM2](https://github.com/InternLM/InternLM#license) / [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md) / [LLaMA-2](https://ai.meta.com/llama/license/) / [LLaMA-3](https://llama.meta.com/llama3/license/) / [Mistral](LICENSE) / [OLMo](LICENSE) / [Phi-1.5/2](https://huggingface.co/microsoft/phi-1_5/resolve/main/Research%20License.docx) / [Qwen](https://github.com/QwenLM/Qwen/blob/main/Tongyi%20Qianwen%20LICENSE%20AGREEMENT) / [StarCoder2](https://huggingface.co/spaces/bigcode/bigcode-model-license-agreement) / [XVERSE](https://github.com/xverse-ai/XVERSE-13B/blob/main/MODEL_LICENSE.pdf) / [Yi](https://huggingface.co/01-ai/Yi-6B/blob/main/LICENSE) / [Yuan](https://github.com/IEIT-Yuan/Yuan-2.0/blob/main/LICENSE-Yuan)
 
 ## Citation
 
 If this work is helpful, please kindly cite as:
 
 ```bibtex
 @article{zheng2024llamafactory,
```

### Comparing `llmtuner-0.6.2/src/llmtuner.egg-info/SOURCES.txt` & `llmtuner-0.6.3/src/llmtuner.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -87,9 +87,11 @@
 src/llmtuner/webui/components/chatbot.py
 src/llmtuner/webui/components/data.py
 src/llmtuner/webui/components/eval.py
 src/llmtuner/webui/components/export.py
 src/llmtuner/webui/components/infer.py
 src/llmtuner/webui/components/top.py
 src/llmtuner/webui/components/train.py
+tests/test_attn.py
+tests/test_galore.py
 tests/test_throughput.py
 tests/test_toolcall.py
```

### Comparing `llmtuner-0.6.2/src/llmtuner.egg-info/requires.txt` & `llmtuner-0.6.3/src/llmtuner.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 torch>=1.13.1
 transformers>=4.37.2
 datasets>=2.14.3
 accelerate>=0.27.2
 peft>=0.10.0
 trl>=0.8.1
-gradio<=4.21.0,>=4.0.0
+gradio>=4.0.0
 scipy
 einops
 sentencepiece
 protobuf
 uvicorn
 pydantic
 fastapi
@@ -18,14 +18,17 @@
 
 [aqlm]
 aqlm[gpu]>=1.1.0
 
 [awq]
 autoawq
 
+[badam]
+badam
+
 [bitsandbytes]
 bitsandbytes>=0.39.0
 
 [deepspeed]
 deepspeed>=0.10.0
 
 [galore]
```

### Comparing `llmtuner-0.6.2/tests/test_throughput.py` & `llmtuner-0.6.3/tests/test_throughput.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.6.2/tests/test_toolcall.py` & `llmtuner-0.6.3/tests/test_toolcall.py`

 * *Files identical despite different names*

