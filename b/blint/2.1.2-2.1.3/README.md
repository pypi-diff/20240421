# Comparing `tmp/blint-2.1.2.tar.gz` & `tmp/blint-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blint-2.1.2.tar", max compression
+gzip compressed data, was "blint-2.1.3.tar", max compression
```

## Comparing `blint-2.1.2.tar` & `blint-2.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1068 2024-04-13 14:33:01.619021 blint-2.1.2/LICENSE
--rw-r--r--   0        0        0     6240 2024-04-13 14:33:01.619021 blint-2.1.2/README.md
--rw-r--r--   0        0        0        0 2024-04-13 14:33:01.623021 blint-2.1.2/blint/__init__.py
--rw-r--r--   0        0        0    24122 2024-04-13 14:33:01.623021 blint-2.1.2/blint/analysis.py
--rw-r--r--   0        0        0    13955 2024-04-13 14:33:01.623021 blint-2.1.2/blint/android.py
--rw-r--r--   0        0        0    56201 2024-04-13 14:33:01.623021 blint-2.1.2/blint/binary.py
--rw-r--r--   0        0        0     2794 2024-04-13 14:33:01.623021 blint-2.1.2/blint/checks.py
--rw-r--r--   0        0        0     6198 2024-04-13 14:33:01.623021 blint-2.1.2/blint/cli.py
--rw-r--r--   0        0        0    20365 2024-04-13 14:33:01.623021 blint-2.1.2/blint/config.py
--rw-r--r--   0        0        0      324 2024-04-13 14:33:01.623021 blint-2.1.2/blint/cyclonedx/README.md
--rw-r--r--   0        0        0        0 2024-04-13 14:33:01.623021 blint-2.1.2/blint/cyclonedx/__init__.py
--rw-r--r--   0        0        0    20843 2024-04-13 14:33:01.623021 blint-2.1.2/blint/cyclonedx/spdx.py
--rw-r--r--   0        0        0   169203 2024-04-13 14:33:01.623021 blint-2.1.2/blint/cyclonedx/spec.py
--rw-r--r--   0        0        0        0 2024-04-13 14:33:01.623021 blint-2.1.2/blint/data/__init__.py
--rw-r--r--   0        0        0        0 2024-04-13 14:33:01.623021 blint-2.1.2/blint/data/annotations/__init__.py
--rw-r--r--   0        0        0     1498 2024-04-13 14:33:01.623021 blint-2.1.2/blint/data/annotations/review_entries_generic.yml
--rw-r--r--   0        0        0     2358 2024-04-13 14:33:01.623021 blint-2.1.2/blint/data/annotations/review_entries_pe.yml
--rw-r--r--   0        0        0    15418 2024-04-13 14:33:01.623021 blint-2.1.2/blint/data/annotations/review_exe_go.yml
--rw-r--r--   0        0        0   124932 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_imports_pe.yml
--rw-r--r--   0        0        0     8155 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_methods_generic.yml
--rw-r--r--   0        0        0     5764 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_methods_mips.yml
--rw-r--r--   0        0        0     2409 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_monero_generic.yml
--rw-r--r--   0        0        0     1522 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_monero_go.yml
--rw-r--r--   0        0        0      994 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_monero_rust
--rw-r--r--   0        0        0      994 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_monero_rust.yml
--rw-r--r--   0        0        0     5646 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_rootkits_win.yml
--rw-r--r--   0        0        0     3507 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_symbols_antiforensic.yml
--rw-r--r--   0        0        0     2943 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_symbols_generic.yml
--rw-r--r--   0        0        0     1277 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_symbols_hooka.yml
--rw-r--r--   0        0        0    23537 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_symbols_macho.yml
--rw-r--r--   0        0        0    10425 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/annotations/review_symbols_rust.yml
--rw-r--r--   0        0        0    11038 2024-04-13 14:33:01.627021 blint-2.1.2/blint/data/rules.yml
--rw-r--r--   0        0        0      936 2024-04-13 14:33:01.627021 blint-2.1.2/blint/logger.py
--rw-r--r--   0        0        0    23315 2024-04-13 14:33:01.627021 blint-2.1.2/blint/sbom.py
--rw-r--r--   0        0        0    14323 2024-04-13 14:33:01.627021 blint-2.1.2/blint/utils.py
--rw-r--r--   0        0        0     1812 2024-04-13 14:33:01.627021 blint-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 blint-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-21 15:41:54.867738 blint-2.1.3/LICENSE
+-rw-r--r--   0        0        0     6240 2024-04-21 15:41:54.867738 blint-2.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-21 15:41:54.867738 blint-2.1.3/blint/__init__.py
+-rw-r--r--   0        0        0    24122 2024-04-21 15:41:54.867738 blint-2.1.3/blint/analysis.py
+-rw-r--r--   0        0        0    13915 2024-04-21 15:41:54.867738 blint-2.1.3/blint/android.py
+-rw-r--r--   0        0        0    56702 2024-04-21 15:41:54.871738 blint-2.1.3/blint/binary.py
+-rw-r--r--   0        0        0     2794 2024-04-21 15:41:54.871738 blint-2.1.3/blint/checks.py
+-rw-r--r--   0        0        0     6198 2024-04-21 15:41:54.871738 blint-2.1.3/blint/cli.py
+-rw-r--r--   0        0        0    20365 2024-04-21 15:41:54.871738 blint-2.1.3/blint/config.py
+-rw-r--r--   0        0        0      324 2024-04-21 15:41:54.871738 blint-2.1.3/blint/cyclonedx/README.md
+-rw-r--r--   0        0        0        0 2024-04-21 15:41:54.871738 blint-2.1.3/blint/cyclonedx/__init__.py
+-rw-r--r--   0        0        0    20843 2024-04-21 15:41:54.871738 blint-2.1.3/blint/cyclonedx/spdx.py
+-rw-r--r--   0        0        0   169203 2024-04-21 15:41:54.871738 blint-2.1.3/blint/cyclonedx/spec.py
+-rw-r--r--   0        0        0        0 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/__init__.py
+-rw-r--r--   0        0        0     1498 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_entries_generic.yml
+-rw-r--r--   0        0        0     2358 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_entries_pe.yml
+-rw-r--r--   0        0        0    15418 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_exe_go.yml
+-rw-r--r--   0        0        0   124932 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_imports_pe.yml
+-rw-r--r--   0        0        0     8155 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_methods_generic.yml
+-rw-r--r--   0        0        0     5764 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_methods_mips.yml
+-rw-r--r--   0        0        0     2409 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_monero_generic.yml
+-rw-r--r--   0        0        0     1522 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_monero_go.yml
+-rw-r--r--   0        0        0      994 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_monero_rust
+-rw-r--r--   0        0        0      994 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_monero_rust.yml
+-rw-r--r--   0        0        0     5646 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_rootkits_win.yml
+-rw-r--r--   0        0        0     3507 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_symbols_antiforensic.yml
+-rw-r--r--   0        0        0     2943 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_symbols_generic.yml
+-rw-r--r--   0        0        0     1277 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_symbols_hooka.yml
+-rw-r--r--   0        0        0    23537 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_symbols_macho.yml
+-rw-r--r--   0        0        0    10425 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/annotations/review_symbols_rust.yml
+-rw-r--r--   0        0        0    11038 2024-04-21 15:41:54.871738 blint-2.1.3/blint/data/rules.yml
+-rw-r--r--   0        0        0      936 2024-04-21 15:41:54.871738 blint-2.1.3/blint/logger.py
+-rw-r--r--   0        0        0    24904 2024-04-21 15:41:54.875738 blint-2.1.3/blint/sbom.py
+-rw-r--r--   0        0        0    14323 2024-04-21 15:41:54.875738 blint-2.1.3/blint/utils.py
+-rw-r--r--   0        0        0     1812 2024-04-21 15:41:54.875738 blint-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7426 1970-01-01 00:00:00.000000 blint-2.1.3/PKG-INFO
```

### Comparing `blint-2.1.2/LICENSE` & `blint-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/README.md` & `blint-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/analysis.py` & `blint-2.1.3/blint/analysis.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/android.py` & `blint-2.1.3/blint/android.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,21 +14,15 @@
     Type,
 )
 from blint.logger import LOG
 from blint.utils import check_command, create_component_evidence, find_files, unzip_unsafe
 
 ANDROID_HOME = os.getenv("ANDROID_HOME")
 APKANALYZER_CMD = os.getenv("APKANALYZER_CMD")
-if (
-        not APKANALYZER_CMD
-        and ANDROID_HOME
-        and (
-        os.path.exists(os.path.join(ANDROID_HOME, "cmdline-tools", "latest", "bin", "apkanalyzer"))
-)
-):
+if not APKANALYZER_CMD and ANDROID_HOME and os.path.exists(os.path.join(ANDROID_HOME, "cmdline-tools", "latest", "bin", "apkanalyzer")):
     APKANALYZER_CMD = os.path.join(ANDROID_HOME, "cmdline-tools", "latest", "bin", "apkanalyzer")
 elif check_command("apkanalyzer"):
     APKANALYZER_CMD = "apkanalyzer"
 
 
 def exec_tool(args, cwd=None, stdout=subprocess.PIPE):
     """
```

### Comparing `blint-2.1.2/blint/binary.py` & `blint-2.1.3/blint/binary.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # pylint: disable=too-many-lines,consider-using-f-string
 import codecs
 import contextlib
 import json
 import sys
+from typing import Tuple
+import zlib
 
 import lief
 
 from blint.logger import DEBUG, LOG
 from blint.utils import calculate_entropy, check_secret, cleanup_dict_lief_errors, decode_base64
 
 MIN_ENTROPY = 0.39
@@ -213,32 +215,14 @@
                             }
                         )
             except (AttributeError, TypeError):
                 continue
     return strings_list
 
 
-def ignorable_symbol(symbol_name: str | None) -> bool:
-    """
-    Determines if a symbol is ignorable.
-
-    Args:
-        symbol_name (str): The name of the symbol to check.
-
-    Returns:
-        bool: True if the symbol is ignorable, False otherwise.
-    """
-    if not symbol_name:
-        return True
-    for pref in ("_$f", "$f64.", "__"):
-        if symbol_name.startswith(pref):
-            return True
-    return False
-
-
 def parse_symbols(symbols):
     """
     Parse symbols from a list of symbols.
 
     Args:
         symbols (it_symbols): A list of symbols to parse.
 
@@ -256,32 +240,31 @@
             if symbol.imported and not isinstance(symbol.imported, lief.lief_errors):
                 is_imported = True
             if symbol.exported and not isinstance(symbol.exported, lief.lief_errors):
                 is_exported = True
             symbol_name = symbol.demangled_name
             if isinstance(symbol_name, lief.lief_errors):
                 symbol_name = symbol.name
-            if not ignorable_symbol(symbol_name):
-                exe_type = guess_exe_type(symbol_name)
-                symbols_list.append(
-                    {
-                        "name": symbol_name,
-                        "type": str(symbol.type).rsplit(".", maxsplit=1)[-1],
-                        "value": symbol.value,
-                        "visibility": str(symbol.visibility).rsplit(".", maxsplit=1)[-1],
-                        "binding": str(symbol.binding).rsplit(".", maxsplit=1)[-1],
-                        "is_imported": is_imported,
-                        "is_exported": is_exported,
-                        "information": symbol.information,
-                        "is_function": symbol.is_function,
-                        "is_static": symbol.is_static,
-                        "is_variable": symbol.is_variable,
-                        "version": str(symbol_version),
-                    }
-                )
+            exe_type = guess_exe_type(symbol_name)
+            symbols_list.append(
+                {
+                    "name": symbol_name,
+                    "type": str(symbol.type).rsplit(".", maxsplit=1)[-1],
+                    "value": symbol.value,
+                    "visibility": str(symbol.visibility).rsplit(".", maxsplit=1)[-1],
+                    "binding": str(symbol.binding).rsplit(".", maxsplit=1)[-1],
+                    "is_imported": is_imported,
+                    "is_exported": is_exported,
+                    "information": symbol.information,
+                    "is_function": symbol.is_function,
+                    "is_static": symbol.is_static,
+                    "is_variable": symbol.is_variable,
+                    "version": str(symbol_version),
+                }
+            )
         except (AttributeError, IndexError, TypeError):
             continue
     return symbols_list, exe_type
 
 
 def detect_exe_type(parsed_obj, metadata):
     """
@@ -652,27 +635,26 @@
                 if symbol.value > 0 or not symbol.has_binding_info
                 else ADDRESS_FMT.format(symbol.binding_info.address)
             )
             symbol_name = symbol.demangled_name
             if not symbol_name or isinstance(symbol_name, lief.lief_errors):
                 symbol_name = symbol.name
             symbol_name = symbol_name.replace("..", "::")
-            if not ignorable_symbol(symbol_name):
-                if not exe_type:
-                    exe_type = guess_exe_type(symbol_name)
-                symbols_list.append(
-                    {
-                        "name": (f"{libname}::{symbol_name}" if libname else symbol_name),
-                        "short_name": symbol_name,
-                        "type": symbol.type,
-                        "num_sections": symbol.numberof_sections,
-                        "description": symbol.description,
-                        "value": symbol_value,
-                    }
-                )
+            if not exe_type:
+                exe_type = guess_exe_type(symbol_name)
+            symbols_list.append(
+                {
+                    "name": (f"{libname}::{symbol_name}" if libname else symbol_name),
+                    "short_name": symbol_name,
+                    "type": symbol.type,
+                    "num_sections": symbol.numberof_sections,
+                    "description": symbol.description,
+                    "value": symbol_value,
+                }
+            )
         except (AttributeError, TypeError):
             continue
     return symbols_list, exe_type
 
 
 def parse(exe_file):  # pylint: disable=too-many-locals,too-many-branches,too-many-statements
     """
@@ -757,14 +739,15 @@
     metadata["dynamic_symbols"], exe_type = parse_symbols(parsed_obj.dynamic_symbols)
     if exe_type:
         metadata["exe_type"] = exe_type
     metadata["functions"] = parse_functions(parsed_obj.functions)
     metadata["ctor_functions"] = parse_functions(parsed_obj.ctor_functions)
     metadata["dotnet_dependencies"] = parse_overlay(parsed_obj)
     metadata["go_dependencies"], metadata["go_formulation"] = parse_go_buildinfo(parsed_obj)
+    metadata["rust_dependencies"] = parse_rust_buildinfo(parsed_obj)
 
     return metadata
 
 
 def add_elf_header(header, metadata):
     """Adds ELF header data to the metadata dictionary.
 
@@ -926,15 +909,15 @@
                     # Use libraries to construct BOM components and targets for the dependency tree
                     deps = json.loads(overlay_str)
                 except json.JSONDecodeError:
                     pass
     return deps
 
 
-def parse_go_buildinfo(parsed_obj: lief.Binary) -> (dict[str, dict[str, str]], dict[str, str]):
+def parse_go_buildinfo(parsed_obj: lief.Binary) -> Tuple[dict[str, dict[str, str]], dict[str, str]]:
     """
     Parse the go build info section to extract go dependencies
     Args:
         parsed_obj (lief.Binary): The parsed object representing the binary.
 
     Returns:
         tuple(dict[str, str], dict[str, str]): Tuple representing the dependencies and formulation.
@@ -979,14 +962,40 @@
         if line.startswith("build "):
             tmp_a = line.removeprefix("build ").split("=")
             formulation[tmp_a[0].replace("-", "")] = tmp_a[1]
 
     return deps, formulation
 
 
+def parse_rust_buildinfo(parsed_obj: lief.Binary) -> list:
+    """
+    Parse the rust build info section of binaries that are cargo-auditable to extract rust dependencies
+    Args:
+        parsed_obj (lief.Binary): The parsed object representing the binary.
+
+    Returns:
+        list: List representing the dependencies.
+    """
+    deps = []
+
+    try:
+        audit_data_section = next(filter(lambda section: section.name == ".dep-v0", parsed_obj.sections), None)
+        if audit_data_section is not None and audit_data_section.content:
+            json_string = zlib.decompress(audit_data_section.content)
+            audit_data = json.loads(json_string)
+
+            if audit_data and audit_data["packages"]:
+                packages = audit_data["packages"]
+                deps = [x for x in packages if 'root' not in x]
+    except json.JSONDecodeError:
+        pass
+
+    return deps
+
+
 def add_pe_metadata(exe_file: str, metadata: dict, parsed_obj: lief.PE.Binary):
     """Adds PE metadata to the given metadata dictionary.
 
     Args:
         exe_file (str): The path of the executable file.
         metadata (dict): The dictionary to store the metadata.
         parsed_obj (lief.PE.Binary): The parsed object representing the PE binary.
@@ -1031,14 +1040,15 @@
         metadata["exception_functions"] = parse_functions(parsed_obj.exception_functions)
         # Detect if this PE might be dotnet
         for i, dd in enumerate(parsed_obj.data_directories):
             if i == 14 and dd.type.value == lief.PE.DataDirectory.TYPES.CLR_RUNTIME_HEADER.value:
                 metadata["is_dotnet"] = True
         metadata["dotnet_dependencies"] = parse_overlay(parsed_obj)
         metadata["go_dependencies"], metadata["go_formulation"] = parse_go_buildinfo(parsed_obj)
+        metadata["rust_dependencies"] = parse_rust_buildinfo(parsed_obj)
         tls = parsed_obj.tls
         if tls and tls.sizeof_zero_fill:
             metadata["tls_address_index"] = tls.addressof_index
             metadata["tls_sizeof_zero_fill"] = tls.sizeof_zero_fill
             metadata["tls_data_template_len"] = len(tls.data_template)
             metadata["tls_characteristics"] = tls.characteristics
             metadata["tls_section_name"] = tls.section.name
@@ -1192,14 +1202,15 @@
         LOG.debug(f"Caught {type(e)}: {e} while parsing {exe_file} Mach0 UUID.")
     metadata = add_mach0_libraries(exe_file, metadata, parsed_obj)
     metadata = add_mach0_header_data(exe_file, metadata, parsed_obj)
     metadata = add_mach0_commands(metadata, parsed_obj)
     metadata = add_mach0_functions(metadata, parsed_obj)
     metadata = add_mach0_signature(exe_file, metadata, parsed_obj)
     metadata["go_dependencies"], metadata["go_formulation"] = parse_go_buildinfo(parsed_obj)
+    metadata["rust_dependencies"] = parse_rust_buildinfo(parsed_obj)
     return metadata
 
 
 def add_mach0_commands(metadata, parsed_obj):
     """Extracts MachO commands metadata from the parsed object and adds it to the metadata.
 
     Args:
```

### Comparing `blint-2.1.2/blint/checks.py` & `blint-2.1.3/blint/checks.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/cli.py` & `blint-2.1.3/blint/cli.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/config.py` & `blint-2.1.3/blint/config.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/cyclonedx/spdx.py` & `blint-2.1.3/blint/cyclonedx/spdx.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/cyclonedx/spec.py` & `blint-2.1.3/blint/cyclonedx/spec.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/data/annotations/review_entries_generic.yml` & `blint-2.1.3/blint/data/annotations/review_entries_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/data/annotations/review_entries_pe.yml` & `blint-2.1.3/blint/data/annotations/review_entries_pe.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/data/annotations/review_exe_go.yml` & `blint-2.1.3/blint/data/annotations/review_exe_go.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/data/annotations/review_imports_pe.yml` & `blint-2.1.3/blint/data/annotations/review_imports_pe.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/data/annotations/review_methods_generic.yml` & `blint-2.1.3/blint/data/annotations/review_methods_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/data/annotations/review_methods_mips.yml` & `blint-2.1.3/blint/data/annotations/review_methods_mips.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/data/annotations/review_monero_generic.yml` & `blint-2.1.3/blint/data/annotations/review_monero_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/data/annotations/review_monero_go.yml` & `blint-2.1.3/blint/data/annotations/review_monero_go.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/data/annotations/review_monero_rust` & `blint-2.1.3/blint/data/annotations/review_monero_rust`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/data/annotations/review_monero_rust.yml` & `blint-2.1.3/blint/data/annotations/review_monero_rust.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/data/annotations/review_rootkits_win.yml` & `blint-2.1.3/blint/data/annotations/review_rootkits_win.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/data/annotations/review_symbols_antiforensic.yml` & `blint-2.1.3/blint/data/annotations/review_symbols_antiforensic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/data/annotations/review_symbols_generic.yml` & `blint-2.1.3/blint/data/annotations/review_symbols_generic.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/data/annotations/review_symbols_hooka.yml` & `blint-2.1.3/blint/data/annotations/review_symbols_hooka.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/data/annotations/review_symbols_macho.yml` & `blint-2.1.3/blint/data/annotations/review_symbols_macho.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/data/annotations/review_symbols_rust.yml` & `blint-2.1.3/blint/data/annotations/review_symbols_rust.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/data/rules.yml` & `blint-2.1.3/blint/data/rules.yml`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/logger.py` & `blint-2.1.3/blint/logger.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/blint/sbom.py` & `blint-2.1.3/blint/sbom.py`

 * *Files 4% similar despite different names*

```diff
@@ -389,14 +389,18 @@
     for k, v in metadata.get("go_formulation", {}).items():
         parent_component.properties.append(
             Property(
                 name=f"internal:{camel_to_snake(k)}",
                 value=str(v).strip(),
             )
         )
+    # Convert rust dependencies
+    if metadata.get("rust_dependencies"):
+        rust_components = process_rust_dependencies(metadata.get("rust_dependencies"), dependencies_dict)
+        lib_components += rust_components
     if lib_components:
         components += lib_components
         track_dependency(dependencies_dict, parent_component, lib_components)
 
     return components
 
 
@@ -579,14 +583,50 @@
         if hash_content:
             comp.hashes = [Hash(alg=HashAlg.SHA_256, content=hash_content)]
         comp.bom_ref = RefType(f"""pkg:golang/{k}@{v.get("version")}""")
         components.append(comp)
     return components
 
 
+def process_rust_dependencies(rust_deps: list, dependencies_dict: dict[str, set]) -> list[Component]:
+    """
+    Process the rust dependencies metadata extracted for binary overlays
+
+    Args:
+        rust_deps (list): dependencies metadata
+
+    Returns:
+        list: New component list
+    """
+    components = []
+    idx_to_purl = {}
+    for idx, dep in enumerate(rust_deps):
+        idx_to_purl[idx] = f"""pkg:cargo/{dep["name"]}@{dep["version"]}"""
+    for dependency in rust_deps:
+        purl = f"""pkg:cargo/{dependency["name"]}@{dependency["version"]}"""
+        purl_qualifer = f"""?repository={dependency.get("source")}""" if dependency.get("source", "") != "crates.io" else ""
+        comp = Component(
+            type=Type.library,
+            name=dependency["name"],
+            version=dependency["version"],
+            purl=f"{purl}{purl_qualifer}",
+            scope=Scope.required,
+            evidence=create_component_evidence(dependency["name"], 0.8)
+        )
+        comp.bom_ref = RefType(purl)
+        components.append(comp)
+        if not dependencies_dict.get(purl):
+            dependencies_dict[purl] = set()
+        # Recover the dependency tree
+        if dependency.get("dependencies"):
+            for adep in dependency.get("dependencies"):
+                dependencies_dict[purl].add(idx_to_purl[adep])
+    return components
+
+
 def track_dependency(
         dependencies_dict: dict[str, set], parent_component: Component, app_components: list[Component]
 ) -> None:
     """
     Track dependencies between components and update the dependencies dict.
 
     Args:
```

### Comparing `blint-2.1.2/blint/utils.py` & `blint-2.1.3/blint/utils.py`

 * *Files identical despite different names*

### Comparing `blint-2.1.2/pyproject.toml` & `blint-2.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blint"
-version = "2.1.2"
+version = "2.1.3"
 description = "Linter and SBOM generator for binary files."
 authors = ["Prabhu Subramanian <prabhu@appthreat.com>", "Caroline Russell <caroline@appthreat.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/OWASP-dep-scan/blint"
 repository = "https://github.com/OWASP-dep-scan/blint"
 keywords = ["linter", "binary", "security", "sast"]
```

### Comparing `blint-2.1.2/PKG-INFO` & `blint-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blint
-Version: 2.1.2
+Version: 2.1.3
 Summary: Linter and SBOM generator for binary files.
 Home-page: https://github.com/OWASP-dep-scan/blint
 License: MIT
 Keywords: linter,binary,security,sast
 Author: Prabhu Subramanian
 Author-email: prabhu@appthreat.com
 Requires-Python: >=3.10,<3.13
```

