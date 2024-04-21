# Comparing `tmp/lisa_on_cuda-1.0.5.tar.gz` & `tmp/lisa_on_cuda-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lisa_on_cuda-1.0.5.tar", max compression
+gzip compressed data, was "lisa_on_cuda-1.0.6.tar", max compression
```

## Comparing `lisa_on_cuda-1.0.5.tar` & `lisa_on_cuda-1.0.6.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rwxr-xr-x   0        0        0    11357 2024-02-27 10:01:49.651600 lisa_on_cuda-1.0.5/LICENSE
--rw-r--r--   0        0        0    19124 2024-03-10 13:39:40.911903 lisa_on_cuda-1.0.5/README.md
--rwxr-xr-x   0        0        0    15366 2024-03-10 17:38:06.460228 lisa_on_cuda-1.0.5/lisa_on_cuda/LISA.py
--rw-r--r--   0        0        0        0 2024-03-10 17:48:49.255341 lisa_on_cuda-1.0.5/lisa_on_cuda/__init__.py
--rw-r--r--   0        0        0       94 2024-03-17 11:54:31.262331 lisa_on_cuda-1.0.5/lisa_on_cuda/__version__.py
--rw-r--r--   0        0        0        0 2024-03-10 17:38:06.436154 lisa_on_cuda-1.0.5/lisa_on_cuda/app/__init__.py
--rwxr-xr-x   0        0        0     6933 2024-03-10 17:56:44.393418 lisa_on_cuda-1.0.5/lisa_on_cuda/app/chat.py
--rwxr-xr-x   0        0        0     1155 2024-03-18 16:53:07.386024 lisa_on_cuda-1.0.5/lisa_on_cuda/app/main.py
--rwxr-xr-x   0        0        0     5621 2024-03-10 17:55:05.058453 lisa_on_cuda-1.0.5/lisa_on_cuda/app/merge_lora_weights_and_save_hf_model.py
--rw-r--r--   0        0        0      403 2024-03-10 21:45:02.699560 lisa_on_cuda-1.0.5/lisa_on_cuda/app/routes.py
--rwxr-xr-x   0        0        0    21445 2024-03-10 17:56:19.198639 lisa_on_cuda-1.0.5/lisa_on_cuda/app/train_ds.py
--rwxr-xr-x   0        0        0       41 2024-03-10 17:38:06.461294 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/__init__.py
--rwxr-xr-x   0        0        0      293 2024-03-10 17:38:06.461805 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/constants.py
--rwxr-xr-x   0        0        0    15685 2024-03-10 17:38:06.478603 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/conversation.py
--rwxr-xr-x   0        0        0     2915 2024-03-10 17:38:06.479108 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/mm_utils.py
--rwxr-xr-x   0        0        0      149 2024-03-10 17:38:06.479986 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/__init__.py
--rwxr-xr-x   0        0        0     2076 2024-03-10 18:01:13.227847 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/apply_delta.py
--rwxr-xr-x   0        0        0     8712 2024-03-10 18:01:13.223736 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/builder.py
--rwxr-xr-x   0        0        0      891 2024-03-10 18:01:13.235286 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/consolidate.py
--rwxr-xr-x   0        0        0     5652 2024-03-10 17:38:06.482471 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/llava_llama.py
--rwxr-xr-x   0        0        0     6593 2024-03-10 17:38:06.482987 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/llava_mpt.py
--rwxr-xr-x   0        0        0     1785 2024-03-10 17:38:06.483681 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/adapt_tokenizer.py
--rwxr-xr-x   0        0        0    19787 2024-03-10 17:38:06.484195 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/attention.py
--rwxr-xr-x   0        0        0     3072 2024-03-10 17:38:06.484699 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/blocks.py
--rwxr-xr-x   0        0        0    10004 2024-03-10 17:38:06.485212 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/configuration_mpt.py
--rwxr-xr-x   0        0        0      308 2024-03-10 17:38:06.485641 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/custom_embedding.py
--rwxr-xr-x   0        0        0    34014 2024-03-10 17:38:06.486248 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/flash_attn_triton.py
--rwxr-xr-x   0        0        0    31405 2024-03-10 17:38:06.486915 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/hf_prefixlm_converter.py
--rwxr-xr-x   0        0        0     3811 2024-03-10 17:38:06.487463 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/meta_init_context.py
--rwxr-xr-x   0        0        0    22633 2024-03-10 17:38:06.487982 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/modeling_mpt.py
--rwxr-xr-x   0        0        0     3057 2024-03-10 17:38:06.488443 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/norm.py
--rwxr-xr-x   0        0        0    14273 2024-03-10 17:38:06.488968 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/param_init_fns.py
--rwxr-xr-x   0        0        0    17841 2024-03-10 18:01:13.240962 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/llava_arch.py
--rwxr-xr-x   0        0        0     2375 2024-03-10 18:01:13.219487 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/make_delta.py
--rwxr-xr-x   0        0        0      517 2024-03-10 17:38:06.490886 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/multimodal_encoder/builder.py
--rwxr-xr-x   0        0        0     2861 2024-03-10 17:38:06.491315 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/multimodal_encoder/clip_encoder.py
--rwxr-xr-x   0        0        0      987 2024-03-10 17:38:06.494938 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/utils.py
--rwxr-xr-x   0        0        0     4581 2024-03-10 17:38:06.495920 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/train/llama_flash_attn_monkey_patch.py
--rwxr-xr-x   0        0        0     2314 2024-03-10 17:38:06.496467 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/train/llava_trainer.py
--rwxr-xr-x   0        0        0    37120 2024-03-10 17:38:06.497057 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/train/train.py
--rwxr-xr-x   0        0        0      477 2024-03-10 18:01:13.231766 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/train/train_mem.py
--rwxr-xr-x   0        0        0     4014 2024-03-10 18:01:13.215938 lisa_on_cuda-1.0.5/lisa_on_cuda/llava/utils.py
--rwxr-xr-x   0        0        0      428 2024-03-10 17:38:06.498626 lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/__init__.py
--rwxr-xr-x   0        0        0    15372 2024-03-10 17:38:06.499125 lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/automatic_mask_generator.py
--rwxr-xr-x   0        0        0     2980 2024-03-10 17:38:06.499758 lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/build_sam.py
--rwxr-xr-x   0        0        0      385 2024-03-10 17:38:06.500831 lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/modeling/__init__.py
--rwxr-xr-x   0        0        0     1479 2024-03-10 17:38:06.501415 lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/modeling/common.py
--rwxr-xr-x   0        0        0    14983 2024-03-10 17:38:06.502164 lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/modeling/image_encoder.py
--rwxr-xr-x   0        0        0     6898 2024-03-10 17:38:06.502991 lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/modeling/mask_decoder.py
--rwxr-xr-x   0        0        0     9229 2024-03-10 17:38:06.503778 lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/modeling/prompt_encoder.py
--rwxr-xr-x   0        0        0     7364 2024-03-10 17:38:06.504479 lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/modeling/sam.py
--rwxr-xr-x   0        0        0     8421 2024-03-10 17:38:06.505141 lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/modeling/transformer.py
--rwxr-xr-x   0        0        0    11850 2024-03-10 17:38:06.505838 lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/predictor.py
--rwxr-xr-x   0        0        0      197 2024-03-10 17:38:06.506836 lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/utils/__init__.py
--rwxr-xr-x   0        0        0    12712 2024-03-10 17:38:06.507495 lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/utils/amg.py
--rwxr-xr-x   0        0        0     5946 2024-03-10 17:38:06.508091 lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/utils/onnx.py
--rwxr-xr-x   0        0        0     4103 2024-03-10 17:38:06.508727 lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/utils/transforms.py
--rw-r--r--   0        0        0       70 2024-03-10 17:39:20.336998 lisa_on_cuda-1.0.5/lisa_on_cuda/utils/__init__.py
--rwxr-xr-x   0        0        0     1684 2024-03-10 17:38:06.529536 lisa_on_cuda-1.0.5/lisa_on_cuda/utils/ade20k_classes.json
--rw-r--r--   0        0        0    12872 2024-03-18 20:54:32.951874 lisa_on_cuda-1.0.5/lisa_on_cuda/utils/app_helpers.py
--rwxr-xr-x   0        0        0     2281 2024-03-10 17:38:06.539596 lisa_on_cuda-1.0.5/lisa_on_cuda/utils/cocostuff_classes.txt
--rw-r--r--   0        0        0     2104 2024-03-10 17:38:06.544548 lisa_on_cuda-1.0.5/lisa_on_cuda/utils/constants.py
--rwxr-xr-x   0        0        0    10826 2024-03-10 17:38:06.545162 lisa_on_cuda-1.0.5/lisa_on_cuda/utils/conversation.py
--rwxr-xr-x   0        0        0     2951 2024-03-10 17:38:06.545571 lisa_on_cuda-1.0.5/lisa_on_cuda/utils/data_processing.py
--rwxr-xr-x   0        0        0    16400 2024-03-10 17:56:44.382410 lisa_on_cuda-1.0.5/lisa_on_cuda/utils/dataset.py
--rwxr-xr-x   0        0        0     6545 2024-03-10 17:38:06.546462 lisa_on_cuda-1.0.5/lisa_on_cuda/utils/grefcoco.py
--rwxr-xr-x   0        0        0    12839 2024-03-10 17:38:06.546916 lisa_on_cuda-1.0.5/lisa_on_cuda/utils/grefer.py
--rwxr-xr-x   0        0        0     7954 2024-03-10 17:56:44.399474 lisa_on_cuda-1.0.5/lisa_on_cuda/utils/reason_seg_dataset.py
--rwxr-xr-x   0        0        0    15139 2024-03-10 17:38:06.547953 lisa_on_cuda-1.0.5/lisa_on_cuda/utils/refer.py
--rwxr-xr-x   0        0        0    10467 2024-03-10 17:56:44.390877 lisa_on_cuda-1.0.5/lisa_on_cuda/utils/refer_seg_dataset.py
--rwxr-xr-x   0        0        0    12054 2024-03-10 17:56:44.385484 lisa_on_cuda-1.0.5/lisa_on_cuda/utils/sem_seg_dataset.py
--rw-r--r--   0        0        0     1111 2024-03-14 22:19:14.582818 lisa_on_cuda-1.0.5/lisa_on_cuda/utils/session_logger.py
--rwxr-xr-x   0        0        0     6226 2024-03-17 22:55:30.314026 lisa_on_cuda-1.0.5/lisa_on_cuda/utils/utils.py
--rwxr-xr-x   0        0        0     4609 2024-03-10 17:56:44.388029 lisa_on_cuda-1.0.5/lisa_on_cuda/utils/vqa_dataset.py
--rw-r--r--   0        0        0      911 2024-03-18 20:50:06.364069 lisa_on_cuda-1.0.5/pyproject.toml
--rw-r--r--   0        0        0    20420 1970-01-01 00:00:00.000000 lisa_on_cuda-1.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0    11357 2024-02-27 10:01:49.651600 lisa_on_cuda-1.0.6/LICENSE
+-rw-r--r--   0        0        0    19093 2024-04-19 22:32:00.431577 lisa_on_cuda-1.0.6/README.md
+-rwxr-xr-x   0        0        0    17565 2024-04-19 22:18:18.961094 lisa_on_cuda-1.0.6/lisa_on_cuda/LISA.py
+-rw-r--r--   0        0        0        0 2024-03-10 17:48:49.255341 lisa_on_cuda-1.0.6/lisa_on_cuda/__init__.py
+-rw-r--r--   0        0        0       94 2024-03-17 11:54:31.262331 lisa_on_cuda-1.0.6/lisa_on_cuda/__version__.py
+-rw-r--r--   0        0        0        0 2024-03-10 17:38:06.436154 lisa_on_cuda-1.0.6/lisa_on_cuda/app/__init__.py
+-rwxr-xr-x   0        0        0     6933 2024-03-10 17:56:44.393418 lisa_on_cuda-1.0.6/lisa_on_cuda/app/chat.py
+-rwxr-xr-x   0        0        0     1155 2024-03-18 16:53:07.386024 lisa_on_cuda-1.0.6/lisa_on_cuda/app/main.py
+-rwxr-xr-x   0        0        0     5621 2024-03-10 17:55:05.058453 lisa_on_cuda-1.0.6/lisa_on_cuda/app/merge_lora_weights_and_save_hf_model.py
+-rw-r--r--   0        0        0      403 2024-03-10 21:45:02.699560 lisa_on_cuda-1.0.6/lisa_on_cuda/app/routes.py
+-rwxr-xr-x   0        0        0    21445 2024-03-10 17:56:19.198639 lisa_on_cuda-1.0.6/lisa_on_cuda/app/train_ds.py
+-rwxr-xr-x   0        0        0       41 2024-03-10 17:38:06.461294 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/__init__.py
+-rwxr-xr-x   0        0        0      293 2024-03-10 17:38:06.461805 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/constants.py
+-rwxr-xr-x   0        0        0    15685 2024-03-10 17:38:06.478603 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/conversation.py
+-rwxr-xr-x   0        0        0     2915 2024-03-10 17:38:06.479108 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/mm_utils.py
+-rwxr-xr-x   0        0        0      149 2024-03-10 17:38:06.479986 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/__init__.py
+-rwxr-xr-x   0        0        0     2076 2024-03-10 18:01:13.227847 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/apply_delta.py
+-rwxr-xr-x   0        0        0     8712 2024-03-10 18:01:13.223736 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/builder.py
+-rwxr-xr-x   0        0        0      891 2024-03-10 18:01:13.235286 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/consolidate.py
+-rwxr-xr-x   0        0        0     5652 2024-03-10 17:38:06.482471 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/llava_llama.py
+-rwxr-xr-x   0        0        0     6593 2024-03-10 17:38:06.482987 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/llava_mpt.py
+-rwxr-xr-x   0        0        0     1785 2024-03-10 17:38:06.483681 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/adapt_tokenizer.py
+-rwxr-xr-x   0        0        0    19787 2024-03-10 17:38:06.484195 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/attention.py
+-rwxr-xr-x   0        0        0     3072 2024-03-10 17:38:06.484699 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/blocks.py
+-rwxr-xr-x   0        0        0    10004 2024-03-10 17:38:06.485212 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/configuration_mpt.py
+-rwxr-xr-x   0        0        0      308 2024-03-10 17:38:06.485641 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/custom_embedding.py
+-rwxr-xr-x   0        0        0    34014 2024-03-10 17:38:06.486248 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/flash_attn_triton.py
+-rwxr-xr-x   0        0        0    31405 2024-03-10 17:38:06.486915 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/hf_prefixlm_converter.py
+-rwxr-xr-x   0        0        0     3811 2024-03-10 17:38:06.487463 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/meta_init_context.py
+-rwxr-xr-x   0        0        0    22633 2024-03-10 17:38:06.487982 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/modeling_mpt.py
+-rwxr-xr-x   0        0        0     3057 2024-03-10 17:38:06.488443 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/norm.py
+-rwxr-xr-x   0        0        0    14273 2024-03-10 17:38:06.488968 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/param_init_fns.py
+-rwxr-xr-x   0        0        0    17841 2024-03-10 18:01:13.240962 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/llava_arch.py
+-rwxr-xr-x   0        0        0     2375 2024-03-10 18:01:13.219487 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/make_delta.py
+-rwxr-xr-x   0        0        0      517 2024-03-10 17:38:06.490886 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/multimodal_encoder/builder.py
+-rwxr-xr-x   0        0        0     2861 2024-03-10 17:38:06.491315 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/multimodal_encoder/clip_encoder.py
+-rwxr-xr-x   0        0        0      987 2024-03-10 17:38:06.494938 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/utils.py
+-rwxr-xr-x   0        0        0     4581 2024-03-10 17:38:06.495920 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/train/llama_flash_attn_monkey_patch.py
+-rwxr-xr-x   0        0        0     2314 2024-03-10 17:38:06.496467 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/train/llava_trainer.py
+-rwxr-xr-x   0        0        0    37120 2024-03-10 17:38:06.497057 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/train/train.py
+-rwxr-xr-x   0        0        0      477 2024-03-10 18:01:13.231766 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/train/train_mem.py
+-rwxr-xr-x   0        0        0     4014 2024-03-10 18:01:13.215938 lisa_on_cuda-1.0.6/lisa_on_cuda/llava/utils.py
+-rwxr-xr-x   0        0        0      428 2024-03-10 17:38:06.498626 lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/__init__.py
+-rwxr-xr-x   0        0        0    15372 2024-03-10 17:38:06.499125 lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/automatic_mask_generator.py
+-rwxr-xr-x   0        0        0     2980 2024-03-10 17:38:06.499758 lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/build_sam.py
+-rwxr-xr-x   0        0        0      385 2024-03-10 17:38:06.500831 lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/modeling/__init__.py
+-rwxr-xr-x   0        0        0     1479 2024-03-10 17:38:06.501415 lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/modeling/common.py
+-rwxr-xr-x   0        0        0    14983 2024-03-10 17:38:06.502164 lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/modeling/image_encoder.py
+-rwxr-xr-x   0        0        0     6898 2024-03-10 17:38:06.502991 lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/modeling/mask_decoder.py
+-rwxr-xr-x   0        0        0     9229 2024-03-10 17:38:06.503778 lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/modeling/prompt_encoder.py
+-rwxr-xr-x   0        0        0     7364 2024-03-10 17:38:06.504479 lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/modeling/sam.py
+-rwxr-xr-x   0        0        0     8421 2024-03-10 17:38:06.505141 lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/modeling/transformer.py
+-rwxr-xr-x   0        0        0    11850 2024-03-10 17:38:06.505838 lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/predictor.py
+-rwxr-xr-x   0        0        0      197 2024-03-10 17:38:06.506836 lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/utils/__init__.py
+-rwxr-xr-x   0        0        0    12712 2024-03-10 17:38:06.507495 lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/utils/amg.py
+-rwxr-xr-x   0        0        0     5946 2024-03-10 17:38:06.508091 lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/utils/onnx.py
+-rwxr-xr-x   0        0        0     4103 2024-03-10 17:38:06.508727 lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/utils/transforms.py
+-rw-r--r--   0        0        0       70 2024-03-10 17:39:20.336998 lisa_on_cuda-1.0.6/lisa_on_cuda/utils/__init__.py
+-rwxr-xr-x   0        0        0     1684 2024-03-10 17:38:06.529536 lisa_on_cuda-1.0.6/lisa_on_cuda/utils/ade20k_classes.json
+-rw-r--r--   0        0        0    14264 2024-04-19 22:05:52.612870 lisa_on_cuda-1.0.6/lisa_on_cuda/utils/app_helpers.py
+-rwxr-xr-x   0        0        0     2281 2024-03-10 17:38:06.539596 lisa_on_cuda-1.0.6/lisa_on_cuda/utils/cocostuff_classes.txt
+-rw-r--r--   0        0        0     2104 2024-03-10 17:38:06.544548 lisa_on_cuda-1.0.6/lisa_on_cuda/utils/constants.py
+-rwxr-xr-x   0        0        0    10826 2024-03-10 17:38:06.545162 lisa_on_cuda-1.0.6/lisa_on_cuda/utils/conversation.py
+-rwxr-xr-x   0        0        0     2951 2024-03-10 17:38:06.545571 lisa_on_cuda-1.0.6/lisa_on_cuda/utils/data_processing.py
+-rwxr-xr-x   0        0        0    16400 2024-03-10 17:56:44.382410 lisa_on_cuda-1.0.6/lisa_on_cuda/utils/dataset.py
+-rwxr-xr-x   0        0        0     6545 2024-03-10 17:38:06.546462 lisa_on_cuda-1.0.6/lisa_on_cuda/utils/grefcoco.py
+-rwxr-xr-x   0        0        0    12839 2024-03-10 17:38:06.546916 lisa_on_cuda-1.0.6/lisa_on_cuda/utils/grefer.py
+-rwxr-xr-x   0        0        0     7954 2024-03-10 17:56:44.399474 lisa_on_cuda-1.0.6/lisa_on_cuda/utils/reason_seg_dataset.py
+-rwxr-xr-x   0        0        0    15139 2024-03-10 17:38:06.547953 lisa_on_cuda-1.0.6/lisa_on_cuda/utils/refer.py
+-rwxr-xr-x   0        0        0    10467 2024-03-10 17:56:44.390877 lisa_on_cuda-1.0.6/lisa_on_cuda/utils/refer_seg_dataset.py
+-rwxr-xr-x   0        0        0    12054 2024-03-10 17:56:44.385484 lisa_on_cuda-1.0.6/lisa_on_cuda/utils/sem_seg_dataset.py
+-rw-r--r--   0        0        0     1111 2024-03-14 22:19:14.582818 lisa_on_cuda-1.0.6/lisa_on_cuda/utils/session_logger.py
+-rwxr-xr-x   0        0        0     6226 2024-03-17 22:55:30.314026 lisa_on_cuda-1.0.6/lisa_on_cuda/utils/utils.py
+-rwxr-xr-x   0        0        0     4609 2024-03-10 17:56:44.388029 lisa_on_cuda-1.0.6/lisa_on_cuda/utils/vqa_dataset.py
+-rw-r--r--   0        0        0      911 2024-04-19 22:28:50.614601 lisa_on_cuda-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    20389 1970-01-01 00:00:00.000000 lisa_on_cuda-1.0.6/PKG-INFO
```

### Comparing `lisa_on_cuda-1.0.5/LICENSE` & `lisa_on_cuda-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/README.md` & `lisa_on_cuda-1.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 sdk: docker
 pinned: false
 ---
 
 # exec jupyter on the remote server with port forwarding on localhost
 
 1. checkout repo, install venv with jupyter
-2. port forwarding in localhost wiht private key: `ssh -i ~/.ssh/id_ecdsa_saturncloud trincuz@ssh.community.saturnenterprise.io -L 8889:localhost:8889 -N -f`
+2. port forwarding in localhost wiht private key: `ssh -i /path/to/private_key name@endpoint.com -L 8889:localhost:8889 -N -f`
 3. start the jupyter-lab server
 4. connect to page in localhost
 
 ## Commands to work on saturncloud after clone and git lfs install
 ```bash
 cd ~/workspace/lisa-on-cuda/
 rm -rf lisa_venv
```

#### html2text {}

```diff
@@ -1,28 +1,27 @@
 --- title: LISA On Cuda emoji: ð colorFrom: yellow colorTo: red sdk: docker
 pinned: false --- # exec jupyter on the remote server with port forwarding on
 localhost 1. checkout repo, install venv with jupyter 2. port forwarding in
-localhost wiht private key: `ssh -i ~/.ssh/id_ecdsa_saturncloud
-trincuz@ssh.community.saturnenterprise.io -L 8889:localhost:8889 -N -f` 3.
-start the jupyter-lab server 4. connect to page in localhost ## Commands to
-work on saturncloud after clone and git lfs install ```bash cd ~/workspace/
-lisa-on-cuda/ rm -rf lisa_venv python3 -m venv lisa_venv ln -s lisa_venv/ venv
-source venv/bin/activate pip --version which python python -m pip install pip
-wheel --upgrade python -m pip install pytest pytest-cov jupyterlab python -
-m pip install -r requirements.txt nohup jupyter-lab & tail -F nohup.out ``` #
-Jupyterlab Howto To run the `test.ipynb` notebook you should already: - cloned
-project https://huggingface.co/spaces/aletrn/lisa-on-cuda with active git lfs -
-created and activated a virtualenv - installed jupyterlab dependencies from
-requirements_jupyter.txt - installed dependencies from requirements.txt ##
-Hardware requirements - an nvidia gpu with 10 or 12GB of memory (a T4 should
-suffice) - at least 16GB of system ram [![Gradio](https://img.shields.io/badge/
-Gradio-Online%20Demo-blue)](http://103.170.5.190:7860/) [![Open in OpenXLab]
-(https://cdn-static.openxlab.org.cn/app-center/openxlab_app.svg)](https://
-openxlab.org.cn/apps/detail/openxlab-app/LISA) # LISA: Reasoning Segmentation
-via Large Language Model
+localhost wiht private key: `ssh -i /path/to/private_key name@endpoint.com -
+L 8889:localhost:8889 -N -f` 3. start the jupyter-lab server 4. connect to page
+in localhost ## Commands to work on saturncloud after clone and git lfs install
+```bash cd ~/workspace/lisa-on-cuda/ rm -rf lisa_venv python3 -m venv lisa_venv
+ln -s lisa_venv/ venv source venv/bin/activate pip --version which python
+python -m pip install pip wheel --upgrade python -m pip install pytest pytest-
+cov jupyterlab python -m pip install -r requirements.txt nohup jupyter-lab &
+tail -F nohup.out ``` # Jupyterlab Howto To run the `test.ipynb` notebook you
+should already: - cloned project https://huggingface.co/spaces/aletrn/lisa-on-
+cuda with active git lfs - created and activated a virtualenv - installed
+jupyterlab dependencies from requirements_jupyter.txt - installed dependencies
+from requirements.txt ## Hardware requirements - an nvidia gpu with 10 or 12GB
+of memory (a T4 should suffice) - at least 16GB of system ram [![Gradio](https:
+//img.shields.io/badge/Gradio-Online%20Demo-blue)](http://103.170.5.190:7860/)
+[![Open in OpenXLab](https://cdn-static.openxlab.org.cn/app-center/
+openxlab_app.svg)](https://openxlab.org.cn/apps/detail/openxlab-app/LISA) #
+LISA: Reasoning Segmentation via Large Language Model
             LLIISSAA: Large LLanguage IInstructed SSegmentation AAssistant
      _*_*_P_a_p_e_r_*_* | _*_*_M_o_d_e_l_s_*_* | [**Training**](#training) | [**Inference**]
 (#inference) | [**Local Deployment**](#deployment) | [**Dataset**](#dataset) |
                                 _*_*_O_n_l_i_n_e_ _D_e_m_o_*_*
           IInnppuutt              OOuuttppuutt               IInnppuutt             OOuuttppuutt
 [resources/imgs/    [vis_output/        [resources/imgs/    [vis_output/
 obama.jpg]          obama.jpg]          trump.jpg]          trump.jpg]
```

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/LISA.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/LISA.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from .llava.model.language_model.llava_llama import (LlavaLlamaForCausalLM, LlavaLlamaModel)
 from .segment_anything import build_sam_vit_h
 
+embedding_dict = {}
+
 
 def dice_loss(
-    inputs: torch.Tensor,
-    targets: torch.Tensor,
-    num_masks: float,
-    scale=1000,  # 100000.0,
-    eps=1e-6,
+        inputs: torch.Tensor,
+        targets: torch.Tensor,
+        num_masks: float,
+        scale=1000,  # 100000.0,
+        eps=1e-6,
 ):
     """
     Compute the DICE loss, similar to generalized IOU for masks
     Args:
         inputs: A float tensor of arbitrary shape.
                 The predictions for each example.
         targets: A float tensor with the same shape as inputs. Stores the binary
@@ -31,17 +33,17 @@
     denominator = (inputs / scale).sum(-1) + (targets / scale).sum(-1)
     loss = 1 - (numerator + eps) / (denominator + eps)
     loss = loss.sum() / (num_masks + 1e-8)
     return loss
 
 
 def sigmoid_ce_loss(
-    inputs: torch.Tensor,
-    targets: torch.Tensor,
-    num_masks: float,
+        inputs: torch.Tensor,
+        targets: torch.Tensor,
+        num_masks: float,
 ):
     """
     Args:
         inputs: A float tensor of arbitrary shape.
                 The predictions for each example.
         targets: A float tensor with the same shape as inputs. Stores the binary
                  classification label for each element in inputs
@@ -52,17 +54,17 @@
     loss = F.binary_cross_entropy_with_logits(inputs, targets, reduction="none")
     loss = loss.flatten(1, 2).mean(1).sum() / (num_masks + 1e-8)
     return loss
 
 
 class LisaMetaModel:
     def __init__(
-        self,
-        config,
-        **kwargs,
+            self,
+            config,
+            **kwargs,
     ):
         super(LisaMetaModel, self).__init__(config)
 
         self.config = config
         if not hasattr(self.config, "train_mask_decoder"):
             self.config.train_mask_decoder = kwargs["train_mask_decoder"]
             self.config.out_dim = kwargs["out_dim"]
@@ -94,17 +96,17 @@
         self.text_hidden_fcs.train()
         for param in self.text_hidden_fcs.parameters():
             param.requires_grad = True
 
 
 class LisaModel(LisaMetaModel, LlavaLlamaModel):
     def __init__(
-        self,
-        config,
-        **kwargs,
+            self,
+            config,
+            **kwargs,
     ):
         super(LisaModel, self).__init__(config, **kwargs)
 
         self.config.use_cache = False
         self.config.vision_tower = self.config.mm_vision_tower
         self.config.mm_vision_select_feature = "patch"
         self.config.image_aspect_ratio = "square"
@@ -113,29 +115,29 @@
         self.config.freeze_mm_mlp_adapter = True
         self.config.pretrain_mm_mlp_adapter = None
         self.config.mm_use_im_patch_token = False
 
 
 class LISAForCausalLM(LlavaLlamaForCausalLM):
     def __init__(
-        self,
-        config,
-        **kwargs,
+            self,
+            config,
+            **kwargs,
     ):
         if not hasattr(config, "train_mask_decoder"):
             config.mm_use_im_start_end = kwargs.pop("use_mm_start_end", True)
             config.mm_vision_tower = kwargs.get(
                 "vision_tower", "openai/clip-vit-large-patch14"
             )
             self.ce_loss_weight = kwargs.pop("ce_loss_weight", None)
             self.dice_loss_weight = kwargs.pop("dice_loss_weight", None)
             self.bce_loss_weight = kwargs.pop("bce_loss_weight", None)
         else:
             config.mm_vision_tower = config.vision_tower
-            
+
         self.seg_token_idx = kwargs.pop("seg_token_idx")
 
         super().__init__(config)
 
         self.model = LisaModel(config, **kwargs)
 
         self.lm_head = nn.Linear(config.hidden_size, config.vocab_size, bias=False)
@@ -158,26 +160,26 @@
 
     def forward(self, **kwargs):
         if "past_key_values" in kwargs:
             return super().forward(**kwargs)
         return self.model_forward(**kwargs)
 
     def model_forward(
-        self,
-        images: torch.FloatTensor,
-        images_clip: torch.FloatTensor,
-        input_ids: torch.LongTensor,
-        labels: torch.LongTensor,
-        attention_masks: torch.LongTensor,
-        offset: torch.LongTensor,
-        masks_list: List[torch.FloatTensor],
-        label_list: List[torch.Tensor],
-        resize_list: List[tuple],
-        inference: bool = False,
-        **kwargs,
+            self,
+            images: torch.FloatTensor,
+            images_clip: torch.FloatTensor,
+            input_ids: torch.LongTensor,
+            labels: torch.LongTensor,
+            attention_masks: torch.LongTensor,
+            offset: torch.LongTensor,
+            masks_list: List[torch.FloatTensor],
+            label_list: List[torch.Tensor],
+            resize_list: List[tuple],
+            inference: bool = False,
+            **kwargs,
     ):
         image_embeddings = self.get_visual_embs(images)
         batch_size = image_embeddings.shape[0]
         assert batch_size == len(offset) - 1
 
         seg_token_mask = input_ids[:, 1:] == self.seg_token_idx
         seg_token_mask = torch.cat(
@@ -305,25 +307,25 @@
         mask_dice_loss = 0
         num_masks = 0
         for batch_idx in range(len(pred_masks)):
             gt_mask = gt_masks[batch_idx]
             pred_mask = pred_masks[batch_idx]
 
             assert (
-                gt_mask.shape[0] == pred_mask.shape[0]
+                    gt_mask.shape[0] == pred_mask.shape[0]
             ), "gt_mask.shape: {}, pred_mask.shape: {}".format(
                 gt_mask.shape, pred_mask.shape
             )
             mask_bce_loss += (
-                sigmoid_ce_loss(pred_mask, gt_mask, num_masks=gt_mask.shape[0])
-                * gt_mask.shape[0]
+                    sigmoid_ce_loss(pred_mask, gt_mask, num_masks=gt_mask.shape[0])
+                    * gt_mask.shape[0]
             )
             mask_dice_loss += (
-                dice_loss(pred_mask, gt_mask, num_masks=gt_mask.shape[0])
-                * gt_mask.shape[0]
+                    dice_loss(pred_mask, gt_mask, num_masks=gt_mask.shape[0])
+                    * gt_mask.shape[0]
             )
             num_masks += gt_mask.shape[0]
 
         mask_bce_loss = self.bce_loss_weight * mask_bce_loss / (num_masks + 1e-8)
         mask_dice_loss = self.dice_loss_weight * mask_dice_loss / (num_masks + 1e-8)
         mask_loss = mask_bce_loss + mask_dice_loss
 
@@ -334,89 +336,120 @@
             "ce_loss": ce_loss,
             "mask_bce_loss": mask_bce_loss,
             "mask_dice_loss": mask_dice_loss,
             "mask_loss": mask_loss,
         }
 
     def evaluate(
-        self,
-        images_clip,
-        images,
-        input_ids,
-        resize_list,
-        original_size_list,
-        max_new_tokens=32,
-        tokenizer=None,
+            self,
+            images_clip,
+            images,
+            input_ids,
+            resize_list,
+            original_size_list,
+            max_new_tokens=32,
+            tokenizer=None,
+            model_logger=None,
+            embedding_key=None
     ):
         with torch.no_grad():
+            if model_logger is None:
+                import logging
+                model_logger = logging
+            model_logger.debug("start output generation...")
             outputs = self.generate(
                 images=images_clip,
                 input_ids=input_ids,
                 max_new_tokens=max_new_tokens,
                 num_beams=1,
                 output_hidden_states=True,
                 return_dict_in_generate=True,
             )
+            model_logger.debug("done output generation...")
             output_hidden_states = outputs.hidden_states[-1]
             output_ids = outputs.sequences
 
             seg_token_mask = output_ids[:, 1:] == self.seg_token_idx
             # hack for IMAGE_TOKEN_INDEX (we suppose that there is only one image, and it is in the front)
+            model_logger.debug(f"start torch.cat to seg_token_mask...")
             seg_token_mask = torch.cat(
                 [
                     torch.zeros((seg_token_mask.shape[0], 255)).bool().cuda(),
                     seg_token_mask,
                 ],
                 dim=1,
             )
+            model_logger.debug("done torch.cat to seg_token_mask...")
 
             hidden_states = []
 
             assert len(self.model.text_hidden_fcs) == 1
             hidden_states.append(self.model.text_hidden_fcs[0](output_hidden_states))
 
+            model_logger.debug("start torch.stack to last_hidden_state...")
             last_hidden_state = torch.stack(hidden_states, dim=-1).sum(dim=-1)
+            model_logger.debug("done torch.stack to last_hidden_state...")
             pred_embeddings = last_hidden_state[seg_token_mask]
 
             seg_token_counts = seg_token_mask.int().sum(-1)  # [bs, ]
             seg_token_offset = seg_token_counts.cumsum(-1)
+            model_logger.debug(f"start torch.cat to seg_token_offset...")
             seg_token_offset = torch.cat(
                 [torch.zeros(1).long().cuda(), seg_token_offset], dim=0
             )
+            model_logger.debug("done torch.cat to seg_token_offset...")
 
             pred_embeddings_ = []
             for i in range(len(seg_token_offset) - 1):
                 start_i, end_i = seg_token_offset[i], seg_token_offset[i + 1]
                 pred_embeddings_.append(pred_embeddings[start_i:end_i])
             pred_embeddings = pred_embeddings_
 
-            image_embeddings = self.get_visual_embs(images)
+            model_logger.debug(f"start get_visual_embs to image_embeddings with embedding_key {embedding_key}.")
+
+            if embedding_key is None:
+                image_embeddings = self.get_visual_embs(images)
+            else:
+                try:
+                    image_embeddings = embedding_dict[embedding_key]
+                except KeyError:
+                    model_logger.debug(f"embedding_key {embedding_key} not in embedding_dict, creating embedding now!")
+                    image_embeddings = self.get_visual_embs(images)
+                    embedding_dict[embedding_key] = image_embeddings
+                    model_logger.debug(f"image embedding added in embedding_dict with embedding_key {embedding_key}!")
+
+            model_logger.debug("done get_visual_embs to image_embeddings...")
 
             multimask_output = False
             pred_masks = []
             for i in range(len(pred_embeddings)):
+                model_logger.debug(f"start ({i}nth time) visual_model.prompt_encoder to sparse/dense")
                 (
                     sparse_embeddings,
                     dense_embeddings,
                 ) = self.model.visual_model.prompt_encoder(
                     points=None,
                     boxes=None,
                     masks=None,
                     text_embeds=pred_embeddings[i].unsqueeze(1),
                 )
-
+                model_logger.debug(f"done ({i}nth) visual_model.prompt_encoder to sparse/dense, start sparse2sparse")
                 sparse_embeddings = sparse_embeddings.to(pred_embeddings[i].dtype)
+                model_logger.debug(f"done ({i}nth) sparse2sparse, start visual_model.mask_decoder")
                 low_res_masks, iou_predictions = self.model.visual_model.mask_decoder(
                     image_embeddings=image_embeddings[i].unsqueeze(0),
                     image_pe=self.model.visual_model.prompt_encoder.get_dense_pe(),
                     sparse_prompt_embeddings=sparse_embeddings,
                     dense_prompt_embeddings=dense_embeddings,
                     multimask_output=multimask_output,
                 )
+                model_logger.debug(f"done ({i}nth) visual_model.mask_decoder, start postprocess_masks")
                 pred_mask = self.model.visual_model.postprocess_masks(
                     low_res_masks,
                     input_size=resize_list[i],
                     original_size=original_size_list[i],
                 )
+                model_logger.debug(f"done ({i}nth) postprocess_masks")
                 pred_masks.append(pred_mask[:, 0])
 
+        model_logger.debug(f"env evaluate! ")
         return output_ids, pred_masks
```

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/app/chat.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/app/chat.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/app/main.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/app/main.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/app/merge_lora_weights_and_save_hf_model.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/app/merge_lora_weights_and_save_hf_model.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/app/train_ds.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/app/train_ds.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/conversation.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/conversation.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/mm_utils.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/mm_utils.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/apply_delta.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/apply_delta.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/builder.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/builder.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/consolidate.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/consolidate.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/llava_llama.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/llava_llama.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/llava_mpt.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/llava_mpt.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/adapt_tokenizer.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/adapt_tokenizer.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/attention.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/attention.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/blocks.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/blocks.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/configuration_mpt.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/configuration_mpt.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/flash_attn_triton.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/flash_attn_triton.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/hf_prefixlm_converter.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/hf_prefixlm_converter.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/meta_init_context.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/meta_init_context.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/modeling_mpt.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/modeling_mpt.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/norm.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/norm.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/language_model/mpt/param_init_fns.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/language_model/mpt/param_init_fns.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/llava_arch.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/llava_arch.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/make_delta.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/make_delta.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/multimodal_encoder/builder.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/multimodal_encoder/builder.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/multimodal_encoder/clip_encoder.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/multimodal_encoder/clip_encoder.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/model/utils.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/model/utils.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/train/llama_flash_attn_monkey_patch.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/train/llama_flash_attn_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/train/llava_trainer.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/train/llava_trainer.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/train/train.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/train/train.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/llava/utils.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/llava/utils.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/automatic_mask_generator.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/automatic_mask_generator.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/build_sam.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/build_sam.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/modeling/common.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/modeling/common.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/modeling/image_encoder.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/modeling/image_encoder.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/modeling/mask_decoder.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/modeling/mask_decoder.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/modeling/prompt_encoder.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/modeling/prompt_encoder.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/modeling/sam.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/modeling/sam.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/modeling/transformer.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/modeling/transformer.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/predictor.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/predictor.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/utils/amg.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/utils/amg.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/utils/onnx.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/segment_anything/utils/transforms.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/segment_anything/utils/transforms.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/utils/ade20k_classes.json` & `lisa_on_cuda-1.0.6/lisa_on_cuda/utils/ade20k_classes.json`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/utils/app_helpers.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/utils/app_helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -207,16 +207,20 @@
 def get_inference_model_by_args(args_to_parse):
     logging.info(f"args_to_parse:{args_to_parse}, creating model...")
     model, clip_image_processor, tokenizer, transform = get_model(args_to_parse)
     logging.info("created model, preparing inference function")
     no_seg_out = placeholders["no_seg_out"]
 
     @session_logger.set_uuid_logging
-    def inference(input_str: str, input_image: str | np.ndarray, internal_logger: logging = None):
-
+    def inference(
+            input_str: str,
+            input_image: str | np.ndarray,
+            internal_logger: logging = None,
+            embedding_key: str = None
+    ):
         if internal_logger is None:
             internal_logger = app_logger
 
         # filter out special chars
         input_str = get_cleaned_input(input_str)
         internal_logger.info(f" input_str type: {type(input_str)}, input_image type: {type(input_image)}.")
         internal_logger.info(f"input_str: {input_str}, input_image: {type(input_image)}.")
@@ -251,48 +255,53 @@
 
         internal_logger.info("read and preprocess image.")
         image_np = input_image
         if isinstance(input_image, str):
             image_np = cv2.imread(input_image)
             image_np = cv2.cvtColor(image_np, cv2.COLOR_BGR2RGB)
         original_size_list = [image_np.shape[:2]]
-
+        app_logger.debug("start clip_image_processor.preprocess")
         image_clip = (
             clip_image_processor.preprocess(image_np, return_tensors="pt")[
                 "pixel_values"
             ][0]
             .unsqueeze(0)
             .cuda()
         )
+        app_logger.debug("done clip_image_processor.preprocess")
         internal_logger.info(f"image_clip type: {type(image_clip)}.")
         image_clip = set_image_precision_by_args(image_clip, args_to_parse.precision)
 
         image = transform.apply_image(image_np)
         resize_list = [image.shape[:2]]
 
+        internal_logger.debug(f"starting preprocess image: {type(image_clip)}.")
         image = (
             preprocess(torch.from_numpy(image).permute(2, 0, 1).contiguous())
             .unsqueeze(0)
             .cuda()
         )
-        internal_logger.info(f"image_clip type: {type(image_clip)}.")
+        internal_logger.info(f"done preprocess image:{type(image)}, image_clip type: {type(image_clip)}.")
         image = set_image_precision_by_args(image, args_to_parse.precision)
 
         input_ids = tokenizer_image_token(prompt, tokenizer, return_tensors="pt")
         input_ids = input_ids.unsqueeze(0).cuda()
 
-        internal_logger.info("start model evaluation...")
+        embedding_key = get_hash_array(embedding_key, image, internal_logger)
+        internal_logger.info(f"start model evaluation with embedding_key {embedding_key}.")
         output_ids, pred_masks = model.evaluate(
             image_clip,
             image,
             input_ids,
             resize_list,
             original_size_list,
             max_new_tokens=512,
             tokenizer=tokenizer,
+            model_logger=internal_logger,
+            embedding_key=embedding_key
         )
         internal_logger.info("model evaluation done, start token decoding...")
         output_ids = output_ids[0][output_ids[0] != utils.IMAGE_TOKEN_INDEX]
 
         text_output = tokenizer.decode(output_ids, skip_special_tokens=False)
         text_output = text_output.replace("\n", "").replace("  ", " ")
         text_output = text_output.split("ASSISTANT: ")[-1]
@@ -343,10 +352,29 @@
         description=constants.description,
         article=constants.article,
         examples=constants.examples,
         allow_flagging="auto"
     )
 
 
+def get_hash_array(embedding_key: str, arr: np.ndarray | torch.Tensor, model_logger: logging):
+    from base64 import b64encode
+    from hashlib import sha256
+
+    model_logger.debug(f"embedding_key {embedding_key} is None? {embedding_key is None}.")
+    if embedding_key is None:
+        img2hash = arr
+        if isinstance(arr, torch.Tensor):
+            model_logger.debug("images variable is a Tensor, start converting back to numpy")
+            img2hash = arr.numpy(force=True)
+            model_logger.debug("done Tensor converted back to numpy")
+        model_logger.debug("start image hashing")
+        img2hash_fn = sha256(img2hash)
+        embedding_key = b64encode(img2hash_fn.digest())
+        embedding_key = embedding_key.decode("utf-8")
+        model_logger.debug(f"done image hashing, now embedding_key is {embedding_key}.")
+    return embedding_key
+
+
 if __name__ == '__main__':
     parsed_args = parse_args([])
     print("arrrrg:", parsed_args)
```

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/utils/cocostuff_classes.txt` & `lisa_on_cuda-1.0.6/lisa_on_cuda/utils/cocostuff_classes.txt`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/utils/constants.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/utils/constants.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/utils/conversation.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/utils/conversation.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/utils/data_processing.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/utils/data_processing.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/utils/dataset.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/utils/grefcoco.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/utils/grefcoco.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/utils/grefer.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/utils/grefer.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/utils/reason_seg_dataset.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/utils/reason_seg_dataset.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/utils/refer.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/utils/refer.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/utils/refer_seg_dataset.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/utils/refer_seg_dataset.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/utils/sem_seg_dataset.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/utils/sem_seg_dataset.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/utils/session_logger.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/utils/session_logger.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/utils/utils.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/lisa_on_cuda/utils/vqa_dataset.py` & `lisa_on_cuda-1.0.6/lisa_on_cuda/utils/vqa_dataset.py`

 * *Files identical despite different names*

### Comparing `lisa_on_cuda-1.0.5/pyproject.toml` & `lisa_on_cuda-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "lisa-on-cuda"
-version = "1.0.5"
+version = "1.0.6"
 description = ""
 authors = ["alessandro trinca tornidor <alessandro@trinca.tornidor.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [metadata]
 name = "lisa-on-cuda"
-version = "1.0.5"
+version = "1.0.6"
 
 [tool.poetry.dependencies]
 python = "~3.10"
 einops = "^0.7.0"
 fastapi = "^0.110.0"
 gradio = "^4.21.0"
 gradio-client = "^0.12.0"
```

### Comparing `lisa_on_cuda-1.0.5/PKG-INFO` & `lisa_on_cuda-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lisa-on-cuda
-Version: 1.0.5
+Version: 1.0.6
 Summary: 
 License: Apache 2.0
 Author: alessandro trinca tornidor
 Author-email: alessandro@trinca.tornidor.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -41,15 +41,15 @@
 sdk: docker
 pinned: false
 ---
 
 # exec jupyter on the remote server with port forwarding on localhost
 
 1. checkout repo, install venv with jupyter
-2. port forwarding in localhost wiht private key: `ssh -i ~/.ssh/id_ecdsa_saturncloud trincuz@ssh.community.saturnenterprise.io -L 8889:localhost:8889 -N -f`
+2. port forwarding in localhost wiht private key: `ssh -i /path/to/private_key name@endpoint.com -L 8889:localhost:8889 -N -f`
 3. start the jupyter-lab server
 4. connect to page in localhost
 
 ## Commands to work on saturncloud after clone and git lfs install
 ```bash
 cd ~/workspace/lisa-on-cuda/
 rm -rf lisa_venv
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lisa-on-cuda Version: 1.0.5 Summary: License:
+Metadata-Version: 2.1 Name: lisa-on-cuda Version: 1.0.6 Summary: License:
 Apache 2.0 Author: alessandro trinca tornidor Author-email:
 alessandro@trinca.tornidor.com Requires-Python: >=3.10,<3.11 Classifier:
 License :: Other/Proprietary License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.10 Requires-Dist:
 bitsandbytes (>=0.42.0,<0.43.0) Requires-Dist: einops (>=0.7.0,<0.8.0)
 Requires-Dist: fastapi (>=0.110.0,<0.111.0) Requires-Dist: gradio
 (>=4.21.0,<5.0.0) Requires-Dist: gradio-client (>=0.12.0,<0.13.0) Requires-
@@ -15,18 +15,17 @@
 shortuuid (>=1.0.12,<2.0.0) Requires-Dist: torch (>=2.2.1,<3.0.0) Requires-
 Dist: torchvision (>=0.17.1,<0.18.0) Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Requires-Dist: transformers (==4.31.0) Requires-Dist: uvicorn
 (>=0.28.0,<0.29.0) Description-Content-Type: text/markdown --- title: LISA On
 Cuda emoji: ð colorFrom: yellow colorTo: red sdk: docker pinned: false --- #
 exec jupyter on the remote server with port forwarding on localhost 1. checkout
 repo, install venv with jupyter 2. port forwarding in localhost wiht private
-key: `ssh -i ~/.ssh/id_ecdsa_saturncloud
-trincuz@ssh.community.saturnenterprise.io -L 8889:localhost:8889 -N -f` 3.
-start the jupyter-lab server 4. connect to page in localhost ## Commands to
-work on saturncloud after clone and git lfs install ```bash cd ~/workspace/
+key: `ssh -i /path/to/private_key name@endpoint.com -L 8889:localhost:8889 -N -
+f` 3. start the jupyter-lab server 4. connect to page in localhost ## Commands
+to work on saturncloud after clone and git lfs install ```bash cd ~/workspace/
 lisa-on-cuda/ rm -rf lisa_venv python3 -m venv lisa_venv ln -s lisa_venv/ venv
 source venv/bin/activate pip --version which python python -m pip install pip
 wheel --upgrade python -m pip install pytest pytest-cov jupyterlab python -
 m pip install -r requirements.txt nohup jupyter-lab & tail -F nohup.out ``` #
 Jupyterlab Howto To run the `test.ipynb` notebook you should already: - cloned
 project https://huggingface.co/spaces/aletrn/lisa-on-cuda with active git lfs -
 created and activated a virtualenv - installed jupyterlab dependencies from
```

