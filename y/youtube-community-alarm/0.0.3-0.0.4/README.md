# Comparing `tmp/youtube_community_alarm-0.0.3-py3-none-any.whl.zip` & `tmp/youtube_community_alarm-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,12 @@
-Zip file size: 6454 bytes, number of entries: 11
--rw-r--r--  2.0 unx      264 b- defN 24-Mar-25 07:42 youtubeCommunityAlarm/__init__.py
--rw-r--r--  2.0 unx     2179 b- defN 24-Mar-25 06:24 youtubeCommunityAlarm/crontab_register.py
--rw-r--r--  2.0 unx      669 b- defN 24-Mar-25 06:21 youtubeCommunityAlarm/test.py
--rw-r--r--  2.0 unx     2092 b- defN 24-Mar-26 08:06 youtubeCommunityAlarm/youtube_community.py
--rw-r--r--  2.0 unx     2019 b- defN 24-Mar-25 07:42 youtubeCommunityAlarm/youtube_community_alarm.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-22 02:39 youtubeCommunityAlarm/test/__init__.py
--rw-r--r--  2.0 unx     1603 b- defN 24-Mar-25 07:42 youtubeCommunityAlarm/test/test_youtube_community.py
--rw-r--r--  2.0 unx     1951 b- defN 24-Mar-27 01:02 youtube_community_alarm-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-27 01:02 youtube_community_alarm-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 24-Mar-27 01:02 youtube_community_alarm-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1039 b- defN 24-Mar-27 01:02 youtube_community_alarm-0.0.3.dist-info/RECORD
-11 files, 11930 bytes uncompressed, 4646 bytes compressed:  61.1%
+Zip file size: 6149 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      264 b- defN 24-Apr-07 04:08 youtubeCommunityAlarm/__init__.py
+-rw-r--r--  2.0 unx     2179 b- defN 24-Apr-07 04:08 youtubeCommunityAlarm/crontab_register.py
+-rw-r--r--  2.0 unx     2343 b- defN 24-Apr-21 06:08 youtubeCommunityAlarm/youtube_community.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-Apr-07 04:08 youtubeCommunityAlarm/youtube_community_alarm.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Mar-23 11:25 youtubeCommunityAlarm/test/__init__.py
+-rw-r--r--  2.0 unx     1603 b- defN 24-Apr-07 04:08 youtubeCommunityAlarm/test/test_youtube_community.py
+-rw-r--r--  2.0 unx     2011 b- defN 24-Apr-21 06:26 youtube_community_alarm-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-21 06:26 youtube_community_alarm-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 24-Apr-21 06:26 youtube_community_alarm-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      954 b- defN 24-Apr-21 06:26 youtube_community_alarm-0.0.4.dist-info/RECORD
+10 files, 11487 bytes uncompressed, 4475 bytes compressed:  61.0%
```

## zipnote {}

```diff
@@ -1,34 +1,31 @@
 Filename: youtubeCommunityAlarm/__init__.py
 Comment: 
 
 Filename: youtubeCommunityAlarm/crontab_register.py
 Comment: 
 
-Filename: youtubeCommunityAlarm/test.py
-Comment: 
-
 Filename: youtubeCommunityAlarm/youtube_community.py
 Comment: 
 
 Filename: youtubeCommunityAlarm/youtube_community_alarm.py
 Comment: 
 
 Filename: youtubeCommunityAlarm/test/__init__.py
 Comment: 
 
 Filename: youtubeCommunityAlarm/test/test_youtube_community.py
 Comment: 
 
-Filename: youtube_community_alarm-0.0.3.dist-info/METADATA
+Filename: youtube_community_alarm-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: youtube_community_alarm-0.0.3.dist-info/WHEEL
+Filename: youtube_community_alarm-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: youtube_community_alarm-0.0.3.dist-info/top_level.txt
+Filename: youtube_community_alarm-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: youtube_community_alarm-0.0.3.dist-info/RECORD
+Filename: youtube_community_alarm-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## youtubeCommunityAlarm/youtube_community.py

```diff
@@ -2,48 +2,57 @@
 import json
 import re
 from retry import retry
 from requests.exceptions import SSLError
 from urllib3.exceptions import MaxRetryError
 
 BASE_URL = "https://www.youtube.com/"
+COMMUNITY = "커뮤니티"
+COMMUNITY_TAB_NUMBER = -2   # 뒤에서 두번째 tab
 REGEX = {
     "YT_INITIAL_DATA": "ytInitialData = ({(?:(?:.|\n)*)?});</script>",
     "HOUR_TIME_PATTERN": r'(\d+)\s*시간\s*전',
     "MINUTE_TIME_PATTERN": r'(\d+)\s*분\s*전',
 }
 
+
 class YoutubeCommunity:
     def __init__(self, channel_id):
         self.channel_id = channel_id
 
+    def find_community_tab(self, tabs) -> dict:
+        for tab in tabs:
+            if tab['tabRenderer']['title'] == COMMUNITY:
+                return tab
+
+        return {}
+
     @retry((SSLError, MaxRetryError), tries=3, delay=2)
     def get_all_posts_with_time(self):
         response = requests.get(f"{BASE_URL + self.channel_id}/community")
         posts_with_time = []
         if response.status_code == 200:
             m = re.findall(REGEX["YT_INITIAL_DATA"], response.text)
             if m:
                 json_data = json.loads(m[0])
             else:
                 print("Regular expression did not match any content in the response text.")
                 return []
 
             tabs = json_data['contents']['twoColumnBrowseResultsRenderer']['tabs']
-            posts = []
-            for tab in tabs:
-                try:
-                    posts = tab['tabRenderer']['content']['sectionListRenderer']['contents'][0]['itemSectionRenderer'][
-                        'contents']
-                except KeyError:
-                    pass
+            tab = tabs[COMMUNITY_TAB_NUMBER]
+
+            if tab['tabRenderer']['title'] != COMMUNITY:
+                tab = self.find_community_tab(tabs)
 
+            posts = tab['tabRenderer']['content']['sectionListRenderer']['contents'][0]['itemSectionRenderer']['contents']
             if not posts:
                 print("No posts found.")
                 return
+
             for post in posts:
                 try:
                     back_stage_post_renderer = post["backstagePostThreadRenderer"]["post"]['backstagePostRenderer']
                     text = back_stage_post_renderer["contentText"]["runs"][0]["text"]
                     time = back_stage_post_renderer["publishedTimeText"]["runs"][0]["text"]
                     posts_with_time.append((time, text))
                 except KeyError:
```

## Comparing `youtube_community_alarm-0.0.3.dist-info/METADATA` & `youtube_community_alarm-0.0.4.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: youtube-community-alarm
-Version: 0.0.3
+Version: 0.0.4
 Summary: youtube community alarm package
 Home-page: https://github.com/SionByeon/YoutubeCommunityAlarm
 Author: palace
 Author-email: ufo3764@naver.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
-# Youtube Community Alarm
+# Youtube Community Alarm ([pypi](https://pypi.org/project/youtube-community-alarm/))
 
 - Python3 interface for scheduling crontab to retrieve YouTube community posts and send notifications
 - Periodically check for new posts, and if any are found, send a notification to macOS.
 
 
 ## Installing
 install youtube-community-alarm
```

## Comparing `youtube_community_alarm-0.0.3.dist-info/RECORD` & `youtube_community_alarm-0.0.4.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 youtubeCommunityAlarm/__init__.py,sha256=Pmyg3Pq7EXt2jga0LURGbUIsQXm6PQEgEYGjm0Aqe-U,264
 youtubeCommunityAlarm/crontab_register.py,sha256=QQISMReI7wZzO_ZITLogbGS4ppLD97l6SDQO6Fr458w,2179
-youtubeCommunityAlarm/test.py,sha256=Wavto8getkQ8ub1zj3P3EyM0o_-hKpmI-MEqzFPneK8,669
-youtubeCommunityAlarm/youtube_community.py,sha256=Bc8jm-IJS3b7gnmG5oMt94Argni1O_grv_ad2x00g1o,2092
+youtubeCommunityAlarm/youtube_community.py,sha256=XrBZZiK077pZgoePGb_h4bUNG0-zOdBtn-9pIfDmlkw,2343
 youtubeCommunityAlarm/youtube_community_alarm.py,sha256=1f7VCWPE4EgszLciFU8v3WciwhcjHRlLGzbWiMTKpJk,2019
 youtubeCommunityAlarm/test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 youtubeCommunityAlarm/test/test_youtube_community.py,sha256=s9T0X7oQAR_9SMxmFle6Kr5rA6Zx9RZlGYHY6jTDxzg,1603
-youtube_community_alarm-0.0.3.dist-info/METADATA,sha256=WRoG28-jjo1wBKiURr313vj8cq0fRELNhYBjK3wYzjU,1951
-youtube_community_alarm-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-youtube_community_alarm-0.0.3.dist-info/top_level.txt,sha256=ikdTj4ZIJ98pw63ycO2_unqfjaMFTlWgLDSfxM7kYLY,22
-youtube_community_alarm-0.0.3.dist-info/RECORD,,
+youtube_community_alarm-0.0.4.dist-info/METADATA,sha256=g3IonMDmuRsbHKVPuZqfCV7DcfMXbcHP4zGqud73qAc,2011
+youtube_community_alarm-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+youtube_community_alarm-0.0.4.dist-info/top_level.txt,sha256=ikdTj4ZIJ98pw63ycO2_unqfjaMFTlWgLDSfxM7kYLY,22
+youtube_community_alarm-0.0.4.dist-info/RECORD,,
```

