# Comparing `tmp/PyPtt-1.2.5.tar.gz` & `tmp/pyptt-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPtt-1.2.5.tar", last modified: Thu Apr 11 07:30:01 2024, max compression
+gzip compressed data, was "pyptt-1.2.6.tar", last modified: Sun Apr 21 12:45:17 2024, max compression
```

## Comparing `PyPtt-1.2.5.tar` & `pyptt-1.2.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:30:01.368799 PyPtt-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-11 07:29:53.000000 PyPtt-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-11 07:29:53.000000 PyPtt-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-11 07:30:01.368799 PyPtt-1.2.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:30:01.368799 PyPtt-1.2.5/PyPtt/
--rw-r--r--   0 runner    (1001) docker     (127)    32091 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/PTT.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-11 07:30:01.000000 PyPtt-1.2.5/PyPtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_call_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_change_pw.py
--rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_del_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_get_board_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_get_board_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_get_bottom_post_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_get_favourite_board.py
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_get_newest_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    21214 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_get_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_get_post_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_get_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_give_money.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_has_new_mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_loginout.py
--rw-r--r--   0 runner    (1001) docker     (127)     9661 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_mark_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_reply_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_search_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_set_board_title.py
--rw-r--r--   0 runner    (1001) docker     (127)    15951 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/_api_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/check_value.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14101 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/connect_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/data_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/i18n.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:30:01.368799 PyPtt-1.2.5/PyPtt/lang/
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/lang/en_US.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/lang/zh_TW.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/lib_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    54872 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/screens.py
--rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:30:01.368799 PyPtt-1.2.5/PyPtt/ssl/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/ssl/cert.pem
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-11 07:29:53.000000 PyPtt-1.2.5/PyPtt/ssl/key.pem
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 07:30:01.368799 PyPtt-1.2.5/PyPtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-11 07:30:01.000000 PyPtt-1.2.5/PyPtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-11 07:30:01.000000 PyPtt-1.2.5/PyPtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 07:30:01.000000 PyPtt-1.2.5/PyPtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-11 07:30:01.000000 PyPtt-1.2.5/PyPtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 07:30:01.000000 PyPtt-1.2.5/PyPtt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-11 07:29:53.000000 PyPtt-1.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 07:30:01.368799 PyPtt-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-11 07:29:53.000000 PyPtt-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:45:17.113764 pyptt-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-21 12:45:07.000000 pyptt-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-21 12:45:07.000000 pyptt-1.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-21 12:45:17.113764 pyptt-1.2.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:45:17.113764 pyptt-1.2.6/PyPtt/
+-rw-r--r--   0 runner    (1001) docker     (127)    32101 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/PTT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-21 12:45:17.000000 pyptt-1.2.6/PyPtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_call_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_change_pw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7012 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_del_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_get_board_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_get_board_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_get_bottom_post_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_get_favourite_board.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_get_newest_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21214 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_get_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_get_post_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_get_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_give_money.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_has_new_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7852 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_loginout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4455 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_mark_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3733 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_reply_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_search_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_set_board_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15951 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/_api_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/check_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14101 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/connect_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5042 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/i18n.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:45:17.113764 pyptt-1.2.6/PyPtt/lang/
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/lang/en_US.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/lang/zh_TW.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/lib_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54872 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/screens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4672 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:45:17.113764 pyptt-1.2.6/PyPtt/ssl/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/ssl/cert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-21 12:45:07.000000 pyptt-1.2.6/PyPtt/ssl/key.pem
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 12:45:17.113764 pyptt-1.2.6/PyPtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-04-21 12:45:17.000000 pyptt-1.2.6/PyPtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-21 12:45:17.000000 pyptt-1.2.6/PyPtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 12:45:17.000000 pyptt-1.2.6/PyPtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-21 12:45:17.000000 pyptt-1.2.6/PyPtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-21 12:45:17.000000 pyptt-1.2.6/PyPtt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-21 12:45:07.000000 pyptt-1.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 12:45:17.113764 pyptt-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-21 12:45:07.000000 pyptt-1.2.6/setup.py
```

### Comparing `PyPtt-1.2.5/LICENSE` & `pyptt-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PKG-INFO` & `pyptt-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPtt
-Version: 1.2.5
+Version: 1.2.6
 Summary: PyPtt
 Home-page: https://pyptt.cc/
 Author: CodingMan
 Author-email: pttcodingman@gmail.com
 Keywords: PTT,crawler,bot,library,websockets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `PyPtt-1.2.5/PyPtt/PTT.py` & `pyptt-1.2.6/PyPtt/PTT.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,22 +348,22 @@
         """
         return _api_get_post.get_post(
             self, board, aid=aid, index=index, search_type=search_type, search_condition=search_condition,
             search_list=search_list, query=query)
 
     def get_newest_index(self, index_type: data_type.NewIndex, board: Optional[str] = None,
                          search_type: Optional[data_type.SearchType] = None, search_condition: Optional[str] = None,
-                         search_list: Optional[List[Tuple[Any | str]]] = None, ) -> int:
+                         search_list: Optional[List[Tuple[Any, str]]] = None) -> int:
         """
         取得最新文章或信箱編號。
 
         Args:
             index_type (:ref:`new-index`): 編號類型。
             board (str): 看板名稱。
-            search_list (List[str]): 搜尋清單。
+            search_list (List[Tuple[Any | str]]): 搜尋清單。
 
         Returns:
             int，最新文章或信箱編號。
 
         Raises:
             RequireLogin: 需要登入。
             NoSuchBoard: 看板不存在。
```

### Comparing `PyPtt-1.2.5/PyPtt/_api_bucket.py` & `pyptt-1.2.6/PyPtt/_api_bucket.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_call_status.py` & `pyptt-1.2.6/PyPtt/_api_call_status.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_change_pw.py` & `pyptt-1.2.6/PyPtt/_api_change_pw.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_comment.py` & `pyptt-1.2.6/PyPtt/_api_comment.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_del_post.py` & `pyptt-1.2.6/PyPtt/_api_del_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_get_board_info.py` & `pyptt-1.2.6/PyPtt/_api_get_board_info.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_get_board_list.py` & `pyptt-1.2.6/PyPtt/_api_get_board_list.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_get_bottom_post_list.py` & `pyptt-1.2.6/PyPtt/_api_get_bottom_post_list.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_get_favourite_board.py` & `pyptt-1.2.6/PyPtt/_api_get_favourite_board.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_get_newest_index.py` & `pyptt-1.2.6/PyPtt/_api_get_newest_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import re
-from typing import Optional
+from typing import Optional, Any, List, Tuple
 
 from . import _api_util
 from . import check_value
 from . import command
 from . import connect_core
 from . import data_type, lib_util
 from . import exceptions
@@ -51,15 +51,15 @@
         raise exceptions.UnknownError('UnknownError')
 
     return newest_index
 
 
 def get_newest_index(api, index_type: data_type.NewIndex, board: Optional[str] = None,
                      search_type: data_type.SearchType = None, search_condition: Optional[str] = None,
-                     search_list: Optional[list] = None) -> int:
+                     search_list: Optional[List[Tuple[Any, str]]] = None) -> int:
     _api_util.one_thread(api)
 
     if not api._is_login:
         raise exceptions.RequireLogin(i18n.require_login)
 
     if search_list is None:
         search_list = []
```

### Comparing `PyPtt-1.2.5/PyPtt/_api_get_post.py` & `pyptt-1.2.6/PyPtt/_api_get_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_get_post_index.py` & `pyptt-1.2.6/PyPtt/_api_get_post_index.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_get_time.py` & `pyptt-1.2.6/PyPtt/_api_get_time.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_get_user.py` & `pyptt-1.2.6/PyPtt/_api_get_user.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_give_money.py` & `pyptt-1.2.6/PyPtt/_api_give_money.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_has_new_mail.py` & `pyptt-1.2.6/PyPtt/_api_has_new_mail.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_loginout.py` & `pyptt-1.2.6/PyPtt/_api_loginout.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_mail.py` & `pyptt-1.2.6/PyPtt/_api_mail.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,14 +177,16 @@
 
     # 使用表示式分析信件作者
     pattern_result = mail_author_pattern.search(origin_mail)
     if pattern_result is None:
         mail_author = None
     else:
         mail_author = pattern_result.group(0)[2:].strip()
+        if '看板' in mail_author:
+            mail_author = mail_author[:mail_author.find('看板')].strip()
 
     # 使用表示式分析信件標題
     pattern_result = mail_title_pattern.search(origin_mail)
     if pattern_result is None:
         mail_title = None
     else:
         mail_title = pattern_result.group(0)[2:].strip()
```

### Comparing `PyPtt-1.2.5/PyPtt/_api_mark_post.py` & `pyptt-1.2.6/PyPtt/_api_mark_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_post.py` & `pyptt-1.2.6/PyPtt/_api_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_reply_post.py` & `pyptt-1.2.6/PyPtt/_api_reply_post.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_search_user.py` & `pyptt-1.2.6/PyPtt/_api_search_user.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_set_board_title.py` & `pyptt-1.2.6/PyPtt/_api_set_board_title.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/_api_util.py` & `pyptt-1.2.6/PyPtt/_api_util.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/check_value.py` & `pyptt-1.2.6/PyPtt/check_value.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/command.py` & `pyptt-1.2.6/PyPtt/command.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/config.py` & `pyptt-1.2.6/PyPtt/config.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/connect_core.py` & `pyptt-1.2.6/PyPtt/connect_core.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/data_type.py` & `pyptt-1.2.6/PyPtt/data_type.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/exceptions.py` & `pyptt-1.2.6/PyPtt/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/i18n.py` & `pyptt-1.2.6/PyPtt/i18n.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/lang/en_US.yaml` & `pyptt-1.2.6/PyPtt/lang/en_US.yaml`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/lang/zh_TW.yaml` & `pyptt-1.2.6/PyPtt/lang/zh_TW.yaml`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/lib_util.py` & `pyptt-1.2.6/PyPtt/lib_util.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/log.py` & `pyptt-1.2.6/PyPtt/log.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/screens.py` & `pyptt-1.2.6/PyPtt/screens.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/service.py` & `pyptt-1.2.6/PyPtt/service.py`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt/ssl/cert.pem` & `pyptt-1.2.6/PyPtt/ssl/cert.pem`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/PyPtt.egg-info/PKG-INFO` & `pyptt-1.2.6/PyPtt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPtt
-Version: 1.2.5
+Version: 1.2.6
 Summary: PyPtt
 Home-page: https://pyptt.cc/
 Author: CodingMan
 Author-email: pttcodingman@gmail.com
 Keywords: PTT,crawler,bot,library,websockets
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
```

### Comparing `PyPtt-1.2.5/PyPtt.egg-info/SOURCES.txt` & `pyptt-1.2.6/PyPtt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/README.md` & `pyptt-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `PyPtt-1.2.5/setup.py` & `pyptt-1.2.6/setup.py`

 * *Files identical despite different names*

