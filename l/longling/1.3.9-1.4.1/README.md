# Comparing `tmp/longling-1.3.9.tar.gz` & `tmp/longling-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/longling-1.3.9.tar", last modified: Wed Jan 15 13:50:25 2020, max compression
+gzip compressed data, was "longling-1.4.1.tar", last modified: Sun Apr 21 04:53:43 2024, max compression
```

## Comparing `longling-1.3.9.tar` & `longling-1.4.1.tar`

### file list

```diff
@@ -1,203 +1,43 @@
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:25.000000 longling-1.3.9/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/Architecture/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/Architecture/cli/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       92 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/cli/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1229 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/cli/main.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1780 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/cli/units.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1901 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/cli/utils.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/Architecture/install_proj/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      171 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/install_proj/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      568 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/install_proj/docs_proj.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      561 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/install_proj/py_proj.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/Architecture/meta_docs/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/Architecture/meta_docs/docs/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       46 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/docs/.math.json
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      588 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/docs/.readthedocs.yml
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     7885 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/docs/conf.py.template
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      121 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/docs/requirements.txt
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/Architecture/meta_docs/gitignore/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1279 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/gitignore/.gitignore
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1285 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/gitignore/docs.gitignore
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1279 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/gitignore/python.gitignore
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/Architecture/meta_docs/nni/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      347 2020-01-14 08:33:11.000000 longling-1.3.9/longling/Architecture/meta_docs/nni/_config.yml
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       66 2020-01-15 13:50:05.000000 longling-1.3.9/longling/Architecture/meta_docs/nni/_search_space.json
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      100 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/.pypirc.template
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      209 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/.travis.yml
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1817 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/Makefile.template
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      455 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/pytest.ini
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      189 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/setup.cfg.template
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      310 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/setup.py.template
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      101 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3952 2020-01-14 08:33:11.000000 longling-1.3.9/longling/Architecture/install_file.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/DL/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      147 2020-01-07 08:11:00.000000 longling-1.3.9/longling/ML/DL/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3544 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/DL/ecli.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      452 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/DL/module.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2707 2020-01-07 08:11:00.000000 longling-1.3.9/longling/ML/DL/service.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/layer/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      302 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/layer/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)    24365 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/layer/attention.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1013 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/layer/highway.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      651 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/layer/normalization.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3276 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/layer/sequence.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      474 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/layer/wrapper.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/loss/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      541 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/loss/PairwiseLoss.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      883 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/loss/TimeSeriesPickLoss.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      143 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/loss/__init__.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/network/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3963 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/network/TextCNN.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1394 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/network/TransE.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      108 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/network/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       51 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/__init__.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      151 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2667 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/fit_eval.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      576 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/net.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1170 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/viz.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      365 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     6115 2020-01-07 08:11:00.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/configuration.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1636 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/etl.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)    10206 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/module.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     5162 2020-01-15 13:50:05.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/run.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)    12781 2020-01-07 08:11:00.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/ModelName.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       74 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/__init__.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/docs/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       51 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/docs/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     5357 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/docs/conf.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      100 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/docs/requirements.txt
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      114 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       35 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/requirements
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      114 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      499 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/glue.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2900 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/module.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2347 2020-01-07 08:11:00.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/parser.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/toolkit/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       51 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/toolkit/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      452 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/toolkit/ctx.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      354 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/toolkit/embedding.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1833 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/toolkit/optimizer_cfg.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      242 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/toolkit/select_exp.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      631 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/toolkit/viz.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       75 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2042 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/helper.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/PytorchHelper/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/PytorchHelper/toolkit/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       52 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/toolkit/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1207 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/toolkit/optimizer.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1439 2020-01-15 13:50:05.000000 longling-1.3.9/longling/ML/PytorchHelper/toolkit/parallel.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/sym/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      126 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/sym/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2485 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/sym/fit_eval.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      623 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/sym/net.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      345 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     6060 2020-01-15 13:50:05.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/configuration.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1624 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/etl.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     9350 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/module.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     4864 2020-01-15 13:50:05.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/run.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)    12588 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/ModelName.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       74 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/__init__.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/docs/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       51 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/docs/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     5357 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/docs/conf.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      100 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/docs/requirements.txt
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      114 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       35 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/requirements
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       75 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1727 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/module.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1058 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/parser.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      502 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/tore.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/PytorchHelper/util/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       52 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/util/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1196 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/util/sequence.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      173 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      305 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/helper.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/toolkit/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/toolkit/analyser/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      105 2020-01-15 13:50:05.000000 longling-1.3.9/longling/ML/toolkit/analyser/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)    12031 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/analyser/analyser.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1113 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/analyser/cli.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1298 2020-01-15 13:50:05.000000 longling-1.3.9/longling/ML/toolkit/analyser/select.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/toolkit/dataset/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/toolkit/dataset/splitter/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       52 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/dataset/splitter/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     4233 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/dataset/splitter/file_splitter.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3853 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/dataset/splitter/iterable_splitter.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      945 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/dataset/splitter/splitter.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      207 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/dataset/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2059 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/dataset/indicesor.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/toolkit/formatter/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     7597 2020-01-07 08:11:00.000000 longling-1.3.9/longling/ML/toolkit/formatter/EvalFormatter.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       81 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/formatter/__init__.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:25.000000 longling-1.3.9/longling/ML/toolkit/hyper_search/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       80 2020-01-14 08:33:11.000000 longling-1.3.9/longling/ML/toolkit/hyper_search/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3993 2020-01-15 13:50:05.000000 longling-1.3.9/longling/ML/toolkit/hyper_search/nni.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:25.000000 longling-1.3.9/longling/ML/toolkit/monitor/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      300 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/monitor/LossMonitor.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     4205 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/monitor/ProgressMonitor.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1457 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/monitor/ValueMonitor.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      178 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/monitor/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      165 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1618 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/equipment.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      116 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/__init__.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:25.000000 longling-1.3.9/longling/lib/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:25.000000 longling-1.3.9/longling/lib/process_pattern/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      216 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/process_pattern/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      861 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/process_pattern/condition_filter.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2687 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/process_pattern/pattener.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3041 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/process_pattern/process_pattern.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      147 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/process_pattern/process_pattern_base.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3085 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/process_pattern/variable.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:25.000000 longling-1.3.9/longling/lib/structure/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1735 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/structure/Factor.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      113 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/structure/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1413 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/structure/dict.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      249 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2713 2020-01-14 08:33:11.000000 longling-1.3.9/longling/lib/candylib.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3044 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/clock.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     6625 2020-01-14 08:33:11.000000 longling-1.3.9/longling/lib/iterator.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1807 2020-01-14 08:33:11.000000 longling-1.3.9/longling/lib/loading.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)    19531 2020-01-14 08:33:11.000000 longling-1.3.9/longling/lib/parser.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1036 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/path.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3085 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/progress.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     4530 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/stream.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2811 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/utilog.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:25.000000 longling-1.3.9/longling/spider/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:25.000000 longling-1.3.9/longling/spider/parser/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       77 2020-01-03 06:07:40.000000 longling-1.3.9/longling/spider/parser/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      503 2020-01-03 06:07:40.000000 longling-1.3.9/longling/spider/parser/lxml_parser.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       41 2020-01-03 06:07:40.000000 longling-1.3.9/longling/spider/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      113 2020-01-03 06:07:40.000000 longling-1.3.9/longling/spider/conf.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1086 2020-01-03 06:07:40.000000 longling-1.3.9/longling/spider/download_data.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2185 2020-01-14 08:33:11.000000 longling-1.3.9/longling/spider/utils.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:25.000000 longling-1.3.9/longling/toolbox/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       63 2020-01-03 06:07:40.000000 longling-1.3.9/longling/toolbox/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2628 2020-01-03 06:07:40.000000 longling-1.3.9/longling/toolbox/toc.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      652 2020-01-15 13:50:05.000000 longling-1.3.9/longling/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      321 2020-01-03 06:07:40.000000 longling-1.3.9/longling/base.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1434 2020-01-14 08:33:11.000000 longling-1.3.9/longling/main.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling.egg-info/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      928 2020-01-15 13:50:22.000000 longling-1.3.9/longling.egg-info/PKG-INFO
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     6832 2020-01-15 13:50:22.000000 longling-1.3.9/longling.egg-info/SOURCES.txt
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)        1 2020-01-15 13:50:22.000000 longling-1.3.9/longling.egg-info/dependency_links.txt
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       93 2020-01-15 13:50:22.000000 longling-1.3.9/longling.egg-info/entry_points.txt
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      457 2020-01-15 13:50:22.000000 longling-1.3.9/longling.egg-info/requires.txt
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)        9 2020-01-15 13:50:22.000000 longling-1.3.9/longling.egg-info/top_level.txt
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       93 2020-01-03 06:07:39.000000 longling-1.3.9/MANIFEST.in
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      195 2020-01-03 06:07:39.000000 longling-1.3.9/README.txt
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      235 2020-01-15 13:50:25.000000 longling-1.3.9/setup.cfg
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3646 2020-01-03 06:07:40.000000 longling-1.3.9/setup.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      928 2020-01-15 13:50:25.000000 longling-1.3.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.775459 longling-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16724 2024-04-21 04:53:40.000000 longling-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-21 04:53:40.000000 longling-1.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-21 04:53:43.775459 longling-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-21 04:53:40.000000 longling-1.4.1/README.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.767459 longling-1.4.1/longling/
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-21 04:53:40.000000 longling-1.4.1/longling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-21 04:53:40.000000 longling-1.4.1/longling/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.763460 longling-1.4.1/longling/infrastructure/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.763460 longling-1.4.1/longling/infrastructure/meta_docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.763460 longling-1.4.1/longling/infrastructure/meta_docs/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.767459 longling-1.4.1/longling/infrastructure/meta_docs/docs/mxnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-21 04:53:40.000000 longling-1.4.1/longling/infrastructure/meta_docs/docs/mxnet/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.767459 longling-1.4.1/longling/infrastructure/meta_docs/docs/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-21 04:53:40.000000 longling-1.4.1/longling/infrastructure/meta_docs/docs/sphinx/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-21 04:53:40.000000 longling-1.4.1/longling/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.767459 longling-1.4.1/longling/spider/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/download_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.767459 longling-1.4.1/longling/spider/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/lib/get_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.767459 longling-1.4.1/longling/spider/meta_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/meta_data/IPpool.json
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/meta_data/user_agents.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.767459 longling-1.4.1/longling/spider/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/parser/lxml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-21 04:53:40.000000 longling-1.4.1/longling/spider/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.767459 longling-1.4.1/longling/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-21 04:53:40.000000 longling-1.4.1/longling/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-21 04:53:40.000000 longling-1.4.1/longling/toolbox/toc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:53:43.767459 longling-1.4.1/longling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-21 04:53:43.000000 longling-1.4.1/longling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-21 04:53:43.000000 longling-1.4.1/longling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 04:53:43.000000 longling-1.4.1/longling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-21 04:53:43.000000 longling-1.4.1/longling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-21 04:53:43.000000 longling-1.4.1/longling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 04:53:43.000000 longling-1.4.1/longling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-21 04:53:43.775459 longling-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-04-21 04:53:40.000000 longling-1.4.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `longling-1.3.9/longling/spider/download_data.py` & `longling-1.4.1/longling/spider/download_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,24 +2,37 @@
 # create by tongshiwei on 2019/7/2
 
 import logging
 
 import os
 
 from urllib.request import urlretrieve
-
-try:
-    from .utils import decompress, reporthook4urlretrieve as _reporthook4urlretrieve
-except (SystemError, ModuleNotFoundError):  # pragma: no cover
-    from utils import decompress, reporthook4urlretrieve as _reporthook4urlretrieve
+from .utils import decompress, reporthook4urlretrieve as _reporthook4urlretrieve
 
 logger = logging.getLogger("spider")
 
+__all__ = ["download_file"]
+
 
 def download_file(url, save_path=None, override=True, decomp=True, reporthook=None):
+    """
+    cli alias: ``download``, download data from specified url
+
+    Parameters
+    ----------
+    url
+    save_path
+    override
+    decomp
+    reporthook
+
+    Returns
+    -------
+
+    """
     save_path = url.split('/')[-1] if not save_path else save_path
     if os.path.exists(save_path):
         if override is True:
             os.remove(save_path)
             logger.warning(save_path + ' will be overridden.')
         else:
             raise FileExistsError("%s existed, downloading abandoned" % save_path)
```

### Comparing `longling-1.3.9/longling/spider/utils.py` & `longling-1.4.1/longling/spider/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import gzip
 import shutil
 import tarfile
 import zipfile
 import rarfile
 
 from longling import flush_print
+from longling.utils.candylib import format_byte_sizeof
 
 __all__ = ["decompress", "get_path", "un_zip", "un_rar", "un_tar", "reporthook4urlretrieve"]
 
 
 def decompress(file):  # pragma: no cover
     for z in [".tar.gz", ".tar.bz2", ".tar.bz", ".tar.tgz", ".tar", ".tgz", ".zip", ".rar", ".gz"]:
         if file.endswith(z):
@@ -79,8 +80,13 @@
     Returns
     -------
 
     """
     per = 100.0 * (blocknum * bs) / size
     if per > 100:
         per = 100
-    flush_print('Downloading %.2f%% : %dB | %dB' % (per, blocknum * bs, size))
+    flush_print(
+        'Downloading %.2f%% : %s | %s' % (
+            per,
+            format_byte_sizeof(blocknum * bs),
+            format_byte_sizeof(size)
+        ))
```

### Comparing `longling-1.3.9/longling/toolbox/toc.py` & `longling-1.4.1/longling/toolbox/toc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,32 @@
 # coding: utf-8
-# reference: https://stackoverflow.com/a/49912639
 
 __all__ = ["toc"]
 
 from pathlib import Path
 
 
 def toc(root="./", parent=None, is_last=False, criteria=None):
+    """
+    打印目录树
+
+    show the tree of contents in the specified root directory
+
+    Parameters
+    ----------
+    root
+    parent
+    is_last
+    criteria
+
+    References
+    ----------
+    https://stackoverflow.com/a/49912639
+
+    """
     paths = DisplayablePath.make_tree(root, parent, is_last, criteria)
     for path in paths:
         print(path.displayable())
 
 
 class DisplayablePath(object):
     display_filename_prefix_middle = '├──'
```

### Comparing `longling-1.3.9/setup.py` & `longling-1.4.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,72 +7,64 @@
 from distutils.core import setup
 
 from setuptools import find_packages
 
 test_deps = [
     'pytest>=4',
     'pytest-cov>=2.6.0',
-    'pytest-pep8>=1',
+    'flake8'
 ]
 
-doc_deps = [
+docs_deps = [
     'sphinx',
-    'sphinx-rtd-theme',
-    'recommonmark'
+    'sphinx_rtd_theme',
+    'nbsphinx',
+    'm2r2',
+    'Image',
+    'recommonmark',
+    'ipython',
+    'sphinx_toggleprompt'
 ]
 
-dev_deps = test_deps + doc_deps + [
+dev_deps = test_deps + docs_deps + [
     'setuptools>=40',
-    'wheel'
+    'wheel',
+    'twine'
 ]
 
-ml_base_deps = [
+dm_base_deps = [
+    "pandas>=2.0",
     "numpy",
-    "scipy",
-    "sklearn",
     "matplotlib",
-    "nvidia-ml-py3",
 ]
 
-try:
-    import mxnet
-
-    mxnet_requires = []
-except ModuleNotFoundError:
-    mxnet_requires = ["mxnet"]
-except Exception as e:
-    mxnet_requires = []
-    logging.error(e)
-
-try:
-    import torch
-
-    ml_pytorch_deps = []
-except ModuleNotFoundError:
-    import sys
-
-    if 5 <= sys.version_info[1] <= 7:
-        ml_pytorch_deps = ["torch"]
-    else:
-        ml_pytorch_deps = []
-        logging.warning("Current python version %s is not supported by pytorch", str(sys.version_info[:2]))
-except Exception as e:
-    ml_pytorch_deps = []
-    logging.error(e)
+ml_base_deps = [
+    "pandas",
+    "numpy>= 1.16.5",
+    "scipy",
+    "scikit-learn",
+    "nni"
+]
+viz_deps = [
+    "matplotlib",
+    "tensorboardx",
+    "tensorboard"
+]
 
-ml_mx_deps = ["gluonnlp"] + mxnet_requires
 
 spider_deps = [
     "requests",
     "rarfile",
     "bs4",
-    "lxml"
+    "lxml",
+    "urllib3"
 ]
 
-ml_full_deps = ml_base_deps + ml_mx_deps + ml_pytorch_deps
+
+ml_full_deps = ml_base_deps + viz_deps
 
 full_deps = ml_full_deps + spider_deps
 
 
 def read(*names, **kwargs):
     with io.open(
             os.path.join(os.path.dirname(__file__), *names),
@@ -102,19 +94,15 @@
     packages=find_packages(
         include=[
             "longling",
             "*.toolbox", "*.toolbox.*",
             "*.lib", "*.lib.*",
             "*.spider", "*.spider.*",
             "*.Architecture", "*.Architecture.*",
-            "*.ML",
-            "*.ML.DL*",
-            "*.ML.MxnetHelper*",
-            "*.ML.PytorchHelper*",
-            "*.ML.toolkit*",
+            "*.ML*",
         ],
         exclude=[
             "*.mx_example", "*.gluon_example*", "*.gluon_exp*",
             "*.mxnet_old*",
         ]
     ),
     entry_points={
@@ -127,27 +115,37 @@
     license='LICENSE.txt',
     description='This project aims to provide some handy toolkit functions to help construct the architecture.',
     long_description=open('README.txt', encoding="utf-8").read(),
     install_requires=[
         "pip",
         "tqdm",
         "fire",
+        "PyYAML>=5.1",
+        "toml",
+        "multiprocess",
+        "joblib"
     ],
     extras_require={
-        'test': test_deps,
-        'doc': doc_deps,
+        'test': test_deps + full_deps,
+        'doc': docs_deps,
         'dev': dev_deps,
+        'dm': dm_base_deps,
         'ml': ml_base_deps,
+        'ml-viz': ml_base_deps + viz_deps,
+        'viz': viz_deps,
         'ml-full': ml_full_deps,
         "spider": spider_deps,
         "full": full_deps
     },
     classifiers=[
-        "Programming Language :: Python :: 3",
-        "Development Status :: 4 - Beta",
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         "Environment :: Other Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
 )
```

