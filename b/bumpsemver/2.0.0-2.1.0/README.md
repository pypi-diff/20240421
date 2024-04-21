# Comparing `tmp/bumpsemver-2.0.0.tar.gz` & `tmp/bumpsemver-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bumpsemver-2.0.0.tar", max compression
+gzip compressed data, was "bumpsemver-2.1.0.tar", max compression
```

## Comparing `bumpsemver-2.0.0.tar` & `bumpsemver-2.1.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1066 2024-04-19 19:52:02.757204 bumpsemver-2.0.0/LICENSE
--rw-r--r--   0        0        0    14259 2024-04-19 19:52:02.758334 bumpsemver-2.0.0/README.md
--rw-r--r--   0        0        0      108 2024-04-19 19:52:02.758812 bumpsemver-2.0.0/bumpsemver/__init__.py
--rw-r--r--   0        0        0       40 2024-04-19 19:52:02.759096 bumpsemver-2.0.0/bumpsemver/__main__.py
--rw-r--r--   0        0        0    20745 2024-04-19 19:52:02.759569 bumpsemver-2.0.0/bumpsemver/cli.py
--rw-r--r--   0        0        0     3289 2024-04-19 19:52:02.759928 bumpsemver-2.0.0/bumpsemver/exceptions.py
--rw-r--r--   0        0        0        2 2024-04-19 19:52:02.760205 bumpsemver-2.0.0/bumpsemver/files/__init__.py
--rw-r--r--   0        0        0     3461 2024-04-19 19:52:02.760539 bumpsemver-2.0.0/bumpsemver/files/base.py
--rw-r--r--   0        0        0     3629 2024-04-19 19:52:02.761016 bumpsemver-2.0.0/bumpsemver/files/json.py
--rw-r--r--   0        0        0     3338 2024-04-19 19:52:02.761192 bumpsemver-2.0.0/bumpsemver/files/text.py
--rw-r--r--   0        0        0     2895 2024-04-19 19:52:02.761346 bumpsemver-2.0.0/bumpsemver/files/toml.py
--rw-r--r--   0        0        0     3886 2024-04-19 19:52:02.761496 bumpsemver-2.0.0/bumpsemver/files/tomlpath.py
--rw-r--r--   0        0        0     4313 2024-04-19 19:52:02.761983 bumpsemver-2.0.0/bumpsemver/files/yaml.py
--rw-r--r--   0        0        0     1150 2024-04-19 19:52:02.762360 bumpsemver-2.0.0/bumpsemver/functions.py
--rw-r--r--   0        0        0     3541 2024-04-19 19:52:02.762704 bumpsemver-2.0.0/bumpsemver/git.py
--rw-r--r--   0        0        0      228 2024-04-19 19:52:02.763044 bumpsemver-2.0.0/bumpsemver/utils.py
--rw-r--r--   0        0        0     5034 2024-04-19 19:52:02.763428 bumpsemver-2.0.0/bumpsemver/version_part.py
--rw-r--r--   0        0        0     3669 2024-04-19 19:52:02.764207 bumpsemver-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    15453 1970-01-01 00:00:00.000000 bumpsemver-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-19 19:52:02.757204 bumpsemver-2.1.0/LICENSE
+-rw-r--r--   0        0        0    14130 2024-04-21 00:44:46.652107 bumpsemver-2.1.0/README.md
+-rw-r--r--   0        0        0      108 2024-04-21 00:44:45.959682 bumpsemver-2.1.0/bumpsemver/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-19 19:52:02.759096 bumpsemver-2.1.0/bumpsemver/__main__.py
+-rw-r--r--   0        0        0    15042 2024-04-21 00:37:46.138178 bumpsemver-2.1.0/bumpsemver/cli.py
+-rw-r--r--   0        0        0     7113 2024-04-21 00:37:46.138426 bumpsemver-2.1.0/bumpsemver/config.py
+-rw-r--r--   0        0        0     3654 2024-04-21 00:37:46.138635 bumpsemver-2.1.0/bumpsemver/discovery.py
+-rw-r--r--   0        0        0     4059 2024-04-21 00:37:46.139098 bumpsemver-2.1.0/bumpsemver/exceptions.py
+-rw-r--r--   0        0        0        2 2024-04-19 19:52:02.760205 bumpsemver-2.1.0/bumpsemver/files/__init__.py
+-rw-r--r--   0        0        0     3461 2024-04-19 19:52:02.760539 bumpsemver-2.1.0/bumpsemver/files/base.py
+-rw-r--r--   0        0        0     3629 2024-04-19 19:52:02.761016 bumpsemver-2.1.0/bumpsemver/files/json.py
+-rw-r--r--   0        0        0     3338 2024-04-19 19:52:02.761192 bumpsemver-2.1.0/bumpsemver/files/text.py
+-rw-r--r--   0        0        0     2895 2024-04-19 19:52:02.761346 bumpsemver-2.1.0/bumpsemver/files/toml.py
+-rw-r--r--   0        0        0     3886 2024-04-19 19:52:02.761496 bumpsemver-2.1.0/bumpsemver/files/tomlpath.py
+-rw-r--r--   0        0        0     4313 2024-04-21 00:19:36.521238 bumpsemver-2.1.0/bumpsemver/files/yaml.py
+-rw-r--r--   0        0        0     1150 2024-04-19 19:52:02.762360 bumpsemver-2.1.0/bumpsemver/functions.py
+-rw-r--r--   0        0        0     4121 2024-04-21 00:37:46.139584 bumpsemver-2.1.0/bumpsemver/git.py
+-rw-r--r--   0        0        0      228 2024-04-19 19:52:02.763044 bumpsemver-2.1.0/bumpsemver/utils.py
+-rw-r--r--   0        0        0     5034 2024-04-19 19:52:02.763428 bumpsemver-2.1.0/bumpsemver/version_part.py
+-rw-r--r--   0        0        0     3675 2024-04-21 00:44:45.982724 bumpsemver-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    15334 1970-01-01 00:00:00.000000 bumpsemver-2.1.0/PKG-INFO
```

### Comparing `bumpsemver-2.0.0/LICENSE` & `bumpsemver-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.0.0/README.md` & `bumpsemver-2.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [![image](https://img.shields.io/pypi/v/bumpsemver.svg)](https://pypi.org/project/bumpsemver/)
 [![image](https://img.shields.io/pypi/l/bumpsemver.svg)](https://pypi.org/project/bumpsemver/)
 [![image](https://img.shields.io/pypi/pyversions/bumpsemver.svg)](https://pypi.org/project/bumpsemver/)
 [![codecov](https://codecov.io/gh/zhaow-de/bumpsemver/graph/badge.svg?token=WP4O30YLO3)](https://codecov.io/gh/zhaow-de/bumpsemver)
 [![GitHub Actions](https://github.com/zhaow-de/bumpsemver/workflows/CI/badge.svg)](https://github.com/zhaow-de/bumpsemver/actions)
 
 
-Current version: **2.0.0**
+Current version: **v2.1.0**
 
 ## Table of contents
 
 <!--TOC-->
 
 - [Overview](#overview)
 - [Installation](#installation)
@@ -72,17 +72,14 @@
 `--allow-dirty`
 Normally, bumpsemver will abort if the working directory is dirty to avoid releasing not versioned files
 and/or overwriting unsaved changes. Use this option to override this check.
 
 `--verbose`
 Print useful information about the action details.
 
-`--alloy-checks`
-Perform some extra checks for a private project. Generally irrelevant to the common daily usages.
-
 `-h, --help`
 Print help and exit.
 
 ##### **`part`**    _**(required)**_
 
 The part of the version to increase. As we support semver only, the valid values include: `major`, `minor`, and `patch`.
 
@@ -203,21 +200,21 @@
 One config file can have zero or more file-specific config sections.
 The section name looks like `[bumpsemver:type:filename]`.
 It specifies the action to be done for a specific file.
 
 We do have the use case that one file has multiple places to change, a popular example is `package-lock.json`:
 ```json
 {
-  "name": "rcplus-app-cli",
+  "name": "app-cli",
   "version": "1.1.0",
   "lockfileVersion": 3,
   "requires": true,
   "packages": {
     "": {
-      "name": "rcplus-app-cli",
+      "name": "app-cli",
       "version": "1.1.0",
       "license": "SEE LICENSE IN LICENSE"
     }
   }
 }
 ```
 We need two config sections for the same file in this case, but INI format does not allow duplicated section names.
```

### Comparing `bumpsemver-2.0.0/bumpsemver/cli.py` & `bumpsemver-2.1.0/bumpsemver/cli.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,38 @@
 import argparse
-import io
 import logging
-import os
-import re
-import sre_constants
 import subprocess
 import sys
-from configparser import NoOptionError, RawConfigParser
 from datetime import datetime
-from typing import Dict, List, Tuple, Type
+from typing import Dict, Tuple
 
 from bumpsemver import __title__, __version__
+from bumpsemver.config import _determine_config_file, _load_configuration, _update_config_file
+from bumpsemver.discovery import discover_unmanaged_files
 from bumpsemver.exceptions import (
     CannotParseVersionError,
+    DiscoveryError,
+    FileTypeMismatchError,
     InvalidConfigSectionError,
     InvalidFileError,
     MixedNewLineError,
     MultiValuesMismatchError,
     PathNotFoundError,
     SingleValueMismatchError,
     VersionNotFoundError,
     WorkingDirectoryIsDirtyError,
 )
-from bumpsemver.files.base import FileTypeBase
-from bumpsemver.files.json import ConfiguredJSONFile
 from bumpsemver.files.text import ConfiguredPlainTextFile
-from bumpsemver.files.toml import ConfiguredTOMLFile
-from bumpsemver.files.yaml import ConfiguredYAMLFile
 from bumpsemver.git import Git
 from bumpsemver.utils import key_value_string
 from bumpsemver.version_part import VersionConfig
 
 python_version = sys.version.split("\n")[0].split(" ")[0]
 DESCRIPTION = f"{__title__}: v{__version__} (using Python v{python_version})"
 
-# detect either:
-# bumpsemver:toml:value
-# bumpsemver:toml(suffix):value
-# bumpsemver:toml ( suffix with spaces):value
-RE_CONFIG_SECTION = re.compile(
-    r"^bumpsemver:((?P<file_type>.+?)(\s*\(\s*(?P<file_suffix>[^):]+)\)?)?):(?P<value>.+)",
-)
-
 logger = logging.getLogger(__name__)
 time_context = {"now": datetime.now(), "utcnow": datetime.utcnow()}
 
 OPTIONAL_ARGUMENTS_THAT_TAKE_VALUES = [
     "--config-file",
     "--current-version",
     "--message",
@@ -53,36 +40,31 @@
     "--search",
     "--replace",
     "--tag-name",
     "--tag-message",
 ]
 
 
-class SectionConfig:
-    def __init__(self, handler: Type[FileTypeBase], xpath_supported: bool, props: Dict[str, str]):
-        self.handler = handler
-        self.xpath_supported = xpath_supported
-        self.props = props
-
-
 def main(original_args=None) -> None:
     try:
         #
         # determine configuration based on command-line arguments and on-disk configuration files
         args, known_args, root_parser, positionals = _parse_arguments_phase_1(original_args)
         _setup_logging(known_args.verbose)
         vcs_info = _determine_vcs_usability()
         defaults = _determine_current_version(vcs_info)
         explicit_config = None
         if hasattr(known_args, "config_file"):
             explicit_config = known_args.config_file
         config_file = _determine_config_file(explicit_config)
-        config, config_file_exists, config_newlines, files = _load_configuration(config_file, explicit_config, defaults)
+        config, config_file_exists, config_newlines, files, ignored_for_discovery = _load_configuration(
+            config_file, explicit_config, defaults
+        )
         known_args, parser2, remaining_argv = _parse_arguments_phase_2(args, defaults, root_parser)
-        version_config = _setup_version_config(known_args)
+        version_config = VersionConfig(search=known_args.search, replace=known_args.replace)
         current_version = version_config.parse(known_args.current_version)
         context = {**time_context, **vcs_info}
         #
         # calculate the desired new version
         new_version = _assemble_new_version(
             current_version, defaults, known_args.current_version, positionals, version_config
         )
@@ -90,19 +72,19 @@
         new_version = _parse_new_version(args, new_version, version_config)
 
         # replace the version in target files
         vcs = _determine_vcs_dirty(defaults)
         files.extend(
             ConfiguredPlainTextFile(file_name, version_config) for file_name in (file_names or positionals[1:])
         )
-        _check_files_contain_version(files, current_version, context)
-        _replace_version_in_files(files, current_version, new_version, args.dry_run, context)
-        config.remove_option("bumpsemver", "new_version")
 
-        # store the new version
+        # discover unmanaged files
+        discover_unmanaged_files([file.filename for file in files], ignored_for_discovery)
+
+        _replace_version_in_files(files, current_version, new_version, args.dry_run, context)
         _update_config_file(config, config_file, config_newlines, config_file_exists, args.new_version, args.dry_run)
 
         # commit and tag
         if vcs:
             context = _commit_to_vcs(files, config_file, config_file_exists, vcs, args, current_version, new_version)
             _tag_in_vcs(vcs, context, args)
 
@@ -114,28 +96,32 @@
         logger.error(f"FileNotFound. {exc!s}")
         sys.exit(2)
     except MixedNewLineError as exc:
         logger.warning(f"{exc.message}")
         sys.exit(3)
     except (
         CannotParseVersionError,
+        FileTypeMismatchError,
         InvalidConfigSectionError,
         InvalidFileError,
         MultiValuesMismatchError,
         PathNotFoundError,
         SingleValueMismatchError,
         VersionNotFoundError,
     ) as exc:
         logger.error(f"{exc.message}")
         sys.exit(4)
     except WorkingDirectoryIsDirtyError as exc:
         logger.error(f"{exc.message}\n\nUse --allow-dirty to override this if you know what you're doing.")
         sys.exit(5)
     except subprocess.CalledProcessError:
         sys.exit(10)
+    except DiscoveryError as exc:
+        logger.error(exc.message)
+        sys.exit(32)
     except Exception as exc:
         logger.error(f"Unexpected error occurred: {exc!s}")
         sys.exit(128)
 
 
 def split_args_in_optional_and_positional(args):
     # manually parsing positional arguments because with argparse we cannot mix positional and optional arguments
@@ -182,14 +168,20 @@
     root_parser.add_argument(
         "--allow-dirty",
         action="store_true",
         default=False,
         help="Don't abort if working directory is dirty",
         required=False,
     )
+    root_parser.add_argument(
+        "--version",
+        action="version",
+        version=f"%(prog)s {__version__}",
+        help="Print version and exit",
+    )
     known_args, _ = root_parser.parse_known_args(args)
     return args, known_args, root_parser, positionals
 
 
 def _setup_logging(verbose: int) -> None:
     try:
         log_level = [logging.WARNING, logging.INFO, logging.DEBUG][verbose]
@@ -211,129 +203,14 @@
 def _determine_current_version(vcs_info):
     defaults = {}
     if "current_version" in vcs_info:
         defaults["current_version"] = vcs_info["current_version"]
     return defaults
 
 
-def _determine_config_file(explicit_config):
-    if explicit_config:
-        return explicit_config
-    return ".bumpsemver.cfg"
-
-
-def _config_file_exists(config_file: str, explicit_config: bool) -> bool:
-    config_file_exists = os.path.exists(config_file)
-    if not config_file_exists:
-        message = f"Could not read config file at {config_file}"
-        if explicit_config:
-            raise argparse.ArgumentTypeError(message)
-        logger.info(message)
-        return False
-    return True
-
-
-def _check_section_config(section: str, acceptable_keys: List[str], actual_config: List[str]):
-    unknown_keys = [item for item in actual_config if item not in acceptable_keys]
-    if unknown_keys:
-        raise InvalidConfigSectionError(f"Invalid config file. Unknown keys {unknown_keys} in section '{section}'")
-
-
-def _parse_sections(config: RawConfigParser, defaults, sections):
-    file_types_config = {
-        "plaintext": SectionConfig(
-            ConfiguredPlainTextFile,
-            False,
-            {"search": "{current_version}", "replace": "{new_version}"},
-        ),
-        "file": SectionConfig(
-            ConfiguredPlainTextFile,
-            False,
-            {"search": "{current_version}", "replace": "{new_version}"},
-        ),
-        "json": SectionConfig(ConfiguredJSONFile, True, {"jsonpath": "version"}),
-        "yaml": SectionConfig(ConfiguredYAMLFile, True, {"yamlpath": "version"}),
-        "toml": SectionConfig(ConfiguredTOMLFile, True, {"tomlpath": "version"}),
-    }
-
-    files: List[FileTypeBase] = []
-
-    for section_name in sections:
-        parsed_section_header = RE_CONFIG_SECTION.match(section_name)
-
-        if not parsed_section_header:
-            continue
-
-        section_type = parsed_section_header.groupdict()
-        file_type = section_type.get("file_type")
-        filename = section_type.get("value")
-        section_props = dict(config.items(section_name))
-
-        if not [x for x in file_types_config.keys() if x == file_type]:
-            raise InvalidConfigSectionError(
-                f"Invalid config file. Unknown file type '{file_type}' in section '{section_name}'"
-            )
-
-        type_info = file_types_config.get(file_type)
-
-        _check_section_config(section_name, list(type_info.props.keys()), [*section_props])
-        if file_type == "file":
-            logger.warning("Using 'file' section type is deprecated, please use 'plaintext' instead.")
-
-        for k, v in type_info.props.items():
-            if k not in section_props:
-                section_props[k] = defaults.get(k, v)
-
-        if type_info.xpath_supported:
-            path_key = next(iter(type_info.props.keys()))
-            path = section_props.pop(path_key, None)
-            files.append(type_info.handler(filename, VersionConfig(**section_props), file_type, path))
-        else:
-            files.append(type_info.handler(filename, VersionConfig(**section_props)))
-
-    return files
-
-
-def _load_configuration(config_file, explicit_config, defaults):
-    # noinspection PyTypeChecker
-    config = RawConfigParser("")
-    # don't transform keys to lowercase (which would be the default)
-    config.optionxform = lambda option: option
-    config.add_section("bumpsemver")
-
-    if not _config_file_exists(config_file, explicit_config):
-        return config, False, None, []
-
-    logger.info(f"Reading config file {config_file}:")
-
-    with open(config_file, "rt", encoding="utf-8") as config_fp:
-        config_content = config_fp.read()
-        config_newlines = config_fp.newlines
-
-    logger.info(config_content)
-    config.read_string(config_content)
-    log_config = io.StringIO()
-    config.write(log_config)
-
-    if config.has_option("bumpsemver", "files"):
-        logger.warning("'files =' configuration will be deprecated, please use [bumpsemver:file:...]")
-
-    defaults.update(dict(config.items("bumpsemver")))
-
-    for bool_value_name in ("commit", "tag", "dry_run"):
-        try:
-            defaults[bool_value_name] = config.getboolean("bumpsemver", bool_value_name)
-        except NoOptionError:
-            pass  # no default value then
-
-    files = _parse_sections(config, defaults, config.sections())
-
-    return config, True, config_newlines, files
-
-
 def _parse_arguments_phase_2(args, defaults, root_parser):
     parser2 = argparse.ArgumentParser(prog="bumpsemver", add_help=False, parents=[root_parser])
     parser2.set_defaults(**defaults)
     parser2.add_argument(
         "--current-version",
         metavar="VERSION",
         help="Version that needs to be updated",
@@ -354,22 +231,14 @@
     known_args, remaining_argv = parser2.parse_known_args(args)
 
     defaults.update(vars(known_args))
 
     return known_args, parser2, remaining_argv
 
 
-def _setup_version_config(known_args):
-    try:
-        version_config = VersionConfig(search=known_args.search, replace=known_args.replace)
-    except sre_constants.error:
-        sys.exit(1)
-    return version_config
-
-
 def _assemble_new_version(current_version, defaults, arg_current_version, positionals, version_config):
     new_version = None
     if "new_version" not in defaults and arg_current_version:
         try:
             if current_version and positionals:
                 logger.info(f"Attempting to increment part '{positionals[0]}'")
                 new_version = current_version.bump(positionals[0], version_config.order())
@@ -502,49 +371,26 @@
         if defaults["allow_dirty"]:
             return None
         raise
 
     return Git
 
 
-def _check_files_contain_version(files, current_version, context: Dict[str, Tuple[str, datetime]]):
+def _replace_version_in_files(files, current_version, new_version, dry_run, context: Dict[str, Tuple[str, datetime]]):
+    #
     # make sure files exist and contain version string
     logger.info(f"Asserting files {', '.join([str(f) for f in files])} contain the version string...")
     for file_item in files:
         file_item.should_contain_version(current_version, context)
-
-
-def _replace_version_in_files(files, current_version, new_version, dry_run, context: Dict[str, Tuple[str, datetime]]):
+    #
     # change version string in files
     for file_item in files:
         file_item.replace(current_version, new_version, context, dry_run)
 
 
-def _update_config_file(config, config_file, config_newlines, config_file_exists, new_version, dry_run):
-    config.set("bumpsemver", "current_version", new_version)
-    new_config = io.StringIO()
-    try:
-        write_to_config_file = (not dry_run) and config_file_exists
-
-        logger.info(f"{'Would write' if not write_to_config_file else 'Writing'} to config file {config_file}:")
-
-        config.write(new_config)
-        logger.info(new_config.getvalue())
-
-        if write_to_config_file:
-            with open(config_file, "wt", encoding="utf-8", newline=config_newlines) as config_fp:
-                config_fp.write(new_config.getvalue().strip() + "\n")
-
-    except UnicodeEncodeError:
-        logger.warning(
-            "Unable to write UTF-8 to config file, because of an old configparser version. "
-            "Update with `pip install --upgrade configparser`."
-        )
-
-
 def _commit_to_vcs(files, config_file, config_file_exists, vcs, args, current_version, new_version):
     commit_files = [f.filename for f in files]
     if config_file_exists:
         commit_files.append(config_file)
     assert vcs.is_usable(), f"Did find '{vcs.__name__}' unusable, unable to commit."
     do_commit = args.commit and not args.dry_run
     logger.info(f"{'Would prepare' if not do_commit else 'Preparing'} {vcs.__name__} commit")
```

### Comparing `bumpsemver-2.0.0/bumpsemver/exceptions.py` & `bumpsemver-2.1.0/bumpsemver/exceptions.py`

 * *Files 23% similar despite different names*

```diff
@@ -24,71 +24,92 @@
     def __init__(self):
         message = "The specific version could not be parsed with semver scheme. Please double check the config file"
         super().__init__(message)
         self.message = message
 
 
 class MixedNewLineError(BumpVersionError):
-    def __init__(self, path: str, file_new_lines: Tuple[str, ...]):
-        message = f"File {path} has mixed newline characters: {file_new_lines}"
+    def __init__(self, filename: str, file_new_lines: Tuple[str, ...]):
+        message = f"File {filename} has mixed newline characters: {file_new_lines}"
         super().__init__(message)
         self.message = message
 
 
 # NOTE: this exception is for plain text file only.
 # because for plain text file we do not have the concept of XPATH-like locator,
 # there is either a match or not.
 # we cannot distinguish the mismatch cases like json, yaml, toml
 # with InvalidFileError, PathNotFoundError, SingleValueMismatchError, and MultiValuesMismatchError
 class VersionNotFoundError(BumpVersionError):
-    def __init__(self, search_expression: str, path: str):
-        message = f"Did not find '{search_expression}' in plaintext file: '{path}'"
+    def __init__(self, search_expression: str, filename: str):
+        message = f"Did not find '{search_expression}' in plaintext file: '{filename}'"
         super().__init__(message)
         self.message = message
 
 
 class InvalidFileError(BumpVersionError):
-    def __init__(self, path: str, file_type: str):
-        message = f"File {path} cannot be parsed as a valid {file_type} file"
+    def __init__(self, filename: str, file_type: str):
+        message = f"File {filename} cannot be parsed as a valid {file_type} file"
         super().__init__(message)
         self.message = message
 
 
 class PathNotFoundError(BumpVersionError):
-    def __init__(self, selector: str, file_type: str, path: str):
-        message = f"Selector '{selector}' does not lead to a valid property in {file_type} file {path}"
+    def __init__(self, selector: str, file_type: str, filename: str):
+        message = f"Selector '{selector}' does not lead to a valid property in {file_type} file {filename}"
         super().__init__(message)
         self.message = message
 
 
 class SingleValueMismatchError(BumpVersionError):
     def __init__(
         self,
         selector: str,
         file_type: str,
-        path: str,
+        filename: str,
         actual_value: Union[str, int, float, bool],
         expected_value: Union[str, int, float, bool],
     ):
         message = (
             f"Selector '{selector}' finds value '{actual_value}' "
-            f"mismatches with the expectation '{expected_value}' in {file_type} file {path}"
+            f"mismatches with the expectation '{expected_value}' in {file_type} file {filename}"
         )
         super().__init__(message)
         self.message = message
 
 
 class MultiValuesMismatchError(BumpVersionError):
     def __init__(
         self,
         selector: str,
         file_type: str,
-        path: str,
+        filename: str,
         actual_value: List[Union[str, int, float, bool]],
         expected_value: Union[str, int, float, bool],
     ):
         message = (
-            f"Selector '{selector}' finds list of values {actual_value} "
-            f"with one more more elements mismatch with the expectation '{expected_value}' in {file_type} file {path}"
+            f"Selector '{selector}' finds list of values {actual_value} with one more more elements "
+            f"mismatch with the expectation '{expected_value}' in {file_type} file {filename}"
+        )
+        super().__init__(message)
+        self.message = message
+
+
+class FileTypeMismatchError(BumpVersionError):
+    def __init__(self, file_type: str, file_type_expected: str, filename: str):
+        message = (
+            f"Wrong file type '{file_type}' specified for file {filename}, "
+            f"please use '{file_type_expected}' instead"
+        )
+        super().__init__(message)
+        self.message = message
+
+
+class DiscoveryError(BumpVersionError):
+    def __init__(self, issues: List[str]):
+        issues_str = "\n  - ".join(issues)
+        message = (
+            f"Discovered unmanaged files. "
+            f"Please add them to the config file for versioning or to ignore:\n  - {issues_str}"
         )
         super().__init__(message)
         self.message = message
```

### Comparing `bumpsemver-2.0.0/bumpsemver/files/base.py` & `bumpsemver-2.1.0/bumpsemver/files/base.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.0.0/bumpsemver/files/json.py` & `bumpsemver-2.1.0/bumpsemver/files/json.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.0.0/bumpsemver/files/text.py` & `bumpsemver-2.1.0/bumpsemver/files/text.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.0.0/bumpsemver/files/toml.py` & `bumpsemver-2.1.0/bumpsemver/files/toml.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.0.0/bumpsemver/files/tomlpath.py` & `bumpsemver-2.1.0/bumpsemver/files/tomlpath.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.0.0/bumpsemver/files/yaml.py` & `bumpsemver-2.1.0/bumpsemver/files/yaml.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.0.0/bumpsemver/functions.py` & `bumpsemver-2.1.0/bumpsemver/functions.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.0.0/bumpsemver/git.py` & `bumpsemver-2.1.0/bumpsemver/git.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import errno
 import logging
 import os
 import subprocess
 from pathlib import Path
 from tempfile import NamedTemporaryFile
-from typing import Optional, Union
+from typing import List, Optional, Union
 
 from bumpsemver.exceptions import WorkingDirectoryIsDirtyError
 
 logger = logging.getLogger(__name__)
 
 
 class Git:
@@ -96,15 +96,28 @@
 
     @classmethod
     def tag(cls, name: str, sign: bool = False, message: Optional[str] = None) -> None:
         """
         Create a tag of the new_version in Git.
 
         If only name is given, bumpversion uses a lightweight tag.
-        Otherwise, it utilizes an annotated tag.
+        Otherwise, it uses an annotated tag.
         """
         command = ["git", "tag", name]
         if sign:
             command += ["--sign"]
         if message:
             command += ["--message", message]
         subprocess.check_output(command)
+
+    @classmethod
+    def list_files(cls) -> List[str]:
+        try:
+            return [line.decode().strip() for line in subprocess.check_output(["git", "ls-files"]).splitlines()]
+        except (subprocess.CalledProcessError, FileNotFoundError):
+            logger.warning("'git ls-files' failed. Listing files without respecting '.gitignore'")
+            path = os.getcwd()
+            return [
+                os.path.relpath(str(os.path.join(dir_path, f)))
+                for (dir_path, dirs, filenames) in os.walk(path)
+                for f in filenames
+            ]
```

### Comparing `bumpsemver-2.0.0/bumpsemver/version_part.py` & `bumpsemver-2.1.0/bumpsemver/version_part.py`

 * *Files identical despite different names*

### Comparing `bumpsemver-2.0.0/pyproject.toml` & `bumpsemver-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -37,23 +37,23 @@
 [tool.ruff.lint.flake8-quotes]
 docstring-quotes = "double"
 
 [tool.ruff.lint.per-file-ignores]
 "tests/*" = ["S101", "PLR0913", "PLR0915", "PGH003", "ANN001", "ANN202", "ANN201", "PLR0912", "TRY301", "PLW0603", "PLR2004", "ANN101", "S106", "TRY201", "ANN003", "ANN002", "S105", "TRY003"]
 
 [tool.ruff.lint.mccabe]
-# Unlike Flake8, default to a complexity level of 10.
-max-complexity = 10
+# Unlike Flake8, default to a complexity level of 15.
+max-complexity = 15
 
 [tool.ruff.lint.isort]
 order-by-type = true
 
 [tool.poetry]
 name = "bumpsemver"
-version = "2.0.0"
+version = "2.1.0"
 description = "Bump semver for git repos with a single command"
 readme = "README.md"
 authors = [ "Zhao Wang <zhaow.km@gmail.com>" ]
 license = "MIT"
 repository = "https://github.com/zhaow-de/bumpsemver"
 classifiers = [
     'Development Status :: 4 - Beta',
@@ -76,15 +76,15 @@
 bumpsemver = "bumpsemver.cli:main"
 
 [tool.poetry.dependencies]
 python = ">= 3.10,< 4"
 "ruamel.yaml" = "*"  # we prefer pyyaml, but ruamel.yaml is being used by yamlpath. no reason to have both.
 jsonpath-ng = "*"
 tomlkit = "*"
-yamlpath = "*"
+yamlpath = ">=3.4.1"
 
 [tool.poetry.group.dev.dependencies]
 coverage = "*"
 generate-changelog = ">=0.7.6"
 git-fame = ">=1.12.2"
 mypy = "*"
 pre-commit = "*"
```

### Comparing `bumpsemver-2.0.0/PKG-INFO` & `bumpsemver-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bumpsemver
-Version: 2.0.0
+Version: 2.1.0
 Summary: Bump semver for git repos with a single command
 Home-page: https://github.com/zhaow-de/bumpsemver
 License: MIT
 Keywords: bumpsemver,semver,version,release
 Author: Zhao Wang
 Author-email: zhaow.km@gmail.com
 Requires-Python: >=3.10,<4
@@ -21,28 +21,28 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: System :: Software Distribution
 Requires-Dist: jsonpath-ng
 Requires-Dist: ruamel.yaml
 Requires-Dist: tomlkit
-Requires-Dist: yamlpath
+Requires-Dist: yamlpath (>=3.4.1)
 Project-URL: Repository, https://github.com/zhaow-de/bumpsemver
 Description-Content-Type: text/markdown
 
 # bumpsemver
 
 [![image](https://img.shields.io/pypi/v/bumpsemver.svg)](https://pypi.org/project/bumpsemver/)
 [![image](https://img.shields.io/pypi/l/bumpsemver.svg)](https://pypi.org/project/bumpsemver/)
 [![image](https://img.shields.io/pypi/pyversions/bumpsemver.svg)](https://pypi.org/project/bumpsemver/)
 [![codecov](https://codecov.io/gh/zhaow-de/bumpsemver/graph/badge.svg?token=WP4O30YLO3)](https://codecov.io/gh/zhaow-de/bumpsemver)
 [![GitHub Actions](https://github.com/zhaow-de/bumpsemver/workflows/CI/badge.svg)](https://github.com/zhaow-de/bumpsemver/actions)
 
 
-Current version: **2.0.0**
+Current version: **v2.1.0**
 
 ## Table of contents
 
 <!--TOC-->
 
 - [Overview](#overview)
 - [Installation](#installation)
@@ -103,17 +103,14 @@
 `--allow-dirty`
 Normally, bumpsemver will abort if the working directory is dirty to avoid releasing not versioned files
 and/or overwriting unsaved changes. Use this option to override this check.
 
 `--verbose`
 Print useful information about the action details.
 
-`--alloy-checks`
-Perform some extra checks for a private project. Generally irrelevant to the common daily usages.
-
 `-h, --help`
 Print help and exit.
 
 ##### **`part`**    _**(required)**_
 
 The part of the version to increase. As we support semver only, the valid values include: `major`, `minor`, and `patch`.
 
@@ -234,21 +231,21 @@
 One config file can have zero or more file-specific config sections.
 The section name looks like `[bumpsemver:type:filename]`.
 It specifies the action to be done for a specific file.
 
 We do have the use case that one file has multiple places to change, a popular example is `package-lock.json`:
 ```json
 {
-  "name": "rcplus-app-cli",
+  "name": "app-cli",
   "version": "1.1.0",
   "lockfileVersion": 3,
   "requires": true,
   "packages": {
     "": {
-      "name": "rcplus-app-cli",
+      "name": "app-cli",
       "version": "1.1.0",
       "license": "SEE LICENSE IN LICENSE"
     }
   }
 }
 ```
 We need two config sections for the same file in this case, but INI format does not allow duplicated section names.
```

