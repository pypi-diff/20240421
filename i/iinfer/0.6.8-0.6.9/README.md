# Comparing `tmp/iinfer-0.6.8.tar.gz` & `tmp/iinfer-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iinfer-0.6.8.tar", last modified: Thu Apr 11 14:35:47 2024, max compression
+gzip compressed data, was "iinfer-0.6.9.tar", last modified: Mon Apr 15 12:38:00 2024, max compression
```

## Comparing `iinfer-0.6.8.tar` & `iinfer-0.6.9.tar`

### file list

```diff
@@ -1,181 +1,192 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.974518 iinfer-0.6.8/
--rw-rw-rw-   0        0        0     1117 2024-02-15 15:34:04.000000 iinfer-0.6.8/LICENSE
--rw-rw-rw-   0        0        0     5553 2024-04-11 14:35:47.973520 iinfer-0.6.8/PKG-INFO
--rw-rw-rw-   0        0        0     4619 2024-03-11 12:57:36.000000 iinfer-0.6.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.440513 iinfer-0.6.8/iinfer/
--rw-rw-rw-   0        0        0       69 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/__init__.py
--rw-rw-rw-   0        0        0      109 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.618517 iinfer-0.6.8/iinfer/app/
--rw-rw-rw-   0        0        0       73 2024-03-10 12:26:23.000000 iinfer-0.6.8/iinfer/app/__init__.py
--rw-rw-rw-   0        0        0    42217 2024-04-11 12:15:10.000000 iinfer-0.6.8/iinfer/app/app.py
--rw-rw-rw-   0        0        0    26784 2024-03-31 14:29:35.000000 iinfer-0.6.8/iinfer/app/client.py
--rw-rw-rw-   0        0        0    12275 2024-04-07 04:28:16.000000 iinfer-0.6.8/iinfer/app/common.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.625515 iinfer-0.6.8/iinfer/app/commons/
--rw-rw-rw-   0        0        0     5433 2024-02-26 12:32:33.000000 iinfer-0.6.8/iinfer/app/commons/convert.py
--rw-rw-rw-   0        0        0     7466 2024-03-30 02:49:07.000000 iinfer-0.6.8/iinfer/app/commons/module.py
--rw-rw-rw-   0        0        0    48856 2024-04-11 14:07:45.000000 iinfer-0.6.8/iinfer/app/gui.py
--rw-rw-rw-   0        0        0     5247 2024-04-11 12:30:41.000000 iinfer-0.6.8/iinfer/app/injection.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.649519 iinfer-0.6.8/iinfer/app/injections/
--rw-rw-rw-   0        0        0     2023 2024-04-11 11:13:52.000000 iinfer-0.6.8/iinfer/app/injections/after_cls_jadge_injection.py
--rw-rw-rw-   0        0        0     4500 2024-04-06 14:50:20.000000 iinfer-0.6.8/iinfer/app/injections/after_csv_injection.py
--rw-rw-rw-   0        0        0     6515 2024-04-07 06:56:33.000000 iinfer-0.6.8/iinfer/app/injections/after_det_filter_injection.py
--rw-rw-rw-   0        0        0     8540 2024-04-07 07:16:07.000000 iinfer-0.6.8/iinfer/app/injections/after_det_jadge_injection.py
--rw-rw-rw-   0        0        0     4790 2024-04-07 00:11:59.000000 iinfer-0.6.8/iinfer/app/injections/after_http_injection.py
--rw-rw-rw-   0        0        0     9077 2024-04-11 13:28:27.000000 iinfer-0.6.8/iinfer/app/injections/after_seg_bbox_injection.py
--rw-rw-rw-   0        0        0     8688 2024-04-11 13:41:09.000000 iinfer-0.6.8/iinfer/app/injections/after_seg_filter_injection.py
--rw-rw-rw-   0        0        0     1810 2024-02-25 07:58:13.000000 iinfer-0.6.8/iinfer/app/injections/before_grayimg_injection.py
--rw-rw-rw-   0        0        0    14447 2024-03-23 14:43:05.000000 iinfer-0.6.8/iinfer/app/install.py
--rw-rw-rw-   0        0        0     4811 2024-03-10 08:54:06.000000 iinfer-0.6.8/iinfer/app/postprocess.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.675518 iinfer-0.6.8/iinfer/app/postprocesses/
--rw-rw-rw-   0        0        0     1935 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/app/postprocesses/cls_jadge.py
--rw-rw-rw-   0        0        0     2393 2024-04-06 14:52:31.000000 iinfer-0.6.8/iinfer/app/postprocesses/csv.py
--rw-rw-rw-   0        0        0     4197 2024-03-10 09:01:15.000000 iinfer-0.6.8/iinfer/app/postprocesses/det_clip.py
--rw-rw-rw-   0        0        0     5063 2024-03-17 02:51:08.000000 iinfer-0.6.8/iinfer/app/postprocesses/det_face_store.py
--rw-rw-rw-   0        0        0     4444 2024-04-11 13:48:21.000000 iinfer-0.6.8/iinfer/app/postprocesses/det_filter.py
--rw-rw-rw-   0        0        0     5201 2024-04-07 07:20:08.000000 iinfer-0.6.8/iinfer/app/postprocesses/det_jadge.py
--rw-rw-rw-   0        0        0     3813 2024-04-07 00:25:09.000000 iinfer-0.6.8/iinfer/app/postprocesses/httpreq.py
--rw-rw-rw-   0        0        0     4369 2024-04-11 13:06:06.000000 iinfer-0.6.8/iinfer/app/postprocesses/seg_bbox.py
--rw-rw-rw-   0        0        0     4252 2024-04-11 12:27:14.000000 iinfer-0.6.8/iinfer/app/postprocesses/seg_filter.py
--rw-rw-rw-   0        0        0     6077 2024-02-24 13:15:38.000000 iinfer-0.6.8/iinfer/app/predict.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.712516 iinfer-0.6.8/iinfer/app/predicts/
--rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/app/predicts/__init__.py
--rw-rw-rw-   0        0        0     7618 2024-03-30 02:49:18.000000 iinfer-0.6.8/iinfer/app/predicts/insightface_det.py
--rw-rw-rw-   0        0        0     4134 2024-03-30 02:49:30.000000 iinfer-0.6.8/iinfer/app/predicts/mmdet_det_YoloX.py
--rw-rw-rw-   0        0        0      384 2024-03-30 02:49:24.000000 iinfer-0.6.8/iinfer/app/predicts/mmdet_det_YoloX_Lite.py
--rw-rw-rw-   0        0        0     4712 2024-03-30 02:49:40.000000 iinfer-0.6.8/iinfer/app/predicts/mmpretrain_cls_swin.py
--rw-rw-rw-   0        0        0      418 2024-03-30 02:49:36.000000 iinfer-0.6.8/iinfer/app/predicts/mmpretrain_cls_swin_Lite.py
--rw-rw-rw-   0        0        0    10366 2024-03-30 02:49:45.000000 iinfer-0.6.8/iinfer/app/predicts/mmrotate_det_ReDet.py
--rw-rw-rw-   0        0        0     5712 2024-04-05 13:16:32.000000 iinfer-0.6.8/iinfer/app/predicts/mmseg_seg_PSPNet.py
--rw-rw-rw-   0        0        0      386 2024-03-30 02:49:57.000000 iinfer-0.6.8/iinfer/app/predicts/mmseg_seg_SwinUpernet.py
--rw-rw-rw-   0        0        0     4647 2024-03-30 02:50:02.000000 iinfer-0.6.8/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py
--rw-rw-rw-   0        0        0     5301 2024-03-30 02:50:07.000000 iinfer-0.6.8/iinfer/app/predicts/onnx_det_TinyYoloV3.py
--rw-rw-rw-   0        0        0     5509 2024-03-30 02:50:11.000000 iinfer-0.6.8/iinfer/app/predicts/onnx_det_YoloV3.py
--rw-rw-rw-   0        0        0     9843 2024-03-30 02:50:23.000000 iinfer-0.6.8/iinfer/app/predicts/onnx_det_YoloX.py
--rw-rw-rw-   0        0        0     2887 2024-03-30 02:50:17.000000 iinfer-0.6.8/iinfer/app/predicts/onnx_det_YoloX_Lite.py
--rw-rw-rw-   0        0        0     2706 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/app/redis.py
--rw-rw-rw-   0        0        0    40369 2024-03-31 14:26:00.000000 iinfer-0.6.8/iinfer/app/server.py
--rw-rw-rw-   0        0        0       54 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/config.yml
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.719521 iinfer-0.6.8/iinfer/datasets/
--rw-rw-rw-   0        0        0      684 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/datasets/label_coco.txt
--rw-rw-rw-   0        0        0      153 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/datasets/label_voc.txt
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.727518 iinfer-0.6.8/iinfer/docker/
--rw-rw-rw-   0        0        0      813 2024-03-11 12:27:01.000000 iinfer-0.6.8/iinfer/docker/Dockerfile
--rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/docker/__init__.py
--rw-rw-rw-   0        0        0      131 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/docker/build.sh
--rw-rw-rw-   0        0        0      319 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/docker/docker-compose.yml
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.393645 iinfer-0.6.8/iinfer/extensions/
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.751519 iinfer-0.6.8/iinfer/extensions/injection/
--rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.6.8/iinfer/extensions/injection/after_cls_jadge_injection.json
--rw-rw-rw-   0        0        0       99 2024-04-11 14:24:51.000000 iinfer-0.6.8/iinfer/extensions/injection/after_csv_injection.json
--rw-rw-rw-   0        0        0      129 2024-04-07 04:03:58.000000 iinfer-0.6.8/iinfer/extensions/injection/after_det_filter_injection.json
--rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.6.8/iinfer/extensions/injection/after_det_jadge_injection.json
--rw-rw-rw-   0        0        0      176 2024-02-25 01:08:47.000000 iinfer-0.6.8/iinfer/extensions/injection/after_http_injection.json
--rw-rw-rw-   0        0        0      107 2024-04-07 03:43:59.000000 iinfer-0.6.8/iinfer/extensions/injection/after_seg_bbox_injection.json
--rw-rw-rw-   0        0        0      115 2024-04-07 03:42:37.000000 iinfer-0.6.8/iinfer/extensions/injection/after_seg_filter_injection.json
--rw-rw-rw-   0        0        0        2 2024-02-18 07:43:45.000000 iinfer-0.6.8/iinfer/extensions/injection/before_gray_injection.json
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.872519 iinfer-0.6.8/iinfer/licenses/
--rw-rw-rw-   0        0        0     1089 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1121 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt
--rw-rw-rw-   0        0        0    10351 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt
--rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.bottle-websocket.0.2.9(MIT License).txt
--rw-rw-rw-   0        0        0     1080 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt
--rw-rw-rw-   0        0        0     1009 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt
--rw-rw-rw-   0        0        0     1320 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1090 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt
--rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt
--rw-rw-rw-   0        0        0     1523 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt
--rw-rw-rw-   0        0        0     1105 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt
--rw-rw-rw-   0        0        0     1093 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt
--rw-rw-rw-   0        0        0     1094 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt
--rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.gevent-websocket.0.10.1(Copyright 2011-2017 Jeffrey Gelens jeffrey@noppo.pro).txt
--rw-rw-rw-   0        0        0     1260 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt
--rw-rw-rw-   0        0        0     1464 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt
--rw-rw-rw-   0        0        0     1572 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt
--rw-rw-rw-   0        0        0     1117 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt
--rw-rw-rw-   0        0        0     3350 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt
--rw-rw-rw-   0        0        0     4928 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt
--rw-rw-rw-   0        0        0     1088 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt
--rw-rw-rw-   0        0        0    48691 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt
--rw-rw-rw-   0        0        0   154222 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt
--rw-rw-rw-   0        0        0      200 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.packaging.24.0(Apache Software License; BSD License).txt
--rw-rw-rw-   0        0        0    56516 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt
--rw-rw-rw-   0        0        0     1113 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt
--rw-rw-rw-   0        0        0     1642 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt
--rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt
--rw-rw-rw-   0        0        0     1041 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt
--rw-rw-rw-   0        0        0     2942 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt
--rw-rw-rw-   0        0        0     1095 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt
--rw-rw-rw-   0        0        0    10317 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt
--rw-rw-rw-   0        0        0    47742 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt
--rw-rw-rw-   0        0        0     1040 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt
--rw-rw-rw-   0        0        0     1084 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt
--rw-rw-rw-   0        0        0     1100 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt
--rw-rw-rw-   0        0        0     1114 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt
--rw-rw-rw-   0        0        0     1349 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt
--rw-rw-rw-   0        0        0     1128 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt
--rw-rw-rw-   0        0        0     1495 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt
--rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt
--rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt
--rw-rw-rw-   0        0        0     6545 2024-03-27 11:58:45.000000 iinfer-0.6.8/iinfer/licenses/files.txt
--rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/logconf_client.yml
--rw-rw-rw-   0        0        0      630 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/logconf_gui.yml
--rw-rw-rw-   0        0        0      655 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/logconf_install.yml
--rw-rw-rw-   0        0        0      669 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/logconf_postprocess.yml
--rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/logconf_redis.yml
--rw-rw-rw-   0        0        0      650 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/logconf_server.yml
--rw-rw-rw-   0        0        0     1010 2024-04-11 14:17:29.000000 iinfer-0.6.8/iinfer/version.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.875520 iinfer-0.6.8/iinfer/web/
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.404514 iinfer-0.6.8/iinfer/web/assets/
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.888521 iinfer-0.6.8/iinfer/web/assets/bootstrap/
--rw-rw-rw-   0        0        0    78749 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js
--rw-rw-rw-   0        0        0    80421 2024-02-18 08:27:56.000000 iinfer-0.6.8/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js
--rw-rw-rw-   0        0        0   155851 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css
--rw-rw-rw-   0        0        0   232914 2024-02-18 08:28:29.000000 iinfer-0.6.8/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.891521 iinfer-0.6.8/iinfer/web/assets/jquery/
--rw-rw-rw-   0        0        0    86600 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery/jquery.min.3.2.0.js
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.893518 iinfer-0.6.8/iinfer/web/assets/jquery-resizable/
--rw-rw-rw-   0        0        0     3448 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.914519 iinfer-0.6.8/iinfer/web/assets/jquery-ui/
--rw-rw-rw-   0        0        0    14615 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/AUTHORS.txt
--rw-rw-rw-   0        0        0     1860 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.930519 iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/
--rw-rw-rw-   0        0        0     7142 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png
--rw-rw-rw-   0        0        0     7126 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png
--rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png
--rw-rw-rw-   0        0        0     7163 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png
--rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png
--rw-rw-rw-   0        0        0     6539 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png
--rw-rw-rw-   0        0        0    32136 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/jquery-ui.min.css
--rw-rw-rw-   0        0        0   255089 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/jquery-ui.min.js
--rw-rw-rw-   0        0        0    15564 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css
--rw-rw-rw-   0        0        0    13895 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css
--rw-rw-rw-   0        0        0     1886 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/jquery-ui/package.json
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.403514 iinfer-0.6.8/iinfer/web/assets/lightbox2/
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.939518 iinfer-0.6.8/iinfer/web/assets/lightbox2/css/
--rw-rw-rw-   0        0        0     2532 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/lightbox2/css/lightbox.min.css
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.953522 iinfer-0.6.8/iinfer/web/assets/lightbox2/images/
--rw-rw-rw-   0        0        0      280 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/lightbox2/images/close.png
--rw-rw-rw-   0        0        0     8476 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/lightbox2/images/loading.gif
--rw-rw-rw-   0        0        0     1350 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/lightbox2/images/next.png
--rw-rw-rw-   0        0        0     1360 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/lightbox2/images/prev.png
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.956519 iinfer-0.6.8/iinfer/web/assets/lightbox2/js/
--rw-rw-rw-   0        0        0     9768 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/lightbox2/js/lightbox.min.js
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.405512 iinfer-0.6.8/iinfer/web/assets/tree-menu/
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.958519 iinfer-0.6.8/iinfer/web/assets/tree-menu/css/
--rw-rw-rw-   0        0        0     1101 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/tree-menu/css/tree-menu.css
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.969523 iinfer-0.6.8/iinfer/web/assets/tree-menu/image/
--rw-rw-rw-   0        0        0      248 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/tree-menu/image/file.png
--rw-rw-rw-   0        0        0      284 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/tree-menu/image/folder-close.png
--rw-rw-rw-   0        0        0      301 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/tree-menu/image/folder-open.png
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.972520 iinfer-0.6.8/iinfer/web/assets/tree-menu/js/
--rw-rw-rw-   0        0        0     1029 2024-02-15 15:34:05.000000 iinfer-0.6.8/iinfer/web/assets/tree-menu/js/tree-menu.js
--rw-rw-rw-   0        0        0    72259 2024-04-11 12:58:28.000000 iinfer-0.6.8/iinfer/web/main.html
-drwxrwxrwx   0        0        0        0 2024-04-11 14:35:47.558516 iinfer-0.6.8/iinfer.egg-info/
--rw-rw-rw-   0        0        0     5553 2024-04-11 14:35:47.000000 iinfer-0.6.8/iinfer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6875 2024-04-11 14:35:47.000000 iinfer-0.6.8/iinfer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 14:35:47.000000 iinfer-0.6.8/iinfer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-04-11 14:35:47.000000 iinfer-0.6.8/iinfer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       88 2024-04-11 14:35:47.000000 iinfer-0.6.8/iinfer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-11 14:35:47.000000 iinfer-0.6.8/iinfer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 14:35:47.975520 iinfer-0.6.8/setup.cfg
--rw-rw-rw-   0        0        0     2185 2024-04-06 23:22:57.000000 iinfer-0.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.944293 iinfer-0.6.9/
+-rw-rw-rw-   0        0        0     1117 2024-02-15 15:34:04.000000 iinfer-0.6.9/LICENSE
+-rw-rw-rw-   0        0        0     5553 2024-04-15 12:38:00.942295 iinfer-0.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4619 2024-03-11 12:57:36.000000 iinfer-0.6.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-15 12:37:59.874571 iinfer-0.6.9/iinfer/
+-rw-rw-rw-   0        0        0       69 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/__init__.py
+-rw-rw-rw-   0        0        0      109 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:37:59.942578 iinfer-0.6.9/iinfer/app/
+-rw-rw-rw-   0        0        0       73 2024-03-10 12:26:23.000000 iinfer-0.6.9/iinfer/app/__init__.py
+-rw-rw-rw-   0        0        0    44638 2024-04-14 02:06:22.000000 iinfer-0.6.9/iinfer/app/app.py
+-rw-rw-rw-   0        0        0    31308 2024-04-14 08:44:28.000000 iinfer-0.6.9/iinfer/app/client.py
+-rw-rw-rw-   0        0        0    12382 2024-04-13 10:46:15.000000 iinfer-0.6.9/iinfer/app/common.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:37:59.962579 iinfer-0.6.9/iinfer/app/commons/
+-rw-rw-rw-   0        0        0     5433 2024-02-26 12:32:33.000000 iinfer-0.6.9/iinfer/app/commons/convert.py
+-rw-rw-rw-   0        0        0     7466 2024-03-30 02:49:07.000000 iinfer-0.6.9/iinfer/app/commons/module.py
+-rw-rw-rw-   0        0        0    57143 2024-04-15 11:48:19.000000 iinfer-0.6.9/iinfer/app/gui.py
+-rw-rw-rw-   0        0        0     5247 2024-04-11 12:30:41.000000 iinfer-0.6.9/iinfer/app/injection.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.019585 iinfer-0.6.9/iinfer/app/injections/
+-rw-rw-rw-   0        0        0     2023 2024-04-11 11:13:52.000000 iinfer-0.6.9/iinfer/app/injections/after_cls_jadge_injection.py
+-rw-rw-rw-   0        0        0     4500 2024-04-06 14:50:20.000000 iinfer-0.6.9/iinfer/app/injections/after_csv_injection.py
+-rw-rw-rw-   0        0        0     6515 2024-04-07 06:56:33.000000 iinfer-0.6.9/iinfer/app/injections/after_det_filter_injection.py
+-rw-rw-rw-   0        0        0     8540 2024-04-07 07:16:07.000000 iinfer-0.6.9/iinfer/app/injections/after_det_jadge_injection.py
+-rw-rw-rw-   0        0        0     4790 2024-04-07 00:11:59.000000 iinfer-0.6.9/iinfer/app/injections/after_http_injection.py
+-rw-rw-rw-   0        0        0     9077 2024-04-11 13:28:27.000000 iinfer-0.6.9/iinfer/app/injections/after_seg_bbox_injection.py
+-rw-rw-rw-   0        0        0     8688 2024-04-11 13:41:09.000000 iinfer-0.6.9/iinfer/app/injections/after_seg_filter_injection.py
+-rw-rw-rw-   0        0        0     1810 2024-02-25 07:58:13.000000 iinfer-0.6.9/iinfer/app/injections/before_grayimg_injection.py
+-rw-rw-rw-   0        0        0    14447 2024-03-23 14:43:05.000000 iinfer-0.6.9/iinfer/app/install.py
+-rw-rw-rw-   0        0        0     4811 2024-03-10 08:54:06.000000 iinfer-0.6.9/iinfer/app/postprocess.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.089592 iinfer-0.6.9/iinfer/app/postprocesses/
+-rw-rw-rw-   0        0        0     1935 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/app/postprocesses/cls_jadge.py
+-rw-rw-rw-   0        0        0     2393 2024-04-06 14:52:31.000000 iinfer-0.6.9/iinfer/app/postprocesses/csv.py
+-rw-rw-rw-   0        0        0     4197 2024-03-10 09:01:15.000000 iinfer-0.6.9/iinfer/app/postprocesses/det_clip.py
+-rw-rw-rw-   0        0        0     5063 2024-03-17 02:51:08.000000 iinfer-0.6.9/iinfer/app/postprocesses/det_face_store.py
+-rw-rw-rw-   0        0        0     4444 2024-04-11 13:48:21.000000 iinfer-0.6.9/iinfer/app/postprocesses/det_filter.py
+-rw-rw-rw-   0        0        0     5201 2024-04-07 07:20:08.000000 iinfer-0.6.9/iinfer/app/postprocesses/det_jadge.py
+-rw-rw-rw-   0        0        0     3813 2024-04-07 00:25:09.000000 iinfer-0.6.9/iinfer/app/postprocesses/httpreq.py
+-rw-rw-rw-   0        0        0     4369 2024-04-11 13:06:06.000000 iinfer-0.6.9/iinfer/app/postprocesses/seg_bbox.py
+-rw-rw-rw-   0        0        0     4252 2024-04-11 12:27:14.000000 iinfer-0.6.9/iinfer/app/postprocesses/seg_filter.py
+-rw-rw-rw-   0        0        0     6077 2024-02-24 13:15:38.000000 iinfer-0.6.9/iinfer/app/predict.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.147601 iinfer-0.6.9/iinfer/app/predicts/
+-rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/app/predicts/__init__.py
+-rw-rw-rw-   0        0        0     7618 2024-03-30 02:49:18.000000 iinfer-0.6.9/iinfer/app/predicts/insightface_det.py
+-rw-rw-rw-   0        0        0     4134 2024-03-30 02:49:30.000000 iinfer-0.6.9/iinfer/app/predicts/mmdet_det_YoloX.py
+-rw-rw-rw-   0        0        0      384 2024-03-30 02:49:24.000000 iinfer-0.6.9/iinfer/app/predicts/mmdet_det_YoloX_Lite.py
+-rw-rw-rw-   0        0        0     4712 2024-03-30 02:49:40.000000 iinfer-0.6.9/iinfer/app/predicts/mmpretrain_cls_swin.py
+-rw-rw-rw-   0        0        0      418 2024-03-30 02:49:36.000000 iinfer-0.6.9/iinfer/app/predicts/mmpretrain_cls_swin_Lite.py
+-rw-rw-rw-   0        0        0    10366 2024-03-30 02:49:45.000000 iinfer-0.6.9/iinfer/app/predicts/mmrotate_det_ReDet.py
+-rw-rw-rw-   0        0        0     5712 2024-04-05 13:16:32.000000 iinfer-0.6.9/iinfer/app/predicts/mmseg_seg_PSPNet.py
+-rw-rw-rw-   0        0        0      386 2024-03-30 02:49:57.000000 iinfer-0.6.9/iinfer/app/predicts/mmseg_seg_SwinUpernet.py
+-rw-rw-rw-   0        0        0     4647 2024-03-30 02:50:02.000000 iinfer-0.6.9/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py
+-rw-rw-rw-   0        0        0     5301 2024-03-30 02:50:07.000000 iinfer-0.6.9/iinfer/app/predicts/onnx_det_TinyYoloV3.py
+-rw-rw-rw-   0        0        0     5509 2024-03-30 02:50:11.000000 iinfer-0.6.9/iinfer/app/predicts/onnx_det_YoloV3.py
+-rw-rw-rw-   0        0        0     9843 2024-03-30 02:50:23.000000 iinfer-0.6.9/iinfer/app/predicts/onnx_det_YoloX.py
+-rw-rw-rw-   0        0        0     2887 2024-03-30 02:50:17.000000 iinfer-0.6.9/iinfer/app/predicts/onnx_det_YoloX_Lite.py
+-rw-rw-rw-   0        0        0     2706 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/app/redis.py
+-rw-rw-rw-   0        0        0    49856 2024-04-15 12:16:57.000000 iinfer-0.6.9/iinfer/app/server.py
+-rw-rw-rw-   0        0        0       54 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/config.yml
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.165604 iinfer-0.6.9/iinfer/datasets/
+-rw-rw-rw-   0        0        0      684 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/datasets/label_coco.txt
+-rw-rw-rw-   0        0        0      153 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/datasets/label_voc.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.195605 iinfer-0.6.9/iinfer/docker/
+-rw-rw-rw-   0        0        0      813 2024-03-11 12:27:01.000000 iinfer-0.6.9/iinfer/docker/Dockerfile
+-rw-rw-rw-   0        0        0        0 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/docker/__init__.py
+-rw-rw-rw-   0        0        0      131 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/docker/build.sh
+-rw-rw-rw-   0        0        0      319 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/docker/docker-compose.yml
+drwxrwxrwx   0        0        0        0 2024-04-15 12:37:59.773558 iinfer-0.6.9/iinfer/extensions/
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.244649 iinfer-0.6.9/iinfer/extensions/injection/
+-rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.6.9/iinfer/extensions/injection/after_cls_jadge_injection.json
+-rw-rw-rw-   0        0        0       99 2024-04-11 14:24:51.000000 iinfer-0.6.9/iinfer/extensions/injection/after_csv_injection.json
+-rw-rw-rw-   0        0        0      129 2024-04-07 04:03:58.000000 iinfer-0.6.9/iinfer/extensions/injection/after_det_filter_injection.json
+-rw-rw-rw-   0        0        0      241 2024-04-07 07:33:42.000000 iinfer-0.6.9/iinfer/extensions/injection/after_det_jadge_injection.json
+-rw-rw-rw-   0        0        0      176 2024-02-25 01:08:47.000000 iinfer-0.6.9/iinfer/extensions/injection/after_http_injection.json
+-rw-rw-rw-   0        0        0      107 2024-04-07 03:43:59.000000 iinfer-0.6.9/iinfer/extensions/injection/after_seg_bbox_injection.json
+-rw-rw-rw-   0        0        0      115 2024-04-07 03:42:37.000000 iinfer-0.6.9/iinfer/extensions/injection/after_seg_filter_injection.json
+-rw-rw-rw-   0        0        0        2 2024-02-18 07:43:45.000000 iinfer-0.6.9/iinfer/extensions/injection/before_gray_injection.json
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.623016 iinfer-0.6.9/iinfer/licenses/
+-rw-rw-rw-   0        0        0     1089 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1121 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt
+-rw-rw-rw-   0        0        0    10351 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt
+-rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.bottle-websocket.0.2.9(MIT License).txt
+-rw-rw-rw-   0        0        0     1080 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt
+-rw-rw-rw-   0        0        0     1009 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt
+-rw-rw-rw-   0        0        0     1320 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1090 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt
+-rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1523 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt
+-rw-rw-rw-   0        0        0     1105 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt
+-rw-rw-rw-   0        0        0     1093 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1094 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt
+-rw-rw-rw-   0        0        0        7 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.gevent-websocket.0.10.1(Copyright 2011-2017 Jeffrey Gelens jeffrey@noppo.pro).txt
+-rw-rw-rw-   0        0        0     1260 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt
+-rw-rw-rw-   0        0        0     1464 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt
+-rw-rw-rw-   0        0        0     1572 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt
+-rw-rw-rw-   0        0        0     1117 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt
+-rw-rw-rw-   0        0        0     3350 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt
+-rw-rw-rw-   0        0        0     4928 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt
+-rw-rw-rw-   0        0        0     1088 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt
+-rw-rw-rw-   0        0        0    48691 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt
+-rw-rw-rw-   0        0        0   154222 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt
+-rw-rw-rw-   0        0        0      200 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.packaging.24.0(Apache Software License; BSD License).txt
+-rw-rw-rw-   0        0        0    56516 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt
+-rw-rw-rw-   0        0        0     1113 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1642 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1563 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt
+-rw-rw-rw-   0        0        0     1041 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt
+-rw-rw-rw-   0        0        0     2942 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt
+-rw-rw-rw-   0        0        0     1095 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt
+-rw-rw-rw-   0        0        0    10317 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt
+-rw-rw-rw-   0        0        0    47742 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt
+-rw-rw-rw-   0        0        0     1040 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1084 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1100 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1114 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt
+-rw-rw-rw-   0        0        0     1349 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt
+-rw-rw-rw-   0        0        0     1128 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt
+-rw-rw-rw-   0        0        0     1495 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt
+-rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt
+-rw-rw-rw-   0        0        0     2114 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt
+-rw-rw-rw-   0        0        0     6545 2024-03-27 11:58:45.000000 iinfer-0.6.9/iinfer/licenses/files.txt
+-rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/logconf_client.yml
+-rw-rw-rw-   0        0        0      630 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/logconf_gui.yml
+-rw-rw-rw-   0        0        0      655 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/logconf_install.yml
+-rw-rw-rw-   0        0        0      669 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/logconf_postprocess.yml
+-rw-rw-rw-   0        0        0      645 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/logconf_redis.yml
+-rw-rw-rw-   0        0        0      650 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/logconf_server.yml
+-rw-rw-rw-   0        0        0     1010 2024-04-15 11:45:35.000000 iinfer-0.6.9/iinfer/version.py
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.628022 iinfer-0.6.9/iinfer/web/
+drwxrwxrwx   0        0        0        0 2024-04-15 12:37:59.807561 iinfer-0.6.9/iinfer/web/assets/
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.667266 iinfer-0.6.9/iinfer/web/assets/bootstrap/
+-rw-rw-rw-   0        0        0    78749 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js
+-rw-rw-rw-   0        0        0    80421 2024-02-18 08:27:56.000000 iinfer-0.6.9/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js
+-rw-rw-rw-   0        0        0   155851 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css
+-rw-rw-rw-   0        0        0   232914 2024-02-18 08:28:29.000000 iinfer-0.6.9/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.736272 iinfer-0.6.9/iinfer/web/assets/iinfer/
+-rw-rw-rw-   0        0        0     5664 2024-04-12 12:02:38.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/filer_modal.js
+-rw-rw-rw-   0        0        0    16712 2024-04-12 12:00:35.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/list_cmd.js
+-rw-rw-rw-   0        0        0     6560 2024-04-12 12:12:27.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/list_pipe.js
+-rw-rw-rw-   0        0        0     4447 2024-04-12 12:12:53.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/main.js
+-rw-rw-rw-   0        0        0      439 2024-04-12 12:08:33.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/open_capture.js
+-rw-rw-rw-   0        0        0      459 2024-04-12 12:07:28.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/open_output_json.js
+-rw-rw-rw-   0        0        0      122 2024-03-03 02:33:47.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/svfiler.css
+-rw-rw-rw-   0        0        0    24743 2024-04-15 12:24:01.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/svfiler.js
+-rw-rw-rw-   0        0        0     1079 2024-04-12 12:06:23.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/view_raw.js
+-rw-rw-rw-   0        0        0     4543 2024-04-12 12:04:28.000000 iinfer-0.6.9/iinfer/web/assets/iinfer/view_result.js
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.739270 iinfer-0.6.9/iinfer/web/assets/jquery/
+-rw-rw-rw-   0        0        0    86600 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery/jquery.min.3.2.0.js
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.744273 iinfer-0.6.9/iinfer/web/assets/jquery-resizable/
+-rw-rw-rw-   0        0        0     3448 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.795280 iinfer-0.6.9/iinfer/web/assets/jquery-ui/
+-rw-rw-rw-   0        0        0    14615 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/AUTHORS.txt
+-rw-rw-rw-   0        0        0     1860 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.866286 iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/
+-rw-rw-rw-   0        0        0     7142 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png
+-rw-rw-rw-   0        0        0     7126 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png
+-rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png
+-rw-rw-rw-   0        0        0     7163 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png
+-rw-rw-rw-   0        0        0     4670 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png
+-rw-rw-rw-   0        0        0     6539 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png
+-rw-rw-rw-   0        0        0    32136 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/jquery-ui.min.css
+-rw-rw-rw-   0        0        0   255089 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/jquery-ui.min.js
+-rw-rw-rw-   0        0        0    15564 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css
+-rw-rw-rw-   0        0        0    13895 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css
+-rw-rw-rw-   0        0        0     1886 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/jquery-ui/package.json
+drwxrwxrwx   0        0        0        0 2024-04-15 12:37:59.806563 iinfer-0.6.9/iinfer/web/assets/lightbox2/
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.872286 iinfer-0.6.9/iinfer/web/assets/lightbox2/css/
+-rw-rw-rw-   0        0        0     2532 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/lightbox2/css/lightbox.min.css
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.903292 iinfer-0.6.9/iinfer/web/assets/lightbox2/images/
+-rw-rw-rw-   0        0        0      280 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/lightbox2/images/close.png
+-rw-rw-rw-   0        0        0     8476 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/lightbox2/images/loading.gif
+-rw-rw-rw-   0        0        0     1350 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/lightbox2/images/next.png
+-rw-rw-rw-   0        0        0     1360 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/lightbox2/images/prev.png
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.907292 iinfer-0.6.9/iinfer/web/assets/lightbox2/js/
+-rw-rw-rw-   0        0        0     9768 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/lightbox2/js/lightbox.min.js
+drwxrwxrwx   0        0        0        0 2024-04-15 12:37:59.808561 iinfer-0.6.9/iinfer/web/assets/tree-menu/
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.911289 iinfer-0.6.9/iinfer/web/assets/tree-menu/css/
+-rw-rw-rw-   0        0        0     1101 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/tree-menu/css/tree-menu.css
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.936295 iinfer-0.6.9/iinfer/web/assets/tree-menu/image/
+-rw-rw-rw-   0        0        0      248 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/tree-menu/image/file.png
+-rw-rw-rw-   0        0        0      284 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/tree-menu/image/folder-close.png
+-rw-rw-rw-   0        0        0      301 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/tree-menu/image/folder-open.png
+drwxrwxrwx   0        0        0        0 2024-04-15 12:38:00.940295 iinfer-0.6.9/iinfer/web/assets/tree-menu/js/
+-rw-rw-rw-   0        0        0     1029 2024-02-15 15:34:05.000000 iinfer-0.6.9/iinfer/web/assets/tree-menu/js/tree-menu.js
+-rw-rw-rw-   0        0        0    30911 2024-04-13 04:36:58.000000 iinfer-0.6.9/iinfer/web/main.html
+drwxrwxrwx   0        0        0        0 2024-04-15 12:37:59.894571 iinfer-0.6.9/iinfer.egg-info/
+-rw-rw-rw-   0        0        0     5553 2024-04-15 12:37:59.000000 iinfer-0.6.9/iinfer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7259 2024-04-15 12:37:59.000000 iinfer-0.6.9/iinfer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 12:37:59.000000 iinfer-0.6.9/iinfer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-04-15 12:37:59.000000 iinfer-0.6.9/iinfer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2024-04-15 12:37:59.000000 iinfer-0.6.9/iinfer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-15 12:37:59.000000 iinfer-0.6.9/iinfer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 12:38:00.944293 iinfer-0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0     2185 2024-04-06 23:22:57.000000 iinfer-0.6.9/setup.py
```

### Comparing `iinfer-0.6.8/LICENSE` & `iinfer-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/PKG-INFO` & `iinfer-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iinfer
-Version: 0.6.8
+Version: 0.6.9
 Summary: iinfer: An application that executes AI model files in onnx or mmlab format.
 Home-page: https://github.com/hamacom2004jp/iinfer
 Author: hamacom2004jp
 Author-email: hamacom2004jp@gmail.com
 Maintainer: hamacom2004jp
 Maintainer-email: hamacom2004jp@gmail.com
 License: MIT
```

### Comparing `iinfer-0.6.8/README.md` & `iinfer-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/app.py` & `iinfer-0.6.9/iinfer/app/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     parser.add_argument('--timeout', help='Setting the cmd timeout.', type=int, default=60)
     parser.add_argument('-c', '--cmd', help='Setting the cmd type.',
                         choices=['redis', 'server', 'onnx', 'mmdet', 'mmseg', 'mmcls', 'mmpretrain', 'insightface', # install mode
                                  'docker_run', 'docker_stop', # redis mode
                                  'start', 'stop', # server or client or gui mode
                                  'list' , # server mode
                                  'deploy', 'deploy_list', 'undeploy', 'predict', 'predict_type_list', 'capture', # client mode
+                                 'file_list', 'file_mkdir', 'file_rmdir', 'file_download', 'file_upload', 'file_remove', # client mode
                                  'cls_jadge', 'csv', 'det_clip', 'det_face_store', 'det_filter', 'det_jadge', 'httpreq', 'seg_bbox', 'seg_filter', # postprocess mode
                                 ])
     parser.add_argument('-T','--use_track', help='Setting the multi object tracking enable for Object Detection.', action='store_true')
     parser.add_argument('--model_img_width', help='Setting the cmd deploy model_img_width.', type=int)
     parser.add_argument('--model_img_height', help='Setting the cmd deploy model_img_height.', type=int)
     parser.add_argument('--model_file', help='Setting the cmd deploy model_file file.')
     parser.add_argument('--model_conf_file', help='Setting the cmd deploy model_conf_file file.', action='append')
@@ -73,14 +74,18 @@
     parser.add_argument('--wsl_user', help='WSL distribution user.')
     parser.add_argument('-d', '--capture_device', help='Setting the capture input device. device id, video file, rtsp url.', default='0')
     parser.add_argument('--capture_frame_width', help='Setting the capture input frame width.', type=int, default=None)
     parser.add_argument('--capture_frame_height', help='Setting the capture input frame height.', type=int, default=None)
     parser.add_argument('--capture_fps', help='Setting the capture input fps.', type=int, default=1000)
     parser.add_argument('--capture_count', help='Setting the capture count.', type=int, default=-1)
 
+    parser.add_argument('--svpath', help='Setting the server file path.', type=str, default='/')
+    parser.add_argument('--download_file', help='Setting the download file path.', type=str, default=None)
+    parser.add_argument('--upload_file', help='Setting the upload file path.', type=str, default=None)
+
     parser.add_argument('--fileup_name', help='Setting the param name of file upload.', type=str, default='file')
     parser.add_argument('--img_connectstr', help='Setting the postprocess img_connectstr.', type=str, default=None)
     parser.add_argument('--json_connectstr', help='Setting the postprocess json_connectstr.', type=str, default=None)
     parser.add_argument('--text_connectstr', help='Setting the postprocess text_connectstr.', type=str, default=None)
 
     parser.add_argument('--out_headers', help='Setting the csv cmd out_headers in postprocess.', type=str, action='append')
     parser.add_argument('--noheader', help='Setting the csv cmd noheader in postprocess.', action='store_true')
@@ -170,14 +175,18 @@
 
     capture_device = common.getopt(opt, 'capture_device', preval=args_dict, withset=True)
     capture_frame_width = common.getopt(opt, 'capture_frame_width', preval=args_dict, withset=True)
     capture_frame_height = common.getopt(opt, 'capture_frame_height', preval=args_dict, withset=True)
     capture_fps = common.getopt(opt, 'capture_fps', preval=args_dict, withset=True)
     capture_count = common.getopt(opt, 'capture_count', preval=args_dict, withset=True)
 
+    svpath = common.getopt(opt, 'svpath', preval=args_dict, withset=True)
+    download_file = common.getopt(opt, 'download_file', preval=args_dict, withset=True)
+    upload_file = common.getopt(opt, 'upload_file', preval=args_dict, withset=True)
+
     json_connectstr = common.getopt(opt, 'json_connectstr', preval=args_dict, withset=True)
     img_connectstr = common.getopt(opt, 'img_connectstr', preval=args_dict, withset=True)
     text_connectstr = common.getopt(opt, 'text_connectstr', preval=args_dict, withset=True)
     fileup_name = common.getopt(opt, 'fileup_name', preval=args_dict, withset=True)
 
     out_headers = common.getopt(opt, 'out_headers', preval=args_dict, withset=True)
     noheader = common.getopt(opt, 'noheader', preval=args_dict, withset=True)
@@ -367,14 +376,53 @@
                     common.print_format(msg, format, tm, output_json, output_json_append)
                     return 1, msg
             finally:
                 try:
                     cv2.destroyWindow('preview')
                 except:
                     pass
+
+        elif cmd == 'file_list':
+            ret = cl.file_list(svpath, timeout=timeout)
+            common.print_format(ret, format, tm, output_json, output_json_append)
+            if 'success' not in ret:
+                return 1, ret
+        
+        elif cmd == 'file_mkdir':
+            ret = cl.file_mkdir(svpath, timeout=timeout)
+            common.print_format(ret, format, tm, output_json, output_json_append)
+            if 'success' not in ret:
+                return 1, ret
+        
+        elif cmd == 'file_rmdir':
+            ret = cl.file_rmdir(svpath, timeout=timeout)
+            common.print_format(ret, format, tm, output_json, output_json_append)
+            if 'success' not in ret:
+                return 1, ret
+        
+        elif cmd == 'file_download':
+            download_file = Path(download_file) if download_file is not None else None
+            ret = cl.file_download(svpath, download_file, timeout=timeout)
+            common.print_format(ret, format, tm, output_json, output_json_append)
+            if 'success' not in ret:
+                return 1, ret
+        
+        elif cmd == 'file_upload':
+            upload_file = Path(upload_file) if upload_file is not None else None
+            ret = cl.file_upload(svpath, upload_file, timeout=timeout)
+            common.print_format(ret, format, tm, output_json, output_json_append)
+            if 'success' not in ret:
+                return 1, ret
+
+        elif cmd == 'file_remove':
+            ret = cl.file_remove(svpath, timeout=timeout)
+            common.print_format(ret, format, tm, output_json, output_json_append)
+            if 'success' not in ret:
+                return 1, ret
+
         elif cmd == 'predict_type_list':
             type_list = [dict(predict_type=key, site=val['site'], image_width=val['image_width'], image_height=val['image_height'],
                               required_model_conf=val['required_model_conf'], required_model_weight=val['required_model_weight']) for key,val in common.BASE_MODELS.items()]
             type_list.append(dict(predict_type='Custom', site='Custom', image_width=None, image_height=None))
             ret = type_list
             common.print_format(ret, format, tm, output_json, output_json_append)
```

### Comparing `iinfer-0.6.8/iinfer/app/client.py` & `iinfer-0.6.9/iinfer/app/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -438,14 +438,121 @@
                 # RGB画像をBGR画像に変換
                 try:
                     cv2.imshow('preview', convert.bgr2rgb(img_npy))
                     cv2.waitKey(1)
                 except KeyboardInterrupt:
                     pass
         return res_json
+    
+    def file_list(self, svpath:str, timeout:int = 60):
+        """
+        サーバー上のファイルリストを取得する
+
+        Args:
+            svpath (Path): サーバー上のファイルパス
+            timeout (int, optional): タイムアウト時間. Defaults to 60.
+
+        Returns:
+            dict: Redisサーバーからの応答
+        """
+        res_json = self._proc(self.svname, 'file_list', [str(svpath)], timeout=timeout)
+        return res_json
+
+    def file_mkdir(self, svpath:str, timeout:int = 60):
+        """
+        サーバー上にディレクトリを作成する
+
+        Args:
+            svpath (Path): サーバー上のディレクトリパス
+            timeout (int, optional): タイムアウト時間. Defaults to 60.
+
+        Returns:
+            dict: Redisサーバーからの応答
+        """
+        res_json = self._proc(self.svname, 'file_mkdir', [str(svpath)], timeout=timeout)
+        return res_json
+    
+    def file_rmdir(self, svpath:str, timeout:int = 60):
+        """
+        サーバー上のディレクトリを削除する
+
+        Args:
+            svpath (Path): サーバー上のディレクトリパス
+            timeout (int, optional): タイムアウト時間. Defaults to 60.
+
+        Returns:
+            dict: Redisサーバーからの応答
+        """
+        res_json = self._proc(self.svname, 'file_rmdir', [str(svpath)], timeout=timeout)
+        return res_json
+    
+    def file_download(self, svpath:str, download_file:Path, timeout:int = 60):
+        """
+        サーバー上のファイルをダウンロードする
+
+        Args:
+            svpath (Path): サーバー上のファイルパス
+            download_file (Path): ローカルのファイルパス
+            timeout (int, optional): タイムアウト時間. Defaults to 60.
+
+        Returns:
+            bytes: ダウンロードファイルの内容
+        """
+        res_json = self._proc(self.svname, 'file_download', [str(svpath)], timeout=timeout)
+        if "success" in res_json:
+            if download_file is not None:
+                if download_file.is_dir():
+                    download_file = download_file / res_json["success"]["name"]
+                if download_file.exists():
+                    self.logger.error(f"download_file {download_file} already exists.")
+                    return {"error": f"download_file {download_file} already exists."}
+                with open(download_file, "wb") as f:
+                    f.write(base64.b64decode(res_json["success"]["data"]))
+                    del res_json["success"]["data"]
+                    res_json["success"]["download_file"] = str(download_file.absolute())
+        return res_json
+    
+    def file_upload(self, svpath:str, upload_file:Path, timeout:int = 60):
+        """
+        サーバー上にファイルをアップロードする
+
+        Args:
+            svpath (Path): サーバー上のファイルパス
+            upload_file (Path): ローカルのファイルパス
+            timeout (int, optional): タイムアウト時間. Defaults to 60.
+
+        Returns:
+            dict: Redisサーバーからの応答
+        """
+        if upload_file is None:
+            self.logger.error(f"upload_file is empty.")
+            return {"error": f"upload_file is empty."}
+        if not upload_file.exists():
+            self.logger.error(f"input_file {upload_file} does not exist.")
+            return {"error": f"input_file {upload_file} does not exist."}
+        if upload_file.is_dir():
+            self.logger.error(f"input_file {upload_file} is directory.")
+            return {"error": f"input_file {upload_file} is directory."}
+        with open(upload_file, "rb") as f:
+            res_json = self._proc(self.svname, 'file_upload', [str(svpath), upload_file.name, base64.b64encode(f.read()).decode('utf-8')], timeout=timeout)
+            return res_json
+
+    def file_remove(self, svpath:str, timeout:int = 60):
+        """
+        サーバー上のファイルを削除する
+
+        Args:
+            svpath (Path): サーバー上のファイルパス
+            timeout (int, optional): タイムアウト時間. Defaults to 60.
+
+        Returns:
+            dict: Redisサーバーからの応答
+        """
+        res_json = self._proc(self.svname, 'file_remove', [str(svpath)], timeout=timeout)
+        return res_json
 
     def capture(self, capture_device='0', image_type:str='capture', capture_frame_width:int=None, capture_frame_height:int=None, capture_fps:int=1000, output_preview:bool=False):
         """
         ビデオをキャプチャしてその結果を出力する
 
         Args:
             capture_device (int or str): キャプチャするディバイス、ビデオデバイスのID, ビデオファイルのパス。rtspのURL. by default 0
```

### Comparing `iinfer-0.6.8/iinfer/app/common.py` & `iinfer-0.6.9/iinfer/app/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pathlib import Path
 from PIL import Image, ImageDraw
 from pkg_resources import resource_string
 from tabulate import tabulate
 from typing import List, Tuple, Dict, Any
 import cv2
+import datetime
 import logging
 import logging.config
 import json
 import numpy as np
 import os
 import platform
 import random
@@ -49,14 +50,16 @@
         return int(o)
     if isinstance(o, np.int32):
         return int(o)
     if isinstance(o, np.intc):
         return int(o)
     if isinstance(o, Path):
         return str(o)
+    if isinstance(o, datetime.datetime):
+        return o.strftime('%Y-%m-%dT%H:%M:%S')
     raise TypeError(f"Type {type(o)} not serializable")
 
 def saveopt(opt:dict, opt_path:Path) -> None:
     """
     コマンドラインオプションをJSON形式でファイルに保存します。
 
     Args:
```

### Comparing `iinfer-0.6.8/iinfer/app/commons/convert.py` & `iinfer-0.6.9/iinfer/app/commons/convert.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/commons/module.py` & `iinfer-0.6.9/iinfer/app/commons/module.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/gui.py` & `iinfer-0.6.9/iinfer/app/gui.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from iinfer import version
 from iinfer.app import app, common
 from iinfer.app.commons import convert
 from pathlib import Path
+import bottle
 import datetime
 import glob
 import html
 import iinfer
 import io
 import json
 import logging
 import os
 import re
 import sys
 import traceback
+import tempfile
 
 
 class Web(object):
     def __init__(self, logger:logging.Logger, data:Path):
         import eel
         eel.init(str(Path(iinfer.__file__).parent / "web"))
         self.logger = logger
@@ -30,15 +32,15 @@
         @eel.expose
         def get_mode_opt():
             return ['', 'client', 'postprocess', 'server', 'redis', 'install']
 
         @eel.expose
         def get_cmd_opt(mode):
             if mode == "client":
-                return ['', 'deploy', 'start', 'stop', 'predict', 'deploy_list', 'undeploy', 'predict_type_list', 'capture']
+                return ['', 'deploy', 'start', 'stop', 'predict', 'deploy_list', 'undeploy', 'predict_type_list', 'capture', 'file_list', 'file_mkdir', 'file_rmdir', 'file_download', 'file_upload', 'file_remove',]
             elif mode == "server":
                 return ['', 'start', 'stop', 'list']
             elif mode == "postprocess":
                 return ['', 'cls_jadge', 'csv', 'det_clip', 'det_face_store', 'det_filter', 'det_jadge', 'httpreq', 'seg_bbox', 'seg_filter']
             elif mode == "redis":
                 return ['', 'docker_run', 'docker_stop']
             elif mode == "install":
@@ -147,14 +149,88 @@
                         dict(opt="output_image", type="file", default="", required=False, multi=False, hide=False, choise=None),
                         dict(opt="output_preview", type="bool", default=False, required=False, multi=False, hide=False, choise=[True, False]),
                         dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None),
                         dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None),
                         dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
                         dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False])
                     ]
+                elif cmd == "file_list":
+                    return [
+                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None),
+                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None),
+                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None),
+                        dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None),
+                        dict(opt="svpath", type="str", default="/", required=True, multi=False, hide=False, choise=None),
+                        dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None),
+                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None),
+                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
+                        dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False])
+                    ]
+                elif cmd == "file_mkdir":
+                    return [
+                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None),
+                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None),
+                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None),
+                        dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None),
+                        dict(opt="svpath", type="str", default="/", required=True, multi=False, hide=False, choise=None),
+                        dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None),
+                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None),
+                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
+                        dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False])
+                    ]
+                elif cmd == "file_rmdir":
+                    return [
+                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None),
+                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None),
+                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None),
+                        dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None),
+                        dict(opt="svpath", type="str", default="/", required=True, multi=False, hide=False, choise=None),
+                        dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None),
+                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None),
+                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
+                        dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False])
+                    ]
+                elif cmd == "file_download":
+                    return [
+                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None),
+                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None),
+                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None),
+                        dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None),
+                        dict(opt="svpath", type="str", default="/", required=True, multi=False, hide=False, choise=None),
+                        dict(opt="download_file", type="file", default="", required=False, multi=False, hide=False, choise=None),
+                        dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None),
+                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None),
+                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
+                        dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False])
+                    ]
+                elif cmd == "file_upload":
+                    return [
+                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None),
+                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None),
+                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None),
+                        dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None),
+                        dict(opt="svpath", type="str", default="/", required=True, multi=False, hide=False, choise=None),
+                        dict(opt="upload_file", type="file", default="", required=True, multi=False, hide=False, choise=None),
+                        dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None),
+                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None),
+                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
+                        dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False])
+                    ]
+                elif cmd == "file_remove":
+                    return [
+                        dict(opt="host", type="str", default="localhost", required=True, multi=False, hide=True, choise=None),
+                        dict(opt="port", type="int", default=6379, required=True, multi=False, hide=True, choise=None),
+                        dict(opt="password", type="str", default="password", required=True, multi=False, hide=True, choise=None),
+                        dict(opt="svname", type="str", default="server", required=True, multi=False, hide=True, choise=None),
+                        dict(opt="svpath", type="str", default="/", required=True, multi=False, hide=False, choise=None),
+                        dict(opt="timeout", type="int", default="15", required=False, multi=False, hide=True, choise=None),
+                        dict(opt="output_json", type="file", default="", required=False, multi=False, hide=True, choise=None),
+                        dict(opt="output_json_append", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False]),
+                        dict(opt="stdout_log", type="bool", default=False, required=False, multi=False, hide=True, choise=[True, False])
+                    ]
                 elif cmd == "capture":
                     return [
                         dict(opt="capture_device", type="str", default="0", required=True, multi=False, hide=True, choise=None),
                         dict(opt="image_type", type="str", default="capture", required=True, multi=False, hide=False, choise=['bmp', 'png', 'jpeg', 'capture']),
                         dict(opt="capture_frame_width", type="int", default=640, required=False, multi=False, hide=True, choise=None),
                         dict(opt="capture_frame_height", type="int", default=480, required=False, multi=False, hide=True, choise=None),
                         dict(opt="capture_fps", type="int", default=5, required=False, multi=False, hide=True, choise=None),
@@ -419,15 +495,15 @@
 
         @eel.expose
         def del_cmd(title):
             opt_path = self.data / f"cmd-{title}.json"
             self.logger.info(f"del_cmd: opt_path={opt_path}")
             opt_path.unlink()
 
-        def mk_opt_list(opt):
+        def mk_opt_list(opt:dict):
             opt_schema = get_opt_opt(opt['mode'], opt['cmd'])
             opt_list = ['-m', opt['mode'], '-c', opt['cmd']]
             for key, val in opt.items():
                 if key in ['stdout_log']:
                     continue
                 schema = [schema for schema in opt_schema if schema['opt'] == key]
                 if len(schema) == 0 or val == '':
@@ -472,36 +548,14 @@
                 try:
                     ret = [to_json(o) for o in output.split('\n') if o.strip() != '']
                 except:
                     ret = to_json(output)
                 return ret
             except:
                 return output
-            """
-            captured_output = io.StringIO()
-            def main_call(opt_list, captured_output):
-                old_stdout = sys.stdout
-                sys.stdout = captured_output
-                app.main(opt_list)
-                sys.stdout = old_stdout
-            th = threading.Thread(target=main_call, args=(opt_list, captured_output))
-            th.start()
-
-            output = ''
-            while th.is_alive():
-                line = captured_output.getvalue()
-                if line.strip() == '':
-                    continue
-                output += line
-                eel.js_console_modal_log_func(line)
-            try:
-                return json.loads(output)
-            except:
-                return output
-            """
 
         @eel.expose
         def raw_cmd(title, opt):
             self.logger.info(f"raw_cmd: title={title}, opt={opt}")
             opt_list = mk_opt_list(opt)
             return [dict(type='cmdline',raw=' '.join(['iinfer']+opt_list)),
                     dict(type='optjson',raw=json.dumps(opt, default=common.default_json_enc))]
@@ -625,14 +679,34 @@
         def versions_used():
             with open(Path(iinfer.__file__).parent / 'licenses' / 'files.txt', 'r', encoding='utf-8') as f:
                 ret = []
                 for i, line in enumerate(f.readlines()):
                     parts = line.strip().split('\t')
                     ret.append(parts)
             return ret
+        
+        @bottle.route('/filer/upload', method='POST')
+        def filer_upload():
+            q = bottle.request.query
+            svpath = q['svpath']
+            opt = dict(mode='client', cmd='file_upload',
+                       host=q['host'], port=q['port'], password=q['password'], svname=q['svname'])
+            for file in bottle.request.files.getall('files'):
+                with tempfile.TemporaryDirectory() as tmpdir:
+                    upload_file:Path = Path(tmpdir) / file.raw_filename
+                    if not upload_file.parent.exists():
+                        upload_file.parent.mkdir(parents=True)
+                    opt['svpath'] = str(svpath / Path(file.raw_filename).parent).replace('\\','/')
+                    opt['upload_file'] = str(upload_file)
+                    file.save(opt['upload_file'])
+                    ret = exec_cmd("file_upload", opt)
+                    if len(ret) == 0 or 'success' not in ret[0]:
+                        return str(ret)
+            return 'upload success'
+            #return f'upload {upload.filename}'
 
         eel.js_console_modal_log_func('== console log start ==\n')
         eel.start("main.html", size=(width, height), block=True, port=web_port, host=web_host, close_callback=self.stop)
 
     def stop(self, route, websockets):
         self.logger.info(f"Stop eel web. {route}")
         exit(0)
```

### Comparing `iinfer-0.6.8/iinfer/app/injection.py` & `iinfer-0.6.9/iinfer/app/injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/injections/after_cls_jadge_injection.py` & `iinfer-0.6.9/iinfer/app/injections/after_cls_jadge_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/injections/after_csv_injection.py` & `iinfer-0.6.9/iinfer/app/injections/after_csv_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/injections/after_det_filter_injection.py` & `iinfer-0.6.9/iinfer/app/injections/after_det_filter_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/injections/after_det_jadge_injection.py` & `iinfer-0.6.9/iinfer/app/injections/after_det_jadge_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/injections/after_http_injection.py` & `iinfer-0.6.9/iinfer/app/injections/after_http_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/injections/after_seg_bbox_injection.py` & `iinfer-0.6.9/iinfer/app/injections/after_seg_bbox_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/injections/after_seg_filter_injection.py` & `iinfer-0.6.9/iinfer/app/injections/after_seg_filter_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/injections/before_grayimg_injection.py` & `iinfer-0.6.9/iinfer/app/injections/before_grayimg_injection.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/install.py` & `iinfer-0.6.9/iinfer/app/install.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/postprocess.py` & `iinfer-0.6.9/iinfer/app/postprocess.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/postprocesses/cls_jadge.py` & `iinfer-0.6.9/iinfer/app/postprocesses/cls_jadge.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/postprocesses/csv.py` & `iinfer-0.6.9/iinfer/app/postprocesses/csv.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/postprocesses/det_clip.py` & `iinfer-0.6.9/iinfer/app/postprocesses/det_clip.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/postprocesses/det_face_store.py` & `iinfer-0.6.9/iinfer/app/postprocesses/det_face_store.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/postprocesses/det_filter.py` & `iinfer-0.6.9/iinfer/app/postprocesses/det_filter.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/postprocesses/det_jadge.py` & `iinfer-0.6.9/iinfer/app/postprocesses/det_jadge.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/postprocesses/httpreq.py` & `iinfer-0.6.9/iinfer/app/postprocesses/httpreq.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/postprocesses/seg_bbox.py` & `iinfer-0.6.9/iinfer/app/postprocesses/seg_bbox.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/postprocesses/seg_filter.py` & `iinfer-0.6.9/iinfer/app/postprocesses/seg_filter.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/predict.py` & `iinfer-0.6.9/iinfer/app/predict.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/predicts/insightface_det.py` & `iinfer-0.6.9/iinfer/app/predicts/insightface_det.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/predicts/mmdet_det_YoloX.py` & `iinfer-0.6.9/iinfer/app/predicts/mmdet_det_YoloX.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/predicts/mmpretrain_cls_swin.py` & `iinfer-0.6.9/iinfer/app/predicts/mmpretrain_cls_swin.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/predicts/mmrotate_det_ReDet.py` & `iinfer-0.6.9/iinfer/app/predicts/mmrotate_det_ReDet.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/predicts/mmseg_seg_PSPNet.py` & `iinfer-0.6.9/iinfer/app/predicts/mmseg_seg_PSPNet.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py` & `iinfer-0.6.9/iinfer/app/predicts/onnx_cls_EfficientNet_Lite4.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/predicts/onnx_det_TinyYoloV3.py` & `iinfer-0.6.9/iinfer/app/predicts/onnx_det_TinyYoloV3.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/predicts/onnx_det_YoloV3.py` & `iinfer-0.6.9/iinfer/app/predicts/onnx_det_YoloV3.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/predicts/onnx_det_YoloX.py` & `iinfer-0.6.9/iinfer/app/predicts/onnx_det_YoloX.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/predicts/onnx_det_YoloX_Lite.py` & `iinfer-0.6.9/iinfer/app/predicts/onnx_det_YoloX_Lite.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/app/redis.py` & `iinfer-0.6.9/iinfer/app/redis.py`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/datasets/label_coco.txt` & `iinfer-0.6.9/iinfer/datasets/label_coco.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/docker/Dockerfile` & `iinfer-0.6.9/iinfer/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.Eel.0.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.PyYAML.6.0.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.argcomplete.3.2.3(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.bottle.0.12.25(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.certifi.2024.2.2(Mozilla Public License 2.0 (MPL 2.0)).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.cffi.1.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.charset-normalizer.3.3.2(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.contourpy.1.2.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.cycler.0.12.1(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.filterpy.1.4.5(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.fonttools.4.50.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.future.1.0.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.gevent.24.2.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.greenlet.3.0.3(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.idna.3.6(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.iinfer.0.6.6(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.kiwisolver.1.4.5(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.matplotlib.3.8.3(Python Software Foundation License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.motpy.0.0.10(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.numpy.1.26.4(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.opencv-python.4.9.0.80(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.pillow.10.2.0(Historical Permission Notice and Disclaimer (HPND)).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.pip.24.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.prettytable.3.10.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.pycparser.2.21(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.pyparsing.3.1.2(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.python-dateutil.2.9.0.post0(Apache Software License; BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.redis.5.0.3(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.requests.2.31.0(Apache Software License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.scipy.1.12.0(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.setuptools.69.2.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.six.1.16.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.tabulate.0.9.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.urllib3.2.2.1(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.wcwidth.0.2.13(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.wheel.0.43.0(MIT License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.whichcraft.0.6.1(BSD License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.zope.event.5.0(Zope Public License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt` & `iinfer-0.6.9/iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/licenses/files.txt` & `iinfer-0.6.9/iinfer/licenses/files.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/logconf_client.yml` & `iinfer-0.6.9/iinfer/logconf_client.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/logconf_gui.yml` & `iinfer-0.6.9/iinfer/logconf_gui.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/logconf_install.yml` & `iinfer-0.6.9/iinfer/logconf_install.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/logconf_postprocess.yml` & `iinfer-0.6.9/iinfer/logconf_postprocess.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/logconf_redis.yml` & `iinfer-0.6.9/iinfer/logconf_redis.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/logconf_server.yml` & `iinfer-0.6.9/iinfer/logconf_server.yml`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/version.py` & `iinfer-0.6.9/iinfer/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 
 
-dt_now = datetime.datetime(2024, 4, 11)
+dt_now = datetime.datetime(2024, 4, 15)
 __title__ = 'iinfer (Image Inference Application)'
-__version__ = '0.6.8'
+__version__ = '0.6.9'
 __copyright__ = f'Copyright © 2023-{dt_now.strftime("%Y")} hamacom2004jp'
 __pypiurl__ = 'https://pypi.org/project/iinfer/'
 __srcurl__ = 'https://github.com/hamacom2004jp/iinfer'
 __docurl__ = 'https://hamacom2004jp.github.io/iinfer/index.html'
 __description__ = f'{__title__} {__version__}\n' + \
                   f'{__copyright__}\n' + \
                   f'Web Site: PyPi <{__pypiurl__}>\n' + \
```

### Comparing `iinfer-0.6.8/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js` & `iinfer-0.6.9/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js` & `iinfer-0.6.9/iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css` & `iinfer-0.6.9/iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css` & `iinfer-0.6.9/iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/jquery/jquery.min.3.2.0.js` & `iinfer-0.6.9/iinfer/web/assets/jquery/jquery.min.3.2.0.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js` & `iinfer-0.6.9/iinfer/web/assets/jquery-resizable/jquery-resizable.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/jquery-ui/AUTHORS.txt` & `iinfer-0.6.9/iinfer/web/assets/jquery-ui/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/jquery-ui/LICENSE.txt` & `iinfer-0.6.9/iinfer/web/assets/jquery-ui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png` & `iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png` & `iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png` & `iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png` & `iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png` & `iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png` & `iinfer-0.6.9/iinfer/web/assets/jquery-ui/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/jquery-ui/jquery-ui.min.css` & `iinfer-0.6.9/iinfer/web/assets/jquery-ui/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/jquery-ui/jquery-ui.min.js` & `iinfer-0.6.9/iinfer/web/assets/jquery-ui/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css` & `iinfer-0.6.9/iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css` & `iinfer-0.6.9/iinfer/web/assets/jquery-ui/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/jquery-ui/package.json` & `iinfer-0.6.9/iinfer/web/assets/jquery-ui/package.json`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/lightbox2/css/lightbox.min.css` & `iinfer-0.6.9/iinfer/web/assets/lightbox2/css/lightbox.min.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/lightbox2/images/loading.gif` & `iinfer-0.6.9/iinfer/web/assets/lightbox2/images/loading.gif`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/lightbox2/images/next.png` & `iinfer-0.6.9/iinfer/web/assets/lightbox2/images/next.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/lightbox2/images/prev.png` & `iinfer-0.6.9/iinfer/web/assets/lightbox2/images/prev.png`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/lightbox2/js/lightbox.min.js` & `iinfer-0.6.9/iinfer/web/assets/lightbox2/js/lightbox.min.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/tree-menu/css/tree-menu.css` & `iinfer-0.6.9/iinfer/web/assets/tree-menu/css/tree-menu.css`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer/web/assets/tree-menu/js/tree-menu.js` & `iinfer-0.6.9/iinfer/web/assets/tree-menu/js/tree-menu.js`

 * *Files identical despite different names*

### Comparing `iinfer-0.6.8/iinfer.egg-info/PKG-INFO` & `iinfer-0.6.9/iinfer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iinfer
-Version: 0.6.8
+Version: 0.6.9
 Summary: iinfer: An application that executes AI model files in onnx or mmlab format.
 Home-page: https://github.com/hamacom2004jp/iinfer
 Author: hamacom2004jp
 Author-email: hamacom2004jp@gmail.com
 Maintainer: hamacom2004jp
 Maintainer-email: hamacom2004jp@gmail.com
 License: MIT
```

### Comparing `iinfer-0.6.8/iinfer.egg-info/SOURCES.txt` & `iinfer-0.6.9/iinfer.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -119,14 +119,24 @@
 iinfer/licenses/LICENSE.zope.interface.6.2(Zope Public License).txt
 iinfer/licenses/files.txt
 iinfer/web/main.html
 iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.0.2.js
 iinfer/web/assets/bootstrap/bootstrap.bundle.min.5.3.0.js
 iinfer/web/assets/bootstrap/bootstrap.min.5.0.2.css
 iinfer/web/assets/bootstrap/bootstrap.min.5.3.0.css
+iinfer/web/assets/iinfer/filer_modal.js
+iinfer/web/assets/iinfer/list_cmd.js
+iinfer/web/assets/iinfer/list_pipe.js
+iinfer/web/assets/iinfer/main.js
+iinfer/web/assets/iinfer/open_capture.js
+iinfer/web/assets/iinfer/open_output_json.js
+iinfer/web/assets/iinfer/svfiler.css
+iinfer/web/assets/iinfer/svfiler.js
+iinfer/web/assets/iinfer/view_raw.js
+iinfer/web/assets/iinfer/view_result.js
 iinfer/web/assets/jquery/jquery.min.3.2.0.js
 iinfer/web/assets/jquery-resizable/jquery-resizable.min.js
 iinfer/web/assets/jquery-ui/AUTHORS.txt
 iinfer/web/assets/jquery-ui/LICENSE.txt
 iinfer/web/assets/jquery-ui/jquery-ui.min.css
 iinfer/web/assets/jquery-ui/jquery-ui.min.js
 iinfer/web/assets/jquery-ui/jquery-ui.structure.min.css
```

### Comparing `iinfer-0.6.8/setup.py` & `iinfer-0.6.9/setup.py`

 * *Files identical despite different names*

