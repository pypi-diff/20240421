# Comparing `tmp/zenguard-0.1.7.tar.gz` & `tmp/zenguard-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zenguard-0.1.7.tar", max compression
+gzip compressed data, was "zenguard-0.1.8.tar", max compression
```

## Comparing `zenguard-0.1.7.tar` & `zenguard-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     2914 2024-03-25 18:23:08.774096 zenguard-0.1.7/README.md
--rw-r--r--   0        0        0      444 2024-03-25 18:24:07.159609 zenguard-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      103 2024-03-25 18:09:28.651591 zenguard-0.1.7/zenguard/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 16:56:11.876514 zenguard-0.1.7/zenguard/pentest/__init__.py
--rw-r--r--   0        0        0      107 2024-03-25 16:56:11.876674 zenguard-0.1.7/zenguard/pentest/prompt_injections/__init__.py
--rw-r--r--   0        0        0      614 2024-03-25 16:56:11.876786 zenguard-0.1.7/zenguard/pentest/prompt_injections/_utils.py
--rw-r--r--   0        0        0      959 2024-03-25 16:56:11.876906 zenguard-0.1.7/zenguard/pentest/prompt_injections/config.py
--rw-r--r--   0        0        0    27037 2024-03-25 16:56:11.877082 zenguard-0.1.7/zenguard/pentest/prompt_injections/prompt_data.py
--rw-r--r--   0        0        0    10014 2024-03-25 16:56:11.877333 zenguard-0.1.7/zenguard/pentest/prompt_injections/prompting.py
--rw-r--r--   0        0        0     1965 2024-03-25 18:05:24.665817 zenguard-0.1.7/zenguard/pentest/prompt_injections/run.py
--rw-r--r--   0        0        0     2369 2024-03-25 16:56:11.877590 zenguard-0.1.7/zenguard/pentest/prompt_injections/scoring.py
--rw-r--r--   0        0        0     1342 2024-03-25 16:56:11.877728 zenguard-0.1.7/zenguard/pentest/prompt_injections/visualization.py
--rw-r--r--   0        0        0     3361 2024-03-25 18:12:20.327973 zenguard-0.1.7/zenguard/zenguard.py
--rw-r--r--   0        0        0     3675 1970-01-01 00:00:00.000000 zenguard-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-03-27 23:17:17.162445 zenguard-0.1.8/LICENSE
+-rw-r--r--   0        0        0     4717 2024-04-21 18:48:37.634036 zenguard-0.1.8/README.md
+-rw-r--r--   0        0        0      444 2024-04-21 18:48:37.634235 zenguard-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      103 2024-03-25 18:32:49.933079 zenguard-0.1.8/zenguard/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 16:56:11.876514 zenguard-0.1.8/zenguard/pentest/__init__.py
+-rw-r--r--   0        0        0      107 2024-03-25 16:56:11.876674 zenguard-0.1.8/zenguard/pentest/prompt_injections/__init__.py
+-rw-r--r--   0        0        0      614 2024-03-25 16:56:11.876786 zenguard-0.1.8/zenguard/pentest/prompt_injections/_utils.py
+-rw-r--r--   0        0        0      959 2024-03-25 16:56:11.876906 zenguard-0.1.8/zenguard/pentest/prompt_injections/config.py
+-rw-r--r--   0        0        0    27037 2024-03-25 16:56:11.877082 zenguard-0.1.8/zenguard/pentest/prompt_injections/prompt_data.py
+-rw-r--r--   0        0        0    10014 2024-03-25 16:56:11.877333 zenguard-0.1.8/zenguard/pentest/prompt_injections/prompting.py
+-rw-r--r--   0        0        0     1965 2024-03-25 18:32:49.933251 zenguard-0.1.8/zenguard/pentest/prompt_injections/run.py
+-rw-r--r--   0        0        0     2369 2024-03-25 16:56:11.877590 zenguard-0.1.8/zenguard/pentest/prompt_injections/scoring.py
+-rw-r--r--   0        0        0     1342 2024-03-25 16:56:11.877728 zenguard-0.1.8/zenguard/pentest/prompt_injections/visualization.py
+-rw-r--r--   0        0        0     3524 2024-04-21 18:29:18.545646 zenguard-0.1.8/zenguard/zenguard.py
+-rw-r--r--   0        0        0     5478 1970-01-01 00:00:00.000000 zenguard-0.1.8/PKG-INFO
```

### Comparing `zenguard-0.1.7/zenguard/pentest/prompt_injections/_utils.py` & `zenguard-0.1.8/zenguard/pentest/prompt_injections/_utils.py`

 * *Files identical despite different names*

### Comparing `zenguard-0.1.7/zenguard/pentest/prompt_injections/config.py` & `zenguard-0.1.8/zenguard/pentest/prompt_injections/config.py`

 * *Files identical despite different names*

### Comparing `zenguard-0.1.7/zenguard/pentest/prompt_injections/prompt_data.py` & `zenguard-0.1.8/zenguard/pentest/prompt_injections/prompt_data.py`

 * *Files identical despite different names*

### Comparing `zenguard-0.1.7/zenguard/pentest/prompt_injections/prompting.py` & `zenguard-0.1.8/zenguard/pentest/prompt_injections/prompting.py`

 * *Files identical despite different names*

### Comparing `zenguard-0.1.7/zenguard/pentest/prompt_injections/run.py` & `zenguard-0.1.8/zenguard/pentest/prompt_injections/run.py`

 * *Files identical despite different names*

### Comparing `zenguard-0.1.7/zenguard/pentest/prompt_injections/scoring.py` & `zenguard-0.1.8/zenguard/pentest/prompt_injections/scoring.py`

 * *Files identical despite different names*

### Comparing `zenguard-0.1.7/zenguard/pentest/prompt_injections/visualization.py` & `zenguard-0.1.8/zenguard/pentest/prompt_injections/visualization.py`

 * *Files identical despite different names*

### Comparing `zenguard-0.1.7/zenguard/zenguard.py` & `zenguard-0.1.8/zenguard/zenguard.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,15 +54,18 @@
     It is used to connect to ZenGuard AI API and its services.
     """
 
     def __init__(
         self,
         config: ZenGuardConfig,
     ):
-        self._api_key = config.credentials.api_key
+        api_key = config.credentials.api_key
+        if type(api_key) != str or api_key == '':
+            raise ValueError("The API key must be a string type and not empty.")
+        self._api_key = api_key
         self._backend = "https://api.zenguard.ai/"
 
         self._llm_client = None
         if config.llm == SupportedLLMs.CHATGPT:
             self._llm_client = OpenAI(
                 api_key=config.credentials.llm_api_key,
             )
@@ -96,19 +99,19 @@
             attack["result"] = attack["settings"]["attack_rogue_string"]
 
     def pentest(self, endpoint: Endpoint, detector: Detector = None):
         base_prompts = config.default_attack_config
         attack_prompts = prompting.build_prompts(base_prompts)
 
         if endpoint == Endpoint.ZENGUARD:
-            print("Running attack on ZenGuard endpoint")
+            print("\nRunning attack on ZenGuard endpoint:")
             assert (
                 detector == Detector.PROMPT_INJECTION
             ), "Only prompt injection pentesting is currently supported"
             self._attack_zenguard(Detector.PROMPT_INJECTION, attack_prompts)
         elif endpoint == Endpoint.OPENAI:
-            print("Running attack on OpenAI endpoint")
+            print("\nRunning attack on OpenAI endpoint:")
             run.run_prompts_api(attack_prompts, self._llm_client)
 
         scoring.score_attacks(attack_prompts)
         df = visualization.build_dataframe(attack_prompts)
         print(scoring.get_metrics(df, "Attack Instruction"))
```

