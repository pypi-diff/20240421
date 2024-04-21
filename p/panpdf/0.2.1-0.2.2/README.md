# Comparing `tmp/panpdf-0.2.1.tar.gz` & `tmp/panpdf-0.2.2.tar.gz`

## Comparing `panpdf-0.2.1.tar` & `panpdf-0.2.2.tar`

### file list

```diff
@@ -1,70 +1,72 @@
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 panpdf-0.2.1/.gitattributes
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 panpdf-0.2.1/mkdocs.yml
--rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 panpdf-0.2.1/ruff_defaults.toml
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 panpdf-0.2.1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 panpdf-0.2.1/.devcontainer/postCreate.sh
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 panpdf-0.2.1/.devcontainer/starship.toml
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 panpdf-0.2.1/.devcontainer/features/zotero/devcontainer-feature.json
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpdf-0.2.1/.devcontainer/features/zotero/install.sh
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 panpdf-0.2.1/examples/defaults.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.1/examples/include-after-body.tex
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.1/examples/include-before-body.tex
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 panpdf-0.2.1/examples/include-in-header.tex
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.2.1/examples/images/figure.tex
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.2.1/examples/images/header.tex
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 panpdf-0.2.1/examples/src/1.md
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 panpdf-0.2.1/examples/src/2.md
--rw-r--r--   0        0        0    30244 2020-02-02 00:00:00.000000 panpdf-0.2.1/notebooks/backend.ipynb
--rw-r--r--   0        0        0    28432 2020-02-02 00:00:00.000000 panpdf-0.2.1/notebooks/hvplot.ipynb
--rw-r--r--   0        0        0    37281 2020-02-02 00:00:00.000000 panpdf-0.2.1/notebooks/pdf.ipynb
--rw-r--r--   0        0        0    67211 2020-02-02 00:00:00.000000 panpdf-0.2.1/notebooks/pgf.ipynb
--rw-r--r--   0        0        0    29602 2020-02-02 00:00:00.000000 panpdf-0.2.1/notebooks/png.ipynb
--rw-r--r--   0        0        0    54421 2020-02-02 00:00:00.000000 panpdf-0.2.1/notebooks/seaborn.ipynb
--rw-r--r--   0        0        0    55134 2020-02-02 00:00:00.000000 panpdf-0.2.1/notebooks/svg.ipynb
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/__init__.py
--rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/formatters.py
--rw-r--r--   0        0        0     8550 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/main.py
--rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/stores.py
--rw-r--r--   0        0        0     9878 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/filters/__init__.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/filters/attribute.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/filters/crossref.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/filters/filter.py
--rw-r--r--   0        0        0     5783 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/filters/jupyter.py
--rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/filters/layout.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/filters/verbatim.py
--rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 panpdf-0.2.1/src/panpdf/filters/zotero.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/test_converters.py
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/test_formatters.py
--rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/test_main.py
--rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/test_stores.py
--rw-r--r--   0        0        0     8282 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/test_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/filters/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/filters/conftest.py
--rw-r--r--   0        0        0     7279 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/filters/test_attribute.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/filters/test_crossref.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/filters/test_filter.py
--rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/filters/test_jupyter.py
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/filters/test_layout.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/filters/test_verbatim.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/filters/test_zotero.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/test_nbformat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/__init__.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/test_cite.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/test_code.py
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/test_figure.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/test_math.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/test_metadata.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/test_raw.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/test_section.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/test_table.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 panpdf-0.2.1/tests/libraries/panflute/test_tex.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 panpdf-0.2.1/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 panpdf-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 panpdf-0.2.1/README.md
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 panpdf-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 panpdf-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 panpdf-0.2.2/.gitattributes
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 panpdf-0.2.2/mkdocs.yml
+-rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 panpdf-0.2.2/ruff_defaults.toml
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 panpdf-0.2.2/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 panpdf-0.2.2/.devcontainer/postCreate.sh
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 panpdf-0.2.2/.devcontainer/starship.toml
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 panpdf-0.2.2/.devcontainer/features/zotero/devcontainer-feature.json
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 panpdf-0.2.2/.devcontainer/features/zotero/install.sh
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 panpdf-0.2.2/examples/defaults.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.2/examples/include-after-body.tex
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.2/examples/include-before-body.tex
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 panpdf-0.2.2/examples/include-in-header.tex
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.2.2/examples/images/figure.tex
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.2.2/examples/images/header.tex
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 panpdf-0.2.2/examples/src/1.md
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 panpdf-0.2.2/examples/src/2.md
+-rw-r--r--   0        0        0    30244 2020-02-02 00:00:00.000000 panpdf-0.2.2/notebooks/backend.ipynb
+-rw-r--r--   0        0        0    28432 2020-02-02 00:00:00.000000 panpdf-0.2.2/notebooks/hvplot.ipynb
+-rw-r--r--   0        0        0    37281 2020-02-02 00:00:00.000000 panpdf-0.2.2/notebooks/pdf.ipynb
+-rw-r--r--   0        0        0    67211 2020-02-02 00:00:00.000000 panpdf-0.2.2/notebooks/pgf.ipynb
+-rw-r--r--   0        0        0    29602 2020-02-02 00:00:00.000000 panpdf-0.2.2/notebooks/png.ipynb
+-rw-r--r--   0        0        0    62999 2020-02-02 00:00:00.000000 panpdf-0.2.2/notebooks/raster.ipynb
+-rw-r--r--   0        0        0    54421 2020-02-02 00:00:00.000000 panpdf-0.2.2/notebooks/seaborn.ipynb
+-rw-r--r--   0        0        0    55134 2020-02-02 00:00:00.000000 panpdf-0.2.2/notebooks/svg.ipynb
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panpdf-0.2.2/src/panpdf/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.2/src/panpdf/__init__.py
+-rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 panpdf-0.2.2/src/panpdf/formatters.py
+-rw-r--r--   0        0        0     8550 2020-02-02 00:00:00.000000 panpdf-0.2.2/src/panpdf/main.py
+-rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 panpdf-0.2.2/src/panpdf/stores.py
+-rw-r--r--   0        0        0    10188 2020-02-02 00:00:00.000000 panpdf-0.2.2/src/panpdf/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.2/src/panpdf/filters/__init__.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 panpdf-0.2.2/src/panpdf/filters/attribute.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.2.2/src/panpdf/filters/crossref.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 panpdf-0.2.2/src/panpdf/filters/filter.py
+-rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 panpdf-0.2.2/src/panpdf/filters/jupyter.py
+-rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 panpdf-0.2.2/src/panpdf/filters/layout.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 panpdf-0.2.2/src/panpdf/filters/verbatim.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 panpdf-0.2.2/src/panpdf/filters/zotero.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/test_converters.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/test_formatters.py
+-rw-r--r--   0        0        0     4432 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/test_main.py
+-rw-r--r--   0        0        0     3608 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/test_stores.py
+-rw-r--r--   0        0        0     8408 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/test_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/filters/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/filters/conftest.py
+-rw-r--r--   0        0        0     7279 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/filters/test_attribute.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/filters/test_crossref.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/filters/test_filter.py
+-rw-r--r--   0        0        0     5673 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/filters/test_jupyter.py
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/filters/test_layout.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/filters/test_verbatim.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/filters/test_zotero.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/libraries/__init__.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/libraries/test_matplotlib.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/libraries/test_nbformat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/libraries/panflute/__init__.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/libraries/panflute/test_cite.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/libraries/panflute/test_code.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/libraries/panflute/test_figure.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/libraries/panflute/test_math.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/libraries/panflute/test_metadata.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/libraries/panflute/test_raw.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/libraries/panflute/test_section.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/libraries/panflute/test_table.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 panpdf-0.2.2/tests/libraries/panflute/test_tex.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 panpdf-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 panpdf-0.2.2/LICENSE.txt
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 panpdf-0.2.2/README.md
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 panpdf-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 panpdf-0.2.2/PKG-INFO
```

### Comparing `panpdf-0.2.1/mkdocs.yml` & `panpdf-0.2.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/ruff_defaults.toml` & `panpdf-0.2.2/ruff_defaults.toml`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/.devcontainer/devcontainer.json` & `panpdf-0.2.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/.devcontainer/starship.toml` & `panpdf-0.2.2/.devcontainer/starship.toml`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/examples/defaults.yaml` & `panpdf-0.2.2/examples/defaults.yaml`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/examples/include-in-header.tex` & `panpdf-0.2.2/examples/include-in-header.tex`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/examples/src/1.md` & `panpdf-0.2.2/examples/src/1.md`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/notebooks/backend.ipynb` & `panpdf-0.2.2/notebooks/backend.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/notebooks/hvplot.ipynb` & `panpdf-0.2.2/notebooks/hvplot.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/notebooks/pdf.ipynb` & `panpdf-0.2.2/notebooks/pdf.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/notebooks/pgf.ipynb` & `panpdf-0.2.2/notebooks/pgf.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/notebooks/png.ipynb` & `panpdf-0.2.2/notebooks/png.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/notebooks/seaborn.ipynb` & `panpdf-0.2.2/notebooks/seaborn.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/notebooks/svg.ipynb` & `panpdf-0.2.2/notebooks/svg.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/src/panpdf/main.py` & `panpdf-0.2.2/src/panpdf/main.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/src/panpdf/stores.py` & `panpdf-0.2.2/src/panpdf/stores.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/src/panpdf/tools.py` & `panpdf-0.2.2/src/panpdf/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,26 @@
         path.write_bytes(text)
 
     os.close(fd)
     atexit.register(lambda: path.unlink(missing_ok=True))
     return path
 
 
+def create_temp_dir(
+    *,
+    suffix: str | None = None,
+    prefix: str = TEMPFILE_PREFIX,
+    dir: str | Path | None = None,  # noqa: A002
+) -> Path:
+    dirname = tempfile.mkdtemp(suffix, prefix, dir)
+    path = Path(dirname)
+    atexit.register(lambda: shutil.rmtree(path))
+    return path
+
+
 def get_file_path(name: Path | str | None, dir: str) -> Path | None:  # noqa: A002
     if not name:
         return None
 
     if (path := Path(name)).exists():
         return path
```

### Comparing `panpdf-0.2.1/src/panpdf/filters/attribute.py` & `panpdf-0.2.2/src/panpdf/filters/attribute.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/src/panpdf/filters/crossref.py` & `panpdf-0.2.2/src/panpdf/filters/crossref.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/src/panpdf/filters/filter.py` & `panpdf-0.2.2/src/panpdf/filters/filter.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/src/panpdf/filters/jupyter.py` & `panpdf-0.2.2/src/panpdf/filters/jupyter.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pathlib import Path
 from typing import Any, ClassVar
 
 import yaml
 from panflute import Doc, Image, Plain, RawInline
 
 from panpdf.filters.filter import Filter
+from panpdf.formatters import convert_pgf_text
 from panpdf.stores import Store
 from panpdf.tools import add_metadata_list, convert_doc, create_temp_file
 
 PGF_PREFIX = "%% Creator: Matplotlib"
 
 
 @dataclass(repr=False)
@@ -46,15 +47,15 @@
         if not (url_or_text := create_image_file(data, standalone=self.standalone)):
             return image
 
         if not url_or_text.startswith(PGF_PREFIX):
             image.url = url_or_text
             return image
 
-        text = url_or_text
+        text = convert_pgf_text(url_or_text)
 
         if not self.preamble:
             self.preamble = get_preamble(text)
 
         if not self.standalone:
             image.url = text
             self.pgf = True
```

### Comparing `panpdf-0.2.1/src/panpdf/filters/layout.py` & `panpdf-0.2.2/src/panpdf/filters/layout.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/src/panpdf/filters/verbatim.py` & `panpdf-0.2.2/src/panpdf/filters/verbatim.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/src/panpdf/filters/zotero.py` & `panpdf-0.2.2/src/panpdf/filters/zotero.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/conftest.py` & `panpdf-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/test_converters.py` & `panpdf-0.2.2/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/test_formatters.py` & `panpdf-0.2.2/tests/test_formatters.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import base64
 import io
+import re
+from pathlib import Path
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
+import numpy as np
+import pytest
 import seaborn.objects as so
 from IPython.core.formatters import PlainTextFormatter
 from IPython.core.interactiveshell import InteractiveShell
 from IPython.lib.pretty import RepresentationPrinter
 
 mpl.use("agg")
 
@@ -89,7 +93,65 @@
     assert func is matplotlib_figure_to_pgf
 
 
 def test_set_formatter_none():
     from panpdf.formatters import set_formatter
 
     set_formatter("matplotlib", "pgf")
+
+
+@pytest.fixture(scope="module")
+def text():
+    from panpdf.formatters import matplotlib_figure_to_pgf
+
+    data = np.random.randn(50, 50)
+    fig, ax = plt.subplots(figsize=(3, 2))
+    a = ax.imshow(data, interpolation="nearest", aspect=1)
+    ax.set(xlabel="x", ylabel="α")
+    fig.colorbar(a)
+
+    out = io.StringIO()
+    rp = RepresentationPrinter(out)
+
+    matplotlib_figure_to_pgf(fig, rp, None)
+    return out.getvalue()
+
+
+def test_matplotlib_figure_to_pgf_raster(text: str):
+    assert "\n%% __panpdf_begin__\n" in text
+    assert text.endswith("%% __panpdf_end__")
+
+
+def test_split_pgf_text(text: str):
+    from panpdf.formatters import split_pgf_text
+
+    text, image_dict = split_pgf_text(text)
+    assert text.startswith("%% Creator: Matplotlib, PGF backend")
+    assert text.endswith("\\endgroup%\n")
+
+    for name, data in image_dict.items():
+        assert name in text
+        assert data.startswith("iVBOR")
+        assert not data.endswith("\n")
+
+
+def test_split_pgf_text_none():
+    from panpdf.formatters import split_pgf_text
+
+    text, image_dict = split_pgf_text("abc")
+    assert text == "abc"
+    assert not image_dict
+
+
+def test_convert_pgf_text(text: str):
+    from panpdf.formatters import convert_pgf_text
+
+    text = convert_pgf_text(text)
+
+    for x in re.findall(r"\\includegraphics\[.+?\]{(.+?)}", text):
+        assert Path(x).exists()
+
+
+def test_convert_pgf_text_none():
+    from panpdf.formatters import convert_pgf_text
+
+    assert convert_pgf_text("abc") == "abc"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `panpdf-0.2.1/tests/test_main.py` & `panpdf-0.2.2/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/test_stores.py` & `panpdf-0.2.2/tests/test_stores.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/test_tools.py` & `panpdf-0.2.2/tests/test_tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,25 +39,32 @@
 def test_get_data_dir():
     from panpdf.tools import get_data_dir
 
     assert get_data_dir().name == "pandoc"
 
 
 @pytest.mark.parametrize("text", ["abcあα", b"abc"])
-def test_create_temp_file(text):
+def test_create_temp_file(text, tmp_path):
     from panpdf.tools import create_temp_file
 
-    with tempfile.TemporaryDirectory() as tmpdir:
-        path = create_temp_file(text, suffix=".txt", dir=tmpdir)
-        assert path.exists()
-        assert path.suffix == ".txt"
-        if isinstance(text, str):
-            assert path.read_text(encoding="utf8") == text
-        else:
-            assert path.read_bytes() == text
+    path = create_temp_file(text, suffix=".txt", dir=tmp_path)
+    assert path.exists()
+    assert path.suffix == ".txt"
+    if isinstance(text, str):
+        assert path.read_text(encoding="utf8") == text
+    else:
+        assert path.read_bytes() == text
+
+
+def test_create_temp_dir(tmp_path):
+    from panpdf.tools import create_temp_dir
+
+    path = create_temp_dir(dir=tmp_path)
+    assert path.exists()
+    assert path.parent == tmp_path
 
 
 def test_get_file_path():
     from panpdf.tools import get_file_path
 
     assert get_file_path(None, "") is None
     path = Path(__file__)
```

### Comparing `panpdf-0.2.1/tests/filters/test_attribute.py` & `panpdf-0.2.2/tests/filters/test_attribute.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/filters/test_crossref.py` & `panpdf-0.2.2/tests/filters/test_crossref.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/filters/test_filter.py` & `panpdf-0.2.2/tests/filters/test_filter.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/filters/test_jupyter.py` & `panpdf-0.2.2/tests/filters/test_jupyter.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,14 +92,20 @@
     text = data["text/plain"]
     preamble = get_preamble(text)
     assert r"\def\mathdefault#1{#1}" in preamble
     assert r"\usepackage[strings]{underscore}" in preamble
     assert r"\setmainfont" not in preamble
 
 
+def test_get_preamble_none():
+    from panpdf.filters.jupyter import get_preamble
+
+    assert get_preamble("") == ""
+
+
 @pytest.mark.parametrize("use_defaults", [False, True])
 def test_create_image_file_pgf(store: Store, defaults, use_defaults):
     from panpdf.filters.jupyter import create_image_file_pgf, get_preamble
 
     data = store.get_data("pgf.ipynb", "fig:pgf")
     text = data["text/plain"]
     defaults = defaults if use_defaults else None
@@ -173,7 +179,22 @@
     from panpdf.filters.jupyter import Jupyter
 
     doc = Doc()
     jupyter = Jupyter()
     image = Image(Str("a"), url="a.ipynb", identifier="a")
     with pytest.raises(ValueError, match=r"\[panpdf\] Unknown"):
         jupyter.action(image, doc)
+
+
+@pytest.mark.parametrize("pgf", [True, False])
+def test_jupyter_finalize(pgf):
+    from panpdf.filters.jupyter import Jupyter
+
+    doc = Doc()
+    jupyter = Jupyter()
+    jupyter.pgf = pgf
+    jupyter.finalize(doc)
+    x = doc.metadata.get("include-in-header")
+    if pgf:
+        assert x
+    else:
+        assert not x
```

### Comparing `panpdf-0.2.1/tests/filters/test_layout.py` & `panpdf-0.2.2/tests/filters/test_layout.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/filters/test_verbatim.py` & `panpdf-0.2.2/tests/filters/test_verbatim.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/filters/test_zotero.py` & `panpdf-0.2.2/tests/filters/test_zotero.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/libraries/test_nbformat.py` & `panpdf-0.2.2/tests/libraries/test_nbformat.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/libraries/panflute/test_cite.py` & `panpdf-0.2.2/tests/libraries/panflute/test_cite.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/libraries/panflute/test_code.py` & `panpdf-0.2.2/tests/libraries/panflute/test_code.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/libraries/panflute/test_figure.py` & `panpdf-0.2.2/tests/libraries/panflute/test_figure.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/libraries/panflute/test_math.py` & `panpdf-0.2.2/tests/libraries/panflute/test_math.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/libraries/panflute/test_metadata.py` & `panpdf-0.2.2/tests/libraries/panflute/test_metadata.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/libraries/panflute/test_raw.py` & `panpdf-0.2.2/tests/libraries/panflute/test_raw.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/libraries/panflute/test_section.py` & `panpdf-0.2.2/tests/libraries/panflute/test_section.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/libraries/panflute/test_table.py` & `panpdf-0.2.2/tests/libraries/panflute/test_table.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/tests/libraries/panflute/test_tex.py` & `panpdf-0.2.2/tests/libraries/panflute/test_tex.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/LICENSE.txt` & `panpdf-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/README.md` & `panpdf-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/pyproject.toml` & `panpdf-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panpdf-0.2.1/PKG-INFO` & `panpdf-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: panpdf
-Version: 0.2.1
+Version: 0.2.2
 Summary: PDF documentation generator
 Project-URL: Documentation, https://daizutabi.github.io/panpdf
 Project-URL: Source, https://github.com/daizutabi/panpdf
 Project-URL: Issues, https://github.com/daizutabi/panpdf/issues
 Author-email: daizutabi <daizutabi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

