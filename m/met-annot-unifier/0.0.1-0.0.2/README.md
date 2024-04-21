# Comparing `tmp/met_annot_unifier-0.0.1.tar.gz` & `tmp/met_annot_unifier-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "met_annot_unifier-0.0.1.tar", max compression
+gzip compressed data, was "met_annot_unifier-0.0.2.tar", max compression
```

## Comparing `met_annot_unifier-0.0.1.tar` & `met_annot_unifier-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1077 2024-04-21 07:42:34.478076 met_annot_unifier-0.0.1/LICENSE
--rw-r--r--   0        0        0     4872 2024-04-21 07:42:34.478076 met_annot_unifier-0.0.1/README.md
--rw-r--r--   0        0        0        0 2024-04-21 07:42:34.494076 met_annot_unifier-0.0.1/met_annot_unifier/__init__.py
--rw-r--r--   0        0        0        0 2024-04-21 07:42:34.494076 met_annot_unifier-0.0.1/met_annot_unifier/aligner/__init__.py
--rw-r--r--   0        0        0     7307 2024-04-21 07:42:34.494076 met_annot_unifier-0.0.1/met_annot_unifier/aligner/aligner.py
--rw-r--r--   0        0        0     8044 2024-04-21 07:42:34.494076 met_annot_unifier-0.0.1/met_annot_unifier/aligner/parser.py
--rw-r--r--   0        0        0      845 2024-04-21 07:42:34.494076 met_annot_unifier-0.0.1/met_annot_unifier/aligner/utils.py
--rw-r--r--   0        0        0     2700 2024-04-21 07:42:34.494076 met_annot_unifier-0.0.1/met_annot_unifier/cli.py
--rw-r--r--   0        0        0      267 2024-04-21 07:42:34.494076 met_annot_unifier-0.0.1/met_annot_unifier/foo.py
--rw-r--r--   0        0        0     2361 2024-04-21 07:42:53.658124 met_annot_unifier-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5768 1970-01-01 00:00:00.000000 met_annot_unifier-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-21 12:56:42.464186 met_annot_unifier-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3877 2024-04-21 12:56:42.464186 met_annot_unifier-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-21 12:56:42.480186 met_annot_unifier-0.0.2/met_annot_unifier/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-21 12:56:42.480186 met_annot_unifier-0.0.2/met_annot_unifier/aligner/__init__.py
+-rw-r--r--   0        0        0     7471 2024-04-21 12:56:42.480186 met_annot_unifier-0.0.2/met_annot_unifier/aligner/aligner.py
+-rw-r--r--   0        0        0     8044 2024-04-21 12:56:42.480186 met_annot_unifier-0.0.2/met_annot_unifier/aligner/parser.py
+-rw-r--r--   0        0        0     2832 2024-04-21 12:56:42.480186 met_annot_unifier-0.0.2/met_annot_unifier/aligner/utils.py
+-rw-r--r--   0        0        0     4896 2024-04-21 12:56:42.480186 met_annot_unifier-0.0.2/met_annot_unifier/cli.py
+-rw-r--r--   0        0        0     9472 2024-04-21 12:56:42.480186 met_annot_unifier-0.0.2/met_annot_unifier/config/column_config.json
+-rw-r--r--   0        0        0      267 2024-04-21 12:56:42.480186 met_annot_unifier-0.0.2/met_annot_unifier/foo.py
+-rw-r--r--   0        0        0     2410 2024-04-21 12:57:09.244197 met_annot_unifier-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4724 1970-01-01 00:00:00.000000 met_annot_unifier-0.0.2/PKG-INFO
```

### Comparing `met_annot_unifier-0.0.1/LICENSE` & `met_annot_unifier-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.1/README.md` & `met_annot_unifier-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: met-annot-unifier
+Version: 0.0.2
+Summary: A Python project to combine tabular outputs from GNPS, Sirius and ISDB
+Home-page: https://github.com/mapp-metabolomics-unit/met-annot-unifier
+Author: Pierre-Marie Allard
+Author-email: pierre-marie.allard@unifr.ch
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: click (>=8.1.7,<9.0.0)
+Requires-Dist: pandas (>=2.2.0,<3.0.0)
+Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
+Project-URL: Documentation, https://mapp-metabolomics-unit.github.io/met-annot-unifier/
+Project-URL: Repository, https://github.com/mapp-metabolomics-unit/met-annot-unifier
+Description-Content-Type: text/markdown
+
 # met-annot-unifier
 
 [![Release](https://img.shields.io/github/v/release/mapp-metabolomics-unit/met-annot-unifier)](https://img.shields.io/github/v/release/mapp-metabolomics-unit/met-annot-unifier)
 [![Build status](https://img.shields.io/github/actions/workflow/status/mapp-metabolomics-unit/met-annot-unifier/main.yml?branch=main)](https://github.com/mapp-metabolomics-unit/met-annot-unifier/actions/workflows/main.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/mapp-metabolomics-unit/met-annot-unifier/branch/main/graph/badge.svg)](https://codecov.io/gh/mapp-metabolomics-unit/met-annot-unifier)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/mapp-metabolomics-unit/met-annot-unifier)](https://img.shields.io/github/commit-activity/m/mapp-metabolomics-unit/met-annot-unifier)
 [![License](https://img.shields.io/github/license/mapp-metabolomics-unit/met-annot-unifier)](https://img.shields.io/github/license/mapp-metabolomics-unit/met-annot-unifier)
@@ -31,15 +50,15 @@
 
 Get help on the available modes with:
 
 ```bash
 python -m met_annot_unifier.cli --help
 ```
 
-#### Examples
+#### Align tables
 
 You can align the annotations tables from GNPS, Sirius and ISDB using two modes:
 
 - `align-horizontally`: This will return a long table with a single row for each unique compound (according to their planar structures or IK2D). This mode can be useful to output a table to be viewed in [Datawarrior](https://openmolecules.org/datawarrior/) or similar tools for chemical structures exploration.
 
 ```bash
 python -m met_annot_unifier.cli align-horizontally --gnps-file <path-to-gnps-table> --sirius-file <path-to-sirius-table> --isdb-file <path-to-isdb-table> --output <output-path>
@@ -47,50 +66,28 @@
 
 - `align-vertically`: This will return a wide table with a single row per feature (m/z and retention time) and columns for each of the three sources. This mode can be useful to output a table to be added to a molecular network to be visualized in [Cytoscape](https://cytoscape.org/) or similar tools for network visualization.
 
 ```bash
 python -m met_annot_unifier.cli align-vertically --gnps-file <path-to-gnps-table> --sirius-file <path-to-sirius-table> --isdb-file <path-to-isdb-table> --output <output-path>
 ```
 
-You can find example tables in the `examples/data` folder of this repository. So from the root of this repository you can run the following command to align the tables horizontally:
-
-```bash
-python -m met_annot_unifier.cli align-horizontally --gnps-file examples/data/gnps_output_example.tsv --sirius-file examples/data/sirius_output_example.tsv --isdb-file examples/data/isdb_output_example.tsv --output examples/data/aligned_table_horizontally.csv
-```
-
-## Getting started with your project
+#### Pruning tables
 
-First, create a repository on GitHub with the same name as this project, and then run the following commands:
+You can prune the aligned tables to remove rows with missing values in the columns of interest. This can be useful to remove rows with missing values in the columns used to merge the tables.
 
 ```bash
-git init -b main
-git add .
-git commit -m "init commit"
-git remote add origin git@github.com:mapp-metabolomics-unit/met-annot-unifier.git
-git push -u origin main
+python -m met_annot_unifier.cli prune-table --input <path-to-aligned-table> --output <output-path>
 ```
 
-Finally, install the environment and the pre-commit hooks with
+### Example
+
+You can align the GNPS, ISDB and Sirius tables found in the `examples/data/in` folder of this repository and prune them to have a Cytoscape compatible table with the following commands:
 
 ```bash
-make install
+python -m met_annot_unifier.cli align-horizontally --gnps-file examples/data/in/gnps_output_example.tsv --sirius-file examples/data/in/sirius_output_example.tsv --isdb-file examples/data/in/isdb_output_example.tsv --output examples/data/out/aligned_table_horizontally.tsv
+python -m met_annot_unifier.cli prune-table --input-file examples/data/out/aligned_table_horizontally.tsv --list-columns "minimal_cytoscape" -o examples/data/out/aligned_table_horizontally_pruned_cytoscape.tsv
 ```
 
-You are now ready to start development on your project!
-The CI/CD pipeline will be triggered when you open a pull request, merge to main, or when you create a new release.
-
-To finalize the set-up for publishing to PyPi or Artifactory, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/publishing/#set-up-for-pypi).
-For activating the automatic documentation with MkDocs, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/mkdocs/#enabling-the-documentation-on-github).
-To enable the code coverage reports, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/codecov/).
-
-## Releasing a new version
-
-- Create an API Token on [Pypi](https://pypi.org/).
-- Add the API Token to your projects secrets with the name `PYPI_TOKEN` by visiting [this page](https://github.com/mapp-metabolomics-unit/met-annot-unifier/settings/secrets/actions/new).
-- Create a [new release](https://github.com/mapp-metabolomics-unit/met-annot-unifier/releases/new) on Github.
-- Create a new tag in the form `*.*.*`.
-
-For more details, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/cicd/#how-to-trigger-a-release).
-
 ---
 
 Repository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).
+
```

### Comparing `met_annot_unifier-0.0.1/met_annot_unifier/aligner/aligner.py` & `met_annot_unifier-0.0.2/met_annot_unifier/aligner/aligner.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,20 +63,24 @@
     # Merge the dataframes on 'feature_id' and 'InChiKey' with an outer join
     combined_data = pd.concat([gnps_data, sirius_data, isdb_data], axis=0, ignore_index=True)
     # Group by 'feature_id' and 'IK2D' and combine the annotations
     merged_data = combined_data.groupby(["feature_id", "IK2D"], as_index=False).agg(
         lambda x: ", ".join(x.dropna().astype(str).unique())
     )
 
-    # Create the 'Sources' column by concatenating sirius_Source, isdb_Source, and gnps_Source
+    # Create the 'Sources' column by concatenating gnps_Source, isdb_Source, and sirius_Source
     merged_data["Sources"] = merged_data.apply(
-        lambda row: ", ".join(filter(None, [row.get("sirius_Source"), row.get("isdb_Source"), row.get("gnps_Source")])),
+        lambda row: "|".join(filter(None, [row.get("gnps_Source"), row.get("isdb_Source"), row.get("sirius_Source")])),
         axis=1,
     )
 
+    # The tools_Source columns are no longer needed. They are dropped.
+
+    merged_data.drop(columns=["gnps_Source", "isdb_Source", "sirius_Source"], inplace=True)
+
     # Create a SMILES column by choosing form the sirius_SMILES, isdb_SMILES, and gnps_smiles columns with this order of preference (sirius, isdb, gnps)
 
     merged_data["SMILES"] = merged_data.apply(
         lambda row: row.get("sirius_SMILES")
         if row.get("sirius_SMILES")
         else row.get("isdb_SMILES")
         if row.get("isdb_SMILES")
```

### Comparing `met_annot_unifier-0.0.1/met_annot_unifier/aligner/parser.py` & `met_annot_unifier-0.0.2/met_annot_unifier/aligner/parser.py`

 * *Files identical despite different names*

### Comparing `met_annot_unifier-0.0.1/pyproject.toml` & `met_annot_unifier-0.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [tool.poetry]
 name = "met-annot-unifier"
-version = "0.0.1"
+version = "0.0.2"
 description = "A Python project to combine tabular outputs from GNPS, Sirius and ISDB"
 authors = ["Pierre-Marie Allard <pierre-marie.allard@unifr.ch>"]
 repository = "https://github.com/mapp-metabolomics-unit/met-annot-unifier"
 documentation = "https://mapp-metabolomics-unit.github.io/met-annot-unifier/"
 readme = "README.md"
 packages = [
   {include = "met_annot_unifier"}
 ]
+include = ["met_annot_unifier/config/*.json"]
+
 
 [tool.poetry.dependencies]
-python = ">=3.9,<4.0"
+python = ">=3.10,<4.0"
 click = "^8.1.7"
 pandas = "^2.2.0"
 pyarrow = "^15.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
@@ -30,14 +32,15 @@
 mkdocstrings = "^0.24.0"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.2.7"
 mkdocstrings = {extras = ["python"], version = "^0.24.0"}
 
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 files = ["met_annot_unifier"]
 disallow_untyped_defs = "True"
```

### Comparing `met_annot_unifier-0.0.1/PKG-INFO` & `met_annot_unifier-0.0.2/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: met-annot-unifier
-Version: 0.0.1
-Summary: A Python project to combine tabular outputs from GNPS, Sirius and ISDB
-Home-page: https://github.com/mapp-metabolomics-unit/met-annot-unifier
-Author: Pierre-Marie Allard
-Author-email: pierre-marie.allard@unifr.ch
-Requires-Python: >=3.9,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: click (>=8.1.7,<9.0.0)
-Requires-Dist: pandas (>=2.2.0,<3.0.0)
-Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
-Project-URL: Documentation, https://mapp-metabolomics-unit.github.io/met-annot-unifier/
-Project-URL: Repository, https://github.com/mapp-metabolomics-unit/met-annot-unifier
-Description-Content-Type: text/markdown
-
 # met-annot-unifier
 
 [![Release](https://img.shields.io/github/v/release/mapp-metabolomics-unit/met-annot-unifier)](https://img.shields.io/github/v/release/mapp-metabolomics-unit/met-annot-unifier)
 [![Build status](https://img.shields.io/github/actions/workflow/status/mapp-metabolomics-unit/met-annot-unifier/main.yml?branch=main)](https://github.com/mapp-metabolomics-unit/met-annot-unifier/actions/workflows/main.yml?query=branch%3Amain)
 [![codecov](https://codecov.io/gh/mapp-metabolomics-unit/met-annot-unifier/branch/main/graph/badge.svg)](https://codecov.io/gh/mapp-metabolomics-unit/met-annot-unifier)
 [![Commit activity](https://img.shields.io/github/commit-activity/m/mapp-metabolomics-unit/met-annot-unifier)](https://img.shields.io/github/commit-activity/m/mapp-metabolomics-unit/met-annot-unifier)
 [![License](https://img.shields.io/github/license/mapp-metabolomics-unit/met-annot-unifier)](https://img.shields.io/github/license/mapp-metabolomics-unit/met-annot-unifier)
@@ -51,15 +31,15 @@
 
 Get help on the available modes with:
 
 ```bash
 python -m met_annot_unifier.cli --help
 ```
 
-#### Examples
+#### Align tables
 
 You can align the annotations tables from GNPS, Sirius and ISDB using two modes:
 
 - `align-horizontally`: This will return a long table with a single row for each unique compound (according to their planar structures or IK2D). This mode can be useful to output a table to be viewed in [Datawarrior](https://openmolecules.org/datawarrior/) or similar tools for chemical structures exploration.
 
 ```bash
 python -m met_annot_unifier.cli align-horizontally --gnps-file <path-to-gnps-table> --sirius-file <path-to-sirius-table> --isdb-file <path-to-isdb-table> --output <output-path>
@@ -67,51 +47,27 @@
 
 - `align-vertically`: This will return a wide table with a single row per feature (m/z and retention time) and columns for each of the three sources. This mode can be useful to output a table to be added to a molecular network to be visualized in [Cytoscape](https://cytoscape.org/) or similar tools for network visualization.
 
 ```bash
 python -m met_annot_unifier.cli align-vertically --gnps-file <path-to-gnps-table> --sirius-file <path-to-sirius-table> --isdb-file <path-to-isdb-table> --output <output-path>
 ```
 
-You can find example tables in the `examples/data` folder of this repository. So from the root of this repository you can run the following command to align the tables horizontally:
-
-```bash
-python -m met_annot_unifier.cli align-horizontally --gnps-file examples/data/gnps_output_example.tsv --sirius-file examples/data/sirius_output_example.tsv --isdb-file examples/data/isdb_output_example.tsv --output examples/data/aligned_table_horizontally.csv
-```
-
-## Getting started with your project
+#### Pruning tables
 
-First, create a repository on GitHub with the same name as this project, and then run the following commands:
+You can prune the aligned tables to remove rows with missing values in the columns of interest. This can be useful to remove rows with missing values in the columns used to merge the tables.
 
 ```bash
-git init -b main
-git add .
-git commit -m "init commit"
-git remote add origin git@github.com:mapp-metabolomics-unit/met-annot-unifier.git
-git push -u origin main
+python -m met_annot_unifier.cli prune-table --input <path-to-aligned-table> --output <output-path>
 ```
 
-Finally, install the environment and the pre-commit hooks with
+### Example
+
+You can align the GNPS, ISDB and Sirius tables found in the `examples/data/in` folder of this repository and prune them to have a Cytoscape compatible table with the following commands:
 
 ```bash
-make install
+python -m met_annot_unifier.cli align-horizontally --gnps-file examples/data/in/gnps_output_example.tsv --sirius-file examples/data/in/sirius_output_example.tsv --isdb-file examples/data/in/isdb_output_example.tsv --output examples/data/out/aligned_table_horizontally.tsv
+python -m met_annot_unifier.cli prune-table --input-file examples/data/out/aligned_table_horizontally.tsv --list-columns "minimal_cytoscape" -o examples/data/out/aligned_table_horizontally_pruned_cytoscape.tsv
 ```
 
-You are now ready to start development on your project!
-The CI/CD pipeline will be triggered when you open a pull request, merge to main, or when you create a new release.
-
-To finalize the set-up for publishing to PyPi or Artifactory, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/publishing/#set-up-for-pypi).
-For activating the automatic documentation with MkDocs, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/mkdocs/#enabling-the-documentation-on-github).
-To enable the code coverage reports, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/codecov/).
-
-## Releasing a new version
-
-- Create an API Token on [Pypi](https://pypi.org/).
-- Add the API Token to your projects secrets with the name `PYPI_TOKEN` by visiting [this page](https://github.com/mapp-metabolomics-unit/met-annot-unifier/settings/secrets/actions/new).
-- Create a [new release](https://github.com/mapp-metabolomics-unit/met-annot-unifier/releases/new) on Github.
-- Create a new tag in the form `*.*.*`.
-
-For more details, see [here](https://fpgmaas.github.io/cookiecutter-poetry/features/cicd/#how-to-trigger-a-release).
-
 ---
 
 Repository initiated with [fpgmaas/cookiecutter-poetry](https://github.com/fpgmaas/cookiecutter-poetry).
-
```

