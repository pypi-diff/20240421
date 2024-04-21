# Comparing `tmp/langfun-0.0.2.dev20240419.tar.gz` & `tmp/langfun-0.0.2.dev20240420.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240419.tar", last modified: Fri Apr 19 08:03:47 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240420.tar", last modified: Sat Apr 20 08:03:38 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240419.tar` & `langfun-0.0.2.dev20240420.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.283416 langfun-0.0.2.dev20240419/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-19 08:03:47.283416 langfun-0.0.2.dev20240419/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.263416 langfun-0.0.2.dev20240419/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.271416 langfun-0.0.2.dev20240419/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.271416 langfun-0.0.2.dev20240419/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.271416 langfun-0.0.2.dev20240419/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.275416 langfun-0.0.2.dev20240419/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55359 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21592 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18331 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.275416 langfun-0.0.2.dev20240419/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/anthropic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.275416 langfun-0.0.2.dev20240419/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/llms/openai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.275416 langfun-0.0.2.dev20240419/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.279416 langfun-0.0.2.dev20240419/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.283416 langfun-0.0.2.dev20240419/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19301 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/function_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/function_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20980 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    19945 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22360 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17662 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.283416 langfun-0.0.2.dev20240419/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 08:03:47.283416 langfun-0.0.2.dev20240419/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-19 08:03:47.000000 langfun-0.0.2.dev20240419/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-19 08:03:47.000000 langfun-0.0.2.dev20240419/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 08:03:47.000000 langfun-0.0.2.dev20240419/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-19 08:03:47.000000 langfun-0.0.2.dev20240419/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-19 08:03:47.000000 langfun-0.0.2.dev20240419/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 08:03:47.283416 langfun-0.0.2.dev20240419/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-19 08:03:28.000000 langfun-0.0.2.dev20240419/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:03:38.819039 langfun-0.0.2.dev20240420/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-20 08:03:38.819039 langfun-0.0.2.dev20240420/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:03:38.803038 langfun-0.0.2.dev20240420/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:03:38.807039 langfun-0.0.2.dev20240420/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:03:38.807039 langfun-0.0.2.dev20240420/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:03:38.811039 langfun-0.0.2.dev20240420/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9674 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:03:38.811039 langfun-0.0.2.dev20240420/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55359 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21592 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11852 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8378 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18331 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13047 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:03:38.811039 langfun-0.0.2.dev20240420/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7865 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/llms/anthropic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:03:38.815039 langfun-0.0.2.dev20240420/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4184 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8624 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/llms/openai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:03:38.815039 langfun-0.0.2.dev20240420/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:03:38.815039 langfun-0.0.2.dev20240420/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:03:38.819039 langfun-0.0.2.dev20240420/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19301 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/function_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/function_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20980 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19945 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25057 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22360 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17662 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13572 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:03:38.819039 langfun-0.0.2.dev20240420/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 08:03:38.819039 langfun-0.0.2.dev20240420/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-20 08:03:38.000000 langfun-0.0.2.dev20240420/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-20 08:03:38.000000 langfun-0.0.2.dev20240420/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 08:03:38.000000 langfun-0.0.2.dev20240420/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-20 08:03:38.000000 langfun-0.0.2.dev20240420/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-20 08:03:38.000000 langfun-0.0.2.dev20240420/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 08:03:38.819039 langfun-0.0.2.dev20240420/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-20 08:03:12.000000 langfun-0.0.2.dev20240420/setup.py
```

### Comparing `langfun-0.0.2.dev20240419/LICENSE` & `langfun-0.0.2.dev20240420/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/PKG-INFO` & `langfun-0.0.2.dev20240420/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240419
+Version: 0.0.2.dev20240420
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240419/README.md` & `langfun-0.0.2.dev20240420/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/__init__.py` & `langfun-0.0.2.dev20240420/langfun/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/__init__.py` & `langfun-0.0.2.dev20240420/langfun/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240420/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240420/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240420/langfun/core/coding/python/correction.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240420/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240420/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240420/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240420/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240420/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240420/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240420/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240420/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240420/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240420/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240420/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/component.py` & `langfun-0.0.2.dev20240420/langfun/core/component.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/component_test.py` & `langfun-0.0.2.dev20240420/langfun/core/component_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240420/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240420/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/console.py` & `langfun-0.0.2.dev20240420/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/console_test.py` & `langfun-0.0.2.dev20240420/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240420/langfun/core/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240420/langfun/core/eval/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240420/langfun/core/eval/base_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240420/langfun/core/eval/matching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240420/langfun/core/eval/matching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240420/langfun/core/eval/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240420/langfun/core/eval/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240420/langfun/core/langfunc.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240420/langfun/core/langfunc_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/language_model.py` & `langfun-0.0.2.dev20240420/langfun/core/language_model.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240420/langfun/core/language_model_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240420/langfun/core/llms/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -31,16 +31,20 @@
 from langfun.core.llms.google_genai import Palm2
 from langfun.core.llms.google_genai import Palm2_IT
 
 # OpenAI models.
 from langfun.core.llms.openai import OpenAI
 
 from langfun.core.llms.openai import Gpt4Turbo
-from langfun.core.llms.openai import Gpt4Turbo_0125
-from langfun.core.llms.openai import Gpt4TurboVision
+from langfun.core.llms.openai import Gpt4Turbo_20240409
+from langfun.core.llms.openai import Gpt4TurboPreview
+from langfun.core.llms.openai import Gpt4TurboPreview_0125
+from langfun.core.llms.openai import Gpt4TurboPreview_1106
+from langfun.core.llms.openai import Gpt4VisionPreview
+from langfun.core.llms.openai import Gpt4VisionPreview_1106
 from langfun.core.llms.openai import Gpt4
 from langfun.core.llms.openai import Gpt4_0613
 from langfun.core.llms.openai import Gpt4_32K
 from langfun.core.llms.openai import Gpt4_32K_0613
 
 from langfun.core.llms.openai import Gpt35Turbo
 from langfun.core.llms.openai import Gpt35Turbo_0125
```

### Comparing `langfun-0.0.2.dev20240419/langfun/core/llms/anthropic.py` & `langfun-0.0.2.dev20240420/langfun/core/llms/anthropic.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,20 @@
 from langfun.core import modalities as lf_modalities
 import pyglove as pg
 import requests
 
 
 SUPPORTED_MODELS_AND_SETTINGS = {
     # See https://docs.anthropic.com/claude/docs/models-overview
-    'claude-3-opus-20240229': pg.Dict(max_tokens=4096, max_concurrency=1),
-    'claude-3-sonnet-20240229': pg.Dict(max_tokens=4096, max_concurrency=4),
+    'claude-3-opus-20240229': pg.Dict(max_tokens=4096, max_concurrency=16),
+    'claude-3-sonnet-20240229': pg.Dict(max_tokens=4096, max_concurrency=16),
     'claude-3-haiku-20240307': pg.Dict(max_tokens=4096, max_concurrency=16),
+    'claude-2.1': pg.Dict(max_tokens=4096, max_concurrency=16),
+    'claude-2.0': pg.Dict(max_tokens=4096, max_concurrency=16),
+    'claude-instant-1.2': pg.Dict(max_tokens=4096, max_concurrency=16),
 }
 
 
 class AnthropicError(Exception):  # pylint: disable=g-bad-exception-name
   """Base class for Anthropic errors."""
 
 
@@ -51,15 +54,15 @@
 @lf.use_init_args(['model'])
 class Anthropic(lf.LanguageModel):
   """Anthropic LLMs (Claude) through REST APIs.
 
   See https://docs.anthropic.com/claude/reference/messages_post
   """
 
-  model: Annotated[  # pytype: disable=invalid-annotation
+  model: pg.typing.Annotated[
       pg.typing.Enum(
           pg.MISSING_VALUE, list(SUPPORTED_MODELS_AND_SETTINGS.keys())
       ),
       'The name of the model to use.',
   ]
 
   multimodal: Annotated[bool, 'Whether this model has multimodal support.'] = (
@@ -206,14 +209,15 @@
         timeout=self.timeout,
     )
     return self._parse_response(response)
 
 
 class Claude3(Anthropic):
   """Base class for Claude 3 models. 200K input tokens and 4K output tokens."""
+  multimodal = True
 
 
 class Claude3Opus(Claude3):
   """Anthropic's most powerful model."""
 
   model = 'claude-3-opus-20240229'
 
@@ -224,7 +228,22 @@
   model = 'claude-3-sonnet-20240229'
 
 
 class Claude3Haiku(Claude3):
   """Anthropic's most compact model."""
 
   model = 'claude-3-haiku-20240307'
+
+
+class Claude2(Anthropic):
+  """Predecessor to Claude 3 with 100K context window.."""
+  model = 'claude-2.0'
+
+
+class Claude21(Anthropic):
+  """Updated Claude 2 model with improved accuracy and 200K context window."""
+  model = 'claude-2.1'
+
+
+class ClaudeInstant(Anthropic):
+  """Cheapest small and fast model, 100K context window."""
+  model = 'claude-instant-1.2'
```

### Comparing `langfun-0.0.2.dev20240419/langfun/core/llms/anthropic_test.py` & `langfun-0.0.2.dev20240420/langfun/core/llms/anthropic_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240420/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240420/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240420/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240420/langfun/core/llms/cache/in_memory_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/llms/fake.py` & `langfun-0.0.2.dev20240420/langfun/core/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240420/langfun/core/llms/fake_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240420/langfun/core/llms/google_genai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240420/langfun/core/llms/google_genai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240420/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240420/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240420/langfun/core/llms/openai.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,18 +27,21 @@
 
 
 SUPPORTED_MODELS_AND_SETTINGS = [
     # Model name, max concurrent requests.
     # The concurrent requests is estimated by TPM/RPM from
     # https://platform.openai.com/account/limits
     # GPT-4 Turbo models.
-    ('gpt-4-turbo-preview', 1),  # GPT-4 Turbo.
-    ('gpt-4-0125-preview', 1),  # GPT-4 Turbo
-    ('gpt-4-1106-preview', 1),  # GPT-4 Turbo
-    ('gpt-4-vision-preview', 1),  # GPT-4 Turbo with Vision.
+    ('gpt-4-turbo', 8),  # GPT-4 Turbo with Vision
+    ('gpt-4-turbo-2024-04-09', 8),  # GPT-4-Turbo with Vision, 04/09/2024
+    ('gpt-4-turbo-preview', 8),  # GPT-4 Turbo Preview
+    ('gpt-4-0125-preview', 8),  # GPT-4 Turbo Preview, 01/25/2024
+    ('gpt-4-1106-preview', 8),  # GPT-4 Turbo Preview, 11/06/2023
+    ('gpt-4-vision-preview', 8),  # GPT-4 Turbo Vision Preview.
+    ('gpt-4-1106-vision-preview', 8),  # GPT-4 Turbo Vision Preview, 11/06/2023
     # GPT-4 models.
     ('gpt-4', 4),
     ('gpt-4-0613', 4),
     ('gpt-4-0314', 4),
     ('gpt-4-32k', 4),
     ('gpt-4-32k-0613', 4),
     ('gpt-4-32k-0314', 4),
@@ -280,34 +283,51 @@
 
 class Gpt4(OpenAI):
   """GPT-4."""
   model = 'gpt-4'
 
 
 class Gpt4Turbo(Gpt4):
-  """GPT-4 Turbo with 128K context window size. Knowledge up to 4-2023."""
-  model = 'gpt-4-turbo-preview'
+  """GPT-4 Turbo with 128K context window. Knowledge up to Dec. 2023."""
+  model = 'gpt-4-turbo'
+  multimodal = True
 
 
-class Gpt4TurboVision(Gpt4Turbo):
-  """GPT-4 Turbo with vision."""
-  model = 'gpt-4-vision-preview'
+class Gpt4Turbo_20240409(Gpt4Turbo):  # pylint:disable=invalid-name
+  """GPT-4 Turbo with 128K context window. Knowledge up to Dec. 2023."""
+  model = 'gpt-4-turbo-2024-04-09'
   multimodal = True
 
 
-class Gpt4Turbo_0125(Gpt4Turbo):   # pylint:disable=invalid-name
-  """GPT-4 Turbo with 128K context window size. Knowledge up to 4-2023."""
+class Gpt4TurboPreview(Gpt4):
+  """GPT-4 Turbo Preview with 128k context window. Knowledge up to Dec. 2023."""
+  model = 'gpt-4-turbo-preview'
+
+
+class Gpt4TurboPreview_0125(Gpt4TurboPreview):  # pylint: disable=invalid-name
+  """GPT-4 Turbo Preview with 128k context window. Knowledge up to Dec. 2023."""
   model = 'gpt-4-0125-preview'
 
 
-class Gpt4Turbo_1106(Gpt4Turbo):   # pylint:disable=invalid-name
-  """GPT-4 Turbo @20231106. 128K context window. Knowledge up to 4-2023."""
+class Gpt4TurboPreview_1106(Gpt4TurboPreview):  # pylint: disable=invalid-name
+  """GPT-4 Turbo Preview with 128k context window. Knowledge up to Apr. 2023."""
   model = 'gpt-4-1106-preview'
 
 
+class Gpt4VisionPreview(Gpt4):
+  """GPT-4 Turbo vision preview. 128k context window. Knowledge to Apr. 2023."""
+  model = 'gpt-4-vision-preview'
+  multimodal = True
+
+
+class Gpt4VisionPreview_1106(Gpt4):  # pylint: disable=invalid-name
+  """GPT-4 Turbo vision preview. 128k context window. Knowledge to Apr. 2023."""
+  model = 'gpt-4-1106-vision-preview'
+
+
 class Gpt4_0613(Gpt4):    # pylint:disable=invalid-name
   """GPT-4 @20230613. 8K context window. Knowledge up to 9-2021."""
   model = 'gpt-4-0613'
 
 
 class Gpt4_32K(Gpt4):       # pylint:disable=invalid-name
   """Latest GPT-4 with 32K context window."""
```

### Comparing `langfun-0.0.2.dev20240419/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240420/langfun/core/llms/openai_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,25 +153,27 @@
           lm('hello', sampling_options=lf.LMSamplingOptions(n=2)),
           'Sample 0 for message.',
       )
 
   def test_call_chat_completion_vision(self):
     with mock.patch('openai.ChatCompletion.create') as mock_chat_completion:
       mock_chat_completion.side_effect = mock_chat_completion_query_vision
-      lm = openai.Gpt4TurboVision(api_key='test_key')
-      self.assertEqual(
-          lm(
-              lf.UserMessage(
-                  'hello {{image}}',
-                  image=lf_modalities.Image.from_uri('https://fake/image')
-              ),
-              sampling_options=lf.LMSamplingOptions(n=2)
-          ),
-          'Sample 0 for message: https://fake/image',
-      )
+      lm_1 = openai.Gpt4Turbo(api_key='test_key')
+      lm_2 = openai.Gpt4VisionPreview(api_key='test_key')
+      for lm in (lm_1, lm_2):
+        self.assertEqual(
+            lm(
+                lf.UserMessage(
+                    'hello {{image}}',
+                    image=lf_modalities.Image.from_uri('https://fake/image')
+                ),
+                sampling_options=lf.LMSamplingOptions(n=2)
+            ),
+            'Sample 0 for message: https://fake/image',
+        )
 
   def test_sample_completion(self):
     with mock.patch('openai.Completion.create') as mock_completion:
       mock_completion.side_effect = mock_completion_query
       lm = openai.OpenAI(api_key='test_key', model='text-davinci-003')
       results = lm.sample(
           ['hello', 'bye'], sampling_options=lf.LMSamplingOptions(n=3)
```

### Comparing `langfun-0.0.2.dev20240419/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240420/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240420/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240420/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/memory.py` & `langfun-0.0.2.dev20240420/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/message.py` & `langfun-0.0.2.dev20240420/langfun/core/message.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/message_test.py` & `langfun-0.0.2.dev20240420/langfun/core/message_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240420/langfun/core/modalities/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240420/langfun/core/modalities/image.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240420/langfun/core/modalities/image_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240420/langfun/core/modalities/mime.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240420/langfun/core/modalities/mime_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/modalities/video.py` & `langfun-0.0.2.dev20240420/langfun/core/modalities/video.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240420/langfun/core/modalities/video_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/modality.py` & `langfun-0.0.2.dev20240420/langfun/core/modality.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240420/langfun/core/modality_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240420/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240420/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/sampling.py` & `langfun-0.0.2.dev20240420/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240420/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/function_generation.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/function_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/function_generation_test.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/function_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/mapping.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/mapping_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/prompting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/prompting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/schema.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/schema_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/schema_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240420/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/subscription.py` & `langfun-0.0.2.dev20240420/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240420/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/template.py` & `langfun-0.0.2.dev20240420/langfun/core/template.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/template_test.py` & `langfun-0.0.2.dev20240420/langfun/core/template_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240420/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240420/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240420/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240420/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240420/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240420/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240420/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240420/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240420/langfun/core/templates/selfplay_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240420/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240420/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240420/langfun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240419
+Version: 0.0.2.dev20240420
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240419/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240420/langfun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240419/setup.py` & `langfun-0.0.2.dev20240420/setup.py`

 * *Files identical despite different names*

