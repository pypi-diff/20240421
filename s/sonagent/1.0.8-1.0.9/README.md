# Comparing `tmp/sonagent-1.0.8.tar.gz` & `tmp/sonagent-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonagent-1.0.8.tar", last modified: Sun Mar 17 16:41:11 2024, max compression
+gzip compressed data, was "sonagent-1.0.9.tar", last modified: Sun Mar 17 17:07:11 2024, max compression
```

## Comparing `sonagent-1.0.8.tar` & `sonagent-1.0.9.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.914302 sonagent-1.0.8/
--rw-r--r--   0 admin      (501) staff       (20)     1074 2023-12-02 11:08:44.000000 sonagent-1.0.8/LICENSE
--rw-r--r--   0 admin      (501) staff       (20)     3259 2024-03-17 16:41:11.913935 sonagent-1.0.8/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)       38 2024-03-17 16:41:11.914370 sonagent-1.0.8/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     3828 2024-03-17 12:51:40.000000 sonagent-1.0.8/setup.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.885710 sonagent-1.0.8/sonagent/
--rw-r--r--   0 admin      (501) staff       (20)       33 2023-12-02 11:35:06.000000 sonagent-1.0.8/sonagent/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      202 2024-01-07 09:00:33.000000 sonagent-1.0.8/sonagent/__main__.py
--rw-r--r--   0 admin      (501) staff       (20)    17505 2024-03-08 18:20:45.000000 sonagent-1.0.8/sonagent/agent.py
--rw-r--r--   0 admin      (501) staff       (20)      556 2023-12-09 08:53:31.000000 sonagent-1.0.8/sonagent/chat.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.888846 sonagent-1.0.8/sonagent/coding/
--rw-r--r--   0 admin      (501) staff       (20)       49 2024-02-27 13:24:06.000000 sonagent-1.0.8/sonagent/coding/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     7243 2024-03-17 16:39:51.000000 sonagent-1.0.8/sonagent/coding/gencode.py
--rw-r--r--   0 admin      (501) staff       (20)     3276 2024-03-08 08:59:13.000000 sonagent-1.0.8/sonagent/coding/sonautogen.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.890382 sonagent-1.0.8/sonagent/commands/
--rw-r--r--   0 admin      (501) staff       (20)      131 2024-03-17 13:40:49.000000 sonagent-1.0.8/sonagent/commands/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     4091 2024-03-17 14:07:25.000000 sonagent-1.0.8/sonagent/commands/arguments.py
--rw-r--r--   0 admin      (501) staff       (20)     2735 2024-01-28 04:55:09.000000 sonagent-1.0.8/sonagent/commands/cli_options.py
--rw-r--r--   0 admin      (501) staff       (20)     3965 2024-03-17 14:26:58.000000 sonagent-1.0.8/sonagent/commands/run_commands.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.891407 sonagent-1.0.8/sonagent/configuration/
--rw-r--r--   0 admin      (501) staff       (20)      136 2024-01-10 17:54:03.000000 sonagent-1.0.8/sonagent/configuration/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      168 2024-01-09 14:49:12.000000 sonagent-1.0.8/sonagent/configuration/detect_environment.py
--rw-r--r--   0 admin      (501) staff       (20)     1822 2024-03-02 06:43:15.000000 sonagent-1.0.8/sonagent/configuration/load_config.py
--rw-r--r--   0 admin      (501) staff       (20)      177 2024-03-02 05:47:11.000000 sonagent-1.0.8/sonagent/constants.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.891858 sonagent-1.0.8/sonagent/core_prompt/
--rw-r--r--   0 admin      (501) staff       (20)        0 2024-01-20 14:12:41.000000 sonagent-1.0.8/sonagent/core_prompt/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      572 2024-01-21 15:31:11.000000 sonagent-1.0.8/sonagent/core_prompt/me.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.893027 sonagent-1.0.8/sonagent/enums/
--rw-r--r--   0 admin      (501) staff       (20)       57 2024-01-07 03:44:36.000000 sonagent-1.0.8/sonagent/enums/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      202 2024-01-07 02:48:46.000000 sonagent-1.0.8/sonagent/enums/enums.py
--rw-r--r--   0 admin      (501) staff       (20)      283 2024-01-07 10:54:29.000000 sonagent-1.0.8/sonagent/enums/rpcmessagetype.py
--rw-r--r--   0 admin      (501) staff       (20)      623 2024-01-07 03:26:35.000000 sonagent-1.0.8/sonagent/exceptions.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.893890 sonagent-1.0.8/sonagent/llm/
--rw-r--r--   0 admin      (501) staff       (20)        0 2024-03-17 13:21:03.000000 sonagent-1.0.8/sonagent/llm/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     4328 2024-03-08 10:07:57.000000 sonagent-1.0.8/sonagent/llm/oai_llm.py
--rw-r--r--   0 admin      (501) staff       (20)    14781 2024-03-08 10:07:57.000000 sonagent-1.0.8/sonagent/llm/prompt.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.895376 sonagent-1.0.8/sonagent/loggers/
--rw-r--r--   0 admin      (501) staff       (20)     4225 2024-01-20 14:36:35.000000 sonagent-1.0.8/sonagent/loggers/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      460 2024-01-07 09:12:54.000000 sonagent-1.0.8/sonagent/loggers/buffering_handler.py
--rw-r--r--   0 admin      (501) staff       (20)     1594 2024-01-07 10:10:45.000000 sonagent-1.0.8/sonagent/loggers/set_log_levels.py
--rw-r--r--   0 admin      (501) staff       (20)      713 2024-01-07 09:13:13.000000 sonagent-1.0.8/sonagent/loggers/std_err_stream_handler.py
--rw-r--r--   0 admin      (501) staff       (20)     1961 2024-01-20 14:42:32.000000 sonagent-1.0.8/sonagent/main.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.896316 sonagent-1.0.8/sonagent/memory/
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-12-02 11:37:31.000000 sonagent-1.0.8/sonagent/memory/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-12-02 09:50:22.000000 sonagent-1.0.8/sonagent/memory/long_memory.py
--rw-r--r--   0 admin      (501) staff       (20)     3205 2024-03-08 10:07:57.000000 sonagent-1.0.8/sonagent/memory/memory.py
--rw-r--r--   0 admin      (501) staff       (20)     1069 2024-03-02 05:47:11.000000 sonagent-1.0.8/sonagent/memory/short_memory.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.897090 sonagent-1.0.8/sonagent/mixins/
--rw-r--r--   0 admin      (501) staff       (20)       69 2024-01-07 10:19:53.000000 sonagent-1.0.8/sonagent/mixins/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     1268 2024-03-17 12:59:47.000000 sonagent-1.0.8/sonagent/mixins/logging_mixin.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.899072 sonagent-1.0.8/sonagent/persistence/
--rw-r--r--   0 admin      (501) staff       (20)      155 2024-01-21 16:41:18.000000 sonagent-1.0.8/sonagent/persistence/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      154 2023-12-04 13:08:47.000000 sonagent-1.0.8/sonagent/persistence/base.py
--rw-r--r--   0 admin      (501) staff       (20)     1626 2024-02-27 14:24:32.000000 sonagent-1.0.8/sonagent/persistence/belief_models.py
--rw-r--r--   0 admin      (501) staff       (20)      526 2023-12-06 13:34:57.000000 sonagent-1.0.8/sonagent/persistence/migrations.py
--rw-r--r--   0 admin      (501) staff       (20)     1893 2023-12-06 13:34:57.000000 sonagent-1.0.8/sonagent/persistence/models.py
--rw-r--r--   0 admin      (501) staff       (20)     1575 2024-01-21 16:43:43.000000 sonagent-1.0.8/sonagent/persistence/planning_models.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.899925 sonagent-1.0.8/sonagent/planning/
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-12-02 10:37:38.000000 sonagent-1.0.8/sonagent/planning/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     3633 2024-01-21 15:10:45.000000 sonagent-1.0.8/sonagent/planning/planner.py
--rw-r--r--   0 admin      (501) staff       (20)     7041 2024-03-05 19:33:49.000000 sonagent-1.0.8/sonagent/planning/prompt.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.901963 sonagent-1.0.8/sonagent/rpc/
--rw-r--r--   0 admin      (501) staff       (20)       97 2024-01-07 03:39:49.000000 sonagent-1.0.8/sonagent/rpc/__init__.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.903746 sonagent-1.0.8/sonagent/rpc/api_server/
--rw-r--r--   0 admin      (501) staff       (20)       46 2024-01-09 14:43:01.000000 sonagent-1.0.8/sonagent/rpc/api_server/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      326 2024-01-10 14:13:17.000000 sonagent-1.0.8/sonagent/rpc/api_server/api_models.py
--rw-r--r--   0 admin      (501) staff       (20)      834 2024-01-09 14:44:22.000000 sonagent-1.0.8/sonagent/rpc/api_server/api_v1.py
--rw-r--r--   0 admin      (501) staff       (20)     2099 2024-01-09 14:31:19.000000 sonagent-1.0.8/sonagent/rpc/api_server/uvicorn_threaded.py
--rw-r--r--   0 admin      (501) staff       (20)     6512 2024-01-10 14:18:41.000000 sonagent-1.0.8/sonagent/rpc/api_server/webserver.py
--rw-r--r--   0 admin      (501) staff       (20)     4331 2024-03-08 17:55:33.000000 sonagent-1.0.8/sonagent/rpc/rpc.py
--rw-r--r--   0 admin      (501) staff       (20)     1910 2024-01-10 18:03:20.000000 sonagent-1.0.8/sonagent/rpc/rpc_manager.py
--rw-r--r--   0 admin      (501) staff       (20)      483 2024-01-07 03:46:27.000000 sonagent-1.0.8/sonagent/rpc/rpc_types.py
--rw-r--r--   0 admin      (501) staff       (20)     1598 2024-02-26 13:28:23.000000 sonagent-1.0.8/sonagent/rpc/schedule_worker.py
--rw-r--r--   0 admin      (501) staff       (20)    20178 2024-03-08 18:16:05.000000 sonagent-1.0.8/sonagent/rpc/telegram.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.905056 sonagent-1.0.8/sonagent/skills/
--rw-r--r--   0 admin      (501) staff       (20)        0 2024-03-17 13:02:49.000000 sonagent-1.0.8/sonagent/skills/__init__.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.908434 sonagent-1.0.8/sonagent/skills/core_skills/
--rw-r--r--   0 admin      (501) staff       (20)      543 2024-01-20 06:22:05.000000 sonagent-1.0.8/sonagent/skills/core_skills/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     2538 2024-01-10 15:17:51.000000 sonagent-1.0.8/sonagent/skills/core_skills/conversation_summary_skill.py
--rw-r--r--   0 admin      (501) staff       (20)     2005 2024-01-10 15:09:14.000000 sonagent-1.0.8/sonagent/skills/core_skills/file_io_skill.py
--rw-r--r--   0 admin      (501) staff       (20)     3800 2024-01-10 15:10:26.000000 sonagent-1.0.8/sonagent/skills/core_skills/http_skill.py
--rw-r--r--   0 admin      (501) staff       (20)     3314 2024-01-20 06:21:10.000000 sonagent-1.0.8/sonagent/skills/core_skills/math_skill.py
--rw-r--r--   0 admin      (501) staff       (20)     2526 2024-01-10 15:11:43.000000 sonagent-1.0.8/sonagent/skills/core_skills/text_skill.py
--rw-r--r--   0 admin      (501) staff       (20)     7959 2024-01-10 15:12:08.000000 sonagent-1.0.8/sonagent/skills/core_skills/time_skill.py
--rw-r--r--   0 admin      (501) staff       (20)      751 2024-01-10 15:12:43.000000 sonagent-1.0.8/sonagent/skills/core_skills/wait_skill.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.909381 sonagent-1.0.8/sonagent/skills/learning_skills/
--rw-r--r--   0 admin      (501) staff       (20)        0 2024-01-10 15:33:48.000000 sonagent-1.0.8/sonagent/skills/learning_skills/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)       28 2023-12-15 10:45:54.000000 sonagent-1.0.8/sonagent/skills/learning_skills/run.py
--rw-r--r--   0 admin      (501) staff       (20)    10363 2024-01-28 04:43:00.000000 sonagent-1.0.8/sonagent/skills/loading.py
--rw-r--r--   0 admin      (501) staff       (20)      256 2024-01-28 10:05:30.000000 sonagent-1.0.8/sonagent/skills/skills.py
--rw-r--r--   0 admin      (501) staff       (20)     4269 2024-03-17 16:40:23.000000 sonagent-1.0.8/sonagent/skills/skills_manager.py
--rw-r--r--   0 admin      (501) staff       (20)     4999 2024-03-08 18:18:05.000000 sonagent-1.0.8/sonagent/sonbot.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.911371 sonagent-1.0.8/sonagent/tools/
--rw-r--r--   0 admin      (501) staff       (20)      141 2024-03-08 08:59:13.000000 sonagent-1.0.8/sonagent/tools/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      624 2024-03-08 08:59:13.000000 sonagent-1.0.8/sonagent/tools/code_manager.py
--rw-r--r--   0 admin      (501) staff       (20)     2989 2024-03-08 08:59:13.000000 sonagent-1.0.8/sonagent/tools/git_manager.py
--rw-r--r--   0 admin      (501) staff       (20)     1224 2024-03-08 08:59:13.000000 sonagent-1.0.8/sonagent/tools/local_code_manager.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.912578 sonagent-1.0.8/sonagent/utils/
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-12-10 14:37:57.000000 sonagent-1.0.8/sonagent/utils/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     2616 2023-12-20 02:00:04.000000 sonagent-1.0.8/sonagent/utils/datetime_helpers.py
--rw-r--r--   0 admin      (501) staff       (20)      458 2024-01-07 04:01:24.000000 sonagent-1.0.8/sonagent/utils/gc_setup.py
--rw-r--r--   0 admin      (501) staff       (20)      397 2024-03-02 07:26:18.000000 sonagent-1.0.8/sonagent/utils/utils.py
--rw-r--r--   0 admin      (501) staff       (20)       22 2024-03-17 16:41:06.000000 sonagent-1.0.8/sonagent/version.py
--rw-r--r--   0 admin      (501) staff       (20)     6427 2024-02-26 13:28:23.000000 sonagent-1.0.8/sonagent/worker.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.913410 sonagent-1.0.8/sonagent.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     3259 2024-03-17 16:41:11.000000 sonagent-1.0.8/sonagent.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     2753 2024-03-17 16:41:11.000000 sonagent-1.0.8/sonagent.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2024-03-17 16:41:11.000000 sonagent-1.0.8/sonagent.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       48 2024-03-17 16:41:11.000000 sonagent-1.0.8/sonagent.egg-info/entry_points.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2024-03-17 11:58:08.000000 sonagent-1.0.8/sonagent.egg-info/not-zip-safe
--rw-r--r--   0 admin      (501) staff       (20)      322 2024-03-17 16:41:11.000000 sonagent-1.0.8/sonagent.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       15 2024-03-17 16:41:11.000000 sonagent-1.0.8/sonagent.egg-info/top_level.txt
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 16:41:11.913142 sonagent-1.0.8/tests/
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-12-02 11:24:39.000000 sonagent-1.0.8/tests/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.616714 sonagent-1.0.9/
+-rw-r--r--   0 admin      (501) staff       (20)     1074 2023-12-02 11:08:44.000000 sonagent-1.0.9/LICENSE
+-rw-r--r--   0 admin      (501) staff       (20)     3259 2024-03-17 17:07:11.616346 sonagent-1.0.9/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)       38 2024-03-17 17:07:11.616799 sonagent-1.0.9/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     3828 2024-03-17 12:51:40.000000 sonagent-1.0.9/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.582966 sonagent-1.0.9/sonagent/
+-rw-r--r--   0 admin      (501) staff       (20)       33 2023-12-02 11:35:06.000000 sonagent-1.0.9/sonagent/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      202 2024-01-07 09:00:33.000000 sonagent-1.0.9/sonagent/__main__.py
+-rw-r--r--   0 admin      (501) staff       (20)    17505 2024-03-08 18:20:45.000000 sonagent-1.0.9/sonagent/agent.py
+-rw-r--r--   0 admin      (501) staff       (20)      556 2023-12-09 08:53:31.000000 sonagent-1.0.9/sonagent/chat.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.585928 sonagent-1.0.9/sonagent/coding/
+-rw-r--r--   0 admin      (501) staff       (20)       49 2024-02-27 13:24:06.000000 sonagent-1.0.9/sonagent/coding/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     7243 2024-03-17 16:39:51.000000 sonagent-1.0.9/sonagent/coding/gencode.py
+-rw-r--r--   0 admin      (501) staff       (20)     3276 2024-03-08 08:59:13.000000 sonagent-1.0.9/sonagent/coding/sonautogen.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.587982 sonagent-1.0.9/sonagent/commands/
+-rw-r--r--   0 admin      (501) staff       (20)      131 2024-03-17 13:40:49.000000 sonagent-1.0.9/sonagent/commands/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     4091 2024-03-17 14:07:25.000000 sonagent-1.0.9/sonagent/commands/arguments.py
+-rw-r--r--   0 admin      (501) staff       (20)     2735 2024-01-28 04:55:09.000000 sonagent-1.0.9/sonagent/commands/cli_options.py
+-rw-r--r--   0 admin      (501) staff       (20)     3965 2024-03-17 17:03:34.000000 sonagent-1.0.9/sonagent/commands/run_commands.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.589108 sonagent-1.0.9/sonagent/configuration/
+-rw-r--r--   0 admin      (501) staff       (20)      136 2024-01-10 17:54:03.000000 sonagent-1.0.9/sonagent/configuration/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      168 2024-01-09 14:49:12.000000 sonagent-1.0.9/sonagent/configuration/detect_environment.py
+-rw-r--r--   0 admin      (501) staff       (20)     1822 2024-03-02 06:43:15.000000 sonagent-1.0.9/sonagent/configuration/load_config.py
+-rw-r--r--   0 admin      (501) staff       (20)      177 2024-03-02 05:47:11.000000 sonagent-1.0.9/sonagent/constants.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.589590 sonagent-1.0.9/sonagent/core_prompt/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2024-01-20 14:12:41.000000 sonagent-1.0.9/sonagent/core_prompt/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      572 2024-01-21 15:31:11.000000 sonagent-1.0.9/sonagent/core_prompt/me.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.590680 sonagent-1.0.9/sonagent/enums/
+-rw-r--r--   0 admin      (501) staff       (20)       57 2024-01-07 03:44:36.000000 sonagent-1.0.9/sonagent/enums/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      202 2024-01-07 02:48:46.000000 sonagent-1.0.9/sonagent/enums/enums.py
+-rw-r--r--   0 admin      (501) staff       (20)      283 2024-01-07 10:54:29.000000 sonagent-1.0.9/sonagent/enums/rpcmessagetype.py
+-rw-r--r--   0 admin      (501) staff       (20)      623 2024-01-07 03:26:35.000000 sonagent-1.0.9/sonagent/exceptions.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.591536 sonagent-1.0.9/sonagent/llm/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2024-03-17 13:21:03.000000 sonagent-1.0.9/sonagent/llm/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     4328 2024-03-08 10:07:57.000000 sonagent-1.0.9/sonagent/llm/oai_llm.py
+-rw-r--r--   0 admin      (501) staff       (20)    14781 2024-03-08 10:07:57.000000 sonagent-1.0.9/sonagent/llm/prompt.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.593670 sonagent-1.0.9/sonagent/loggers/
+-rw-r--r--   0 admin      (501) staff       (20)     4225 2024-01-20 14:36:35.000000 sonagent-1.0.9/sonagent/loggers/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      460 2024-01-07 09:12:54.000000 sonagent-1.0.9/sonagent/loggers/buffering_handler.py
+-rw-r--r--   0 admin      (501) staff       (20)     1594 2024-01-07 10:10:45.000000 sonagent-1.0.9/sonagent/loggers/set_log_levels.py
+-rw-r--r--   0 admin      (501) staff       (20)      713 2024-01-07 09:13:13.000000 sonagent-1.0.9/sonagent/loggers/std_err_stream_handler.py
+-rw-r--r--   0 admin      (501) staff       (20)     1961 2024-01-20 14:42:32.000000 sonagent-1.0.9/sonagent/main.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.595039 sonagent-1.0.9/sonagent/memory/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-12-02 11:37:31.000000 sonagent-1.0.9/sonagent/memory/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-12-02 09:50:22.000000 sonagent-1.0.9/sonagent/memory/long_memory.py
+-rw-r--r--   0 admin      (501) staff       (20)     3205 2024-03-08 10:07:57.000000 sonagent-1.0.9/sonagent/memory/memory.py
+-rw-r--r--   0 admin      (501) staff       (20)     1069 2024-03-02 05:47:11.000000 sonagent-1.0.9/sonagent/memory/short_memory.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.595921 sonagent-1.0.9/sonagent/mixins/
+-rw-r--r--   0 admin      (501) staff       (20)       69 2024-01-07 10:19:53.000000 sonagent-1.0.9/sonagent/mixins/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1268 2024-03-17 12:59:47.000000 sonagent-1.0.9/sonagent/mixins/logging_mixin.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.599060 sonagent-1.0.9/sonagent/persistence/
+-rw-r--r--   0 admin      (501) staff       (20)      155 2024-01-21 16:41:18.000000 sonagent-1.0.9/sonagent/persistence/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      154 2023-12-04 13:08:47.000000 sonagent-1.0.9/sonagent/persistence/base.py
+-rw-r--r--   0 admin      (501) staff       (20)     1626 2024-02-27 14:24:32.000000 sonagent-1.0.9/sonagent/persistence/belief_models.py
+-rw-r--r--   0 admin      (501) staff       (20)      526 2023-12-06 13:34:57.000000 sonagent-1.0.9/sonagent/persistence/migrations.py
+-rw-r--r--   0 admin      (501) staff       (20)     1893 2023-12-06 13:34:57.000000 sonagent-1.0.9/sonagent/persistence/models.py
+-rw-r--r--   0 admin      (501) staff       (20)     1575 2024-01-21 16:43:43.000000 sonagent-1.0.9/sonagent/persistence/planning_models.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.600026 sonagent-1.0.9/sonagent/planning/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-12-02 10:37:38.000000 sonagent-1.0.9/sonagent/planning/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     3633 2024-01-21 15:10:45.000000 sonagent-1.0.9/sonagent/planning/planner.py
+-rw-r--r--   0 admin      (501) staff       (20)     7041 2024-03-05 19:33:49.000000 sonagent-1.0.9/sonagent/planning/prompt.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.602577 sonagent-1.0.9/sonagent/rpc/
+-rw-r--r--   0 admin      (501) staff       (20)       97 2024-01-07 03:39:49.000000 sonagent-1.0.9/sonagent/rpc/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.606132 sonagent-1.0.9/sonagent/rpc/api_server/
+-rw-r--r--   0 admin      (501) staff       (20)       46 2024-01-09 14:43:01.000000 sonagent-1.0.9/sonagent/rpc/api_server/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      326 2024-01-10 14:13:17.000000 sonagent-1.0.9/sonagent/rpc/api_server/api_models.py
+-rw-r--r--   0 admin      (501) staff       (20)      834 2024-01-09 14:44:22.000000 sonagent-1.0.9/sonagent/rpc/api_server/api_v1.py
+-rw-r--r--   0 admin      (501) staff       (20)     2099 2024-01-09 14:31:19.000000 sonagent-1.0.9/sonagent/rpc/api_server/uvicorn_threaded.py
+-rw-r--r--   0 admin      (501) staff       (20)     6512 2024-01-10 14:18:41.000000 sonagent-1.0.9/sonagent/rpc/api_server/webserver.py
+-rw-r--r--   0 admin      (501) staff       (20)     4331 2024-03-08 17:55:33.000000 sonagent-1.0.9/sonagent/rpc/rpc.py
+-rw-r--r--   0 admin      (501) staff       (20)     1910 2024-01-10 18:03:20.000000 sonagent-1.0.9/sonagent/rpc/rpc_manager.py
+-rw-r--r--   0 admin      (501) staff       (20)      483 2024-01-07 03:46:27.000000 sonagent-1.0.9/sonagent/rpc/rpc_types.py
+-rw-r--r--   0 admin      (501) staff       (20)     1598 2024-02-26 13:28:23.000000 sonagent-1.0.9/sonagent/rpc/schedule_worker.py
+-rw-r--r--   0 admin      (501) staff       (20)    20289 2024-03-17 17:06:21.000000 sonagent-1.0.9/sonagent/rpc/telegram.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.607797 sonagent-1.0.9/sonagent/skills/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2024-03-17 13:02:49.000000 sonagent-1.0.9/sonagent/skills/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.610958 sonagent-1.0.9/sonagent/skills/core_skills/
+-rw-r--r--   0 admin      (501) staff       (20)      543 2024-01-20 06:22:05.000000 sonagent-1.0.9/sonagent/skills/core_skills/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2538 2024-01-10 15:17:51.000000 sonagent-1.0.9/sonagent/skills/core_skills/conversation_summary_skill.py
+-rw-r--r--   0 admin      (501) staff       (20)     2005 2024-01-10 15:09:14.000000 sonagent-1.0.9/sonagent/skills/core_skills/file_io_skill.py
+-rw-r--r--   0 admin      (501) staff       (20)     3800 2024-01-10 15:10:26.000000 sonagent-1.0.9/sonagent/skills/core_skills/http_skill.py
+-rw-r--r--   0 admin      (501) staff       (20)     3314 2024-01-20 06:21:10.000000 sonagent-1.0.9/sonagent/skills/core_skills/math_skill.py
+-rw-r--r--   0 admin      (501) staff       (20)     2526 2024-01-10 15:11:43.000000 sonagent-1.0.9/sonagent/skills/core_skills/text_skill.py
+-rw-r--r--   0 admin      (501) staff       (20)     7959 2024-01-10 15:12:08.000000 sonagent-1.0.9/sonagent/skills/core_skills/time_skill.py
+-rw-r--r--   0 admin      (501) staff       (20)      751 2024-01-10 15:12:43.000000 sonagent-1.0.9/sonagent/skills/core_skills/wait_skill.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.611709 sonagent-1.0.9/sonagent/skills/learning_skills/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2024-01-10 15:33:48.000000 sonagent-1.0.9/sonagent/skills/learning_skills/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)       28 2023-12-15 10:45:54.000000 sonagent-1.0.9/sonagent/skills/learning_skills/run.py
+-rw-r--r--   0 admin      (501) staff       (20)    10363 2024-01-28 04:43:00.000000 sonagent-1.0.9/sonagent/skills/loading.py
+-rw-r--r--   0 admin      (501) staff       (20)      256 2024-01-28 10:05:30.000000 sonagent-1.0.9/sonagent/skills/skills.py
+-rw-r--r--   0 admin      (501) staff       (20)     4269 2024-03-17 16:40:23.000000 sonagent-1.0.9/sonagent/skills/skills_manager.py
+-rw-r--r--   0 admin      (501) staff       (20)     4999 2024-03-08 18:18:05.000000 sonagent-1.0.9/sonagent/sonbot.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.613879 sonagent-1.0.9/sonagent/tools/
+-rw-r--r--   0 admin      (501) staff       (20)      141 2024-03-08 08:59:13.000000 sonagent-1.0.9/sonagent/tools/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      624 2024-03-08 08:59:13.000000 sonagent-1.0.9/sonagent/tools/code_manager.py
+-rw-r--r--   0 admin      (501) staff       (20)     2989 2024-03-08 08:59:13.000000 sonagent-1.0.9/sonagent/tools/git_manager.py
+-rw-r--r--   0 admin      (501) staff       (20)     1224 2024-03-08 08:59:13.000000 sonagent-1.0.9/sonagent/tools/local_code_manager.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.615193 sonagent-1.0.9/sonagent/utils/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-12-10 14:37:57.000000 sonagent-1.0.9/sonagent/utils/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     2616 2023-12-20 02:00:04.000000 sonagent-1.0.9/sonagent/utils/datetime_helpers.py
+-rw-r--r--   0 admin      (501) staff       (20)      458 2024-01-07 04:01:24.000000 sonagent-1.0.9/sonagent/utils/gc_setup.py
+-rw-r--r--   0 admin      (501) staff       (20)      397 2024-03-02 07:26:18.000000 sonagent-1.0.9/sonagent/utils/utils.py
+-rw-r--r--   0 admin      (501) staff       (20)       22 2024-03-17 17:06:37.000000 sonagent-1.0.9/sonagent/version.py
+-rw-r--r--   0 admin      (501) staff       (20)     6427 2024-02-26 13:28:23.000000 sonagent-1.0.9/sonagent/worker.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.615714 sonagent-1.0.9/sonagent.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     3259 2024-03-17 17:07:11.000000 sonagent-1.0.9/sonagent.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     2753 2024-03-17 17:07:11.000000 sonagent-1.0.9/sonagent.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2024-03-17 17:07:11.000000 sonagent-1.0.9/sonagent.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)       48 2024-03-17 17:07:11.000000 sonagent-1.0.9/sonagent.egg-info/entry_points.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2024-03-17 11:58:08.000000 sonagent-1.0.9/sonagent.egg-info/not-zip-safe
+-rw-r--r--   0 admin      (501) staff       (20)      322 2024-03-17 17:07:11.000000 sonagent-1.0.9/sonagent.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       15 2024-03-17 17:07:11.000000 sonagent-1.0.9/sonagent.egg-info/top_level.txt
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-03-17 17:07:11.615503 sonagent-1.0.9/tests/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-12-02 11:24:39.000000 sonagent-1.0.9/tests/__init__.py
```

### Comparing `sonagent-1.0.8/LICENSE` & `sonagent-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/PKG-INFO` & `sonagent-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonagent
-Version: 1.0.8
+Version: 1.0.9
 Summary: Autonomous Agent for Digital Consciousness Backup Using Large Language Models (LLM).
 Home-page: https://github.com/sonnhfit/sonagent
 Author: Son Nguyen Huu
 Author-email: sonnhfit@gmail.com
 License: MIT
 Keywords: agent ai ml language-model autonomus-robots large-language-models llm chatgpt llama2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sonagent-1.0.8/setup.py` & `sonagent-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/agent.py` & `sonagent-1.0.9/sonagent/agent.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/chat.py` & `sonagent-1.0.9/sonagent/chat.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/coding/gencode.py` & `sonagent-1.0.9/sonagent/coding/gencode.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/coding/sonautogen.py` & `sonagent-1.0.9/sonagent/coding/sonautogen.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/commands/arguments.py` & `sonagent-1.0.9/sonagent/commands/arguments.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/commands/cli_options.py` & `sonagent-1.0.9/sonagent/commands/cli_options.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/commands/run_commands.py` & `sonagent-1.0.9/sonagent/commands/run_commands.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/configuration/load_config.py` & `sonagent-1.0.9/sonagent/configuration/load_config.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/core_prompt/me.py` & `sonagent-1.0.9/sonagent/core_prompt/me.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/exceptions.py` & `sonagent-1.0.9/sonagent/exceptions.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/llm/oai_llm.py` & `sonagent-1.0.9/sonagent/llm/oai_llm.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/llm/prompt.py` & `sonagent-1.0.9/sonagent/llm/prompt.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/loggers/__init__.py` & `sonagent-1.0.9/sonagent/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/loggers/set_log_levels.py` & `sonagent-1.0.9/sonagent/loggers/set_log_levels.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/loggers/std_err_stream_handler.py` & `sonagent-1.0.9/sonagent/loggers/std_err_stream_handler.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/main.py` & `sonagent-1.0.9/sonagent/main.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/memory/memory.py` & `sonagent-1.0.9/sonagent/memory/memory.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/memory/short_memory.py` & `sonagent-1.0.9/sonagent/memory/short_memory.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/mixins/logging_mixin.py` & `sonagent-1.0.9/sonagent/mixins/logging_mixin.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/persistence/belief_models.py` & `sonagent-1.0.9/sonagent/persistence/belief_models.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/persistence/migrations.py` & `sonagent-1.0.9/sonagent/persistence/migrations.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/persistence/models.py` & `sonagent-1.0.9/sonagent/persistence/models.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/persistence/planning_models.py` & `sonagent-1.0.9/sonagent/persistence/planning_models.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/planning/planner.py` & `sonagent-1.0.9/sonagent/planning/planner.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/planning/prompt.py` & `sonagent-1.0.9/sonagent/planning/prompt.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/rpc/api_server/api_v1.py` & `sonagent-1.0.9/sonagent/rpc/api_server/api_v1.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/rpc/api_server/uvicorn_threaded.py` & `sonagent-1.0.9/sonagent/rpc/api_server/uvicorn_threaded.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/rpc/api_server/webserver.py` & `sonagent-1.0.9/sonagent/rpc/api_server/webserver.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/rpc/rpc.py` & `sonagent-1.0.9/sonagent/rpc/rpc.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/rpc/rpc_manager.py` & `sonagent-1.0.9/sonagent/rpc/rpc_manager.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/rpc/schedule_worker.py` & `sonagent-1.0.9/sonagent/rpc/schedule_worker.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/rpc/telegram.py` & `sonagent-1.0.9/sonagent/rpc/telegram.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,14 +375,16 @@
         Handler for /show_skills.
         Show version information
         :param bot: telegram bot
         :param update: message update
         :return: None
         """
         result = await self._rpc.show_skills()
+        if result is None or len(result) == 0:
+            result = "Agent doesn't have any available skills."
         await update.message.reply_text(result)
 
     async def _reload_skills(self, update: Update, context: CallbackContext) -> None:
         """
         Handler for /reload_skills.
         Show version information
         :param bot: telegram bot
```

### Comparing `sonagent-1.0.8/sonagent/skills/core_skills/__init__.py` & `sonagent-1.0.9/sonagent/skills/core_skills/__init__.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/skills/core_skills/conversation_summary_skill.py` & `sonagent-1.0.9/sonagent/skills/core_skills/conversation_summary_skill.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/skills/core_skills/file_io_skill.py` & `sonagent-1.0.9/sonagent/skills/core_skills/file_io_skill.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/skills/core_skills/http_skill.py` & `sonagent-1.0.9/sonagent/skills/core_skills/http_skill.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/skills/core_skills/math_skill.py` & `sonagent-1.0.9/sonagent/skills/core_skills/math_skill.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/skills/core_skills/text_skill.py` & `sonagent-1.0.9/sonagent/skills/core_skills/text_skill.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/skills/core_skills/time_skill.py` & `sonagent-1.0.9/sonagent/skills/core_skills/time_skill.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/skills/core_skills/wait_skill.py` & `sonagent-1.0.9/sonagent/skills/core_skills/wait_skill.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/skills/loading.py` & `sonagent-1.0.9/sonagent/skills/loading.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/skills/skills_manager.py` & `sonagent-1.0.9/sonagent/skills/skills_manager.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/sonbot.py` & `sonagent-1.0.9/sonagent/sonbot.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/tools/code_manager.py` & `sonagent-1.0.9/sonagent/tools/code_manager.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/tools/git_manager.py` & `sonagent-1.0.9/sonagent/tools/git_manager.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/tools/local_code_manager.py` & `sonagent-1.0.9/sonagent/tools/local_code_manager.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/utils/datetime_helpers.py` & `sonagent-1.0.9/sonagent/utils/datetime_helpers.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent/worker.py` & `sonagent-1.0.9/sonagent/worker.py`

 * *Files identical despite different names*

### Comparing `sonagent-1.0.8/sonagent.egg-info/PKG-INFO` & `sonagent-1.0.9/sonagent.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonagent
-Version: 1.0.8
+Version: 1.0.9
 Summary: Autonomous Agent for Digital Consciousness Backup Using Large Language Models (LLM).
 Home-page: https://github.com/sonnhfit/sonagent
 Author: Son Nguyen Huu
 Author-email: sonnhfit@gmail.com
 License: MIT
 Keywords: agent ai ml language-model autonomus-robots large-language-models llm chatgpt llama2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sonagent-1.0.8/sonagent.egg-info/SOURCES.txt` & `sonagent-1.0.9/sonagent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

