# Comparing `tmp/spotdl_rockbox-4.2.6.tar.gz` & `tmp/spotdl_rockbox-4.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotdl_rockbox-4.2.6.tar", max compression
+gzip compressed data, was "spotdl_rockbox-4.2.7.tar", max compression
```

## Comparing `spotdl_rockbox-4.2.6.tar` & `spotdl_rockbox-4.2.7.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1074 2024-04-21 08:10:32.037891 spotdl_rockbox-4.2.6/LICENSE
--rw-r--r--   0        0        0     2815 2024-04-21 08:59:23.545026 spotdl_rockbox-4.2.6/pyproject.toml
--rw-r--r--   0        0        0     6337 2024-04-21 08:10:32.038891 spotdl_rockbox-4.2.6/README.md
--rw-r--r--   0        0        0     4977 2024-04-21 08:52:55.439012 spotdl_rockbox-4.2.6/spotdl_rockbox/__init__.py
--rw-r--r--   0        0        0      225 2024-04-21 08:53:01.968536 spotdl_rockbox-4.2.6/spotdl_rockbox/__main__.py
--rw-r--r--   0        0        0       58 2024-04-21 08:10:32.056290 spotdl_rockbox-4.2.6/spotdl_rockbox/_version.py
--rw-r--r--   0        0        0      194 2024-04-21 08:58:06.601510 spotdl_rockbox-4.2.6/spotdl_rockbox/console/__init__.py
--rw-r--r--   0        0        0      824 2024-04-21 08:58:06.279478 spotdl_rockbox-4.2.6/spotdl_rockbox/console/download.py
--rw-r--r--   0        0        0     5414 2024-04-21 08:58:06.306471 spotdl_rockbox-4.2.6/spotdl_rockbox/console/entry_point.py
--rw-r--r--   0        0        0     6902 2024-04-21 08:58:06.564198 spotdl_rockbox-4.2.6/spotdl_rockbox/console/meta.py
--rw-r--r--   0        0        0     3257 2024-04-21 08:58:06.190782 spotdl_rockbox-4.2.6/spotdl_rockbox/console/save.py
--rw-r--r--   0        0        0     5702 2024-04-21 08:58:06.527767 spotdl_rockbox-4.2.6/spotdl_rockbox/console/sync.py
--rw-r--r--   0        0        0     1941 2024-04-21 08:58:06.650649 spotdl_rockbox-4.2.6/spotdl_rockbox/console/url.py
--rw-r--r--   0        0        0     3675 2024-04-21 08:58:06.152808 spotdl_rockbox-4.2.6/spotdl_rockbox/console/web.py
--rw-r--r--   0        0        0       80 2024-04-21 08:10:32.061006 spotdl_rockbox-4.2.6/spotdl_rockbox/download/__init__.py
--rw-r--r--   0        0        0    31047 2024-04-21 08:58:06.508173 spotdl_rockbox-4.2.6/spotdl_rockbox/download/downloader.py
--rw-r--r--   0        0        0    13148 2024-04-21 08:58:06.202535 spotdl_rockbox-4.2.6/spotdl_rockbox/download/progress_handler.py
--rw-r--r--   0        0        0       54 2024-04-21 08:10:32.063249 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/__init__.py
--rw-r--r--   0        0        0      725 2024-04-21 08:58:06.658161 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/__init__.py
--rw-r--r--   0        0        0     6307 2024-04-21 08:58:06.417368 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/bandcamp.py
--rw-r--r--   0        0        0    12168 2024-04-21 08:58:06.324813 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/base.py
--rw-r--r--   0        0        0     5339 2024-04-21 08:58:06.227820 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/piped.py
--rw-r--r--   0        0        0     2801 2024-04-21 08:58:06.713153 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/sliderkz.py
--rw-r--r--   0        0        0     2848 2024-04-21 08:58:06.470970 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/soundcloud.py
--rw-r--r--   0        0        0     1856 2024-04-21 08:58:06.165447 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/youtube.py
--rw-r--r--   0        0        0     2869 2024-04-21 08:58:06.551703 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/ytmusic.py
--rw-r--r--   0        0        0      422 2024-04-21 08:58:06.285507 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/__init__.py
--rw-r--r--   0        0        0     3829 2024-04-21 08:58:06.133656 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/azlyrics.py
--rw-r--r--   0        0        0     3874 2024-04-21 08:58:06.350412 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/base.py
--rw-r--r--   0        0        0     3443 2024-04-21 08:58:06.117623 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/genius.py
--rw-r--r--   0        0        0     3033 2024-04-21 08:58:06.342861 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/musixmatch.py
--rw-r--r--   0        0        0     2309 2024-04-21 08:58:06.520722 spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/synced.py
--rw-r--r--   0        0        0       38 2024-04-21 08:10:32.071415 spotdl_rockbox-4.2.6/spotdl_rockbox/types/__init__.py
--rw-r--r--   0        0        0     3640 2024-04-21 08:54:19.592091 spotdl_rockbox-4.2.6/spotdl_rockbox/types/album.py
--rw-r--r--   0        0        0     3132 2024-04-21 08:58:06.438091 spotdl_rockbox-4.2.6/spotdl_rockbox/types/artist.py
--rw-r--r--   0        0        0     4652 2024-04-21 08:10:32.073462 spotdl_rockbox-4.2.6/spotdl_rockbox/types/options.py
--rw-r--r--   0        0        0     4622 2024-04-21 08:58:06.622462 spotdl_rockbox-4.2.6/spotdl_rockbox/types/playlist.py
--rw-r--r--   0        0        0     2187 2024-04-21 08:10:32.074551 spotdl_rockbox-4.2.6/spotdl_rockbox/types/result.py
--rw-r--r--   0        0        0     3351 2024-04-21 08:10:32.074551 spotdl_rockbox-4.2.6/spotdl_rockbox/types/saved.py
--rw-r--r--   0        0        0    10343 2024-04-21 08:58:06.271422 spotdl_rockbox-4.2.6/spotdl_rockbox/types/song.py
--rw-r--r--   0        0        0      103 2024-04-21 08:10:32.076554 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/__init__.py
--rw-r--r--   0        0        0     1001 2024-04-21 08:10:32.076554 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/archive.py
--rw-r--r--   0        0        0    22908 2024-04-21 08:49:05.109376 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/arguments.py
--rw-r--r--   0        0        0     8310 2024-04-21 08:49:21.340072 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/config.py
--rw-r--r--   0        0        0     3141 2024-04-21 08:55:55.038705 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/console.py
--rw-r--r--   0        0        0      579 2024-04-21 08:49:59.616753 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/downloader.py
--rw-r--r--   0        0        0    12046 2024-04-21 08:50:07.334761 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/ffmpeg.py
--rw-r--r--   0        0        0    17914 2024-04-21 08:50:17.666572 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/formatter.py
--rw-r--r--   0        0        0     5605 2024-04-21 08:10:32.080304 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/logging.py
--rw-r--r--   0        0        0     1205 2024-04-21 08:50:31.807959 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/lrc.py
--rw-r--r--   0        0        0     5099 2024-04-21 08:50:37.028317 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/m3u.py
--rw-r--r--   0        0        0    23106 2024-04-21 08:50:47.530339 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/matching.py
--rw-r--r--   0        0        0    19529 2024-04-21 08:50:57.292888 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/metadata.py
--rw-r--r--   0        0        0    23666 2024-04-21 08:51:09.200552 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/search.py
--rw-r--r--   0        0        0     6975 2024-04-21 08:51:14.952780 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/spotify.py
--rw-r--r--   0        0        0    28221 2024-04-21 08:10:32.084160 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/static.py
--rw-r--r--   0        0        0    16513 2024-04-21 08:52:42.082765 spotdl_rockbox-4.2.6/spotdl_rockbox/utils/web.py
--rw-r--r--   0        0        0     8451 1970-01-01 00:00:00.000000 spotdl_rockbox-4.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-21 08:10:32.037891 spotdl_rockbox-4.2.7/LICENSE
+-rw-r--r--   0        0        0     2815 2024-04-21 09:04:14.647777 spotdl_rockbox-4.2.7/pyproject.toml
+-rw-r--r--   0        0        0     6337 2024-04-21 08:10:32.038891 spotdl_rockbox-4.2.7/README.md
+-rw-r--r--   0        0        0     4977 2024-04-21 08:52:55.439012 spotdl_rockbox-4.2.7/spotdl_rockbox/__init__.py
+-rw-r--r--   0        0        0      225 2024-04-21 08:53:01.968536 spotdl_rockbox-4.2.7/spotdl_rockbox/__main__.py
+-rw-r--r--   0        0        0       58 2024-04-21 08:10:32.056290 spotdl_rockbox-4.2.7/spotdl_rockbox/_version.py
+-rw-r--r--   0        0        0      194 2024-04-21 08:58:06.601510 spotdl_rockbox-4.2.7/spotdl_rockbox/console/__init__.py
+-rw-r--r--   0        0        0      824 2024-04-21 08:58:06.279478 spotdl_rockbox-4.2.7/spotdl_rockbox/console/download.py
+-rw-r--r--   0        0        0     5486 2024-04-21 09:03:20.342904 spotdl_rockbox-4.2.7/spotdl_rockbox/console/entry_point.py
+-rw-r--r--   0        0        0     6902 2024-04-21 08:58:06.564198 spotdl_rockbox-4.2.7/spotdl_rockbox/console/meta.py
+-rw-r--r--   0        0        0     3257 2024-04-21 08:58:06.190782 spotdl_rockbox-4.2.7/spotdl_rockbox/console/save.py
+-rw-r--r--   0        0        0     5702 2024-04-21 08:58:06.527767 spotdl_rockbox-4.2.7/spotdl_rockbox/console/sync.py
+-rw-r--r--   0        0        0     1941 2024-04-21 08:58:06.650649 spotdl_rockbox-4.2.7/spotdl_rockbox/console/url.py
+-rw-r--r--   0        0        0     3675 2024-04-21 08:58:06.152808 spotdl_rockbox-4.2.7/spotdl_rockbox/console/web.py
+-rw-r--r--   0        0        0       80 2024-04-21 08:10:32.061006 spotdl_rockbox-4.2.7/spotdl_rockbox/download/__init__.py
+-rw-r--r--   0        0        0    31151 2024-04-21 09:03:20.226328 spotdl_rockbox-4.2.7/spotdl_rockbox/download/downloader.py
+-rw-r--r--   0        0        0    13148 2024-04-21 08:58:06.202535 spotdl_rockbox-4.2.7/spotdl_rockbox/download/progress_handler.py
+-rw-r--r--   0        0        0       54 2024-04-21 08:10:32.063249 spotdl_rockbox-4.2.7/spotdl_rockbox/providers/__init__.py
+-rw-r--r--   0        0        0      725 2024-04-21 08:58:06.658161 spotdl_rockbox-4.2.7/spotdl_rockbox/providers/audio/__init__.py
+-rw-r--r--   0        0        0     6307 2024-04-21 08:58:06.417368 spotdl_rockbox-4.2.7/spotdl_rockbox/providers/audio/bandcamp.py
+-rw-r--r--   0        0        0    12168 2024-04-21 08:58:06.324813 spotdl_rockbox-4.2.7/spotdl_rockbox/providers/audio/base.py
+-rw-r--r--   0        0        0     5339 2024-04-21 08:58:06.227820 spotdl_rockbox-4.2.7/spotdl_rockbox/providers/audio/piped.py
+-rw-r--r--   0        0        0     2801 2024-04-21 08:58:06.713153 spotdl_rockbox-4.2.7/spotdl_rockbox/providers/audio/sliderkz.py
+-rw-r--r--   0        0        0     2848 2024-04-21 08:58:06.470970 spotdl_rockbox-4.2.7/spotdl_rockbox/providers/audio/soundcloud.py
+-rw-r--r--   0        0        0     1856 2024-04-21 08:58:06.165447 spotdl_rockbox-4.2.7/spotdl_rockbox/providers/audio/youtube.py
+-rw-r--r--   0        0        0     2869 2024-04-21 08:58:06.551703 spotdl_rockbox-4.2.7/spotdl_rockbox/providers/audio/ytmusic.py
+-rw-r--r--   0        0        0      422 2024-04-21 08:58:06.285507 spotdl_rockbox-4.2.7/spotdl_rockbox/providers/lyrics/__init__.py
+-rw-r--r--   0        0        0     3829 2024-04-21 08:58:06.133656 spotdl_rockbox-4.2.7/spotdl_rockbox/providers/lyrics/azlyrics.py
+-rw-r--r--   0        0        0     3874 2024-04-21 08:58:06.350412 spotdl_rockbox-4.2.7/spotdl_rockbox/providers/lyrics/base.py
+-rw-r--r--   0        0        0     3443 2024-04-21 08:58:06.117623 spotdl_rockbox-4.2.7/spotdl_rockbox/providers/lyrics/genius.py
+-rw-r--r--   0        0        0     3033 2024-04-21 08:58:06.342861 spotdl_rockbox-4.2.7/spotdl_rockbox/providers/lyrics/musixmatch.py
+-rw-r--r--   0        0        0     2309 2024-04-21 08:58:06.520722 spotdl_rockbox-4.2.7/spotdl_rockbox/providers/lyrics/synced.py
+-rw-r--r--   0        0        0       38 2024-04-21 08:10:32.071415 spotdl_rockbox-4.2.7/spotdl_rockbox/types/__init__.py
+-rw-r--r--   0        0        0     3640 2024-04-21 08:54:19.592091 spotdl_rockbox-4.2.7/spotdl_rockbox/types/album.py
+-rw-r--r--   0        0        0     3132 2024-04-21 08:58:06.438091 spotdl_rockbox-4.2.7/spotdl_rockbox/types/artist.py
+-rw-r--r--   0        0        0     4652 2024-04-21 08:10:32.073462 spotdl_rockbox-4.2.7/spotdl_rockbox/types/options.py
+-rw-r--r--   0        0        0     4622 2024-04-21 08:58:06.622462 spotdl_rockbox-4.2.7/spotdl_rockbox/types/playlist.py
+-rw-r--r--   0        0        0     2187 2024-04-21 08:10:32.074551 spotdl_rockbox-4.2.7/spotdl_rockbox/types/result.py
+-rw-r--r--   0        0        0     3367 2024-04-21 09:03:20.490757 spotdl_rockbox-4.2.7/spotdl_rockbox/types/saved.py
+-rw-r--r--   0        0        0    10343 2024-04-21 08:58:06.271422 spotdl_rockbox-4.2.7/spotdl_rockbox/types/song.py
+-rw-r--r--   0        0        0      103 2024-04-21 08:10:32.076554 spotdl_rockbox-4.2.7/spotdl_rockbox/utils/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-21 08:10:32.076554 spotdl_rockbox-4.2.7/spotdl_rockbox/utils/archive.py
+-rw-r--r--   0        0        0    22908 2024-04-21 08:49:05.109376 spotdl_rockbox-4.2.7/spotdl_rockbox/utils/arguments.py
+-rw-r--r--   0        0        0     8310 2024-04-21 08:49:21.340072 spotdl_rockbox-4.2.7/spotdl_rockbox/utils/config.py
+-rw-r--r--   0        0        0     3141 2024-04-21 08:55:55.038705 spotdl_rockbox-4.2.7/spotdl_rockbox/utils/console.py
+-rw-r--r--   0        0        0      579 2024-04-21 08:49:59.616753 spotdl_rockbox-4.2.7/spotdl_rockbox/utils/downloader.py
+-rw-r--r--   0        0        0    12046 2024-04-21 08:50:07.334761 spotdl_rockbox-4.2.7/spotdl_rockbox/utils/ffmpeg.py
+-rw-r--r--   0        0        0    17914 2024-04-21 08:50:17.666572 spotdl_rockbox-4.2.7/spotdl_rockbox/utils/formatter.py
+-rw-r--r--   0        0        0     5605 2024-04-21 08:10:32.080304 spotdl_rockbox-4.2.7/spotdl_rockbox/utils/logging.py
+-rw-r--r--   0        0        0     1205 2024-04-21 08:50:31.807959 spotdl_rockbox-4.2.7/spotdl_rockbox/utils/lrc.py
+-rw-r--r--   0        0        0     5099 2024-04-21 08:50:37.028317 spotdl_rockbox-4.2.7/spotdl_rockbox/utils/m3u.py
+-rw-r--r--   0        0        0    23106 2024-04-21 08:50:47.530339 spotdl_rockbox-4.2.7/spotdl_rockbox/utils/matching.py
+-rw-r--r--   0        0        0    19529 2024-04-21 08:50:57.292888 spotdl_rockbox-4.2.7/spotdl_rockbox/utils/metadata.py
+-rw-r--r--   0        0        0    23666 2024-04-21 08:51:09.200552 spotdl_rockbox-4.2.7/spotdl_rockbox/utils/search.py
+-rw-r--r--   0        0        0     6975 2024-04-21 08:51:14.952780 spotdl_rockbox-4.2.7/spotdl_rockbox/utils/spotify.py
+-rw-r--r--   0        0        0    28221 2024-04-21 08:10:32.084160 spotdl_rockbox-4.2.7/spotdl_rockbox/utils/static.py
+-rw-r--r--   0        0        0    16513 2024-04-21 08:52:42.082765 spotdl_rockbox-4.2.7/spotdl_rockbox/utils/web.py
+-rw-r--r--   0        0        0     8451 1970-01-01 00:00:00.000000 spotdl_rockbox-4.2.7/PKG-INFO
```

### Comparing `spotdl_rockbox-4.2.6/LICENSE` & `spotdl_rockbox-4.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/pyproject.toml` & `spotdl_rockbox-4.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotdl_rockbox"
-version = "4.2.6"
+version = "4.2.7"
 description = "Fox for rockbox. Download your Spotify playlists and songs along with album art and metadata"
 license = "MIT"
 authors = ["spotDL Team <spotdladmins@googlegroups.com>", "MisteryDush <ikrom.arifdjanov@gmail.com>"]
 maintainers = ["xnetcat <xnetcat.dev@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/MisteryDush/spotify-downloader-rockbox.git"
 homepage = "https://github.com/spotDL/spotify-downloader/"
```

### Comparing `spotdl_rockbox-4.2.6/README.md` & `spotdl_rockbox-4.2.7/README.md`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/__init__.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/__init__.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/console/download.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/console/download.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/console/entry_point.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/console/entry_point.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 import time
 
 from spotdl_rockbox.console.download import download
 from spotdl_rockbox.console.meta import meta
 from spotdl_rockbox.console.save import save
 from spotdl_rockbox.console.sync import sync
 from spotdl_rockbox.console.url import url
-from spotdl.console.web import web
-from spotdl.download.downloader import Downloader, DownloaderError
-from spotdl.utils.arguments import parse_arguments
-from spotdl.utils.config import create_settings
-from spotdl.utils.console import ACTIONS, generate_initial_config, is_executable
-from spotdl.utils.downloader import check_ytmusic_connection
-from spotdl.utils.ffmpeg import FFmpegError, download_ffmpeg, is_ffmpeg_installed
-from spotdl.utils.logging import init_logging
-from spotdl.utils.spotify import SpotifyClient, SpotifyError, save_spotify_cache
+from spotdl_rockbox.console.web import web
+from spotdl_rockbox.download.downloader import Downloader, DownloaderError
+from spotdl_rockbox.utils.arguments import parse_arguments
+from spotdl_rockbox.utils.config import create_settings
+from spotdl_rockbox.utils.console import ACTIONS, generate_initial_config, is_executable
+from spotdl_rockbox.utils.downloader import check_ytmusic_connection
+from spotdl_rockbox.utils.ffmpeg import FFmpegError, download_ffmpeg, is_ffmpeg_installed
+from spotdl_rockbox.utils.logging import init_logging
+from spotdl_rockbox.utils.spotify import SpotifyClient, SpotifyError, save_spotify_cache
 
 __all__ = ["console_entry_point", "OPERATIONS"]
 
 OPERATIONS = {
     "download": download,
     "sync": sync,
     "save": save,
```

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/console/meta.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/console/meta.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/console/save.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/console/save.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/console/sync.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/console/sync.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/console/url.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/console/url.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/console/web.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/console/web.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/download/downloader.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/download/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,41 +14,41 @@
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Type, Union
 
 from yt_dlp.postprocessor.modify_chapters import ModifyChaptersPP
 from yt_dlp.postprocessor.sponsorblock import SponsorBlockPP
 
 from spotdl_rockbox.download.progress_handler import ProgressHandler
-from spotdl.providers.audio import (
+from spotdl_rockbox.providers.audio import (
     AudioProvider,
     BandCamp,
     Piped,
     SliderKZ,
     SoundCloud,
     YouTube,
     YouTubeMusic,
 )
-from spotdl.providers.lyrics import AzLyrics, Genius, LyricsProvider, MusixMatch, Synced
-from spotdl.types.options import DownloaderOptionalOptions, DownloaderOptions
-from spotdl.types.song import Song
-from spotdl.utils.archive import Archive
-from spotdl.utils.config import (
+from spotdl_rockbox.providers.lyrics import AzLyrics, Genius, LyricsProvider, MusixMatch, Synced
+from spotdl_rockbox.types.options import DownloaderOptionalOptions, DownloaderOptions
+from spotdl_rockbox.types.song import Song
+from spotdl_rockbox.utils.archive import Archive
+from spotdl_rockbox.utils.config import (
     DOWNLOADER_OPTIONS,
     GlobalConfig,
     create_settings_type,
     get_errors_path,
     get_temp_path,
     modernize_settings,
 )
-from spotdl.utils.ffmpeg import FFmpegError, convert, get_ffmpeg_path
-from spotdl.utils.formatter import create_file_name
-from spotdl.utils.lrc import generate_lrc
-from spotdl.utils.m3u import gen_m3u_files
-from spotdl.utils.metadata import MetadataError, embed_metadata
-from spotdl.utils.search import gather_known_songs, reinit_song, songs_from_albums
+from spotdl_rockbox.utils.ffmpeg import FFmpegError, convert, get_ffmpeg_path
+from spotdl_rockbox.utils.formatter import create_file_name
+from spotdl_rockbox.utils.lrc import generate_lrc
+from spotdl_rockbox.utils.m3u import gen_m3u_files
+from spotdl_rockbox.utils.metadata import MetadataError, embed_metadata
+from spotdl_rockbox.utils.search import gather_known_songs, reinit_song, songs_from_albums
 
 __all__ = [
     "AUDIO_PROVIDERS",
     "LYRICS_PROVIDERS",
     "Downloader",
     "DownloaderError",
     "SPONSOR_BLOCK_CATEGORIES",
@@ -115,15 +115,15 @@
             the next provider in the list will be used.
         """
 
         if settings is None:
             settings = {}
 
         # Create settings dictionary, fill in missing values with defaults
-        # from spotdl.types.options.DOWNLOADER_OPTIONS
+        # from spotdl_rockbox.types.options.DOWNLOADER_OPTIONS
         self.settings: DownloaderOptions = DownloaderOptions(
             **create_settings_type(
                 Namespace(config=False), dict(settings), DOWNLOADER_OPTIONS
             )  # type: ignore
         )
 
         # Handle deprecated values in config file
```

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/download/progress_handler.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/download/progress_handler.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/__init__.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/providers/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/bandcamp.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/providers/audio/bandcamp.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/base.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/providers/audio/base.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/piped.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/providers/audio/piped.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/sliderkz.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/providers/audio/sliderkz.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/soundcloud.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/providers/audio/soundcloud.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/youtube.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/providers/audio/youtube.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/audio/ytmusic.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/providers/audio/ytmusic.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/azlyrics.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/providers/lyrics/azlyrics.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/base.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/providers/lyrics/base.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/genius.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/providers/lyrics/genius.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/musixmatch.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/providers/lyrics/musixmatch.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/providers/lyrics/synced.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/providers/lyrics/synced.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/types/album.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/types/album.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/types/artist.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/types/artist.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/types/options.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/types/options.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/types/playlist.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/types/playlist.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/types/result.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/types/result.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/types/saved.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/types/saved.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Saved module for handing the saved tracks from user library
 """
 
 from dataclasses import dataclass
 from typing import Any, Dict, List, Tuple
 
-from spotdl.types.song import Song, SongList
-from spotdl.utils.spotify import SpotifyClient
+from spotdl_rockbox.types.song import Song, SongList
+from spotdl_rockbox.utils.spotify import SpotifyClient
 
 __all__ = ["Saved", "SavedError"]
 
 
 class SavedError(Exception):
     """
     Base class for all exceptions related to saved tracks.
```

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/types/song.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/types/song.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/archive.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/utils/archive.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/arguments.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/utils/arguments.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/config.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/utils/config.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/console.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/utils/console.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/downloader.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/ffmpeg.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/utils/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/formatter.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/logging.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/utils/logging.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/lrc.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/utils/lrc.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/m3u.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/utils/m3u.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/matching.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/utils/matching.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/metadata.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/utils/metadata.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/search.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/utils/search.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/spotify.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/utils/spotify.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/static.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/utils/static.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/spotdl_rockbox/utils/web.py` & `spotdl_rockbox-4.2.7/spotdl_rockbox/utils/web.py`

 * *Files identical despite different names*

### Comparing `spotdl_rockbox-4.2.6/PKG-INFO` & `spotdl_rockbox-4.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotdl_rockbox
-Version: 4.2.6
+Version: 4.2.7
 Summary: Fox for rockbox. Download your Spotify playlists and songs along with album art and metadata
 Home-page: https://github.com/spotDL/spotify-downloader/
 License: MIT
 Keywords: spotify,downloader,spotdl,music
 Author: spotDL Team
 Author-email: spotdladmins@googlegroups.com
 Maintainer: xnetcat
```

