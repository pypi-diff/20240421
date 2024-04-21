# Comparing `tmp/longling-1.3.8.tar.gz` & `tmp/longling-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/longling-1.3.8.tar", last modified: Tue Jan 14 08:34:13 2020, max compression
+gzip compressed data, was "dist/longling-1.3.9.tar", last modified: Wed Jan 15 13:50:25 2020, max compression
```

## Comparing `longling-1.3.8.tar` & `longling-1.3.9.tar`

### file list

```diff
@@ -1,203 +1,203 @@
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/Architecture/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/Architecture/cli/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       92 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/cli/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1229 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/cli/main.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1780 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/cli/units.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1901 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/cli/utils.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/Architecture/install_proj/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      171 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/install_proj/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      568 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/install_proj/docs_proj.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      561 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/install_proj/py_proj.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/Architecture/meta_docs/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/Architecture/meta_docs/docs/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       46 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/meta_docs/docs/.math.json
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      588 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/meta_docs/docs/.readthedocs.yml
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     7885 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/meta_docs/docs/conf.py.template
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      121 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/meta_docs/docs/requirements.txt
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/Architecture/meta_docs/gitignore/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1279 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/meta_docs/gitignore/.gitignore
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1285 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/meta_docs/gitignore/docs.gitignore
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1279 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/meta_docs/gitignore/python.gitignore
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/Architecture/meta_docs/nni/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      347 2020-01-14 08:33:11.000000 longling-1.3.8/longling/Architecture/meta_docs/nni/_config.yml
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       64 2020-01-14 08:33:11.000000 longling-1.3.8/longling/Architecture/meta_docs/nni/_search_space.json
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      100 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/meta_docs/.pypirc.template
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      209 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/meta_docs/.travis.yml
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1817 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/meta_docs/Makefile.template
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      455 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/meta_docs/pytest.ini
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      189 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/meta_docs/setup.cfg.template
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      310 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/meta_docs/setup.py.template
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      101 2020-01-03 06:07:39.000000 longling-1.3.8/longling/Architecture/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3952 2020-01-14 08:33:11.000000 longling-1.3.8/longling/Architecture/install_file.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/DL/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      147 2020-01-07 08:11:00.000000 longling-1.3.8/longling/ML/DL/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3544 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/DL/ecli.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      452 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/DL/module.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2707 2020-01-07 08:11:00.000000 longling-1.3.8/longling/ML/DL/service.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/MxnetHelper/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/MxnetHelper/gallery/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/MxnetHelper/gallery/layer/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      302 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/gallery/layer/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)    24365 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/gallery/layer/attention.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1013 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/gallery/layer/highway.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      651 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/gallery/layer/normalization.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3276 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/gallery/layer/sequence.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      474 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/gallery/layer/wrapper.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/MxnetHelper/gallery/loss/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      541 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/gallery/loss/PairwiseLoss.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      883 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/gallery/loss/TimeSeriesPickLoss.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      143 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/gallery/loss/__init__.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/MxnetHelper/gallery/network/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3963 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/gallery/network/TextCNN.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1394 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/gallery/network/TransE.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      108 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/gallery/network/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       51 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/gallery/__init__.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      151 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2667 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/fit_eval.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      576 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/net.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1170 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/viz.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      365 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     6115 2020-01-07 08:11:00.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/configuration.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1636 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/etl.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)    10206 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/module.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     4691 2020-01-07 08:11:00.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/run.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)    12781 2020-01-07 08:11:00.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/ModelName.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       74 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/__init__.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/docs/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       51 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/docs/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     5357 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/docs/conf.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      100 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/docs/requirements.txt
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      114 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       35 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/requirements
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      114 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      499 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/glue.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2900 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/module.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2347 2020-01-07 08:11:00.000000 longling-1.3.8/longling/ML/MxnetHelper/glue/parser.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/MxnetHelper/toolkit/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       51 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/toolkit/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      452 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/toolkit/ctx.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      354 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/toolkit/embedding.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1833 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/toolkit/optimizer_cfg.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      242 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/toolkit/select_exp.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      631 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/toolkit/viz.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       75 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2042 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/MxnetHelper/helper.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/PytorchHelper/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/PytorchHelper/toolkit/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       52 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/PytorchHelper/toolkit/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1207 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/PytorchHelper/toolkit/optimizer.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1235 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/PytorchHelper/toolkit/parallel.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/sym/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      126 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/sym/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2485 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/sym/fit_eval.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      623 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/sym/net.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      345 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     5914 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/configuration.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1624 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/etl.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     9350 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/module.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     4485 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/run.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)    12588 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/ModelName.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       74 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/__init__.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/docs/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       51 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/docs/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     5357 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/docs/conf.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      100 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/docs/requirements.txt
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      114 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       35 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/requirements
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       75 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1727 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/module.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1058 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/parser.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      502 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/PytorchHelper/tore/tore.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/PytorchHelper/util/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       52 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/PytorchHelper/util/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1196 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/PytorchHelper/util/sequence.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      173 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/PytorchHelper/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      305 2020-01-03 06:07:39.000000 longling-1.3.8/longling/ML/PytorchHelper/helper.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/toolkit/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/toolkit/analyser/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       81 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/toolkit/analyser/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)    12031 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/toolkit/analyser/analyser.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1113 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/toolkit/analyser/cli.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1270 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/toolkit/analyser/select.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/toolkit/dataset/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/toolkit/dataset/splitter/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       52 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/toolkit/dataset/splitter/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     4233 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/toolkit/dataset/splitter/file_splitter.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3853 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/toolkit/dataset/splitter/iterable_splitter.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      945 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/toolkit/dataset/splitter/splitter.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      207 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/toolkit/dataset/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2059 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/toolkit/dataset/indicesor.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/toolkit/formatter/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     7597 2020-01-07 08:11:00.000000 longling-1.3.8/longling/ML/toolkit/formatter/EvalFormatter.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       81 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/toolkit/formatter/__init__.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/toolkit/hyper_search/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       80 2020-01-14 08:33:11.000000 longling-1.3.8/longling/ML/toolkit/hyper_search/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2949 2020-01-14 08:33:11.000000 longling-1.3.8/longling/ML/toolkit/hyper_search/nni.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/ML/toolkit/monitor/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      300 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/toolkit/monitor/LossMonitor.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     4205 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/toolkit/monitor/ProgressMonitor.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1457 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/toolkit/monitor/ValueMonitor.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      178 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/toolkit/monitor/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      165 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/toolkit/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1618 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/toolkit/equipment.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      116 2020-01-03 06:07:40.000000 longling-1.3.8/longling/ML/__init__.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/lib/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/lib/process_pattern/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      216 2020-01-03 06:07:40.000000 longling-1.3.8/longling/lib/process_pattern/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      861 2020-01-03 06:07:40.000000 longling-1.3.8/longling/lib/process_pattern/condition_filter.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2687 2020-01-03 06:07:40.000000 longling-1.3.8/longling/lib/process_pattern/pattener.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3041 2020-01-03 06:07:40.000000 longling-1.3.8/longling/lib/process_pattern/process_pattern.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      147 2020-01-03 06:07:40.000000 longling-1.3.8/longling/lib/process_pattern/process_pattern_base.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3085 2020-01-03 06:07:40.000000 longling-1.3.8/longling/lib/process_pattern/variable.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/lib/structure/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1735 2020-01-03 06:07:40.000000 longling-1.3.8/longling/lib/structure/Factor.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      113 2020-01-03 06:07:40.000000 longling-1.3.8/longling/lib/structure/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1413 2020-01-03 06:07:40.000000 longling-1.3.8/longling/lib/structure/dict.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      249 2020-01-03 06:07:40.000000 longling-1.3.8/longling/lib/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2713 2020-01-14 08:33:11.000000 longling-1.3.8/longling/lib/candylib.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3044 2020-01-03 06:07:40.000000 longling-1.3.8/longling/lib/clock.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     6625 2020-01-14 08:33:11.000000 longling-1.3.8/longling/lib/iterator.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1807 2020-01-14 08:33:11.000000 longling-1.3.8/longling/lib/loading.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)    19531 2020-01-14 08:33:11.000000 longling-1.3.8/longling/lib/parser.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1036 2020-01-03 06:07:40.000000 longling-1.3.8/longling/lib/path.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3085 2020-01-03 06:07:40.000000 longling-1.3.8/longling/lib/progress.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     4530 2020-01-03 06:07:40.000000 longling-1.3.8/longling/lib/stream.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2811 2020-01-03 06:07:40.000000 longling-1.3.8/longling/lib/utilog.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/spider/
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/spider/parser/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       77 2020-01-03 06:07:40.000000 longling-1.3.8/longling/spider/parser/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      503 2020-01-03 06:07:40.000000 longling-1.3.8/longling/spider/parser/lxml_parser.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       41 2020-01-03 06:07:40.000000 longling-1.3.8/longling/spider/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      113 2020-01-03 06:07:40.000000 longling-1.3.8/longling/spider/conf.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1086 2020-01-03 06:07:40.000000 longling-1.3.8/longling/spider/download_data.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2185 2020-01-14 08:33:11.000000 longling-1.3.8/longling/spider/utils.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling/toolbox/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       63 2020-01-03 06:07:40.000000 longling-1.3.8/longling/toolbox/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2628 2020-01-03 06:07:40.000000 longling-1.3.8/longling/toolbox/toc.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      652 2020-01-14 08:33:11.000000 longling-1.3.8/longling/__init__.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      321 2020-01-03 06:07:40.000000 longling-1.3.8/longling/base.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1434 2020-01-14 08:33:11.000000 longling-1.3.8/longling/main.py
-drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-14 08:34:13.000000 longling-1.3.8/longling.egg-info/
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      928 2020-01-14 08:34:11.000000 longling-1.3.8/longling.egg-info/PKG-INFO
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     6832 2020-01-14 08:34:11.000000 longling-1.3.8/longling.egg-info/SOURCES.txt
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)        1 2020-01-14 08:34:11.000000 longling-1.3.8/longling.egg-info/dependency_links.txt
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       93 2020-01-14 08:34:11.000000 longling-1.3.8/longling.egg-info/entry_points.txt
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      457 2020-01-14 08:34:11.000000 longling-1.3.8/longling.egg-info/requires.txt
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)        9 2020-01-14 08:34:11.000000 longling-1.3.8/longling.egg-info/top_level.txt
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       93 2020-01-03 06:07:39.000000 longling-1.3.8/MANIFEST.in
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      195 2020-01-03 06:07:39.000000 longling-1.3.8/README.txt
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      235 2020-01-14 08:34:13.000000 longling-1.3.8/setup.cfg
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3646 2020-01-03 06:07:40.000000 longling-1.3.8/setup.py
--rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      928 2020-01-14 08:34:13.000000 longling-1.3.8/PKG-INFO
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:25.000000 longling-1.3.9/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/Architecture/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/Architecture/cli/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       92 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/cli/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1229 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/cli/main.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1780 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/cli/units.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1901 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/cli/utils.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/Architecture/install_proj/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      171 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/install_proj/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      568 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/install_proj/docs_proj.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      561 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/install_proj/py_proj.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/Architecture/meta_docs/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/Architecture/meta_docs/docs/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       46 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/docs/.math.json
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      588 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/docs/.readthedocs.yml
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     7885 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/docs/conf.py.template
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      121 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/docs/requirements.txt
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/Architecture/meta_docs/gitignore/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1279 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/gitignore/.gitignore
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1285 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/gitignore/docs.gitignore
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1279 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/gitignore/python.gitignore
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/Architecture/meta_docs/nni/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      347 2020-01-14 08:33:11.000000 longling-1.3.9/longling/Architecture/meta_docs/nni/_config.yml
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       66 2020-01-15 13:50:05.000000 longling-1.3.9/longling/Architecture/meta_docs/nni/_search_space.json
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      100 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/.pypirc.template
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      209 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/.travis.yml
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1817 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/Makefile.template
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      455 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/pytest.ini
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      189 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/setup.cfg.template
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      310 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/meta_docs/setup.py.template
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      101 2020-01-03 06:07:39.000000 longling-1.3.9/longling/Architecture/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3952 2020-01-14 08:33:11.000000 longling-1.3.9/longling/Architecture/install_file.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/DL/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      147 2020-01-07 08:11:00.000000 longling-1.3.9/longling/ML/DL/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3544 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/DL/ecli.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      452 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/DL/module.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2707 2020-01-07 08:11:00.000000 longling-1.3.9/longling/ML/DL/service.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/layer/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      302 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/layer/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)    24365 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/layer/attention.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1013 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/layer/highway.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      651 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/layer/normalization.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3276 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/layer/sequence.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      474 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/layer/wrapper.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/loss/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      541 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/loss/PairwiseLoss.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      883 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/loss/TimeSeriesPickLoss.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      143 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/loss/__init__.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/network/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3963 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/network/TextCNN.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1394 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/network/TransE.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      108 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/network/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       51 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/gallery/__init__.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      151 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2667 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/fit_eval.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      576 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/net.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1170 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/viz.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      365 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     6115 2020-01-07 08:11:00.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/configuration.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1636 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/etl.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)    10206 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/module.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     5162 2020-01-15 13:50:05.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/run.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)    12781 2020-01-07 08:11:00.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/ModelName.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       74 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/__init__.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/docs/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       51 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/docs/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     5357 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/docs/conf.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      100 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/docs/requirements.txt
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      114 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       35 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/requirements
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      114 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      499 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/glue.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2900 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/module.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2347 2020-01-07 08:11:00.000000 longling-1.3.9/longling/ML/MxnetHelper/glue/parser.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/MxnetHelper/toolkit/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       51 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/toolkit/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      452 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/toolkit/ctx.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      354 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/toolkit/embedding.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1833 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/toolkit/optimizer_cfg.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      242 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/toolkit/select_exp.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      631 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/toolkit/viz.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       75 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2042 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/MxnetHelper/helper.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/PytorchHelper/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/PytorchHelper/toolkit/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       52 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/toolkit/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1207 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/toolkit/optimizer.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1439 2020-01-15 13:50:05.000000 longling-1.3.9/longling/ML/PytorchHelper/toolkit/parallel.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/sym/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      126 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/sym/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2485 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/sym/fit_eval.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      623 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/sym/net.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      345 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     6060 2020-01-15 13:50:05.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/configuration.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1624 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/etl.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     9350 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/module.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     4864 2020-01-15 13:50:05.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/run.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)    12588 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/ModelName.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       74 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/__init__.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/docs/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       51 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/docs/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     5357 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/docs/conf.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      100 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/docs/requirements.txt
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      114 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       35 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/requirements
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       75 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1727 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/module.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1058 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/parser.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      502 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/tore/tore.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/PytorchHelper/util/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       52 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/util/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1196 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/PytorchHelper/util/sequence.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      173 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      305 2020-01-03 06:07:39.000000 longling-1.3.9/longling/ML/PytorchHelper/helper.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/toolkit/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/toolkit/analyser/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      105 2020-01-15 13:50:05.000000 longling-1.3.9/longling/ML/toolkit/analyser/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)    12031 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/analyser/analyser.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1113 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/analyser/cli.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1298 2020-01-15 13:50:05.000000 longling-1.3.9/longling/ML/toolkit/analyser/select.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/toolkit/dataset/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/toolkit/dataset/splitter/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       52 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/dataset/splitter/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     4233 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/dataset/splitter/file_splitter.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3853 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/dataset/splitter/iterable_splitter.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      945 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/dataset/splitter/splitter.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      207 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/dataset/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2059 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/dataset/indicesor.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling/ML/toolkit/formatter/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     7597 2020-01-07 08:11:00.000000 longling-1.3.9/longling/ML/toolkit/formatter/EvalFormatter.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       81 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/formatter/__init__.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:25.000000 longling-1.3.9/longling/ML/toolkit/hyper_search/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       80 2020-01-14 08:33:11.000000 longling-1.3.9/longling/ML/toolkit/hyper_search/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3993 2020-01-15 13:50:05.000000 longling-1.3.9/longling/ML/toolkit/hyper_search/nni.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:25.000000 longling-1.3.9/longling/ML/toolkit/monitor/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      300 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/monitor/LossMonitor.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     4205 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/monitor/ProgressMonitor.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1457 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/monitor/ValueMonitor.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      178 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/monitor/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      165 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1618 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/toolkit/equipment.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      116 2020-01-03 06:07:40.000000 longling-1.3.9/longling/ML/__init__.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:25.000000 longling-1.3.9/longling/lib/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:25.000000 longling-1.3.9/longling/lib/process_pattern/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      216 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/process_pattern/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      861 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/process_pattern/condition_filter.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2687 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/process_pattern/pattener.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3041 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/process_pattern/process_pattern.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      147 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/process_pattern/process_pattern_base.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3085 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/process_pattern/variable.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:25.000000 longling-1.3.9/longling/lib/structure/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1735 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/structure/Factor.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      113 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/structure/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1413 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/structure/dict.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      249 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2713 2020-01-14 08:33:11.000000 longling-1.3.9/longling/lib/candylib.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3044 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/clock.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     6625 2020-01-14 08:33:11.000000 longling-1.3.9/longling/lib/iterator.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1807 2020-01-14 08:33:11.000000 longling-1.3.9/longling/lib/loading.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)    19531 2020-01-14 08:33:11.000000 longling-1.3.9/longling/lib/parser.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1036 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/path.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3085 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/progress.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     4530 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/stream.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2811 2020-01-03 06:07:40.000000 longling-1.3.9/longling/lib/utilog.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:25.000000 longling-1.3.9/longling/spider/
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:25.000000 longling-1.3.9/longling/spider/parser/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       77 2020-01-03 06:07:40.000000 longling-1.3.9/longling/spider/parser/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      503 2020-01-03 06:07:40.000000 longling-1.3.9/longling/spider/parser/lxml_parser.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       41 2020-01-03 06:07:40.000000 longling-1.3.9/longling/spider/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      113 2020-01-03 06:07:40.000000 longling-1.3.9/longling/spider/conf.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1086 2020-01-03 06:07:40.000000 longling-1.3.9/longling/spider/download_data.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2185 2020-01-14 08:33:11.000000 longling-1.3.9/longling/spider/utils.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:25.000000 longling-1.3.9/longling/toolbox/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       63 2020-01-03 06:07:40.000000 longling-1.3.9/longling/toolbox/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     2628 2020-01-03 06:07:40.000000 longling-1.3.9/longling/toolbox/toc.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      652 2020-01-15 13:50:05.000000 longling-1.3.9/longling/__init__.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      321 2020-01-03 06:07:40.000000 longling-1.3.9/longling/base.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     1434 2020-01-14 08:33:11.000000 longling-1.3.9/longling/main.py
+drwxrwxr-x   0 tongshiwei  (1030) tongshiwei  (1030)        0 2020-01-15 13:50:24.000000 longling-1.3.9/longling.egg-info/
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      928 2020-01-15 13:50:22.000000 longling-1.3.9/longling.egg-info/PKG-INFO
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     6832 2020-01-15 13:50:22.000000 longling-1.3.9/longling.egg-info/SOURCES.txt
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)        1 2020-01-15 13:50:22.000000 longling-1.3.9/longling.egg-info/dependency_links.txt
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       93 2020-01-15 13:50:22.000000 longling-1.3.9/longling.egg-info/entry_points.txt
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      457 2020-01-15 13:50:22.000000 longling-1.3.9/longling.egg-info/requires.txt
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)        9 2020-01-15 13:50:22.000000 longling-1.3.9/longling.egg-info/top_level.txt
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)       93 2020-01-03 06:07:39.000000 longling-1.3.9/MANIFEST.in
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      195 2020-01-03 06:07:39.000000 longling-1.3.9/README.txt
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      235 2020-01-15 13:50:25.000000 longling-1.3.9/setup.cfg
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)     3646 2020-01-03 06:07:40.000000 longling-1.3.9/setup.py
+-rw-rw-r--   0 tongshiwei  (1030) tongshiwei  (1030)      928 2020-01-15 13:50:25.000000 longling-1.3.9/PKG-INFO
```

### Comparing `longling-1.3.8/longling/Architecture/cli/main.py` & `longling-1.3.9/longling/Architecture/cli/main.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/Architecture/cli/units.py` & `longling-1.3.9/longling/Architecture/cli/units.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/Architecture/cli/utils.py` & `longling-1.3.9/longling/Architecture/cli/utils.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/Architecture/install_proj/docs_proj.py` & `longling-1.3.9/longling/Architecture/install_proj/docs_proj.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/Architecture/install_proj/py_proj.py` & `longling-1.3.9/longling/Architecture/install_proj/py_proj.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/Architecture/meta_docs/docs/.readthedocs.yml` & `longling-1.3.9/longling/Architecture/meta_docs/docs/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/Architecture/meta_docs/docs/conf.py.template` & `longling-1.3.9/longling/Architecture/meta_docs/docs/conf.py.template`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/Architecture/meta_docs/gitignore/.gitignore` & `longling-1.3.9/longling/Architecture/meta_docs/gitignore/.gitignore`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/Architecture/meta_docs/gitignore/docs.gitignore` & `longling-1.3.9/longling/Architecture/meta_docs/gitignore/docs.gitignore`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/Architecture/meta_docs/gitignore/python.gitignore` & `longling-1.3.9/longling/Architecture/meta_docs/gitignore/python.gitignore`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/Architecture/meta_docs/Makefile.template` & `longling-1.3.9/longling/Architecture/meta_docs/Makefile.template`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/Architecture/install_file.py` & `longling-1.3.9/longling/Architecture/install_file.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/DL/ecli.py` & `longling-1.3.9/longling/ML/DL/ecli.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/DL/service.py` & `longling-1.3.9/longling/ML/DL/service.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/gallery/layer/attention.py` & `longling-1.3.9/longling/ML/MxnetHelper/gallery/layer/attention.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/gallery/layer/highway.py` & `longling-1.3.9/longling/ML/MxnetHelper/gallery/layer/highway.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/gallery/layer/normalization.py` & `longling-1.3.9/longling/ML/MxnetHelper/gallery/layer/normalization.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/gallery/layer/sequence.py` & `longling-1.3.9/longling/ML/MxnetHelper/gallery/layer/sequence.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/gallery/loss/PairwiseLoss.py` & `longling-1.3.9/longling/ML/MxnetHelper/gallery/loss/PairwiseLoss.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/gallery/loss/TimeSeriesPickLoss.py` & `longling-1.3.9/longling/ML/MxnetHelper/gallery/loss/TimeSeriesPickLoss.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/gallery/network/TextCNN.py` & `longling-1.3.9/longling/ML/MxnetHelper/gallery/network/TextCNN.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/gallery/network/TransE.py` & `longling-1.3.9/longling/ML/MxnetHelper/gallery/network/TransE.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/fit_eval.py` & `longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/fit_eval.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/net.py` & `longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/net.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/viz.py` & `longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/sym/viz.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/configuration.py` & `longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/configuration.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/etl.py` & `longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/etl.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/module.py` & `longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/module.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/Module/run.py` & `longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/run.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 # coding: utf-8
 # create by tongshiwei on 2019-9-1
 from longling import path_append
 
 try:
     # for python module
-    from .sym import get_net, get_bp_loss, fit_f, eval_f, net_viz
     from .etl import transform, etl, pseudo_data_iter
     from .configuration import Configuration, ConfigurationParser
+    from .sym import get_net, get_bp_loss, fit_f, eval_f
 except (ImportError, SystemError):  # pragma: no cover
     # for python script
-    from sym import get_net, get_bp_loss, fit_f, eval_f, net_viz
     from etl import transform, etl, pseudo_data_iter
     from configuration import Configuration, ConfigurationParser
+    from sym import get_net, get_bp_loss, fit_f, eval_f
 
+from longling.ML.PytorchHelper import set_device
 
-def numerical_check(_net, _cfg: Configuration, train_data, test_data, dump_result=False):  # pragma: no cover
+
+def numerical_check(_net, _cfg: Configuration, train_data, test_data, dump_result=False,
+                    reporthook=None, final_reporthook=None):  # pragma: no cover
     ctx = _cfg.ctx
-    batch_size = _cfg.batch_size
 
-    _net.initialize(ctx=ctx)
+    _net = set_device(_net, ctx)
 
-    bp_loss_f = get_bp_loss(**_cfg.loss_params)
+    bp_loss_f = get_bp_loss(ctx, **_cfg.loss_params)
     loss_function = {}
     loss_function.update(bp_loss_f)
 
-    from longling.ML.MxnetHelper.glue import module
     from longling.ML.toolkit import EvalFormatter as Formatter
     from longling.ML.toolkit import MovingLoss
     from tqdm import tqdm
 
     loss_monitor = MovingLoss(loss_function)
     progress_monitor = tqdm
     if dump_result:
@@ -43,104 +44,109 @@
             logger=validation_logger,
             dump_file=_cfg.validation_result_file,
         )
     else:
         evaluation_formatter = Formatter()
 
     # train check
-    trainer = module.Module.get_trainer(
+    from longling.ML.PytorchHelper.toolkit.optimizer import get_trainer
+    trainer = get_trainer(
         _net, optimizer=_cfg.optimizer,
         optimizer_params=_cfg.optimizer_params,
         select=_cfg.train_select
     )
 
     for epoch in range(_cfg.begin_epoch, _cfg.end_epoch):
         for batch_data in progress_monitor(train_data, "Epoch: %s" % epoch):
             fit_f(
-                net=_net, batch_size=batch_size, batch_data=batch_data,
+                net=_net, batch_data=batch_data,
                 trainer=trainer, bp_loss_f=bp_loss_f,
                 loss_function=loss_function,
                 loss_monitor=loss_monitor,
-                ctx=ctx,
             )
 
         if epoch % 1 == 0:
-            if epoch % 1 == 0:
-                print(
-                    evaluation_formatter(
-                        epoch=epoch,
-                        loss_name_value=dict(loss_monitor.items()),
-                        eval_name_value=eval_f(_net, test_data, ctx=ctx),
-                        extra_info=None,
-                        dump=True,
-                    )[0]
-                )
+            msg, data = evaluation_formatter(
+                epoch=epoch,
+                loss_name_value=dict(loss_monitor.items()),
+                eval_name_value=eval_f(_net, test_data, ctx=ctx),
+                extra_info=None,
+                dump=dump_result,
+            )
+            print(msg)
+            if reporthook is not None:
+                reporthook(data)
+
+    if final_reporthook is not None:
+        final_reporthook()
 
 
 def pseudo_numerical_check(_net, _cfg):  # pragma: no cover
-    datas = pseudo_data_iter(_cfg)
+    datas = pesudo_data_iter(_cfg)
     numerical_check(_net, _cfg, datas, datas, dump_result=False)
 
 
-def train(train_fn, test_fn, **cfg_kwargs):  # pragma: no cover
+def train(train_fn, test_fn, reporthook=None, final_reporthook=None, **cfg_kwargs):  # pragma: no cover
+    from longling.ML.toolkit.hyper_search import prepare_hyper_search
+
+    cfg_kwargs, reporthook, final_reporthook, tag = prepare_hyper_search(
+        cfg_kwargs, Configuration, reporthook, final_reporthook, primary_key="prf:avg:f1"
+    )
+
     _cfg = Configuration(**cfg_kwargs)
     _net = get_net(**_cfg.hyper_params)
 
     train_data = etl(_cfg.var2val(train_fn), params=_cfg)
     test_data = etl(_cfg.var2val(test_fn), params=_cfg)
 
     numerical_check(_net, _cfg, train_data, test_data, dump_result=True)
 
 
 def sym_run(stage: (int, str) = "viz"):  # pragma: no cover
     if isinstance(stage, str):
         stage = {
-            "viz": 0,
-            "pseudo": 1,
-            "real": 2,
-            "cli": 3,
+            "pseudo": 0,
+            "real": 1,
+            "cli": 2,
         }[stage]
 
-    if stage <= 1:
+    if stage == 0:
+        # ############################## Pesudo Test #################################
         cfg = Configuration(
-            hyper_params={}
+            hyper_params={
+            },
+            ctx="cuda:0,1,2",
         )
         net = get_net(**cfg.hyper_params)
+        pseudo_numerical_check(net, cfg)
 
-        if stage == 0:
-            # ############################## Net Visualization ###########################
-            net_viz(net, cfg, False)
-        else:
-            # ############################## Pseudo Test #################################
-            pseudo_numerical_check(net, cfg)
-
-    elif stage == 2:
+    elif stage == 1:
         # ################################# Simple Train ###############################
-        import mxnet as mx
         train(
             "$data_dir/train",
             "$data_dir/test",
-            ctx=mx.cpu(),
+            dataset="",
+            ctx="cuda:0",
             optimizer_params={
-                "learning_rate": 0.001
+                "lr": 0.001
             },
             hyper_params={
             },
             batch_size=16,
         )
 
-    elif stage == 3:
+    elif stage == 2:
         # ################################# CLI ###########################
         cfg_parser = ConfigurationParser(Configuration, commands=[train])
         cfg_kwargs = cfg_parser()
         assert "subcommand" in cfg_kwargs
         subcommand = cfg_kwargs["subcommand"]
         del cfg_kwargs["subcommand"]
         print(cfg_kwargs)
         eval("%s" % subcommand)(**cfg_kwargs)
 
     else:
         raise TypeError
 
 
-if __name__ == '__main__':  # pragma: no cover
-    sym_run("viz")
+if __name__ == '__main__':
+    sym_run("pseudo")
```

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/ModelName/ModelName.py` & `longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/ModelName/ModelName.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/glue/ModelName/docs/conf.py` & `longling-1.3.9/longling/ML/MxnetHelper/glue/ModelName/docs/conf.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/glue/module.py` & `longling-1.3.9/longling/ML/MxnetHelper/glue/module.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/glue/parser.py` & `longling-1.3.9/longling/ML/MxnetHelper/glue/parser.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/toolkit/optimizer_cfg.py` & `longling-1.3.9/longling/ML/MxnetHelper/toolkit/optimizer_cfg.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/toolkit/viz.py` & `longling-1.3.9/longling/ML/MxnetHelper/toolkit/viz.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/MxnetHelper/helper.py` & `longling-1.3.9/longling/ML/MxnetHelper/helper.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/PytorchHelper/toolkit/optimizer.py` & `longling-1.3.9/longling/ML/PytorchHelper/toolkit/optimizer.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/PytorchHelper/toolkit/parallel.py` & `longling-1.3.9/longling/ML/PytorchHelper/toolkit/parallel.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 # coding: utf-8
 # create by tongshiwei on 2019-8-30
+import logging
 import torch
 from torch.nn import DataParallel
 
 
 def set_device(_net, ctx, **kwargs):
     if ctx == "cpu":
         return _net
     elif any(map(lambda x: x in ctx, ["cuda", "gpu"])):
         if not torch.cuda.is_available():
             try:
                 torch.ones((1,), device=torch.device("cuda: 0"))
             except AssertionError as e:
                 raise TypeError("no cuda detected, noly cpu is supported, the detailed error msg:%s" % str(e))
-        if torch.cuda.device_count() > 1:
+        if torch.cuda.device_count() >= 1:
             if ":" in ctx:
                 ctx_name, device_ids = ctx.split(":")
                 assert ctx_name in ["cuda", "gpu"], "the equipment should be 'cpu', 'cuda' or 'gpu', now is %s" % ctx
                 device_ids = [int(i) for i in device_ids.strip().split(",")]
-                return DataParallel(_net, device_ids).cuda()
+                try:
+                    return DataParallel(_net, device_ids).cuda()
+                except AssertionError as e:
+                    logging.error(device_ids)
+                    raise e
             elif ctx in ["cuda", "gpu"]:
                 return DataParallel(_net).cuda()
             else:
                 raise TypeError("the equipment should be 'cpu', 'cuda' or 'gpu', now is %s" % ctx)
         else:
+            print(torch.cuda.device_count())
             raise TypeError("0 gpu can be used, use cpu")
     else:
         return DataParallel(_net, device_ids=ctx).cuda()
```

### Comparing `longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/sym/fit_eval.py` & `longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/sym/fit_eval.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/sym/net.py` & `longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/sym/net.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/configuration.py` & `longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/configuration.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,19 +20,19 @@
     model_name = str(pathlib.Path(__file__).parents[1].name)
 
     root = pathlib.Path(__file__).parents[3]
     dataset = ""
     timestamp = datetime.datetime.now().strftime("%Y%m%d%H%M%S")
     workspace = ""
 
-    root_data_dir = "$root/data/$dataset" if dataset else "$root/data"
-    data_dir = "$root_data_dir/data"
-    root_model_dir = "$root_data_dir/model/$model_name"
-    model_dir = "$root_model_dir/$workspace" if workspace else root_model_dir
-    cfg_path = "$model_dir/configuration.json"
+    root_data_dir = path_append("$root", "data", "$dataset") if dataset else path_append("$root", "data")
+    data_dir = path_append("$root_data_dir", "data")
+    root_model_dir = path_append("$root_data_dir", "model", "$model_name")
+    model_dir = path_append("$root_model_dir", "$workspace") if workspace else root_model_dir
+    cfg_path = path_append("$model_dir", "configuration.json")
 
     root = str(root)
     root_data_dir = str(root_data_dir)
     root_model_dir = str(root_model_dir)
 
     # 训练参数设置
     begin_epoch = 0
@@ -102,35 +102,35 @@
         )
 
         params = self.class_var
         if params_json:
             params.update(self.load_cfg(params_json=params_json))
         params.update(**kwargs)
 
-        for param, value in params.items():
-            setattr(self, "%s" % param, value)
-
         # path_override_check
         path_check_list = ["dataset", "root_data_dir", "workspace", "root_model_dir", "model_dir"]
         _overridden = {}
         for path_check in path_check_list:
-            _overridden[path_check] = False if kwargs.get(path_check) == getattr(self, "%s" % path_check) else True
+            if kwargs.get(path_check) is None or kwargs[path_check] == getattr(self, "%s" % path_check):
+                _overridden[path_check] = False
+            else:
+                _overridden[path_check] = True
 
         for param, value in params.items():
             setattr(self, "%s" % param, value)
 
         def is_overridden(varname):
             return _overridden["%s" % varname]
 
         # set dataset
         if is_overridden("dataset") and not is_overridden("root_data_dir"):
-            kwargs["root_data_dir"] = "$root/data/$dataset"
+            kwargs["root_data_dir"] = path_append("$root", "data", "$dataset")
         # set workspace
         if (is_overridden("workspace") or is_overridden("root_model_dir")) and not is_overridden("model_dir"):
-            kwargs["model_dir"] = "$root_model_dir/$workspace"
+            kwargs["model_dir"] = path_append("$root_model_dir", "workspace")
 
         # rebuild relevant directory or file path according to the kwargs
         _dirs = [
             "workspace", "root_data_dir", "data_dir", "root_model_dir",
             "model_dir"
         ]
         for _dir in _dirs:
```

### Comparing `longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/etl.py` & `longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/etl.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/module.py` & `longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/Module/module.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/ModelName/ModelName.py` & `longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/ModelName/ModelName.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/PytorchHelper/tore/ModelName/docs/conf.py` & `longling-1.3.9/longling/ML/PytorchHelper/tore/ModelName/docs/conf.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/PytorchHelper/tore/module.py` & `longling-1.3.9/longling/ML/PytorchHelper/tore/module.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/PytorchHelper/tore/parser.py` & `longling-1.3.9/longling/ML/PytorchHelper/tore/parser.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/PytorchHelper/util/sequence.py` & `longling-1.3.9/longling/ML/PytorchHelper/util/sequence.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/toolkit/analyser/analyser.py` & `longling-1.3.9/longling/ML/toolkit/analyser/analyser.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/toolkit/analyser/cli.py` & `longling-1.3.9/longling/ML/toolkit/analyser/cli.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/toolkit/analyser/select.py` & `longling-1.3.9/longling/ML/toolkit/analyser/select.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 # 2019/12/20 @ tongshiwei
 
 import json
 from longling.lib.candylib import as_list
 from longling import PATH_TYPE, loading
 
-__all__ = ["get_max"]
+__all__ = ["get_max", "key_parser", "get_by_key"]
 
 
 def key_parser(key):
     if ":" in key:
         # prf:0:f1
         return key.split(":")
     return key
```

### Comparing `longling-1.3.8/longling/ML/toolkit/dataset/splitter/file_splitter.py` & `longling-1.3.9/longling/ML/toolkit/dataset/splitter/file_splitter.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/toolkit/dataset/splitter/iterable_splitter.py` & `longling-1.3.9/longling/ML/toolkit/dataset/splitter/iterable_splitter.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/toolkit/dataset/splitter/splitter.py` & `longling-1.3.9/longling/ML/toolkit/dataset/splitter/splitter.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/toolkit/dataset/indicesor.py` & `longling-1.3.9/longling/ML/toolkit/dataset/indicesor.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/toolkit/formatter/EvalFormatter.py` & `longling-1.3.9/longling/ML/toolkit/formatter/EvalFormatter.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/toolkit/monitor/ProgressMonitor.py` & `longling-1.3.9/longling/ML/toolkit/monitor/ProgressMonitor.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/toolkit/monitor/ValueMonitor.py` & `longling-1.3.9/longling/ML/toolkit/monitor/ValueMonitor.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/ML/toolkit/equipment.py` & `longling-1.3.9/longling/ML/toolkit/equipment.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/lib/process_pattern/condition_filter.py` & `longling-1.3.9/longling/lib/process_pattern/condition_filter.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/lib/process_pattern/pattener.py` & `longling-1.3.9/longling/lib/process_pattern/pattener.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/lib/process_pattern/process_pattern.py` & `longling-1.3.9/longling/lib/process_pattern/process_pattern.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/lib/process_pattern/variable.py` & `longling-1.3.9/longling/lib/process_pattern/variable.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/lib/structure/Factor.py` & `longling-1.3.9/longling/lib/structure/Factor.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/lib/structure/dict.py` & `longling-1.3.9/longling/lib/structure/dict.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/lib/candylib.py` & `longling-1.3.9/longling/lib/candylib.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/lib/clock.py` & `longling-1.3.9/longling/lib/clock.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/lib/iterator.py` & `longling-1.3.9/longling/lib/iterator.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/lib/loading.py` & `longling-1.3.9/longling/lib/loading.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/lib/parser.py` & `longling-1.3.9/longling/lib/parser.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/lib/path.py` & `longling-1.3.9/longling/lib/path.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/lib/progress.py` & `longling-1.3.9/longling/lib/progress.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/lib/stream.py` & `longling-1.3.9/longling/lib/stream.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/lib/utilog.py` & `longling-1.3.9/longling/lib/utilog.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/spider/download_data.py` & `longling-1.3.9/longling/spider/download_data.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/spider/utils.py` & `longling-1.3.9/longling/spider/utils.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/toolbox/toc.py` & `longling-1.3.9/longling/toolbox/toc.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling/__init__.py` & `longling-1.3.9/longling/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 from longling.lib import process_pattern
 from longling.lib import stream
 from longling.lib import utilog
 from longling.lib import candylib
 from longling.lib import path
 from longling.lib import parser
 
-__version__ = '1.3.8'
+__version__ = '1.3.9'
```

### Comparing `longling-1.3.8/longling/main.py` & `longling-1.3.9/longling/main.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/longling.egg-info/PKG-INFO` & `longling-1.3.9/longling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: longling
-Version: 1.3.8
+Version: 1.3.9
 Summary: This project aims to provide some handy toolkit functions to help construct the architecture.
 Home-page: https://gitlab.com/tswsxk/longling.git
 Author: Sherlock, Shiwei Tong
 Author-email: tongsw@mail.ustc.edu.cn
 License: LICENSE.txt
 Description: This project aims to provide some handy toolkit functions to help construct the architecture.
         Tutorial and full documentation can be found in https://longling.readthedocs.io/zh/latest/index.html.
```

### Comparing `longling-1.3.8/longling.egg-info/SOURCES.txt` & `longling-1.3.9/longling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/setup.py` & `longling-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `longling-1.3.8/PKG-INFO` & `longling-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: longling
-Version: 1.3.8
+Version: 1.3.9
 Summary: This project aims to provide some handy toolkit functions to help construct the architecture.
 Home-page: https://gitlab.com/tswsxk/longling.git
 Author: Sherlock, Shiwei Tong
 Author-email: tongsw@mail.ustc.edu.cn
 License: LICENSE.txt
 Description: This project aims to provide some handy toolkit functions to help construct the architecture.
         Tutorial and full documentation can be found in https://longling.readthedocs.io/zh/latest/index.html.
```

