# Comparing `tmp/synth_mapping_helper-1.4.0.tar.gz` & `tmp/synth_mapping_helper-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synth_mapping_helper-1.4.0.tar", last modified: Sat Apr 13 14:19:41 2024, max compression
+gzip compressed data, was "synth_mapping_helper-1.4.1.tar", last modified: Sun Apr 21 13:45:18 2024, max compression
```

## Comparing `synth_mapping_helper-1.4.0.tar` & `synth_mapping_helper-1.4.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:19:41.233991 synth_mapping_helper-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-04-13 14:19:41.233991 synth_mapping_helper-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-13 14:19:41.233991 synth_mapping_helper-1.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:19:41.225990 synth_mapping_helper-1.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:19:41.229990 synth_mapping_helper-1.4.0/src/synth_mapping_helper/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28847 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    28170 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/companion.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/finalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4788 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:19:41.229990 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/autobackup.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    35892 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    14395 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/local_dir_picker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/map_render.py
--rw-r--r--   0 runner    (1001) docker     (127)    26703 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/stacking.py
--rw-r--r--   0 runner    (1001) docker     (127)    18509 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/text_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    34011 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/wall_art.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/movement.py
--rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/pattern_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/rails.py
--rw-r--r--   0 runner    (1001) docker     (127)    27884 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/synth_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:19:41.233991 synth_mapping_helper-1.4.0/src/synth_mapping_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-04-13 14:19:41.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-13 14:19:41.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:19:41.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-13 14:19:41.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-13 14:19:41.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-13 14:19:41.000000 synth_mapping_helper-1.4.0/src/synth_mapping_helper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:19:41.233991 synth_mapping_helper-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-13 14:19:29.000000 synth_mapping_helper-1.4.0/tests/test_synth_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:18.812765 synth_mapping_helper-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-04-21 13:45:18.812765 synth_mapping_helper-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-21 13:45:18.812765 synth_mapping_helper-1.4.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:18.804765 synth_mapping_helper-1.4.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:18.808765 synth_mapping_helper-1.4.1/src/synth_mapping_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28847 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28170 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/companion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:18.812765 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/autobackup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8812 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35909 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/local_dir_picker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8895 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/map_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26721 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/stacking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18510 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/text_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41790 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/wall_art.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/movement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8139 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/pattern_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15230 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/rails.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27884 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/synth_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5006 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:18.812765 synth_mapping_helper-1.4.1/src/synth_mapping_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5557 2024-04-21 13:45:18.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-21 13:45:18.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 13:45:18.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-21 13:45:18.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-21 13:45:18.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-21 13:45:18.000000 synth_mapping_helper-1.4.1/src/synth_mapping_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 13:45:18.812765 synth_mapping_helper-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-21 13:45:07.000000 synth_mapping_helper-1.4.1/tests/test_synth_format.py
```

### Comparing `synth_mapping_helper-1.4.0/LICENSE` & `synth_mapping_helper-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.0/PKG-INFO` & `synth_mapping_helper-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth_mapping_helper
-Version: 1.4.0
+Version: 1.4.1
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Author: adosikas
 License: MIT License
         
         Copyright (c) 2024 adosikas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `synth_mapping_helper-1.4.0/README.md` & `synth_mapping_helper-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.0/pyproject.toml` & `synth_mapping_helper-1.4.1/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -46,8 +46,8 @@
 Repository = "https://github.com/adosikas/synth_mapping_helper"
 "Bug Tracker" = "https://github.com/adosikas/synth_mapping_helper/issues"
 Changelog = "https://github.com/adosikas/synth_mapping_helper/releases"
 
 [project.scripts]
 smh-cli = "synth_mapping_helper.cli:entrypoint"
 smh-gui = "synth_mapping_helper.gui:entrypoint"
-smh-companion = "synth_mapping_helper.companion:entrypoint"
+smh-companion = "synth_mapping_helper.companion:entrypoint"
```

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/cli.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/cli.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/companion.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/companion.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/finalize.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/finalize.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -290,8 +290,8 @@
             beatmap["Bookmarks"]["BookmarksList"].append(FINALIZED_BOOKMARK)
         # write modified beatmap json
         outzip.writestr(inzip.getinfo(BEATMAP_JSON_FILE), json.dumps(beatmap))
     # write output zip
     options.output.write_bytes(out_buffer.getbuffer())
 
 if __name__ == "__main__":
-    main(get_parser().parse_args())
+    main(get_parser().parse_args())
```

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from argparse import ArgumentParser, ArgumentError
 from io import BytesIO
 import logging
+import sys
 from typing import Optional
 
 from nicegui import app, ui, events
+import requests
 
 from . import synth_format, cli, __version__
 from .gui_tabs.utils import *
 from .gui_tabs.commands import command_tab
 from .gui_tabs.file_utils import file_utils_tab
 from .gui_tabs.dashboard import dashboard_tab
 from .gui_tabs.autobackup import autobackup_tab
@@ -23,31 +25,54 @@
     ["Wall Art", "wallpaper", wall_art_tab, None],
     ["Commands", "play_arrow", command_tab, None],
     ["File utils", "construction", file_utils_tab, None],
     ["Autobackup", "manage_history", autobackup_tab, None],
     ["Version History", "update", version_tab, None],
 ]
 
+version = f"SMH-GUI v{__version__}"
+
+@app.get("/version")
+def get_version():
+    return version
+
 async def stop():
     logger.info("Stopping...")
     await ui.run_javascript("setTimeout(window.close, 100);")
     app.shutdown()
+
 def entrypoint():
-    parser = ArgumentParser()
+    parser = ArgumentParser(description=version)
     parser.add_argument("-l", "--log-level", type=str, default="INFO", help="Set log level")
     parser.add_argument("--host", type=str, default="127.0.0.1",
-        help="""Host for the webserver. Defaults to localhost.
+        help="""Host for the webserver. Defaults to 127.0.0.1 (localhost).
             Can be set to a local IP if you want to access the GUI from another device, eg. tablet.\n
-            Note that there is NO PASSWORD CHECK, so only use if you trust ALL devices on that network.""")
+            Note that there is NO PASSWORD CHECK, so only use if you trust ALL devices on that network to have access to your clipboard and files.""")
     parser.add_argument("--port", type=int, default=8080, help="Port for the webserver")
     parser.add_argument("--background", action="store_true", help="Open in background (does not open browser)")
     parser.add_argument("--dev-mode", action="store_true", help="Open in dev mode (reloads when editing python files)")
 
     args = parser.parse_args()
 
+    if not args.dev_mode:
+        try:
+            resp = requests.get(f"http://{args.host}:{args.port}/version")
+            resp.raise_for_status()
+            print(f"ERROR: {resp.json()} is already running on http://{args.host}:{args.port}")
+            sys.exit(-1)
+        except requests.ConnectionError:
+            # we want an connection error to occur, else there is another instance (or something else) running
+            pass
+        except Exception as e:
+            # unexpected error getting or parsing version
+            print(f"ERROR: Could not check if there is another instance already running on http://{args.host}:{args.port}")
+            print(f"           {e!r}")
+            print("       If this persists after a restart, something else may be using that port and you could add e.g. --port=8181 to change the SMH-GUI port")
+            sys.exit(-1)
+
     @ui.page("/")
     def index():
         ui.add_head_html("""<style>
             .q-field__suffix {
                 color: grey !important;
             }
             .q-field__bottom {
@@ -89,19 +114,19 @@
             logging.FileHandler("smh_gui.log"),
             logging.StreamHandler()
         ]
     )
     if args.dev_mode:
         logging.getLogger("watchfiles.main").level = logging.WARN  # hide change detection
 
-    logger.info(f"Starting v{__version__}{' in background' if args.background else ''}...")
+    logger.info(f"Starting {version}{' in background' if args.background else ''}...")
     ui.run(
         host=args.host,
         port=args.port,
-        title=f"SMH-GUI v{__version__} [beta]",
+        title=f"{version} [beta]",
         favicon="🚧" if args.dev_mode else "🤦",
         reload=args.dev_mode,
         storage_secret="smh_gui",
         show=not args.background,
     )
 
 if __name__ in {"__main__", "__mp_main__"}:
```

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/autobackup.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/autobackup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -77,8 +77,8 @@
     @ui.refreshable
     def log():
         for _, b in sorted(last_backup.values(), key=lambda tb: tb[0], reverse=True):
             ui.label(str(b))
 
     ui.label("Last backup:").classes("my-4")
     with ui.card().classes("w-full"):
-            log()
+            log()
```

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/commands.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/commands.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -180,8 +180,8 @@
                 wiki_reference("Miscellaneous-Options#use-original-json")
             with ui.checkbox("Mirror for left hand") as mirror_left_cb:
                 wiki_reference("Miscellaneous-Options#mirror-operations-for-left-hand")
         ui.separator()
     
         ui.label("Quick run:")
         with ui.row():
-            quick_run_buttons()
+            quick_run_buttons()
```

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/dashboard.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 from nicegui import app, events, ui
 import pyperclip
 
 from .utils import *
 from .. import movement, pattern_generation, rails, synth_format
-from ..utils import parse_number
+from ..utils import parse_number, pretty_list
 
 def _movement_helper(data: synth_format.DataContainer, mirror_left: bool, base_func, relative_func, pivot_func, relative: bool, pivot: Optional[list[int]], *args, **kwargs) -> None:
     """pick the right function depending on relative or pivot being set"""
     if relative:
         data.apply_for_all(relative_func, *args, mirror_left=mirror_left, **kwargs)
     elif pivot is not None:
         data.apply_for_all(pivot_func, *args, mirror_left=mirror_left, pivot_3d=pivot, **kwargs)
@@ -145,15 +145,15 @@
                 return
             except Exception as exc:
                 error(f"Error executing '{self._tooltip}'", exc, settings=settings, data=clipboard)
                 return
             counts = d.get_counts()
             info(
                 f"Completed: '{self._tooltip}'",
-                caption=", ".join(f"{counts[t]['total']} {t if counts[t]['total'] != 1 else t.rstrip('s')}" for t in ("notes", "rails", "rail_nodes", "walls")),
+                caption=pretty_list([f"{counts[t]['total']} {t if counts[t]['total'] != 1 else t.rstrip('s')}" for t in ("notes", "rails", "rail_nodes", "walls")]),
             )
             synth_format.export_clipboard(d, realign_start=sw_realign.value)
 
     with ui.row():
         with ui.card():
             with ui.label("Offset"):
                 wiki_reference("Movement-Options#offset")
```

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/file_utils.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/file_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Optional
 import sys
 
 import plotly.graph_objects as go
 from nicegui import app, events, ui
 
 from .utils import *
+from ..utils import pretty_list
 from .. import synth_format, movement
 from .. import __version__
 
 density_container = tuple[list[float], list[int], float]
 
 def density(times: list[float], window: float) -> density_container:
     if not times:
@@ -151,15 +152,15 @@
 
             ui.label("Object counts (click to see more)")
             def _stats_notify(ev: events.GenericEventArguments) -> None:
                 if "." in ev.args["colId"]:
                     col = ev.args["colId"].rsplit(".",1)[0]
                     col_data = ev.args["data"][col]
                     ui.notify(
-                        f"{col_data['total']} {col}: " + ", ".join(f"{k}: {v}" for k,v in col_data.items() if k != "total"),
+                        f"{col_data['total']} {col}: " + pretty_list([f"{v} {k}" for k,v in col_data.items() if k != "total"]),
                         position="center",
                         type="info"
                     )
             ui.aggrid({
                 "domLayout": "autoHeight",
                 "columnDefs": [
                     {"headerName": "Difficulty", "field": "diff"},
@@ -294,8 +295,8 @@
         with ui.card():
             ui.label("Merge files into base")
             merge_bookmarks = ui.switch("Merge Bookmarks", value=True).classes("w-full").bind_value(app.storage.user, "merge_bookmarks").bind_enabled_from(fi, "is_valid").tooltip("Disable this if you merge maps that contain the same bookmarks")
             ui.upload(label="One or more files", multiple=True, auto_upload=True, on_upload=fi.upload_merge).props('color="positive"').classes("h-14 w-full").bind_enabled_from(fi, "is_valid")
             ui.label("Note: BPM & Offset will be matched automatically.")
             ui.tooltip("Select a base file first").bind_visibility_from(fi, "is_valid", backward=lambda v: not v).classes("bg-red")
     with ui.card().classes("w-full"):
-        fi.info_card()
+        fi.info_card()
```

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/local_dir_picker.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/local_dir_picker.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -67,8 +67,8 @@
             for p in paths
         ]
         if self.path != self.path.parent:
             self.grid.options['rowData'].insert(0, {
                 'name': '↖️ <strong>..</strong>',
                 'path': str(self.path.parent),
             })
-        self.grid.update()
+        self.grid.update()
```

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/map_render.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/map_render.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,9 +171,7 @@
                                 self.to_scene(diff[i-1]),
                                 self.to_scene((diff[i-1]+diff[i])/2),
                                 self.to_scene(diff[i]),
                                 radius=settings.rail.size,
                             ).material(
                                 color, settings.rail.opacity
                             )
-
-
```

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/stacking.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/stacking.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from nicegui import app, ui, elements
 import numpy as np
 import pyperclip
 
 from .utils import *
 from .map_render import SettingsPanel, MapScene
-from ..utils import parse_number, parse_range, parse_xy_range, pretty_fraction
+from ..utils import parse_number, parse_range, parse_xy_range, pretty_fraction, pretty_list
 from .. import synth_format, movement, pattern_generation
 
 def _negate(val: str|None) -> str|None:
     if not val:
         return val
     if val.startswith("-"):
         return val[1:]
@@ -378,15 +378,15 @@
                 _stack(d, c, p, o, s, r, wr, outset, random_ranges_offset, random_step_offset, random_ranges_angle, random_step_angle)
             except Exception as exc:
                 error(f"Error executing stack", exc, settings={"count": c, "pivot": p, "offset": o, "scale": s, "rotation": r, "wall_rotation": wr, "outset": outset}, data=clipboard)
                 return
             counts = d.get_counts()
             info(
                 f"Completed stack",
-                caption=", ".join(f"{counts[t]['total']} {t if counts[t]['total'] != 1 else t.rstrip('s')}" for t in ("notes", "rails", "rail_nodes", "walls")),
+                caption=pretty_list([f"{counts[t]['total']} {t if counts[t]['total'] != 1 else t.rstrip('s')}" for t in ("notes", "rails", "rail_nodes", "walls")]),
             )
             synth_format.export_clipboard(d, realign_start=False)
             if preview_scene is not None:
                 try:
                     preview_settings = sp.parse_settings()
                 except ParseInputError as pie:
                     error(f"Error parsing preview setting: {pie.input_id}", pie, data=pie.value)
@@ -489,8 +489,8 @@
                 t = time_scale.parsed_value
             except ParseInputError as pie:
                 error(f"Error parsing preview setting: {pie.input_id}", pie, data=pie.value)
                 return
             preview_scene = MapScene(width=w, height=h, frame_length=l, time_scale=t)
             _soft_refresh()
         draw_preview_scene()
-        apply_button.on("click", draw_preview_scene.refresh)
+        apply_button.on("click", draw_preview_scene.refresh)
```

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/text_gen.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/text_gen.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -210,8 +210,8 @@
             except ParseInputError as pie:
                 error(f"Error parsing preview setting: {pie.input_id}", pie, data=pie.value)
                 return
             preview_scene = MapScene(width=w, height=h, frame_length=l, time_scale=t, zoomout=40)
             _soft_refresh(False)
         draw_preview_scene()
         apply_button.on("click", draw_preview_scene.refresh)
-        generate_button.on("click", _soft_refresh)
+        generate_button.on("click", _soft_refresh)
```

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/utils.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/utils.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -95,8 +95,8 @@
     if not suffix:
         return filename
     return f"{filename.removesuffix('.synth')}_{suffix}.synth"
 
 class ParseInputError(ValueError):
     def __init__(self, input_id: str, value: Any) -> None:
         self.input_id = input_id
-        self.value = value
+        self.value = value
```

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/version.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 import datetime
 
 from nicegui import app, ui
 import requests
+import logging
 
 from .utils import error
 from .. import __version__
+from ..utils import pretty_time_delta
 
 releases = None
 
 def version_tab():
     @ui.refreshable
     def release_list():
         if releases == "error":
             ui.label("Error requesting version information")
         elif releases:
             now = datetime.datetime.now(datetime.timezone.utc)
             new = True
             for r in releases[:10]:
                 try:
                     time_delta = now - datetime.datetime.fromisoformat(r["created_at"]).replace(tzinfo=datetime.timezone.utc)
-                    time_delta_str = f"{time_delta.days} day{'' if time_delta.days==1 else 's'}" if time_delta.days else f"{time_delta.seconds//3600} day{'' if time_delta.seconds//3600==1 else 's'}"
+                    name = r["name"]
                     v = r["tag_name"][1:]
-                    color = "positive" if new else "dark"
+                    url = r["html_url"]
+                    body = r["body"]
+                except:
+                    ui.label("Error parsing version information")
+                else:
+                    color = "positive" if new else "auto"
                     icon = "stars" if new else "check_circle"
                     if v == __version__:
                         color = "primary"
                         icon = "play_circle"
                         new = False
-                    with ui.expansion(f'{r["name"]} ({time_delta_str} ago)', icon=icon).props(f'group="ver_hist" header-class="bg-{color}"').classes("textcolor-red"):
-                        ui.link(r["html_url"], target=r["html_url"], new_tab=True) 
-                        ui.markdown(r["body"])
-                except:
-                    ui.label("Error parsing version information")
+                    with ui.expansion(f'{name} ({pretty_time_delta(time_delta.total_seconds())} ago)', icon=icon).props(f'group="ver_hist" header-class="bg-{color} w-auto"'):
+                        with ui.row():
+                            ui.label("Github link:")
+                            ui.link(url, target=url, new_tab=True) 
+                        with ui.card().props("bordered"):
+                            ui.markdown()
         elif releases is not None:
             with ui.row():
                 ui.spinner()
                 ui.label("Requesting...")
         else:
             ui.label("To protect your privacy, this does not automatically contact github.com. Press the button or enable auto-check below.")
 
@@ -61,15 +69,15 @@
                 )
             release_list.refresh()
         except Exception as exc:
             releases = "error"
             release_list.refresh()
             error("Requesting version information from github.com failed", exc)
 
-    with ui.card():
+    with ui.card().classes("w-full"):
         release_list()
 
     with ui.row():
         ui.button("Check now", icon="sync", on_click=check, color="positive")
         auto_check = ui.switch("Check on start", value=False).bind_value(app.storage.user, "version_history_autocheck")
 
     if auto_check.value:
```

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/gui_tabs/wall_art.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/gui_tabs/wall_art.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from nicegui.elements.scene_objects import Extrusion, Texture
 import numpy as np
 import pyperclip
 import requests
 
 from .map_render import MapScene, SettingsPanel
 from .utils import ParseInputError, info, error
-from ..utils import parse_number, pretty_time_delta
+from ..utils import parse_number, pretty_time_delta, pretty_fraction, pretty_list
 from .. import synth_format, movement, pattern_generation
 
 class SMHInput(ui.input):
     def __init__(self, label: str, value: str|float, storage_id: str, tooltip: str|None=None, suffix: str|None = None, **kwargs):
         super().__init__(label=label, value=str(value), **kwargs)
         self.bind_value(app.storage.user, f"wall_art_{storage_id}")
         self.classes("w-16 h-10")
@@ -41,14 +41,22 @@
     @property
     def parsed_value(self) -> float:
         try:
             return parse_number(self.value)
         except ValueError as ve:
             raise ParseInputError(self.storage_id, self.value) from ve
 
+class LargeSwitch(ui.switch):
+    def __init__(self, storage_id: str, tooltip: str|None=None, color: str="primary", icon_unchecked: str|None=None, icon_checked: str|None=None):
+        super().__init__()
+        self.bind_value(app.storage.user, f"wall_art_{storage_id}")
+        self.classes("my-auto")
+        self.props(f'dense size="xl" color="{color}" keep-color' + (f' unchecked-icon="{icon_unchecked}"' if icon_unchecked is not None else '') + (f' checked-icon="{icon_checked}"' if icon_checked is not None else ''))
+        self.tooltip(tooltip)
+
 @app.get("/image_proxy")
 def image_proxy(url:str):
     r = requests.get(url)
     return Response(content=r.content)
 
 def wall_art_tab():
     preview_scene: MapScene|None = None
@@ -71,49 +79,50 @@
             if len(self.undo_stack) > self.max_steps:
                 del self.undo_stack[0]
             self.redo_stack.clear()
         
         def undo(self):
             nonlocal walls
             if not self.undo_stack:
-                ui.notify("Nothing to undo", type="info")
+                ui.notify("Nothing to undo", type="info", timeout=1000)
                 return
             label, timestamp, undo_walls, undo_selection = self.undo_stack.pop()
             self.redo_stack.append((label, timestamp, walls.copy(), selection.sources.copy()))
             selection.clear()
             walls.clear()
             walls |= undo_walls
             selection.select(undo_selection, mode="set")
             _soft_refresh()
-            ui.notify(f"Undo: {label} ({pretty_time_delta(time() - timestamp)} ago)", type="info")
+            ui.notify(f"Undo: {label} ({pretty_time_delta(time() - timestamp)} ago)", type="info", timeout=1000)
 
         def redo(self):
             nonlocal walls
             if not self.redo_stack:
-                ui.notify("Nothing to redo", type="info")
+                ui.notify("Nothing to redo", type="info", timeout=1000)
                 return
             label, timestamp, redo_walls, redo_selection = self.redo_stack.pop()
             self.undo_stack.append((label, timestamp, walls.copy(), selection.sources.copy()))
             selection.clear()
             walls.clear()
             walls |= redo_walls
             selection.select(redo_selection, mode="set")
             _soft_refresh()
-            ui.notify(f"Redo: {label} ({pretty_time_delta(time() - timestamp)} ago)", type="info")
+            ui.notify(f"Redo: {label} ({pretty_time_delta(time() - timestamp)} ago)", type="info", timeout=1000)
 
     undo = Undo()
 
     @dataclass
     class Selection:
         sources: set[float] = field(default_factory=set)
         cursors: dict[float, Extrusion] = field(default_factory=dict)
         drag_time: float = None
         offset: "np.array (3)" = field(default_factory=lambda: np.array([0.0, 0.0, 0.0]))
         mirrored: bool = False
         rotation: float = 0.0
+        copy: bool = False
 
         def clear(self):
             self.sources = set()
             if self.drag_time is not None:
                 # everything is parented to this one
                 self.cursors[self.drag_time].delete()
             else:
@@ -156,79 +165,123 @@
                 elif new_t > high:
                     new_sources = self.sources | {t for t in walls if high <= t <= new_t}
                 else:
                     new_sources = self.sources | {t for t in walls if low <= t <= high}
             # else: leave new_sources as is
             self.clear()
             self.sources = new_sources
-            if self.sources:
-                if copy.value:
-                    first = min(self.sources)
-                    self.offset += [0,0,_find_free_slot(first)-first]
+            self._update_cursors()
+
+        def _update_cursors(self):
+            if not self.sources:
+                return
+            first = min(self.sources)
+            copy_offset = [0.0,0.0,_find_free_slot(first+self.offset[2])-first-self.offset[2],0.0,0.0] if self.copy else 0.0
+            if self.drag_time is None:
+                # re-create cursors
+                for c in self.cursors.values():
+                    c.delete()
                 preview_settings = sp.parse_settings()
                 with preview_scene:
+                    pivot_3d = walls[first][0,:3]
+                    scale_3d = np.array([1.0, -1.0 if self.mirrored else 1.0, 1.0])
                     for t in self.sources:
-                        e = preview_scene.wall_extrusion(walls[t] + [*self.offset, 0.0, 0.0], preview_settings.wall.size * time_scale.parsed_value).draggable()
-                        if copy.value:
+                        w = walls[t] + copy_offset
+                        w = movement.rotate_around(w, self.rotation, pivot_3d)
+                        w = movement.scale_from(w, scale_3d, pivot_3d)
+                        w = movement.offset(w, self.offset)
+                        e = preview_scene.wall_extrusion(w, preview_settings.wall.size * time_scale.parsed_value).draggable()
+                        if self.copy:
                             e.material(copy_color.value, copy_opacity.parsed_value)
                         else:
                             e.material(move_color.value, move_opacity.parsed_value)
                         self.cursors[t] = e
-
-        def _update_cursors(self):
-            pivot = walls[self.drag_time if self.drag_time is not None else min(self.sources)]
-            for t, c in ([(self.drag_time, self.cursors[self.drag_time])] if self.drag_time is not None else self.cursors.items()):
-                xyt = pivot[0,:3]+movement.rotate((walls[t]-pivot)[0,:3], self.rotation)*[1, -1 if self.mirrored else 1,1]+self.offset
-                c.move(xyt[0], xyt[2]*time_scale.parsed_value, xyt[1])
+                preview_scene.props('drag_constraints=""')
+            else:
+                w = walls[self.drag_time][0] + copy_offset
+                scene_pos = preview_scene.to_scene(w[:3] + self.offset)
+                # move cursor
+                cur = self.cursors[self.drag_time]
+                cur.move(*scene_pos)
+                rot = w[4]+self.rotation
                 if self.mirrored:
-                    # couldn't figure out how to change the verts, so just mirror by scaling
-                    c.scale(1, -1, 1)
-                    c.rotate(np.deg2rad(90), np.deg2rad(180 + (walls[t][0,4]+self.rotation)), 0)
-
+                    cur.scale(1,-1,1)
+                    cur.rotate(np.deg2rad(90), np.deg2rad(180 + rot), 0)
                 else:
-                    c.scale(1, 1, 1)
-                    c.rotate(np.deg2rad(90), np.deg2rad(180 - (walls[t][0,4]+self.rotation)), 0)
-
-            if selection.drag_time is not None:
+                    cur.scale(1,1,1)
+                    cur.rotate(np.deg2rad(90), np.deg2rad(180 - rot), 0)
+                # update drag constraints
                 if axis_z.value:
-                    x, y = walls[selection.drag_time][0,:2]+selection.offset[:2]
-                    preview_scene.props(f'drag_constraints="x={x},z={y},y=Math.round(y/({time_step.parsed_value*time_scale.parsed_value}))*({time_step.parsed_value*time_scale.parsed_value})"')
+                    scene_time_step = time_step.parsed_value*time_scale.parsed_value
+                    preview_scene.props(f'drag_constraints="x={scene_pos[0]},z={scene_pos[2]},y=Math.round(y/({scene_time_step}))*({scene_time_step})"')
+                else:
+                    preview_scene.props(f'drag_constraints="y={scene_pos[1]}"')
+            
+            for c in self.cursors.values():
+                if self.copy:
+                    c.material(copy_color.value, copy_opacity.parsed_value)
                 else:
-                    t = (_find_free_slot(selection.drag_time + selection.offset[2]) if copy.value else selection.drag_time + selection.offset[2])
-                    preview_scene.props(f'drag_constraints="y={t*time_scale.parsed_value}"')
+                    c.material(move_color.value, move_opacity.parsed_value)
 
-        def move(self, offset: "numpy array (4)"):
+        def move(self, offset: "numpy array (3)"):
             self.offset += offset
             self._update_cursors()
 
         def rotate(self, rotation: float):
             self.rotation += rotation if not self.mirrored else -rotation
             self._update_cursors()
 
         def mirror(self, horizontal: bool):
             self.mirrored = not self.mirrored
             if horizontal:
                 self.rotation += 180
             self._update_cursors()
 
+        def set_copy(self, copy: bool):
+            self.copy = copy
+            self._update_cursors()
+
         def apply(self):
             nonlocal walls
-            undo.push_undo("apply transform")
-            pivot_3d = walls[self.drag_time if self.drag_time is not None else min(self.sources)][0,:3]
+            ops = [l for v, l in [(self.copy, "copy"), (self.rotation, "rotate"), (self.mirrored, "mirror"), (np.any(self.offset), "offset")] if v]
+            undo.push_undo(f"{pretty_list(ops)} {len(self.sources)} walls")
+            first = min(self.sources)
+            copy_offset = [0.0,0.0,_find_free_slot(first+self.offset[2])-first-self.offset[2],0.0,0.0] if self.copy else 0.0
+            pivot_3d = walls[self.drag_time if self.drag_time is not None else first][0,:3]
             scale_3d = np.array([1.0, -1.0 if self.mirrored else 1.0, 1.0])
             new_sources = set()
             new_walls = {}
             for t in sorted(self.sources):
-                w = walls[t] if copy.value else walls.pop(t)
+                w = walls[t]+copy_offset if self.copy else walls.pop(t)
                 w = movement.rotate_around(w, self.rotation, pivot_3d)
                 w = movement.scale_from(w, scale_3d, pivot_3d)
                 w = movement.offset(w, self.offset)
                 new_walls[w[0,2]] = w
                 new_sources |= {w[0,2]}
-            walls |= new_walls
+
+            try:
+                sym_ops: list[str|int] = []
+                if mirror_x.value:
+                    sym_ops.append("mirror_x")
+                if mirror_y.value:
+                    sym_ops.append("mirror_y")
+                if rotsym_direction.value is not None:
+                    rsym = rotsym.value * (-1 if rotsym_direction.value else 1)
+                    if rotate_first.value:
+                        sym_ops.insert(0, int(rsym))
+                    else:
+                        sym_ops.append(int(rsym))
+                sym_interval = symmetry_step.parsed_value
+                new_walls |= pattern_generation.generate_symmetry(new_walls, sym_ops, sym_interval)
+            except ParseInputError as pie:
+                error(f"Error parsing symmetry setting: {pie.input_id}", pie, data=pie.value)
+                # continue anyway
+                
+            for _, w in sorted(new_walls.items()):
+                _insert_wall(w, displace_forward=self.offset[2]>0)
             _soft_refresh()
             self.select(new_sources, "set")
 
         def start_drag(self, object_id: str):
             for t, c in self.cursors.items():
                 if c.id == object_id:
                     self.drag_time = t
@@ -244,34 +297,47 @@
                 for t in self.sources:
                     if t != self.drag_time:
                         w = walls[t]
                         relative = np.array([[0.0,0.0,0.0, w[0,3], 0.0]])
                         e = preview_scene.wall_extrusion(relative, preview_settings.wall.size * time_scale.parsed_value)
                         offset = movement.rotate(w-pivot, 180-pivot[0,4])
                         e.move(offset[0,0], offset[0,1], -(w[0,2]-pivot[0,2])*time_scale.parsed_value).rotate(0,0,np.deg2rad(w[0,4]-pivot[0,4]))
-                        if copy.value:
+                        if self.copy:
                             e.material(copy_color.value, copy_opacity.parsed_value/2)
                         else:
                             e.material(move_color.value, move_opacity.parsed_value/2)
                         self.cursors[t] = e
             self._update_cursors()
 
         def end_drag(self, xyt: tuple[float, float, float]):
             self.offset = np.array(xyt) - walls[self.drag_time][0,:3]
             self.apply()
 
     selection = Selection()
 
     def _on_key(e: events.KeyEventArguments) -> None:
+        if e.key.control:
+            selection.set_copy(e.action.keydown)
         if not e.action.keydown:
             return
         try:
             # note: don't use key.code, as that doesn't account for keyboard layout
             key_name = e.key.name.upper()  # key.name is upper/lowercase depending on shift
-            if e.modifiers.ctrl:
+            # CTRL-independent
+            if e.key.number in range(1, len(synth_format.WALL_LOOKUP)+1):
+                wall_type = sorted(synth_format.WALL_LOOKUP)[e.key.number-1]
+                _spawn_wall(wall_type=wall_type, change_selection=e.modifiers.ctrl, extend_selection=e.modifiers.shift)
+            elif e.key.is_cursorkey:
+                selection.move(np.array([(e.key.arrow_right-e.key.arrow_left),(e.key.arrow_up-e.key.arrow_down),0.0])*offset_step.parsed_value)
+            elif e.key.page_up or e.key.page_down:
+                selection.move(np.array([0.0,0.0,(e.key.page_up-e.key.page_down)*time_step.parsed_value])*offset_step.parsed_value)
+            elif e.key.enter or e.key.space:
+                selection.apply()
+            # CTRL: Yes
+            elif e.modifiers.ctrl:
                 if key_name == "A":
                     # select all
                     selection.select(set(walls), mode="set")
                     # clear text selection
                     ui.run_javascript("""
                     var sel = window.getSelection ? window.getSelection() : document.selection;
                         if (sel) {
@@ -294,87 +360,78 @@
                         _soft_refresh()
                 elif key_name == "V":
                     _paste()
                 elif key_name == "Z":
                     undo.undo()
                 elif key_name == "Y":
                     undo.redo()
+            # CTRL: No
             elif e.key.escape:
                 selection.select(set(), "set")
             elif key_name == "T":
                 axis_z.value = not axis_z.value
                 selection.select(set(), "toggle")
-            elif key_name == "C":
-                copy.value = not copy.value
-                for c in selection.cursors.values():
-                    if copy.value:
-                        c.material(copy_color.value, copy_opacity.parsed_value)
-                    else:
-                        c.material(move_color.value, move_opacity.parsed_value)
-                selection.select(set(), "toggle")
             elif key_name == "R":
                 _compress()
             elif key_name == "B":
                 _open_blend_dialog()
-            elif e.key.number in range(1, len(synth_format.WALL_LOOKUP)+1):
-                wall_type = sorted(synth_format.WALL_LOOKUP)[e.key.number]
-                new_t = _find_free_slot(max(selection.sources, default=0.0))
-                _insert_wall(np.array([[0.0,0.0,new_t,wall_type,0.0]]))
-                _soft_refresh()
-                selection.select({new_t}, mode="set" if not e.modifiers.shift else "toggle")
             elif key_name == "E":
                 ordered_keys = sorted(walls)
                 if not ordered_keys:
                     return
                 if not selection.sources:
                     selection.select({ordered_keys[0]}, mode="set")
                 elif max(selection.sources) in ordered_keys[:-1]:
                     selection.select({ordered_keys[ordered_keys.index(max(selection.sources))+1]}, mode="set" if not e.modifiers.shift else "expand")
-            elif key_name == "E":
+            elif key_name == "Q":
                 ordered_keys = sorted(walls)
                 if not ordered_keys:
                     return
                 if not selection.sources:
                     selection.select({ordered_keys[-1]}, mode="set")
                 elif min(selection.sources) in ordered_keys[1:]:
                     selection.select({ordered_keys[ordered_keys.index(min(selection.sources))-1]}, mode="set" if not e.modifiers.shift else "expand")
             elif not selection.sources:
                 return
             elif e.key.delete or e.key.backspace:
                 selection.delete()
-            elif e.key.enter or e.key.space:
-                selection.apply()
-            elif e.key.is_cursorkey:
-                selection.move(np.array([(e.key.arrow_right-e.key.arrow_left),(e.key.arrow_up-e.key.arrow_down),0.0])*offset_step.parsed_value)
-            elif e.key.page_up or e.key.page_down:
-                selection.move(np.array([0.0,0.0,(e.key.page_up-e.key.page_down)*time_step.parsed_value])*offset_step.parsed_value)
             elif key_name == "D":
                 selection.rotate(-(angle_step.parsed_value if not e.modifiers.shift else 90.0))
             elif key_name == "A":
                 selection.rotate(angle_step.parsed_value if not e.modifiers.shift else 90.0)
             elif key_name in "WS":
                 selection.mirror(horizontal=(key_name=="S"))
         except ParseInputError as pie:
-            error(f"Error parsing preview setting: {pie.input_id}", pie, data=pie.value)
+            error(f"Error parsing setting: {pie.input_id}", pie, data=pie.value)
             return
-    keyboard = ui.keyboard(on_key=_on_key)
+    keyboard = ui.keyboard(on_key=_on_key, ignore=['input', 'select', 'button', 'textarea', "switch"])
     # dummy checkbox to bind keyboard enable state
     kb_enable = ui.checkbox(value=False).style("display:none").bind_enabled_to(keyboard, "active").bind_value_from(app.storage.user, "active_tab", backward=lambda v: v=="Wall Art")
     with ui.card():
         with ui.row():
             with ui.row():
-                ui.label("Axis:").classes("my-auto")
-                with ui.toggle({False: "X&Y", True: "Time"}, value=False).props('color="grey-7" rounded dense').classes("my-auto") as axis_z:
-                    ui.tooltip("Change movement axis (T)")
-                ui.label("Copy:").classes("my-auto")
-                with ui.switch().props("dense").classes("my-auto") as copy:
-                    ui.tooltip("Copy to next free slot instead of moving (C). Makes selection look weird.")
-                time_step = SMHInput("Time Step", "1/64", "time_step", suffix="b", tooltip="Time step for adding and moving walls via (page-up)/(page-down)")
-                offset_step = SMHInput("Offset Step", "1", "offset_step", suffix="sq", tooltip="Step for offsetting when pressing (arrow keys)")
-                angle_step = SMHInput("Angle Step", "15", "angle_step", suffix="°", tooltip="Rotation when pressing (A)/(D)")
+                axis_z = LargeSwitch("axis", "(T) Change movement axis between X/Y and Time", color="info", icon_unchecked="open_with", icon_checked="schedule")
+                displace = LargeSwitch("displace", "Displace existing walls when moving in time instead of replacing them.", color="warning", icon_unchecked="cancel", icon_checked="move_up")
+                time_step = SMHInput("Time Step", "1/64", "time_step", suffix="b", tooltip="Time step for adding walls or moving via dragg or (page-up)/(page-down)")
+                offset_step = SMHInput("Offset Step", "1", "offset_step", suffix="sq", tooltip="Step for moving via (arrow keys)")
+                angle_step = SMHInput("Angle Step", "15", "angle_step", suffix="°", tooltip="Step for rotation via (A)/(D)")
+            with ui.expansion("Symmetry", icon="flip").props("dense"):
+                with ui.row():
+                    symmetry_step = SMHInput("Interval", "1/4", "symmetry_step", suffix="b", tooltip="Time step for symmetry copies")
+                    rotate_first = LargeSwitch("rotate_first", "Mirror or rotate first", color="secondary", icon_unchecked="flip", icon_checked="rotate_left")
+                    ui.separator().props("vertical")
+                    mirror_x = LargeSwitch("mirror_x", "Mirror across X axis, ie left-right", color="negative", icon_unchecked="align_horizontal_left", icon_checked="align_horizontal_center")
+                    mirror_y = LargeSwitch("mirror_y", "Mirror across Y axis, ie up-down", color="positive", icon_unchecked="align_vertical_bottom", icon_checked="align_vertical_center")
+                with ui.row():
+                    ui.label("Rotation: ").classes("my-auto")
+                    rotsym_direction = LargeSwitch("rotsym_direction", "Rotation direction", color="secondary", icon_unchecked="rotate_left", icon_checked="rotate_right").props('toggle-indeterminate indeterminate-icon="cancel"')
+                    with ui.row():
+                        ui.tooltip("Number of rotational symmetry. Note that mirror in both X and Y overlaps with even symmetries, ie 2x/4x/etc")
+                        rotsym = ui.slider(min=2, max=12, value=2).props('snap markers selection-color="transparent" color="secondary" track-size="2px" thumb-size="25px"').classes("w-28").bind_value(app.storage.user, "wall_art_rotsym").bind_enabled_from(rotsym_direction, "value", backward=lambda v: v is not None)
+                        ui.label().classes("my-auto w-8").bind_text_from(rotsym, "value", backward=lambda v: f"x{v}")
             with ui.expansion("Preview setttings", icon="palette").props("dense"):
                 sp = SettingsPanel()
                 ui.separator()
                 with ui.row():
                     move_color = ui.color_input("Move", value="#888888", preview=True).props("dense").classes("w-28").bind_value(app.storage.user, "wall_art_move_color")
                     move_color.button.style("color: black")
                     move_opacity = SMHInput("Opacity", "0.5", "move_opacity")
@@ -400,22 +457,48 @@
                         refimg_y = SMHInput("Y", "0", "wall_art_ref_y", suffix="sq", tooltip="Center Y of the reference image in sq")
                         refimg_t = SMHInput("Time", "1/4", "wall_art_ref_time", suffix="b", tooltip="Time of the reference image in beats")
                 apply_button = ui.button("Apply").props("outline")
         def _find_free_slot(t: float) -> float:
             while t in walls:
                 t = np.round(t/time_step.parsed_value + 1)*time_step.parsed_value
             return t
-        def _insert_wall(w: "np.array (1,5)"):
-            undo.push_undo(f"add {synth_format.WALL_LOOKUP[w[0,3]]}")
+
+        def _insert_wall(w: "np.array (1,5)", displace_forward: bool = False):
+            if not displace.value:
+                walls[w[0,2]] = w
+                return
             pending = w
+            displace_dir = -1 if displace_forward else 1
             while pending[0,2] in walls:
                 walls[pending[0,2]], pending = pending, walls[pending[0,2]]
-                pending[0,2] = np.round(pending[0,2]/time_step.parsed_value + 1)*time_step.parsed_value
+                pending[0,2] = np.round(pending[0,2]/time_step.parsed_value + displace_dir)*time_step.parsed_value
             walls[pending[0,2]] = pending
 
+        def _spawn_wall(wall_type: int, change_selection: bool = False, extend_selection: bool = False):
+            if change_selection:
+                if not selection.sources:
+                    return
+                undo.push_undo(f"change {len(selection.sources)} walls to {synth_format.WALL_LOOKUP[wall_type]}")
+                for s in selection.sources:
+                    walls[s] = np.array([[0.0,0.0,s, wall_type,0.0]])
+                _soft_refresh()
+                selection.select(set(), "toggle")
+            else:
+                undo.push_undo(f"add {synth_format.WALL_LOOKUP[wall_type]}")
+                try:
+                    new_t = 0.0 if not selection.sources else max(selection.sources) + time_step.parsed_value
+                    if not displace.value:
+                        new_t = _find_free_slot(max(selection.sources, default=0.0))
+                    _insert_wall(np.array([[0.0,0.0,new_t,wall_type,0.0]]))
+                    _soft_refresh()
+                    selection.select({new_t}, mode="set" if not extend_selection else "toggle")
+                except ParseInputError as pie:
+                    error(f"Error parsing setting: {pie.input_id}", pie, data=pie.value)
+                    return
+
         def _soft_refresh():
             nonlocal refimg_obj
             try:
                 preview_settings = sp.parse_settings()
             except ParseInputError as pie:
                 error(f"Error parsing preview setting: {pie.input_id}", pie, data=pie.value)
                 return
@@ -483,57 +566,57 @@
                 with ui.dialog() as key_dialog, ui.card():
                     with ui.row().classes("bg-orange w-full"):
                         ui.icon("warning", size="xl").classes("my-auto")
                         ui.label("This is quite experimental. Let me know if you run into any bugs.").classes("m-auto")
                         ui.icon("warning", size="xl").classes("my-auto")
                     ui.markdown("""
                         ## Camera
-                        Use left mouse to rotate the camera, right mouse (or left mouse and SHIFT or CTRL) to move. Scroll wheel zooms.  
+                        Use left mouse to rotate the camera, right mouse to move. Scroll wheel zooms.  
                         To turn the camera *without* deselecting, hold down ALT.
 
-                        Click on a wall to select it. Multiple walls can be selected by CTRL-Click (add/remove), or SHIFT-Click (expand selection to clicked wall).
-                        Then drag it around using left mouse and/or use one of the edit keys below.
+                        Click on a wall to select it. Multiple walls can be selected by CTRL-Click (to add), or SHIFT-Click (expand selection to clicked wall).
+                        Then drag it around using left mouse and/or use one of the edit keys below. Holding CTRL copies to the next free slot instead of moving.
 
                         ## General
                         |Key|Function|
                         |-|-|
                         |ESC|Deselect all|
                         |CTRL+🇦|Select all|
                         |CTRL+🇨|Copy to clipboard (selection or everything)|
                         |CTRL+🇽|Cut to clipboard (selection or everything)|
                         |CTRL+🇻|Add walls from clipboard (overrides existing)|
                         |CTRL+🇿|Undo last operation|
                         |CTRL+🇾|Redo last operation|
-                        |🇪/🇶|Next or previous Wall (SHIFT: Expand selection)|
+                        |🇶/🇪|Select previous/next Wall (SHIFT: Expand selection)|
                         |🇹|Change Axis between X/Y and Time|
-                        |🇨|Toggle Copy (Makes selection look weird)|
                         |🇷|Compress all walls to timestep|
                         |🇧|Open Blender|
 
                         ## Edit
                         If you use keyboard shortcuts instead of dragging, press enter, space or click the shadow to apply.
 
                         |Key|Function|
                         |-|-|
-                        |1️⃣-8️⃣|Spawn & select wall (SHIFT: Add to selection)|
+                        |1️⃣-8️⃣|Spawn & select wall (SHIFT: Add to current selection)|
+                        |CTRL+1️⃣-8️⃣|Change wall type|
                         |`Del`/Backspace|Delete selection|
                         |🇦/🇩|Rotate by step (SHIFT: 90 degree)|
                         |🇼|Mirror on Y axis (up-down)|
                         |🇸|Mirror on X axis (left-right)|
                         |⬅️➡️⬆️⬇️|Offset X/Y|
                         |Page Up/Down|Offset Time|
-                        |Enter/Space|Apply|
+                        |Enter/Space|Apply (CTRL: Copy to next free slot)|
                     """)
                 with ui.button(icon="keyboard", on_click=key_dialog.open, color="info").classes("cursor-help").style("width: 36px"):
                     ui.tooltip("Show controls")
                 ui.separator()
                 with ui.button(icon="undo", color="negative", on_click=undo.undo).props("outline").style("width: 36px").bind_enabled_from(undo, "undo_stack", backward=bool):
-                    ui.tooltip("Undo (CTRL+Z)")
+                    ui.tooltip().bind_text_from(undo, "undo_stack", backward=lambda us: f"Undo '{us[-1][0]}' (CTRL+Z) [{len(us)} steps]" if us else "Undo (CTRL+Z)")
                 with ui.button(icon="redo", color="positive", on_click=undo.redo).props("outline").style("width: 36px").bind_enabled_from(undo, "redo_stack", backward=bool):
-                    ui.tooltip("Redo (CTRL+Y)")
+                    ui.tooltip().bind_text_from(undo, "redo_stack", backward=lambda rs: f"Redo '{rs[-1][0]}' (CTRL+Y) [{len(rs)} steps]" if rs else "Redo (CTRL+Y)")
                 ui.separator()
                 def _paste():
                     clipboard = pyperclip.paste()
                     try:
                         data = synth_format.import_clipboard_json(clipboard, use_original=False)
                     except ValueError as ve:
                         error(f"Error reading data from clipboard", ve, data=clipboard)
@@ -553,81 +636,116 @@
                 with ui.button(icon="clear", color="negative", on_click=lambda _: (undo.reset(), walls.clear(), _soft_refresh())).props("outline").style("width: 36px"):
                     ui.tooltip("Clear everything (includes undo steps)")
                 ui.separator()
                 def _compress():
                     undo.push_undo("compress")
                     new_sources = set()
                     for i, (t, w) in enumerate(sorted(walls.items())):
+                        w = w.copy()
                         del walls[t]
                         w[...,2] = i * time_step.parsed_value
                         walls[w[0,2]] = w
                         if t in selection.sources:
                             new_sources.add(w[0,2])
                     selection.select(new_sources, mode="set")
                     _soft_refresh()
 
                 with ui.button(icon="compress", on_click=_compress).props("outline").style("width: 36px"):
                     ui.tooltip("Compress wall spacing to time step (effects all walls)")
                 with ui.dialog() as blend_dialog, ui.card():
                     ui.label("Blend between patterns")
+                    blend_pattern = ui.select({}, label="Choose a detected pattern:")
+                    # >1 option: show selector
+                    blend_pattern.bind_visibility_from(blend_pattern, "options", backward=lambda opts: len(opts)!=1)
+                    # 1 option: show just text
+                    ui.label("").bind_visibility_from(blend_pattern, "options", backward=lambda opts: len(opts)==1).bind_text_from(
+                        blend_pattern, "options", backward=lambda opts: "Detected: " + next(iter(opts.values())) if opts else ""
+                    )
                     with ui.row():
-                        blend_wallcount = SMHInput("Walls", 0, "blend_wallcount", "Walls per pattern. Can be -1 if pattern count is set")
-                        blend_patterncount = SMHInput("Patterns", 0, "blend_patterncount", "Number of patterns to blend between. Can be -1 if wall count is set")
-                    with ui.row():
-                        blend_spacing = SMHInput("Spacing", "1/2", "blend_spacing", "Interval between blending stemps")
+                        blend_interval = SMHInput("Interval", "1/2", "blend_interval", "Interval between blending steps", suffix="b")
                         def _do_blend():
                             nonlocal walls
-                            try:
-                                patterns = np.array([w[0] for _, w in sorted(walls.items())]).reshape((int(blend_patterncount.parsed_value), int(blend_wallcount.parsed_value), 5))
-                                interval = blend_spacing.parsed_value
-                            except ParseInputError as pie:
-                                error(f"Error parsing blend inputs: {pie.input_id}", pie, data=pie.value)
+                            wc, pc, pl = blend_pattern.value
+                            if len(walls) != wc*pc:
+                                error(f"Wall count changed! Expected {pc*wc}, found {len(walls)}", data=walls)
                                 return
+                            try:
+                                patterns = np.array([w[0] for _, w in sorted(walls.items())]).reshape((pc, wc, 5))
+                                interval = blend_interval.parsed_value
                             except ValueError as ve:
-                                error(f"Could not split up walls into {blend_patterncount.parsed_value} x {blend_wallcount.parsed_value}", ve, data=walls)
+                                error(f"Could not split up {len(walls)} walls into {pc} patterns with {wc} wall{'s'*(wc!=1)} each", ve, data=walls)
+                                return
+                            pattern_deltas = np.diff(patterns[:,0,2])
+                            if pattern_deltas.max() <= interval:
+                                error(
+                                    f"Blend interval ({pretty_fraction(interval)}b) must be greater than largest pattern distance ({pretty_fraction(pattern_deltas.max())}b), else blending will do nothing.",
+                                    data=walls,
+                                )
                                 return
+
+                            if interval <= pl:
+                                ui.notify(
+                                    f"Blend interval ({pretty_fraction(interval)}b) is shorter than pattern length ({pretty_fraction(pl)}b), leading to overlaps. This may result in strange results.",
+                                    type="warning",
+                                )
+
+                            small_deltas = np.sum(pattern_deltas < interval)  # equal is a "regular" usecase, ie when re-blending some parts
+                            if small_deltas: 
+                                ui.notify(
+                                    f"Blend interval ({pretty_fraction(interval)}b) is smaller than {small_deltas} of {patterns.shape[0]-1} pattern distances. Blending will do nothing between these.",
+                                    type="warning"
+                                )
                             undo.push_undo("blend")
                             try:
                                 walls |= pattern_generation.blend_walls_multiple(patterns, interval=interval)
                             except ValueError as ve:
                                 error("Error blending walls", ve, data=walls)
                                 return
+                            added = len(walls)//patterns.shape[1] - patterns.shape[0]
+                            ui.notify(f"Created {added} additional pattern{'s'*(added!=1)} between the existing {patterns.shape[0]}", type="info")
                             _soft_refresh()
                             blend_dialog.close()
                         ui.button(icon="blender", on_click=_do_blend).props("outline").classes("w-16 h-10")
 
                 def _open_blend_dialog():
+                    if len(walls) < 2:
+                        error("Need at least two walls to do blending", data=walls)
+                        returnc
                     # autodetect patterns
                     try:
-                        wallcount, patterncount = pattern_generation.find_wall_patterns(walls)
+                        detected_patterns = pattern_generation.find_wall_patterns(walls)
                     except ValueError as ve:
-                        error("Could not detect patterns in walls", ve, data=walls)
+                        error(f"Could not detect patterns in walls: {ve}", data=walls)
                         return
                     blend_dialog.open()
-                    blend_wallcount.set_value(str(wallcount))
-                    blend_patterncount.set_value(str(patterncount))
-                    blend_spacing.update()  # workaround for nicegui#2149
+                    blend_pattern.set_options({
+                        (w, p, l): (
+                            f"{p} patterns, each with {w} walls and {pretty_fraction(l)}b long"
+                            if w != 1 else f"{p} instances of a single wall"
+                        )
+                        for w, p, l in detected_patterns
+                    })
+                    blend_pattern.set_value(detected_patterns[0])
+                    blend_interval.update()  # workaround for nicegui#2149
 
                 with ui.button(icon="blender", on_click=_open_blend_dialog, color="info").style("width: 36px"):
                     ui.tooltip("Blend wall patterns (effects all walls)")
             draw_preview_scene()
             with ui.column():
                 with ui.button(icon="delete", color="negative", on_click=selection.delete).style("width: 36px").bind_enabled_from(selection, "sources", backward=bool):
                     ui.tooltip("Delete selection (Delete/Backspace)")
                 for k, (i, t) in enumerate(sorted(synth_format.WALL_LOOKUP.items())):
-                    def _add_wall(*_, wall_type=i):  # python closure doesn't work as needed here, so enclose i as default param instead
-                        new_t = _find_free_slot(max(selection.sources, default=0.0))
-                        _insert_wall(np.array([[0.0,0.0,new_t, wall_type,0.0]]))
-                        _soft_refresh()
-                        selection.select({new_t}, "set")
-                    with ui.button(color="positive", on_click=_add_wall).classes("p-2"):
-                        ui.tooltip(f"Spawn '{t}' wall after selection ({k})")
+                    def _add_wall(e: events.GenericEventArguments, wall_type=i):
+                        # python closure doesn't work as needed here, so enclose i as default param instead
+                        _spawn_wall(wall_type=wall_type, change_selection=e.args["ctrlKey"], extend_selection=e.args["shiftKey"])
+                    with ui.button(color="positive").on("click", _add_wall).classes("p-2"):
+                        ui.tooltip(f"({k+1}) Spawn '{t}' wall (after selection), hold CTRL to change wall type instead")
                         v = synth_format.WALL_VERTS[t]
                         # draw wall vertices as svg
                         content = f'''
                             <svg viewBox="-10 -10 20 20" width="20" height="20" xmlns="http://www.w3.org/2000/svg">
                                 <polygon points="{' '.join(f"{-x},{y}" for x,y in v)}" stroke="white"/>
                             </svg>
                         '''
                         ui.html(content)
             
-        apply_button.on("click", draw_preview_scene.refresh)
+        apply_button.on("click", draw_preview_scene.refresh)
```

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/movement.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/movement.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/pattern_generation.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/pattern_generation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Literal
+
 import numpy as np
 
 from .synth_format import DataContainer, WALLS, WALL_LOOKUP, WALL_SYMMETRY
 from .utils import bounded_arange
 from . import movement
 
 # generic helpers
@@ -64,19 +66,19 @@
         | {t: nodes + [distance/2,0,0] for t, nodes in sorted(data.single.items())}
         | {t: nodes + [distance/2,0,0] for t, nodes in sorted(data.both.items())}
     )
     # wipe single & both
     data.single = {}
     data.both = {}
 
-def find_wall_patterns(walls: WALLS) -> tuple[int, int]:
-    """try to find repeating "patterns" with identical wall type and timing"""
+def find_wall_patterns(walls: WALLS) -> list[tuple[int, int, float]]:
+    """try to find repeating "patterns" with identical wall type and timing, returns wall count per pattern, pattern count and pattern length for all possible candidates"""
     wall_count = len(walls)
     if wall_count < 2:
-        raise ValueError("At least two walls must be selected")
+        raise ValueError("Need at least two walls to find repeating patterns")
     wall_types = [w[0,3] for _, w in sorted(walls.items())]
 
     # find candidates for patterns, by looking where the first wall type is repeated
     matching_first = [i for i, t in enumerate(wall_types) if i and t == wall_types[0]]
     if not matching_first:
         raise ValueError(f"Could not find any repeats of first wall ({WALL_LOOKUP[wall_types[0]]})")
     # now ensure it is an divisor of the wall count
@@ -85,19 +87,22 @@
         raise ValueError(f"Could not find any repeats of first wall that are divisors of total wall count ({wall_count})")
     # now check if types match
     matching_types = [i for i in matching_count if wall_types == wall_types[:i] * (wall_count//i)]
     if not matching_types:
         raise ValueError(f"Could not find any wall type pattern that repeats consistently")
     # finally check times
     wall_times = np.array([w[0,2] for _, w in sorted(walls.items())])
+    out = []
     for walls_per_pattern in reversed(matching_types):  # start with the largest candidate
         reshaped = wall_times.reshape((-1, walls_per_pattern)).copy()
         reshaped -= reshaped[:,0,np.newaxis]
         if np.allclose(reshaped[0], reshaped):
-            return walls_per_pattern, wall_count // walls_per_pattern
+            out.append((walls_per_pattern, wall_count//walls_per_pattern, reshaped[0,-1]-reshaped[0,0]))
+    if out:
+        return out
     raise ValueError(f"Could not find any pattern of type AND timing that repeats consistently")
 
 def blend_wall_single(first: "numpy array (n, 5)", second: "numpy array (n, 5)", interval: float, with_symmetry: bool=True) -> dict[str, "numpy array (1, 5)"]:
     """create blending substeps between two patterns
     
     first and second must be numpy arrays of the patterns (each with n walls)
     with_symmetry can be set to false to disregard that symetrical walls (like squares) look the same in multiple orientations
@@ -136,7 +141,31 @@
 
 def blend_walls_multiple(patterns: list["numpy array (n, 5)"], interval: float, with_symmetry: bool=True) -> dict[str, "numpy array (1, 5)"]:
     """calls blend_wall_single to blending between multiple patterns, each with n walls"""
     out_walls = {}
     for first, second in zip(patterns[:-1], patterns[1:]):
         out_walls |= blend_wall_single(first, second, interval=interval, with_symmetry=with_symmetry)
     return out_walls
+
+def generate_symmetry(source: dict[str, "numpy array (n, 5)"], operations: list[Literal["mirror_x", "mirror_y"]|int], interval: float, pivot_3d: "numpy_array (3)" = np.zeros((3,))) -> dict[str, "numpy array (n, 5)"]:
+    out = source.copy()
+    offset = np.array([0.0,0.0,interval,0.0,0.0])
+    counter = 1
+    for o in operations:
+        new_out = out.copy()
+        if o in ("mirror_x", "mirror_y"):
+            scale = np.array([-1.0,1.0,1.0]) if o=="mirror_x" else np.array([1.0,-1.0,1.0])
+            for _, v in sorted(out.items()):
+                v = movement.scale_from(v, scale, pivot_3d=pivot_3d) + offset*counter
+                new_out[v[0,2]] = v
+            counter += 1
+        elif isinstance(o, int):
+            for _, v in sorted(out.items()):
+                ang = 360 / o
+                for r in range(1,abs(o)):
+                    vrot = movement.rotate_around(v, ang*r, pivot_3d=pivot_3d) + offset*counter*r
+                    new_out[vrot[0,2]] = vrot
+            counter += (abs(o)-1)
+        else:
+            raise ValueError(f"Unknown symmetry operation {o!r}")
+        out = new_out
+    return out
```

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/rails.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/rails.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -353,8 +353,8 @@
             out[time] = nodes
             continue
 
         steps = bounded_arange_plusminus(nodes[0,2], nodes[-1,2], max_length)
         new_z = np.union1d(nodes[:,2], steps)
         for start in steps[:-1]:
             out[start] = interpolate_spline(nodes, new_z=new_z[np.logical_and(new_z>=start, new_z<=(start+abs(max_length)))])
-    return out
+    return out
```

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/synth_format.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/synth_format.py`

 * *Files identical despite different names*

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper/utils.py` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union
+from typing import Any, Union
 
 import numpy as np
 
 def bounded_arange(start: float, end: float, step: float) -> "numpy array (x)":
     # arange would not include the end position, so we intentially overshoot, then correct
     new_times = np.arange(start, end + step, step)
     if np.isclose(new_times[-2], end):
@@ -127,21 +127,31 @@
             return f"{i} {v//gcd}/{192//gcd}"
     return str(val)
 
 def pretty_time_delta(seconds: float) -> str:
     seconds = abs(seconds)
     if seconds < 1:
         return f"{seconds*1000:.0f} ms"
-    if seconds < 60:
-        return f"{seconds:.0f} seconds"
-    if seconds < 3600:
-        return f"{seconds//60} minutes"
-    if seconds < 24*3600:
-        return f"{seconds//3600} hours"
-    days = seconds // (24*3600)
-    if days < 7:
-        return f"{days} days"
-    if days < 30:
-        return f"{days//7} weeks"
-    if days < 365:
-        return f"{days//30} months"
-    return f"{days//365} years"
+    units = {
+        "second": 60,
+        "minute": 60,
+        "hour": 24,
+        "day": 7,
+        "week": 30/7,
+        "month": 365/30,
+        "year": 1000,
+    }
+    value = seconds
+    for unit, next_unit in units.items():
+        if value < next_unit:
+            # add 's' if value rounds to 2 or more
+            return f"{value:.0f} {unit}{'s' if value >= 1.5 else ''}"
+        value = value / next_unit
+    return "a really long time"
+
+
+def pretty_list(data: list[Any]) -> str:
+    if not data:
+        return ""
+    if len(data) == 1:
+        return str(data[0])
+    return ", ".join(map(str, data[:-1])) + f" and {data[-1]}"
```

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper.egg-info/PKG-INFO` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synth_mapping_helper
-Version: 1.4.0
+Version: 1.4.1
 Summary: Toolbox for manipulating the JSON-Format used by Synth Riders Beatmap Editor in the clipboard
 Author: adosikas
 License: MIT License
         
         Copyright (c) 2024 adosikas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `synth_mapping_helper-1.4.0/src/synth_mapping_helper.egg-info/SOURCES.txt` & `synth_mapping_helper-1.4.1/src/synth_mapping_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

