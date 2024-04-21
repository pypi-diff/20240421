# Comparing `tmp/fei_crypto-0.1.7.tar.gz` & `tmp/fei_crypto-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fei_crypto-0.1.7.tar", max compression
+gzip compressed data, was "fei_crypto-0.1.8.tar", max compression
```

## Comparing `fei_crypto-0.1.7.tar` & `fei_crypto-0.1.8.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0       78 2024-04-16 13:51:49.192517 fei_crypto-0.1.7/fei_crypto/__init__.py
--rw-r--r--   0        0        0      876 2024-04-16 13:53:17.866879 fei_crypto-0.1.7/fei_crypto/captcha.py
--rw-r--r--   0        0        0      488 2023-11-29 13:54:30.172545 fei_crypto-0.1.7/fei_crypto/crypto.py
--rw-r--r--   0        0        0     1218 2024-03-29 08:54:22.246792 fei_crypto-0.1.7/fei_crypto/discordwebhook.py
--rw-r--r--   0        0        0       79 2024-03-21 04:40:21.216364 fei_crypto-0.1.7/fei_crypto/env.py
--rw-r--r--   0        0        0      137 2023-09-26 15:21:11.446999 fei_crypto-0.1.7/fei_crypto/md5.py
--rw-r--r--   0        0        0      319 2023-09-26 14:30:44.514337 fei_crypto-0.1.7/fei_crypto/os.py
--rw-r--r--   0        0        0     1338 2023-11-29 17:18:37.219370 fei_crypto-0.1.7/fei_crypto/rmw.py
--rw-r--r--   0        0        0     1138 2023-09-28 06:14:48.561059 fei_crypto-0.1.7/fei_crypto/rnd_emoj.py
--rw-r--r--   0        0        0     2166 2024-03-29 02:58:44.194898 fei_crypto-0.1.7/fei_crypto/t2m.py
--rw-r--r--   0        0        0      369 2023-09-26 14:38:05.472651 fei_crypto-0.1.7/fei_crypto/time.py
--rw-r--r--   0        0        0     1067 2023-09-18 06:59:02.002584 fei_crypto-0.1.7/LICENSE
--rw-r--r--   0        0        0       58 2023-09-26 14:44:19.909970 fei_crypto-0.1.7/main/__init__.py
--rw-r--r--   0        0        0      120 2023-12-20 05:11:23.650909 fei_crypto-0.1.7/main/btc_eth.py
--rw-r--r--   0        0        0      137 2024-03-29 08:38:57.954290 fei_crypto-0.1.7/main/captcha.py
--rw-r--r--   0        0        0      138 2024-03-29 08:38:24.168499 fei_crypto-0.1.7/main/dc_webhook_send.py
--rw-r--r--   0        0        0      124 2023-12-20 05:11:23.620986 fei_crypto-0.1.7/main/emoj.py
--rw-r--r--   0        0        0      266 2023-12-20 05:11:23.679147 fei_crypto-0.1.7/main/env.py
--rw-r--r--   0        0        0      159 2023-12-20 05:11:54.326071 fei_crypto-0.1.7/main/main.py
--rw-r--r--   0        0        0       98 2023-12-20 05:11:23.591706 fei_crypto-0.1.7/main/os.py
--rw-r--r--   0        0        0      125 2023-12-20 05:11:23.709307 fei_crypto-0.1.7/main/rmw.py
--rw-r--r--   0        0        0       60 2023-09-26 16:09:10.583645 fei_crypto-0.1.7/main/say.py
--rw-r--r--   0        0        0      125 2024-03-28 19:31:13.343469 fei_crypto-0.1.7/main/t2m.py
--rw-r--r--   0        0        0       81 2024-04-02 12:09:40.362527 fei_crypto-0.1.7/main/tg_forward.py
--rw-r--r--   0        0        0      156 2024-04-17 12:01:33.870269 fei_crypto-0.1.7/main/tg_koltime_menu.py
--rw-r--r--   0        0        0       75 2024-04-02 12:07:53.673901 fei_crypto-0.1.7/main/tg_login.py
--rw-r--r--   0        0        0      348 2023-12-20 05:11:23.737349 fei_crypto-0.1.7/main/ts.py
--rw-r--r--   0        0        0       97 2023-09-26 16:09:52.597612 fei_crypto-0.1.7/main/uu_id.py
--rw-r--r--   0        0        0     1614 2024-04-17 12:06:50.897188 fei_crypto-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     3631 2024-04-16 05:01:03.117989 fei_crypto-0.1.7/README.md
--rw-r--r--   0        0        0      389 2024-04-16 14:59:52.401824 fei_crypto-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0      196 2024-04-03 09:48:00.078906 fei_crypto-0.1.7/tests/calc.py
--rw-r--r--   0        0        0      356 2024-04-02 16:40:47.033897 fei_crypto-0.1.7/tests/console.py
--rw-r--r--   0        0        0      183 2024-04-03 03:01:53.459809 fei_crypto-0.1.7/tests/dict.py
--rw-r--r--   0        0        0      463 2024-04-16 14:07:08.378494 fei_crypto-0.1.7/tests/enum_test.py
--rw-r--r--   0        0        0       88 2024-04-17 10:03:49.057111 fei_crypto-0.1.7/tests/env_test.py
--rw-r--r--   0        0        0      206 2024-04-02 15:53:35.170989 fei_crypto-0.1.7/tests/getattr.py
--rw-r--r--   0        0        0       53 2024-03-21 03:22:41.838133 fei_crypto-0.1.7/tests/hello.py
--rw-r--r--   0        0        0     1155 2024-03-21 04:51:46.085571 fei_crypto-0.1.7/tests/image_base64.py
--rw-r--r--   0        0        0      349 2024-04-15 08:49:16.084219 fei_crypto-0.1.7/tests/logging_test.py
--rw-r--r--   0        0        0     1665 2024-03-28 19:19:29.326677 fei_crypto-0.1.7/tests/manim.py
--rw-r--r--   0        0        0      186 2024-04-03 08:27:11.338227 fei_crypto-0.1.7/tests/open.py
--rw-r--r--   0        0        0      545 2024-03-29 07:27:10.711077 fei_crypto-0.1.7/tests/path.py
--rw-r--r--   0        0        0     1312 2024-04-17 11:34:47.610297 fei_crypto-0.1.7/tests/redis_hash.py
--rw-r--r--   0        0        0     2611 2024-04-17 11:57:24.452664 fei_crypto-0.1.7/tests/redis_koltime_channels.py
--rw-r--r--   0        0        0     1036 2024-04-17 09:58:52.863717 fei_crypto-0.1.7/tests/redis_set_test.py
--rw-r--r--   0        0        0      158 2024-04-17 10:41:30.695499 fei_crypto-0.1.7/tests/scope_test.py
--rw-r--r--   0        0        0      495 2024-04-16 20:41:31.838245 fei_crypto-0.1.7/tests/str_test.py
--rw-r--r--   0        0        0     4083 2024-04-16 15:12:18.915950 fei_crypto-0.1.7/tests/tg_arbitrarycallbackdatabot.py
--rw-r--r--   0        0        0     3228 2024-04-16 14:04:46.204833 fei_crypto-0.1.7/tests/tg_inlinebot.py
--rw-r--r--   0        0        0     2468 2024-04-16 14:04:52.248862 fei_crypto-0.1.7/tests/tg_inlinekeyboard.py
--rw-r--r--   0        0        0     6858 2024-04-16 14:05:05.464671 fei_crypto-0.1.7/tests/tg_inlinekeyboard2.py
--rw-r--r--   0        0        0    13620 2024-04-16 14:05:18.553946 fei_crypto-0.1.7/tests/tg_nestedconversationbot.py
--rw-r--r--   0        0        0     6587 2024-04-16 13:40:50.781376 fei_crypto-0.1.7/tests/tg_pollbot.py
--rw-r--r--   0        0        0     2382 2024-04-16 13:40:28.566730 fei_crypto-0.1.7/tests/tg_rawapibot.py
--rw-r--r--   0        0        0     2707 2024-04-16 14:06:07.187762 fei_crypto-0.1.7/tests/tg_webappbot.py
--rw-r--r--   0        0        0      140 2024-04-03 05:46:33.338377 fei_crypto-0.1.7/tests/time.py
--rw-r--r--   0        0        0      924 2024-04-03 02:55:54.333858 fei_crypto-0.1.7/tests/tuple.py
--rw-r--r--   0        0        0      143 2024-04-17 06:38:57.801384 fei_crypto-0.1.7/tests/tuple_list.py
--rw-r--r--   0        0        0      455 2023-11-29 13:21:57.903302 fei_crypto-0.1.7/tests/typer.py
--rw-r--r--   0        0        0       56 2024-04-02 12:07:46.806912 fei_crypto-0.1.7/tg/__init__.py
--rw-r--r--   0        0        0       33 2024-04-02 20:14:26.971417 fei_crypto-0.1.7/tg/bot/__init__.py
--rw-r--r--   0        0        0     4040 2024-04-16 05:45:45.842618 fei_crypto-0.1.7/tg/bot/live_bot.py
--rw-r--r--   0        0        0     1757 2024-04-16 05:44:27.008518 fei_crypto-0.1.7/tg/bot/utils.py
--rw-r--r--   0        0        0     3966 2024-04-16 03:35:51.804389 fei_crypto-0.1.7/tg/cli_forward.py
--rw-r--r--   0        0        0     1665 2024-04-03 03:07:19.467042 fei_crypto-0.1.7/tg/cli_login.py
--rw-r--r--   0        0        0     6472 2024-04-15 12:37:24.327913 fei_crypto-0.1.7/tg/config.py
--rw-r--r--   0        0        0      338 2024-04-03 08:04:18.836132 fei_crypto-0.1.7/tg/const.py
--rw-r--r--   0        0        0     4833 2024-04-17 12:00:28.700820 fei_crypto-0.1.7/tg/koltime_menu_bot.py
--rw-r--r--   0        0        0     3903 2024-04-15 12:46:20.229789 fei_crypto-0.1.7/tg/live.py
--rw-r--r--   0        0        0     2974 2024-04-03 03:07:42.633426 fei_crypto-0.1.7/tg/login.py
--rw-r--r--   0        0        0     2407 2024-04-03 09:46:41.767357 fei_crypto-0.1.7/tg/message.py
--rw-r--r--   0        0        0      356 2024-04-02 17:19:01.228599 fei_crypto-0.1.7/tg/parse.py
--rw-r--r--   0        0        0     3031 2024-04-03 08:31:15.484901 fei_crypto-0.1.7/tg/past.py
--rw-r--r--   0        0        0     1504 2024-04-03 03:07:53.634670 fei_crypto-0.1.7/tg/plugin_models.py
--rw-r--r--   0        0        0     2533 2024-04-03 08:01:56.261327 fei_crypto-0.1.7/tg/plugins/__init__.py
--rw-r--r--   0        0        0      438 2024-04-03 03:06:07.826906 fei_crypto-0.1.7/tg/plugins/caption.py
--rw-r--r--   0        0        0     2401 2024-04-03 07:12:39.950474 fei_crypto-0.1.7/tg/plugins/filter.py
--rw-r--r--   0        0        0      608 2024-04-03 03:06:20.136916 fei_crypto-0.1.7/tg/plugins/fmt.py
--rw-r--r--   0        0        0      573 2024-04-03 03:05:11.028077 fei_crypto-0.1.7/tg/plugins/replace.py
--rw-r--r--   0        0        0      905 2024-04-02 12:49:19.540873 fei_crypto-0.1.7/tg/storage.py
--rw-r--r--   0        0        0     1954 2024-04-16 05:44:49.091593 fei_crypto-0.1.7/tg/utils.py
--rw-r--r--   0        0        0     4729 1970-01-01 00:00:00.000000 fei_crypto-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       78 2024-04-16 13:51:49.192517 fei_crypto-0.1.8/fei_crypto/__init__.py
+-rw-r--r--   0        0        0      876 2024-04-16 13:53:17.866879 fei_crypto-0.1.8/fei_crypto/captcha.py
+-rw-r--r--   0        0        0      488 2023-11-29 13:54:30.172545 fei_crypto-0.1.8/fei_crypto/crypto.py
+-rw-r--r--   0        0        0     1218 2024-03-29 08:54:22.246792 fei_crypto-0.1.8/fei_crypto/discord_webhook.py
+-rw-r--r--   0        0        0       79 2024-03-21 04:40:21.216364 fei_crypto-0.1.8/fei_crypto/env.py
+-rw-r--r--   0        0        0      137 2023-09-26 15:21:11.446999 fei_crypto-0.1.8/fei_crypto/md5.py
+-rw-r--r--   0        0        0      319 2023-09-26 14:30:44.514337 fei_crypto-0.1.8/fei_crypto/os.py
+-rw-r--r--   0        0        0     1338 2023-11-29 17:18:37.219370 fei_crypto-0.1.8/fei_crypto/rmw.py
+-rw-r--r--   0        0        0     1138 2023-09-28 06:14:48.561059 fei_crypto-0.1.8/fei_crypto/rnd_emoj.py
+-rw-r--r--   0        0        0     2166 2024-03-29 02:58:44.194898 fei_crypto-0.1.8/fei_crypto/t2m.py
+-rw-r--r--   0        0        0      369 2023-09-26 14:38:05.472651 fei_crypto-0.1.8/fei_crypto/time.py
+-rw-r--r--   0        0        0     1067 2023-09-18 06:59:02.002584 fei_crypto-0.1.8/LICENSE
+-rw-r--r--   0        0        0       58 2023-09-26 14:44:19.909970 fei_crypto-0.1.8/main/__init__.py
+-rw-r--r--   0        0        0      120 2023-12-20 05:11:23.650909 fei_crypto-0.1.8/main/btc_eth.py
+-rw-r--r--   0        0        0      137 2024-03-29 08:38:57.954290 fei_crypto-0.1.8/main/captcha.py
+-rw-r--r--   0        0        0      139 2024-04-21 00:43:55.013673 fei_crypto-0.1.8/main/dc_webhook_send.py
+-rw-r--r--   0        0        0      124 2023-12-20 05:11:23.620986 fei_crypto-0.1.8/main/emoj.py
+-rw-r--r--   0        0        0      266 2023-12-20 05:11:23.679147 fei_crypto-0.1.8/main/env.py
+-rw-r--r--   0        0        0      159 2023-12-20 05:11:54.326071 fei_crypto-0.1.8/main/main.py
+-rw-r--r--   0        0        0       98 2023-12-20 05:11:23.591706 fei_crypto-0.1.8/main/os.py
+-rw-r--r--   0        0        0      125 2023-12-20 05:11:23.709307 fei_crypto-0.1.8/main/rmw.py
+-rw-r--r--   0        0        0       60 2023-09-26 16:09:10.583645 fei_crypto-0.1.8/main/say.py
+-rw-r--r--   0        0        0      125 2024-03-28 19:31:13.343469 fei_crypto-0.1.8/main/t2m.py
+-rw-r--r--   0        0        0       81 2024-04-02 12:09:40.362527 fei_crypto-0.1.8/main/tg_forward.py
+-rw-r--r--   0        0        0      156 2024-04-17 12:01:33.870269 fei_crypto-0.1.8/main/tg_koltime_menu.py
+-rw-r--r--   0        0        0       75 2024-04-02 12:07:53.673901 fei_crypto-0.1.8/main/tg_login.py
+-rw-r--r--   0        0        0      348 2023-12-20 05:11:23.737349 fei_crypto-0.1.8/main/ts.py
+-rw-r--r--   0        0        0       97 2023-09-26 16:09:52.597612 fei_crypto-0.1.8/main/uu_id.py
+-rw-r--r--   0        0        0     1614 2024-04-21 06:13:13.413216 fei_crypto-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     3627 2024-04-19 14:51:10.754145 fei_crypto-0.1.8/README.md
+-rw-r--r--   0        0        0      389 2024-04-16 14:59:52.401824 fei_crypto-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0      196 2024-04-03 09:48:00.078906 fei_crypto-0.1.8/tests/calc.py
+-rw-r--r--   0        0        0      356 2024-04-02 16:40:47.033897 fei_crypto-0.1.8/tests/console.py
+-rw-r--r--   0        0        0      183 2024-04-03 03:01:53.459809 fei_crypto-0.1.8/tests/dict.py
+-rw-r--r--   0        0        0      463 2024-04-16 14:07:08.378494 fei_crypto-0.1.8/tests/enum_test.py
+-rw-r--r--   0        0        0       88 2024-04-17 10:03:49.057111 fei_crypto-0.1.8/tests/env_test.py
+-rw-r--r--   0        0        0      206 2024-04-02 15:53:35.170989 fei_crypto-0.1.8/tests/getattr.py
+-rw-r--r--   0        0        0       53 2024-03-21 03:22:41.838133 fei_crypto-0.1.8/tests/hello.py
+-rw-r--r--   0        0        0     1155 2024-03-21 04:51:46.085571 fei_crypto-0.1.8/tests/image_base64.py
+-rw-r--r--   0        0        0      349 2024-04-15 08:49:16.084219 fei_crypto-0.1.8/tests/logging_test.py
+-rw-r--r--   0        0        0     1665 2024-03-28 19:19:29.326677 fei_crypto-0.1.8/tests/manim.py
+-rw-r--r--   0        0        0      186 2024-04-03 08:27:11.338227 fei_crypto-0.1.8/tests/open.py
+-rw-r--r--   0        0        0      545 2024-03-29 07:27:10.711077 fei_crypto-0.1.8/tests/path.py
+-rw-r--r--   0        0        0     1312 2024-04-17 11:34:47.610297 fei_crypto-0.1.8/tests/redis_hash.py
+-rw-r--r--   0        0        0     2692 2024-04-17 12:25:13.994779 fei_crypto-0.1.8/tests/redis_koltime_channels.py
+-rw-r--r--   0        0        0     1036 2024-04-17 09:58:52.863717 fei_crypto-0.1.8/tests/redis_set_test.py
+-rw-r--r--   0        0        0      158 2024-04-17 10:41:30.695499 fei_crypto-0.1.8/tests/scope_test.py
+-rw-r--r--   0        0        0      495 2024-04-16 20:41:31.838245 fei_crypto-0.1.8/tests/str_test.py
+-rw-r--r--   0        0        0     4083 2024-04-16 15:12:18.915950 fei_crypto-0.1.8/tests/tg_arbitrarycallbackdatabot.py
+-rw-r--r--   0        0        0     3228 2024-04-16 14:04:46.204833 fei_crypto-0.1.8/tests/tg_inlinebot.py
+-rw-r--r--   0        0        0     2468 2024-04-16 14:04:52.248862 fei_crypto-0.1.8/tests/tg_inlinekeyboard.py
+-rw-r--r--   0        0        0     6858 2024-04-16 14:05:05.464671 fei_crypto-0.1.8/tests/tg_inlinekeyboard2.py
+-rw-r--r--   0        0        0    13620 2024-04-16 14:05:18.553946 fei_crypto-0.1.8/tests/tg_nestedconversationbot.py
+-rw-r--r--   0        0        0     6587 2024-04-16 13:40:50.781376 fei_crypto-0.1.8/tests/tg_pollbot.py
+-rw-r--r--   0        0        0     2382 2024-04-16 13:40:28.566730 fei_crypto-0.1.8/tests/tg_rawapibot.py
+-rw-r--r--   0        0        0     2707 2024-04-16 14:06:07.187762 fei_crypto-0.1.8/tests/tg_webappbot.py
+-rw-r--r--   0        0        0      176 2024-04-21 02:34:34.699548 fei_crypto-0.1.8/tests/time_test.py
+-rw-r--r--   0        0        0      924 2024-04-03 02:55:54.333858 fei_crypto-0.1.8/tests/tuple.py
+-rw-r--r--   0        0        0      143 2024-04-17 06:38:57.801384 fei_crypto-0.1.8/tests/tuple_list.py
+-rw-r--r--   0        0        0      455 2023-11-29 13:21:57.903302 fei_crypto-0.1.8/tests/typer.py
+-rw-r--r--   0        0        0       56 2024-04-02 12:07:46.806912 fei_crypto-0.1.8/tg/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-02 20:14:26.971417 fei_crypto-0.1.8/tg/bot/__init__.py
+-rw-r--r--   0        0        0     4040 2024-04-16 05:45:45.842618 fei_crypto-0.1.8/tg/bot/live_bot.py
+-rw-r--r--   0        0        0     1757 2024-04-16 05:44:27.008518 fei_crypto-0.1.8/tg/bot/utils.py
+-rw-r--r--   0        0        0     3966 2024-04-16 03:35:51.804389 fei_crypto-0.1.8/tg/cli_forward.py
+-rw-r--r--   0        0        0     1665 2024-04-03 03:07:19.467042 fei_crypto-0.1.8/tg/cli_login.py
+-rw-r--r--   0        0        0     6472 2024-04-15 12:37:24.327913 fei_crypto-0.1.8/tg/config.py
+-rw-r--r--   0        0        0      338 2024-04-03 08:04:18.836132 fei_crypto-0.1.8/tg/const.py
+-rw-r--r--   0        0        0     5038 2024-04-21 04:25:21.632950 fei_crypto-0.1.8/tg/koltime_menu_bot.py
+-rw-r--r--   0        0        0     3903 2024-04-15 12:46:20.229789 fei_crypto-0.1.8/tg/live.py
+-rw-r--r--   0        0        0     2974 2024-04-03 03:07:42.633426 fei_crypto-0.1.8/tg/login.py
+-rw-r--r--   0        0        0     2407 2024-04-03 09:46:41.767357 fei_crypto-0.1.8/tg/message.py
+-rw-r--r--   0        0        0      356 2024-04-02 17:19:01.228599 fei_crypto-0.1.8/tg/parse.py
+-rw-r--r--   0        0        0     3031 2024-04-03 08:31:15.484901 fei_crypto-0.1.8/tg/past.py
+-rw-r--r--   0        0        0     1504 2024-04-03 03:07:53.634670 fei_crypto-0.1.8/tg/plugin_models.py
+-rw-r--r--   0        0        0     2533 2024-04-03 08:01:56.261327 fei_crypto-0.1.8/tg/plugins/__init__.py
+-rw-r--r--   0        0        0      438 2024-04-03 03:06:07.826906 fei_crypto-0.1.8/tg/plugins/caption.py
+-rw-r--r--   0        0        0     2401 2024-04-03 07:12:39.950474 fei_crypto-0.1.8/tg/plugins/filter.py
+-rw-r--r--   0        0        0      608 2024-04-03 03:06:20.136916 fei_crypto-0.1.8/tg/plugins/fmt.py
+-rw-r--r--   0        0        0      573 2024-04-03 03:05:11.028077 fei_crypto-0.1.8/tg/plugins/replace.py
+-rw-r--r--   0        0        0      905 2024-04-02 12:49:19.540873 fei_crypto-0.1.8/tg/storage.py
+-rw-r--r--   0        0        0     1954 2024-04-16 05:44:49.091593 fei_crypto-0.1.8/tg/utils.py
+-rw-r--r--   0        0        0     4725 1970-01-01 00:00:00.000000 fei_crypto-0.1.8/PKG-INFO
```

### Comparing `fei_crypto-0.1.7/fei_crypto/captcha.py` & `fei_crypto-0.1.8/fei_crypto/captcha.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/fei_crypto/discordwebhook.py` & `fei_crypto-0.1.8/fei_crypto/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/fei_crypto/rmw.py` & `fei_crypto-0.1.8/fei_crypto/rmw.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/fei_crypto/rnd_emoj.py` & `fei_crypto-0.1.8/fei_crypto/rnd_emoj.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/fei_crypto/t2m.py` & `fei_crypto-0.1.8/fei_crypto/t2m.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/LICENSE` & `fei_crypto-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/pyproject.toml` & `fei_crypto-0.1.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 packages = [
     { include = "fei_crypto" },
     { include = "tg" },
     { include = "main" },
     { include = "tests" },
 ]
 readme = "README.md"
-version = "0.1.7"
+version = "0.1.8"
 
 [tool.poetry.dependencies]
 cowsay = "^6.1"
 filestools = "^0.2.1"
 pillow = "^9.5.0"
 python = "<3.12,>=3.10"
 discord-webhook = "^1.3.1"
```

### Comparing `fei_crypto-0.1.7/README.md` & `fei_crypto-0.1.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     - --out_filename:输出文件名,输出目录为当前目录下的media文件夹,默认值`t2m`
     - --quality:生成媒体质量,默认`low_quality`,还可设置为`medium_quality`|`high_quality`
     - --out_format:输出格式`png`,`gif`,`mp4`,`webm`,`mov`. 默认`gif`
     - --style:动画样式,默认值`0`
     - --preview:是否生成后立即预览
     - --help:帮助文档
 14. dcw # 使用discord webhook send发送消息
-    - 示例:`dc-send 'https://discord.com/api/webhooks/{}' --text 'hello' --file-paths 'e:/btc.mp4,e:/pepe.mp4'`
+    - 示例:`dcw 'https://discord.com/api/webhooks/{}' --text 'hello' --file-paths 'e:/btc.mp4,e:/pepe.mp4'`
     - webhook_url:webhook url
     - --text:发送的文本
     - --file-paths:发送的文件路径,多个路径用逗号分隔
     - --proxy:使用代理,例如`http://127.0.0.1:7890`
     - --help:帮助文档
 15. tgf # 转发telegram group或channel,支持用户转发和机器人转发,转发规则在配置文件`forwards`节点下
     - 用户转发需申请对应的api_id,api_hash,并使用以上`tgl`命令获取`sesssionString`,网址:`https://my.telegram.org/auth`
```

### Comparing `fei_crypto-0.1.7/tests/image_base64.py` & `fei_crypto-0.1.8/tests/image_base64.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tests/manim.py` & `fei_crypto-0.1.8/tests/manim.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tests/path.py` & `fei_crypto-0.1.8/tests/path.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tests/redis_hash.py` & `fei_crypto-0.1.8/tests/redis_hash.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tests/redis_koltime_channels.py` & `fei_crypto-0.1.8/tests/redis_koltime_channels.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,12 +34,13 @@
         ('-1002039765755,WWG-Coinguru,https://t.me/+RdPF6mSz4m8yODM5', 3.0),
         ('-1002136805635,WWG-Trades,https://t.me/+iHRaqQz6SKUzOWMx', 3.0),
         ('-1002006972061,WWG-Hbj,https://t.me/+NSaXsfZaOg0yOTNh', 3.0),
         ('-1002066980585,Eli,https://t.me/+QjNgmwjQtAYzM2Q5', 3.0),
         ('-1002137050425,Woods,https://t.me/+YfRWHc3Gq6JhOGQx', 3.0),
         ('-1002059758917,Johnny,https://t.me/+u4my9wuDIJo1ZDcx', 3.0),
         ('-1002007381555,Rezeh,https://t.me/+bnAFzhnFwnIyYjIx', 3.0),
+        ('-1002012829012,Dr-Profit-Arena,https://t.me/+eV42e2RXgvVjN2Yx', 3.0),
     ]
 
     for v in pindao_sorted_set:
         r.zadd('koltime_menu_bot_channels', {v[0]: v[1]})
         print(v)
```

### Comparing `fei_crypto-0.1.7/tests/redis_set_test.py` & `fei_crypto-0.1.8/tests/redis_set_test.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tests/tg_arbitrarycallbackdatabot.py` & `fei_crypto-0.1.8/tests/tg_arbitrarycallbackdatabot.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tests/tg_inlinebot.py` & `fei_crypto-0.1.8/tests/tg_inlinebot.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tests/tg_inlinekeyboard.py` & `fei_crypto-0.1.8/tests/tg_inlinekeyboard.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tests/tg_inlinekeyboard2.py` & `fei_crypto-0.1.8/tests/tg_inlinekeyboard2.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tests/tg_nestedconversationbot.py` & `fei_crypto-0.1.8/tests/tg_nestedconversationbot.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tests/tg_pollbot.py` & `fei_crypto-0.1.8/tests/tg_pollbot.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tests/tg_rawapibot.py` & `fei_crypto-0.1.8/tests/tg_rawapibot.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tests/tg_webappbot.py` & `fei_crypto-0.1.8/tests/tg_webappbot.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tests/tuple.py` & `fei_crypto-0.1.8/tests/tuple.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tg/bot/live_bot.py` & `fei_crypto-0.1.8/tg/bot/live_bot.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tg/bot/utils.py` & `fei_crypto-0.1.8/tg/bot/utils.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tg/cli_forward.py` & `fei_crypto-0.1.8/tg/cli_forward.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tg/cli_login.py` & `fei_crypto-0.1.8/tg/cli_login.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tg/config.py` & `fei_crypto-0.1.8/tg/config.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tg/koltime_menu_bot.py` & `fei_crypto-0.1.8/tg/koltime_menu_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import os
+from datetime import datetime
+from tg.utils import clean_session_files
 import redis
 import dotenv
 from telegram.ext import (
     Application,
     CommandHandler,
     MessageHandler,
     ContextTypes,
@@ -114,14 +116,15 @@
 
 
 async def qun(update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
     await update.message.reply_text('🍄开发中...')
 
 
 def koltime_menu_bot(env_path: str = '.env') -> None:
+    clean_session_files()
     dotenv.load_dotenv(env_path)
     global r
     if r is None:
         r = redis.Redis(
             host=os.getenv(f'{ENV_PREFIX}REDIS_HOST'),
             port=os.getenv(f'{ENV_PREFIX}REDIS_PORT'),
             password=os.getenv(f'{ENV_PREFIX}REDIS_PASSWORD'),
@@ -147,13 +150,16 @@
     application.add_handler(MessageHandler(filters.Text(['?', FAQ_TEXT]), faq))
     application.add_handler(MessageHandler(filters.Text([PINDAO_TEXT]), pindao))
     application.add_handler(MessageHandler(filters.Text([XUEXI_TEXT]), xuexi))
     application.add_handler(MessageHandler(filters.Text([SHIYONG_TEXT]), shiyong))
     application.add_handler(MessageHandler(filters.Text([VIP_TEXT]), vip))
     application.add_handler(MessageHandler(filters.Text([FANYONG_TEXT]), fanyong))
     application.add_handler(MessageHandler(filters.Text([QUN_TEXT]), qun))
-
-    application.run_polling(allowed_updates=Update.ALL_TYPES)
+    try:
+        print(f"✅ koltime_menu_bot start...,{datetime.now()}")
+        application.run_polling(allowed_updates=Update.ALL_TYPES)
+    except:
+        pass
 
 
 if __name__ == '__main__':
     koltime_menu_bot('d:/.env')
```

### Comparing `fei_crypto-0.1.7/tg/live.py` & `fei_crypto-0.1.8/tg/live.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tg/login.py` & `fei_crypto-0.1.8/tg/login.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tg/message.py` & `fei_crypto-0.1.8/tg/message.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tg/past.py` & `fei_crypto-0.1.8/tg/past.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tg/plugin_models.py` & `fei_crypto-0.1.8/tg/plugin_models.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tg/plugins/__init__.py` & `fei_crypto-0.1.8/tg/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tg/plugins/filter.py` & `fei_crypto-0.1.8/tg/plugins/filter.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tg/plugins/fmt.py` & `fei_crypto-0.1.8/tg/plugins/fmt.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tg/plugins/replace.py` & `fei_crypto-0.1.8/tg/plugins/replace.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tg/storage.py` & `fei_crypto-0.1.8/tg/storage.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/tg/utils.py` & `fei_crypto-0.1.8/tg/utils.py`

 * *Files identical despite different names*

### Comparing `fei_crypto-0.1.7/PKG-INFO` & `fei_crypto-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fei-crypto
-Version: 0.1.7
+Version: 0.1.8
 Summary: fei crypto command utils
 License: MIT
 Author: feicrypto
 Author-email: feicrypto@proton.me
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -74,15 +74,15 @@
     - --out_filename:输出文件名,输出目录为当前目录下的media文件夹,默认值`t2m`
     - --quality:生成媒体质量,默认`low_quality`,还可设置为`medium_quality`|`high_quality`
     - --out_format:输出格式`png`,`gif`,`mp4`,`webm`,`mov`. 默认`gif`
     - --style:动画样式,默认值`0`
     - --preview:是否生成后立即预览
     - --help:帮助文档
 14. dcw # 使用discord webhook send发送消息
-    - 示例:`dc-send 'https://discord.com/api/webhooks/{}' --text 'hello' --file-paths 'e:/btc.mp4,e:/pepe.mp4'`
+    - 示例:`dcw 'https://discord.com/api/webhooks/{}' --text 'hello' --file-paths 'e:/btc.mp4,e:/pepe.mp4'`
     - webhook_url:webhook url
     - --text:发送的文本
     - --file-paths:发送的文件路径,多个路径用逗号分隔
     - --proxy:使用代理,例如`http://127.0.0.1:7890`
     - --help:帮助文档
 15. tgf # 转发telegram group或channel,支持用户转发和机器人转发,转发规则在配置文件`forwards`节点下
     - 用户转发需申请对应的api_id,api_hash,并使用以上`tgl`命令获取`sesssionString`,网址:`https://my.telegram.org/auth`
```

