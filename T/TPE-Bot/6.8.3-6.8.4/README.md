# Comparing `tmp/TPE-Bot-6.8.3.tar.gz` & `tmp/TPE-Bot-6.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TPE-Bot-6.8.3.tar", last modified: Thu Apr 18 10:51:05 2024, max compression
+gzip compressed data, was "TPE-Bot-6.8.4.tar", last modified: Sun Apr 21 08:40:54 2024, max compression
```

## Comparing `TPE-Bot-6.8.3.tar` & `TPE-Bot-6.8.4.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.109480 TPE-Bot-6.8.3/
--rw-r--r--   0 ester      (501) staff       (20)      276 2024-04-18 10:51:05.109247 TPE-Bot-6.8.3/PKG-INFO
--rwxr-xr-x   0 ester      (501) staff       (20)     1228 2023-12-07 03:26:39.000000 TPE-Bot-6.8.3/README.md
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.067060 TPE-Bot-6.8.3/TPE_Bot.egg-info/
--rw-r--r--   0 ester      (501) staff       (20)      276 2024-04-18 10:51:04.000000 TPE-Bot-6.8.3/TPE_Bot.egg-info/PKG-INFO
--rw-r--r--   0 ester      (501) staff       (20)     7054 2024-04-18 10:51:05.000000 TPE-Bot-6.8.3/TPE_Bot.egg-info/SOURCES.txt
--rw-r--r--   0 ester      (501) staff       (20)        1 2024-04-18 10:51:04.000000 TPE-Bot-6.8.3/TPE_Bot.egg-info/dependency_links.txt
--rw-r--r--   0 ester      (501) staff       (20)      144 2024-04-18 10:51:04.000000 TPE-Bot-6.8.3/TPE_Bot.egg-info/requires.txt
--rw-r--r--   0 ester      (501) staff       (20)       17 2024-04-18 10:51:04.000000 TPE-Bot-6.8.3/TPE_Bot.egg-info/top_level.txt
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.067768 TPE-Bot-6.8.3/buildABot/
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.068584 TPE-Bot-6.8.3/buildABot/Bot/
--rw-rw-r--   0 ester      (501) staff       (20)    51887 2024-04-18 10:04:26.000000 TPE-Bot-6.8.3/buildABot/Bot/BotController.py
--rw-rw-r--   0 ester      (501) staff       (20)    31775 2024-04-18 10:04:26.000000 TPE-Bot-6.8.3/buildABot/Bot/BotManager.py
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.069139 TPE-Bot-6.8.3/buildABot/Bot/Dashboard/
--rw-rw-r--   0 ester      (501) staff       (20)    40955 2024-04-18 10:07:42.000000 TPE-Bot-6.8.3/buildABot/Bot/Dashboard/Analytics.py
--rw-rw-r--   0 ester      (501) staff       (20)     8583 2024-04-18 10:07:42.000000 TPE-Bot-6.8.3/buildABot/Bot/Dashboard/TelegramLogs.py
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.069384 TPE-Bot-6.8.3/buildABot/Bot/Dashboard/pytransform/
--rw-rw-r--   0 ester      (501) staff       (20)    13587 2024-04-18 09:40:40.000000 TPE-Bot-6.8.3/buildABot/Bot/Dashboard/pytransform/__init__.py
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.070731 TPE-Bot-6.8.3/buildABot/Bot/Firebase/
--rw-rw-r--   0 ester      (501) staff       (20)    15995 2024-04-18 10:07:22.000000 TPE-Bot-6.8.3/buildABot/Bot/Firebase/Entities.py
--rw-rw-r--   0 ester      (501) staff       (20)    12667 2024-04-18 10:07:22.000000 TPE-Bot-6.8.3/buildABot/Bot/Firebase/Firebase_Learn.py
--rw-rw-r--   0 ester      (501) staff       (20)    14443 2024-04-18 10:07:22.000000 TPE-Bot-6.8.3/buildABot/Bot/Firebase/Firebase_Reco.py
--rw-rw-r--   0 ester      (501) staff       (20)    17443 2024-04-18 10:07:22.000000 TPE-Bot-6.8.3/buildABot/Bot/Firebase/Webhook_Learn.py
--rw-rw-r--   0 ester      (501) staff       (20)    36671 2024-04-18 10:07:22.000000 TPE-Bot-6.8.3/buildABot/Bot/Firebase/Webhook_Reco.py
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.071026 TPE-Bot-6.8.3/buildABot/Bot/Firebase/pytransform/
--rw-rw-r--   0 ester      (501) staff       (20)    13587 2024-04-18 09:40:40.000000 TPE-Bot-6.8.3/buildABot/Bot/Firebase/pytransform/__init__.py
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.074828 TPE-Bot-6.8.3/buildABot/Bot/Intents/
--rw-rw-r--   0 ester      (501) staff       (20)    17491 2024-04-18 10:06:38.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/CustomIntents.py
--rw-rw-r--   0 ester      (501) staff       (20)    27091 2024-04-18 10:06:38.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/CustomMenu.py
--rw-rw-r--   0 ester      (501) staff       (20)    30703 2024-04-18 10:06:38.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/CustomRecommendedMenu.py
--rw-rw-r--   0 ester      (501) staff       (20)     9167 2024-04-18 10:06:38.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/CustomResponse.py
--rw-rw-r--   0 ester      (501) staff       (20)    16135 2024-04-18 10:06:40.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/CustomTeleResponse.py
--rw-rw-r--   0 ester      (501) staff       (20)    28675 2024-04-18 10:06:40.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/DefaultIntent.py
--rw-rw-r--   0 ester      (501) staff       (20)    24343 2024-04-18 10:06:40.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/FAQ.py
--rw-rw-r--   0 ester      (501) staff       (20)    11403 2024-04-18 10:06:40.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/FallbackSocialTag.py
--rw-rw-r--   0 ester      (501) staff       (20)    16991 2024-04-18 10:06:40.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/Paraphraser.py
--rw-rw-r--   0 ester      (501) staff       (20)    14847 2024-04-18 10:06:40.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/RelatedIntents.py
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.076830 TPE-Bot-6.8.3/buildABot/Bot/Intents/Type/
--rw-rw-r--   0 ester      (501) staff       (20)     7907 2024-04-18 10:41:38.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/Type/AccordionCard.py
--rw-rw-r--   0 ester      (501) staff       (20)     5059 2024-04-18 10:41:38.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/Type/ButtonCard.py
--rw-rw-r--   0 ester      (501) staff       (20)    12923 2024-04-18 10:41:38.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/Type/Chips.py
--rw-rw-r--   0 ester      (501) staff       (20)     5979 2024-04-18 10:41:38.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/Type/DescriptionCard.py
--rw-rw-r--   0 ester      (501) staff       (20)     4291 2024-04-18 10:41:38.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/Type/ImageCard.py
--rw-rw-r--   0 ester      (501) staff       (20)     7079 2024-04-18 10:41:38.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/Type/InfoCard.py
--rw-rw-r--   0 ester      (501) staff       (20)    11023 2024-04-18 10:41:38.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/Type/ListCard.py
--rw-rw-r--   0 ester      (501) staff       (20)    21975 2024-04-18 10:06:40.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/Usersays.py
--rw-rw-r--   0 ester      (501) staff       (20)    15903 2024-04-18 10:06:40.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/WelcomeIntent.py
--rw-rw-r--   0 ester      (501) staff       (20)    30215 2024-04-18 10:06:40.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/Worksheets_Learn.py
--rw-rw-r--   0 ester      (501) staff       (20)    30547 2024-04-18 10:06:40.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/Worksheets_Reco.py
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.077117 TPE-Bot-6.8.3/buildABot/Bot/Intents/pytransform/
--rw-rw-r--   0 ester      (501) staff       (20)    13587 2024-04-18 09:40:40.000000 TPE-Bot-6.8.3/buildABot/Bot/Intents/pytransform/__init__.py
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.077956 TPE-Bot-6.8.3/buildABot/Bot/Webapp/
--rw-rw-r--   0 ester      (501) staff       (20)    17163 2024-04-18 10:08:00.000000 TPE-Bot-6.8.3/buildABot/Bot/Webapp/WebApp_Learn.py
--rw-rw-r--   0 ester      (501) staff       (20)     7767 2024-04-18 10:08:00.000000 TPE-Bot-6.8.3/buildABot/Bot/Webapp/WebApp_Reco.py
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.078305 TPE-Bot-6.8.3/buildABot/Bot/Webapp/pytransform/
--rw-rw-r--   0 ester      (501) staff       (20)    13587 2024-04-18 09:40:40.000000 TPE-Bot-6.8.3/buildABot/Bot/Webapp/pytransform/__init__.py
--rw-rw-r--   0 ester      (501) staff       (20)    24155 2024-04-18 10:04:26.000000 TPE-Bot-6.8.3/buildABot/Bot/WriteToFile.py
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.078597 TPE-Bot-6.8.3/buildABot/Bot/pytransform/
--rw-rw-r--   0 ester      (501) staff       (20)    13587 2024-04-18 09:40:40.000000 TPE-Bot-6.8.3/buildABot/Bot/pytransform/__init__.py
--rw-rw-r--   0 ester      (501) staff       (20)    14207 2024-04-18 10:03:50.000000 TPE-Bot-6.8.3/buildABot/BotHelper.py
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.078879 TPE-Bot-6.8.3/buildABot/Data/
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.088256 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/
--rw-rw-r--   0 ester      (501) staff       (20)     1169 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Default Welcome Intent - Telegram - Check Submission.json
--rw-rw-r--   0 ester      (501) staff       (20)      267 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Default Welcome Intent - Telegram - Check Submission_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)      244 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Default Welcome Intent - Telegram_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)     1524 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Default Welcome Intent - Web - Fallback.json
--rw-rw-r--   0 ester      (501) staff       (20)     1676 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Default Welcome Intent - Web.json
--rw-rw-r--   0 ester      (501) staff       (20)      451 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Default Welcome Intent - Web_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)     2486 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Downvote.json
--rw-rw-r--   0 ester      (501) staff       (20)      982 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Downvote_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)     3787 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Email Enquiry.json
--rw-rw-r--   0 ester      (501) staff       (20)     2453 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)     1518 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Exit Conversation.json
--rw-rw-r--   0 ester      (501) staff       (20)     2173 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)     1846 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Fallback - no.json
--rw-rw-r--   0 ester      (501) staff       (20)    10352 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Fallback - no_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)      943 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Fallback - yes - fallback.json
--rw-rw-r--   0 ester      (501) staff       (20)     1225 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Fallback - yes.json
--rw-rw-r--   0 ester      (501) staff       (20)     9708 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Fallback - yes_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)      612 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Fallback.json
--rw-rw-r--   0 ester      (501) staff       (20)     1166 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Remember Name.json
--rw-rw-r--   0 ester      (501) staff       (20)      239 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Remember Name_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)      249 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Sentiment (Awesome)_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)      252 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Sentiment (Doing Fine)_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)      264 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Sentiment (It's been a rough week)_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)      261 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Sentiment (Still Hanging There)_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)     1154 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login.json
--rw-rw-r--   0 ester      (501) staff       (20)      597 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)     1079 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Thankyou.json
--rw-rw-r--   0 ester      (501) staff       (20)     1496 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Thankyou_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)     1724 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Upvote.json
--rw-rw-r--   0 ester      (501) staff       (20)      241 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Upvote_usersays_en.json
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.100054 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/
--rw-rw-r--   0 ester      (501) staff       (20)     1169 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Default Welcome Intent - Telegram - Check Submission.json
--rw-rw-r--   0 ester      (501) staff       (20)      267 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Default Welcome Intent - Telegram - Check Submission_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)      244 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Default Welcome Intent - Telegram_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)     1524 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Default Welcome Intent - Web - Fallback.json
--rw-rw-r--   0 ester      (501) staff       (20)     1676 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Default Welcome Intent - Web.json
--rw-rw-r--   0 ester      (501) staff       (20)      451 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Default Welcome Intent - Web_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)     2486 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Downvote.json
--rw-rw-r--   0 ester      (501) staff       (20)      982 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Downvote_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)     3787 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Email Enquiry.json
--rw-rw-r--   0 ester      (501) staff       (20)     2453 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)     1518 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Exit Conversation.json
--rw-rw-r--   0 ester      (501) staff       (20)     2173 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)     1074 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Log In.json
--rw-rw-r--   0 ester      (501) staff       (20)     1846 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Fallback - no.json
--rw-rw-r--   0 ester      (501) staff       (20)    10352 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Fallback - no_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)      943 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Fallback - yes - fallback.json
--rw-rw-r--   0 ester      (501) staff       (20)     1225 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Fallback - yes.json
--rw-rw-r--   0 ester      (501) staff       (20)     9708 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Fallback - yes_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)      612 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Fallback.json
--rw-rw-r--   0 ester      (501) staff       (20)     1166 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Remember Name.json
--rw-rw-r--   0 ester      (501) staff       (20)      239 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Remember Name_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)      249 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Sentiment (Awesome)_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)      252 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Sentiment (Doing Fine)_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)      264 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Sentiment (It's been a rough week)_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)      261 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Sentiment (Still Hanging There)_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)     1154 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login.json
--rw-rw-r--   0 ester      (501) staff       (20)      597 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)     2493 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Menu - Main.json
--rw-rw-r--   0 ester      (501) staff       (20)     2454 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)     1079 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Thankyou.json
--rw-rw-r--   0 ester      (501) staff       (20)     1496 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)     1724 2024-04-18 09:57:36.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Upvote.json
--rw-rw-r--   0 ester      (501) staff       (20)      241 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Upvote_usersays_en.json
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.101421 TPE-Bot-6.8.3/buildABot/Data/Default - Worksheets/
--rw-rw-r--   0 ester      (501) staff       (20)      249 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Worksheets/Log In - Sentiment (Awesome)_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)      252 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Worksheets/Log In - Sentiment (Doing Fine)_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)      264 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Worksheets/Log In - Sentiment (It's been a rough week)_usersays_en.json
--rw-rw-r--   0 ester      (501) staff       (20)      261 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/Default - Worksheets/Log In - Sentiment (Still Hanging There)_usersays_en.json
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.101739 TPE-Bot-6.8.3/buildABot/Data/Entities/
--rw-rw-r--   0 ester      (501) staff       (20)      208 2024-04-18 09:57:38.000000 TPE-Bot-6.8.3/buildABot/Data/Entities/LoginID.json
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.102718 TPE-Bot-6.8.3/buildABot/Data/WebApp/
--rw-rw-r--   0 ester      (501) staff       (20)    26864 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/WebApp/index_template_LEARN.html
--rw-rw-r--   0 ester      (501) staff       (20)    26864 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/WebApp/index_template_RECO.html
--rw-rw-r--   0 ester      (501) staff       (20)   817197 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/WebApp/reset_template_RECO.js
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.105710 TPE-Bot-6.8.3/buildABot/Data/Webhook/
--rw-rw-r--   0 ester      (501) staff       (20)     2162 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/Webhook/CheckPwd_Template_RECO.js
--rw-rw-r--   0 ester      (501) staff       (20)     4597 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js
--rw-rw-r--   0 ester      (501) staff       (20)     3951 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/Webhook/ReportCard_Template_RECO.js
--rw-rw-r--   0 ester      (501) staff       (20)     9491 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/Webhook/index_template_LEARN.js
--rw-rw-r--   0 ester      (501) staff       (20)    12453 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/Webhook/index_template_RECO.js
--rw-rw-r--   0 ester      (501) staff       (20)      720 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/Webhook/package.json
--rw-rw-r--   0 ester      (501) staff       (20)       18 2024-04-18 09:57:34.000000 TPE-Bot-6.8.3/buildABot/Data/__init__.py
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.106806 TPE-Bot-6.8.3/buildABot/QA/
--rw-rw-r--   0 ester      (501) staff       (20)    10471 2024-04-18 10:09:00.000000 TPE-Bot-6.8.3/buildABot/QA/DataBank.py
--rw-rw-r--   0 ester      (501) staff       (20)     6603 2024-04-18 10:09:00.000000 TPE-Bot-6.8.3/buildABot/QA/Para.py
--rw-rw-r--   0 ester      (501) staff       (20)    16483 2024-04-18 10:09:00.000000 TPE-Bot-6.8.3/buildABot/QA/QAManager.py
--rw-rw-r--   0 ester      (501) staff       (20)     5863 2024-04-18 10:09:00.000000 TPE-Bot-6.8.3/buildABot/QA/Responses.py
--rw-rw-r--   0 ester      (501) staff       (20)     6375 2024-04-18 10:03:50.000000 TPE-Bot-6.8.3/buildABot/QAHelper.py
--rw-rw-r--   0 ester      (501) staff       (20)     7919 2024-04-18 10:03:50.000000 TPE-Bot-6.8.3/buildABot/__init__.py
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.107088 TPE-Bot-6.8.3/buildABot/pytransform/
--rw-rw-r--   0 ester      (501) staff       (20)    13587 2024-04-18 09:40:40.000000 TPE-Bot-6.8.3/buildABot/pytransform/__init__.py
-drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-18 10:51:05.108853 TPE-Bot-6.8.3/parrot/
--rwx------   0 ester      (501) staff       (20)       34 2023-03-23 19:45:54.000000 TPE-Bot-6.8.3/parrot/__init__.py
--rwx------   0 ester      (501) staff       (20)      804 2023-03-23 19:45:54.000000 TPE-Bot-6.8.3/parrot/demo.py
--rwx------   0 ester      (501) staff       (20)     6089 2023-03-23 19:45:54.000000 TPE-Bot-6.8.3/parrot/filters.py
--rwx------   0 ester      (501) staff       (20)     5955 2023-03-23 19:45:54.000000 TPE-Bot-6.8.3/parrot/parrot.py
--rw-r--r--   0 ester      (501) staff       (20)       38 2024-04-18 10:51:05.109563 TPE-Bot-6.8.3/setup.cfg
--rwx------   0 ester      (501) staff       (20)      954 2024-04-18 10:50:51.000000 TPE-Bot-6.8.3/setup.py
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.339459 TPE-Bot-6.8.4/
+-rw-r--r--   0 ester      (501) staff       (20)      276 2024-04-21 08:40:54.339275 TPE-Bot-6.8.4/PKG-INFO
+-rwxr-xr-x   0 ester      (501) staff       (20)     1228 2023-12-07 03:26:39.000000 TPE-Bot-6.8.4/README.md
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.308005 TPE-Bot-6.8.4/TPE_Bot.egg-info/
+-rw-r--r--   0 ester      (501) staff       (20)      276 2024-04-21 08:40:53.000000 TPE-Bot-6.8.4/TPE_Bot.egg-info/PKG-INFO
+-rw-r--r--   0 ester      (501) staff       (20)     7054 2024-04-21 08:40:54.000000 TPE-Bot-6.8.4/TPE_Bot.egg-info/SOURCES.txt
+-rw-r--r--   0 ester      (501) staff       (20)        1 2024-04-21 08:40:53.000000 TPE-Bot-6.8.4/TPE_Bot.egg-info/dependency_links.txt
+-rw-r--r--   0 ester      (501) staff       (20)      144 2024-04-21 08:40:54.000000 TPE-Bot-6.8.4/TPE_Bot.egg-info/requires.txt
+-rw-r--r--   0 ester      (501) staff       (20)       17 2024-04-21 08:40:54.000000 TPE-Bot-6.8.4/TPE_Bot.egg-info/top_level.txt
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.308702 TPE-Bot-6.8.4/buildABot/
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.309490 TPE-Bot-6.8.4/buildABot/Bot/
+-rw-rw-r--   0 ester      (501) staff       (20)    51887 2024-04-18 10:04:26.000000 TPE-Bot-6.8.4/buildABot/Bot/BotController.py
+-rw-rw-r--   0 ester      (501) staff       (20)    31775 2024-04-18 10:04:26.000000 TPE-Bot-6.8.4/buildABot/Bot/BotManager.py
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.310003 TPE-Bot-6.8.4/buildABot/Bot/Dashboard/
+-rw-rw-r--   0 ester      (501) staff       (20)    40955 2024-04-18 10:07:42.000000 TPE-Bot-6.8.4/buildABot/Bot/Dashboard/Analytics.py
+-rw-rw-r--   0 ester      (501) staff       (20)     8583 2024-04-18 10:07:42.000000 TPE-Bot-6.8.4/buildABot/Bot/Dashboard/TelegramLogs.py
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.310225 TPE-Bot-6.8.4/buildABot/Bot/Dashboard/pytransform/
+-rw-rw-r--   0 ester      (501) staff       (20)    13587 2024-04-18 09:40:40.000000 TPE-Bot-6.8.4/buildABot/Bot/Dashboard/pytransform/__init__.py
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.311442 TPE-Bot-6.8.4/buildABot/Bot/Firebase/
+-rw-rw-r--   0 ester      (501) staff       (20)    15995 2024-04-18 10:07:22.000000 TPE-Bot-6.8.4/buildABot/Bot/Firebase/Entities.py
+-rw-rw-r--   0 ester      (501) staff       (20)    12667 2024-04-18 10:07:22.000000 TPE-Bot-6.8.4/buildABot/Bot/Firebase/Firebase_Learn.py
+-rw-rw-r--   0 ester      (501) staff       (20)    14443 2024-04-18 10:07:22.000000 TPE-Bot-6.8.4/buildABot/Bot/Firebase/Firebase_Reco.py
+-rw-rw-r--   0 ester      (501) staff       (20)    17443 2024-04-18 10:07:22.000000 TPE-Bot-6.8.4/buildABot/Bot/Firebase/Webhook_Learn.py
+-rw-rw-r--   0 ester      (501) staff       (20)    36671 2024-04-18 10:07:22.000000 TPE-Bot-6.8.4/buildABot/Bot/Firebase/Webhook_Reco.py
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.311729 TPE-Bot-6.8.4/buildABot/Bot/Firebase/pytransform/
+-rw-rw-r--   0 ester      (501) staff       (20)    13587 2024-04-18 09:40:40.000000 TPE-Bot-6.8.4/buildABot/Bot/Firebase/pytransform/__init__.py
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.315318 TPE-Bot-6.8.4/buildABot/Bot/Intents/
+-rw-rw-r--   0 ester      (501) staff       (20)    17491 2024-04-18 10:06:38.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/CustomIntents.py
+-rw-rw-r--   0 ester      (501) staff       (20)    27091 2024-04-18 10:06:38.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/CustomMenu.py
+-rw-rw-r--   0 ester      (501) staff       (20)    30703 2024-04-18 10:06:38.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/CustomRecommendedMenu.py
+-rw-rw-r--   0 ester      (501) staff       (20)     9167 2024-04-18 10:06:38.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/CustomResponse.py
+-rw-rw-r--   0 ester      (501) staff       (20)    16135 2024-04-18 10:06:40.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/CustomTeleResponse.py
+-rw-rw-r--   0 ester      (501) staff       (20)    28675 2024-04-18 10:06:40.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/DefaultIntent.py
+-rw-rw-r--   0 ester      (501) staff       (20)    24343 2024-04-18 10:06:40.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/FAQ.py
+-rw-rw-r--   0 ester      (501) staff       (20)    11403 2024-04-18 10:06:40.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/FallbackSocialTag.py
+-rw-rw-r--   0 ester      (501) staff       (20)    16991 2024-04-18 10:06:40.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/Paraphraser.py
+-rw-rw-r--   0 ester      (501) staff       (20)    14847 2024-04-18 10:06:40.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/RelatedIntents.py
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.317051 TPE-Bot-6.8.4/buildABot/Bot/Intents/Type/
+-rw-rw-r--   0 ester      (501) staff       (20)     7907 2024-04-18 10:41:38.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/Type/AccordionCard.py
+-rw-rw-r--   0 ester      (501) staff       (20)     5059 2024-04-18 10:41:38.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/Type/ButtonCard.py
+-rw-rw-r--   0 ester      (501) staff       (20)    12923 2024-04-18 10:41:38.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/Type/Chips.py
+-rw-rw-r--   0 ester      (501) staff       (20)     5979 2024-04-18 10:41:38.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/Type/DescriptionCard.py
+-rw-rw-r--   0 ester      (501) staff       (20)     4291 2024-04-18 10:41:38.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/Type/ImageCard.py
+-rw-rw-r--   0 ester      (501) staff       (20)     7079 2024-04-18 10:41:38.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/Type/InfoCard.py
+-rw-rw-r--   0 ester      (501) staff       (20)    11023 2024-04-18 10:41:38.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/Type/ListCard.py
+-rw-rw-r--   0 ester      (501) staff       (20)    21975 2024-04-18 10:06:40.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/Usersays.py
+-rw-rw-r--   0 ester      (501) staff       (20)    15903 2024-04-18 10:06:40.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/WelcomeIntent.py
+-rw-rw-r--   0 ester      (501) staff       (20)    30215 2024-04-18 10:06:40.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/Worksheets_Learn.py
+-rw-rw-r--   0 ester      (501) staff       (20)    30547 2024-04-18 10:06:40.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/Worksheets_Reco.py
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.317275 TPE-Bot-6.8.4/buildABot/Bot/Intents/pytransform/
+-rw-rw-r--   0 ester      (501) staff       (20)    13587 2024-04-18 09:40:40.000000 TPE-Bot-6.8.4/buildABot/Bot/Intents/pytransform/__init__.py
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.317768 TPE-Bot-6.8.4/buildABot/Bot/Webapp/
+-rw-rw-r--   0 ester      (501) staff       (20)    17163 2024-04-18 10:08:00.000000 TPE-Bot-6.8.4/buildABot/Bot/Webapp/WebApp_Learn.py
+-rw-rw-r--   0 ester      (501) staff       (20)     7767 2024-04-18 10:08:00.000000 TPE-Bot-6.8.4/buildABot/Bot/Webapp/WebApp_Reco.py
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.318002 TPE-Bot-6.8.4/buildABot/Bot/Webapp/pytransform/
+-rw-rw-r--   0 ester      (501) staff       (20)    13587 2024-04-18 09:40:40.000000 TPE-Bot-6.8.4/buildABot/Bot/Webapp/pytransform/__init__.py
+-rw-rw-r--   0 ester      (501) staff       (20)    24155 2024-04-18 10:04:26.000000 TPE-Bot-6.8.4/buildABot/Bot/WriteToFile.py
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.318231 TPE-Bot-6.8.4/buildABot/Bot/pytransform/
+-rw-rw-r--   0 ester      (501) staff       (20)    13587 2024-04-18 09:40:40.000000 TPE-Bot-6.8.4/buildABot/Bot/pytransform/__init__.py
+-rw-rw-r--   0 ester      (501) staff       (20)    14207 2024-04-18 10:03:50.000000 TPE-Bot-6.8.4/buildABot/BotHelper.py
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.318444 TPE-Bot-6.8.4/buildABot/Data/
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.325393 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/
+-rw-rw-r--   0 ester      (501) staff       (20)     1169 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Default Welcome Intent - Telegram - Check Submission.json
+-rw-rw-r--   0 ester      (501) staff       (20)      267 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Default Welcome Intent - Telegram - Check Submission_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)      244 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Default Welcome Intent - Telegram_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1524 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Default Welcome Intent - Web - Fallback.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1676 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Default Welcome Intent - Web.json
+-rw-rw-r--   0 ester      (501) staff       (20)      451 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Default Welcome Intent - Web_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)     2486 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Downvote.json
+-rw-rw-r--   0 ester      (501) staff       (20)      982 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Downvote_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)     3787 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Email Enquiry.json
+-rw-rw-r--   0 ester      (501) staff       (20)     2453 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1518 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Exit Conversation.json
+-rw-rw-r--   0 ester      (501) staff       (20)     2173 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1846 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Fallback - no.json
+-rw-rw-r--   0 ester      (501) staff       (20)    10352 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Fallback - no_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)      943 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Fallback - yes - fallback.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1225 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Fallback - yes.json
+-rw-rw-r--   0 ester      (501) staff       (20)     9708 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Fallback - yes_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)      612 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Fallback.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1166 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Remember Name.json
+-rw-rw-r--   0 ester      (501) staff       (20)      239 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Remember Name_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)      249 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Sentiment (Awesome)_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)      252 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Sentiment (Doing Fine)_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)      264 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Sentiment (It's been a rough week)_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)      261 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Sentiment (Still Hanging There)_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1154 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login.json
+-rw-rw-r--   0 ester      (501) staff       (20)      597 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1079 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Thankyou.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1496 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Thankyou_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1724 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Upvote.json
+-rw-rw-r--   0 ester      (501) staff       (20)      241 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Upvote_usersays_en.json
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.333078 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/
+-rw-rw-r--   0 ester      (501) staff       (20)     1169 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Default Welcome Intent - Telegram - Check Submission.json
+-rw-rw-r--   0 ester      (501) staff       (20)      267 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Default Welcome Intent - Telegram - Check Submission_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)      244 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Default Welcome Intent - Telegram_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1524 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Default Welcome Intent - Web - Fallback.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1676 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Default Welcome Intent - Web.json
+-rw-rw-r--   0 ester      (501) staff       (20)      451 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Default Welcome Intent - Web_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)     2486 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Downvote.json
+-rw-rw-r--   0 ester      (501) staff       (20)      982 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Downvote_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)     3787 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Email Enquiry.json
+-rw-rw-r--   0 ester      (501) staff       (20)     2453 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1518 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Exit Conversation.json
+-rw-rw-r--   0 ester      (501) staff       (20)     2173 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1074 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Log In.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1846 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Fallback - no.json
+-rw-rw-r--   0 ester      (501) staff       (20)    10352 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Fallback - no_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)      943 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Fallback - yes - fallback.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1225 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Fallback - yes.json
+-rw-rw-r--   0 ester      (501) staff       (20)     9708 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Fallback - yes_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)      612 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Fallback.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1166 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Remember Name.json
+-rw-rw-r--   0 ester      (501) staff       (20)      239 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Remember Name_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)      249 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Sentiment (Awesome)_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)      252 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Sentiment (Doing Fine)_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)      264 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Sentiment (It's been a rough week)_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)      261 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Sentiment (Still Hanging There)_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1154 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login.json
+-rw-rw-r--   0 ester      (501) staff       (20)      597 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)     2493 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Menu - Main.json
+-rw-rw-r--   0 ester      (501) staff       (20)     2454 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1079 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Thankyou.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1496 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)     1724 2024-04-18 09:57:36.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Upvote.json
+-rw-rw-r--   0 ester      (501) staff       (20)      241 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Upvote_usersays_en.json
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.334029 TPE-Bot-6.8.4/buildABot/Data/Default - Worksheets/
+-rw-rw-r--   0 ester      (501) staff       (20)      249 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Worksheets/Log In - Sentiment (Awesome)_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)      252 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Worksheets/Log In - Sentiment (Doing Fine)_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)      264 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Worksheets/Log In - Sentiment (It's been a rough week)_usersays_en.json
+-rw-rw-r--   0 ester      (501) staff       (20)      261 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/Default - Worksheets/Log In - Sentiment (Still Hanging There)_usersays_en.json
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.334262 TPE-Bot-6.8.4/buildABot/Data/Entities/
+-rw-rw-r--   0 ester      (501) staff       (20)      208 2024-04-18 09:57:38.000000 TPE-Bot-6.8.4/buildABot/Data/Entities/LoginID.json
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.334960 TPE-Bot-6.8.4/buildABot/Data/WebApp/
+-rw-rw-r--   0 ester      (501) staff       (20)    26864 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/WebApp/index_template_LEARN.html
+-rw-rw-r--   0 ester      (501) staff       (20)    26864 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/WebApp/index_template_RECO.html
+-rw-rw-r--   0 ester      (501) staff       (20)   817197 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/WebApp/reset_template_RECO.js
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.337075 TPE-Bot-6.8.4/buildABot/Data/Webhook/
+-rw-rw-r--   0 ester      (501) staff       (20)     2162 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/Webhook/CheckPwd_Template_RECO.js
+-rw-rw-r--   0 ester      (501) staff       (20)     4597 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js
+-rw-rw-r--   0 ester      (501) staff       (20)     3951 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/Webhook/ReportCard_Template_RECO.js
+-rw-rw-r--   0 ester      (501) staff       (20)     9491 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/Webhook/index_template_LEARN.js
+-rw-rw-r--   0 ester      (501) staff       (20)    12453 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/Webhook/index_template_RECO.js
+-rw-rw-r--   0 ester      (501) staff       (20)      720 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/Webhook/package.json
+-rw-rw-r--   0 ester      (501) staff       (20)       18 2024-04-18 09:57:34.000000 TPE-Bot-6.8.4/buildABot/Data/__init__.py
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.337916 TPE-Bot-6.8.4/buildABot/QA/
+-rw-rw-r--   0 ester      (501) staff       (20)    10471 2024-04-18 10:09:00.000000 TPE-Bot-6.8.4/buildABot/QA/DataBank.py
+-rw-rw-r--   0 ester      (501) staff       (20)     6603 2024-04-18 10:09:00.000000 TPE-Bot-6.8.4/buildABot/QA/Para.py
+-rw-rw-r--   0 ester      (501) staff       (20)    16483 2024-04-18 10:09:00.000000 TPE-Bot-6.8.4/buildABot/QA/QAManager.py
+-rw-rw-r--   0 ester      (501) staff       (20)     5863 2024-04-18 10:09:00.000000 TPE-Bot-6.8.4/buildABot/QA/Responses.py
+-rw-rw-r--   0 ester      (501) staff       (20)     6375 2024-04-18 10:03:50.000000 TPE-Bot-6.8.4/buildABot/QAHelper.py
+-rw-rw-r--   0 ester      (501) staff       (20)     7919 2024-04-18 10:03:50.000000 TPE-Bot-6.8.4/buildABot/__init__.py
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.338121 TPE-Bot-6.8.4/buildABot/pytransform/
+-rw-rw-r--   0 ester      (501) staff       (20)    13587 2024-04-18 09:40:40.000000 TPE-Bot-6.8.4/buildABot/pytransform/__init__.py
+drwxr-xr-x   0 ester      (501) staff       (20)        0 2024-04-21 08:40:54.338959 TPE-Bot-6.8.4/parrot/
+-rwx------   0 ester      (501) staff       (20)       34 2023-03-23 19:45:54.000000 TPE-Bot-6.8.4/parrot/__init__.py
+-rwx------   0 ester      (501) staff       (20)      804 2023-03-23 19:45:54.000000 TPE-Bot-6.8.4/parrot/demo.py
+-rwx------   0 ester      (501) staff       (20)     6089 2023-03-23 19:45:54.000000 TPE-Bot-6.8.4/parrot/filters.py
+-rwx------   0 ester      (501) staff       (20)     5955 2023-03-23 19:45:54.000000 TPE-Bot-6.8.4/parrot/parrot.py
+-rw-r--r--   0 ester      (501) staff       (20)       38 2024-04-21 08:40:54.339522 TPE-Bot-6.8.4/setup.cfg
+-rwx------   0 ester      (501) staff       (20)      954 2024-04-21 08:40:07.000000 TPE-Bot-6.8.4/setup.py
```

### Comparing `TPE-Bot-6.8.3/README.md` & `TPE-Bot-6.8.4/README.md`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/TPE_Bot.egg-info/SOURCES.txt` & `TPE-Bot-6.8.4/TPE_Bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/BotController.py` & `TPE-Bot-6.8.4/buildABot/Bot/BotController.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/BotManager.py` & `TPE-Bot-6.8.4/buildABot/Bot/BotManager.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Dashboard/Analytics.py` & `TPE-Bot-6.8.4/buildABot/Bot/Dashboard/Analytics.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Dashboard/TelegramLogs.py` & `TPE-Bot-6.8.4/buildABot/Bot/Dashboard/TelegramLogs.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Dashboard/pytransform/__init__.py` & `TPE-Bot-6.8.4/buildABot/Bot/Dashboard/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Firebase/Entities.py` & `TPE-Bot-6.8.4/buildABot/Bot/Firebase/Entities.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Firebase/Firebase_Learn.py` & `TPE-Bot-6.8.4/buildABot/Bot/Firebase/Firebase_Learn.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Firebase/Firebase_Reco.py` & `TPE-Bot-6.8.4/buildABot/Bot/Firebase/Firebase_Reco.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Firebase/Webhook_Learn.py` & `TPE-Bot-6.8.4/buildABot/Bot/Firebase/Webhook_Learn.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Firebase/Webhook_Reco.py` & `TPE-Bot-6.8.4/buildABot/Bot/Firebase/Webhook_Reco.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Firebase/pytransform/__init__.py` & `TPE-Bot-6.8.4/buildABot/Bot/Firebase/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/CustomIntents.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/CustomIntents.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/CustomMenu.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/CustomMenu.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/CustomRecommendedMenu.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/CustomRecommendedMenu.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/CustomResponse.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/CustomResponse.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/CustomTeleResponse.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/CustomTeleResponse.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/DefaultIntent.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/DefaultIntent.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/FAQ.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/FAQ.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/FallbackSocialTag.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/FallbackSocialTag.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/Paraphraser.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/Paraphraser.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/RelatedIntents.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/RelatedIntents.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/Type/AccordionCard.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/Type/AccordionCard.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/Type/ButtonCard.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/Type/ButtonCard.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/Type/Chips.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/Type/Chips.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/Type/DescriptionCard.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/Type/DescriptionCard.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/Type/ImageCard.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/Type/ImageCard.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/Type/InfoCard.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/Type/InfoCard.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/Type/ListCard.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/Type/ListCard.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/Usersays.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/Usersays.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/WelcomeIntent.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/WelcomeIntent.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/Worksheets_Learn.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/Worksheets_Learn.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/Worksheets_Reco.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/Worksheets_Reco.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Intents/pytransform/__init__.py` & `TPE-Bot-6.8.4/buildABot/Bot/Intents/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Webapp/WebApp_Learn.py` & `TPE-Bot-6.8.4/buildABot/Bot/Webapp/WebApp_Learn.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Webapp/WebApp_Reco.py` & `TPE-Bot-6.8.4/buildABot/Bot/Webapp/WebApp_Reco.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/Webapp/pytransform/__init__.py` & `TPE-Bot-6.8.4/buildABot/Bot/Webapp/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/WriteToFile.py` & `TPE-Bot-6.8.4/buildABot/Bot/WriteToFile.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Bot/pytransform/__init__.py` & `TPE-Bot-6.8.4/buildABot/Bot/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/BotHelper.py` & `TPE-Bot-6.8.4/buildABot/BotHelper.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Default Welcome Intent - Telegram - Check Submission.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Default Welcome Intent - Telegram - Check Submission.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Default Welcome Intent - Web - Fallback.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Default Welcome Intent - Web - Fallback.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Default Welcome Intent - Web.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Default Welcome Intent - Web.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Downvote.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Downvote.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Downvote_usersays_en.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Downvote_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Email Enquiry.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Email Enquiry.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Email Enquiry_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Exit Conversation.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Exit Conversation.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Exit Conversation_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Fallback - no.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Fallback - no.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Fallback - no_usersays_en.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Fallback - no_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Fallback - yes - fallback.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Fallback - yes - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Fallback - yes.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Fallback - yes.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Fallback - yes_usersays_en.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Fallback - yes_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Fallback.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Fallback.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login - Remember Name.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login - Remember Name.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Login_usersays_en.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Login_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Thankyou.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Thankyou.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Thankyou_usersays_en.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Thankyou_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Learn/Upvote.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Learn/Upvote.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Default Welcome Intent - Telegram - Check Submission.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Default Welcome Intent - Telegram - Check Submission.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Default Welcome Intent - Web - Fallback.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Default Welcome Intent - Web - Fallback.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Default Welcome Intent - Web.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Default Welcome Intent - Web.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Downvote.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Downvote.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Downvote_usersays_en.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Downvote_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Email Enquiry.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Email Enquiry.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Email Enquiry_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Exit Conversation.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Exit Conversation.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Exit Conversation_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Log In.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Log In.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Fallback - no.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Fallback - no.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Fallback - no_usersays_en.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Fallback - no_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Fallback - yes - fallback.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Fallback - yes - fallback.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Fallback - yes.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Fallback - yes.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Fallback - yes_usersays_en.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Fallback - yes_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Fallback.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Fallback.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login - Remember Name.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login - Remember Name.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Login_usersays_en.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Login_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Menu - Main.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Menu - Main.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Menu - Main_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Thankyou.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Thankyou.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Thankyou_usersays_en.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Default - Recommended/Upvote.json` & `TPE-Bot-6.8.4/buildABot/Data/Default - Recommended/Upvote.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/WebApp/index_template_LEARN.html` & `TPE-Bot-6.8.4/buildABot/Data/WebApp/index_template_LEARN.html`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/WebApp/index_template_RECO.html` & `TPE-Bot-6.8.4/buildABot/Data/WebApp/index_template_RECO.html`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/WebApp/reset_template_RECO.js` & `TPE-Bot-6.8.4/buildABot/Data/WebApp/reset_template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Webhook/CheckPwd_Template_RECO.js` & `TPE-Bot-6.8.4/buildABot/Data/Webhook/CheckPwd_Template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js` & `TPE-Bot-6.8.4/buildABot/Data/Webhook/RecommendedMenu_Template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Webhook/ReportCard_Template_RECO.js` & `TPE-Bot-6.8.4/buildABot/Data/Webhook/ReportCard_Template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Webhook/index_template_LEARN.js` & `TPE-Bot-6.8.4/buildABot/Data/Webhook/index_template_LEARN.js`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Webhook/index_template_RECO.js` & `TPE-Bot-6.8.4/buildABot/Data/Webhook/index_template_RECO.js`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/Data/Webhook/package.json` & `TPE-Bot-6.8.4/buildABot/Data/Webhook/package.json`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/QA/DataBank.py` & `TPE-Bot-6.8.4/buildABot/QA/DataBank.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/QA/Para.py` & `TPE-Bot-6.8.4/buildABot/QA/Para.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/QA/QAManager.py` & `TPE-Bot-6.8.4/buildABot/QA/QAManager.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/QA/Responses.py` & `TPE-Bot-6.8.4/buildABot/QA/Responses.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/QAHelper.py` & `TPE-Bot-6.8.4/buildABot/QAHelper.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/__init__.py` & `TPE-Bot-6.8.4/buildABot/__init__.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/buildABot/pytransform/__init__.py` & `TPE-Bot-6.8.4/buildABot/pytransform/__init__.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/parrot/demo.py` & `TPE-Bot-6.8.4/parrot/demo.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/parrot/filters.py` & `TPE-Bot-6.8.4/parrot/filters.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/parrot/parrot.py` & `TPE-Bot-6.8.4/parrot/parrot.py`

 * *Files identical despite different names*

### Comparing `TPE-Bot-6.8.3/setup.py` & `TPE-Bot-6.8.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="TPE-Bot", # Replace with your own username
-    version="6.8.3",
+    version="6.8.4",
     author="Ester Goh",
     description="A TPEdu All-in-one Chatbot Package",
     packages=setuptools.find_packages(),
     package_data={'': ['Bot/*.py','Bot/*/*.py', 'Bot/*/*/*.py', 'Data/*/*.js', 'Data/*/*.html', 'Data/*/*.json', 'QA/*.py']},
     include_package_data=True,
     install_requires=[
         'pandas',
```

