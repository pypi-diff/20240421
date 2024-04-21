# Comparing `tmp/vsmuxtools-0.0.9.tar.gz` & `tmp/vsmuxtools-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsmuxtools-0.0.9.tar", last modified: Mon Oct 30 21:14:00 2023, max compression
+gzip compressed data, was "vsmuxtools-0.1.0.tar", last modified: Sun Apr 21 19:30:49 2024, max compression
```

## Comparing `vsmuxtools-0.0.9.tar` & `vsmuxtools-0.1.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 21:14:00.147928 vsmuxtools-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2023-10-30 21:13:40.000000 vsmuxtools-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-10-30 21:14:00.147928 vsmuxtools-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      486 2023-10-30 21:13:40.000000 vsmuxtools-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      997 2023-10-30 21:13:40.000000 vsmuxtools-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-30 21:14:00.147928 vsmuxtools-0.0.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 21:14:00.143928 vsmuxtools-0.0.9/vsmuxtools/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2023-10-30 21:13:40.000000 vsmuxtools-0.0.9/vsmuxtools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 21:14:00.147928 vsmuxtools-0.0.9/vsmuxtools/extension/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-10-30 21:13:40.000000 vsmuxtools-0.0.9/vsmuxtools/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2023-10-30 21:13:40.000000 vsmuxtools-0.0.9/vsmuxtools/extension/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2023-10-30 21:13:40.000000 vsmuxtools-0.0.9/vsmuxtools/extension/chapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2023-10-30 21:13:40.000000 vsmuxtools-0.0.9/vsmuxtools/extension/sub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 21:14:00.147928 vsmuxtools-0.0.9/vsmuxtools/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2023-10-30 21:13:40.000000 vsmuxtools-0.0.9/vsmuxtools/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2023-10-30 21:13:40.000000 vsmuxtools-0.0.9/vsmuxtools/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (127)     7971 2023-10-30 21:13:40.000000 vsmuxtools-0.0.9/vsmuxtools/utils/src.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-10-30 21:13:40.000000 vsmuxtools-0.0.9/vsmuxtools/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 21:14:00.147928 vsmuxtools-0.0.9/vsmuxtools/video/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-10-30 21:13:40.000000 vsmuxtools-0.0.9/vsmuxtools/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14791 2023-10-30 21:13:40.000000 vsmuxtools-0.0.9/vsmuxtools/video/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2023-10-30 21:13:40.000000 vsmuxtools-0.0.9/vsmuxtools/video/resumable.py
--rw-r--r--   0 runner    (1001) docker     (127)    10086 2023-10-30 21:13:40.000000 vsmuxtools-0.0.9/vsmuxtools/video/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2023-10-30 21:13:40.000000 vsmuxtools-0.0.9/vsmuxtools/video/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 21:14:00.143928 vsmuxtools-0.0.9/vsmuxtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-10-30 21:14:00.000000 vsmuxtools-0.0.9/vsmuxtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      598 2023-10-30 21:14:00.000000 vsmuxtools-0.0.9/vsmuxtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 21:14:00.000000 vsmuxtools-0.0.9/vsmuxtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-30 21:14:00.000000 vsmuxtools-0.0.9/vsmuxtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-30 21:14:00.000000 vsmuxtools-0.0.9/vsmuxtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:30:49.458114 vsmuxtools-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-21 19:30:41.000000 vsmuxtools-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-21 19:30:49.458114 vsmuxtools-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-21 19:30:41.000000 vsmuxtools-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-21 19:30:41.000000 vsmuxtools-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 19:30:49.458114 vsmuxtools-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:30:49.454114 vsmuxtools-0.1.0/vsmuxtools/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-21 19:30:41.000000 vsmuxtools-0.1.0/vsmuxtools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:30:49.454114 vsmuxtools-0.1.0/vsmuxtools/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-21 19:30:41.000000 vsmuxtools-0.1.0/vsmuxtools/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-21 19:30:41.000000 vsmuxtools-0.1.0/vsmuxtools/extension/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-21 19:30:41.000000 vsmuxtools-0.1.0/vsmuxtools/extension/chapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-21 19:30:41.000000 vsmuxtools-0.1.0/vsmuxtools/extension/sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 19:30:41.000000 vsmuxtools-0.1.0/vsmuxtools/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:30:49.454114 vsmuxtools-0.1.0/vsmuxtools/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-21 19:30:41.000000 vsmuxtools-0.1.0/vsmuxtools/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-04-21 19:30:41.000000 vsmuxtools-0.1.0/vsmuxtools/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-21 19:30:41.000000 vsmuxtools-0.1.0/vsmuxtools/utils/src.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-21 19:30:41.000000 vsmuxtools-0.1.0/vsmuxtools/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:30:49.458114 vsmuxtools-0.1.0/vsmuxtools/video/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-21 19:30:41.000000 vsmuxtools-0.1.0/vsmuxtools/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14791 2024-04-21 19:30:41.000000 vsmuxtools-0.1.0/vsmuxtools/video/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-04-21 19:30:41.000000 vsmuxtools-0.1.0/vsmuxtools/video/resumable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10003 2024-04-21 19:30:41.000000 vsmuxtools-0.1.0/vsmuxtools/video/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-04-21 19:30:41.000000 vsmuxtools-0.1.0/vsmuxtools/video/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 19:30:49.458114 vsmuxtools-0.1.0/vsmuxtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-21 19:30:49.000000 vsmuxtools-0.1.0/vsmuxtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-21 19:30:49.000000 vsmuxtools-0.1.0/vsmuxtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 19:30:49.000000 vsmuxtools-0.1.0/vsmuxtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-21 19:30:49.000000 vsmuxtools-0.1.0/vsmuxtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-21 19:30:49.000000 vsmuxtools-0.1.0/vsmuxtools.egg-info/top_level.txt
```

### Comparing `vsmuxtools-0.0.9/LICENSE` & `vsmuxtools-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.9/PKG-INFO` & `vsmuxtools-0.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmuxtools
-Version: 0.0.9
+Version: 0.1.0
 Summary: The extension to muxtools with vapoursynth and encoding stuff
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Vodes/vs-muxtools
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -17,23 +17,23 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: vapoursynth>=60
 Requires-Dist: vstools>=1.6.2
 Requires-Dist: numpy>=1.24.3
-Requires-Dist: muxtools>=0.0.9
+Requires-Dist: muxtools>=0.1.0
 
 # vs-muxtools
 
 The extension to muxtools with vapoursynth and encoding stuff
 
 ## How do I use this?
 
-You might wanna check out the [wiki](https://github.com/Irrational-Encoding-Wizardry/vs-muxtools/wiki).
+You might wanna check out the [guide/wiki](https://muxtools.vodes.pw/).
 
 ## Installation
 
 Git is always the most updated one obviously but I can't guarantee that everything is in a working state.
 
 You can also grab the latest stable ish versions from pip.
```

### Comparing `vsmuxtools-0.0.9/pyproject.toml` & `vsmuxtools-0.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 [project]
 name = "vsmuxtools"
-version = "0.0.9"
+version = "0.1.0"
 description = "The extension to muxtools with vapoursynth and encoding stuff"
 authors = [{ name = "Vodes", email = "vodes.imp@gmail.com" }]
 dependencies = [
     "vapoursynth>=60",
     "vstools>=1.6.2",
     "numpy>=1.24.3",
-    "muxtools>=0.0.9",
+    "muxtools>=0.1.0",
 ]
 classifiers = [
     "Natural Language :: English",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
```

### Comparing `vsmuxtools-0.0.9/vsmuxtools/extension/audio.py` & `vsmuxtools-0.1.0/vsmuxtools/extension/audio.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.9/vsmuxtools/extension/chapters.py` & `vsmuxtools-0.1.0/vsmuxtools/extension/chapters.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.9/vsmuxtools/extension/sub.py` & `vsmuxtools-0.1.0/vsmuxtools/extension/sub.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.9/vsmuxtools/utils/audio.py` & `vsmuxtools-0.1.0/vsmuxtools/utils/audio.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.9/vsmuxtools/utils/src.py` & `vsmuxtools-0.1.0/vsmuxtools/utils/src.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,82 @@
 import shutil as sh
-from os import PathLike
 from pathlib import Path
 from typing import Callable
 from fractions import Fraction
-from vstools import vs, core, initialize_clip, copy_signature
+from vstools import vs, core, initialize_clip, copy_signature, KwargsT
 from muxtools import (
     Trim,
     PathLike,
     parse_m2ts_path,
     ensure_path_exists,
     warn,
     info,
     get_workdir,
     get_temp_workdir,
     clean_temp_files,
     get_absolute_track,
     TrackType,
     GlobSearch,
+    error,
 )
 
 
 __all__ = ["src_file", "SRC_FILE", "FileInfo", "src", "frames_to_samples", "f2s"]
 
 
 class src_file:
-    file: PathLike
+    file: Path
     force_lsmas: bool = False
+    force_bs: bool = False
     trim: Trim = None
     idx: Callable[[str], vs.VideoNode] | None = None
     idx_args = {}
 
     def __init__(
-        self, file: PathLike | GlobSearch, force_lsmas: bool = False, trim: Trim = None, idx: Callable[[str], vs.VideoNode] | None = None, **kwargs
+        self,
+        file: PathLike | GlobSearch,
+        force_lsmas: bool = False,
+        trim: Trim = None,
+        idx: Callable[[str], vs.VideoNode] | None = None,
+        force_bs: bool = False,
+        **kwargs,
     ):
         """
         Custom `FileInfo` kind of thing for convenience
 
         :param file:            Either a string based filepath or a Path object
-        :param force_lsmas:     Forces the use of lsmas inside of `vodesfunc.src`
+        :param force_lsmas:     Forces the use of lsmas inside of the default indexer function.
         :param trim:            Can be a single trim or a sequence of trims.
         :param idx:             Indexer for the input file. Pass a function that takes a string in and returns a vs.VideoNode.
-                                Defaults to `vodesfunc.src`
+        :param force_bs:        Forces the use of bestsource inside of the default indexer function.
         """
         self.file = ensure_path_exists(file, self)
         self.force_lsmas = force_lsmas
+        self.force_bs = force_bs
         self.trim = trim
         self.idx = idx
         self.idx_args = kwargs
 
     def __index_clip(self):
-        indexed = self.idx(str(self.file.resolve())) if self.idx else src(str(self.file.resolve()), self.force_lsmas, **self.idx_args)
+        indexed = self.idx(str(self.file.resolve())) if self.idx else src(str(self.file.resolve()), self.force_lsmas, self.force_bs, **self.idx_args)
         cut = indexed
         if self.trim:
             self.trim = list(self.trim)
             if self.trim[0] is None:
                 self.trim[0] = 0
             if self.trim[1] is None or self.trim[1] == 0:
-                cut = indexed[self.trim[0] :]
+                if self.trim[0] < 0:
+                    cut = (indexed[0] * abs(self.trim[0])) + indexed
+                else:
+                    cut = indexed[self.trim[0] :]
             else:
-                cut = indexed[self.trim[0] : self.trim[1]]
+                if self.trim[0] < 0:
+                    cut = (indexed[0] * abs(self.trim[0])) + indexed[: self.trim[1]]
+                else:
+                    cut = indexed[self.trim[0] : self.trim[1]]
             self.trim = tuple(self.trim)
 
         if self.file.suffix.lower() == ".dgi":
             if self.file.with_suffix(".m2ts").exists():
                 self.file = self.file.with_suffix(".m2ts")
             else:
                 self.file = parse_m2ts_path(self.file)
@@ -100,20 +114,17 @@
         """
         return initialize_clip(self.src_cut, *args, **kwargs)
 
     def get_audio(self, track: int = 0, **kwargs) -> vs.AudioNode:
         """
         Indexes the specified audio track from the input file.
         """
-        args = dict(exact=True)
-        args.update(**kwargs)
-
         absolute = get_absolute_track(self.file, track, TrackType.AUDIO)
 
-        return core.bs.AudioSource(str(self.file.resolve()), absolute.track_id, **args)
+        return core.bs.AudioSource(str(self.file.resolve()), absolute.track_id, **kwargs)
 
     def get_audio_trimmed(self, track: int = 0, **kwargs) -> vs.AudioNode:
         """
         Gets the indexed audio track with the trim specified in the src_file.
         """
         node = self.get_audio(track, **kwargs)
         if self.trim:
@@ -124,63 +135,55 @@
         return node
 
 
 SRC_FILE = src_file
 FileInfo = src_file
 
 
-def src(filePath: PathLike, force_lsmas: bool = False, delete_dgi_log: bool = True, **kwargs) -> vs.VideoNode:
+def src(filePath: PathLike, force_lsmas: bool = False, force_bs: bool = False, **kwargs: KwargsT) -> vs.VideoNode:
     """
-    Uses dgindex as Source and requires dgindexnv in path
-    to generate files if they don't exist.
+    Uses lsmas for previewing and bestsource otherwise.
+    Still supports dgi files directly if dgdecodenv is installed to not break existing scripts.
 
     :param filepath:        Path to video or dgi file
-    :param force_lsmas:     Skip dgsource entirely and use lsmas
-    :param delete_dgi_log:  Delete the .log files dgindexnv creates
+    :param force_lsmas:     Force the use of lsmas.LWLibavSource
+    :param force_bs:        Force the use of bs.VideoSource. This takes priority over the force_lsmas param.
+    :param kwargs:          Other arguments you may or may not wanna pass to the indexer.
     :return:                Video Node
     """
     filePath = ensure_path_exists(filePath, src)
-    filePath = str(filePath)
-    if filePath.lower().endswith(".dgi"):
-        return core.lazy.dgdecodenv.DGSource(filePath, **kwargs)
-
-    forceFallBack = sh.which("dgindexnv") is None or not hasattr(core, "dgdecodenv")
-
-    if not force_lsmas:
-        import pymediainfo as pym
-
-        parsed = pym.MediaInfo.parse(filePath, parse_speed=0.25)
-        trackmeta = parsed.video_tracks[0].to_data()
-        format = trackmeta.get("format")
-        bitdepth = trackmeta.get("bit_depth")
-        if format is not None and bitdepth is not None:
-            if str(format).strip().lower() == "avc" and int(bitdepth) > 8:
-                forceFallBack = True
-                warn(f"Falling back to lsmas for Hi10 ({Path(filePath).name})", src)
-            elif str(format).strip().lower() == "ffv1":
-                forceFallBack = True
-                warn(f"Falling back to lsmas for FFV1 ({Path(filePath).name})", src)
-
-    if force_lsmas or forceFallBack:
-        return core.lsmas.LWLibavSource(filePath, **kwargs)
-
-    path = Path(filePath)
-    dgiFile = path.with_suffix(".dgi")
-
-    if dgiFile.exists():
-        return core.dgdecodenv.DGSource(dgiFile.resolve(True), **kwargs)
+    dgiFile = filePath.with_suffix(".dgi")
+    if filePath.suffix.lower() == ".dgi" or dgiFile.exists():
+        if not hasattr(core, "dgdecodenv"):
+            raise error("Trying to use a dgi file without dgdecodenv installed.", src)
+        return core.lazy.dgdecodenv.DGSource(str(filePath.resolve()) if not dgiFile.exists() else str(dgiFile.resolve()), **kwargs)
+
+    has_bestsource, has_lsmas = hasattr(core, "bs"), hasattr(core, "lsmas")
+    if not has_bestsource and not has_lsmas:
+        raise error("Neither bestsource nor lsmas are installed.", src)
+    if force_lsmas and not has_lsmas and not force_bs:
+        raise error("You cannot force lsmas indexing without lsmas installed!", src)
+    if force_bs and not has_bestsource:
+        raise error("You cannot force bestsource indexing without bestsource installed!", src)
+
+    is_previewing = False
+    try:
+        from vspreview import is_preview
+
+        is_previewing = is_preview()
+    except:
+        pass
+
+    if (is_previewing or force_lsmas) and not force_bs and has_lsmas:
+        info(f"Indexing '{filePath.name}' using lsmas LWLibavSource", src)
+        return core.lazy.lsmas.LWLibavSource(str(filePath.resolve()), **kwargs)
     else:
-        info("Generating dgi file...", src)
-        import os
-        import subprocess as sub
-
-        sub.Popen(f'dgindexnv -i "{path.name}" -h -o "{dgiFile.name}" -e', shell=True, stdout=sub.DEVNULL, cwd=path.parent.resolve(True)).wait()
-        if path.with_suffix(".log").exists() and delete_dgi_log:
-            os.remove(path.with_suffix(".log").resolve(True))
-        return core.dgdecodenv.DGSource(dgiFile.resolve(True), **kwargs)
+        info(f"Indexing '{filePath.name}' using bestsource.", src)
+        show_progress = kwargs.pop("showprogress", True)
+        return core.lazy.bs.VideoSource(str(filePath.resolve()), showprogress=show_progress, **kwargs)
 
 
 def frames_to_samples(frame: int, sample_rate: vs.AudioNode | int = 48000, fps: vs.VideoNode | Fraction = Fraction(24000, 1001)) -> int:
     """
     Converts a frame number to a sample number
 
     :param frame:           The frame number
```

### Comparing `vsmuxtools-0.0.9/vsmuxtools/video/encoders.py` & `vsmuxtools-0.1.0/vsmuxtools/video/encoders.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.9/vsmuxtools/video/resumable.py` & `vsmuxtools-0.1.0/vsmuxtools/video/resumable.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.9/vsmuxtools/video/settings.py` & `vsmuxtools-0.1.0/vsmuxtools/video/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-from genericpath import isfile
 import re
 import os
-from tracemalloc import start
 from muxtools import error, PathLike, ensure_path, warn
-from vstools import vs, Matrix, Primaries, Transfer, ColorRange, ChromaLocation, get_prop, Colorspace
+from vstools import vs, Matrix, Primaries, Transfer, ColorRange, ChromaLocation
 from ..utils.types import Zone
 
 __all__ = ["settings_builder_x265", "settings_builder_x264", "sb", "sb265", "sb264"]
 
 
 def is_full_zone(zone: Zone) -> bool:
     if isinstance(zone[2], str):
```

### Comparing `vsmuxtools-0.0.9/vsmuxtools/video/testing.py` & `vsmuxtools-0.1.0/vsmuxtools/video/testing.py`

 * *Files identical despite different names*

### Comparing `vsmuxtools-0.0.9/vsmuxtools.egg-info/PKG-INFO` & `vsmuxtools-0.1.0/vsmuxtools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsmuxtools
-Version: 0.0.9
+Version: 0.1.0
 Summary: The extension to muxtools with vapoursynth and encoding stuff
 Author-email: Vodes <vodes.imp@gmail.com>
 License: MPL 2.0
 Project-URL: Source Code, https://github.com/Vodes/vs-muxtools
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
@@ -17,23 +17,23 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: vapoursynth>=60
 Requires-Dist: vstools>=1.6.2
 Requires-Dist: numpy>=1.24.3
-Requires-Dist: muxtools>=0.0.9
+Requires-Dist: muxtools>=0.1.0
 
 # vs-muxtools
 
 The extension to muxtools with vapoursynth and encoding stuff
 
 ## How do I use this?
 
-You might wanna check out the [wiki](https://github.com/Irrational-Encoding-Wizardry/vs-muxtools/wiki).
+You might wanna check out the [guide/wiki](https://muxtools.vodes.pw/).
 
 ## Installation
 
 Git is always the most updated one obviously but I can't guarantee that everything is in a working state.
 
 You can also grab the latest stable ish versions from pip.
```

### Comparing `vsmuxtools-0.0.9/vsmuxtools.egg-info/SOURCES.txt` & `vsmuxtools-0.1.0/vsmuxtools.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 vsmuxtools/__init__.py
+vsmuxtools/py.typed
 vsmuxtools.egg-info/PKG-INFO
 vsmuxtools.egg-info/SOURCES.txt
 vsmuxtools.egg-info/dependency_links.txt
 vsmuxtools.egg-info/requires.txt
 vsmuxtools.egg-info/top_level.txt
 vsmuxtools/extension/__init__.py
 vsmuxtools/extension/audio.py
```

