# Comparing `tmp/vot-toolkit-0.6.4.tar.gz` & `tmp/vot-toolkit-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vot-toolkit-0.6.4.tar", last modified: Wed May 31 07:41:25 2023, max compression
+gzip compressed data, was "vot-toolkit-0.7.0.tar", last modified: Sun Apr 21 18:30:28 2024, max compression
```

## Comparing `vot-toolkit-0.6.4.tar` & `vot-toolkit-0.7.0.tar`

### file list

```diff
@@ -1,119 +1,126 @@
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.533292 vot-toolkit-0.6.4/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      211 2022-03-25 11:28:05.000000 vot-toolkit-0.6.4/MANIFEST.in
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3769 2023-05-31 07:41:25.533292 vot-toolkit-0.6.4/PKG-INFO
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2823 2023-05-31 07:22:20.000000 vot-toolkit-0.6.4/README.md
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      295 2023-05-31 07:14:15.000000 vot-toolkit-0.6.4/requirements.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       38 2023-05-31 07:41:25.533292 vot-toolkit-0.6.4/setup.cfg
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1427 2023-05-09 11:09:24.000000 vot-toolkit-0.6.4/setup.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.501293 vot-toolkit-0.6.4/vot/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3368 2023-05-25 09:52:52.000000 vot-toolkit-0.6.4/vot/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      254 2023-05-20 18:58:54.000000 vot-toolkit-0.6.4/vot/__main__.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.501293 vot-toolkit-0.6.4/vot/analysis/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    24213 2023-05-22 14:54:27.000000 vot-toolkit-0.6.4/vot/analysis/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    11736 2023-05-19 09:42:24.000000 vot-toolkit-0.6.4/vot/analysis/accuracy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3878 2023-05-29 15:05:06.000000 vot-toolkit-0.6.4/vot/analysis/failures.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    26037 2023-05-19 11:07:21.000000 vot-toolkit-0.6.4/vot/analysis/longterm.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    17278 2023-05-29 15:05:26.000000 vot-toolkit-0.6.4/vot/analysis/multistart.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    30789 2023-05-19 11:11:46.000000 vot-toolkit-0.6.4/vot/analysis/processor.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    13994 2023-05-19 11:09:41.000000 vot-toolkit-0.6.4/vot/analysis/supervised.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.505293 vot-toolkit-0.6.4/vot/dataset/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    38943 2023-05-30 13:49:40.000000 vot-toolkit-0.6.4/vot/dataset/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    11781 2023-05-30 15:42:52.000000 vot-toolkit-0.6.4/vot/dataset/common.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14672 2020-12-04 15:25:26.000000 vot-toolkit-0.6.4/vot/dataset/cow.png
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3545 2023-05-30 11:19:19.000000 vot-toolkit-0.6.4/vot/dataset/dummy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4216 2023-05-30 13:47:46.000000 vot-toolkit-0.6.4/vot/dataset/got10k.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    11337 2023-05-30 10:50:38.000000 vot-toolkit-0.6.4/vot/dataset/otb.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12655 2023-05-30 11:11:21.000000 vot-toolkit-0.6.4/vot/dataset/proxy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3917 2023-05-30 13:50:11.000000 vot-toolkit-0.6.4/vot/dataset/trackingnet.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.509292 vot-toolkit-0.6.4/vot/document/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16066 2023-05-30 14:50:52.000000 vot-toolkit-0.6.4/vot/document/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      465 2020-12-04 15:25:26.000000 vot-toolkit-0.6.4/vot/document/commands.tex
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6115 2023-05-19 11:23:17.000000 vot-toolkit-0.6.4/vot/document/common.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5950 2023-05-19 11:31:01.000000 vot-toolkit-0.6.4/vot/document/html.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    89476 2020-12-04 15:25:26.000000 vot-toolkit-0.6.4/vot/document/jquery.js
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6911 2023-05-19 11:31:15.000000 vot-toolkit-0.6.4/vot/document/latex.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16184 2020-12-04 15:25:26.000000 vot-toolkit-0.6.4/vot/document/pure.css
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      647 2020-12-04 15:25:26.000000 vot-toolkit-0.6.4/vot/document/report.css
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1212 2020-12-04 15:25:26.000000 vot-toolkit-0.6.4/vot/document/report.js
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9933 2020-12-04 15:25:26.000000 vot-toolkit-0.6.4/vot/document/table.js
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        0 2022-03-23 08:48:42.000000 vot-toolkit-0.6.4/vot/document/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.509292 vot-toolkit-0.6.4/vot/experiment/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    13067 2023-05-31 07:39:21.000000 vot-toolkit-0.6.4/vot/experiment/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1702 2023-05-20 19:07:07.000000 vot-toolkit-0.6.4/vot/experiment/helpers.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10048 2023-05-30 15:28:37.000000 vot-toolkit-0.6.4/vot/experiment/multirun.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4945 2023-05-29 15:08:02.000000 vot-toolkit-0.6.4/vot/experiment/multistart.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4567 2023-05-29 15:08:15.000000 vot-toolkit-0.6.4/vot/experiment/transformer.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.509292 vot-toolkit-0.6.4/vot/region/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3728 2023-05-20 18:47:22.000000 vot-toolkit-0.6.4/vot/region/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10387 2023-05-30 15:43:52.000000 vot-toolkit-0.6.4/vot/region/io.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14049 2023-05-20 18:36:18.000000 vot-toolkit-0.6.4/vot/region/raster.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16612 2023-05-25 09:54:33.000000 vot-toolkit-0.6.4/vot/region/shapes.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3706 2023-05-20 18:08:57.000000 vot-toolkit-0.6.4/vot/region/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.513292 vot-toolkit-0.6.4/vot/stack/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4320 2023-05-20 10:50:01.000000 vot-toolkit-0.6.4/vot/stack/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      249 2023-05-30 10:06:51.000000 vot-toolkit-0.6.4/vot/stack/otb100.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      247 2023-05-30 10:06:43.000000 vot-toolkit-0.6.4/vot/stack/otb50.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.517292 vot-toolkit-0.6.4/vot/stack/tests/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      184 2023-05-30 11:25:27.000000 vot-toolkit-0.6.4/vot/stack/tests/basic.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      541 2023-05-16 13:31:56.000000 vot-toolkit-0.6.4/vot/stack/tests/multiobject.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      638 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/tests/segmentation.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      969 2023-05-20 10:42:49.000000 vot-toolkit-0.6.4/vot/stack/tests.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      351 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2013.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      374 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2014.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.517292 vot-toolkit-0.6.4/vot/stack/vot2015/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      405 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2015/rgb.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      322 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2015/tir.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.517292 vot-toolkit-0.6.4/vot/stack/vot2016/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      540 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2016/rgb.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2016/tir.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      856 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2017.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.517292 vot-toolkit-0.6.4/vot/stack/vot2018/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2018/longterm.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      791 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2018/shortterm.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.521292 vot-toolkit-0.6.4/vot/stack/vot2019/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2019/longterm.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2019/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2019/rgbtir.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      789 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2019/shortterm.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.521292 vot-toolkit-0.6.4/vot/stack/vot2020/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2020/longterm.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2020/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2020/rgbtir.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2020/shortterm.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.521292 vot-toolkit-0.6.4/vot/stack/vot2021/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2021/lt.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2021/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2021/st.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.525292 vot-toolkit-0.6.4/vot/stack/vot2022/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      422 2023-05-05 11:01:43.000000 vot-toolkit-0.6.4/vot/stack/vot2022/depth.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      482 2022-03-25 11:28:05.000000 vot-toolkit-0.6.4/vot/stack/vot2022/lt.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      424 2022-03-25 11:28:05.000000 vot-toolkit-0.6.4/vot/stack/vot2022/rgbd.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2022-03-25 11:28:05.000000 vot-toolkit-0.6.4/vot/stack/vot2022/stb.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2022-03-25 11:28:05.000000 vot-toolkit-0.6.4/vot/stack/vot2022/sts.yaml
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      193 2023-05-10 17:51:17.000000 vot-toolkit-0.6.4/vot/stack/vots2023.yaml
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.525292 vot-toolkit-0.6.4/vot/tracker/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    33330 2023-05-30 13:51:34.000000 vot-toolkit-0.6.4/vot/tracker/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      808 2023-05-20 10:05:10.000000 vot-toolkit-0.6.4/vot/tracker/dummy.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9243 2023-05-20 10:44:10.000000 vot-toolkit-0.6.4/vot/tracker/results.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      631 2023-05-30 11:22:50.000000 vot-toolkit-0.6.4/vot/tracker/tests.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    29316 2023-05-20 10:43:30.000000 vot-toolkit-0.6.4/vot/tracker/trax.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.529292 vot-toolkit-0.6.4/vot/utilities/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    18320 2023-05-30 15:21:21.000000 vot-toolkit-0.6.4/vot/utilities/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    17701 2023-05-30 11:19:42.000000 vot-toolkit-0.6.4/vot/utilities/cli.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5740 2023-05-20 10:01:49.000000 vot-toolkit-0.6.4/vot/utilities/data.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10476 2023-05-19 11:41:40.000000 vot-toolkit-0.6.4/vot/utilities/draw.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4351 2023-05-20 09:57:10.000000 vot-toolkit-0.6.4/vot/utilities/migration.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7113 2023-05-20 10:02:38.000000 vot-toolkit-0.6.4/vot/utilities/net.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10059 2023-05-29 15:09:15.000000 vot-toolkit-0.6.4/vot/utilities/notebook.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       45 2023-05-29 11:34:41.000000 vot-toolkit-0.6.4/vot/version.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.529292 vot-toolkit-0.6.4/vot/workspace/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7526 2023-05-20 18:57:16.000000 vot-toolkit-0.6.4/vot/workspace/__init__.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    13864 2023-05-20 18:55:39.000000 vot-toolkit-0.6.4/vot/workspace/storage.py
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1840 2023-05-20 18:48:56.000000 vot-toolkit-0.6.4/vot/workspace/tests.py
-drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2023-05-31 07:41:25.533292 vot-toolkit-0.6.4/vot_toolkit.egg-info/
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3769 2023-05-31 07:41:25.000000 vot-toolkit-0.6.4/vot_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2411 2023-05-31 07:41:25.000000 vot-toolkit-0.6.4/vot_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        1 2023-05-31 07:41:25.000000 vot-toolkit-0.6.4/vot_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       48 2023-05-31 07:41:25.000000 vot-toolkit-0.6.4/vot_toolkit.egg-info/entry_points.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2023-05-31 07:41:25.000000 vot-toolkit-0.6.4/vot_toolkit.egg-info/requires.txt
--rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        4 2023-05-31 07:41:25.000000 vot-toolkit-0.6.4/vot_toolkit.egg-info/top_level.txt
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    35149 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/LICENSE
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      205 2024-04-21 18:27:03.000000 vot-toolkit-0.7.0/MANIFEST.in
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3548 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/PKG-INFO
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2919 2024-04-18 08:40:54.000000 vot-toolkit-0.7.0/README.md
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      295 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/requirements.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       38 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/setup.cfg
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1427 2023-05-09 11:09:24.000000 vot-toolkit-0.7.0/setup.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.770643 vot-toolkit-0.7.0/vot/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4545 2024-04-21 09:13:18.000000 vot-toolkit-0.7.0/vot/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      254 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/__main__.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.770643 vot-toolkit-0.7.0/vot/analysis/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    24213 2024-04-20 20:32:32.000000 vot-toolkit-0.7.0/vot/analysis/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    17333 2024-04-21 16:09:08.000000 vot-toolkit-0.7.0/vot/analysis/accuracy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3872 2024-04-21 13:51:39.000000 vot-toolkit-0.7.0/vot/analysis/failures.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    29495 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/analysis/longterm.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    17775 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/analysis/multistart.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    30789 2024-04-20 20:39:42.000000 vot-toolkit-0.7.0/vot/analysis/processor.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14055 2024-04-21 14:36:12.000000 vot-toolkit-0.7.0/vot/analysis/supervised.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      591 2024-04-21 16:05:33.000000 vot-toolkit-0.7.0/vot/analysis/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.770643 vot-toolkit-0.7.0/vot/dataset/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    39096 2024-04-18 08:34:19.000000 vot-toolkit-0.7.0/vot/dataset/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    12821 2024-04-18 08:34:19.000000 vot-toolkit-0.7.0/vot/dataset/common.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14672 2020-12-04 15:25:26.000000 vot-toolkit-0.7.0/vot/dataset/cow.png
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3545 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/dataset/dummy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4216 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/dataset/got10k.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    11383 2024-04-20 20:38:34.000000 vot-toolkit-0.7.0/vot/dataset/otb.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    14274 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/dataset/proxy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3828 2024-04-12 12:03:00.000000 vot-toolkit-0.7.0/vot/dataset/trackingnet.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.774643 vot-toolkit-0.7.0/vot/experiment/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    13889 2024-04-21 16:38:01.000000 vot-toolkit-0.7.0/vot/experiment/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1702 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/experiment/helpers.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10048 2024-01-16 15:51:12.000000 vot-toolkit-0.7.0/vot/experiment/multirun.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4945 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/experiment/multistart.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6040 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/experiment/transformer.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.774643 vot-toolkit-0.7.0/vot/region/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3728 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/region/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10604 2024-04-18 08:34:19.000000 vot-toolkit-0.7.0/vot/region/io.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    15220 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/region/raster.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16612 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/region/shapes.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4202 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/region/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.774643 vot-toolkit-0.7.0/vot/report/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    24824 2024-04-21 18:05:49.000000 vot-toolkit-0.7.0/vot/report/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      465 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/report/commands.tex
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9966 2024-04-21 17:02:49.000000 vot-toolkit-0.7.0/vot/report/common.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7543 2024-04-21 17:09:49.000000 vot-toolkit-0.7.0/vot/report/html.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    89476 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/report/jquery.js
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     6753 2024-04-21 09:38:48.000000 vot-toolkit-0.7.0/vot/report/latex.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    16184 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/report/pure.css
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2160 2024-04-21 10:45:44.000000 vot-toolkit-0.7.0/vot/report/report.css
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1212 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/report/report.js
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9933 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/report/table.js
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        0 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/report/tests.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4125 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/report/video.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.774643 vot-toolkit-0.7.0/vot/stack/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3929 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/stack/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      249 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/stack/otb100.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      247 2024-03-18 10:30:36.000000 vot-toolkit-0.7.0/vot/stack/otb50.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.774643 vot-toolkit-0.7.0/vot/stack/tests/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      184 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/stack/tests/basic.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      541 2023-05-16 13:31:56.000000 vot-toolkit-0.7.0/vot/stack/tests/multiobject.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      638 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/tests/segmentation.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      969 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/stack/tests.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      351 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2013.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      374 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2014.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.774643 vot-toolkit-0.7.0/vot/stack/vot2015/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      405 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2015/rgb.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      322 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2015/tir.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.774643 vot-toolkit-0.7.0/vot/stack/vot2016/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      542 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/stack/vot2016/rgb.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      303 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/stack/vot2016/tir.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      856 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2017.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.774643 vot-toolkit-0.7.0/vot/stack/vot2018/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2018/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      791 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2018/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.774643 vot-toolkit-0.7.0/vot/stack/vot2019/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2019/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2019/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2019/rgbtir.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      789 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2019/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/vot/stack/vot2020/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2020/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2020/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      396 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2020/rgbtir.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2020/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/vot/stack/vot2021/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      486 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/stack/vot2021/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      300 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2021/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      867 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/stack/vot2021/shortterm.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/vot/stack/vot2022/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      422 2023-05-05 11:01:43.000000 vot-toolkit-0.7.0/vot/stack/vot2022/depth.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      482 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/stack/vot2022/longterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      424 2022-03-25 11:28:05.000000 vot-toolkit-0.7.0/vot/stack/vot2022/rgbd.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/stack/vot2022/shortterm.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      875 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/stack/vot2022/shorttermbox.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      193 2023-05-10 17:51:17.000000 vot-toolkit-0.7.0/vot/stack/vots2023.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/vot/stack/vots2024/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      193 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/stack/vots2024/main.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      193 2024-04-18 08:34:19.000000 vot-toolkit-0.7.0/vot/stack/vots2024/votst.yaml
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      688 2024-04-18 08:34:19.000000 vot-toolkit-0.7.0/vot/stack/vots2024/votstval.yaml
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/vot/tracker/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    33466 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/tracker/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      808 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/tracker/dummy.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     9417 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/tracker/results.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      631 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/tracker/tests.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    29426 2024-04-12 12:01:42.000000 vot-toolkit-0.7.0/vot/tracker/trax.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/vot/utilities/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    21476 2024-04-21 16:29:00.000000 vot-toolkit-0.7.0/vot/utilities/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    22345 2024-04-21 09:12:45.000000 vot-toolkit-0.7.0/vot/utilities/cli.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     5740 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/utilities/data.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10476 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/utilities/draw.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     4351 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/utilities/migration.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7113 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/utilities/net.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    10059 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/utilities/notebook.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       45 2024-04-18 08:34:19.000000 vot-toolkit-0.7.0/vot/version.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/vot/workspace/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     7922 2024-04-21 16:18:22.000000 vot-toolkit-0.7.0/vot/workspace/__init__.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)    13864 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/workspace/storage.py
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     1840 2023-06-14 09:31:05.000000 vot-toolkit-0.7.0/vot/workspace/tests.py
+drwxrwxr-x   0 lukacu    (1000) lukacu    (1000)        0 2024-04-21 18:30:28.778643 vot-toolkit-0.7.0/vot_toolkit.egg-info/
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     3548 2024-04-21 18:30:28.000000 vot-toolkit-0.7.0/vot_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)     2565 2024-04-21 18:30:28.000000 vot-toolkit-0.7.0/vot_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        1 2024-04-21 18:30:28.000000 vot-toolkit-0.7.0/vot_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)       48 2024-04-21 18:30:28.000000 vot-toolkit-0.7.0/vot_toolkit.egg-info/entry_points.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)      296 2024-04-21 18:30:28.000000 vot-toolkit-0.7.0/vot_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 lukacu    (1000) lukacu    (1000)        4 2024-04-21 18:30:28.000000 vot-toolkit-0.7.0/vot_toolkit.egg-info/top_level.txt
```

### Comparing `vot-toolkit-0.6.4/PKG-INFO` & `vot-toolkit-0.7.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 Metadata-Version: 2.1
 Name: vot-toolkit
-Version: 0.6.4
+Version: 0.7.0
 Summary: Perform visual object tracking experiments and analyze results
 Home-page: https://github.com/votchallenge/toolkit
 Author: Luka Cehovin Zajc
 Author-email: luka.cehovin@gmail.com
 License: UNKNOWN
-Description: 
-        The VOT evaluation toolkit
-        ==========================
-        
-        [![PyPI package version](https://badge.fury.io/py/vot-toolkit.svg)](https://badge.fury.io/py/vot-toolkit)
-        
-        This repository contains the official evaluation toolkit for the [Visual Object Tracking (VOT) challenge](http://votchallenge.net/). This is the official version of the toolkit, implemented in Python 3 language. If you are looking for the old Matlab version, you can find an archived repository [here](https://github.com/votchallenge/toolkit-legacy).
-        
-        For more detailed informations consult the documentation available in the source or a compiled version of the documentation [here](http://www.votchallenge.net/howto/). You can also subscribe to the VOT [mailing list](https://liste.arnes.si/mailman3/lists/votchallenge.lists.arnes.si/) to receive news about challenges and important software updates or join our [support form](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help) to ask questions.
-        
-        Developers
-        ----------
-        
-        The VOT toolkit is developed and maintained by  [Luka Čehovin Zajc](https://vicos.si/lukacu) with the help of the VOT innitiative members and the VOT community.
-        
-        Contributors:
-        
-        * [Luka Čehovin Zajc](https://vicos.si/lukacu), University of Ljubljana
-        * [Alan Lukežič](https://vicos.si/people/alan_lukezic/), University of Ljubljana
-        * Yan Song, Tampere University
-        
-        Acknowledgements
-        ----------------
-        
-        The development of this package was supported by Sloveninan research agency (ARRS) projects Z2-1866 and J2-316.
-        
-        License
-        -------
-        
-        Copyright (C) 2023 Luka Čehovin Zajc and the [VOT Challenge innitiative](http://votchallenge.net/).
-        
-        This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
-        
-        This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-        
-        You should have received a copy of the GNU General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.
-        
-        Enquiries, Question and Comments
-        --------------------------------
-        
-        If you have any further enquiries, question, or comments, please refer to the contact information link on the [VOT homepage](http://votchallenge.net/). If you would like to file a bug report or a feature request, use the  [Github issue tracker](https://github.com/votchallenge/toolkit/issues). **The issue tracker is for toolkit issues only**, if you have a problem with tracker integration or any other questions, please use our [support forum](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help).
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+The VOT evaluation toolkit
+==========================
+
+[![Documentation Status](https://readthedocs.org/projects/vot-toolkit/badge/?version=latest)](https://vot-toolkit.readthedocs.io/en/latest/?badge=latest)
+[![PyPI package version](https://badge.fury.io/py/vot-toolkit.svg)](https://badge.fury.io/py/vot-toolkit)
+
+This repository contains the official evaluation toolkit for the [Visual Object Tracking (VOT) challenge](http://votchallenge.net/). This is the official version of the toolkit, implemented in Python 3 language. If you are looking for the old Matlab version, you can find an archived repository [here](https://github.com/votchallenge/toolkit-legacy).
+
+For more detailed informations consult the documentation available [here](http://vot-toolkit.readthedocs.io/). You can also subscribe to the VOT [mailing list](https://liste.arnes.si/mailman3/lists/votchallenge.lists.arnes.si/) to receive news about challenges and important software updates or join our [support form](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help) to ask questions.
+
+Developers
+----------
+
+The VOT toolkit is developed and maintained by  [Luka Čehovin Zajc](https://vicos.si/lukacu) with the help of the VOT innitiative members and the VOT community.
+
+Contributors:
+
+* [Luka Čehovin Zajc](https://vicos.si/lukacu), University of Ljubljana
+* [Alan Lukežič](https://vicos.si/people/alan_lukezic/), University of Ljubljana
+* Yan Song, Tampere University
+
+Acknowledgements
+----------------
+
+The development of this package was supported by Slovenian research agency (ARRS) projects Z2-1866 and J2-316.
+
+License
+-------
+
+Copyright (C) 2024 Luka Čehovin Zajc and the [VOT Challenge innitiative](http://votchallenge.net/).
+
+This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+
+This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+Enquiries, Question and Comments
+--------------------------------
+
+If you have any further enquiries, question, or comments, please refer to the contact information link on the [VOT homepage](http://votchallenge.net/). If you would like to file a bug report or a feature request, use the  [Github issue tracker](https://github.com/votchallenge/toolkit/issues). **The issue tracker is for toolkit issues only**, if you have a problem with tracker integration or any other questions, please use our [support forum](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help).
+
+
```

### Comparing `vot-toolkit-0.6.4/README.md` & `vot-toolkit-0.7.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 
 The VOT evaluation toolkit
 ==========================
 
+[![Documentation Status](https://readthedocs.org/projects/vot-toolkit/badge/?version=latest)](https://vot-toolkit.readthedocs.io/en/latest/?badge=latest)
 [![PyPI package version](https://badge.fury.io/py/vot-toolkit.svg)](https://badge.fury.io/py/vot-toolkit)
 
 This repository contains the official evaluation toolkit for the [Visual Object Tracking (VOT) challenge](http://votchallenge.net/). This is the official version of the toolkit, implemented in Python 3 language. If you are looking for the old Matlab version, you can find an archived repository [here](https://github.com/votchallenge/toolkit-legacy).
 
-For more detailed informations consult the documentation available in the source or a compiled version of the documentation [here](http://www.votchallenge.net/howto/). You can also subscribe to the VOT [mailing list](https://liste.arnes.si/mailman3/lists/votchallenge.lists.arnes.si/) to receive news about challenges and important software updates or join our [support form](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help) to ask questions.
+For more detailed informations consult the documentation available [here](http://vot-toolkit.readthedocs.io/). You can also subscribe to the VOT [mailing list](https://liste.arnes.si/mailman3/lists/votchallenge.lists.arnes.si/) to receive news about challenges and important software updates or join our [support form](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help) to ask questions.
 
 Developers
 ----------
 
 The VOT toolkit is developed and maintained by  [Luka Čehovin Zajc](https://vicos.si/lukacu) with the help of the VOT innitiative members and the VOT community.
 
 Contributors:
@@ -18,20 +19,20 @@
 * [Luka Čehovin Zajc](https://vicos.si/lukacu), University of Ljubljana
 * [Alan Lukežič](https://vicos.si/people/alan_lukezic/), University of Ljubljana
 * Yan Song, Tampere University
 
 Acknowledgements
 ----------------
 
-The development of this package was supported by Sloveninan research agency (ARRS) projects Z2-1866 and J2-316.
+The development of this package was supported by Slovenian research agency (ARRS) projects Z2-1866 and J2-316.
 
 License
 -------
 
-Copyright (C) 2023 Luka Čehovin Zajc and the [VOT Challenge innitiative](http://votchallenge.net/).
+Copyright (C) 2024 Luka Čehovin Zajc and the [VOT Challenge innitiative](http://votchallenge.net/).
 
 This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
 
 This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `vot-toolkit-0.6.4/setup.py` & `vot-toolkit-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/__init__.py` & `vot-toolkit-0.7.0/vot/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,15 @@
 """ Some basic functions and classes used by the toolkit. """
 
 import os
 import logging
 
 from .version import __version__
 
-_logger = logging.getLogger("vot")
-
-def get_logger() -> logging.Logger:
-    """Returns the default logger object used to log different messages.
-
-    Returns:
-        logging.Logger: Logger handle
-    """
-    return _logger
+from lazy_object_proxy import Proxy
 
 class ToolkitException(Exception):
     """Base class for all toolkit related exceptions
     """
     pass
 
 
@@ -62,45 +54,82 @@
 
     else:
         return False, None
 
 from attributee import Attributee, Integer, Boolean
 
 class GlobalConfiguration(Attributee):
-    """Global configuration object for the toolkit. It is used to store global configuration options.
+    """Global configuration object for the toolkit. It is used to store global configuration options. It can be initialized
+    from environment variables. The following options are supported:
+
+    - ``VOT_DEBUG_MODE``: Enables debug mode for the toolkit.
+    - ``VOT_SEQUENCE_CACHE_SIZE``: Maximum number of sequences to keep in cache.
+    - ``VOT_RESULTS_BINARY``: Enables binary results format.
+    - ``VOT_MASK_OPTIMIZE_READ``: Enables mask optimization when reading masks.
+    - ``VOT_WORKER_POOL_SIZE``: Number of workers to use for parallel processing.
+    - ``VOT_PERSISTENT_CACHE``: Enables persistent cache for analysis results in workspace.
+
     """
 
     debug_mode = Boolean(default=False, description="Enables debug mode for the toolkit.")
-    sequence_cache_size = Integer(default=1000, description="Maximum number of sequences to keep in cache.")
+    sequence_cache_size = Integer(default=100, description="Maximum number of sequences to keep in cache.")
     results_binary = Boolean(default=True, description="Enables binary results format.")
     mask_optimize_read = Boolean(default=True, description="Enables mask optimization when reading masks.")
+    worker_pool_size = Integer(default=1, description="Number of workers to use for parallel processing.")
+    persistent_cache = Boolean(default=True, description="Enables persistent cache for analysis results in workspace.")
 
     def __init__(self):
         """Initializes the global configuration object. It reads the configuration from environment variables.
         
         Raises:
             ValueError: When an invalid value is provided for an attribute.
         """
+        
         kwargs = {}
         for k in self.attributes():
             envname = "VOT_{}".format(k.upper())
             if envname in os.environ:
                 kwargs[k] = os.environ[envname]
         super().__init__(**kwargs)
-        _logger.debug("Global configuration: %s", self)
 
     def __repr__(self):
         """Returns a string representation of the global configuration object."""
-        return "debug_mode={} sequence_cache_size={} results_binary={} mask_optimize_read={}".format(
-            self.debug_mode, self.sequence_cache_size, self.results_binary, self.mask_optimize_read
-        )
+        return " ".join(["{}={}".format(k, getattr(self, k)) for k in self.attributes()])
+
+#_logger = None
+
+from vot.utilities import singleton
+
+@singleton
+def get_logger() -> logging.Logger:
+    """Returns the default logger object used to log different messages.
+
+    Returns:
+        logging.Logger: Logger handle
+    """
+
+    def init():
+        from .utilities import ColoredFormatter
+        logger = logging.getLogger("vot")
+        stream = logging.StreamHandler()
+        stream.setFormatter(ColoredFormatter())
+        logger.addHandler(stream)
+        if check_debug():
+            logger.setLevel(logging.DEBUG)
+        return logger
+
+    return Proxy(init)
 
-config = GlobalConfiguration()
+config = Proxy(lambda: GlobalConfiguration())
 
 def check_debug() -> bool:
     """Checks if debug is enabled for the toolkit via an environment variable.
 
     Returns:
         bool: True if debug is enabled, False otherwise
     """
     return config.debug_mode
 
+def print_config():
+    """Prints the global configuration object to the logger."""
+    if check_debug():
+        get_logger().debug("Configuration: %s", config)
```

### Comparing `vot-toolkit-0.6.4/vot/analysis/__init__.py` & `vot-toolkit-0.7.0/vot/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/analysis/accuracy.py` & `vot-toolkit-0.7.0/vot/analysis/accuracy.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 """Accuracy analysis. Computes average overlap between predicted and groundtruth regions."""
 
 from typing import List, Tuple, Any
 
 import numpy as np
 
-from attributee import Boolean, Integer, Include, Float
+from attributee import Boolean, Integer, Include, Float, String
 
 from vot.analysis import (Measure,
                           MissingResultsException,
                           SequenceAggregator, Sorting,
                           is_special, SeparableAnalysis,
                           analysis_registry, Curve)
 from vot.dataset import Sequence
 from vot.experiment import Experiment
 from vot.experiment.multirun import (MultiRunExperiment)
 from vot.region import Region, calculate_overlaps
 from vot.tracker import Tracker, Trajectory
 from vot.utilities.data import Grid
 
 def gather_overlaps(trajectory: List[Region], groundtruth: List[Region], burnin: int = 10, 
-    ignore_unknown: bool = True, ignore_invisible: bool = False, bounds = None, threshold: float = None) -> np.ndarray:
+    ignore_unknown: bool = True, ignore_invisible: bool = False, bounds = None, threshold: float = None, ignore_masks: List[Region] = None) -> np.ndarray:
     """Gather overlaps between trajectory and groundtruth regions. 
     
     Args:
         trajectory (List[Region]): List of regions predicted by the tracker.
         groundtruth (List[Region]): List of groundtruth regions.
         burnin (int, optional): Number of frames to skip at the beginning of the sequence. Defaults to 10.
         ignore_unknown (bool, optional): Ignore unknown regions in the groundtruth. Defaults to True.
         ignore_invisible (bool, optional): Ignore invisible regions in the groundtruth. Defaults to False.
         bounds ([type], optional): Bounds of the sequence. Defaults to None.
         threshold (float, optional): Minimum overlap to consider. Defaults to None.
+        ignore_masks (List[Region], optional): List of regions to ignore. Defaults to None.
         
     Returns:
         np.ndarray: List of overlaps."""
 
-    overlaps = np.array(calculate_overlaps(trajectory, groundtruth, bounds))
+    assert len(trajectory) == len(groundtruth), "Trajectory and groundtruth must have the same length."
+
+    if ignore_masks is not None:
+        assert len(trajectory) == len(ignore_masks), "Trajectory and ignore mask must have the same length."
+
+    overlaps = np.array(calculate_overlaps(trajectory, groundtruth, bounds, ignore=ignore_masks))
     mask = np.ones(len(overlaps), dtype=bool)
 
     if threshold is None: threshold = -1
 
     for i, (region_tr, region_gt) in enumerate(zip(trajectory, groundtruth)):
         # Skip if groundtruth is unknown
         if is_special(region_gt, Sequence.UNKNOWN):
@@ -53,25 +59,99 @@
             for j in range(i, min(len(trajectory), i + burnin)):
                 mask[j] = False
         elif is_special(region_tr, Trajectory.FAILURE):
             mask[i] = False
         elif overlaps[i] <= threshold:
             mask[i] = False
 
-    return overlaps[mask]
+    return overlaps[mask], [i for i in range(len(overlaps)) if mask[i]]
+
+class Overlaps(SeparableAnalysis):
+    """Overlaps analysis. Computes overlaps between predicted and groundtruth regions."""
+
+    burnin = Integer(default=10, val_min=0, description="Number of frames to skip after the initialization.")
+    ignore_unknown = Boolean(default=True, description="Ignore unknown regions in the groundtruth.")
+    ignore_invisible = Boolean(default=False, description="Ignore invisible regions in the groundtruth.")
+    bounded = Boolean(default=True, description="Consider only the bounded region of the sequence.")
+    threshold = Float(default=None, val_min=0, val_max=1, description="Minimum overlap to consider.")
+    ignore_masks = String(default="_ignore", description="Object ID used to get ignore masks.")
+    filter_tag = String(default=None, description="Filter tag for the analysis.")
+
+    def compatible(self, experiment: Experiment):
+        """Check if the experiment is compatible with the analysis."""
+        return isinstance(experiment, MultiRunExperiment)
+
+    @property
+    def _title_default(self):
+        """Default title of the analysis."""
+        return "Overlaps"
+
+    def describe(self):
+        """Describe the analysis."""
+        return Measure(self.title, "", 0, 1, Sorting.DESCENDING),
+
+    def subcompute(self, experiment: Experiment, tracker: Tracker, sequence: Sequence, dependencies: List[Grid]) -> Tuple[Any]:
+        """Compute the analysis for a single sequence. 
+        
+        Args:
+            experiment (Experiment): Experiment.
+            tracker (Tracker): Tracker.
+            sequence (Sequence): Sequence.
+            dependencies (List[Grid]): List of dependencies.
+            
+        Returns:
+            Tuple[Any]: Tuple of results.
+        """
+        assert isinstance(experiment, MultiRunExperiment)
+
+        objects = sequence.objects()
+        bounds = (sequence.size) if self.bounded else None
+
+        ignore_masks = sequence.object(self.ignore_masks)
+
+        if self.filter_tag is not None:
+            frame_mask = [self.filter_tag in sequence.tags(i) for i in range(len(sequence))]
+        else:
+            frame_mask = None
+
+        results = []
+
+        for object in objects:
+            trajectories = experiment.gather(tracker, sequence, objects=[object])
+            if len(trajectories) == 0:
+                raise MissingResultsException()
+
+            for trajectory in trajectories:
+                if frame_mask is not None:
+                    trajectory = [region for region, m in zip(trajectory, frame_mask) if m]
+                    groundtruth = [region for region, m in zip(sequence.object(object), frame_mask) if m]
+                    masks = [region for region, m in zip(ignore_masks, frame_mask) if m]
+                else:
+                    trajectory = trajectory
+                    groundtruth = sequence.object(object)
+                    masks = ignore_masks
+                    
+                overlaps, frames = gather_overlaps(trajectory, groundtruth, self.burnin, 
+                                        ignore_unknown=self.ignore_unknown, ignore_invisible=self.ignore_invisible, bounds=bounds, threshold=self.threshold, ignore_masks=masks)
+
+                results.append((object, overlaps, frames))
+
+        return results,
 
 @analysis_registry.register("accuracy")
 class SequenceAccuracy(SeparableAnalysis):
     """Sequence accuracy analysis. Computes average overlap between predicted and groundtruth regions."""
 
     burnin = Integer(default=10, val_min=0, description="Number of frames to skip after the initialization.")
     ignore_unknown = Boolean(default=True, description="Ignore unknown regions in the groundtruth.")
     ignore_invisible = Boolean(default=False, description="Ignore invisible regions in the groundtruth.")    
     bounded = Boolean(default=True, description="Consider only the bounded region of the sequence.")
     threshold = Float(default=None, val_min=0, val_max=1, description="Minimum overlap to consider.")
+    ignore_masks = String(default="_ignore", description="Object ID used to get ignore masks.")
+    filter_tag = String(default=None, description="Filter tag for the analysis.")
 
     def compatible(self, experiment: Experiment):
         """Check if the experiment is compatible with the analysis."""
         return isinstance(experiment, MultiRunExperiment)
 
     @property
     def _title_default(self):
@@ -96,24 +176,42 @@
         """
         assert isinstance(experiment, MultiRunExperiment)
 
         objects = sequence.objects()
         objects_accuracy = 0
         bounds = (sequence.size) if self.bounded else None
 
+        ignore_masks = sequence.object(self.ignore_masks)
+
+        if self.filter_tag is not None:
+            frame_mask = [self.filter_tag in sequence.tags(i) for i in range(len(sequence))]
+        else:
+            frame_mask = None
+
         for object in objects:
             trajectories = experiment.gather(tracker, sequence, objects=[object])
             if len(trajectories) == 0:
                 raise MissingResultsException()
 
             cummulative = 0
 
             for trajectory in trajectories:
-                overlaps = gather_overlaps(trajectory.regions(), sequence.object(object), self.burnin, 
-                                        ignore_unknown=self.ignore_unknown, ignore_invisible=self.ignore_invisible, bounds=bounds, threshold=self.threshold)
+                if frame_mask is not None:
+                    trajectory = [region for region, m in zip(trajectory, frame_mask) if m]
+                    groundtruth = [region for region, m in zip(sequence.object(object), frame_mask) if m]
+                    masks = [region for region, m in zip(ignore_masks, frame_mask) if m] 
+                else:
+                    trajectory = trajectory
+                    groundtruth = sequence.object(object)
+                    masks = ignore_masks
+
+                overlaps, _ = gather_overlaps(trajectory, groundtruth, self.burnin, 
+                                        ignore_unknown=self.ignore_unknown, ignore_invisible=self.ignore_invisible, bounds=bounds, threshold=self.threshold, ignore_masks=masks)
+                
+                
                 if overlaps.size > 0:
                     cummulative += np.mean(overlaps)
 
             objects_accuracy += cummulative / len(trajectories)
 
         return objects_accuracy / len(objects),
 
@@ -175,14 +273,16 @@
 
     ignore_unknown = Boolean(default=True, description="Ignore unknown regions in the groundtruth.")
     ignore_invisible = Boolean(default=False, description="Ignore invisible regions in the groundtruth.")
     burnin = Integer(default=0, val_min=0, description="Number of frames to skip after the initialization.")
     bounded = Boolean(default=True, description="Consider only the bounded region of the sequence.")
     threshold = Float(default=None, val_min=0, val_max=1, description="Minimum overlap to consider.")
     resolution = Integer(default=100, val_min=2, description="Number of points in the plot.")
+    ignore_masks = String(default="_ignore", description="Object ID used to get ignore masks.")
+    filter_tag = String(default=None, description="Filter tag for the analysis.")
 
     def compatible(self, experiment: Experiment):
         """Check if the experiment is compatible with the analysis. This analysis is only compatible with multi-run experiments."""
         return isinstance(experiment, MultiRunExperiment)
 
     @property
     def _title_default(self):
@@ -210,23 +310,39 @@
 
         objects = sequence.objects()
         bounds = (sequence.size) if self.bounded else None
 
         axis_x = np.linspace(0, 1, self.resolution)
         axis_y = np.zeros_like(axis_x)
 
+        ignore_masks = sequence.object(self.ignore_masks)
+
         for object in objects:
             trajectories = experiment.gather(tracker, sequence, objects=[object])
             if len(trajectories) == 0:
                 raise MissingResultsException()
 
             object_y = np.zeros_like(axis_x) 
 
+            if self.filter_tag is not None:
+                frame_mask = [self.filter_tag in sequence.tags(i) for i in range(len(sequence))]
+            else:
+                frame_mask = None
+
             for trajectory in trajectories:
-                overlaps = gather_overlaps(trajectory.regions(), sequence.object(object), burnin=self.burnin, ignore_unknown=self.ignore_unknown, ignore_invisible=self.ignore_invisible, bounds=bounds, threshold=self.threshold)
+                if frame_mask is not None:
+                    trajectory = [region for region, m in zip(trajectory, frame_mask) if m]
+                    groundtruth = [region for region, m in zip(sequence.object(object), frame_mask) if m] 
+                    masks = [region for region, m in zip(ignore_masks, frame_mask) if m]
+                else:
+                    groundtruth = sequence.object(object)
+                    masks = ignore_masks
+        
+                overlaps, _ = gather_overlaps(trajectory, groundtruth, burnin=self.burnin, ignore_unknown=self.ignore_unknown, 
+                                            ignore_invisible=self.ignore_invisible, bounds=bounds, threshold=self.threshold, ignore_masks=masks)
 
                 for i, threshold in enumerate(axis_x):
                     if threshold == 1:
                         # Nicer handling of the edge case
                         object_y[i] += np.sum(overlaps >= threshold) / len(overlaps)
                     else:
                         object_y[i] += np.sum(overlaps > threshold) / len(overlaps)
```

### Comparing `vot-toolkit-0.6.4/vot/analysis/failures.py` & `vot-toolkit-0.7.0/vot/analysis/failures.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,27 +8,27 @@
                           MissingResultsException,
                           SequenceAggregator, Sorting,
                           is_special, SeparableAnalysis,
                           analysis_registry)
 from vot.dataset import Sequence
 from vot.experiment import Experiment
 from vot.experiment.multirun import (SupervisedExperiment)
-from vot.region import Region, Special, calculate_overlaps
+from vot.region import Region
 from vot.tracker import Tracker
 from vot.utilities.data import Grid
 
 
 def count_failures(trajectory: List[Region]) -> Tuple[int, int]:
-    """Count the number of failures in a trajectory. A failure is defined as a region that overlaps with a Special.FAILURE region."""
+    """Count the number of failures in a trajectory. A failure is defined as a region is annotated as Special.FAILURE by the experiment."""
     return len([region for region in trajectory if is_special(region, SupervisedExperiment.FAILURE)]), len(trajectory)
 
 
 @analysis_registry.register("failures")
 class FailureCount(SeparableAnalysis):
-    """Count the number of failures in a sequence. A failure is defined as a region that overlaps with a Special.FAILURE region."""
+    """Count the number of failures in a sequence. A failure is defined as a region is annotated as Special.FAILURE by the experiment."""
 
     def compatible(self, experiment: Experiment):
         """Check if the experiment is compatible with the analysis."""
         return isinstance(experiment, SupervisedExperiment)
 
     @property
     def _title_default(self):
@@ -57,15 +57,15 @@
                 failures = failures + count_failures(trajectory.regions())[0]
             objects_failures += failures / len(trajectories)
 
         return objects_failures / len(objects), len(sequence)
 
 @analysis_registry.register("cumulative_failures")
 class CumulativeFailureCount(SequenceAggregator):
-    """Count the number of failures in a sequence. A failure is defined as a region that overlaps with a Special.FAILURE region."""
+    """Count the number of failures over all sequences. A failure is defined as a region is annotated as Special.FAILURE by the experiment."""
 
     analysis = Include(FailureCount)
 
     def compatible(self, experiment: Experiment):
         """Check if the experiment is compatible with the analysis."""
         return isinstance(experiment, SupervisedExperiment)
```

### Comparing `vot-toolkit-0.6.4/vot/analysis/longterm.py` & `vot-toolkit-0.7.0/vot/analysis/longterm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This module contains the implementation of the long term tracking performance measures."""
 import math
 import numpy as np
 from typing import List, Iterable, Tuple, Any
 import itertools
 
-from attributee import Float, Integer, Boolean, Include
+from attributee import Float, Integer, Boolean, Include, String
 
 from vot.tracker import Tracker
 from vot.dataset import Sequence
 from vot.region import Region, RegionType, calculate_overlaps
 from vot.experiment import Experiment
 from vot.experiment.multirun import UnsupervisedExperiment, MultiRunExperiment
 from vot.analysis import SequenceAggregator, Analysis, SeparableAnalysis, \
@@ -39,30 +39,34 @@
 
     thresholds.insert(0, math.inf)
     thresholds.insert(len(thresholds), -math.inf)
 
     return thresholds
 
 def compute_tpr_curves(trajectory: List[Region], confidence: List[float], sequence: Sequence, thresholds: List[float],
-    ignore_unknown: bool = True, bounded: bool = True):
+    ignore_unknown: bool = True, bounded: bool = True, ignore_masks: List[Region] = None) -> Tuple[List[float], List[float]]:
     """Compute the TPR curves for a given trajectory and confidence scores. 
     
     Args:
         trajectory (List[Region]): Trajectory to compute the TPR curves for.
         confidence (List[float]): Confidence scores for the trajectory.
         sequence (Sequence): Sequence to compute the TPR curves for.
         thresholds (List[float]): Thresholds to compute the TPR curves for.
         ignore_unknown (bool, optional): Ignore unknown regions. Defaults to True.
         bounded (bool, optional): Bounded evaluation. Defaults to True.
+        ignore_masks (List[Region], optional): Ignore masks. Defaults to None.
 
     Returns:
         List[float], List[float]: TPR curves for the given thresholds.
     """
+    assert len(trajectory) == len(confidence), "Trajectory and confidence must have the same length"
+    if ignore_masks is not None:
+        assert len(trajectory) == len(ignore_masks), "Trajectory and ignore masks must have the same length"
 
-    overlaps = np.array(calculate_overlaps(trajectory, sequence.groundtruth(), (sequence.size) if bounded else None))
+    overlaps = np.array(calculate_overlaps(trajectory, sequence.groundtruth(), (sequence.size) if bounded else None, ignore=ignore_masks))
     confidence = np.array(confidence)
 
     n_visible = len([region for region in sequence.groundtruth() if region.type is not RegionType.SPECIAL])
 
     precision = len(thresholds) * [float(0)]
     recall = len(thresholds) * [float(0)]
 
@@ -160,14 +164,15 @@
 @analysis_registry.register("pr_curves")
 class PrecisionRecallCurves(SeparableAnalysis):
     """ Computes the precision/recall curves for a tracker for given sequences. """
 
     thresholds = Include(_Thresholds)
     ignore_unknown = Boolean(default=True, description="Ignore unknown regions")
     bounded = Boolean(default=True, description="Bounded evaluation")
+    ignore_masks = String(default="_ignore", description="Object ID used to get ignore masks.")
 
     @property
     def _title_default(self):
         """Title of the analysis."""
         return "Tracking precision/recall"
 
     def describe(self):
@@ -195,22 +200,24 @@
             Tuple[Any]: Precision/recall curves for the given sequence.
         """
 
         thresholds = dependencies[0, 0][0][0] # dependencies[0][0, 0]
 
         trajectories = experiment.gather(tracker, sequence)
 
+        ignore_masks = sequence.object(self.ignore_masks)
+
         if len(trajectories) == 0:
             raise MissingResultsException()
 
         precision = len(thresholds) * [float(0)]
         recall = len(thresholds) * [float(0)]
         for trajectory in trajectories:
             confidence = [trajectory.properties(i).get('confidence', 0) for i in range(len(trajectory))]
-            pr, re = compute_tpr_curves(trajectory.regions(), confidence, sequence, thresholds, self.ignore_unknown, self.bounded)
+            pr, re = compute_tpr_curves(trajectory.regions(), confidence, sequence, thresholds, self.ignore_unknown, self.bounded, ignore_masks=ignore_masks)
             for i in range(len(thresholds)):
                 precision[i] += pr[i]
                 recall[i] += re[i]
 
 #         return [(re / len(trajectories), pr / len(trajectories)) for pr, re in zip(precision, recall)], thresholds
         return [(pr / len(trajectories), re / len(trajectories)) for pr, re in zip(precision, recall)], thresholds
 
@@ -372,28 +379,34 @@
 
     @property
     def axes(self):
         """Axes of the analysis."""
         return Axes.TRACKERS
 
 
-def count_frames(trajectory: List[Region], groundtruth: List[Region], bounds = None, threshold: float = 0) -> float:
+def count_frames(trajectory: List[Region], groundtruth: List[Region], bounds = None, threshold: float = 0, ignore_masks: List[Region] = None) -> float:
     """Counts the number of frames where the tracker is correct, fails, misses, hallucinates or notices an object.
     
     Args:
         trajectory (List[Region]): Trajectory of the tracker.
         groundtruth (List[Region]): Groundtruth trajectory.
         bounds (Optional[Region]): Bounds of the sequence.
         threshold (float): Threshold for the overlap.
+        ignore_masks (List[Region]): Ignore masks.
         
     Returns:
         float: Number of frames where the tracker is correct, fails, misses, hallucinates or notices an object.
     """
 
-    overlaps = np.array(calculate_overlaps(trajectory, groundtruth, bounds))
+    assert len(trajectory) == len(groundtruth), "Trajectory and groundtruth must have the same length"
+
+    if ignore_masks is not None:
+        assert len(trajectory) == len(ignore_masks), "Trajectory and ignore masks must have the same length"
+
+    overlaps = np.array(calculate_overlaps(trajectory, groundtruth, bounds, ignore=ignore_masks))
     if threshold is None: threshold = -1
 
     # Tracking, Failure, Miss, Halucination, Notice
     T, F, M, H, N = 0, 0, 0, 0, 0
 
     for i, (region_tr, region_gt) in enumerate(zip(trajectory, groundtruth)):
         if (is_special(region_gt, Sequence.UNKNOWN)):
@@ -410,19 +423,41 @@
                 if region_tr.is_empty():
                     M += 1
                 else:
                     F += 1
 
     return T, F, M, H, N
 
+class SafeAverage(object):
+    
+    def __init__(self):
+        self._sum = 0
+        self._count = 0
+
+    def add(self, value):
+        if value is None:
+            return
+        self._sum += value
+        self._count += 1
+
+    def average(self):
+        if self._count == 0:
+            return None
+        return self._sum / self._count
+    
+    def empty(self):
+        return self._count == 0
+
 class CountFrames(SeparableAnalysis):
     """Counts the number of frames where the tracker is correct, fails, misses, hallucinates or notices an object."""
 
     threshold = Float(default=0.0, val_min=0, val_max=1)
     bounded = Boolean(default=True)
+    ignore_masks = String(default="_ignore", description="Object ID used to get ignore masks.")
+    filter_tag = String(default=None, description="Filter tag for the analysis.")
 
     def compatible(self, experiment: Experiment):
         """Checks if the experiment is compatible with the analysis. This analysis is compatible with multi-run experiments."""
         return isinstance(experiment, MultiRunExperiment)
 
     def describe(self):
         """Describes the analysis."""
@@ -433,23 +468,39 @@
 
         assert isinstance(experiment, MultiRunExperiment)
 
         objects = sequence.objects()
         distribution = []
         bounds = (sequence.size) if self.bounded else None
 
+        ignore_masks = sequence.object(self.ignore_masks)
+
+        if self.filter_tag is not None:
+            frame_mask = [self.filter_tag in sequence.tags(i) for i in range(len(sequence))]
+        else:
+            frame_mask = None
+
         for object in objects:
             trajectories = experiment.gather(tracker, sequence, objects=[object])
             if len(trajectories) == 0:
                 raise MissingResultsException()
 
             CN, CF, CM, CH, CT = 0, 0, 0, 0, 0
 
             for trajectory in trajectories:
-                T, F, M, H, N = count_frames(trajectory.regions(), sequence.object(object), bounds=bounds)
+                if frame_mask is not None:
+                    trajectory = [region for region, m in zip(trajectory, frame_mask) if m]
+                    groundtruth = [region for region, m in zip(sequence.object(object), frame_mask) if m]
+                    masks = [region for region, m in zip(ignore_masks, frame_mask) if m] 
+                else:
+                    trajectory = trajectory
+                    groundtruth = sequence.object(object)
+                    masks = ignore_masks
+                
+                T, F, M, H, N = count_frames(trajectory, groundtruth, bounds=bounds, ignore_masks=masks)
                 CN += N
                 CF += F
                 CM += M
                 CH += H
                 CT += T
             CN /= len(trajectories)
             CF /= len(trajectories)
@@ -465,28 +516,30 @@
 @analysis_registry.register("quality_auxiliary")
 class QualityAuxiliary(SeparableAnalysis):
     """Computes the non-reported error, drift-rate error and absence-detection quality."""
 
     threshold = Float(default=0.0, val_min=0, val_max=1)
     bounded = Boolean(default=True)
     absence_threshold = Integer(default=10, val_min=0)
+    ignore_masks = String(default="_ignore", description="Object ID used to get ignore masks.")
+    filter_tag = String(default=None, description="Filter tag for the analysis.")
 
     def compatible(self, experiment: Experiment):
         """Checks if the experiment is compatible with the analysis. This analysis is compatible with multi-run experiments."""
         return isinstance(experiment, MultiRunExperiment)
 
     @property
     def _title_default(self):
         """Default title of the analysis."""
         return "Quality Auxiliary"
 
     def describe(self):
         """Describes the analysis."""
-        return Measure("Non-reported Error", "NRE", 0, 1, Sorting.DESCENDING), \
-            Measure("Drift-rate Error", "DRE", 0, 1, Sorting.DESCENDING), \
+        return Measure("Non-reported Error", "NRE", 0, 1, Sorting.ASCENDING), \
+            Measure("Drift-rate Error", "DRE", 0, 1, Sorting.ASCENDING), \
             Measure("Absence-detection Quality", "ADQ", 0, 1, Sorting.DESCENDING),
 
     def subcompute(self, experiment: Experiment, tracker: Tracker, sequence: Sequence, dependencies: List[Grid]) -> Tuple[Any]:
         """Computes the non-reported error, drift-rate error and absence-detection quality.
         
         Args:
             experiment (Experiment): Experiment.
@@ -497,56 +550,65 @@
         Returns:
             Tuple[Any]: Non-reported error, drift-rate error and absence-detection quality.
 
         """
 
         assert isinstance(experiment, MultiRunExperiment)
 
-        not_reported_error = 0
-        drift_rate_error = 0
-        absence_detection = 0
+        not_reported_error = SafeAverage()
+        drift_rate_error = SafeAverage()
+        absence_detection = SafeAverage()
 
         objects = sequence.objects()
         bounds = (sequence.size) if self.bounded else None
 
-        absence_valid = 0
+        ignore_masks = sequence.object(self.ignore_masks)
+
+        if self.filter_tag is not None:
+            frame_mask = [self.filter_tag in sequence.tags(i) for i in range(len(sequence))]
+        else:
+            frame_mask = None
 
         for object in objects:
             trajectories = experiment.gather(tracker, sequence, objects=[object])
             if len(trajectories) == 0:
                 raise MissingResultsException()
 
             CN, CF, CM, CH, CT = 0, 0, 0, 0, 0
 
             for trajectory in trajectories:
-                T, F, M, H, N = count_frames(trajectory.regions(), sequence.object(object), bounds=bounds)
+                if frame_mask is not None:
+                    trajectory = [region for region, m in zip(trajectory, frame_mask) if m]
+                    groundtruth = [region for region, m in zip(sequence.object(object), frame_mask) if m]
+                    masks = [region for region, m in zip(ignore_masks, frame_mask) if m] 
+                else:
+                    trajectory = trajectory
+                    groundtruth = sequence.object(object)
+                    masks = ignore_masks
+                
+                T, F, M, H, N = count_frames(trajectory, groundtruth, bounds=bounds, ignore_masks=masks)
                 CN += N
                 CF += F
                 CM += M
                 CH += H
                 CT += T
             CN /= len(trajectories)
             CF /= len(trajectories)
             CM /= len(trajectories)
             CH /= len(trajectories)
             CT /= len(trajectories)
 
-            not_reported_error += CM / (CT + CF + CM)
-            drift_rate_error += CF / (CT + CF + CM)
+            if CT + CF + CM > 0:
+                not_reported_error.add(CM / (CT + CF + CM))
+                drift_rate_error.add(CF / (CT + CF + CM))
 
             if CN + CH > self.absence_threshold:
-                absence_detection += CN / (CN + CH)
-                absence_valid += 1
-
-        if absence_valid > 0:
-            absence_detection /= absence_valid
-        else:
-            absence_detection = None
+                absence_detection.add(CN / (CN + CH))
 
-        return not_reported_error / len(objects), drift_rate_error / len(objects), absence_detection,
+        return not_reported_error.average(), drift_rate_error.average(), absence_detection.average(),
 
 
 @analysis_registry.register("average_quality_auxiliary")
 class AverageQualityAuxiliary(SequenceAggregator):
     """Computes the average non-reported error, drift-rate error and absence-detection quality."""
 
     analysis = Include(QualityAuxiliary)
@@ -558,16 +620,16 @@
 
     def dependencies(self):
         """Returns the dependencies of the analysis."""
         return self.analysis,
 
     def describe(self):
         """Describes the analysis."""
-        return Measure("Non-reported Error", "NRE", 0, 1, Sorting.DESCENDING), \
-            Measure("Drift-rate Error", "DRE", 0, 1, Sorting.DESCENDING), \
+        return Measure("Non-reported Error", "NRE", 0, 1, Sorting.ASCENDING), \
+            Measure("Drift-rate Error", "DRE", 0, 1, Sorting.ASCENDING), \
             Measure("Absence-detection Quality", "ADQ", 0, 1, Sorting.DESCENDING),
 
     def compatible(self, experiment: Experiment):
         """Checks if the experiment is compatible with the analysis. This analysis is compatible with multi-run experiments."""
         return isinstance(experiment, MultiRunExperiment)
 
     def aggregate(self, tracker: Tracker, sequences: List[Sequence], results: Grid):
@@ -578,45 +640,41 @@
             sequences (List[Sequence]): Sequences.
             results (Grid): Results.
             
         Returns:
             Tuple[Any]: Non-reported error, drift-rate error and absence-detection quality.
         """
 
-        not_reported_error = 0
-        drift_rate_error = 0
-        absence_detection = 0
-        absence_count = 0
+        not_reported_error = SafeAverage()
+        drift_rate_error = SafeAverage()
+        absence_detection = SafeAverage()
 
         for nre, dre, ad in results:
-            not_reported_error += nre
-            drift_rate_error += dre
-            if ad is not None:
-                absence_count += 1
-                absence_detection += ad
+            not_reported_error.add(nre)
+            drift_rate_error.add(dre)
+            absence_detection.add(ad)
 
-        if absence_count > 0:
-            absence_detection /= absence_count
-
-        return not_reported_error / len(sequences), drift_rate_error / len(sequences), absence_detection
+        return not_reported_error.average(), drift_rate_error.average(), absence_detection.average(),
 
 from vot.analysis import SequenceAggregator
 from vot.analysis.accuracy import SequenceAccuracy
 
 @analysis_registry.register("longterm_ar")
 class AccuracyRobustness(Analysis):
     """Longterm multi-object accuracy-robustness measure. """
 
     threshold = Float(default=0.0, val_min=0, val_max=1)
     bounded = Boolean(default=True)
     counts = Include(CountFrames)
+    ignore_masks = String(default="_ignore", description="Object ID used to get ignore masks.")
+    filter_tag = String(default=None, description="Filter tag for the analysis.")
 
     def dependencies(self) -> List[Analysis]:
         """Returns the dependencies of the analysis."""
-        return self.counts, SequenceAccuracy(burnin=0, threshold=self.threshold, bounded=self.bounded, ignore_invisible=True, ignore_unknown=False)
+        return self.counts, SequenceAccuracy(burnin=0, threshold=self.threshold, bounded=self.bounded, ignore_invisible=True, ignore_unknown=False, ignore_masks=self.ignore_masks, filter_tag=self.filter_tag)
     
     def compatible(self, experiment: Experiment):
         """Checks if the experiment is compatible with the analysis. This analysis is compatible with multi-run experiments."""
         return isinstance(experiment, MultiRunExperiment)
 
     @property
     def _title_default(self):
@@ -645,33 +703,36 @@
 
         frame_counts = dependencies[0]
         accuracy_analysis = dependencies[1]
 
         results = Grid(len(trackers), 1)
 
         for j, _ in enumerate(trackers):
-            accuracy = 0
-            robustness = 0
-            count = 0
+            accuracy = SafeAverage()
+            robustness = SafeAverage()
 
             for i, _ in enumerate(sequences):
                 if accuracy_analysis[j, i] is None:
                     continue
 
-                accuracy += accuracy_analysis[j, i][0]
-
+                accuracy.add(accuracy_analysis[j, i][0])
                 frame_counts_sequence = frame_counts[j, i][0]
-
                 objects = len(frame_counts_sequence)
+                
+                sequence_robustness = SafeAverage()
+                
                 for o in range(objects):
-                    robustness += (1/objects) * frame_counts_sequence[o][0] / (frame_counts_sequence[o][0] + frame_counts_sequence[o][1] + frame_counts_sequence[o][2])
-
-                count += 1
-
-            results[j, 0] = (accuracy / count, robustness / count, (robustness / count, accuracy / count))
+                    
+                    n = (frame_counts_sequence[o][0] + frame_counts_sequence[o][1] + frame_counts_sequence[o][2])
+                    if n > 0: sequence_robustness.add(frame_counts_sequence[o][0] / n)
+
+                if not sequence_robustness.empty():
+                    robustness.add(sequence_robustness.average())
+                
+            results[j, 0] = (accuracy.average(), robustness.average(), (robustness.average(), accuracy.average()))
 
         return results
 
     @property
     def axes(self) -> Axes:
         """Returns the axes of the analysis."""
         return Axes.TRACKERS
```

### Comparing `vot-toolkit-0.6.4/vot/analysis/multistart.py` & `vot-toolkit-0.7.0/vot/analysis/multistart.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """This module contains the implementation of the accuracy-robustness analysis and EAO analysis for the multistart experiment."""
 
 from typing import List, Tuple, Any
 
 import numpy as np
 
-from attributee import Integer, Boolean, Float, Include
+from attributee import Integer, Boolean, Float, Include, String
 
 from vot.tracker import Tracker, Trajectory
 from vot.dataset import Sequence
 from vot.dataset.proxy import FrameMapSequence
 from vot.experiment import Experiment
 from vot.experiment.multistart import MultiStartExperiment, find_anchors
 from vot.region import calculate_overlaps
@@ -51,14 +51,15 @@
 class AccuracyRobustness(SeparableAnalysis):
     """This analysis computes the accuracy-robustness curve for the multistart experiment."""
 
     burnin = Integer(default=10, val_min=0)
     grace = Integer(default=10, val_min=0)
     bounded = Boolean(default=True)
     threshold = Float(default=0.1, val_min=0, val_max=1)
+    ignore_masks = String(default="_ignore", description="Object ID used to get ignore masks.")
 
     @property
     def _title_default(self):
         """Title of the analysis."""
         return "AR Analysis"
 
     def describe(self):
@@ -105,15 +106,17 @@
             if reverse:
                 proxy = FrameMapSequence(sequence, list(reversed(range(0, i + 1))))
             else:
                 proxy = FrameMapSequence(sequence, list(range(i, len(sequence))))
 
             trajectory = Trajectory.read(results, name)
 
-            overlaps = calculate_overlaps(trajectory.regions(), proxy.groundtruth(), (proxy.size) if self.burnin else None)
+            masks = proxy.object(self.ignore_masks)
+
+            overlaps = calculate_overlaps(trajectory.regions(), proxy.groundtruth(), (proxy.size) if self.burnin else None, ignore=masks)
 
             grace = self.grace
             progress = len(proxy)
 
             for j, overlap in enumerate(overlaps):
                 if overlap <= self.threshold and not proxy.groundtruth(j).is_empty():
                     grace = grace - 1
@@ -188,14 +191,15 @@
 class MultiStartFragments(SeparableAnalysis):
     """This analysis computes the accuracy-robustness curve for the multistart experiment."""
 
     burnin = Integer(default=10, val_min=0)
     grace = Integer(default=10, val_min=0)
     bounded = Boolean(default=True)
     threshold = Float(default=0.1, val_min=0, val_max=1)
+    ignore_masks = String(default="_ignore", description="Object ID used to get ignore masks.")
 
     @property
     def _title_default(self):
         """Title of the analysis."""
         return "Fragment Analysis"
 
     def describe(self):
@@ -237,15 +241,17 @@
             if reverse:
                 proxy = FrameMapSequence(sequence, list(reversed(range(0, i + 1))))
             else:
                 proxy = FrameMapSequence(sequence, list(range(i, len(sequence))))
 
             trajectory = Trajectory.read(results, name)
 
-            overlaps = calculate_overlaps(trajectory.regions(), proxy.groundtruth(), (proxy.size) if self.burnin else None)
+            masks = proxy.object(self.ignore_masks)
+
+            overlaps = calculate_overlaps(trajectory.regions(), proxy.groundtruth(), (proxy.size) if self.burnin else None, ignore=masks)
 
             grace = self.grace
             progress = len(proxy)
 
             for j, overlap in enumerate(overlaps):
                 if overlap <= self.threshold and not proxy.groundtruth(j).is_empty():
                     grace = grace - 1
@@ -265,14 +271,15 @@
 class EAOCurves(SeparableAnalysis):
     """This analysis computes the expected average overlap curve for the multistart experiment."""
 
     burnin = Integer(default=10, val_min=0)
     grace = Integer(default=10, val_min=0)
     bounded = Boolean(default=True)
     threshold = Float(default=0.1, val_min=0, val_max=1)
+    ignore_masks = String(default="_ignore", description="Object ID used to get ignore masks.")
 
     high = Integer()
 
     @property
     def _title_default(self):
         """Title of the analysis."""
         return "EAO Curve"
@@ -317,15 +324,17 @@
             if reverse:
                 proxy = FrameMapSequence(sequence, list(reversed(range(0, i + 1))))
             else:
                 proxy = FrameMapSequence(sequence, list(range(i, len(sequence))))
 
             trajectory = Trajectory.read(results, name)
 
-            overlaps = calculate_overlaps(trajectory.regions(), proxy.groundtruth(), proxy.size if self.burnin else None)
+            masks = proxy.object(self.ignore_masks)
+
+            overlaps = calculate_overlaps(trajectory.regions(), proxy.groundtruth(), proxy.size if self.burnin else None, ignore=masks)
 
             grace = self.grace
             progress = len(proxy)
 
             for j, overlap in enumerate(overlaps):
                 if overlap <= self.threshold and not proxy.groundtruth(j).is_empty():
                     grace = grace - 1
```

### Comparing `vot-toolkit-0.6.4/vot/analysis/processor.py` & `vot-toolkit-0.7.0/vot/analysis/processor.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/analysis/supervised.py` & `vot-toolkit-0.7.0/vot/analysis/supervised.py`

 * *Files 4% similar despite different names*

```diff
@@ -136,17 +136,20 @@
 
         accuracy = 0
         failures = 0
         for trajectory in trajectories:
             failures += count_failures(trajectory.regions())[0]
             accuracy += compute_accuracy(trajectory.regions(), sequence, self.burnin, self.ignore_unknown, self.bounded)[0]
 
-        ar = (math.exp(- (float(failures) / len(trajectories)) * self.sensitivity), accuracy / len(trajectories))
+        failures /= len(trajectories)
+        accuracy /= len(trajectories)
 
-        return accuracy / len(trajectories), failures / len(trajectories), ar, len(trajectories[0])
+        ar = (math.exp(- (float(failures) / len(sequence)) * self.sensitivity), accuracy)
+
+        return accuracy, failures, ar, len(sequence)
 
 @analysis_registry.register("supervised_average_ar")
 class AverageAccuracyRobustness(SequenceAggregator):
     """Average accuracy-robustness analysis. Computes average accuracy and robustness of a tracker on a given sequence. 
 
     Accuracy is defined as mean overlap of the tracker region with the groundtruth region. The overlap is computed only for frames where the tracker is not in
     initialization or failure state. The overlap is computed only for frames after the burnin period.
@@ -194,17 +197,21 @@
         weight_total = 0
 
         for a, f, _, w in results:
             failures += f * w
             accuracy += a * w
             weight_total += w
 
-        ar = (math.exp(- (failures / weight_total) * self.analysis.sensitivity), accuracy / weight_total)
+        failures /= weight_total
+        accuracy /= weight_total
+        length = weight_total / len(results)
+
+        ar = (math.exp(- (failures / length) * self.analysis.sensitivity), accuracy)
 
-        return accuracy / weight_total, failures / weight_total, ar, weight_total
+        return accuracy, failures, ar, length
 
 @analysis_registry.register("supervised_eao_curve")
 class EAOCurve(TrackerSeparableAnalysis):
     """Expected Average Overlap curve analysis. Computes expected average overlap of a tracker on a given sequence.
     The overlap is computed only for frames where the tracker is not in initialization or failure state.
     The overlap is computed only for frames after the burnin period.
     The analysis is computed as an average of accuracy and robustness over all sequences.
```

### Comparing `vot-toolkit-0.6.4/vot/dataset/__init__.py` & `vot-toolkit-0.7.0/vot/dataset/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,31 +4,30 @@
 import logging
 
 from numbers import Number
 from collections import namedtuple
 from abc import abstractmethod, ABC
 from typing import List, Mapping, Optional, Set, Tuple, Iterator
 
-from class_registry import ClassRegistry
-
 from PIL.Image import Image
 import numpy as np
 
 from cachetools import cached, LRUCache
 
 from vot.region import Region
 from vot import ToolkitException
+from vot.utilities import Registry
 
 import cv2
 
 logger = logging.getLogger("vot")
 
-dataset_downloader = ClassRegistry("vot_downloader")
-sequence_indexer = ClassRegistry("vot_indexer")
-sequence_reader = ClassRegistry("vot_sequence")
+dataset_downloader = Registry("vot_downloader")
+sequence_indexer = Registry("vot_indexer")
+sequence_reader = Registry("vot_sequence")
 
 class DatasetException(ToolkitException):
     """Dataset and sequence related exceptions
     """
     pass
 
 class Channel(ABC):
@@ -280,16 +279,15 @@
         else:
             self._width = width
             self._height = height
             self._depth = depth
 
         self._images.append(image)
 
-    @property
-    def length(self) -> int:
+    def __len__(self) -> int:
         """Returns the length of the sequence channel in number of frames
         
         Returns:
             int: Length of the sequence channel
         """
         return len(self._images)
 
@@ -856,27 +854,32 @@
             return obj
         if obj is None:
             return None
         return obj[index]
 
     def groundtruth(self, index=None):
         """Returns the groundtruth object. If the index is specified, the object is returned as a Region object. If the
-        sequence contains more than one object, an exception is raised.
+        sequence contains more than one object, an exception is raised. If more objects are present, this method 
+        ignores special objects.
         
         Args:
             index (int, optional): Frame index. Defaults to None.
             
         Returns:
             Region: Groundtruth region
         """
-        data = self.__preload()
-        if len(self.objects()) != 1:
-            raise DatasetException("More than one object in sequence")
+        objids = self.objects()
+   
+        if len(objids) != 1:
+            # Filter special objects first
+            objids = [o for o in objids if not o.startswith("_")]
+            if len(objids) != 1:
+                raise DatasetException("More than one object in sequence")
 
-        id = next(iter(data.objects))
+        id = next(iter(objids))
         return self.object(id, index)
 
     def tags(self, index: int = None) -> List[str]:
         """Returns a list of tags in the sequence. If the index is specified, only the tags that are present in the frame 
         with the specified index are returned.
         
         Args:
@@ -947,15 +950,15 @@
         Args:
             name (str): Sequence name
             channels (list): List of channel names
             
         Raises:
             DatasetException: If images are not provided for all channels
         """
-        super().__init__(name, None)
+        super().__init__(name)
         self._channels = {c: InMemoryChannel() for c in channels}
         self._tags = {}
         self._values = {}
         self._groundtruth = []
 
     def append(self, images: dict, region: "Region", tags: list = None, values: dict = None):
         """Appends a new frame to the sequence. The frame is specified by a dictionary of images, a region and optional
@@ -1010,15 +1013,15 @@
     def channels(self) -> List[str]:
         """Returns a list of channel names.
 
         Returns:
             List[str]: List of channel names
 
         """
-        return self._channels.keys()
+        return set(self._channels.keys())
     
     def frame(self, index : int) -> "Frame":
         """Returns the specified frame. The frame is returned as a Frame object.
         
         Args:
             index (int): Frame index
             
@@ -1129,23 +1132,22 @@
     def size(self) -> tuple:
         """Returns the sequence size as a tuple (width, height) 
         
         Returns:
             tuple: Sequence size
         """
         return self.channel().size
-    
-    @property
+
     def channels(self) -> list:
         """Returns a list of channel names 
         
         Returns:
             list: List of channel names
         """
-        return self._channels.keys()
+        return set(self._channels.keys())
 
 def download_bundle(url: str, path: str = "."):
     """Downloads a dataset bundle as a ZIP file and decompresses it.
 
     Args:
         url (str): Source bundle URL
         path (str, optional): Destination directory. Defaults to ".".
@@ -1176,35 +1178,30 @@
         path (str): Destination directory
 
     Raises:
         DatasetException: If the dataset is not found or a network error occured
     """
     from urllib.parse import urlsplit
 
-    try:
-        res = urlsplit(url)
+    res = urlsplit(url)
 
-        if res.scheme in ["http", "https"]:
-            if res.path.endswith(".json"):
-                from .common import download_dataset_meta
-                download_dataset_meta(url, path)
-                return
-            else:
-                download_bundle(url, path)
-                return
-
-        raise DatasetException("Unknown dataset domain: {}".format(res.scheme))
-
-    except ValueError:
-
-        if url in dataset_downloader:
-            dataset_downloader[url](path)
+    if res.scheme in ["http", "https"]:
+        if res.path.endswith(".json"):
+            from .common import download_dataset_meta
+            download_dataset_meta(url, path)
+            return
+        else:
+            download_bundle(url, path)
             return
 
-        raise DatasetException("Illegal dataset identifier: {}".format(url))
+    if url in dataset_downloader:
+        dataset_downloader.get_class(url)(path)
+        return
+
+    raise DatasetException("Illegal dataset identifier: {}".format(url))
 
 
 def load_dataset(path: str) -> Dataset:
     """Loads a dataset from a local directory
 
     Args:
         path (str): The path to the local dataset data
@@ -1214,37 +1211,37 @@
 
     Returns:
         Dataset: Dataset object
     """
 
     from collections import OrderedDict
 
-    names = []
+    sequence_list = None
 
-    if os.path.isfile(path):
-        with open(os.path.join(path), 'r') as fd:
-            names = fd.readlines()
-
-    if os.path.isdir(path):
-        if os.path.isfile(os.path.join(path, "list.txt")):
-            with open(os.path.join(path, "list.txt"), 'r') as fd:
-                names = fd.readlines()
-
-    if len(names) == 0:
-        raise DatasetException("Dataset directory does not contain a list.txt file")
+    for _, indexer in sequence_indexer.items():
+        logger.debug("Attempting to index sequences with {}.{}".format(indexer.__module__, indexer.__name__))
+        sequence_list = indexer(path)
+        if sequence_list is not None:
+            break
+        
+    if sequence_list is None or len(sequence_list) == 0:
+        raise DatasetException("Unable to locate sequences in {}".format(path))
 
     sequences = OrderedDict()
 
     logger.debug("Loading sequences...")
 
-    for name in names:
-        root = os.path.join(path, name.strip())
-        sequences[name.strip()] = load_sequence(root)
+    for sequence_id in sequence_list:
+        sequence_path = sequence_id.strip()
+        if not os.path.isabs(sequence_id):
+            sequence_path = os.path.join(path, sequence_id)
+        sequence = load_sequence(sequence_path)
+        sequences[sequence.name] = sequence
 
-    logger.debug("Found %d sequences in dataset" % len(names))
+    logger.debug("Found %d sequences in dataset" % len(sequence_list))
 
     return Dataset(sequences)
 
 def load_sequence(path: str) -> Sequence:
     """Loads a sequence from a given path (directory), tries to guess the format of the sequence.
 
     Args:
@@ -1254,17 +1251,17 @@
         DatasetException: If an loading error occures, unsupported format or other issues.
 
     Returns:
         Sequence: Sequence object
     """
 
     for _, loader in sequence_reader.items():
-        logger.debug("Trying to load sequence with {}.{}".format(loader.__module__, loader.__name__))
         sequence = loader(path)
         if sequence is not None:
+            logger.debug("Loaded sequence with {}.{}".format(loader.__module__, loader.__name__))
             return sequence
 
     raise DatasetException("Unable to load sequence, unknown format or unsupported sequence: {}".format(path))
 
 import importlib
 for module in [".common", ".otb", ".got10k", ".trackingnet"]:
     importlib.import_module(module, package="vot.dataset")
```

### Comparing `vot-toolkit-0.6.4/vot/dataset/common.py` & `vot-toolkit-0.7.0/vot/dataset/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import glob
 import logging
 
 import six
 
 import cv2
 
-from vot.dataset import Dataset, DatasetException, Sequence, BasedSequence, PatternFileListChannel, SequenceData
+from vot.dataset import DatasetException, Sequence, BasedSequence, PatternFileListChannel, SequenceData
 from vot.region.io import write_trajectory, read_trajectory
 from vot.region import Special
 from vot.utilities import Progress, localize_path, read_properties, write_properties
 
 logger = logging.getLogger("vot")
 
 def convert_int(value: str) -> int:
@@ -151,15 +151,15 @@
     metadata["length"] = convert_int(metadata.get("length", None))
     metadata["fps"] = convert_int(metadata.get("fps", None))
 
     metadata["root"] = path
 
     return metadata
 
-from vot.dataset import sequence_reader
+from vot.dataset import sequence_reader, sequence_indexer
 
 @sequence_reader.register("default")
 def read_sequence(path):
     """Reads a sequence from the given path.
 
     Args:
         path (str): The path to read the sequence from.
@@ -182,18 +182,44 @@
         Sequence: The sequence read from the given path.
     """
     if not os.path.isfile(os.path.join(path, "groundtruth.txt")):
         return None
 
     metadata = dict(fps=30, format="default")
     metadata["channel.default"] = "color"
-    metadata["channel.color"] = "%08d.jpg"
+    metadata["channels.color"] = "%08d.jpg"
+    metadata["root"] = path
+    metadata["length"] = None
 
     return BasedSequence(os.path.basename(path), _read_data, metadata=metadata)
 
+@sequence_indexer.register("default")
+def index_sequences(path: str) -> None:
+    """Indexes the sequences in the given path. Only works if there is a list.txt file in the given path or the path is a list file.
+    
+    Args:
+        path (str): The path to index sequences in.
+    """
+    names = None
+
+    if os.path.isfile(path):
+        with open(os.path.join(path), 'r') as fd:
+            names = fd.readlines()
+
+    if os.path.isdir(path):
+        if os.path.isfile(os.path.join(path, "list.txt")):
+            with open(os.path.join(path, "list.txt"), 'r') as fd:
+                names = fd.readlines()
+
+    if names is None:
+        return None
+
+    names = [name.strip() for name in names]
+    return names
+
 def download_dataset_meta(url: str, path: str) -> None:
     """Downloads the metadata of a dataset from a given URL and stores it in the given path.
     
     Args:
         url (str): The URL to download the metadata from.
         path (str): The path to store the metadata in.
         
@@ -315,9 +341,15 @@
             fp.write(data)
 
     for value in sequence.values():
         data = "\n".join([ str(sequence.values(i).get(value, "")) for i in range(len(sequence))])
         with open(os.path.join(directory, "%s.value" % value), "w") as fp:
             fp.write(data)
 
-    write_trajectory(os.path.join(directory, "groundtruth.txt"), [f.groundtruth() for f in sequence])
+    # Write groundtruth in case of single object
+    if len(sequence.objects()) == 1:
+        write_trajectory(os.path.join(directory, "groundtruth.txt"), [f.groundtruth() for f in sequence])
+    else:
+        for id in sequence.objects():
+            write_trajectory(os.path.join(directory, "groundtruth_%s.txt" % id), [f.object(id) for f in sequence])
+
     write_properties(os.path.join(directory, "sequence"), metadata)
```

### Comparing `vot-toolkit-0.6.4/vot/dataset/cow.png` & `vot-toolkit-0.7.0/vot/dataset/cow.png`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/dataset/dummy.py` & `vot-toolkit-0.7.0/vot/dataset/dummy.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/dataset/got10k.py` & `vot-toolkit-0.7.0/vot/dataset/got10k.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/dataset/otb.py` & `vot-toolkit-0.7.0/vot/dataset/otb.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from vot import get_logger
 from vot.dataset import BasedSequence, DatasetException, PatternFileListChannel, SequenceData
 from vot.utilities import Progress
 from vot.region.io import parse_region
 
 logger = get_logger()
 
-_BASE_URL = "http://cvlab.hanyang.ac.kr/tracker_benchmark/seq/"
+_BASE_URL = "https://web.archive.org/web/20221118171918/http://cvlab.hanyang.ac.kr/tracker_benchmark/   seq/"
 
 _OTB50_SUBSET = ["Basketball", "Biker", "Bird1", "BlurBody", "BlurCar2", "BlurFace", "BlurOwl", "Bolt", "Box",
     "Car1", "Car4", "CarDark", "CarScale", "ClifBar", "Couple", "Crowds", "David", "Deer", "Diving",
     "DragonBaby", "Dudek", "Football", "Freeman4", "Girl", "Human3", "Human4", "Human6", "Human9",
     "Ironman", "Jump", "Jumping", "Liquor", "Matrix", "MotorRolling", "Panda", "RedTeam", "Shaking",
     "Singer2", "Skating1", "Skating2_1", "Skating2_2", "Skiing", "Soccer", "Surfer", "Sylvester", "Tiger2",
     "Trellis", "Walking", "Walking2", "Woman"]
```

### Comparing `vot-toolkit-0.6.4/vot/dataset/proxy.py` & `vot-toolkit-0.7.0/vot/dataset/proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     def __len__(self):
         """Returns the length of the sequence. Forwards the request to the source sequence.
         
         Returns:
             int: Length of the sequence.
         """
-        return len(self)
+        return len(self._source)
 
     def frame(self, index: int) -> Frame:
         """Returns a frame object for the given index. Forwards the request to the source sequence.
         
         Args:
             index (int): Index of the frame.
             
@@ -126,15 +126,15 @@
         Returns:
             Tuple[int, int]: Size of the sequence.
         """
         return self._source.size
 
 
 class FrameMapChannel(Channel):
-    """A proxy channel that maps frames from a source channel in another order."""
+    """A proxy channel that maps frames to a different order."""
 
     def __init__(self, source: Channel, frame_map: List[int]):
         """Creates a frame mapping proxy channel.
         
         Args:
             source (Channel): Source channel object
             frame_map (List[int]): A list of frame indices in the source channel that will form the proxy. The list is filtered
@@ -380,8 +380,54 @@
 
     def groundtruth(self, index: int = None) -> List[Region]:
         """Returns the groundtruth for the given index.
         
         Args:
             index (int): Index of the frame.
         """
-        return self._source.object(self._id, index)
+        return self._source.object(self._id, index)
+    
+class ObjectsHideFilterSequence(ProxySequence):
+    """A proxy sequence that virtually removes specified objects from the sequence. Note that the object is not removed from the sequence, but only hidden when listing them.
+    """
+
+    def __init__(self, source: Sequence, ids: Set[str]):
+        """Creates an object hide filter proxy sequence.
+    
+        Args:
+            source (Sequence): Source sequence object
+            ids (Set[str]): IDs of the objects that will be hidden in the proxy sequence.
+        """
+        super().__init__(source)
+        self._ids = ids
+    
+    def objects(self):
+        """Returns a dictionary of all objects in the sequence.
+        
+        Returns:
+            Dict[str, Object]: Dictionary of all objects in the sequence.
+        """
+        objects = self._source.objects()
+        return {id for id in objects if id not in self._ids}
+
+def IgnoreSpecialObjects(sequence: Sequence) -> Sequence:
+    """Creates a proxy sequence that ignores special objects.Special objects are denoted by a 
+        leading underscore in the object name. Usually, those objects are used for storing additional
+        information about the sequence.
+    
+    Args:
+        sequence (Sequence): Source sequence object.
+        
+    Returns:
+        Sequence: Proxy sequence object.
+    """
+
+    def is_special(id: str):
+        """Checks if the object id is special (starts with underscore)."""
+        return id.startswith("_")
+    
+    ids = [id for id in sequence.objects() if is_special(id)]
+
+    if len(ids) == 0:
+        return sequence
+
+    return ObjectsHideFilterSequence(sequence, ids)
```

### Comparing `vot-toolkit-0.6.4/vot/dataset/trackingnet.py` & `vot-toolkit-0.7.0/vot/dataset/trackingnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """ Dataset adapter for the TrackingNet dataset. Note that the dataset is organized a different way than the VOT datasets,
 annotated frames are stored in a separate directory. The dataset also contains train and test splits. The loader 
 assumes that only one of the splits is used at a time and that the path is given to this part of the dataset. """
 
 import os
 import glob
 import logging
-from collections import OrderedDict
 
 import six
 
-from vot.dataset import Dataset, DatasetException, \
-    BasedSequence, PatternFileListChannel, SequenceData, \
+from vot.dataset import BasedSequence, PatternFileListChannel, SequenceData, \
     Sequence
+from vot import get_logger
 from vot.region import Special
 from vot.region.io import read_trajectory
-from vot.utilities import Progress
 
-logger = logging.getLogger("vot")
+logger = get_logger()
 
 def load_channel(source):
     """ Load channel from the given source.
     
     Args:
         source (str): Path to the source. If the source is a directory, it is
             assumed to be a pattern file list. If the source is a file, it is
```

### Comparing `vot-toolkit-0.6.4/vot/document/__init__.py` & `vot-toolkit-0.7.0/vot/report/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 """ This module contains classes for generating reports and visualizations. """
 
 import typing
-from abc import ABC, abstractmethod
 import json
 import inspect
 import threading
 import datetime
 import collections
 import collections.abc
 import sys
-from asyncio import wait
+from asyncio import wait, ensure_future
 from asyncio.futures import wrap_future
 
 import numpy as np
 import yaml
 
 from matplotlib.cm import get_cmap
 from matplotlib.figure import Figure
 from matplotlib.axes import Axes as PlotAxes
 import matplotlib.colors as colors
 
 from attributee import Attributee, Object, Nested, String, Callable, Integer, List
 
 from vot import __version__ as version
 from vot import get_logger
-from vot.dataset import Sequence
+from vot.dataset import Sequence, FrameList
 from vot.tracker import Tracker
 from vot.analysis import Axes
 from vot.utilities import class_fullname
 from vot.utilities.data import Grid
+from vot.utilities import ClassRegistry, ObjectResolver
+
+report_registry = ClassRegistry("vot_reports")
+
+Table = collections.namedtuple("Table", ["header", "data", "order"])
 
 class Plot(object):
     """ Base class for all plots. """
 
     def __init__(self, identifier: str, xlabel: str, ylabel: str,
         xlimits: typing.Tuple[float, float], ylimits: typing.Tuple[float, float], trait = None):
         """ Initializes the plot.
@@ -71,34 +75,109 @@
         raise NotImplementedError
     
     @property
     def axes(self) -> Axes:
         """ Returns the axes of the plot."""
         return self._axes
 
-    def save(self, output, fmt):
-        """ Saves the plot to a file."""
+    def save(self, output: str, fmt: str):
+        """ Saves the plot to a file.
+        
+        Args:
+            output (str): The output file.
+            fmt (str): The format of the output file.
+        """
         self._figure.savefig(output, format=fmt, bbox_inches='tight', transparent=True)
 
     @property
     def identifier(self):
         """ Returns the identifier of the plot."""
         return self._identifier
 
+class Video(object):
+    """ Base class for all videos. """
+
+    def __init__(self, identifier: str, frames: FrameList, fps: int = 30, trait = None):
+        """ Initializes the video object.
+        
+        Args:
+            identifier (str): The identifier of the video.
+            frames (FrameList): The frames of the video.
+            fps (int): The frames per second of the video.
+            trait (str): The trait of the video.    
+        """
+
+        self._identifier = identifier
+        self._frames = frames
+        self._fps = fps
+        self._manager = StyleManager.default()
+
+    def __call__(self, frame: int, key, data):
+        """ Draws the data on the frame."""
+        self.draw(frame, key, data)
+
+    def draw(self, frame: int, key, data):
+        """ Draws the data on the plot."""
+        raise NotImplementedError
+
+    def render(self, frame: int):
+        """ Renders the frame and returns it as a NumPy array."""
+        raise NotImplementedError
+
+    def save(self, output: str, fmt: str):
+        import tempfile
+        import shutil
+        import os
+        from .video import VideoWriterScikitH264, VideoWriterOpenCV
+
+        supported_mappings = {
+            "mp4": VideoWriterScikitH264,
+            "avi": VideoWriterOpenCV
+        }
+
+        if not fmt in supported_mappings:
+            raise ValueError("Unsupported video format: {}".format(fmt))
+
+        if not isinstance(output, str):
+            fd, tempname = tempfile.mkstemp(prefix="video_", suffix=".{}".format(fmt))
+            os.close(fd)
+        else: 
+            tempname = output
+
+        writer = supported_mappings[fmt](tempname, self._fps)
+
+        for i in range(0, len(self._frames)):
+            writer(self.render(i))
+
+        writer.close()
+
+        if tempname == output:
+            return
+        
+        shutil.copyfileobj(open(tempname, 'rb'), output)
+        os.remove(tempname)
+
+    def __len__(self):
+        return len(self._frames)
+
+    @property
+    def identifier(self):
+        """ Returns the identifier of the plot."""
+        return self._identifier
+
 class ScatterPlot(Plot):
     """ A scatter plot."""
 
     def draw(self, key, data):
         """ Draws the data on the plot. """
         if data is None or len(data) != 2:
             return
 
         style = self._manager.plot_style(key)
-        handle = self._axes.scatter(data[0], data[1], **style.point_style())
-        #handle.set_gid("report_%s_%d" % (self._identifier, style["number"]))
+        self._axes.scatter(data[0], data[1], **style.point_style())
 
 class LinePlot(Plot):
     """ A line plot."""
 
     def draw(self, key, data):
         """ Draws the data on the plot."""
         if data is None or len(data) < 1:
@@ -111,16 +190,51 @@
             x, y = zip(*data)
         else:
             y = data
             x = range(len(data))
 
         style = self._manager.plot_style(key)
 
-        handle = self._axes.plot(x, y, **style.line_style())
-       # handle[0].set_gid("report_%s_%d" % (self._identifier, style["number"]))
+        self._axes.plot(x, y, **style.line_style())
+
+class ObjectVideo(Video):
+
+    def __init__(self, identifier: str, frames: FrameList, fps=10, trait=None):
+        super().__init__(identifier, frames, fps=fps, trait=trait)
+        self._regions = {}
+
+    def draw(self, frame, key, data):
+        """Draws the data on the frame."""
+        from vot.region import Region
+        assert isinstance(data, Region)
+
+        if not key in self._regions:
+            self._regions[key] = [None] * len(self)
+
+        self._regions[key][frame] = data
+
+    def render(self, frame: int):
+        """Renders the frame and returns it as an array."""
+        from vot.utilities.draw import ImageDrawHandle
+
+        assert frame >= 0 and frame < len(self)
+
+        handle = ImageDrawHandle(self._frames.frame(frame).image())
+
+        for key, regions in self._regions.items():
+            if regions[frame] is None:
+                continue
+
+            style = self._manager.plot_style(key)
+
+            handle.style(**style.region_style())
+            regions[frame].draw(handle)
+
+        return handle.array
+
 
 class ResultsJSONEncoder(json.JSONEncoder):
     """ JSON encoder for results. """
 
     def default(self, o):
         """ Default encoder. """
         if isinstance(o, Grid):
@@ -154,15 +268,15 @@
 ResultsYAMLEncoder.add_representer(collections.OrderedDict, ResultsYAMLEncoder.represent_dict)
 ResultsYAMLEncoder.add_representer(tuple, ResultsYAMLEncoder.represent_tuple)
 ResultsYAMLEncoder.add_representer(Grid, ResultsYAMLEncoder.represent_object)
 ResultsYAMLEncoder.add_representer(np.ndarray, ResultsYAMLEncoder.represent_object)
 ResultsYAMLEncoder.add_multi_representer(np.integer, ResultsYAMLEncoder.represent_int)
 ResultsYAMLEncoder.add_multi_representer(np.inexact, ResultsYAMLEncoder.represent_float)
 
-def generate_serialized(trackers: typing.List[Tracker], sequences: typing.List[Sequence], results, storage: "Storage", serializer: str):
+def generate_serialized(trackers: typing.List[Tracker], sequences: typing.List[Sequence], results, storage: "Storage", serializer: str, name: str):
     """ Generates a serialized report of the results.  """
 
     doc = dict()
     doc["toolkit"] = version
     doc["timestamp"] = datetime.datetime.now().isoformat()
     doc["trackers"] = {t.reference : t.describe() for t in trackers}
     doc["sequences"] = {s.name : s.describe() for s in sequences}
@@ -173,18 +287,18 @@
         exp = dict(parameters=experiment.dump(), type=class_fullname(experiment))
         exp["results"] = []
         for _, data in analyses.items():
             exp["results"].append(data)
         doc["results"][experiment.identifier] = exp
 
     if serializer == "json":
-        with storage.write("results.json") as handle:
+        with storage.write(name + "." + serializer) as handle:
             json.dump(doc, handle, indent=2, cls=ResultsJSONEncoder)
     elif serializer == "yaml":
-        with storage.write("results.yaml") as handle:
+        with storage.write(name + "." + serializer) as handle:
             yaml.dump(doc, handle, Dumper=ResultsYAMLEncoder)
     else:
         raise RuntimeError("Unknown serializer")
 
 def configure_axes(figure, rect=None, _=None):
     """ Configures the axes of the plot. """
 
@@ -214,18 +328,22 @@
         """ Returns the style for a line."""
         raise NotImplementedError
 
     def point_style(self):
         """ Returns the style for a point."""
         raise NotImplementedError
 
+    def region_style(self):
+        """ Returns the style for a region, used with DrawHandle."""
+        raise NotImplementedError
+
 class DefaultStyle(PlotStyle):
     """ The default style for a plot."""
 
-    colormap = get_cmap("tab20b")
+    colormap = get_cmap("Set1", 9)
     colorcount = 20
     markers = ["o", "v", "<", ">", "^", "8", "*"]
 
     def __init__(self, number):
         """ Initializes the style. 
         
         Args:
@@ -236,30 +354,35 @@
 
     def line_style(self, opacity=1):
         """ Returns the style for a line.
         
         Args:
             opacity (float): The opacity of the line.
         """
-        color = DefaultStyle.colormap((self._number % DefaultStyle.colorcount + 1) / DefaultStyle.colorcount)
+        color = self.colormap((self._number % self.colormap.N))
         if opacity < 1:
             color = colors.to_rgba(color, opacity)
         return dict(linewidth=1, c=color)
 
     def point_style(self):
         """ Returns the style for a point.
         
         Args:
             color (str): The color of the point.
             opacity (float): The opacity of the line.
         """
-        color = DefaultStyle.colormap((self._number % DefaultStyle.colorcount + 1) / DefaultStyle.colorcount)
+        color = self.colormap((self._number % self.colormap.N))
         marker = DefaultStyle.markers[self._number % len(DefaultStyle.markers)]
         return dict(marker=marker, c=[color])
 
+    def region_style(self):
+        """ Returns the style for a region, used with DrawHandle."""
+        color = self.colormap((self._number % self.colormap.N))
+        return dict(color=color, fill=True)
+
 class Legend(object):
     """ A legend for a plot."""
 
     def __init__(self, style_factory=DefaultStyle):
         """ Initializes the legend.
         
         Args:
@@ -316,38 +439,38 @@
         self._legends = dict()
 
     def __getitem__(self, key) -> PlotStyle:
         """ Gets the style for the given key."""
         return self.plot_style(key)
 
     def legend(self, key) -> Legend:
-        """ Gets the legend for the given key."""
+        """ Gets the legend for a given key."""
         if inspect.isclass(key):
             klass = key
         else:
             klass = type(key)
 
         if not klass in self._legends:
             self._legends[klass] = Legend(self.plots)
 
         return self._legends[klass]
 
     def plot_style(self, key) -> PlotStyle:
-        """ Gets the plot style for the given key."""
+        """ Gets the plot style for a given key."""
         return self.legend(key)[key]
 
     def make_axes(self, figure, rect=None, trait=None) -> Axes:
-        """ Makes the axes for the given figure."""
+        """ Makes the axes for a given figure."""
         return self.axes(figure, rect, trait)
 
     def make_figure(self, trait=None) -> typing.Tuple[Figure, Axes]:
-        """ Makes the figure for the given trait.
+        """ Makes the figure for a given trait.
         
         Args:
-            trait: The trait for which to make the figure.
+            trait (str): The trait for which to make the figure.
 
         Returns:
             A tuple containing the figure and the axes.
         """
         figure = self.figure(trait)
         axes = self.make_axes(figure, trait=trait)
 
@@ -374,34 +497,34 @@
 
     @staticmethod
     def default() -> "StyleManager":
         """ Gets the default style manager."""
 
         manager = getattr(StyleManager._context, 'style_manager', None)
         if manager is None:
-            get_logger().info("Creating new style manager")
+            get_logger().info("Creating new style manager", stack_info=True)
             manager = StyleManager()
             StyleManager._context.style_manager = manager
 
         return manager
 
 class TrackerSorter(Attributee):
     """ A sorter for trackers. """
 
     experiment = String(default=None)
     analysis = String(default=None)
     result = Integer(val_min=0, default=0)
 
-    def __call__(self, experiments, trackers, sequences):
+    def __call__(self, experiments: typing.List["Experiment"], trackers: typing.List["Tracker"], sequences: typing.List["Sequence"]):
         """ Sorts the trackers. 
         
         Arguments:
-            experiments (list of Experiment): The experiments.
-            trackers (list of Tracker): The trackers.
-            sequences (list of Sequence): The sequences.
+            experiments (typing.List[Experiment]): The experiments.
+            trackers (typing.List[Tracker]): The trackers.
+            sequences (typing.List[Sequence]): The sequences.
             
         Returns:
             A list of indices of the trackers in the sorted order.
         """
         from vot.analysis import AnalysisError
 
         if self.experiment is None or self.analysis is None:
@@ -425,72 +548,220 @@
             raise RuntimeError("Unable to sort trackers", e)
 
         scores = [x[self.result] for x in result]
         indices = [i[0] for i in sorted(enumerate(scores), reverse=True, key=lambda x: x[1])]
 
         return indices
 
-class Generator(Attributee):
-    """ A generator for reports."""
+class Report(Attributee):
+    """ A report generator for various reports. Base class for all report generators. """
 
     async def generate(self, experiments, trackers, sequences):
-        raise NotImplementedError
+        raise NotImplementedError()
 
     async def process(self, analyses, experiment, trackers, sequences):
+
+        sequences = experiment.transform(sequences)
+
         if sys.version_info >= (3, 3):
             _Iterable = collections.abc.Iterable
         else:
             _Iterable = collections.Iterable
         if not isinstance(analyses, _Iterable):
             analyses = [analyses]
 
         futures = []
 
         for analysis in analyses:
             futures.append(wrap_future(analysis.commit(experiment, trackers, sequences)))
 
         await wait(futures)
 
-        if len(futures) == 1:
-            return futures[0].result()
-        else:
-            return (future.result() for future in futures)
+        return (future.result() for future in futures)
+
+class SeparableReport(Report):
+    """ A report generator that is separable across experiments. Base class for all separable report generators. """
+
+    async def perexperiment(self, experiment, trackers, sequences):
+        raise NotImplementedError()
+
+    def compatible(self, experiment):
+        raise NotImplementedError()
+
+    async def generate(self, experiments, trackers, sequences):
+
+        futures = []
+        texperiments = []
+
+        for experiment in experiments:
+
+            tsequences = experiment.transform(sequences)
+
+            if self.compatible(experiment):
+                futures.append(ensure_future(self.perexperiment(experiment, trackers, tsequences)))
+                texperiments.append(experiment)
+            else:
+                continue
+
+        await wait(futures)
+
+        items = dict()
+
+        for experiment, future in zip(texperiments, futures):
+            items[experiment.identifier] = future.result()
+
+        return items
+
+
 
 class ReportConfiguration(Attributee):
     """ A configuration for reports."""
 
     style = Nested(StyleManager)
     sort = Nested(TrackerSorter)
-    generators = List(Object(subclass=Generator), default=[])
+    index = List(Object(ObjectResolver(report_registry), subclass=Report), default=[], description="The reports to include.")
+
+def generate_document(workspace: "Workspace", trackers: typing.List[Tracker], format: str, name: str, select_sequences: typing.Optional[str] = None, select_experiments: typing.Optional[str] = None):
+    """Generate a report for a one or multiple trackers on an experiment stack and a set of sequences.
 
-# TODO: replace this with report generator and separate json/yaml dump
-def generate_document(format: str, config: ReportConfiguration, trackers: typing.List[Tracker], sequences: typing.List[Sequence], results, storage: "Storage"):
-    """ Generates a report document.
-    
     Args:
-        format: The format of the report.
-        config: The configuration of the report.
+        workspace (Workspace): The workspace to use for the report.
         trackers: The trackers to include in the report.
-        sequences: The sequences to include in the report.
-        results: The results to include in the report.
-        storage: The storage to use for the report.
-        
+        format: The format of the report.
+        name: The name of the report.
     """
+    from asyncio import ensure_future, get_event_loop, wait
+
+    from vot.analysis import AnalysisProcessor
+    from vot.utilities import Progress
+    from vot.workspace.storage import Cache
+    from vot import config
+    from vot.report.common import StackAnalysesTable, StackAnalysesPlots
+
+    def merge_tree(src, dest):
+
+        for key, value in src.items():
+            if not key in dest:        
+                dest[key] = list()
+            dest[key] += value
+
+    logger = get_logger()
+
+    if config.worker_pool_size == 1:
+
+        if config.debug_mode:
+            import logging
+            from vot.analysis.processor import DebugExecutor
+            logging.getLogger("concurrent.futures").setLevel(logging.DEBUG)
+            executor = DebugExecutor()
+        else:
+            from vot.utilities import ThreadPoolExecutor
+            executor = ThreadPoolExecutor(1)
 
-    from .html import generate_html_document
-    from .latex import generate_latex_document
+    else:
+        from concurrent.futures import ProcessPoolExecutor
+        executor = ProcessPoolExecutor(config.workers)
 
-    if format == "json":
-        generate_serialized(trackers, sequences, results, storage, "json")
-    elif format == "yaml":
-        generate_serialized(trackers, sequences, results, storage, "yaml")
+    if not config.persistent_cache:
+        from cachetools import LRUCache
+        cache = LRUCache(1000)
     else:
-        order = config.sort(results.keys(), trackers, sequences)
+        cache = Cache(workspace.storage.substorage("cache").substorage("analysis"))
 
-        with config.style:
-            if format == "html":
-                generate_html_document(trackers, sequences, results, storage)
-            elif format == "latex":
-                generate_latex_document(trackers, sequences, results, storage, False, order=order)
-            elif format == "pdf":
-                generate_latex_document(trackers, sequences, results, storage, True, order=order)
+    index = workspace.report.index
+    if len(index) == 0:
+        # Default report content
+        index = [StackAnalysesTable(), StackAnalysesPlots()]
+        
+    with workspace.report.style:
 
+        experiments = workspace.stack
+        sequences = workspace.dataset
+        
+        if not select_experiments is None:
+            experiments = [experiment for name, experiment in workspace.stack.experiments.items() if name in select_experiments.split(",")]
+        if not select_sequences is None:
+            sequences = [sequence for sequence in sequences if sequence.name in select_sequences.split(",")]
+
+
+        if len(experiments) == 0:
+            logger.warning("No experiments selected")
+
+        if len(sequences) == 0:
+            logger.warning("No sequences selected")
+
+        try:
+
+            with AnalysisProcessor(executor, cache) as processor:
+                
+                order = workspace.report.sort(experiments, trackers, sequences)
+
+                trackers = [trackers[i] for i in order]
+
+                futures = []
+
+                for report in index:
+                    futures.append(ensure_future(report.generate(experiments, trackers, sequences)))
+
+                loop = get_event_loop()
+
+                progress = Progress("Processing", processor.total)
+
+                def update():
+                    progress.total(processor.total)
+                    progress.absolute(processor.total - processor.pending)
+                    loop.call_later(1, update)
+
+                update()
+
+                if len(futures) > 0:
+                    loop.run_until_complete(wait(futures))
+
+                progress.close()
+
+                reports = dict()
+
+                for future in futures:
+                    merge_tree(future.result(), reports)
+
+        finally:
+
+            executor.shutdown(wait=True)
+
+        report_storage = workspace.storage.substorage("reports").substorage(name)
+
+        def only_plots(reports, storage: "Storage"):
+            """Filter out all non-plot items from the report and save them to storage.
+            
+            Args:
+                reports: The reports to filter.
+            """
+            for key, section in reports.items():
+                for item in section:
+                    if isinstance(item, Plot):
+                        logger.debug("Saving plot %s", item.identifier)
+                        with storage.write(key + "_" + item.identifier + '.pdf', binary=True) as out:
+                            item.save(out, "PDF")
+                        with storage.write(key + "_" + item.identifier + '.png', binary=True) as out:
+                            item.save(out, "PNG")
+                    if isinstance(item, Video):
+                        logger.debug("Saving video %s", item.identifier)
+                        with storage.write(key + "_" + item.identifier + '.avi', binary=True) as out:
+                            item.save(out, "avi")
+
+        metadata = {"Stack": workspace.stack.title}
+
+        # Prune empty sections
+        reports = {key: section for key, section in reports.items() if len(section) > 0}
+
+        if format == "html":
+            from .html import generate_html_document
+            generate_html_document(trackers, workspace.dataset, reports, report_storage, metadata=metadata)
+        elif format == "latex":
+            from .latex import generate_latex_document
+            generate_latex_document(trackers, workspace.dataset, reports, report_storage, metadata=metadata)
+        elif format == "plots":
+            only_plots(reports, report_storage)
+        else:
+            raise ValueError("Unknown report format %s" % format)
+        
+import vot.report.common
```

### Comparing `vot-toolkit-0.6.4/vot/document/jquery.js` & `vot-toolkit-0.7.0/vot/report/jquery.js`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/document/latex.py` & `vot-toolkit-0.7.0/vot/report/latex.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from pylatex import Document, Section, Command, LongTable, MultiColumn, Figure, UnsafeCommand
 from pylatex.utils import NoEscape
 
 from vot import toolkit_version, get_logger
 from vot.tracker import Tracker
 from vot.dataset import Sequence
 from vot.workspace import Storage
-from vot.document.common import format_value, read_resource, merge_repeats, extract_measures_table, extract_plots
-from vot.document import StyleManager
+from vot.report.common import format_value, read_resource, merge_repeats
+from vot.report import StyleManager, Plot, Table
 
 TRACKER_GROUP = "default"
 
 class Chunk(Container):
     """A container that does not add a newline after the content."""
 
     def dumps(self):
@@ -50,123 +50,113 @@
     container.append(Command("makeatletter"))
     for tracker in trackers:
         container.append(UnsafeCommand('DefineTracker', [tracker.reference, TRACKER_GROUP],
              extra_arguments=insert_mplfigure(legend.figure(tracker), False) + r' \replunderscores{%s}' % tracker.label))
 
     container.append(Command("makeatother"))
 
-
-def generate_latex_document(trackers: List[Tracker], sequences: List[Sequence], results, storage: Storage, build=False, multipart=True, order=None) -> str:
+def generate_latex_document(trackers: List[Tracker], sequences: List[Sequence], reports, storage: Storage, multipart=True, metadata: dict = None) -> str:
     """Generates a LaTeX document with the results. The document is returned as a string. If build is True, the document is compiled and the PDF is returned.
     
     Args:
         
         trackers (list): List of trackers.
         sequences (list): List of sequences.
-        results (dict): Dictionary of results.
+        reports (list): List of results tuples.
         storage (Storage): Storage object.
-        build (bool): If True, the document is compiled and the PDF is returned.
         multipart (bool): If True, the document is split into multiple files.
-        order (list): List of tracker indices to use for ordering.
+        metadata (dict): Metadata dictionary.
     """
 
     order_marks = {1: "first", 2: "second", 3: "third"}
 
     def format_cell(value, order):
         """Formats a cell in the data table."""
         cell = format_value(value)
         if order in order_marks:
             cell = Command(order_marks[order], cell)
         return cell
 
     logger = get_logger()
 
-    table_header, table_data, table_order = extract_measures_table(trackers, results)
-
-    if order is not None:
-        ordered_trackers = [trackers[i] for i in order]
-    else:
-        ordered_trackers = trackers
-
     doc = Document(page_numbers=True)
 
     doc.preamble.append(Package('pgf'))
     doc.preamble.append(Package('xcolor'))
     doc.preamble.append(Package('fullpage'))
 
     doc.preamble.append(NoEscape(read_resource("commands.tex")))
 
     doc.preamble.append(UnsafeCommand('newcommand', r'\first', options=1, extra_arguments=r'{\color{red} #1 }'))
     doc.preamble.append(UnsafeCommand('newcommand', r'\second', options=1, extra_arguments=r'{\color{green} #1 }'))
     doc.preamble.append(UnsafeCommand('newcommand', r'\third', options=1, extra_arguments=r'{\color{blue} #1 }'))
 
+    # TODO: make table more general (now it assumes a tracker per row)
+    def make_table(doc, table):
+
+        if len(table.header[2]) == 0:
+            logger.debug("No measures found, skipping table")
+        else:
+
+            # Generate data table
+            with doc.create(LongTable("l " * (len(table.header[2]) + 1))) as data_table:
+                data_table.add_hline()
+                data_table.add_row([" "] + [MultiColumn(c[1], data=c[0].identifier) for c in merge_repeats(table.header[0])])
+                data_table.add_hline()
+                data_table.add_row([" "] + [MultiColumn(c[1], data=c[0].title) for c in merge_repeats(table.header[1])])
+                data_table.add_hline()
+                data_table.add_row(["Tracker"] + [" " + c.abbreviation + " " for c in table.header[2]])
+                data_table.add_hline()
+                data_table.end_table_header()
+                data_table.add_hline()
+
+                for tracker, data in table.data.items():
+                    data_table.add_row([UnsafeCommand("Tracker", [tracker.reference, TRACKER_GROUP])] +
+                        [format_cell(x, order[tracker] if not order is None else None) for x, order in zip(data, table.order)])
+
     if multipart:
         container = Chunk()
-        generate_symbols(container, ordered_trackers)
+        generate_symbols(container, trackers)
         with storage.write("symbols.tex") as out:
             container.dump(out)
         doc.preamble.append(Command("input", "symbols.tex"))
     else:
-        generate_symbols(doc.preamble, ordered_trackers)
+        generate_symbols(doc.preamble, trackers)
 
-    doc.preamble.append(Command('title', 'VOT report'))
+    doc.preamble.append(Command('title', 'VOT toolkit report'))
     doc.preamble.append(Command('author', 'Toolkit version ' + toolkit_version()))
     doc.preamble.append(Command('date', datetime.datetime.now().isoformat()))
     doc.append(NoEscape(r'\maketitle'))
 
+    for key, section in reports.items():
 
-    if len(table_header[2]) == 0:
-        logger.debug("No measures found, skipping table")
-    else:
-
-        # Generate data table
-        with doc.create(LongTable("l " * (len(table_header[2]) + 1))) as data_table:
-            data_table.add_hline()
-            data_table.add_row([" "] + [MultiColumn(c[1], data=c[0].identifier) for c in merge_repeats(table_header[0])])
-            data_table.add_hline()
-            data_table.add_row([" "] + [MultiColumn(c[1], data=c[0].title) for c in merge_repeats(table_header[1])])
-            data_table.add_hline()
-            data_table.add_row(["Tracker"] + [" " + c.abbreviation + " " for c in table_header[2]])
-            data_table.add_hline()
-            data_table.end_table_header()
-            data_table.add_hline()
-
-            for tracker in ordered_trackers:
-                data = table_data[tracker]
-                data_table.add_row([UnsafeCommand("Tracker", [tracker.reference, TRACKER_GROUP])] +
-                    [format_cell(x, order[tracker] if not order is None else None) for x, order in zip(data, table_order)])
-
-    if order is not None:
-        z_order = [0] * len(order)
-        for i, j in enumerate(order):
-            z_order[max(order) - i] = j
-    else:
-        z_order = list(range(len(trackers)))
+        doc.append(Section(key))
 
-    plots = extract_plots(trackers, results, z_order)
-
-    for experiment, experiment_plots in plots.items():
-        if len(experiment_plots) == 0:
-            continue
-
-        doc.append(Section("Experiment " + experiment.identifier))
-
-        for title, plot in experiment_plots:
-
-            with doc.create(Figure(position='htbp')) as container:
-                if multipart:
-                    plot_name = plot.identifier + ".pdf"
-                    with storage.write(plot_name, binary=True) as out:
-                        plot.save(out, "PDF")
-                    container.add_image(plot_name)
-                else:
-                    container.append(insert_figure(plot))
-                container.add_caption(title)
-                
-    if build:
-        temp = tempfile.mktemp()
-        logger.debug("Generating to temporary output %s", temp)
-        doc.generate_pdf(temp, clean_tex=True)
-        storage.copy(temp + ".pdf", "report.pdf")
-    else:
-        with storage.write("report.tex") as out:
-            doc.dump(out)
+        for item in section:
+            if isinstance(item, Table):
+                make_table(doc, item)
+            elif isinstance(item, Plot):
+                plot = item
+                with doc.create(Figure(position='htbp')) as container:
+                    if multipart:
+                        plot_name = plot.identifier + ".pdf"
+                        with storage.write(plot_name, binary=True) as out:
+                            plot.save(out, "PDF")
+                        container.add_image(plot_name)
+                    else:
+                        container.append(insert_figure(plot))
+                    container.add_caption(plot.identifier)
+
+                logger.debug("Saving plot %s", item.identifier)
+                item.save(key + "_" + item.identifier + '.pdf', "PDF")
+            else:
+                logger.warning("Unsupported report item type %s", item)
+
+    # TODO: Move to separate function
+    #if build:
+    #    temp = tempfile.mktemp()
+    #    logger.debug("Generating to temporary output %s", temp)
+    #    doc.generate_pdf(temp, clean_tex=True)
+    #    storage.copy(temp + ".pdf", "report.pdf")
+    #else:
+    with storage.write("report.tex") as out:
+        doc.dump(out)
```

### Comparing `vot-toolkit-0.6.4/vot/document/pure.css` & `vot-toolkit-0.7.0/vot/report/pure.css`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/document/report.js` & `vot-toolkit-0.7.0/vot/report/report.js`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/document/table.js` & `vot-toolkit-0.7.0/vot/report/table.js`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/experiment/__init__.py` & `vot-toolkit-0.7.0/vot/experiment/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 import logging
 import typing
 from datetime import datetime
 from abc import abstractmethod
 
 from class_registry import ClassRegistry
 
-from attributee import Attributee, Object, Integer, Float, Nested, List
+from attributee import Attributee, Object, Integer, Float, Nested, List, Boolean
 
 from vot import get_logger
 from vot.tracker import TrackerException
-from vot.utilities import Progress, to_number, import_class
+from vot.utilities import Progress, to_number, import_class, ObjectResolver
+from vot.dataset.proxy import IgnoreSpecialObjects
 
 experiment_registry = ClassRegistry("vot_experiment")
 transformer_registry = ClassRegistry("vot_transformer")
 
 class RealtimeConfig(Attributee):
     """Config proxy for real-time experiment.
     """
@@ -43,15 +44,19 @@
         context (Attributee): Context of the resolver
         
     Returns:
         Transformer: Resolved transformer
     """
     from vot.experiment.transformer import Transformer
 
-    storage = context.parent.storage.substorage("cache").substorage("transformer")
+
+    if context.parent.storage is None:
+        storage = None
+    else:
+        storage = context.parent.storage.substorage("cache").substorage("transformer")
 
     if typename in transformer_registry:
         transformer = transformer_registry.get(typename, cache=storage, **kwargs)
         assert isinstance(transformer, Transformer)
         return transformer
     else:
         transformer_class = import_class(typename)
@@ -93,14 +98,15 @@
     INITIALIZATION = 1
 
     realtime = Nested(RealtimeConfig, default=None, description="Realtime modifier config")
     noise = Nested(NoiseConfig, default=None)
     inject = Nested(InjectConfig, default=None)
     transformers = List(Object(transformer_resolver), default=[])
     analyses = List(Object(analysis_resolver), default=[])
+    ignore_special = Boolean(default=True, description="Ignore special objects in experiment")
 
     def __init__(self, _identifier: str, _storage: "Storage", **kwargs):
         """Initialize an experiment.
         
         Args:
             _identifier (str): Identifier of the experiment
             _storage (Storage): Storage to use for storing results
@@ -113,14 +119,23 @@
         """
         self._identifier = _identifier
         self._storage = _storage
         super().__init__(**kwargs)
         # TODO: validate analysis names
 
     @property
+    def storage(self) -> "Storage":
+        """Storage to use for storing results. Can be None if the experiment is not supposed to store results.
+
+        Returns:
+            Storage: Storage to use for storing results
+        """
+        return self._storage
+
+    @property
     def identifier(self) -> str:
         """Identifier of the experiment.
 
         Returns:
             str: Identifier of the experiment
         """
         return self._identifier
@@ -131,23 +146,14 @@
 
         Returns:
             bool: Whether the experiment is multi-object or not
         """
         # TODO: at some point this may be a property for all experiments
         return False
 
-    @property
-    def storage(self) -> "Storage":
-        """Storage used by the experiment.
-
-        Returns:
-            Storage: Storage used by the experiment
-        """
-        return self._storage
-
     def _get_initialization(self, sequence: "Sequence", index: int, id: str = None):
         """Get initialization for a given sequence, index and object id.
 
         Args:
             sequence (Sequence): Sequence to get initialization for
             index (int): Index of the frame to get initialization for
             id (str): Object id to get initialization for
@@ -232,25 +238,33 @@
             sequence (Sequence): Sequence to get results for
 
         Returns:
             Results: Results for the tracker and sequence
         """
         if tracker.storage is not None:
             return tracker.storage.results(tracker, self, sequence)
+        if not hasattr(self, "_storage"):
+            from vot.workspace import WorkspaceException
+            raise WorkspaceException("Experiment has no storage")
+        
         return self._storage.results(tracker, self, sequence)
 
     def log(self, identifier: str):
         """Get a log file for the experiment.
 
         Args:
             identifier (str): Identifier of the log
 
         Returns:
             str: Path to the log file
         """
+        if not hasattr(self, "_storage"):
+            # Return a devnull file if the experiment has no storage
+            return open(os.devnull, 'w') 
+        
         return self._storage.substorage("logs").write("{}_{:%Y-%m-%dT%H-%M-%S.%f%z}.log".format(identifier, datetime.now()))
 
     def transform(self, sequences):
         """Transform a list of sequences using the experiment transformers.
 
         Args:
             sequences (typing.List[Sequence]): List of sequences to transform
@@ -269,18 +283,21 @@
             get_logger().debug("Adding single object transformer since experiment is not multi-object")
             transformers.insert(0, SingleObject(cache=None))
 
         # Process sequences one transformer at the time. The number of sequences may grow
         for transformer in transformers:
             transformed = []
             for sequence in sequences:
-                get_logger().debug("Transforming sequence {} with transformer {}.{}".format(sequence.identifier, transformer.__module__, transformer.__name__))
+                get_logger().debug("Transforming sequence {} with transformer {}.{}".format(sequence.identifier, transformer.__class__.__module__, transformer.__class__.__name__))
                 transformed.extend(transformer(sequence))
             sequences = transformed
 
+        if self.ignore_special:
+            sequences = [IgnoreSpecialObjects(sequence) for sequence in sequences]
+
         return sequences
 
 from .multirun import UnsupervisedExperiment, SupervisedExperiment
 from .multistart import MultiStartExperiment
 
 def run_experiment(experiment: Experiment, tracker: "Tracker", sequences: typing.List["Sequence"], force: bool = False, persist: bool = False):
     """A helper function that performs a given experiment with a given tracker on a list of sequences.
@@ -340,15 +357,15 @@
     sequences = transformed
 
     progress = EvaluationProgress("{}/{}".format(tracker.identifier, experiment.identifier), len(sequences))
     for sequence in sequences:
         try:
             experiment.execute(tracker, sequence, force=force, callback=progress)
         except TrackerException as te:
-            logger.error("Tracker %s encountered an error: %s", te.tracker.identifier, te)
+            logger.error("Tracker %s encountered an error on sequence %s: %s", te.tracker.identifier, sequence.name, te)
             logger.debug(te, exc_info=True)
             if not te.log is None:
                 with experiment.log(te.tracker.identifier) as flog:
                     flog.write(te.log)
                     logger.error("Tracker output written to file: %s", flog.name)
             if not persist:
                 raise TrackerException("Experiment interrupted", te, tracker=tracker)
```

### Comparing `vot-toolkit-0.6.4/vot/experiment/helpers.py` & `vot-toolkit-0.7.0/vot/experiment/helpers.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/experiment/multirun.py` & `vot-toolkit-0.7.0/vot/experiment/multirun.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/experiment/multistart.py` & `vot-toolkit-0.7.0/vot/experiment/multistart.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/experiment/transformer.py` & `vot-toolkit-0.7.0/vot/experiment/transformer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ Transformer module for experiments."""
 
 import os
 from abc import abstractmethod
-from typing import List
+import typing
 
 from PIL import Image
 
-from attributee import Attributee, Integer, Float, Boolean
+from attributee import Attributee, Integer, Float, Boolean, String, List
 
 from vot.dataset import Sequence, InMemorySequence
 from vot.dataset.proxy import FrameMapSequence
 from vot.dataset.common import write_sequence, read_sequence
 from vot.region import RegionType
 from vot.utilities import arg_hash
 from vot.experiment import transformer_registry
@@ -24,15 +24,15 @@
         Args:
             cache (LocalStorage): The cache to be used for storing generated sequences.
         """
         super().__init__(**kwargs)
         self._cache = cache
 
     @abstractmethod
-    def __call__(self, sequence: Sequence) -> List[Sequence]:
+    def __call__(self, sequence: Sequence) -> typing.List[Sequence]:
         """Generate a list of sequences from the given sequence. The generated sequences are stored in the cache if needed.
 
         Args:
             sequence (Sequence): The sequence to be transformed.
         
         Returns:
             [list]: A list of generated sequences.
@@ -41,15 +41,15 @@
 
 @transformer_registry.register("singleobject")
 class SingleObject(Transformer):
     """Transformer that generates a sequence for each object in the given sequence."""
 
     trim = Boolean(default=False, description="Trim each generated sequence to a visible subsection for the selected object")
 
-    def __call__(self, sequence: Sequence) -> List[Sequence]:
+    def __call__(self, sequence: Sequence) -> typing.List[Sequence]:
         """Generate a list of sequences from the given sequence.
         
         Args:
             sequence (Sequence): The sequence to be transformed.
         """
         from vot.dataset.proxy import ObjectFilterSequence
         
@@ -65,21 +65,23 @@
     This tranformer can only be used with single-object sequences."""
 
     length = Integer(default=100, val_min=1)
     initialization = Integer(default=5, val_min=1)
     padding = Float(default=2, val_min=0)
     scaling = Float(default=1, val_min=0.1, val_max=10)
 
-    def __call__(self, sequence: Sequence) -> List[Sequence]:
+    def __call__(self, sequence: Sequence) -> typing.List[Sequence]:
         """Generate a list of sequences from the given sequence.
         
         Args:
             sequence (Sequence): The sequence to be transformed.
         """
 
+        assert self._cache is not None, "Local cache is required for redetection transformer."
+
         assert len(sequence.objects()) == 1, "Redetection transformer can only be used with single-object sequences."
 
         chache_dir = self._cache.directory(self, arg_hash(sequence.name, **self.dump()))
 
         if not os.path.isfile(os.path.join(chache_dir, "sequence")):
             generated = InMemorySequence(sequence.name, sequence.channels())
             size = (int(sequence.size[0] * self.scaling), int(sequence.size[1] * self.scaling))
@@ -104,9 +106,44 @@
 
             generated.append(initial_images, sequence.frame(0).groundtruth())
             generated.append(redetect_images, sequence.frame(0).groundtruth().move(size[0] - template.width, size[1] - template.height))
 
             write_sequence(chache_dir, generated)
 
         source = read_sequence(chache_dir)
-        mapping = [0] * self.initialization + [1] * (len(self) - self.initialization)
+        mapping = [0] * self.initialization + [1] * (len(source) - self.initialization)
         return [FrameMapSequence(source, mapping)]
+
+@transformer_registry.register("ignore")
+class IgnoreObjects(Transformer):
+    """Transformer that hides objects with certain ids from the sequence."""
+
+    ids = List(String(), default=[], description="List of ids to be ignored")
+
+    def __call__(self, sequence: Sequence) -> typing.List[Sequence]:
+        """Generate a list of sequences from the given sequence.
+        
+        Args:
+            sequence (Sequence): The sequence to be transformed.
+        """
+        from vot.dataset.proxy import ObjectsHideFilterSequence
+        
+        return [ObjectsHideFilterSequence(sequence, self.ids)]
+    
+@transformer_registry.register("downsample")
+class Downsample(Transformer):
+    """Transformer that downsamples the sequence by a given factor."""
+
+    factor = Integer(default=2, val_min=1, description="Downsampling factor")
+    offset = Integer(default=0, val_min=0, description="Offset for the downsampling")
+
+    def __call__(self, sequence: Sequence) -> typing.List[Sequence]:
+        """Generate a list of sequences from the given sequence.
+        
+        Args:
+            sequence (Sequence): The sequence to be transformed.
+        """
+        from vot.dataset.proxy import FrameMapSequence
+        
+        map = [i for i in range(self.offset, len(sequence), self.factor)]
+        
+        return [FrameMapSequence(sequence, map)]
```

### Comparing `vot-toolkit-0.6.4/vot/region/__init__.py` & `vot-toolkit-0.7.0/vot/region/__init__.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/region/io.py` & `vot-toolkit-0.7.0/vot/region/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -135,34 +135,35 @@
         # extract target region from the full mask and calculate RLE
         # do not use full mask to optimize speed and space
         target_mask = mask[tl_y:tl_y+region_h, tl_x:tl_x+region_w]
         rle = mask_to_rle(np.array(target_mask))
 
         return (tl_x, tl_y, region_w, region_h), rle
 
-def parse_region(string: str) -> "Region":
+def parse_region(string: str, separator: str = ",") -> "Region":
     """Parse input string to the appropriate region format and return Region object
 
     Args:
         string (str): comma separated list of values
+        separator (str): separator of values in the input string
 
     Returns:
         Region: resulting region
     """
     from vot import config
     from vot.region import Special
     from vot.region.shapes import Rectangle, Polygon, Mask
 
     if string[0] == 'm':
         # input is a mask - decode it
-        m_, offset_ = create_mask_from_string(string[1:].split(','))
+        m_, offset_ = create_mask_from_string(string[1:].split(separator))
         return Mask(m_, offset=offset_, optimize=config.mask_optimize_read)
     else:
         # input is not a mask - check if special, rectangle or polygon
-        tokens = [float(t) for t in string.split(',')]
+        tokens = [float(t) for t in string.split(separator)]
         if len(tokens) == 1:
             return Special(tokens[0])
         if len(tokens) == 4:
             if any([math.isnan(el) for el in tokens]):
                 return Special(0)
             else:
                 return Rectangle(tokens[0], tokens[1], tokens[2], tokens[3])
@@ -240,19 +241,20 @@
         elif isinstance(r, Polygon): fp.write(struct.pack("<BH%df" % (2 * r.size), 2, r.size, *[item for sublist in r.points() for item in sublist]))
         elif isinstance(r, Mask): 
             rle = mask_to_rle(r.mask, maxstride=255*255)
             fp.write(struct.pack("<BhhHHH%dH" % len(rle), 3, r.offset[0], r.offset[1], r.mask.shape[1], r.mask.shape[0], len(rle), *rle))
         else:
             raise IOError("Wrong region type")
 
-def read_trajectory(fp: Union[str, TextIO]):
+def read_trajectory(fp: Union[str, TextIO], separator: str = ","):
     """Reads a trajectory from a file and returns a list of regions.
     
     Args:
         fp (str or TextIO): File path or file pointer to the trajectory file
+        separator (str): Separator of values in the region, only used for text files
         
     Returns:
         list: List of regions
     """
     if isinstance(fp, str):
         try:
             import struct
@@ -270,15 +272,15 @@
         close = False
 
     if binary:
         regions = read_trajectory_binary(fp)
     else:
         regions = []
         for line in fp.readlines():
-            regions.append(parse_region(line.strip()))
+            regions.append(parse_region(line.strip(), separator))
 
     if close:
         fp.close()
 
     return regions
 
 def write_trajectory(fp: Union[str, TextIO], data: List["Region"]):
```

### Comparing `vot-toolkit-0.6.4/vot/region/raster.py` & `vot-toolkit-0.7.0/vot/region/raster.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 @numba.njit(cache=True)
 def mask_bounds(mask: np.ndarray):
     """ Compute bounds of a binary mask. Bounds are defined as the minimal axis-aligned region containing all positive pixels.
     This is a Numba implementation of the function that is compiled to machine code for faster execution.
 
     Args:
-        mask: 2-D array with a binary mask
+        mask (np.ndarray): 2-D array with a binary mask
 
     Returns:
         coordinates of the top-left and bottom-right corners of the minimal axis-aligned region containing all positive pixels
     """
     ii32 = np.iinfo(np.int32)
     top = ii32.max
     bottom = ii32.min
@@ -275,25 +275,28 @@
     elif t == _TYPE_MASK:
         return copy_mask(a, o, bounds)
     
     return np.zeros((bounds[3] - bounds[1] + 1, bounds[2] - bounds[0] + 1), dtype=np.uint8)
 
 @numba.njit(cache=True)
 def _calculate_overlap(a: np.ndarray, b: np.ndarray, at: int, bt: int, ao: Optional[Tuple[int, int]] = None,
-        bo: Optional[Tuple[int, int]] = None, bounds: Optional[Tuple[int, int]] = None):
+        bo: Optional[Tuple[int, int]] = None, bounds: Optional[Tuple[int, int]] = None, ignore: Optional[np.array] = None, it: Optional[int] = None, io: Optional[Tuple[int, int]] = None):
     """ Calculate the overlap between two regions. This is a Numba implementation of the function that is compiled to machine code for faster execution.
     
     Args:
         a: 2-D array with the mask of the first region
         b: 2-D array with the mask of the second region
         at: type of the first region
         bt: type of the second region
         ao: 2-tuple with the offset of the first mask
         bo: 2-tuple with the offset of the second mask
         bounds: 2-tuple with the bounds of the image (left, top, right, bottom)
+        ignore: 2-D array with the mask of the region to ignore
+        it: type of the region to ignore
+        io: 2-tuple with the offset of the mask to ignore
     
     Returns:
         float with the overlap between the two regions. Note that overlap is one by definition if both regions are empty.
     """
 
     bounds1 = _region_bounds(a, at, ao)
     bounds2 = _region_bounds(b, bt, bo)
@@ -318,86 +321,96 @@
 
     a1 = m1.ravel()
     a2 = m2.ravel()
 
     intersection = 0
     union_ = 0
 
-    for i in range(a1.size):
-        if a1[i] != 0 or a2[i] != 0:
-            union_ += 1
-            if a1[i] != 0 and a2[i] != 0:
-                intersection += 1
+    if not ignore is None and it != _TYPE_EMPTY:
+        m3 = _region_raster(ignore, raster_bounds, it, io)
+        a3 = m3.ravel()
+        for i in range(a1.size):
+            if a3[i] == 0: # Non-negative value means that we ignore the pixel
+                if a1[i] != 0 or a2[i] != 0:
+                    union_ += 1
+                    if a1[i] != 0 and a2[i] != 0:
+                        intersection += 1
+    else:
+        for i in range(a1.size):
+            if a1[i] != 0 or a2[i] != 0:
+                union_ += 1
+                if a1[i] != 0 and a2[i] != 0:
+                    intersection += 1
 
     return float(intersection) / float(union_) if union_ > 0 else float(0)
 
 from vot.region import Region, RegionException
 from vot.region.shapes import Shape, Rectangle, Polygon, Mask
 
 Bounds = Tuple[int, int]
 
-def calculate_overlap(reg1: Shape, reg2: Shape, bounds: Optional[Bounds] = None):
+def _infer_meta(reg: Region):
+    if isinstance(reg, Rectangle):
+        data1 = np.round(reg._data)
+        offset1 = (0, 0)
+        type1 = _TYPE_RECTANGLE
+    elif isinstance(reg, Polygon):
+        data1 = np.round(reg._points)
+        offset1 = (0, 0)
+        type1 = _TYPE_POLYGON
+    elif isinstance(reg, Mask):
+        data1 = reg.mask
+        offset1 = reg.offset
+        type1 = _TYPE_MASK
+    else:
+        data1 = np.zeros((1, 1))
+        offset1 = (0, 0)
+        type1 = _TYPE_EMPTY
+
+    return data1, offset1, type1
+
+def calculate_overlap(reg1: Shape, reg2: Shape, bounds: Optional[Bounds] = None, ignore: Optional[Shape] = None):
     """ Calculate the overlap between two regions. The function first rasterizes both regions to 2-D binary masks and calculates overlap between them
 
     Args:
         reg1: first region
         reg2: second region
         bounds: 2-tuple with the bounds of the image (width, height)
+        ignore: region to ignore when calculating overlap, usually a mask
 
     Returns:
         float with the overlap between the two regions. Note that overlap is one by definition if both regions are empty.
     
     """
 
-    if isinstance(reg1, Rectangle):
-        data1 = np.round(reg1._data)
-        offset1 = (0, 0)
-        type1 = _TYPE_RECTANGLE
-    elif isinstance(reg1, Polygon):
-        data1 = np.round(reg1._points)
-        offset1 = (0, 0)
-        type1 = _TYPE_POLYGON
-    elif isinstance(reg1, Mask):
-        data1 = reg1.mask
-        offset1 = reg1.offset
-        type1 = _TYPE_MASK
-    else:
-        data1 = np.zeros((1, 1))
-        offset1 = (0, 0)
-        type1 = _TYPE_EMPTY
+    data1, offset1, type1 = _infer_meta(reg1)
+    data2, offset2, type2 = _infer_meta(reg2)
 
-    if isinstance(reg2, Rectangle):
-        data2 = np.round(reg2._data)
-        offset2 = (0, 0)
-        type2 = _TYPE_RECTANGLE
-    elif isinstance(reg2, Polygon):
-        data2 = np.round(reg2._points)
-        offset2 = (0, 0)
-        type2 = _TYPE_POLYGON
-    elif isinstance(reg2, Mask):
-        data2 = reg2.mask
-        offset2 = reg2.offset
-        type2 = _TYPE_MASK
-    else:
-        data2 = np.zeros((1, 1))
-        offset2 = (0, 0)
-        type2 = _TYPE_EMPTY
+    if not ignore is None:
+        ignore_data, ignore_offset, ignore_type = _infer_meta(ignore)
+        return _calculate_overlap(data1, data2, type1, type2, offset1, offset2, bounds, ignore_data, ignore_type, ignore_offset)
 
     return _calculate_overlap(data1, data2, type1, type2, offset1, offset2, bounds)
 
-def calculate_overlaps(first: List[Region], second: List[Region], bounds: Optional[Bounds] = None):
+def calculate_overlaps(first: List[Region], second: List[Region], bounds: Optional[Bounds] = None, ignore: Optional[List[Region]] = None):
     """ Calculate the overlap between two lists of regions. The function first rasterizes both regions to 2-D binary masks and calculates overlap between them
 
     Args:
         first: first list of regions
         second: second list of regions
         bounds: 2-tuple with the bounds of the image (width, height)
+        ignore: list of regions to ignore when calculating overlap, usually a list of masks
 
     Returns:
         list of floats with the overlap between the two regions. Note that overlap is one by definition if both regions are empty.
 
     Raises:
         RegionException: if the lists are not of the same size
     """
     if not len(first) == len(second):
         raise RegionException("List not of the same size {} != {}".format(len(first), len(second)))
+    
+    if not ignore is None:
+        if not len(first) == len(ignore):
+            raise RegionException("List not of the same size {} != {}".format(len(first), len(ignore)))
+        return [calculate_overlap(pairs[0], pairs[1], bounds=bounds, ignore=ignore[i]) for i, pairs in enumerate(zip(first, second))]
     return [calculate_overlap(pairs[0], pairs[1], bounds=bounds) for i, pairs in enumerate(zip(first, second))]
```

### Comparing `vot-toolkit-0.6.4/vot/region/shapes.py` & `vot-toolkit-0.7.0/vot/region/shapes.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/region/tests.py` & `vot-toolkit-0.7.0/vot/region/tests.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,26 @@
 
         r1 = Rectangle(0, 0, 100, 100)
         self.assertEqual(calculate_overlap(r1, r1), 1)
 
         r1 = Rectangle(0, 0, 0, 0)        
         self.assertEqual(calculate_overlap(r1, r1), 1)
 
+    def test_ignore_mask(self):
+        """Tests if the mask ignore works correctly."""
+        from vot.region import Mask
+
+        r1 = Mask(np.ones((100, 100), dtype=np.uint8))
+        r2 = Mask(np.ones((100, 100), dtype=np.uint8))
+        ignore = Mask(np.zeros((100, 100), dtype=np.uint8))
+        self.assertEqual(calculate_overlap(r1, r2, ignore=ignore), 0)
+
+        ignore = Mask(np.ones((100, 100), dtype=np.uint8))
+        self.assertEqual(calculate_overlap(r1, r2, ignore=ignore), 1)
+
     def test_empty_mask(self):
         """Tests if the empty mask is correctly detected."""
         from vot.region import Mask
 
         mask = Mask(np.zeros((100, 100), dtype=np.uint8))
         self.assertTrue(mask.is_empty())
```

### Comparing `vot-toolkit-0.6.4/vot/stack/__init__.py` & `vot-toolkit-0.7.0/vot/stack/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 import os
 from typing import List, Mapping
 
 import yaml
 
 from attributee import Attributee, String, Boolean, Map, Object
+from attributee.io import Serializable
 
 from vot.experiment import Experiment, experiment_registry
 from vot.utilities import import_class
 
 def experiment_resolver(typename, context, **kwargs):
     """Resolves experiment objects from stack definitions. This function is used by the stack module to resolve experiment objects from stack
     definitions. It is not intended to be used directly.
@@ -35,45 +36,28 @@
         assert isinstance(experiment, Experiment)
         return experiment
     else:
         experiment_class = import_class(typename)
         assert issubclass(experiment_class, Experiment)
         return experiment_class(_identifier=identifier, _storage=storage, **kwargs)
 
-class Stack(Attributee):
+class Stack(Attributee, Serializable):
     """Stack class represents a collection of experiments. Stacks are used to organize experiments and to run them in batch mode.
     """
 
     title = String(default="Stack")
     dataset = String(default=None)
     url = String(default="")
     deprecated = Boolean(default=False)
     experiments = Map(Object(experiment_resolver))
 
-    def __init__(self, name: str, workspace: "Workspace", **kwargs):
-        """Creates a new stack object.
-
-        Args:
-            name (str): Name of the stack
-            workspace (Workspace): Workspace object
-        """
-        self._workspace = workspace
-        self._name = name
-
-        super().__init__(**kwargs)
-
-    @property
-    def workspace(self):
-        """Returns the workspace object for the stack."""
-        return self._workspace
-
     @property
     def name(self):
         """Returns the name of the stack."""
-        return self._name
+        return self.get("_name", None)
 
     def __iter__(self):
         """Iterates over experiments in the stack."""
         return iter(self.experiments.values())
 
     def __len__(self):
         """Returns the number of experiments in the stack."""
```

### Comparing `vot-toolkit-0.6.4/vot/stack/tests/multiobject.yaml` & `vot-toolkit-0.7.0/vot/stack/tests/multiobject.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/stack/tests/segmentation.yaml` & `vot-toolkit-0.7.0/vot/stack/tests/segmentation.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/stack/tests.py` & `vot-toolkit-0.7.0/vot/stack/tests.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/stack/vot2016/rgb.yaml` & `vot-toolkit-0.7.0/vot/stack/vot2018/shortterm.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,33 @@
-title: VOT2016 challenge
-dataset: http://data.votchallenge.net/vot2016/main/description.json
-url: http://www.votchallenge.net/vot2016/
+title: VOT-ST2018 challenge
+dataset: http://data.votchallenge.net/vot2018/main/description.json
+url: http://www.votchallenge.net/vot2018/
 experiments:
   baseline:
     type: supervised
     repetitions: 15
     skip_initialize: 5
     analyses:
       - type: supervised_average_ar
         sensitivity: 30
-      - type: cumulative_failures
       - type: supervised_eao_score
-        low: 108
-        high: 371
+        low: 100
+        high: 356
+      - type: supervised_eao_curve
+  realtime:
+    type: supervised
+    realtime:
+      grace: 3
+    repetitions: 1
+    skip_initialize: 5
+    analyses:
+      - type: supervised_average_ar
+        sensitivity: 30
+      - type: supervised_eao_score
+        low: 100
+        high: 356
       - type: supervised_eao_curve
   unsupervised:
     type: unsupervised
     repetitions: 1
     analyses:
-      - type: average_accuracy
+      - type: average_accuracy
```

### Comparing `vot-toolkit-0.6.4/vot/stack/vot2017.yaml` & `vot-toolkit-0.7.0/vot/stack/vot2017.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/stack/vot2018/shortterm.yaml` & `vot-toolkit-0.7.0/vot/stack/vot2016/rgb.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,21 @@
-title: VOT-ST2018 challenge
-dataset: http://data.votchallenge.net/vot2018/main/description.json
-url: http://www.votchallenge.net/vot2018/
+title: VOT2016 challenge
+dataset: https://data.votchallenge.net/vot2016/main/description.json
+url: https://www.votchallenge.net/vot2016/
 experiments:
   baseline:
     type: supervised
     repetitions: 15
     skip_initialize: 5
     analyses:
       - type: supervised_average_ar
         sensitivity: 30
+      - type: cumulative_failures
       - type: supervised_eao_score
-        low: 100
-        high: 356
-      - type: supervised_eao_curve
-  realtime:
-    type: supervised
-    realtime:
-      grace: 3
-    repetitions: 1
-    skip_initialize: 5
-    analyses:
-      - type: supervised_average_ar
-        sensitivity: 30
-      - type: supervised_eao_score
-        low: 100
-        high: 356
+        low: 108
+        high: 371
       - type: supervised_eao_curve
   unsupervised:
     type: unsupervised
     repetitions: 1
     analyses:
-      - type: average_accuracy
+      - type: average_accuracy
```

### Comparing `vot-toolkit-0.6.4/vot/stack/vot2019/shortterm.yaml` & `vot-toolkit-0.7.0/vot/stack/vot2019/shortterm.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/stack/vot2020/shortterm.yaml` & `vot-toolkit-0.7.0/vot/stack/vot2020/shortterm.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/stack/vot2021/st.yaml` & `vot-toolkit-0.7.0/vot/stack/vot2021/shortterm.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/stack/vot2022/stb.yaml` & `vot-toolkit-0.7.0/vot/stack/vot2022/shorttermbox.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/stack/vot2022/sts.yaml` & `vot-toolkit-0.7.0/vot/stack/vot2022/shortterm.yaml`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/tracker/__init__.py` & `vot-toolkit-0.7.0/vot/tracker/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -600,60 +600,60 @@
         """
         super().__init__(runtime.tracker)
         self._runtime = runtime
         self._grace = grace
         self._interval = interval
         self._countdown = 0
         self._time = 0
-        self._out = None
+        self._status = None
 
     @property
     def multiobject(self):
         """Returns True if the tracker supports multiple objects, False otherwise."""
         return self._runtime.multiobject
 
     def stop(self):
         """Stops the tracker runtime."""
         self._runtime.stop()
         self._time = 0
-        self._out = None
+        self._status = None
 
     def restart(self):
         """Restarts the tracker runtime, usually stars a new process."""
         self._runtime.restart()
         self._time = 0
-        self._out = None
+        self._status = None
 
     def initialize(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
         """Initializes the tracker runtime with specified frame and objects. Returns the initial objects and the time it took to initialize the tracker.
         
         Arguments:
             frame {Frame} -- The frame to initialize the tracker with.
             new {Objects} -- The objects to initialize the tracker with.
             properties {dict} -- The properties to initialize the tracker with.
             
         Returns:
             Tuple[Objects, float] -- The initial objects and the time it took to initialize the tracker.
         """
         self._countdown = self._grace
-        self._out = None
+        self._status = None
 
-        out, prop, time = self._runtime.initialize(frame, new, properties)
+        status, time = self._runtime.initialize(frame, new, properties)
 
         if time > self._interval:
             if self._countdown > 0:
                 self._countdown = self._countdown - 1
                 self._time = 0
             else:
                 self._time = time - self._interval
-                self._out = out
+                self._status = status
         else:
             self._time = 0
 
-        return out, prop, time
+        return status, time
 
 
     def update(self, frame: Frame, _: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
         """Updates the tracker runtime with specified frame and objects. Returns the updated objects and the time it took to update the tracker.
         
         Arguments:
             frame {Frame} -- The frame to update the tracker with.
@@ -662,30 +662,30 @@
             
         Returns:
             Tuple[Objects, float] -- The updated objects and the time it took to update the tracker.
         """
 
         if self._time > self._interval:
             self._time = self._time - self._interval
-            return self._out, dict(), 0
+            return self._status, 0
         else:
-            self._out = None
+            self._status = None
             self._time = 0
 
-        out, prop, time = self._runtime.update(frame, properties)
+        status, time = self._runtime.update(frame, properties)
 
         if time > self._interval:
             if self._countdown > 0:
                 self._countdown = self._countdown - 1
                 self._time = 0
             else:
                 self._time = time - self._interval
-                self._out = out
+                self._status = status
 
-        return out, prop, time
+        return status, time
 
 
 class PropertyInjectorTrackerRuntime(TrackerRuntime):
     """Base class for tracker runtime implementations that inject properties into the tracker runtime."""
 
     def __init__(self, runtime: TrackerRuntime, **kwargs):
         """Initializes the property injector tracker runtime with specified tracker runtime and properties.
@@ -790,34 +790,37 @@
             properties {dict} -- The properties to initialize the tracker with.
         
         Returns:
             Tuple[Objects, float] -- The initial objects and the time it took to initialize the tracker.
         """
 
         if isinstance(new, list) and len(new) != 1: raise TrackerException("Only supports single object tracking", tracker=self.tracker)
-        status = self._runtime.initialize(frame, new, properties)
+        status, time = self._runtime.initialize(frame, new, properties)
         if isinstance(status, list): status = status[0]
-        return status
+        return status, time
 
     def update(self, frame: Frame, new: Objects = None, properties: dict = None) -> Tuple[Objects, float]:
         """Updates the tracker runtime with specified frame and objects. Returns the updated objects and the time it took to update the tracker.
         
         Arguments:
             frame {Frame} -- The frame to update the tracker with.
             new {Objects} -- The objects to update the tracker with.
             properties {dict} -- The properties to update the tracker with.
             
         Returns:
             Tuple[Objects, float] -- The updated objects and the time it took to update the tracker.
         """
 
-        if not new is None: raise TrackerException("Only supports single object tracking", tracker=self.tracker)
-        status = self._runtime.update(frame, new, properties)
+        if not new is None and isinstance(new, list) and len(new) != 0:
+            raise TrackerException("Only supports single object tracking", tracker=self.tracker)
+        if new is None: 
+            new = []
+        status, time = self._runtime.update(frame, new, properties)
         if isinstance(status, list): status = status[0]
-        return status
+        return status, time
 
 class MultiObjectTrackerRuntime(TrackerRuntime):
     """ This is a wrapper for tracker runtimes that do not support multi object tracking. STILL IN DEVELOPMENT!"""
 
     def __init__(self, runtime: TrackerRuntime):
         """Initializes the multi object tracker runtime with specified tracker runtime.
```

### Comparing `vot-toolkit-0.6.4/vot/tracker/dummy.py` & `vot-toolkit-0.7.0/vot/tracker/dummy.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/tracker/results.py` & `vot-toolkit-0.7.0/vot/tracker/results.py`

 * *Files 4% similar despite different names*

```diff
@@ -242,14 +242,22 @@
     def __len__(self):
         """Returns the length of the trajectory.
 
         Returns:
             int: Length
         """
         return len(self._regions)
+    
+    def __iter__(self):
+        """Returns an iterator over the regions.
+
+        Returns:
+            Iterator: Iterator
+        """
+        return iter(self._regions)
 
     def write(self, results: Results, name: str):
         """Writes the trajectory to the results storage. 
 
         Args:
             results (Results): Results storage
             name (str): Trajectory name (without extension)
```

### Comparing `vot-toolkit-0.6.4/vot/tracker/tests.py` & `vot-toolkit-0.7.0/vot/tracker/tests.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/tracker/trax.py` & `vot-toolkit-0.7.0/vot/tracker/trax.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     """
     if isinstance(region, Rectangle):
         return TraxRectangle.create(region.x, region.y, region.width, region.height)
     elif isinstance(region, Polygon):
         return TraxPolygon.create([region[i] for i in range(region.size)])
     elif isinstance(region, Mask):
         return TraxMask.create(region.mask, x=region.offset[0], y=region.offset[1])
-    return None
+    raise TraxException("Unknown region type {}".format(type(region))) 
 
 def convert_traxregion(region: TraxRegion) -> Region:
     """ Converts a Trax region to a region.
 
     Args:
         region: The Trax region to be converted.
 
@@ -142,15 +142,15 @@
     if region.type == TraxRegion.RECTANGLE:
         x, y, width, height = region.bounds()
         return Rectangle(x, y, width, height)
     elif region.type == TraxRegion.POLYGON:
         return Polygon(list(region))
     elif region.type == TraxRegion.MASK:
         return Mask(region.array(), region.offset(), optimize=True)
-    return None
+    raise TraxException("Unknown region type {}".format(region.type))
 
 def convert_objects(objects: Objects) -> TraxRegion:
     """ Converts a list of objects to a Trax region.
 
     Args:
         objects: The list of objects to be converted.
```

### Comparing `vot-toolkit-0.6.4/vot/utilities/__init__.py` & `vot-toolkit-0.7.0/vot/utilities/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 import time
 import concurrent.futures as futures
 from logging import Formatter, LogRecord
 
 from numbers import Number
 from typing import Any, Mapping, Tuple
 import typing
-from vot import get_logger
 
 import six
 import colorama
 
+from class_registry import ClassRegistry
+
 __ALIASES = dict()
 
 def import_class(classpath: str) -> typing.Type:
     """Import a class from a string by importing parent packages. 
 
     Args:
         classpath (str): String representing a canonical class name with all parent packages.
@@ -150,19 +151,20 @@
     def __init__(self, description="Processing", total=100):
         """Creates a new progress bar.
 
         Args:
             description: The description of the progress bar.
             total: The total number of steps.
         """
+        from vot import get_logger
         silent = get_logger().level > logging.INFO
 
         if not silent:
-            self._tqdm = tqdm(disable=False if is_notebook() else None,
-                bar_format=" {desc:20.20} |{bar}| {percentage:3.0f}% [{elapsed}<{remaining}]")
+            self._tqdm = tqdm(disable=False if is_notebook() else None, 
+                bar_format=" {desc:20.20} |{bar}| {percentage:3.0f}% [{elapsed}<{remaining}]", file=sys.stdout, leave=False)
             self._tqdm.desc = description
             self._tqdm.total = total
         if silent or self._tqdm.disable:
             self._tqdm = None
             self._value = 0
             self._total = total if not silent else 0
 
@@ -601,8 +603,84 @@
 
     def __exit__(self, type, value, traceback):
         """Stops the timer and prints the elapsed time."""
         elapsed = time.time() - self._tstart
         if self.name:
             print('[%s]: %.4fs' % (self.name, elapsed))
         else:
-            print('Elapsed: %.4fs' % elapsed)
+            print('Elapsed: %.4fs' % elapsed)
+
+class Registry(ClassRegistry):
+    """A class registry for storing classes with a fallback to entry point registry."""
+
+    def __init__(self, group: str, attr_name: typing.Optional[str] = None) -> None:
+        """Initializes the registry.
+
+        Args:
+            group (str): The name of the entry point group that will be used to load new classes.
+            attr_name (typing.Optional[str], optional): If set, the registry will "brand" each class with its corresponding registry key. Defaults to None.
+        """
+        from class_registry import EntryPointClassRegistry
+        super(Registry, self).__init__(group, attr_name)
+        self._entry_point = EntryPointClassRegistry(group=group, attr_name=attr_name)
+
+
+    def __missing__(self, key: str) -> object:
+        """Attempts to load a class from the entry point registry if it is not found in the local registry.
+        
+        Args:
+            key (str): Key of the class to load
+
+        Returns:
+            object: Loaded class or None if not found
+        """
+        return self._entry_point.get(key)
+    
+class ObjectResolver(object):
+    
+    
+    def __init__(self, registry: ClassRegistry, extra_arguments: typing.Optional[typing.Callable] = None,
+                class_check: typing.Optional[typing.Callable] = None, object_check: typing.Optional[typing.Callable] = None):
+        """Initializes the object resolver. 
+        
+        Args:
+            registry (ClassRegistry): Registry of classes
+            extra_arguments (typing.Optional[typing.Callable], optional): Extra arguments to pass to the class constructor
+            class_check (typing.Optional[typing.Callable], optional): Function to check if the class is compatible with the purpose
+            object_check (typing.Optional[typing.Callable], optional): Function to check if the object is compatible with the purpose
+        """
+        self._registry = registry
+        self._extra_arguments = extra_arguments
+        self._class_check = class_check
+        self._object_check = object_check
+    
+    
+    
+    def __call__(self, typename, context, **kwargs):
+        """Resolve an object from a string. If the object is not registered, it is imported as a class and
+        instantiated with the provided arguments.
+
+        Args:
+            typename (str): Name of the analysis
+            context (Attributee): Context of the resolver
+
+        Returns:
+            Analysis: Resolved analysis
+        """
+
+        if self._extra_arguments:
+            kwargs.update(self._extra_arguments(context))
+
+        if typename in self._registry:
+            analysis = self._registry.get(typename, **kwargs)
+            if self._class_check:
+                assert self._class_check(analysis, context)
+        else:
+            analysis_class = import_class(typename)
+            if self._class_check:
+                assert self._class_check(analysis, context)
+            analysis = analysis_class(**kwargs)
+
+        if self._object_check:
+            assert self._object_check(analysis, context)
+
+        return analysis
```

### Comparing `vot-toolkit-0.6.4/vot/utilities/cli.py` & `vot-toolkit-0.7.0/vot/utilities/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,16 @@
 import os
 import sys
 import argparse
 import logging
 import yaml
 from datetime import datetime
 
-from .. import check_updates, check_debug, toolkit_version, get_logger
-from ..tracker import Registry, TrackerException
-from ..stack import resolve_stack, list_integrated_stacks
-from ..workspace import Workspace
-from ..workspace.storage import Cache
-from . import Progress, normalize_path, ColoredFormatter
+from .. import check_updates, toolkit_version, get_logger
+from . import Progress, normalize_path
 
 logger = get_logger()
 
 class EnvDefault(argparse.Action):
     """Argparse action that resorts to a value in a specified envvar if no value is provided via program arguments.
     """
     def __init__(self, envvar, required=True, default=None, separator=None, **kwargs):
@@ -42,16 +38,17 @@
     """Run a test for a tracker
 
     Args:
         config (argparse.Namespace): Configuration
     """
     from vot.dataset.dummy import generate_dummy
     from vot.dataset import load_sequence, Frame
-    from vot.tracker import ObjectStatus
+    from vot.tracker import ObjectStatus, Registry, TrackerException
     from vot.experiment.helpers import MultiObjectHelper
+    from vot.dataset.proxy import ObjectsHideFilterSequence
 
     trackers = Registry(config.registry)
 
     if not config.tracker:
         logger.error("Unable to continue without a tracker")
         logger.error("List of found trackers: ")
         for k in trackers.identifiers():
@@ -89,14 +86,17 @@
         logger.info("Generating dummy sequence")
 
         if config.sequence is None:
             sequence = generate_dummy(50, objects=3 if runtime.multiobject else 1)
         else:
             sequence = load_sequence(normalize_path(config.sequence))
 
+        if config.ignore:
+            sequence = ObjectsHideFilterSequence(sequence, config.ignore)
+
         logger.info("Obtaining runtime for tracker %s", tracker.identifier)
 
         context = {"continue" : True}
 
         def on_press(event):
             """Callback for key press event.
             
@@ -106,15 +106,16 @@
             if event.key == 'q':
                 context["continue"] = False
 
         if config.visualize:
             import matplotlib.pylab as plt
             from vot.utilities.draw import MatplotlibDrawHandle
             figure = plt.figure()
-            figure.canvas.set_window_title('VOT Test')
+            if hasattr(figure.canvas, "set_window_title"):
+                figure.canvas.set_window_title('VOT Test')
             axes = figure.add_subplot(1, 1, 1)
             axes.set_aspect("equal")
             handle = MatplotlibDrawHandle(axes, size=sequence.size)
             context["click"] = figure.canvas.mpl_connect('key_press_event', on_press)
             handle.style(fill=False)
             figure.show()
 
@@ -153,35 +154,61 @@
         logger.error("Error during tracker execution: {}".format(te))
         if runtime:
             runtime.stop()
     except KeyboardInterrupt:
         if runtime:
             runtime.stop()
 
-def do_workspace(config: argparse.Namespace):
-    """Initialize / manage a workspace.
+def do_initialize(config: argparse.Namespace):
+    """Initialize a workspace. If a stack is provided, the workspace is initialized with the stack. If no stack is provided,
+    but a dataset exists, then a dummy config can be created for this custom dataset. If neither is provided, the user is prompted to
+    provide a stack.
 
     Args:
         config (argparse.Namespace): Configuration
     """
 
-    from vot.workspace import WorkspaceException
+    from vot.workspace import WorkspaceException, Workspace
+    from ..stack import resolve_stack, list_integrated_stacks
 
-    if config.stack is None and os.path.isfile(os.path.join(config.workspace, "configuration.m")):
-        from vot.utilities.migration import migrate_matlab_workspace
-        migrate_matlab_workspace(config.workspace)
+    if Workspace.exists(config.workspace):
+        logger.error("Workspace already initialized")
         return
-    elif config.stack is None:
-        stacks = list_integrated_stacks()
-        logger.error("Unable to continue without a stack")
-        logger.error("List of available integrated stacks: ")
-        for k, v in sorted(stacks.items(), key=lambda x: x[0]):
-            logger.error(" * %s - %s", k, v)
 
-        return
+    if config.stack is None:
+        if os.path.isfile(os.path.join(config.workspace, "configuration.m")):
+            from vot.utilities.migration import migrate_matlab_workspace
+            migrate_matlab_workspace(config.workspace)
+            return
+        elif os.path.isfile(os.path.join(config.workspace, "sequences")):
+            sequences_directory = os.path.join(config.workspace, "sequences")
+            # Attempt to load a dataset from the sequences directory
+            from vot.dataset import load_dataset
+            logger.info("Found sequences directory, attempting to load dataset")
+            try:
+                dataset = load_dataset(sequences_directory)
+                logger.info("Loaded dataset: %s", dataset)
+
+            except Exception as e:
+                pass
+            if dataset is not None:
+                logger.info("Loaded dataset: %s", dataset)
+                default_config = dict(dataset=dataset)
+                Workspace.initialize(config.workspace, default_config, download=False)
+                logger.info("Initialized workspace in '%s'", config.workspace)
+                return
+
+        else:
+            stacks = list_integrated_stacks()
+            logger.error("Unable to continue without a stack")
+            logger.error("List of available integrated stacks: ")
+            for k, v in sorted(stacks.items(), key=lambda x: x[0]):
+                logger.error(" * %s - %s", k, v)
+
+            return
 
     stack_file = resolve_stack(config.stack)
 
     if stack_file is None:
         logger.error("Experiment stack %s not found", stack_file)
         return
 
@@ -197,14 +224,16 @@
     """Run an evaluation for a tracker on an experiment stack and a set of sequences.
     
     Args:
         config (argparse.Namespace): Configuration    
     """
 
     from vot.experiment import run_experiment
+    from ..tracker import Registry, TrackerException
+    from ..workspace import Workspace
 
     workspace = Workspace.load(config.workspace)
 
     logger.debug("Loaded workspace in '%s'", config.workspace)
 
     global_registry = [os.path.abspath(x) for x in config.registry]
 
@@ -217,113 +246,176 @@
     if len(trackers) == 0:
         logger.error("Unable to continue without at least on tracker")
         logger.error("List of available found trackers: ")
         for k in registry.identifiers():
             logger.error(" * %s", k)
         return
 
+    # Filter experiments
+    if config.experiments:
+        experiments = [v for k, v in workspace.stack.experiments.items() if k in config.experiments.split(",")]
+    else:
+        experiments = workspace.stack
+
+    if len(experiments) == 0:
+        logger.error("No experiments found, stopping.")
+        return
+
     try:
         for tracker in trackers:
             logger.debug("Evaluating tracker %s", tracker.identifier)
-            for experiment in workspace.stack:
+            for experiment in experiments:
                 run_experiment(experiment, tracker, workspace.dataset, config.force, config.persist)
 
         logger.info("Evaluation concluded successfuly")
 
     except KeyboardInterrupt:
         logger.info("Evaluation interrupted by the user")
     except TrackerException as te:
         logger.error("Evaluation interrupted by tracker error: {}".format(te))
 
-def do_analysis(config: argparse.Namespace):
-    """Run an analysis for a tracker on an experiment stack and a set of sequences.
+def do_analysis(args: argparse.Namespace):
+    """Run an analysis for a tracker on an experiment stack and a set of sequences. Analysis results are serialized
+    to disk either as a JSON file or as a YAML file.
 
     Args:
-        config (argparse.Namespace): Configuration
+        args (argparse.Namespace): Configuration
     """
+    from vot import config
 
     from vot.analysis import AnalysisProcessor, process_stack_analyses
-    from vot.document import generate_document
+    from vot.report import generate_serialized
+    from ..tracker import Registry
+    from ..workspace import Workspace
+    from ..workspace.storage import Cache
 
-    workspace = Workspace.load(config.workspace)
+    workspace = Workspace.load(args.workspace)
 
-    logger.debug("Loaded workspace in '%s'", config.workspace)
+    logger.debug("Loaded workspace in '%s'", args.workspace)
 
-    global_registry = [os.path.abspath(x) for x in config.registry]
+    global_registry = [os.path.abspath(x) for x in args.registry]
 
-    registry = Registry(list(workspace.registry) + global_registry, root=config.workspace)
+    registry = Registry(list(workspace.registry) + global_registry, root=args.workspace)
 
     logger.debug("Found data for %d trackers", len(registry))
 
-    if not config.trackers:
+    if not args.trackers:
         trackers = workspace.list_results(registry)
     else:
-        trackers = registry.resolve(*config.trackers, storage=workspace.storage.substorage("results"), skip_unknown=False)
+        trackers = registry.resolve(*args.trackers, storage=workspace.storage.substorage("results"), skip_unknown=False)
 
     if not trackers:
         logger.warning("No trackers resolved, stopping.")
         return
 
     logger.debug("Running analysis for %d trackers", len(trackers))
 
-    if config.workers == 1:
+    if config.worker_pool_size == 1:
 
-        if config.debug:
+        if args.debug:
             from vot.analysis.processor import DebugExecutor
             logging.getLogger("concurrent.futures").setLevel(logging.DEBUG)
             executor = DebugExecutor()
         else:
             from vot.utilities import ThreadPoolExecutor
             executor = ThreadPoolExecutor(1)
 
     else:
         from concurrent.futures import ProcessPoolExecutor
-        executor = ProcessPoolExecutor(config.workers)
+        executor = ProcessPoolExecutor(config.worker_pool_size)
 
-    if config.nocache:
+    if not config.persistent_cache:
         from cachetools import LRUCache
         cache = LRUCache(1000)
     else:
         cache = Cache(workspace.storage.substorage("cache").substorage("analysis"))
 
     try:
 
         with AnalysisProcessor(executor, cache):
 
             results = process_stack_analyses(workspace, trackers)
 
             if results is None:
                 return
 
-            if config.name is None:
+            if args.name is None:
                 name = "{:%Y-%m-%dT%H-%M-%S.%f%z}".format(datetime.now())
             else:
-                name = config.name
+                name = args.name
 
-            storage = workspace.storage.substorage("analysis").substorage(name)
+            storage = workspace.storage.substorage("analysis")
 
-            generate_document(config.format, workspace.report, trackers, workspace.dataset, results, storage)
+            if args.format == "json":
+                generate_serialized(trackers, workspace.dataset, results, storage, "json", name)
+            elif args.format == "yaml":
+                generate_serialized(trackers, workspace.dataset, results, storage, "yaml", name)
+            else:
+                raise ValueError("Unknown format '{}'".format(args.format))
 
             logger.info("Analysis successful, report available as %s", name)
 
     finally:
 
         executor.shutdown(wait=True)
 
+def do_report(config: argparse.Namespace):
+    """Generate a report for a one or multiple trackers on an experiment stack and a set of sequences.
+
+    Args:
+        config (argparse.Namespace): Configuration
+    """
+
+    from vot.report import generate_document
+    from ..tracker import Registry
+    from ..workspace import Workspace
+
+
+    if config.name is None:
+        name = "{:%Y-%m-%dT%H-%M-%S.%f%z}".format(datetime.now())
+    else:
+        name = config.name
+
+    workspace = Workspace.load(config.workspace)
+
+    logger.debug("Loaded workspace in '%s'", config.workspace)
+
+    global_registry = [os.path.abspath(x) for x in config.registry]
+
+    registry = Registry(list(workspace.registry) + global_registry, root=config.workspace)
+
+    logger.debug("Found data for %d trackers", len(registry))
+
+    if not config.trackers:
+        trackers = workspace.list_results(registry)
+    else:
+        trackers = registry.resolve(*config.trackers, storage=workspace.storage.substorage("results"), skip_unknown=False)
+
+    if not trackers:
+        logger.warning("No trackers resolved, stopping.")
+        return
+
+    logger.debug("Running analysis for %d trackers", len(trackers))
+
+    generate_document(workspace, trackers, config.format, name, config.sequences, config.experiments)
+    
     
 def do_pack(config: argparse.Namespace):
     """Package results to a ZIP file so that they can be submitted to a challenge.
 
     Args:
         config (argparse.Namespace): Configuration
     """
 
     import zipfile, io
     from shutil import copyfileobj
 
+    from ..tracker import Registry
+    from ..workspace import Workspace
+
     workspace = Workspace.load(config.workspace)
 
     logger.debug("Loaded workspace in '%s'", config.workspace)
 
     registry = Registry(list(workspace.registry) + config.registry, root=config.workspace)
 
     tracker = registry[config.tracker]
@@ -355,15 +447,15 @@
 
     archive_name = "{}_{:%Y-%m-%dT%H-%M-%S.%f%z}.zip".format(tracker.identifier, timestamp)
 
     with Progress("Compressing", len(all_files)) as progress:
 
         manifest = dict(identifier=tracker.identifier, configuration=tracker.describe(),
             timestamp="{:%Y-%m-%dT%H-%M-%S.%f%z}".format(timestamp), platform=sys.platform,
-            python=sys.version, toolkit=toolkit_version())
+            python=sys.version, toolkit=toolkit_version(), stack=workspace.stack.dump())
 
         with zipfile.ZipFile(workspace.storage.write(archive_name, binary=True), mode="w") as archive:
             for f in all_files:
                 info = zipfile.ZipInfo(filename=os.path.join(f[1], f[2], f[0]), date_time=timestamp.timetuple())
                 with archive.open(info, mode="w") as fout, f[3].read(f[0]) as fin:
                     if isinstance(fin, io.TextIOBase):
                         copyfileobj(fin, io.TextIOWrapper(fout))
@@ -376,80 +468,93 @@
                 yaml.dump(manifest, fout)
 
     logger.info("Result packaging successful, archive available in %s", archive_name)
 
 def main():
     """Entrypoint to the toolkit Command Line Interface utility, should be executed as a program and provided with arguments.
     """
-    stream = logging.StreamHandler()
-    stream.setFormatter(ColoredFormatter())
-    logger.addHandler(stream)
 
     parser = argparse.ArgumentParser(description='VOT Toolkit Command Line Interface', prog="vot")
     parser.add_argument("--debug", "-d", default=False, help="Backup backend", required=False, action='store_true')
     parser.add_argument("--registry", default=".", help='Tracker registry paths', required=False, action=EnvDefault, \
         separator=os.path.pathsep, envvar='VOT_REGISTRY')
 
     subparsers = parser.add_subparsers(help='commands', dest='action', title="Commands")
 
     test_parser = subparsers.add_parser('test', help='Test a tracker integration on a synthetic sequence')
     test_parser.add_argument("tracker", help='Tracker identifier', nargs="?")
     test_parser.add_argument("--visualize", "-g", default=False, required=False, help='Visualize results of the test session', action='store_true')
     test_parser.add_argument("--sequence", "-s", required=False, help='Path to sequence to use instead of dummy')
+    test_parser.add_argument("--ignore", required=False, help='Object IDs to ignore', type=lambda x: x.split(","), default=[])
 
-    workspace_parser = subparsers.add_parser('initialize', help='Setup a new workspace and download data')
+    workspace_parser = subparsers.add_parser('configure', aliases=["initialize"], help='Setup a new workspace and download data')
     workspace_parser.add_argument("--workspace", default=os.getcwd(), help='Workspace path')
     workspace_parser.add_argument("--nodownload", default=False, required=False, help="Do not download dataset if specified in stack", action='store_true')
     workspace_parser.add_argument("stack", nargs="?", help='Experiment stack')
 
-    evaluate_parser = subparsers.add_parser('evaluate', help='Evaluate one or more trackers in a given workspace')
+    evaluate_parser = subparsers.add_parser('evaluate', aliases=["run"], help='Evaluate one or more trackers in a given workspace')
     evaluate_parser.add_argument("trackers", nargs='+', default=None, help='Tracker identifiers')
     evaluate_parser.add_argument("--force", "-f", default=False, help="Force rerun of the entire evaluation", required=False, action='store_true')
     evaluate_parser.add_argument("--persist", "-p", default=False, help="Persist execution even in case of an error", required=False, action='store_true')
     evaluate_parser.add_argument("--workspace", default=os.getcwd(), help='Workspace path')
+    evaluate_parser.add_argument("--experiments", default=None, help='Filter specified experiments (comma separated names)', required=False)
 
-    analysis_parser = subparsers.add_parser('analysis', help='Run analysis of results')
+    analysis_parser = subparsers.add_parser('analysis', aliases=["analyse", "analyze"], help='Run analysis of results')
     analysis_parser.add_argument("trackers", nargs='*', help='Tracker identifiers')
     analysis_parser.add_argument("--workspace", default=os.getcwd(), help='Workspace path')
-    analysis_parser.add_argument("--format", choices=("html", "latex", "pdf", "json", "yaml"), default="html", help='Analysis output format')
+    analysis_parser.add_argument("--format", choices=("json", "yaml"), default="json", help='Analysis output format')
     analysis_parser.add_argument("--name", required=False, help='Analysis output name')
-    analysis_parser.add_argument("--workers", default=1, required=False, help='Number of parallel workers', type=int)
-    analysis_parser.add_argument("--nocache", default=False, required=False, help="Do not cache data to disk", action='store_true')
+
+    report_parser = subparsers.add_parser('report', aliases=["document"], help='Generate report document')
+    report_parser.add_argument("trackers", nargs='*', help='Tracker identifiers')
+    report_parser.add_argument("--workspace", default=os.getcwd(), help='Workspace path')
+    report_parser.add_argument("--format", choices=("html", "latex", "plots"), default="html", help='Analysis output format')
+    report_parser.add_argument("--name", required=False, help='Document output name')
+    report_parser.add_argument("--sequences", default=None, help='Filter specified sequences (comma separated names)', required=False)
+    report_parser.add_argument("--experiments", default=None, help='Filter specified experiments (comma separated names)', required=False)
 
     pack_parser = subparsers.add_parser('pack', help='Package results for submission')
     pack_parser.add_argument("--workspace", default=os.getcwd(), help='Workspace path')
     pack_parser.add_argument("tracker", help='Tracker identifier')
 
+    from vot import print_config
+
     try:
 
         args = parser.parse_args()
 
-        logger.setLevel(logging.INFO)
-
-        if args.debug or check_debug():
+        if args.debug:
+            os.environ["VOT_DEBUG_MODE"] = "1"
             logger.setLevel(logging.DEBUG)
+        else:
+            logger.setLevel(logging.INFO)
 
+        print_config()
+        
         def check_version():
             """Check if a newer version of the toolkit is available."""
             update, version = check_updates()
             if update:
                 logger.warning("A newer version of the VOT toolkit is available (%s), please update.", version)
 
         if args.action == "test":
             check_version()
             do_test(args)
-        elif args.action == "initialize":
+        elif args.action in ["configure", "initialize"]:
             check_version()
-            do_workspace(args)
-        elif args.action == "evaluate":
+            do_initialize(args)
+        elif args.action in ["evaluate", "run"]:
             check_version()
             do_evaluate(args)
-        elif args.action == "analysis":
+        elif args.action in ["analysis", "analyse", "analyze"]:
             check_version()
             do_analysis(args)
+        elif args.action in ["report", "document"]:
+            check_version()
+            do_report(args)
         elif args.action == "pack":
             check_version()
             do_pack(args)
         else:
             parser.print_help()
 
     except argparse.ArgumentError as e:
```

### Comparing `vot-toolkit-0.6.4/vot/utilities/data.py` & `vot-toolkit-0.7.0/vot/utilities/data.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/utilities/draw.py` & `vot-toolkit-0.7.0/vot/utilities/draw.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/utilities/migration.py` & `vot-toolkit-0.7.0/vot/utilities/migration.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/utilities/net.py` & `vot-toolkit-0.7.0/vot/utilities/net.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/utilities/notebook.py` & `vot-toolkit-0.7.0/vot/utilities/notebook.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/workspace/__init__.py` & `vot-toolkit-0.7.0/vot/workspace/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 from attributee import Attribute, Attributee, Nested, List, String, CoerceContext
 
 from .. import ToolkitException, get_logger
 from ..dataset import Dataset, load_dataset
 from ..tracker import Registry, Tracker
 from ..stack import Stack, resolve_stack
 from ..utilities import normalize_path
-from ..document import ReportConfiguration
+from ..report import ReportConfiguration
 from .storage import LocalStorage, Storage, NullStorage
 
-
 _logger = get_logger()
 
 class WorkspaceException(ToolkitException):
     """Errors related to workspace raise this exception
     """
     pass
 
@@ -44,19 +43,20 @@
         if isinstance(value, str):
 
             stack_file = resolve_stack(value, context.parent.directory)
 
             if stack_file is None:
                 raise WorkspaceException("Experiment stack does not exist")
 
-            with open(stack_file, 'r') as fp:
-                stack_metadata = yaml.load(fp, Loader=yaml.BaseLoader)
-                return Stack(value, context.parent, **stack_metadata)
+            stack = Stack.read(stack_file)
+            stack._name = value
+
+            return stack
         else:
-            return Stack(None, context.parent, **value)
+            return Stack(**value)
 
     def dump(self, value: "Stack") -> str:
         """Dump a Stack object to a string or a dictionary
         
         Args:
             value (Stack): Value to dump
             
@@ -75,28 +75,40 @@
 
     registry = List(String(transformer=lambda x, ctx: normalize_path(x, ctx.parent.directory)))
     stack = StackLoader()
     sequences = String(default="sequences")
     report = Nested(ReportConfiguration)
 
     @staticmethod
+    def exists(directory: str) -> bool:
+        """Check if a workspace exists in a given directory.
+
+        Args:
+            directory (str): Directory to check
+
+        Returns:
+            bool: True if the workspace exists, False otherwise.
+        """
+        return os.path.isfile(os.path.join(directory, "config.yaml"))
+
+    @staticmethod
     def initialize(directory: str, config: typing.Optional[typing.Dict] = None, download: bool = True) -> None:
         """Initialize a new workspace in a given directory with the given config
 
         Args:
             directory (str): Root for workspace storage
             config (typing.Optional[typing.Dict], optional): Workspace initial configuration. Defaults to None.
             download (bool, optional): Download the dataset immediately. Defaults to True.
 
         Raises:
             WorkspaceException: When a workspace cannot be created.
         """
 
         config_file = os.path.join(directory, "config.yaml")
-        if os.path.isfile(config_file):
+        if Workspace.exists(directory):
             raise WorkspaceException("Workspace already initialized")
 
         os.makedirs(directory, exist_ok=True)
 
         with open(config_file, 'w') as fp:
             yaml.dump(config if config is not None else dict(), fp)
 
@@ -152,15 +164,14 @@
         directory = normalize_path(directory)
         config_file = os.path.join(directory, "config.yaml")
         if not os.path.isfile(config_file):
             raise WorkspaceException("Workspace not initialized")
 
         with open(config_file, 'r') as fp:
             config = yaml.load(fp, Loader=yaml.BaseLoader)
-
             return Workspace(directory, **config)
 
     def __init__(self, directory: str, **kwargs):
         """Do not call this constructor directly unless you know what you are doing, 
         instead use the static Workspace.load method.
 
         Args:
@@ -168,22 +179,25 @@
         """
         self._directory = directory
 
         self._storage = Proxy(lambda: LocalStorage(directory) if directory is not None else NullStorage())
         
         super().__init__(**kwargs)
 
-        
         dataset_directory = normalize_path(self.sequences, directory)
 
         if not self.stack.dataset is None:
             Workspace.download_dataset(self.stack.dataset, dataset_directory)
 
         self._dataset = load_dataset(dataset_directory)
 
+        # Register storage with all experiments in the stack
+        for experiment in self.stack.experiments.values():
+            experiment._storage = self._storage
+
     @property
     def directory(self) -> str:
         """Returns the root directory for the workspace.
 
         Returns:
             str: The absolute path to the root of the workspace.
         """
```

### Comparing `vot-toolkit-0.6.4/vot/workspace/storage.py` & `vot-toolkit-0.7.0/vot/workspace/storage.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot/workspace/tests.py` & `vot-toolkit-0.7.0/vot/workspace/tests.py`

 * *Files identical despite different names*

### Comparing `vot-toolkit-0.6.4/vot_toolkit.egg-info/PKG-INFO` & `vot-toolkit-0.7.0/vot_toolkit.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 Metadata-Version: 2.1
 Name: vot-toolkit
-Version: 0.6.4
+Version: 0.7.0
 Summary: Perform visual object tracking experiments and analyze results
 Home-page: https://github.com/votchallenge/toolkit
 Author: Luka Cehovin Zajc
 Author-email: luka.cehovin@gmail.com
 License: UNKNOWN
-Description: 
-        The VOT evaluation toolkit
-        ==========================
-        
-        [![PyPI package version](https://badge.fury.io/py/vot-toolkit.svg)](https://badge.fury.io/py/vot-toolkit)
-        
-        This repository contains the official evaluation toolkit for the [Visual Object Tracking (VOT) challenge](http://votchallenge.net/). This is the official version of the toolkit, implemented in Python 3 language. If you are looking for the old Matlab version, you can find an archived repository [here](https://github.com/votchallenge/toolkit-legacy).
-        
-        For more detailed informations consult the documentation available in the source or a compiled version of the documentation [here](http://www.votchallenge.net/howto/). You can also subscribe to the VOT [mailing list](https://liste.arnes.si/mailman3/lists/votchallenge.lists.arnes.si/) to receive news about challenges and important software updates or join our [support form](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help) to ask questions.
-        
-        Developers
-        ----------
-        
-        The VOT toolkit is developed and maintained by  [Luka Čehovin Zajc](https://vicos.si/lukacu) with the help of the VOT innitiative members and the VOT community.
-        
-        Contributors:
-        
-        * [Luka Čehovin Zajc](https://vicos.si/lukacu), University of Ljubljana
-        * [Alan Lukežič](https://vicos.si/people/alan_lukezic/), University of Ljubljana
-        * Yan Song, Tampere University
-        
-        Acknowledgements
-        ----------------
-        
-        The development of this package was supported by Sloveninan research agency (ARRS) projects Z2-1866 and J2-316.
-        
-        License
-        -------
-        
-        Copyright (C) 2023 Luka Čehovin Zajc and the [VOT Challenge innitiative](http://votchallenge.net/).
-        
-        This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
-        
-        This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
-        
-        You should have received a copy of the GNU General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.
-        
-        Enquiries, Question and Comments
-        --------------------------------
-        
-        If you have any further enquiries, question, or comments, please refer to the contact information link on the [VOT homepage](http://votchallenge.net/). If you would like to file a bug report or a feature request, use the  [Github issue tracker](https://github.com/votchallenge/toolkit/issues). **The issue tracker is for toolkit issues only**, if you have a problem with tracker integration or any other questions, please use our [support forum](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help).
-        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+The VOT evaluation toolkit
+==========================
+
+[![Documentation Status](https://readthedocs.org/projects/vot-toolkit/badge/?version=latest)](https://vot-toolkit.readthedocs.io/en/latest/?badge=latest)
+[![PyPI package version](https://badge.fury.io/py/vot-toolkit.svg)](https://badge.fury.io/py/vot-toolkit)
+
+This repository contains the official evaluation toolkit for the [Visual Object Tracking (VOT) challenge](http://votchallenge.net/). This is the official version of the toolkit, implemented in Python 3 language. If you are looking for the old Matlab version, you can find an archived repository [here](https://github.com/votchallenge/toolkit-legacy).
+
+For more detailed informations consult the documentation available [here](http://vot-toolkit.readthedocs.io/). You can also subscribe to the VOT [mailing list](https://liste.arnes.si/mailman3/lists/votchallenge.lists.arnes.si/) to receive news about challenges and important software updates or join our [support form](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help) to ask questions.
+
+Developers
+----------
+
+The VOT toolkit is developed and maintained by  [Luka Čehovin Zajc](https://vicos.si/lukacu) with the help of the VOT innitiative members and the VOT community.
+
+Contributors:
+
+* [Luka Čehovin Zajc](https://vicos.si/lukacu), University of Ljubljana
+* [Alan Lukežič](https://vicos.si/people/alan_lukezic/), University of Ljubljana
+* Yan Song, Tampere University
+
+Acknowledgements
+----------------
+
+The development of this package was supported by Slovenian research agency (ARRS) projects Z2-1866 and J2-316.
+
+License
+-------
+
+Copyright (C) 2024 Luka Čehovin Zajc and the [VOT Challenge innitiative](http://votchallenge.net/).
+
+This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+
+This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+Enquiries, Question and Comments
+--------------------------------
+
+If you have any further enquiries, question, or comments, please refer to the contact information link on the [VOT homepage](http://votchallenge.net/). If you would like to file a bug report or a feature request, use the  [Github issue tracker](https://github.com/votchallenge/toolkit/issues). **The issue tracker is for toolkit issues only**, if you have a problem with tracker integration or any other questions, please use our [support forum](https://groups.google.com/forum/?hl=en#!forum/votchallenge-help).
+
+
```

### Comparing `vot-toolkit-0.6.4/vot_toolkit.egg-info/SOURCES.txt` & `vot-toolkit-0.7.0/vot_toolkit.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,53 @@
+LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 vot/__init__.py
 vot/__main__.py
 vot/version.py
 vot/analysis/__init__.py
 vot/analysis/accuracy.py
 vot/analysis/failures.py
 vot/analysis/longterm.py
 vot/analysis/multistart.py
 vot/analysis/processor.py
 vot/analysis/supervised.py
+vot/analysis/tests.py
 vot/dataset/__init__.py
 vot/dataset/common.py
 vot/dataset/cow.png
 vot/dataset/dummy.py
 vot/dataset/got10k.py
 vot/dataset/otb.py
 vot/dataset/proxy.py
 vot/dataset/trackingnet.py
-vot/document/__init__.py
-vot/document/commands.tex
-vot/document/common.py
-vot/document/html.py
-vot/document/jquery.js
-vot/document/latex.py
-vot/document/pure.css
-vot/document/report.css
-vot/document/report.js
-vot/document/table.js
-vot/document/tests.py
 vot/experiment/__init__.py
 vot/experiment/helpers.py
 vot/experiment/multirun.py
 vot/experiment/multistart.py
 vot/experiment/transformer.py
 vot/region/__init__.py
 vot/region/io.py
 vot/region/raster.py
 vot/region/shapes.py
 vot/region/tests.py
+vot/report/__init__.py
+vot/report/commands.tex
+vot/report/common.py
+vot/report/html.py
+vot/report/jquery.js
+vot/report/latex.py
+vot/report/pure.css
+vot/report/report.css
+vot/report/report.js
+vot/report/table.js
+vot/report/tests.py
+vot/report/video.py
 vot/stack/__init__.py
 vot/stack/otb100.yaml
 vot/stack/otb50.yaml
 vot/stack/tests.py
 vot/stack/vot2013.yaml
 vot/stack/vot2014.yaml
 vot/stack/vot2017.yaml
@@ -62,22 +65,25 @@
 vot/stack/vot2019/rgbd.yaml
 vot/stack/vot2019/rgbtir.yaml
 vot/stack/vot2019/shortterm.yaml
 vot/stack/vot2020/longterm.yaml
 vot/stack/vot2020/rgbd.yaml
 vot/stack/vot2020/rgbtir.yaml
 vot/stack/vot2020/shortterm.yaml
-vot/stack/vot2021/lt.yaml
+vot/stack/vot2021/longterm.yaml
 vot/stack/vot2021/rgbd.yaml
-vot/stack/vot2021/st.yaml
+vot/stack/vot2021/shortterm.yaml
 vot/stack/vot2022/depth.yaml
-vot/stack/vot2022/lt.yaml
+vot/stack/vot2022/longterm.yaml
 vot/stack/vot2022/rgbd.yaml
-vot/stack/vot2022/stb.yaml
-vot/stack/vot2022/sts.yaml
+vot/stack/vot2022/shortterm.yaml
+vot/stack/vot2022/shorttermbox.yaml
+vot/stack/vots2024/main.yaml
+vot/stack/vots2024/votst.yaml
+vot/stack/vots2024/votstval.yaml
 vot/tracker/__init__.py
 vot/tracker/dummy.py
 vot/tracker/results.py
 vot/tracker/tests.py
 vot/tracker/trax.py
 vot/utilities/__init__.py
 vot/utilities/cli.py
```

