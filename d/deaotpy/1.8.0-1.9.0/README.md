# Comparing `tmp/deaotpy-1.8.0.tar.gz` & `tmp/deaotpy-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deaotpy-1.8.0.tar", last modified: Sun Apr  7 15:12:44 2024, max compression
+gzip compressed data, was "deaotpy-1.9.0.tar", last modified: Sun Apr  7 16:02:17 2024, max compression
```

## Comparing `deaotpy-1.8.0.tar` & `deaotpy-1.9.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.304015 deaotpy-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-07 15:03:06.000000 deaotpy-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-04-07 15:12:44.304015 deaotpy-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-07 15:03:06.000000 deaotpy-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.280014 deaotpy-1.8.0/aot/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13858 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.280014 deaotpy-1.8.0/aot/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5579 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.288015 deaotpy-1.8.0/aot/configs/models/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/aotb.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/aotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/aots.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/aott.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/deaotb.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/deaotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/deaots.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/deaott.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      957 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/default.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      420 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/default_deaot.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/r101_aotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/r50_aotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/r50_deaotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/rs101_aotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/swinb_aotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/swinb_deaotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/pre.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/pre_dav.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/pre_ytb.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/pre_ytb_dav.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/ytb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.288015 deaotpy-1.8.0/aot/dataloaders/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/dataloaders/eval_datasets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19828 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/dataloaders/image_transforms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24646 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/dataloaders/train_datasets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23575 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/dataloaders/video_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.288015 deaotpy-1.8.0/aot/networks/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.288015 deaotpy-1.8.0/aot/networks/decoders/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/decoders/fpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.292015 deaotpy-1.8.0/aot/networks/encoders/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1405 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/mobilenetv2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7899 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/mobilenetv3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.292015 deaotpy-1.8.0/aot/networks/encoders/resnest/
--rwxr-xr-x   0 runner    (1001) docker     (127)       23 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/resnest/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3343 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/resnest/resnest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16474 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/resnest/resnet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4467 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/resnest/splat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6692 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.292015 deaotpy-1.8.0/aot/networks/encoders/swin/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/swin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/swin/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    27345 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/swin/swin_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.296015 deaotpy-1.8.0/aot/networks/engines/
--rwxr-xr-x   0 runner    (1001) docker     (127)      693 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24646 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/engines/aot_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/engines/deaot_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.296015 deaotpy-1.8.0/aot/networks/layers/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32782 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/layers/attention.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5111 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/layers/basic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6698 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/layers/loss.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1700 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/layers/normalization.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2810 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/layers/position.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24836 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/layers/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.296015 deaotpy-1.8.0/aot/networks/managers/
--rwxr-xr-x   0 runner    (1001) docker     (127)    25895 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/managers/evaluator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29712 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/managers/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.300015 deaotpy-1.8.0/aot/networks/models/
--rwxr-xr-x   0 runner    (1001) docker     (127)      344 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4546 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/models/aot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/models/deaot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.300015 deaotpy-1.8.0/aot/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/tools/demo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3472 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/tools/eval.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2668 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/tools/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.304015 deaotpy-1.8.0/aot/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6200 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/cp_ckpt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3561 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/ema.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      443 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/eval.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6075 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/image.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3454 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/learning.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      829 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/math.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      860 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/meters.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1102 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.304015 deaotpy-1.8.0/deaotpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-04-07 15:12:44.000000 deaotpy-1.8.0/deaotpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-07 15:12:44.000000 deaotpy-1.8.0/deaotpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:12:44.000000 deaotpy-1.8.0/deaotpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-07 15:12:44.000000 deaotpy-1.8.0/deaotpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-07 15:12:44.000000 deaotpy-1.8.0/deaotpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-07 15:03:06.000000 deaotpy-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:12:44.304015 deaotpy-1.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:02:17.476481 deaotpy-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-07 15:57:45.000000 deaotpy-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-04-07 16:02:17.476481 deaotpy-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-07 15:57:45.000000 deaotpy-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:02:17.448481 deaotpy-1.9.0/aot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13858 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:02:17.448481 deaotpy-1.9.0/aot/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5583 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:02:17.456481 deaotpy-1.9.0/aot/configs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/models/aotb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/models/aotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/models/aots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/models/aott.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/models/deaotb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/models/deaotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/models/deaots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/models/deaott.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      957 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/models/default.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      420 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/models/default_deaot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/models/r101_aotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/models/r50_aotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/models/r50_deaotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/models/rs101_aotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/models/swinb_aotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/models/swinb_deaotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/pre.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/pre_dav.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/pre_ytb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/pre_ytb_dav.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/configs/ytb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:02:17.456481 deaotpy-1.9.0/aot/dataloaders/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/dataloaders/eval_datasets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19828 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/dataloaders/image_transforms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24646 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/dataloaders/train_datasets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23575 2024-04-07 15:57:46.000000 deaotpy-1.9.0/aot/dataloaders/video_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:02:17.456481 deaotpy-1.9.0/aot/networks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:02:17.460481 deaotpy-1.9.0/aot/networks/decoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/decoders/fpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:02:17.460481 deaotpy-1.9.0/aot/networks/encoders/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1405 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/encoders/mobilenetv2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7899 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/encoders/mobilenetv3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:02:17.460481 deaotpy-1.9.0/aot/networks/encoders/resnest/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       23 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/encoders/resnest/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3343 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/encoders/resnest/resnest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16474 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/encoders/resnest/resnet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4467 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/encoders/resnest/splat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6692 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/encoders/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:02:17.464481 deaotpy-1.9.0/aot/networks/encoders/swin/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/encoders/swin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/encoders/swin/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27345 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/encoders/swin/swin_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:02:17.464481 deaotpy-1.9.0/aot/networks/engines/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      693 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24646 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/engines/aot_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/engines/deaot_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:02:17.468481 deaotpy-1.9.0/aot/networks/layers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32782 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/layers/attention.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5111 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/layers/basic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6698 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/layers/loss.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1700 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/layers/normalization.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2810 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/layers/position.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24836 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/layers/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:02:17.468481 deaotpy-1.9.0/aot/networks/managers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25895 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/managers/evaluator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29712 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/managers/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:02:17.468481 deaotpy-1.9.0/aot/networks/models/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      344 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4546 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/models/aot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/networks/models/deaot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:02:17.472481 deaotpy-1.9.0/aot/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/tools/demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3472 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/tools/eval.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2668 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/tools/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:02:17.476481 deaotpy-1.9.0/aot/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6197 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/utils/cp_ckpt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3561 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/utils/ema.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      443 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/utils/eval.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6075 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/utils/image.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3454 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/utils/learning.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      829 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/utils/math.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      860 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/utils/meters.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1102 2024-04-07 15:57:47.000000 deaotpy-1.9.0/aot/utils/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:02:17.476481 deaotpy-1.9.0/deaotpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-04-07 16:02:17.000000 deaotpy-1.9.0/deaotpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-07 16:02:17.000000 deaotpy-1.9.0/deaotpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 16:02:17.000000 deaotpy-1.9.0/deaotpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-07 16:02:17.000000 deaotpy-1.9.0/deaotpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-07 16:02:17.000000 deaotpy-1.9.0/deaotpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-07 15:57:45.000000 deaotpy-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 16:02:17.476481 deaotpy-1.9.0/setup.cfg
```

### Comparing `deaotpy-1.8.0/LICENSE` & `deaotpy-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/PKG-INFO` & `deaotpy-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deaotpy
-Version: 1.8.0
+Version: 1.9.0
 Summary: Decoupling Features in Hierarchical Propagation for Video Object Segmentation.
 License: BSD 3-Clause License
         
         Copyright (c) 2020, z-x-yang
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `deaotpy-1.8.0/README.md` & `deaotpy-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/LICENSE` & `deaotpy-1.9.0/aot/LICENSE`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/README.md` & `deaotpy-1.9.0/aot/README.md`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/configs/default.py` & `deaotpy-1.9.0/aot/configs/default.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import importlib
 
 
 class DefaultEngineConfig():
     def __init__(self, exp_name='default', model='aott'):
-        model_cfg = importlib.import_module('configs.models.' +
+        model_cfg = importlib.import_module('aot.configs.models.' +
                                             model).ModelConfig()
         self.__dict__.update(model_cfg.__dict__)  # add model config
 
         self.EXP_NAME = exp_name + '_' + self.MODEL_NAME
 
         self.STAGE_NAME = 'YTB'
```

### Comparing `deaotpy-1.8.0/aot/configs/models/default.py` & `deaotpy-1.9.0/aot/configs/models/default.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/configs/models/r101_aotl.py` & `deaotpy-1.9.0/aot/configs/models/r101_aotl.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/configs/models/r50_aotl.py` & `deaotpy-1.9.0/aot/configs/models/r50_aotl.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/configs/models/r50_deaotl.py` & `deaotpy-1.9.0/aot/configs/models/r50_deaotl.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/configs/models/rs101_aotl.py` & `deaotpy-1.9.0/aot/configs/models/rs101_aotl.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/configs/models/swinb_aotl.py` & `deaotpy-1.9.0/aot/configs/models/swinb_aotl.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/configs/models/swinb_deaotl.py` & `deaotpy-1.9.0/aot/configs/models/swinb_deaotl.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/configs/pre.py` & `deaotpy-1.9.0/aot/configs/pre.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/configs/pre_dav.py` & `deaotpy-1.9.0/aot/configs/pre_dav.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/configs/pre_ytb.py` & `deaotpy-1.9.0/aot/configs/pre_ytb.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/configs/pre_ytb_dav.py` & `deaotpy-1.9.0/aot/configs/pre_ytb_dav.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/dataloaders/eval_datasets.py` & `deaotpy-1.9.0/aot/dataloaders/eval_datasets.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/dataloaders/image_transforms.py` & `deaotpy-1.9.0/aot/dataloaders/image_transforms.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/dataloaders/train_datasets.py` & `deaotpy-1.9.0/aot/dataloaders/train_datasets.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/dataloaders/video_transforms.py` & `deaotpy-1.9.0/aot/dataloaders/video_transforms.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/decoders/fpn.py` & `deaotpy-1.9.0/aot/networks/decoders/fpn.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/encoders/__init__.py` & `deaotpy-1.9.0/aot/networks/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/encoders/mobilenetv2.py` & `deaotpy-1.9.0/aot/networks/encoders/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/encoders/mobilenetv3.py` & `deaotpy-1.9.0/aot/networks/encoders/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/encoders/resnest/resnest.py` & `deaotpy-1.9.0/aot/networks/encoders/resnest/resnest.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/encoders/resnest/resnet.py` & `deaotpy-1.9.0/aot/networks/encoders/resnest/resnet.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/encoders/resnest/splat.py` & `deaotpy-1.9.0/aot/networks/encoders/resnest/splat.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/encoders/resnet.py` & `deaotpy-1.9.0/aot/networks/encoders/resnet.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/encoders/swin/build.py` & `deaotpy-1.9.0/aot/networks/encoders/swin/build.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/encoders/swin/swin_transformer.py` & `deaotpy-1.9.0/aot/networks/encoders/swin/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/engines/__init__.py` & `deaotpy-1.9.0/aot/networks/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/engines/aot_engine.py` & `deaotpy-1.9.0/aot/networks/engines/aot_engine.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/engines/deaot_engine.py` & `deaotpy-1.9.0/aot/networks/engines/deaot_engine.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/layers/attention.py` & `deaotpy-1.9.0/aot/networks/layers/attention.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/layers/basic.py` & `deaotpy-1.9.0/aot/networks/layers/basic.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/layers/loss.py` & `deaotpy-1.9.0/aot/networks/layers/loss.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/layers/normalization.py` & `deaotpy-1.9.0/aot/networks/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/layers/position.py` & `deaotpy-1.9.0/aot/networks/layers/position.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/layers/transformer.py` & `deaotpy-1.9.0/aot/networks/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/managers/evaluator.py` & `deaotpy-1.9.0/aot/networks/managers/evaluator.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/managers/trainer.py` & `deaotpy-1.9.0/aot/networks/managers/trainer.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/models/aot.py` & `deaotpy-1.9.0/aot/networks/models/aot.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/networks/models/deaot.py` & `deaotpy-1.9.0/aot/networks/models/deaot.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/tools/demo.py` & `deaotpy-1.9.0/aot/tools/demo.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/tools/eval.py` & `deaotpy-1.9.0/aot/tools/eval.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/tools/train.py` & `deaotpy-1.9.0/aot/tools/train.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/utils/checkpoint.py` & `deaotpy-1.9.0/aot/utils/checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import torch
 import os
 import shutil
 import numpy as np
 
 
-def load_network_and_optimizer(net, opt, pretrained_dir, gpu, scaler=None):
+def load_network_and_optimizer(net, opt, pretrained_dir, device, scaler=None):
     pretrained = torch.load(pretrained_dir,
-                            map_location=torch.device("cuda:" + str(gpu)))
+                            map_location=torch.device(device))
     pretrained_dict = pretrained['state_dict']
     model_dict = net.state_dict()
     pretrained_dict_update = {}
     pretrained_dict_remove = []
     for k, v in pretrained_dict.items():
         if k in model_dict:
             pretrained_dict_update[k] = v
@@ -21,20 +21,20 @@
             pretrained_dict_remove.append(k)
     model_dict.update(pretrained_dict_update)
     net.load_state_dict(model_dict)
     opt.load_state_dict(pretrained['optimizer'])
     if scaler is not None and 'scaler' in pretrained.keys():
         scaler.load_state_dict(pretrained['scaler'])
     del (pretrained)
-    return net.cuda(gpu), opt, pretrained_dict_remove
+    return net.to(device=device), opt, pretrained_dict_remove
 
 
-def load_network_and_optimizer_v2(net, opt, pretrained_dir, gpu, scaler=None):
+def load_network_and_optimizer_v2(net, opt, pretrained_dir, device, scaler=None):
     pretrained = torch.load(pretrained_dir,
-                            map_location=torch.device("cuda:" + str(gpu)))
+                            map_location=torch.device(device))
     # load model
     pretrained_dict = pretrained['state_dict']
     model_dict = net.state_dict()
     pretrained_dict_update = {}
     pretrained_dict_remove = []
     for k, v in pretrained_dict.items():
         if k in model_dict:
@@ -66,20 +66,20 @@
     opt_dict.update(pretrained_opt_dict)
     opt.load_state_dict(opt_dict)
 
     # load scaler
     if scaler is not None and 'scaler' in pretrained.keys():
         scaler.load_state_dict(pretrained['scaler'])
     del (pretrained)
-    return net.cuda(gpu), opt, pretrained_dict_remove
+    return net.to(device=device), opt, pretrained_dict_remove
 
 
-def load_network(net, pretrained_dir, gpu):
+def load_network(net, pretrained_dir, device):
     pretrained = torch.load(pretrained_dir,
-                            map_location=torch.device("cuda:" + str(gpu)))
+                            map_location=torch.device(device))
     if 'state_dict' in pretrained.keys():
         pretrained_dict = pretrained['state_dict']
     elif 'model' in pretrained.keys():
         pretrained_dict = pretrained['model']
     else:
         pretrained_dict = pretrained
     model_dict = net.state_dict()
@@ -92,15 +92,15 @@
             if k[7:] in model_dict:
                 pretrained_dict_update[k[7:]] = v
         else:
             pretrained_dict_remove.append(k)
     model_dict.update(pretrained_dict_update)
     net.load_state_dict(model_dict)
     del (pretrained)
-    return net.cuda(gpu), pretrained_dict_remove
+    return net.to(device=device), pretrained_dict_remove
 
 
 def save_network(net,
                  opt,
                  step,
                  save_path,
                  max_keep=8,
```

### Comparing `deaotpy-1.8.0/aot/utils/cp_ckpt.py` & `deaotpy-1.9.0/aot/utils/cp_ckpt.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/utils/ema.py` & `deaotpy-1.9.0/aot/utils/ema.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/utils/image.py` & `deaotpy-1.9.0/aot/utils/image.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/utils/learning.py` & `deaotpy-1.9.0/aot/utils/learning.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/utils/math.py` & `deaotpy-1.9.0/aot/utils/math.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/utils/meters.py` & `deaotpy-1.9.0/aot/utils/meters.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/aot/utils/metric.py` & `deaotpy-1.9.0/aot/utils/metric.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/deaotpy.egg-info/PKG-INFO` & `deaotpy-1.9.0/deaotpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deaotpy
-Version: 1.8.0
+Version: 1.9.0
 Summary: Decoupling Features in Hierarchical Propagation for Video Object Segmentation.
 License: BSD 3-Clause License
         
         Copyright (c) 2020, z-x-yang
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `deaotpy-1.8.0/deaotpy.egg-info/SOURCES.txt` & `deaotpy-1.9.0/deaotpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deaotpy-1.8.0/pyproject.toml` & `deaotpy-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools",
   "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deaotpy"
-version = "1.8.0"
+version = "1.9.0"
 description = "Decoupling Features in Hierarchical Propagation for Video Object Segmentation."
 readme = { file = "aot/README.md" , content-type = "text/markdown" }
 
 license = { file = "aot/LICENSE" }
 requires-python = ">=3.10"
 keywords = [
     "deep-learning",
```

