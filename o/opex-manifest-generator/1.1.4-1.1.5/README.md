# Comparing `tmp/opex_manifest_generator-1.1.4.tar.gz` & `tmp/opex_manifest_generator-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opex_manifest_generator-1.1.4.tar", last modified: Fri Apr 12 14:05:21 2024, max compression
+gzip compressed data, was "opex_manifest_generator-1.1.5.tar", last modified: Sun Apr 21 18:50:39 2024, max compression
```

## Comparing `opex_manifest_generator-1.1.4.tar` & `opex_manifest_generator-1.1.5.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 14:05:21.069555 opex_manifest_generator-1.1.4/
--rw-rw-rw-   0        0        0      124 2024-04-12 13:39:12.000000 opex_manifest_generator-1.1.4/.gitignore
--rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 opex_manifest_generator-1.1.4/LICENSE.md
--rw-rw-rw-   0        0        0      701 2024-04-12 14:05:21.067543 opex_manifest_generator-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    19695 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 14:05:21.034551 opex_manifest_generator-1.1.4/opex_manifest_generator/
--rw-rw-rw-   0        0        0      439 2024-02-20 12:38:50.000000 opex_manifest_generator-1.1.4/opex_manifest_generator/__init__.py
--rw-rw-rw-   0        0        0     6050 2024-04-12 13:08:38.000000 opex_manifest_generator-1.1.4/opex_manifest_generator/cli.py
--rw-rw-rw-   0        0        0      676 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.4/opex_manifest_generator/common.py
--rw-rw-rw-   0        0        0      966 2024-02-18 22:01:42.000000 opex_manifest_generator-1.1.4/opex_manifest_generator/hash.py
-drwxrwxrwx   0        0        0        0 2024-04-12 14:05:21.057544 opex_manifest_generator-1.1.4/opex_manifest_generator/metadata/
--rw-rw-rw-   0        0        0      775 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.4/opex_manifest_generator/metadata/DublinCore Template.xml
--rw-rw-rw-   0        0        0     2268 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.4/opex_manifest_generator/metadata/EAD Template.xml
--rw-rw-rw-   0        0        0      483 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.4/opex_manifest_generator/metadata/GDPR Template.xml
--rw-rw-rw-   0        0        0     2701 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.4/opex_manifest_generator/metadata/MODS Template.xml
--rw-rw-rw-   0        0        0    27312 2024-04-12 14:02:21.000000 opex_manifest_generator-1.1.4/opex_manifest_generator/opex_manifest.py
-drwxrwxrwx   0        0        0        0 2024-04-12 14:05:21.060593 opex_manifest_generator-1.1.4/opex_manifest_generator/samples/
--rw-rw-rw-   0        0        0      389 2023-02-23 12:37:11.000000 opex_manifest_generator-1.1.4/opex_manifest_generator/samples/Opex.xml
--rw-rw-rw-   0        0        0    29091 2024-04-04 10:37:30.000000 opex_manifest_generator-1.1.4/opex_manifest_generator/samples/opex_manifest_generator_AutoClass.xlsx
-drwxrwxrwx   0        0        0        0 2024-04-12 14:05:21.064544 opex_manifest_generator-1.1.4/opex_manifest_generator/samples/spreads/
--rw-rw-rw-   0        0        0    22794 2024-04-04 14:48:01.000000 opex_manifest_generator-1.1.4/opex_manifest_generator/samples/spreads/dctemplate.xlsx
--rw-rw-rw-   0        0        0    19299 2024-04-04 14:45:30.000000 opex_manifest_generator-1.1.4/opex_manifest_generator/samples/spreads/eadtemplate.xlsx
--rw-rw-rw-   0        0        0    18662 2024-04-04 14:51:01.000000 opex_manifest_generator-1.1.4/opex_manifest_generator/samples/spreads/gdprtemplate.xlsx
--rw-rw-rw-   0        0        0    19509 2024-04-04 14:46:22.000000 opex_manifest_generator-1.1.4/opex_manifest_generator/samples/spreads/modstemplate.xlsx
--rw-rw-rw-   0        0        0       58 2024-02-20 15:05:15.000000 opex_manifest_generator-1.1.4/opex_manifest_generator/test_cli.py
--rw-rw-rw-   0        0        0       21 2024-04-12 14:03:16.000000 opex_manifest_generator-1.1.4/opex_manifest_generator/version.py
-drwxrwxrwx   0        0        0        0 2024-04-12 14:05:21.066543 opex_manifest_generator-1.1.4/opex_manifest_generator.egg-info/
--rw-rw-rw-   0        0        0      701 2024-04-12 14:05:20.000000 opex_manifest_generator-1.1.4/opex_manifest_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1125 2024-04-12 14:05:21.000000 opex_manifest_generator-1.1.4/opex_manifest_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 14:05:20.000000 opex_manifest_generator-1.1.4/opex_manifest_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-12 14:05:20.000000 opex_manifest_generator-1.1.4/opex_manifest_generator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2024-04-12 14:05:20.000000 opex_manifest_generator-1.1.4/opex_manifest_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-04-12 14:05:20.000000 opex_manifest_generator-1.1.4/opex_manifest_generator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      837 2024-04-12 14:04:19.000000 opex_manifest_generator-1.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 14:05:21.069555 opex_manifest_generator-1.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-21 18:50:39.880282 opex_manifest_generator-1.1.5/
+-rw-rw-rw-   0        0        0      124 2024-04-12 13:39:12.000000 opex_manifest_generator-1.1.5/.gitignore
+-rw-rw-rw-   0        0        0    11558 2024-02-18 12:39:01.000000 opex_manifest_generator-1.1.5/LICENSE.md
+-rw-rw-rw-   0        0        0      701 2024-04-21 18:50:39.880282 opex_manifest_generator-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    21573 2024-04-21 18:27:56.000000 opex_manifest_generator-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-21 18:50:39.409942 opex_manifest_generator-1.1.5/assets/
+-rw-rw-rw-   0        0        0     8271 2024-04-12 14:39:11.000000 opex_manifest_generator-1.1.5/assets/Column Headers.png
+-rw-rw-rw-   0        0        0    27359 2024-04-12 14:49:33.000000 opex_manifest_generator-1.1.5/assets/FullName Column.png
+-rw-rw-rw-   0        0        0    16064 2024-04-12 14:57:04.000000 opex_manifest_generator-1.1.5/assets/Hash Headers.png
+-rw-rw-rw-   0        0        0     4920 2024-04-12 14:58:52.000000 opex_manifest_generator-1.1.5/assets/Identifiers Headers.png
+-rw-rw-rw-   0        0        0     2602 2024-04-12 15:01:06.000000 opex_manifest_generator-1.1.5/assets/XML Headers.png
+drwxrwxrwx   0        0        0        0 2024-04-21 18:50:39.499178 opex_manifest_generator-1.1.5/opex_manifest_generator/
+-rw-rw-rw-   0        0        0      476 2024-04-21 18:41:39.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/__init__.py
+-rw-rw-rw-   0        0        0     6046 2024-04-21 18:36:34.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/cli.py
+-rw-rw-rw-   0        0        0      676 2024-04-04 09:48:17.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/common.py
+-rw-rw-rw-   0        0        0      966 2024-02-18 22:01:42.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/hash.py
+drwxrwxrwx   0        0        0        0 2024-04-21 18:50:39.717914 opex_manifest_generator-1.1.5/opex_manifest_generator/metadata/
+-rw-rw-rw-   0        0        0      775 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/metadata/DublinCore Template.xml
+-rw-rw-rw-   0        0        0     2268 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/metadata/EAD Template.xml
+-rw-rw-rw-   0        0        0      483 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/metadata/GDPR Template.xml
+-rw-rw-rw-   0        0        0     2701 2023-12-13 09:26:40.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/metadata/MODS Template.xml
+-rw-rw-rw-   0        0        0    28748 2024-04-18 10:19:35.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/opex_manifest.py
+drwxrwxrwx   0        0        0        0 2024-04-21 18:50:39.775124 opex_manifest_generator-1.1.5/opex_manifest_generator/samples/
+-rw-rw-rw-   0        0        0      389 2023-02-23 12:37:11.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/samples/Opex.xml
+-rw-rw-rw-   0        0        0    24938 2024-04-12 14:50:52.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/samples/opex_manifest_generator_AutoClass.xlsx
+drwxrwxrwx   0        0        0        0 2024-04-21 18:50:39.872280 opex_manifest_generator-1.1.5/opex_manifest_generator/samples/spreads/
+-rw-rw-rw-   0        0        0    22794 2024-04-04 14:48:01.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/samples/spreads/dctemplate.xlsx
+-rw-rw-rw-   0        0        0    19299 2024-04-04 14:45:30.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/samples/spreads/eadtemplate.xlsx
+-rw-rw-rw-   0        0        0    18662 2024-04-04 14:51:01.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/samples/spreads/gdprtemplate.xlsx
+-rw-rw-rw-   0        0        0    19509 2024-04-04 14:46:22.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/samples/spreads/modstemplate.xlsx
+-rw-rw-rw-   0        0        0       58 2024-02-20 15:05:15.000000 opex_manifest_generator-1.1.5/opex_manifest_generator/test_cli.py
+drwxrwxrwx   0        0        0        0 2024-04-21 18:50:39.872280 opex_manifest_generator-1.1.5/opex_manifest_generator.egg-info/
+-rw-rw-rw-   0        0        0      701 2024-04-21 18:50:38.000000 opex_manifest_generator-1.1.5/opex_manifest_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1221 2024-04-21 18:50:39.000000 opex_manifest_generator-1.1.5/opex_manifest_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-21 18:50:38.000000 opex_manifest_generator-1.1.5/opex_manifest_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-21 18:50:38.000000 opex_manifest_generator-1.1.5/opex_manifest_generator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2024-04-21 18:50:38.000000 opex_manifest_generator-1.1.5/opex_manifest_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-21 18:50:38.000000 opex_manifest_generator-1.1.5/opex_manifest_generator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      940 2024-04-21 18:48:58.000000 opex_manifest_generator-1.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-21 18:50:39.888287 opex_manifest_generator-1.1.5/setup.cfg
```

### Comparing `opex_manifest_generator-1.1.4/LICENSE.md` & `opex_manifest_generator-1.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.4/PKG-INFO` & `opex_manifest_generator-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opex_manifest_generator
-Version: 1.1.4
+Version: 1.1.5
 Summary: Opex Manifest Generator Tool for use with Opex / Preservica
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/opex_manifest_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/opex_manifest_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opex_manifest_generator-1.1.4/README.md` & `opex_manifest_generator-1.1.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 This tool was primarily intended to allow users, to undertake larger uploads safely utilising bulk ingests, utilising the Opex Ingest Workflow, with Folder Manifest's checked to ensure safe transfer. However, it has been tested as functioning with:
 - Bulk / Opex Ingest Workflow
 - PUT Tool / Auto Ingest Workflows
 - Manual Ingest
 - Starter/UX2 Ingest uploads (Both File and Folder)
 
-## Additional features
+## Features
 
-There are a number of additional feature's utilised including:
+There are a number of features including:
 - Generating Fixities for files, with SHA1, MD5, SHA256, SHA512 (Default is SHA1)
 - OPEX's can also be cleared, for repeated / ease of use.
 - OPEX's can be zipped with the file, for imports use with Starter/UX2/Manual ingest methods
 
 The Program also makes use of the Auto Classification Generator, allowing for:
 - Reference's can be automatically generated and embedded into the Opex, with assignable prefixes.
 - This can utilise either the Catalog or Accession mode, or both!
@@ -75,149 +75,189 @@
 
 `opex_generate "C:\Users\Christopher\Downloads\" -fx SHA-1 -z`
 
 Currently, no files will be removed after the zipping. Be aware that running this command multiple times in row will break existing Opex's.
 
 ### Clearing Opex's
 
-Mistakes happen! So, the clear option will remove all existing Opex's in a directory.
+Mistakes happen! The clear option will remove all existing Opex's in a directory.
 
 `opex_generate "C:\Users\Christopher\Downloads\" -clr`
 
 Running this command with no additional options will end the program after clearing the Opex's; if other options are enabled it will proceed with the generation of those Opex's.
 
-## Filtering note
+### Removing Empty Directories
 
-Currently a number of filters are applied to certain files / folders.
+You can also clear any empty directories from the  by using `--remove-empty` option. This will remove any empty directories and generate a simple text document with a list of all the directories that were removed. This process is not reversible and you will be asked to confirm your choice.
 
-1) Hidden directories / files and those starting with '.' are not included.
+## Filtering
+
+Currently 2 filters are applied to certain files / folders:
+
+1) Hidden directories / files, either by Flag in Windows or starting with '.' in MacOS / Linux, are not included.
 2) Folder's titled 'meta' are not included.
 
 Hidden files and directories can be included by utilising the `--hidden` option.
 
+meta folders will always be generated automatically when used with the Fixity and Clearing Empty Directories options; meta directories are also created when using the Auto Classification Generator. You can redirect the path using the `-o` option:
+
+`-o {/path/to/meta/output}`
+
 ## Use with the Auto Classification Generator
 
 The Opex Manifest generator becomes much more powerful when utilised with another tool: the Auto Classification Generator, see [here](https://github.com/CPJPRINCE/auto_classification_generator) for further details.
 
-This is built-in to the Opex Manifest Generator and can be utilised to embed identifiers and metadata directly to an Opex or through use of a spreadsheet / CSV file.
+This is built-in to the Opex Manifest Generator and can be utilised to embed identifiers and metadata directly to an Opex or through the use of an Excel spreadsheet or CSV file.
 
-The Opex Manifest Generator makes use of the auto_class_generator as a module. It's behaviour differs somewhat when compared to utilising the standalone command `auto_class.exe`.
+The Opex Manifest Generator makes use of the auto_class_generator as a module, therefore it's behaviour differs somewhat when compared to utilising the standalone command `auto_class.exe`.
 
 ### Auto Classification - Code Generation
 
-To generate an auto classification code, call on `-c` option with `catalog` choice. You can also assign a prefix using `-p ARCH`:
+To generate an auto classification code, call on `-c` option with `catalog` choice. You can also assign a prefix using `-p "ARCH"`:
 
 `opex_generate -c catalog -p "ARCH" C:\Users\Christopher\Downloads`
 
-This will generate Opex's with an identifier `code` for each of the files / folders. As described in the Auto Class module, the reference codes will take the hierarchy of the directories. You can use the `-s` option to set a starting reference.
+This will generate Opex's with an identifier `code` for each of the files / folders. As described in the Auto Class module, the reference codes will take the hierarchy of the directories. You can also use the `-s` option to set a starting reference.
 
-You can alternatively utilise the "Accession" / running number mode of generating a code using `-c accession` with prefix `2024`. *To note Accession is currently hard-coded to use "File" mode*:
+You can alternatively utilise the "Accession" / running number mode of generating a code using `-c accession` with the prefix "2024". *Accession is currently hard-coded to use the "File" mode*:
 
 `opex_generate -c accession -p "2024" C:\Users\Christopher\Downloads`
 
 Alternatively you can do both Catalogue / Accession at the same time:
 
 `opex_generate -c both -p "ARCH" "2024" C:\Users\Christopher\Downloads`
 
-To note: when using the `catalog` option, the key `code` is always used by default. When using `accession` the default key is `accref`. This is currently not adjustable, see [here](### XIP Metadata - Identifiers) for utilising other keys. 
+To note: when using the `catalog` option, the key `code` is always used by default. When using `accession` the default key is `accref`. This is currently not adjustable, see [here](#XIP-Metadata---Identifiers) for utilising other keys. 
 
-It's possible to also create a `generic` set of metadata which will take the XIP metadata for Title, Description from the basename of the folder/file and will set the Security Status to `open`. 
+It's possible to also create a `generic` set of metadata which will take the XIP metadata for the Title and Description fields, from the basename of the folder/file. It will also set the Security Status to "open".
 
 `opex_generate -c generic C:\Users\Christopher\Downloads`
 
-You can combine generic options with catalog, accession, both to also generate an identifer.
-
-You can also clear Empty Directory by using `--remove-empty` option. This will also generate 
+You can combine the generic options with `catalog, accession, both` to generate an identifier alongside generic data.
 
-## Auto Classification - Spreadsheet as Input 
+## Auto Classification - Spreadsheet as an Input Override 
 
-This program also supports utilising an Auto Class spreadsheet as an input, utilising the data added into said spreadsheet, instead of generating them on command.
+This program also supports utilising an Auto Class spreadsheet as an input override, utilising the data added into said spreadsheet, instead of generating them ad hoc.
 
 In this way, metadata can be set on XIP Metadata fields, including:
  - Title
  - Description
  - Security Status
  - Identifiers
  - SourceID
 
 As well as XML metadata templates, including the default templates and custom templates.
 
 ### XIP metadata - Title, Description and Security Status
 
-To create the spreadsheet base spreadsheet:
+To use an input override, we need to first create a spreadsheet with the path of. You can utilise the `auto_class` tool installed alongside the Opex Generator.
+
+`auto_class -p "ARCH" "C:\Users\Christopher\Downloads"`
 
-`opex_generate -c catalog -p "ARCH" -ex "C:\Users\Christopher\Downloads"` or `auto_class -p "ARCH" "C:\Users\Christopher\Downloads"` to avoid unnecessary OPEX creation.
+In the resultant spreadsheet, add in "Title", "Description", and "Security" as new columns. The column headers have to match exactly, and are case-sensitive; these fields would then be filled in with the relevant data.
 
-In the resultant spreadsheet, add in "Title", "Description", and "Security" as new columns. The column headers have to match exactly, including capitalisation; these fields would then be filled in with the relevant data.
+![ScreenshotXIPColumns](assets/Column%20Headers.png)
 
 Once the cells are filled in with data; to initialise the generation run: `opex_generate -i "{/path/to/your/spreadsheet.xlsx}" "{/path/to/root/directory}"`
 
 Ensure that the root directory matches the original directory of the export. In the above case this would be: `opex_generate -i "C:\Users\Christopher\Downloads\meta\Downloads_AutoClass.xlsx" "C:\Users\Christopher\Downloads"`
 
-To note, the column headers are drop-in, drop-out, meaning you can the columns as and when you need them. You can also leave blank data,the cell you leave blank will simply not these will not be assigned.
+The column headers are drop-in, drop-out, meaning you can the columns as and when you need them. You can also leave blank data,the cell you leave blank will simply not these will not be assigned.
 
-To also note, the `Security` must match an existing tag in your system, exactly by it's name.
+When assigning the `Security` field, the tag must be a match to an existing tag in your system. This is case-sensitive, so "Closed" will NOT match to a tag called "closed".
 
-To also also note, if there are any changes to the hierarchy data, such as a file/folder (not including a 'meta' folder) being removed or added, after the export of the initial spreadsheet, the data may not be assigned correctly.
+### Important Note
+
+If there are any changes to the hierarchy data, such as a file/folder (not including a 'meta' folder) being removed or added after the export of the spreadsheet, the data may not be assigned correctly, or it may be assigned as "ERROR", or the program may simply fail.
 
 ### XIP Metadata - Identifiers
 
-Custom Identifiers can be added by naming columns: `"Archive_Reference", "Accession_Reference", "Identifier", or "Identifer:Keyname"`.
+Custom Identifiers can be added by adding the columns: `"Archive_Reference", "Accession_Reference", "Identifier", or "Identifer:Keyname"`.
+
+![Identifier Screenshot](assets/Identifiers%20Headers.png)
+
+`Archive_Reference` or `Identifier` will default to the keyname `code`; `Accession_Reference` will default to `accref`. When using the Auto Classification Generator it will always generate a column called `Archive_Reference`, but you can simply rename or remove this column as neccessary. 
+
+To add a custom identifier import, do so like: `Identifier:MyCodeName`. As many identifier's as needed can be added.
+
+No additional parameter's need to be set in the command line when using Identifier's, addition is enabled by default. Leaving a cell blank will use Preservica's defaults.
 
-If named `Archive_Reference` or `Identifier` the keyname will default to `code`, if named `Accession_Reference` the keyname will default to `accref`. Using the Auto Classification Generator will always generate a column called `Archive_Reference`, you can simply rename or remove this column if not needed. 
+### XIP Metadata - Hashes
 
-To add a custom identifier import, do so like so: `Identifier:MyCodeName`. As many identifier's as needed can be added.
+If you utilise the Auto Classification's tool for generating Hashes; when utilising the `-fx` option in combination with `-i`, if the columns `Hash` and `Algorithm` are both present the program will read the hashes from the spreadsheet instead of generating them.
 
-No additional parameter's need to be set in the command line when using Identifier's, addition is detected by default.
+![Hash Screenshot](assets/Hash%20Headers.png)
+
+*Be aware that interruption / resuming is not currently supported with the Auto Class Tool.
 
 ### XML Metadata - Basic Templates
 
-To utilise an import with XML Metadata templates, first the XML template has to be stored in the source 'metadata' directory. DC, MODS, GPDR, and EAD templates come with the package.
+DC, MODS, GPDR, and EAD templates are supported alongside installation of the package.
+
+After exporting an Auto Class spreadsheet, add in additional columns to the spreadsheet; like the XIP data, all fields are optional, and can added on a 'drop-in' basis. 
+
+![XML Headers](assets/XML%20Headers.png)
 
-After exporting an Auto Class spreadsheet, add in additional columns to the spreadsheet; like the XIP data, all fields are optional, and can added on a 'drop-in' basis. You can add in the column header in two ways: 'exactly' or 'flatly'.
+You can add in the column header in two ways: *'exactly'* or *'flatly'*. (There are probably better words to describe this behaviour)
 
-An Exactly match requires that the full path from the XML document is added to the column, with parent to child separated by a `/`; 'flatly' requires only a the matching end tag. For example, the below will match to the same `recordIdentifer` field in the mods template:
+An Exactly match requires that the full path from the XML document is added to the column, with parent to child separated by a `/`; 'flatly' requires only the matching end tag.
+
+To give an example, the below will match to the same `recordIdentifer` field in the mods template:
 
 ```
 Exactly:
 mods:recordInfo/mods:recordIdentifier
 
 Flatly:
 mods:recordIdentifier
 ```
 
-In both cases, the header has to match both namespace and tag and isI case sensitive. While using the flat method is easier, be aware that if there's non-unique tags, such as `mods:note`, the flat method will only import to the first match, which might not be it's intended destination.
+In both cases, the header has to match both the namespace and tag. This is also case sensitive.
+
+While using the flat method is easier, be aware that if there's non-unique tags, such as `mods:note`, the flat method will only import to the first match, which might not be it's intended destination.
 
 When using the 'exactly' and you have non-unique tags, again such as `mods:note`, you will need add an index in square brackets `[0]` to indicate which tag to assign the data to, like: `mods:note[1] mods:notes[2] ...` The number of field will simply be the order they appear in the XML.
 
-This is all probably easier done, than said :\). For convenience I've also included *(Note to self: ADD THEM!)*, spreadsheet templates of DC, MODS, GDPR and EAD, with their explicit names in the headers.
+This is all probably easier done, than said :\). For convenience I've also included full templates for DC, MODS, GDPR and EAD, with their explicit names in the headers [here](opex_manifest_generator/samples/spreads).
 
-Once the above is setup, and all the data added; to create the OPEX's simply add `-m` with the chosen method of import `flat|exact`, so:
+Once you have added in your headers and the necessary data to create the OPEX's simply add `-m` with the chosen method of import `flat|exact`, so:
 `opex_generate -i "{/path/to/your/spreadsheet.xlsx}" "{/path/to/root/directory}" -m flat` or 
 `opex_generate -i "{/path/to/your/spreadsheet.xlsx}" "{/path/to/root/directory}" -m exact`
 
-To note: when you add an XML Metadata column to the XL spreadsheet, it will always add this to the OPEX - even if the cell is left blank... This may be configurable in the future, but for now please be aware of it.
+Be aware that when you add an XML Metadata column to the spreadsheet, it will always add the entire metadata template to the OPEX - even if all the cells are left blank. As this is a useful function (adding blank templates to your import), I will leave this for now, but may adjust this in the future.
 
 ### XML Metadata Templates - Custom Templates
 
-Any custom template can be added to the metadata folder and it will work 'out of the box', as long as they are functioning within Preservica.
+Any custom XML template can be added to the 'metadata' folder in the installation directory. As long as the XML template is functioning in Preservica, it will work 'out of the box'. All XML's in the directory are checked when enabling the `-m` option.
+
+The location of this will depend on the install path utilising by Python; typically it will be under `/path/to/ptyhoninstall/Lib/site-packages/opex_manifest_generator/metadata`
+
+*In the future I will likely allow the destination of this directory to be set by an option or adjustable, for ease of use.*
+
+Then in the spreadsheet you simply need to add matching column headers - you can utilise either flat or exact methods as described above.
+
+### Custom Spreadsheets - Quick Note
+
+You technically don't have to utilise the AutoClass tool at all. Any old spreadsheet will do!
+
+The only requirement to use the input override, is the presence of the `FullName` column. With an accurate list of paths.
 
-All that is necessary to do, is add the XML Template document and then add it to the 'metadata' folder within the site-package files within the program. Then in the spreadsheet you simply need to add neccesary column headers - you can utilise either flat or exact methods as described above. You can then save this as a template for reuse.
+![FullName Column](assets/FullName%20Column.png)
 
-*In the future I will likely allow the destination of this directory to be set by an option or adjustable in one way or aanother, for use without having to go into the Site-Packages.*
+Other columns can be added or removed as needed.
 
 #### Additional Information
 
 A SourceID can also be set by adding a `SourceID` header. The behaviour of this is not fully tested yet.
 
 Ignoring Files can also be set by adding an `Ignore` header. When this is set to `TRUE` this will skip the generation of an Opex for the specified File or Folder; when done for folder's, the folder Opex will still include any ignored file's in its manifest.
 
 Removing Files or Folders is also possible, by adding a `Removals` header. When this is set to `TRUE`, the specified File or Folder will be removed from the system. As a safeguard this must be enabled by adding the parameter `-rm, --remove`, and confirming. *Currently this process is failing...* 
 
-To note when importing a column for an XML Metadata template that needs to be a boolean IE `TRUE/FALSE`. Please ensure that none are left blank, otherwise these may be imported inaccurately as `1.0` or `0.0`. This is a pandas issue, that I'm not sure how to fix... :/
+To note when importing a column for an XML Metadata template that needs to be a boolean IE `TRUE/FALSE`. Please ensure that no cells are left blank, otherwise these may be imported inaccurately as `1.0` or `0.0`. This is a pandas issue, that I'm not sure how to fix... :/
 
 ## Options
 
 The following options are currently available to run the program with, and can be utilised in various combinations with each other, although some combinations will clash:
 
 ```
 Options:
@@ -314,28 +354,29 @@
         -fmt,   --format    Set whether to export as a CSV or XLSX file.            {csv,xlsx}
                             Otherwise defaults to xlsx.
 
 ```
 
 ## Future Developments
 
+- Customisable Filtering
 - Adjust Accession so the different modes can utilised from Opex.
-- Add SourceID as option for use with Auto Class Spreadsheets.
-- Allow for multiple Identifier's to be added with Auto Class Spreadsheets. Currently only 1 or 2 identifiers can be added at a time, under "Archive_Reference" or "Accesion_Refernce". These are also tied to be either "code" or "accref". An Option needs to be added to allow custom setting of identifier...
-- Zipping to conform to PAX, 
+- Add SourceID as option for use with Auto Class Spreadsheets. *Added!*
+- Allow for multiple Identifier's to be added with Auto Class Spreadsheets. Currently only 1 or 2 identifiers can be added at a time, under "Archive_Reference" or "Accesion_Refernce". These are also tied to be either "code" or "accref". An Option needs to be added to allow custom setting of identifier... *Added!*
+- Zipping to conform to PAX
 - Add an option / make it a default for Metadata XML's to be located in a specified directory rather than in the package.
 - In theory, this tool should be compatible with any system that makes use of the OPEX standard. But in theory Communism works, in theory.
 
 ## Developers
 
-You should also be able to embed the program into Python a Script. Though be warned I haven't tested this functionally much!
+You should also be able to embed the program directly in Python. Though be warned I haven't tested this functionally much!
 
 ```
 from opex_manifest_generator import OpexManifestGenerator as OMG
  
-OMG(root="/my/directory/path", fixity_flag= True, algorithm = "SHA-256").main()
+OMG(root="/my/directory/path", algorithm = "SHA-256").main()
 
 ```
 
 ## Contributing
 
 I welcome further contributions and feedback.
```

### Comparing `opex_manifest_generator-1.1.4/opex_manifest_generator/cli.py` & `opex_manifest_generator-1.1.5/opex_manifest_generator/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 license: Apache License 2.0"
 """
 
 import argparse
 import os
 import time
 from opex_manifest_generator.opex_manifest import OpexManifestGenerator
-from opex_manifest_generator.version import __version__
-import inspect
+import importlib.metadata
 
 def parse_args():
     parser = argparse.ArgumentParser(description="OPEX Manifest Generator for Preservica Uploads")
     parser.add_argument('root',default=os.getcwd())
     parser.add_argument("-c","--autoclass",required=False,choices=['catalog','c','accession','a','both','b','generic','g','catalog-generic','cg',"accession-generic","ag","both-generic","bg"],type=str.lower)
     parser.add_argument("-p","--prefix",required=False, nargs='+')
     parser.add_argument("-fx","--fixity",required=False,const="SHA-1",default=None, nargs='?', choices=['NONE','SHA-1','MD5','SHA-256','SHA-512'],type=str.upper)
@@ -25,15 +24,15 @@
     parser.add_argument("-m","--metadata",required=False,const='e',default='none',nargs='?',choices=['none','n','exact','e','flat','f'],type=str.lower)
     parser.add_argument("-dmd", "--disable-meta-dir",required=False,action='store_false')
     parser.add_argument("-ex","--export",required=False,action='store_true',default=False)
     parser.add_argument("-i","--input",required=False)
     parser.add_argument("-rm","--remove",required=False,action="store_true",default=False)
     parser.add_argument("-z","--zip", required=False,action='store_true')
     parser.add_argument("-fmt", "--output-format",required=False,default="xlsx", choices=['xlsx','csv'])
-    parser.add_argument("-v", "--version",action='version',version='%(prog)s {version}'.format(version=__version__))
+    parser.add_argument("-v", "--version",action='version',version='%(prog)s {version}'.format(version=importlib.metadata.version("opex_manifest_generator")))
     parser.add_argument("--hidden",required=False,action='store_true',default=False)
     args = parser.parse_args()
     return args
 
 def run_cli():
     args = parse_args()
     os.chdir(args.root)
```

### Comparing `opex_manifest_generator-1.1.4/opex_manifest_generator/common.py` & `opex_manifest_generator-1.1.5/opex_manifest_generator/common.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.4/opex_manifest_generator/hash.py` & `opex_manifest_generator-1.1.5/opex_manifest_generator/hash.py`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.4/opex_manifest_generator/metadata/DublinCore Template.xml` & `opex_manifest_generator-1.1.5/opex_manifest_generator/metadata/DublinCore Template.xml`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.4/opex_manifest_generator/metadata/EAD Template.xml` & `opex_manifest_generator-1.1.5/opex_manifest_generator/metadata/EAD Template.xml`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.4/opex_manifest_generator/metadata/MODS Template.xml` & `opex_manifest_generator-1.1.5/opex_manifest_generator/metadata/MODS Template.xml`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.4/opex_manifest_generator/opex_manifest.py` & `opex_manifest_generator-1.1.5/opex_manifest_generator/opex_manifest.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,163 +70,213 @@
         self.metadata_flag = metadata_flag
         self.metadata_dir = metadata_dir
         
     def print_running_time(self):
         print(f'Running time: {datetime.now() - self.start_time}')
         time.sleep(1)
     
-    def index_df_lookup(self,file_path: str):
-        idx = self.df['FullName'].index[self.df['FullName'] == file_path]
-        return idx 
-
-    def meta_df_lookup(self, file_path: str, idx):
-        #idx = self.df.index[self.df['FullName'] == file_path]
-        if idx.empty:
-            title = None
-            description = None
-            security = None
-        else:
-            try:
-                if self.title_flag:
-                    title = self.df['Title'].loc[idx].item()
-                    if str(title).lower() in {"nan","nat"}: title = None
-                else: title = None
-                if self.description_flag: 
-                    description = self.df['Description'].loc[idx].item()
-                    if str(description).lower() in {"nan","nat"}: description = None
-                else: description = None
-                if self.security_flag: 
-                    security = self.df['Security'].loc[idx].item()
-                    if str(security).lower() in {"nan","nat"}: security = None
-                else: security = None
-            except Exception as e:
-                print(e)
-                raise SystemError()
-        return title,description,security
+    def index_df_lookup(self, path: str):
+        idx = self.df['FullName'].index[self.df['FullName'] == path]
+        return idx
+
+    def meta_df_lookup(self, idx):
+        try:
+            if idx.empty:
+                title = None
+                description = None
+                security = None
+            else:
+                    if self.title_flag:
+                        title = self.df['Title'].loc[idx].item()
+                        if str(title).lower() in {"nan","nat"}: title = None
+                    else: title = None
+                    if self.description_flag: 
+                        description = self.df['Description'].loc[idx].item()
+                        if str(description).lower() in {"nan","nat"}: description = None
+                    else: description = None
+                    if self.security_flag: 
+                        security = self.df['Security'].loc[idx].item()
+                        if str(security).lower() in {"nan","nat"}: security = None
+                    else: security = None
+            return title,description,security
+        except Exception as e:
+            print('Error Looking up XIP Metadata')
+            print(e)
     
-    def remove_df_lookup(self, file_path: str,idx):
-        #idx = self.df.index[self.df['FullName'] == file_path]
-        if idx.empty: return False
-        else:
-            remove = self.df['Removals'].loc[idx].item()
-            if str(remove).lower() in {"nan","nat"}: return False
-            elif bool(remove):
-                print(f"Removing: {file_path}")
-                # Not functioning correctly
-                if os.path.isdir(file_path): shutil.rmtree(dir)
-                else: os.remove(file_path)
-                return True
-            else: return False
+    def remove_df_lookup(self, path: str, idx):
+        try:
+            if idx.empty:
+                return False
+            else:
+                remove = self.df['Removals'].loc[idx].item()
+                if str(remove).lower() in {"nan","nat"}:
+                    return False
+                elif bool(remove):
+                    print(f"Removing: {path}")
+                    # Not functioning correctly
+                    if os.path.isdir(path):
+                        shutil.rmtree(path)
+                    else:
+                        os.remove(path)
+                    return True
+                else:
+                    return False
+        except Exception as e:
+            print('Error looking up Removals')
+            print(e)
                 
-    def ignore_df_lookup(self, file_path: str, idx):
-        #idx = self.df.index[self.df['FullName'] == file_path]
-        if idx.empty: return False
-        else: ignore = self.df['Ignore'].loc[idx].item()
-        if str(ignore).lower() in {"nan","nat"}: return False
-        elif str(ignore).lower() in {"true"}: return True
-        else: return False
-
-    def sourceid_df_lookup(self, xml_element, file_path: str, idx):
-        #idx = self.df.index[self.df['FullName'] == file_path]
-        if idx.empty: pass
-        else:
-            sourceid = self.df['SourceID'].loc[idx].item()
-            if str(sourceid) in {"nan","nat"}: pass
+    def ignore_df_lookup(self, idx):
+        try:
+            if idx.empty:
+                return False
+            else:
+                ignore = self.df['Ignore'].loc[idx].item()
+            if str(ignore).lower() in {"nan","nat"}:
+                return False
+            elif str(ignore).lower() in {"true", "1.0"}:
+                return True
+            elif str(ignore).lower() in {"false", "0.0"}:
+                return False
+        except Exception as e:
+            print('Error looking up Removals')
+            print(e)
+
+    def sourceid_df_lookup(self, xml_element, idx):
+        try:
+            if idx.empty:
+                pass
             else:
-                source_xml = ET.SubElement(xml_element,f"{{{self.opexns}}}SourceID")
-                source_xml.text = str(sourceid)
+                sourceid = self.df['SourceID'].loc[idx].item()
+                if str(sourceid) in {"nan","nat"}:
+                    pass
+                else:
+                    source_xml = ET.SubElement(xml_element,f"{{{self.opexns}}}SourceID")
+                    source_xml.text = str(sourceid)
+        except Exception as e:
+            print('Error looking up SourceID')
+            print(e)
 
     def hash_df_lookup(self, file_path, xml_fixities, idx):
-        #idx = self.df.index[self.df['FullName'] == file_path]
-        if idx.empty: pass
-        else:
-            if "Hash" in self.column_headers and "Algorithm" in self.column_headers:
-                self.fixity = ET.SubElement(xml_fixities,f"{{{self.opexns}}}Fixity")        
-                self.hash = self.df["Hash"].loc[idx].item()
-                self.algorithm = self.df["Algorithm"].loc[idx].item()
-                self.hash = HashGenerator(algorithm=self.algorithm).hash_generator(file_path)
-                self.fixity.set("type", self.algorithm)
-                self.fixity.set("value",self.hash)
-            else: pass
-
-    def ident_df_lookup(self, file_path, idx):
-        #idx = self.df.index[self.df['FullName'] == file_path]
-        if idx.empty:
-            ident = "ERROR"
-            self.identifier = ET.SubElement(self.identifiers,f"{{{self.opexns}}}Identifier") 
-            self.identifier.set("type","code")
-            self.identifier.text = ident
-        else:
-            for header in self.column_headers:
-                if any(s in header for s in {'Identifier','Archive_Reference','Accession_Reference'}):
-                    ident = self.df[header].loc[idx].item()
-                    if 'Identifier:' in header: code_name = str(header).rsplit(':')[-1]
-                    elif 'Archive_Reference' in header: code_name = "code"
-                    elif 'Accession_Reference' in header: code_name = "accref"
-                else: ident = None
-                if str(ident).lower() in {"nan","nat"} or not ident: pass
+        try:
+            if idx.empty:
+                pass
+            else:
+                if "Hash" in self.column_headers and "Algorithm" in self.column_headers:
+                    self.fixity = ET.SubElement(xml_fixities,f"{{{self.opexns}}}Fixity")        
+                    self.hash = self.df["Hash"].loc[idx].item()
+                    self.algorithm = self.df["Algorithm"].loc[idx].item()
+                    self.hash = HashGenerator(algorithm=self.algorithm).hash_generator(file_path)
+                    self.fixity.set("type", self.algorithm)
+                    self.fixity.set("value",self.hash)
+        except Exception as e:
+            print('Error looking up Removals')
+            print(e)
+
+    def ident_df_lookup(self, idx, key_override = None):
+        try:
+            if idx.empty:
+                ident = "ERROR"
+                self.identifier = ET.SubElement(self.identifiers,f"{{{self.opexns}}}Identifier") 
+                if key_override is None:
+                    key_name = "code"
                 else:
-                    self.identifier = ET.SubElement(self.identifiers,f"{{{self.opexns}}}Identifier") 
-                    self.identifier.set("type",code_name)
-                    self.identifier.text = str(ident)
+                    key_name = key_override
+                self.identifier.set("type",key_name)
+                self.identifier.text = ident
+            else:
+                for header in self.column_headers:
+                    if any(s in header for s in {'Identifier','Archive_Reference','Accession_Reference'}):
+                        ident = self.df[header].loc[idx].item()
+                        if 'Identifier:' in header:
+                            key_name = str(header).rsplit(':')[-1]
+                        elif key_override is None:
+                            if 'Archive_Reference' in header:
+                                key_name = "code"
+                            elif 'Accession_Reference' in header:
+                                key_name = "accref"
+                            elif 'Identifier' in header:
+                                key_name = "code"
+                        else: 
+                            key_name = key_override
+                    else: ident = None
+                    if str(ident).lower() in {"nan","nat"} or not ident: pass
+                    else:
+                        self.identifier = ET.SubElement(self.identifiers,f"{{{self.opexns}}}Identifier") 
+                        self.identifier.set("type",key_name)
+                        self.identifier.text = str(ident)
+        except Exception as e:
+            print('Error looking up Identifiers')
+            print(e)            
     
-    def check_opex(self,opex_path):
-        if os.path.exists(win_256_check(opex_path)): return False
-        else: return True
-
-    def write_opex(self,file_path,opexxml):
-        opex_path = str(win_256_check(file_path)) + ".opex"
-        opex = ET.indent(opexxml,"  ")
-        opex = ET.tostring(opexxml,pretty_print=True,xml_declaration=True,encoding="UTF-8",standalone=True)
-        with open(f'{opex_path}','w',encoding="UTF-8") as writer:
+    def check_opex(self, opex_path):
+        if os.path.exists(win_256_check(opex_path)):
+            return False
+        else:
+            return True
+
+    def write_opex(self, path, opexxml):
+        opex_path = str(win_256_check(path)) + ".opex"
+        opex = ET.indent(opexxml, "  ")
+        opex = ET.tostring(opexxml, pretty_print=True, xml_declaration=True, encoding="UTF-8", standalone=True)
+        with open(f'{opex_path}', 'w', encoding="UTF-8") as writer:
             writer.write(opex.decode('UTF-8'))
             print('Saved Opex File to: ' + opex_path)
         return opex_path
 
     def init_df(self):
         if self.autoclass_flag:
-            if self.autoclass_flag in {"catalog","c","catalog-generic","cg"}:
-                ac = ClassificationGenerator(self.root,output_path=self.output_path,prefix=self.prefix,start_ref=self.startref,empty_flag=self.empty_flag,accession_flag=False)
-            elif self.autoclass_flag in {"accession","a","accession-generic","ag","both","b","both-generic","bg"}:
-                ac = ClassificationGenerator(self.root,output_path=self.output_path,prefix=self.prefix,accprefix=self.acc_prefix,start_ref=self.startref,empty_flag=self.empty_flag,accession_flag="File")
+            if self.autoclass_flag in {"catalog", "c", "catalog-generic", "cg"}:
+                ac = ClassificationGenerator(self.root, output_path = self.output_path, prefix = self.prefix, start_ref = self.startref, empty_flag = self.empty_flag, accession_flag = False)
+            elif self.autoclass_flag in {"accession", "a", "accession-generic", "ag", "both", "b", "both-generic", "bg"}:
+                ac = ClassificationGenerator(self.root, output_path = self.output_path, prefix = self.prefix, accprefix = self.acc_prefix, start_ref = self.startref, empty_flag = self.empty_flag, accession_flag="File")
             self.df = ac.init_dataframe()
-            if self.autoclass_flag in {"accession","a","accesion-generic","ag"}:
+            if self.autoclass_flag in {"accession", "a", "accesion-generic", "ag"}:
                 self.df = self.df.drop('Archive_Reference',axis=1)
             self.column_headers = self.df.columns.values.tolist()
             if self.export_flag:
-                output_path = define_output_file(self.output_path,self.root,meta_dir_flag=self.meta_dir_flag,output_format=self.output_format)                
-                if self.output_format == "xlsx": export_xl(self.df,output_path)
-                elif self.output_format == "csv": export_csv(self.df,output_path)
+                output_path = define_output_file(self.output_path, self.root, meta_dir_flag = self.meta_dir_flag, output_format = self.output_format)                
+                if self.output_format == "xlsx":
+                    export_xl(self.df, output_path)
+                elif self.output_format == "csv":
+                    export_csv(self.df, output_path)
         elif self.input:
-            if self.input.endswith('xlsx'): self.df = pd.read_excel(self.input)
-            elif self.input.endswith('csv'): self.df = pd.read_csv(self.input)
+            if self.input.endswith('xlsx'):
+                self.df = pd.read_excel(self.input)
+            elif self.input.endswith('csv'):
+                self.df = pd.read_csv(self.input)
             self.column_headers = self.df.columns.values.tolist()
-            self.set_flags()
+            self.set_input_flags()
         else:
             self.df = None
             self.column_headers = None
                 
     def clear_opex(self):
         walk = list(os.walk(self.root))
         for dir,_,files in walk[::-1]:
             for file in files:
                 file_path = win_256_check(os.path.join(dir,file))   
                 if str(file_path).endswith('.opex'):
                     os.remove(file_path)
                     print(f'Cleared Opex: {file_path}')
     
-    def set_flags(self):
-        if 'Title' in self.df: self.title_flag = True
-        if 'Description' in self.df: self.description_flag = True
-        if 'Security' in self.df: self.security_flag = True
-        if 'SourceID' in self.df: self.sourceid_flag = True
-        if 'Ignore' in self.df: self.ignore_flag = True
-        if 'Hash' in self.df and 'Algorithm' in self.df:
+    def set_input_flags(self):
+        if 'Title' in self.column_headers:
+            self.title_flag = True
+        if 'Description' in self.column_headers:
+            self.description_flag = True
+        if 'Security' in self.column_headers:
+            self.security_flag = True
+        if 'SourceID' in self.column_headers:
+            self.sourceid_flag = True
+        if 'Ignore' in self.column_headers:
+            self.ignore_flag = True
+        if 'Hash' in self.column_headers and 'Algorithm' in self.column_headers:
             self.hash_from_spread = True
-            print("Hash detected in Spreadsheet; taking hashes from spreadsheet");time.sleep(3)
+            print("Hash detected in Spreadsheet; taking hashes from spreadsheet")
+            time.sleep(3)
 
     def print_descriptive_xmls(self):
         for file in os.scandir(self.metadata_dir):
             path = os.path.join(self.metadata_dir,file.name)
             print(path)
             xml_file = ET.parse(path)
             root_element = ET.QName(xml_file.find('.'))
@@ -265,23 +315,22 @@
                 list_xml = []
                 for elem_dict in elements_list:
                     if elem_dict.get('Name') in self.column_headers or elem_dict.get('Path') in self.column_headers:
                         list_xml.append({"Name":elem_dict.get('Name'),"Namespace":elem_dict.get('Namespace'),"Path":elem_dict.get('Path')})
             if len(list_xml) > 0:
                 self.xml_files.append({'data':list_xml, 'localname':root_element_ln, 'xmlfile': path})
 
-    def generate_descriptive_metadata(self,xml_desc,file_path, idx):
+    def generate_descriptive_metadata(self,xml_desc, idx):
         for xml_file in self.xml_files:
             list_xml = xml_file.get('data')
             localname = xml_file.get('localname')
             """
             Composes the data into an xml file.
             """
             if len(list_xml):
-                #idx = self.df.index[self.df['FullName'] == file_path]
                 if not idx.empty:
                     xml_new = ET.parse(xml_file.get('xmlfile'))
                     for elem_dict in list_xml:
                         name = elem_dict.get('Name')
                         path = elem_dict.get('Path')
                         ns = elem_dict.get('Namespace')
                         try:
@@ -294,62 +343,63 @@
                                 if is_datetime64_any_dtype(val):
                                     val = pd.to_datetime(val)
                                     val = datetime.strftime(val,"%Y-%m-%dT%H-%M-%S.00Z")
                         except KeyError as e:
                             print('Key Error: please ensure column header\'s are an exact match...')
                             print(f'Missing Column: {e}')
                             print('Alternatively use flat mode...')
-                            time.sleep(5)
+                            time.sleep(3)
                             raise SystemError()
                         except IndexError as e:
                             print("""Index Error; it is likely you have removed or added a file/folder to the directory \
                                 after generating the spreadsheet. An opex will still be generated but with no xml metadata. \
                                 To ensure metadata match up please regenerate the spreadsheet...""")
                             print(f'Error: {e}')
-                            time.sleep(1)
+                            time.sleep(3)
                             break
-                        if str(val).lower() in {"nan","nat"}: continue
+                        if str(val).lower() in {"nan","nat"}:
+                            continue
                         if self.metadata_flag in {'e','exact'}:
                             n = path.replace(localname + ":", f"{{{ns}}}")
                             elem = xml_new.find(f'/{n}')
                         elif self.metadata_flag in {'f','flat'}:
                             n = name.split(':')[-1]
                             elem = xml_new.find(f'//{{{ns}}}{n}')
                         elem.text = str(val)    
                     xml_desc.append(xml_new.find('.'))
                 else: pass
             else: pass
 
-    def generate_opex_properties(self,xmlroot,file_path, idx, title=None,description=None,security=None):
+    def generate_opex_properties(self, xmlroot, idx, title=None,description=None,security=None):
         self.properties = ET.SubElement(xmlroot,f"{{{self.opexns}}}Properties")
         self.identifiers = ET.SubElement(self.properties,f"{{{self.opexns}}}Identifiers")
         if title:
             self.titlexml = ET.SubElement(self.properties,f"{{{self.opexns}}}Title")
             self.titlexml.text = str(title)
         if description:
             self.descriptionxml = ET.SubElement(self.properties,f"{{{self.opexns}}}Description")
             self.descriptionxml.text = str(description)      
         if security:
             self.securityxml = ET.SubElement(self.properties,f"{{{self.opexns}}}SecurityDescriptor")
             self.securityxml.text = str(security)
         if self.autoclass_flag in {"generic","g"}:
             self.properties.remove(self.identifiers)
         elif self.autoclass_flag or self.input:
-            self.ident_df_lookup(file_path, idx)
+            self.ident_df_lookup(idx)
         if self.identifiers is None:
             self.properties.remove(self.identifiers)
         if self.properties is None:
             xmlroot.remove(self.properties)
 
-    def genererate_opex_fixity(self,file_path):
-        self.fixity = ET.SubElement(self.fixities,f"{{{self.opexns}}}Fixity")        
+    def genererate_opex_fixity(self, file_path):
+        self.fixity = ET.SubElement(self.fixities, f"{{{self.opexns}}}Fixity")        
         self.hash = HashGenerator(algorithm=self.algorithm).hash_generator(file_path)
         self.fixity.set("type", self.algorithm)
-        self.fixity.set("value",self.hash)
-        self.OMG.list_fixity.append([self.algorithm,self.hash,file_path])
+        self.fixity.set("value", self.hash)
+        self.OMG.list_fixity.append([self.algorithm, self.hash, file_path])
         self.OMG.list_path.append(file_path)
 
     def main(self):
         print(f"Start time: {self.start_time}")        
         if self.clear_opex_flag:
             self.clear_opex()
             if self.autoclass_flag or self.algorithm or self.input:
@@ -379,19 +429,19 @@
             self.folder_path = folder_path.replace(u'\\\\?\\',"")
         else:
             self.folder_path = folder_path
         if self.OMG.input or not self.OMG.autoclass_flag in {"g","generic"} or self.OMG.ignore_flag or self.OMG.remove_flag or self.OMG.sourceid_flag or self.OMG.title_flag or self.OMG.description_flag or self.OMG.security_flag:
             self.index = self.OMG.index_df_lookup(self.folder_path)
         if self.OMG.ignore_flag or self.OMG.remove_flag:
             if self.OMG.ignore_flag:
-                self.ignore = self.OMG.ignore_df_lookup(folder_path,self.index)
+                self.ignore = self.OMG.ignore_df_lookup(self.index)
                 if self.ignore:
                     return
             if self.OMG.remove_flag:
-                self.removal = self.OMG.remove_df_lookup(self.folder_path,self.index)
+                self.removal = self.OMG.remove_df_lookup(self.folder_path, self.index)
                 if self.removal:
                     return        
         else:
             self.ignore = False
             self.removal = False
 
         self.xmlroot = ET.Element(f"{{{self.opexns}}}OPEXMetadata",nsmap={"opex":self.opexns})
```

### Comparing `opex_manifest_generator-1.1.4/opex_manifest_generator/samples/opex_manifest_generator_AutoClass.xlsx` & `opex_manifest_generator-1.1.5/opex_manifest_generator/samples/opex_manifest_generator_AutoClass.xlsx`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-00000000: 504b 0304 1400 0600 0800 0000 2100 df73  PK..........!..s
-00000010: 5b55 9b01 0000 1d07 0000 1300 eb01 5b43  [U............[C
+00000000: 504b 0304 1400 0600 0800 0000 2100 0b39  PK..........!..9
+00000010: 366e 8b01 0000 1d07 0000 1300 0802 5b43  6n............[C
 00000020: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
-00000030: 6c20 a2e7 0128 a000 0200 0000 0000 0000  l ...(..........
+00000030: 6c20 a204 0228 a000 0200 0000 0000 0000  l ...(..........
 00000040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -27,45 +27,45 @@
 000001a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000210: 0000 0000 0000 0000 0000 0000 bc95 4d4f  ..............MO
-00000220: c240 1086 ef26 fe87 66af 862e a031 c650  .@...&..f....1.P
-00000230: 3cf8 7154 1331 f1ba 7607 ba61 bfb2 3328  <.qT.1..v..a..3(
-00000240: fc7b b70b 1443 1050 8897 6eda cebc efb3  .{...C.P..n.....
-00000250: 33dd 69ef 666a 74f6 0101 95b3 05eb e46d  3.i.fjt........m
-00000260: 9681 2d9d 5476 54b0 d7c1 43eb 8a65 48c2  ..-.TvT...C..eH.
-00000270: 4aa1 9d85 82cd 00d9 4dff f4a4 3798 79c0  J.......M...7.y.
-00000280: 2c66 5b2c 5845 e4af 39c7 b202 2330 771e  ,f[,XE..9...#0w.
-00000290: 6c7c 3374 c108 8ab7 61c4 bd28 c762 04bc  l|3t....a..(.b..
-000002a0: db6e 5ff2 d259 024b 2daa 3558 bf77 0743  .n_..Y.K-.5X.w.C
-000002b0: 31d1 94dd 4fe3 e339 4900 8d2c bb9d 07d6  1...O..9I..,....
-000002c0: 5e05 13de 6b55 0a8a a4fc c3ca 3597 d6c2  ^...kU......5...
-000002d0: 218f 9929 062b e5f1 2c62 30be d1a1 7ef3  !..).+..,b0...~.
-000002e0: b3c1 22ef 2996 2628 09d9 b308 f428 4cc4  ..".).&(.....(L.
-000002f0: e053 cd3f 5d18 bf3b 37ce b78b 6ca0 74c3  .S.?]..;7...l.t.
-00000300: a12a 41ba 7262 6205 72f4 0184 c40a 808c  .*A.rbb.r.......
-00000310: ced3 9a1b a1ec 927b 8b7f 0a46 9e96 ce91  .......{...F....
-00000320: 41ea fd25 e11d 1c14 fb0d 3c5d 0f47 4832  A..%......<].GH2
-00000330: 3b0c 9166 1af0 c8bb 9d8b ee72 ae44 00f9  ;..f.......r.D..
-00000340: 4221 9e8c a303 7cd7 dec6 514e 909c 7933  B!....|...QN..y3
-00000350: 9a2b 02f3 1c9c c7c3 ebde 88d6 7a10 4841  .+..........z.HA
-00000360: 736c 367d 7e4d f88a a17b 7043 1ad1 3f33  sl6}~M...{pC..?3
-00000370: 9cff 3743 3cc3 a901 719a 05f8 bdf9 725c  ..7C<...q.....r\
-00000380: d5d9 2dbf 57e5 1bc7 3809 7f6f b836 79a0  ..-.W...8..o.6y.
-00000390: 9eb5 12e4 9ede 4d83 565d bf38 98a1 11dd  ......M.V].8....
-000003a0: afeb cdfe e779 47b2 df50 009e 7e6e fd2f  .....yG..P..~n./
-000003b0: 0000 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-000003c0: 0000 0021 0013 5ebe 6505 0100 00df 0200  ...!..^.e.......
-000003d0: 000b 00f7 015f 7265 6c73 2f2e 7265 6c73  ....._rels/.rels
-000003e0: 20a2 f301 28a0 0002 0000 0000 0000 0000   ...(...........
-000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000230: 0000 0000 0000 0000 00cc 95c9 4ec3 3010  ............N.0.
+00000240: 86ef 48bc 43e4 2b6a 5c16 2184 9a72 6039  ..H.C.+j\.!..r`9
+00000250: 4225 8ac4 d5c4 d3c6 aa37 79a6 d0be 3d8e  B%.......7y...=.
+00000260: bb08 a1d0 5225 425c 6225 f6fc ffe7 197b  ....R%B\b%.....{
+00000270: 32b8 5918 9dbd 4340 e56c c14e f33e cbc0  2.Y...C@.l.N.>..
+00000280: 964e 2a3b 2dd8 cbf8 a177 c532 2461 a5d0  .N*;-....w.2$a..
+00000290: ce42 c196 80ec 6678 7c34 182f 3d60 16a3  .B....fx|4./=`..
+000002a0: 2d16 ac22 f2d7 9c63 5981 1198 3b0f 36ce  -.."...cY...;.6.
+000002b0: 4c5c 3082 e26b 9872 2fca 9998 023f ebf7  L\0..k.r/....?..
+000002c0: 2f79 e92c 81a5 1ed5 1a6c 38b8 8389 986b  /y.,.....l8....k
+000002d0: caee 17f1 f38a 2480 4696 ddae 16d6 5e05  ......$.F.....^.
+000002e0: 13de 6b55 0a8a a4fc ddca 6f2e bdb5 431e  ..kU......o...C.
+000002f0: 23d3 1aac 94c7 9388 c178 a343 3df3 b3c1  #........x.C=...
+00000300: 3aee 29a6 2628 09d9 4804 7a14 2662 f085  :.).&(..H.z.&b..
+00000310: e61f 2ecc de9c 9be5 bb45 1a28 dd64 a24a  .........E.(.d.J
+00000320: 90ae 9c9b 9881 1c7d 0021 b102 20a3 f334  .......}.!.. ..4
+00000330: e646 28bb e1de e19f 1623 4fc3 69c7 20f5  .F(......#O.i. .
+00000340: fe92 f01e 0e8a f506 9e9e ed11 92cc 1e43  ...............C
+00000350: a4a5 06ec 3aed 4974 9f73 2502 c867 0af1  ....:.It.s%..g..
+00000360: 6674 0ef0 557b 1747 3947 72e6 d568 ae08  ft..U{.G9Gr..h..
+00000370: cc28 388f edf3 be15 adf5 2090 82ed b569  .(8....... ....i
+00000380: 3a7e 0d0c 67ad 0bd2 9ee1 fc1f 305c fc35  :~..g.......0\.5
+00000390: 43ec 23e9 10c4 8e1a e070 f34d cbac a37b  C.#......p.M...{
+000003a0: fe57 d5df 3ac6 6edc 7ab7 50f7 7b09 f250  .W..:.n.z.P.{..P
+000003b0: efd5 69e9 28d9 0de6 3cfd dc86 9f00 0000  ..i.(...<.......
+000003c0: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+000003d0: 2100 135e be65 0201 0000 df02 0000 0b00  !..^.e..........
+000003e0: 0802 5f72 656c 732f 2e72 656c 7320 a204  .._rels/.rels ..
+000003f0: 0228 a000 0200 0000 0000 0000 0000 0000  .(..............
 00000400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -87,1256 +87,1256 @@
 00000560: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000570: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000005a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000005b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000005c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000005d0: 0000 0000 0000 00ac 92cf 4ec3 300c c6ef  ..........N.0...
-000005e0: 48bc 4394 fbea 6e20 84d0 d25d 26a4 dd10  H.C...n ...]&...
-000005f0: 2a0f 6012 f78f dac6 5192 41f7 f604 2404  *.`.....Q.A...$.
-00000600: 9546 bb03 c7d8 9f3f fffc 29db dd38 f4e2  .F.....?..)..8..
-00000610: 8d7c 68d9 2ab9 ce72 29c8 6a36 adad 957c  .|h.*..r).j6...|
-00000620: 291f 57f7 5284 88d6 60cf 9694 3c51 90bb  ).W.R...`...<Q..
-00000630: e2fa 6afb 4c3d c634 149a d605 915c 6c50  ..j.L=.4.....\lP
-00000640: b289 d13d 0004 ddd0 8021 6347 3675 2af6  ...=.....!cG6u*.
-00000650: 03c6 f4f4 3538 d41d d604 9b3c bf03 ffdb  ....58.....<....
-00000660: 4316 134f 7130 4afa 83b9 91a2 3cb9 b479  C..Oq0J.....<..y
-00000670: d99b abaa d5b4 677d 1cc8 c633 2b80 c648  ......g}...3+..H
-00000680: d690 5939 9fd8 7c6c d335 a244 5f53 54d2  ..Y9..|l.5.D_ST.
-00000690: b07e 4ae5 00e8 5c96 b025 9c27 da5c 4ef4  .~J...\..%.'.\N.
-000006a0: f7b5 3050 4483 1141 b3a7 799e 4fc5 1cd0  ..0PD..A..y.O...
-000006b0: fa72 a0e5 88a6 8a9f 74c6 1ede d977 afcc  .r......t....w..
-000006c0: dd1c cbed 7fb2 e863 883c 2c84 f3a5 f946  .......c.<,....F
-000006d0: 82c9 b72c 3e00 0000 ffff 0300 504b 0304  ...,>.......PK..
-000006e0: 1400 0600 0800 0000 2100 f938 46ef df02  ........!..8F...
-000006f0: 0000 6b06 0000 0f00 0000 786c 2f77 6f72  ..k.......xl/wor
-00000700: 6b62 6f6f 6b2e 786d 6ca4 556d 6fda 3010  kbook.xml.Umo.0.
-00000710: fe3e 69ff c1f2 f7e0 3884 14a2 d229 25a0  .>i.....8....)%.
-00000720: 555a 27d4 d78f 9549 0cb1 9ad8 99ed 0055  UZ'....I.......U
-00000730: b5ff be73 02b4 1d9a d4b5 11f8 ede0 f173  ...s...........s
-00000740: 77cf 5d4e bf6d ab12 adb9 3642 c931 a63d  w.]N.m....6B.1.=
-00000750: 1f23 2e33 950b b91a e3db 9b99 37c4 c858  .#.3........7..X
-00000760: 2673 562a c9c7 f889 1bfc edec eb97 d38d  &sV*............
-00000770: d28f 0ba5 1e11 0048 33c6 85b5 754c 88c9  .......H3...uL..
-00000780: 0a5e 31d3 5335 9760 592a 5d31 0b5b bd22  .^1.S5.`Y*]1.[."
-00000790: a6d6 9ce5 a6e0 dc56 2509 7c3f 2215 1312  .......V%.|?"...
-000007a0: 7708 b17e 0f86 5a2e 45c6 5395 3515 97b6  w..~..Z.E.S.5...
-000007b0: 03d1 bc64 16e8 9b42 d466 8f56 65ef 81ab  ...d...B.f.Ve...
-000007c0: 987e 6c6a 2f53 550d 100b 510a fbd4 8262  .~lj/SU...Q....b
-000007d0: 5465 f1c5 4a2a cd16 25b8 bda5 03b4 d5f0  Te..J*..%.......
-000007e0: 89e0 4b7d 1882 fd4d 603a baaa 1299 5646  ..K}...M`:....VF
-000007f0: 2d6d 0fa0 4947 fac8 7fea 134a df84 607b  -m..IG.....J..`{
-00000800: 1c83 f721 8544 f3b5 7039 3cb0 d2d1 0759  ...!.D..p9<....Y
-00000810: 4507 ace8 058c fa9f 46a3 20ad 562b 3104  E.......F. .V+1.
-00000820: ef83 6883 03b7 009f 9d2e 45c9 ef3a e922  ..h.......E..:."
-00000830: 56d7 3f59 e532 5562 5432 63a7 b9b0 3c1f  V.?Y.2UbT2c...<.
-00000840: e313 d8aa 0d7f 73a0 9bfa bc11 2558 8393  ......s.....%X..
-00000850: a04f 3139 3bc8 79ae 6103 b94f 4acb b564  .O19;.y.a..OJ..d
-00000860: 964f 94b4 20b5 1df5 cfca aac5 9e14 0a44  .O.. ..........D
-00000870: 8cae f8af 4668 0eb5 0312 0277 6064 59cc  ....Fh.....w`dY.
-00000880: 1666 ce6c 811a 5d76 4132 5055 8d04 57a1  .f.l..]vA2PU..W.
-00000890: 4a7b a660 9ad7 4ac8 4e59 96b3 ca90 dbe4  J{.`..J.NY......
-000008a0: eaf2 c6ad c063 92e8 ac10 6b4e 52b1 1296  .....c....kNR...
-000008b0: 9568 0e37 70bd 6e2b 84c0 51d1 2c08 14e7  .h.7p.n+..Q.,...
-000008c0: f6a1 6252 2c21 2e0f 2b2e b966 56e9 7f9e  ..bR,!..+..fV...
-000008d0: 1b56 d525 37a4 e296 9157 ba67 c745 f61f  .V.%7....W.g.E..
-000008e0: ca67 990b 3c81 6077 01e9 d67f 071e e2a2  .g..<.`w........
-000008f0: e3bd bae7 5623 585f a43f 20c3 d76c 0df9  ....V#X_.? ..l..
-00000900: 0e06 18e5 bb7e 7001 19a5 f4e1 24f1 cfa7  .....~p.....$...
-00000910: d341 38a5 c328 0c68 18f9 d373 1a8d 4e46  .A8..(.h...s..NF
-00000920: a3c1 6418 4c92 611a 44c1 c877 7ad4 519c  ..d.L.a.D..wz.Q.
-00000930: 29d6 d862 a723 873b c621 88e6 c874 c9b6  )..b.#.;.!...t..
-00000940: 7b0b f5e3 46e4 2f1c 9e93 d92c 0cd2 61e8  {...F./....,..a.
-00000950: 8d82 64e0 85fd 847a 49da 1f7a e174 3019  ..d....zI..z.t0.
-00000960: d120 1acd d2f4 b7f3 d675 cc3b c137 e645  . .......u.;.7.E
-00000970: 716e 8bb6 f742 e66a 33c6 1ef5 a1e3 3ebd  qn...B.j3.....>.
-00000980: dd6e 5ae3 bdc8 6d01 0ef7 8301 5466 77f6  .nZ...m.....Tfw.
-00000990: 9d8b 5501 8c69 7f38 72e5 aa03 c76c 8c9f  ..U..i.8r....l..
-000009a0: fddd e3c1 9cba c1f7 66f0 b4c3 ded6 3222  ........f.....2"
-000009b0: af28 b5bd 19a8 b533 926d 3d5d bb7e 4de1  .(.....3.m=].~M.
-000009c0: 25e0 e636 c018 e9d8 dda1 2ff2 b674 c8fe  %..6....../..t..
-000009d0: 6f19 2bb3 b946 6e72 3ff4 dbf4 eedf 1367  o.+..Fnr?......g
-000009e0: 7f00 0000 ffff 0300 504b 0304 1400 0600  ........PK......
-000009f0: 0800 0000 2100 8582 6b55 2401 0000 f204  ....!...kU$.....
-00000a00: 0000 1a00 fe00 786c 2f5f 7265 6c73 2f77  ......xl/_rels/w
-00000a10: 6f72 6b62 6f6f 6b2e 786d 6c2e 7265 6c73  orkbook.xml.rels
-00000a20: 20a2 fa00 28a0 0001 0000 0000 0000 0000   ...(...........
-00000a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000005f0: 0000 0000 00ac 924d 4b03 3110 86ef 82ff  .......MK.1.....
+00000600: 21cc bd3b db2a 22d2 6c2f 45e8 4d64 fd01  !..;.*".l/E.Md..
+00000610: 3199 fd60 3799 90a4 bafd f746 4174 a1b6  1..`7......FAt..
+00000620: 1e7a 9caf 779e 7999 f566 b2a3 78a3 107b  .z..w.y..f..x..{
+00000630: 7612 9645 0982 9c66 d3bb 56c2 4bfd b8b8  v..E...f..V.K...
+00000640: 0711 9372 468d ec48 c281 226c aaeb abf5  ...rF..H.."l....
+00000650: 338d 2ae5 a1d8 f53e 8aac e2a2 842e 25ff  3.*....>......%.
+00000660: 8018 7547 56c5 823d b95c 6938 5895 7218  ..uGV..=.\i8X.r.
+00000670: 5af4 4a0f aa25 5c95 e51d 86df 1a50 cd34  Z.J..%\......P.4
+00000680: c5ce 4808 3b73 03a2 3ef8 bcf9 bc36 374d  ..H.;s..>....67M
+00000690: af69 cb7a 6fc9 a523 2b90 a644 ce90 59f8  .i.zo..#+..D..Y.
+000006a0: 90d9 42ea f335 a256 a1a5 24c1 b07e cae9  ..B..5.V..$..~..
+000006b0: 88ca fb22 6303 1e27 5afd 9fe8 ef6b d152  ..."c..'Z....k.R
+000006c0: 5246 2585 9a03 9de6 f9ec 3805 b4bc a445  RF%.......8....E
+000006d0: 7313 7fdc 9946 7ce7 30bc 320f a758 6e2f  s....F|.0.2..Xn/
+000006e0: c9a2 f731 b13d 63ce 57cf 3712 cede b2fa  ...1.=c.W.7.....
+000006f0: 0000 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
+00000700: 0000 0021 00fd 33d2 52e6 0200 0075 0600  ...!..3.R....u..
+00000710: 000f 0000 0078 6c2f 776f 726b 626f 6f6b  .....xl/workbook
+00000720: 2e78 6d6c a455 6d4f db30 10fe 3e69 ff21  .xml.UmO.0..>i.!
+00000730: f2f7 603b a449 1351 50a1 4543 1a53 c5eb  ..`;.I.QP.EC.S..
+00000740: 47e4 266e 6311 db99 edb4 6568 ff7d e784  G.&nc.....eh.}..
+00000750: f2b2 6a12 83a8 f5cb 5dfa f8b9 bbe7 dc83  ..j.....].......
+00000760: a38d ac83 1537 5668 3542 748f a080 ab42  .....7Vh5Bt....B
+00000770: 9742 2d47 e8fa ea34 1ca2 c03a a64a 566b  .B-G...4...:.JVk
+00000780: c547 e881 5b74 74f8 f5cb c15a 9bfb b9d6  .G..[tt....Z....
+00000790: f701 0028 3b42 9573 4d8e b12d 2a2e 99dd  ...(;B.sM..-*...
+000007a0: d30d 57e0 5968 2399 83ad 5962 db18 ce4a  ..W.Yh#...Yb...J
+000007b0: 5b71 ee64 8d23 4212 2c99 50a8 47c8 cd7b  [q.d.#B.,.P.G..{
+000007c0: 30f4 6221 0a3e d145 2bb9 723d 88e1 3573  0.b!.>.E+.r=..5s
+000007d0: 40df 56a2 b15b 3459 bc07 4e32 73df 3661  @.V..[4Y..N2s.6a
+000007e0: a165 0310 7351 0bf7 d081 a240 16f9 d952  .e..sQ.....@...R
+000007f0: 69c3 e635 84bd a183 6063 e093 c097 1218  i..5....`c......
+00000800: a2ed 49e0 da39 4a8a c268 ab17 6e0f a071  ..I..9J..h..n..q
+00000810: 4f7a 277e 4a30 a56f 52b0 d9cd c1fb 9062  Oz'~J0.oR......b
+00000820: 6cf8 4af8 1a3e b332 c907 5925 cf58 c90b  l.J..>.2..Y%.X..
+00000830: 1825 9f46 a320 ad4e 2b39 24ef 8368 8367  .%.F. .N+9$..h.g
+00000840: 6e11 3a3c 5888 9adf f4d2 0d58 d3fc 60d2  n.:<X......X..`.
+00000850: 57aa 4641 cdac 9b96 c2f1 7284 52d8 ea35  W.FA......r.R..5
+00000860: 7f63 306d 73dc 8a1a bc51 1aed 5384 0f9f  .c0ms....Q..S...
+00000870: e53c 33b0 81da 8f6b c78d 628e 9f68 e540  .<3....k..b..h.@
+00000880: 6a4f d43f 2bab 0efb a4d2 20e2 e082 ff6c  jO.?+..... ....l
+00000890: 85e1 d03b 2021 0807 4656 e46c 6e67 cc55  ...; !..FV.lng.U
+000008a0: 416b ea3e 4916 baaa 5510 2a74 e99e ad98  Ak.>I...U.*t....
+000008b0: e18d 16aa 5796 e34c 5a7c 3dbe 38bf f22b  ....W..LZ|=.8..+
+000008c0: 8818 8f4d 5189 15c7 13b1 148e d5c1 0c4e  ...MQ..........N
+000008d0: e066 d575 0806 53d5 ce31 34e7 e64e 3225  .f.u..S..14..N2%
+000008e0: 1690 97bb 2557 dc30 a7cd 3fed 96c9 a6e6  ....%W.0..?.....
+000008f0: 16bf 923c dbed afff 103d 2b7c ce31 e4b9  ...<.....=+|.1..
+00000900: cf45 bffe 3be7 9012 936f 853d 7326 80f5  .E..;....o.=s&..
+00000910: d9e4 3b14 f792 ada0 d411 d4b6 7cba 0ace  ..;.........|...
+00000920: a098 94de a563 723c 9d0e e229 1d26 7144  .....cr<...).&qD
+00000930: e384 4c8f 6992 a559 3638 1946 27e3 e124  ..L.i..Y68.F'..$
+00000940: 4aa2 8c78 299a 242f 346b 5df5 2421 8f3b  J..x).$/4k].$!.;
+00000950: 4231 60ee b8ce d966 eba1 246f 45f9 c2e1  B1`....f..$oE...
+00000960: 7118 c713 92ee 0fc2 38cb 2661 9c1e 0fc2  q.......8.&a....
+00000970: 8cd2 3404 d324 2329 21c3 41f2 db47 eb2f  ..4..$#)!.A..G./
+00000980: cb1b c1d7 f645 6c7e 1b48 a184 14bf bc56  .....El~.H.....V
+00000990: 299c 7d2b 54a9 d723 1446 d17e 043c 1fb6  ).}+T..#.F.~.<..
+000009a0: 8694 c055 bcee bcb7 a274 15bc 9ed1 015c  ...U.....t.....\
+000009b0: 43bd ed1b 17cb 0a02 a034 8a63 1f43 e489  C........4.c.C..
+000009c0: 8ed0 2379 7a42 9827 7e20 e129 3cdd b0f5  ..#yzB.'~ .)<...
+000009d0: 7504 f12b 86dd 2d0d 4cbb 3950 5d67 5dfa  u..+..-.L.9P]g].
+000009e0: 9b1b 2876 b62e df28 30b9 3fc3 9c95 5d13  ..(v...(0.?...].
+000009f0: e1ed cf0a 5617 3313 f8c9 bf48 ba6a 6fff  ....V.3....H.jo.
+00000a00: 310e ff00 0000 ffff 0300 504b 0304 1400  1.........PK....
+00000a10: 0600 0800 0000 2100 8582 6b55 1f01 0000  ......!...kU....
+00000a20: f204 0000 1a00 0801 786c 2f5f 7265 6c73  ........xl/_rels
+00000a30: 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e 7265  /workbook.xml.re
+00000a40: 6c73 20a2 0401 28a0 0001 0000 0000 0000  ls ...(.........
 00000a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b10: 0000 0000 0000 0000 0000 0000 0000 bc94  ................
-00000b20: cb6a c330 1045 f785 fe83 d1be 96ed a469  .j.0.E.........i
-00000b30: 2991 b329 856c db14 ba15 f6f8 412c c968  )..).l......A,.h
-00000b40: 266d fdf7 152e 8d1d 086a 1622 1bc1 cca0  &m.......j."....
-00000b50: 7b0f 578f f5e6 5b75 d127 586c 8d16 2c8d  {.W...[u.'Xl..,.
-00000b60: 1316 812e 4cd9 ea5a b0f7 ddcb dd23 8b90  ....L..Z.....#..
-00000b70: a42e 6567 3408 3600 b24d 7e7b b37e 854e  ..eg4.6..M~{.~.N
-00000b80: 92db 844d db63 e454 340a d610 f54f 9c63  ...M.c.T4....O.c
-00000b90: d180 9218 9b1e b49b 54c6 2a49 aeb4 35ef  ........T.*I..5.
-00000ba0: 65b1 9735 f02c 4956 dcce 3558 7ea2 196d  e..5.,IV..5X~..m
-00000bb0: 4bc1 ecb6 74fe bba1 77ce ff6b 9baa 6a0b  K...t...w..k..j.
-00000bc0: 7836 c541 81a6 3316 bc38 2019 f5a1 3a27  x6.A..3..8 ...:'
-00000bd0: 2a6d 0d24 581c 4f5d de12 a865 ec90 193f  *m.$X.O]...e...?
-00000be0: 4fb3 0849 8334 742e ce23 ca6f edb3 7f08  O..I.4t..#.o....
-00000bf0: 697f 4918 0b1f 4d16 9286 dc95 8129 8bb1  i.I...M......)..
-00000c00: e4e3 9afa 18d2 900c 5fc6 eeb1 01a0 89e3  ........_.......
-00000c10: d842 3e4e bc30 ab90 3097 1c4f e68b e6fe  .B>N.0..0..O....
-00000c20: da34 de6c 9621 69b0 9116 ca37 b2ee 9b9a  .4.l.!i....7....
-00000c30: 3fa0 79fb 2f1a 7ef2 53e5 3f00 0000 ffff  ?.y./.~.S.?.....
-00000c40: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-00000c50: 7d6f bac0 4315 0000 b06e 0000 1800 0000  }o..C....n......
-00000c60: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
-00000c70: 6565 7431 2e78 6d6c 9c94 db8e 9b30 1086  eet1.xml.....0..
-00000c80: ef2b f51d 2cdf 0730 21e4 a090 55d5 d56a  .+..,..0!...U..j
-00000c90: 57ea 45d5 4ddb 6bc7 0cc1 0ac6 d476 4eaa  W.E.M.k......vN.
-00000ca0: faee 1d4c 4856 8ad4 a41b 1133 60fe ef9f  ...LHV.....3`...
-00000cb0: b107 e60f 0755 911d 182b 759d 5116 4494  .....U...+u.Q.D.
-00000cc0: 402d 742e eb75 46bf 2f9f 0613 4aac e375  @-t..uF./...J..u
-00000cd0: ce2b 5d43 468f 60e9 c3e2 e387 f95e 9b8d  .+]CF.`......^..
-00000ce0: 2d01 1c41 426d 335a 3ad7 ccc2 d08a 1214  -..ABm3Z:.......
-00000cf0: b781 6ea0 c699 421b c51d 5e9a 7568 1b03  ..n...B...^.uh..
-00000d00: 3cf7 2255 8571 14a5 a1e2 b2a6 1d61 66ee  <."U.q.......af.
-00000d10: 61e8 a290 021e b5d8 2aa8 5d07 3150 7187  a.......*.].1Pq.
-00000d20: f9db 5236 b6a7 2971 0f4e 71b3 d936 03a1  ..R6..)q.Nq..6..
-00000d30: 5583 8895 aca4 3b7a 2825 4acc 5ed6 b536  U.....;z(%J.^..6
-00000d40: 7c55 61dd 0796 7041 0e06 8f18 ffc3 dec6  |Ua...pA........
-00000d50: dfbf 7252 5218 6d75 e102 2487 5dce d7e5  ..rRR.mu..$.]...
-00000d60: 4fc3 69c8 c599 745d ff5d 1896 8406 76b2  O.i...t].]....v.
-00000d70: ddc0 0b2a 7e5f 4a6c 7466 c517 d8f0 9db0  ...*~_Jltf......
-00000d80: f40c 6b97 cbcc b632 cfe8 efe8 f41b e099  ..k....2........
-00000d90: b543 7419 fab9 3f74 31cf 25ee 705b 1531  .Ct...?t1.%.p[.1
-00000da0: 5064 f413 9b2d 478c 868b b96f a01f 12f6  Pd...-G....o....
-00000db0: f64d 4c1c 5fbd 4205 c201 9a30 4a9c 6ebe  .ML._.B....0J.n.
-00000dc0: 40e1 3e43 5565 f419 6fb4 0dbb d27a d32a  @.>CUe..o....z.*
-00000dd0: 5ff0 9908 3dac 57b4 1e5c 38b9 83ee e925  _...=.W..\8....%
-00000de0: d66e 7f79 570c d131 3c5b be8d 7bfb 27df  .n.yW..1<[..{.'.
-00000df0: e25f 0dc9 a1e0 dbca 7dd3 fb67 90eb d261  ._......}..g...a
-00000e00: 1e49 9060 e96d efcc f2e3 2358 814d 8bd6  .I.`.m....#X.M..
-00000e10: c1b0 c50a 5d21 0347 a224 be7c b848 8a1f  ....]!.G.$.|.H..
-00000e20: fc79 2f73 5766 3449 82d1 2849 27e3 1125  .y/sWf4I..(I'..%
-00000e30: 626b 9d56 3fbb 09bf 0e67 21c3 69af 6c83  bk.V?....g!.i.l.
-00000e40: 9334 8e02 164d 87b7 9469 afc4 e0a2 4cd3  .4...M...i....L.
-00000e50: 244a e31b a6e3 5e8a 412f 4dee 32c5 4f4a  $J....^.A/M.2.OJ
-00000e60: 972e 0627 2563 c164 928e d9cd 52a7 bd16  ...'%c.d....R...
-00000e70: 83ff 2a35 c62f 9b77 6d83 de35 fed7 fa86  ..*5./.wm..5....
-00000e80: 7e7f fe02 0000 ffff 0000 00ff ff94 9deb  ~...............
-00000e90: 8ee3 3612 855f 2598 07e8 48d4 3d98 0cb0  ..6.._%...H.=...
-00000ea0: b2db 1ddb dd76 2efb 02c1 ec00 fb2b bbc8  .....v.......+..
-00000eb0: 04d9 ddb7 df22 454b acaf 2875 140c 3201  ....."EK..(u..2.
-00000ec0: 4f49 2659 8764 d521 a97c fcfa cf2f 5ffe  OI&Y.d.!.|.../_.
-00000ed0: 38fe fac7 af9f 3efe feaf ff7c f3fb f71f  8.....>....|....
-00000ee0: ca0f df7c fdf7 afbf 7d95 fffa ce15 1fbe  ...|....}.......
-00000ef0: f96f 59ff faf9 bb7f fcef f8e5 ebe7 2fbf  .oY.........../.
-00000f00: fdf1 fd87 e2a9 faf0 e9e3 676f fb37 6f1c  ..........go.7o.
-00000f10: 1e91 f2af 52fa e7a7 e2e3 b77f 7efa f8ed  ....R.......~...
-00000f20: e768 315a 8b52 5b1c ac85 d316 476b 5169  .h1Z.R[.....GkQi
-00000f30: 8b67 6b51 6b8b 93b5 68b4 c58b b568 b5c5  .gkQk...h....h..
-00000f40: 0fd6 a2d3 1667 6bd1 6b8b 8bb5 18b4 c535  .....gk.k......5
-00000f50: d363 e8d4 d78c 097a f52d 6382 6ebd 654c  .c.....z.-c.n.eL
-00000f60: d0af f78c 093a f6c7 c9a4 faf0 cd4c 01e7  .....:.......L..
-00000f70: d071 3fe5 6cd0 753f e76c d079 bfe4 6cd0  .q?.l.u?.l.y..l.
-00000f80: 7d7f cfd8 544b b3be 1596 cf54 777b a8ee  }...TK.....Tw{..
-00000f90: 8d3d d573 2417 6c6e 7d09 5e1d 1488 9e39  .=.s$.ln}.^....9
-00000fa0: 2a10 5d72 5220 fae2 4581 e884 1f5c a866  *.]rR ..E....\.f
-00000fb0: 5d0c f8bd f3d4 8a08 3755 5d3e 556d d176  ].......7U]>Um.v
-00000fc0: 85fc bbab f0fb 1718 f7ed 53dd 0e65 5dbb  ..........S..e].
-00000fd0: b6eb 1da8 72cd 18f7 c5d0 9485 7365 0576  ....r.......se.v
-00000fe0: be4e 1500 addf b2a5 b76c e93d 6dbe c38b  .N.......l.=m...
-00000ff0: 7e54 6005 deff a451 3cfb b346 51f1 5fa6  ~T`....Q<..FQ._.
-00001000: ca2c a58a 4f32 08fe fad4 e98d 1f7c c2af  .,..O2.......|..
-00001010: 8c6a 3471 bed4 430d 53a5 02e1 a253 0a96  .j4q..C.S....S..
-00001020: 60c6 8b02 c927 3fe3 fff9 29c3 a7a9 15e0  `....'?...).....
-00001030: 5337 f4ae 746e 40c7 5f60 1cf8 e49c 139a  S7..tn@._`......
-00001040: 542d 2972 cd18 7745 d937 45d5 b902 83e1  T-)r..wE.7E.....
-00001050: 75aa 1fe7 c06c e96d 2a85 dbef aae3 9639  u....l.m*......9
-00001060: 4ef9 b7de e35f 6ffc f02f 3a62 146c 992d  N...._o../:b.l.-
-00001070: 395f 2890 f385 0231 5e9f 1588 2e3a 2910  9_(....1^....:).
-00001080: 157a 5120 9d5f 07e7 9775 6966 93a9 8da9  .zQ ._...uif....
-00001090: f76b 57b7 c550 9745 5b82 7d17 1abb a7b6  .kW..P.E[.}.....
-000010a0: 765d 3f54 4dd9 d7a8 ed15 c69e 2aeb de9f  v]?TM.......*...
-000010b0: 2a88 36bd c56a eb01 72cb 96de d3f6 570b  *.6..j..r.....W.
-000010c0: 3594 f79b 3dde f7c6 0fef a323 46c1 66ef  5...=......#F.f.
-000010d0: 93f6 0705 3210 5220 6320 0532 fc49 4147  ....2.R c .2.IAG
-000010e0: ef2b 90de 6f26 ef77 1567 d9f3 d446 78bf  .+..o&.w.g...Fx.
-000010f0: 7643 3114 b2b2 20ee a171 f07e d374 bdac  vC1... ..q.~.t..
-00001100: 3d1d 06ee 15c6 dbde 9f2a 48ef 674b 6fb1  =........*H.gKo.
-00001110: 31ba 6e77 d573 cb70 54de 6ff7 78df 1b3f  1.nw.s.pT.o.x..?
-00001120: bc8f 8e18 055b bc8f e17d 5020 86f7 5181  .....[...}P ..Q.
-00001130: 1830 cf29 e838 f615 48ef 2b90 de6f e7b1  .0.).8..H.+..o..
-00001140: 0fe4 3cb5 71f1 be38 b491 81df 7765 cf91  ..<.q..8....we..
-00001150: 9f37 2d86 4e26 ff92 e12f 8cb7 7d3f 558f  .7-.N&.../..}?U.
-00001160: be9f 4a51 8b5b 6c0a 7caf 3a75 a98b f27d  ..JQ.[l.|.:u...}
-00001170: b7c7 f7de f8e1 7b4c eda3 60b3 ef6b ac40  ......{L..`..k.@
-00001180: 0705 6244 1c15 88f6 3ea7 2007 de29 05cd  ..bD....>. ..)..
-00001190: c857 207d dfc5 91ef 7aa6 3953 1be1 fb52  .W }....z.9S...R
-000011a0: d6fc 4622 4346 912b c632 ecfd 528e e407  ..F"CF.+.2..R...
-000011b0: c6db de9f 2a48 ef4f a518 76b7 d818 785f  ....*H.O..v...x_
-000011c0: 75eb 4a96 d0ef f1be 377e 781f 837b 146c  u.J.....7~x..{.l
-000011d0: f13e ea77 5020 7873 5420 5efb 9c82 66e4  .>.wP xsT ^...f.
-000011e0: 2b90 235f 81f4 7e3f 797f 18f8 cef3 d4c6  +.#_..~?y.......
-000011f0: d9fb 8f30 ae2b 9d2c e51c fb2b c67d 21c1  ...0.+.,...+.}!.
-00001200: e400 aa5c 33c6 ebab fe54 417a 7f2a 4507  ...\3....TAz.*E.
-00001210: de62 63e0 7dd5 ad4b 5dd4 d81f f678 df1b  .bc.}..K]....x..
-00001220: 3fbc 8fb6 8d82 2dde c704 7d50 203c 714c  ?.....-...}P <qL
-00001230: c106 b3c6 730a 9ab1 9f82 66ec 2b90 de1f  ....s.....f.+...
-00001240: 82f7 5d51 0fa8 ea79 6aa3 f67e 390c 455b  ..]Q...yj..~9.E[
-00001250: c9aa 8f69 ebb2 622c 9124 5d9f b10c ae97  ...i..b,.$].....
-00001260: dcb1 33e1 7eac 9d76 e7db 548a e171 9b4a  ..3.~..v..T..q.J
-00001270: 51b1 bbea d395 74ae 14f5 6b87 14e6 ad1f  Q.....t...k.....
-00001280: ce47 a78d fe55 b3f7 1b70 f6a0 518c a0a3  .G...U...p..Q...
-00001290: 4631 6f3c 6b14 bc3f 29d4 a47c 0a75 a480  F1o<k..?)..|.u..
-000012a0: a03e e92b cba6 2107 42cf 7cff c1a4 7d32  .>.+..!.B.|...}2
-000012b0: a5db e4ec 62ac 8ba7 c675 9225 0ca2 3998  ....b....u.%..9.
-000012c0: 3980 d6f3 1250 d695 8914 5f1f 9504 1562  9....P...._....b
-000012d0: 313a fa16 8b99 fbe9 3e5c 08a4 2682 d20b  1:......>\..&...
-000012e0: 4b7f 5d18 7d28 67be 0bd1 b3a3 7fd5 c206  K.].}(g.........
-000012f0: 8c84 8346 d1f5 4785 9654 8c34 ca14 5fa3  ...F..G..T.4.._.
-00001300: c6df 93b6 9549 f243 d38d bbdb def5 92e3  .....I.C........
-00001310: b778 cf85 d6de 814d e124 23ac 8bae e582  .x.....M.$#.....
-00001320: 9fb3 0eba 5159 4928 81f6 bd8a 75e0 24dd  ....QYI(....u.$.
-00001330: 3d15 33e2 8bd6 c6dd aafb 5762 be72 9738  =.3.......Wb.r.8
-00001340: 18ac 6735 c768 e0a9 a6d4 32ee f3cf ce6c  ..g5.h....2....l
-00001350: 6819 f869 9491 9f46 a9f7 2894 83f8 45a1  h..i...F..(...E.
-00001360: 76f4 c7c1 5d31 ee8f 4d35 63df 35fd d0b4  v...]1..M5c.5...
-00001370: 5cfe 8db5 93b1 dfca f4df 0873 0a6a 88b4  \..........s.j..
-00001380: 5ec6 7ed3 b78e 22a2 587b 3230 0288 c5b0  ^.~...".X{20....
-00001390: bec5 62a3 70ab de5f 117e ca5d ca5e b09e  ..b.p.._.~.].^..
-000013a0: c940 6dcf a38b bb29 fe68 94ea 8f46 cde0  .@m....).h...F..
-000013b0: 4fdf 6cdd bd29 f0c9 9b57 14be d89a 34d8  O.l..)...W....4.
-000013c0: 6fca a6e8 eac6 c982 8fce bfd0 3a0c 7e89  o...........:.~.
-000013d0: 21ab ae15 91cf 0cfe 3591 afcc fa7b aaa3  !.......5....{..
-000013e0: f177 b6f8 165b 64fc adba 7f99 5df5 5cbf  .w...[d.....].\.
-000013f0: 4be9 2b53 a9af 44f5 468f 2efe c668 3a28  K.+S..D.F....h:(
-00001400: b4c3 d470 d428 98f4 ac51 fcee 49ff ae59  ...p.(...Q..I..Y
-00001410: 0a36 153f 79d6 b3a1 e3ac 708e 4d55 6470  .6.?y.....p.MUdp
-00001420: 9d08 fc4d 5716 03a3 bf35 eba2 ad7b 6e93  ...MW....5...{n.
-00001430: 5c69 bc8c 7d51 149c 5908 a61a c2bb 6fb1  \i..}Q..Y.....o.
-00001440: e266 ec67 15c2 bbee c095 f4af dca5 fb05  .f.g............
-00001450: eb79 ec53 f9f3 e8cc 858e 29a0 4699 036a  .y.S......).F..j
-00001460: 9449 a046 0d17 d2df 6d0d 1736 f53f 79b3  .I.F....m..6.?y.
-00001470: e782 0c5f ee75 42a5 eb9a a761 68fa ba15  ..._.uB....ah...
-00001480: 09c8 1554 0162 c7cc cce9 daa7 a26c 3ae1  ...T.b.......l:.
-00001490: 8d1b 5af2 ec4a eb85 0c43 2151 a0ae c96b  ..Z..J...C!Q...k
-000014a0: aca2 2143 5e03 8cd6 e8a3 bbee c195 6cb0  ..!C^.........l.
-000014b0: dc25 0306 eb99 0c14 023d ba90 8119 a146  .%.......=.....F
-000014c0: 9912 2ab4 674e a89f 3564 487f d792 6153  ..*.gN..5dH...aS
-000014d0: 0e94 3787 65a2 e2f6 df39 b655 e585 4d98  ..7.e....9.U..M.
-000014e0: f85d c5fc edb2 c7f8 9a33 9e52 c32c 17b2  .].......3.R.,..
-000014f0: e2df 5bac b889 10b3 02e2 5d77 ef5a 7a98  ..[.......]w.Zz.
-00001500: ca82 9e3d db27 2552 5d90 93df 58a6 4254  ...=.'%R]...X.BT
-00001510: 6ff2 4385 9afc 50a1 263f 4c51 ca6d 27f5  o.C...P.&?LQ.m'.
-00001520: bb96 0b9b f2a0 3c1b 1609 b36f 7cf6 6f95  ......<....o|.o.
-00001530: 5478 19eb 7166 e8aa 82bc b9d0 b677 4f43  Tx..qf.......wOC
-00001540: 55c9 f2d0 35ce b0ec 6aac 1ffb 4265 960b  U...5...j...Be..
-00001550: 530d cdbc 9057 0863 7bcc bca0 ba77 6577  S....W.c{....wew
-00001560: a04c 45c2 f7b9 90aa 84cc ca47 ffae 795e  .LE........G..y^
-00001570: e8b9 43a0 516e 1168 947b 040a b55c 487f  ..C.Qn.h.{...\H.
-00001580: d772 6153 2c94 3787 4477 c054 740e 1d93  .raS,.7.Dw.Tt...
-00001590: 5061 8e07 db46 7689 4dea 9811 00c3 24d2  Pa...Fv.M.....$.
-000015a0: b643 8305 f19a 7bf5 c6bc 30d5 d070 21af  .C....{...0..p!.
-000015b0: 17c6 f618 2e28 d7ac 658e a964 f83e 1752  .....(..e..d.>.R
-000015c0: cd90 f9fc 58a6 3a15 3bf7 a051 9339 aa67  ....X.:.;..Q.9.g
-000015d0: 4de6 98a2 960b 296a b9b0 291d 4aad 428e  M.....)j..).J.B.
-000015e0: 5eb7 988b cebe bed9 7941 9688 8eb9 fec5  ^.......yA......
-000015f0: 58fb 88a1 6bea baef 6bd9 68e0 a9a9 5501  X...k...k.h...U.
-00001600: 313b 334c 7534 6cc8 4b88 b145 860d aa83  1;3Lu4l.K..E....
-00001610: 57c2 477f 846e 968d de65 43b0 9e23 06aa  W.G..n...eC..#..
-00001620: 881e 9d67 8681 e1a3 4619 3e6a 94e1 a342  ...g....F.>j...B
-00001630: 0d1b 146a d8a0 50a3 2308 1ad8 e0b8 c97b  ...j..P.#......{
-00001640: 8e6d 4562 5916 a5e4 892d f5e1 4bde ba18  .mEbY....-..K...
-00001650: 9c08 09f2 076c a0f5 76fc 18eb 4836 c462  .....l..v...H6.b
-00001660: ccb1 b758 4c36 e80e 5e89 1f5d 2a22 becf  ...XL6..^..]*"..
-00001670: 8654 44e4 46e9 e8df b5b0 81f1 a346 193f  .TD.F........F.?
-00001680: 2ab4 2c18 402a d8d2 21fd 614b 8714 b574  *.,.@*..!.aK...t
-00001690: 8802 9e1c 2343 3a11 ba26 1734 945d 3d30  ....#C:..&.4.]=0
-000016a0: abbe 18eb 904e f465 d7d7 928e a2b9 575a  .....N.e......WZ
-000016b0: bf43 87ac 9af8 262f f14c 4647 df62 b1a1  .C....&/.LFG.b..
-000016c0: 43da 0d42 eab9 b5fa 0462 aa32 becf 87e9  C..B.....b.2....
-000016d0: 8cdd 540f 1ec7 189d 3a11 5830 8804 cc28  ..T.....:.X0...(
-000016e0: 1230 c348 055b 4628 118d f9a5 7ad6 3262  .0.H.[F(....z.2b
-000016f0: 9a00 ca66 60ac 73f6 0fa6 ebc5 123c 1445  ...f`.s......<.E
-00001700: daa5 e12c f265 97f5 3567 1da2 0799 a88c  ...,.e..5g......
-00001710: ec2c c6de f566 8298 8ac1 b65b b436 8cd0  .,...f.....[.6..
-00001720: fe59 8924 5d2a 35be cf88 4940 8b8c a0d4  .Y.$]*5...I@....
-00001730: e8df 35cf 1072 244b 8fb8 0360 c692 8019  ..5..r$K...`....
-00001740: 4c2a d832 42c9 6c86 11ea b41d 3722 e4cd  L*.2B.l.....7"..
-00001750: a1b7 ebae e7c6 53e8 9dcc 2421 2b46 5f32  ......S...$!+F_2
-00001760: 7aba d0da e716 5ddf b8b2 6de4 5c2a bc79  z.....]...m.\*.y
-00001770: 35d6 8fdc c2f5 8d9c 7e82 e6f0 a824 7622  5.......~....$v"
-00001780: 6271 8919 f516 cb0d 27b4 8756 224a 97ca  bq......'..V"J..
-00001790: 91ef 7342 9d3c c42f 8efe 5d0b 2758 cf03  ..sB.<./..].'X..
-000017a0: 60c6 9480 1954 2ad8 7242 29a1 8613 9b8a  `....T*.rB).....
-000017b0: a4bc 3968 fde2 0ad4 e91c 7a47 a718 5537  ..9h......zG..U7
-000017c0: c871 35d9 c92a 6aea 50b4 eeba a7a1 280a  .q5..*j.P.....(.
-000017d0: 11b3 fd79 14b3 70ac 9d43 cc73 222f 4ac6  ...y..p..C.s"/J.
-000017e0: ba97 5425 1f6d c2a9 04f4 f15a 5c99 ca92  ..T%.m.....Z\...
-000017f0: ef73 62d2 eae2 3c41 59d2 a502 60c9 95f9  .sb...<AY...`...
-00001800: 00d8 4496 fa69 135a 2acd 9362 947a b78d  ..D..i.Z*..b.z..
-00001810: 2536 9549 7936 7082 99e1 d9bf 34bb 6ee4  %6.Iy6p.....4.n.
-00001820: 3621 2ebb acaf 39eb b06e 5445 6db7 a862  6!....9..nTEm..b
-00001830: 15cd c211 cf21 a237 6e8f 1691 11ba 87d7  .....!.7n.......
-00001840: 62cb 549b 7c9f 11e9 1945 476d d2a5 2a60  b.T.|....EGm..*`
-00001850: 599a e052 c326 ba54 3003 9567 f572 3b4b  Y..R.&.T0..g.r;K
-00001860: 6cca 93ea 591b 4bc4 337e 3c54 70f6 8fe5  l...Y.K.3~<Tp...
-00001870: 32cf b697 4882 079c 2ec6 3a06 977d 27cb  2...H.....:..}'.
-00001880: 4c63 d68d b513 8b55 29cb 9259 37f2 faa4  Lc.....U)..Y7...
-00001890: fc64 4893 2850 c672 b36e e81e 5e8b 2e77  .dH.(P.r.n..^..w
-000018a0: 2994 2e55 281d 8f2e 7a74 5937 7898 e800  )..U(...ztY7x...
-000018b0: d844 97fa 6913 5da6 30f7 904f eadd 665f  .D..i.].0..O..f_
-000018c0: 53a1 9611 93d6 d78a 3ec8 7c03 22e5 7415  S.......>.|.".t.
-000018d0: 4616 0ee1 83a3 932f b173 b4bc bd7a a821  F....../.s...z.!
-000018e0: 67dd c99e 6951 b9b2 e192 f42a d6b9 7dec  g...iQ.....*..}.
-000018f0: 586c 1891 1535 ef70 c05a 74b9 4ba7 74a9  Xl...5.p.Zt.K.t.
-00001900: 4ec9 4b5d a347 1346 98e8 52c3 26ba d4b0  N.K].G.F..R.&...
-00001910: 892e 9518 893e 38a9 9fb6 8cd8 942a e5d9  .....>8......*..
-00001920: b09f d5a1 c2e7 d85a 7ba8 a9a8 1a39 daac  .......Z{....9..
-00001930: e973 a1f5 f629 979c f506 21f2 471b 63cd  .s...)....!.G.c.
-00001940: 79b2 3516 a38f ee70 cf5a 68b9 4bac 74a9  y.5....p.Zh.K.t.
-00001950: 58c9 3dd9 d1a3 0b21 926b 1421 3f3b 0036  X.=....!.k.!?;.6
-00001960: a1a5 7eda 8496 4a91 3484 50e7 f940 a617  ..~...J.4.P..@..
-00001970: f5cb 768a 9844 bf81 d1c7 39b6 d69e 7419  ..v..D....9...t.
-00001980: 1a39 ba86 2a5c 8c75 f134 4c72 44ee 943b  .9..*\.u.4LrD..;
-00001990: ad67 45a2 922b 3115 1af0 2ad6 d919 622a  .gE..+1...*...b*
-000019a0: e661 d768 6d08 a13b 7825 aeac 76e9 95c1  .a.hm..;x%..v...
-000019b0: 7abe e544 bdd2 a309 2128 5802 665c 0918  z..D....!(X.f\..
-000019c0: c3f5 a460 3307 e887 9961 0a1a b631 edfd  ...`3....a...1..
-000019d0: c8d8 20f8 dc1f 75eb 5b91 2830 09d0 5abc  .. ...u.[.(0..Z.
-000019e0: 38a5 1ead 5873 d7f3 9ab1 ae65 974b 24ed  8...Xs.....e.K$.
-000019f0: 7e68 0bf4 ce6b ac23 c6c1 5b2c 466f dc62  ~h...k.#..[,Fo.b
-00001a00: 317d 8e3e 5c89 1cab 5daa 64b0 9e7d 8e2e  1}.>\...].d..}..
-00001a10: 193d 9af8 9c91 2360 468e 1ae6 1589 67c0  .=....#`F.....g.
-00001a20: 9842 4e78 3908 f5a2 6033 0d08 3a6d 67e2  .BNx9...`3..:mg.
-00001a30: b173 6c2f a701 39ba e0e4 2014 fc73 81b5  .sl/..9... ..s..
-00001a40: ebaa a72a 5c71 935b 6ef2 073a 35df bd3d  ...*\q.[n..:5..=
-00001a50: 0dc4 2a32 9b88 c54c 2f63 3198 7247 1f2e  ..*2...L/c1.rG..
-00001a60: f5d7 5759 7709 9355 2a4c 72e2 1f3d ba50  ..WYw..U*Lr..=.P
-00001a70: a246 f50f 8031 0e8e 80e1 9d67 c086 12ea  .F...1.....g....
-00001a80: b72b 4309 75db d74c 13f1 80a1 44fd 081e  .+C.u..L....D...
-00001a90: 6383 2d27 64e3 a265 4a73 81f5 7b9c c8a8  c.-'d..eJs..{...
-00001aa0: 9e53 8699 5b1a e4dd 3969 3216 33c1 8cc5  .S..[...9i2.3...
-00001ab0: 8613 da43 0bac 39b1 4b9a ac52 6992 1703  ...C..9.K..Ri...
-00001ac0: 468f 269c e019 68c0 e8fe 2360 f8ed 19b0  F.&...h...#`....
-00001ad0: e184 fa6d cb89 4d71 52de 1d96 0e5e 723b  ...m..MqR....^r;
-00001ae0: c7f6 6628 2127 dd6b 334d e893 8fef 5162  ..f(!'.k3M....Qb
-00001af0: ed9c 6436 5a88 5534 d344 9455 3595 6fd1  ..d6Z.U4.D.U5.o.
-00001b00: da50 4275 5272 ed44 5362 9732 59a5 ca24  .PBuRr.DSb.2Y..$
-00001b10: 15d5 d1a3 0b25 1a78 ed00 181d 7a04 8cc6  .....%.x....z...
-00001b20: 3f6b b836 9450 bf6d 29b1 a94d cabb 4374  ?k.6.P.m)..M..Ct
-00001b30: 2683 94d3 04e4 c398 6376 8de8 cf4d f255  &.......cv...M.U
-00001b40: 8a69 0323 76cf 8341 ef71 624d 9a94 bbf4  .i.#v..A.qbM....
-00001b50: ccde 5f63 150d 25a6 9a33 a388 d686 12da  .._c..%..3......
-00001b60: 412b 67a5 ab5d c264 b09e 2f4a a37e a347  A+g..].d../J.~.G
-00001b70: 134a f0b0 3460 d4f7 0818 73cc b382 8de8  .J..4`....s.....
-00001b80: a050 1b5e 6e0a 93f2 6c20 44d5 f238 ff39  .P.^n...l D..8.9
-00001b90: b6d7 ce12 b55c 7630 87a3 68bd 9d64 e6ac  .....\v0..h..d..
-00001ba0: 3ba1 595b cb07 3e40 cdd7 471d b17f 118b  ;.Y[..>@..G.....
-00001bb0: b9e7 1d8b 4d78 a9fd b34c d37a 92d8 254c  ....Mx...L.z..%L
-00001bc0: 56a9 30c9 1b6d a347 1346 60e6 3f68 9857  V.0..m.G.F`.?h.W
-00001bd0: 2d8e 80d1 27cf 0ab6 8c48 7fda 3262 f3dc  -...'....H..2b..
-00001be0: a4bc 3930 4276 1a4c 2861 e543 9f43 9443  ..90Bv.L(a.C.C.C
-00001bf0: 2747 ecb9 6770 89bd b31c adeb 9efa 6190  'G..gp........a.
-00001c00: add3 bead e46b 0a0c 2f57 a5c9 cef3 0d5b  .....k../W.....[
-00001c10: 5a8f 4a92 1253 ddb9 ef1d ad0d 2594 8312  Z.J..S......%...
-00001c20: f953 5362 9732 59a5 ca24 27e7 d1a3 0b25  .SSb.2Y..$'....%
-00001c30: e8b6 0360 135e eaa7 31c5 9cd4 d3d6 e9ea  ...`.^..1.......
-00001c40: 6113 3ec6 7386 992c 33ab 3d4a 9629 9182  a.>.s..,3.=J.)..
-00001c50: fd6a 0a8c c37d db5e 2ec3 c919 0afb e984  .j...}.^........
-00001c60: d857 4aa8 f4f7 a9e4 b67d 638f d18b 754e  .WJ......}c...uN
-00001c70: 5888 c5dc d88e c5c6 e5ba 0bd7 a2c7 5dd2  X.............].
-00001c80: 6395 4a8f 1566 f6d1 a389 cb4d f4a8 6113  c.J..f.....M..a.
-00001c90: 3d6a d844 8f0a b6a1 827e 1a7c 7a51 55b3  =j.D.....~.|zQU.
-00001ca0: 4966 3c85 c893 8fe7 d8de 4c92 d957 f2d5  If<.......L..W..
-00001cb0: 1bea 0eea 9ca4 dcd1 f537 2ac5 bd72 3c4e  .........7*..r<N
-00001cc0: ae55 a14a 57be 7b49 32fb 86a2 d7ab 1867  .U.JW.{I2......g
-00001cd0: f389 ec0d ea5b b446 17de b57f 926b 2d7a  .....[.F.....k-z
-00001ce0: 12d8 a53d 56a9 f6c8 2b00 a347 1746 708f  ...=V...+..G.Fp.
-00001cf0: f800 d804 8ffa 69aa 8bfa 69f6 ef8b 86cd  ......i...i.....
-00001d00: 2c30 8974 b96f 2765 8e2c b6bd dc88 7575  ,0.t.o'e.,....uu
-00001d10: d99a c30c b1fd 6a60 cba5 9b5a 6e61 c959  ......j`...Zna.Y
-00001d20: 6954 f99a b39e a601 3975 cb83 36af 629d  iT......9u..6.b.
-00001d30: 757a 5676 bc45 6be3 74dd 892b e161 bd4b  uzVv.Ek.t..+.a.K
-00001d40: 5f0c d673 7848 7dd1 a389 d319 1e02 6678  _..sxH}.......fx
-00001d50: 0898 e121 60fc f609 3018 f5a2 6033 0d08  ...!`...0...`3..
-00001d60: 1a76 fb7a 3911 8f94 21b6 58b9 5936 1dfd  .v.z9...!.X.Y6..
-00001d70: d1f9 a137 0264 deba 6f84 40f2 0f3c 74cd  ...7.d..o.@..<t.
-00001d80: 5a0f 72c3 5e96 9dba 46ff bcc6 4a62 3679  Z.r.^...F...Jb6y
-00001d90: 7bd4 1d69 642c e646 25ba 6965 17a2 de25  {..id,.F%.ie...%
-00001da0: 4006 eb99 1414 203d ba90 8277 630e 80b9  @..... =...wc...
-00001db0: 0b01 98bb 100a 3611 a242 4db0 a050 4b89  ......6..BM..PK.
-00001dc0: 497e 3457 ed63 6397 8541 2ed0 8abf e4e2  I~4W.cc..A......
-00001dd0: 7c29 7f53 90ce 58b7 ae6f eba6 af2a d10a  |).S..X..o...*..
-00001de0: 101e d27a 5e18 1a79 3b17 9d57 b1ce c50a  ...z^..y;..W....
-00001df0: b1d8 9c78 8ae5 0c16 d0c1 2bbb 10f5 2ef9  ...x......+.....
-00001e00: 3158 cfdf 5be2 ed6b 8f26 84e0 2e04 60ee  1X..[..k.&....`.
-00001e10: 4200 e6e9 1605 5b42 a43f 6d09 b129 3eca  B.....[B.?m..)>.
-00001e20: 9b43 7753 5388 8d55 8470 722a aa94 4bb6  .CwSS..U.pr*..K.
-00001e30: 7227 1791 02ad b733 c89c f5fa 36e5 a386  r'.....3....6...
-00001e40: c817 62b1 39ee 14cb 0d21 b47b 56b6 28ea  ..b.9....!.{V.(.
-00001e50: 5dda 63b0 9e09 811e 1c3d 9a10 825b 1480  ].c......=...[..
-00001e60: b945 a161 b36a a877 f3d0 c149 3f0c 32bd  .E.a.j.w...I?.2.
-00001e70: 6894 8184 a02b 9b56 b1b9 0c1e 659d 9723  h....+.V....e..#
-00001e80: 07f6 3b7c 1931 51ce 47f4 f2dd b64a 3eb6  ..;|.1Q.G....J>.
-00001e90: c239 2227 3dae 6e5a c53a a2c7 df1e 55e7  .9"'=.nZ.:....U.
-00001ea0: 9a91 ff14 23ba 61e5 704b bd4b 7a0c d633  ....#.a.pK.Kz..3
-00001eb0: 2330 4a46 8f2e 8c60 0676 000c 061f 01f3  #0JF...`.v......
-00001ec0: 700b 6066 981a 6662 f0a2 60bb 6a64 3f67  p.`f..fb..`.jd?g
-00001ed0: 788e ad35 8490 35a3 2b8d ee48 eb90 607a  x..5..5.+..H..`z
-00001ee0: 42c8 d55c 7b67 3f67 bdbe 8b29 d6d9 4563  B..\{g?g...)..Ec
-00001ef0: e5e3 8c59 3df2 8e1e 5c49 30eb 5dc2 63b0  ...Y=...\I0.].c.
-00001f00: 9e09 41e1 d1a3 0921 9860 0266 8209 9809  ..A....!.`.f....
-00001f10: 2660 4308 f5db 9610 9bd2 a3bc 3bec 629a  &`C.........;.b.
-00001f20: b012 4722 1fa7 9de4 133c 2205 81b2 97d8  ..G".....<".....
-00001f30: 393a 080d 8c90 34c6 4e11 99e3 961b 8cc8  9:....4.N.......
-00001f40: 7faf 3156 9c1b 56b1 1815 bcab 2e74 c9fd  ..1V..V......t..
-00001f50: 15fd bdd6 5dc2 639d 0a8f 357e 71f4 e8cc  ....].c...5~q...
-00001f60: 0847 39f5 0098 0926 6026 980a 2ead cb37  .G9....&`&.....7
-00001f70: b545 7978 72b9 8914 32ea df34 d1cb 3d19  .Eyxr...2..4..=.
-00001f80: 9e8b 8ead b72e cfaf 0a39 6171 7d55 c87f  .........9aq}U..
-00001f90: a631 561c 9d71 8bc5 c6e5 da01 6be9 e52e  .1V..q......k...
-00001fa0: 61b1 4e85 c59a 471e 3d9a b8dc a497 1a36  a.N...G.=......6
-00001fb0: e9a5 864d a0a0 a543 3309 28d8 3242 bddc  ...M...C3.(.2B..
-00001fc0: 440a 93aa c72d b473 6cae 8d13 e42a 6ed1  D....-.sl....*n.
-00001fd0: 995c 22a7 3bae 4f02 19eb 8d49 20af 3b4a  .\".;.O....I .;J
-00001fe0: 0543 88c3 3821 5b7c 877f 5676 1fea 5dba  .C..8![|..Vv..].
-00001ff0: 63b0 9e97 05ea 8e1e 4d18 c1dd 070d 3323  c.......M.....3#
-00002000: 3a02 e6ee 8382 cbc1 3042 e98e 9611 9b87  :.......0B......
-00002010: 1ee5 ddbe 635b b3fb 10db 6b29 21e1 60db  ....c[....k)!.`.
-00002020: 6168 5e68 3d47 0a72 3241 3efd cad0 51a9  ah^h=G.r2A>...Q.
-00002030: 944d f548 2fdb a268 e533 ded8 7d88 55e4  .M.H/..h.3..}.U.
-00002040: 79a7 58cc 336e b1d8 4c12 aa17 925b 837a  y.X.3n..L....[.z
-00002050: 5dd8 253c d6a9 f0c8 c3bb a347 174a 30d8  ].%<.......G.J0.
-00002060: 3e00 e6ee 0360 1e6e 5170 8612 4a71 b394  >....`.nQp..Jq..
-00002070: 5055 3393 4414 f750 a573 6c6e 2699 18e4  PU3.D..P.sln&...
-00002080: 734f 20ed 85d6 4bec 2882 34f9 90d1 3b37  sO ...K.(.4...;7
-00002090: a688 fc99 47f9 c1c0 644e 1151 65d5 c577  ....G...dN.Qe..w
-000020a0: f4ef 4ae4 d8ec d224 83f5 3c45 5093 f468  ..J....$..<EP..h
-000020b0: c207 468e 8019 3902 66e4 a861 5eac 3829  ..F...9.f..a^.8)
-000020c0: d87c ed51 3f4c 3a08 eafb b5e7 ddd9 736c  .|.Q?L:.......sl
-000020d0: aee1 83bf a52d d120 f406 5a07 bd41 3e08  .....-. ..Z..A>.
-000020e0: 247b 55f2 7538 2697 396b 6144 3d88 aadd  ${U.u8&.9kaD=...
-000020f0: 324f 798d 5564 7219 8b39 43c4 627e fc0f  2Oy.Udr..9C.b~..
-00002100: 5db8 925c 36bb 04c9 603d 3382 82a4 4717  ]..\6...`=3...G.
-00002110: 4698 9b13 8099 5c02 6672 a960 5e84 3a29  F.....\.fr.`^.:)
-00002120: d412 62f3 a6b6 3c1b 34ea 413e bd01 8d3a  ..b...<.4.A>...:
-00002130: b697 9490 6fb6 89e6 cc19 82c6 db0a 54ce  ....o.........T.
-00002140: 7a5d 817a d411 0a54 2cc6 ea7d 8bc5 8611  z].z...T,..}....
-00002150: da3f 4b63 a735 e3db e57f 91f4 7f00 0000  .?Kc.5..........
-00002160: ffff 0000 00ff ffb2 2948 4c4f f54d 2c4a  ........)HLO.M,J
-00002170: cfcc 2b56 c849 4d2b b155 32d0 3337 5552  ..+V.IM+.U2.37UR
-00002180: 28ca 4ccf 8073 4af2 0b6c 950c 9514 92f2  (.L..sJ..l......
-00002190: 4b4a f273 c1cc 8cd4 c494 d422 906a a0e2  KJ.s.......".j..
-000021a0: b4fc fc12 1847 dfce 46bf 3cbf 28bb 3823  .....G..F.<.(.8#
-000021b0: 35b5 c40e 0000 00ff ff03 0050 4b03 0414  5..........PK...
-000021c0: 0006 0008 0000 0021 00e9 a625 b866 0600  .......!...%.f..
-000021d0: 0053 1b00 0013 0000 0078 6c2f 7468 656d  .S.......xl/them
-000021e0: 652f 7468 656d 6531 2e78 6d6c ec59 cd6e  e/theme1.xml.Y.n
-000021f0: 1b37 10be 17e8 3b10 7b4f 2cd9 9262 1991  .7....;.{O,..b..
-00002200: 034b 96e2 3671 62d8 4a8a 1ca9 5d6a 9711  .K..6qb.J...]j..
-00002210: 77b9 2029 3bba 15c9 b140 81a2 69d1 4b81  w. );....@..i.K.
-00002220: de7a 28da 0648 805e d2a7 719b a24d 81bc  .z(..H.^..q..M..
-00002230: 4287 e44a 5a5a 546c 2706 fa17 1d6c 2df7  B..JZZTl'....l-.
-00002240: e3fc cf70 86ba 7aed 41ca d021 1192 f2ac  ...p..z.A..!....
-00002250: 1554 2f57 0244 b290 4734 8b5b c19d 7eef  .T/W.D..G4.[..~.
-00002260: d27a 80a4 c259 8419 cf48 2b98 1019 5cdb  .z...Y...H+...\.
-00002270: 7cff bdab 7843 2524 2508 f667 7203 b782  |...xC%$%..gr...
-00002280: 44a9 7c63 6545 86b0 8ce5 659e 930c de0d  D.|ceE....e.....
-00002290: b948 b182 4711 af44 021f 01dd 94ad ac56  .H..G..D.......V
-000022a0: 2a8d 9514 d32c 4019 4e81 eced e190 8604  *....,@.N.......
-000022b0: f535 c960 734a bccb e031 5352 2f84 4c1c  .5.`sJ...1SR/.L.
-000022c0: 68d2 c4d9 61b0 d1a8 aa11 7222 3b4c a043  h...a.....r";L.C
-000022d0: cc5a 01f0 89f8 519f 3c50 0162 582a 78d1  .Z....Q.<P.bX*x.
-000022e0: 0a2a e613 ac6c 5e5d c11b c526 a696 ec2d  .*...l^]...&...-
-000022f0: edeb 994f b1af d810 8d56 0d4f 110f 664c  ...O.....V.O..fL
-00002300: abbd 5af3 caf6 8cbe 0130 b588 eb76 bb9d  ..Z......0...v..
-00002310: 6e75 46cf 0070 1882 a656 9632 cd5a 6fbd  nuF..p...V.2.Zo.
-00002320: da9e d22c 81ec d745 da9d 4abd 5273 f125  ...,...E..J.Rs.%
-00002330: fa6b 0b32 37db ed76 bd59 c862 891a 90fd  .k.27..v.Y.b....
-00002340: 5a5b c0af 571a b5ad 5507 6f40 165f 5fc0  Z[..W...U.o@.__.
-00002350: d7da 5b9d 4ec3 c11b 90c5 3716 f0bd 2bcd  ..[.N.....7...+.
-00002360: 46cd c51b 50c2 6836 5a40 6b87 f67a 05f5  F...P.h6Z@k..z..
-00002370: 1964 c8d9 8e17 be0e f0f5 4a01 9fa3 201a  .d........J... .
-00002380: 66d1 a559 0c79 a696 c55a 8aef 73d1 0380  f..Y.y...Z..s...
-00002390: 0632 ac68 86d4 2427 431c 4214 7770 3a10  .2.h..$'C.B.wp:.
-000023a0: 146b 0678 83e0 d21b bb14 ca85 25cd 0bc9  .k.x........%...
-000023b0: 50d0 5cb5 820f 730c 1931 a7f7 eaf9 f7af  P.\...s..1......
-000023c0: 9e3f 45af 9e3f 397e f8ec f8e1 4fc7 8f1e  .?E..?9~....O...
-000023d0: 1d3f fcd1 d272 36ee e02c 2e6f 7cf9 ed67  .?...r6..,.o|..g
-000023e0: 7f7e fd31 fae3 e937 2f1f 7fe1 c7cb 32fe  .~.1...7/.....2.
-000023f0: d71f 3ef9 e5e7 cffd 40c8 a0b9 442f be7c  ..>.....@...D/.|
-00002400: f2db b327 2fbe faf4 f7ef 1e7b e05b 020f  ...'/......{.[..
-00002410: caf0 3e4d 8944 b7c8 11da e729 e866 0ce3  ..>M.D.....).f..
-00002420: 4a4e 06e2 7c3b fa09 a6ce 0e9c 006d 0fe9  JN..|;.......m..
-00002430: ae4a 1ce0 ad09 663e 5c9b b8c6 bb2b a078  .J....f>\....+.x
-00002440: f880 d7c7 f71d 590f 1231 56d4 c3f9 4692  ......Y..1V...F.
-00002450: 3ac0 5dce 599b 0baf 016e 685e 250b f7c7  :.].Y....nh^%...
-00002460: 59ec 672e c665 dc3e c687 3ede 1d9c 39ae  Y.g..e.>..>...9.
-00002470: ed8e 73a8 9ad3 a074 6cdf 4988 23e6 1ec3  ..s....tl.I.#...
-00002480: 99c2 31c9 8842 fa1d 1f11 e2d1 ee1e a58e  ..1..B..........
-00002490: 5d77 6928 b8e4 4385 ee51 d4c6 d46b 923e  ]wi(..C..Q...k.>
-000024a0: 1d38 8134 dfb4 4353 f0cb c4a7 33b8 dab1  .8.4..CS....3...
-000024b0: cdee 5dd4 e6cc a7f5 3639 7491 9010 9879  ..].....69t....y
-000024c0: 84ef 13e6 98f1 3a1e 2b9c fa48 f671 caca  ......:.+..H.q..
-000024d0: 06bf 8955 e213 f260 22c2 32ae 2b15 783a  ...U...`".2.+.x:
-000024e0: 268c a36e 44a4 f4ed b92d 40df 92d3 6f60  &..nD....-@...o`
-000024f0: a857 5eb7 efb2 49ea 2285 a223 1fcd 9b98  .W^...I."..#....
-00002500: f332 729b 8f3a 094e 73af cc34 4bca d80f  .2r..:.Ns..4K...
-00002510: e408 4214 a33d ae7c f05d ee66 887e 063f  ..B..=.|.].f.~.?
-00002520: e06c a9bb ef52 e2b8 fbf4 4270 87c6 8e48  .l...R....Bp...H
-00002530: f300 d16f c6a2 a8da 4efd 4d69 f6ba 62cc  ...o....N.Mi..b.
-00002540: 2854 e377 c578 7a3a 6dc1 d1e4 4b89 9d13  (T.w.xz:m...K...
-00002550: 2578 19ee 5f58 78b7 f138 db23 10eb 8b07  %x.._Xx..8.#....
-00002560: cfbb bafb aeee 06ff f9ba bb2c 97cf 5a6d  ...........,..Zm
-00002570: e705 169a e479 5f6c bae4 7469 933c a48c  .....y_l..ti.<..
-00002580: 1da8 0923 37a5 e993 251c 1651 0f16 4d03  ...#7...%..Q..M.
-00002590: 6fa6 b8d9 d094 27f0 b528 ee0e 2e16 d8ec  o.....'..(......
-000025a0: 4182 ab8f a84a 0e12 9c43 8f5d 3523 5f2c  A....J...C.]5#_,
-000025b0: 0bd2 b144 3997 30db 9965 337c 9213 b4cd  ...D9.0..e3|....
-000025c0: 3849 a1cd 3693 615d cf0c b61e 48ac 7679  8I..6.a]....H.vy
-000025d0: 6497 d7ca b3e1 8c8c 9914 6333 7f4e 19ad  d.........c3.N..
-000025e0: 6902 6765 b676 e5ed 9855 ad54 4bcd e6aa  i.ge.v...U.TK...
-000025f0: 5635 a299 52e7 a836 5319 7cb8 a81a 2cce  V5..R..6S.|...,.
-00002600: ac09 5d08 82de 05ac dc80 115d cb0e b309  ..]........]....
-00002610: 6624 d276 b773 f3d4 2d9a f585 ba48 2638  f$.v.s..-....H&8
-00002620: 2285 8fb4 de8b 3eaa 1a27 4d63 651a 461e  ".....>..'Mce.F.
-00002630: 1fe9 39ef 141f 95b8 3535 d9b7 e076 1627  ..9.....55...v.'
-00002640: 95d9 d596 b09b 7aef 6dbc 341d 6ee7 5ed2  ......z.m.4.n.^.
-00002650: 797b 221d 5956 4e4e 96a1 a356 d0ac afd6  y{".YVNN...V....
-00002660: 0314 e2bc 150c 61ac 85af 690e 5e97 baf1  ......a...i.^...
-00002670: c32c 86bb a150 091b f6a7 26b3 09d7 b937  .,...P....&....7
-00002680: 9bfe b0ac c24d 85b5 fb82 c24e 1dc8 8554  .....M.....N...T
-00002690: db58 2636 34cc ab22 0458 6686 7023 ff6a  .X&64..".Xf.p#.j
-000026a0: 1dcc 7a51 0ad8 487f 0329 d6d6 2118 fe36  ..zQ..H..)..!..6
-000026b0: 29c0 8eae 6bc9 7048 4255 7676 69c5 dc51  )...k.pHBUvvi..Q
-000026c0: 1840 514a f958 1171 9044 4768 c0c6 621f  .@QJ.X.q.DGh..b.
-000026d0: 83fb 75a8 823e 1195 703b 612a 827e 80ab  ..u..>..p;a*.~..
-000026e0: 346d 6df3 ca2d ce45 d295 2fb0 0cce ae63  4mm..-.E../....c
-000026f0: 9627 b828 b73a 45a7 996c e126 8f67 3298  .'.(.:E..l.&.g2.
-00002700: 272b ad11 0f74 f3ca 6e94 3bbf 2a26 e52f  '+...t..n.;.*&./
-00002710: 4895 7218 ffcf 54d1 e709 5c17 ac45 da03  H.r...T...\..E..
-00002720: 21dc e40a 8c74 beb6 022e 54c2 a10a e509  !....t....T.....
-00002730: 0d7b 022e b94c ed80 6881 eb58 780d 4105  .{...L..h..Xx.A.
-00002740: f7c9 e6bf 2087 fabf cd39 4bc3 a435 4c7d  .... ....9K..5L}
-00002750: 6a9f c648 5038 8f54 2208 d983 b264 a2ef  j..HP8.T"....d..
-00002760: 1462 d5e2 ecb2 2459 41c8 4454 495c 995b  .b....$YA.DTI\.[
-00002770: b107 e490 b0be ae81 0d7d b607 2881 5037  .........}..(.P7
-00002780: d5a4 2803 0677 32fe dce7 2283 06b1 6e72  ..(..w2..."...nr
-00002790: fea9 9d8f 4de6 f3b6 07ba 3bb0 2d96 dd7f  ....M.....;.-...
-000027a0: c65e a456 2afa a5a3 a0e9 3dfb 4c4f 352b  .^.V*.....=.LO5+
-000027b0: 07af 39d8 cf79 d4da 8ab5 a0f1 6afd cc47  ..9..y......j..G
-000027c0: 6d0e 973e 48ff 81f3 8f8a 90d9 1f27 f481  m..>H........'..
-000027d0: dae7 fb50 5b11 fcd6 60db 2b04 517d c936  ...P[...`.+.Q}.6
-000027e0: 1e48 1748 5b1e 07d0 38d9 451b 4c9a 946d  .H.H[...8.E.L..m
-000027f0: 588a eef6 c2db 28b8 912e 3add 195f c8d2  X.....(...:.._..
-00002800: 37e9 74cf 69ec 5973 e6b2 7372 f1f5 dde7  7.t.i.Ys..sr....
-00002810: f98c 5d58 d8b1 75b9 d3f5 981a 92f6 648a  ..]X..u.......d.
-00002820: eaf6 683a c818 c798 5fb5 ca3f 3cf1 c17d  ..h:...._..?<..}
-00002830: 70f4 365c f18f 9992 f66a ff01 5cf1 c194  p.6\.....j..\...
-00002840: 617f 2480 e4b7 ce35 5b37 ff02 0000 ffff  a.$....5[7......
-00002850: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-00002860: 8c3e 5b78 7803 0000 d609 0000 0d00 0000  .>[xx...........
-00002870: 786c 2f73 7479 6c65 732e 786d 6cc4 564b  xl/styles.xml.VK
-00002880: 6fdb 3810 be2f d0ff 40f0 aee8 11cb 6b1b  o.8../..@.....k.
-00002890: 928a 3a8e 8002 dd62 8164 811e 72a1 25ca  ..:....b.d..r.%.
-000028a0: 26ca 8740 d1a9 dcc5 fef7 1d92 92ad b469  &..@...........i
-000028b0: bdcd a2a8 0e12 391c 7ef3 fa86 54f6 ba17  ......9.~...T...
-000028c0: 1c3d 52dd 3125 731c 5f45 1851 59a9 9ac9  .=R.1%s._E.QY...
-000028d0: 5d8e ffba 2f83 0546 9d21 b226 5c49 9ae3  ].../..F.!.&\I..
-000028e0: 23ed f0eb e2d5 6f59 678e 9cde ed29 3508  #.....oYg....)5.
-000028f0: 2064 97e3 bd31 ed2a 0cbb 6a4f 05e9 ae54   d...1.*..jO...T
-00002900: 4b25 ac34 4a0b 6260 aa77 61d7 6a4a eace  K%.4J.b`.wa.jJ..
-00002910: 6e12 3c4c a268 1e0a c224 f608 2b51 fd17  n.<L.h...$..+Q..
-00002920: 1041 f4c7 431b 544a b4c4 b02d e3cc 1c1d  .A..C.TJ...-....
-00002930: 1646 a25a bddd 49a5 c996 83ab 7d3c 2315  .F.Z..I.....}<#.
-00002940: eae3 b94e 50af 4723 4efa 951d c12a ad3a  ...NP.G#N....*.:
-00002950: d598 2bc0 0d55 d3b0 8a7e edee 325c 86a4  ..+..U...~..2\..
-00002960: 3a23 01f2 cb90 e234 8c92 27b1 f7fa 8548  :#.....4..'....H
-00002970: b350 d347 66cb 878b 4c1e 4429 4c87 2a75  .P.Gf...L.D)L.*u
-00002980: 9006 ca79 1221 bff2 b606 e13c c5c8 57e5  ...y.!.....<..W.
-00002990: 46d5 b6a4 f03c 0442 3c04 75fd 80f6 fb95  F....<.B<.u.....
-000029a0: 10ab aec3 6191 8503 5e91 354a 9e61 13c8  ....a...^.5J.a..
-000029b0: 80cd edea a354 9f64 6997 bc2d ab55 64dd  .....T.di..-.Ud.
-000029c0: 67f4 4838 4862 8b51 29ae 3432 c009 30e5  g.H8Hb.Q).42..0.
-000029d0: 2492 08ea 356e 0867 5bcd ac5a 4304 e347  $...5n.g[..ZC..G
-000029e0: 2f4e acc0 d168 d013 0c8a ea1c f216 fc7b  /N...h.........{
-000029f0: 6bb5 9ed8 7a16 39f4 daee d381 21c6 f929  k...z.9.....!..)
-00002a00: 4109 24c8 0a8a 0cb8 64a8 9625 4cd0 30be  A.$.....d..%L.0.
-00002a10: 3fb6 e0b2 04da 7bd3 4eef 82f6 4e93 639c  ?.....{.N...N.c.
-00002a20: a493 0da1 3358 645b a56b 68b3 b134 d760  ....3Xd[.kh..4.`
-00002a30: d98b 8a8c d3c6 402c 9aed f6f6 6b54 0bef  ......@,....kT..
-00002a40: ad32 06a8 5864 3523 3b25 09b7 f518 774c  .2..Xd5#;%....wL
-00002a50: 7742 7b42 27e6 d8ec a193 c67c 9383 5143  wB{B'......|..QC
-00002a60: ba43 0b3f a05f d475 3e38 172e aa82 9ba3  .C.?._.u>8......
-00002a70: 9717 757d 30bf 2c96 4be9 1cf2 0aec a828  ..u}0.,.K......(
-00002a80: e777 369f 1f9a 275d d437 930e 8233 d272  .w6...'].7...3.r
-00002a90: ca36 931d 022f 86a1 2f8b 9fd8 724d d13c  .6.../../...rM.<
-00002aa0: f604 7606 c5fa 7158 d437 27fc 6fed 8ebf  ..v...qX.7'.o...
-00002ab0: e114 c8c7 dd88 b42d 3fda d6b5 2cf1 b3b5  .......-?...,...
-00002ac0: 63e8 79fe 86b3 9d14 743c 48a0 57fd 14ed  c.y.....t<H.W...
-00002ad0: 9566 9f61 ab6d f20a d629 1cae 7085 1856  .f.a.m...)..p..V
-00002ae0: 5909 f0c2 d1bf 6fbe 886f 3878 2e25 ee0b  Y.....o..o8x.%..
-00002af0: 1fdf 1fc4 96ea d2dd 2203 a37f 346e 7b5e  ........"...4n{^
-00002b00: 0d59 7b2e 6edb f33f 350b 8e07 50f9 09bd  .Y{.n..?5...P...
-00002b10: 9e90 eb44 1364 0fb0 1cbf b7c1 f289 d3db  ...D.d..........
-00002b20: 03e3 86c9 6788 0598 757f a66a 6433 6fec  ....g...u..jd3o.
-00002b30: f5e7 487c b202 34ad 6943 0edc dc9f 1673  ..H|..4.iC.....s
-00002b40: 7c1e ff41 6b76 10cb 93d6 9fec 5119 0791  |..Akv......Q...
-00002b50: e3f3 f89d 3da0 e2b9 b541 7bf3 ae83 5305  ....=....A{...S.
-00002b60: bee8 a059 8eff be5d ffbe dcdc 9649 b088  ...Y...].....I..
-00002b70: d68b 6076 4dd3 6099 ae37 413a bb59 6f36  ..`vM.`..7A:.Yo6
-00002b80: e532 4aa2 9b7f 2697 f0ff b882 dd3f 0390  .2J...&......?..
-00002b90: 2b9e ad3a 0e17 b51e 821d 42bc 3bcb 723c  +..:......B.;.r<
-00002ba0: 9978 f71d 37c1 eda9 efcb 641e bd49 e328  .x..7.....d..I.(
-00002bb0: 28af a338 98cd c922 58cc afd3 a04c e364  (..8..."X....L.d
-00002bc0: 339f ad6f d332 9df8 9ebe f0aa 8ec2 38f6  3..o.2........8.
-00002bd0: 97be 753e 5d19 2628 6772 acd5 58a1 a914  ..u>].&(gr..X...
-00002be0: 8a04 d3ef 0411 8e95 08cf 3f64 c5bf 0000  ..........?d....
-00002bf0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00002c00: 0021 006b dcd4 f9ab 0500 00e1 3e00 0014  .!.k........>...
-00002c10: 0000 0078 6c2f 7368 6172 6564 5374 7269  ...xl/sharedStri
-00002c20: 6e67 732e 786d 6cd4 9b5b 6fe2 3818 86ef  ngs.xml..[o.8...
-00002c30: 57da ff90 e59e a494 969d a928 a32e d051  W..........(...Q
-00002c40: b5d3 83a0 bd8b 14a5 c180 7713 2763 3b6c  ..........w.'c;l
-00002c50: 995f bf5f cad9 0730 4d54 928b 5ed4 87f8  ._._...0MT..^...
-00002c60: fd9e bcf1 09bb fded 2d0a ad19 a20c c7e4  ........-.......
-00002c70: bad6 b0cf 6a16 2241 3cc2 6472 5d7b 79be  ....j."A<.dr]{y.
-00002c80: ad7f a959 8cfb 64e4 8731 41d7 b539 62b5  ...Y..d..1A..9b.
-00002c90: 6f9d df7f 6b33 c62d a84b d875 6dca 7972  o...k3.-.K.um.yr
-00002ca0: e538 2c98 a2c8 6776 9c20 0239 e398 463e  .8,...gv. .9..F>
-00002cb0: 877f e9c4 6109 45fe 884d 11e2 51e8 9c9f  ....a.E..M..Q...
-00002cc0: 9db5 9cc8 c7a4 6605 714a f875 add9 baac  ......f.qJ.u....
-00002cd0: 5929 c13f 53d4 5da4 9c37 2f6a 9d36 c39d  Y).?S.]..7/j.6..
-00002ce0: 36ef dc91 117a 6b3b bcd3 76b2 8445 e200  6....zk;..v..E..
-00002cf0: 853e c733 f4e0 4748 ccbb 4dc3 5095 fe97  .>.3..GH..M.P...
-00002d00: cf10 5194 efbf 7144 3202 e283 9e7c 8a08  ..Q...qD2....|..
-00002d10: 1753 6f38 a7f8 35e5 52bb 43fc 4b4a eb42  .So8..5.R.C.KJ.B
-00002d20: e41c f5e0 4f7c cc3d 501e 6334 52e5 dd04  ....O|.=P.c4R...
-00002d30: 0162 4c95 f303 cd50 28c3 187b 4314 706d  .bL....P(..{C.pm
-00002d40: 08de 008d a530 6830 0580 5916 8230 0349  .....0h0..Y..0.I
-00002d50: a00b 6ff2 cd8b 7c82 c788 716f 8208 a23e  ..o...|...qo...>
-00002d60: 8fa9 f8a0 ee95 fbc2 c042 6e77 4a31 b39f  .........BnwJ1..
-00002d70: 2886 87b9 2f04 87a0 95ba 2f37 837b eb19  (.../...../7.{..
-00002d80: f911 c31c 5975 eb66 d1ae dbc3 13cc fdd0  ....Yu.f........
-00002d90: 7aa2 086a cfe0 6dc6 c485 a469 fa6a daf2  z..j..m....i.j..
-00002da0: c904 8a08 7a58 a272 2696 d105 e58e 3093  ....zX.r&.....0.
-00002db0: 3cf6 794c 95cd ab24 358e 0a48 176d 1dfa  <.yL...$5..H.m..
-00002dc0: 18fb b29e cc9b 7502 3d4a dd27 73fb bfa9  ......u.=J.'s...
-00002dd0: e4e8 4f8e 3fa7 5a8d 0f15 b18a 0c55 b1df  ..O.?.Z......U..
-00002de0: c287 2396 6b38 45e2 b7b9 4fed c9af d37d  ..#.k8E...O....}
-00002df0: c8ef a6db 0f5d a371 2fea ac8e 4458 8eb3  .....].q/...DX..
-00002e00: e19c 17e7 e556 a5bc 7c58 ed3e c0bb b565  .....V..|X.>...e
-00002e10: 8f36 0bc4 5a01 8fb6 3ee0 d1f7 3a32 b98b  .6..Z...>...:2..
-00002e20: a2c8 41f7 5a21 439a a8d5 1b52 ac2d 63bd  ..A.Z!C....R.-c.
-00002e30: 2c10 6be9 0d99 8dac ea8e 7d2f 4255 a7d9  ,.k.......}/BU..
-00002e40: 705a c6e4 7edc 75fb 0fc3 be1d 8d4e 389e  pZ..~.u......N8.
-00002e50: e845 2c73 a461 4196 6b3e 2894 6e62 6c3a  .E,s.aA.k>(.nbl:
-00002e60: 6136 efa0 3521 ba9e 8709 e69e 6727 f313  a6..5!......g'..
-00002e70: beee 0fa8 5b09 978c 2007 d23c 62b2 a557  ....[... ..<b..W
-00002e80: 92cc 031f 96c4 9e57 4a4e 5a75 9ea7 cd6a  .......WJNZu...j
-00002e90: 1e31 6f32 e0b2 f152 90cc f934 26f5 66e3  .1o2...R...4&.f.
-00002ea0: 0c7c 1594 1b98 b1ec f5a7 b215 9ec2 7d52  .|............}R
-00002eb0: b880 b958 03aa 149f 5713 b452 b602 b4d4  ...X....W..R....
-00002ec0: 9767 5073 77f0 0072 fd71 b841 88ed 6a19  .gPsw..r.q.A..j.
-00002ed0: d740 b150 44b4 6b46 b188 3144 47b1 0aae  .@.PD.kF..1DG...
-00002ee0: dc45 a454 2c14 5151 349f f09b f4a4 411c  .E.T,.QQ4.....A.
-00002ef0: 4531 a99a 1d8d 44cb a1a9 709a 4ff4 3f84  E1....D...p.O.?.
-00002f00: b312 be14 71aa ad29 9552 e134 9ffd 9be0  ....q..).R.4....
-00002f10: 9cfa 6c5a 316f 9a48 16cb a840 fe69 bc8c  ..lZ1o.H...@.i..
-00002f20: fa00 c82a b852 80a4 942c 9651 81fc 5228  ...*.R...,.Q..R(
-00002f30: c81d d815 b3e6 51da b585 558c bf7e 0ae3  ......Q...U..~..
-00002f40: 2ab8 5687 4da9 5d5b 58c5 b861 febb 9049  *.V.M.][X..a...I
-00002f50: 8fb0 5b66 d6d8 f272 e538 7b87 e5ef 0b57  ..[f...r.8{....W
-00002f60: 49db fc57 1313 dacb 1fca 2bd6 6118 aa56  I..W......+.a..V
-00002f70: 1453 222d 7615 25b7 5a05 df1a aa56 1453  .S"-v.%.Z....V.S
-00002f80: 22cd bfa4 ca56 1ca5 dc91 530b 8354 1944  "....V....S..T.D
-00002f90: 0114 1693 db72 82d0 695b 2c70 641c f957  .....r..i[,pd..W
-00002fa0: 88ef f3aa 52c2 d028 cb92 6510 f9d7 7611  ....R..(..e...v.
-00002fb0: e2fe c8e7 bef8 ec4f 3c65 a01b 5e74 d274  .......O<e..^t.t
-00002fc0: e9cd 237e 9939 d4a6 db4b 5f43 4cba 3145  ..#~.9...K_CL.1E
-00002fd0: 7040 274a e044 15b2 e1e8 5689 3199 4a56  p@'J.D....V.1.JV
-00002fe0: 4426 46a5 8a14 e816 b0f5 ba7a 776e ffa6  D&F........zwn..
-00002ff0: 5719 b087 b46e e7cb df68 ab80 cdd5 35b6  W....n...h....5.
-00003000: efbd a741 65b8 1d14 bb53 4045 2eff b8b7  ...Ae....S@E....
-00003010: 2677 ffd8 1b56 86dc 41b1 3b05 54e4 f20f  &w...V..A.;.T...
-00003020: 91bb 6bb7 528e 9587 24ee e4cb 94f2 ef40  ..k.R...$......@
-00003030: 498b aef2 63ca 9692 b24a 3110 1956 fe5d  I...c....J1..V.]
-00003040: 26e6 c338 8a58 0987 508d 324d 72d3 c9bf  &..8.X..P.2Mr...
-00003050: 1bb4 7cb4 fb08 e788 4b3a af38 2431 932e  ..|.....K:.8$1..
-00003060: dbe4 6b01 9384 55cb cbb3 f1e5 358c ab51  ..k...U.....5..Q
-00003070: a849 06e3 1430 1710 e8b8 a380 af27 a821  .I...0.......'.!
-00003080: 935e 4909 26f2 472a de04 24cf 4b15 01be  .^I.&.G*..$.K...
-00003090: 532d c075 3c3b c95f dacd 823d ea56 59f2  S-.u<;._...=.VY.
-000030a0: c758 c08e ea6a 9fa6 9403 9b5e dc32 4781  .X...j.....^.2G.
-000030b0: 24f7 b6a7 8d26 933a 26e3 b87c fd92 569a  $....&.:&..|..V.
-000030c0: 3623 f734 71fd 6477 84e0 76d3 086e cbcc  6#.4q.dw..v..n..
-000030d0: 3d58 39ff cb6c fe76 cabb 1b9a 15fe 717a  =X9..l.v......qz
-000030e0: c598 a40e 4911 e345 febe 6823 12ee 58d1  ....I..E..h#..X.
-000030f0: b997 c498 c07d b192 033d a475 3b5f 0479  .....}...=.u;_.y
-00003100: 917f 60dc 407b fafb 7bfd eee1 f6b1 c41f  ..`.@{..{.......
-00003110: a8ab d3a8 4bbf c87f b868 0388 a29f 2986  ....K....h....).
-00003120: bb65 6577 d43e 9dab 3cd9 4905 f669 c3c7  .eew.>..<.I..i..
-00003130: 9741 b73f 2c3b a73d 3297 5932 a5dc 5bc7  .A.?,;.=2.Y2..[.
-00003140: 1b3b f138 f1b2 0b8d 61d9 39ed 15ba ce94  .;.8....a.9.....
-00003150: 5999 9ff9 49e6 098d ff81 fba6 368f 4fba  Y...I.......6.O.
-00003160: 5bbc 5fc8 3a57 1ed0 14b2 cdad 3280 add0  [._.:W......2...
-00003170: fb13 df77 d06a 5864 8811 4bef f619 73f9  ...w.jXd..K...s.
-00003180: 9261 0fb1 80e2 4475 8d18 6e17 a714 73e9  .a....Du..n...s.
-00003190: ccff 1dcc 8578 768d 995e 7553 0676 b8eb  .....xv..^uS.v..
-000031a0: 896d f709 47d4 9ac7 29b5 b61a b0a6 70e9  .m..G...).....p.
-000031b0: f80f b12c 2cb7 a54b d85b f5df 55ab 6b0e  ...,,..K.[..U.k.
-000031c0: e1f9 01da 6edd 812b ea9d ff01 0000 ffff  ....n..+........
-000031d0: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-000031e0: bd84 6223 9000 0000 db00 0000 1300 2800  ..b#..........(.
-000031f0: 6375 7374 6f6d 586d 6c2f 6974 656d 312e  customXml/item1.
-00003200: 786d 6c20 a224 0028 a020 0000 0000 0000  xml .$.(. ......
-00003210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003220: 0000 0000 0000 0000 0000 006c 8e3b 0ec2  ...........l.;..
-00003230: 3010 05af 82d2 932d e8d0 e234 810a 51e5  0......-...4..Q.
-00003240: 02c6 388a a5ac d7f2 2e1f df1e 0741 8194  ..8..........A..
-00003250: 7a9e 661e 7624 bc75 1cd5 471d 4af2 9dc1  z.f.v$.u..G.J...
-00003260: 1367 1a3c a5d9 aa97 cd8b e628 8766 524d  .g.<.......(.fRM
-00003270: 7b00 7193 272b 2d05 9759 78d4 d631 814c  {.q.'+-..Yx..1.L
-00003280: 36fb c421 2a3c 76f0 b569 b5c1 585d d218  6..!*<v..i..X]..
-00003290: ec83 545f 313d bb3b d5d4 395c b3cd 6549  ..T_1=.;..9\..eI
-000032a0: 21fc 201e 6f41 d727 1f82 17ff 5cc7 0b40  !. .oA.'....\..@
-000032b0: f83b 6ede 0000 00ff ff03 0050 4b03 0414  .;n........PK...
-000032c0: 0006 0008 0000 0021 0035 9680 1df1 0000  .......!.5......
-000032d0: 004f 0100 0018 0028 0063 7573 746f 6d58  .O.....(.customX
-000032e0: 6d6c 2f69 7465 6d50 726f 7073 312e 786d  ml/itemProps1.xm
-000032f0: 6c20 a224 0028 a020 0000 0000 0000 0000  l .$.(. ........
-00003300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003310: 0000 0000 0000 0000 0064 9041 6bc3 300c  .........d.Ak.0.
-00003320: 85ef 83fd 87a0 7b6a 3749 c728 494a 3a77  ......{j7I.(IJ:w
-00003330: d0eb d860 57e3 288d 21b6 82ad 948d b1ff  ...`W.(.!.......
-00003340: 3e87 9dba 5d24 9e84 def7 507d f870 5376  >...]$....P}.pSv
-00003350: c510 2df9 06b6 1b09 197a 43bd f597 06de  ..-......zC.....
-00003360: 5e9f f347 c822 6bdf eb89 3c36 e009 0eed  ^..G."k...<6....
-00003370: fd5d ddc7 7daf 5947 a680 6746 97a5 814d  .]..}.YG..gF...M
-00003380: fdac 1af8 aaba 62a7 4e4f bbfc 7494 5d5e  ......b.NO..t.]^
-00003390: 55a5 cc3b a552 29ab 6d71 2c55 51c9 f21b  U..;.R).mq,UQ...
-000033a0: b284 f6c9 2636 3032 cf7b 21a2 19d1 e9b8  ....&602.{!.....
-000033b0: a119 7d5a 0e14 9ce6 24c3 45d0 3058 838a  ..}Z....$.E.0X..
-000033c0: cce2 d0b3 28a4 7c10 6649 78f7 ee26 68d7  ....(.|.fIx..&h.
-000033d0: 3cbf d72f 38c4 5bb9 465b 82fd 4771 d604  <../8.[.F[..Gq..
-000033e0: 8a34 f0c6 9013 71d4 0167 b2c9 fc5a 0a43  .4....q..g...Z.C
-000033f0: 9e13 873f 6714 6b8c 08a2 adc5 1fc8 aa6f  ...?g.k........o
-00003400: 9ed0 fe00 0000 ffff 0300 504b 0304 1400  ..........PK....
-00003410: 0600 0800 0000 2100 635b 0d84 6001 0000  ......!.c[..`...
-00003420: 9106 0000 1300 2400 6375 7374 6f6d 586d  ......$.customXm
-00003430: 6c2f 6974 656d 322e 786d 6c20 a220 0028  l/item2.xml . .(
-00003440: a020 0000 0000 0000 0000 0000 0000 0000  . ..............
-00003450: 0000 0000 0000 0000 0000 0000 0000 00ec  ................
-00003460: 955d 4fc2 3014 86ff cac2 35ae 1b12 0ca4  .]O.0.....5.....
-00003470: 2b31 1095 18d0 007a df95 836b ecc7 ec07  +1.....z...k....
-00003480: 71fe 7abb 9141 b820 f146 aec8 92f5 9c9e  q.z..A. .F......
-00003490: f6f4 ed79 d216 8fa5 d537 4c2b 07ca adab  ...y.....7L+....
-000034a0: 12c6 04db 1246 4b60 c077 606c f42d 85b2  .....FK`.w`l.-..
-000034b0: a3d0 9775 0ae7 ca11 4296 1520 a98d 2567  ...u....B.. ..%g
-000034c0: 465b bd75 31d3 12d9 821a 2835 570e c12e  F[.u1.....(5W...
-000034d0: 24b3 1d82 db2c 042f a804 32d5 cccb 108a  $....,./..2.....
-000034e0: 66d3 e811 1418 eab4 c1a8 89e1 55a5 5861  f...........U.Xa
-000034f0: b4e2 3fd4 71ad 48eb 6b6f 316a 9d36 886b  ..?.q.H.ko1j.6.k
-00003500: a924 4d92 24c5 a8b1 f10a be3c 2806 0b2f  .$M.$......<(../
-00003510: 7330 4d2c cc3b edc4 6f46 108c 9aff bdb5  s0M,.;..oF......
-00003520: 2073 5191 f961 1b2f db2d 6710 b732 e754   sQ..a./.-g..2.T
-00003530: d10f a805 77a3 f750 8aa0 2a4b 0771 527f  ....w..P..*K.qR.
-00003540: dd68 e285 f306 3205 de19 2aba d1ab cf05  .h....2...*.....
-00003550: 67cf 50ad f527 a8ec 2e85 61ce 204d 43db  g.P..'....a. MC.
-00003560: ef0d 1946 8715 f144 506b ffb2 703c 0b60  ...F...DPk..p<.`
-00003570: 8ca2 a216 35db 3c51 b511 104a b64f 80a7  ....5.<Q...J.O..
-00003580: d4d1 b09f 7df3 c045 181b dc83 712c ffd1  ....}..E....q,..
-00003590: fa37 10bd f320 02a3 2b88 fa34 5de4 44f4  .7... ..+..4].D.
-000035a0: cf83 088c ae20 2e06 6270 1ec4 ed15 c4fe  ..... ..bp......
-000035b0: 7d09 d7d5 c973 437e 0100 00ff ff03 0050  }....sC~.......P
-000035c0: 4b03 0414 0006 0008 0000 0021 00b8 b7cf  K..........!....
-000035d0: 58ea 0000 0041 0100 0018 0028 0063 7573  X....A.....(.cus
-000035e0: 746f 6d58 6d6c 2f69 7465 6d50 726f 7073  tomXml/itemProps
-000035f0: 322e 786d 6c20 a224 0028 a020 0000 0000  2.xml .$.(. ....
-00003600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003610: 0000 0000 0000 0000 0000 0000 0064 8f41  .............d.A
-00003620: 6b83 4010 85ef 85fe 0799 bbae d16a 6c50  k.@..........jlP
-00003630: 4352 1bc8 b534 d0eb b28e 71c1 dd91 9d35  CR...4....q....5
-00003640: 144a ff7b 577a 4a7b 1886 37c3 bcef 4dbd  .J.{WzJ{..7...M.
-00003650: ff34 5374 43c7 9a6c 039b 2485 08ad a25e  .4StC..l..$....^
-00003660: db6b 0397 f753 5c41 c45e da5e 4e64 b101  .k...S\A.^.^Nd..
-00003670: 4bb0 6f1f 1fea 9e77 bdf4 923d 393c 7b34  K.o....w...=9<{4
-00003680: 5118 e8d0 cf5d 035f d969 7b78 4ebb 2e0e  Q....]._.i{xN...
-00003690: 95c6 4f45 99c7 873c 2be2 eaf5 a52b 8fdb  ..OE...<+....+..
-000036a0: 63b1 c9ab 6f88 02da 061b 6e60 f47e de09  c...o.....n`.~..
-000036b0: c16a 4423 39a1 196d 580e e48c f441 baab  .jD#9..mX....A..
-000036c0: a061 d00a 3b52 8b41 eb45 96a6 a550 4bc0  .a..;R.A.E...PK.
-000036d0: 9b0f 3341 bbe6 f9bd 7ec3 81ef e51a 6d71  ..3A....~.....mq
-000036e0: fa1f c568 e588 69f0 8922 2378 940e 67d2  ...h..i.."#x..g.
-000036f0: c11c 6f01 c120 da5a fcb1 5df5 dddb ed0f  ..o.. .Z..].....
-00003700: 0000 00ff ff03 0050 4b03 040a 0000 0000  .......PK.......
-00003710: 0000 0021 00ff ffff ffd5 0d00 00d5 0d00  ...!............
-00003720: 0010 0000 005b 7472 6173 685d 2f30 3030  .....[trash]/000
-00003730: 302e 6461 74ff ffff ff00 0000 0000 0000  0.dat...........
-00003740: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003750: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000b40: 0000 0000 0000 0000 0000 bc94 4d6b c330  ............Mk.0
+00000b50: 0c86 ef83 fd87 e0fb e224 edba 31ea f432  .........$..1..2
+00000b60: 06bd 6e1d ec6a 1ce5 83c6 76b0 d46d f9f7  ..n..j....v..m..
+00000b70: 3319 6b52 28de 25e4 6290 845f 3dbc b6b4  3.kR(.%.b.._=...
+00000b80: dd7d eb36 fa04 878d 3582 a571 c222 30ca  .}.6....5..q."0.
+00000b90: 168d a904 7b3f bcdc 3db2 0849 9a42 b6d6  ....{?..=..I.B..
+00000ba0: 8060 3d20 dbe5 b737 db57 6825 f94b 5837  .`= ...7.Wh%.KX7
+00000bb0: 1d46 5ec5 a060 3551 f7c4 39aa 1ab4 c4d8  .F^..`5Q..9.....
+00000bc0: 7660 7ca5 b44e 4bf2 a1ab 7827 d551 56c0  v`|..NK...x'.QV.
+00000bd0: b324 d970 37d5 60f9 8566 b42f 0473 fbc2  .$.p7.`..f./.s..
+00000be0: f73f f49d effc bfb6 2dcb 46c1 b355 270d  .?......-.F..U'.
+00000bf0: 86ae b4e0 ea84 64f5 876e bda8 7415 9060  ......d..n..t..`
+00000c00: 713c 6679 43a0 d7b1 4766 fc3a cd6a 4e1a  q<fyC...Gf.:.jN.
+00000c10: a4be f576 9e51 7ee3 50fb 87a5 cd58 8568  ...v.Q~.P....X.h
+00000c20: b239 69c8 7f19 18bd 1842 3e9c 6988 219d  .9i......B>.i.!.
+00000c30: 93e1 cbba 23d6 0034 729c 53c8 874a 1066  ....#..4r.S..J.f
+00000c40: b3f4 f364 216b ee97 a609 7ab3 9e75 726a  ...d!k....z..urj
+00000c50: e9a0 7823 e7d7 d474 80a6 e93f 6bf8 c5a6  ..x#...t...?k...
+00000c60: ca7f 0000 00ff ff03 0050 4b03 0414 0006  .........PK.....
+00000c70: 0008 0000 0021 00c1 fe8f 3939 1500 009e  .....!....99....
+00000c80: 6e00 0018 0000 0078 6c2f 776f 726b 7368  n......xl/worksh
+00000c90: 6565 7473 2f73 6865 6574 312e 786d 6c9c  eets/sheet1.xml.
+00000ca0: 94dd 8e9b 3010 85ef 2bf5 1d2c df07 6342  ....0...+..,..cB
+00000cb0: 4882 4256 d5ae 56dd bbaa ddb6 d78e 1982  H.BV..V.........
+00000cc0: 158c a9ed fca9 eabb 7780 90ac 1455 4917  ........w....UI.
+00000cd0: 8119 6cce 773c f6c0 e2e1 a02b b203 eb94  ..l.w<.....+....
+00000ce0: a933 ca83 9012 a8a5 c955 bdce e8f7 d7e7  .3.......U......
+00000cf0: d18c 12e7 459d 8bca d490 d123 38fa b0fc  ....E......#8...
+00000d00: f861 b137 76e3 4a00 4f90 50bb 8c96 de37  .a.7v.J.O.P....7
+00000d10: 2963 4e96 a085 0b4c 0335 8e14 c66a e1f1  )cN....L.5...j..
+00000d20: d1ae 996b 2c88 bc13 e98a 4561 9830 2d54  ...k,.....Ea.0-T
+00000d30: 4d7b 426a ef61 98a2 5012 9e8c dc6a a87d  M{Bj.a..P....j.}
+00000d40: 0fb1 5009 8ff3 77a5 6adc 40d3 f21e 9c16  ..P...w.j.@.....
+00000d50: 76b3 6d46 d2e8 0611 2b55 297f eca0 9468  v.mF....+U)....h
+00000d60: 99be ac6b 63c5 aac2 bc0f 3c16 921c 2c9e  ...kc.....<...,.
+00000d70: 115e e3c1 a6eb bf72 d24a 5ae3 4ce1 0324  .^.....r.JZ.L..$
+00000d80: b37e ced7 e9cf d99c 0979 265d e77f 1786  .~.......y&]....
+00000d90: c7cc c24e b51b 7841 45ef 9b12 9f9c 59d1  ...N..xAE.....Y.
+00000da0: 0536 7e27 2c39 c3da e5b2 e956 e519 fd1d  .6~',9.....V....
+00000db0: 9e8e 11de 79db 8497 6618 fb43 978b 5ce1  ....y...f..C..\.
+00000dc0: 0eb7 5911 0b45 463f f1f4 75c2 295b 2eba  ..Y..EF?..u.)[..
+00000dd0: 02fa a160 efde c4c4 8bd5 37a8 407a 4013  ...`......7.@z@.
+00000de0: 4e49 5b9f 2b63 36ed 8b2f d815 22d2 752f  NI[.+c6../..".u/
+00000df0: b448 21bd dac1 2354 5546 1f31 55f7 ab33  .H!...#TUF.1U..3
+00000e00: c110 0dd8 d9e1 6d3c b83d 7715 fdc5 921c  ......m<.=w.....
+00000e10: 0ab1 adfc 57b3 ff0c 6a5d 7ab4 8d83 1833  ....W...j]z....3
+00000e20: 6d4b 25cd 8f4f e024 d628 5a07 e316 2b4d  mK%..O.$.(Z...+M
+00000e30: 850c 6c89 56f8 ade1 9a68 71e8 ee7b 95fb  ..l.V....hq..{..
+00000e40: 12e5 e134 88f8 6c3a a144 6e9d 37fa e7a9  ...4..l:.Dn.7...
+00000e50: ffa4 ee75 1c87 3b61 1b9c 9451 18f0 703e  ...u..;a...Q..p>
+00000e60: bea5 4c06 2506 1765 92c4 6112 dd30 9d0e  ..L.%..e..a..0..
+00000e70: 520c 0669 7c97 29fe 40fa e962 3024 ca83  R..i|.).@..b0$..
+00000e80: d92c 99de 4e75 3e68 31f8 af54 23fc 8f75  .,..Nu>h1..T#..u
+00000e90: ae6d 30b8 46c1 6412 27ff 585f d66d cf5f  .m0.F.d.'.X_.m._
+00000ea0: 0000 00ff ff00 0000 ffff 949d eb8e e336  ...............6
+00000eb0: 1285 5f25 9807 e848 d43d 980c b0b2 db1d  .._%...H.=......
+00000ec0: dbdd 762e fb02 c1ec 00fb 2bbb c804 d9dd  ..v.......+.....
+00000ed0: b7df 2245 4bac af28 7514 0c32 014f 4926  .."EK..(u..2.OI&
+00000ee0: 5987 64d5 21a9 7cfc facf 2f5f fe38 fefa  Y.d.!.|.../_.8..
+00000ef0: c7af 9f3e fefe afff 7cf3 fbf7 1fca 0fdf  ...>....|.......
+00000f00: 7cfd f7af bf7d 95ff face 151f bef9 6f59  |....}........oY
+00000f10: fffa f9bb 7ffc eff8 e5eb e72f bffd f1fd  .........../....
+00000f20: 87e2 a9fa f0e9 e367 6ffb 376f 1c1e 91f2  .......go.7o....
+00000f30: af52 fae7 a7e2 e3b7 7f7e faf8 ede7 6831  .R.......~....h1
+00000f40: 5a8b 525b 1cac 85d3 1647 6b51 698b 676b  Z.R[.....GkQi.gk
+00000f50: 516b 8b93 b568 b4c5 8bb5 68b5 c50f d6a2  Qk...h....h.....
+00000f60: d316 676b d16b 8b8b b518 b4c5 35d3 63e8  ..gk.k......5.c.
+00000f70: d4d7 8c09 7af5 2d63 826e bd65 4cd0 aff7  ....z.-c.n.eL...
+00000f80: 8c09 3af6 c7c9 a4fa f0cd 4c01 e7d0 713f  ..:.......L...q?
+00000f90: e56c d075 3fe7 6cd0 79bf e46c d07d 7fcf  .l.u?.l.y..l.}..
+00000fa0: d854 4bb3 be15 96cf 5477 7ba8 ee8d 3dd5  .TK.....Tw{...=.
+00000fb0: 7324 176c 6e7d 095e 1d14 889e 392a 105d  s$.ln}.^....9*.]
+00000fc0: 7252 20fa e245 81e8 841f 5ca8 665d 0cf8  rR ..E....\.f]..
+00000fd0: bdf3 d48a 0837 555d 3e55 6dd1 7685 fcbb  .....7U]>Um.v...
+00000fe0: abf0 fb17 18f7 ed53 dd0e 655d bbb6 eb1d  .......S..e]....
+00000ff0: a872 cd18 f7c5 d094 8573 6505 76be 4e15  .r.......se.v.N.
+00001000: 00ad dfb2 a5b7 6ce9 3d6d bec3 8b7e 5460  ......l.=m...~T`
+00001010: 05de ffa4 513c fbb3 4651 f15f a6ca 2ca5  ....Q<..FQ._..,.
+00001020: 8a4f 3208 fefa d4e9 8d1f 7cc2 af8c 6a34  .O2.......|...j4
+00001030: 71be d443 0d53 a502 e1a2 530a 9660 c68b  q..C.S....S..`..
+00001040: 02c9 273f e3ff f929 c3a7 a915 e053 37f4  ..'?...).....S7.
+00001050: ae74 6e40 c75f 601c f8e4 9c13 9a54 2d29  .tn@._`......T-)
+00001060: 72cd 1877 45d9 3745 d5b9 0283 e175 aa1f  r..wE.7E.....u..
+00001070: e7c0 6ce9 6d2a 85db efaa e396 394e f9b7  ..l.m*......9N..
+00001080: dee3 5f6f fcf0 2f3a 6214 6c99 2d39 5f28  .._o../:b.l.-9_(
+00001090: 90f3 8502 315e 9f15 882e 3a29 1015 7a51  ....1^....:)..zQ
+000010a0: 209d 5f07 e797 7569 6693 a98d a9f7 6b57   ._...uif.....kW
+000010b0: b7c5 5097 455b 827d 171a bba7 b676 5d3f  ..P.E[.}.....v]?
+000010c0: 544d d9d7 a8ed 15c6 9e2a ebde 9f2a 8836  TM.......*...*.6
+000010d0: bdc5 6aeb 0172 cb96 ded3 f657 0b35 94f7  ..j..r.....W.5..
+000010e0: 9b3d def7 c60f efa3 2346 c166 ef93 f607  .=......#F.f....
+000010f0: 0532 1052 2063 2005 32fc 4941 47ef 2b90  .2.R c .2.IAG.+.
+00001100: de6f 26ef 7715 67d9 f3d4 4678 bf76 4331  .o&.w.g...Fx.vC1
+00001110: 14b2 b220 eea1 71f0 7ed3 74bd ac3d 1d06  ... ..q.~.t..=..
+00001120: ee15 c6db de9f 2a48 ef67 4b6f b131 ba6e  ......*H.gKo.1.n
+00001130: 77d5 73cb 7054 de6f f778 df1b 3fbc 8f8e  w.s.pT.o.x..?...
+00001140: 1805 5bbc 8fe1 7d50 2086 f751 8118 30cf  ..[...}P ..Q..0.
+00001150: 29e8 38f6 1548 ef2b 90de 6fe7 b10f e43c  ).8..H.+..o....<
+00001160: b571 f1be 38b4 9181 df77 65cf 919f 372d  .q..8....we...7-
+00001170: 864e 26ff 92e1 2f8c b77d 3f55 8fbe 9f4a  .N&.../..}?U...J
+00001180: 518b 5b6c 0a7c af3a 75a9 8bf2 7db7 c7f7  Q.[l.|.:u...}...
+00001190: def8 e17b 4ced a360 b3ef 6bac 4007 0562  ...{L..`..k.@..b
+000011a0: 441c 1588 f63e a720 07de 2905 cdc8 5720  D....>. ..)...W 
+000011b0: 7ddf c591 ef7a a639 531b e1fb 52d6 fc46  }....z.9S...R..F
+000011c0: 2243 4691 2bc6 32ec fd52 8ee4 07c6 dbde  "CF.+.2..R......
+000011d0: 9f2a 48ef 4fa5 1876 b7d8 1878 5f75 eb4a  .*H.O..v...x_u.J
+000011e0: 96d0 eff1 be37 7e78 1f83 7b14 6cf1 3eea  .....7~x..{.l.>.
+000011f0: 7750 2078 7354 205e fb9c 8266 e42b 9023  wP xsT ^...f.+.#
+00001200: 5f81 f47e 3f79 7f18 f8ce f3d4 c6d9 fb8f  _..~?y..........
+00001210: 30ae 2b9d 2ce5 1cfb 2bc6 7d21 c1e4 00aa  0.+.,...+.}!....
+00001220: 5c33 c6eb abfe 5441 7a7f 2a45 07de 6263  \3....TAz.*E..bc
+00001230: e07d d5ad 4b5d d4d8 1ff6 78df 1b3f bc8f  .}..K]....x..?..
+00001240: b68d 822d dec7 047d 5020 3c71 4cc1 06b3  ...-...}P <qL...
+00001250: c673 0a9a b19f 8266 ec2b 90de 1f82 f75d  .s.....f.+.....]
+00001260: 510f a8ea 796a a3f6 7e39 0c45 5bc9 aa8f  Q...yj..~9.E[...
+00001270: 69eb b262 2c91 245d 9fb1 0cae 97dc b133  i..b,.$].......3
+00001280: e17e ac9d 76e7 db54 8ae1 719b 4a51 b1bb  .~..v..T..q.JQ..
+00001290: ead3 9574 ae14 f56b 8714 e6ad 1fce 47a7  ...t...k......G.
+000012a0: 8dfe 55b3 f71b 70f6 a051 8ca0 a346 316f  ..U...p..Q...F1o
+000012b0: 3c6b 14bc 3f29 d4a4 7c0a 75a4 80a0 3ee9  <k..?)..|.u...>.
+000012c0: 2bcb a621 0742 cf7c ffc1 a47d 32a5 dbe4  +..!.B.|...}2...
+000012d0: ec62 ac8b a7c6 7592 250c a239 9839 80d6  .b....u.%..9.9..
+000012e0: f312 50d6 9589 145f 1f95 0415 6231 3afa  ..P...._....b1:.
+000012f0: 168b 99fb e93e 5c08 a426 82d2 0b4b 7f5d  .....>\..&...K.]
+00001300: 187d 2867 be0b d1b3 a37f d5c2 068c 8483  .}(g............
+00001310: 46d1 f547 8596 548c 34ca 145f a3c6 df93  F..G..T.4.._....
+00001320: b695 49f2 43d3 8dbb dbde f592 e3b7 78cf  ..I.C.........x.
+00001330: 85d6 de81 4de1 2423 ac8b aee5 829f b30e  ....M.$#........
+00001340: ba51 5949 2881 f6bd 8a75 e024 dd3d 1533  .QYI(....u.$.=.3
+00001350: e28b d6c6 ddaa fb57 62be 7297 3818 ac67  .......Wb.r.8..g
+00001360: 35c7 68e0 a9a6 d432 eef3 cfce 6c68 19f8  5.h....2....lh..
+00001370: 6994 919f 46a9 f728 9483 f845 a176 f4c7  i...F..(...E.v..
+00001380: c15d 31ee 8f4d 3563 df35 fdd0 b45c fe8d  .]1..M5c.5...\..
+00001390: b593 b1df caf4 df08 730a 6a88 b45e c67e  ........s.j..^.~
+000013a0: d3b7 8e22 a258 7b32 3002 88c5 b0be c562  ...".X{20......b
+000013b0: a370 abde 5f11 7eca 5dca 5eb0 9ec9 406d  .p.._.~.].^...@m
+000013c0: cfa3 8bbb 29fe 6894 ea8f 46cd e04f df6c  ....).h...F..O.l
+000013d0: ddbd 29f0 c99b 5714 bed8 9a34 d86f caa6  ..)...W....4.o..
+000013e0: e8ea c6c9 828f cebf d03a 0c7e 8921 abae  .........:.~.!..
+000013f0: 1591 cf0c fe35 91af ccfa 7baa a3f1 77b6  .....5....{...w.
+00001400: f816 5b64 fcad ba7f 995d f55c bf4b e92b  ..[d.....].\.K.+
+00001410: 53a9 af44 f546 8f2e fec6 683a 28b4 c3d4  S..D.F....h:(...
+00001420: 70d4 2898 f4ac 51fc ee49 ffae 590a 3615  p.(...Q..I..Y.6.
+00001430: 3f79 d6b3 a1e3 ac70 8e4d 5564 709d 08fc  ?y.....p.MUdp...
+00001440: 4d57 1603 a3bf 35eb a2ad 7b6e 935c 69bc  MW....5...{n.\i.
+00001450: 8c7d 5114 9c59 08a6 1ac2 bb6f b1e2 66ec  .}Q..Y.....o..f.
+00001460: 6715 c2bb eec0 95f4 afdc a5fb 05eb 79ec  g.............y.
+00001470: 53f9 f3e8 cc85 8e29 a046 9903 6a94 49a0  S......).F..j.I.
+00001480: 460d 17d2 df6d 0d17 36f5 3f79 b3e7 820c  F....m..6.?y....
+00001490: 5fee 7542 a5eb 9aa7 6168 faba 1509 c815  _.uB....ah......
+000014a0: 5401 62c7 cccc e9da a7a2 6c3a e18d 1b5a  T.b.......l:...Z
+000014b0: f2ec 4aeb 850c 4321 51a0 aec9 6bac a221  ..J...C!Q...k..!
+000014c0: 435e 038c d6e8 a3bb eec1 956c b0dc 2503  C^.........l..%.
+000014d0: 06eb 990c 1402 3dba 9081 19a1 4699 122a  ......=.....F..*
+000014e0: b467 4ea8 9f35 6448 7fd7 9261 530e 9437  .gN..5dH...aS..7
+000014f0: 8765 a2e2 f6df 39b6 55e5 854d 98f8 5dc5  .e....9.U..M..].
+00001500: fced b2c7 f89a 339e 52c3 2c17 b2e2 df5b  ......3.R.,....[
+00001510: acb8 8910 b302 e25d 77ef 5a7a 98ca 829e  .......]w.Zz....
+00001520: 3ddb 2725 525d 9093 df58 a642 546f f243  =.'%R]...X.BTo.C
+00001530: 859a fc50 a126 3f4c 51ca 6d27 f5bb 960b  ...P.&?LQ.m'....
+00001540: 9bf2 a03c 1b16 09b3 6f7c f66f 9554 7819  ...<....o|.o.Tx.
+00001550: eb71 66e8 aa82 bcb9 d0b6 774f 4355 c9f2  .qf.......wOCU..
+00001560: d035 ceb0 ec6a ac1f fb42 6596 0b53 0dcd  .5...j...Be..S..
+00001570: bc90 5708 637b ccbc a0ba 7765 77a0 4c45  ..W.c{....wew.LE
+00001580: c2f7 b990 aa84 ccca 47ff ae79 5ee8 b943  ........G..y^..C
+00001590: a051 6e11 6894 7b04 0ab5 5c48 7fd7 7261  .Qn.h.{...\H..ra
+000015a0: 532c 9437 8744 77c0 5474 0e1d 9350 618e  S,.7.Dw.Tt...Pa.
+000015b0: 07db 4676 894d ea98 1100 c324 d2b6 4383  ..Fv.M.....$..C.
+000015c0: 05f1 9a7b f5c6 bc30 d5d0 7021 af17 c6f6  ...{...0..p!....
+000015d0: 182e 28d7 ac65 8ea9 64f8 3e17 52cd 90f9  ..(..e..d.>.R...
+000015e0: fc58 a63a 153b f7a0 5193 39aa 674d e698  .X.:.;..Q.9.gM..
+000015f0: a296 0b29 6ab9 b029 1d4a ad42 8e5e b798  ...)j..).J.B.^..
+00001600: 8bce bebe d979 4196 888e b9fe c558 fb88  .....yA......X..
+00001610: a16b eaba ef6b d968 e0a9 a955 0131 3b33  .k...k.h...U.1;3
+00001620: 4c75 346c c84b 88b1 4586 0daa 8357 c247  Lu4l.K..E....W.G
+00001630: 7f84 6e96 8dde 6543 b09e 2306 aa88 1e9d  ..n...eC..#.....
+00001640: 6786 81e1 a346 193e 6a94 e1a3 420d 1b14  g....F.>j...B...
+00001650: 6ad8 a050 a323 081a d8e0 b8c9 7b8e 6d45  j..P.#......{.mE
+00001660: 6259 16a5 e489 2df5 e14b deba 189c 0809  bY....-..K......
+00001670: f207 6ca0 f576 fc18 eb48 36c4 62cc b1b7  ..l..v...H6.b...
+00001680: 584c 36e8 0e5e 891f 5d2a 22be cf86 5444  XL6..^..]*"...TD
+00001690: e446 e9e8 dfb5 b081 f1a3 4619 3f2a b42c  .F........F.?*.,
+000016a0: 1840 2ad8 d221 fd61 4b87 14b5 7488 029e  .@*..!.aK...t...
+000016b0: 1c23 433a 11ba 2617 3494 5d3d 30ab be18  .#C:..&.4.]=0...
+000016c0: eb90 4ef4 65d7 d792 8ea2 b957 5abf 4387  ..N.e......WZ.C.
+000016d0: ac9a f826 2ff1 4c46 47df 62b1 a143 da0d  ...&/.LFG.b..C..
+000016e0: 42ea b9b5 fa04 62aa 32be cf87 e98c dd54  B.....b.2......T
+000016f0: 0f1e c718 9d3a 1158 3088 04cc 2812 30c3  .....:.X0...(.0.
+00001700: 4805 5b46 2811 8df9 a57a d632 629a 00ca  H.[F(....z.2b...
+00001710: 6660 ac73 f60f a6eb c512 3c14 45da a5e1  f`.s......<.E...
+00001720: 2cf2 6597 f535 671d a207 99a8 8cec 2cc6  ,.e..5g.......,.
+00001730: def5 6682 988a c1b6 5bb4 368c d0fe 5989  ..f.....[.6...Y.
+00001740: 245d 2a35 becf 8849 408b 8ca0 d4e8 df35  $]*5...I@......5
+00001750: cf10 7224 4b8f b803 60c6 9280 194c 2ad8  ..r$K...`....L*.
+00001760: 3242 c96c 8611 eab4 1d37 22e4 cda1 b7eb  2B.l.....7".....
+00001770: aee7 c653 e89d cc24 212b 465f 327a bad0  ...S...$!+F_2z..
+00001780: dae7 165d dfb8 b26d e45c 2abc 7935 d68f  ...]...m.\*.y5..
+00001790: dcc2 f58d 9c7e 82e6 f0a8 2476 2262 7189  .....~....$v"bq.
+000017a0: 19f5 16cb 0d27 b487 5622 4a97 ca91 ef73  .....'..V"J....s
+000017b0: 429d 3cc4 2f8e fe5d 0b27 58cf 0360 c694  B.<./..].'X..`..
+000017c0: 8019 542a d872 4229 a186 139b 8aa4 bc39  ..T*.rB).......9
+000017d0: 68fd e20a d4e9 1c7a 47a7 1855 37c8 7135  h......zG..U7.q5
+000017e0: d9c9 2a6a ea50 b4ee baa7 a128 0a11 b3fd  ..*j.P.....(....
+000017f0: 7914 b370 ac9d 43cc 7322 2f4a c6ba 9754  y..p..C.s"/J...T
+00001800: 251f 6dc2 a904 f4f1 5a5c 99ca 92ef 7362  %.m.....Z\....sb
+00001810: d2ea e23c 4159 d2a5 0260 c995 f900 d844  ...<AY...`.....D
+00001820: 96fa 6913 5a2a cd93 6294 7ab7 8d25 3695  ..i.Z*..b.z..%6.
+00001830: 4979 3670 8299 e1d9 bf34 bb6e e436 212e  Iy6p.....4.n.6!.
+00001840: bbac af39 ebb0 6e54 456d b7a8 6215 cdc2  ...9..nTEm..b...
+00001850: 11cf 21a2 376e 8f16 9111 ba87 d762 cb54  ..!.7n.......b.T
+00001860: 9b7c 9f11 e919 4547 6dd2 a52a 6059 9ae0  .|....EGm..*`Y..
+00001870: 52c3 26ba 5430 0395 67f5 723b 4b6c ca93  R.&.T0..g.r;Kl..
+00001880: ea59 1b4b c433 7e3c 5470 f68f e532 cfb6  .Y.K.3~<Tp...2..
+00001890: 9748 8207 9c2e c63a 0697 7d27 cb4c 63d6  .H.....:..}'.Lc.
+000018a0: 8db5 138b 5529 cb92 5937 f2fa a4fc 6448  ....U)..Y7....dH
+000018b0: 9328 50c6 72b3 6ee8 1e5e 8b2e 7729 942e  .(P.r.n..^..w)..
+000018c0: 5528 1d8f 2e7a 7459 3778 98e8 00d8 4497  U(...ztY7x....D.
+000018d0: fa69 135d a630 f790 4fea dd66 5f53 a196  .i.].0..O..f_S..
+000018e0: 1193 d6d7 8a3e c87c 0322 e574 1546 160e  .....>.|.".t.F..
+000018f0: e183 a393 2fb1 73b4 bcbd 7aa8 2167 ddc9  ..../.s...z.!g..
+00001900: 9e69 51b9 b2e1 92f4 2ad6 b97d ec58 6c18  .iQ.....*..}.Xl.
+00001910: 9115 35ef 70c0 5a74 b94b a774 a94e c94b  ..5.p.Zt.K.t.N.K
+00001920: 5da3 4713 4698 e852 c326 bad4 b089 2e95  ].G.F..R.&......
+00001930: 1889 3e38 a99f b68c d894 2ae5 d9b0 9fd5  ..>8......*.....
+00001940: a1c2 e7d8 5a7b a8a9 a81a 39da ace9 73a1  ....Z{....9...s.
+00001950: f5f6 2997 9cf5 0621 f247 1b63 cd79 b235  ..)....!.G.c.y.5
+00001960: 16a3 8fee 70cf 5a68 b94b ac74 a958 c93d  ....p.Zh.K.t.X.=
+00001970: d9d1 a30b 2192 6b14 213f 3b00 36a1 a57e  ....!.k.!?;.6..~
+00001980: da84 964a 9134 8450 e7f9 40a6 17f5 cb76  ...J.4.P..@....v
+00001990: 8a98 44bf 81d1 c739 b6d6 9e74 191a 39ba  ..D....9...t..9.
+000019a0: 862a 5c8c 75f1 344c 7244 ee94 3bad 6745  .*\.u.4LrD..;.gE
+000019b0: a292 2b31 151a f02a d6d9 1962 2ae6 61d7  ..+1...*...b*.a.
+000019c0: 686d 08a1 3b78 25ae ac76 e995 c17a bee5  hm..;x%..v...z..
+000019d0: 44bd d2a3 0921 2858 0266 5c09 18c3 f5a4  D....!(X.f\.....
+000019e0: 6033 07e8 8799 610a 1ab6 31ed fdc8 d820  `3....a...1.... 
+000019f0: f8dc 1f75 eb5b 9128 3009 d05a bc38 a51e  ...u.[.(0..Z.8..
+00001a00: ad58 73d7 f39a b1ae 6597 4b24 ed7e 680b  .Xs.....e.K$.~h.
+00001a10: f4ce 6bac 23c6 c15b 2c46 6fdc 6231 7d8e  ..k.#..[,Fo.b1}.
+00001a20: 3e5c 891c ab5d aa64 b09e 7d8e 2e19 3d9a  >\...].d..}...=.
+00001a30: f89c 9123 6046 8e1a e615 8967 c098 424e  ...#`F.....g..BN
+00001a40: 7839 08f5 a260 330d 083a 6d67 e2b1 736c  x9...`3..:mg..sl
+00001a50: 2fa7 0139 bae0 e420 14fc 7381 b5eb aaa7  /..9... ..s.....
+00001a60: 2a5c 7193 5b6e f207 3a35 dfbd 3d0d c42a  *\q.[n..:5..=..*
+00001a70: 329b 88c5 4c2f 6331 9872 471f 2ef5 d757  2...L/c1.rG....W
+00001a80: 5977 0993 552a 4c72 e21f 3dba 50a2 46f5  Yw..U*Lr..=.P.F.
+00001a90: 0f80 310e 8e80 e19d 67c0 8612 eab7 2b43  ..1.....g.....+C
+00001aa0: 0975 dbd7 4c13 f180 a144 fd08 1e63 832d  .u..L....D...c.-
+00001ab0: 2764 e3a2 654a 7381 f57b 9cc8 a89e 5386  'd..eJs..{....S.
+00001ac0: 995b 1ae4 dd39 6932 1633 c18c c586 13da  .[...9i2.3......
+00001ad0: 430b ac39 b14b 9aac 5269 9217 0346 8f26  C..9.K..Ri...F.&
+00001ae0: 9ce0 1968 c0e8 fe23 60f8 ed19 b0e1 84fa  ...h...#`.......
+00001af0: 6dcb 894d 7152 de1d 960e 5e72 3bc7 f666  m..MqR....^r;..f
+00001b00: 2821 27dd 6b33 4de8 938f ef51 62ed 9c64  (!'.k3M....Qb..d
+00001b10: 365a 8855 34d3 4494 5535 956f d1da 5042  6Z.U4.D.U5.o..PB
+00001b20: 7552 72ed 4453 6297 3259 a5ca 2415 d5d1  uRr.DSb.2Y..$...
+00001b30: a30b 251a 78ed 0018 1d7a 048c c63f 6bb8  ..%.x....z...?k.
+00001b40: 3694 50bf 6d29 b1a9 4dca bb43 7426 8394  6.P.m)..M..Ct&..
+00001b50: d304 e4c3 9863 768d e8cf 4df2 558a 6903  .....cv...M.U.i.
+00001b60: 2376 cf83 41ef 7162 4d9a 94bb f4cc de5f  #v..A.qbM......_
+00001b70: 6315 0d25 a69a 33a3 88d6 8612 da41 2b67  c..%..3......A+g
+00001b80: a5ab 5dc2 64b0 9e2f 4aa3 7ea3 4713 4af0  ..].d../J.~.G.J.
+00001b90: b034 60d4 f708 1873 ccb3 828d e8a0 501b  .4`....s......P.
+00001ba0: 5e6e 0a93 f26c 2044 d5f2 38ff 39b6 d7ce  ^n...l D..8.9...
+00001bb0: 12b5 5c76 3087 a368 bd9d 64e6 ac3b a159  ..\v0..h..d..;.Y
+00001bc0: 5bcb 073e 40cd d747 1db1 7f11 8bb9 e71d  [..>@..G........
+00001bd0: 8b4d 78a9 fdb3 4cd3 7a92 d825 4c56 a930  .Mx...L.z..%LV.0
+00001be0: c91b 6da3 4713 4660 e63f 6898 572d 8e80  ..m.G.F`.?h.W-..
+00001bf0: d127 cf0a b68c 487f da32 62f3 dca4 bc39  .'....H..2b....9
+00001c00: 3042 761a 4c28 61e5 439f 4394 4327 47ec  0Bv.L(a.C.C.C'G.
+00001c10: b967 7089 bdb3 1cad eb9e fa61 90ad d3be  .gp........a....
+00001c20: ade4 6b0a 0c2f 57a5 c9ce f30d 5b5a 8f4a  ..k../W.....[Z.J
+00001c30: 9212 53dd b9ef 1dad 0d25 9483 12f9 5353  ..S......%....SS
+00001c40: 6297 3259 a5ca 2427 e7d1 a30b 25e8 b603  b.2Y..$'....%...
+00001c50: 6013 5eea a731 c59c d4d3 d6e9 ea61 133e  `.^..1.......a.>
+00001c60: c673 8699 2c33 ab3d 4a96 2991 82fd 6a0a  .s..,3.=J.)...j.
+00001c70: 8cc3 7ddb 5e2e c3c9 190a fbe9 84d8 574a  ..}.^.........WJ
+00001c80: a8f4 f7a9 e4b6 7d63 8fd1 8b75 4e58 88c5  ......}c...uNX..
+00001c90: dcd8 8ec5 c6e5 ba0b d7a2 c75d d263 954a  ...........].c.J
+00001ca0: 8f15 66f6 d1a3 89cb 4df4 a861 133d 6ad8  ..f.....M..a.=j.
+00001cb0: 448f 0ab6 a182 7e1a 7c7a 5155 b349 663c  D.....~.|zQU.If<
+00001cc0: 85c8 938f e7d8 de4c 92d9 57f2 d51b ea0e  .......L..W.....
+00001cd0: ea9c a4dc d1f5 372a c5bd 723c 4eae 55a1  ......7*..r<N.U.
+00001ce0: 4a57 be7b 4932 fb86 a2d7 ab18 67f3 89ec  JW.{I2......g...
+00001cf0: 0dea 5bb4 4617 deb5 7f92 6b2d 7a12 d8a5  ..[.F.....k-z...
+00001d00: 3d56 a9f6 c82b 00a3 4717 4670 8ff8 00d8  =V...+..G.Fp....
+00001d10: 048f fa69 aa8b fa69 f6ef 8b86 cd2c 3089  ...i...i.....,0.
+00001d20: 74b9 6f27 658e 2cb6 bddc 8875 75d9 9ac3  t.o'e.,....uu...
+00001d30: 0cb1 fd6a 60cb a59b 5a6e 61c9 5969 54f9  ...j`...Zna.YiT.
+00001d40: 9ab3 9ea6 0139 75cb 8336 af62 9d75 7a56  .....9u..6.b.uzV
+00001d50: 76bc 456b e374 dd89 2be1 61bd 4b5f 0cd6  v.Ek.t..+.a.K_..
+00001d60: 7378 487d d1a3 89d3 191e 0266 7808 98e1  sxH}.......fx...
+00001d70: 2160 fcf6 0930 18f5 a260 330d 081a 76fb  !`...0...`3...v.
+00001d80: 7a39 118f 9421 b658 b959 361d fdd1 f9a1  z9...!.X.Y6.....
+00001d90: 3702 64de ba6f 8440 f20f 3c74 cd5a 0f72  7.d..o.@..<t.Z.r
+00001da0: c35e 969d ba46 ffbc c64a 6236 797b d41d  .^...F...Jb6y{..
+00001db0: 6964 2ce6 4625 ba69 6517 a2de 2540 06eb  id,.F%.ie...%@..
+00001dc0: 9914 1420 3dba 9082 7763 0e80 b90b 0198  ... =...wc......
+00001dd0: bb10 0a36 11a2 424d b0a0 504b 8949 7e34  ...6..BM..PK.I~4
+00001de0: 57ed 6363 9785 412e d08a bfe4 e27c 297f  W.cc..A......|).
+00001df0: 5390 ce58 b7ae 6feb a6af 2ad1 0a10 1ed2  S..X..o...*.....
+00001e00: 7a5e 181a 793b 179d 57b1 cec5 0ab1 d89c  z^..y;..W.......
+00001e10: 788a e50c 16d0 c12b bb10 f52e f931 58cf  x......+.....1X.
+00001e20: df5b e2ed 6b8f 2684 e02e 0460 ee42 00e6  .[..k.&....`.B..
+00001e30: e916 055b 42a4 3f6d 09b1 293e ca9b 4377  ...[B.?m..)>..Cw
+00001e40: 5353 888d 5584 7072 2aaa 944b b672 2717  SS..U.pr*..K.r'.
+00001e50: 9102 adb7 33c8 9cf5 fa36 e5a3 86c8 1762  ....3....6.....b
+00001e60: b139 ee14 cb0d 21b4 7b56 b628 ea5d da63  .9....!.{V.(.].c
+00001e70: b09e 0981 1e1c 3d9a 1082 5b14 80b9 45a1  ......=...[...E.
+00001e80: 61b3 6aa8 77f3 d0c1 493f 0c32 bd68 9481  a.j.w...I?.2.h..
+00001e90: 84a0 2b9b 56b1 b90c 1e65 9d97 2307 f63b  ..+.V....e..#..;
+00001ea0: 7c19 3151 ce47 f4f2 ddb6 4a3e b6c2 3922  |.1Q.G....J>..9"
+00001eb0: 273d ae6e 5ac5 3aa2 c7df 1e55 e79a 91ff  '=.nZ.:....U....
+00001ec0: 1423 ba61 e570 4bbd 4b7a 0cd6 3323 304a  .#.a.pK.Kz..3#0J
+00001ed0: 468f 2e8c 6006 7600 0c06 1f01 f370 0b60  F...`.v......p.`
+00001ee0: 6698 1a66 62f0 a260 bb6a 643f 6778 8ead  f..fb..`.jd?gx..
+00001ef0: 3584 9035 a32b 8dee 48eb 9060 7a42 c8d5  5..5.+..H..`zB..
+00001f00: 5c7b 673f 67bd be8b 29d6 d945 63e5 e38c  \{g?g...)..Ec...
+00001f10: 593d f28e 1e5c 4930 eb5d c263 b09e 0941  Y=...\I0.].c...A
+00001f20: e1d1 a309 2198 6002 6682 0998 0926 6043  ....!.`.f....&`C
+00001f30: 08f5 db96 109b d2a3 bc3b ec62 9ab0 1247  .........;.b...G
+00001f40: 221f a79d e413 3c22 0581 b297 d839 3a08  ".....<".....9:.
+00001f50: 0d8c 9034 c64e 1199 e396 1b8c c87f af31  ...4.N.........1
+00001f60: 569c 1b56 b118 15bc ab2e 74c9 fd15 fdbd  V..V......t.....
+00001f70: d65d c263 9d0a 8f35 7e71 f4e8 cc08 4739  .].c...5~q....G9
+00001f80: f500 9809 2660 2698 0a2e adcb 37b5 4579  ....&`&.....7.Ey
+00001f90: 7872 b989 1432 eadf 34d1 cb3d 199e 8b8e  xr...2..4..=....
+00001fa0: adb7 2ecf af0a 3961 717d 55c8 7fa6 3156  ......9aq}U...1V
+00001fb0: 1c9d 718b c5c6 e5da 016b e9e5 2e61 b14e  ..q......k...a.N
+00001fc0: 85c5 9a47 1e3d 9ab8 dca4 971a 36e9 a586  ...G.=......6...
+00001fd0: 4da0 a0a5 4333 0928 d832 42bd dc44 0a93  M...C3.(.2B..D..
+00001fe0: aac7 2db4 736c ae8d 13e4 2a6e d199 5c22  ..-.sl....*n..\"
+00001ff0: a73b ae4f 0219 eb8d 4920 af3b 4a05 4388  .;.O....I .;J.C.
+00002000: c338 215b 7c87 7f56 761f ea5d ba63 b09e  .8![|..Vv..].c..
+00002010: 9705 ea8e 1e4d 18c1 dd07 0d33 233a 02e6  .....M.....3#:..
+00002020: ee83 82cb c130 42e9 8e96 119b 871e e5dd  .....0B.........
+00002030: be63 5bb3 fb10 db6b 2921 e160 db61 685e  .c[....k)!.`.ah^
+00002040: 683d 470a 7232 413e fdca d051 a994 4df5  h=G.r2A>...Q..M.
+00002050: 482f dba2 68e5 33de d87d 8855 e479 a758  H/..h.3..}.U.y.X
+00002060: cc33 6eb1 d84c 12aa 1792 5b83 7a5d d825  .3n..L....[.z].%
+00002070: 3cd6 a9f0 c8c3 bba3 4717 4a30 d83e 00e6  <.......G.J0.>..
+00002080: ee03 601e 6e51 7086 124a 71b3 9450 5533  ..`.nQp..Jq..PU3
+00002090: 9344 14f7 50a5 736c 6e26 9918 e473 4f20  .D..P.sln&...sO 
+000020a0: ed85 d64b ec28 8234 f990 d13b 37a6 88fc  ...K.(.4...;7...
+000020b0: 9947 f9c1 c064 4e11 5165 d5c5 77f4 ef4a  .G...dN.Qe..w..J
+000020c0: e4d8 ecd2 2483 f53c 4550 93f4 68c2 0746  ....$..<EP..h..F
+000020d0: 8e80 1939 0266 e4a8 615e ac38 29d8 7ced  ...9.f..a^.8).|.
+000020e0: 513f 4c3a 08ea fbb5 e7dd d973 6cae e183  Q?L:.......sl...
+000020f0: bfa5 2dd1 20f4 065a 07bd 413e 0824 7b55  ..-. ..Z..A>.${U
+00002100: f275 3826 9739 6b61 443d 88aa dd32 4f79  .u8&.9kaD=...2Oy
+00002110: 8d55 6472 198b 3943 c462 7efc 0f5d b892  .Udr..9C.b~..]..
+00002120: 5c36 bb04 c960 3d33 8282 a447 1746 989b  \6...`=3...G.F..
+00002130: 1380 995c 0266 72a9 605e 843a 29d4 1262  ...\.fr.`^.:)..b
+00002140: f3a6 b63c 1b34 ea41 3ebd 018d 3ab6 9794  ...<.4.A>...:...
+00002150: 906f b689 e6cc 1982 c6db 0a54 ce7a 5d81  .o.........T.z].
+00002160: 7ad4 110a 542c c6ea 7d8b c586 11da 3f4b  z...T,..}.....?K
+00002170: 63a7 35e3 dbe5 7f91 f47f 0000 00ff ff00  c.5.............
+00002180: 0000 ffff b229 484c 4ff5 4d2c 4acf cc2b  .....)HLO.M,J..+
+00002190: 56c8 494d 2bb1 5532 d033 3755 5228 ca4c  V.IM+.U2.37UR(.L
+000021a0: cf80 734a f20b 6c95 0c95 1492 f24b 4af2  ..sJ..l......KJ.
+000021b0: 73c1 cc8c d4c4 94d4 2290 6aa0 e2b4 fcfc  s.......".j.....
+000021c0: 1218 47df ce46 bf3c bf28 bb38 2335 b5c4  ..G..F.<.(.8#5..
+000021d0: 0e00 0000 ffff 0300 504b 0304 1400 0600  ........PK......
+000021e0: 0800 0000 2100 e9a6 25b8 6606 0000 531b  ....!...%.f...S.
+000021f0: 0000 1300 0000 786c 2f74 6865 6d65 2f74  ......xl/theme/t
+00002200: 6865 6d65 312e 786d 6cec 59cd 6e1b 3710  heme1.xml.Y.n.7.
+00002210: be17 e83b 107b 4f2c d992 6219 9103 4b96  ...;.{O,..b...K.
+00002220: e236 7162 d84a 8a1c a95d 6a97 1177 b920  .6qb.J...]j..w. 
+00002230: 293b ba15 c9b1 4081 a269 d14b 81de 7a28  );....@..i.K..z(
+00002240: da06 4880 5ed2 a771 9ba2 4d81 bc42 87e4  ..H.^..q..M..B..
+00002250: 4a5a 5a54 6c27 06fa 171d 6c2d f7e3 fccf  JZZTl'....l-....
+00002260: 7086 ba7a ed41 cad0 2111 92f2 ac15 542f  p..z.A..!.....T/
+00002270: 5702 44b2 9047 348b 5bc1 9d7e efd2 7a80  W.D..G4.[..~..z.
+00002280: a4c2 5984 19cf 482b 9810 195c db7c ffbd  ..Y...H+...\.|..
+00002290: ab78 4325 2425 08f6 6772 03b7 8244 a97c  .xC%$%..gr...D.|
+000022a0: 6365 4586 b08c e565 9e93 0cde 0db9 48b1  ceE....e......H.
+000022b0: 8247 11af 4402 1f01 dd94 adac 562a 8d95  .G..D.......V*..
+000022c0: 14d3 2c40 194e 81ec ede1 9086 04f5 35c9  ..,@.N........5.
+000022d0: 6073 4abc cbe0 3153 522f 844c 1c68 d2c4  `sJ...1SR/.L.h..
+000022e0: d961 b0d1 a8aa 1172 223b 4ca0 43cc 5a01  .a.....r";L.C.Z.
+000022f0: f089 f851 9f3c 5001 6258 2a78 d10a 2ae6  ...Q.<P.bX*x..*.
+00002300: 13ac 6c5e 5dc1 1bc5 26a6 96ec 2ded eb99  ..l^]...&...-...
+00002310: 4fb1 afd8 108d 560d 4f11 0f66 4cab bd5a  O.....V.O..fL..Z
+00002320: f3ca f68c be01 30b5 88eb 76bb 9d6e 7546  ......0...v..nuF
+00002330: cf00 7018 82a6 5696 32cd 5a6f bdda 9ed2  ..p...V.2.Zo....
+00002340: 2c81 ecd7 45da 9d4a bd52 73f1 25fa 6b0b  ,...E..J.Rs.%.k.
+00002350: 3237 dbed 76bd 59c8 6289 1a90 fd5a 5bc0  27..v.Y.b....Z[.
+00002360: af57 1ab5 ad55 076f 4016 5f5f c0d7 da5b  .W...U.o@.__...[
+00002370: 9d4e c3c1 1b90 c537 16f0 bd2b cd46 cdc5  .N.....7...+.F..
+00002380: 1b50 c268 365a 406b 87f6 7a05 f519 64c8  .P.h6Z@k..z...d.
+00002390: d98e 17be 0ef0 f54a 019f a320 1a66 d1a5  .......J... .f..
+000023a0: 590c 79a6 96c5 5a8a ef73 d103 8006 32ac  Y.y...Z..s....2.
+000023b0: 6886 d424 2743 1c42 1477 703a 1014 6b06  h..$'C.B.wp:..k.
+000023c0: 7883 e0d2 1bbb 14ca 8525 cd0b c950 d05c  x........%...P.\
+000023d0: b582 0f73 0c19 31a7 f7ea f9f7 af9e 3f45  ...s..1.......?E
+000023e0: af9e 3f39 7ef8 ecf8 e14f c78f 1e1d 3ffc  ..?9~....O....?.
+000023f0: d1d2 7236 eee0 2c2e 6f7c f9ed 677f 7efd  ..r6..,.o|..g.~.
+00002400: 31fa e3e9 372f 1f7f e1c7 cb32 fed7 1f3e  1...7/.....2...>
+00002410: f9e5 e7cf fd40 c8a0 b944 2fbe 7cf2 dbb3  .....@...D/.|...
+00002420: 272f befa f4f7 ef1e 7be0 5b02 0fca f03e  '/......{.[....>
+00002430: 4d89 44b7 c811 dae7 29e8 660c e34a 4e06  M.D.....).f..JN.
+00002440: e27c 3bfa 09a6 ce0e 9c00 6d0f e9ae 4a1c  .|;.......m...J.
+00002450: e0ad 0966 3e5c 9bb8 c6bb 2ba0 78f8 80d7  ...f>\....+.x...
+00002460: c7f7 1d59 0f12 3156 d4c3 f946 923a c05d  ...Y..1V...F.:.]
+00002470: ce59 9b0b af01 6e68 5e25 0bf7 c759 ec67  .Y....nh^%...Y.g
+00002480: 2ec6 65dc 3ec6 873e de1d 9c39 aeed 8e73  ..e.>..>...9...s
+00002490: a89a d3a0 746c df49 8823 e61e c399 c231  ....tl.I.#.....1
+000024a0: c988 42fa 1d1f 11e2 d1ee 1ea5 8e5d 7769  ..B..........]wi
+000024b0: 28b8 e443 85ee 51d4 c6d4 6b92 3e1d 3881  (..C..Q...k.>.8.
+000024c0: 34df b443 53f0 cbc4 a733 b8da b1cd ee5d  4..CS....3.....]
+000024d0: d4e6 cca7 f536 3974 9190 1098 7984 ef13  .....69t....y...
+000024e0: e698 f13a 1e2b 9cfa 48f6 71ca ca06 bf89  ...:.+..H.q.....
+000024f0: 55e2 13f2 6022 c232 ae2b 1578 3a26 8ca3  U...`".2.+.x:&..
+00002500: 6e44 a4f4 edb9 2d40 df92 d36f 60a8 575e  nD....-@...o`.W^
+00002510: b7ef b249 ea22 85a2 231f cd9b 98f3 3272  ...I."..#.....2r
+00002520: 9b8f 3a09 4e73 afcc 344b cad8 0fe4 0842  ..:.Ns..4K.....B
+00002530: 14a3 3dae 7cf0 5dee 6688 7e06 3fe0 6ca9  ..=.|.].f.~.?.l.
+00002540: bbef 52e2 b8fb f442 7087 c68e 48f3 00d1  ..R....Bp...H...
+00002550: 6fc6 a2a8 da4e fd4d 69f6 ba62 cc28 54e3  o....N.Mi..b.(T.
+00002560: 77c5 787a 3a6d c1d1 e44b 899d 1325 7819  w.xz:m...K...%x.
+00002570: ee5f 5878 b7f1 38db 2310 eb8b 07cf bbba  ._Xx..8.#.......
+00002580: fbae ee06 fff9 babb 2c97 cf5a 6de7 0516  ........,..Zm...
+00002590: 9ae4 795f 6cba e474 6993 3ca4 8c1d a809  ..y_l..ti.<.....
+000025a0: 2337 a5e9 9325 1c16 510f 164d 036f a6b8  #7...%..Q..M.o..
+000025b0: d9d0 9427 f0b5 28ee 0e2e 16d8 ec41 82ab  ...'..(......A..
+000025c0: 8fa8 4a0e 129c 438f 5d35 235f 2c0b d2b1  ..J...C.]5#_,...
+000025d0: 4439 9730 db99 6533 7c92 13b4 cd38 49a1  D9.0..e3|....8I.
+000025e0: cd36 9361 5dcf 0cb6 1e48 ac76 7964 97d7  .6.a]....H.vyd..
+000025f0: cab3 e18c 8c99 1463 337f 4e19 ad69 0267  .......c3.N..i.g
+00002600: 65b6 76e5 ed98 55ad 544b cde6 aa56 35a2  e.v...U.TK...V5.
+00002610: 9952 e7a8 3653 197c b8a8 1a2c ceac 095d  .R..6S.|...,...]
+00002620: 0882 de05 acdc 8011 5dcb 0eb3 0966 24d2  ........]....f$.
+00002630: 76b7 73f3 d42d 9af5 85ba 4826 3822 858f  v.s..-....H&8"..
+00002640: b4de 8b3e aa1a 274d 6365 1a46 1e1f e939  ...>..'Mce.F...9
+00002650: ef14 1f95 b835 35d9 b7e0 7616 2795 d9d5  .....55...v.'...
+00002660: 96b0 9b7a ef6d bc34 1d6e e75e d279 7b22  ...z.m.4.n.^.y{"
+00002670: 1d59 564e 4e96 a1a3 56d0 acaf d603 14e2  .YVNN...V.......
+00002680: bc15 0c61 ac85 af69 0e5e 97ba f1c3 2c86  ...a...i.^....,.
+00002690: bba1 5009 1bf6 a726 b309 d7b9 379b feb0  ..P....&....7...
+000026a0: acc2 4d85 b5fb 82c2 4e1d c885 54db 5826  ..M.....N...T.X&
+000026b0: 3634 ccab 2204 5866 8670 23ff 6a1d cc7a  64..".Xf.p#.j..z
+000026c0: 510a d848 7f03 29d6 d621 18fe 3629 c08e  Q..H..)..!..6)..
+000026d0: ae6b c970 4842 5576 7669 c5dc 5118 4051  .k.pHBUvvi..Q.@Q
+000026e0: 4af9 5811 7190 4447 68c0 c662 1f83 fb75  J.X.q.DGh..b...u
+000026f0: a882 3e11 9570 3b61 2a82 7e80 ab34 6d6d  ..>..p;a*.~..4mm
+00002700: f3ca 2dce 45d2 952f b00c ceae 6396 27b8  ..-.E../....c.'.
+00002710: 28b7 3a45 a799 6ce1 268f 6732 9827 2bad  (.:E..l.&.g2.'+.
+00002720: 110f 74f3 ca6e 943b bf2a 26e5 2f48 9572  ..t..n.;.*&./H.r
+00002730: 18ff cf54 d1e7 095c 17ac 45da 0321 dce4  ...T...\..E..!..
+00002740: 0a8c 74be b602 2e54 c2a1 0ae5 090d 7b02  ..t....T......{.
+00002750: 2eb9 4ced 8068 81eb 5878 0d41 05f7 c9e6  ..L..h..Xx.A....
+00002760: bf20 87fa bfcd 394b c3a4 354c 7d6a 9fc6  . ....9K..5L}j..
+00002770: 4850 388f 5422 08d9 83b2 64a2 ef14 62d5  HP8.T"....d...b.
+00002780: e2ec b224 5941 c844 5449 5c99 5bb1 07e4  ...$YA.DTI\.[...
+00002790: 90b0 beae 810d 7db6 0728 8150 37d5 a428  ......}..(.P7..(
+000027a0: 0306 7732 fedc e722 8306 b16e 72fe a99d  ..w2..."...nr...
+000027b0: 8f4d e6f3 b607 ba3b b02d 96dd 7fc6 5ea4  .M.....;.-....^.
+000027c0: 562a faa5 a3a0 e93d fb4c 4f35 2b07 af39  V*.....=.LO5+..9
+000027d0: d8cf 79d4 da8a b5a0 f16a fdcc 476d 0e97  ..y......j..Gm..
+000027e0: 3e48 ff81 f38f 8a90 d91f 27f4 81da e7fb  >H........'.....
+000027f0: 505b 11fc d660 db2b 0451 7dc9 361e 4817  P[...`.+.Q}.6.H.
+00002800: 485b 1e07 d038 d945 1b4c 9a94 6d58 8aee  H[...8.E.L..mX..
+00002810: f6c2 db28 b891 2e3a dd19 5fc8 d237 e974  ...(...:.._..7.t
+00002820: cf69 ec59 73e6 b273 72f1 f5dd e7f9 8c5d  .i.Ys..sr......]
+00002830: 58d8 b175 b9d3 f598 1a92 f664 8aea f668  X..u.......d...h
+00002840: 3ac8 18c7 985f b5ca 3f3c f1c1 7d70 f436  :...._..?<..}p.6
+00002850: 5cf1 8f99 92f6 6aff 015c f1c1 9461 7f24  \.....j..\...a.$
+00002860: 80e4 b7ce 355b 37ff 0200 00ff ff03 0050  ....5[7........P
+00002870: 4b03 0414 0006 0008 0000 0021 0000 d49f  K..........!....
+00002880: c473 0300 00c8 0900 000d 0000 0078 6c2f  .s...........xl/
+00002890: 7374 796c 6573 2e78 6d6c c456 5b8f a336  styles.xml.V[..6
+000028a0: 147e afd4 ff60 f99d e132 9026 11b0 da4c  .~...`...2.&...L
+000028b0: 0669 a5ed aad2 4ca5 3ecc 8b03 26b1 d617  .i....L.>...&...
+000028c0: 649c 29d9 aaff bdc7 3624 cc5e 9aee 546a  d.).....6$.^..Tj
+000028d0: 7900 fbf8 f83b b7ef d8e4 6f06 c1d1 33d5  y....;....o...3.
+000028e0: 3d53 b2c0 f14d 8411 95b5 6a98 dc17 f8d7  =S...M....j.....
+000028f0: c72a 5862 d41b 221b c295 a405 3ed1 1ebf  .*Xb..".....>...
+00002900: 297f fc21 efcd 89d3 8703 a506 0184 ec0b  )..!............
+00002910: 7c30 a65b 8761 5f1f a820 fd8d eaa8 8495  |0.[.a_.. ......
+00002920: 5669 410c 4cf5 3eec 3b4d 49d3 db4d 8287  ViA.L.>.;MI..M..
+00002930: 4914 2d42 4198 c41e 612d ea7f 0222 88fe  I.-BA...a-..."..
+00002940: 78ec 825a 898e 18b6 639c 9993 c3c2 48d4  x..Z....c.....H.
+00002950: eb77 7ba9 34d9 7170 7588 5352 a321 5ee8  .w{.4.qpu.SR.!^.
+00002960: 040d 7a32 e2a4 5fd8 11ac d6aa 57ad b901  ..z2.._.....W...
+00002970: dc50 b52d abe9 97ee aec2 5548 ea0b 1220  .P.-......UH... 
+00002980: bf0e 29ce c228 7911 fba0 5f89 9486 9a3e  ..)..(y..._....>
+00002990: 335b 3e5c e6f2 282a 617a 54ab a334 50ce  3[>\..(*azT..4P.
+000029a0: b308 f995 770d 0817 2946 be2a 77aa b125  ....w...)F.*w..%
+000029b0: 85e7 2910 e229 689a 2774 38ac 8558 f73d  ..)..)h.'t8..X.=
+000029c0: 0ecb 3c1c f1ca bc55 f202 9b40 066c 6ed7  ..<....U...@.ln.
+000029d0: 1fa5 fa5d 5676 c9db b25a 65de 7f42 cf84  ...]Vv...Ze..B..
+000029e0: 8324 b618 b5e2 4a23 039c 0053 4e22 89a0  .$....J#...SN"..
+000029f0: 5ee3 8e70 b6d3 ccaa b544 307e f2e2 c40a  ^..p.....D0~....
+00002a00: 1c8d 463d c1a0 a8ce 216f c1bf 7756 eb85  ..F=....!o..wV..
+00002a10: adaf 2287 5edb 7d7a 30c4 383f 2728 8104  ..".^.}z0.8?'(..
+00002a20: 5941 9903 970c d5b2 8209 1ac7 8fa7 0e5c  YA.............\
+00002a30: 9640 7b6f dae9 5dd1 de6b 728a 936c b621  .@{o..]..kr..l.!
+00002a40: 7406 cb7c a774 036d 3695 e616 2c7b 5199  t..|.t.m6...,{Q.
+00002a50: 73da 1a88 45b3 fdc1 7e8d eae0 bd53 c600  s...E...~....S..
+00002a60: 15cb bc61 64af 24e1 b61e d38e f94e 684f  ...ad.$......NhO
+00002a70: e8c4 029b 0374 d294 6f72 346a 4c77 68e1  .....t..or4jLwh.
+00002a80: 47f4 abba ce07 e7c2 5555 7073 f2f2 aaae  G.......UUps....
+00002a90: 0fe6 7f8b e55a 3ac7 bc02 3b6a caf9 83cd  .....Z:...;j....
+00002aa0: e76f ed8b 2e1a da59 07c1 1969 3965 9bc9  .o.....Y...i9e..
+00002ab0: 0e81 17e3 d097 c54f 6cb9 e668 1e7b 069b  .......Ol..h.{..
+00002ac0: 42b1 be1f 160d ed19 ff5b bbe3 6f38 05f2  B........[..o8..
+00002ad0: 6937 225d c74f b675 2d4b fc6c e318 7a99  i7"].O.u-K.l..z.
+00002ae0: bfe5 6c2f 059d 0e12 e855 3f45 07a5 d927  ..l/.....U?E...'
+00002af0: d86a 9bbc 8675 0a87 2b5c 2186 d556 02bc  .j...u..+\!..V..
+00002b00: 70f4 1fda cfe2 1b0f 9e6b 89fb ccc7 0f47  p........k.....G
+00002b10: b1a3 ba72 b7c8 c8e8 ef8d db9e 5763 d6fe  ...r........Wc..
+00002b20: a3b8 5de5 a1d6 3342 bda0 d399 18c8 1e59  ..]...3B.......Y
+00002b30: 05fe 60c3 e333 3777 47c6 0d93 5fa1 1260  ..`..37wG..._..`
+00002b40: 36c3 859c 91cd b5b1 179e a3ed d90a 10b3  6...............
+00002b50: a12d 3972 f378 5e2c f065 fc33 6dd8 51ac  .-9r.x^,.e.3m.Q.
+00002b60: ce5a bfb0 6765 1c44 812f e3f7 f648 8a17  .Z..ge.D./...H..
+00002b70: d606 1dcc fb1e ce11 f8a2 a366 05fe e37e  ...........f...~
+00002b80: f3d3 6a7b 5f25 c132 da2c 83f4 9666 c12a  ..j{_%.2.,...f.*
+00002b90: db6c 832c bddb 6cb7 d52a 4aa2 bb3f 67d7  .l.,..l..*J..?g.
+00002ba0: eebf b874 dd5f 02d0 294e d73d 87ab 598f  ...t._..)N.=..Y.
+00002bb0: c18e 213e 5c64 059e 4dbc fb8e 8de0 f6dc  ..!>\d..M.......
+00002bc0: f755 b288 de66 7114 54b7 511c a40b b20c  .U...fq.T.Q.....
+00002bd0: 968b db2c a8b2 38d9 2ed2 cd7d 5665 33df  ...,..8....}Ve3.
+00002be0: b357 5ece 5118 c7fe 9ab7 ce67 6bc3 04e5  .W^.Q......gk...
+00002bf0: 4c4e b59a 2a34 9742 9160 fa37 4184 5325  LN..*4.B.`.7A.S%
+00002c00: c2cb 2f58 f917 0000 00ff ff03 0050 4b03  ../X.........PK.
+00002c10: 0414 0006 0008 0000 0021 006b dcd4 f9ab  .........!.k....
+00002c20: 0500 00e1 3e00 0014 0000 0078 6c2f 7368  ....>......xl/sh
+00002c30: 6172 6564 5374 7269 6e67 732e 786d 6cd4  aredStrings.xml.
+00002c40: 9b5b 6fe2 3818 86ef 57da ff90 e59e a494  .[o.8...W.......
+00002c50: 969d a928 a32e d051 b5d3 83a0 bd8b 14a5  ...(...Q........
+00002c60: c180 7713 2763 3b6c 995f bf5f cad9 0730  ..w.'c;l._._...0
+00002c70: 4d54 928b 5ed4 87f8 fd9e bcf1 09bb fded  MT..^...........
+00002c80: 2d0a ad19 a20c c7e4 bad6 b0cf 6a16 2241  -...........j."A
+00002c90: 3cc2 6472 5d7b 79be ad7f a959 8cfb 64e4  <.dr]{y....Y..d.
+00002ca0: 8731 41d7 b539 62b5 6f9d df7f 6b33 c62d  .1A..9b.o...k3.-
+00002cb0: a84b d875 6dca 7972 e538 2c98 a2c8 6776  .K.um.yr.8,...gv
+00002cc0: 9c20 0239 e398 463e 877f e9c4 6109 45fe  . .9..F>....a.E.
+00002cd0: 884d 11e2 51e8 9c9f 9db5 9cc8 c7a4 6605  .M..Q.........f.
+00002ce0: 714a f875 add9 baac 5929 c13f 53d4 5da4  qJ.u....Y).?S.].
+00002cf0: 9c37 2f6a 9d36 c39d 36ef dc91 117a 6b3b  .7/j.6..6....zk;
+00002d00: bcd3 76b2 8445 e200 853e c733 f4e0 4748  ..v..E...>.3..GH
+00002d10: ccbb 4dc3 5095 fe97 cf10 5194 efbf 7144  ..M.P.....Q...qD
+00002d20: 3202 e283 9e7c 8a08 1753 6f38 a7f8 35e5  2....|...So8..5.
+00002d30: 52bb 43fc 4b4a eb42 e41c f5e0 4f7c cc3d  R.C.KJ.B....O|.=
+00002d40: 501e 6334 52e5 dd04 0162 4c95 f303 cd50  P.c4R....bL....P
+00002d50: 28c3 187b 4314 706d 08de 008d a530 6830  (..{C.pm.....0h0
+00002d60: 0580 5916 8230 0349 a00b 6ff2 cd8b 7c82  ..Y..0.I..o...|.
+00002d70: c788 716f 8208 a23e 8fa9 f8a0 ee95 fbc2  ..qo...>........
+00002d80: c042 6e77 4a31 b39f 2886 87b9 2f04 87a0  .BnwJ1..(.../...
+00002d90: 95ba 2f37 837b eb19 f911 c31c 5975 eb66  ../7.{......Yu.f
+00002da0: d1ae dbc3 13cc fdd0 7aa2 086a cfe0 6dc6  ........z..j..m.
+00002db0: c485 a469 fa6a daf2 c904 8a08 7a58 a272  ...i.j......zX.r
+00002dc0: 2696 d105 e58e 3093 3cf6 794c 95cd ab24  &.....0.<.yL...$
+00002dd0: 358e 0a48 176d 1dfa 18fb b29e cc9b 7502  5..H.m........u.
+00002de0: 3d4a dd27 73fb bfa9 e4e8 4f8e 3fa7 5a8d  =J.'s.....O.?.Z.
+00002df0: 0f15 b18a 0c55 b1df c287 2396 6b38 45e2  .....U....#.k8E.
+00002e00: b7b9 4fed c9af d37d c8ef a6db 0f5d a371  ..O....}.....].q
+00002e10: 2fea ac8e 4458 8eb3 e19c 17e7 e556 a5bc  /...DX.......V..
+00002e20: 7c58 ed3e c0bb b565 8f36 0bc4 5a01 8fb6  |X.>...e.6..Z...
+00002e30: 3ee0 d1f7 3a32 b98b a2c8 41f7 5a21 439a  >...:2....A.Z!C.
+00002e40: a8d5 1b52 ac2d 63bd 2c10 6be9 0d99 8dac  ...R.-c.,.k.....
+00002e50: ea8e 7d2f 4255 a7d9 705a c6e4 7edc 75fb  ..}/BU..pZ..~.u.
+00002e60: 0fc3 be1d 8d4e 389e e845 2c73 a461 4196  .....N8..E,s.aA.
+00002e70: 6b3e 2894 6e62 6c3a 6136 efa0 3521 ba9e  k>(.nbl:a6..5!..
+00002e80: 8709 e69e 6727 f313 beee 0fa8 5b09 978c  ....g'......[...
+00002e90: 2007 d23c 62b2 a557 92cc 031f 96c4 9e57   ..<b..W.......W
+00002ea0: 4a4e 5a75 9ea7 cd6a 1e31 6f32 e0b2 f152  JNZu...j.1o2...R
+00002eb0: 90cc f934 26f5 66e3 0c7c 1594 1b98 b1ec  ...4&.f..|......
+00002ec0: f5a7 b215 9ec2 7d52 b880 b958 03aa 149f  ......}R...X....
+00002ed0: 5713 b452 b602 b4d4 9767 5073 77f0 0072  W..R.....gPsw..r
+00002ee0: fd71 b841 88ed 6a19 d740 b150 44b4 6b46  .q.A..j..@.PD.kF
+00002ef0: b188 3144 47b1 0aae dc45 a454 2c14 5151  ..1DG....E.T,.QQ
+00002f00: 349f f09b f4a4 411c 4531 a99a 1d8d 44cb  4.....A.E1....D.
+00002f10: a1a9 709a 4ff4 3f84 b312 be14 71aa ad29  ..p.O.?.....q..)
+00002f20: 9552 e134 9ffd 9be0 9cfa 6c5a 316f 9a48  .R.4......lZ1o.H
+00002f30: 16cb a840 fe69 bc8c fa00 c82a b852 80a4  ...@.i.....*.R..
+00002f40: 942c 9651 81fc 5228 c81d d815 b3e6 51da  .,.Q..R(......Q.
+00002f50: b585 558c bf7e 0ae3 2ab8 5687 4da9 5d5b  ..U..~..*.V.M.][
+00002f60: 58c5 b861 febb 9049 8fb0 5b66 d6d8 f272  X..a...I..[f...r
+00002f70: e538 7b87 e5ef 0b57 49db fc57 1313 dacb  .8{....WI..W....
+00002f80: 1fca 2bd6 6118 aa56 1453 222d 7615 25b7  ..+.a..V.S"-v.%.
+00002f90: 5a05 df1a aa56 1453 22cd bfa4 ca56 1ca5  Z....V.S"....V..
+00002fa0: dc91 530b 8354 1944 0114 1693 db72 82d0  ..S..T.D.....r..
+00002fb0: 695b 2c70 641c f957 88ef f3aa 52c2 d028  i[,pd..W....R..(
+00002fc0: cb92 6510 f9d7 7611 e2fe c8e7 bef8 ec4f  ..e...v........O
+00002fd0: 3c65 a01b 5e74 d274 e9cd 237e 9939 d4a6  <e..^t.t..#~.9..
+00002fe0: db4b 5f43 4cba 3145 7040 274a e044 15b2  .K_CL.1Ep@'J.D..
+00002ff0: e1e8 5689 3199 4a56 4426 46a5 8a14 e816  ..V.1.JVD&F.....
+00003000: b0f5 ba7a 776e ffa6 5719 b087 b46e e7cb  ...zwn..W....n..
+00003010: df68 ab80 cdd5 35b6 efbd a741 65b8 1d14  .h....5....Ae...
+00003020: bb53 4045 2eff b8b7 2677 ffd8 1b56 86dc  .S@E....&w...V..
+00003030: 41b1 3b05 54e4 f20f 91bb 6bb7 528e 9587  A.;.T.....k.R...
+00003040: 24ee e4cb 94f2 ef40 498b aef2 63ca 9692  $......@I...c...
+00003050: b24a 3110 1956 fe5d 26e6 c338 8a58 0987  .J1..V.]&..8.X..
+00003060: 508d 324d 72d3 c9bf 1bb4 7cb4 fb08 e788  P.2Mr.....|.....
+00003070: 4b3a af38 2431 932e dbe4 6b01 9384 55cb  K:.8$1....k...U.
+00003080: cbb3 f1e5 358c ab51 a849 06e3 1430 1710  ....5..Q.I...0..
+00003090: e8b8 a380 af27 a821 935e 4909 26f2 472a  .....'.!.^I.&.G*
+000030a0: de04 24cf 4b15 01be 532d c075 3c3b c95f  ..$.K...S-.u<;._
+000030b0: dacd 823d ea56 59f2 c758 c08e ea6a 9fa6  ...=.VY..X...j..
+000030c0: 9403 9b5e dc32 4781 24f7 b6a7 8d26 933a  ...^.2G.$....&.:
+000030d0: 26e3 b87c fd92 569a 3623 f734 71fd 6477  &..|..V.6#.4q.dw
+000030e0: 84e0 76d3 086e cbcc 3d58 39ff cb6c fe76  ..v..n..=X9..l.v
+000030f0: cabb 1b9a 15fe 717a c598 a40e 4911 e345  ......qz....I..E
+00003100: febe 6823 12ee 58d1 b997 c498 c07d b192  ..h#..X......}..
+00003110: 033d a475 3b5f 0479 917f 60dc 407b fafb  .=.u;_.y..`.@{..
+00003120: 7bfd eee1 f6b1 c41f a8ab d3a8 4bbf c87f  {...........K...
+00003130: b868 0388 a29f 2986 bb65 6577 d43e 9dab  .h....)..eew.>..
+00003140: 3cd9 4905 f669 c3c7 9741 b73f 2c3b a73d  <.I..i...A.?,;.=
+00003150: 3297 5932 a5dc 5bc7 1b3b f138 f1b2 0b8d  2.Y2..[..;.8....
+00003160: 61d9 39ed 15ba ce94 5999 9ff9 49e6 098d  a.9.....Y...I...
+00003170: ff81 fba6 368f 4fba 5bbc 5fc8 3a57 1ed0  ....6.O.[._.:W..
+00003180: 14b2 cdad 3280 add0 fb13 df77 d06a 5864  ....2......w.jXd
+00003190: 8811 4bef f619 73f9 9261 0fb1 80e2 4475  ..K...s..a....Du
+000031a0: 8d18 6e17 a714 73e9 ccff 1dcc 8578 768d  ..n...s......xv.
+000031b0: 995e 7553 0676 b8eb 896d f709 47d4 9ac7  .^uS.v...m..G...
+000031c0: 29b5 b61a b0a6 70e9 f80f b12c 2cb7 a54b  ).....p....,,..K
+000031d0: d85b f5df 55ab 6b0e e1f9 01da 6edd 812b  .[..U.k.....n..+
+000031e0: ea9d ff01 0000 ffff 0300 504b 0304 1400  ..........PK....
+000031f0: 0600 0800 0000 2100 635b 0d84 5c01 0000  ......!.c[..\...
+00003200: 9106 0000 1300 2800 6375 7374 6f6d 586d  ......(.customXm
+00003210: 6c2f 6974 656d 312e 786d 6c20 a224 0028  l/item1.xml .$.(
+00003220: a020 0000 0000 0000 0000 0000 0000 0000  . ..............
+00003230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003240: 0000 00ec 955d 4fc2 3014 86ff cac2 35ae  .....]O.0.....5.
+00003250: 1b12 0ca4 2b31 1095 18d0 087a df95 836b  ....+1.....z...k
+00003260: ecc7 6c3b e2fc f59e 8d80 c184 c42b ae48  ..l;.........+.H
+00003270: 937e 9df6 f4ed 79d2 1e3a d6de 5e09 6b02  .~....y..:..^.k.
+00003280: 98b0 aa4b 1833 ea4b 18bd 8000 b905 e7a3  ...K.3.K........
+00003290: 2fad 8c1f e15c d629 4228 4784 7851 80e6  /....\.)B(G.xQ..
+000032a0: 3ed6 5238 ebed 26c4 c26a e20b eea0 b4d2  >.R8..&..j......
+000032b0: 0402 5b74 e63b 8cee bd30 bae0 1ad8 d48a  ..[t.;...0......
+000032c0: 4aa3 299a 4da3 7b30 e078 b08e 92d6 4697  J.).M.{0.x....F.
+000032d0: b511 85b3 467e f320 ad61 fbb1 ad3c 257f  ....F~. .a...<%.
+000032e0: 8db4 91ca d224 4952 4ada 3e5d c267 0546  .....$IRJ.>].g.F
+000032f0: c0a2 d239 b8d6 86fb 8e27 e9ab 538c 92b6  ...9.....'..S...
+00003300: bef5 1e74 ae6a 363f 5ce3 69b3 9102 e2bd  ...t.j6?\.i.....
+00003310: cc39 37fc 1d1a c1dd e80d 4381 aab2 7410  .97.......C...t.
+00003320: 274d e946 934a 85ca 4166 a00a 8eab 6ef4  'M.F.J..Af....n.
+00003330: 5ce5 4a8a 47a8 57f6 034c 7693 c230 1790  \.J.G.W..Lv..0..
+00003340: a6d8 f67b 4341 c9e1 443a 51dc fbff 1c1c  ...{CA..D:Q.....
+00003350: cf10 8c33 5c35 a266 eb07 6ed6 0a30 643b  ...3\5.f..n..0d;
+00003360: 0774 ca03 c7fb ec9a 3ba9 702d 0e0f 9ddf  .t......;.p-....
+00003370: f09f 0144 ef34 0864 7401 d1bc a6b3 bc88  ...D.4.dt.......
+00003380: fe69 10c8 e802 e26c 2006 a741 5c5f 40ec  .i.....l ..A\_@.
+00003390: f20b 7e57 47e9 86fd 0000 00ff ff03 0050  ..~WG..........P
+000033a0: 4b03 0414 0006 0008 0000 0021 00b8 b7cf  K..........!....
+000033b0: 58ea 0000 0041 0100 0018 0028 0063 7573  X....A.....(.cus
+000033c0: 746f 6d58 6d6c 2f69 7465 6d50 726f 7073  tomXml/itemProps
+000033d0: 312e 786d 6c20 a224 0028 a020 0000 0000  1.xml .$.(. ....
+000033e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000033f0: 0000 0000 0000 0000 0000 0000 0064 8f41  .............d.A
+00003400: 6b83 4010 85ef 85fe 0799 bbae d16a 6c50  k.@..........jlP
+00003410: 4352 1bc8 b534 d0eb b28e 71c1 dd91 9d35  CR...4....q....5
+00003420: 144a ff7b 577a 4a7b 1886 37c3 bcef 4dbd  .J.{WzJ{..7...M.
+00003430: ff34 5374 43c7 9a6c 039b 2485 08ad a25e  .4StC..l..$....^
+00003440: db6b 0397 f753 5c41 c45e da5e 4e64 b101  .k...S\A.^.^Nd..
+00003450: 4bb0 6f1f 1fea 9e77 bdf4 923d 393c 7b34  K.o....w...=9<{4
+00003460: 5118 e8d0 cf5d 035f d969 7b78 4ebb 2e0e  Q....]._.i{xN...
+00003470: 95c6 4f45 99c7 873c 2be2 eaf5 a52b 8fdb  ..OE...<+....+..
+00003480: 63b1 c9ab 6f88 02da 061b 6e60 f47e de09  c...o.....n`.~..
+00003490: c16a 4423 39a1 196d 580e e48c f441 baab  .jD#9..mX....A..
+000034a0: a061 d00a 3b52 8b41 eb45 96a6 a550 4bc0  .a..;R.A.E...PK.
+000034b0: 9b0f 3341 bbe6 f9bd 7ec3 81ef e51a 6d71  ..3A....~.....mq
+000034c0: fa1f c568 e588 69f0 8922 2378 940e 67d2  ...h..i.."#x..g.
+000034d0: c11c 6f01 c120 da5a fcb1 5df5 dddb ed0f  ..o.. .Z..].....
+000034e0: 0000 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
+000034f0: 0000 0021 00bd 8462 2390 0000 00db 0000  ...!...b#.......
+00003500: 0013 0028 0063 7573 746f 6d58 6d6c 2f69  ...(.customXml/i
+00003510: 7465 6d32 2e78 6d6c 20a2 2400 28a0 2000  tem2.xml .$.(. .
+00003520: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003530: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003540: 6c8e 3b0e c230 1005 af82 d293 2de8 d0e2  l.;..0......-...
+00003550: 3481 0a51 e502 c638 8aa5 acd7 f22e 1fdf  4..Q...8........
+00003560: 1e07 4181 947a 9e66 1e76 24bc 751c d547  ..A..z.f.v$.u..G
+00003570: 1d4a f29d c113 671a 3ca5 d9aa 97cd 8be6  .J....g.<.......
+00003580: 2887 6652 4d7b 0071 9327 2b2d 0597 5978  (.fRM{.q.'+-..Yx
+00003590: d4d6 3181 4c36 fbc4 212a 3c76 f0b5 69b5  ..1.L6..!*<v..i.
+000035a0: c158 5dd2 18ec 8354 5f31 3dbb 3bd5 d439  .X]....T_1=.;..9
+000035b0: 5cb3 cd65 4921 fc20 1e6f 41d7 271f 8217  \..eI!. .oA.'...
+000035c0: ff5c c70b 40f8 3b6e de00 0000 ffff 0300  .\..@.;n........
+000035d0: 504b 0304 1400 0600 0800 0000 2100 3596  PK..........!.5.
+000035e0: 801d f100 0000 4f01 0000 1800 2800 6375  ......O.....(.cu
+000035f0: 7374 6f6d 586d 6c2f 6974 656d 5072 6f70  stomXml/itemProp
+00003600: 7332 2e78 6d6c 20a2 2400 28a0 2000 0000  s2.xml .$.(. ...
+00003610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003620: 0000 0000 0000 0000 0000 0000 0000 6490  ..............d.
+00003630: 416b c330 0c85 ef83 fd87 a07b 6a37 49c7  Ak.0.......{j7I.
+00003640: 2849 4a3a 77d0 ebd8 6057 e328 8d21 b682  (IJ:w...`W.(.!..
+00003650: ad94 8db1 ff3e 879d ba5d 249e 84de f750  .....>...]$....P
+00003660: 7df8 7053 76c5 102d f906 b61b 0919 7a43  }.pSv..-......zC
+00003670: bdf5 9706 de5e 9ff3 47c8 226b dfeb 893c  .....^..G."k...<
+00003680: 36e0 090e edfd 5ddd c77d af59 47a6 8067  6.....]..}.YG..g
+00003690: 4697 a581 4dfd ac1a f8aa ba62 a74e 4fbb  F...M......b.NO.
+000036a0: fc74 945d 5e55 a5cc 3ba5 5229 ab6d 712c  .t.]^U..;.R).mq,
+000036b0: 5551 c9f2 1bb2 84f6 c926 3630 32cf 7b21  UQ.......&602.{!
+000036c0: a219 d1e9 b8a1 197d 5a0e 149c e624 c345  .......}Z....$.E
+000036d0: d030 5883 8acc e2d0 b328 a47c 1066 4978  .0X......(.|.fIx
+000036e0: f7ee 2668 d73c bfd7 2f38 c45b b946 5b82  ..&h.<../8.[.F[.
+000036f0: fd47 71d6 048a 34f0 c690 1371 d401 67b2  .Gq...4....q..g.
+00003700: c9fc 5a0a 439e 1387 3f67 146b 8c08 a2ad  ..Z.C...?g.k....
+00003710: c51f c8aa 6f9e d0fe 0000 00ff ff03 0050  ....o..........P
+00003720: 4b03 0414 0006 0008 0000 0021 0070 ed44  K..........!.p.D
+00003730: 6efa 0100 0078 0400 0013 0028 0063 7573  n....x.....(.cus
+00003740: 746f 6d58 6d6c 2f69 7465 6d33 2e78 6d6c  tomXml/item3.xml
+00003750: 20a2 2400 28a0 2000 0000 0000 0000 0000   .$.(. .........
 00003760: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003770: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000037a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000037b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000037c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000037d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000037e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000037f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003800: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000038a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000038b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000038c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000038d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000038e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000038f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003980: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000039a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00003770: 0000 0000 0000 0000 ac54 4d6f e230 14fc  .........TMo.0..
+00003780: 2b28 77c7 ce77 8c42 102a 974a 8bd4 a574  +(w..w.B.*.J...t
+00003790: d51b 32f6 3358 4aec c836 85fe fb4d 680b  ..2.3XJ..6...Mh.
+000037a0: 1c56 02a4 3dc5 87cc bcf1 bc19 57d3 63db  .V..=.......W.c.
+000037b0: 8c3e c03a 65f4 2488 4212 8c40 7323 94de  .>.:e.$.B..@s#..
+000037c0: 4e82 bd97 a80c a675 d58d 3b6b 3ab0 5e81  N......u..;k:.^.
+000037d0: 1bf5 08ed c6dd 24d8 79df 8d31 767c 072d  ......$.y..1v|.-
+000037e0: 7361 abb8 35ce 481f 72d3 6223 a5e2 8063  sa..5.H.r.b#...c
+000037f0: 4272 dc82 6782 7986 2f2c c137 cdd1 a933  Br..g.y./,.7...3
+00003800: d1e1 7008 0f49 68ec 7680 45f8 7df1 ebf5  ..p..Ih.v.E.}...
+00003810: c48d 9476 9e69 0e3f a88e df37 5d69 693a  ...v.i.?...7]ii:
+00003820: e677 035f 815f 98f5 1aec 93d1 de9a c605  .w._._..........
+00003830: 7525 0cdf b7a0 fd82 69b6 85e1 5457 6bd1  u%......i...TWk.
+00003840: f0f5 dcf0 67f1 2571 1294 7102 8432 4039  ....g.%q..q..2@9
+00003850: cf39 4a09 8b51 4912 8aa2 98d2 9264 5224  .9J..QI......dR$
+00003860: 9206 f5db 2cff bd58 a6af 2f7f 66ef a84c  ....,..X../.f..L
+00003870: cb38 4b0b 9aa3 880c df0a 5f68 ebaa e1b2  .8K......._h....
+00003880: c865 9465 1c44 2a04 dfa4 8416 5192 4a99  .e.e.D*.....Q.J.
+00003890: f024 89e5 7930 e329 dde4 0215 3900 4a59  .$..y0.)....9.JY
+000038a0: cc11 1332 46a9 a025 6325 cb37 11f4 b758  ...2F..%c%.7...X
+000038b0: 816d bfd7 f27f 6cc1 27c6 bac2 b784 f6b3  .m....l.'.......
+000038c0: d9f1 8979 be9b 35cd 8fea 98c6 8208 1e23  ...y..5........#
+000038d0: c828 4529 308a 3619 4894 241b 298a deb4  .(E)0.6.H.$.)...
+000038e0: 8c17 fd22 9d1a 6bd5 4c02 6ff7 10e0 baea  ..."..k.L.o.....
+000038f0: 2d3f ed62 7d24 2426 ebd5 6707 e421 237a  -?.b}$$&..g..!#z
+00003900: 8e19 f7ea 031e 42dd 25e4 511d 9765 bfd9  ......B.%.Q..e..
+00003910: b32f f7c5 a8ea 11f5 d02c d757 6bdf 3b04  ./.......,.Wk.;.
+00003920: 7d3b 43b7 6316 3aa3 f457 b93c b0d6 e1b7  };C.c.:..W.<....
+00003930: d972 b11a 4eca 035e 37ec d3ec bdc3 5186  .r..N..^7.....Q.
+00003940: 4fe9 5d82 5036 64ae 3b4e 9fe7 931b e91c  O.].P6d.;N......
+00003950: 8656 7370 dcaa cef7 4fc1 ad34 5fff 7a9d  .Vsp....O..4_.z.
+00003960: ed13 0ffe 57ad f0f5 1b52 ff05 0000 ffff  ....W....R......
+00003970: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00003980: 8f88 54fb 5b01 0000 6002 0000 1800 2800  ..T.[...`.....(.
+00003990: 6375 7374 6f6d 586d 6c2f 6974 656d 5072  customXml/itemPr
+000039a0: 6f70 7333 2e78 6d6c 20a2 2400 28a0 2000  ops3.xml .$.(. .
 000039b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000039c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000039d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000039e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000039f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000039d0: a492 416b 1b31 1085 ef85 fe87 45f7 b1b4  ..Ak.1......E...
+000039e0: daf5 ae14 b20e b653 436e a5a4 d0eb 581a  .......SCn....X.
+000039f0: c50b 9664 2439 044a ff7b b5a4 97b4 f8d4  ...d$9.J.{......
+00003a00: 9378 12ef 7b4f c3dc 3fbc f973 f34a 29cf  .x..{O..?..s.J).
+00003a10: 314c ac5d 09d6 5030 d1ce e165 62df 9f0f  1L.]..P0...eb...
+00003a20: a058 930b 068b e718 6862 21b2 87cd e74f  .X......hb!....O
+00003a30: f736 df59 2c98 4b4c f454 c837 f562 aee7  .6.Y,.KL.T.7.b..
+00003a40: d3e3 c47e 764a 6d77 07d1 c37e bf6f a197  ...~vJmw...~.o..
+00003a50: bb03 e8b1 dd82 94db 411c 7a31 ecbe ec7e  ........A.z1...~
+00003a60: b1a6 4687 8ac9 133b 9572 b9e3 3c9b 1379  ..F....;.r..<..y
+00003a70: ccab 78a1 501f 5d4c 1e4b 95e9 8547 e766  ..x.P.]L.K...G.f
+00003a80: 438f d15c 3d85 c2a5 1003 37d7 1aef 7ff8  C..\=.....7.....
+00003a90: 33db 2c7d dedd dfc8 e58f 72a9 764d f33f  3.,}......r.vM.?
+00003aa0: 297e 3629 e6e8 caca 44ff 27e0 1dec a9e0  )~6)....D.'.....
+00003ab0: f23b 7e49 b54a 2a33 65c6 ff03 3a07 172f  .;~I.J*3e...:../
+00003ac0: 584e 0b7d e45f 3195 4069 1f43 49f1 7c9b  XN.}._1.@i.CI.|.
+00003ad0: ac64 4742 23c1 6006 03bd 4009 4a74 1a5a  .dGB#.`...@.Jt.Z
+00003ae0: a9b5 126b 673b a76f d652 687a 7d1c 2c8c  ...kg;.o.Rhz}.,.
+00003af0: 0311 f428 0da0 7512 7aab 15a2 c2e1 d8d2  ...(..u.z.......
+00003b00: 4db3 d4d2 0a6b 24d0 5a6b e809 351c d7e4  M....k$.Zk..5...
+00003b10: a0eb 8ece 8e35 7f6d c6c5 ccff 9afa a23f  .....5.m.......?
+00003b20: 6cc5 e637 0000 00ff ff03 0050 4b03 0414  l..7.......PK...
+00003b30: 0006 0008 0000 0021 00c3 945c adaa 0d00  .......!...\....
+00003b40: 0057 4f00 0013 0028 0063 7573 746f 6d58  .WO....(.customX
+00003b50: 6d6c 2f69 7465 6d34 2e78 6d6c 20a2 2400  ml/item4.xml .$.
+00003b60: 28a0 2000 0000 0000 0000 0000 0000 0000  (. .............
 00003b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003c90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ca0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003cb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003db0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003dc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003dd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003de0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003df0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003e00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003e10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004000: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000040a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000040b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000040c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000040d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000040e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000040f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000041a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000041b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000041c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000041d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000041e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000041f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000042a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000042b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000042c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000042d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000042e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000042f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000043a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000043b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000043c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000043d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000043e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000043f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000044a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000044b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000044c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000044d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000044e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000044f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004500: 0000 0000 0000 0000 0000 504b 0304 1400  ..........PK....
-00004510: 0600 0800 0000 2100 af39 1aeb d401 0000  ......!..9......
-00004520: ba04 0000 1800 2800 6375 7374 6f6d 586d  ......(.customXm
-00004530: 6c2f 6974 656d 5072 6f70 7333 2e78 6d6c  l/itemProps3.xml
-00004540: 20a2 2400 28a0 2000 0000 0000 0000 0000   .$.(. .........
-00004550: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004560: 0000 0000 0000 0000 b494 6f6b db30 10c6  ..........ok.0..
-00004570: df0f f61d 82de 2bf2 bfd8 5669 52d2 b481  ......+...ViR...
-00004580: c20a 63eb a06f cfd2 2931 b324 2329 cbc6  ..c..o..)1.$#)..
-00004590: d877 9fec 768c ae09 d958 fb4a 9ccc dd73  .w..v....X.J...s
-000045a0: f7f8 773a bff8 aabb c917 74be b566 4ed2  ..w:......t..fN.
-000045b0: 6942 2668 8495 add9 ccc9 a7bb 35ad c9c4  iB&h........5...
-000045c0: 0730 123a 6b70 4e8c 2517 8bb7 6fce a53f  .0.:kpN.%...o..?
-000045d0: 9310 c007 ebf0 26a0 9ec4 8b36 9e37 5773  ......&....6.7Ws
-000045e0: f2fd 322d 9655 be2a e8f5 72cd 6951 acd6  ..2-.U.*..r.iQ..
-000045f0: 7459 f135 cd2f 7916 cf75 9524 d73f c824  tY.5./y..u.$.?.$
-00004600: 4a9b 58c6 cfc9 3684 fe8c 312f b6a8 c14f  J.X...6...1/...O
-00004610: 6d8f 267e 54d6 6908 3174 1b66 956a 055e  m.&~T.i.1t.f.j.^
-00004620: 59b1 d368 02cb 92a4 6462 17e5 f5bd eec8  Y..h....db......
-00004630: 62e8 e721 fb03 2aff 341c 5adb b9f6 998a  b..!..*.4.Z.....
-00004640: 6e85 b3de aa30 1556 3f0a 3c14 d618 6098  n....0.V?.<...`.
-00004650: 8e09 6b42 94bb fbd6 2361 2f56 b577 7140  ..kB....#a/V.wq@
-00004660: 175a f46c 505a 86e0 da66 17d0 9fd2 d8ef  .Z.lPZ...f......
-00004670: f7d3 7d3e fa11 0d48 d9fd edbb 8fa3 65af  ..}>...H......e.
-00004680: d2dc d1a2 7596 63c2 0169 294a 418b 0432  ....u.c..i)JA..2
-00004690: 5a27 39a7 69c6 799d cc94 cc15 3f9e 0ca2  Z'9.i.y.....?...
-000046a0: e04d 2969 5522 d202 3241 41aa 8c16 92d7  .M)iU"..2AA.....
-000046b0: 0035 944d 7adc eb8c 6732 9122 a338 e311  .5.Mz...g2.".8..
-000046c0: 2c04 4e9b 192a 9ae7 8d92 55d4 9f89 eaff  ,.N..*....U.....
-000046d0: bd90 8f94 dd82 810d 8ebc 8548 c0c9 dff3  ...........H....
-000046e0: 0bdf 8360 b546 d91e c276 20ac 62ef c105  ...`.F...v .b...
-000046f0: 836e 15f9 72b6 fbeb ca07 16a3 07f1 3976  .n..r.........9v
-00004700: f90c 5c87 f437 67a7 3ce9 77ae 1bb1 9282  ..\..7g.<.w.....
-00004710: 6137 8eec 593a 4dd9 bf24 0674 da9f cc38  a7..Y:M..$.t...8
-00004720: 6c52 1bf7 cc19 e898 6de4 a0c9 fed8 e721  lR......m......!
-00004730: 7ef2 de2c 7e02 0000 ffff 0300 504b 0304  ~..,~.......PK..
-00004740: 1400 0600 0800 0000 2100 167c ddd5 4901  ........!..|..I.
-00004750: 0000 6602 0000 1100 0801 646f 6350 726f  ..f.......docPro
-00004760: 7073 2f63 6f72 652e 786d 6c20 a204 0128  ps/core.xml ...(
-00004770: a000 0100 0000 0000 0000 0000 0000 0000  ................
-00004780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000047a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000047b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000047c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000047d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000047e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000047f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004800: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004870: 0000 008c 925f 4bc3 3014 c5df 05bf 43c9  ....._K.0.....C.
-00004880: b36d d2d5 bfa1 edc0 c99e 1c08 4e14 df42  .m..........N..B
-00004890: 72b7 059b 3424 d1ae dfde b4dd 6a87 3e08  r...4$......j.>.
-000048a0: 79c9 bde7 fe72 ce25 f97c afaa e80b ac93  y....r.%.|......
-000048b0: b52e 509a 1014 81e6 b590 7a5b a097 f532  ..P.......z[...2
-000048c0: be45 91f3 4c0b 56d5 1a0a d482 43f3 f2fc  .E..L.V.....C...
-000048d0: 2ce7 86f2 dac2 93ad 0d58 2fc1 4581 a41d  ,........X/.E...
-000048e0: e5a6 403b ef0d c5d8 f11d 28e6 92a0 d0a1  ..@;......(.....
-000048f0: b9a9 ad62 3e5c ed16 1bc6 3fd8 16f0 8c90  ...b>\....?.....
-00004900: 6bac c033 c13c c31d 3036 2311 1d90 828f  k..3.<..06#.....
-00004910: 48f3 69ab 1e20 3886 0a14 68ef 709a a4f8  H.i.. 8...h.p...
-00004920: 47eb c12a f7e7 40df 9928 95f4 ad09 990e  G..*..@..(......
-00004930: 76a7 6cc1 87e6 a8de 3b39 0a9b a649 9aac  v.l.....;9...I..
-00004940: b711 fca7 f86d f5f8 dc47 8da5 ee76 c501  .....m...G...v..
-00004950: 95b9 e094 5b60 beb6 6597 dfb4 fb2a c793  ....[`..e....*..
-00004960: 62b7 c08a 39bf 0abb de48 10f7 6df9 6465  b...9....H..m.de
-00004970: 98bd 8816 3b2b 5d8e 7f0b 02b4 cf30 9041  ....;+]......0.A
-00004980: 44c1 151d 321c 3baf d9e2 61bd 44e5 8ccc  D...2.;...a.D...
-00004990: 2e63 d29d 754a 6876 45c9 dd7b f7fe c97c  .c..uJhvE..{...|
-000049a0: e772 28a8 838b ff13 6f68 4626 c423 a0ec  .r(.....ohF&.#..
-000049b0: 7d9f fe8c f21b 0000 ffff 0300 504b 0304  }...........PK..
-000049c0: 1400 0600 0800 0000 2100 290f f5c6 7d01  ........!.)...}.
-000049d0: 0000 fe02 0000 1000 0801 646f 6350 726f  ..........docPro
-000049e0: 7073 2f61 7070 2e78 6d6c 20a2 0401 28a0  ps/app.xml ...(.
-000049f0: 0001 0000 0000 0000 0000 0000 0000 0000  ................
-00004a00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004af0: 0000 9c92 cb4e c330 1045 f748 fc43 e43d  .....N.0.E.H.C.=
-00004b00: 750a 08a1 ca31 423c c402 44a5 1658 1b67  u....1B<..D..X.g
-00004b10: d258 b876 e419 a296 af67 9288 9202 2b76  .X.v.....g....+v
-00004b20: f3b8 ba3e beb6 bad8 ac7d d642 4217 4321  ...>.....}.BB.C!
-00004b30: a693 5c64 106c 2c5d 5815 e269 797b 742e  ..\d.l,]X..iy{t.
-00004b40: 3224 134a e363 8042 6c01 c585 3e3c 50f3  2$.J.c.Bl...><P.
-00004b50: 141b 48e4 0033 b608 5888 9aa8 9949 89b6  ..H..3..X....I..
-00004b60: 86b5 c109 af03 6faa 98d6 86b8 4d2b 19ab  ......o.....M+..
-00004b70: ca59 b88e f67d 0d81 e471 9e9f 49d8 1084  .Y...}...q..I...
-00004b80: 12ca a366 6728 06c7 594b ff35 2da3 edf8  ...fg(..YK.5-...
-00004b90: f079 b96d 1858 abcb a6f1 ce1a e25b ea07  .y.m.X.......[..
-00004ba0: 6753 c458 5176 b3b1 e095 1c2f 15d3 2dc0  gS.XQv...../..-.
-00004bb0: be27 475b 9d2b 396e d5c2 1a0f 576c ac2b  .'G[.+9n....Wl.+
-00004bc0: e311 94fc 1ea8 3b30 5d68 73e3 126a d5d2  ......;0]hs..j..
-00004bd0: ac05 4b31 65e8 3e38 b663 91bd 1a84 0ea7  ..K1e.>8.c......
-00004be0: 10ad 49ce 0462 ac4e 3634 7ded 1ba4 a45f  ..I..b.N64}...._
-00004bf0: 627a c31a 8050 4916 0cc3 be1c 6bc7 b53b  bz...PI.....k..;
-00004c00: d5d3 5ec0 c5be b033 1840 78b1 8fb8 74e4  ..^....3.@x...t.
-00004c10: 011f abb9 49f4 07f1 744c dc33 0cbc 03ce  ....I...tL.3....
-00004c20: a2e3 1bce 1cf3 f557 e693 7e78 dfbb f086  .......W..~x....
-00004c30: 4fcd 325e 1b82 afec f687 6a51 9b04 25c7  O.2^......jQ..%.
-00004c40: bdcb 7637 5077 1c5b f29d c955 6dc2 0aca  ..v7Pw.[...Um...
-00004c50: 2fcd ef45 f7d2 cfc3 77d6 d3b3 497e 92f3  /..E....w...I~..
-00004c60: 238e 664a 7e7f 5cfd 0900 00ff ff03 0050  #.fJ~.\........P
-00004c70: 4b03 0414 0006 0008 0000 0021 0074 3f39  K..........!.t?9
-00004c80: 7ac2 0000 0028 0100 001e 0008 0163 7573  z....(.......cus
-00004c90: 746f 6d58 6d6c 2f5f 7265 6c73 2f69 7465  tomXml/_rels/ite
-00004ca0: 6d31 2e78 6d6c 2e72 656c 7320 a204 0128  m1.xml.rels ...(
-00004cb0: a000 0100 0000 0000 0000 0000 0000 0000  ................
-00004cc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004cd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004ce0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004cf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004d00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004d10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004d20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004d30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004d40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004d50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004d60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004d70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004d80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004d90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004da0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004db0: 0000 0084 cfc1 8a02 310c 06e0 bbe0 3b94  ........1.....;.
-00004dc0: dc9d ce78 1091 e978 5916 bc89 b8e0 b574  ...x...xY......t
-00004dd0: 3233 c569 539a 28fa f616 4f2b 2cec 3109  23.iS.(...O+,.1.
-00004de0: f9fe a4dd 3fc2 acee 98d9 5334 d054 3528  ....?.....S4.T5(
-00004df0: 8c8e 7a1f 4703 3fe7 efd5 1614 8b8d bd9d  ..z.G.?.........
-00004e00: 29a2 8127 32ec bbe5 a23d e16c a52c f1e4  )..'2....=.l.,..
-00004e10: 13ab a244 3630 89a4 9dd6 ec26 0c96 2b4a  ...D60.....&..+J
-00004e20: 18cb 64a0 1cac 9432 8f3a 5977 b523 ea75  ..d....2.:Yw.#.u
-00004e30: 5d6f 74fe 6d40 f761 aa43 6f20 1ffa 06d4  ]ot.m@.a.Co ....
-00004e40: f999 4af2 ff36 0d83 77f8 45ee 1630 ca1f  ..J..6..w.E..0..
-00004e50: 11da dd58 285c c27c cc94 b8c8 368f 2806  ...X(\.|....6.(.
-00004e60: bc60 78b7 9aaa dc0b ba6b f5c7 7fdd 0b00  .`x......k......
-00004e70: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00004e80: 0021 005c 9627 22c3 0000 0028 0100 001e  .!.\.'"....(....
-00004e90: 0008 0163 7573 746f 6d58 6d6c 2f5f 7265  ...customXml/_re
-00004ea0: 6c73 2f69 7465 6d32 2e78 6d6c 2e72 656c  ls/item2.xml.rel
-00004eb0: 7320 a204 0128 a000 0100 0000 0000 0000  s ...(..........
+00003b80: 0000 0000 ec1c 6b8f db36 f27b 81fe 07c1  ......k..6.{....
+00003b90: f759 6bbd fc90 51a7 d847 b75d 74d3 04d9  .Yk...Q..G.]t...
+00003ba0: 4def be05 1449 ad75 2b4b ae24 ef03 87fb  M....I.u+K.$....
+00003bb0: ef37 24f5 a09e a6e5 a497 144d 8126 b634  .7$........M.&.4
+00003bc0: c3e1 7038 eff1 0f3f be6c 43ed 8926 6910  ..p8...?.lC..&i.
+00003bd0: 47eb 8979 664c 341a e198 04d1 c37a b2cf  G..yfL4......z..
+00003be0: 7c7d 39f9 f1cd 0f38 5be1 38ca 6894 ddbf  |}9....8[.8.h...
+00003bf0: eee8 1dde d02d d2e0 cb4f ebc9 44db a2f2  .....-...O..D...
+00003c00: 6fe9 a5df d096 ae27 5731 de6f 018c bf25  o......'W1.o...%
+00003c10: 3dbd b95a 4f8c 17c3 84ff 0cfb f27a 69d9  =..ZO........zi.
+00003c20: 8bf9 a56d 9b17 a663 9ec3 1fcb b1cf 7fba  ...m...c........
+00003c30: 7617 d67c 6137 617f 2fa8 9d9b cd47 5734  v..|a7a./....GW4
+00003c40: c549 b0cb f866 2e13 8a32 aa21 2da2 cf1a  .I...f...2.!-...
+00003c50: c909 396b 82dc e178 0784 f2af 733e 30e2  ..9k...x....s>0.
+00003c60: b085 5dcf f7e8 d2c5 33c3 c308 51e4 cc89  ..].....3...Q...
+00003c70: eb2f 1125 73c3 04a2 8071 51ba c2d9 7ab2  ./.%s....qQ...z.
+00003c80: c9b2 dd6a 3a4d 395b d2b3 6d80 9338 8dfd  ...j:M9[..m..8..
+00003c90: ec0c c7db 69ec fb01 a653 cb30 e6d3 2dcd  ....i....S.0..-.
+00003ca0: 1041 199a 4a9c 2810 6dd1 1844 bb04 a84f  .A..J.(.m..D...O
+00003cb0: b280 a61c f979 9625 81b7 cf68 3a79 f3fd  .....y.%...h:y..
+00003cc0: 773f bca4 6425 a8d2 3294 3cd0 8c1d 4aba  w?..d%..2.<...J.
+00003cd0: 4318 367c 3cd1 d55a 9c59 491c c3de b364  C.6|<..Z.YI....d
+00003ce0: 4ff9 473f a021 49f9 b922 64d9 c830 ad25  O.G?.!I.."d..0.%
+00003cf0: 6c9a 9ad6 c25c 2c5c d336 90b3 2498 2ed0  l....\,\.6..$...
+00003d00: 448b 524b 884c 94da c53f 1cf1 0fc1 5520  D.RK.L...?....U 
+00003d10: bca4 f0f9 f9f9 ecd9 3e8b 9307 c644 73fa  ........>....Ds.
+00003d20: afb7 b742 000b cebd a4ea efee 4edd b8a0  ...B........N...
+00003d30: 0f36 b09e 80d0 52c3 4554 9fe3 39d6 1d03  .6....R.ET..9...
+00003d40: 59fa d2b0 5ddd b45c 7769 cc7c 62fb 6e41  Y...]..\wi.|b.nA
+00003d50: 236c 1400 1076 5c6f 4ef4 c59c 52dd 4116  #l...v\oN...R.A.
+00003d60: d611 f12d dd21 ee12 a125 9a7b 26f0 b258  ...-.!...%.{&..X
+00003d70: c159 4f2c d722 06c1 964e 67ae ab3b 14b9  .YO,."...Ng..;..
+00003d80: ba37 a3be 6edb 9e4f 16b0 ce0c 2fca 830e  .7..n..O..../...
+00003d90: b6bb 38c9 b4a8 3a62 2502 a785 a074 c0ab  ..8...:b%....t..
+00003da0: d03b 00af 447e 094f 43ca 3405 dfc0 7a22  .;..D~.OC.4...z"
+00003db0: 095b 4120 dca6 5d48 5f98 062a 859b feb1  .[A ..]H_..*....
+00003dc0: 0775 557e aee3 28ee fc5b 14a1 078e bc64  .uU~..(..[.....d
+00003dd0: 5607 2e14 8605 da02 4d42 fdf5 840b 2b09  V.......MB....+.
+00003de0: f127 d065 3704 643d 88de 61bc 4f40 ea8c  .'.e7.d=..a.O@..
+00003df0: 498b fa0e 908f 4938 02ea 3dd3 7269 a6bc  I.....I8..=.ri..
+00003e00: a2bd 2a74 eda7 17c3 b08c 4f8c 4f8a eb76  ..*t......O.O..v
+00003e10: c282 2550 daaa bd3a c759 f0a4 ba96 b5ba  ..%P...:.Y......
+00003e20: dba0 8492 7f06 d9e6 630a 9b54 e64d 0577  ........c..T.M.w
+00003e30: 057a 3408 d521 6f51 9a09 e88b 57b6 a6f2  .z4..!oQ....W...
+00003e40: 9232 e07d b055 e7e7 5b4a 0274 4793 27d0  .2.}.U..[J.tG.'.
+00003e50: fd6f 73ad afcc 4f19 f81a 483f 09c1 15d8  .os...O...H?....
+00003e60: c07b f448 a351 cb9f efb3 f81e 3da8 b2da  .{.H.Q......=...
+00003e70: 5ec9 b4bf bbfc 306a d1db 1823 66c2 4701  ^.....0j...#f.G.
+00003e80: ff4c 239a 70f0 d107 f6d3 13e8 a15f 50ba  .L#.p........_P.
+00003e90: b98c c9b8 2367 6cfb 95be be8f 8328 1bc7  ....#gl......(..
+00003ea0: bb91 d0b7 347a c836 37d1 1d05 1783 a82f  ....4z.67....../
+00003eb0: 1d62 7f31 f7cd d90c 53e2 1082 3dc7 7017  .b.1....S...=.p.
+00003ec0: a6ed f8be 8d6d dbf2 158f c259 dda3 974b  .....m.....Y...K
+00003ed0: 94e1 cd79 a8aa f41a 32e3 fd9b e20c 2e38  ...y....2......8
+00003ee0: fc3f 4e72 576f 1c0b ef28 4af0 e67d e921  .?NrWo...(J..}.!
+00003ef0: 75ed 61ca 5ca4 5cf3 f37f 370c 03ff 2e37  u.a.\.\...7....7
+00003f00: 07cc 3af0 cfa9 6475 d481 b877 78c8 2b53  ..:...du...wx.+S
+00003f10: f329 7282 aee3 647b 457d b40f c111 fb63  .)r...d{E}.....c
+00003f20: 8fc2 009c 30b0 505f d887 22db cae1 3aec  ....0.P_.."...:.
+00003f30: f3b6 8df0 3403 cb04 472a c8dc 6135 972c  ....4...G*..a5.,
+00003f40: 88fc 7887 b20d 7302 17d3 f728 c9e0 9e5f  ..x...s....(..._
+00003f50: 4250 92c4 6009 fa9d 1865 3fb7 97d0 010f  BP..`....e?.....
+00003f60: 4705 f930 e13d eecf 27d9 e140 ab20 22f4  G..0.=..'..@. ".
+00003f70: 653d 71c0 750e c210 7921 38f0 a5e7 4d82  e=q.u...y!8...M.
+00003f80: 7417 a2d7 7ac0 a5dd 5c69 bfa3 3077 ce89  t...z...\i..0w..
+00003f90: 1c17 dd6f a8f6 c41e 69b1 af65 f0a1 d839  ...o....i..e...9
+00003fa0: 8341 691a 3c44 9468 590c cf82 540b 32ba  .Ai.<D.hY...T.2.
+00003fb0: 1541 13e8 329a 4428 140b 3528 8458 8bbc  .A..2.D(..5(.X..
+00003fc0: 8bc2 d79c ae52 cec1 ab0c a9ec b225 3485  .....R.......%4.
+00003fd0: 1805 3c86 38d2 3c94 c246 409e 56f7 f425  ..<.8.<..F@.V..%
+00003fe0: 13ce 94b8 6135 b0e6 2564 77b6 eee9 55c4  ....a5..%dw...U.
+00003ff0: 0867 abe4 d8ec 288e f140 a6c6 2bf0 c2b6  .g....(..@..+...
+00004000: 2862 6e69 1844 8f25 53ea d1e4 2620 8442  (bni.D.%S...& .B
+00004010: f45c 9e48 1fa7 0ae2 7a98 d5e1 94e6 5f31  .\.H....z....._1
+00004020: 3907 224a fff4 053e b188 5de2 e0c7 0fb7  9."J...>..].....
+00004030: 55cc 37e8 1673 2ad8 1d14 ac07 2909 48db  U.7..s*.....).H.
+00004040: 476d 4a5a 8fa0 4a11 f744 1348 79d4 0967  GmJZ..J..D.Hy..g
+00004050: 1c3d b498 cf91 74eb 5010 00b1 a752 cdb6  .=....t.P....R..
+00004060: f7ae a26c 8784 43f6 a94b 1199 1f16 911c  ...l..C..K......
+00004070: 0eee 475b 427e a574 c72e 0e1c 0622 44dc  ..G[B~.t....."D.
+00004080: 1465 81a8 1374 e21d ba88 e390 a2e8 846b  .e...t.........k
+00004090: d4f6 cc4b 2e99 0aba 4780 6bcc b36f f389  ...K....G.k..o..
+000040a0: 7f53 bf18 5dcb 7d91 ab01 2eff 5b30 9281  .S..].}.....[0..
+000040b0: ea05 81f7 6fc0 dc34 1c06 4874 bd14 91df  ....o..4..Ht....
+000040c0: 3ef2 e23d 2865 3214 51ca 7e42 5b2c af2a  >..=(e2.Q.~B[,.*
+000040d0: b5dd 7573 8663 2f16 e5af 27e7 1803 153c  ..us.c/...'....<
+000040e0: 46ac ee33 0b70 5a51 a3e2 6dce 118a d0b1  F..3.pZQ..m.....
+000040f0: 7d9b db34 9de0 0f35 9da8 2fa7 00ba 02c7  }..4...5../.....
+00004100: 4ab0 154c 8424 d85a 157b a255 cd54 0c0a  J..L.$.Z.{.U.T..
+00004110: b80c 75e2 35ff 2dce 6829 7520 92c2 e517  ..u.5.-.h)u ....
+00004120: 161d 5246 b399 a400 2463 5b79 af47 dad6  ..RF....$c[y.G..
+00004130: 8ee0 b962 9e82 f264 f05a cec1 8b57 2d8f  ...b...d.Z...W-.
+00004140: bf0f 33af 73dd 6f98 7779 385a f16e 71d8  ..3.s.o.wy8Z.nq.
+00004150: f034 7857 a238 2478 1d79 0bb4 3a91 773c  .4xW.8$x.y..:.w<
+00004160: 91c0 7220 9211 1f14 25a1 1bd4 c21e a5cc  ..r ....%.......
+00004170: e8df 61cf 5f3d ece9 4e61 9657 46e1 c640  ..a._=..Na.WF..@
+00004180: f281 3ec4 c96b ee80 e4c1 f139 2402 2045  ..>..k.....9$. E
+00004190: a99d 1330 6190 5515 09a2 0e8d dd47 4075  ...0a.U......G@u
+000041a0: 777c 14a6 a2e2 9180 050b 2093 c95d 8bcb  w|........ ..]..
+000041b0: 4d0c a9be 46f4 7392 432f a155 f45b ca78  M...F.s.C/.U.[.x
+000041c0: afc3 4da9 e772 9bee c0b1 e19a d86d 4916  ..M..r.......mI.
+000041d0: 8da0 c827 785a d8a1 1e8e 5751 441b e402  ...'xZ....WQD...
+000041e0: 2243 ed7d 8220 36c4 50b6 8b88 0689 7bc8  "C.}. 6.P.....{.
+000041f0: 6aa4 5296 bd0d 7519 2750 f760 853e e6b2  j.R...u.'P.`.>..
+00004200: 41b4 c633 8743 ebdc 065e 8240 4286 de79  A..3.C...^.@B..y
+00004210: 97a0 50fb 0524 8589 d2d0 8b2c 400c 2066  ..P..$.....,@. f
+00004220: 8ea3 6132 dfef bd30 1069 cde1 173f d05d  ..a2...0.i...?.]
+00004230: 9c06 6c5d 2dcf 6e0c aeff 81a6 3ccd 0549  ..l]-.n.....<..I
+00004240: edc1 fdf0 2a64 53fe 8720 3e9e 5f9e e448  ....*dS.. >._..H
+00004250: fcd9 515e c7cd 6515 8c52 772c 8fc8 04e4  ..Q^..e..Rw,....
+00004260: a513 e6a3 140a 6484 e210 cbff ad39 6a69  ......d......9ji
+00004270: 8ac3 9ae3 1a92 5d90 3bd0 5000 f9eb e17b  ......].;.P....{
+00004280: 9c42 727d f08d bc90 30fc 56c3 280c 21bc  .Br}....0.V.(.!.
+00004290: cb40 bda4 a09f 0e60 dc67 9b38 09b2 57ed  .@.....`.g.8..W.
+000042a0: 3a08 21d5 3984 120c 160a e387 fd81 d76e  :.!.9..........n
+000042b0: 4127 42ca 0772 2a43 c8ce f724 38c4 13e4  A'B..r*C...$8...
+000042c0: d103 2af5 8665 1b0f d093 ab66 aea6 7fde  ..*..e.....f....
+000042d0: 0704 4115 7690 34a1 4c41 0586 ca8a 5a59  ..A.v.4.LA....ZY
+000042e0: 6716 c6e6 2280 cce8 2015 f714 f291 602c  g..."... .....`,
+000042f0: be29 d556 d657 4b65 067d 0587 12c1 1250  .).V.WKe.}.....P
+00004300: a9c5 44bf 4c3d 0923 bdd7 5455 c77a 05a7  ..D.L=.#..TU.z..
+00004310: 27a0 7aca a655 cca4 a0c5 7b71 b483 a603  '.z..U....{q....
+00004320: 79ba 5e4c 9f23 0a55 8da2 da89 a381 f270  y.^L.#.U.......p
+00004330: c528 0509 19c4 7312 b31a 45eb 9343 4f9e  .(....s...E..CO.
+00004340: f2f8 3c0c 93cb e125 b72c 30d5 87ee 93cc  ..<....%.,0.....
+00004350: ad3a 9223 a4a8 0ef8 ffad 99c8 1b92 cafc  .:.#............
+00004360: 1553 405b 1cc3 9406 0eb9 56d4 bbd4 d7c3  .S@[......V.....
+00004370: 01d1 ab50 6dde 3a6e f315 78df be8b 37be  ...Pm.:n..x...7.
+00004380: b10c 967c 7452 5f46 c528 e884 3c24 250d  ...|tR_F.(..<$%.
+00004390: b83e 0ed5 5efb 7a24 a3d5 5052 ed5d a126  .>..^.z$..PR.].&
+000043a0: 22f3 af03 d311 baa3 03fa eb61 52b3 65a6  "..........aR.e.
+000043b0: e291 427a 5de6 511b d111 2c6a 037f 5d2a  ..Bz].Q...,j..]*
+000043c0: 566e eaa9 38a4 9043 6f2a d03a a223 38d4  Vn..8..Co*.:.#8.
+000043d0: 6c4c fa9a 4c73 3777 1472 7e4d c03e 0553  lL..Ls7w.r~M.>.S
+000043e0: 7fef 5b54 c4ed f6ae 4a8c 545d e32e 1c2a  ..[T....J.T]...*
+000043f0: 12d4 0577 220f 3f46 8f51 fc7c 4ac5 5aa1  ...w".?F.Q.|J.Z.
+00004400: 6fad e490 dded e565 e825 8ee2 6dd1 b922  o......e.%..m.."
+00004410: 5246 b208 29ad 5160 b966 6df0 a243 46be  RF..).Q`.fm..CF.
+00004420: b437 5be8 40ce 1b29 21ad 2477 ecf0 475a  .7[.@..)!.$w..GZ
+00004430: f9ac 2b5f c47b eb6f a025 fe3f b3bc 4f4f  ..+_.{.o.%.?..OO
+00004440: 678d 7ad0 384e b0ce 5af5 74b9 57ef bf3c  g.z.8N..Z.t.W..<
+00004450: ed55 10c4 d3c8 526f 4a9a ee18 266f e1cf  .U....RoJ...&o..
+00004460: 660e 7575 e4ce 6ddd 3117 aeee da64 a97b  f.uu..m.1....d.{
+00004470: ee02 9bee c231 cc25 5837 489f 0127 b677  .....1.%X7H..'.w
+00004480: 146a ccd0 eeec 2e4d 0713 5b9f cd97 54f7  .j.....M..[...T.
+00004490: a96b e8ec 1b7d 49e6 96e9 fb4b dfcb 6120  .k...}I....K..a 
+000044a0: 1900 f90f 06e2 7b68 e6f8 9ead 639b 9a00  ......{h....c...
+000044b0: b234 75b4 58cc 758c 1c6f ee9a ce12 3bac  .4u.X.u..o....;.
+000044c0: a51a ad60 8ca1 d641 93c2 657d 8e13 8682  ...`...A..e}....
+000044d0: 27dc 4734 81f3 56ec 1d86 dea2 64db ec20  '.G4..V.....d.. 
+000044e0: 946b f9e6 e48d e8eb 3bb5 cf6f 3854 7bd7  .k......;..o8T{.
+000044f0: d7d9 5809 e8b1 4e67 3fc6 8e0b cd72 3ac0  ..X...Ng?....r:.
+00004500: ce9e 26a5 5adf 6e3f deaf c79e 7674 7756  ..&.Z.n?....vtwV
+00004510: 8c54 704a e50d 77e2 3ac2 aa76 c2ff 9949  .TpJ..w.:..v...I
+00004520: 8223 4aad 4a43 19da dfa5 d6bf 7aa9 b5de  .#J.JC......z...
+00004530: a85d 5d1d 85a8 1f40 b9c5 d478 a7b7 06ad  .]]....@...x....
+00004540: de50 aa0a f75b d6b0 8f56 ad7b 1342 c61c  .P...[...V.{.B..
+00004550: 4c17 8159 bea5 415c 9d12 174c d76c eeeb  L..Y..A\...L.l..
+00004560: c89a d9ba 61cd e678 36b7 30f6 b130 5df5  ....a..x6.0..0].
+00004570: 0465 93d0 7413 3f73 2bbb 9e14 9de6 9056  .e..t.?s+......V
+00004580: 81a9 3258 fb99 7a8a 7359 03f6 44bd e752  ..2X..z.sY..D..R
+00004590: 2ad1 dec6 f1e3 7e77 5ca1 b6ea d9ca a1bb  *.....~w\.......
+000045a0: 3bcc 864b b77f 424b e511 daa5 d110 cdac  ;..K..BK........
+000045b0: 3ab4 798b ba6c ca67 f860 faf0 117c a1d6  :.y..l.g.`...|..
+000045c0: 4064 4275 79c0 f080 0242 c5a0 63ad 077e  @dBuy....B..c..~
+000045d0: 1f49 5df0 5e18 e3c7 b23d fe1f d0e4 9fb7  .I].^....=......
+000045e0: 9cb7 facd c753 39aa d33e 383c aea8 0751  .....S9..>8<...Q
+000045f0: 9af1 924a de25 4faa 2ef9 dd3e 0939 2709  ...J.%O....>.9'.
+00004600: 9ee6 5c4a a7e6 9939 2d3a ea09 663e 5bd5  ..\J...9-:..f>[.
+00004610: a32f 03f0 27e5 9b31 f431 1fe8 be2f eee2  ./..'..1.1.../..
+00004620: 34f6 aa5e c7f6 a860 7eee 03b4 8949 8122  4..^...`~....I."
+00004630: c753 ae4a 585d 1c06 8e13 caf7 94cf 134c  .S.JX].........L
+00004640: 81b1 e9f4 0fd8 2174 fbdb 53c3 991a d694  ......!t..S.....
+00004650: e033 f0b0 aaf2 8e12 15c5 863f c7f2 1c57  .3.........?...W
+00004660: 9d86 7a1b 3adb 863c 6f22 2ef8 e5fd a7c6  ..z.:..<o"......
+00004670: 83b2 8427 3588 e473 8fed 970b 4dd5 379f  ...'5..s....M.7.
+00004680: 48f0 0a83 af01 1d03 03fd aaa6 5415 cbe7  H...........T...
+00004690: 2cb9 7b9c cb8a c0c0 6647 6a2d 9e75 2fb9  ,.{.....fGj-.u/.
+000046a0: 2a3c d631 ac02 e87e cfd8 ecc9 9114 8826  *<.1...~.......&
+000046b0: d6da 2cf4 c0f2 1ddd e555 75df 14c5 f65a  ..,......Uu....Z
+000046c0: 6095 37cd 6bbc 9adf 4b7c 1664 5033 1cda  `.7.k...K|.dP3..
+000046d0: b7d4 4420 66d1 6bab dc73 f85e f4e9 9e3b  ..D f.k..s.^...;
+000046e0: d3e3 182b 1561 8e43 2038 fb28 42a8 e1d8  ...+.a.C 8.(B...
+000046f0: a7cd d6de bd84 287a d883 ee1e 430b b4be  ......(z....C...
+00004700: 147d 59f2 fc6c 5dc2 1468 113b cb07 f587  .}Y..l]..h.;....
+00004710: 8fad d5bf dcda 9840 96d0 a780 35f0 1c89  .......@....5...
+00004720: adbc 9751 14b3 b680 382a be29 a643 8a2f  ...Q....8*.).C./
+00004730: b59e 3ff7 6cbe 464c e2b0 9e07 c6a2 940f  ..?.l.FL........
+00004740: e440 9793 4713 369e 93a2 27f8 2e4e b482  .@..G.6...'..N..
+00004750: c8f4 4c63 f33b 68b7 2bda 8934 4002 7dbe  ..Lc.;h.+..4@.}.
+00004760: 3be8 4062 e56f 0d8c adb6 dfc1 cf0c b026  ;.@b.o.........&
+00004770: 0a3e c223 9640 3ee8 2f8d 22bc 2991 9d7d  .>.#.@>./.".)..}
+00004780: ff5d 1769 221a 6eee 427c 8b6a bb3d 3c99  .].i".n.B|.j.=<.
+00004790: 13b2 f955 f839 0936 9976 c1ba f24e 3afd  ...U.9.6.v...N:.
+000047a0: 9ace dae6 6847 89a3 18a8 61fd 1cfb 51f7  ....hG....a...Q.
+000047b0: 4369 7050 181d 2116 27fd 10c3 f00c d9a1  CipP..!.'.......
+000047c0: 684d c159 fa9c b378 e5fc a1c2 cf32 e4bc  hM.Y...x.....2..
+000047d0: a99b 5136 1503 d731 7fd6 6aa2 5cd5 e72a  ..Q6...1..j.\..*
+000047e0: ca51 b022 df53 1bac a8c9 1bcf f314 ef37  .Q.".S.........7
+000047f0: 962e a0a5 998a b1b0 1d93 f7ad 9541 7e6a  .............A~j
+00004800: fb60 9fdb b3a7 3db4 0abd d539 40b2 62d3  .`....=....9@.b.
+00004810: 75d0 2534 b4d5 9ee1 1146 d191 c0f5 4111  u.%4.....F....A.
+00004820: 75f0 8bab cbf3 348d 7100 2a8f fc04 ce43  u.....4.q.*....C
+00004830: f63a fab8 0157 8ea1 5fb9 48e3 3a4c 8dc9  .:...W.._.H.:L..
+00004840: 6c6d 1e04 3c2d ef0b 284a f801 0848 218a  lm..<-..(J...H!.
+00004850: 05ca 5f4f c9b9 5bbe 978b d210 9c32 c8dd  .._O..[......2..
+00004860: 6b0a 1397 37b9 ffcf 9654 062d 580a a6a8  k...7....T.-X...
+00004870: 0f4e 49cc aa7d 0849 69ee be34 d3f5 03ef  .NI..}.Ii..4....
+00004880: 6747 134d 35ef 741c 860e de8c a4a5 c92a  gG.M5.t........*
+00004890: 4534 753d 5549 de58 5525 387b 9ac2 1238  E4u=UI.XU%8{...8
+000048a0: 0a81 f940 7d9a b09f 4469 5845 15d5 9763  ...@}...DiXE...c
+000048b0: 22ac 4d4c 36d3 c7c0 420a 7b34 2cf3 aec7  ".ML6...B.{4,...
+000048c0: aecb 8a15 6361 a144 3d0c fb19 9475 c749  ....ca.D=....u.I
+000048d0: 17fe a9ba daec 3dea d1a8 d859 8f07 86c3  ......=....Y....
+000048e0: 1e0f 0ca7 3d1e 188e 7b3c 309c f7f1 c0a2  ....=...{<0.....
+000048f0: 8a34 f6a2 3368 f591 d243 366a 84b3 5012  .4..3h...C6j..P.
+00004900: 70ca 0eb8 5539 fe9e f1b5 9bb9 852f e111  p...U9......./..
+00004910: b185 048d e3ce 978d cd1e 84e4 caa0 9c6a  ...............j
+00004920: 9b76 fd34 de9b ff01 0000 ffff 0300 504b  .v.4..........PK
+00004930: 0304 1400 0600 0800 0000 2100 af39 1aeb  ..........!..9..
+00004940: d401 0000 ba04 0000 1800 2800 6375 7374  ..........(.cust
+00004950: 6f6d 586d 6c2f 6974 656d 5072 6f70 7334  omXml/itemProps4
+00004960: 2e78 6d6c 20a2 2400 28a0 2000 0000 0000  .xml .$.(. .....
+00004970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004980: 0000 0000 0000 0000 0000 0000 b494 6f6b  ..............ok
+00004990: db30 10c6 df0f f61d 82de 2bf2 bfd8 5669  .0........+...Vi
+000049a0: 52d2 b481 c20a 63eb a06f cfd2 2931 b324  R.....c..o..)1.$
+000049b0: 2329 cbc6 d877 9fec 768c ae09 d958 fb4a  #)...w..v....X.J
+000049c0: 9ccc dd73 f7f8 773a bff8 aabb c917 74be  ...s..w:......t.
+000049d0: b566 4ed2 6942 2668 8495 add9 ccc9 a7bb  .fN.iB&h........
+000049e0: 35ad c9c4 0730 123a 6b70 4e8c 2517 8bb7  5....0.:kpN.%...
+000049f0: 6fce a53f 9310 c007 ebf0 26a0 9ec4 8b36  o..?......&....6
+00004a00: 9e37 5773 f2fd 322d 9655 be2a e8f5 72cd  .7Ws..2-.U.*..r.
+00004a10: 6951 acd6 7459 f135 cd2f 7916 cf75 9524  iQ..tY.5./y..u.$
+00004a20: d73f c824 4a9b 58c6 cfc9 3684 fe8c 312f  .?.$J.X...6...1/
+00004a30: b6a8 c14f 6d8f 267e 54d6 6908 3174 1b66  ...Om.&~T.i.1t.f
+00004a40: 956a 055e 59b1 d368 02cb 92a4 6462 17e5  .j.^Y..h....db..
+00004a50: f5bd eec8 62e8 e721 fb03 2aff 341c 5adb  ....b..!..*.4.Z.
+00004a60: b9f6 998a 6e85 b3de aa30 1556 3f0a 3c14  ....n....0.V?.<.
+00004a70: d618 6098 8e09 6b42 94bb fbd6 2361 2f56  ..`...kB....#a/V
+00004a80: b577 7140 175a f46c 505a 86e0 da66 17d0  .wq@.Z.lPZ...f..
+00004a90: 9fd2 d8ef f7d3 7d3e fa11 0d48 d9fd edbb  ......}>...H....
+00004aa0: 8fa3 65af d2dc d1a2 7596 63c2 0169 294a  ..e.....u.c..i)J
+00004ab0: 418b 0432 5a27 39a7 69c6 799d cc94 cc15  A..2Z'9.i.y.....
+00004ac0: 3f9e 0ca2 e04d 2969 5522 d202 3241 41aa  ?....M)iU"..2AA.
+00004ad0: 8c16 92d7 0035 944d 7adc eb8c 6732 9122  .....5.Mz...g2."
+00004ae0: a338 e311 2c04 4e9b 192a 9ae7 8d92 55d4  .8..,.N..*....U.
+00004af0: 9f89 eaff bd90 8f94 dd82 810d 8ebc 8548  ...............H
+00004b00: c0c9 dff3 0bdf 8360 b546 d91e c276 20ac  .......`.F...v .
+00004b10: 62ef c105 836e 15f9 72b6 fbeb ca07 16a3  b....n..r.......
+00004b20: 07f1 3976 f90c 5c87 f437 67a7 3ce9 77ae  ..9v..\..7g.<.w.
+00004b30: 1bb1 9282 6137 8eec 593a 4dd9 bf24 0674  ....a7..Y:M..$.t
+00004b40: da9f cc38 6c52 1bf7 cc19 e898 6de4 a0c9  ...8lR......m...
+00004b50: fed8 e721 7ef2 de2c 7e02 0000 ffff 0300  ...!~..,~.......
+00004b60: 504b 0304 1400 0600 0800 0000 2100 1599  PK..........!...
+00004b70: 551d 4f01 0000 6602 0000 1100 0801 646f  U.O...f.......do
+00004b80: 6350 726f 7073 2f63 6f72 652e 786d 6c20  cProps/core.xml 
+00004b90: a204 0128 a000 0100 0000 0000 0000 0000  ...(............
+00004ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004c80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004c90: 0000 0000 0000 008c 9251 4bc3 3014 85df  .........QK.0...
+00004ca0: 05ff 43c9 b36d d26e 130d 6d07 4ef6 e460  ..C..m.n..m.N..`
+00004cb0: 6045 f12d 2477 5bb0 4d43 12ed faef 4ddb  `E.-$w[.MC....M.
+00004cc0: ad76 e883 9097 dc7b ee97 732e 4997 c7aa  .v.....{..s.I...
+00004cd0: 0cbe c058 59ab 0cc5 1141 0128 5e0b a9f6  ...XY....A.(^...
+00004ce0: 197a 29d6 e11d 0aac 634a b0b2 5690 a116  .z).....cJ..V...
+00004cf0: 2c5a e6d7 5729 d794 d706 b6a6 d660 9c04  ,Z..W).......`..
+00004d00: 1b78 92b2 94eb 0c1d 9cd3 1463 cb0f 5031  .x.........c..P1
+00004d10: 1b79 85f2 cd5d 6d2a e6fc d5ec b166 fc83  .y...]m*.....f..
+00004d20: ed01 2784 dce2 0a1c 13cc 31dc 0143 3d12  ..'.......1..C=.
+00004d30: d109 29f8 88d4 9fa6 ec01 8263 28a1 02e5  ..)........c(...
+00004d40: 2c8e a318 ff68 1d98 cafe 39d0 7726 ca4a  ,....h....9.w&.J
+00004d50: ba56 fb4c 27bb 53b6 e043 7354 1fad 1c85  .V.L'.S..CsT....
+00004d60: 4dd3 44cd acb7 e1fd c7f8 6df3 f4dc 470d  M.D.......m...G.
+00004d70: a5ea 76c5 01e5 a9e0 941b 60ae 3679 975f  ..v.......`.6y._
+00004d80: b7c7 32c5 9362 b7c0 9259 b7f1 bbde 4910  ..2..b...Y....I.
+00004d90: 0f6d be35 d2cf de04 ab83 9136 c5bf 051e  .m.5.......6....
+00004da0: da67 18c8 2002 ef8a 0e19 ce9d d7d9 eab1  .g.. ...........
+00004db0: 58a3 3c21 c93c 24dd 2962 4267 0b4a eedf  X.<!.<$.)bBg.J..
+00004dc0: bbf7 2fe6 3b97 43a1 3ab9 f807 314e 8a78  ../.;.C.:...1N.x
+00004dd0: 4e17 842e 9209 f10c c87b df97 3f23 ff06  N........{..?#..
+00004de0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+00004df0: 0000 2100 290f f5c6 7d01 0000 fe02 0000  ..!.)...}.......
+00004e00: 1000 0801 646f 6350 726f 7073 2f61 7070  ....docProps/app
+00004e10: 2e78 6d6c 20a2 0401 28a0 0001 0000 0000  .xml ...(.......
+00004e20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004e30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004e40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004e50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004e60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004e70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004e80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004e90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004ea0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004eb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ec0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ed0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ee0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004ef0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00004f00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00004fb0: 0000 0000 0000 0000 0084 cfc1 6ac3 300c  ............j.0.
-00004fc0: 06e0 7ba1 ef60 745f 9cf6 304a 89d3 4b19  ..{..`t_..0J..K.
-00004fd0: e436 460b bd1a 4749 4c63 cb58 4a69 df7e  .6F...GILc.XJi.~
-00004fe0: a6a7 1606 3b4a 42df 2f35 877b 98d5 0d33  ....;JB./5.{...3
-00004ff0: 7b8a 0636 550d 0aa3 a3de c7d1 c0f9 f4f5  {..6U...........
-00005000: b103 c562 636f 678a 68e0 810c 8776 bd6a  ...bcog.h....v.j
-00005010: 7e70 b652 9678 f289 5551 221b 9844 d25e  ~p.R.x..UQ"..D.^
-00005020: 6b76 1306 cb15 258c 6532 500e 564a 9947  kv....%.e2P.VJ.G
-00005030: 9dac bbda 11f5 b6ae 3f75 7e35 a07d 3355  ........?u~5.}3U
-00005040: d71b c85d bf01 757a a492 fcbf 4dc3 e01d  ...]..uz....M...
-00005050: 1ec9 2d01 a3fc 11a1 ddc2 42e1 12e6 ef4c  ..-.......B....L
-00005060: 898b 6cf3 8862 c00b 8667 6b5b 957b 41b7  ..l..b...gk[.{A.
-00005070: 8d7e fbaf fd05 0000 ffff 0300 504b 0304  .~..........PK..
-00005080: 1400 0600 0800 0000 2100 7bf3 02a3 c300  ........!.{.....
-00005090: 0000 2801 0000 1e00 0801 6375 7374 6f6d  ..(.......custom
-000050a0: 586d 6c2f 5f72 656c 732f 6974 656d 332e  Xml/_rels/item3.
-000050b0: 786d 6c2e 7265 6c73 20a2 0401 28a0 0001  xml.rels ...(...
-000050c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000050d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00004f10: 0000 0000 0000 0000 0000 0000 9c92 cb4e  ...............N
+00004f20: c330 1045 f748 fc43 e43d 750a 08a1 ca31  .0.E.H.C.=u....1
+00004f30: 423c c402 44a5 1658 1b67 d258 b876 e419  B<..D..X.g.X.v..
+00004f40: a296 af67 9288 9202 2b76 f3b8 ba3e beb6  ...g....+v...>..
+00004f50: bad8 ac7d d642 4217 4321 a693 5c64 106c  ...}.BB.C!..\d.l
+00004f60: 2c5d 5815 e269 797b 742e 3224 134a e363  ,]X..iy{t.2$.J.c
+00004f70: 8042 6c01 c585 3e3c 50f3 141b 48e4 0033  .Bl...><P...H..3
+00004f80: b608 5888 9aa8 9949 89b6 86b5 c109 af03  ..X....I........
+00004f90: 6faa 98d6 86b8 4d2b 19ab ca59 b88e f67d  o.....M+...Y...}
+00004fa0: 0d81 e471 9e9f 49d8 1084 12ca a366 6728  ...q..I......fg(
+00004fb0: 06c7 594b ff35 2da3 edf8 f079 b96d 1858  ..YK.5-....y.m.X
+00004fc0: abcb a6f1 ce1a e25b ea07 6753 c458 5176  .......[..gS.XQv
+00004fd0: b3b1 e095 1c2f 15d3 2dc0 be27 475b 9d2b  ...../..-..'G[.+
+00004fe0: 396e d5c2 1a0f 576c ac2b e311 94fc 1ea8  9n....Wl.+......
+00004ff0: 3b30 5d68 73e3 126a d5d2 ac05 4b31 65e8  ;0]hs..j....K1e.
+00005000: 3e38 b663 91bd 1a84 0ea7 10ad 49ce 0462  >8.c........I..b
+00005010: ac4e 3634 7ded 1ba4 a45f 627a c31a 8050  .N64}...._bz...P
+00005020: 4916 0cc3 be1c 6bc7 b53b d5d3 5ec0 c5be  I.....k..;..^...
+00005030: b033 1840 78b1 8fb8 74e4 011f abb9 49f4  .3.@x...t.....I.
+00005040: 07f1 744c dc33 0cbc 03ce a2e3 1bce 1cf3  ..tL.3..........
+00005050: f557 e693 7e78 dfbb f086 4fcd 325e 1b82  .W..~x....O.2^..
+00005060: afec f687 6a51 9b04 25c7 bdcb 7637 5077  ....jQ..%...v7Pw
+00005070: 1c5b f29d c955 6dc2 0aca 2fcd ef45 f7d2  .[...Um.../..E..
+00005080: cfc3 77d6 d3b3 497e 92f3 238e 664a 7e7f  ..w...I~..#.fJ~.
+00005090: 5cfd 0900 00ff ff03 0050 4b03 0414 0006  \........PK.....
+000050a0: 0008 0000 0021 0029 e752 8d5a 0100 00b3  .....!.).R.Z....
+000050b0: 0200 0013 0008 0164 6f63 5072 6f70 732f  .......docProps/
+000050c0: 6375 7374 6f6d 2e78 6d6c 20a2 0401 28a0  custom.xml ...(.
+000050d0: 0001 0000 0000 0000 0000 0000 0000 0000  ................
 000050e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000050f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005190: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000051a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000051b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000051c0: 84cf c16a c330 0c06 e07b 61ef 6074 5f9c  ...j.0...{a.`t_.
-000051d0: 7430 4a89 d3cb 28e4 3646 07bb 1a47 71cc  t0J...(.6F...Gq.
-000051e0: 62cb 58ea 58df 7ea6 a716 063d 4a42 df2f  b.X.X.~....=JB./
-000051f0: f587 dfb8 aa1f 2c1c 2819 e89a 1614 2647  ......,.(.....&G
-00005200: 5348 dec0 e7e9 f8bc 03c5 62d3 6457 4a68  SH........b.dWJh
-00005210: e082 0c87 e169 d37f e06a a52e f112 32ab  .....i...j....2.
-00005220: aa24 36b0 88e4 bdd6 ec16 8c96 1bca 98ea  .$6.............
-00005230: 64a6 12ad d4b2 789d adfb b61e f5b6 6d5f  d.....x.......m_
-00005240: 75b9 3560 b833 d538 1928 e3d4 813a 5d72  u.5`.3.8.(...:]r
-00005250: 4d7e 6cd3 3c07 876f e4ce 1193 fc13 a1dd  M~l.<..o........
-00005260: 9985 e257 5cdf 0b65 aeb2 2d1e c540 108c  ...W\..e..-..@..
-00005270: d7d6 4b53 ef05 3df4 faee bfe1 0f00 00ff  ..KS..=.........
-00005280: ff03 0050 4b03 040a 0000 0000 0000 0021  ...PK..........!
-00005290: 00ff ffff ffe2 0100 00e2 0100 0010 0000  ................
-000052a0: 005b 7472 6173 685d 2f30 3030 312e 6461  .[trash]/0001.da
-000052b0: 74ff ffff ff00 0000 0000 0000 0000 0000  t...............
-000052c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000052d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000052e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000052f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000051c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000051d0: 0000 b492 5f4b c330 14c5 df05 bf43 c97b  ...._K.0.....C.{
+000051e0: d6fc 69d7 75b4 1d5b b74a 1f04 c1e9 eb08  ..i.u..[.J......
+000051f0: 49b6 159a a434 5975 88df dd0c 9dba 075f  I....4Yu......._
+00005200: 14f3 74c3 bd9c f33b 37c9 66cf aa0d 06d9  ..t....;7.f.....
+00005210: dbc6 e81c e011 0281 d4dc 8846 ef72 f0b0  ...........F.r..
+00005220: aee0 0404 d631 2d58 6bb4 ccc1 515a 302b  .....1-Xk...QZ0+
+00005230: aeaf b2bb de74 b277 8db4 8197 d036 077b  .....t.w.....6.{
+00005240: e7ba 6918 5abe 978a d991 6f6b dfd9 9a5e  ..i.Z.....ok...^
+00005250: 31e7 affd 2e34 db6d c3e5 d2f0 8392 da85  1....4.m........
+00005260: 04a1 71c8 0fd6 1905 bb4f 39f0 ae37 1ddc  ..q......O9..7..
+00005270: 6f25 85e1 273a fbb8 3e76 1eb7 c83e c48f  o%..':..>v...>..
+00005280: c156 b946 e4e0 6519 97cb 658c 6248 5669  .V.F..e...e.bHVi
+00005290: 0931 c20b 98d2 3481 6882 1059 90b2 4ae7  .1....4.h..Y..J.
+000052a0: ab57 1074 a761 0202 cd94 8f7e 2b45 c3ee  .W.t.a.....~+E..
+000052b0: 653f f80c b562 3bb9 66bb 93fa e0a6 6df7  e?...b;.f.....m.
+000052c0: 645d 5f64 e1f7 faec fa47 7f7a f62f 8d76  d]_d.....G.z./.v
+000052d0: 7e6d a750 b5b8 f045 cfc8 6740 8896 d584  ~m.P...E..g@....
+000052e0: d064 5c52 8a17 38c2 737f 4844 e7ab 2a4d  .d\R..8.s.HD..*M
+000052f0: c838 a1ff c217 9df9 36a2 e51b ffb8 b5a8  .8......6.......
+00005300: 9d54 3787 e612 5250 8409 a331 e41e 1446  .T7...RP...1...F
+00005310: 298f 61ca 62bf 7349 05c5 5246 1ca3 9f00  ).a.b.sI..RF....
+00005320: c3af df56 bc01 0000 ffff 0300 504b 0304  ...V........PK..
+00005330: 1400 0600 0800 0000 2100 743f 397a c200  ........!.t?9z..
+00005340: 0000 2801 0000 1e00 0801 6375 7374 6f6d  ..(.......custom
+00005350: 586d 6c2f 5f72 656c 732f 6974 656d 312e  Xml/_rels/item1.
+00005360: 786d 6c2e 7265 6c73 20a2 0401 28a0 0001  xml.rels ...(...
 00005370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000053a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000053b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000053c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000053d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -1345,475 +1345,215 @@
 00005400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005440: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005490: 0000 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-000054a0: 0034 50cf 2bb9 0000 00c9 0000 0018 0028  .4P.+..........(
-000054b0: 0063 7573 746f 6d58 6d6c 2f69 7465 6d50  .customXml/itemP
-000054c0: 726f 7073 342e 786d 6c20 a224 0028 a020  rops4.xml .$.(. 
-000054d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000054e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000054f0: 000c 8dc1 8ac2 3014 45f7 03fe 4378 fb98  ......0.E...Cx..
-00005500: b496 4e15 5369 ab05 f70e cc36 a4af b6d0  ..N.Si.....6....
-00005510: bc27 4d94 81c1 7f37 abcb bd07 ee39 9efe  .'M....7.....9..
-00005520: fc22 5eb8 8699 c940 b6d5 2090 1c0f 33dd  ."^....@.. ...3.
-00005530: 0dfc dc7a 5981 08d1 d260 1726 3440 0ca7  ...zY....`.&4@..
-00005540: 7af3 751c c261 b0d1 86c8 2b5e 237a 9186  z.u..a....+^#z..
-00005550: 39e5 f56c e07f 5755 4ddb eb42 765d 97c9  9..l..WUM..Bv]..
-00005560: 226f 7bb9 ffce 1a99 e74d a9fb 4297 eda5  "o{......M..B...
-00005570: 7d83 486a 4a37 c1c0 14e3 e3a0 5470 137a  }.HjJ7......Tp.z
-00005580: 1bb6 fc40 4a70 e4d5 db98 ea7a 573c 8eb3  ...@Jp.....zW<..
-00005590: c333 bba7 478a 2ad7 ba54 ee99 f4fe d72f  .3..G.*..T...../
-000055a0: a0ea 0f00 0000 ffff 0300 504b 0304 1400  ..........PK....
-000055b0: 0600 0800 0000 2100 29e7 528d 5c01 0000  ......!.).R.\...
-000055c0: b302 0000 1300 a600 646f 6350 726f 7073  ........docProps
-000055d0: 2f63 7573 746f 6d2e 786d 6c20 a2a2 0028  /custom.xml ...(
-000055e0: a000 0100 0000 0000 0000 0000 0000 0000  ................
+00005470: 84cf c18a 0231 0c06 e0bb e03b 94dc 9dce  .....1.....;....
+00005480: 7810 91e9 7859 16bc 89b8 e0b5 7432 33c5  x...xY......t23.
+00005490: 6953 9a28 faf6 164f 2b2c ec31 09f9 fea4  iS.(...O+,.1....
+000054a0: dd3f c2ac ee98 d953 34d0 5435 288c 8e7a  .?.....S4.T5(..z
+000054b0: 1f47 033f e7ef d516 148b 8dbd 9d29 a281  .G.?.........)..
+000054c0: 2732 ecbb e5a2 3de1 6ca5 2cf1 e413 aba2  '2....=.l.,.....
+000054d0: 4436 3089 a49d d6ec 260c 962b 4a18 cb64  D60.....&..+J..d
+000054e0: a01c ac94 328f 3a59 77b5 23ea 755d 6f74  ....2.:Yw.#.u]ot
+000054f0: fe6d 40f7 61aa 436f 201f fa06 d4f9 994a  .m@.a.Co ......J
+00005500: f2ff 360d 8377 f845 ee16 30ca 1f11 dadd  ..6..w.E..0.....
+00005510: 5828 5cc2 7ccc 94b8 c836 8f28 06bc 6078  X(\.|....6.(..`x
+00005520: b79a aadc 0bba 6bf5 c77f dd0b 0000 ffff  ......k.........
+00005530: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00005540: 5c96 2722 c300 0000 2801 0000 1e00 0801  \.'"....(.......
+00005550: 6375 7374 6f6d 586d 6c2f 5f72 656c 732f  customXml/_rels/
+00005560: 6974 656d 322e 786d 6c2e 7265 6c73 20a2  item2.xml.rels .
+00005570: 0401 28a0 0001 0000 0000 0000 0000 0000  ..(.............
+00005580: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005590: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000055a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000055b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000055c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000055d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000055e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000055f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005680: 00b4 925f 4bc3 3014 c5df 05bf 43c9 7bd6  ..._K.0.....C.{.
-00005690: fc69 d775 ac1d 5bbb 491f 04c1 e9eb 0849  .i.u..[.I......I
-000056a0: d615 9aa4 34d9 7488 dfdd 9439 710f be28  ....4.t....9q..(
-000056b0: e629 e15e cef9 9d7b 339b bfaa 3638 cade  .).^...{3...68..
-000056c0: 3646 6700 8f10 08a4 e646 34ba cec0 d366  6Fg......F4....f
-000056d0: 0d27 20b0 8e69 c15a a365 064e d282 797e  .' ..i.Z.e.N..y~
-000056e0: 7b33 7be8 4d27 7bd7 481b 7809 6d33 b077  {3{.M'{.H.x.m3.w
-000056f0: ae9b 86a1 e57b a998 1df9 b2f6 959d e915  .....{..........
-00005700: 73fe d9d7 a1d9 ed1a 2e4b c30f 4a6a 1712  s........K..Jj..
-00005710: 84c6 213f 5867 14ec bee4 c059 6f7a 74bf  ..!?Xg.....Yozt.
-00005720: 9514 860f 74f6 7973 ea3c 6e3e fb14 3f05  ....t.ys.<n>..?.
-00005730: 3be5 1a91 81b7 322e ca32 4631 24ab b480  ;.....2..2F1$...
-00005740: 18e1 254c 699a 4034 4188 2c49 b14e 17ab  ..%Li.@4A.,I.N..
-00005750: 7710 7443 3301 8166 ca47 bf97 a261 8fb2  w.tC3..f.G...a..
-00005760: 3ffa 0c95 62b5 dcb0 7a50 3fba 69db bd58  ?...b...zP?.i..X
-00005770: d7e7 b3f0 fbfd e2fa 477f 7af1 2f8c 767e  ........G.z./.v~
-00005780: 6c43 a84a 5cf9 a257 e433 2044 8bf5 84d0  lC.J\..W.3 D....
-00005790: 645c 508a 9738 c20b 7f48 4417 ab75 9a90  d\P..8...HD..u..
-000057a0: 7142 ff85 2fba f06d 45cb b77e b995 a89c  qB../..mE..~....
-000057b0: 5477 87e6 1a52 5084 09a3 31e4 1e14 4629  Tw...RP...1...F)
-000057c0: 8f61 ca62 3f73 4905 c552 461c a39f 00c3  .a.b?sI..RF.....
-000057d0: 619f e7df 967f 0000 00ff ff03 0050 4b03  a............PK.
-000057e0: 0414 0006 0008 0000 0021 000c c41a 92c3  .........!......
-000057f0: 0000 0028 0100 001e 0008 0163 7573 746f  ...(.......custo
-00005800: 6d58 6d6c 2f5f 7265 6c73 2f69 7465 6d34  mXml/_rels/item4
-00005810: 2e78 6d6c 2e72 656c 7320 a204 0128 a000  .xml.rels ...(..
-00005820: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+00005670: 0000 0000 0000 84cf c16a c330 0c06 e07b  .........j.0...{
+00005680: a1ef 6074 5f9c f630 4a89 d34b 19e4 3646  ..`t_..0J..K..6F
+00005690: 0bbd 1a47 494c 63cb 584a 69df 7ea6 a716  ...GILc.XJi.~...
+000056a0: 063b 4a42 df2f 3587 7b98 d50d 337b 8a06  .;JB./5.{...3{..
+000056b0: 3655 0d0a a3a3 dec7 d1c0 f9f4 f5b1 03c5  6U..............
+000056c0: 6263 6f67 8a68 e081 0c87 76bd 6a7e 70b6  bcog.h....v.j~p.
+000056d0: 5296 78f2 8955 5122 1b98 44d2 5e6b 7613  R.x..UQ"..D.^kv.
+000056e0: 06cb 1525 8c65 3250 0e56 4a99 479d acbb  ...%.e2P.VJ.G...
+000056f0: da11 f5b6 ae3f 757e 35a0 7d33 55d7 1bc8  .....?u~5.}3U...
+00005700: 5dbf 0175 7aa4 92fc bf4d c3e0 1d1e c92d  ]..uz....M.....-
+00005710: 01a3 fc11 a1dd c242 e112 e6ef 4c89 8b6c  .......B....L..l
+00005720: f388 62c0 0b86 676b 5b95 7b41 b78d 7efb  ..b...gk[.{A..~.
+00005730: affd 0500 00ff ff03 0050 4b03 0414 0006  .........PK.....
+00005740: 0008 0000 0021 007b f302 a3c3 0000 0028  .....!.{.......(
+00005750: 0100 001e 0008 0163 7573 746f 6d58 6d6c  .......customXml
+00005760: 2f5f 7265 6c73 2f69 7465 6d33 2e78 6d6c  /_rels/item3.xml
+00005770: 2e72 656c 7320 a204 0128 a000 0100 0000  .rels ...(......
+00005780: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005790: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000057a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000057b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000057c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000057d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000057e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000057f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005800: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005820: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005830: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005840: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005850: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005860: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005870: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000058a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000058b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000058c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000058d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000058e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000058f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005920: 0084 cfc1 6ac3 300c 06e0 7b61 ef60 745f  ....j.0...{a.`t_
-00005930: 9c94 314a 89d3 cb28 e436 4607 bb1a 4771  ..1J...(.6F...Gq
-00005940: cc62 cb58 ea58 df7e a6a7 1606 3d4a 42df  .b.X.X.~....=JB.
-00005950: 2ff5 87df b8aa 1f2c 1c28 19e8 9a16 1426  /......,.(.....&
-00005960: 4753 48de c0e7 e9f8 bc03 c562 d364 574a  GSH........b.dWJ
-00005970: 68e0 820c 87e1 69d3 7fe0 6aa5 2ef1 1232  h.....i...j....2
-00005980: abaa 2436 b088 e4bd d6ec 168c 961b ca98  ..$6............
-00005990: ea64 a612 add4 b278 9dad fbb6 1ef5 b66d  .d.....x.......m
-000059a0: 5f75 b935 60b8 33d5 3819 28e3 d481 3a5d  _u.5`.3.8.(...:]
-000059b0: 724d 7e6c d33c 0787 6fe4 ce11 93fc 13a1  rM~l.<..o.......
-000059c0: dd99 85e2 575c df0b 65ae b22d 1ec5 4010  ....W\..e..-..@.
-000059d0: 8cd7 d64b 53ef 053d f4fa eebf e10f 0000  ...KS..=........
-000059e0: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-000059f0: 2100 c394 5cad 6c0e 0000 574f 0000 1300  !...\.l...WO....
-00005a00: 2800 6375 7374 6f6d 586d 6c2f 6974 656d  (.customXml/item
-00005a10: 332e 786d 6c20 a224 0028 a020 0000 0000  3.xml .$.(. ....
+00005870: 0000 0000 0000 0000 0000 0000 0084 cfc1  ................
+00005880: 6ac3 300c 06e0 7b61 ef60 745f 9c74 304a  j.0...{a.`t_.t0J
+00005890: 89d3 cb28 e436 4607 bb1a 4771 cc62 cb58  ...(.6F...Gq.b.X
+000058a0: ea58 df7e a6a7 1606 3d4a 42df 2ff5 87df  .X.~....=JB./...
+000058b0: b8aa 1f2c 1c28 19e8 9a16 1426 4753 48de  ...,.(.....&GSH.
+000058c0: c0e7 e9f8 bc03 c562 d364 574a 68e0 820c  .......b.dWJh...
+000058d0: 87e1 69d3 7fe0 6aa5 2ef1 1232 abaa 2436  ..i...j....2..$6
+000058e0: b088 e4bd d6ec 168c 961b ca98 ea64 a612  .............d..
+000058f0: add4 b278 9dad fbb6 1ef5 b66d 5f75 b935  ...x.......m_u.5
+00005900: 60b8 33d5 3819 28e3 d481 3a5d 724d 7e6c  `.3.8.(...:]rM~l
+00005910: d33c 0787 6fe4 ce11 93fc 13a1 dd99 85e2  .<..o...........
+00005920: 575c df0b 65ae b22d 1ec5 4010 8cd7 d64b  W\..e..-..@....K
+00005930: 53ef 053d f4fa eebf e10f 0000 ffff 0300  S..=............
+00005940: 504b 0304 1400 0600 0800 0000 2100 0cc4  PK..........!...
+00005950: 1a92 c300 0000 2801 0000 1e00 0801 6375  ......(.......cu
+00005960: 7374 6f6d 586d 6c2f 5f72 656c 732f 6974  stomXml/_rels/it
+00005970: 656d 342e 786d 6c2e 7265 6c73 20a2 0401  em4.xml.rels ...
+00005980: 28a0 0001 0000 0000 0000 0000 0000 0000  (...............
+00005990: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000059a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000059b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000059c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000059d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000059e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000059f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005a00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005a10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00005a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00005a30: 0000 0000 0000 0000 0000 0000 00ec 1c6b  ...............k
-00005a40: 6fe3 36f2 7b81 fe07 c1f7 59b1 65f9 25a3  o.6.{.....Y.e.%.
-00005a50: de22 8fa6 0d9a ed2e 36d9 de7d 5bd0 2415  ."......6..}[.$.
-00005a60: eb22 4bae 24e7 81e2 fefb 0d49 91a2 9ea6  ."K.$......I....
-00005a70: e5b4 d816 6d81 3696 35c3 99e1 bc39 f477  ....m.6.5....9.w
-00005a80: dfbf 6c43 eb89 2669 1047 ab81 7336 1a58  ..lC..&i.G..s6.X
-00005a90: 34c2 3109 a287 d560 9ff9 f662 f0fd bbef  4.1....`...b....
-00005aa0: 70b6 c471 94d1 28bb 7fdd d13b bca1 5b64  p..q..(....;..[d
-00005ab0: c1c3 2fab c1c0 da22 f57f eda5 5fd0 96ae  ../...."...._...
-00005ac0: 0657 31de 6f01 8cbf a57d 7b73 b51a 8c5e  .W1.o....}{s...^
-00005ad0: 460e fc3b 722f af17 6377 3ebb 745d e7c2  F..;r/..cw>.t]..
-00005ae0: 9938 e7f0 cf78 e29e ff70 edcd c7b3 b95b  .8...x...p.....[
-00005af0: 85fd 5552 3b73 aa5f 5dd1 1427 c12e e3cc  ..UR;s._]..'....
-00005b00: 5c26 1465 d442 5644 9f2d 9213 7256 05b9  \&.e.BVD.-..rV..
-00005b10: c3f1 0e08 e58f 7339 30e2 f018 7b6b 7f4d  ......s90...{k.M
-00005b20: 171e 9e8e d618 218a 2633 e2f9 0b44 c96c  ......!.&3...D.l
-00005b30: e400 5120 b828 5de2 6c35 d864 d96e 391c  ..Q .(].l5.d.n9.
-00005b40: a65c 2ce9 d936 c049 9cc6 7e76 86e3 ed30  .\,..6.I..~v...0
-00005b50: f6fd 00d3 e178 349a 0db7 3443 0465 68a8  .....x4...4C.eh.
-00005b60: 4942 22da a23e 8876 0950 9f64 014d 39f2  IB"..>.v.P.d.M9.
-00005b70: f32c 4b82 f53e a3e9 e0dd b7df 7cf7 9292  .,K..>......|...
-00005b80: a5a0 caca 50f2 4033 b629 e90e 6160 f878  ....P.@3.)..a`.x
-00005b90: a28b b5b8 b092 3806 deb3 644f f947 3fa0  ......8...dO.G?.
-00005ba0: 2149 f9be 2234 76d1 c819 2f80 69ea 8ce7  !I.."4v.../.i...
-00005bb0: ce7c ee39 ee08 4d16 04d3 391a 5851 3a16  .|.9..M...9.XQ:.
-00005bc0: 2a13 a5ae fc63 22fe 1052 05c2 1585 cfcf  *....c"..R......
-00005bd0: cf67 cfee 599c 3c30 213a c3ff bcbf 150a  .g..Y.<0!:......
-00005be0: 2825 f792 9abf bb53 af1e b15b 3ae3 823e  (%.....S...[:..>
-00005bf0: 6060 3500 a5a5 230f 517b 8667 d89e 8cd0  ``5...#.Q{.g....
-00005c00: d85e 8c5c cf76 c69e b718 4d7d e2fa 9ea4  .^.\.v....M}....
-00005c10: 1118 0500 8427 de7a 46ec f98c 527b 82c6  .....'.zF...R{..
-00005c20: d846 c41f db13 e22d 105a a0d9 da01 59ca  .F.....-.Z....Y.
-00005c30: 1526 abc1 d81b 9311 c163 9b4e 3dcf 9e50  .&.......c.N=..P
-00005c40: e4d9 eb29 f56d d75d fb64 0eeb 4cf1 5c6d  ...).m.].d..L.\m
-00005c50: 74b0 ddc5 4966 45c5 161b 1138 948a d200  t...IfE....8....
-00005c60: 6f42 6f07 bc11 f90a 9e86 9479 0ace c06a  oBo........y...j
-00005c70: a0c9 5c12 08d6 b40b e90b f340 f251 4a7f  ..\........@.QJ.
-00005c80: db83 bb52 9fcb 38a4 cdbf 4711 7ae0 c895  ...R..8...G.z...
-00005c90: b01a 70a1 3094 6825 9a84 faab 0157 5612  ..p.0.h%.....WV.
-00005ca0: e22f e0cb 6e08 e87a 107d c078 9f80 d68d  ./..n..z.}.x....
-00005cb0: 0635 ea1b 403e 2761 0fa8 8fcc cba5 99f1  .5..@>'a........
-00005cc0: 8aee 52fa da2f 2fa3 d178 f485 c9c9 70dd  ..R..//..x....p.
-00005cd0: 4658 8804 46ac bacb 739c 054f a66b 8d97  FX..F...s..O.k..
-00005ce0: 771b 9450 f2ef 20db 7c4e 8149 c365 74b8  w..P.. .|N.I.et.
-00005cf0: 2bf0 a341 680e 798b d24c ac7a f1ca d634  +..Ah.y..L.z...4
-00005d00: 5e52 07bc 0fb6 a63c bacb f794 04e8 8e26  ^R.....<.......&
-00005d10: 4fe0 fbdf e75e df70 d532 f035 907e 1282  O....^.p.2.5.~..
-00005d20: 2b88 81f7 e891 46bd 963f df67 f13d 7a30  +.....F..?.g.=z0
-00005d30: 1575 99f6 0f97 9f7a 2d7a 1b63 c442 782f  .u.....z-z.c.Bx/
-00005d40: e01f 6944 130e de7b c37e 7802 3ff4 134a  ..iD...{.~x.?..J
-00005d50: 3797 31e9 b7e5 4c6c 3fd3 d78f 7110 65fd  7.1...Ll?...q.e.
-00005d60: 64d7 13fa 9646 0fd9 e626 baa3 9062 10f3  d....F...&...b..
-00005d70: a543 eccf 67be 339d 624a 2684 e0f5 64e4  .C..g.3.bJ&...d.
-00005d80: cd1d 77e2 fb2e 76dd b16f b815 93e5 3d7a  ..w...v..o....=z
-00005d90: b944 19de 9c87 a64e afa2 33eb ff52 9c81  .D.....N..3..R..
-00005da0: 81c3 7fe3 244f f5cc f9d0 edee 8ea2 046f  ....$O.........o
-00005db0: 3eaa 0ca9 8987 214b 9172 cfcf ffae 0406  >.....!K.r......
-00005dc0: fe2c 0f07 2c3a f0cf 7ad4 3107 e2d9 a18c  .,..,:..z.1.....
-00005dd0: 306d 5999 51c8 b672 82ae e364 7b45 7db4  0mY.Q..r...d{E}.
-00005de0: 0f21 11fb 6d8f c200 9230 8850 7f70 0e45  .!..m....0.P.p.E
-00005df0: b645 c275 388b aa07 e161 0691 09b6 5490  .E.u8....a....T.
-00005e00: b9c3 6629 5910 f9f1 0e65 1b96 04ce 871f  ..f)Y....e......
-00005e10: 5192 819d 5f42 5192 c410 09a4 5ceb 498c  Q..._BQ.....\.I.
-00005e20: 719e db4a a88a f1fd 9077 13ae 90cb 9c83  q..J.....w......
-00005e30: e56f abc1 173d e140 cb20 22f4 6535 9840  .o...=.@. ".e5.@
-00005e40: ea1c 8421 5a87 f08a cabc 4990 ee42 f45a  ...!Z.....I..B.Z
-00005e50: 2eb8 ac9b 2beb 5714 e6c9 39d1 eba2 fb0d  ....+.W...9.....
-00005e60: b59e d857 56ec 5b19 7c90 9c33 1894 a6c1  ...WV.[.|..3....
-00005e70: 4344 8995 c5f0 5d90 5a41 46b7 a268 025f  CD....].ZAF..h._
-00005e80: 4693 0885 62a1 0a85 506b 910f 51f8 9ad3  F...b...Pk..Q...
-00005e90: 25f7 2305 9985 544f d912 9a42 8d02 1943  %.#...TO...B...C
-00005ea0: 1c59 6b94 0223 a04f cb7b fa92 8964 4a58  .Yk..#.O.{...dJX
-00005eb0: 5809 ac6a 84cc 66db c425 922d 25b1 e951  X..j..f..%.-%..Q
-00005ec0: 1203 0f81 9625 5941 16b6 4511 4b4b c320  .....%YA..E.KK. 
-00005ed0: 7a54 4291 1213 82d9 0484 50a8 9ed5 8eb4  zTB.......P.....
-00005ee0: 494a 12d7 22ac 8aef 616c e68f 989e 0311  IJ.."...al......
-00005ef0: 52aa 202c 1ab1 8a5d 93e0 e74f b7ca 0a74  R. ,...]...O...t
-00005f00: 0755 1716 a782 d9a0 103d 6849 40ea 396a  .U.......=hI@.9j
-00005f10: 55d3 5a14 55ab b807 9640 ca56 647b 1c3d  U.Z.U....@.Vd{.=
-00005f20: d484 cf91 34fb 50c5 1363 52f7 aa1a effa  ....4.P..cR.....
-00005f30: 63a9 53c7 2887 9e53 2b15 99d5 a8e4 5aa0  c.S.(..S+.....Z.
-00005f40: 1b55 0e07 f651 d790 9f29 dd31 c381 cd40  .U...Q...).1...@
-00005f50: 841c a910 6582 5ad4 c2d4 862e e238 a428  ....e.Z......8.(
-00005f60: 3ac1 8cea 99b9 9292 63e0 7b04 b8c5 32fb  :.......c.{...2.
-00005f70: ba9c f893 b261 342d d722 83d3 4c03 52fe  .....a4-."..L.R.
-00005f80: f710 2403 5303 81f7 6f20 dc00 c97a ad07  ..$.S...o ...z..
-00005f90: 6af1 222b bf7d b48e f7e0 9489 42d9 4061  j."+.}......B.@a
-00005fa0: b719 5e15 1ad6 6439 a5a5 5b8c ef1c 63a0  ..^...d9..[...c.
-00005fb0: 82d7 8885 3db3 02a7 5635 1a5a 738e 90d9  ....=...V5.Zs...
-00005fc0: 9619 4dcd b65c 9145 d544 9b81 fe38 0750  ..M..\.E.D...8.P
-00005fd0: e859 5138 168a 6d10 2234 c5b6 7414 a550  .YQ8..m."4..t..P
-00005fe0: d1a9 e03a 548b 8a9b 9af9 2f71 4695 d681  ...:T...../qF...
-00005ff0: 4a8a 945f 4474 6819 4da7 9a03 d082 ad72  J.._Dth.M......r
-00006000: abe5 75aa 7b53 0f17 7a0d 9c17 cf85 f00c  ..u.{S..z.......
-00006010: 9c27 83b7 7209 5ebc 5a0a c521 e135 aefb  .'..r.^.Z..!.5..
-00006020: 1796 5d5e 8e16 b29b 1f0e 3c15 d929 14c7  ..]^......<..)..
-00006030: c84e 019d 283b de48 603d 102d 8877 a669  .N..(;.H`=.-.w.i
-00006040: c2cc cdca 1e93 4ee3 3f65 cfdf beec b9ca  ......N.?e......
-00006050: 4f69 ca2d 4c65 3206 1603 cd07 fa10 27af  Oi.-Le2.......'.
-00006060: 7902 9217 c7e7 d008 8016 a575 4e20 ac42  y..........uN .B
-00006070: 5755 3488 1a3c 761b 0185 edf8 284c 5953  WU4..<v.....(LYS
-00006080: 082d 1368 3e07 d0c9 e4a9 c5e5 2686 565f  .-.h>.......&.V_
-00006090: a5fa a9c4 c1e3 127a 0dad 72f7 dd19 85aa  .......z..r.....
-000060a0: f71a d294 4a2a 5329 2365 6151 8e0d 8c5e  ....J*S)#eaQ...^
-000060b0: 2d82 68c5 86e0 5691 4523 38e4 1332 9571  -.h...V.E#8..2.q
-000060c0: a845 e245 2253 07b9 80ca d0fa 9820 a80d  .E.E"S....... ..
-000060d0: 311c db45 c482 c63d 7435 52e1 7178 64aa  1..E...=t5R.qxd.
-000060e0: 435d c609 9c7b b083 3e96 b241 b5c6 3b87  C]...{..>..A..;.
-000060f0: 5deb dc06 eb04 8186 74bd f321 41a1 f513  ].......t..!A...
-00006100: 680a 53a5 ae17 5981 1840 cd1c 47dd 647e  h.S...Y..@..G.d~
-00006110: dcaf c340 b435 bb5f fc44 7771 1ab0 75ad  ...@.5._.Dwq..u.
-00006120: bcbb d1b9 fe27 9af2 3617 34b5 bbc8 fcc0  .....'..6.4.....
-00006130: 4f21 abfa df05 f1f9 fc52 60e4 6e5c 5303  O!.......R`.n\S.
-00006140: c344 e2cf 4ef2 1a2c 979d 6028 dfb1 381c  .D..N..,..`(..8.
-00006150: 6d25 0a4b e4bf bc17 201d 480f c721 96ff  m%.K.... .H..!..
-00006160: c773 94da 1487 3dc7 3534 bba0 7760 a100  .s....=.54..w`..
-00006170: fad7 5d1a 7a0b e679 e08d fc20 a1fb ad4a  ..].z..y... ...J
-00006180: 50e8 5af2 2e03 f792 827f 3a80 719f 6de2  P.Z.......:.q.m.
-00006190: 24c8 5ead eb20 8456 6717 4a08 5828 8c1f  $.^.. .Vg.J.X(..
-000061a0: f607 5ebb 059f 082d 1fe8 a974 213b df93  ..^....-...t!;..
-000061b0: e090 4cd0 9a1e 70a9 37ac db78 809e dc35  ..L...p.7..x...5
-000061c0: 7337 fde3 3e20 084e 613b 4913 ce14 5c60  s7..> .Na;I...\`
-000061d0: 68ec a88d 7da6 0c36 1701 7446 3ba9 b8a7  h...}..6..tF;...
-000061e0: d08f 8460 215e fa8b b836 75be aa9c 19cc  ...`!^...6u.....
-000061f0: 1554 2278 ad67 a501 1179 4620 e665 ca4d  .T"x.g...yF .e.M
-00006200: 18ed bdaa ab3a 362b 38bd 01a5 1fdf 68a7  .....:6+8.....h.
-00006210: 9e8a 6fc7 c08b b7e2 a817 4d07 1ab7 ad98  ..o.......M.....
-00006220: 0a41 f196 efb1 72e2 153c 3763 1124 3bab  .A....r..<7c.$;.
-00006230: a87a 41ae 9355 391e 2e04 65a0 219d 784e  .zA..U9...e.!.xN
-00006240: 1256 8daa af47 60fa 71b8 92d6 1842 f521  .V...G`.q....B.!
-00006250: 7bd2 a555 4672 8416 9501 4f94 ca89 6726  {..UFr....O...g&
-00006260: 3a43 da31 7f21 14f0 16c7 08a5 8243 3f2b  :C.1.!.......C?+
-00006270: 6a5d eaeb 9180 9855 2898 1f1f c77c 01de  j].....U(....|..
-00006280: c6b7 7ce3 4496 ffec ee9f be75 da5c 4621  ..|.D......u.\F!
-00006290: 28f7 b0a0 2a70 6d12 2abd 76a2 98de d036  (...*pm.*.v....6
-000062a0: 6a03 2505 ef06 6722 bafc 1a30 1de1 3b1a  j.%...g"...0..;.
-000062b0: a0bf 1e21 5547 660a 1919 b4d7 7519 d511  ...!UGf.....u...
-000062c0: 1d21 a23a f0d7 23a1 ea48 5021 2183 1eba  .!.:..#..HP!!...
-000062d0: 2ea1 3aa2 2324 5407 3e51 426f 98cb e823  ..:.#$T.>QBo...#
-000062e0: 4f85 740c 7a7e 55c0 3607 537e ef2d 1897  O.t.z~U.6.S~.-..
-000062f0: 99df 9f70 0cc3 55a0 3ede 5508 ca34 356e  ...p..U.>.U..45n
-00006300: c261 a241 4d70 27ca f073 f418 c5cf a79c  .a.AMp'..s......
-00006310: 581b ccad 2909 b9cd 595e 865e e228 deca  X...)...Y^.^.(..
-00006320: c915 d132 d255 c868 0d89 e59a 8dc1 8b09  ...2.U.h........
-00006330: 19dd 686f b630 819c 0f52 c288 4971 f4bb  ..ho.0...R..Iq..
-00006340: 1af0 af2c f55d 21d2 a2d3 cc67 eb6f 6024  ...,.]!....g.o`$
-00006350: fef7 693e a767 b341 3d18 1c27 d866 a37a  ..i>.g.A=..'.f.z
-00006360: b63e abf7 3fde f692 04f1 36b2 369b 92a6  .>..?.....6.6...
-00006370: 3b86 693d f7a7 d309 f56c e4cd 5c7b e2cc  ;.i=.....l..\{..
-00006380: 3ddb 73c9 c25e 7b73 ec78 f3c9 c859 4074  =.s..^{s.x...Y@t
-00006390: 8316 1848 627b 47e1 8c19 c69d bd85 33c1  ...Hb{G.......3.
-000063a0: c4b5 a7b3 05b5 7dea 8d6c f6c4 5e90 d9d8  ......}..l..^...
-000063b0: f1fd 85bf ce61 a019 00fd 0f06 e2af d174  .....a.........t
-000063c0: e2af 5d1b bbd4 0190 8563 a3f9 7c66 6334  ..]......c..|fc4
-000063d0: 59cf 3c67 b2c0 13c2 9781 6b0c a509 9a14  Y.<g......k.....
-000063e0: 8cf5 394e 180a de70 9796 d6d0 526f 6b8a  ..9N...p....Rok.
-000063f0: f351 ec1d 86d9 a264 5b9d 2004 ce54 93dc  .Q.....d[. ..T..
-00006400: 19bc 1303 27a7 cef9 7597 6a1f da26 1b0b  ....'...u.j..&..
-00006410: 053d 36e9 6cc7 d860 d0ac a703 e26c 1952  .=6.l..`.....l.R
-00006420: d295 b583 d242 3b7b 55be 6f98 9635 4c77  .....B;{U.o..5Lw
-00006430: 1682 3448 4a75 861b 7135 8850 f70a 07e1  ..4HJu..q5.P....
-00006440: 4f14 d551 8155 f411 8c8e 5a8d 2e65 fc73  O..Q.U....Z..e.s
-00006450: d4fa b73f 6a2d 0f6a 17a6 6350 f503 288f  ...?j-.j..cP..(.
-00006460: 9816 9ff4 b660 d41b 8eaa c2fd 960d eca3  .....`..........
-00006470: 65cd 6e42 e898 43e8 2270 976f 3122 9e4d  e.nB..C."p.o1".M
-00006480: 8907 a16b 3af3 6d34 9eba f668 3c9d e1e9  ...k:.m4...h<...
-00006490: 6c8c b18f 45e8 2a37 28ab 84a6 9bf8 9947  l...E.*7(......G
-000064a0: d9d5 80af 0fcb 435b 056e 95c1 dacf 746d  ......C[.n....tm
-000064b0: 782f ab23 9ee4 2146 9b3b e48e bd61 e652  x/.#..!F.;...a.R
-000064c0: 3ba2 bd8d e3c7 fd4e 9d88 b6c5 2431 dd9b  ;......N....$1..
-000064d0: 1fd4 1633 5b39 b41e 958a 09b3 eea3 5bad  ...3[9........[.
-000064e0: 8fa8 5d86 e20e e1ad 26aa 8ef0 2e95 696b  ..].....&.....ik
-000064f0: 16d5 61cc 5b9c cba6 fc0e 1fdc 3e7c 845c  ..a.[.......>|.\
-00006500: a876 2132 a1b6 76e7 eb90 0342 f2a2 6369  .v!2..v....B..ci
-00006510: 067e 1f69 53f0 eb30 c68f 6a3c fe5f 30e4  .~.iS..0..j<._0.
-00006520: 9f8f 9cd7 e6cd fb53 d96b d23e 5004 b45e  .......S.k.>P..^
-00006530: 6db4 8328 cdf8 914a 3e25 4f8a 29f9 dd3e  m..(...J>%O.)..>
-00006540: 09b9 2409 1ee6 194b 3a74 ce9c a19c a827  ..$....K:t.....'
-00006550: 98e5 6cc5 8cbe 0ec0 bf51 6fc6 242e f036  ..l......Qo.$..6
-00006560: 8ff2 4b5b 1cc6 eb62 d611 1ad6 95ab 86f9  ..K[...b........
-00006570: beeb 4b55 6813 e865 8f47 8980 b073 71b8  ..KUh..e.G...sq.
-00006580: 709c 50ce 534e c410 049b 0e7f 030e 61da  p.P.SN........a.
-00006590: df1d 8e26 c3d1 7848 f019 1862 71bc 6344  ...&..xH...bq.cD
-000065a0: 8564 f82d 96e7 b8ca 3494 c7d0 191b fa7d  .d.-....4......}
-000065b0: 1361 e097 f75f 2a5f a823 3c2d 9bcd ef3d  .a..._*_.#<-...=
-000065c0: d65f 969e 2abf a5a2 2799 3cc3 2578 8921  ._..*...'.<.%x.!
-000065d0: d780 8901 7081 6df3 aa4e 2136 4972 0ecc  ....p.m..N!6Ir..
-000065e0: 9912 18d8 dd91 1e18 9601 4cbf 67ec eec9  ..........L.g...
-000065f0: 9114 0867 888b 8be5 9dcb 374c 9783 c7cf  ...g......7L....
-00006600: 6f46 38e2 b0bd 5458 e50e 5c9c e62b 9157  oF8...TX..\..+.W
-00006610: d85f 6641 0667 865d 7cb3 c092 2f03 7925  ._fA.g.]|.../.y%
-00006620: 7c28 ad72 cfe1 5bd1 a77b 9ea4 772e d00a  |(.r..[..{..w...
-00006630: ac1d c21c 8740 48f6 5194 50dd b54f 5dac  .....@H.Q.P..O].
-00006640: ade4 8428 7ad8 83ef ee43 0b8c bec8 b9ac  ...(z....C......
-00006650: 761d 35a0 4570 965f d4ef 24c4 1859 429f  v.5.Ep._..$..YB.
-00006660: 0236 c073 2436 6597 5114 677c ea48 3e01  .6.s$6e.Q.g|.H>.
-00006670: af0a f350 917a 68b5 fc73 cfee d73c f19b  ...P.zh..s...<..
-00006680: 386c e681 8928 e517 7260 ca69 4d13 763d  8l...(..r`.iM.v=
-00006690: 2745 4ff0 2c4e 2c49 647a 66b1 fb3b 68b7  'EO.,N,Idzf..;h.
-000066a0: 93e3 4416 2081 f19c 1d4c 20b1 e36f 0b82  ..D. ....L ..o..
-000066b0: adb5 df11 a008 8628 f815 1eb1 04f2 c1d4  .......(........
-000066c0: 2d8a f046 213b fbf6 9b26 d244 355c e542  -..F!;...&.D5\.B
-000066d0: 3c45 256e 459a 212e 6e4b eea5 8189 9d0a  <E%nE.!.nK......
-000066e0: d9fd 55f8 3909 f00e e482 4de5 9db4 fb25  ..U.9.....M....%
-000066f0: 9fb5 cdd1 7622 ad29 73c9 e9b0 798e 7d2f  ....v".)s...y.}/
-00006700: fbe0 9ce7 2e99 ffad b972 2689 5ace 74d2  .........r&.Z.t.
-00006710: 0f31 74df 217b 8364 e92d efe2 a9fb 872a  .1t.!{.d.-.....*
-00006720: c8b7 e639 79be 5cb9 cdc5 6ec5 8039 0a85  ...9y.\...n..9..
-00006730: 9257 a0d8 4c56 fea4 9c5c 2b60 d9ef b92a  .W..LV...\+`...*
-00006740: ba6b 15d5 e07d 1ef9 7e8e 4caa ab84 d6ee  .k...}..~.L.....
-00006750: 5494 74f5 08d8 7c7c 4cd7 f41a 34e8 c752  T.t...||L...4..R
-00006760: e783 7dae ab50 0bad 4287 4b7c 8a54 8321  ..}..P..B.K|.T.!
-00006770: 1537 af6a 0bc2 5792 5501 ae31 da1b 5870  .7.j..W.U..1..Xp
-00006780: 7a3c f8c5 d5e5 799a c638 0097 477e 80e4  z<....y..8..G~..
-00006790: 217b edbd dd80 2bc7 d0ee 5c8a 62aa 2697  !{....+...\.b.&.
-000067a0: ea46 809c 5471 018e 127e 0002 5a88 6281  .F..Tq...~..Z.b.
-000067b0: 5fe4 4f6b 8886 61f1 5eae 4a5d 70c6 2077  _.Ok..a.^.J]p. w
-000067c0: af29 dcb8 bcc9 f37f b6a4 31a8 1429 c4b2  .)........1..)..
-000067d0: 3638 2335 2bf8 109a 52e5 5e45 d6b2 b229  68#5+...R.^E...)
-000067e0: b09a 38aa 688a bb45 c761 6890 4d4f 5aaa  ..8.h..E.ah.MOZ.
-000067f0: a232 4453 b6a0 42f3 728e 2b06 ccac 51ab  .2DS..B.r.+...Q.
-00006800: c935 0b2c eb55 c990 8f76 3a62 77a4 c27c  .5.,.U...v:bw..|
-00006810: a23e 4dd8 4fa2 f470 7d39 26c2 c6c4 3a9d  .>M.O..p}9&...:.
-00006820: 572b 2737 045a d8bd 6159 76dd 775d 7658  W+'7.Z..aYv.w]vX
-00006830: d117 168e a8bb 61ab 3ec2 c88a caba 2264  ......a.>....."d
-00006840: 5bda e9e3 dd66 eb56 f746 c5f6 ba3f 306c  [....f.V.F...?0l
-00006850: 767f 60d8 edfe c0b0 ddfd 8161 bf8f 07be  v.`........a....
-00006860: e7a7 487d 0d9d 419b 5f29 65d9 a38c d66c  ..H}..A._)e....l
-00006870: c537 d03f 45c0 291c f0a8 72c0 560a ca55  .7.?E.)...r.V..U
-00006880: f4e4 6b57 7b0b 0703 710f 2363 0b09 1afb  ..kW{...q.#c....
-00006890: ed2f bb36 7b10 926f 863a 6a19 36fd 34de  ./.6{..o.:j.6.4.
-000068a0: bbff 0300 00ff ff03 0050 4b03 0414 0006  .........PK.....
-000068b0: 0008 0000 0021 0070 ed44 6e02 0200 0078  .....!.p.Dn....x
-000068c0: 0400 0013 0028 0063 7573 746f 6d58 6d6c  .....(.customXml
-000068d0: 2f69 7465 6d34 2e78 6d6c 20a2 2400 28a0  /item4.xml .$.(.
-000068e0: 2000 0000 0000 0000 0000 0000 0000 0000   ...............
-000068f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00006900: 0000 ac94 4f6f e230 10c5 bf0a cadd b1f3  ....Oo.0........
-00006910: 3f46 2108 954b a545 eab6 b4ea 0d19 7b0c  ?F!..K.E......{.
-00006920: 9612 3bb2 4da1 df7e 1d5a 680f ab6d 2bed  ..;.M..~.Zh..m+.
-00006930: 293e e4fd 66fc e68d 9bf9 a9ef 262f 609d  )>..f.......&/`.
-00006940: 327a 1625 3189 26a0 b911 4aef 66d1 c14b  2z.%1.&...J.f..K
-00006950: 5447 f3b6 19a6 8335 0358 afc0 4d82 42bb  TG.....5.X..M.B.
-00006960: e930 8bf6 de0f 538c 1ddf 43cf 5cdc 2b6e  .0....S...C.\.+n
-00006970: 8d33 d2c7 dcf4 d848 a938 e094 9012 f7e0  .3.....H.8......
-00006980: 9960 9ee1 0f4a f48e 3939 7505 1d8f c7f8  .`...J..99u.....
-00006990: 98c5 c6ee 4659 829f 57bf 1ece 6ca4 b4f3  ....FY..W...l...
-000069a0: 4c73 b8a8 067e 15fd b3ba d2d2 0ccc ef47  Ls...~.........G
-000069b0: 5e85 ef98 f51a ec8d d1de 9ace 456d 230c  ^...........Em#.
-000069c0: 3ff4 a0fd 8a69 b683 f1d4 361b d1f1 cdd2  ?....i....6.....
-000069d0: f05b f1d6 e22c aad3 0c08 6580 4a5e 7294  .[...,....e.J^r.
-000069e0: 1396 a29a 6414 2529 a535 29a4 c824 8dda  ....d.%).5)..$..
-000069f0: c745 f97b 759f 3fdc 3d2d 9e51 9dd7 6991  .E.{u.?.=-.Q..i.
-00006a00: 57b4 4409 19bf 0dfe c0b6 4dc7 6555 caa4  W.D.......M.eU..
-00006a10: 2838 885c 08be cd09 ad92 2c97 32e3 5996  (8.\......,.2.Y.
-00006a20: ca6b 61c6 73ba 2d05 aa4a 0094 b394 2326  .ka.s.-..J....#&
-00006a30: 648a 7241 6bc6 6a56 6e13 08b7 5883 eddf  d.rAk.jVn...X...
-00006a40: c7f2 7f6c c167 62db e0af 1a0d b5d9 e986  ...l.gb.........
-00006a50: 79be 5f74 dda5 eb94 a682 089e 2228 2845  y._t........"((E
-00006a60: 3930 8ab6 0548 9465 5b29 aa60 5ac1 ab30  90...H.e[).`Z..0
-00006a70: 48a7 a65a 75b3 c8db 0344 b86d 82e5 e759  H..Zu....D.m...Y
-00006a80: 6c4e 84a4 64b3 7e1d 805c 90f5 778c 088c  lN..d.~..\..w...
-00006a90: 05f7 ea05 7ea4 fa56 233f 2286 3e3e 86fd  ....~..V#?".>>..
-00006aa0: 68af be7c 2f46 4d50 b4e3 66b9 b05a 87e0  h..|/FMP..f..Z..
-00006ab0: 1084 ed8c dd9e 5918 8cd2 6fcb e581 f50e  ......Y...o.....
-00006ac0: 3f2e ee57 ebf1 a43c e04d c75e cdc1 3b9c  ?..W...<.M.^..;.
-00006ad0: 14f8 9cde 7b10 cac6 cc0d a7f9 ed72 f645  ....{........r.E
-00006ae0: 3ac7 a2cd 121c b76a f0e1 29f8 2acd 9f7f  :......j..).*...
-00006af0: fd9c ed33 07ff 6dad f0e7 37a4 fd03 0000  ...3..m...7.....
-00006b00: ffff 0300 504b 0102 2d00 1400 0600 0800  ....PK..-.......
-00006b10: 0000 2100 df73 5b55 9b01 0000 1d07 0000  ..!..s[U........
-00006b20: 1300 0000 0000 0000 0000 0000 0000 0000  ................
-00006b30: 0000 5b43 6f6e 7465 6e74 5f54 7970 6573  ..[Content_Types
-00006b40: 5d2e 786d 6c50 4b01 022d 0014 0006 0008  ].xmlPK..-......
-00006b50: 0000 0021 0013 5ebe 6505 0100 00df 0200  ...!..^.e.......
-00006b60: 000b 0000 0000 0000 0000 0000 0000 00b7  ................
-00006b70: 0300 005f 7265 6c73 2f2e 7265 6c73 504b  ..._rels/.relsPK
-00006b80: 0102 2d00 1400 0600 0800 0000 2100 f938  ..-.........!..8
-00006b90: 46ef df02 0000 6b06 0000 0f00 0000 0000  F.....k.........
-00006ba0: 0000 0000 0000 0000 dc06 0000 786c 2f77  ............xl/w
-00006bb0: 6f72 6b62 6f6f 6b2e 786d 6c50 4b01 022d  orkbook.xmlPK..-
-00006bc0: 0014 0006 0008 0000 0021 0085 826b 5524  .........!...kU$
-00006bd0: 0100 00f2 0400 001a 0000 0000 0000 0000  ................
-00006be0: 0000 0000 00e8 0900 0078 6c2f 5f72 656c  .........xl/_rel
-00006bf0: 732f 776f 726b 626f 6f6b 2e78 6d6c 2e72  s/workbook.xml.r
-00006c00: 656c 7350 4b01 022d 0014 0006 0008 0000  elsPK..-........
-00006c10: 0021 007d 6fba c043 1500 00b0 6e00 0018  .!.}o..C....n...
-00006c20: 0000 0000 0000 0000 0000 0000 0042 0c00  .............B..
-00006c30: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
-00006c40: 6865 6574 312e 786d 6c50 4b01 022d 0014  heet1.xmlPK..-..
-00006c50: 0006 0008 0000 0021 00e9 a625 b866 0600  .......!...%.f..
-00006c60: 0053 1b00 0013 0000 0000 0000 0000 0000  .S..............
-00006c70: 0000 00bb 2100 0078 6c2f 7468 656d 652f  ....!..xl/theme/
-00006c80: 7468 656d 6531 2e78 6d6c 504b 0102 2d00  theme1.xmlPK..-.
-00006c90: 1400 0600 0800 0000 2100 8c3e 5b78 7803  ........!..>[xx.
-00006ca0: 0000 d609 0000 0d00 0000 0000 0000 0000  ................
-00006cb0: 0000 0000 5228 0000 786c 2f73 7479 6c65  ....R(..xl/style
-00006cc0: 732e 786d 6c50 4b01 022d 0014 0006 0008  s.xmlPK..-......
-00006cd0: 0000 0021 006b dcd4 f9ab 0500 00e1 3e00  ...!.k........>.
-00006ce0: 0014 0000 0000 0000 0000 0000 0000 00f5  ................
-00006cf0: 2b00 0078 6c2f 7368 6172 6564 5374 7269  +..xl/sharedStri
-00006d00: 6e67 732e 786d 6c50 4b01 022d 0014 0006  ngs.xmlPK..-....
-00006d10: 0008 0000 0021 00bd 8462 2390 0000 00db  .....!...b#.....
-00006d20: 0000 0013 0000 0000 0000 0000 0000 0000  ................
-00006d30: 00d2 3100 0063 7573 746f 6d58 6d6c 2f69  ..1..customXml/i
-00006d40: 7465 6d31 2e78 6d6c 504b 0102 2d00 1400  tem1.xmlPK..-...
-00006d50: 0600 0800 0000 2100 3596 801d f100 0000  ......!.5.......
-00006d60: 4f01 0000 1800 0000 0000 0000 0000 0000  O...............
-00006d70: 0000 bb32 0000 6375 7374 6f6d 586d 6c2f  ...2..customXml/
-00006d80: 6974 656d 5072 6f70 7331 2e78 6d6c 504b  itemProps1.xmlPK
-00006d90: 0102 2d00 1400 0600 0800 0000 2100 635b  ..-.........!.c[
-00006da0: 0d84 6001 0000 9106 0000 1300 0000 0000  ..`.............
-00006db0: 0000 0000 0000 0000 0a34 0000 6375 7374  .........4..cust
-00006dc0: 6f6d 586d 6c2f 6974 656d 322e 786d 6c50  omXml/item2.xmlP
-00006dd0: 4b01 022d 0014 0006 0008 0000 0021 00b8  K..-.........!..
-00006de0: b7cf 58ea 0000 0041 0100 0018 0000 0000  ..X....A........
-00006df0: 0000 0000 0000 0000 00bf 3500 0063 7573  ..........5..cus
-00006e00: 746f 6d58 6d6c 2f69 7465 6d50 726f 7073  tomXml/itemProps
-00006e10: 322e 786d 6c50 4b01 022d 000a 0000 0000  2.xmlPK..-......
-00006e20: 0000 0021 00ff ffff ffd5 0d00 00d5 0d00  ...!............
-00006e30: 0010 0000 0000 0000 0000 0000 0000 0007  ................
-00006e40: 3700 005b 7472 6173 685d 2f30 3030 302e  7..[trash]/0000.
-00006e50: 6461 7450 4b01 022d 0014 0006 0008 0000  datPK..-........
-00006e60: 0021 00af 391a ebd4 0100 00ba 0400 0018  .!..9...........
-00006e70: 0000 0000 0000 0000 0000 0000 000a 4500  ..............E.
-00006e80: 0063 7573 746f 6d58 6d6c 2f69 7465 6d50  .customXml/itemP
-00006e90: 726f 7073 332e 786d 6c50 4b01 022d 0014  rops3.xmlPK..-..
-00006ea0: 0006 0008 0000 0021 0016 7cdd d549 0100  .......!..|..I..
-00006eb0: 0066 0200 0011 0000 0000 0000 0000 0000  .f..............
-00006ec0: 0000 003c 4700 0064 6f63 5072 6f70 732f  ...<G..docProps/
-00006ed0: 636f 7265 2e78 6d6c 504b 0102 2d00 1400  core.xmlPK..-...
-00006ee0: 0600 0800 0000 2100 290f f5c6 7d01 0000  ......!.)...}...
-00006ef0: fe02 0000 1000 0000 0000 0000 0000 0000  ................
-00006f00: 0000 bc49 0000 646f 6350 726f 7073 2f61  ...I..docProps/a
-00006f10: 7070 2e78 6d6c 504b 0102 2d00 1400 0600  pp.xmlPK..-.....
-00006f20: 0800 0000 2100 743f 397a c200 0000 2801  ....!.t?9z....(.
-00006f30: 0000 1e00 0000 0000 0000 0000 0000 0000  ................
-00006f40: 6f4c 0000 6375 7374 6f6d 586d 6c2f 5f72  oL..customXml/_r
-00006f50: 656c 732f 6974 656d 312e 786d 6c2e 7265  els/item1.xml.re
-00006f60: 6c73 504b 0102 2d00 1400 0600 0800 0000  lsPK..-.........
-00006f70: 2100 5c96 2722 c300 0000 2801 0000 1e00  !.\.'"....(.....
-00006f80: 0000 0000 0000 0000 0000 0000 754e 0000  ............uN..
-00006f90: 6375 7374 6f6d 586d 6c2f 5f72 656c 732f  customXml/_rels/
-00006fa0: 6974 656d 322e 786d 6c2e 7265 6c73 504b  item2.xml.relsPK
-00006fb0: 0102 2d00 1400 0600 0800 0000 2100 7bf3  ..-.........!.{.
-00006fc0: 02a3 c300 0000 2801 0000 1e00 0000 0000  ......(.........
-00006fd0: 0000 0000 0000 0000 7c50 0000 6375 7374  ........|P..cust
-00006fe0: 6f6d 586d 6c2f 5f72 656c 732f 6974 656d  omXml/_rels/item
-00006ff0: 332e 786d 6c2e 7265 6c73 504b 0102 2d00  3.xml.relsPK..-.
-00007000: 0a00 0000 0000 0000 2100 ffff ffff e201  ........!.......
-00007010: 0000 e201 0000 1000 0000 0000 0000 0000  ................
-00007020: 0000 0000 8352 0000 5b74 7261 7368 5d2f  .....R..[trash]/
-00007030: 3030 3031 2e64 6174 504b 0102 2d00 1400  0001.datPK..-...
-00007040: 0600 0800 0000 2100 3450 cf2b b900 0000  ......!.4P.+....
-00007050: c900 0000 1800 0000 0000 0000 0000 0000  ................
-00007060: 0000 9354 0000 6375 7374 6f6d 586d 6c2f  ...T..customXml/
-00007070: 6974 656d 5072 6f70 7334 2e78 6d6c 504b  itemProps4.xmlPK
-00007080: 0102 2d00 1400 0600 0800 0000 2100 29e7  ..-.........!.).
-00007090: 528d 5c01 0000 b302 0000 1300 0000 0000  R.\.............
-000070a0: 0000 0000 0000 0000 aa55 0000 646f 6350  .........U..docP
-000070b0: 726f 7073 2f63 7573 746f 6d2e 786d 6c50  rops/custom.xmlP
-000070c0: 4b01 022d 0014 0006 0008 0000 0021 000c  K..-.........!..
-000070d0: c41a 92c3 0000 0028 0100 001e 0000 0000  .......(........
-000070e0: 0000 0000 0000 0000 00dd 5700 0063 7573  ..........W..cus
-000070f0: 746f 6d58 6d6c 2f5f 7265 6c73 2f69 7465  tomXml/_rels/ite
-00007100: 6d34 2e78 6d6c 2e72 656c 7350 4b01 022d  m4.xml.relsPK..-
-00007110: 0014 0006 0008 0000 0021 00c3 945c ad6c  .........!...\.l
-00007120: 0e00 0057 4f00 0013 0000 0000 0000 0000  ...WO...........
-00007130: 0000 0000 00e4 5900 0063 7573 746f 6d58  ......Y..customX
-00007140: 6d6c 2f69 7465 6d33 2e78 6d6c 504b 0102  ml/item3.xmlPK..
-00007150: 2d00 1400 0600 0800 0000 2100 70ed 446e  -.........!.p.Dn
-00007160: 0202 0000 7804 0000 1300 0000 0000 0000  ....x...........
-00007170: 0000 0000 0000 a968 0000 6375 7374 6f6d  .......h..custom
-00007180: 586d 6c2f 6974 656d 342e 786d 6c50 4b05  Xml/item4.xmlPK.
-00007190: 0600 0000 0019 0019 0089 0600 0004 6b00  ..............k.
-000071a0: 0000 00                                  ...
+00005a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00005a80: 0000 0000 84cf c16a c330 0c06 e07b 61ef  .......j.0...{a.
+00005a90: 6074 5f9c 9431 4a89 d3cb 28e4 3646 07bb  `t_..1J...(.6F..
+00005aa0: 1a47 71cc 62cb 58ea 58df 7ea6 a716 063d  .Gq.b.X.X.~....=
+00005ab0: 4a42 df2f f587 dfb8 aa1f 2c1c 2819 e89a  JB./......,.(...
+00005ac0: 1614 2647 5348 dec0 e7e9 f8bc 03c5 62d3  ..&GSH........b.
+00005ad0: 6457 4a68 e082 0c87 e169 d37f e06a a52e  dWJh.....i...j..
+00005ae0: f112 32ab aa24 36b0 88e4 bdd6 ec16 8c96  ..2..$6.........
+00005af0: 1bca 98ea 64a6 12ad d4b2 789d adfb b61e  ....d.....x.....
+00005b00: f5b6 6d5f 75b9 3560 b833 d538 1928 e3d4  ..m_u.5`.3.8.(..
+00005b10: 813a 5d72 4d7e 6cd3 3c07 876f e4ce 1193  .:]rM~l.<..o....
+00005b20: fc13 a1dd 9985 e257 5cdf 0b65 aeb2 2d1e  .......W\..e..-.
+00005b30: c540 108c d7d6 4b53 ef05 3df4 faee bfe1  .@....KS..=.....
+00005b40: 0f00 00ff ff03 0050 4b01 022d 0014 0006  .......PK..-....
+00005b50: 0008 0000 0021 000b 3936 6e8b 0100 001d  .....!..96n.....
+00005b60: 0700 0013 0000 0000 0000 0000 0000 0000  ................
+00005b70: 0000 0000 005b 436f 6e74 656e 745f 5479  .....[Content_Ty
+00005b80: 7065 735d 2e78 6d6c 504b 0102 2d00 1400  pes].xmlPK..-...
+00005b90: 0600 0800 0000 2100 135e be65 0201 0000  ......!..^.e....
+00005ba0: df02 0000 0b00 0000 0000 0000 0000 0000  ................
+00005bb0: 0000 c403 0000 5f72 656c 732f 2e72 656c  ......_rels/.rel
+00005bc0: 7350 4b01 022d 0014 0006 0008 0000 0021  sPK..-.........!
+00005bd0: 00fd 33d2 52e6 0200 0075 0600 000f 0000  ..3.R....u......
+00005be0: 0000 0000 0000 0000 0000 00f7 0600 0078  ...............x
+00005bf0: 6c2f 776f 726b 626f 6f6b 2e78 6d6c 504b  l/workbook.xmlPK
+00005c00: 0102 2d00 1400 0600 0800 0000 2100 8582  ..-.........!...
+00005c10: 6b55 1f01 0000 f204 0000 1a00 0000 0000  kU..............
+00005c20: 0000 0000 0000 0000 0a0a 0000 786c 2f5f  ............xl/_
+00005c30: 7265 6c73 2f77 6f72 6b62 6f6f 6b2e 786d  rels/workbook.xm
+00005c40: 6c2e 7265 6c73 504b 0102 2d00 1400 0600  l.relsPK..-.....
+00005c50: 0800 0000 2100 c1fe 8f39 3915 0000 9e6e  ....!....99....n
+00005c60: 0000 1800 0000 0000 0000 0000 0000 0000  ................
+00005c70: 690c 0000 786c 2f77 6f72 6b73 6865 6574  i...xl/worksheet
+00005c80: 732f 7368 6565 7431 2e78 6d6c 504b 0102  s/sheet1.xmlPK..
+00005c90: 2d00 1400 0600 0800 0000 2100 e9a6 25b8  -.........!...%.
+00005ca0: 6606 0000 531b 0000 1300 0000 0000 0000  f...S...........
+00005cb0: 0000 0000 0000 d821 0000 786c 2f74 6865  .......!..xl/the
+00005cc0: 6d65 2f74 6865 6d65 312e 786d 6c50 4b01  me/theme1.xmlPK.
+00005cd0: 022d 0014 0006 0008 0000 0021 0000 d49f  .-.........!....
+00005ce0: c473 0300 00c8 0900 000d 0000 0000 0000  .s..............
+00005cf0: 0000 0000 0000 006f 2800 0078 6c2f 7374  .......o(..xl/st
+00005d00: 796c 6573 2e78 6d6c 504b 0102 2d00 1400  yles.xmlPK..-...
+00005d10: 0600 0800 0000 2100 6bdc d4f9 ab05 0000  ......!.k.......
+00005d20: e13e 0000 1400 0000 0000 0000 0000 0000  .>..............
+00005d30: 0000 0d2c 0000 786c 2f73 6861 7265 6453  ...,..xl/sharedS
+00005d40: 7472 696e 6773 2e78 6d6c 504b 0102 2d00  trings.xmlPK..-.
+00005d50: 1400 0600 0800 0000 2100 635b 0d84 5c01  ........!.c[..\.
+00005d60: 0000 9106 0000 1300 0000 0000 0000 0000  ................
+00005d70: 0000 0000 ea31 0000 6375 7374 6f6d 586d  .....1..customXm
+00005d80: 6c2f 6974 656d 312e 786d 6c50 4b01 022d  l/item1.xmlPK..-
+00005d90: 0014 0006 0008 0000 0021 00b8 b7cf 58ea  .........!....X.
+00005da0: 0000 0041 0100 0018 0000 0000 0000 0000  ...A............
+00005db0: 0000 0000 009f 3300 0063 7573 746f 6d58  ......3..customX
+00005dc0: 6d6c 2f69 7465 6d50 726f 7073 312e 786d  ml/itemProps1.xm
+00005dd0: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
+00005de0: 00bd 8462 2390 0000 00db 0000 0013 0000  ...b#...........
+00005df0: 0000 0000 0000 0000 0000 00e7 3400 0063  ............4..c
+00005e00: 7573 746f 6d58 6d6c 2f69 7465 6d32 2e78  ustomXml/item2.x
+00005e10: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
+00005e20: 2100 3596 801d f100 0000 4f01 0000 1800  !.5.......O.....
+00005e30: 0000 0000 0000 0000 0000 0000 d035 0000  .............5..
+00005e40: 6375 7374 6f6d 586d 6c2f 6974 656d 5072  customXml/itemPr
+00005e50: 6f70 7332 2e78 6d6c 504b 0102 2d00 1400  ops2.xmlPK..-...
+00005e60: 0600 0800 0000 2100 70ed 446e fa01 0000  ......!.p.Dn....
+00005e70: 7804 0000 1300 0000 0000 0000 0000 0000  x...............
+00005e80: 0000 1f37 0000 6375 7374 6f6d 586d 6c2f  ...7..customXml/
+00005e90: 6974 656d 332e 786d 6c50 4b01 022d 0014  item3.xmlPK..-..
+00005ea0: 0006 0008 0000 0021 008f 8854 fb5b 0100  .......!...T.[..
+00005eb0: 0060 0200 0018 0000 0000 0000 0000 0000  .`..............
+00005ec0: 0000 0072 3900 0063 7573 746f 6d58 6d6c  ...r9..customXml
+00005ed0: 2f69 7465 6d50 726f 7073 332e 786d 6c50  /itemProps3.xmlP
+00005ee0: 4b01 022d 0014 0006 0008 0000 0021 00c3  K..-.........!..
+00005ef0: 945c adaa 0d00 0057 4f00 0013 0000 0000  .\.....WO.......
+00005f00: 0000 0000 0000 0000 002b 3b00 0063 7573  .........+;..cus
+00005f10: 746f 6d58 6d6c 2f69 7465 6d34 2e78 6d6c  tomXml/item4.xml
+00005f20: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00005f30: af39 1aeb d401 0000 ba04 0000 1800 0000  .9..............
+00005f40: 0000 0000 0000 0000 0000 2e49 0000 6375  ...........I..cu
+00005f50: 7374 6f6d 586d 6c2f 6974 656d 5072 6f70  stomXml/itemProp
+00005f60: 7334 2e78 6d6c 504b 0102 2d00 1400 0600  s4.xmlPK..-.....
+00005f70: 0800 0000 2100 1599 551d 4f01 0000 6602  ....!...U.O...f.
+00005f80: 0000 1100 0000 0000 0000 0000 0000 0000  ................
+00005f90: 604b 0000 646f 6350 726f 7073 2f63 6f72  `K..docProps/cor
+00005fa0: 652e 786d 6c50 4b01 022d 0014 0006 0008  e.xmlPK..-......
+00005fb0: 0000 0021 0029 0ff5 c67d 0100 00fe 0200  ...!.)...}......
+00005fc0: 0010 0000 0000 0000 0000 0000 0000 00e6  ................
+00005fd0: 4d00 0064 6f63 5072 6f70 732f 6170 702e  M..docProps/app.
+00005fe0: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
+00005ff0: 0021 0029 e752 8d5a 0100 00b3 0200 0013  .!.).R.Z........
+00006000: 0000 0000 0000 0000 0000 0000 0099 5000  ..............P.
+00006010: 0064 6f63 5072 6f70 732f 6375 7374 6f6d  .docProps/custom
+00006020: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00006030: 0000 2100 743f 397a c200 0000 2801 0000  ..!.t?9z....(...
+00006040: 1e00 0000 0000 0000 0000 0000 0000 2c53  ..............,S
+00006050: 0000 6375 7374 6f6d 586d 6c2f 5f72 656c  ..customXml/_rel
+00006060: 732f 6974 656d 312e 786d 6c2e 7265 6c73  s/item1.xml.rels
+00006070: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00006080: 5c96 2722 c300 0000 2801 0000 1e00 0000  \.'"....(.......
+00006090: 0000 0000 0000 0000 0000 3255 0000 6375  ..........2U..cu
+000060a0: 7374 6f6d 586d 6c2f 5f72 656c 732f 6974  stomXml/_rels/it
+000060b0: 656d 322e 786d 6c2e 7265 6c73 504b 0102  em2.xml.relsPK..
+000060c0: 2d00 1400 0600 0800 0000 2100 7bf3 02a3  -.........!.{...
+000060d0: c300 0000 2801 0000 1e00 0000 0000 0000  ....(...........
+000060e0: 0000 0000 0000 3957 0000 6375 7374 6f6d  ......9W..custom
+000060f0: 586d 6c2f 5f72 656c 732f 6974 656d 332e  Xml/_rels/item3.
+00006100: 786d 6c2e 7265 6c73 504b 0102 2d00 1400  xml.relsPK..-...
+00006110: 0600 0800 0000 2100 0cc4 1a92 c300 0000  ......!.........
+00006120: 2801 0000 1e00 0000 0000 0000 0000 0000  (...............
+00006130: 0000 4059 0000 6375 7374 6f6d 586d 6c2f  ..@Y..customXml/
+00006140: 5f72 656c 732f 6974 656d 342e 786d 6c2e  _rels/item4.xml.
+00006150: 7265 6c73 504b 0506 0000 0000 1700 1700  relsPK..........
+00006160: 0d06 0000 475b 0000 0000                 ....G[....
```

### Comparing `opex_manifest_generator-1.1.4/opex_manifest_generator/samples/spreads/dctemplate.xlsx` & `opex_manifest_generator-1.1.5/opex_manifest_generator/samples/spreads/dctemplate.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.4/opex_manifest_generator/samples/spreads/eadtemplate.xlsx` & `opex_manifest_generator-1.1.5/opex_manifest_generator/samples/spreads/eadtemplate.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.4/opex_manifest_generator/samples/spreads/gdprtemplate.xlsx` & `opex_manifest_generator-1.1.5/opex_manifest_generator/samples/spreads/gdprtemplate.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.4/opex_manifest_generator/samples/spreads/modstemplate.xlsx` & `opex_manifest_generator-1.1.5/opex_manifest_generator/samples/spreads/modstemplate.xlsx`

 * *Files identical despite different names*

### Comparing `opex_manifest_generator-1.1.4/opex_manifest_generator.egg-info/PKG-INFO` & `opex_manifest_generator-1.1.5/opex_manifest_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opex_manifest_generator
-Version: 1.1.4
+Version: 1.1.5
 Summary: Opex Manifest Generator Tool for use with Opex / Preservica
 Author-email: Christopher Prince <c.pj.prince@gmail.com>
 Project-URL: Homepage, https://github.com/CPJPRINCE/opex_manifest_generator
 Project-URL: Issues, https://github.com/CPJPRINCE/opex_manifest_generator/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `opex_manifest_generator-1.1.4/opex_manifest_generator.egg-info/SOURCES.txt` & `opex_manifest_generator-1.1.5/opex_manifest_generator.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 .gitignore
 LICENSE.md
 README.md
 pyproject.toml
+assets/Column Headers.png
+assets/FullName Column.png
+assets/Hash Headers.png
+assets/Identifiers Headers.png
+assets/XML Headers.png
 opex_manifest_generator/__init__.py
 opex_manifest_generator/cli.py
 opex_manifest_generator/common.py
 opex_manifest_generator/hash.py
 opex_manifest_generator/opex_manifest.py
 opex_manifest_generator/test_cli.py
-opex_manifest_generator/version.py
 opex_manifest_generator.egg-info/PKG-INFO
 opex_manifest_generator.egg-info/SOURCES.txt
 opex_manifest_generator.egg-info/dependency_links.txt
 opex_manifest_generator.egg-info/entry_points.txt
 opex_manifest_generator.egg-info/requires.txt
 opex_manifest_generator.egg-info/top_level.txt
 opex_manifest_generator/metadata/DublinCore Template.xml
```

