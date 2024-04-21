# Comparing `tmp/relatorio-0.9.2.tar.gz` & `tmp/relatorio-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/relatorio-0.9.2.tar", last modified: Thu Aug  6 07:10:42 2020, max compression
+gzip compressed data, was "relatorio-0.9.3.tar", last modified: Fri May  7 11:52:49 2021, max compression
```

## Comparing `relatorio-0.9.2.tar` & `relatorio-0.9.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2020-08-06 07:10:42.000000 relatorio-0.9.2/
--rw-r--r--   0 ced       (1000) ced       (1000)      684 2019-12-26 09:42:44.000000 relatorio-0.9.2/.drone.yml
--rw-r--r--   0 ced       (1000) ced       (1000)       41 2020-02-29 23:31:40.000000 relatorio-0.9.2/.flake8
--rw-r--r--   0 ced       (1000) ced       (1000)      157 2018-08-18 11:27:26.000000 relatorio-0.9.2/.hgignore
--rw-r--r--   0 ced       (1000) ced       (1000)     1410 2020-08-06 07:09:30.000000 relatorio-0.9.2/.hgtags
--rw-r--r--   0 ced       (1000) ced       (1000)     4192 2020-08-06 07:09:14.000000 relatorio-0.9.2/CHANGELOG
--rw-r--r--   0 ced       (1000) ced       (1000)      834 2020-02-23 16:24:17.000000 relatorio-0.9.2/COPYRIGHT
--rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 11:27:26.000000 relatorio-0.9.2/LICENSE
--rw-r--r--   0 ced       (1000) ced       (1000)       81 2020-02-23 16:25:47.000000 relatorio-0.9.2/MANIFEST.in
--rw-r--r--   0 ced       (1000) ced       (1000)     1629 2020-08-06 07:10:42.000000 relatorio-0.9.2/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)      461 2018-08-18 11:27:26.000000 relatorio-0.9.2/README
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2020-08-06 07:10:42.000000 relatorio-0.9.2/doc/
--rw-r--r--   0 ced       (1000) ced       (1000)     5576 2018-08-18 11:27:26.000000 relatorio-0.9.2/doc/Makefile
--rw-r--r--   0 ced       (1000) ced       (1000)    65202 2018-08-18 11:27:26.000000 relatorio-0.9.2/doc/basic.png
--rw-r--r--   0 ced       (1000) ced       (1000)    82006 2018-08-18 11:27:26.000000 relatorio-0.9.2/doc/basic_generated.png
--rw-r--r--   0 ced       (1000) ced       (1000)    98276 2018-08-18 11:27:26.000000 relatorio-0.9.2/doc/bonham_basic.png
--rw-r--r--   0 ced       (1000) ced       (1000)    74946 2018-08-18 11:27:26.000000 relatorio-0.9.2/doc/complicated.png
--rw-r--r--   0 ced       (1000) ced       (1000)    76468 2018-08-18 11:27:26.000000 relatorio-0.9.2/doc/complicated_rendered.png
--rw-r--r--   0 ced       (1000) ced       (1000)     7694 2020-02-29 23:37:03.000000 relatorio-0.9.2/doc/conf.py
--rw-r--r--   0 ced       (1000) ced       (1000)    25208 2018-08-18 11:27:26.000000 relatorio-0.9.2/doc/frame.png
--rw-r--r--   0 ced       (1000) ced       (1000)    29219 2018-08-18 11:27:26.000000 relatorio-0.9.2/doc/hyperlink.png
--rw-r--r--   0 ced       (1000) ced       (1000)     5008 2018-08-18 11:27:26.000000 relatorio-0.9.2/doc/indepthexample.rst
--rw-r--r--   0 ced       (1000) ced       (1000)      372 2018-08-18 11:27:26.000000 relatorio-0.9.2/doc/index.rst
--rw-r--r--   0 ced       (1000) ced       (1000)     5102 2018-08-18 11:27:26.000000 relatorio-0.9.2/doc/make.bat
--rw-r--r--   0 ced       (1000) ced       (1000)    27012 2018-08-18 11:27:26.000000 relatorio-0.9.2/doc/pie.png
--rw-r--r--   0 ced       (1000) ced       (1000)    67227 2018-08-18 11:27:26.000000 relatorio-0.9.2/doc/pivot.png
--rw-r--r--   0 ced       (1000) ced       (1000)    75354 2018-08-18 11:27:26.000000 relatorio-0.9.2/doc/pivot_rendered.png
--rw-r--r--   0 ced       (1000) ced       (1000)     2250 2018-08-18 11:27:26.000000 relatorio-0.9.2/doc/quickexample.rst
--rw-r--r--   0 ced       (1000) ced       (1000)    79043 2018-08-18 11:27:26.000000 relatorio-0.9.2/doc/relatorio_basic.png
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2020-08-06 07:10:42.000000 relatorio-0.9.2/examples/
--rw-r--r--   0 ced       (1000) ced       (1000)    29415 2018-08-18 11:27:26.000000 relatorio-0.9.2/examples/basic.odt
--rw-r--r--   0 ced       (1000) ced       (1000)      385 2018-08-18 11:27:26.000000 relatorio-0.9.2/examples/basic.tex
--rw-r--r--   0 ced       (1000) ced       (1000)     8452 2018-11-09 16:22:41.000000 relatorio-0.9.2/examples/big.odt
--rw-r--r--   0 ced       (1000) ced       (1000)    11101 2018-08-18 11:27:26.000000 relatorio-0.9.2/examples/bouteille.png
--rw-r--r--   0 ced       (1000) ced       (1000)    20675 2018-08-18 11:27:26.000000 relatorio-0.9.2/examples/columns.odt
--rw-r--r--   0 ced       (1000) ced       (1000)     1576 2018-08-18 11:27:26.000000 relatorio-0.9.2/examples/common.py
--rw-r--r--   0 ced       (1000) ced       (1000)    27915 2018-08-18 11:27:26.000000 relatorio-0.9.2/examples/complicated.odt
--rw-r--r--   0 ced       (1000) ced       (1000)      968 2018-08-18 11:27:26.000000 relatorio-0.9.2/examples/demo_chart.py
--rw-r--r--   0 ced       (1000) ced       (1000)      468 2018-11-09 15:41:53.000000 relatorio-0.9.2/examples/demo_context.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2932 2018-11-09 21:48:09.000000 relatorio-0.9.2/examples/demo_odf.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1475 2018-11-09 15:41:53.000000 relatorio-0.9.2/examples/demo_repository.py
--rw-r--r--   0 ced       (1000) ced       (1000)    10878 2018-08-18 11:27:26.000000 relatorio-0.9.2/examples/demo_sheets.ods
--rw-r--r--   0 ced       (1000) ced       (1000)      634 2018-08-18 11:27:26.000000 relatorio-0.9.2/examples/hbar_chart
--rw-r--r--   0 ced       (1000) ced       (1000)      502 2018-08-18 11:27:26.000000 relatorio-0.9.2/examples/line_chart
--rw-r--r--   0 ced       (1000) ced       (1000)      337 2018-08-18 11:27:26.000000 relatorio-0.9.2/examples/pie_chart
--rw-r--r--   0 ced       (1000) ced       (1000)    11577 2018-08-18 11:27:26.000000 relatorio-0.9.2/examples/pivot.ods
--rw-r--r--   0 ced       (1000) ced       (1000)    22604 2018-08-18 11:27:26.000000 relatorio-0.9.2/examples/presentation.odp
--rw-r--r--   0 ced       (1000) ced       (1000)      634 2018-08-18 11:27:26.000000 relatorio-0.9.2/examples/vbar_chart
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2020-08-06 07:10:42.000000 relatorio-0.9.2/relatorio/
--rw-r--r--   0 ced       (1000) ced       (1000)      568 2020-01-26 10:04:42.000000 relatorio-0.9.2/relatorio/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     5592 2020-07-30 13:52:07.000000 relatorio-0.9.2/relatorio/reporting.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2020-08-06 07:10:42.000000 relatorio-0.9.2/relatorio/templates/
--rw-r--r--   0 ced       (1000) ced       (1000)     1006 2018-08-18 11:27:26.000000 relatorio-0.9.2/relatorio/templates/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)     1777 2020-02-29 23:38:56.000000 relatorio-0.9.2/relatorio/templates/base.py
--rw-r--r--   0 ced       (1000) ced       (1000)     3445 2018-11-09 21:48:09.000000 relatorio-0.9.2/relatorio/templates/chart.py
--rw-r--r--   0 ced       (1000) ced       (1000)    47970 2020-07-01 07:42:11.000000 relatorio-0.9.2/relatorio/templates/opendocument.py
--rw-r--r--   0 ced       (1000) ced       (1000)     2368 2018-11-09 21:48:09.000000 relatorio-0.9.2/relatorio/templates/pdf.py
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2020-08-06 07:10:42.000000 relatorio-0.9.2/relatorio/tests/
--rw-r--r--   0 ced       (1000) ced       (1000)     1569 2020-02-29 23:41:43.000000 relatorio-0.9.2/relatorio/tests/__init__.py
--rw-r--r--   0 ced       (1000) ced       (1000)    29425 2018-08-18 11:27:26.000000 relatorio-0.9.2/relatorio/tests/egg.jpg
--rw-r--r--   0 ced       (1000) ced       (1000)    28373 2018-08-18 11:27:26.000000 relatorio-0.9.2/relatorio/tests/one.jpg
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2020-08-06 07:10:42.000000 relatorio-0.9.2/relatorio/tests/templates/
--rw-r--r--   0 ced       (1000) ced       (1000)       25 2018-08-18 11:27:26.000000 relatorio-0.9.2/relatorio/tests/templates/include.tmpl
--rw-r--r--   0 ced       (1000) ced       (1000)       15 2018-08-18 11:27:26.000000 relatorio-0.9.2/relatorio/tests/templates/other.tmpl
--rw-r--r--   0 ced       (1000) ced       (1000)       17 2018-08-18 11:27:26.000000 relatorio-0.9.2/relatorio/tests/templates/test.tmpl
--rw-r--r--   0 ced       (1000) ced       (1000)       43 2018-08-18 11:27:26.000000 relatorio-0.9.2/relatorio/tests/templates/time.tmpl
--rw-r--r--   0 ced       (1000) ced       (1000)    62931 2018-08-18 11:27:26.000000 relatorio-0.9.2/relatorio/tests/test.fodt
--rw-r--r--   0 ced       (1000) ced       (1000)    12530 2020-07-01 07:41:38.000000 relatorio-0.9.2/relatorio/tests/test.odt
--rw-r--r--   0 ced       (1000) ced       (1000)     4850 2018-08-18 11:27:26.000000 relatorio-0.9.2/relatorio/tests/test_api.py
--rw-r--r--   0 ced       (1000) ced       (1000)    24221 2020-07-01 07:44:07.000000 relatorio-0.9.2/relatorio/tests/test_odt.py
--rw-r--r--   0 ced       (1000) ced       (1000)   172354 2018-08-18 11:27:26.000000 relatorio-0.9.2/relatorio/tests/two.png
-drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2020-08-06 07:10:42.000000 relatorio-0.9.2/relatorio.egg-info/
--rw-r--r--   0 ced       (1000) ced       (1000)     1629 2020-08-06 07:10:42.000000 relatorio-0.9.2/relatorio.egg-info/PKG-INFO
--rw-r--r--   0 ced       (1000) ced       (1000)     1524 2020-08-06 07:10:42.000000 relatorio-0.9.2/relatorio.egg-info/SOURCES.txt
--rw-r--r--   0 ced       (1000) ced       (1000)        1 2020-08-06 07:10:42.000000 relatorio-0.9.2/relatorio.egg-info/dependency_links.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       72 2020-08-06 07:10:42.000000 relatorio-0.9.2/relatorio.egg-info/requires.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       10 2020-08-06 07:10:42.000000 relatorio-0.9.2/relatorio.egg-info/top_level.txt
--rw-r--r--   0 ced       (1000) ced       (1000)       38 2020-08-06 07:10:42.000000 relatorio-0.9.2/setup.cfg
--rw-r--r--   0 ced       (1000) ced       (1000)     1989 2020-02-23 16:20:17.000000 relatorio-0.9.2/setup.py
--rw-r--r--   0 ced       (1000) ced       (1000)      394 2019-12-26 09:42:44.000000 relatorio-0.9.2/tox.ini
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2021-05-07 11:52:49.767762 relatorio-0.9.3/
+-rw-r--r--   0 ced       (1000) ced       (1000)      735 2020-12-19 12:41:40.000000 relatorio-0.9.3/.drone.yml
+-rw-r--r--   0 ced       (1000) ced       (1000)       41 2020-02-29 23:31:40.000000 relatorio-0.9.3/.flake8
+-rw-r--r--   0 ced       (1000) ced       (1000)      157 2018-08-18 11:27:26.000000 relatorio-0.9.3/.hgignore
+-rw-r--r--   0 ced       (1000) ced       (1000)     1457 2021-05-07 11:51:51.000000 relatorio-0.9.3/.hgtags
+-rw-r--r--   0 ced       (1000) ced       (1000)     4277 2021-05-07 10:11:09.000000 relatorio-0.9.3/CHANGELOG
+-rw-r--r--   0 ced       (1000) ced       (1000)      834 2020-02-23 16:24:17.000000 relatorio-0.9.3/COPYRIGHT
+-rw-r--r--   0 ced       (1000) ced       (1000)    35147 2018-08-18 11:27:26.000000 relatorio-0.9.3/LICENSE
+-rw-r--r--   0 ced       (1000) ced       (1000)       81 2020-02-23 16:25:47.000000 relatorio-0.9.3/MANIFEST.in
+-rw-r--r--   0 ced       (1000) ced       (1000)     1629 2021-05-07 11:52:49.767762 relatorio-0.9.3/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)      461 2018-08-18 11:27:26.000000 relatorio-0.9.3/README
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2021-05-07 11:52:49.744428 relatorio-0.9.3/doc/
+-rw-r--r--   0 ced       (1000) ced       (1000)     5576 2018-08-18 11:27:26.000000 relatorio-0.9.3/doc/Makefile
+-rw-r--r--   0 ced       (1000) ced       (1000)    65202 2018-08-18 11:27:26.000000 relatorio-0.9.3/doc/basic.png
+-rw-r--r--   0 ced       (1000) ced       (1000)    82006 2018-08-18 11:27:26.000000 relatorio-0.9.3/doc/basic_generated.png
+-rw-r--r--   0 ced       (1000) ced       (1000)    98276 2018-08-18 11:27:26.000000 relatorio-0.9.3/doc/bonham_basic.png
+-rw-r--r--   0 ced       (1000) ced       (1000)    74946 2018-08-18 11:27:26.000000 relatorio-0.9.3/doc/complicated.png
+-rw-r--r--   0 ced       (1000) ced       (1000)    76468 2018-08-18 11:27:26.000000 relatorio-0.9.3/doc/complicated_rendered.png
+-rw-r--r--   0 ced       (1000) ced       (1000)     7694 2020-08-06 07:14:00.000000 relatorio-0.9.3/doc/conf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    25208 2018-08-18 11:27:26.000000 relatorio-0.9.3/doc/frame.png
+-rw-r--r--   0 ced       (1000) ced       (1000)    29219 2018-08-18 11:27:26.000000 relatorio-0.9.3/doc/hyperlink.png
+-rw-r--r--   0 ced       (1000) ced       (1000)     5008 2018-08-18 11:27:26.000000 relatorio-0.9.3/doc/indepthexample.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)      372 2018-08-18 11:27:26.000000 relatorio-0.9.3/doc/index.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)     5102 2018-08-18 11:27:26.000000 relatorio-0.9.3/doc/make.bat
+-rw-r--r--   0 ced       (1000) ced       (1000)    27012 2018-08-18 11:27:26.000000 relatorio-0.9.3/doc/pie.png
+-rw-r--r--   0 ced       (1000) ced       (1000)    67227 2018-08-18 11:27:26.000000 relatorio-0.9.3/doc/pivot.png
+-rw-r--r--   0 ced       (1000) ced       (1000)    75354 2018-08-18 11:27:26.000000 relatorio-0.9.3/doc/pivot_rendered.png
+-rw-r--r--   0 ced       (1000) ced       (1000)     2250 2018-08-18 11:27:26.000000 relatorio-0.9.3/doc/quickexample.rst
+-rw-r--r--   0 ced       (1000) ced       (1000)    79043 2018-08-18 11:27:26.000000 relatorio-0.9.3/doc/relatorio_basic.png
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2021-05-07 11:52:49.754428 relatorio-0.9.3/examples/
+-rw-r--r--   0 ced       (1000) ced       (1000)    29415 2018-08-18 11:27:26.000000 relatorio-0.9.3/examples/basic.odt
+-rw-r--r--   0 ced       (1000) ced       (1000)      385 2018-08-18 11:27:26.000000 relatorio-0.9.3/examples/basic.tex
+-rw-r--r--   0 ced       (1000) ced       (1000)     8452 2018-11-09 16:22:41.000000 relatorio-0.9.3/examples/big.odt
+-rw-r--r--   0 ced       (1000) ced       (1000)    11101 2018-08-18 11:27:26.000000 relatorio-0.9.3/examples/bouteille.png
+-rw-r--r--   0 ced       (1000) ced       (1000)    20675 2018-08-18 11:27:26.000000 relatorio-0.9.3/examples/columns.odt
+-rw-r--r--   0 ced       (1000) ced       (1000)     1576 2018-08-18 11:27:26.000000 relatorio-0.9.3/examples/common.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    27915 2018-08-18 11:27:26.000000 relatorio-0.9.3/examples/complicated.odt
+-rw-r--r--   0 ced       (1000) ced       (1000)      968 2018-08-18 11:27:26.000000 relatorio-0.9.3/examples/demo_chart.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      468 2018-11-09 15:41:53.000000 relatorio-0.9.3/examples/demo_context.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2932 2018-11-09 21:48:09.000000 relatorio-0.9.3/examples/demo_odf.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1475 2018-11-09 15:41:53.000000 relatorio-0.9.3/examples/demo_repository.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    10878 2018-08-18 11:27:26.000000 relatorio-0.9.3/examples/demo_sheets.ods
+-rw-r--r--   0 ced       (1000) ced       (1000)      634 2018-08-18 11:27:26.000000 relatorio-0.9.3/examples/hbar_chart
+-rw-r--r--   0 ced       (1000) ced       (1000)      502 2018-08-18 11:27:26.000000 relatorio-0.9.3/examples/line_chart
+-rw-r--r--   0 ced       (1000) ced       (1000)      337 2018-08-18 11:27:26.000000 relatorio-0.9.3/examples/pie_chart
+-rw-r--r--   0 ced       (1000) ced       (1000)    11577 2018-08-18 11:27:26.000000 relatorio-0.9.3/examples/pivot.ods
+-rw-r--r--   0 ced       (1000) ced       (1000)    22604 2018-08-18 11:27:26.000000 relatorio-0.9.3/examples/presentation.odp
+-rw-r--r--   0 ced       (1000) ced       (1000)      634 2018-08-18 11:27:26.000000 relatorio-0.9.3/examples/vbar_chart
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2021-05-07 11:52:49.754428 relatorio-0.9.3/relatorio/
+-rw-r--r--   0 ced       (1000) ced       (1000)      568 2020-08-06 07:14:07.000000 relatorio-0.9.3/relatorio/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     5592 2020-07-30 13:52:07.000000 relatorio-0.9.3/relatorio/reporting.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2021-05-07 11:52:49.761095 relatorio-0.9.3/relatorio/templates/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1006 2018-08-18 11:27:26.000000 relatorio-0.9.3/relatorio/templates/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     1777 2020-02-29 23:38:56.000000 relatorio-0.9.3/relatorio/templates/base.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     3445 2018-11-09 21:48:09.000000 relatorio-0.9.3/relatorio/templates/chart.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    48069 2021-03-27 11:52:33.000000 relatorio-0.9.3/relatorio/templates/opendocument.py
+-rw-r--r--   0 ced       (1000) ced       (1000)     2368 2018-11-09 21:48:09.000000 relatorio-0.9.3/relatorio/templates/pdf.py
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2021-05-07 11:52:49.764428 relatorio-0.9.3/relatorio/tests/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1569 2020-02-29 23:41:43.000000 relatorio-0.9.3/relatorio/tests/__init__.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    29425 2018-08-18 11:27:26.000000 relatorio-0.9.3/relatorio/tests/egg.jpg
+-rw-r--r--   0 ced       (1000) ced       (1000)    28373 2018-08-18 11:27:26.000000 relatorio-0.9.3/relatorio/tests/one.jpg
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2021-05-07 11:52:49.767762 relatorio-0.9.3/relatorio/tests/templates/
+-rw-r--r--   0 ced       (1000) ced       (1000)       25 2018-08-18 11:27:26.000000 relatorio-0.9.3/relatorio/tests/templates/include.tmpl
+-rw-r--r--   0 ced       (1000) ced       (1000)       15 2018-08-18 11:27:26.000000 relatorio-0.9.3/relatorio/tests/templates/other.tmpl
+-rw-r--r--   0 ced       (1000) ced       (1000)       17 2018-08-18 11:27:26.000000 relatorio-0.9.3/relatorio/tests/templates/test.tmpl
+-rw-r--r--   0 ced       (1000) ced       (1000)       43 2018-08-18 11:27:26.000000 relatorio-0.9.3/relatorio/tests/templates/time.tmpl
+-rw-r--r--   0 ced       (1000) ced       (1000)    62931 2018-08-18 11:27:26.000000 relatorio-0.9.3/relatorio/tests/test.fodt
+-rw-r--r--   0 ced       (1000) ced       (1000)    12530 2020-07-01 07:41:38.000000 relatorio-0.9.3/relatorio/tests/test.odt
+-rw-r--r--   0 ced       (1000) ced       (1000)     4850 2018-08-18 11:27:26.000000 relatorio-0.9.3/relatorio/tests/test_api.py
+-rw-r--r--   0 ced       (1000) ced       (1000)    24296 2021-03-27 11:57:46.000000 relatorio-0.9.3/relatorio/tests/test_odt.py
+-rw-r--r--   0 ced       (1000) ced       (1000)   172354 2018-08-18 11:27:26.000000 relatorio-0.9.3/relatorio/tests/two.png
+drwxr-xr-x   0 ced       (1000) ced       (1000)        0 2021-05-07 11:52:49.754428 relatorio-0.9.3/relatorio.egg-info/
+-rw-r--r--   0 ced       (1000) ced       (1000)     1629 2021-05-07 11:52:49.000000 relatorio-0.9.3/relatorio.egg-info/PKG-INFO
+-rw-r--r--   0 ced       (1000) ced       (1000)     1524 2021-05-07 11:52:49.000000 relatorio-0.9.3/relatorio.egg-info/SOURCES.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)        1 2021-05-07 11:52:49.000000 relatorio-0.9.3/relatorio.egg-info/dependency_links.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       72 2021-05-07 11:52:49.000000 relatorio-0.9.3/relatorio.egg-info/requires.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       10 2021-05-07 11:52:49.000000 relatorio-0.9.3/relatorio.egg-info/top_level.txt
+-rw-r--r--   0 ced       (1000) ced       (1000)       38 2021-05-07 11:52:49.771095 relatorio-0.9.3/setup.cfg
+-rw-r--r--   0 ced       (1000) ced       (1000)     1989 2020-02-23 16:20:17.000000 relatorio-0.9.3/setup.py
+-rw-r--r--   0 ced       (1000) ced       (1000)      400 2020-12-19 12:41:50.000000 relatorio-0.9.3/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `relatorio-0.9.2/.drone.yml` & `relatorio-0.9.3/.drone.yml`

 * *Files 14% similar despite different names*

```diff
@@ -25,7 +25,9 @@
           TOXENV: py35
         - IMAGE: python:3.6
           TOXENV: py36
         - IMAGE: python:3.7
           TOXENV: py37
         - IMAGE: python:3.8
           TOXENV: py38
+        - IMAGE: python:3.9
+          TOXENV: py39
```

### Comparing `relatorio-0.9.2/.hgtags` & `relatorio-0.9.3/.hgtags`

 * *Files 4% similar despite different names*

```diff
@@ -24,7 +24,8 @@
 50115e7464e35bc1517b23ed4fd4eed1d284273a 0.7.0
 8ee1d7515d35918944151d3a44003063e1ab6a18 0.7.1
 0775b131b51d40c2147b1ae104f760698a8d9f9e 0.8.0
 a9a586fec08da03f86ec781472a981949d4c455a 0.8.1
 a0cf6c5a86e3eaf125a96f942f64114b326dba3b 0.9.0
 34f63c525603ed1fe903703725a51d28cdfa622f 0.9.1
 9c0efe3507a42762e2128f9ad475f463da253c2b 0.9.2
+b190bcec6e4440fd4d21400bb1a6b01291448e41 0.9.3
```

### Comparing `relatorio-0.9.2/CHANGELOG` & `relatorio-0.9.3/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+0.9.3 - 20210507
+* Support empty image in opendocument
+* Add support for Python 3.9
+
 0.9.2 - 20200826
 * Support draw name tuple without parenthesis
 
 0.9.1 - 20200126
 * Do not guess type of cell if directive is not alone
 * Add support for Python 3.8
 * Support file-magic as fallback to python-magic
```

### Comparing `relatorio-0.9.2/COPYRIGHT` & `relatorio-0.9.3/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/LICENSE` & `relatorio-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/PKG-INFO` & `relatorio-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relatorio
-Version: 0.9.2
+Version: 0.9.3
 Summary: A templating library able to output odt and pdf files
 Home-page: https://pypi.python.org/pypi/relatorio
 Author: Tryton
 Author-email: relatorio@tryton.org
 License: GPL License
 Download-URL: https://downloads.tryton.org/relatorio/
 Project-URL: Bug Tracker, https://relatorio.tryton.org/
```

### Comparing `relatorio-0.9.2/doc/Makefile` & `relatorio-0.9.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/doc/basic.png` & `relatorio-0.9.3/doc/basic.png`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/doc/basic_generated.png` & `relatorio-0.9.3/doc/basic_generated.png`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/doc/bonham_basic.png` & `relatorio-0.9.3/doc/bonham_basic.png`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/doc/complicated.png` & `relatorio-0.9.3/doc/complicated.png`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/doc/complicated_rendered.png` & `relatorio-0.9.3/doc/complicated_rendered.png`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/doc/conf.py` & `relatorio-0.9.3/doc/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = '0.9'
 # The full version, including alpha/beta/rc tags.
-release = '0.9.2'
+release = '0.9.3'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `relatorio-0.9.2/doc/frame.png` & `relatorio-0.9.3/doc/frame.png`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/doc/hyperlink.png` & `relatorio-0.9.3/doc/hyperlink.png`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/doc/indepthexample.rst` & `relatorio-0.9.3/doc/indepthexample.rst`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/doc/make.bat` & `relatorio-0.9.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/doc/pie.png` & `relatorio-0.9.3/doc/pie.png`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/doc/pivot.png` & `relatorio-0.9.3/doc/pivot.png`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/doc/pivot_rendered.png` & `relatorio-0.9.3/doc/pivot_rendered.png`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/doc/quickexample.rst` & `relatorio-0.9.3/doc/quickexample.rst`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/doc/relatorio_basic.png` & `relatorio-0.9.3/doc/relatorio_basic.png`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/examples/basic.odt` & `relatorio-0.9.3/examples/basic.odt`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/examples/big.odt` & `relatorio-0.9.3/examples/big.odt`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/examples/bouteille.png` & `relatorio-0.9.3/examples/bouteille.png`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/examples/columns.odt` & `relatorio-0.9.3/examples/columns.odt`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/examples/common.py` & `relatorio-0.9.3/examples/common.py`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/examples/complicated.odt` & `relatorio-0.9.3/examples/complicated.odt`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/examples/demo_chart.py` & `relatorio-0.9.3/examples/demo_chart.py`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/examples/demo_odf.py` & `relatorio-0.9.3/examples/demo_odf.py`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/examples/demo_repository.py` & `relatorio-0.9.3/examples/demo_repository.py`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/examples/demo_sheets.ods` & `relatorio-0.9.3/examples/demo_sheets.ods`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/examples/hbar_chart` & `relatorio-0.9.3/examples/hbar_chart`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/examples/pivot.ods` & `relatorio-0.9.3/examples/pivot.ods`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/examples/presentation.odp` & `relatorio-0.9.3/examples/presentation.odp`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/examples/vbar_chart` & `relatorio-0.9.3/examples/vbar_chart`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/relatorio/__init__.py` & `relatorio-0.9.3/relatorio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 
 relatorio also provides a report repository allowing you to link python objects
 and report together, find reports by mimetypes/name/python objects.
 """
 from .reporting import MIMETemplateLoader, ReportRepository, Report
 from . import templates
 
-__version__ = '0.9.2'
+__version__ = '0.9.3'
 __all__ = ['MIMETemplateLoader', 'ReportRepository', 'Report', 'templates']
```

### Comparing `relatorio-0.9.2/relatorio/reporting.py` & `relatorio-0.9.3/relatorio/reporting.py`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/relatorio/templates/__init__.py` & `relatorio-0.9.3/relatorio/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/relatorio/templates/base.py` & `relatorio-0.9.3/relatorio/templates/base.py`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/relatorio/templates/chart.py` & `relatorio-0.9.3/relatorio/templates/chart.py`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/relatorio/templates/opendocument.py` & `relatorio-0.9.3/relatorio/templates/opendocument.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 import relatorio
 from relatorio.templates.base import RelatorioStream
 from relatorio.reporting import Report, MIMETemplateLoader
 try:
     from relatorio.templates.chart import Template as ChartTemplate
 except ImportError:
-    ChartTemplate = type(None)
+    ChartTemplate = None
 
 try:
     basestring
 except NameError:
     basestring = str
 try:
     long
@@ -128,23 +128,26 @@
         self.serializer = serializer
         self.context = context.copy()
 
     def __call__(self, expr):
         bitstream, mimetype = expr[:2]
         if isinstance(bitstream, Report):
             bitstream = bitstream(**self.context).render()
-        elif isinstance(bitstream, ChartTemplate):
+        elif ChartTemplate and isinstance(bitstream, ChartTemplate):
             bitstream = bitstream.generate(**self.context).render()
         elif not hasattr(bitstream, 'seek') or not hasattr(bitstream, 'read'):
             bitstream = BytesIO(bitstream)
-        bitstream.seek(0)
-        file_content = bitstream.read()
+        if bitstream:
+            bitstream.seek(0)
+            file_content = bitstream.read()
+        else:
+            file_content = b''
         name = md5(file_content).hexdigest()
         path = 'Pictures/%s%s' % (
-            name, mimetypes.guess_extension(mimetype))
+            name, mimetypes.guess_extension(mimetype or '') or '')
         self.serializer.add_file(path, file_content, mimetype)
         return {'{http://www.w3.org/1999/xlink}href': path}
 
 
 class ImageDimension:
     "A class used to set dimension in draw tags"
```

### Comparing `relatorio-0.9.2/relatorio/templates/pdf.py` & `relatorio-0.9.3/relatorio/templates/pdf.py`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/relatorio/tests/__init__.py` & `relatorio-0.9.3/relatorio/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/relatorio/tests/egg.jpg` & `relatorio-0.9.3/relatorio/tests/egg.jpg`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/relatorio/tests/one.jpg` & `relatorio-0.9.3/relatorio/tests/one.jpg`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/relatorio/tests/test.fodt` & `relatorio-0.9.3/relatorio/tests/test.fodt`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/relatorio/tests/test.odt` & `relatorio-0.9.3/relatorio/tests/test.odt`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/relatorio/tests/test_api.py` & `relatorio-0.9.3/relatorio/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/relatorio/tests/test_odt.py` & `relatorio-0.9.3/relatorio/tests/test_odt.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,22 +75,24 @@
                                  {'first_name': u'Mathias',
                                   'last_name': u'Lechat'}],
                      'hobbies': [u'Music', u'Dancing', u'DJing'],
                      'animals': [u'Felix da housecat', u'Dog eat Dog'],
                      'images': [(open(os.path.join(thisdir, 'one.jpg'), 'rb'),
                                  'image/jpeg', None, None, 'One'),
                                 (open(os.path.join(thisdir, 'two.png'), 'rb'),
-                                 'image/png', '2cm', '2.2cm', 'Two')],
+                                 'image/png', '2cm', '2.2cm', 'Two'),
+                                (None, None)],
                      'oeuf': open(os.path.join(thisdir, 'egg.jpg'), 'rb'),
                      'footer': u'We sell stuff'}
 
     def tearDown(self):
         self._source.close()
         for image in self.data['images']:
-            image[0].close()
+            if image[0]:
+                image[0].close()
         self.data['oeuf'].close()
 
     def test_init(self):
         "Testing the correct handling of the styles.xml and content.xml files"
         self.assertTrue(isinstance(self.oot.stream, list))
         self.assertEqual(
             self.oot.stream[0], (PI, ('relatorio', 'content.xml'), None))
@@ -421,15 +423,15 @@
         "Testing the image replacement directive"
         stream = self.oot.generate(**self.data)
         rendered = stream_to_string(stream.events.render(encoding='utf-8'))
         styles_idx = rendered.find('<?relatorio styles.xml?>')
         tree = lxml.etree.parse(StringIO(rendered[25:styles_idx]))
         root = tree.getroot()
         images = root.xpath('//draw:frame', namespaces=self.oot.namespaces)
-        self.assertEqual(len(images), 4)
+        self.assertEqual(len(images), 5)
         self.assertFalse(
             images[0].get('{%s}name' % self.oot.namespaces['draw']))
         self.assertFalse(
             images[1].get('{%s}name' % self.oot.namespaces['draw']))
         self.assertEqual(
             images[2].get('{%s}name' % self.oot.namespaces['draw']), 'One')
         self.assertEqual(
```

### Comparing `relatorio-0.9.2/relatorio/tests/two.png` & `relatorio-0.9.3/relatorio/tests/two.png`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/relatorio.egg-info/PKG-INFO` & `relatorio-0.9.3/relatorio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relatorio
-Version: 0.9.2
+Version: 0.9.3
 Summary: A templating library able to output odt and pdf files
 Home-page: https://pypi.python.org/pypi/relatorio
 Author: Tryton
 Author-email: relatorio@tryton.org
 License: GPL License
 Download-URL: https://downloads.tryton.org/relatorio/
 Project-URL: Bug Tracker, https://relatorio.tryton.org/
```

### Comparing `relatorio-0.9.2/relatorio.egg-info/SOURCES.txt` & `relatorio-0.9.3/relatorio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `relatorio-0.9.2/setup.py` & `relatorio-0.9.3/setup.py`

 * *Files identical despite different names*

