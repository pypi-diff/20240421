# Comparing `tmp/envix-0.1.1.tar.gz` & `tmp/envix-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envix-0.1.1.tar", max compression
+gzip compressed data, was "envix-0.2.0.tar", max compression
```

## Comparing `envix-0.1.1.tar` & `envix-0.2.0.tar`

### file list

```diff
@@ -1,29 +1,33 @@
--rw-r--r--   0        0        0      297 2024-04-16 16:31:25.690912 envix-0.1.1/README.md
--rw-r--r--   0        0        0      937 2024-04-16 16:31:25.690912 envix-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       78 2024-04-16 16:31:25.690912 envix-0.1.1/src/envix/__init__.py
--rw-r--r--   0        0        0       28 2024-04-16 16:31:25.690912 envix-0.1.1/src/envix/cli/__init__.py
--rw-r--r--   0        0        0      154 2024-04-16 16:31:25.690912 envix-0.1.1/src/envix/cli/__main__.py
--rw-r--r--   0        0        0     3081 2024-04-16 16:31:25.690912 envix-0.1.1/src/envix/cli/app.py
--rw-r--r--   0        0        0        0 2024-04-16 16:31:25.690912 envix-0.1.1/src/envix/cli/commands/__init__.py
--rw-r--r--   0        0        0      765 2024-04-16 16:31:25.690912 envix-0.1.1/src/envix/cli/commands/config.py
--rw-r--r--   0        0        0     1162 2024-04-16 16:31:25.690912 envix-0.1.1/src/envix/cli/commands/config_schema.py
--rw-r--r--   0        0        0     2544 2024-04-16 16:31:25.690912 envix-0.1.1/src/envix/cli/commands/export.py
--rw-r--r--   0        0        0     1745 2024-04-16 16:31:25.690912 envix-0.1.1/src/envix/cli/commands/inject.py
--rw-r--r--   0        0        0      196 2024-04-16 16:31:25.690912 envix-0.1.1/src/envix/cli/default.py
--rw-r--r--   0        0        0      640 2024-04-16 16:31:25.690912 envix-0.1.1/src/envix/cli/field.py
--rw-r--r--   0        0        0       59 2024-04-16 16:31:25.690912 envix-0.1.1/src/envix/config/__init__.py
--rw-r--r--   0        0        0     1649 2024-04-16 16:31:25.690912 envix-0.1.1/src/envix/config/config.py
--rw-r--r--   0        0        0        0 2024-04-16 16:31:25.690912 envix-0.1.1/src/envix/config/v1/__init__.py
--rw-r--r--   0        0        0      233 2024-04-16 16:31:25.690912 envix-0.1.1/src/envix/config/v1/config.py
--rw-r--r--   0        0        0      230 2024-04-16 16:31:25.690912 envix-0.1.1/src/envix/config/v1/envix_v1.py
--rw-r--r--   0        0        0      243 2024-04-16 16:31:25.690912 envix-0.1.1/src/envix/config/v1/envs/__init__.py
--rw-r--r--   0        0        0      250 2024-04-16 16:31:25.690912 envix-0.1.1/src/envix/config/v1/envs/_common.py
--rw-r--r--   0        0        0     1619 2024-04-16 16:31:25.694912 envix-0.1.1/src/envix/config/v1/envs/google_cloud_secret_manager_envs_v1.py
--rw-r--r--   0        0        0     1381 2024-04-16 16:31:25.694912 envix-0.1.1/src/envix/config/v1/envs/local_envs_v1.py
--rw-r--r--   0        0        0      790 2024-04-16 16:31:25.694912 envix-0.1.1/src/envix/config/v1/envs/raw_envs_v1.py
--rw-r--r--   0        0        0     1555 2024-04-16 16:31:25.694912 envix-0.1.1/src/envix/exception.py
--rw-r--r--   0        0        0      799 2024-04-16 16:31:25.694912 envix-0.1.1/src/envix/loader/__init__.py
--rw-r--r--   0        0        0     2969 2024-04-16 16:31:25.694912 envix-0.1.1/src/envix/loader/v1_loader.py
--rw-r--r--   0        0        0       71 2024-04-16 16:31:25.694912 envix-0.1.1/src/envix/pattern.py
--rw-r--r--   0        0        0       63 2024-04-16 16:31:25.694912 envix-0.1.1/src/envix/types.py
--rw-r--r--   0        0        0      885 1970-01-01 00:00:00.000000 envix-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      360 2024-04-21 16:39:15.892651 envix-0.2.0/README.md
+-rw-r--r--   0        0        0      937 2024-04-21 16:39:15.896651 envix-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/cli/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/cli/__main__.py
+-rw-r--r--   0        0        0     2908 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/cli/app.py
+-rw-r--r--   0        0        0        0 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/cli/commands/__init__.py
+-rw-r--r--   0        0        0      986 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/cli/commands/config.py
+-rw-r--r--   0        0        0     1436 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/cli/commands/config_edit.py
+-rw-r--r--   0        0        0      886 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/cli/commands/config_list.py
+-rw-r--r--   0        0        0     1162 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/cli/commands/config_schema.py
+-rw-r--r--   0        0        0     3105 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/cli/commands/export.py
+-rw-r--r--   0        0        0     2148 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/cli/commands/inject.py
+-rw-r--r--   0        0        0      196 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/cli/default.py
+-rw-r--r--   0        0        0      640 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/cli/field.py
+-rw-r--r--   0        0        0       59 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/config/__init__.py
+-rw-r--r--   0        0        0     2056 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/config/config.py
+-rw-r--r--   0        0        0        0 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/config/v1/__init__.py
+-rw-r--r--   0        0        0      233 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/config/v1/config.py
+-rw-r--r--   0        0        0      230 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/config/v1/envix_v1.py
+-rw-r--r--   0        0        0      243 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/config/v1/envs/__init__.py
+-rw-r--r--   0        0        0      250 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/config/v1/envs/_common.py
+-rw-r--r--   0        0        0     1619 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/config/v1/envs/google_cloud_secret_manager_envs_v1.py
+-rw-r--r--   0        0        0     1381 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/config/v1/envs/local_envs_v1.py
+-rw-r--r--   0        0        0      790 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/config/v1/envs/raw_envs_v1.py
+-rw-r--r--   0        0        0      118 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/envname.py
+-rw-r--r--   0        0        0     1555 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/exception.py
+-rw-r--r--   0        0        0      799 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/loader/__init__.py
+-rw-r--r--   0        0        0     2969 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/loader/v1_loader.py
+-rw-r--r--   0        0        0     1167 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/path.py
+-rw-r--r--   0        0        0       71 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/pattern.py
+-rw-r--r--   0        0        0       63 2024-04-21 16:39:15.896651 envix-0.2.0/src/envix/types.py
+-rw-r--r--   0        0        0      948 1970-01-01 00:00:00.000000 envix-0.2.0/PKG-INFO
```

### Comparing `envix-0.1.1/pyproject.toml` & `envix-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "envix"
-version = "0.1.1"
+version = "0.2.0"
 description = "convinient secret manager."
 authors = ["yassun7010 <yassun7010@outlook.com>"]
 readme = "README.md"
 packages = [{ include = "envix", from = "src" }]
 
 [tool.poetry.scripts]
 envix = "envix.cli.__main__:main"
```

### Comparing `envix-0.1.1/src/envix/cli/app.py` & `envix-0.2.0/src/envix/cli/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
 import sys
 from argparse import ArgumentParser, BooleanOptionalAction
-from logging import getLogger
 from typing import NoReturn
 
 from rich.console import Console as RichConsole
 from rich.logging import RichHandler
 from rich_argparse import ArgumentDefaultsRichHelpFormatter
 
 import envix
-from envix.cli.commands import config, export, inject
+
+from .commands import config, export, inject
 
 logger = logging.getLogger(__name__)
 
 
 class EnvixArgumentParser(ArgumentParser):
     def error(self, message: str) -> NoReturn:
         self.print_usage(sys.stderr)
@@ -37,16 +37,14 @@
                         show_path=False,
                         rich_tracebacks=True,
                         markup=True,
                     )
                 ],
             )
             logging.root.setLevel(logging.DEBUG if verbose else logging.INFO)
-            for mod in ("google", "snowflake"):
-                getLogger(mod).setLevel(logging.DEBUG if verbose else logging.WARNING)
 
             formatter_class = ArgumentDefaultsRichHelpFormatter
             formatter_class.styles["argparse.default"] = "dark_orange"
 
             parser = EnvixArgumentParser(
                 prog="envix",
                 description="A tool to retrieve environment variables from the Secret Manager and execute commands.",
@@ -67,16 +65,16 @@
 
             subparser = parser.add_subparsers(
                 title="commands",
                 metavar="COMMAND",
             )
 
             inject.add_subparser(subparser, formatter_class=parser.formatter_class)
-            config.add_subparser(subparser, formatter_class=parser.formatter_class)
             export.add_subparser(subparser, formatter_class=parser.formatter_class)
+            config.add_subparser(subparser, formatter_class=parser.formatter_class)
 
             parser.set_defaults(handler=lambda _: parser.print_help())
 
             space = parser.parse_args(args)
 
             if hasattr(space, "handler"):
                 space.handler(space)
```

### Comparing `envix-0.1.1/src/envix/cli/commands/config.py` & `envix-0.2.0/src/envix/cli/commands/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from argparse import ArgumentParser, _SubParsersAction
 from typing import Any, cast
 
 from pydantic import BaseModel
 
-from . import config_schema
+from envix.cli.commands import config_edit
+
+from . import config_list, config_schema
 
 
 class Args(BaseModel):
     commands: list[str]
 
 
 def add_subparser(subparsers: "_SubParsersAction[Any]", **kwargs: Any) -> None:
@@ -24,10 +26,12 @@
     )
 
     subparsers = parser.add_subparsers(
         title="commands",
         metavar="COMMAND",
     )
 
+    config_list.add_subparser(subparsers, formatter_class=parser.formatter_class)
+    config_edit.add_subparser(subparsers, formatter_class=parser.formatter_class)
     config_schema.add_subparser(subparsers, formatter_class=parser.formatter_class)
 
     parser.set_defaults(handler=lambda _: parser.print_help())
```

### Comparing `envix-0.1.1/src/envix/cli/commands/config_schema.py` & `envix-0.2.0/src/envix/cli/commands/config_schema.py`

 * *Files identical despite different names*

### Comparing `envix-0.1.1/src/envix/cli/commands/export.py` & `envix-0.2.0/src/envix/cli/commands/export.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,25 +6,23 @@
 from shlex import quote
 from typing import Annotated, Any, Literal, assert_never, cast, get_args
 
 from pydantic import BaseModel, ConfigDict
 
 from envix.cli.default import AUTO_SEARCH, STDOUT
 from envix.cli.field import ConfigFileValidator, OutputFileValidator
-from envix.config.config import Config
-from envix.exception import EnvixLoadEnvsError
-from envix.loader import load_envs
 
 OutputFormat = Literal["dotenv", "json"]
 
 
 class Args(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
 
     config_file: Annotated[Path | None, ConfigFileValidator]
+    config_name: list[str] | None
     output_file: Annotated[TextIOWrapper | None, OutputFileValidator]
     format: OutputFormat
 
 
 def add_subparser(subparsers: "_SubParsersAction[Any]", **kwargs: Any) -> None:
     help = "Output environment variables to a file."
 
@@ -36,21 +34,31 @@
             help=help,
             **kwargs,
         ),
     )
 
     parser.add_argument(
         "--config-file",
+        "--file",
         metavar="CONFIG_FILE",
         help="config file path.",
         type=Path,
         default=AUTO_SEARCH,
     )
 
     parser.add_argument(
+        "--config-name",
+        "--config",
+        metavar="CONFIG_NAME",
+        help="user registered setting name.",
+        type=str,
+        nargs="*",
+    )
+
+    parser.add_argument(
         "--output-file",
         "-o",
         help="output file path.",
         type=FileType("w"),
         default=STDOUT,
     )
 
@@ -61,35 +69,50 @@
         default="dotenv",
     )
 
     parser.set_defaults(handler=lambda space: export_command(Args(**vars(space))))
 
 
 def export_command(args: Args) -> None:
-    config = Config.load(args.config_file)
-    secrets, errors = asyncio.run(load_envs(config))
-    if errors:
-        raise EnvixLoadEnvsError(errors)
+    from envix.config.config import load_configs
+    from envix.exception import (
+        EnvixEnvInjectionError,
+        EnvixLoadEnvsError,
+    )
+    from envix.loader import load_envs
+    from envix.types import Secrets
+
+    total_secrets: Secrets = {}
+    total_errors: list[EnvixEnvInjectionError] = []
+
+    for config in load_configs(args.config_file, args.config_name):
+        secrets, errors = asyncio.run(load_envs(config))
+
+        total_secrets.update(secrets)
+        total_errors.extend(errors)
+
+    if total_errors:
+        raise EnvixLoadEnvsError(total_errors)
 
     match args.format:
         case "dotenv":
             print(
                 "\n".join(
                     f"{envname}={quote(secret.get_secret_value())}"
-                    for envname, secret in secrets.items()
+                    for envname, secret in total_secrets.items()
                 ),
                 file=args.output_file,
             )
 
         case "json":
             print(
                 json.dumps(
                     {
                         envname: secret.get_secret_value()
-                        for envname, secret in secrets.items()
+                        for envname, secret in total_secrets.items()
                     }
                 ),
                 file=args.output_file,
             )
 
         case _:
             assert_never(args.format)
```

### Comparing `envix-0.1.1/src/envix/cli/commands/inject.py` & `envix-0.2.0/src/envix/cli/commands/inject.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from envix.cli.field import ConfigFileValidator
 
 
 class Args(BaseModel):
     command: str
     args: list[str]
     config_file: Annotated[Path | None, ConfigFileValidator]
+    config_name: list[str] | None
     clear_environments: bool
 
 
 def add_subparser(subparsers: "_SubParsersAction[Any]", **kwargs: Any) -> None:
     help = "Inject environment variables and execute the command."
 
     parser = cast(
@@ -33,42 +34,55 @@
         metavar="COMMAND",
     )
 
     parser.add_argument("args", metavar="ARGS", nargs="*")
 
     parser.add_argument(
         "--config-file",
+        "--file",
         metavar="CONFIG_FILE",
         help="config file path.",
         type=Path,
         default=None,
     )
 
     parser.add_argument(
+        "--config-name",
+        "--config",
+        metavar="CONFIG_NAME",
+        help="user registered setting name.",
+        type=str,
+        nargs="*",
+    )
+
+    parser.add_argument(
         "--clear-environments",
         action="store_true",
         help="Running commands with no environment variables set.",
         default=False,
     )
 
     parser.set_defaults(handler=lambda space: inject_command(Args(**vars(space))))
 
 
 def inject_command(args: Args) -> None:
     import asyncio
     import subprocess
 
-    from envix.config.config import Config
-    from envix.exception import EnvixLoadEnvsError
+    from envix.config.config import load_configs
+    from envix.exception import EnvixEnvInjectionError, EnvixLoadEnvsError
     from envix.loader import load_envs
 
-    config = Config.load(args.config_file)
+    total_errors: list[EnvixEnvInjectionError] = []
 
     if args.clear_environments:
         os.environ.clear()
 
-    _, errors = asyncio.run(load_envs(config))
+    for config in load_configs(args.config_file, args.config_name):
+        _, errors = asyncio.run(load_envs(config))
+
+        total_errors.extend(errors)
 
-    if errors:
-        raise EnvixLoadEnvsError(errors)
+    if total_errors:
+        raise EnvixLoadEnvsError(total_errors)
 
     subprocess.call([args.command] + args.args)
```

### Comparing `envix-0.1.1/src/envix/cli/field.py` & `envix-0.2.0/src/envix/cli/field.py`

 * *Files identical despite different names*

### Comparing `envix-0.1.1/src/envix/config/config.py` & `envix-0.2.0/src/envix/config/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 from logging import getLogger
 from pathlib import Path
 from typing import Self
 
 from pydantic import RootModel
 
 from envix.exception import EnvixConfigFileExtensionError, EnvixConfigFileNotFound
+from envix.path import get_user_config_path
 
 from .v1.config import ConfigV1
 
 logger = getLogger(__name__)
 
 
 class Config(RootModel):
     root: ConfigV1
 
     @classmethod
     def load(cls, filepath: Path | None) -> Self:
         import tomllib
 
         if not (filepath := filepath or _find_config_file()):
-            raise EnvixConfigFileNotFound(Path(os.getcwd()))
+            raise EnvixConfigFileNotFound(Path(os.getcwd()).joinpath("envix.yml"))
 
         if not filepath.exists():
             raise EnvixConfigFileNotFound(filepath)
 
         match filepath.suffix:
             case ".toml":
                 with open(filepath, "rb") as f:
@@ -49,12 +50,26 @@
 def _find_config_file() -> Path | None:
     import os
     from pathlib import Path
 
     cwd = Path(os.getcwd())
 
     for directory in (cwd, *cwd.parents):
-        for filename in ("envix.toml", "envix.yaml", "envix.yml", "envix.json"):
+        for filename in ("envix.yml", "envix.yaml", "envix.toml", "envix.json"):
             config_filepath = directory / filename
             if config_filepath.exists():
                 logger.debug(f"Found config file: {config_filepath}")
                 return config_filepath
+
+
+def load_configs(
+    config_file: Path | None, config_names: list[str] | None = None
+) -> list[Config]:
+    configs = [
+        Config.load(get_user_config_path(config_name))
+        for config_name in config_names or []
+    ]
+
+    if not configs or config_file:
+        configs = [Config.load(config_file)] + configs
+
+    return configs
```

### Comparing `envix-0.1.1/src/envix/config/v1/envs/google_cloud_secret_manager_envs_v1.py` & `envix-0.2.0/src/envix/config/v1/envs/google_cloud_secret_manager_envs_v1.py`

 * *Files identical despite different names*

### Comparing `envix-0.1.1/src/envix/config/v1/envs/local_envs_v1.py` & `envix-0.2.0/src/envix/config/v1/envs/local_envs_v1.py`

 * *Files identical despite different names*

### Comparing `envix-0.1.1/src/envix/config/v1/envs/raw_envs_v1.py` & `envix-0.2.0/src/envix/config/v1/envs/raw_envs_v1.py`

 * *Files identical despite different names*

### Comparing `envix-0.1.1/src/envix/exception.py` & `envix-0.2.0/src/envix/exception.py`

 * *Files identical despite different names*

### Comparing `envix-0.1.1/src/envix/loader/__init__.py` & `envix-0.2.0/src/envix/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `envix-0.1.1/src/envix/loader/v1_loader.py` & `envix-0.2.0/src/envix/loader/v1_loader.py`

 * *Files identical despite different names*

### Comparing `envix-0.1.1/PKG-INFO` & `envix-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: envix
-Version: 0.1.1
+Version: 0.2.0
 Summary: convinient secret manager.
 Author: yassun7010
 Author-email: yassun7010@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -15,14 +15,18 @@
 Requires-Dist: rich-argparse (>=1.4.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Simple Secret Injector CLI tool
 
 [![pypi package](https://badge.fury.io/py/envix.svg)](https://pypi.org/project/envix)
 
+## Support Envs Types
+- Raw
+- Local
+- GoogleCloudSecretManager
 
 ## Usage
 
 ```sh
 cat > envix.toml <<EOF
 [envix]
 version = 1
```

