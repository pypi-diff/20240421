# Comparing `tmp/youtube-comment-downloader-0.1.72.tar.gz` & `tmp/youtube_comment_downloader-0.1.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube-comment-downloader-0.1.72.tar", last modified: Sun Apr  7 18:58:51 2024, max compression
+gzip compressed data, was "youtube_comment_downloader-0.1.73.tar", last modified: Sun Apr 21 10:14:52 2024, max compression
```

## Comparing `youtube-comment-downloader-0.1.72.tar` & `youtube_comment_downloader-0.1.73.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:58:51.895699 youtube-comment-downloader-0.1.72/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-07 18:58:44.000000 youtube-comment-downloader-0.1.72/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-07 18:58:51.895699 youtube-comment-downloader-0.1.72/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-07 18:58:44.000000 youtube-comment-downloader-0.1.72/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-07 18:58:44.000000 youtube-comment-downloader-0.1.72/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-07 18:58:51.895699 youtube-comment-downloader-0.1.72/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 18:58:44.000000 youtube-comment-downloader-0.1.72/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:58:51.895699 youtube-comment-downloader-0.1.72/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-07 18:58:44.000000 youtube-comment-downloader-0.1.72/tests/test_search_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:58:51.895699 youtube-comment-downloader-0.1.72/youtube_comment_downloader/
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-07 18:58:44.000000 youtube-comment-downloader-0.1.72/youtube_comment_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-07 18:58:44.000000 youtube-comment-downloader-0.1.72/youtube_comment_downloader/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7475 2024-04-07 18:58:44.000000 youtube-comment-downloader-0.1.72/youtube_comment_downloader/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:58:51.895699 youtube-comment-downloader-0.1.72/youtube_comment_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-07 18:58:51.000000 youtube-comment-downloader-0.1.72/youtube_comment_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-07 18:58:51.000000 youtube-comment-downloader-0.1.72/youtube_comment_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:58:51.000000 youtube-comment-downloader-0.1.72/youtube_comment_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-07 18:58:51.000000 youtube-comment-downloader-0.1.72/youtube_comment_downloader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-07 18:58:51.000000 youtube-comment-downloader-0.1.72/youtube_comment_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-07 18:58:51.000000 youtube-comment-downloader-0.1.72/youtube_comment_downloader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:14:52.160450 youtube_comment_downloader-0.1.73/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-21 10:14:39.000000 youtube_comment_downloader-0.1.73/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-21 10:14:52.160450 youtube_comment_downloader-0.1.73/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-21 10:14:39.000000 youtube_comment_downloader-0.1.73/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-21 10:14:39.000000 youtube_comment_downloader-0.1.73/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-21 10:14:52.160450 youtube_comment_downloader-0.1.73/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 10:14:39.000000 youtube_comment_downloader-0.1.73/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:14:52.156450 youtube_comment_downloader-0.1.73/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-21 10:14:39.000000 youtube_comment_downloader-0.1.73/tests/test_search_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:14:52.160450 youtube_comment_downloader-0.1.73/youtube_comment_downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-21 10:14:39.000000 youtube_comment_downloader-0.1.73/youtube_comment_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-21 10:14:39.000000 youtube_comment_downloader-0.1.73/youtube_comment_downloader/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8006 2024-04-21 10:14:39.000000 youtube_comment_downloader-0.1.73/youtube_comment_downloader/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 10:14:52.160450 youtube_comment_downloader-0.1.73/youtube_comment_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-21 10:14:52.000000 youtube_comment_downloader-0.1.73/youtube_comment_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-21 10:14:52.000000 youtube_comment_downloader-0.1.73/youtube_comment_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 10:14:52.000000 youtube_comment_downloader-0.1.73/youtube_comment_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-21 10:14:52.000000 youtube_comment_downloader-0.1.73/youtube_comment_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-21 10:14:52.000000 youtube_comment_downloader-0.1.73/youtube_comment_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-21 10:14:52.000000 youtube_comment_downloader-0.1.73/youtube_comment_downloader.egg-info/top_level.txt
```

### Comparing `youtube-comment-downloader-0.1.72/LICENSE` & `youtube_comment_downloader-0.1.73/LICENSE`

 * *Files identical despite different names*

### Comparing `youtube-comment-downloader-0.1.72/PKG-INFO` & `youtube_comment_downloader-0.1.73/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube-comment-downloader
-Version: 0.1.72
+Version: 0.1.73
 Summary: Simple script for downloading Youtube comments without using the Youtube API
 Home-page: https://github.com/egbertbouman/youtube-comment-downloader
 Author: Egbert Bouman
 Author-email: ebouman@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
```

### Comparing `youtube-comment-downloader-0.1.72/README.md` & `youtube_comment_downloader-0.1.73/README.md`

 * *Files identical despite different names*

### Comparing `youtube-comment-downloader-0.1.72/setup.cfg` & `youtube_comment_downloader-0.1.73/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = youtube-comment-downloader
-version = 0.1.72
+version = 0.1.73
 description = Simple script for downloading Youtube comments without using the Youtube API
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license-file = LICENSE
 url = https://github.com/egbertbouman/youtube-comment-downloader
 author = Egbert Bouman
```

### Comparing `youtube-comment-downloader-0.1.72/tests/test_search_dict.py` & `youtube_comment_downloader-0.1.73/tests/test_search_dict.py`

 * *Files identical despite different names*

### Comparing `youtube-comment-downloader-0.1.72/youtube_comment_downloader/__init__.py` & `youtube_comment_downloader-0.1.73/youtube_comment_downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `youtube-comment-downloader-0.1.72/youtube_comment_downloader/downloader.py` & `youtube_comment_downloader-0.1.73/youtube_comment_downloader/downloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,45 +101,50 @@
                                               'shorts-engagement-panel-comments-section']:
                         # Process continuations for comments and replies.
                         continuations[:0] = [ep for ep in self.search_dict(item, 'continuationEndpoint')]
                     if action['targetId'].startswith('comment-replies-item') and 'continuationItemRenderer' in item:
                         # Process the 'Show more replies' button
                         continuations.append(next(self.search_dict(item, 'buttonRenderer'))['command'])
 
+            surface_payloads = self.search_dict(response, 'commentSurfaceEntityPayload')
+            payments = {payload['key']: next(self.search_dict(payload, 'simpleText'), '')
+                        for payload in surface_payloads if 'pdgCommentChip' in payload}
+            if payments:
+                # We need to map the payload keys to the comment IDs.
+                view_models = [vm['commentViewModel'] for vm in self.search_dict(response, 'commentViewModel')]
+                surface_keys = {vm['commentSurfaceKey']: vm['commentId']
+                                for vm in view_models if 'commentSurfaceKey' in vm}
+                payments = {surface_keys[key]: payment for key, payment in payments.items() if key in surface_keys}
+
             toolbar_payloads = self.search_dict(response, 'engagementToolbarStateEntityPayload')
-            toolbar_states = {payloads['key']:payloads for payloads in toolbar_payloads}
+            toolbar_states = {payload['key']: payload for payload in toolbar_payloads}
             for comment in reversed(list(self.search_dict(response, 'commentEntityPayload'))):
                 properties = comment['properties']
+                cid = properties['commentId']
                 author = comment['author']
                 toolbar = comment['toolbar']
                 toolbar_state = toolbar_states[properties['toolbarStateKey']]
-                result = {'cid': properties['commentId'],
+                result = {'cid': cid,
                           'text': properties['content']['content'],
                           'time': properties['publishedTime'],
                           'author': author['displayName'],
                           'channel': author['channelId'],
                           'votes': toolbar['likeCountLiked'],
                           'replies': toolbar['replyCount'],
                           'photo': author['avatarThumbnailUrl'],
                           'heart': toolbar_state.get('heartState', '') == 'TOOLBAR_HEART_STATE_HEARTED',
-                          'reply': '.' in properties['commentId']}
+                          'reply': '.' in cid}
 
                 try:
                     result['time_parsed'] = dateparser.parse(result['time'].split('(')[0].strip()).timestamp()
                 except AttributeError:
                     pass
 
-                paid = (
-                    comment.get('paidCommentChipRenderer', {})
-                    .get('pdgCommentChipRenderer', {})
-                    .get('chipText', {})
-                    .get('simpleText')
-                )
-                if paid:
-                    result['paid'] = paid
+                if cid in payments:
+                    result['paid'] = payments[cid]
 
                 yield result
             time.sleep(sleep)
 
     @staticmethod
     def regex_search(text, pattern, group=1, default=None):
         match = re.search(pattern, text)
```

### Comparing `youtube-comment-downloader-0.1.72/youtube_comment_downloader.egg-info/PKG-INFO` & `youtube_comment_downloader-0.1.73/youtube_comment_downloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube-comment-downloader
-Version: 0.1.72
+Version: 0.1.73
 Summary: Simple script for downloading Youtube comments without using the Youtube API
 Home-page: https://github.com/egbertbouman/youtube-comment-downloader
 Author: Egbert Bouman
 Author-email: ebouman@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
```

