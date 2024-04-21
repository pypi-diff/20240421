# Comparing `tmp/muxtools-0.0.9.tar.gz` & `tmp/muxtools-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muxtools-0.0.9.tar", last modified: Mon Oct 30 21:09:35 2023, max compression
+gzip compressed data, was "muxtools-0.1.0.tar", last modified: Sun Apr 21 19:26:30 2024, max compression
```

## Comparing `muxtools-0.0.9.tar` & `muxtools-0.1.0.tar`

### file list

```diff
@@ -1,53 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 21:09:35.899859 muxtools-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2023-10-30 21:09:21.000000 muxtools-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2023-10-30 21:09:35.899859 muxtools-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      601 2023-10-30 21:09:21.000000 muxtools-0.0.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 21:09:35.895859 muxtools-0.0.9/muxtools/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 21:09:35.895859 muxtools-0.0.9/muxtools/audio/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11281 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/audio/audioutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16728 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/audio/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    16909 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/audio/extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)     9051 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/audio/memecoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     8982 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/audio/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/audio/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7933 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 21:09:35.895859 muxtools-0.0.9/muxtools/misc/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9554 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/misc/chapters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 21:09:35.895859 muxtools-0.0.9/muxtools/muxing/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/muxing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/muxing/mux.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/muxing/muxfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6371 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/muxing/tmdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     8498 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/muxing/tracks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 21:09:35.899859 muxtools-0.0.9/muxtools/subtitle/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/subtitle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/subtitle/font.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/subtitle/styles.py
--rw-r--r--   0 runner    (1001) docker     (127)    32085 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/subtitle/sub.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/subtitle/subutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 21:09:35.899859 muxtools-0.0.9/muxtools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4425 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6088 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/utils/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/utils/glob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     8194 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/utils/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2023-10-30 21:09:21.000000 muxtools-0.0.9/muxtools/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 21:09:35.895859 muxtools-0.0.9/muxtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2023-10-30 21:09:35.000000 muxtools-0.0.9/muxtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-10-30 21:09:35.000000 muxtools-0.0.9/muxtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 21:09:35.000000 muxtools-0.0.9/muxtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-10-30 21:09:35.000000 muxtools-0.0.9/muxtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-10-30 21:09:35.000000 muxtools-0.0.9/muxtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-30 21:09:35.000000 muxtools-0.0.9/muxtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-10-30 21:09:21.000000 muxtools-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-30 21:09:35.899859 muxtools-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:26:30.439458 muxtools-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-21 19:26:22.000000 muxtools-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-21 19:26:30.439458 muxtools-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-21 19:26:22.000000 muxtools-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:26:30.431458 muxtools-0.1.0/muxtools/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:26:30.435458 muxtools-0.1.0/muxtools/audio/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13464 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/audio/audioutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16898 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/audio/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17130 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/audio/extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9131 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/audio/memecoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9081 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/audio/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/audio/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:26:30.435458 muxtools-0.1.0/muxtools/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9993 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/misc/chapters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:26:30.435458 muxtools-0.1.0/muxtools/muxing/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/muxing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8334 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/muxing/mux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/muxing/muxfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10149 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/muxing/tmdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/muxing/tracks.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:26:30.435458 muxtools-0.1.0/muxtools/subtitle/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/subtitle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7138 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/subtitle/basesub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/subtitle/font.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/subtitle/styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31928 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/subtitle/sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/subtitle/subutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:26:30.439458 muxtools-0.1.0/muxtools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/utils/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/utils/glob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/utils/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/utils/subprogress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-21 19:26:22.000000 muxtools-0.1.0/muxtools/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:26:30.439458 muxtools-0.1.0/muxtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-21 19:26:30.000000 muxtools-0.1.0/muxtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-21 19:26:30.000000 muxtools-0.1.0/muxtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:26:30.000000 muxtools-0.1.0/muxtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-21 19:26:30.000000 muxtools-0.1.0/muxtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-21 19:26:30.000000 muxtools-0.1.0/muxtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 19:26:30.000000 muxtools-0.1.0/muxtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-21 19:26:22.000000 muxtools-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:26:30.439458 muxtools-0.1.0/setup.cfg
```

### Comparing `muxtools-0.0.9/LICENSE` & `muxtools-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.9/PKG-INFO` & `muxtools-0.1.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muxtools
-Version: 0.0.9
+Version: 0.1.0
 Summary: A library for various muxing and automation tools for anything and everything fansubbing related
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Vodes/muxtools
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -30,15 +30,15 @@
 
 # muxtools
 
 A library for various muxing and automation tools for anything and everything fansubbing related
 
 ## How do I use this?
 
-You might wanna check out the [wiki](https://github.com/Irrational-Encoding-Wizardry/vs-muxtools/wiki) in the [vs-muxtools](https://github.com/Irrational-Encoding-Wizardry/vs-muxtools) repo.
+You might wanna check out the [guide/wiki](https://muxtools.vodes.pw/).
 
 ## Installation
 
 Git is always the most updated one obviously but I can't guarantee that everything is in a working state.
 
 You can also grab the latest stable ish versions from pip.
```

### Comparing `muxtools-0.0.9/muxtools/__init__.py` & `muxtools-0.1.0/muxtools/__init__.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.9/muxtools/audio/audioutils.py` & `muxtools-0.1.0/muxtools/audio/audioutils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import os
 import re
 import subprocess
-from typing import Sequence
+from datetime import timedelta
+from typing import Any
+from collections.abc import Sequence
 
 from pymediainfo import Track, MediaInfo
 
 from .preprocess import Preprocessor, Resample
-from ..utils.files import make_output
+from ..utils.files import make_output, ensure_path_exists
 from ..muxing.muxfiles import AudioFile
 from ..utils.log import debug, warn, error
 from ..utils.download import get_executable
 from ..utils.env import get_temp_workdir, run_commandline
-from ..utils.types import DitherType, Trim, AudioFormat, ValidInputType
+from ..utils.types import DitherType, Trim, AudioFormat, ValidInputType, PathLike
+from ..utils.subprogress import run_cmd_pb, ProgressBarConfig
 
 __all__ = ["ensure_valid_in", "sanitize_trims", "format_from_track", "is_fancy_codec", "has_libFLAC", "has_libFDK"]
 
 
 def sanitize_pre(preprocess: Preprocessor | Sequence[Preprocessor] | None = None) -> list[Preprocessor]:
     if not preprocess:
         return []
@@ -23,15 +26,15 @@
 
 
 def ensure_valid_in(
     fileIn: AudioFile,
     supports_pipe: bool = True,
     preprocess: Preprocessor | Sequence[Preprocessor] | None = None,
     valid_type: ValidInputType = ValidInputType.FLAC,
-    caller: any = None,
+    caller: Any = None,
 ) -> AudioFile | subprocess.Popen:
     """
     Ensures valid input for any encoder that accepts flac (all of them).
     Passes existing file if no need to dither and is either wav or flac.
     """
     if fileIn.has_multiple_tracks(caller):
         msg = f"'{fileIn.file.name}' is a container with multiple tracks.\n"
@@ -67,21 +70,39 @@
             return FF_FLAC(compression_level=0, preprocess=preprocess, output=os.path.join(get_temp_workdir(), "tempflac")).encode_audio(
                 fileIn, temp=True
             )
     else:
         return get_pcm(fileIn, trackinfo, supports_pipe, preprocess, valid_type, caller)
 
 
+def get_preprocess_args(
+    fileIn: AudioFile, preprocessors: Preprocessor | Sequence[Preprocessor] | None, mediainfo: Track, caller: Any = None
+) -> list[str]:
+    preprocessors = sanitize_pre(preprocessors)
+    args = list[str]()
+    if any([p.can_run(mediainfo, preprocessors) for p in preprocessors]):
+        filters = list[str]()
+        for pre in [p for p in preprocessors if p.can_run(mediainfo, preprocessors)]:
+            pre.analyze(fileIn)
+            args.extend(pre.get_args(caller=caller))
+            filt = pre.get_filter(caller=caller)
+            if filt:
+                filters.append(filt)
+        if filters:
+            args.extend(["-filter:a", ",".join(filters)])
+    return args
+
+
 def get_pcm(
     fileIn: AudioFile,
     minfo: Track,
     supports_pipe: bool = True,
     preprocess: Sequence[Preprocessor] | None = None,
     valid_type: ValidInputType = ValidInputType.RF64,
-    caller: any = None,
+    caller: Any = None,
 ) -> AudioFile | subprocess.Popen:
     ffmpeg = get_executable("ffmpeg")
     args = [ffmpeg, "-i", str(fileIn.file), "-map", "0:a:0"]
     cope = "pcm_s24be" if valid_type == ValidInputType.AIFF else "pcm_s24le"
     codec = "pcm_s16le" if getattr(minfo, "bit_depth", 16) == 16 else cope
     filters = list[str]()
     preprocess = sanitize_pre(preprocess)
@@ -108,22 +129,22 @@
         debug(f"Piping audio to ensure valid input using ffmpeg...", caller)
         args.extend(["-f", "aiff" if valid_type == ValidInputType.AIFF else "w64", "-"])
         p = subprocess.Popen(args, stdin=subprocess.DEVNULL, stdout=subprocess.PIPE, stderr=subprocess.DEVNULL, text=False)
         return p
     else:
         debug(f"Preparing audio to ensure valid input using ffmpeg...", caller)
         args.append(str(output))
-        if not run_commandline(args):
+        if not run_cmd_pb(args, pbc=ProgressBarConfig("Preparing...", duration_from_file(fileIn))):
             return AudioFile(output, fileIn.container_delay, fileIn.source)
         else:
             raise error("Failed to convert to desired intermediary!", ensure_valid_in)
 
 
 def sanitize_trims(
-    trims: Trim | list[Trim], total_frames: int = 0, uses_frames: bool = True, allow_negative_start: bool = False, caller: any = None
+    trims: Trim | list[Trim], total_frames: int = 0, uses_frames: bool = True, allow_negative_start: bool = False, caller: Any = None
 ) -> list[Trim]:
     caller = caller if caller else sanitize_trims
     if not isinstance(trims, (list, tuple)):
         raise error("Trims must be a list of 2-tuples (or just one 2-tuple)", caller)
     if not isinstance(trims, list):
         trims = [trims]
     for index, trim in enumerate(trims):
@@ -137,15 +158,15 @@
         if trim[-1] == 0:
             raise error("Slices cannot end with 0, if attempting to use an empty slice, use `None`", caller)
 
         if trim[0] and trim[0] < 0 and not allow_negative_start and index == 0:
             raise error("The first part of a trim cannot be negative.", caller)
 
         has_negative = (trim[1] is not None and trim[1] < 0) or (trim[0] is not None and trim[0] < 0)
-        if not uses_frames and has_negative:
+        if not uses_frames and has_negative and index != 0:
             raise error(f"If you use milliseconds to trim you cannot use negative values.")
 
         if not total_frames and has_negative:
             raise error(f"If you want to use negative trims you gotta pass a total frame number.")
 
         if trim[1] is not None and trim[1] < 0:
             trim = (trim[0], total_frames + trim[1])
@@ -165,28 +186,33 @@
     # Lossy
     AudioFormat("AC-3",         "ac3",      "A_AC3"),
     AudioFormat("E-AC-3",       "eac3",     "A_EAC3"),
     AudioFormat("AAC*",         "m4a",      "A_AAC*"), # Lots of different AAC formats idk what they mean, don't care either
     AudioFormat("Opus",         "opus",     "A_OPUS"),
     AudioFormat("Vorbis",       "ogg",      "A_VORBIS"),
     AudioFormat("/",            "mp3",      "mp4a-6B"), # MP3 has the format name split up into 3 variables so we're gonna ignore this
-    
+
     # Lossless
     AudioFormat("FLAC",         "flac",     "A_FLAC", False),
     AudioFormat("MLP FBA*",     "thd",      "A_TRUEHD", False), # Atmos stuff has some more shit in the format name
     AudioFormat("PCM*",         "wav",      "A_PCM*", False),
 
     # Disgusting DTS Stuff
     AudioFormat("DTS XLL*",     "dtshd",    "A_DTS", False), # Can be HD-MA or Headphone X or X, who the fuck knows
     AudioFormat("DTS",          "dts",      "A_DTS"), # Can be lossy
 ]
 # fmt: on
 
 
 def format_from_track(track: Track) -> AudioFormat | None:
+    comm_name = getattr(track, "commercial_name", None)
+    compression_mode = str(getattr(track, "compression_mode", ""))
+    if comm_name and str(comm_name).lower() == "dts" and compression_mode.lower() == "lossy":
+        return formats[-1]
+
     for format in formats:
         f = str(track.format)
         if hasattr(track, "format_additionalfeatures") and track.format_additionalfeatures:
             f = f"{f} {track.format_additionalfeatures}"
         if "*" in format.format:
             # matches = filter([f.lower()], format.format.lower())
             if re.match(format.format.replace("*", ".*"), f, re.IGNORECASE):
@@ -201,14 +227,47 @@
                 return format
         else:
             if format.codecid.casefold() == str(track.codec_id).casefold():
                 return format
     return None
 
 
+def duration_from_file(fileIn: PathLike | AudioFile, track: int = 0, caller: Any = None) -> timedelta:
+    from ..utils.parsing import timedelta_from_formatted
+
+    if isinstance(fileIn, AudioFile):
+        if fileIn.duration:
+            return fileIn.duration
+        else:
+            fileIn = fileIn.file
+
+    args = [
+        get_executable("ffprobe"),
+        "-v",
+        "error",
+        "-select_streams",
+        str(track),
+        "-show_entries",
+        "format=duration",
+        "-of",
+        "default=noprint_wrappers=1:nokey=1",
+        "-sexagesimal",
+        str(ensure_path_exists(fileIn, duration_from_file)),
+    ]
+
+    try:
+        p = subprocess.run(args, capture_output=True, text=True)
+        if p.returncode != 0:
+            raise Exception("Failed to parse")
+        return timedelta_from_formatted((p.stderr + p.stdout).strip())
+    except:
+        warn("Could not parse duration from track. Will assume 24 minutes.", caller)
+        return timedelta(minutes=24)
+
+
 def is_fancy_codec(track: Track) -> bool:
     """
     Tries to check if a track is some fancy DTS (X, Headphone X) or TrueHD with Atmos
 
     :param track:   Input track to check
     """
     codec_id = str(track.codec_id).casefold()
```

### Comparing `muxtools-0.0.9/muxtools/audio/encoders.py` & `muxtools-0.1.0/muxtools/audio/encoders.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from shlex import split as splitcommand
 from dataclasses import dataclass, field
-from typing import Sequence
+from collections.abc import Sequence
 import subprocess
 import os
 
 from .tools import Encoder, LosslessEncoder
 from .preprocess import Preprocessor, Resample, Downmix
 from ..muxing.muxfiles import AudioFile
 from ..utils.env import run_commandline
 from ..utils.download import get_executable
 from ..utils.log import warn, crit, debug, error
 from ..utils.files import make_output, clean_temp_files
-from ..utils.types import DitherType, ValidInputType, qAAC_MODE, PathLike
-from .audioutils import ensure_valid_in, has_libFDK, qaac_compatcheck, sanitize_pre
+from ..utils.types import ValidInputType, qAAC_MODE, PathLike
+from ..utils.subprogress import run_cmd_pb, ProgressBarConfig
+from .audioutils import ensure_valid_in, has_libFDK, qaac_compatcheck, duration_from_file, get_preprocess_args, sanitize_pre
 
 __all__ = ["FLAC", "FLACCL", "FF_FLAC", "Opus", "qAAC", "FDK_AAC"]
 
 
 @dataclass
 class FLAC(LosslessEncoder):
     """
@@ -32,35 +33,34 @@
 
     compression_level: int = 8
     preprocess: Preprocessor | Sequence[Preprocessor] | None = field(default_factory=Resample)
     verify: bool = True
     append: str = ""
     output: PathLike | None = None
 
-    def encode_audio(self, input: AudioFile, quiet: bool = True, **kwargs) -> AudioFile:
-        if not isinstance(input, AudioFile):
-            input = AudioFile.from_file(input, self)
+    def encode_audio(self, fileIn: AudioFile | PathLike, quiet: bool = True, **kwargs) -> AudioFile:
+        if not isinstance(fileIn, AudioFile):
+            fileIn = AudioFile.from_file(fileIn, self)
         flac = get_executable("flac")
-        output = make_output(input.file, "flac", "libflac", self.output)
-        source = ensure_valid_in(input, preprocess=self.preprocess, caller=self, valid_type=ValidInputType.W64_OR_FLAC, supports_pipe=False)
-        debug(f"Encoding '{input.file.stem}' to FLAC using libFLAC...", self)
+        output = make_output(fileIn.file, "flac", "libflac", self.output)
+        source = ensure_valid_in(fileIn, preprocess=self.preprocess, caller=self, valid_type=ValidInputType.W64_OR_FLAC, supports_pipe=False)
+        debug(f"Encoding '{fileIn.file.stem}' to FLAC using libFLAC...", self)
 
         args = [flac, f"-{self.compression_level}", "-o", str(output)]
         if self.verify:
             args.append("--verify")
         if self.append:
             args.extend(splitcommand(self.append))
         args.append(str(source.file.resolve()) if isinstance(source, AudioFile) else "-")
 
         stdin = subprocess.DEVNULL if isinstance(source, AudioFile) else source.stdout
 
-        if not run_commandline(args, quiet, False, stdin):
-            debug("Done", self)
+        if not run_cmd_pb(args, quiet, ProgressBarConfig("Encoding..."), shell=False, stdin=stdin):
             clean_temp_files()
-            return AudioFile(output, input.container_delay, input.source)
+            return AudioFile(output, fileIn.container_delay, fileIn.source)
         else:
             raise crit("Encoding to FLAC using libFLAC failed!", self)
 
 
 @dataclass
 class FLACCL(LosslessEncoder):
     """
@@ -78,21 +78,21 @@
 
     compression_level: int = 8
     preprocess: Preprocessor | Sequence[Preprocessor] | None = field(default_factory=Resample)
     verify: bool = True
     append: str = ""
     output: PathLike | None = None
 
-    def encode_audio(self, input: AudioFile, quiet: bool = True, **kwargs) -> AudioFile:
-        if not isinstance(input, AudioFile):
-            input = AudioFile.from_file(input, self)
+    def encode_audio(self, fileIn: AudioFile | PathLike, quiet: bool = True, **kwargs) -> AudioFile:
+        if not isinstance(fileIn, AudioFile):
+            fileIn = AudioFile.from_file(fileIn, self)
         flaccl = get_executable("CUETools.FLACCL.cmd")
-        output = make_output(input.file, "flac", "flaccl", self.output)
-        source = ensure_valid_in(input, preprocess=self.preprocess, caller=self, valid_type=ValidInputType.FLAC, supports_pipe=False)
-        debug(f"Encoding '{input.file.stem}' to FLAC using FLACCL...", self)
+        output = make_output(fileIn.file, "flac", "flaccl", self.output)
+        source = ensure_valid_in(fileIn, preprocess=self.preprocess, caller=self, valid_type=ValidInputType.FLAC, supports_pipe=False)
+        debug(f"Encoding '{fileIn.file.stem}' to FLAC using FLACCL...", self)
 
         args = [flaccl, f"-{self.compression_level}", "-o", str(output)]
         if self.compression_level > 8:
             args.append("--lax")
         if self.verify:
             args.append("--verify")
         if self.append:
@@ -100,15 +100,15 @@
         args.append(str(source.file.resolve()) if isinstance(source, AudioFile) else "-")
 
         stdin = subprocess.DEVNULL if isinstance(source, AudioFile) else source.stdout
 
         if not run_commandline(args, quiet, False, stdin):
             debug("Done", self)
             clean_temp_files()
-            return AudioFile(output, input.container_delay, input.source)
+            return AudioFile(output, fileIn.container_delay, fileIn.source)
         else:
             raise crit("Encoding to FLAC using FLACCL failed!", self)
 
 
 @dataclass
 class FF_FLAC(LosslessEncoder):
     """
@@ -122,54 +122,45 @@
     """
 
     compression_level: int = 10
     preprocess: Preprocessor | Sequence[Preprocessor] | None = field(default_factory=Resample)
     append: str = ""
     output: PathLike | None = None
 
-    def _base_command(self, input: AudioFile, compression: int = 0) -> list[str]:
+    def _base_command(self, fileIn: AudioFile, compression: int = 0) -> list[str]:
         # fmt: off
-        args = [get_executable("ffmpeg"), "-hide_banner", "-i", str(input.file.resolve()), "-map", "0:a:0", "-c:a", "flac", "-compression_level", str(compression)]
-        preprocess = sanitize_pre(self.preprocess)
-        minfo = input.get_mediainfo()
-        if any([p.can_run(minfo, preprocess) for p in preprocess]):
-            filters = list[str]()
-            for pre in [p for p in preprocess if p.can_run(minfo, preprocess)]:
-                pre.analyze(input)
-                args.extend(pre.get_args(caller=self))
-                filt = pre.get_filter(caller=self)
-                if filt:
-                    filters.append(filt)
-            if filters:
-                args.extend(["-filter:a", ",".join(filters)])
+        args = [get_executable("ffmpeg"), "-hide_banner", "-i", str(fileIn.file.resolve()), "-map", "0:a:0", "-c:a", "flac", "-compression_level", str(compression)]
+        minfo = fileIn.get_mediainfo()
+        args.extend(get_preprocess_args(fileIn, self.preprocess, minfo, self))
         if self.append:
             args.extend(splitcommand(self.append))
         return args
         # fmt: on
 
-    def encode_audio(self, input: AudioFile, quiet: bool = True, **kwargs) -> AudioFile:
-        if not isinstance(input, AudioFile):
-            input = AudioFile.from_file(input, self)
-        output = make_output(input.file, "flac", "ffmpeg", self.output)
+    def encode_audio(self, fileIn: AudioFile | PathLike, quiet: bool = True, **kwargs) -> AudioFile:
+        if not isinstance(fileIn, AudioFile):
+            fileIn = AudioFile.from_file(fileIn, self)
+        output = make_output(fileIn.file, "flac", "ffmpeg", self.output)
         if "temp" in kwargs.keys():
             debug(f"Preparing audio for input to other encoder using ffmpeg...", self)
         else:
-            debug(f"Encoding '{input.file.stem}' to FLAC using ffmpeg...", self)
-        args = self._base_command(input, self.compression_level)
+            debug(f"Encoding '{fileIn.file.stem}' to FLAC using ffmpeg...", self)
+        args = self._base_command(fileIn, self.compression_level)
         args.append(str(output.resolve()))
 
-        if not run_commandline(args, quiet):
-            debug("Done", self)
-            return AudioFile(output, input.container_delay, input.source)
+        if not run_cmd_pb(
+            args, quiet, ProgressBarConfig("Preparing..." if "temp" in kwargs.keys() else "Encoding...", duration_from_file(fileIn, 0))
+        ):
+            return AudioFile(output, fileIn.container_delay, fileIn.source)
         else:
             raise crit("Encoding to flac using ffmpeg failed!", self)
 
-    def get_pipe(self, input: AudioFile) -> subprocess.Popen:
+    def get_pipe(self, fileIn: AudioFile) -> subprocess.Popen:
         debug(f"Piping audio for input to other encoder using ffmpeg...", self)
-        args = self._base_command(input, 0)
+        args = self._base_command(fileIn, 0)
         args.extend(["-f", "flac", "-"])
         p = subprocess.Popen(args, stdin=subprocess.DEVNULL, stdout=subprocess.PIPE, stderr=subprocess.DEVNULL, text=False)
         return p
 
 
 @dataclass
 class Opus(Encoder):
@@ -188,48 +179,52 @@
 
     bitrate: int | None = None
     vbr: bool = True
     preprocess: Preprocessor | Sequence[Preprocessor] | None = None
     append: str = ""
     output: PathLike | None = None
 
-    def encode_audio(self, input: AudioFile | PathLike, quiet: bool = True, **kwargs) -> AudioFile:
-        if not isinstance(input, AudioFile):
-            input = AudioFile.from_file(input, self)
+    def encode_audio(self, fileIn: AudioFile | PathLike, quiet: bool = True, **kwargs) -> AudioFile:
+        if not isinstance(fileIn, AudioFile):
+            fileIn = AudioFile.from_file(fileIn, self)
 
         exe = get_executable("opusenc")
-        source = ensure_valid_in(input, preprocess=self.preprocess, caller=self, valid_type=ValidInputType.FLAC, supports_pipe=True)
+        source = ensure_valid_in(fileIn, preprocess=self.preprocess, caller=self, valid_type=ValidInputType.FLAC, supports_pipe=True)
         bitrate = self.bitrate
         if not bitrate:
-            info = input.get_mediainfo()
+            info = fileIn.get_mediainfo()
             match info.channel_s:
                 case _ if info.channel_s == 2 or [p for p in sanitize_pre(self.preprocess) if isinstance(p, Downmix)]:
                     bitrate = 192
                 case _ if info.channel_s > 6:
                     bitrate = 420
                 case _:
                     bitrate = 320
-            debug(f"Encoding '{input.file.stem}' to Opus ({bitrate} kbps) using opusenc...", self)
+            debug(f"Encoding '{fileIn.file.stem}' to Opus ({bitrate} kbps) using opusenc...", self)
         else:
-            debug(f"Encoding '{input.file.stem}' to Opus using opusenc...", self)
+            debug(f"Encoding '{fileIn.file.stem}' to Opus using opusenc...", self)
 
-        output = make_output(input.file, "opus", "opusenc", self.output)
+        output = make_output(fileIn.file, "opus", "opusenc", self.output)
 
         args = [exe, "--vbr" if self.vbr else "--cvbr", "--bitrate", str(bitrate)]
         if self.append:
             args.extend(splitcommand(self.append))
         args.append(str(source.file.resolve()) if isinstance(source, AudioFile) else "-")
         args.append(str(output))
 
         stdin = subprocess.DEVNULL if isinstance(source, AudioFile) else source.stdout
 
-        if not run_commandline(args, quiet, False, stdin):
-            debug("Done", self)
+        if isinstance(source, AudioFile):
+            config = ProgressBarConfig("Encoding...")
+        else:
+            config = ProgressBarConfig("Encoding...", duration_from_file(fileIn, 0), regex=r".*\] (\d+:\d+:\d+.\d+).*")
+
+        if not run_cmd_pb(args, quiet, config, shell=False, stdin=stdin):
             clean_temp_files()
-            return AudioFile(output, input.container_delay, input.source)
+            return AudioFile(output, fileIn.container_delay, fileIn.source)
         else:
             raise crit("Encoding to opus using opusenc failed!", self)
 
 
 @dataclass
 class qAAC(Encoder):
     """
@@ -246,34 +241,33 @@
 
     q: int = 127
     mode: qAAC_MODE | int = qAAC_MODE.TVBR
     preprocess: Preprocessor | Sequence[Preprocessor] | None = None
     append: str = ""
     output: PathLike | None = None
 
-    def encode_audio(self, input: AudioFile, quiet: bool = True, **kwargs) -> AudioFile:
-        if not isinstance(input, AudioFile):
-            input = AudioFile.from_file(input, self)
-        output = make_output(input.file, "aac", "qaac", self.output)
-        source = ensure_valid_in(input, preprocess=self.preprocess, caller=self, valid_type=ValidInputType.AIFF_OR_FLAC, supports_pipe=False)
+    def encode_audio(self, fileIn: AudioFile | PathLike, quiet: bool = True, **kwargs) -> AudioFile:
+        if not isinstance(fileIn, AudioFile):
+            fileIn = AudioFile.from_file(fileIn, self)
+        output = make_output(fileIn.file, "aac", "qaac", self.output)
+        source = ensure_valid_in(fileIn, preprocess=self.preprocess, caller=self, valid_type=ValidInputType.AIFF_OR_FLAC, supports_pipe=False)
         qaac = get_executable("qaac")
         qaac_compatcheck()
 
-        debug(f"Encoding '{input.file.stem}' to AAC using qAAC...", self)
+        debug(f"Encoding '{fileIn.file.stem}' to AAC using qAAC...", self)
         args = [qaac, "--no-delay", "--no-optimize", "--threading", f"--{self.mode.name.lower()}", str(self.q)]
         if self.append:
             args.extend(splitcommand(self.append))
         args.extend(["-o", str(output), str(source.file.resolve()) if isinstance(source, AudioFile) else "-"])
 
         stdin = subprocess.DEVNULL if isinstance(source, AudioFile) else source.stdout
 
-        if not run_commandline(args, quiet, False, stdin):
-            debug("Done", self)
+        if not run_cmd_pb(args, quiet, ProgressBarConfig("Encoding..."), shell=False, stdin=stdin):
             clean_temp_files()
-            return AudioFile(output, input.container_delay, input.source)
+            return AudioFile(output, fileIn.container_delay, fileIn.source)
         else:
             raise crit("Encoding to AAC using qAAC failed!", self)
 
 
 @dataclass
 class FDK_AAC(Encoder):
     """
@@ -298,18 +292,18 @@
     bitrate: int = 256
     cutoff: int = 20000
     preprocess: Preprocessor | Sequence[Preprocessor] | None = None
     use_binary: bool = False
     append: str = ""
     output: PathLike | None = None
 
-    def encode_audio(self, input: AudioFile, quiet: bool = True, **kwargs) -> AudioFile:
-        if not isinstance(input, AudioFile):
-            input = AudioFile.from_file(input, self)
-        output = make_output(input.file, "m4a", "fdkaac", self.output)
+    def encode_audio(self, fileIn: AudioFile | PathLike, quiet: bool = True, **kwargs) -> AudioFile:
+        if not isinstance(fileIn, AudioFile):
+            fileIn = AudioFile.from_file(fileIn, self)
+        output = make_output(fileIn.file, "m4a", "fdkaac", self.output)
         if not has_libFDK():
             exe = get_executable("fdkaac", False, False)
             if not exe:
                 raise error(
                     "Your installation of ffmpeg wasn't compiled with libFDK."
                     + "\nYou can download builds with the non-free flag from https://github.com/AnimMouse/ffmpeg-autobuild/releases"
                     + "\nYou can also use the FDKAAC binary if you can find a built version.",
@@ -317,40 +311,42 @@
                 )
             self.use_binary = True
         else:
             exe = get_executable("ffmpeg") if not self.use_binary else get_executable("fdkaac")
 
         if os.name == "nt":
             warn("It is strongly recommended to use qAAC on windows. See docs.", self, 5)
-        debug(f"Encoding '{input.file.stem}' to AAC using libFDK...", self)
+        debug(f"Encoding '{fileIn.file.stem}' to AAC using libFDK...", self)
         # fmt: off
         if self.use_binary:
             source = ensure_valid_in(
-                input, preprocess=self.preprocess, caller=self, valid_type=ValidInputType.RF64, supports_pipe=False
+                fileIn, preprocess=self.preprocess, caller=self, valid_type=ValidInputType.RF64, supports_pipe=False
             )
             args = [exe, "-m", str(self.bitrate_mode), "-w", str(self.cutoff), "-a", "1"]
             if self.bitrate_mode == 0:
                 args.extend(["-b", str(self.bitrate)])
             if self.append:
                 args.extend(splitcommand(self.append))
             args.extend(["-o", str(output), str(source.file)])
         else:
-            args = [exe, "-hide_banner", "-i", str(input.file), "-map", "0:a:0", "-c:a", "libfdk_aac", "-cutoff", str(self.cutoff)]
+            args = [exe, "-hide_banner", "-i", str(fileIn.file), "-map", "0:a:0", "-c:a", "libfdk_aac", "-cutoff", str(self.cutoff)]
             if self.bitrate_mode > 0:
                 args.extend(['-vbr', str(self.bitrate_mode)])
             else:
                 args.extend(['-b:a', f'{self.bitrate}k'])
-            if self.dither:
-                args.extend(['-sample_fmt', 's16', '-ar', '48000', '-resampler', 'soxr', '-precision', '24', '-dither_method', self.dither_type.name.lower()])
+            args.extend(get_preprocess_args(fileIn, self.preprocess, fileIn.get_mediainfo(), self))
             if self.append:
                 args.extend(splitcommand(self.append))
             args.append(str(output))
         # fmt: on
-        if not run_commandline(args, quiet, False):
-            debug("Done", self)
+        if self.use_binary:
+            config = ProgressBarConfig("Encoding...")
+        else:
+            config = ProgressBarConfig("Encoding...", duration_from_file(fileIn, 0))
+        if not run_cmd_pb(args, quiet, config, shell=False):
             clean_temp_files()
-            return AudioFile(output, input.container_delay, input.source)
+            return AudioFile(output, fileIn.container_delay, fileIn.source)
         else:
             raise crit("Encoding to AAC using libFDK failed!", self)
 
 
 # TODO: Implement the dolby shit
```

### Comparing `muxtools-0.0.9/muxtools/audio/extractors.py` & `muxtools-0.1.0/muxtools/audio/extractors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from shlex import split as splitcommand
 from dataclasses import dataclass
 from datetime import timedelta
 from fractions import Fraction
 from pathlib import Path
-import shutil
 import os
 import re
 
-from .audioutils import format_from_track, is_fancy_codec, sanitize_trims, ensure_valid_in
+from .audioutils import format_from_track, is_fancy_codec, sanitize_trims, ensure_valid_in, duration_from_file
 from .tools import *
 from ..utils.files import *
 from ..utils.log import error, warn, debug
 from ..utils.download import get_executable
 from ..utils.parsing import parse_audioinfo
 from ..utils.files import get_absolute_track
 from ..utils.types import Trim, PathLike, TrackType
 from ..utils.env import get_temp_workdir, run_commandline
+from ..utils.subprogress import run_cmd_pb, ProgressBarConfig
 from ..utils.convert import frame_to_timedelta, format_timedelta, frame_to_ms
 
 __all__ = ["Eac3to", "Sox", "FFMpeg", "MkvExtract"]
 
 
 @dataclass
 class Eac3to(Extractor):
@@ -58,15 +58,17 @@
                 pattern = re.compile(pattern_str, re.IGNORECASE)
                 for f in os.listdir(out.parent):
                     if pattern.match(f):
                         f = Path(out.parent, f)
                         out = f.rename(f.with_stem(out.stem))
                         break
 
-            return AudioFile(out, getattr(track, "delay_relative_to_video", 0) if self.preserve_delay else 0, input)
+            return AudioFile(
+                out, getattr(track, "delay_relative_to_video", 0) if self.preserve_delay else 0, input, duration=duration_from_file(input, self.track)
+            )
         else:
             raise error(f"eac3to failed to extract audio track {self.track} from '{input}'", self.extract_audio)
 
 
 @dataclass
 class MkvExtract(Extractor):
     def __post_init__(self):
@@ -126,18 +128,17 @@
                     args.extend(["-c:a", "pcm_s16le" if specified_depth == 16 else "pcm_s24le", "-rf64", "auto"])
                 else:
                     args.extend(["-c:a", "copy"])
                     if extension == "dtshd" or extension == "dts":
                         # FFMPEG screams about dtshd not being a known output format but ffmpeg -formats lists it....
                         args.extend(["-f", "dts"])
             args.append(str(out))
-
-            if not run_commandline(args, quiet):
-                debug("Done", self)
-                return AudioFile(out, getattr(track, "delay_relative_to_video", 0) if self.preserve_delay else 0, input, ainfo)
+            duration = duration_from_file(input, self.track)
+            if not run_cmd_pb(args, quiet, ProgressBarConfig("Extracting...", duration)):
+                return AudioFile(out, getattr(track, "delay_relative_to_video", 0) if self.preserve_delay else 0, input, ainfo, duration)
             else:
                 raise error("Failed to extract audio track using ffmpeg", self)
 
     @dataclass
     class Trimmer(Trimmer):
         """
         Trims audio files using FFMPEG.
```

### Comparing `muxtools-0.0.9/muxtools/audio/memecoders.py` & `muxtools-0.1.0/muxtools/audio/memecoders.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 
 Thought they might be cool to have atleast.
 """
 
 from pathlib import Path
 from dataclasses import dataclass, field
 from shlex import split as splitcommand
-from typing import Sequence
+from collections.abc import Sequence
 
 
 from .encoders import FLAC
 from .preprocess import Preprocessor, Resample
 from .tools import Encoder, LosslessEncoder
 from ..utils.log import crit, debug, error
 from ..muxing.muxfiles import AudioFile
-from ..utils.env import get_temp_workdir, run_commandline
+from ..utils.env import get_temp_workdir
 from ..utils.download import get_executable
 from ..utils.files import clean_temp_files, make_output
-from .audioutils import ensure_valid_in, qaac_compatcheck
+from ..utils.subprogress import run_cmd_pb, ProgressBarConfig
+from .audioutils import ensure_valid_in, qaac_compatcheck, duration_from_file, get_preprocess_args
 from ..utils.types import DitherType, LossyWavQuality, PathLike, ValidInputType
 
 __all__ = ["qALAC", "TTA", "TrueAudio", "TheTrueAudio", "LossyWav", "Wavpack"]
 
 
 @dataclass
 class qALAC(Encoder):
@@ -36,76 +37,69 @@
                                 Do not specify an extension unless you know what you're doing.
     """
 
     preprocess: Preprocessor | Sequence[Preprocessor] | None = field(default_factory=Resample)
     append: str = ""
     output: PathLike | None = None
 
-    def encode_audio(self, input: AudioFile, quiet: bool = True, **kwargs) -> AudioFile:
-        if not isinstance(input, AudioFile):
-            input = AudioFile.from_file(input, self)
-        output = make_output(input.file, "alac", "qaac", self.output)
-        source = ensure_valid_in(input, preprocess=self.preprocess, caller=self, valid_type=ValidInputType.AIFF_OR_FLAC, supports_pipe=False)
+    def encode_audio(self, fileIn: AudioFile | PathLike, quiet: bool = True, **kwargs) -> AudioFile:
+        if not isinstance(fileIn, AudioFile):
+            fileIn = AudioFile.from_file(fileIn, self)
+        output = make_output(fileIn.file, "alac", "qaac", self.output)
+        source = ensure_valid_in(fileIn, preprocess=self.preprocess, caller=self, valid_type=ValidInputType.AIFF_OR_FLAC, supports_pipe=False)
         qaac = get_executable("qaac")
         qaac_compatcheck()
 
-        debug(f"Encoding '{input.file.stem}' to ALAC using qAAC...", self)
+        debug(f"Encoding '{fileIn.file.stem}' to ALAC using qAAC...", self)
         args = [qaac, "-A", "--no-optimize", "--threading", "-o", str(output)]
         if self.append:
             args.extend(splitcommand(self.append))
         args.append(str(source.file))
 
-        if not run_commandline(args, quiet):
-            debug("Done", self)
+        if not run_cmd_pb(args, quiet, ProgressBarConfig("Encoding...")):
             clean_temp_files()
-            return AudioFile(output, input.container_delay, input.source)
+            return AudioFile(output, fileIn.container_delay, fileIn.source)
         else:
             raise crit("Encoding to ALAC using qAAC failed!", self)
 
 
 @dataclass
 class TTA(LosslessEncoder):
     """
     Uses ffmpeg to encode audio to TTA/The True Audio.
     (I could not get the reference encoder to work with any ffmpeg wav or any flac)
     This doesn't really seem to have any benefit over FLAC except for maybe encode speed?
     Definitely has a cool name tho.
 
 
-    :param dither:              Dithers any input down to 16 bit 48 khz if True
-    :param dither_type:         FFMPEG dither_method used for dithering
+    :param preprocess:          Any amount of preprocessors to run before passing it to the encoder.
     :param append:              Any other args one might pass to the encoder
     :param output:              Custom output. Can be a dir or a file.
                                 Do not specify an extension unless you know what you're doing.
     """
 
-    dither: bool = True
-    dither_type: DitherType = DitherType.TRIANGULAR
+    preprocess: Preprocessor | Sequence[Preprocessor] | None = field(default_factory=Resample)
     append: str = ""
     output: PathLike | None = None
 
-    def encode_audio(self, input: AudioFile, quiet: bool = True, **kwargs) -> AudioFile:
-        if not isinstance(input, AudioFile):
-            input = AudioFile.from_file(input, self)
-        output = make_output(input.file, "tta", "encoded", self.output)
-
-        args = [get_executable("ffmpeg"), "-hide_banner", "-i", str(input.file.resolve()), "-map", "0:a:0", "-c:a", "tta"]
-        if self.dither:
-            args.extend(
-                ["-sample_fmt", "s16", "-ar", "48000", "-resampler", "soxr", "-precision", "24", "-dither_method", self.dither_type.name.lower()]
-            )
+    def encode_audio(self, fileIn: AudioFile | PathLike, quiet: bool = True, **kwargs) -> AudioFile:
+        if not isinstance(fileIn, AudioFile):
+            fileIn = AudioFile.from_file(fileIn, self)
+        output = make_output(fileIn.file, "tta", "encoded", self.output)
+
+        args = [get_executable("ffmpeg"), "-hide_banner", "-i", str(fileIn.file.resolve()), "-map", "0:a:0", "-c:a", "tta"]
+        args.extend(get_preprocess_args(fileIn, self.preprocess, fileIn.get_mediainfo(), self))
         if self.append:
             args.extend(splitcommand(self.append))
         args.append(str(output))
 
-        debug(f"Encoding '{input.file.stem}' to TTA using ffmpeg...", self)
-        if not run_commandline(args, quiet):
-            debug("Done", self)
+        debug(f"Encoding '{fileIn.file.stem}' to TTA using ffmpeg...", self)
+        if not run_cmd_pb(args, quiet, ProgressBarConfig("Encoding...", duration_from_file(fileIn))):
             clean_temp_files()
-            return AudioFile(output, input.container_delay, input.source)
+            return AudioFile(output, fileIn.container_delay, fileIn.source)
         else:
             raise crit("Encoding to TTA using ffmpeg failed!", self)
 
 
 TrueAudio = TTA
 TheTrueAudio = TTA
 
@@ -124,33 +118,32 @@
     """
 
     fast: bool = False
     preprocess: Preprocessor | Sequence[Preprocessor] | None = field(default_factory=Resample)
     append: str = ""
     output: PathLike | None = None
 
-    def encode_audio(self, input: AudioFile, quiet: bool = True, **kwargs) -> AudioFile:
-        if not isinstance(input, AudioFile):
-            input = AudioFile.from_file(input, self)
+    def encode_audio(self, fileIn: AudioFile | PathLike, quiet: bool = True, **kwargs) -> AudioFile:
+        if not isinstance(fileIn, AudioFile):
+            fileIn = AudioFile.from_file(fileIn, self)
 
-        valid_in = ensure_valid_in(input, False, self.preprocess, valid_type=ValidInputType.AIFF, caller=self)
-        output = make_output(input.file, "wv", "wavpack", self.output)
+        valid_in = ensure_valid_in(fileIn, False, self.preprocess, valid_type=ValidInputType.AIFF, caller=self)
+        output = make_output(fileIn.file, "wv", "wavpack", self.output)
 
         wavpack = get_executable("wavpack")
         args = [wavpack, "-f" if self.fast else "-h"]
         if self.append:
             args.extend(splitcommand(self.append))
         args.extend([str(valid_in.file), str(output)])
-        debug(f"Encoding '{input.file.stem}' to wavpack...", self)
-        if run_commandline(args, quiet):
+        debug(f"Encoding '{fileIn.file.stem}' to wavpack...", self)
+        if run_cmd_pb(args, quiet, ProgressBarConfig("Encoding...")):
             raise error("Failed to encode audio to wavpack!", self)
 
         clean_temp_files()
-        debug("Done", self)
-        return AudioFile(output, input.container_delay, input.source)
+        return AudioFile(output, fileIn.container_delay, fileIn.source)
 
 
 @dataclass
 class LossyWav(Encoder):
     """
     A lossy (lol) preprocessor for wav/pcm audio that selectively reduces bitdepth by zero'ing out certain bits.
     Certain lossless encoders like FLAC (only the reference one) will get a massive size reduction that way.
@@ -169,34 +162,34 @@
 
     quality: LossyWavQuality = LossyWavQuality.INSANE
     target_encoder: LosslessEncoder | None = None
     override_options: bool = True
     preprocess: Preprocessor | Sequence[Preprocessor] | None = field(default_factory=Resample)
     output: PathLike | None = None
 
-    def encode_audio(self, input: AudioFile, quiet: bool = True, **kwargs) -> AudioFile:
+    def encode_audio(self, fileIn: AudioFile | PathLike, quiet: bool = True, **kwargs) -> AudioFile:
         if not self.target_encoder:
             self.target_encoder = FLAC()
         if not self.target_encoder.lossless:
             raise error("Target Encoder can only be a lossless one.", self)
-        if not isinstance(input, AudioFile):
-            input = AudioFile.from_file(input, self)
+        if not isinstance(fileIn, AudioFile):
+            fileIn = AudioFile.from_file(fileIn, self)
 
-        output = ensure_valid_in(input, False, self.preprocess, valid_type=ValidInputType.W64, caller=self)
+        output = ensure_valid_in(fileIn, False, self.preprocess, valid_type=ValidInputType.W64, caller=self)
 
         args = [get_executable("lossyWAV", False), str(output.file), "--quality", self.quality.name.lower(), "-o", str(get_temp_workdir())]
         debug(f"Doing lossywav magic...", self)
-        if run_commandline(args, quiet):
+        if run_cmd_pb(args, quiet, ProgressBarConfig("Encoding...")):
             raise crit("LossyWAV conversion failed!", self)
 
         lossy = Path(get_temp_workdir(), output.file.with_stem(output.file.stem + ".lossy").name)
         setattr(self.target_encoder, "preprocess", None)
         if self.override_options:
             if isinstance(self.target_encoder, FLAC):
                 setattr(self.target_encoder, "compression_level", 5)
                 setattr(self.target_encoder, "append", "-b 512")
             elif isinstance(self.target_encoder, Wavpack):
                 setattr(self.target_encoder, "append", "--blocksize=512 --merge-blocks")
 
-        encoded = self.target_encoder.encode_audio(AudioFile(lossy, input.container_delay, input.source), quiet)
+        encoded = self.target_encoder.encode_audio(AudioFile(lossy, fileIn.container_delay, fileIn.source), quiet)
         clean_temp_files()
         return encoded
```

### Comparing `muxtools-0.0.9/muxtools/audio/preprocess.py` & `muxtools-0.1.0/muxtools/audio/preprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import re
 import subprocess
-from typing import Any, Sequence
+from typing import Any
+from collections.abc import Sequence
 from dataclasses import dataclass
 from abc import ABC, abstractmethod
 from pymediainfo import Track
 
 from ..utils.log import error, debug
 from ..utils.types import DitherType
 from ..muxing.muxfiles import AudioFile
@@ -14,26 +15,25 @@
 
 __all__ = ["Resample", "Loudnorm", "Downmix", "Pan", "CustomPreprocessor"]
 
 
 class Preprocessor(ABC):
     refresh_metadata = False
 
-    def get_filter(self, caller: any = None) -> str | None:
+    def get_filter(self, caller: Any = None) -> str | None:
         return None
 
-    def get_args(self, caller: any = None) -> list[str]:
+    def get_args(self, caller: Any = None) -> Sequence[str]:
         return []
 
     def analyze(self, file: AudioFile):
         return None
 
     @abstractmethod
-    def can_run(self, track: Track, preprocessors: list[Any]) -> bool:
-        ...
+    def can_run(self, track: Track, preprocessors: Sequence[Any]) -> bool: ...
 
 
 @dataclass
 class Resample(Preprocessor):
     """
     A FFMPEG Resampling preprocessor.
     This is used to dither down to 16 bit and resample to 48kHz by default.
@@ -46,28 +46,30 @@
     """
 
     dither: DitherType = DitherType.TRIANGULAR
     depth: int | None = 16
     sample_rate: int = 48000
     refresh_metadata = True
 
-    def can_run(self, track: Track, preprocessors: list[Any]) -> bool:
+    def can_run(self, track: Track, preprocessors: Sequence[Any]) -> bool:
         # Run if depth or sample rate differ. Also run if loudnorm is being used.
         return (
             (self.depth and getattr(track, "bit_depth", 24) != self.depth)
             or getattr(track, "sampling_rate", 0) != self.sample_rate
             or [p for p in preprocessors if isinstance(p, Loudnorm)]
         )
 
-    def get_args(self, caller: any = None) -> list[str]:
+    def get_args(self, caller: Any = None) -> Sequence[str]:
         if caller:
             debug(
-                f"Resampling to {self.depth} bit and {self.sample_rate / 1000} kHz..."
-                if self.depth
-                else f"Resampling to {self.sample_rate / 1000} kHz...",
+                (
+                    f"Resampling to {self.depth} bit and {self.sample_rate / 1000} kHz..."
+                    if self.depth
+                    else f"Resampling to {self.sample_rate / 1000} kHz..."
+                ),
                 caller,
             )
         return (
             []
             if not self.depth
             else ["-sample_fmt", f"s{self.depth}"]
             + [
@@ -106,18 +108,18 @@
     :param force:       Force processing even if there are only 2 channels.
     """
 
     mixing: str | None = None
     force: bool = False
     refresh_metadata = True
 
-    def can_run(self, track: Track, preprocessors: list[Any]) -> bool:
+    def can_run(self, track: Track, preprocessors: Sequence[Any]) -> bool:
         return getattr(track, "channel_s", 2) > 2 or self.force
 
-    def get_filter(self, caller: any = None) -> str:
+    def get_filter(self, caller: Any = None) -> str:
         if not self.mixing:
             self.mixing = Downmix.Dave_750
         if caller:
             debug("Applying downmix/pan filter...", caller)
         return f"pan={self.mixing}"
 
     @classproperty
@@ -164,15 +166,15 @@
     class Measurements:
         i: float
         lra: float
         tp: float
         thresh: float
         target_offset: float
 
-    def can_run(self, track: Track, preprocessors: list[Any]) -> bool:
+    def can_run(self, track: Track, preprocessors: Sequence[Any]) -> bool:
         return True
 
     def analyze(self, file: AudioFile):
         debug("Analyzing file loudness...", self)
         ffmpeg = get_executable("ffmpeg")
         out_var = "NUL" if os.name == "nt" else "/dev/null"
         args = [
@@ -204,15 +206,15 @@
             float(i_match[0]),
             float(lra_match[0]),
             float(tp_match[0]),
             float(thresh_match[0]),
             float(offset_match[0]),
         )
 
-    def get_filter(self, caller: any = None) -> str | None:
+    def get_filter(self, caller: Any = None) -> str | None:
         if caller:
             debug(f"Applying loudnorm...", caller)
         if not hasattr(self, "measurements"):
             # Ideally shouldn't run into this lmfao
             return ""
         return (
             f"loudnorm=linear=true:i={self.i}:lra={self.lra}:tp={self.tp}:offset={self.offset if self.offset else self.measurements.target_offset}"
@@ -229,17 +231,17 @@
                         It should look like this `afade=t=in:ss=0:d=15`
     :param args:        Other args you may want to pass to ffmpeg.
     """
 
     filt: str | None = None
     args: str | Sequence[str] | None = None
 
-    def can_run(self, track: Track, preprocessors: list[Any]) -> bool:
+    def can_run(self, track: Track, preprocessors: Sequence[Any]) -> bool:
         return True
 
-    def get_filter(self, caller: any = None) -> str | None:
+    def get_filter(self, caller: Any = None) -> str | None:
         return self.filt
 
-    def get_args(self, caller: any = None) -> list[str]:
+    def get_args(self, caller: Any = None) -> Sequence[str]:
         if isinstance(self.args, str) and not isinstance(self.args, Sequence):
             self.args = [self.args]
         return list(self.args) if self.args else []
```

### Comparing `muxtools-0.0.9/muxtools/audio/tools.py` & `muxtools-0.1.0/muxtools/audio/tools.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.9/muxtools/cli.py` & `muxtools-0.1.0/muxtools/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,31 +126,36 @@
             ("versions", ""),
             "ffmpeg-gyan-nightly",
         )
     if not shutil.which("fdkaac"):
         request_install(
             "fdkaac",
             "The second best AAC encoder. Not really necessary tbf.",
-            "hoilc_scoop-lemon/fdkaac",
-            ("hoilc_scoop-lemon", "https://github.com/hoilc/scoop-lemon"),
-            "fdkaac"
+            "vodes/fdkaac",
+            ("vodes", "https://github.com/Vodes/Bucket"),
+            "fdkaac",
         )
     if not shutil.which("sox"):
         request_install("SoX", "This is used & preferred for trimming lossless audio.")
 
     if not shutil.which("mkvmerge") or not shutil.which("mkvextract"):
         request_install(
             "Mkvtoolnix",
             "This is used for all muxing operations.\nYou might have already installed this but mkvmerge and mkvextract could not be found in path!",
             "extras/mkvtoolnix",
             ("extras", ""),
         )
 
     if not shutil.which("opusenc"):
-        request_install("opus-tools", "This is used for encoding audio to opus via opusenc.")
+        request_install(
+            "opus-tools",
+            "This is used for encoding audio to opus via opusenc.",
+            "vodes/opus-tools-rarewares",
+            ("vodes", "https://github.com/Vodes/Bucket"),
+        )
 
     if not shutil.which("flac"):
         request_install("FLAC", "This is used for encoding audio to flac via the official reference encoder.")
 
     if not shutil.which("qaac"):
         if not request_install("qaac", "This is used for encoding audio to aac."):
             warn("qAAC requires external libraries from iTunes because apple is funny.\nYou can automatically install these with [b u]libs[/].")
```

### Comparing `muxtools-0.0.9/muxtools/functions.py` & `muxtools-0.1.0/muxtools/functions.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.9/muxtools/main.py` & `muxtools-0.1.0/muxtools/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import os
 import json
-from typing import TypeVar
+from typing import Any, TypeVar
 from pathlib import Path
 from dataclasses import dataclass
 from configparser import ConfigParser
 
 from .utils.log import error
 
 __all__ = ["Setup"]
@@ -91,15 +91,15 @@
         self.work_dir.mkdir(parents=True, exist_ok=True)
         self.work_dir = str(self.work_dir)
 
         from .utils.env import save_setup
 
         save_setup(self)
 
-    def edit(self: SetupSelf, attr: str, value: any) -> SetupSelf:
+    def edit(self: SetupSelf, attr: str, value: Any) -> SetupSelf:
         """
         Sets a variable inside of Setup and saves it to the environment variables.
         You should use this to apply any changes because other functions will not make use of them otherwise!
 
         :param attr:        The name of the variable/attribute you want to change
         :param value:       The value this variable/attribute will have.
         """
```

### Comparing `muxtools-0.0.9/muxtools/misc/chapters.py` & `muxtools-0.1.0/muxtools/misc/chapters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 from datetime import timedelta
 from fractions import Fraction
-from os import PathLike
 from pathlib import Path
 from typing import TypeVar
 import os
 import re
 
 from ..subtitle.sub import SubFile
 from ..utils.log import error, info, warn
@@ -132,41 +131,54 @@
                 converted.append(ch)
 
         for ch in converted:
             self.chapters.insert(index, ch)
             index += 1
         return self
 
-    def shift_chapter(self, chapter: int = 0, shift_amount: int = 0) -> "Chapters":
+    def shift_chapter(self: ChaptersSelf, chapter: int = 0, shift_amount: int = 0) -> ChaptersSelf:
         """
         Used to shift a single chapter by x frames
 
         :param chapter:         Chapter number (starting at 0)
         :param shift_amount:    Frames to shift by
         """
         ch = list(self.chapters[chapter])
-        shifted_frame = ch[0] + frame_to_timedelta(shift_amount, self.fps)
+        shift_delta = frame_to_timedelta(abs(shift_amount), self.fps)
+        if shift_amount < 0:
+            shifted_frame = ch[0] - shift_delta
+        else:
+            shifted_frame = ch[0] + shift_delta
+
         if shifted_frame.total_seconds() > 0:
             ch[0] = shifted_frame
         else:
             ch[0] = timedelta(seconds=0)
         self.chapters[chapter] = tuple(ch)
         return self
 
-    def print(self) -> "Chapters":
+    def shift(self: ChaptersSelf, shift_amount: int) -> ChaptersSelf:
+        """
+        Shifts all chapters by x frames.
+
+        :param shift_amount:    Frames to shift by
+        """
+        return [self.shift_chapter(i, shift_amount) for i, _ in enumerate(self.chapters)][-1]
+
+    def print(self: ChaptersSelf) -> ChaptersSelf:
         """
         Prettier print for these because default timedelta formatting sucks
         """
         info("Chapters:")
         for time, name in self.chapters:
             print(f"{name}: {format_timedelta(time)} | {timedelta_to_frame(time, self.fps)}")
         print("", end="\n")
         return self
 
-    def to_file(self, out: PathLike | None = None) -> str:
+    def to_file(self: ChaptersSelf, out: PathLike | None = None) -> str:
         """
         Outputs the chapters to an OGM file
 
         :param out:     Can be either a directory or a full file path
         """
         if not out:
             out = get_workdir()
```

### Comparing `muxtools-0.0.9/muxtools/muxing/muxfiles.py` & `muxtools-0.1.0/muxtools/muxing/muxfiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from pathlib import Path
 from dataclasses import dataclass
 from pymediainfo import MediaInfo, Track
+from datetime import timedelta
+from typing import Any
 
 from .tracks import VideoTrack
 
 from ..utils.log import error
 from ..utils.glob import GlobSearch
 from ..utils.env import run_commandline
 from ..utils.download import get_executable
@@ -74,14 +76,15 @@
         """
         return VideoTrack(self.file, name, lang, default, forced, self.container_delay, timecode_file, crop, args)
 
 
 @dataclass
 class AudioFile(MuxingFile):
     info: AudioInfo | None = None
+    duration: timedelta | None = None
 
     def __post_init__(self):
         self.file = ensure_path_exists(self.file, self)
 
     def get_containerinfo(self, mediainfo: MediaInfo | None = None) -> Track:
         if not mediainfo:
             mediainfo = MediaInfo.parse(self.file)
@@ -98,15 +101,15 @@
         minfo = self.get_mediainfo()
         form = format_from_track(minfo)
         if form:
             return form.lossy
 
         return getattr(minfo, "compression_mode", "lossless").lower() == "lossy"
 
-    def has_multiple_tracks(self, caller: any = None) -> bool:
+    def has_multiple_tracks(self, caller: Any = None) -> bool:
         fileIn = ensure_path_exists(self.file, caller)
         minfo = MediaInfo.parse(fileIn)
         if len(minfo.audio_tracks) > 1 or len(minfo.video_tracks) > 1 or len(minfo.text_tracks) > 1:
             return True
         elif len(minfo.audio_tracks) == 0:
             raise error(f"'{fileIn.name}' does not contain an audio track!", caller)
         return False
@@ -129,15 +132,15 @@
             if delete:
                 self.file.unlink()
             return out
         else:
             raise error("Failed to mux AudioFile to mka.", self)
 
     @staticmethod
-    def from_file(pathIn: PathLike, caller: any):
+    def from_file(pathIn: PathLike, caller: Any):
         from ..utils.log import warn
 
         file = ensure_path_exists(pathIn, caller)
         if file.suffix.lower() != ".wav":
             warn("It's strongly recommended to explicitly extract tracks first!", caller, 1)
 
         return AudioFile(file, 0, file)
```

### Comparing `muxtools-0.0.9/muxtools/muxing/tracks.py` & `muxtools-0.1.0/muxtools/muxing/tracks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from shlex import join as join_args, split as split_args
+from shlex import split as split_args
 
 from ..utils.glob import GlobSearch
 from ..utils.types import PathLike, TrackType
 from ..utils.files import ensure_path_exists, get_absolute_tracknum
 
 # fmt: off
 __all__ = [
@@ -53,38 +53,51 @@
         self.forced = forced
         self.name = name
         self.delay = file.container_delay if isinstance(file, MuxingFile) else delay
         self.lang = lang
         self.type = type if isinstance(type, TrackType) else (TrackType(type) if isinstance(type, int) else TrackType[type.upper()])
         self.args = args
 
-    def mkvmerge_args(self) -> str:
-        self.file = self.file if isinstance(self.file, Path) else Path(self.file)
+    def mkvmerge_args(self) -> list[str]:
+        filepath = str(self.file.resolve())
         if self.type == TrackType.ATTACHMENT:
             is_font = self.file.suffix.lower() in [".ttf", ".otf"]
             if not is_font and not self.lang:
                 raise ValueError(f"Please specify a mimetype for the attachments if they're not fonts!")
             if not is_font:
-                return f' --attachment-mime-type {self.lang} --attach-file "{self.file.resolve()}"'
+                args = ["--attachment-mime-type", self.lang]
             else:
-                return f' --attachment-mime-type {"font/ttf" if self.file.suffix.lower() == ".ttf" else "font/otf"} --attach-file "{self.file.resolve()}"'
+                args = ["--attachment-mime-type", "font/ttf" if self.file.suffix.lower() == ".ttf" else "font/otf"]
+            if self.name:
+                args.extend(["--attachment-name", self.name])
+
+            args.extend(["--attach-file", filepath])
+            return args
+
         elif self.type == TrackType.MKV:
-            return f' {join_args(self.args)} "{self.file.resolve()}"'
+            return [*self.args, filepath]
         elif self.type == TrackType.CHAPTERS:
-            return f' --chapters "{self.file.resolve()}"'
-        name_args = f' --track-name "0:{self.name}"' if self.name else ""
-        lang_args = f" --language 0:{self.lang}" if self.lang else ""
-        delay_args = f" --sync 0:{self.delay}" if self.delay else ""
-        default_args = f' --default-track-flag 0:{"yes" if self.default else "no"}'
-        forced_args = f' --forced-display-flag 0:{"yes" if self.forced else "no"}'
+            return ["--chapters", filepath]
+        args = ["--track-name", f"0:{self.name}"]
+        if self.lang:
+            args.extend(["--language", f"0:{self.lang}"])
+        if self.delay:
+            args.extend(["--sync", f"0:{self.delay}"])
+        args.extend(
+            [
+                "--default-track-flag",
+                f"0:{'yes' if self.default else 'no'}",
+                "--forced-display-flag",
+                f"0:{'yes' if self.forced else 'no'}",
+            ]
+        )
         if self.args:
-            other_args = join_args(self.args)
-        else:
-            other_args = ""
-        return f'{other_args}{name_args}{lang_args}{default_args}{forced_args}{delay_args} "{self.file.resolve()}"'
+            args.extend(self.args)
+        args.append(filepath)
+        return args
 
 
 class VideoTrack(_track):
     """
     _track object with VIDEO type preselected and japanese language default
 
     :param timecode_file:       Pass a path for proper vfr playback if needed.
@@ -134,16 +147,16 @@
 
 
 class Attachment(_track):
     """
     pseudo _track object for attachments
     """
 
-    def __init__(self, file: str | Path, mimetype: str = "") -> None:
-        super().__init__(file, TrackType.ATTACHMENT, lang=mimetype)
+    def __init__(self, file: str | Path, mimetype: str = "", name: str = "") -> None:
+        super().__init__(file, TrackType.ATTACHMENT, lang=mimetype, name=name)
 
 
 class SubTrack(_track):
     """
     _track object with SUB type preselected and english language default
 
     Supports merging multiple files by passing a List of Path objects or filepath strings
@@ -167,73 +180,77 @@
     def __init__(
         self,
         file: PathLike | GlobSearch,
         video: int | list[int] | None = -1,
         audio: int | list[int] | None = -1,
         subtitles: int | list[int] | None = -1,
         keep_attachments: bool = True,
-        mkvmerge_args: str = "--no-global-tags",
+        mkvmerge_args: str | list[str] = "--no-global-tags",
+        assume_absolute: bool = False,
     ) -> None:
         """
         Custom Track object to arbitrarily grab tracks from an existing file.
 
         For all track params:
         `None` means there won't be any chosen and `-1` means all will be chosen.
         You can also specify a single or multiple *relative* track numbers to choose any.
 
         :param video:               Video Track(s) to choose
         :param audio:               Audio Track(s) to choose
         :param subtitles:           Subtitle Track(s) to choose
         :param keep_attachments:    Whether to keep attachments from the file. Fonts for example.
         :param mkvmerge_args:       Any other args you may want to pass.
+        :param assume_absolute:     Assume that the track numbers passed were already absolute to begin with.
+                                    If False it will simply get absolute numbers derived from the relative ones.
         """
         args = ""
         if video is None:
             args += " -D"
         elif video != -1:
             if isinstance(video, list):
                 lv = []
                 for num in video:
-                    abso = get_absolute_tracknum(file, num, TrackType.VIDEO)
+                    abso = get_absolute_tracknum(file, num, TrackType.VIDEO) if not assume_absolute else num
                     lv.append(abso)
                 args += f" -d {','.join(str(i) for i in lv)}"
             else:
-                abso = get_absolute_tracknum(file, video, TrackType.VIDEO)
+                abso = get_absolute_tracknum(file, video, TrackType.VIDEO) if not assume_absolute else video
                 args += f" -d {abso}"
 
         if audio is None:
             args += " -A"
         elif audio != -1:
             if isinstance(audio, list):
                 la = []
                 for num in audio:
-                    abso = get_absolute_tracknum(file, num, TrackType.AUDIO)
+                    abso = get_absolute_tracknum(file, num, TrackType.AUDIO) if not assume_absolute else num
                     la.append(abso)
                 args += f" -a {','.join(str(i) for i in la)}"
             else:
-                abso = get_absolute_tracknum(file, audio, TrackType.AUDIO)
+                abso = get_absolute_tracknum(file, audio, TrackType.AUDIO) if not assume_absolute else audio
                 args += f" -a {abso}"
 
         if subtitles is None:
             args += " -S"
         elif subtitles != -1:
             if isinstance(subtitles, list):
                 ls = []
                 for num in subtitles:
-                    abso = get_absolute_tracknum(file, num, TrackType.SUB)
+                    abso = get_absolute_tracknum(file, num, TrackType.SUB) if not assume_absolute else num
                     ls.append(abso)
                 args += f" -s {','.join(str(i) for i in ls)}"
             else:
-                abso = get_absolute_tracknum(file, subtitles, TrackType.SUB)
+                abso = get_absolute_tracknum(file, subtitles, TrackType.SUB) if not assume_absolute else subtitles
                 args += f" -s {abso}"
 
         if not keep_attachments:
             args += " -M"
 
-        args = f" {args.strip()} {mkvmerge_args.strip()}"
-        super().__init__(file, TrackType.MKV, args=split_args(args))
+        args = split_args(args.strip())
+        mkvmerge_args = split_args(mkvmerge_args.strip()) if isinstance(mkvmerge_args, str) else mkvmerge_args
+        super().__init__(file, TrackType.MKV, args=args + mkvmerge_args)
 
 
 VT = VideoTrack
 AT = AudioTrack
 ST = SubTrack
 MkvTrack = Premux
```

### Comparing `muxtools-0.0.9/muxtools/subtitle/font.py` & `muxtools-0.1.0/muxtools/subtitle/font.py`

 * *Files 17% similar despite different names*

```diff
@@ -34,24 +34,36 @@
     from font_collector import set_loglevel
 
     set_loglevel(logging.CRITICAL)
 
     from font_collector import AssDocument, FontLoader, Helpers, Font
 
     def _get_fontname(font: Font) -> str:
+        filename_fallback = False
+        exact_fallback = False
         try:
-            familyname = font.family_names.pop()
-            if " " in familyname:
-                familyname = "".join([part.capitalize() for part in familyname.split(" ")])
+            try:
+                name = font.family_names.pop().strip()
+            except:
+                name = font.exact_names.pop().strip()
+                exact_fallback = True
+        except:
+            name = Path(font.filename).with_suffix("").name.strip()
+            filename_fallback = True
+
+        if not filename_fallback:
+            if " " in name:
+                name = "".join([part.capitalize() for part in name.split(" ")])
+            elif "-" in name and exact_fallback:
+                name = "".join([part.strip().capitalize() for part in name.split("-")])
             else:
-                familyname.capitalize()
+                name = name.capitalize()
             weight = _weight_to_name(font.weight)
-            name = f"{familyname}{'-' + weight if weight else ''}{'Italic' if font.italic else ''}"
-        except:
-            name = Path(font.filename).name
+            name = f"{name}{'-' + weight if weight and weight not in name else ''}{'Italic' if font.italic else ''}"
+
         return name
 
     loaded_fonts = FontLoader(additional_fonts, use_system_font=use_system_fonts).fonts
 
     doc = AssDocument(sub._read_doc())
     styles = doc.get_used_style(collect_draw_fonts)
```

### Comparing `muxtools-0.0.9/muxtools/subtitle/sub.py` & `muxtools-0.1.0/muxtools/subtitle/sub.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 from __future__ import annotations
 from ass import Document, Comment, Dialogue, Style, parse as parseDoc
+from collections.abc import Callable
 from dataclasses import dataclass
 from typing import Any, TypeVar
 from datetime import timedelta
 from fractions import Fraction
 from pathlib import Path
 import shutil
 import json
 import re
 import os
 
-from .styles import GJM_GANDHI_PRESET
+from .styles import GJM_GANDHI_PRESET, resize_preset
 from .subutils import create_document, dummy_video, has_arch_resampler
 from ..utils.glob import GlobSearch
 from ..utils.download import get_executable
 from ..utils.types import PathLike, TrackType
 from ..utils.log import debug, error, info, warn
 from ..utils.convert import frame_to_timedelta, timedelta_to_frame
 from ..utils.env import get_temp_workdir, get_workdir, run_commandline
 from ..utils.files import ensure_path_exists, get_absolute_track, make_output, clean_temp_files, uniquify_path
 from ..muxing.muxfiles import MuxingFile
+from .basesub import BaseSubFile, _Line, ASSHeader
 
 __all__ = ["FontFile", "SubFile", "DEFAULT_DIALOGUE_STYLES"]
 
-
 DEFAULT_DIALOGUE_STYLES = ["default", "main", "alt", "overlap", "flashback", "top", "italics"]
 SRT_REGEX = r"\d+[\r\n](?:(?P<start>\d+:\d+:\d+,\d+) --> (?P<end>\d+:\d+:\d+,\d+))[\r\n](?P<text>(?:.+\r?\n)+(?=(\r?\n)?))"
+LINES = list[_Line]
 
 
 @dataclass
 class FontFile(MuxingFile):
     pass
 
 
 @dataclass
-class SubFile(MuxingFile):
+class SubFile(BaseSubFile):
     """
     Utility class representing a subtitle file with various functions to run on.
 
     :param file:            Can be a string, Path object or GlobSearch.
                             If the GlobSearch returns multiple results or if a list was passed it will merge them.
 
     :param container_delay: Set a container delay used in the muxing process later.
@@ -84,176 +86,218 @@
             self.source = self.file
             if not os.path.samefile(self.file.parent, get_workdir()):
                 out = make_output(self.file, "ass", "vof")
                 with open(out, "w", encoding=self.encoding) as writer:
                     self._read_doc().dump_file(writer)
                 self.file = out
 
-    def _read_doc(self, file: PathLike | None = None) -> Document:
-        with open(self.file if not file else file, "r", encoding=self.encoding) as reader:
-            return parseDoc(reader)
+    def manipulate_lines(self: SubFileSelf, func: Callable[[LINES], LINES | None]) -> SubFileSelf:
+        """
+        Function to manipulate any lines.
 
-    def __update_doc(self, doc: Document):
-        with open(self.file, "w", encoding=self.encoding) as writer:
-            doc.dump_file(writer)
+        :param func:        Your own function you want to run on the list of lines.
+                            This can return a new list or just edit the one passed into it.
+        """
+        super().manipulate_lines(func)
+        return self
+
+    def set_header(self: SubFileSelf, header: str | ASSHeader, value: str | int | bool | None) -> SubFileSelf:
+        """
+        A function to add headers to the "Script Info" section of the subtitle file.
+        This will validate the input for known functional headers but also allows arbitrary ones.
+        If you're planning on setting multiple at the same time, use the `set_headers` function instead to avoid a lot of I/O.
+
+        :param header:      The name of the header or a header chosen from the enum.
+        :param value:       The value of the header. None will remove the header unless it's the Matrix header because None has a meaning there.
+        """
+        super().set_header(header, value)
+        return self
+
+    def set_headers(self: SubFileSelf, *headers: tuple[str | ASSHeader, str | int | bool | None]) -> SubFileSelf:
+        """
+        A function to add headers to the "Script Info" section of the subtitle file.
+        This will validate the input for known functional headers but also allows arbitrary ones.
+
+        :param headers:     Any amount of tuples with the same typing as the single header function.
+        """
+        doc = self._read_doc()
+        for header, value in headers:
+            super().set_header(header, value, doc)
+        self._update_doc(doc)
+        return self
 
     def clean_styles(self: SubFileSelf) -> SubFileSelf:
         """
         Deletes unused styles from the document
         """
         doc = self._read_doc()
         used_styles = {line.style for line in doc.events if line.TYPE == "Dialogue"}
         regex = re.compile(r"\{.*?\\r([^\\]+)\}")
         for line in [line for line in doc.events if line.TYPE == "Dialogue"]:
             for match in regex.finditer(line.text):
                 used_styles.add(match.group(1))
         doc.styles = [style for style in doc.styles if style.name in used_styles]
-        self.__update_doc(doc)
+        self._update_doc(doc)
         return self
 
     def clean_garbage(self: SubFileSelf) -> SubFileSelf:
         """
         Removes the "Aegisub Project Garbage" section from the file
         """
         doc = self._read_doc()
         doc.sections.pop("Aegisub Project Garbage", None)
-        self.__update_doc(doc)
+        self._update_doc(doc)
         return self
 
-    def autoswapper(self: SubFileSelf, allowed_styles: list[str] | None = DEFAULT_DIALOGUE_STYLES, print_swaps: bool = False) -> SubFileSelf:
+    def autoswapper(
+        self: SubFileSelf,
+        allowed_styles: list[str] | None = DEFAULT_DIALOGUE_STYLES,
+        print_swaps: bool = False,
+        inline_marker: str = "*",
+        line_marker: str = "***",
+    ) -> SubFileSelf:
         """
         autoswapper does the swapping.
         Too lazy to explain
 
         :param allowed_styles:      List of allowed styles to do the swapping on
                                     Will run on every line if passed `None`
         :param print_swaps:         Prints the swaps
+        :param inline_marker:       Marker to use for inline swaps.
+                                    Should be one character. Default `*`
+        :param line_marker:         Marker to use for full-line swaps. Default `***`
 
         :return:                    This SubTrack
         """
-        doc = self._read_doc()
-
-        events = []
+        if not isinstance(inline_marker, str) or not inline_marker.strip():
+            warn("Given invalid inline marker. Using default '*'.", self)
+            inline_marker = "*"
+
+        if not isinstance(line_marker, str) or not line_marker.strip():
+            warn("Given invalid line marker. Using default '***'.", self)
+            line_marker = "***"
+
+        marker = re.escape(inline_marker)
+
+        ab_swap_regex = re.compile(rf"{{{marker}}}([^{{]*){{{marker}([^}}*]+)}}")
+        show_word_regex = re.compile(rf"{{{marker}{marker}([^}}]+)}}")
+        hide_word_regex = re.compile(rf"{{{marker}}}([^{{]*){{{marker} *}}")
+
+        def _do_autoswap(lines: LINES):
+            for i, line in enumerate(lines):
+                if not allowed_styles or str(line.style).casefold() in {style.casefold() for style in allowed_styles}:
+                    to_swap: dict = {}
+                    # {*}This will be replaced{*With this}
+                    for match in re.finditer(ab_swap_regex, line.text):
+                        to_swap.update({f"{match.group(0)}": f"{{{inline_marker}}}{match.group(2)}{{{inline_marker}{match.group(1)}}}"})
+
+                    # This sentence is no longer{** incomplete}
+                    for match in re.finditer(show_word_regex, line.text):
+                        to_swap.update({f"{match.group(0)}": f"{{{inline_marker}}}{match.group(1)}{{{inline_marker}}}"})
+
+                    # This sentence is no longer{*} incomplete{*}
+                    for match in re.finditer(hide_word_regex, line.text):
+                        to_swap.update({f"{match.group(0)}": f"{{{inline_marker*2}{match.group(1)}}}"})
+                    # print(to_swap)
+                    for key, val in to_swap.items():
+                        if print_swaps:
+                            info(f'autoswapper: Swapped "{key}" for "{val}" on line {i}', self)
+                        line.text = line.text.replace(key, val)
+
+                    if line.effect.strip() == line_marker or line.name.strip() == line_marker:
+                        if isinstance(line, Comment):
+                            line.TYPE = "Dialogue"
+                            if print_swaps:
+                                info(f'autoswapper: Uncommented Line {i} - "{line.text}"', self)
+                        elif isinstance(line, Dialogue):
+                            line.TYPE = "Comment"
+                            if print_swaps:
+                                info(f'autoswapper: Commented Line {i} - "{line.text}"', self)
 
-        for i, line in enumerate(doc.events):
-            if not allowed_styles or line.style.lower() in (style.lower() for style in allowed_styles):
-                to_swap: dict = {}
-                # {*}This will be replaced{*With this}
-                for match in re.finditer(re.compile(r"\{\*\}([^{]*)\{\*([^}*]+)\}"), line.text):
-                    to_swap.update({f"{match.group(0)}": f"{{*}}{match.group(2)}{{*{match.group(1)}}}"})
-
-                # This sentence is no longer{** incomplete}
-                for match in re.finditer(re.compile(r"\{\*\*([^}]+)\}"), line.text):
-                    to_swap.update({f"{match.group(0)}": f"{{*}}{match.group(1)}{{*}}"})
-
-                # This sentence is no longer{*} incomplete{*}
-                for match in re.finditer(re.compile(r"\{\*\}([^{]*)\{\* *\}"), line.text):
-                    to_swap.update({f"{match.group(0)}": f"{{**{match.group(1)}}}"})
-                # print(to_swap)
-                for key, val in to_swap.items():
-                    if print_swaps:
-                        info(f'autoswapper: Swapped "{key}" for "{val}" on line {i}', self)
-                    line.text = line.text.replace(key, val)
-
-            if line.effect.strip() == "***" or line.name.strip() == "***":
-                if isinstance(line, Comment):
-                    line.TYPE = "Dialogue"
-                elif isinstance(line, Dialogue):
-                    line.TYPE = "Comment"
-
-            events.append(line)
-
-        doc.events = events
-        self.__update_doc(doc)
+        self.manipulate_lines(_do_autoswap)
         return self
 
     def unfuck_cr(
         self: SubFileSelf,
         default_style: str = "Default",
         keep_flashback: bool = True,
         dialogue_styles: list[str] | None = ["main", "default", "narrator", "narration"],
         top_styles: list[str] | None = ["top"],
         italics_styles: list[str] | None = ["italics", "internal"],
+        alt_style: str = "Alt",
+        alt_styles: list[str] | None = None,
     ) -> SubFileSelf:
         """
         Removes any top and italics styles and replaces them with tags.
 
         :param default_style:       The default style that everything will be set to
         :param keep_flashback:      If not it will set the flashback styles to default_style
         :param dialogue_styles:     Styles that will be set to default_style
         :param top_styles:          Styles that will be set to default_style and an8 added to tags
         :param italics_styles:      Styles that will be set to default_style and i1 added to tags
+        :param alt_style:           The default alt/overlap style that lines will be set to
+        :param alt_styles:          Possible identifiers for styles that should be set to the alt_style
         """
-        doc = self._read_doc()
-        events = []
-        for line in doc.events:
-            add_italics_tag = False
-            if italics_styles:
-                for s in italics_styles:
-                    if s.casefold() in line.style.casefold():
-                        add_italics_tag = True
-                        if "flashback" in line.style.lower():
-                            line.style = default_style if not keep_flashback else "Flashback"
-                        else:
-                            line.style = default_style
-                        break
-            add_top_tag = False
-            if top_styles:
-                for s in top_styles:
+
+        def get_default(line: _Line, allow_default: bool = True) -> str:
+            placeholder = default_style
+            is_default = True
+            if alt_styles:
+                for s in alt_styles:
                     if s.casefold() in line.style.casefold():
-                        add_top_tag = True
-                        if "flashback" in line.style.lower():
-                            line.style = default_style if not keep_flashback else "Flashback"
-                        else:
+                        placeholder = alt_style
+                        is_default = False
+            if "flashback" in line.style.lower():
+                return placeholder if not keep_flashback else "Flashback"
+
+            if is_default:
+                return placeholder if allow_default else line.style
+
+            return placeholder
+
+        def _func(lines: LINES):
+            for line in lines:
+                add_italics_tag = italics_styles and bool([s for s in italics_styles if s.casefold() in line.style.casefold()])
+                add_top_tag = top_styles and bool([s for s in top_styles if s.casefold() in line.style.casefold()])
+
+                if any([add_italics_tag, add_top_tag]):
+                    line.style = get_default(line)
+                    tags = "" if not add_italics_tag else R"\i1"
+                    tags = tags if not add_top_tag else tags + R"\an8"
+                    line.text = f"{{{tags}}}{line.text}"
+
+                line.style = get_default(line, False)
+
+                if dialogue_styles:
+                    for s in dialogue_styles:
+                        if s.casefold() in line.style.casefold():
                             line.style = default_style
-                        break
-            if add_italics_tag and add_top_tag:
-                line.text = R"{\i1\an8}" + line.text
-            elif add_italics_tag:
-                line.text = R"{\i1}" + line.text
-            elif add_top_tag:
-                line.text = R"{\an8}" + line.text
-
-            if not keep_flashback:
-                if "flashback" in line.style.lower():
-                    line.style = default_style
-            else:
-                if line.style == "flashback":
-                    line.style = "Flashback"
-            if dialogue_styles:
-                for s in dialogue_styles:
-                    if s.casefold() in line.style.casefold():
-                        line.style = default_style
-            events.append(line)
-        doc.events = events
-        self.__update_doc(doc)
-        return self.clean_styles()
+
+        return self.manipulate_lines(_func).clean_styles()
 
     def shift_0(
         self: SubFileSelf, fps: Fraction | PathLike = Fraction(24000, 1001), allowed_styles: list[str] | None = DEFAULT_DIALOGUE_STYLES
     ) -> SubFileSelf:
         """
         Does the famous shift by 0 frames to fix frame timing issues.
         (It's basically just converting time to frame and back)
 
         This does not currently exactly reproduce the aegisub behaviour but it should have the same effect.
 
         :param fps:             The fps fraction used for conversions. Also accepts a timecode (v2) file.
         :param allowed_styles:  A list of style names this will run on. Will run on every line if None.
         """
-        doc = self._read_doc()
-        events = []
-        for line in doc.events:
-            if not allowed_styles or line.style.lower() in allowed_styles:
-                line.start = frame_to_timedelta(timedelta_to_frame(line.start, fps), fps, True)
-                line.end = frame_to_timedelta(timedelta_to_frame(line.end, fps), fps, True)
-            events.append(line)
-        doc.events = events
-        self.__update_doc(doc)
-        return self
+
+        def _func(lines: LINES):
+            for line in lines:
+                if not allowed_styles or line.style.lower() in allowed_styles:
+                    line.start = frame_to_timedelta(timedelta_to_frame(line.start, fps, exclude_boundary=True), fps, True)
+                    line.end = frame_to_timedelta(timedelta_to_frame(line.end, fps, exclude_boundary=True), fps, True)
+
+        return self.manipulate_lines(_func)
 
     def merge(
         self: SubFileSelf,
         file: PathLike | GlobSearch,
         sync: None | int | str = None,
         sync2: None | str = None,
         fps: Fraction | PathLike = Fraction(24000, 1001),
@@ -283,15 +327,15 @@
 
         # Find syncpoint in current document if sync is a string
         for line in doc.events:
             events.append(line)
             if target == None and isinstance(sync, str):
                 field = line.name if use_actor_field else line.effect
                 if field.lower().strip() == sync.lower().strip() or line.text.lower().strip() == sync.lower().strip():
-                    target = timedelta_to_frame(line.start, fps)
+                    target = timedelta_to_frame(line.start, fps, exclude_boundary=True) + 1
 
         if target == None and isinstance(sync, str):
             msg = f"Syncpoint '{sync}' was not found."
             if no_error:
                 warn(msg, self)
                 return self
             raise error(msg, self)
@@ -301,142 +345,48 @@
         for line in mergedoc.events:
             if not isinstance(sync, str) and not sync2:
                 break
             else:
                 sync2 = sync2 or sync
             field = line.name if use_actor_field else line.effect
             if field.lower().strip() == sync2.lower().strip() or line.text.lower().strip() == sync2.lower().strip():
-                second_sync = timedelta_to_frame(line.start, fps)
+                second_sync = timedelta_to_frame(line.start, fps, exclude_boundary=True) + 1
                 mergedoc.events.remove(line)
                 break
 
         sorted_lines = sorted(mergedoc.events, key=lambda event: event.start)
 
         # Assume the first line to be the second syncpoint if none was found
         if second_sync == None:
             for l in filter(lambda event: event.TYPE != "Comment", sorted_lines):
-                second_sync = timedelta_to_frame(l.start, fps)
+                second_sync = timedelta_to_frame(l.start, fps, exclude_boundary=True) + 1
                 break
 
         # Merge lines from file
         for line in sorted_lines:
             # Don't apply any offset if sync=None for plain merging or if target == source
             if target == None or target == second_sync:
                 tomerge.append(line)
                 continue
 
             # Apply frame offset
             offset = (target or -1) - second_sync
-            line.start = frame_to_timedelta(timedelta_to_frame(line.start, fps) + offset, fps, True)
-            line.end = frame_to_timedelta(timedelta_to_frame(line.end, fps) + offset, fps, True)
+            line.start = frame_to_timedelta(timedelta_to_frame(line.start, fps, exclude_boundary=True) + offset, fps, True)
+            line.end = frame_to_timedelta(timedelta_to_frame(line.end, fps, exclude_boundary=True) + offset, fps, True)
             tomerge.append(line)
 
         if tomerge:
             events.extend(tomerge)
             doc.events = events
             for style in mergedoc.styles:
                 if style.name in existing_styles:
                     continue
                 doc.styles.append(style)
 
-        self.__update_doc(doc)
-        return self
-
-    def syncpoint_merge(
-        self: SubFileSelf,
-        syncpoint: str,
-        mergefile: PathLike | GlobSearch,
-        use_actor_field: bool = False,
-        use_frames: bool = False,
-        fps: Fraction | PathLike = Fraction(24000, 1001),
-        override_p1: int | timedelta = None,
-        add_offset: int | timedelta = None,
-    ) -> SubFileSelf:
-        """
-        Merge other sub files (Opening/Ending kfx for example) with offsetting by syncpoints
-
-        :param syncpoint:           The syncpoint to be used
-        :param mergefile:           The file to be merged
-        :param use_actor_field:     Search the actor field instead of the effect field for the syncpoint
-        :param use_frames:          Uses frames to shift lines instead of direct timestamps
-        :param fps:                 The fps to go off of for the conversion. Also accepts a timecode (v2) file.
-        :param override_p1:         A manual override of the initial syncpoint
-                                    Obviously either a frame number or timedelta
-
-        :return:                    This SubTrack
-        """
-        mergefile = ensure_path_exists(mergefile, self)
-        was_merged = False
-
-        doc = self._read_doc()
-        mergedoc = self._read_doc(mergefile)
-
-        events = []
-        tomerge = []
-        existing_styles = [style.name for style in doc.styles]
-
-        if isinstance(add_offset, int) and not use_frames:
-            add_offset = frame_to_timedelta(add_offset, fps, True)
-
-        for line in doc.events:
-            events.append(line)
-            if was_merged:
-                continue
-            field = line.name if use_actor_field else line.effect
-            if (
-                field.lower().strip() == syncpoint.lower().strip()
-                or line.text.lower().strip() == syncpoint.lower().strip()
-                or override_p1 is not None
-            ):
-                was_merged = True
-                start = line.start if override_p1 is None else override_p1
-                offset: timedelta | int = None
-                for l in mergedoc.events:
-                    lfield = l.name if use_actor_field else l.effect
-                    if lfield.lower().strip() == syncpoint.lower().strip() or l.text.lower().strip() == syncpoint.lower().strip():
-                        mergedoc.events.remove(l)
-                        if use_frames:
-                            offset = timedelta_to_frame(start - l.start, fps)
-                        else:
-                            offset = start - l.start
-
-                        if add_offset:
-                            offset += add_offset
-                        break
-
-                for l in sorted(mergedoc.events, key=lambda event: event.start):
-                    if offset is None:
-                        if use_frames:
-                            offset = timedelta_to_frame(start - l.start, fps)
-                        else:
-                            offset = start - l.start
-
-                        if add_offset:
-                            offset += add_offset
-
-                        l.start = start
-                        l.end = l.end + (frame_to_timedelta(offset, fps, True) if use_frames else offset)
-                    else:
-                        l.start = l.start + (frame_to_timedelta(offset, fps, True) if use_frames else offset)
-                        l.end = l.end + (frame_to_timedelta(offset, fps, True) if use_frames else offset)
-                    tomerge.append(l)
-
-        if was_merged:
-            events.extend(tomerge)
-            # Merge the styles in aswell
-            for style in mergedoc.styles:
-                if style.name in existing_styles:
-                    continue
-                doc.styles.append(style)
-
-            doc.events = events
-            self.__update_doc(doc)
-        else:
-            warn(f"Syncpoint '{syncpoint}' was not found!", self)
-
+        self._update_doc(doc)
         return self
 
     def collect_fonts(
         self, use_system_fonts: bool = True, search_current_dir: bool = True, additional_fonts: list[PathLike] = [], collect_draw_fonts: bool = True
     ) -> list[FontFile]:
         """
         Collects fonts for current subtitle.
@@ -470,37 +420,45 @@
                 resolved_paths.append(f)
         from .font import collect_fonts as collect
 
         debug(f"Collecting fonts for '{self.file.stem}'...", self)
 
         return collect(self, use_system_fonts, resolved_paths, collect_draw_fonts)
 
-    def restyle(self: SubFileSelf, styles: Style | list[Style], clean_after: bool = True, delete_existing: bool = False) -> SubFileSelf:
+    def restyle(
+        self: SubFileSelf, styles: Style | list[Style], clean_after: bool = True, delete_existing: bool = False, adjust_styles: bool = True
+    ) -> SubFileSelf:
         """
         Add (and replace existing) styles to the subtitle file.
 
         :param styles:          Either a single or a list of ass Styles
         :param clean_after:     Clean unused styles after
         :param delete_existing: Delete all existing styles before adding new ones
+        :param adjust_styles:   Resize the styles to match the script resolution.
+                                This assumes 1080p for the actual style res as all the presets are that.
         """
         if not isinstance(styles, list):
             styles = [styles]
 
         styles = styles.copy()
 
         doc = self._read_doc()
+        script_res = int(doc.info.get("PlayResY", 360))
+        if script_res != 1080 and adjust_styles:
+            styles = resize_preset(styles, script_res)
+
         if delete_existing:
             doc.styles = []
 
         names = [style.name.casefold() for style in styles]
         existing = [style for style in doc.styles if style.name.casefold() not in names]
         styles.extend(existing)
         doc.styles = styles
 
-        self.__update_doc(doc)
+        self._update_doc(doc)
         if clean_after:
             return self.clean_styles()
         else:
             return self
 
     def resample(
         self: SubFileSelf,
@@ -573,83 +531,79 @@
                     skip = not inverse
                     break
 
             if skip:
                 continue
             events.append(line)
         doc.events = events
-        self.__update_doc(doc)
+        self._update_doc(doc)
         return self.clean_styles()
 
-    def change_layers(self: SubFileSelf, styles: list[str] = DEFAULT_DIALOGUE_STYLES, layer: int = 99) -> SubFileSelf:
+    def change_layers(self: SubFileSelf, styles: list[str] = DEFAULT_DIALOGUE_STYLES, layer: int | None = None, additive: bool = True) -> SubFileSelf:
         """
-        Set layer to the specified number on every line with a style you selected.
+        Set layer to the specified number or adds the number to the existing one on every line with a style you selected.
 
-        :param styles:      List of styles to look for
-        :param layer:       The layer you want
+        :param styles:      List of styles to look for.
+        :param layer:       The layer you want. Defaults to 50 for additive and 99 otherwise.
+        :param additive:    Add specified layer number instead of replacing the existing one.
         """
-        doc = self._read_doc()
-        events = []
-        for line in doc.events:
-            for style in styles:
-                if str(line.style).strip().casefold() == style.strip().casefold():
-                    line.layer = layer
-            events.append(line)
-        doc.events = events
-        self.__update_doc(doc)
-        return self
+        if not layer:
+            layer = 50 if additive else 99
+
+        def _func(lines: LINES):
+            for line in lines:
+                for style in styles:
+                    if str(line.style).strip().casefold() == style.strip().casefold():
+                        line.layer = layer if not additive else line.layer + layer
+
+        return self.manipulate_lines(_func)
 
     def purge_macrons(self: SubFileSelf, styles: list[str] | None = DEFAULT_DIALOGUE_STYLES) -> SubFileSelf:
         """
         Removes romaji macrons from every dialogue line.
         German subs use this a lot and a lot of fonts don't support it, so I like to purge them.
 
         :param styles:      List of styles to look for
         """
-        macrons: list[tuple[str, str]] = [("ā", "a"), ("ē", "e"), ("Ī", "i"), ("ō", "o"), ("ū", "u")]
-        doc = self._read_doc()
-        events = []
-        for line in doc.events:
-            process = not styles
-            for style in styles or []:
-                if str(line.style).strip().casefold() == style.strip().casefold():
-                    process = True
-            if process:
-                for macron in macrons + [(m[0].upper(), m[1].upper()) for m in macrons]:
-                    line.text: str = line.text.replace(macron[0], macron[1])
-            events.append(line)
-        doc.events = events
-        self.__update_doc(doc)
-        return self
+        macrons: list[tuple[str, str]] = [("ā", "a"), ("ē", "e"), ("ī", "i"), ("ō", "o"), ("ū", "u")]
+
+        def _func(lines: LINES):
+            for line in lines:
+                process = not styles
+                for style in styles or []:
+                    if str(line.style).strip().casefold() == style.strip().casefold():
+                        process = True
+                if process:
+                    for macron in macrons + [(m[0].upper(), m[1].upper()) for m in macrons]:
+                        line.text = line.text.replace(macron[0], macron[1])
+
+        return self.manipulate_lines(_func)
 
     def shift(self: SubFileSelf, frames: int, fps: Fraction | PathLike = Fraction(24000, 1001)) -> SubFileSelf:
         """
         Shifts all lines by any frame number.
 
         :param frames:      Number of frames to shift by
         :param fps:         FPS needed for the timing calculations. Also accepts a timecode (v2) file.
         """
-        doc = self._read_doc()
-        events = []
-        for line in doc.events:
-            start = timedelta_to_frame(line.start, fps) + frames
-            if start < 0:
-                start = 0
-            start = frame_to_timedelta(start, fps, compensate=True)
-            end = timedelta_to_frame(line.end, fps) + frames
-            if end < 0:
-                continue
-            end = frame_to_timedelta(end, fps, compensate=True)
-            line.start = start
-            line.end = end
-            events.append(line)
 
-        doc.events = events
-        self.__update_doc(doc)
-        return self
+        def _func(lines: LINES):
+            for line in lines:
+                start = timedelta_to_frame(line.start, fps, exclude_boundary=True) + frames
+                if start < 0:
+                    start = 0
+                start = frame_to_timedelta(start, fps, compensate=True)
+                end = timedelta_to_frame(line.end, fps, exclude_boundary=True) + frames
+                if end < 0:
+                    continue
+                end = frame_to_timedelta(end, fps, compensate=True)
+                line.start = start
+                line.end = end
+
+        return self.manipulate_lines(_func)
 
     def copy(self: SubFileSelf) -> SubFileSelf:
         """
         Creates a new copy of the current SubFile object, including its file.
         So you can run anything on the new one without impacting the other one.
         """
         doc = self._read_doc()
@@ -659,59 +613,67 @@
 
         new = self.__class__(new_path, self.container_delay, self.source)
         new.encoding = self.encoding
         return new
 
     @classmethod
     def from_srt(
-        cls: type[SubFileSelf], file: PathLike, an8_all_caps: bool = True, fps: Fraction | PathLike = Fraction(24000, 1001), encoding: str = "UTF8"
+        cls: type[SubFileSelf],
+        file: PathLike,
+        an8_all_caps: bool = True,
+        style_all_caps: bool = True,
+        fps: Fraction | PathLike = Fraction(24000, 1001),
+        encoding: str = "UTF8",
     ) -> SubFileSelf:
         """
         Convert srt subtitles to an ass SubFile.
         Automatically applies Gandhi styling. Feel free to restyle.
         Also worth noting that this creates a file that assumes 1920x1080. Use the resample function if you need something else.
 
         :param file:            Input srt file
-        :param an8_all_caps:    Automatically an8 every full caps line with over 7 characters because they're usually signs
+        :param an8_all_caps:    Automatically an8 every full caps line with over 7 characters because they're usually signs.
+        :param style_all_caps:  Also set the style of these lines to "Sign" wether it exists or not.
         :param fps:             FPS needed for the time conversion. Also accepts a timecode (v2) file.
         :param encoding:        Encoding used to read the file. Defaults to UTF8.
         """
         caller = "SubFile.from_srt"
         file = ensure_path_exists(file, caller)
 
         compiled = re.compile(SRT_REGEX, re.MULTILINE)
 
         def srt_timedelta(timestamp: str) -> timedelta:
             args = timestamp.split(",")[0].split(":")
             parsed = timedelta(hours=int(args[0]), minutes=int(args[1]), seconds=int(args[2]), milliseconds=int(timestamp.split(",")[1]))
-            cope = timedelta_to_frame(parsed, fps)
+            cope = timedelta_to_frame(parsed, fps, exclude_boundary=True)
             cope = frame_to_timedelta(cope, fps, compensate=True)
             return cope
 
-        def convert_tags(text: str) -> str:
+        def convert_tags(text: str) -> tuple[str, bool]:
             text = text.strip().replace("\n", "\\N")
+            is_sign = False
             if an8_all_caps and text.upper() == text and len(text) > 7:
                 text = R"{\an8}" + text
+                is_sign = True
             text = re.sub(r"[\<|{]i[\>|}]", "{\\\i1}", text)
             text = re.sub(r"[\<|{]\/i[\>|}]", "{\\\i}", text)
             text = re.sub(r"[\<|{]b[\>|}]", "{\\b1}", text)
             text = re.sub(r"[\<|{]\/b[\>|}]", "{\\b}", text)
             text = re.sub(r"[\<|{]u[\>|}]", R"{\\u1}", text)
             text = re.sub(r"[\<|{]\/u[\>|}]", R"{\\u}", text)
-            return text
+            return text, is_sign
 
         doc = create_document()
 
         with open(file, "r", encoding=encoding) as reader:
             content = reader.read() + "\n"
             for match in compiled.finditer(content):
                 start = srt_timedelta(match["start"])
                 end = srt_timedelta(match["end"])
-                text = convert_tags(match["text"])
-                doc.events.append(Dialogue(layer=99, start=start, end=end, text=text))
+                text, sign = convert_tags(match["text"])
+                doc.events.append(Dialogue(layer=99, start=start, end=end, text=text, style="Sign" if sign and style_all_caps else "Default"))
 
         out = file.with_suffix(".ass")
         with open(out, "w", encoding="utf_8_sig") as writer:
             doc.dump_file(writer)
         out = cls(out, 0, file)
         return out.restyle(GJM_GANDHI_PRESET)
```

### Comparing `muxtools-0.0.9/muxtools/subtitle/subutils.py` & `muxtools-0.1.0/muxtools/subtitle/subutils.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.9/muxtools/utils/convert.py` & `muxtools-0.1.0/muxtools/utils/convert.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 from math import trunc
-from decimal import ROUND_HALF_DOWN, Decimal
+from decimal import *
 from fractions import Fraction
 from datetime import timedelta
-from typing import Any
 
 from ..utils.types import PathLike
 from ..utils.files import ensure_path_exists
 from ..utils.log import error
 
 __all__: list[str] = [
     "mpls_timestamp_to_timedelta",
@@ -31,90 +30,98 @@
 
     :return:                The resulting timedelta
     """
     seconds = Decimal(timestamp) / Decimal(45000)
     return timedelta(seconds=float(seconds))
 
 
-def _timedelta_from_timecodes(timecodes: PathLike, frame: int, compensate: bool = False, rounding: bool = False) -> timedelta:
+def _timedelta_from_timecodes(timecodes: PathLike, frame: int) -> timedelta:
     timecode_file = ensure_path_exists(timecodes, _timedelta_from_timecodes)
     parsed = [float(x) / 1000 for x in open(timecode_file, "r").read().splitlines()[1:]]
     if len(parsed) <= frame:
         raise error(f"Frame {frame} is out of range for the given timecode file!", _timedelta_from_timecodes)
 
     target = timedelta(seconds=parsed[frame])
-    if compensate and len(parsed) - 1 >= frame + 1:
-        next = timedelta(seconds=parsed[frame + 1])
-        target = target + (next - target) / 2
-        if rounding:
-            return timedelta(seconds=round(target.total_seconds(), 2))
     return target
 
 
 def _frame_from_timecodes(timecodes: PathLike, time: timedelta) -> int:
     timecode_file = ensure_path_exists(timecodes, _frame_from_timecodes)
-    parsed = [float(x) / 1000 for x in open(timecode_file, "r").read().splitlines()[1:]]
+    # Subtract 0.5 from timecodes to ensure correct behavior even with small rounding errors
+    # (A timedelta of 42ms should belong to frame [42, 83) with a timecode list [0, 42, 83, ...])
+    parsed = [(float(x) - 0.5) / 1000 for x in open(timecode_file, "r").read().splitlines()[1:]]
 
-    nearest_frame = min(parsed, key=lambda val: abs(val - time.total_seconds()))
-    return parsed.index(nearest_frame)
+    return len([t for t in parsed if t < time.total_seconds()]) - 1
 
 
-def timedelta_to_frame(time: timedelta, fps: Fraction | PathLike = Fraction(24000, 1001)) -> int:
+def timedelta_to_frame(
+    time: timedelta, fps: Fraction | PathLike = Fraction(24000, 1001), exclude_boundary: bool = False, allow_rounding: bool = True
+) -> int:
     """
     Converts a timedelta to a frame number.
 
-    :param time:    The timedelta
-    :param fps:     A Fraction containing fps_num and fps_den. Also accepts a timecode (v2) file.
+    :param time:                The timedelta
+    :param fps:                 A Fraction containing fps_num and fps_den. Also accepts a timecode (v2) file.
+
+    :param exclude_boundary:    Associate frame boundaries with the previous frame rather than the current one.
+                                Use this option when dealing with subtitle start/end times.
 
-    :return:        The resulting frame number
+    :param allow_rounding:      Use the next int if the difference to the next frame is smaller than 0.01.
+                                This should *probably* not be used for subtitles. We are not sure.
+
+    :return:                    The resulting frame number
     """
+    if exclude_boundary:
+        return timedelta_to_frame(time - timedelta(milliseconds=1), fps, allow_rounding=False)
+
     if not isinstance(fps, Fraction):
         return _frame_from_timecodes(fps, time)
-    ms = Decimal(time.total_seconds()) * 1000
-    fps_dec = _fraction_to_decimal(fps)
 
-    upper_bound = (ms + Decimal(0.5)) * fps_dec / 1000
-    trunc_frame = int(upper_bound)
+    ms = int(Decimal(time.total_seconds()).__round__(3) * 1000)
+    frame = ms * fps / 1000
+    frame_dec = Decimal(frame.numerator) / Decimal(frame.denominator)
+
+    # Return next int if difference is less than 0.01
+    if allow_rounding and abs(frame_dec.__round__(3) - frame_dec.__ceil__()) < 0.01:
+        return frame_dec.__ceil__()
 
-    if upper_bound == trunc_frame:
-        return trunc_frame - 1
-
-    return trunc_frame
+    return int(frame)
 
 
 def frame_to_timedelta(f: int, fps: Fraction | PathLike = Fraction(24000, 1001), compensate: bool = False, rounding: bool = True) -> timedelta:
     """
     Converts a frame number to a timedelta.
     Mostly used in the conversion for manually defined chapters.
 
     :param f:           The frame number
     :param fps:         A Fraction containing fps_num and fps_den. Also accepts a timecode (v2) file.
     :param compensate:  Whether to place the timestamp in the middle of said frame
                         Useful for subtitles, not so much for audio where you'd want to be accurate
     :param rounding:    Round compensated value to centi seconds if True
     :return:            The resulting timedelta
     """
-    if not f or f < 0:
-        return timedelta(seconds=0)
-
-    if not isinstance(fps, Fraction):
-        return _timedelta_from_timecodes(fps, f, compensate, rounding)
+    result = None
 
-    fps_dec = _fraction_to_decimal(fps)
-    seconds = Decimal(f) / fps_dec
-    if not compensate:
-        return timedelta(seconds=float(seconds))
+    if compensate:
+        result = (frame_to_timedelta(f, fps, rounding=False) + frame_to_timedelta(f + 1, fps, rounding=False)) / 2
     else:
-        t1 = timedelta(seconds=float(seconds))
-        t2 = timedelta(seconds=float(Decimal(f + 1) / fps_dec))
-        result = t1 + (t2 - t1) / 2
-        if not rounding:
-            return result
-        rounded = round(result.total_seconds(), 2)
-        return timedelta(seconds=rounded)
+        if not f or f < 0:
+            return timedelta(seconds=0)
+
+        if isinstance(fps, Fraction):
+            fps_dec = _fraction_to_decimal(fps)
+            seconds = Decimal(f) / fps_dec
+            result = timedelta(seconds=float(seconds))
+        else:
+            result = _timedelta_from_timecodes(fps, f)
+
+    if not rounding:
+        return result
+    rounded = round(result.total_seconds(), 2)
+    return timedelta(seconds=rounded)
 
 
 def frame_to_ms(f: int, fps: Fraction | PathLike = Fraction(24000, 1001), compensate: bool = False) -> float:
     """
     Converts a frame number to it's ms value.
 
     :param f:           The frame number
@@ -155,13 +162,12 @@
     Mostly to be used for ogm/xml files.
 
     :param formatted:       The timestamp string
 
     :return:                The parsed timedelta
     """
     # 00:05:25.534...
-    seconds: float = 0.0
     split = formatted.split(":")
-    seconds += float(split[0]) * 3600
-    seconds += float(split[1]) * 60
-    seconds += float(split[2])
-    return timedelta(seconds=seconds)
+    seconds = Decimal(split[0]) * Decimal(3600)
+    seconds = seconds + (Decimal(split[1]) * Decimal(60))
+    seconds = seconds + (Decimal(split[2]))
+    return timedelta(seconds=seconds.__float__())
```

### Comparing `muxtools-0.0.9/muxtools/utils/download.py` & `muxtools-0.1.0/muxtools/utils/download.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,23 +22,23 @@
     url: str
     alias: list[str] | None = None
 
 
 # fmt: off
 # Feel free to compare the hashes if you don't like the custom files
 tools = [
-    Tool("CUETools.FLACCL.cmd", "https://github.com/gchudov/cuetools.net/releases/download/v2.2.4/CUETools_2.2.4.zip", ["flaccl"]),
+    Tool("CUETools.FLACCL.cmd", "https://github.com/gchudov/cuetools.net/releases/download/v2.2.5/CUETools_2.2.5.zip", ["flaccl"]),
     # non-free builds for libfdk_aac if one so desires
-    Tool("ffmpeg", "https://github.com/AnimMouse/ffmpeg-autobuild/releases/download/m-2023-06-12-17-58/ffmpeg-09621fd-9b0e37c-win64-nonfree.7z", ["ffprobe"]),
-    Tool("mkvmerge", "https://mkvtoolnix.download/windows/releases/77.0/mkvtoolnix-64-bit-77.0.7z", ['mkvextract', 'mkvinfo', 'mkvpropedit']), 
+    Tool("ffmpeg", "https://github.com/AnimMouse/ffmpeg-autobuild/releases/download/2024-03-10-12-25-64634e8-a8e823a/ffmpeg-64634e8-a8e823a-win64-nonfree.7z", ["ffprobe"]),
+    Tool("mkvmerge", "https://mkvtoolnix.download/windows/releases/83.0/mkvtoolnix-64-bit-83.0.7z", ['mkvextract', 'mkvinfo', 'mkvpropedit']), 
     Tool("eac3to", "https://files.catbox.moe/hn9oms.7z"), # Custom package because of removed sounds and updated libFlac
     Tool("x264", "https://github.com/DJATOM/x264-aMod/releases/download/r3101+20/x264-aMod-x64-core164-r3101+20.7z"),
     Tool("x265", "https://github.com/DJATOM/x265-aMod/releases/download/3.5+67/x265-x64-v3.5+67-aMod-gcc12.2.1+opt.7z"),
     Tool("qaac", "https://files.catbox.moe/z9q796.7z"), # 2.79 with flac, w64 and iTunes libraries included
-    Tool("opusenc", "https://archive.mozilla.org/pub/opus/win32/opus-tools-0.2-opus-1.3.zip"),
+    Tool("opusenc", "https://www.rarewares.org/files/opus/opustools-0.2-20230419-x64.zip"),
     Tool("flac", "https://github.com/xiph/flac/releases/download/1.4.3/flac-1.4.3-win.zip"),
     Tool("wavpack", "https://github.com/dbry/WavPack/releases/download/5.6.0/wavpack-5.6.0-x64.zip")
 ]
 # fmt: on
 
 # TODO: check CPU to decide on which x264/5 file to use
```

### Comparing `muxtools-0.0.9/muxtools/utils/env.py` & `muxtools-0.1.0/muxtools/utils/env.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 import os
 import json
 import subprocess
 from pathlib import Path
+from typing import Any
 
 from ..main import Setup
 
-__all__ = ["save_setup", "get_setup_attr", "get_workdir", "get_temp_workdir", "is_debug", "download_allowed", "run_commandline"]
+__all__ = ["save_setup", "get_setup_attr", "get_setup_dir", "get_workdir", "get_temp_workdir", "is_debug", "download_allowed", "run_commandline"]
 
 
 def save_setup(setup: Setup):
     os.environ["vof_setup"] = setup._toJson()
 
 
-def get_setup_attr(attr: str, default: any = None) -> any:
+def get_setup_attr(attr: str, default: Any = None) -> Any:
     envi = os.environ.get("vof_setup")
     if not envi:
         return default
     loaded = json.loads(envi)
     if loaded:
         if isinstance(loaded, dict):
             return loaded.get(attr, default)
         return getattr(loaded, attr, default)
     return default
 
 
+def get_setup_dir() -> list[str]:
+    envi = os.environ.get("vof_setup")
+    if not envi:
+        return []
+    loaded = json.loads(envi)
+    return loaded.keys() if isinstance(loaded, dict) else dir(loaded)
+
+
 def get_workdir() -> Path:
     return Path(get_setup_attr("work_dir", os.getcwd()))
 
 
 def get_temp_workdir() -> Path:
     wd = Path(get_workdir(), ".temp")
     wd.mkdir(parents=True, exist_ok=True)
@@ -38,16 +47,27 @@
     return get_setup_attr("debug", True)
 
 
 def download_allowed() -> bool:
     return get_setup_attr("allow_binary_download", False)
 
 
-def run_commandline(command: str | list[str], quiet: bool = True, shell: bool = False, stdin=subprocess.DEVNULL, **kwargs) -> int:
+def run_commandline(
+    command: str | list[str], quiet: bool = True, shell: bool = False, stdin=subprocess.DEVNULL, mkvmerge: bool = False, **kwargs
+) -> int:
     if os.name != "nt" and isinstance(command, str):
         shell = True
     if quiet:
-        p = subprocess.Popen(command, stdin=stdin, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL, shell=shell, **kwargs)
+        p = subprocess.Popen(
+            command, stdin=stdin, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, universal_newlines=True, text=True, shell=shell, **kwargs
+        )
     else:
         p = subprocess.Popen(command, stdin=stdin, shell=shell, **kwargs)
 
-    return p.wait()
+    returncode = p.wait()
+    if returncode > (1 if mkvmerge else 0) and p.stdout and quiet and (lines := p.stdout.readlines()):
+        print("\n----------------------")
+        for line in lines:
+            print(line.rstrip("\n"))
+        print("----------------------")
+
+    return returncode
```

### Comparing `muxtools-0.0.9/muxtools/utils/files.py` & `muxtools-0.1.0/muxtools/utils/files.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import os
+import re
 import binascii
 from pathlib import Path
 from shutil import rmtree
 from copy import deepcopy
+from typing import Any
+from collections.abc import Callable
 from pymediainfo import Track, MediaInfo
 
 from .log import *
 from .glob import GlobSearch
 from .types import PathLike, TrackType
 from .env import get_temp_workdir, get_workdir
 
@@ -14,31 +17,33 @@
     "ensure_path",
     "uniquify_path",
     "get_crc32",
     "make_output",
     "ensure_path_exists",
     "clean_temp_files",
     "get_absolute_track",
+    "get_track_list",
+    "find_tracks",
 ]
 
 
-def ensure_path(pathIn: PathLike, caller: any) -> Path:
+def ensure_path(pathIn: PathLike, caller: Any) -> Path:
     """
     Utility function for other functions to make sure a path was passed to them.
 
     :param pathIn:      Supposed passed Path
     :param caller:      Caller name used for the exception and error message
     """
     if pathIn is None:
         raise crit("Path cannot be None.", caller)
     else:
         return Path(pathIn).resolve()
 
 
-def ensure_path_exists(pathIn: PathLike | list[PathLike] | GlobSearch, caller: any, allow_dir: bool = False) -> Path:
+def ensure_path_exists(pathIn: PathLike | list[PathLike] | GlobSearch, caller: Any, allow_dir: bool = False) -> Path:
     """
     Utility function for other functions to make sure a path was passed to them and that it exists.
 
     :param pathIn:      Supposed passed Path
     :param caller:      Caller name used for the exception and error message
     """
     from ..muxing.muxfiles import MuxingFile
@@ -106,50 +111,122 @@
             return Path(user_passed, f"{source_stem}.{ext}").resolve()
         else:
             return user_passed.with_suffix(f".{ext}").resolve()
     else:
         return Path(uniquify_path(os.path.join(workdir, f"{source_stem}{f'_{suffix}' if suffix else ''}.{ext}"))).resolve()
 
 
-def get_absolute_track(file: PathLike, track: int, type: TrackType, caller: any = None) -> Track:
-    """
-    Finds the absolute track for a relative track number of a specific type.
-
-    :param file:    String or pathlib based Path
-    :param track:   Relative track number
-    :param type:    TrackType of the requested relative track
-    """
-    caller = caller if caller else get_absolute_track
-    file = ensure_path_exists(file, get_absolute_track)
+def get_track_list(file: PathLike, caller: Any = None) -> list[Track]:
+    """Makes a sanitized mediainfo track list"""
+    caller = caller if caller else get_track_list
+    file = ensure_path_exists(file, caller)
     mediainfo = MediaInfo.parse(file)
-
     current = 0
+    indexes = {"video": 0, "audio": 0, "text": 0}
     sanitized_list = []
     # Weird mediainfo quirks
     for t in mediainfo.tracks:
-        sanitized_list.append(t)
-        if t.track_type.lower() not in ["video", "audio", "text"]:
+        ttype = t.track_type.lower()
+        if ttype not in ["video", "audio", "text"]:
             continue
+        sanitized_list.append(t)
+
         t.track_id = current
+        current += 1
+        setattr(t, "relative_id", indexes[ttype])
+        indexes[ttype] = indexes[ttype] + 1
         if "truehd" in (getattr(t, "commercial_name", "") or "").lower() and "extension" in (getattr(t, "muxing_mode", "") or "").lower():
-            current += 1
             identifier = getattr(t, "format_identifier", "AC-3") or "AC-3"
             compat_track = deepcopy(t)
             compat_track.format = identifier
             compat_track.codec_id = f"A_{identifier.replace('-', '')}"
             compat_track.commercial_name = ""
             compat_track.compression_mode = "Lossy"
             compat_track.track_id = current
+            current += 1
+            setattr(compat_track, "relative_id", indexes[ttype])
+            indexes[ttype] = indexes[ttype] + 1
             sanitized_list.append(compat_track)
-        current += 1
 
-    mediainfo.tracks = sanitized_list
-    videos = mediainfo.video_tracks
-    audios = mediainfo.audio_tracks
-    subtitles = mediainfo.text_tracks
+    return sanitized_list
+
+
+def find_tracks(
+    file: PathLike,
+    name: str | None = None,
+    lang: str | None = None,
+    type: TrackType | None = None,
+    use_regex: bool = True,
+    reverse_lang: bool = False,
+    custom_condition: Callable[[Track], bool] | None = None,
+) -> list[Track]:
+    """
+    Convenience function to find tracks with some conditions.
+
+    :param file:                File to parse with MediaInfo.
+    :param name:                Name to match, case insensitively.
+    :param lang:                Language to match. This can be any of the possible formats like English/eng/en and is case insensitive.
+    :param type:                Track Type to search for.
+    :param use_regex:           Use regex for the name search instead of checking for equality.
+    :param reverse_lang:        If you want the `lang` param to actually exclude that language.
+    :param custom_condition:    Here you can pass any function to create your own conditions. (They have to return a bool)
+                                For example: custom_condition=lambda track: track.codec_id == "A_EAC3"
+    """
+
+    if not name and not lang and not type and not custom_condition:
+        return []
+    tracks = get_track_list(file)
+
+    def name_matches(title: str) -> bool:
+        if title.casefold().strip() == name.casefold().strip():
+            return True
+        if use_regex:
+            return re.match(name, title, re.I)
+        return False
+
+    def get_languages(track: MediaInfo) -> list[str]:
+        languages: list[str] = getattr(track, "other_language", None) or list[str]()
+        return [l.casefold() for l in languages]
+
+    if name:
+        tracks = [track for track in tracks if name_matches(getattr(track, "title", "") or "")]
+
+    if lang:
+        if reverse_lang:
+            tracks = [track for track in tracks if lang.casefold() not in get_languages(track)]
+        else:
+            tracks = [track for track in tracks if lang.casefold() in get_languages(track)]
+
+    if type:
+        if type not in (TrackType.VIDEO, TrackType.AUDIO, TrackType.SUB):
+            raise error("You can only search for video, audio and subtitle tracks!", find_tracks)
+        type_string = (str(type.name) if type != TrackType.SUB else "Text").casefold()
+        tracks = [track for track in tracks if track.track_type.casefold() == type_string]
+
+    if custom_condition:
+        tracks = [track for track in tracks if custom_condition(track)]
+
+    return tracks
+
+
+def get_absolute_track(file: PathLike, track: int, type: TrackType, caller: Any = None) -> Track:
+    """
+    Finds the absolute track for a relative track number of a specific type.
+
+    :param file:    String or pathlib based Path
+    :param track:   Relative track number
+    :param type:    TrackType of the requested relative track
+    """
+    caller = caller if caller else get_absolute_track
+    file = ensure_path_exists(file, caller)
+
+    tracks = get_track_list(file, caller)
+    videos = [track for track in tracks if track.track_type.casefold() == "Video".casefold()]
+    audios = [track for track in tracks if track.track_type.casefold() == "Audio".casefold()]
+    subtitles = [track for track in tracks if track.track_type.casefold() == "Text".casefold()]
     match type:
         case TrackType.VIDEO:
             if not videos:
                 raise error(f"No video tracks have been found in '{file.name}'!", caller)
             try:
                 return videos[track]
             except:
@@ -168,15 +245,15 @@
                 return subtitles[track]
             except:
                 raise error(f"Your requested track doesn't exist.", caller)
         case _:
             raise error("Not implemented for anything other than Video, Audio or Subtitles.", caller)
 
 
-def get_absolute_tracknum(file: PathLike, track: int, type: TrackType, caller: any = None) -> int:
+def get_absolute_tracknum(file: PathLike, track: int, type: TrackType, caller: Any = None) -> int:
     """
     Finds the absolute track number for a relative track number of a specific type.
 
     :param file:    String or pathlib based Path
     :param track:   Relative track number
     :param type:    TrackType of the requested relative track
     """
```

### Comparing `muxtools-0.0.9/muxtools/utils/format.py` & `muxtools-0.1.0/muxtools/utils/format.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from pymediainfo import MediaInfo, Track
-from .types import TrackType, PathLike, AudioFormat
+from .types import TrackType, PathLike
 from .files import ensure_path_exists
-from .log import error, warn
-import re
+from .log import error
 
 
 def get_absolute_track(file: PathLike, track: int, type: TrackType) -> Track:
     """
     Finds the absolute track for a relative track number of a specific type.
 
     :param file:    String or pathlib based Path
```

### Comparing `muxtools-0.0.9/muxtools/utils/glob.py` & `muxtools-0.1.0/muxtools/utils/glob.py`

 * *Files identical despite different names*

### Comparing `muxtools-0.0.9/muxtools/utils/log.py` & `muxtools-0.1.0/muxtools/utils/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,65 @@
 import logging
 from rich.logging import RichHandler
+from typing import Any
 import time
-import inspect
 
-__all__ = ["crit", "debug", "error", "exit", "info", "warn", "logger"]
+__all__ = ["crit", "debug", "error", "exit", "info", "warn", "logger", "LoggingException"]
+
+
+class LoggingException(Exception):
+    """Custom exception returned from log.crit and log.error"""
+
 
 FORMAT = "%(name)s | %(message)s"  #
 logging.basicConfig(format=FORMAT, datefmt="[%X]", handlers=[RichHandler(markup=True, omit_repeated_times=False, show_path=False)])
 
 logger = logging.getLogger("muxtools")
 logger.setLevel(logging.DEBUG)
 
 
-def _format_msg(msg: str, caller: any) -> str:
+def _format_msg(msg: str, caller: Any) -> str:
     if caller and not isinstance(caller, str):
         caller = caller.__class__.__qualname__ if hasattr(caller, "__class__") and caller.__class__.__name__ not in ["function", "method"] else caller
         caller = caller.__name__ if not isinstance(caller, str) else caller
     return msg if caller is None else f"[bold]{caller}:[/] {msg}"
 
 
-def crit(msg: str, caller: any = None) -> Exception:
+def crit(msg: str, caller: Any = None) -> LoggingException:
     message = _format_msg(msg, caller)
     logger.critical(message)
-    return Exception(message)
+    return LoggingException(message)
 
 
-def debug(msg: str, caller: any = None):
+def debug(msg: str, caller: Any = None):
     from .env import is_debug
 
     if not is_debug():
         return
     message = _format_msg(msg, caller)
     logger.debug(message)
 
 
-def info(msg: str, caller: any = None):
+def info(msg: str, caller: Any = None):
     message = _format_msg(msg, caller)
     logger.info(message)
 
 
-def warn(msg: str, caller: any = None, sleep: int = 0):
+def warn(msg: str, caller: Any = None, sleep: int = 0):
     message = _format_msg(msg, caller)
     logger.warning(message)
     if sleep:
         time.sleep(sleep)
 
 
-def error(msg: str, caller: any = None) -> Exception:
+def error(msg: str, caller: Any = None) -> LoggingException:
     message = _format_msg(msg, caller)
     logger.error(message)
-    return Exception(message)
+    return LoggingException(message)
 
 
-def exit(msg: str, caller: any = None):
+def exit(msg: str, caller: Any = None):
     message = _format_msg(msg, caller)
     logger.info(message)
     import sys
 
     sys.exit(0)
```

### Comparing `muxtools-0.0.9/muxtools/utils/parsing.py` & `muxtools-0.1.0/muxtools/utils/parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import re
 import os
 import subprocess
 from pathlib import Path
 from fractions import Fraction
+from typing import Any
 from pyparsebluray import mpls
-from .types import Chapter, PathLike, AudioInfo, AudioStats, AudioFrame, TrackType
+from .types import Chapter, PathLike, AudioInfo, AudioStats, AudioFrame
 from .files import ensure_path_exists
 from .log import error, warn, debug, info
 from .download import get_executable
-from .files import get_absolute_tracknum
 from .convert import (
     timedelta_from_formatted,
     timedelta_to_frame,
     frame_to_timedelta,
     mpls_timestamp_to_timedelta,
     format_timedelta,
 )
@@ -71,15 +71,15 @@
                 m2tsFile = Path(match.group(1))
                 if m2tsFile.exists():
                     return m2tsFile
     print("Warning!\nCould not resolve origin file path from the dgindex input!")
     return dgiFile
 
 
-def parse_audioinfo(file: PathLike, track: int = 0, caller: any = None, is_thd: bool = False) -> AudioInfo:
+def parse_audioinfo(file: PathLike, track: int = 0, caller: Any = None, is_thd: bool = False) -> AudioInfo:
     f_compiled = re.compile(AUDIOFRAME_REGEX, re.IGNORECASE)
     s_compiled = re.compile(AUDIOSTATS_REGEX, re.IGNORECASE)
     file = ensure_path_exists(file, parse_audioinfo)
     ffmpeg = get_executable("ffmpeg")
     out_var = "NUL" if os.name == "nt" else "/dev/null"
     args = [
         ffmpeg,
```

### Comparing `muxtools-0.0.9/muxtools/utils/types.py` & `muxtools-0.1.0/muxtools/utils/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from enum import IntEnum, Enum
 from pathlib import Path
-from typing import TypeVar, Union, Optional
+from typing import Union, Optional
 from datetime import timedelta
 from dataclasses import dataclass
 
 __all__ = [
     "PathLike",
     "Paths",
     "Trim",
@@ -14,15 +14,15 @@
     "AudioStats",
     "AudioInfo",
     "Chapter",
     "DitherType",
     "LossyWavQuality",
 ]
 
-PathLike = TypeVar("PathLike", str, Path, None)
+PathLike = Union[Path, str, None]
 Trim = tuple[int | None, int | None]
 
 Paths = Union[PathLike, list[PathLike]]
 
 # Timedelta (or frame, which will be converted internally), Optional Name
 Chapter = tuple[timedelta | int, Optional[str]]
```

### Comparing `muxtools-0.0.9/muxtools.egg-info/PKG-INFO` & `muxtools-0.1.0/muxtools.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muxtools
-Version: 0.0.9
+Version: 0.1.0
 Summary: A library for various muxing and automation tools for anything and everything fansubbing related
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Vodes/muxtools
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -30,15 +30,15 @@
 
 # muxtools
 
 A library for various muxing and automation tools for anything and everything fansubbing related
 
 ## How do I use this?
 
-You might wanna check out the [wiki](https://github.com/Irrational-Encoding-Wizardry/vs-muxtools/wiki) in the [vs-muxtools](https://github.com/Irrational-Encoding-Wizardry/vs-muxtools) repo.
+You might wanna check out the [guide/wiki](https://muxtools.vodes.pw/).
 
 ## Installation
 
 Git is always the most updated one obviously but I can't guarantee that everything is in a working state.
 
 You can also grab the latest stable ish versions from pip.
```

### Comparing `muxtools-0.0.9/muxtools.egg-info/SOURCES.txt` & `muxtools-0.1.0/muxtools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 muxtools/__init__.py
 muxtools/__main__.py
 muxtools/cli.py
 muxtools/functions.py
 muxtools/main.py
+muxtools/py.typed
 muxtools.egg-info/PKG-INFO
 muxtools.egg-info/SOURCES.txt
 muxtools.egg-info/dependency_links.txt
 muxtools.egg-info/entry_points.txt
 muxtools.egg-info/requires.txt
 muxtools.egg-info/top_level.txt
 muxtools/audio/__init__.py
@@ -23,21 +24,23 @@
 muxtools/misc/chapters.py
 muxtools/muxing/__init__.py
 muxtools/muxing/mux.py
 muxtools/muxing/muxfiles.py
 muxtools/muxing/tmdb.py
 muxtools/muxing/tracks.py
 muxtools/subtitle/__init__.py
+muxtools/subtitle/basesub.py
 muxtools/subtitle/font.py
 muxtools/subtitle/styles.py
 muxtools/subtitle/sub.py
 muxtools/subtitle/subutils.py
 muxtools/utils/__init__.py
 muxtools/utils/convert.py
 muxtools/utils/download.py
 muxtools/utils/env.py
 muxtools/utils/files.py
 muxtools/utils/format.py
 muxtools/utils/glob.py
 muxtools/utils/log.py
 muxtools/utils/parsing.py
+muxtools/utils/subprogress.py
 muxtools/utils/types.py
```

### Comparing `muxtools-0.0.9/pyproject.toml` & `muxtools-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [project]
 name = "muxtools"
-version = "0.0.9"
+version = "0.1.0"
 description = "A library for various muxing and automation tools for anything and everything fansubbing related"
 authors = [{ name = "Vodes", email = "vodes.imp@gmail.com" }]
 dependencies = [
     "requests>=2.31.0",
     "fontcollector>=2.1.4",
     "ass>=0.5.3",
     "wget>=3.2",
```

