# Comparing `tmp/asyncpraw_stubs-0.0.1.tar.gz` & `tmp/asyncpraw_stubs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncpraw_stubs-0.0.1.tar", max compression
+gzip compressed data, was "asyncpraw_stubs-0.0.2.tar", max compression
```

## Comparing `asyncpraw_stubs-0.0.1.tar` & `asyncpraw_stubs-0.0.2.tar`

### file list

```diff
@@ -1,37 +1,75 @@
--rw-r--r--   0        0        0     1071 2024-03-31 21:00:44.277324 asyncpraw_stubs-0.0.1/LICENSE
--rw-r--r--   0        0        0      271 2024-03-31 22:41:00.453411 asyncpraw_stubs-0.0.1/README.md
--rw-r--r--   0        0        0     2149 2024-04-01 05:37:02.153334 asyncpraw_stubs-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      106 2024-03-31 23:57:34.408635 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/__init__.pyi
--rw-r--r--   0        0        0        0 2024-03-31 21:24:14.125379 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/config.pyi
--rw-r--r--   0        0        0      166 2024-03-31 22:11:42.938962 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/const.pyi
--rw-r--r--   0        0        0       25 2024-03-31 22:19:54.788289 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/endpoints.pyi
--rw-r--r--   0        0        0     2494 2024-03-31 22:26:44.034061 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/exceptions.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/__init__.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/auth.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/base.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/comment_forest.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/front.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/helpers.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/inbox.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/list.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/listing.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/mod_action.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/mod_note.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/mod_notes.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/preferences.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/reddit.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/redditors.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/stylesheet.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/subreddits.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/trophy.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/user.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:02:58.661808 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/models/util.pyi
--rw-r--r--   0        0        0      693 2024-03-31 22:43:40.516544 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/objector.pyi
--rw-r--r--   0        0        0        0 2024-03-31 22:07:07.276459 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/py.typed
--rw-r--r--   0        0        0     4558 2024-04-01 04:58:20.470017 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/reddit.pyi
--rw-r--r--   0        0        0        0 2024-03-31 21:27:37.520269 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/util/__init__.pyi
--rw-r--r--   0        0        0      368 2024-04-01 04:57:51.638170 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/util/cache.pyi
--rw-r--r--   0        0        0      182 2024-04-01 04:57:26.582302 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/util/deprecated_args.pyi
--rw-r--r--   0        0        0      236 2024-04-01 04:53:07.487673 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/util/snake.pyi
--rw-r--r--   0        0        0     1849 2024-04-01 04:57:35.430256 asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/util/token_manager.pyi
--rw-r--r--   0        0        0     1248 1970-01-01 00:00:00.000000 asyncpraw_stubs-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/LICENSE
+-rw-r--r--   0        0        0      271 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/README.md
+-rw-r--r--   0        0        0     2190 2024-04-21 00:03:00.082766 asyncpraw_stubs-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      106 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/config.pyi
+-rw-r--r--   0        0        0      166 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/const.pyi
+-rw-r--r--   0        0        0       25 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/endpoints.pyi
+-rw-r--r--   0        0        0     2502 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/exceptions.pyi
+-rw-r--r--   0        0        0      380 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/auth.pyi
+-rw-r--r--   0        0        0      106 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/base.pyi
+-rw-r--r--   0        0        0       25 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/comment_forest.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/front.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/helpers.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/inbox.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/list.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/listing/__init__.pyi
+-rw-r--r--   0        0        0      202 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/listing/domain.py
+-rw-r--r--   0        0        0      192 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/listing/mixins/__init__.pyi
+-rw-r--r--   0        0        0      171 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/listing/mixins/base.pyi
+-rw-r--r--   0        0        0      175 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/listing/mixins/rising.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/listing.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/mod_action.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/mod_note.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/mod_notes.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/preferences.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/__init__.pyi
+-rw-r--r--   0        0        0     1006 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/base.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/collections.pyi
+-rw-r--r--   0        0        0     2048 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/comment.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/draft.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/emoji.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/inline_media.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/live.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/message.pyi
+-rw-r--r--   0        0        0     2305 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/mixins/__init__.pyi
+-rw-r--r--   0        0        0      329 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/mixins/editable.pyi
+-rw-r--r--   0        0        0      110 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/mixins/fullname.pyi
+-rw-r--r--   0        0        0      434 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/mixins/gildable.pyi
+-rw-r--r--   0        0        0      327 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/mixins/inboxable.pyi
+-rw-r--r--   0        0        0      184 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/mixins/inboxtoggleable.pyi
+-rw-r--r--   0        0        0      481 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/mixins/messageable.pyi
+-rw-r--r--   0        0        0      452 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/mixins/modnote.pyi
+-rw-r--r--   0        0        0      284 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/mixins/replyable.pyi
+-rw-r--r--   0        0        0      153 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/mixins/reportable.pyi
+-rw-r--r--   0        0        0      298 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/mixins/savable.pyi
+-rw-r--r--   0        0        0      276 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/mixins/votable.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/modmail.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/more.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/multi.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/poll.pyi
+-rw-r--r--   0        0        0       55 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/redditor.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/removal_reasons.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/rules.pyi
+-rw-r--r--   0        0        0       22 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/submission.pyi
+-rw-r--r--   0        0        0       21 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/subreddit.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/user_subreddit.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/widgets.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit/wikipage.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.282751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/reddit.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/redditors.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/stylesheet.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/subreddits.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/trophy.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/user.pyi
+-rw-r--r--   0        0        0      194 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/models/util.pyi
+-rw-r--r--   0        0        0      701 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/objector.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/py.typed
+-rw-r--r--   0        0        0     9310 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/reddit.pyi
+-rw-r--r--   0        0        0        0 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/util/__init__.pyi
+-rw-r--r--   0        0        0      368 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/util/cache.pyi
+-rw-r--r--   0        0        0      182 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/util/deprecated_args.pyi
+-rw-r--r--   0        0        0      236 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/util/snake.pyi
+-rw-r--r--   0        0        0     1772 2024-04-21 00:02:48.286751 asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/util/token_manager.pyi
+-rw-r--r--   0        0        0     1300 1970-01-01 00:00:00.000000 asyncpraw_stubs-0.0.2/PKG-INFO
```

### Comparing `asyncpraw_stubs-0.0.1/LICENSE` & `asyncpraw_stubs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncpraw_stubs-0.0.1/pyproject.toml` & `asyncpraw_stubs-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asyncpraw-stubs"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python stubs for AsyncPRAW, a python package that allows for simple access to Reddit's API asynchronously."
 authors = ["Yoshikage Kira"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "asyncpraw-stubs", from = "src" }]
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
@@ -26,14 +26,15 @@
 Readme = "https://github.com/isFakeAccount/asyncpraw-stubs/blob/master/README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 asyncpraw = "^7.7.1"
 asyncprawcore = "^2.4.0"
 typing-extensions = "^4.10.0"
+asyncprawcore-stubs = "^0.0.1"
 
 
 [tool.poetry.group.typing.dependencies]
 pyright = "^1.1.356"
 mypy = "^1.9.0"
 
 [tool.poetry.group.linting.dependencies]
@@ -72,8 +73,8 @@
 [tool.black]
 line-length = 160
 
 [tool.ruff]
 line-length = 160
 
 [tool.ruff.lint]
-select = ["E", "F", "I001", "I002"]
+select = ["E", "F", "I001", "I002", "TID252"]
```

### Comparing `asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/exceptions.pyi` & `asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/exceptions.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 class RedditErrorItem:
     error_type: str
     message: Union[str, None]
     field: Union[str, None]
 
     @property
     def error_message(self) -> str: ...
-    def __eq__(self, other: Union["RedditErrorItem", list[str]]) -> bool: ...
+    def __eq__(self, other: Union["RedditErrorItem", list[str], object]) -> bool: ...
     def __init__(
         self,
         error_type: str,
         *,
         field: Union[str, None] = None,
         message: Union[str, None] = None,
     ) -> None: ...
```

### Comparing `asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/objector.pyi` & `asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/objector.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 from typing import TYPE_CHECKING, Any, NoReturn
 
 from .exceptions import RedditAPIException
 
 if TYPE_CHECKING:
     import asyncpraw
-
-    from .models.reddit.base import RedditBase
+    from asyncpraw.models.reddit.base import RedditBase
 
 class Objector:
     @classmethod
     def check_error(cls, data: list[Any] | dict[str, dict[str, str]]) -> NoReturn: ...
     @classmethod
     def parse_error(cls, data: list[Any] | dict[str, dict[str, str]]) -> RedditAPIException | None: ...
     def __init__(self, reddit: asyncpraw.Reddit, parsers: dict[str, Any] | None = None) -> None: ...
```

### Comparing `asyncpraw_stubs-0.0.1/src/asyncpraw-stubs/util/token_manager.pyi` & `asyncpraw_stubs-0.0.2/src/asyncpraw-stubs/util/token_manager.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -15,32 +15,32 @@
 
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     import aiosqlite
     import asyncpraw
-    import asyncprawcore
+    from asyncprawcore.auth import BaseAuthorizer
 
 class BaseTokenManager(ABC):
     @abstractmethod
-    def post_refresh_callback(self, authorizer: asyncprawcore.auth.BaseAuthorizer) -> None: ...
+    async def post_refresh_callback(self, authorizer: BaseAuthorizer) -> None: ...
     @abstractmethod
-    def pre_refresh_callback(self, authorizer: asyncprawcore.auth.BaseAuthorizer) -> None: ...
+    async def pre_refresh_callback(self, authorizer: BaseAuthorizer) -> None: ...
     @property
     def reddit(self) -> asyncpraw.Reddit: ...
     @reddit.setter
     def reddit(self, value: asyncpraw.Reddit) -> None: ...
 
 class FileTokenManager(BaseTokenManager):
     def __init__(self, filename: str) -> None: ...
-    async def post_refresh_callback(self, authorizer: asyncprawcore.auth.BaseAuthorizer) -> None: ...
-    async def pre_refresh_callback(self, authorizer: asyncprawcore.auth.BaseAuthorizer) -> None: ...
+    async def post_refresh_callback(self, authorizer: BaseAuthorizer) -> None: ...
+    async def pre_refresh_callback(self, authorizer: BaseAuthorizer) -> None: ...
 
 class SQLiteTokenManager(BaseTokenManager):
     def __init__(self, database: str, key: str) -> None: ...
     async def close(self) -> None: ...
     async def connection(self) -> "aiosqlite.Connection": ...
     async def is_registered(self) -> bool: ...
-    async def post_refresh_callback(self, authorizer: asyncprawcore.auth.BaseAuthorizer) -> None: ...
-    async def pre_refresh_callback(self, authorizer: asyncprawcore.auth.BaseAuthorizer) -> None: ...
+    async def post_refresh_callback(self, authorizer: BaseAuthorizer) -> None: ...
+    async def pre_refresh_callback(self, authorizer: BaseAuthorizer) -> None: ...
     async def register(self, refresh_token: str) -> bool: ...
```

