# Comparing `tmp/spotdl_rockbox-4.2.5.tar.gz` & `tmp/spotdl_rockbox-4.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotdl_rockbox-4.2.5.tar", max compression
+gzip compressed data, was "spotdl_rockbox-4.2.6.tar", max compression
```

## Comparing `spotdl_rockbox-4.2.5.tar` & `spotdl_rockbox-4.2.6.tar`

### file list

```diff
@@ -1,59 +1,58 @@
--rw-r--r--   0        0        0     1074 2024-04-21 08:10:32.037891 spotdl_rockbox-4.2.5/LICENSE
--rw-r--r--   0        0        0     2815 2024-04-21 08:37:34.977270 spotdl_rockbox-4.2.5/pyproject.toml
--rw-r--r--   0        0        0     6337 2024-04-21 08:10:32.038891 spotdl_rockbox-4.2.5/README.md
--rw-r--r--   0        0        0     4921 2024-04-21 08:10:32.055284 spotdl_rockbox-4.2.5/spotdl_rockbox/__init__.py
--rw-r--r--   0        0        0      209 2024-04-21 08:10:32.055284 spotdl_rockbox-4.2.5/spotdl_rockbox/__main__.py
--rw-r--r--   0        0        0       58 2024-04-21 08:10:32.056290 spotdl_rockbox-4.2.5/spotdl_rockbox/_version.py
--rw-r--r--   0        0        0      186 2024-04-21 08:10:32.056290 spotdl_rockbox-4.2.5/spotdl_rockbox/console/__init__.py
--rw-r--r--   0        0        0      808 2024-04-21 08:10:32.057700 spotdl_rockbox-4.2.5/spotdl_rockbox/console/download.py
--rw-r--r--   0        0        0     5374 2024-04-21 08:10:32.057700 spotdl_rockbox-4.2.5/spotdl_rockbox/console/entry_point.py
--rw-r--r--   0        0        0     6854 2024-04-21 08:10:32.058814 spotdl_rockbox-4.2.5/spotdl_rockbox/console/meta.py
--rw-r--r--   0        0        0     3225 2024-04-21 08:10:32.058814 spotdl_rockbox-4.2.5/spotdl_rockbox/console/save.py
--rw-r--r--   0        0        0     5662 2024-04-21 08:10:32.059819 spotdl_rockbox-4.2.5/spotdl_rockbox/console/sync.py
--rw-r--r--   0        0        0     1917 2024-04-21 08:10:32.059819 spotdl_rockbox-4.2.5/spotdl_rockbox/console/url.py
--rw-r--r--   0        0        0     3627 2024-04-21 08:10:32.061006 spotdl_rockbox-4.2.5/spotdl_rockbox/console/web.py
--rw-r--r--   0        0        0       80 2024-04-21 08:10:32.061006 spotdl_rockbox-4.2.5/spotdl_rockbox/download/__init__.py
--rw-r--r--   0        0        0    31039 2024-04-21 08:10:32.062153 spotdl_rockbox-4.2.5/spotdl_rockbox/download/downloader.py
--rw-r--r--   0        0        0    13132 2024-04-21 08:10:32.063249 spotdl_rockbox-4.2.5/spotdl_rockbox/download/progress_handler.py
--rw-r--r--   0        0        0       54 2024-04-21 08:10:32.063249 spotdl_rockbox-4.2.5/spotdl_rockbox/providers/__init__.py
--rw-r--r--   0        0        0      669 2024-04-21 08:10:32.064653 spotdl_rockbox-4.2.5/spotdl_rockbox/providers/audio/__init__.py
--rw-r--r--   0        0        0     6283 2024-04-21 08:10:32.065156 spotdl_rockbox-4.2.5/spotdl_rockbox/providers/audio/bandcamp.py
--rw-r--r--   0        0        0    12128 2024-04-21 08:10:32.065156 spotdl_rockbox-4.2.5/spotdl_rockbox/providers/audio/base.py
--rw-r--r--   0        0        0     5307 2024-04-21 08:10:32.065156 spotdl_rockbox-4.2.5/spotdl_rockbox/providers/audio/piped.py
--rw-r--r--   0        0        0     2777 2024-04-21 08:10:32.066661 spotdl_rockbox-4.2.5/spotdl_rockbox/providers/audio/sliderkz.py
--rw-r--r--   0        0        0     2832 2024-04-21 08:10:32.066661 spotdl_rockbox-4.2.5/spotdl_rockbox/providers/audio/soundcloud.py
--rw-r--r--   0        0        0     1840 2024-04-21 08:10:32.067674 spotdl_rockbox-4.2.5/spotdl_rockbox/providers/audio/youtube.py
--rw-r--r--   0        0        0     2845 2024-04-21 08:10:32.067674 spotdl_rockbox-4.2.5/spotdl_rockbox/providers/audio/ytmusic.py
--rw-r--r--   0        0        0      382 2024-04-21 08:10:32.068907 spotdl_rockbox-4.2.5/spotdl_rockbox/providers/lyrics/__init__.py
--rw-r--r--   0        0        0     3821 2024-04-21 08:10:32.068907 spotdl_rockbox-4.2.5/spotdl_rockbox/providers/lyrics/azlyrics.py
--rw-r--r--   0        0        0     3858 2024-04-21 08:10:32.069912 spotdl_rockbox-4.2.5/spotdl_rockbox/providers/lyrics/base.py
--rw-r--r--   0        0        0     3427 2024-04-21 08:10:32.069912 spotdl_rockbox-4.2.5/spotdl_rockbox/providers/lyrics/genius.py
--rw-r--r--   0        0        0     3017 2024-04-21 08:10:32.069912 spotdl_rockbox-4.2.5/spotdl_rockbox/providers/lyrics/musixmatch.py
--rw-r--r--   0        0        0     2301 2024-04-21 08:10:32.071415 spotdl_rockbox-4.2.5/spotdl_rockbox/providers/lyrics/synced.py
--rw-r--r--   0        0        0       38 2024-04-21 08:10:32.071415 spotdl_rockbox-4.2.5/spotdl_rockbox/types/__init__.py
--rw-r--r--   0        0        0     3624 2024-04-21 08:10:32.072460 spotdl_rockbox-4.2.5/spotdl_rockbox/types/album.py
--rw-r--r--   0        0        0     3100 2024-04-21 08:10:32.072460 spotdl_rockbox-4.2.5/spotdl_rockbox/types/artist.py
--rw-r--r--   0        0        0     4652 2024-04-21 08:10:32.073462 spotdl_rockbox-4.2.5/spotdl_rockbox/types/options.py
--rw-r--r--   0        0        0     4606 2024-04-21 08:10:32.073462 spotdl_rockbox-4.2.5/spotdl_rockbox/types/playlist.py
--rw-r--r--   0        0        0     2187 2024-04-21 08:10:32.074551 spotdl_rockbox-4.2.5/spotdl_rockbox/types/result.py
--rw-r--r--   0        0        0     3351 2024-04-21 08:10:32.074551 spotdl_rockbox-4.2.5/spotdl_rockbox/types/saved.py
--rw-r--r--   0        0        0    10335 2024-04-21 08:10:32.075555 spotdl_rockbox-4.2.5/spotdl_rockbox/types/song.py
--rw-r--r--   0        0        0      103 2024-04-21 08:10:32.076554 spotdl_rockbox-4.2.5/spotdl_rockbox/utils/__init__.py
--rw-r--r--   0        0        0     1001 2024-04-21 08:10:32.076554 spotdl_rockbox-4.2.5/spotdl_rockbox/utils/archive.py
--rw-r--r--   0        0        0    22868 2024-04-21 08:10:32.077058 spotdl_rockbox-4.2.5/spotdl_rockbox/utils/arguments.py
--rw-r--r--   0        0        0     8302 2024-04-21 08:10:32.077058 spotdl_rockbox-4.2.5/spotdl_rockbox/utils/config.py
--rw-r--r--   0        0        0     3109 2024-04-21 08:10:32.078297 spotdl_rockbox-4.2.5/spotdl_rockbox/utils/console.py
--rw-r--r--   0        0        0      571 2024-04-21 08:10:32.078297 spotdl_rockbox-4.2.5/spotdl_rockbox/utils/downloader.py
--rw-r--r--   0        0        0    12030 2024-04-21 08:10:32.079301 spotdl_rockbox-4.2.5/spotdl_rockbox/utils/ffmpeg.py
--rw-r--r--   0        0        0    17906 2024-04-21 08:10:32.079301 spotdl_rockbox-4.2.5/spotdl_rockbox/utils/formatter.py
--rw-r--r--   0        0        0     7018 2024-04-21 08:10:32.080304 spotdl_rockbox-4.2.5/spotdl_rockbox/utils/github.py
--rw-r--r--   0        0        0     5605 2024-04-21 08:10:32.080304 spotdl_rockbox-4.2.5/spotdl_rockbox/utils/logging.py
--rw-r--r--   0        0        0     1197 2024-04-21 08:10:32.080304 spotdl_rockbox-4.2.5/spotdl_rockbox/utils/lrc.py
--rw-r--r--   0        0        0     5083 2024-04-21 08:10:32.081807 spotdl_rockbox-4.2.5/spotdl_rockbox/utils/m3u.py
--rw-r--r--   0        0        0    23074 2024-04-21 08:10:32.081807 spotdl_rockbox-4.2.5/spotdl_rockbox/utils/matching.py
--rw-r--r--   0        0        0    19497 2024-04-21 08:10:32.082868 spotdl_rockbox-4.2.5/spotdl_rockbox/utils/metadata.py
--rw-r--r--   0        0        0    23610 2024-04-21 08:10:32.082868 spotdl_rockbox-4.2.5/spotdl_rockbox/utils/search.py
--rw-r--r--   0        0        0     6967 2024-04-21 08:10:32.082868 spotdl_rockbox-4.2.5/spotdl_rockbox/utils/spotify.py
--rw-r--r--   0        0        0    28221 2024-04-21 08:10:32.084160 spotdl_rockbox-4.2.5/spotdl_rockbox/utils/static.py
--rw-r--r--   0        0        0    16417 2024-04-21 08:10:32.084160 spotdl_rockbox-4.2.5/spotdl_rockbox/utils/web.py
--rw-r--r--   0        0        0     8451 1970-01-01 00:00:00.000000 spotdl_rockbox-4.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-21 08:10:32.037891 spotdl_rockbox-4.2.6/LICENSE
+-rw-r--r--   0        0        0     2815 2024-04-21 08:59:23.545026 spotdl_rockbox-4.2.6/pyproject.toml
+-rw-r--r--   0        0        0     6337 2024-04-21 08:10:32.038891 spotdl_rockbox-4.2.6/README.md
+-rw-r--r--   0        0        0     4977 2024-04-21 08:52:55.439012 spotdl_rockbox-4.2.6/spotdl_rockbox/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-21 08:53:01.968536 spotdl_rockbox-4.2.6/spotdl_rockbox/__main__.py
+-rw-r--r--   0        0        0       58 2024-04-21 08:10:32.056290 spotdl_rockbox-4.2.6/spotdl_rockbox/_version.py
+-rw-r--r--   0        0        0      194 2024-04-21 08:58:06.601510 spotdl_rockbox-4.2.6/spotdl_rockbox/console/__init__.py
+-rw-r--r--   0        0        0      824 2024-04-21 08:58:06.279478 spotdl_rockbox-4.2.6/spotdl_rockbox/console/download.py
+-rw-r--r--   0        0        0     5414 2024-04-21 08:58:06.306471 spotdl_rockbox-4.2.6/spotdl_rockbox/console/entry_point.py
+-rw-r--r--   0        0        0     6902 2024-04-21 08:58:06.564198 spotdl_rockbox-4.2.6/spotdl_rockbox/console/meta.py
+-rw-r--r--   0        0        0     3257 2024-04-21 08:58:06.190782 spotdl_rockbox-4.2.6/spotdl_rockbox/console/save.py
+-rw-r--r--   0        0        0     5702 2024-04-21 08:58:06.527767 spotdl_rockbox-4.2.6/spotdl_rockbox/console/sync.py
+-rw-r--r--   0        0        0     1941 2024-04-21 08:58:06.650649 spotdl_rockbox-4.2.6/spotdl_rockbox/console/url.py
+-rw-r--r--   0        0        0     3675 2024-04-21 08:58:06.152808 spotdl_rockbox-4.2.6/spotdl_rockbox/console/web.py
+-rw-r--r--   0        0        0       80 2024-04-21 08:10:32.061006 spotdl_rockbox-4.2.6/spotdl_rockbox/download/__init__.py
+-rw-r--r--   0        0        0    31047 2024-04-21 08:58:06.508173 spotdl_rockbox-4.2.6/spotdl_rockbox/download/downloader.py
+-rw-r--r--   0        0        0    13148 2024-04-21 08:58:06.202535 spotdl_rockbox-4.2.6/spotdl_rockbox/download/progress_handler.py
+-rw-r--r--   0        0        0       54 2024-04-21 08:10:32.063249 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/__init__.py
+-rw-r--r--   0        0        0      725 2024-04-21 08:58:06.658161 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/__init__.py
+-rw-r--r--   0        0        0     6307 2024-04-21 08:58:06.417368 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/bandcamp.py
+-rw-r--r--   0        0        0    12168 2024-04-21 08:58:06.324813 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/base.py
+-rw-r--r--   0        0        0     5339 2024-04-21 08:58:06.227820 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/piped.py
+-rw-r--r--   0        0        0     2801 2024-04-21 08:58:06.713153 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/sliderkz.py
+-rw-r--r--   0        0        0     2848 2024-04-21 08:58:06.470970 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/soundcloud.py
+-rw-r--r--   0        0        0     1856 2024-04-21 08:58:06.165447 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/youtube.py
+-rw-r--r--   0        0        0     2869 2024-04-21 08:58:06.551703 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/ytmusic.py
+-rw-r--r--   0        0        0      422 2024-04-21 08:58:06.285507 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/__init__.py
+-rw-r--r--   0        0        0     3829 2024-04-21 08:58:06.133656 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/azlyrics.py
+-rw-r--r--   0        0        0     3874 2024-04-21 08:58:06.350412 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/base.py
+-rw-r--r--   0        0        0     3443 2024-04-21 08:58:06.117623 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/genius.py
+-rw-r--r--   0        0        0     3033 2024-04-21 08:58:06.342861 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/musixmatch.py
+-rw-r--r--   0        0        0     2309 2024-04-21 08:58:06.520722 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/synced.py
+-rw-r--r--   0        0        0       38 2024-04-21 08:10:32.071415 spotdl_rockbox-4.2.6/spotdl_rockbox/types/__init__.py
+-rw-r--r--   0        0        0     3640 2024-04-21 08:54:19.592091 spotdl_rockbox-4.2.6/spotdl_rockbox/types/album.py
+-rw-r--r--   0        0        0     3132 2024-04-21 08:58:06.438091 spotdl_rockbox-4.2.6/spotdl_rockbox/types/artist.py
+-rw-r--r--   0        0        0     4652 2024-04-21 08:10:32.073462 spotdl_rockbox-4.2.6/spotdl_rockbox/types/options.py
+-rw-r--r--   0        0        0     4622 2024-04-21 08:58:06.622462 spotdl_rockbox-4.2.6/spotdl_rockbox/types/playlist.py
+-rw-r--r--   0        0        0     2187 2024-04-21 08:10:32.074551 spotdl_rockbox-4.2.6/spotdl_rockbox/types/result.py
+-rw-r--r--   0        0        0     3351 2024-04-21 08:10:32.074551 spotdl_rockbox-4.2.6/spotdl_rockbox/types/saved.py
+-rw-r--r--   0        0        0    10343 2024-04-21 08:58:06.271422 spotdl_rockbox-4.2.6/spotdl_rockbox/types/song.py
+-rw-r--r--   0        0        0      103 2024-04-21 08:10:32.076554 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-21 08:10:32.076554 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/archive.py
+-rw-r--r--   0        0        0    22908 2024-04-21 08:49:05.109376 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/arguments.py
+-rw-r--r--   0        0        0     8310 2024-04-21 08:49:21.340072 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/config.py
+-rw-r--r--   0        0        0     3141 2024-04-21 08:55:55.038705 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/console.py
+-rw-r--r--   0        0        0      579 2024-04-21 08:49:59.616753 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/downloader.py
+-rw-r--r--   0        0        0    12046 2024-04-21 08:50:07.334761 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/ffmpeg.py
+-rw-r--r--   0        0        0    17914 2024-04-21 08:50:17.666572 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/formatter.py
+-rw-r--r--   0        0        0     5605 2024-04-21 08:10:32.080304 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/logging.py
+-rw-r--r--   0        0        0     1205 2024-04-21 08:50:31.807959 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/lrc.py
+-rw-r--r--   0        0        0     5099 2024-04-21 08:50:37.028317 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/m3u.py
+-rw-r--r--   0        0        0    23106 2024-04-21 08:50:47.530339 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/matching.py
+-rw-r--r--   0        0        0    19529 2024-04-21 08:50:57.292888 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/metadata.py
+-rw-r--r--   0        0        0    23666 2024-04-21 08:51:09.200552 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/search.py
+-rw-r--r--   0        0        0     6975 2024-04-21 08:51:14.952780 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/spotify.py
+-rw-r--r--   0        0        0    28221 2024-04-21 08:10:32.084160 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/static.py
+-rw-r--r--   0        0        0    16513 2024-04-21 08:52:42.082765 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/web.py
+-rw-r--r--   0        0        0     8451 1970-01-01 00:00:00.000000 spotdl_rockbox-4.2.6/PKG-INFO
```

### Comparing `spotdl_rockbox-4.2.5/LICENSE` & `spotdl_rockbox-4.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.5/pyproject.toml` & `spotdl_rockbox-4.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotdl_rockbox"
-version = "4.2.5"
+version = "4.2.6"
 description = "Fox for rockbox. Download your Spotify playlists and songs along with album art and metadata"
 license = "MIT"
 authors = ["spotDL Team <spotdladmins@googlegroups.com>", "MisteryDush <ikrom.arifdjanov@gmail.com>"]
 maintainers = ["xnetcat <xnetcat.dev@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/MisteryDush/spotify-downloader-rockbox.git"
 homepage = "https://github.com/spotDL/spotify-downloader/"
```

### Comparing `spotdl_rockbox-4.2.5/README.md` & `spotdl_rockbox-4.2.6/README.md`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/__init__.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 import asyncio
 import concurrent.futures
 import logging
 from pathlib import Path
 from typing import List, Optional, Tuple, Union
 
-from spotdl._version import __version__
-from spotdl.console import console_entry_point
-from spotdl.download.downloader import Downloader
-from spotdl.types.options import DownloaderOptionalOptions, DownloaderOptions
-from spotdl.types.song import Song
-from spotdl.utils.search import parse_query
-from spotdl.utils.spotify import SpotifyClient
+from spotdl_rockbox._version import __version__
+from spotdl_rockbox.console import console_entry_point
+from spotdl_rockbox.download.downloader import Downloader
+from spotdl_rockbox.types.options import DownloaderOptionalOptions, DownloaderOptions
+from spotdl_rockbox.types.song import Song
+from spotdl_rockbox.utils.search import parse_query
+from spotdl_rockbox.utils.spotify import SpotifyClient
 
 __all__ = ["Spotdl", "console_entry_point", "__version__"]
 
 logger = logging.getLogger(__name__)
 
 
 class Spotdl:
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/console/entry_point.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/console/entry_point.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 """
 
 import logging
 import signal
 import sys
 import time
 
-from spotdl.console.download import download
-from spotdl.console.meta import meta
-from spotdl.console.save import save
-from spotdl.console.sync import sync
-from spotdl.console.url import url
+from spotdl_rockbox.console.download import download
+from spotdl_rockbox.console.meta import meta
+from spotdl_rockbox.console.save import save
+from spotdl_rockbox.console.sync import sync
+from spotdl_rockbox.console.url import url
 from spotdl.console.web import web
 from spotdl.download.downloader import Downloader, DownloaderError
 from spotdl.utils.arguments import parse_arguments
 from spotdl.utils.config import create_settings
 from spotdl.utils.console import ACTIONS, generate_initial_config, is_executable
 from spotdl.utils.downloader import check_ytmusic_connection
 from spotdl.utils.ffmpeg import FFmpegError, download_ffmpeg, is_ffmpeg_installed
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/console/meta.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/console/meta.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 """
 
 import asyncio
 import logging
 from pathlib import Path
 from typing import List
 
-from spotdl.download.downloader import Downloader
-from spotdl.types.song import Song
-from spotdl.utils.ffmpeg import FFMPEG_FORMATS
-from spotdl.utils.lrc import generate_lrc
-from spotdl.utils.metadata import embed_metadata, get_file_metadata
-from spotdl.utils.search import QueryError, get_search_results, parse_query, reinit_song
+from spotdl_rockbox.download.downloader import Downloader
+from spotdl_rockbox.types.song import Song
+from spotdl_rockbox.utils.ffmpeg import FFMPEG_FORMATS
+from spotdl_rockbox.utils.lrc import generate_lrc
+from spotdl_rockbox.utils.metadata import embed_metadata, get_file_metadata
+from spotdl_rockbox.utils.search import QueryError, get_search_results, parse_query, reinit_song
 
 __all__ = ["meta"]
 
 logger = logging.getLogger(__name__)
 
 
 def meta(query: List[str], downloader: Downloader) -> None:
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/console/save.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/console/save.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 """
 
 import asyncio
 import json
 import logging
 from typing import List
 
-from spotdl.download.downloader import Downloader, DownloaderError
-from spotdl.types.song import Song
-from spotdl.utils.m3u import gen_m3u_files
-from spotdl.utils.search import parse_query
+from spotdl_rockbox.download.downloader import Downloader, DownloaderError
+from spotdl_rockbox.types.song import Song
+from spotdl_rockbox.utils.m3u import gen_m3u_files
+from spotdl_rockbox.utils.search import parse_query
 
 __all__ = ["save"]
 
 logger = logging.getLogger(__name__)
 
 
 def save(
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/console/sync.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/console/sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 Sync module for the console.
 """
 
 import json
 import logging
 from typing import List
 
-from spotdl.download.downloader import Downloader
-from spotdl.types.song import Song
-from spotdl.utils.formatter import create_file_name
-from spotdl.utils.m3u import gen_m3u_files
-from spotdl.utils.search import parse_query
+from spotdl_rockbox.download.downloader import Downloader
+from spotdl_rockbox.types.song import Song
+from spotdl_rockbox.utils.formatter import create_file_name
+from spotdl_rockbox.utils.m3u import gen_m3u_files
+from spotdl_rockbox.utils.search import parse_query
 
 __all__ = ["sync"]
 
 logger = logging.getLogger(__name__)
 
 
 def sync(
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/console/url.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/console/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Url module for the console.
 """
 
 import asyncio
 import logging
 from typing import List
 
-from spotdl.download.downloader import Downloader
-from spotdl.types.song import Song
-from spotdl.utils.search import parse_query
+from spotdl_rockbox.download.downloader import Downloader
+from spotdl_rockbox.types.song import Song
+from spotdl_rockbox.utils.search import parse_query
 
 __all__ = ["url"]
 
 logger = logging.getLogger(__name__)
 
 
 def url(
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/console/web.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/console/web.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 import sys
 import webbrowser
 
 from fastapi import Depends, FastAPI
 from fastapi.middleware.cors import CORSMiddleware
 from uvicorn import Config, Server
 
-from spotdl._version import __version__
-from spotdl.types.options import DownloaderOptions, WebOptions
-from spotdl.utils.config import get_spotdl_path
-from spotdl.utils.github import download_github_dir
-from spotdl.utils.logging import NAME_TO_LEVEL
-from spotdl.utils.web import (
+from spotdl_rockbox._version import __version__
+from spotdl_rockbox.types.options import DownloaderOptions, WebOptions
+from spotdl_rockbox.utils.config import get_spotdl_path
+from spotdl_rockbox.utils.github import download_github_dir
+from spotdl_rockbox.utils.logging import NAME_TO_LEVEL
+from spotdl_rockbox.utils.web import (
     ALLOWED_ORIGINS,
     SPAStaticFiles,
     app_state,
     fix_mime_types,
     get_current_state,
     router,
 )
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/download/downloader.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/download/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from argparse import Namespace
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Type, Union
 
 from yt_dlp.postprocessor.modify_chapters import ModifyChaptersPP
 from yt_dlp.postprocessor.sponsorblock import SponsorBlockPP
 
-from spotdl.download.progress_handler import ProgressHandler
+from spotdl_rockbox.download.progress_handler import ProgressHandler
 from spotdl.providers.audio import (
     AudioProvider,
     BandCamp,
     Piped,
     SliderKZ,
     SoundCloud,
     YouTube,
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/download/progress_handler.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/download/progress_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     Task,
     TaskID,
     TimeRemainingColumn,
 )
 from rich.style import StyleType
 from rich.text import Text
 
-from spotdl.types.song import Song
-from spotdl.utils.static import BAD_CHARS
+from spotdl_rockbox.types.song import Song
+from spotdl_rockbox.utils.static import BAD_CHARS
 
 __all__ = [
     "ProgressHandler",
     "SongTracker",
     "ProgressHandlerError",
     "SizedTextColumn",
 ]
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/providers/audio/__init__.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 Audio providers for spotdl.
 """
 
-from spotdl.providers.audio.bandcamp import BandCamp
-from spotdl.providers.audio.base import (
+from spotdl_rockbox.providers.audio.bandcamp import BandCamp
+from spotdl_rockbox.providers.audio.base import (
     ISRC_REGEX,
     AudioProvider,
     AudioProviderError,
     YTDLLogger,
 )
-from spotdl.providers.audio.piped import Piped
-from spotdl.providers.audio.sliderkz import SliderKZ
-from spotdl.providers.audio.soundcloud import SoundCloud
-from spotdl.providers.audio.youtube import YouTube
-from spotdl.providers.audio.ytmusic import YouTubeMusic
+from spotdl_rockbox.providers.audio.piped import Piped
+from spotdl_rockbox.providers.audio.sliderkz import SliderKZ
+from spotdl_rockbox.providers.audio.soundcloud import SoundCloud
+from spotdl_rockbox.providers.audio.youtube import YouTube
+from spotdl_rockbox.providers.audio.ytmusic import YouTubeMusic
 
 __all__ = [
     "YouTube",
     "YouTubeMusic",
     "SliderKZ",
     "SoundCloud",
     "BandCamp",
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/providers/audio/bandcamp.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/bandcamp.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """
 
 import logging
 from typing import Any, Dict, List, Optional, Tuple
 
 import requests
 
-from spotdl.providers.audio.base import AudioProvider
-from spotdl.types.result import Result
-from spotdl.utils.config import GlobalConfig
+from spotdl_rockbox.providers.audio.base import AudioProvider
+from spotdl_rockbox.types.result import Result
+from spotdl_rockbox.utils.config import GlobalConfig
 
 __all__ = ["BandCamp"]
 
 logger = logging.getLogger(__name__)
 
 
 class BandCampTrack:
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/providers/audio/base.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 import logging
 import re
 import shlex
 from typing import Any, Dict, List, Optional, Tuple
 
 from yt_dlp import YoutubeDL
 
-from spotdl.types.result import Result
-from spotdl.types.song import Song
-from spotdl.utils.config import get_temp_path
-from spotdl.utils.formatter import (
+from spotdl_rockbox.types.result import Result
+from spotdl_rockbox.types.song import Song
+from spotdl_rockbox.utils.config import get_temp_path
+from spotdl_rockbox.utils.formatter import (
     args_to_ytdlp_options,
     create_search_query,
     create_song_title,
 )
-from spotdl.utils.matching import get_best_matches, order_results
+from spotdl_rockbox.utils.matching import get_best_matches, order_results
 
 __all__ = ["AudioProviderError", "AudioProvider", "ISRC_REGEX", "YTDLLogger"]
 
 logger = logging.getLogger(__name__)
 
 
 class AudioProviderError(Exception):
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/providers/audio/piped.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/piped.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import logging
 import shlex
 from typing import Any, Dict, List, Optional
 
 import requests
 from yt_dlp import YoutubeDL
 
-from spotdl.providers.audio.base import ISRC_REGEX, AudioProvider, YTDLLogger
-from spotdl.types.result import Result
-from spotdl.utils.config import GlobalConfig, get_temp_path
-from spotdl.utils.formatter import args_to_ytdlp_options
+from spotdl_rockbox.providers.audio.base import ISRC_REGEX, AudioProvider, YTDLLogger
+from spotdl_rockbox.types.result import Result
+from spotdl_rockbox.utils.config import GlobalConfig, get_temp_path
+from spotdl_rockbox.utils.formatter import args_to_ytdlp_options
 
 __all__ = ["Piped"]
 logger = logging.getLogger(__name__)
 
 HEADERS = {
     "accept": "*/*",
 }
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/providers/audio/sliderkz.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/sliderkz.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 """
 
 import logging
 from typing import Any, Dict, List
 
 import requests
 
-from spotdl.providers.audio.base import AudioProvider
-from spotdl.types.result import Result
-from spotdl.utils.config import GlobalConfig
+from spotdl_rockbox.providers.audio.base import AudioProvider
+from spotdl_rockbox.types.result import Result
+from spotdl_rockbox.utils.config import GlobalConfig
 
 __all__ = ["SliderKZ"]
 
 logger = logging.getLogger(__name__)
 
 HEADERS = {
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:109.0) Gecko/20100101 Firefox/111.0"
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/providers/audio/soundcloud.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/soundcloud.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import logging
 import re
 from itertools import islice
 from typing import Any, Dict, List
 
 from soundcloud import SoundCloud as SoundCloudClient
 
-from spotdl.providers.audio.base import AudioProvider
-from spotdl.types.result import Result
+from spotdl_rockbox.providers.audio.base import AudioProvider
+from spotdl_rockbox.types.result import Result
 
 __all__ = ["SoundCloud"]
 
 logger = logging.getLogger(__name__)
 
 
 class SoundCloud(AudioProvider):
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/providers/audio/youtube.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/youtube.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 """
 
 from typing import Any, Dict, List, Optional
 
 from pytube import Search
 from pytube import YouTube as PyTube
 
-from spotdl.providers.audio.base import AudioProvider
-from spotdl.types.result import Result
+from spotdl_rockbox.providers.audio.base import AudioProvider
+from spotdl_rockbox.types.result import Result
 
 __all__ = ["YouTube"]
 
 
 class YouTube(AudioProvider):
     """
     YouTube audio provider class
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/providers/audio/ytmusic.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/ytmusic.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 YTMusic module for downloading and searching songs.
 """
 
 from typing import Any, Dict, List
 
 from ytmusicapi import YTMusic
 
-from spotdl.providers.audio.base import ISRC_REGEX, AudioProvider
-from spotdl.types.result import Result
-from spotdl.utils.formatter import parse_duration
+from spotdl_rockbox.providers.audio.base import ISRC_REGEX, AudioProvider
+from spotdl_rockbox.types.result import Result
+from spotdl_rockbox.utils.formatter import parse_duration
 
 __all__ = ["YouTubeMusic"]
 
 
 class YouTubeMusic(AudioProvider):
     """
     YouTube Music audio provider class
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/providers/lyrics/azlyrics.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/azlyrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from typing import Dict, List, Optional
 
 import requests
 from bs4 import BeautifulSoup
 
-from spotdl.providers.lyrics.base import LyricsProvider
+from spotdl_rockbox.providers.lyrics.base import LyricsProvider
 
 __all__ = ["AzLyrics"]
 
 
 class AzLyrics(LyricsProvider):
     """
     AZLyrics lyrics provider class.
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/providers/lyrics/base.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Base module for all other lyrics providers.
 """
 
 import logging
 from typing import Dict, List, Optional
 
-from spotdl.utils.formatter import ratio, slugify
-from spotdl.utils.matching import based_sort
+from spotdl_rockbox.utils.formatter import ratio, slugify
+from spotdl_rockbox.utils.matching import based_sort
 
 __all__ = ["LyricsProvider"]
 logger = logging.getLogger(__name__)
 
 
 class LyricsProvider:
     """
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/providers/lyrics/genius.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/genius.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 """
 
 from typing import Dict, List, Optional
 
 import requests
 from bs4 import BeautifulSoup
 
-from spotdl.providers.lyrics.base import LyricsProvider
-from spotdl.utils.config import GlobalConfig
+from spotdl_rockbox.providers.lyrics.base import LyricsProvider
+from spotdl_rockbox.utils.config import GlobalConfig
 
 __all__ = ["Genius"]
 
 
 class Genius(LyricsProvider):
     """
     Genius lyrics provider class.
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/providers/lyrics/musixmatch.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/musixmatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 from typing import Dict, List, Optional
 from urllib.parse import quote
 
 import requests
 from bs4 import BeautifulSoup
 
-from spotdl.providers.lyrics.base import LyricsProvider
-from spotdl.utils.config import GlobalConfig
+from spotdl_rockbox.providers.lyrics.base import LyricsProvider
+from spotdl_rockbox.utils.config import GlobalConfig
 
 __all__ = ["MusixMatch"]
 
 
 class MusixMatch(LyricsProvider):
     """
     MusixMatch lyrics provider class.
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/providers/lyrics/synced.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/synced.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from typing import Dict, List, Optional
 
 import requests
 import syncedlyrics
 
-from spotdl.providers.lyrics.base import LyricsProvider
+from spotdl_rockbox.providers.lyrics.base import LyricsProvider
 
 __all__ = ["Synced"]
 
 
 class Synced(LyricsProvider):
     """
     Lyrics provider for synced lyrics using the syncedlyrics library
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/types/album.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/types/album.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Artist module for retrieving artist data from Spotify.
 """
 
 from dataclasses import dataclass
 from typing import Any, Dict, List, Tuple
 
-from spotdl.types.song import Song, SongList
-from spotdl.utils.spotify import SpotifyClient
+from spotdl_rockbox.types.song import Song, SongList
+from spotdl_rockbox.utils.spotify import SpotifyClient
 
 __all__ = ["Album", "AlbumError"]
 
 
 class AlbumError(Exception):
     """
     Base class for all exceptions related to albums.
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/types/artist.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/types/artist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Artist module for retrieving artist data from Spotify.
 """
 
 from dataclasses import dataclass
 from typing import Any, Dict, List, Set, Tuple
 
-from spotdl.types.album import Album
-from spotdl.types.song import Song, SongList
-from spotdl.utils.formatter import slugify
-from spotdl.utils.spotify import SpotifyClient
+from spotdl_rockbox.types.album import Album
+from spotdl_rockbox.types.song import Song, SongList
+from spotdl_rockbox.utils.formatter import slugify
+from spotdl_rockbox.utils.spotify import SpotifyClient
 
 __all__ = ["Artist", "ArtistError"]
 
 
 class ArtistError(Exception):
     """
     Base class for all exceptions related to artists.
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/types/options.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/types/options.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/types/playlist.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/types/playlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 Playlist module for retrieving playlist data from Spotify.
 """
 
 import logging
 from dataclasses import dataclass
 from typing import Any, Dict, List, Tuple
 
-from spotdl.types.song import Song, SongList
-from spotdl.utils.spotify import SpotifyClient
+from spotdl_rockbox.types.song import Song, SongList
+from spotdl_rockbox.utils.spotify import SpotifyClient
 
 __all__ = ["Playlist", "PlaylistError"]
 
 logger = logging.getLogger(__name__)
 
 
 class PlaylistError(Exception):
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/types/result.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/types/result.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/types/saved.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/types/saved.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/types/song.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/types/song.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import json
 from dataclasses import asdict, dataclass
 from typing import Any, Dict, List, Optional, Tuple
 
 from rapidfuzz import fuzz
 
-from spotdl.utils.spotify import SpotifyClient
+from spotdl_rockbox.utils.spotify import SpotifyClient
 
 __all__ = ["Song", "SongList", "SongError"]
 
 
 class SongError(Exception):
     """
     Base class for all exceptions related to songs.
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/utils/archive.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/archive.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/utils/arguments.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 import argparse
 import sys
 import textwrap
 from argparse import ArgumentParser, Namespace, _ArgumentGroup
 from typing import List
 
-from spotdl import _version
-from spotdl.download.downloader import AUDIO_PROVIDERS, LYRICS_PROVIDERS
-from spotdl.utils.ffmpeg import FFMPEG_FORMATS
-from spotdl.utils.formatter import VARS
-from spotdl.utils.logging import NAME_TO_LEVEL
+from spotdl_rockbox import _version
+from spotdl_rockbox.download.downloader import AUDIO_PROVIDERS, LYRICS_PROVIDERS
+from spotdl_rockbox.utils.ffmpeg import FFMPEG_FORMATS
+from spotdl_rockbox.utils.formatter import VARS
+from spotdl_rockbox.utils.logging import NAME_TO_LEVEL
 
 __all__ = ["OPERATIONS", "SmartFormatter", "parse_arguments"]
 
 OPERATIONS = ["download", "save", "web", "sync", "meta", "url"]
 
 
 class SmartFormatter(argparse.HelpFormatter):
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/utils/config.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import platform
 from argparse import Namespace
 from pathlib import Path
 from typing import Any, Dict, Tuple, Union
 
 import platformdirs
 
-from spotdl.types.options import (
+from spotdl_rockbox.types.options import (
     DownloaderOptions,
     SpotDLOptions,
     SpotifyOptions,
     WebOptions,
 )
 
 __all__ = [
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/utils/console.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/console.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Module for holding console related actions.
 """
 
 import json
 import sys
 
-from spotdl.utils.config import DEFAULT_CONFIG, get_config_file
-from spotdl.utils.ffmpeg import download_ffmpeg as ffmpeg_download
-from spotdl.utils.ffmpeg import get_local_ffmpeg, is_ffmpeg_installed
-from spotdl.utils.github import check_for_updates as get_update_status
+from spotdl_rockbox.utils.config import DEFAULT_CONFIG, get_config_file
+from spotdl_rockbox.utils.ffmpeg import download_ffmpeg as ffmpeg_download
+from spotdl_rockbox.utils.ffmpeg import get_local_ffmpeg, is_ffmpeg_installed
+from spotdl_rockbox.utils.github import check_for_updates as get_update_status
 
 __all__ = [
     "is_frozen",
     "is_executable",
     "generate_initial_config",
     "generate_config",
     "check_for_updates",
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/utils/downloader.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/downloader.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Module for functions related to downloading songs.
 """
 
-from spotdl.providers.audio import YouTubeMusic
+from spotdl_rockbox.providers.audio import YouTubeMusic
 
 __all__ = ["check_ytmusic_connection"]
 
 
 def check_ytmusic_connection() -> bool:
     """
     Check if we can connect to YouTube Music API
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/utils/ffmpeg.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/ffmpeg.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 import stat
 import subprocess
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import requests
 
-from spotdl.utils.config import get_spotdl_path
-from spotdl.utils.formatter import to_ms
+from spotdl_rockbox.utils.config import get_spotdl_path
+from spotdl_rockbox.utils.formatter import to_ms
 
 __all__ = [
     "FFMPEG_URLS",
     "FFMPEG_FORMATS",
     "DUR_REGEX",
     "TIME_REGEX",
     "VERSION_REGEX",
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/utils/formatter.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import pykakasi
 from rapidfuzz import fuzz
 from slugify import slugify as py_slugify
 from yt_dlp.options import create_parser
 from yt_dlp.utils import sanitize_filename
 
-from spotdl.types.song import Song
+from spotdl_rockbox.types.song import Song
 
 __all__ = [
     "VARS",
     "JAP_REGEX",
     "DISALLOWED_REGEX",
     "create_song_title",
     "sanitize_string",
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/utils/logging.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/logging.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/utils/lrc.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/lrc.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 import re
 from pathlib import Path
 
 from syncedlyrics import search as syncedlyrics_search
 from syncedlyrics.utils import is_lrc_valid, save_lrc_file
 
-from spotdl.types.song import Song
+from spotdl_rockbox.types.song import Song
 
 logger = logging.getLogger(__name__)
 
 __all__ = ["generate_lrc", "remomve_lrc"]
 
 
 def generate_lrc(song: Song, output_file: Path):
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/utils/m3u.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/m3u.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Module for creating m3u content and writing it to a file.
 """
 
 from typing import Dict, List, Optional
 
-from spotdl.types.song import Song
-from spotdl.utils.formatter import create_file_name
+from spotdl_rockbox.types.song import Song
+from spotdl_rockbox.utils.formatter import create_file_name
 
 __all__ = [
     "create_m3u_content",
     "gen_m3u_files",
     "create_m3u_file",
 ]
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/utils/matching.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/matching.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 """
 
 import logging
 from itertools import product, zip_longest
 from math import exp
 from typing import Dict, List, Optional, Tuple
 
-from spotdl.types.result import Result
-from spotdl.types.song import Song
-from spotdl.utils.formatter import (
+from spotdl_rockbox.types.result import Result
+from spotdl_rockbox.types.song import Song
+from spotdl_rockbox.utils.formatter import (
     create_search_query,
     create_song_title,
     ratio,
     slugify,
 )
-from spotdl.utils.logging import MATCH
+from spotdl_rockbox.utils.logging import MATCH
 
 __all__ = [
     "FORBIDDEN_WORDS",
     "fill_string",
     "create_clean_string",
     "sort_string",
     "based_sort",
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/utils/metadata.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,18 @@
     USLT,
     WOAS,
 )
 from mutagen.id3._specs import Encoding
 from mutagen.mp4 import MP4Cover
 from mutagen.wave import WAVE
 
-from spotdl.types.song import Song
-from spotdl.utils.config import GlobalConfig
-from spotdl.utils.formatter import to_ms
-from spotdl.utils.lrc import remomve_lrc
+from spotdl_rockbox.types.song import Song
+from spotdl_rockbox.utils.config import GlobalConfig
+from spotdl_rockbox.utils.formatter import to_ms
+from spotdl_rockbox.utils.lrc import remomve_lrc
 
 logger = logging.getLogger(__name__)
 
 __all__ = [
     "MetadataError",
     "M4A_TAG_PRESET",
     "MP3_TAG_PRESET",
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/utils/search.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 import re
 from pathlib import Path
 from typing import Dict, List, Optional
 
 import requests
 from ytmusicapi import YTMusic
 
-from spotdl.types.album import Album
-from spotdl.types.artist import Artist
-from spotdl.types.playlist import Playlist
-from spotdl.types.saved import Saved
-from spotdl.types.song import Song, SongList
-from spotdl.utils.metadata import get_file_metadata
-from spotdl.utils.spotify import SpotifyClient, SpotifyError
+from spotdl_rockbox.types.album import Album
+from spotdl_rockbox.types.artist import Artist
+from spotdl_rockbox.types.playlist import Playlist
+from spotdl_rockbox.types.saved import Saved
+from spotdl_rockbox.types.song import Song, SongList
+from spotdl_rockbox.utils.metadata import get_file_metadata
+from spotdl_rockbox.utils.spotify import SpotifyClient, SpotifyError
 
 __all__ = [
     "QueryError",
     "get_search_results",
     "parse_query",
     "get_simple_songs",
     "reinit_song",
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/utils/spotify.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/spotify.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from typing import Dict, Optional
 
 import requests
 from spotipy import Spotify
 from spotipy.cache_handler import CacheFileHandler, MemoryCacheHandler
 from spotipy.oauth2 import SpotifyClientCredentials, SpotifyOAuth
 
-from spotdl.utils.config import get_cache_path, get_spotify_cache_path
+from spotdl_rockbox.utils.config import get_cache_path, get_spotify_cache_path
 
 __all__ = [
     "SpotifyError",
     "SpotifyClient",
     "save_spotify_cache",
 ]
```

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/utils/static.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/static.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.5/spotdl_rockbox/utils/web.py` & `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/web.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,34 +24,34 @@
     WebSocketDisconnect,
 )
 from fastapi.responses import FileResponse
 from fastapi.staticfiles import StaticFiles
 from starlette.types import Scope
 from uvicorn import Server
 
-from spotdl._version import __version__
-from spotdl.download.downloader import Downloader
-from spotdl.download.progress_handler import ProgressHandler, SongTracker
-from spotdl.types.album import Album
-from spotdl.types.artist import Artist
-from spotdl.types.options import (
+from spotdl_rockbox._version import __version__
+from spotdl_rockbox.download.downloader import Downloader
+from spotdl_rockbox.download.progress_handler import ProgressHandler, SongTracker
+from spotdl_rockbox.types.album import Album
+from spotdl_rockbox.types.artist import Artist
+from spotdl_rockbox.types.options import (
     DownloaderOptionalOptions,
     DownloaderOptions,
     WebOptions,
 )
-from spotdl.types.playlist import Playlist
-from spotdl.types.song import Song
-from spotdl.utils.arguments import create_parser
-from spotdl.utils.config import (
+from spotdl_rockbox.types.playlist import Playlist
+from spotdl_rockbox.types.song import Song
+from spotdl_rockbox.utils.arguments import create_parser
+from spotdl_rockbox.utils.config import (
     DOWNLOADER_OPTIONS,
     create_settings_type,
     get_spotdl_path,
 )
-from spotdl.utils.github import RateLimitError, get_latest_version, get_status
-from spotdl.utils.search import get_search_results
+from spotdl_rockbox.utils.github import RateLimitError, get_latest_version, get_status
+from spotdl_rockbox.utils.search import get_search_results
 
 __all__ = [
     "ALLOWED_ORIGINS",
     "SPAStaticFiles",
     "Client",
     "ApplicationState",
     "router",
```

### Comparing `spotdl_rockbox-4.2.5/PKG-INFO` & `spotdl_rockbox-4.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotdl_rockbox
-Version: 4.2.5
+Version: 4.2.6
 Summary: Fox for rockbox. Download your Spotify playlists and songs along with album art and metadata
 Home-page: https://github.com/spotDL/spotify-downloader/
 License: MIT
 Keywords: spotify,downloader,spotdl,music
 Author: spotDL Team
 Author-email: spotdladmins@googlegroups.com
 Maintainer: xnetcat
```

