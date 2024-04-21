# Comparing `tmp/fuo_qqmusic-1.0.2.tar.gz` & `tmp/fuo_qqmusic-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuo_qqmusic-1.0.2.tar", last modified: Mon Mar  4 10:31:20 2024, max compression
+gzip compressed data, was "fuo_qqmusic-1.0.3.tar", last modified: Sun Apr 21 10:31:31 2024, max compression
```

## Comparing `fuo_qqmusic-1.0.2.tar` & `fuo_qqmusic-1.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:31:20.354940 fuo_qqmusic-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-04 10:31:20.354940 fuo_qqmusic-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-03-04 10:31:18.000000 fuo_qqmusic-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:31:20.350939 fuo_qqmusic-1.0.2/fuo_qqmusic/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-04 10:31:18.000000 fuo_qqmusic-1.0.2/fuo_qqmusic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22322 2024-03-04 10:31:18.000000 fuo_qqmusic-1.0.2/fuo_qqmusic/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:31:20.354940 fuo_qqmusic-1.0.2/fuo_qqmusic/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-03-04 10:31:18.000000 fuo_qqmusic-1.0.2/fuo_qqmusic/assets/icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-04 10:31:18.000000 fuo_qqmusic-1.0.2/fuo_qqmusic/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-04 10:31:18.000000 fuo_qqmusic-1.0.2/fuo_qqmusic/excs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12908 2024-03-04 10:31:18.000000 fuo_qqmusic-1.0.2/fuo_qqmusic/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-03-04 10:31:18.000000 fuo_qqmusic-1.0.2/fuo_qqmusic/provider_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-03-04 10:31:18.000000 fuo_qqmusic-1.0.2/fuo_qqmusic/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 10:31:20.354940 fuo_qqmusic-1.0.2/fuo_qqmusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-04 10:31:20.000000 fuo_qqmusic-1.0.2/fuo_qqmusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-04 10:31:20.000000 fuo_qqmusic-1.0.2/fuo_qqmusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 10:31:20.000000 fuo_qqmusic-1.0.2/fuo_qqmusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-04 10:31:20.000000 fuo_qqmusic-1.0.2/fuo_qqmusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-04 10:31:20.000000 fuo_qqmusic-1.0.2/fuo_qqmusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-04 10:31:20.000000 fuo_qqmusic-1.0.2/fuo_qqmusic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 10:31:20.354940 fuo_qqmusic-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-04 10:31:18.000000 fuo_qqmusic-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:31:31.102727 fuo_qqmusic-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-21 10:31:31.102727 fuo_qqmusic-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:31:31.102727 fuo_qqmusic-1.0.3/fuo_qqmusic/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/fuo_qqmusic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23378 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/fuo_qqmusic/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:31:31.102727 fuo_qqmusic-1.0.3/fuo_qqmusic/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/fuo_qqmusic/assets/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/fuo_qqmusic/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/fuo_qqmusic/excs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14059 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/fuo_qqmusic/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/fuo_qqmusic/provider_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/fuo_qqmusic/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:31:31.102727 fuo_qqmusic-1.0.3/fuo_qqmusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-21 10:31:31.000000 fuo_qqmusic-1.0.3/fuo_qqmusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-21 10:31:31.000000 fuo_qqmusic-1.0.3/fuo_qqmusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 10:31:31.000000 fuo_qqmusic-1.0.3/fuo_qqmusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-21 10:31:31.000000 fuo_qqmusic-1.0.3/fuo_qqmusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-21 10:31:31.000000 fuo_qqmusic-1.0.3/fuo_qqmusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-21 10:31:31.000000 fuo_qqmusic-1.0.3/fuo_qqmusic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 10:31:31.102727 fuo_qqmusic-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-21 10:31:30.000000 fuo_qqmusic-1.0.3/setup.py
```

### Comparing `fuo_qqmusic-1.0.2/PKG-INFO` & `fuo_qqmusic-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuo_qqmusic
-Version: 1.0.2
+Version: 1.0.3
 Summary: feeluown qqmusic plugin
 Home-page: https://github.com/feeluown/feeluown-qqmusic
 Author: Cosven
 Author-email: yinshaowen241@gmail.com
 Keywords: feeluown,plugin,qqmusic
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `fuo_qqmusic-1.0.2/README.md` & `fuo_qqmusic-1.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 ## 使用说明
 
 ### 登录
 在网页登录微信/QQ后（在任意网站），复制请求中的 cookies 至程序登录框，
 [操作示例](https://github.com/feeluown/feeluown-qqmusic/issues/6)。
 
 ## changelog
+### 1.0.3 (2024-04-21)
+- 适配 feeluown 4.1.3 的新主页功能
+
 ### 1.0.2 (2024-03-04)
 - 修复获取歌单封面失败的问题 #21
 - 修复获取歌曲播放链接失败的问题 #20
 
 ### 1.0 (2024-01-1)
 - 使用 FeelUOwn 新接口
 - 支持发现，推荐等接口
```

### Comparing `fuo_qqmusic-1.0.2/fuo_qqmusic/__init__.py` & `fuo_qqmusic-1.0.3/fuo_qqmusic/__init__.py`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-1.0.2/fuo_qqmusic/api.py` & `fuo_qqmusic-1.0.3/fuo_qqmusic/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,14 +173,33 @@
         }
         js = self.rpc(payload)
         data_song = js['detail']['data']['track_info']
         if data_song['id'] <= 0:
             return None
         return data_song
 
+    def batch_song_details(self, song_ids):
+        """
+        song_ids should be a list of int
+        """
+        payload = {
+            'comm': self.get_wkv17_common_params(),
+            'req_0': {
+                'module': 'music.trackInfo.UniformRuleCtrl',
+                'method': 'CgiGetTrackInfo',
+                'param': {
+                    'ids': song_ids,
+                    'types': [200]*len(song_ids),
+                    'source': 'AiNoFree',
+                }
+            }
+        }
+        js = self.rpc(payload)
+        return js['req_0']['data']['tracks']
+
     def song_similar(self, song_id):
         payload = {
             "simsongs": {
                 "module": "rcmusic.similarSongRadioServer",
                 "method": "get_simsongs",
                 "param": {
                     "songid": song_id,
@@ -373,32 +392,32 @@
                 }
             },
         }
         js = self.rpc(data)
         playlist = js['recomPlaylist']
         return playlist['data']['v_hot']
 
-    def get_recommend_playlists_ids(self, index=0):
+    def get_recommend_feed(self, page=1):
+        # APIs are found in https://y.qq.com/wk_v17/#/recommend
         data = {
             'req_0': {
                 'module': 'recommend.RecommendFeedServer',
                 'method': 'get_recommend_feed',
                 'param': {
                     'direction': 0,
-                    'page': 1,
+                    'page': page,
                     'v_cache': [],
                     'v_uniq': [],
                     's_num': 0
                 }
             },
+            'comm': self.get_wkv17_common_params(),
         }
         js = self.rpc(data)
-        ids = [card['id']
-               for card in js['req_0']['data']['v_shelf'][index]['v_niche'][0]['v_card']]
-        return ids
+        return js['req_0']['data']
 
     def get_lyric_by_songmid(self, songmid):
         url = api_base_url + '/lyric/fcgi-bin/fcg_query_lyric_new.fcg'
         params = {
             'songmid': songmid,
             'pcachetime': int(round(time.time() * 1000)),
             'format': 'json',
@@ -422,14 +441,30 @@
         url = 'https://u.y.qq.com/cgi-bin/musicu.fcg'
         resp = requests.get(url, params=params, headers=self._headers,
                             cookies=self._cookies, timeout=self._timeout)
         js = resp.json()
         CodeShouldBe0.check(js)
         return js
 
+    def get_wkv17_common_params(self):
+        return {
+            # ct field is important, without this field,
+            # the req_0 result is completely different.
+            "ct": 20,
+            "cv": 1770,
+            'g_tk': 5381,
+            'uin': self._uin,
+            'format': 'json',
+            'inCharset': 'utf-8',
+            'outCharset': 'utf-8',
+            'platform': 'wk_v17',
+            'uid': '',
+            'guid': '',
+        }
+
     def get_common_params(self):
         return {
             'loginUin': self._uin,
             'hostUin': 0,
             'g_tk': self.get_token_from_cookies(),
             'inCharset': 'utf8',
             'outCharset': 'utf-8',
```

### Comparing `fuo_qqmusic-1.0.2/fuo_qqmusic/assets/icon.svg` & `fuo_qqmusic-1.0.3/fuo_qqmusic/assets/icon.svg`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-1.0.2/fuo_qqmusic/provider.py` & `fuo_qqmusic-1.0.3/fuo_qqmusic/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import logging
 from typing import List, Optional, Protocol
 from feeluown.excs import ModelNotFound
 from feeluown.library import (
     AbstractProvider,
+    BriefSongModel,
+    PlaylistModel,
+    Collection,
+    CollectionType,
     ProviderV2,
     ProviderFlags as PF,
     SupportsSongGet,
     SupportsSongMultiQuality,
     SupportsSongMV,
     VideoModel,
     LyricModel,
     SupportsCurrentUser,
     SupportsVideoGet,
     SupportsSongLyric,
     SupportsAlbumGet,
     SupportsArtistGet,
     SupportsPlaylistGet,
     SupportsPlaylistSongsReader,
+    SupportsRecACollectionOfSongs,
     SimpleSearchResult,
     SearchType,
     ModelType,
 )
 from feeluown.media import Media, Quality
 from feeluown.utils.reader import create_reader, SequentialReader
 from .api import API
@@ -38,14 +43,15 @@
     SupportsCurrentUser,
     SupportsVideoGet,
     SupportsSongLyric,
     SupportsAlbumGet,
     SupportsArtistGet,
     SupportsPlaylistGet,
     SupportsPlaylistSongsReader,
+    SupportsRecACollectionOfSongs,
     Protocol,
 ):
     pass
 
 
 class QQProvider(AbstractProvider, ProviderV2):
     class meta:
@@ -243,14 +249,39 @@
         playlists = self.api.recommend_playlists()
         for pl in playlists:
             pl["dissid"] = pl["content_id"]
             pl["dissname"] = pl["title"]
             pl["logo"] = pl["cover"]
         return [_deserialize(playlist, QQPlaylistSchema) for playlist in playlists]
 
+    def rec_a_collection_of_songs(self):
+        # TODO: cache API result
+        feed = self.api.get_recommend_feed()
+        shelf = None
+        for shelf in feed['v_shelf']:
+            # I guess 10046 means 'song'.
+            if shelf['miscellany'].get('jumptype') == 10046:
+                shelf = shelf
+        if shelf is None:
+            return '', []
+        title = shelf['title_content'] or shelf['title_template']
+        song_ids = []
+        for batch in shelf['v_niche']:
+            for card in batch['v_card']:
+                if card['jumptype'] == 10046:
+                    song_id = int(card['id'])
+                    if song_id not in song_ids:
+                        song_ids.append(song_id)
+
+        tracks = self.api.batch_song_details(song_ids)
+        return Collection(name=title,
+                          type_=CollectionType.only_songs,
+                          models=[_deserialize(track, QQSongSchema) for track in tracks],
+                          description='')
+
     def current_user_get_radio_songs(self):
         songs_data = self.api.get_radio_music()
         return [_deserialize(s, QQSongSchema) for s in songs_data]
 
     def current_user_list_playlists(self):
         user = self.get_current_user()
         if user is None:
```

### Comparing `fuo_qqmusic-1.0.2/fuo_qqmusic/provider_ui.py` & `fuo_qqmusic-1.0.3/fuo_qqmusic/provider_ui.py`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-1.0.2/fuo_qqmusic/schemas.py` & `fuo_qqmusic-1.0.3/fuo_qqmusic/schemas.py`

 * *Files identical despite different names*

### Comparing `fuo_qqmusic-1.0.2/fuo_qqmusic.egg-info/PKG-INFO` & `fuo_qqmusic-1.0.3/fuo_qqmusic.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuo-qqmusic
-Version: 1.0.2
+Version: 1.0.3
 Summary: feeluown qqmusic plugin
 Home-page: https://github.com/feeluown/feeluown-qqmusic
 Author: Cosven
 Author-email: yinshaowen241@gmail.com
 Keywords: feeluown,plugin,qqmusic
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `fuo_qqmusic-1.0.2/setup.py` & `fuo_qqmusic-1.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from setuptools import setup
 
 
 setup(
     name='fuo_qqmusic',
-    version='1.0.2',
+    version='1.0.3',
     description='feeluown qqmusic plugin',
     author='Cosven',
     author_email='yinshaowen241@gmail.com',
     packages=[
         'fuo_qqmusic',
     ],
     package_data={
@@ -23,15 +23,15 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3 :: Only',
     ],
     install_requires=[
-        'feeluown>=4.0a0',
+        'feeluown>=4.1.3',
         'requests',
         'marshmallow>=3.0'
     ],
     entry_points={
         'fuo.plugins_v1': [
             'qqmusic = fuo_qqmusic',
         ]
```

