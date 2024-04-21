# Comparing `tmp/sdcopy-0.1.0.tar.gz` & `tmp/sdcopy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdcopy-0.1.0.tar", max compression
+gzip compressed data, was "sdcopy-0.2.0.tar", max compression
```

## Comparing `sdcopy-0.1.0.tar` & `sdcopy-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1075 2024-04-01 04:33:11.680411 sdcopy-0.1.0/LICENSE
--rw-r--r--   0        0        0       47 2024-04-01 04:34:29.140646 sdcopy-0.1.0/README.md
--rw-r--r--   0        0        0      997 2024-04-01 04:22:50.686881 sdcopy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-31 18:01:35.189331 sdcopy-0.1.0/sdcopy/__init__.py
--rw-r--r--   0        0        0       67 2024-04-01 04:10:57.087909 sdcopy-0.1.0/sdcopy/__main__.py
--rw-r--r--   0        0        0     3220 2024-04-01 04:22:17.997237 sdcopy-0.1.0/sdcopy/cli.py
--rw-r--r--   0        0        0        0 2024-03-31 19:27:11.415684 sdcopy-0.1.0/sdcopy/utils.py
--rw-r--r--   0        0        0      932 1970-01-01 00:00:00.000000 sdcopy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-04-01 04:33:11.680411 sdcopy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2082 2024-04-21 16:25:38.186079 sdcopy-0.2.0/README.md
+-rw-r--r--   0        0        0      980 2024-04-21 17:10:24.768763 sdcopy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-31 18:01:35.189331 sdcopy-0.2.0/sdcopy/__init__.py
+-rw-r--r--   0        0        0       67 2024-04-21 16:25:37.852573 sdcopy-0.2.0/sdcopy/__main__.py
+-rw-r--r--   0        0        0     3325 2024-04-21 17:18:29.787350 sdcopy-0.2.0/sdcopy/cli.py
+-rw-r--r--   0        0        0     2929 1970-01-01 00:00:00.000000 sdcopy-0.2.0/PKG-INFO
```

### Comparing `sdcopy-0.1.0/LICENSE` & `sdcopy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdcopy-0.1.0/pyproject.toml` & `sdcopy-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdcopy"
-version = "0.1.0"
+version = "0.2.0"
 description = "Tool for saving files off SD cards"
 authors = ["Dmitry Gerasimenko <kiddima@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/kidig/sdcopy"
 packages = [
     { include = "sdcopy" },
@@ -22,15 +22,14 @@
 ]
 
 [tool.poetry.scripts]
 sdcopy = "sdcopy.__main__:main"
 
 [tool.poetry.dependencies]
 python = "^3.11"
-click = "^8.1.7"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.7.0"
 
 
 [build-system]
```

### Comparing `sdcopy-0.1.0/sdcopy/cli.py` & `sdcopy-0.2.0/sdcopy/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,107 +1,110 @@
+import argparse
+import logging
 import os
 import shutil
+import time
 from concurrent.futures import ThreadPoolExecutor
 from configparser import ConfigParser
 from datetime import datetime
 from pathlib import Path
 
-import click
-
-DEFAULT_CFG = [
+DEFAULT_CONFIG_PATHS = [
     "config.ini",
     Path.home() / ".sdcopy",
 ]
+if default_config := os.getenv("SDCOPY_CONFIG"):
+    DEFAULT_CONFIG_PATHS = [default_config]
+
+DEFAULT_LOG_LEVEL = "INFO"
+LOG_LEVEL = os.getenv("SDCOPY_LOG_LEVEL", DEFAULT_LOG_LEVEL)
+LOG_FORMAT = os.getenv("SDCOPY_LOG_FORMAT", "%(message)s")
+
+log_level = logging.getLevelNamesMapping().get(LOG_LEVEL, DEFAULT_LOG_LEVEL)
+logging.basicConfig(level=log_level, format=LOG_FORMAT)
 
 
 def file_times(src: Path) -> tuple[float, float]:
     """Get file timestamps"""
     stat = src.stat()
     return stat.st_atime, stat.st_mtime
 
 
-def format_path(src: Path, fmt: str) -> str:
-    """Format path pattern"""
-    mtime = datetime.fromtimestamp(src.stat().st_mtime)
-    return fmt.format(
-        year=mtime.year,
-        month=str(mtime.month).zfill(2),
-        day=str(mtime.day).zfill(2),
-    )
-
-
 def copy_file(src: Path, dst: Path, dry_run: bool = False) -> None:
-    click.echo(f"copying {src.name} -> {dst}")
     if not dry_run:
         os.makedirs(dst.parent, exist_ok=True)
         if not os.path.exists(dst):
             shutil.copy(src, dst)
             os.utime(dst, times=file_times(src))
-            click.echo(f"{src.name} done.")
+            logging.info("%s -> %s is done", src.name, dst)
         else:
-            click.echo(f"{src.name} already exists.")
+            logging.info("%s -> %s is already exists", src.name, dst)
+
     else:
-        click.echo(f"{src.name} done.")
+        logging.info("%s -> %s is done", src.name, dst)
 
 
-@click.command()
-@click.argument("source", nargs=-1, type=click.Path(exists=True))
-@click.argument("dest", nargs=1, type=click.Path())
-@click.option("-c", "--config", type=click.Path(dir_okay=False))
-@click.option("-df", "--dest-format", default="{year}-{month}-{day}")
-@click.option("--dry-run", is_flag=True)
-@click.option("--threads", default=4)
-def main(source, dest, config, dest_format, dry_run, threads) -> None:
-    dst_path = Path(dest)
+def create_default_config(cfg: ConfigParser, section: str = "Default") -> None:
+    cfg.add_section(section)
+    cfg.set(section, "path", "")
+    cfg.set(section, "format", "")
 
-    cfg = ConfigParser()
-    if not config:
-        config = DEFAULT_CFG
 
-    config_exists = cfg.read(config)
+def main() -> None:
+    parser = argparse.ArgumentParser()
+    parser.add_argument("source", type=str)
+    parser.add_argument("dest", type=str)
+    parser.add_argument("-c", "--config")
+    parser.add_argument("--dry-run", action="store_true")
+    parser.add_argument("--threads", type=int, default=4)
 
-    if dry_run:
-        click.echo("Dry-run mode is ENABLED")
-    else:
-        os.makedirs(dest, exist_ok=True)
+    args = parser.parse_args()
+    time_start = time.perf_counter()
 
-    with ThreadPoolExecutor(threads) as t:
-        if config_exists:
-            click.echo(f"Config loaded: {config_exists}")
-
-            for section in cfg.sections():
-                folder = cfg[section]
-                if "path" not in folder:
-                    continue
+    if args.dry_run:
+        logging.info("Dry-run mode is ENABLED")
 
-                folder_format = folder.get("format", dest_format)
+    dst_path = Path(args.dest)
 
-                for src_folder in source:
-                    src_path = Path(src_folder) / folder["path"]
-                    click.echo(f"== {section} [{src_path}] ==")
-
-                    if not src_path.is_dir():
-                        click.echo(f"{src_path} not found!")
-                        continue
-
-                    for src_file in src_path.iterdir():
-                        if src_file.is_dir():
-                            continue
+    config = args.config
+    if not config:
+        config = DEFAULT_CONFIG_PATHS
 
-                        dst_file = dst_path / format_path(src_file, folder_format) / src_file.name
-                        t.submit(copy_file, src_file, dst_file, dry_run)
+    cfg = ConfigParser(interpolation=None)
 
-        else:
-            for src_folder in source:
-                src_path = Path(src_folder)
-                for src_file in src_path.iterdir():
-                    dst_file = dst_path / format_path(src_file, dest_format) / src_file.name
-                    t.submit(copy_file, src_file, dst_file, dry_run=dry_run)
+    if config_exists := cfg.read(config):
+        logging.info(f"Config loaded: {config_exists}")
+    else:
+        create_default_config(cfg)
+
+    threads = min(1, args.threads)
+    for section in cfg.sections():
+        folder = cfg[section]
+        if "path" not in folder:
+            continue
+
+        folder_fmt = folder.get("destination")
+
+        src_path = Path(args.source) / folder["path"]
+        logging.info("[%s] from %s", section, src_path)
+
+        if not src_path.is_dir():
+            logging.warning("%s not found!", src_path)
+            continue
+        with ThreadPoolExecutor(threads) as t:
+            for src_file in src_path.iterdir():
+                if src_file.is_dir():
+                    continue
+
+                src_file_mtime = datetime.fromtimestamp(src_file.stat().st_mtime)
+                dst_path_resolved = Path(src_file_mtime.strftime(str(dst_path)))
+                dst_file = dst_path_resolved / Path(src_file_mtime.strftime(str(folder_fmt))) / src_file.name
+                t.submit(copy_file, src_file, dst_file, args.dry_run)
 
-    if dry_run:
-        click.echo("Dry-run mode. NO CHANGES MADE")
+    if args.dry_run:
+        logging.info("Dry-run mode. NO CHANGES MADE")
 
-    click.echo("Done")
+    logging.debug("Done in %.02f sec", (time.perf_counter() - time_start) / 60)
 
 
 if __name__ == "__main__":
     main()
```

