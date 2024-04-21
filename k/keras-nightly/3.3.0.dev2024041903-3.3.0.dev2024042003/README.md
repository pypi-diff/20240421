# Comparing `tmp/keras_nightly-3.3.0.dev2024041903.tar.gz` & `tmp/keras_nightly-3.3.0.dev2024042003.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_nightly-3.3.0.dev2024041903.tar", last modified: Fri Apr 19 03:21:54 2024, max compression
+gzip compressed data, was "keras_nightly-3.3.0.dev2024042003.tar", last modified: Sat Apr 20 03:21:22 2024, max compression
```

## Comparing `keras_nightly-3.3.0.dev2024041903.tar` & `keras_nightly-3.3.0.dev2024042003.tar`

### file list

```diff
@@ -1,921 +1,921 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.888486 keras_nightly-3.3.0.dev2024041903/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-19 03:21:54.888486 keras_nightly-3.3.0.dev2024041903/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.744486 keras_nightly-3.3.0.dev2024041903/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.744486 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/activation_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/attention_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/base_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/conv_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/core_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/merge_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/normalization_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/pooling_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/regularization_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/reshaping_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/rnn_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.744486 keras_nightly-3.3.0.dev2024041903/benchmarks/model_benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/model_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/model_benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/model_benchmark/bert_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/model_benchmark/image_classification_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.744486 keras_nightly-3.3.0.dev2024041903/benchmarks/torch_ctl_benchmark/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/torch_ctl_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/torch_ctl_benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.748486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.752486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.756486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.760486 keras_nightly-3.3.0.dev2024041903/keras/api/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.764486 keras_nightly-3.3.0.dev2024041903/keras/api/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8721 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5606 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.768486 keras_nightly-3.3.0.dev2024041903/keras/api/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/api/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.772486 keras_nightly-3.3.0.dev2024041903/keras/src/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.772486 keras_nightly-3.3.0.dev2024041903/keras/src/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)    30862 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/activations/activations_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.776486 keras_nightly-3.3.0.dev2024041903/keras/src/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10394 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/applications_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24919 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40460 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/imagenet_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/applications/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.776486 keras_nightly-3.3.0.dev2024041903/keras/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.780486 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/backend_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/compute_output_spec_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/dtypes_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/global_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/global_state_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/keras_tensor_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/name_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/name_scope_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/stateless_scope_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    31785 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/variables_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/exports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.780486 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/distribution_lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    30159 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.784486 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    27786 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.788486 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/distribute_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11445 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/name_scope_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26461 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    67883 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/optimizer_distribute_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6210 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/saved_model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.792486 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    24031 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    46016 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.792486 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.796486 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/backup_and_restore_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/callback_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/callback_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/csv_logger_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/early_stopping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/lambda_callback_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/learning_rate_scheduler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/model_checkpoint_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/reduce_lr_on_plateau_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/remote_monitor_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/swap_ema_weights_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    27236 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/tensorboard_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/terminate_on_nan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/terminate_on_nan_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.800486 keras_nightly-3.3.0.dev2024041903/keras/src/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/constraints/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/constraints/constraints_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.800486 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/boston_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/cifar100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/imdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/datasets/reuters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.800486 keras_nightly-3.3.0.dev2024041903/keras/src/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/distribution/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    18510 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/distribution/distribution_lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.800486 keras_nightly-3.3.0.dev2024041903/keras/src/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/dtype_policies/dtype_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17217 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/dtype_policies/dtype_policy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.804486 keras_nightly-3.3.0.dev2024041903/keras/src/export/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32830 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/export/export_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    33240 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/export/export_lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.804486 keras_nightly-3.3.0.dev2024041903/keras/src/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/initializers/constant_initializers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/initializers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/initializers/random_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/initializers/random_initializers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.804486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.808486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/activation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/elu.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/elu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/leaky_relu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/prelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/prelu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/relu_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/softmax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/softmax_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.808486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/additive_attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/grouped_query_attention_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/multi_head_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    13745 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/multi_head_attention_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.812486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17043 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    32424 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27575 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv_transpose_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/depthwise_conv_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/separable_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/separable_conv_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.816486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24999 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    26286 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/dense_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    41791 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    30544 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/einsum_dense_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17144 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    15413 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/embedding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/identity_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/input_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/lambda_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/masking_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/wrapper_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    63788 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    34277 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/layer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.820486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/average.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/merging_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.820486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/batch_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/group_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/layer_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/spectral_normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/unit_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/unit_normalization_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.824486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/average_pooling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_average_pooling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_max_pooling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/max_pooling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.832486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/audio_preprocessing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/category_encoding_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/center_crop_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/discretization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 runner    (1001) docker     (127)    21053 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/feature_space_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/hashed_crossing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20526 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/hashing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/index_lookup_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/integer_lookup_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/normalization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_brightness_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_contrast_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_crop_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_flip_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_rotation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_translation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_zoom_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/rescaling_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/resizing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/string_lookup_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/text_vectorization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.836486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/activity_regularization_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/alpha_dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/gaussian_dropout_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/gaussian_noise_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/spatial_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/spatial_dropout_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.840486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/flatten_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/permute_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/repeat_vector_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/reshape_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding3d_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.844486 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13203 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/bidirectional_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm1d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm2d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm3d_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/dropout_rnn_cell_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/gru_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/lstm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    15320 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/rnn_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/simple_rnn_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/stacked_rnn_cells_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/time_distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/time_distributed_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.848486 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.848486 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.848486 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/json_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/legacy_h5_format_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.848486 keras_nightly-3.3.0.dev2024041903/keras/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/losses/loss_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    69132 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/losses/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)    54720 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/losses/losses_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.852486 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17463 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/accuracy_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    63267 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/confusion_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/f_score_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/hinge_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17104 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/iou_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/metric_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/probabilistic_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/reduction_metrics_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/regression_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/metrics/regression_metrics_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.856486 keras_nightly-3.3.0.dev2024041903/keras/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/cloning_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    32453 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/functional_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22766 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    23758 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/sequential_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/variable_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/models/variable_mapping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.860486 keras_nightly-3.3.0.dev2024041903/keras/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    31327 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/core_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/function_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    37256 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    31485 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    19959 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/linalg_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    47868 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/math_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    62113 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    81862 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/nn_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/node_test.py
--rw-r--r--   0 runner    (1001) docker     (127)   190918 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)   279186 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/numpy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/operation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/operation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/operation_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/symbolic_arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/ops/symbolic_arguments_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.868486 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adadelta_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adafactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adafactor_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adagrad_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adam_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adamax_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adamw_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    40410 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/ftrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/ftrl_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/lion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/loss_scale_optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/nadam_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/optimizer_sparse_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13009 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/optimizer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/rmsprop_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.868486 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    15392 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/schedules/learning_rate_schedule_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/sgd_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.868486 keras_nightly-3.3.0.dev2024041903/keras/src/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/quantizers/quantizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/quantizers/quantizers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.868486 keras_nightly-3.3.0.dev2024041903/keras/src/random/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/random/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    17949 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/random/random_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/random/seed_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/random/seed_generator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.872486 keras_nightly-3.3.0.dev2024041903/keras/src/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/regularizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/regularizers/regularizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/regularizers/regularizers_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.872486 keras_nightly-3.3.0.dev2024041903/keras/src/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/saving/object_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/saving/object_registration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/saving/saving_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/saving/saving_api_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    27008 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/saving/saving_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    33448 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/saving/saving_lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28700 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/saving/serialization_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    13623 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/saving/serialization_lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.872486 keras_nightly-3.3.0.dev2024041903/keras/src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27552 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/testing/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/testing/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/testing/test_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.876486 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/compile_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/compile_utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.876486 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/array_data_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/generator_data_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9799 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/py_dataset_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/epoch_iterator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    46440 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)    51439 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/trainers/trainer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.880486 keras_nightly-3.3.0.dev2024041903/keras/src/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/tree/dmtree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/tree/optree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/tree/tree_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/tree/tree_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.888486 keras_nightly-3.3.0.dev2024041903/keras/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/audio_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/code_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/code_stats_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/dtype_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    28322 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/file_utils_test.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16538 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20039 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/image_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/io_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/jax_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23050 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/jax_layer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/model_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/naming_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/numerical_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/numerical_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/progbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/python_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/rng_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/rng_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/sequence_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/summary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/summary_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/text_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/timeseries_dataset_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/torch_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/traceback_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/keras/src/utils/tracking_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-19 03:21:52.000000 keras_nightly-3.3.0.dev2024041903/keras/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 03:21:54.888486 keras_nightly-3.3.0.dev2024041903/keras_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-19 03:21:54.000000 keras_nightly-3.3.0.dev2024041903/keras_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    30410 2024-04-19 03:21:54.000000 keras_nightly-3.3.0.dev2024041903/keras_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 03:21:54.000000 keras_nightly-3.3.0.dev2024041903/keras_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 03:21:54.000000 keras_nightly-3.3.0.dev2024041903/keras_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 03:21:54.000000 keras_nightly-3.3.0.dev2024041903/keras_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-19 03:20:08.000000 keras_nightly-3.3.0.dev2024041903/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 03:21:54.888486 keras_nightly-3.3.0.dev2024041903/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-19 03:21:52.000000 keras_nightly-3.3.0.dev2024041903/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.711296 keras_nightly-3.3.0.dev2024042003/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-20 03:21:22.711296 keras_nightly-3.3.0.dev2024042003/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.583294 keras_nightly-3.3.0.dev2024042003/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.587295 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/activation_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/attention_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/base_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/conv_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/core_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/merge_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/normalization_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/pooling_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/regularization_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/reshaping_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/rnn_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.587295 keras_nightly-3.3.0.dev2024042003/benchmarks/model_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/model_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/model_benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/model_benchmark/bert_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/model_benchmark/image_classification_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.587295 keras_nightly-3.3.0.dev2024042003/benchmarks/torch_ctl_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/torch_ctl_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/torch_ctl_benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.587295 keras_nightly-3.3.0.dev2024042003/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.587295 keras_nightly-3.3.0.dev2024042003/keras/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.591295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.595295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.599295 keras_nightly-3.3.0.dev2024042003/keras/api/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.603295 keras_nightly-3.3.0.dev2024042003/keras/api/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.607295 keras_nightly-3.3.0.dev2024042003/keras/api/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/api/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/api/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.611295 keras_nightly-3.3.0.dev2024042003/keras/src/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30862 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/activations/activations_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.615295 keras_nightly-3.3.0.dev2024042003/keras/src/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10394 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/applications_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24919 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40460 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11284 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/imagenet_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/applications/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.619295 keras_nightly-3.3.0.dev2024042003/keras/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.619295 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/backend_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/compute_output_spec_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/dtypes_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/global_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/global_state_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15026 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/keras_tensor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/name_scope_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/stateless_scope_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31785 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/variables_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/exports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.623295 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13481 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/distribution_lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18803 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30577 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.627295 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27893 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.627295 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9444 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/distribute_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/name_scope_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26461 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77115 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/optimizer_distribute_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/saved_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.631295 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24031 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47135 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.631295 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.639295 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/backup_and_restore_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/callback_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5831 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/csv_logger_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/early_stopping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/lambda_callback_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/learning_rate_scheduler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18107 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/model_checkpoint_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4313 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/reduce_lr_on_plateau_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/remote_monitor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6707 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/swap_ema_weights_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27236 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/tensorboard_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/terminate_on_nan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/terminate_on_nan_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.639295 keras_nightly-3.3.0.dev2024042003/keras/src/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/constraints/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/constraints/constraints_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.639295 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7149 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/datasets/reuters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.639295 keras_nightly-3.3.0.dev2024042003/keras/src/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/distribution/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18510 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/distribution/distribution_lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.639295 keras_nightly-3.3.0.dev2024042003/keras/src/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12320 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/dtype_policies/dtype_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17217 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/dtype_policies/dtype_policy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.639295 keras_nightly-3.3.0.dev2024042003/keras/src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32830 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/export/export_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33240 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/export/export_lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.643295 keras_nightly-3.3.0.dev2024042003/keras/src/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/initializers/constant_initializers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/initializers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/initializers/random_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6637 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/initializers/random_initializers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.643295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.643295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/activation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/elu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/elu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/leaky_relu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/prelu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/relu_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/softmax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/softmax_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.647295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/additive_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/grouped_query_attention_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28353 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/multi_head_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13745 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/multi_head_attention_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.651295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17043 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32424 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27575 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv_transpose_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5999 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6087 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14801 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/depthwise_conv_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/separable_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11914 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/separable_conv_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.651295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24999 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26286 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/dense_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41791 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30544 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/einsum_dense_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17144 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15413 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/embedding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/identity_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5107 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/input_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/lambda_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/masking_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/wrapper_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63788 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34277 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/layer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.655295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6586 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/merging_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.655295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/batch_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/group_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9836 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/layer_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/spectral_normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/unit_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/unit_normalization_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.659295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/average_pooling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_average_pooling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_max_pooling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9863 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/max_pooling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.667295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/audio_preprocessing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12397 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/category_encoding_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/center_crop_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/discretization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21053 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/feature_space_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/hashed_crossing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20526 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/hashing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/index_lookup_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/integer_lookup_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/normalization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_brightness_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_contrast_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_crop_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_flip_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_rotation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_translation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_zoom_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/rescaling_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/resizing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17734 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/string_lookup_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/text_vectorization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.667295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/activity_regularization_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/alpha_dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/gaussian_dropout_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/gaussian_noise_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/spatial_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/spatial_dropout_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.671296 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4368 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/flatten_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/permute_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/repeat_vector_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/reshape_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4862 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding3d_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.675295 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13203 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9359 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/bidirectional_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm1d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm2d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm3d_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/dropout_rnn_cell_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27701 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/gru_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9743 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/lstm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15320 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/rnn_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9276 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/simple_rnn_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/stacked_rnn_cells_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/time_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/time_distributed_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.679295 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.679295 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.679295 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/json_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/legacy_h5_format_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.679295 keras_nightly-3.3.0.dev2024042003/keras/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9374 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/losses/loss_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69132 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/losses/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54720 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/losses/losses_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.683296 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17463 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/accuracy_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63267 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/confusion_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15184 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/f_score_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/hinge_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17104 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/iou_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8186 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/metric_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/probabilistic_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5044 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/reduction_metrics_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/regression_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/metrics/regression_metrics_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.687296 keras_nightly-3.3.0.dev2024042003/keras/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11094 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/cloning_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32453 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14762 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/functional_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23789 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24695 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/sequential_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/variable_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/models/variable_mapping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.691295 keras_nightly-3.3.0.dev2024042003/keras/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22866 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31327 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/core_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/function_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37256 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31485 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19959 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/linalg_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47868 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/math_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62113 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81862 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/nn_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/node_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)   193387 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)   283774 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/numpy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/operation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13759 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/operation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/operation_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/symbolic_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/ops/symbolic_arguments_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.695296 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adadelta_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3791 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adafactor_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adagrad_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adam_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adamax_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adamw_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40410 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/ftrl_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2985 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/lion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/loss_scale_optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/nadam_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/optimizer_sparse_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13009 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/optimizer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/rmsprop_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.695296 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15392 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/schedules/learning_rate_schedule_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/sgd_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.695296 keras_nightly-3.3.0.dev2024042003/keras/src/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/quantizers/quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/quantizers/quantizers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.695296 keras_nightly-3.3.0.dev2024042003/keras/src/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/random/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17949 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/random/random_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/random/seed_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/random/seed_generator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.699296 keras_nightly-3.3.0.dev2024042003/keras/src/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/regularizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/regularizers/regularizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/regularizers/regularizers_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.699296 keras_nightly-3.3.0.dev2024042003/keras/src/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/saving/object_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/saving/object_registration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/saving/saving_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/saving/saving_api_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27008 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/saving/saving_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33448 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/saving/saving_lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29052 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/saving/serialization_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13761 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/saving/serialization_lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.699296 keras_nightly-3.3.0.dev2024042003/keras/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27552 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/testing/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/testing/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10599 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/testing/test_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.699296 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/compile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13799 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/compile_utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.703296 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/array_data_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/generator_data_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9799 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/py_dataset_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10998 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5843 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/epoch_iterator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51439 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/trainers/trainer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.703296 keras_nightly-3.3.0.dev2024042003/keras/src/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/tree/dmtree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/tree/optree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/tree/tree_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/tree/tree_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.711296 keras_nightly-3.3.0.dev2024042003/keras/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14664 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/audio_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/code_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/code_stats_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/dtype_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28322 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/file_utils_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16538 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20039 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/image_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/io_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/jax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23050 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/jax_layer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/model_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/naming_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/numerical_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/progbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/python_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/rng_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/rng_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/sequence_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/summary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/summary_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/text_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/timeseries_dataset_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8232 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/torch_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/keras/src/utils/tracking_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-20 03:21:20.000000 keras_nightly-3.3.0.dev2024042003/keras/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 03:21:22.711296 keras_nightly-3.3.0.dev2024042003/keras_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-04-20 03:21:22.000000 keras_nightly-3.3.0.dev2024042003/keras_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30410 2024-04-20 03:21:22.000000 keras_nightly-3.3.0.dev2024042003/keras_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 03:21:22.000000 keras_nightly-3.3.0.dev2024042003/keras_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-20 03:21:22.000000 keras_nightly-3.3.0.dev2024042003/keras_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-20 03:21:22.000000 keras_nightly-3.3.0.dev2024042003/keras_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-20 03:19:48.000000 keras_nightly-3.3.0.dev2024042003/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-20 03:21:22.715296 keras_nightly-3.3.0.dev2024042003/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-20 03:21:20.000000 keras_nightly-3.3.0.dev2024042003/setup.py
```

### Comparing `keras_nightly-3.3.0.dev2024041903/LICENSE` & `keras_nightly-3.3.0.dev2024042003/LICENSE`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/PKG-INFO` & `keras_nightly-3.3.0.dev2024042003/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.0.dev2024041903
+Version: 3.3.0.dev2024042003
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.3.0.dev2024041903/README.md` & `keras_nightly-3.3.0.dev2024042003/README.md`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/activation_benchmark.py` & `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/activation_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/attention_benchmark.py` & `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/attention_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/base_benchmark.py` & `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/base_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/conv_benchmark.py` & `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/conv_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/core_benchmark.py` & `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/core_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/merge_benchmark.py` & `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/merge_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/normalization_benchmark.py` & `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/normalization_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/pooling_benchmark.py` & `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/pooling_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/regularization_benchmark.py` & `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/regularization_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/reshaping_benchmark.py` & `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/reshaping_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/benchmarks/layer_benchmark/rnn_benchmark.py` & `keras_nightly-3.3.0.dev2024042003/benchmarks/layer_benchmark/rnn_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/benchmarks/model_benchmark/benchmark_utils.py` & `keras_nightly-3.3.0.dev2024042003/benchmarks/model_benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/benchmarks/model_benchmark/bert_benchmark.py` & `keras_nightly-3.3.0.dev2024042003/benchmarks/model_benchmark/bert_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/benchmarks/model_benchmark/image_classification_benchmark.py` & `keras_nightly-3.3.0.dev2024042003/benchmarks/model_benchmark/image_classification_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/benchmarks/torch_ctl_benchmark/benchmark_utils.py` & `keras_nightly-3.3.0.dev2024042003/benchmarks/torch_ctl_benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py` & `keras_nightly-3.3.0.dev2024042003/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py` & `keras_nightly-3.3.0.dev2024042003/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/activations/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/convnext/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/backend/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/callbacks/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/config/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/constraints/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/distribution/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/initializers/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/layers/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/losses/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/metrics/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/mixed_precision/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,14 +186,15 @@
 from keras.src.ops.numpy import ravel
 from keras.src.ops.numpy import real
 from keras.src.ops.numpy import reciprocal
 from keras.src.ops.numpy import repeat
 from keras.src.ops.numpy import reshape
 from keras.src.ops.numpy import roll
 from keras.src.ops.numpy import round
+from keras.src.ops.numpy import select
 from keras.src.ops.numpy import sign
 from keras.src.ops.numpy import sin
 from keras.src.ops.numpy import sinh
 from keras.src.ops.numpy import size
 from keras.src.ops.numpy import sort
 from keras.src.ops.numpy import split
 from keras.src.ops.numpy import sqrt
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/linalg/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/nn/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/ops/numpy/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 from keras.src.ops.numpy import ravel
 from keras.src.ops.numpy import real
 from keras.src.ops.numpy import reciprocal
 from keras.src.ops.numpy import repeat
 from keras.src.ops.numpy import reshape
 from keras.src.ops.numpy import roll
 from keras.src.ops.numpy import round
+from keras.src.ops.numpy import select
 from keras.src.ops.numpy import sign
 from keras.src.ops.numpy import sin
 from keras.src.ops.numpy import sinh
 from keras.src.ops.numpy import size
 from keras.src.ops.numpy import sort
 from keras.src.ops.numpy import split
 from keras.src.ops.numpy import sqrt
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/optimizers/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/quantizers/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/random/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/regularizers/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/saving/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/tree/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/_tf_keras/keras/utils/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/activations/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/applications/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/applications/convnext/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/applications/efficientnet/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/backend/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/callbacks/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/config/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/constraints/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/distribution/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/initializers/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/layers/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/losses/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/metrics/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/mixed_precision/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/ops/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/ops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,14 +186,15 @@
 from keras.src.ops.numpy import ravel
 from keras.src.ops.numpy import real
 from keras.src.ops.numpy import reciprocal
 from keras.src.ops.numpy import repeat
 from keras.src.ops.numpy import reshape
 from keras.src.ops.numpy import roll
 from keras.src.ops.numpy import round
+from keras.src.ops.numpy import select
 from keras.src.ops.numpy import sign
 from keras.src.ops.numpy import sin
 from keras.src.ops.numpy import sinh
 from keras.src.ops.numpy import size
 from keras.src.ops.numpy import sort
 from keras.src.ops.numpy import split
 from keras.src.ops.numpy import sqrt
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/ops/linalg/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/ops/nn/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/ops/numpy/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/ops/numpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 from keras.src.ops.numpy import ravel
 from keras.src.ops.numpy import real
 from keras.src.ops.numpy import reciprocal
 from keras.src.ops.numpy import repeat
 from keras.src.ops.numpy import reshape
 from keras.src.ops.numpy import roll
 from keras.src.ops.numpy import round
+from keras.src.ops.numpy import select
 from keras.src.ops.numpy import sign
 from keras.src.ops.numpy import sin
 from keras.src.ops.numpy import sinh
 from keras.src.ops.numpy import size
 from keras.src.ops.numpy import sort
 from keras.src.ops.numpy import split
 from keras.src.ops.numpy import sqrt
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/optimizers/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/optimizers/legacy/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/optimizers/schedules/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/quantizers/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/random/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/regularizers/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/saving/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/tree/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/api/utils/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/activations/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/activations/activations.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/activations/activations_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/activations/activations_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/api_export.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/applications/applications_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/applications/applications_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/applications/convnext.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/applications/densenet.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/applications/efficientnet.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/applications/efficientnet_v2.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/applications/imagenet_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/applications/imagenet_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/applications/imagenet_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/applications/inception_resnet_v2.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/applications/inception_v3.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/applications/mobilenet.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/applications/mobilenet_v2.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/applications/mobilenet_v3.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/applications/nasnet.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/applications/resnet.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/applications/resnet_v2.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/applications/vgg16.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/applications/vgg19.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/applications/xception.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/backend_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/backend_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/backend_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/compute_output_spec_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/compute_output_spec_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/dtypes.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/dtypes.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/dtypes_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/dtypes_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/global_state.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/global_state.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/keras_tensor.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/keras_tensor_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/keras_tensor_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/name_scope.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/name_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/name_scope_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/name_scope_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/stateless_scope.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/stateless_scope_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/stateless_scope_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/variables.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/variables.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/common/variables_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/common/variables_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/config.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/exports.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/core.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/distribution_lib.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/distribution_lib_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/distribution_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/image.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/linalg.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/math.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/nn.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/numpy.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,18 +219,16 @@
 
 @sparse.elementwise_unary(linear=False)
 def absolute(x):
     x = convert_to_tensor(x)
     return jnp.absolute(x)
 
 
-@sparse.elementwise_unary(linear=False)
 def abs(x):
-    x = convert_to_tensor(x)
-    return jnp.absolute(x)
+    return absolute(x)
 
 
 def all(x, axis=None, keepdims=False):
     return jnp.all(x, axis=axis, keepdims=keepdims)
 
 
 def any(x, axis=None, keepdims=False):
@@ -970,15 +968,26 @@
     x2 = convert_to_tensor(x2)
     return jnp.tensordot(x1, x2, axes=axes)
 
 
 @sparse.elementwise_unary(linear=False)
 def round(x, decimals=0):
     x = convert_to_tensor(x)
-    return jnp.round(x, decimals=decimals)
+
+    # jnp.round doesn't support decimals < 0 for integers
+    x_dtype = standardize_dtype(x.dtype)
+    if "int" in x_dtype and decimals < 0:
+        factor = cast(math.pow(10, decimals), config.floatx())
+        x = cast(x, config.floatx())
+        x = jnp.multiply(x, factor)
+        x = jnp.round(x)
+        x = jnp.divide(x, factor)
+        return cast(x, x_dtype)
+    else:
+        return jnp.round(x, decimals=decimals)
 
 
 def tile(x, repeats):
     return jnp.tile(x, repeats)
 
 
 def trace(x, offset=0, axis1=0, axis2=1):
@@ -1139,7 +1148,11 @@
     return jnp.logical_xor(x1, x2)
 
 
 def correlate(x1, x2, mode="valid"):
     x1 = convert_to_tensor(x1)
     x2 = convert_to_tensor(x2)
     return jnp.correlate(x1, x2, mode)
+
+
+def select(condlist, choicelist, default=0):
+    return jnp.select(condlist, choicelist, default=default)
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/optimizer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/random.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/rnn.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/sparse.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/jax/trainer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/jax/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/core.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/image.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/linalg.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/math.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/nn.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/numpy.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1086,7 +1086,11 @@
         dtype = "float64"
     elif dtype not in ["bfloat16", "float16", "float64"]:
         dtype = "float32"
 
     x1 = convert_to_tensor(x1, dtype)
     x2 = convert_to_tensor(x2, dtype)
     return np.correlate(x1, x2, mode)
+
+
+def select(condlist, choicelist, default=0):
+    return np.select(condlist, choicelist, default=default)
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/random.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/rnn.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/numpy/trainer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/numpy/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/core.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/distribute_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/distribute_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/distribution_lib.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/image.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/layer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/linalg.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/linalg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import tensorflow as tf
-from tensorflow.experimental import numpy as tfnp
 
 from keras.src.backend import config
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common import dtypes
 from keras.src.backend.tensorflow.core import cast
 from keras.src.backend.tensorflow.core import convert_to_tensor
 
@@ -32,14 +31,16 @@
 
 def lu_factor(a):
     lu, p = tf.linalg.lu(a)
     return lu, tf.math.invert_permutation(p)
 
 
 def norm(x, ord=None, axis=None, keepdims=False):
+    from keras.src.backend.tensorflow.numpy import moveaxis
+
     x = convert_to_tensor(x)
     x_shape = x.shape
     ndim = x_shape.rank
 
     if axis is None:
         axis = tuple(range(ndim))
     elif isinstance(axis, int):
@@ -125,15 +126,15 @@
                 row_axis -= 1
             x = tf.math.reduce_min(
                 tf.reduce_sum(tf.math.abs(x), axis=col_axis, keepdims=keepdims),
                 axis=row_axis,
                 keepdims=keepdims,
             )
         elif ord in ("nuc", 2, -2):
-            x = tfnp.moveaxis(x, axis, (-2, -1))
+            x = moveaxis(x, axis, (-2, -1))
             if ord == -2:
                 x = tf.math.reduce_min(
                     tf.linalg.svd(x, compute_uv=False), axis=-1
                 )
             elif ord == 2:
                 x = tf.math.reduce_max(
                     tf.linalg.svd(x, compute_uv=False), axis=-1
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/math.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/math.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import tensorflow as tf
-from tensorflow.experimental import numpy as tfnp
 
 from keras.src.backend import config
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common import dtypes
 from keras.src.backend.tensorflow.core import cast
 from keras.src.backend.tensorflow.core import convert_to_tensor
 
@@ -256,14 +255,16 @@
 def solve(a, b):
     a = convert_to_tensor(a)
     b = convert_to_tensor(b)
     return tf.linalg.solve(a, b)
 
 
 def norm(x, ord=None, axis=None, keepdims=False):
+    from keras.src.backend.tensorflow.numpy import moveaxis
+
     x = convert_to_tensor(x)
     x_shape = x.shape
     ndim = x_shape.rank
 
     if axis is None:
         axis = tuple(range(ndim))
     elif isinstance(axis, int):
@@ -324,15 +325,15 @@
                 col_axis -= 1
             x = tf.math.reduce_min(
                 tf.reduce_sum(tf.math.abs(x), axis=row_axis, keepdims=keepdims),
                 axis=col_axis,
                 keepdims=keepdims,
             )
         else:
-            x = tfnp.moveaxis(x, axis, (-2, -1))
+            x = moveaxis(x, axis, (-2, -1))
             if ord == -2:
                 x = tf.math.reduce_min(
                     tf.linalg.svd(x, compute_uv=False), axis=-1
                 )
             else:
                 x = tf.math.reduce_sum(
                     tf.linalg.svd(x, compute_uv=False), axis=-1
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/name_scope_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/name_scope_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/nn.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/numpy.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/numpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import functools
 import math
 import string
 import warnings
 
 import numpy as np
 import tensorflow as tf
-from tensorflow.experimental import numpy as tfnp
 from tensorflow.python.ops.linalg.sparse import sparse_csr_matrix_ops
 
 from keras.src import tree
 from keras.src.backend import config
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common import dtypes
 from keras.src.backend.common.backend_utils import canonicalize_axis
@@ -571,54 +570,63 @@
     output = tf.reduce_mean(
         tf.cast(x, compute_dtype), axis=axis, keepdims=keepdims
     )
     return tf.cast(output, result_dtype)
 
 
 def max(x, axis=None, keepdims=False, initial=None):
+    x = convert_to_tensor(x)
+
     # The TensorFlow numpy API implementation doesn't support `initial` so we
     # handle it manually here.
     if initial is not None:
-        return tf.math.maximum(
-            tfnp.max(x, axis=axis, keepdims=keepdims), initial
-        )
+        if standardize_dtype(x.dtype) == "bool":
+            x = tf.reduce_any(x, axis=axis, keepdims=keepdims)
+            x = tf.math.maximum(tf.cast(x, "int32"), tf.cast(initial, "int32"))
+            return tf.cast(x, "bool")
+        else:
+            x = tf.reduce_max(x, axis=axis, keepdims=keepdims)
+            return tf.math.maximum(x, initial)
 
     # TensorFlow returns -inf by default for an empty list, but for consistency
     # with other backends and the numpy API we want to throw in this case.
     if tf.executing_eagerly():
         size_x = size(x)
         tf.assert_greater(
             size_x,
             tf.constant(0, dtype=size_x.dtype),
             message="Cannot compute the max of an empty tensor.",
         )
 
-    return tfnp.max(x, axis=axis, keepdims=keepdims)
+    if standardize_dtype(x.dtype) == "bool":
+        return tf.reduce_any(x, axis=axis, keepdims=keepdims)
+    else:
+        return tf.reduce_max(x, axis=axis, keepdims=keepdims)
 
 
 def ones(shape, dtype=None):
     dtype = dtype or config.floatx()
     return tf.ones(shape, dtype=dtype)
 
 
 def zeros(shape, dtype=None):
     dtype = dtype or config.floatx()
     return tf.zeros(shape, dtype=dtype)
 
 
 @sparse.elementwise_unary
 def absolute(x):
+    x = convert_to_tensor(x)
     # uintx and bool are always non-negative
     dtype = standardize_dtype(x.dtype)
     if "uint" in dtype or dtype == "bool":
         return x
     return tf.abs(x)
 
 
-@sparse.elementwise_unary
 def abs(x):
     return absolute(x)
 
 
 def all(x, axis=None, keepdims=False):
     x = tf.cast(x, "bool")
     return tf.reduce_all(x, axis=axis, keepdims=keepdims)
@@ -646,16 +654,14 @@
     if axis is None:
         return tf.concat([tf.reshape(x1, [-1]), tf.reshape(x2, [-1])], axis=0)
     else:
         return tf.concat([x1, x2], axis=axis)
 
 
 def arange(start, stop=None, step=1, dtype=None):
-    # tfnp.arange has trouble with dynamic Tensors in compiled function.
-    # tf.range does not.
     if dtype is None:
         dtypes_to_resolve = [
             getattr(start, "dtype", type(start)),
             getattr(step, "dtype", type(step)),
         ]
         if stop is not None:
             dtypes_to_resolve.append(getattr(stop, "dtype", type(stop)))
@@ -793,35 +799,47 @@
 
 def array(x, dtype=None):
     return convert_to_tensor(x, dtype=dtype)
 
 
 def average(x, axis=None, weights=None):
     x = convert_to_tensor(x)
-    axis = to_tuple_or_list(axis)
-    dtypes_to_resolve = [x.dtype, float]
-    if weights is not None:
+
+    if weights is None:  # Treat all weights as 1
+        dtype = dtypes.result_type(x.dtype, float)
+        x = tf.cast(x, dtype)
+        avg = tf.reduce_mean(x, axis=axis)
+    else:
         weights = convert_to_tensor(weights)
-        dtypes_to_resolve.append(weights.dtype)
-    result_dtype = dtypes.result_type(*dtypes_to_resolve)
-    compute_dtype = result_dtype
-    # TODO: since tfnp.average incorrectly promote bfloat16 to float64, we
-    # need to cast to float32 first and then cast back to bfloat16
-    if compute_dtype == "bfloat16":
-        compute_dtype = "float32"
-    x = tf.cast(x, compute_dtype)
-    if weights is not None:
-        weights = tf.cast(weights, compute_dtype)
-    if axis is None:
-        x = tfnp.average(x, weights=weights, axis=None)
-        return tf.cast(x, result_dtype)
-    for a in axis:
-        # `tfnp.average` does not handle multiple axes.
-        x = tfnp.average(x, weights=weights, axis=a)
-    return tf.cast(x, result_dtype)
+        dtype = dtypes.result_type(x.dtype, weights.dtype, float)
+        x = tf.cast(x, dtype)
+        weights = tf.cast(weights, dtype)
+
+        def _rank_equal_case():
+            weights_sum = tf.reduce_sum(weights, axis=axis)
+            return tf.reduce_sum(x * weights, axis=axis) / weights_sum
+
+        def _rank_not_equal_case():
+            weights_sum = tf.reduce_sum(weights)
+            axes = tf.convert_to_tensor([[axis], [0]])
+            return tf.tensordot(x, weights, axes) / weights_sum
+
+        if axis is None:
+            avg = _rank_equal_case()
+        else:
+            # We condition on rank rather than shape equality, because if we do
+            # the latter, when the shapes are partially unknown but the ranks
+            # are known and different, np_utils.cond will run shape checking on
+            # the true branch, which will raise a shape-checking error.
+            avg = tf.cond(
+                tf.equal(tf.rank(x), tf.rank(weights)),
+                _rank_equal_case,
+                _rank_not_equal_case,
+            )
+    return avg
 
 
 def broadcast_to(x, shape):
     return tf.broadcast_to(x, shape)
 
 
 @sparse.elementwise_unary
@@ -872,15 +890,16 @@
 @sparse.elementwise_unary
 def conj(x):
     return tf.math.conj(x)
 
 
 @sparse.elementwise_unary
 def copy(x):
-    return tfnp.copy(x)
+    x = convert_to_tensor(x)
+    return tf.identity(x)
 
 
 @sparse.densifying_unary(1)
 def cos(x):
     x = convert_to_tensor(x)
     if standardize_dtype(x.dtype) == "int64":
         dtype = config.floatx()
@@ -904,25 +923,60 @@
 def count_nonzero(x, axis=None):
     return tf.math.count_nonzero(x, axis=axis, dtype="int32")
 
 
 def cross(x1, x2, axisa=-1, axisb=-1, axisc=-1, axis=None):
     x1 = convert_to_tensor(x1)
     x2 = convert_to_tensor(x2)
+    if axis is not None:
+        axisa = axis
+        axisb = axis
+        axisc = axis
+    x1 = moveaxis(x1, axisa, -1)
+    x2 = moveaxis(x2, axisb, -1)
+
     dtype = dtypes.result_type(x1.dtype, x2.dtype)
     x1 = tf.cast(x1, dtype)
     x2 = tf.cast(x2, dtype)
-    return tfnp.cross(
-        x1,
-        x2,
-        axisa=axisa,
-        axisb=axisb,
-        axisc=axisc,
-        axis=axis,
+
+    def maybe_pad_zeros(x, size_of_last_dim):
+        def pad_zeros(x):
+            return tf.pad(
+                x,
+                tf.concat(
+                    [
+                        tf.zeros([tf.rank(x) - 1, 2], "int32"),
+                        tf.constant([[0, 1]], "int32"),
+                    ],
+                    axis=0,
+                ),
+            )
+
+        return tf.cond(
+            tf.equal(size_of_last_dim, 2), lambda: pad_zeros(x), lambda: x
+        )
+
+    x1_dim = tf.shape(x1)[-1]
+    x2_dim = tf.shape(x2)[-1]
+    x1 = maybe_pad_zeros(x1, x1_dim)
+    x2 = maybe_pad_zeros(x2, x2_dim)
+
+    # Broadcast each other
+    shape = tf.shape(x1)
+    shape = tf.broadcast_dynamic_shape(shape, tf.shape(x2))
+    x1 = tf.broadcast_to(x1, shape)
+    x2 = tf.broadcast_to(x2, shape)
+
+    c = tf.linalg.cross(x1, x2)
+    c = tf.cond(
+        (x1_dim == 2) & (x2_dim == 2),
+        lambda: c[..., 2],
+        lambda: moveaxis(c, -1, axisc),
     )
+    return c
 
 
 def cumprod(x, axis=None, dtype=None):
     x = convert_to_tensor(x, dtype=dtype)
     # tf.math.cumprod doesn't support bool
     if standardize_dtype(x.dtype) == "bool":
         x = tf.cast(x, "int32")
@@ -940,28 +994,78 @@
     if axis is None:
         x = tf.reshape(x, [-1])
         axis = 0
     return tf.math.cumsum(x, axis=axis)
 
 
 def diag(x, k=0):
-    return tfnp.diag(x, k=k)
+    x = convert_to_tensor(x)
+    if len(x.shape) == 1:
+        return tf.cond(
+            tf.equal(tf.size(x), 0),
+            lambda: tf.zeros([builtins.abs(k), builtins.abs(k)], dtype=x.dtype),
+            lambda: tf.linalg.diag(x, k=k),
+        )
+    elif len(x.shape) == 2:
+        return diagonal(x, offset=k)
+    else:
+        raise ValueError(f"`x` must be 1d or 2d. Received: x.shape={x.shape}")
 
 
 def diagonal(x, offset=0, axis1=0, axis2=1):
-    return tfnp.diagonal(
-        x,
-        offset=offset,
-        axis1=axis1,
-        axis2=axis2,
+    x = convert_to_tensor(x)
+    x_rank = x.ndim
+    if (
+        offset == 0
+        and (axis1 == x_rank - 2 or axis1 == -2)
+        and (axis2 == x_rank - 1 or axis2 == -1)
+    ):
+        return tf.linalg.diag_part(x)
+
+    x = moveaxis(x, (axis1, axis2), (-2, -1))
+    x_shape = tf.shape(x)
+
+    def _zeros():
+        return tf.zeros(tf.concat([x_shape[:-1], [0]], 0), dtype=x.dtype)
+
+    x, offset = tf.cond(
+        tf.logical_or(
+            tf.less_equal(offset, -1 * x_shape[-2]),
+            tf.greater_equal(offset, x_shape[-1]),
+        ),
+        _zeros,
+        lambda: (x, offset),
     )
+    return tf.linalg.diag_part(x, k=offset)
 
 
 def diff(a, n=1, axis=-1):
-    return tfnp.diff(a, n=n, axis=axis)
+    a = convert_to_tensor(a)
+    if n == 0:
+        return a
+    elif n < 0:
+        raise ValueError(f"Order `n` must be non-negative. Received n={n}")
+    elif a.ndim == 0:
+        raise ValueError(
+            "`diff` requires input that is at least one dimensional. "
+            f"Received: a={a}"
+        )
+    axis = canonicalize_axis(axis, a.ndim)
+    slice1 = [slice(None)] * a.ndim
+    slice2 = [slice(None)] * a.ndim
+    slice1[axis] = slice(1, None)
+    slice2[axis] = slice(None, -1)
+    slice1_tuple = tuple(slice1)
+    slice2_tuple = tuple(slice2)
+    for _ in range(n):
+        if standardize_dtype(a.dtype) == "bool":
+            a = tf.not_equal(a[slice1_tuple], a[slice2_tuple])
+        else:
+            a = tf.subtract(a[slice1_tuple], a[slice2_tuple])
+    return a
 
 
 def digitize(x, bins):
     x = convert_to_tensor(x)
     bins = list(bins)
 
     # bins must be float type
@@ -1148,33 +1252,30 @@
         return tf.abs(x1 - x2) <= (1e-08 + 1e-05 * tf.abs(x2))
     else:
         return tf.equal(x1, x2)
 
 
 @sparse.densifying_unary(True)
 def isfinite(x):
-    # `tfnp.isfinite` requires `enable_numpy_behavior`, so we reimplement it.
     x = convert_to_tensor(x)
     dtype_as_dtype = tf.as_dtype(x.dtype)
     if dtype_as_dtype.is_integer or not dtype_as_dtype.is_numeric:
         return tf.ones(x.shape, tf.bool)
     return tf.math.is_finite(x)
 
 
 def isinf(x):
-    # `tfnp.isinf` requires `enable_numpy_behavior`, so we reimplement it.
     x = convert_to_tensor(x)
     dtype_as_dtype = tf.as_dtype(x.dtype)
     if dtype_as_dtype.is_integer or not dtype_as_dtype.is_numeric:
         return tf.zeros(x.shape, tf.bool)
     return tf.math.is_inf(x)
 
 
 def isnan(x):
-    # `tfnp.isnan` requires `enable_numpy_behavior`, so we reimplement it.
     x = convert_to_tensor(x)
     dtype_as_dtype = tf.as_dtype(x.dtype)
     if dtype_as_dtype.is_integer or not dtype_as_dtype.is_numeric:
         return tf.zeros(x.shape, tf.bool)
     return tf.math.is_nan(x)
 
 
@@ -1202,23 +1303,45 @@
     if dtype is None:
         dtypes_to_resolve = [
             getattr(start, "dtype", type(start)),
             getattr(stop, "dtype", type(stop)),
             float,
         ]
         dtype = dtypes.result_type(*dtypes_to_resolve)
-    return tfnp.linspace(
-        start,
-        stop,
-        num=num,
-        endpoint=endpoint,
-        retstep=retstep,
-        dtype=dtype,
-        axis=axis,
-    )
+    else:
+        dtype = standardize_dtype(dtype)
+    start = convert_to_tensor(start, dtype=dtype)
+    stop = convert_to_tensor(stop, dtype=dtype)
+    if num < 0:
+        raise ValueError(
+            f"`num` must be a non-negative integer. Received: num={num}"
+        )
+    step = tf.convert_to_tensor(np.nan)
+    if endpoint:
+        result = tf.linspace(start, stop, num, axis=axis)
+        if num > 1:
+            step = (stop - start) / (num - 1)
+    else:
+        # tf.linspace doesn't support endpoint=False, so we manually handle it
+        if num > 0:
+            step = (stop - start) / num
+        if num > 1:
+            new_stop = tf.cast(stop, step.dtype) - step
+            start = tf.cast(start, new_stop.dtype)
+            result = tf.linspace(start, new_stop, num, axis=axis)
+        else:
+            result = tf.linspace(start, stop, num, axis=axis)
+    if dtype is not None:
+        if "int" in dtype:
+            result = tf.floor(result)
+        result = tf.cast(result, dtype)
+    if retstep:
+        return (result, step)
+    else:
+        return result
 
 
 @sparse.densifying_unary(-np.inf)
 def log(x):
     x = convert_to_tensor(x)
     dtype = (
         config.floatx()
@@ -1267,17 +1390,14 @@
 
 def logaddexp(x1, x2):
     x1 = convert_to_tensor(x1)
     x2 = convert_to_tensor(x2)
     dtype = dtypes.result_type(x1.dtype, x2.dtype, float)
     x1 = tf.cast(x1, dtype)
     x2 = tf.cast(x2, dtype)
-
-    # Below is the same implementation as tfnp.logaddexp using all native
-    # ops to prevent incorrect promotion of bfloat16.
     delta = x1 - x2
     return tf.where(
         tf.math.is_nan(delta),
         x1 + x2,
         tf.maximum(x1, x2) + tf.math.log1p(tf.math.exp(-tf.abs(delta))),
     )
 
@@ -1296,32 +1416,23 @@
 def logical_or(x1, x2):
     x1 = tf.cast(x1, "bool")
     x2 = tf.cast(x2, "bool")
     return tf.logical_or(x1, x2)
 
 
 def logspace(start, stop, num=50, endpoint=True, base=10, dtype=None, axis=0):
-    if dtype is None:
-        dtypes_to_resolve = [
-            getattr(start, "dtype", type(start)),
-            getattr(stop, "dtype", type(stop)),
-            float,
-        ]
-        dtype = dtypes.result_type(*dtypes_to_resolve)
-    start = tf.cast(start, dtype)
-    stop = tf.cast(stop, dtype)
-    return tfnp.logspace(
-        start,
-        stop,
+    result = linspace(
+        start=start,
+        stop=stop,
         num=num,
         endpoint=endpoint,
-        base=base,
         dtype=dtype,
         axis=axis,
     )
+    return tf.pow(tf.cast(base, result.dtype), result)
 
 
 @sparse.elementwise_binary_union(tf.sparse.maximum, densify_mixed=True)
 def maximum(x1, x2):
     if not isinstance(x1, (int, float)):
         x1 = convert_to_tensor(x1)
     if not isinstance(x2, (int, float)):
@@ -1341,32 +1452,40 @@
 
 def meshgrid(*x, indexing="xy"):
     return tf.meshgrid(*x, indexing=indexing)
 
 
 def min(x, axis=None, keepdims=False, initial=None):
     x = convert_to_tensor(x)
+
     # The TensorFlow numpy API implementation doesn't support `initial` so we
     # handle it manually here.
     if initial is not None:
-        return tf.math.minimum(
-            tfnp.min(x, axis=axis, keepdims=keepdims), initial
-        )
+        if standardize_dtype(x.dtype) == "bool":
+            x = tf.reduce_all(x, axis=axis, keepdims=keepdims)
+            x = tf.math.minimum(tf.cast(x, "int32"), tf.cast(initial, "int32"))
+            return tf.cast(x, "bool")
+        else:
+            x = tf.reduce_min(x, axis=axis, keepdims=keepdims)
+        return tf.math.minimum(x, initial)
 
     # TensorFlow returns inf by default for an empty list, but for consistency
     # with other backends and the numpy API we want to throw in this case.
     if tf.executing_eagerly():
         size_x = size(x)
         tf.assert_greater(
             size_x,
             tf.constant(0, dtype=size_x.dtype),
             message="Cannot compute the min of an empty tensor.",
         )
 
-    return tfnp.min(x, axis=axis, keepdims=keepdims)
+    if standardize_dtype(x.dtype) == "bool":
+        return tf.reduce_all(x, axis=axis, keepdims=keepdims)
+    else:
+        return tf.reduce_min(x, axis=axis, keepdims=keepdims)
 
 
 @sparse.elementwise_binary_union(tf.sparse.minimum, densify_mixed=True)
 def minimum(x1, x2):
     if not isinstance(x1, (int, float)):
         x1 = convert_to_tensor(x1)
     if not isinstance(x2, (int, float)):
@@ -1388,15 +1507,32 @@
         dtype = "int32"
     x1 = tf.cast(x1, dtype)
     x2 = tf.cast(x2, dtype)
     return tf.math.mod(x1, x2)
 
 
 def moveaxis(x, source, destination):
-    return tfnp.moveaxis(x, source=source, destination=destination)
+    x = convert_to_tensor(x)
+
+    _source = to_tuple_or_list(source)
+    _destination = to_tuple_or_list(destination)
+    _source = tuple(canonicalize_axis(i, x.ndim) for i in _source)
+    _destination = tuple(canonicalize_axis(i, x.ndim) for i in _destination)
+    if len(_source) != len(_destination):
+        raise ValueError(
+            "Inconsistent number of `source` and `destination`. "
+            f"Received: source={source}, destination={destination}"
+        )
+    # Directly return x if no movement is required
+    if _source == _destination:
+        return x
+    perm = [i for i in range(x.ndim) if i not in _source]
+    for dest, src in sorted(zip(_destination, _source)):
+        perm.insert(dest, src)
+    return tf.transpose(x, perm)
 
 
 def nan_to_num(x):
     x = convert_to_tensor(x)
 
     dtype = x.dtype
     dtype_as_dtype = tf.as_dtype(dtype)
@@ -1611,16 +1747,14 @@
 @sparse.densifying_unary(np.inf)
 def reciprocal(x):
     x = convert_to_tensor(x)
     return tf.math.reciprocal(x)
 
 
 def repeat(x, repeats, axis=None):
-    # tfnp.repeat has trouble with dynamic Tensors in compiled function.
-    # tf.repeat does not.
     x = convert_to_tensor(x)
     # TODO: tf.repeat doesn't support uint16
     if standardize_dtype(x.dtype) == "uint16":
         x = tf.cast(x, "uint32")
         return tf.cast(tf.repeat(x, repeats, axis=axis), "uint16")
     return tf.repeat(x, repeats, axis=axis)
 
@@ -1636,15 +1770,22 @@
         output = tf.sparse.reshape(x, newshape)
         output.set_shape(output_shape)
         return output
     return tf.reshape(x, newshape)
 
 
 def roll(x, shift, axis=None):
-    return tfnp.roll(x, shift, axis=axis)
+    x = convert_to_tensor(x)
+    if axis is not None:
+        return tf.roll(x, shift=shift, axis=axis)
+
+    # If axis is None, the roll happens as a 1-d tensor.
+    original_shape = tf.shape(x)
+    x = tf.roll(tf.reshape(x, [-1]), shift, 0)
+    return tf.reshape(x, original_shape)
 
 
 @sparse.elementwise_unary
 def sign(x):
     x = convert_to_tensor(x)
     ori_dtype = standardize_dtype(x.dtype)
     # TODO: tf.sign doesn't support uint8, uint16, uint32
@@ -1691,22 +1832,20 @@
     return tf.sort(x, axis=axis)
 
 
 def split(x, indices_or_sections, axis=0):
     if not isinstance(indices_or_sections, int):
         # `tf.split` requires `num_or_size_splits`, so we need to convert
         # `indices_or_sections` to the appropriate format.
-        # The following implementation offers better compatibility for the
-        # tensor argument `indices_or_sections` than original `tfnp.split`.
         total_size = x.shape[axis]
         indices_or_sections = convert_to_tensor(indices_or_sections)
         start_size = indices_or_sections[0:1]
         end_size = total_size - indices_or_sections[-1:]
         num_or_size_splits = tf.concat(
-            [start_size, tfnp.diff(indices_or_sections), end_size], axis=0
+            [start_size, diff(indices_or_sections), end_size], axis=0
         )
     else:
         num_or_size_splits = indices_or_sections
     return tf.split(x, num_or_size_splits, axis=axis)
 
 
 def stack(x, axis=0):
@@ -1722,51 +1861,135 @@
     ori_dtype = standardize_dtype(x.dtype)
     if "int" in ori_dtype or ori_dtype == "bool":
         x = tf.cast(x, config.floatx())
     return tf.math.reduce_std(x, axis=axis, keepdims=keepdims)
 
 
 def swapaxes(x, axis1, axis2):
-    return tfnp.swapaxes(x, axis1=axis1, axis2=axis2)
+    x = convert_to_tensor(x)
+
+    if (
+        x.shape.rank is not None
+        and isinstance(axis1, int)
+        and isinstance(axis2, int)
+    ):
+        # This branch makes sure `perm` is statically known, to avoid a
+        # not-compile-time-constant XLA error.
+        axis1 = canonicalize_axis(axis1, x.ndim)
+        axis2 = canonicalize_axis(axis2, x.ndim)
+
+        # Directly return x if no movement is required
+        if axis1 == axis2:
+            return x
+
+        perm = list(range(x.ndim))
+        perm[axis1] = axis2
+        perm[axis2] = axis1
+    else:
+        x_rank = tf.rank(x)
+        axis1 = tf.where(axis1 < 0, tf.add(axis1, x_rank), axis1)
+        axis2 = tf.where(axis2 < 0, tf.add(axis2, x_rank), axis2)
+        perm = tf.range(x_rank)
+        perm = tf.tensor_scatter_nd_update(
+            perm, [[axis1], [axis2]], [axis2, axis1]
+        )
+    return tf.transpose(x, perm)
 
 
 def take(x, indices, axis=None):
     if isinstance(indices, tf.SparseTensor):
         if x.dtype not in (tf.float16, tf.float32, tf.float64, tf.bfloat16):
             warnings.warn(
                 "`take` with the TensorFlow backend does not support "
                 f"`x.dtype={x.dtype}` when `indices` is a sparse tensor; "
                 "densifying `indices`."
             )
-            return tfnp.take(
-                x, convert_to_tensor(indices, sparse=False), axis=axis
-            )
+            return take(x, convert_to_tensor(indices, sparse=False), axis=axis)
         if axis is None:
             x = tf.reshape(x, (-1,))
         elif axis != 0:
             warnings.warn(
                 "`take` with the TensorFlow backend does not support "
                 f"`axis={axis}` when `indices` is a sparse tensor; "
                 "densifying `indices`."
             )
-            return tfnp.take(
-                x, convert_to_tensor(indices, sparse=False), axis=axis
-            )
+            return take(x, convert_to_tensor(indices, sparse=False), axis=axis)
         output = tf.nn.safe_embedding_lookup_sparse(
             embedding_weights=tf.convert_to_tensor(x),
             sparse_ids=tf.sparse.expand_dims(indices, axis=-1),
             default_id=0,
         )
         output.set_shape(indices.shape + output.shape[len(indices.shape) :])
         return output
-    return tfnp.take(x, indices, axis=axis)
+
+    x = convert_to_tensor(x)
+    indices = convert_to_tensor(indices)
+    if axis is None:
+        x = tf.reshape(x, [-1])
+        axis = 0
+    # Correct the indices using "fill" mode which is the same as in jax
+    indices = tf.where(
+        indices < 0,
+        indices + tf.cast(tf.shape(x)[axis], indices.dtype),
+        indices,
+    )
+    return tf.gather(x, indices, axis=axis)
 
 
 def take_along_axis(x, indices, axis=None):
-    return tfnp.take_along_axis(x, indices, axis=axis)
+    x = convert_to_tensor(x)
+    indices = convert_to_tensor(indices, "int64")
+    if axis is None:
+        if indices.ndim != 1:
+            raise ValueError(
+                "`indices` must be 1D if axis=None. "
+                f"Received: indices.shape={indices.shape}"
+            )
+        return take_along_axis(tf.reshape(x, [-1]), indices, 0)
+    rank = tf.rank(x)
+    static_axis = axis
+    axis = axis + rank if axis < 0 else axis
+
+    # Broadcast shapes to match, ensure that the axis of interest is not
+    # broadcast.
+    x_shape_original = tf.shape(x, out_type=indices.dtype)
+    indices_shape_original = tf.shape(indices, out_type=indices.dtype)
+    x_shape = tf.tensor_scatter_nd_update(x_shape_original, [[axis]], [1])
+    indices_shape = tf.tensor_scatter_nd_update(
+        indices_shape_original, [[axis]], [1]
+    )
+    broadcasted_shape = tf.broadcast_dynamic_shape(x_shape, indices_shape)
+    x_shape = tf.tensor_scatter_nd_update(
+        broadcasted_shape, [[axis]], [x_shape_original[axis]]
+    )
+    indices_shape = tf.tensor_scatter_nd_update(
+        broadcasted_shape, [[axis]], [indices_shape_original[axis]]
+    )
+    x = tf.broadcast_to(x, x_shape)
+    indices = tf.broadcast_to(indices, indices_shape)
+
+    # Save indices shape so we can restore it later.
+    possible_result_shape = indices.shape
+
+    # Correct the indices using "fill" mode which is the same as in jax
+    indices = tf.where(indices < 0, indices + x_shape[static_axis], indices)
+
+    x = swapaxes(x, static_axis, -1)
+    indices = swapaxes(indices, static_axis, -1)
+
+    x_shape = tf.shape(x)
+    x = tf.reshape(x, [-1, x_shape[-1]])
+    indices_shape = tf.shape(indices)
+    indices = tf.reshape(indices, [-1, indices_shape[-1]])
+
+    result = tf.gather(x, indices, batch_dims=1)
+    result = tf.reshape(result, indices_shape)
+    result = swapaxes(result, static_axis, -1)
+    result.set_shape(possible_result_shape)
+    return result
 
 
 @sparse.elementwise_unary
 def tan(x):
     x = convert_to_tensor(x)
     if standardize_dtype(x.dtype) == "int64":
         dtype = config.floatx()
@@ -1796,15 +2019,14 @@
     x1 = tf.cast(x1, compute_dtype)
     x2 = tf.cast(x2, compute_dtype)
     return tf.cast(tf.tensordot(x1, x2, axes=axes), dtype=result_dtype)
 
 
 @sparse.elementwise_unary
 def round(x, decimals=0):
-    # `tfnp.round` requires `enable_numpy_behavior`, so we reimplement it.
     if decimals == 0:
         return tf.round(x)
     x_dtype = x.dtype
     if tf.as_dtype(x_dtype).is_integer:
         # int
         if decimals > 0:
             return x
@@ -1817,15 +2039,14 @@
     x = tf.multiply(x, factor)
     x = tf.round(x)
     x = tf.divide(x, factor)
     return tf.cast(x, x_dtype)
 
 
 def tile(x, repeats):
-    # The TFNP implementation is buggy, we roll our own.
     x = convert_to_tensor(x)
     repeats = tf.reshape(convert_to_tensor(repeats, dtype="int32"), [-1])
     repeats_size = tf.size(repeats)
     repeats = tf.pad(
         repeats,
         [[tf.maximum(x.shape.rank - repeats_size, 0), 0]],
         constant_values=1,
@@ -1840,20 +2061,47 @@
 
 
 def trace(x, offset=0, axis1=0, axis2=1):
     x = convert_to_tensor(x)
     dtype = standardize_dtype(x.dtype)
     if dtype not in ("int64", "uint32", "uint64"):
         dtype = dtypes.result_type(dtype, "int32")
-    return tfnp.trace(x, offset=offset, axis1=axis1, axis2=axis2, dtype=dtype)
+    x_shape = tf.shape(x)
+    x = moveaxis(x, (axis1, axis2), (-2, -1))
+    # Mask out the diagonal and reduce.
+    x = tf.where(
+        eye(x_shape[axis1], x_shape[axis2], k=offset, dtype="bool"),
+        x,
+        tf.zeros_like(x),
+    )
+    # The output dtype is set to "int32" if the input dtype is "bool"
+    if standardize_dtype(x.dtype) == "bool":
+        x = tf.cast(x, "int32")
+    return tf.cast(tf.reduce_sum(x, axis=(-2, -1)), dtype)
 
 
 def tri(N, M=None, k=0, dtype=None):
-    dtype = dtype or config.floatx()
-    return tfnp.tri(N, M=M, k=k, dtype=dtype)
+    M = M if M is not None else N
+    dtype = standardize_dtype(dtype or config.floatx())
+    if k < 0:
+        lower = -k - 1
+        if lower > N:
+            r = tf.zeros([N, M], dtype=dtype)
+        else:
+            o = tf.ones([N, M], dtype="bool")
+            r = tf.cast(
+                tf.logical_not(tf.linalg.band_part(o, lower, -1)), dtype=dtype
+            )
+    else:
+        o = tf.ones([N, M], dtype=dtype)
+        if k > M:
+            r = o
+        else:
+            r = tf.linalg.band_part(o, -1, k)
+    return r
 
 
 def tril(x, k=0):
     x = convert_to_tensor(x)
 
     if k >= 0:
         return tf.linalg.band_part(x, -1, k)
@@ -2065,15 +2313,37 @@
             x, axis=axis, keepdims=keepdims, output_is_sparse=True
         )
     return tf.reduce_sum(x, axis=axis, keepdims=keepdims)
 
 
 def eye(N, M=None, k=0, dtype=None):
     dtype = dtype or config.floatx()
-    return tfnp.eye(N, M=M, k=k, dtype=dtype)
+    if not M:
+        M = N
+    # Making sure N, M and k are `int`
+    N, M, k = int(N), int(M), int(k)
+    if k >= M or -k >= N:
+        # tf.linalg.diag will raise an error in this case
+        return zeros([N, M], dtype=dtype)
+    if k == 0:
+        return tf.eye(N, M, dtype=dtype)
+    # We need the precise length, otherwise tf.linalg.diag will raise an error
+    diag_len = builtins.min(N, M)
+    if k > 0:
+        if N >= M:
+            diag_len -= k
+        elif N + k > M:
+            diag_len = M - k
+    elif k <= 0:
+        if M >= N:
+            diag_len += k
+        elif M - k > N:
+            diag_len = N + k
+    diagonal_ = tf.ones([diag_len], dtype=dtype)
+    return tf.linalg.diag(diagonal=diagonal_, num_rows=N, num_cols=M, k=k)
 
 
 def floor_divide(x1, x2):
     if not isinstance(x1, (int, float)):
         x1 = convert_to_tensor(x1)
     if not isinstance(x2, (int, float)):
         x2 = convert_to_tensor(x2)
@@ -2128,7 +2398,11 @@
 
         return tf.squeeze(tf.nn.conv1d(x1, x2, stride=1, padding="SAME"))
 
     x1 = tf.reshape(x1, (1, x1_len, 1))
     x2 = tf.reshape(x2, (x2_len, 1, 1))
 
     return tf.squeeze(tf.nn.conv1d(x1, x2, stride=1, padding=mode.upper()))
+
+
+def select(condlist, choicelist, default=0):
+    return tf.experimental.numpy.select(condlist, choicelist, default=default)
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/optimizer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/optimizer_distribute_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/optimizer_distribute_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/random.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/random.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import tensorflow as tf
-from tensorflow.experimental import numpy as tfnp
 
 from keras.src.backend.common import standardize_dtype
 from keras.src.backend.config import floatx
 from keras.src.random.seed_generator import SeedGenerator
 from keras.src.random.seed_generator import draw_seed
 from keras.src.random.seed_generator import make_default_seed
 
@@ -83,20 +82,22 @@
         rate=rate,
         noise_shape=noise_shape,
         seed=seed,
     )
 
 
 def shuffle(x, axis=0, seed=None):
+    from keras.src.backend.tensorflow.numpy import swapaxes
+
     seed = tf_draw_seed(seed)
     if axis == 0:
         return tf.random.experimental.stateless_shuffle(x, seed=seed)
-    x = tfnp.swapaxes(x, axis1=0, axis2=axis)
+    x = swapaxes(x, axis1=0, axis2=axis)
     x = tf.random.experimental.stateless_shuffle(x, seed=seed)
-    x = tfnp.swapaxes(x, axis1=0, axis2=axis)
+    x = swapaxes(x, axis1=0, axis2=axis)
     return x
 
 
 def gamma(shape, alpha, dtype=None, seed=None):
     dtype = dtype or floatx()
     seed = tf_draw_seed(seed)
     # TODO: `tf.random.stateless_gamma` doesn't support bfloat16
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/rnn.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/saved_model_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/saved_model_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/sparse.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/trackable.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/tensorflow/trainer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/tensorflow/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/core.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/image.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/layer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/linalg.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/math.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/nn.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/numpy.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,16 +168,19 @@
         result = torch.max(x)
     else:
         result = amax(x, axis=axis, keepdims=keepdims)
     if isinstance(getattr(result, "values", None), torch.Tensor):
         result = result.values
 
     if initial is not None:
-        initial = convert_to_tensor(initial)
-        return torch.maximum(result, torch.full(result.shape, initial))
+        dtype = to_torch_dtype(result.dtype)
+        initial = convert_to_tensor(initial, dtype=dtype)
+        return torch.maximum(
+            result, torch.full(result.shape, initial, dtype=dtype)
+        )
     return result
 
 
 def ones(shape, dtype=None):
     dtype = to_torch_dtype(dtype or config.floatx())
     if isinstance(shape, int):
         shape = (shape,)
@@ -194,25 +197,25 @@
 def zeros_like(x, dtype=None):
     x = convert_to_tensor(x)
     dtype = to_torch_dtype(dtype or x.dtype)
     return torch.zeros_like(x, dtype=dtype)
 
 
 def absolute(x):
-    return abs(x)
-
-
-def abs(x):
     x = convert_to_tensor(x)
     # bool are always non-negative
     if standardize_dtype(x.dtype) == "bool":
         return x
     return torch.abs(x)
 
 
+def abs(x):
+    return absolute(x)
+
+
 def all(x, axis=None, keepdims=False):
     x = convert_to_tensor(x)
     if axis is None:
         return cast(torch.all(x), "bool")
     axis = to_tuple_or_list(axis)
     for a in axis:
         # `torch.all` does not handle multiple axes.
@@ -740,16 +743,23 @@
             getattr(start, "dtype", type(start)),
             getattr(stop, "dtype", type(stop)),
             float,
         ]
         dtype = dtypes.result_type(*dtypes_to_resolve)
     dtype = to_torch_dtype(dtype)
 
-    if endpoint is False:
-        stop = stop - ((stop - start) / num)
+    step = convert_to_tensor(torch.nan)
+    if endpoint:
+        if num > 1:
+            step = (stop - start) / (num - 1)
+    else:
+        if num > 0:
+            step = (stop - start) / num
+        if num > 1:
+            stop = stop - ((stop - start) / num)
     if hasattr(start, "__len__") and hasattr(stop, "__len__"):
         start = convert_to_tensor(start, dtype=dtype)
         stop = convert_to_tensor(stop, dtype=dtype)
         steps = torch.arange(num, dtype=dtype, device=get_device()) / (num - 1)
 
         # reshape `steps` to allow for broadcasting
         for i in range(start.ndim):
@@ -762,15 +772,15 @@
             start=start,
             end=stop,
             steps=num,
             dtype=dtype,
             device=get_device(),
         )
     if retstep is True:
-        return (linspace, num)
+        return (linspace, step)
     return linspace
 
 
 def log(x):
     x = convert_to_tensor(x)
     return torch.log(x)
 
@@ -945,15 +955,16 @@
     else:
         result = amin(x, axis=axis, keepdims=keepdims)
 
     if isinstance(getattr(result, "values", None), torch.Tensor):
         result = result.values
 
     if initial is not None:
-        initial = convert_to_tensor(initial)
+        dtype = to_torch_dtype(result.dtype)
+        initial = convert_to_tensor(initial, dtype=dtype)
         return torch.minimum(result, initial)
     return result
 
 
 def minimum(x1, x2):
     if not isinstance(x1, (int, float)):
         x1 = convert_to_tensor(x1)
@@ -1261,14 +1272,21 @@
     x = convert_to_tensor(x)
     return torch.swapaxes(x, axis0=axis1, axis1=axis2)
 
 
 def take(x, indices, axis=None):
     x = convert_to_tensor(x)
     indices = convert_to_tensor(indices).long()
+    # Correct the indices using "fill" mode which is the same as in jax
+    x_dim = x.shape[axis] if axis is not None else x.shape[0]
+    indices = torch.where(
+        indices < 0,
+        indices + x_dim,
+        indices,
+    )
     if x.ndim == 2 and axis == 0:
         # This case is equivalent to embedding lookup.
         return torch.nn.functional.embedding(indices, x)
     if axis is None:
         x = torch.reshape(x, (-1,))
         axis = 0
     if axis is not None:
@@ -1281,14 +1299,21 @@
         return out.reshape(shape)
     return torch.take(x, index=indices)
 
 
 def take_along_axis(x, indices, axis=None):
     x = convert_to_tensor(x)
     indices = convert_to_tensor(indices).long()
+    # Correct the indices using "fill" mode which is the same as in jax
+    x_dim = x.shape[axis] if axis is not None else x.shape[0]
+    indices = torch.where(
+        indices < 0,
+        indices + x_dim,
+        indices,
+    )
     return torch.take_along_dim(x, indices, dim=axis)
 
 
 def tan(x):
     x = convert_to_tensor(x)
     return torch.tan(x)
 
@@ -1563,7 +1588,16 @@
         result = result[..., start_idx : start_idx + target_length]
 
     if mode == "same":
         start_idx = (result.size(-1) - x1_len) // 2
         result = result[..., start_idx : start_idx + x1_len]
 
     return torch.squeeze(result)
+
+
+def select(condlist, choicelist, default=0):
+    condlist = [convert_to_tensor(c) for c in condlist]
+    choicelist = [convert_to_tensor(c) for c in choicelist]
+    out = convert_to_tensor(default)
+    for c, v in reversed(list(zip(condlist, choicelist))):
+        out = torch.where(c, v, out)
+    return out
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_adam.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_lion.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/random.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/rnn.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/backend/torch/trainer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/backend/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/backup_and_restore.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/backup_and_restore_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/backup_and_restore_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/callback.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/callback_list.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/callback_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/callback_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/csv_logger.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/csv_logger_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/csv_logger_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/early_stopping.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/early_stopping_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/early_stopping_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/history.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/lambda_callback.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/lambda_callback_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/lambda_callback_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/learning_rate_scheduler.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/learning_rate_scheduler_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/learning_rate_scheduler_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/model_checkpoint.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/model_checkpoint_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/model_checkpoint_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/progbar_logger.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/reduce_lr_on_plateau_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/reduce_lr_on_plateau_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/remote_monitor.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/remote_monitor_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/remote_monitor_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/swap_ema_weights.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/swap_ema_weights_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/swap_ema_weights_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/tensorboard.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/tensorboard_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/tensorboard_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/terminate_on_nan.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/callbacks/terminate_on_nan_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/callbacks/terminate_on_nan_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/constraints/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/constraints/constraints.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/constraints/constraints_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/constraints/constraints_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/datasets/boston_housing.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/datasets/california_housing.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/datasets/cifar.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/datasets/cifar10.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/datasets/cifar100.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/datasets/fashion_mnist.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/datasets/imdb.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/datasets/mnist.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/datasets/reuters.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/distribution/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/distribution/distribution_lib.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/distribution/distribution_lib_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/distribution/distribution_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/dtype_policies/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/dtype_policies/dtype_policy.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/dtype_policies/dtype_policy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/dtype_policies/dtype_policy_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/dtype_policies/dtype_policy_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/export/export_lib.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/export/export_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/export/export_lib_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/export/export_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/initializers/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/initializers/constant_initializers.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/initializers/constant_initializers_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/initializers/constant_initializers_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/initializers/initializer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/initializers/random_initializers.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/initializers/random_initializers_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/initializers/random_initializers_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/activation.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/activation_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/activation_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/elu.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/elu_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/elu_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/leaky_relu.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/leaky_relu_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/leaky_relu_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/prelu.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/prelu_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/prelu_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/relu.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/relu_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/relu_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/softmax.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/activations/softmax_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/activations/softmax_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/additive_attention.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/additive_attention_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/additive_attention_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/attention.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/attention_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/attention_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/grouped_query_attention.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/grouped_query_attention_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/grouped_query_attention_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/multi_head_attention.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/attention/multi_head_attention_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/attention/multi_head_attention_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/base_conv.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/base_conv_transpose.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/base_separable_conv.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv1d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv1d_transpose.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv2d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv2d_transpose.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv3d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv3d_transpose.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/conv_transpose_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/conv_transpose_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/depthwise_conv_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/depthwise_conv_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/separable_conv1d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/separable_conv2d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/convolutional/separable_conv_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/convolutional/separable_conv_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/dense.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/dense.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/dense_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/dense_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/einsum_dense.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/einsum_dense.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/einsum_dense_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/einsum_dense_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/embedding.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/embedding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/embedding_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/embedding_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/identity.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/identity_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/identity_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/input_layer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/input_layer_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/input_layer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/lambda_layer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/lambda_layer_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/lambda_layer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/masking.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/masking_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/masking_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/wrapper.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/core/wrapper_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/core/wrapper_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/input_spec.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/input_spec.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/layer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/layer_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/layer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/add.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/average.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/base_merge.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/concatenate.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/dot.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/maximum.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/merging_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/merging_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/minimum.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/multiply.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/merging/subtract.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/batch_normalization.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/batch_normalization_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/batch_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/group_normalization.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/group_normalization_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/group_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/layer_normalization.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/layer_normalization_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/layer_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/spectral_normalization.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/spectral_normalization_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/spectral_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/unit_normalization.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/normalization/unit_normalization_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/normalization/unit_normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/average_pooling1d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/average_pooling2d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/average_pooling3d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/average_pooling_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/average_pooling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/base_global_pooling.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/base_pooling.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_average_pooling1d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_average_pooling2d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_average_pooling3d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_average_pooling_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_average_pooling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_max_pooling1d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_max_pooling2d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_max_pooling3d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/global_max_pooling_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/global_max_pooling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/max_pooling1d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/max_pooling2d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/max_pooling3d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/pooling/max_pooling_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/pooling/max_pooling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/audio_preprocessing_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/audio_preprocessing_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/category_encoding.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/category_encoding_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/category_encoding_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/center_crop.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/center_crop_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/center_crop_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/discretization.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/discretization_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/discretization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/feature_space.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/feature_space.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/feature_space_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/feature_space_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/hashed_crossing.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/hashed_crossing_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/hashed_crossing_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/hashing.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/hashing_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/hashing_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/index_lookup.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/index_lookup_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/index_lookup_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/integer_lookup.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/integer_lookup_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/integer_lookup_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/normalization.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/normalization_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/normalization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_brightness.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_brightness_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_brightness_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_contrast.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_contrast_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_contrast_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_crop.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_crop_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_crop_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_flip.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_flip_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_flip_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_rotation.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_rotation_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_rotation_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_translation.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_translation_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_translation_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_zoom.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/random_zoom_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/random_zoom_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/rescaling.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/rescaling_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/rescaling_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/resizing.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/resizing_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/resizing_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/string_lookup.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/string_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/string_lookup_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/string_lookup_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/text_vectorization.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/text_vectorization_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/text_vectorization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/preprocessing/tf_data_layer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/activity_regularization.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/activity_regularization_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/activity_regularization_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/alpha_dropout.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/alpha_dropout_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/alpha_dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/dropout.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/dropout_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/gaussian_dropout.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/gaussian_dropout_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/gaussian_dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/gaussian_noise.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/gaussian_noise_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/gaussian_noise_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/spatial_dropout.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/regularization/spatial_dropout_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/regularization/spatial_dropout_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping1d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping1d_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping1d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping2d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping2d_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping2d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping3d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/cropping3d_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/cropping3d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/flatten.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/flatten_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/flatten_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/permute.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/permute_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/permute_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/repeat_vector.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/repeat_vector_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/repeat_vector_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/reshape.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/reshape_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/reshape_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling1d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling1d_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling1d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling2d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling2d_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling2d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling3d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/up_sampling3d_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/up_sampling3d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding1d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding1d_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding1d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding2d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding2d_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding2d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding3d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/reshaping/zero_padding3d_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/reshaping/zero_padding3d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/bidirectional.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/bidirectional_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/bidirectional_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm1d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm1d_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm1d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm2d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm2d_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm2d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm3d.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm3d_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm3d_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/conv_lstm_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/conv_lstm_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/dropout_rnn_cell_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/dropout_rnn_cell_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/gru.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/gru_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/gru_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/lstm.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/lstm_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/lstm_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/rnn.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/rnn_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/rnn_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/simple_rnn.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/simple_rnn_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/simple_rnn_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/stacked_rnn_cells_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/stacked_rnn_cells_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/time_distributed.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/layers/rnn/time_distributed_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/layers/rnn/time_distributed_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/backend.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/layers.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/losses.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/preprocessing/image.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/preprocessing/sequence.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/preprocessing/text.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/json_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/json_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/json_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/legacy_h5_format.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/legacy_h5_format_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/legacy_h5_format_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/saving_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/legacy/saving/serialization.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/losses/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/losses/loss.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/losses/loss.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/losses/loss_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/losses/loss_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/losses/losses.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/losses/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/losses/losses_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/losses/losses_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/accuracy_metrics.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/accuracy_metrics_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/accuracy_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/confusion_metrics.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/confusion_metrics_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/confusion_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/f_score_metrics.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/f_score_metrics_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/f_score_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/hinge_metrics.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/hinge_metrics_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/hinge_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/iou_metrics.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/iou_metrics_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/iou_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/metric.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/metric_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/metric_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/metrics_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/probabilistic_metrics.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/probabilistic_metrics_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/probabilistic_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/reduction_metrics.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/reduction_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/reduction_metrics_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/reduction_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/regression_metrics.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/metrics/regression_metrics_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/metrics/regression_metrics_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/models/cloning.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/models/cloning.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/models/cloning_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/models/cloning_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/models/functional.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/models/functional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/models/functional_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/models/functional_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/models/model.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/models/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import inspect
+import io
 import json
 import typing
 import warnings
 
+import keras.src.saving.saving_lib as saving_lib
 from keras.src import backend
 from keras.src import utils
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
 from keras.src.models.variable_mapping import map_trackable_variables
 from keras.src.saving import saving_api
 from keras.src.trainers import trainer as base_trainer
@@ -344,14 +346,38 @@
                 there is a mismatch in the number of weights, or a mismatch in
                 the shape of the weights.
         """
         saving_api.load_weights(
             self, filepath, skip_mismatch=skip_mismatch, **kwargs
         )
 
+    # Note: renaming this function will cause old pickles to be broken.
+    # This is probably not a huge deal, as pickle should not be a recommended
+    # saving format -- it should only be supported for use with distributed
+    # computing frameworks.
+    @classmethod
+    def _unpickle_model(cls, bytesio):
+        # pickle is not safe regardless of what you do.
+        return saving_lib._load_model_from_fileobj(
+            bytesio, custom_objects=None, compile=True, safe_mode=False
+        )
+
+    def __reduce__(self):
+        """__reduce__ is used to customize the behavior of `pickle.pickle()`.
+
+        The method returns a tuple of two elements: a function, and a list of
+        arguments to pass to that function.  In this case we just leverage the
+        keras saving library."""
+        buf = io.BytesIO()
+        saving_lib._save_model_to_fileobj(self, buf, "h5")
+        return (
+            self._unpickle_model,
+            (buf,),
+        )
+
     def quantize(self, mode):
         """Quantize the weights of the model.
 
         Note that the model must be built first before calling this method.
         `quantize` will recursively call `quantize(mode)` in all layers and
         will be skipped if the layer doesn't implement the function.
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/models/model_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/models/model_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pickle
+
 import numpy as np
 import pytest
 from absl.testing import parameterized
 
 from keras.src import backend
 from keras.src import layers
 from keras.src import testing
@@ -113,14 +115,37 @@
 
         new_model = Model.from_config(
             config, custom_objects={"CustomDense": CustomDense}
         )
         self.assertIsInstance(new_model, Functional)
 
     @parameterized.named_parameters(
+        ("single_output_1", _get_model_single_output),
+        ("single_output_2", _get_model_single_output),
+        ("single_output_3", _get_model_single_output),
+        ("single_output_4", _get_model_single_output),
+        ("single_list_output_1", _get_model_single_output_list),
+        ("single_list_output_2", _get_model_single_output_list),
+        ("single_list_output_3", _get_model_single_output_list),
+        ("single_list_output_4", _get_model_single_output_list),
+    )
+    def test_functional_pickling(self, model_fn):
+        model = model_fn()
+        self.assertIsInstance(model, Functional)
+        model.compile()
+        x = np.random.rand(8, 3)
+
+        reloaded_pickle = pickle.loads(pickle.dumps(model))
+
+        pred_reloaded = reloaded_pickle.predict(x)
+        pred = model.predict(x)
+
+        self.assertAllClose(np.array(pred_reloaded), np.array(pred))
+
+    @parameterized.named_parameters(
         ("single_output_1", _get_model_single_output, None),
         ("single_output_2", _get_model_single_output, "list"),
         ("single_output_3", _get_model_single_output, "dict"),
         ("single_output_4", _get_model_single_output, "dict_list"),
         ("single_list_output_1", _get_model_single_output_list, None),
         ("single_list_output_2", _get_model_single_output_list, "list"),
         ("single_list_output_3", _get_model_single_output_list, "dict"),
@@ -134,15 +159,15 @@
         model = model_fn()
         self.assertIsInstance(model, Functional)
         loss = "mean_squared_error"
         if loss_type == "list":
             loss = [loss]
         elif loss_type == "dict":
             loss = {"output_a": loss}
-        elif loss_type == "dict_lsit":
+        elif loss_type == "dict_list":
             loss = {"output_a": [loss]}
         model.compile(
             optimizer="sgd",
             loss=loss,
             metrics={
                 "output_a": ["mean_squared_error", "mean_absolute_error"],
             },
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/models/sequential.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/models/sequential.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/models/sequential_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/models/sequential_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/models/variable_mapping.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/models/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/models/variable_mapping_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/models/variable_mapping_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/core.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/core_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/core_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/function.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/function.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/function_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/function_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/image.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/image_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/image_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/linalg.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/linalg_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/linalg_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/math.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/math_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/math_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/nn.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/nn_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/nn_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/node.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/node_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/node_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/numpy.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -5262,22 +5262,26 @@
     """
     if any_symbolic_tensors((x,)):
         return Trace(offset, axis1, axis2).symbolic_call(x)
     return backend.numpy.trace(x, offset=offset, axis1=axis1, axis2=axis2)
 
 
 class Tri(Operation):
-    def call(self, N, M=None, k=0, dtype=None):
-        return backend.numpy.tri(N, M=M, k=k, dtype=dtype)
+    def __init__(self, k=0, dtype=None):
+        super().__init__()
+        self.k = k
+        self.dtype = dtype or backend.floatx()
 
-    def compute_output_spec(self, N, M=None, k=0, dtype=None):
+    def call(self, N, M=None):
+        return backend.numpy.tri(N=N, M=M, k=self.k, dtype=self.dtype)
+
+    def compute_output_spec(self, N, M=None):
         if M is None:
             M = N
-        dtype = dtype or backend.floatx()
-        return KerasTensor((N, M), dtype=dtype)
+        return KerasTensor((N, M), dtype=self.dtype)
 
 
 @keras_export(["keras.ops.tri", "keras.ops.numpy.tri"])
 def tri(N, M=None, k=0, dtype=None):
     """Return a tensor with ones at and below a diagonal and zeros elsewhere.
 
     Args:
@@ -6017,22 +6021,26 @@
     Returns:
         Tensor of ones with the given shape and dtype.
     """
     return backend.numpy.ones(shape, dtype=dtype)
 
 
 class Eye(Operation):
-    def call(self, N, M=None, k=0, dtype=None):
-        return backend.numpy.eye(N, M=M, k=k, dtype=dtype)
+    def __init__(self, k=0, dtype=None):
+        super().__init__()
+        self.k = k
+        self.dtype = dtype or backend.floatx()
+
+    def call(self, N, M=None):
+        return backend.numpy.eye(N, M=M, k=self.k, dtype=self.dtype)
 
-    def compute_output_spec(self, N, M=None, k=0, dtype=None):
+    def compute_output_spec(self, N, M=None):
         if M is None:
             M = N
-        dtype = dtype or backend.floatx()
-        return KerasTensor((N, M), dtype=dtype)
+        return KerasTensor((N, M), dtype=self.dtype)
 
 
 @keras_export(["keras.ops.eye", "keras.ops.numpy.eye"])
 def eye(N, M=None, k=0, dtype=None):
     """Return a 2-D tensor with ones on the diagonal and zeros elsewhere.
 
     Args:
@@ -6168,7 +6176,70 @@
 
     Returns:
         Output tensor, cross-correlation of `x1` and `x2`.
     """
     if any_symbolic_tensors((x1, x2)):
         return Correlate(mode=mode).symbolic_call(x1, x2)
     return backend.numpy.correlate(x1, x2, mode=mode)
+
+
+class Select(Operation):
+    def __init__(self):
+        super().__init__()
+
+    def call(self, condlist, choicelist, default=0):
+        return backend.numpy.correlate(condlist, choicelist, default)
+
+    def compute_output_spec(self, condlist, choicelist, default=0):
+        first_element = choicelist[0]
+        return KerasTensor(first_element.shape, dtype=first_element.dtype)
+
+
+@keras_export(["keras.ops.select", "keras.ops.numpy.select"])
+def select(condlist, choicelist, default=0):
+    """Return elements from `choicelist`, based on conditions in `condlist`.
+
+    Args:
+        condlist: List of boolean tensors.
+            The list of conditions which determine from which array
+            in choicelist the output elements are taken.
+            When multiple conditions are satisfied,
+            the first one encountered in condlist is used.
+        choicelist: List of tensors.
+            The list of tensors from which the output elements are taken.
+            This list has to be of the same length as `condlist`.
+        defaults: Optional scalar value.
+            The element inserted in the output
+            when all conditions evaluate to `False`.
+
+    Returns:
+        Tensor where the output at position `m` is the `m`-th element
+        of the tensor in `choicelist` where the `m`-th element of the
+        corresponding tensor in `condlist` is `True`.
+
+    Example:
+
+    ```python
+    from keras import ops
+
+    x = ops.arange(6)
+    condlist = [x<3, x>3]
+    choicelist = [x, x**2]
+    ops.select(condlist, choicelist, 42)
+    # Returns: tensor([0,  1,  2, 42, 16, 25])
+    ```
+    """
+    if not isinstance(condlist, list) or not isinstance(choicelist, list):
+        raise ValueError(
+            "condlist and choicelist must be lists. Received: "
+            f"type(condlist) = {type(condlist)}, "
+            f"type(choicelist) = {type(choicelist)}"
+        )
+    if not condlist or not choicelist:
+        raise ValueError(
+            "condlist and choicelist must not be empty. Received: "
+            f"condlist = {condlist}, "
+            f"choicelist = {choicelist}"
+        )
+    if any_symbolic_tensors(condlist + choicelist + [default]):
+        return Select().symbolic_call(condlist, choicelist, default)
+    return backend.numpy.select(condlist, choicelist, default)
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/numpy_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/numpy_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -2166,14 +2166,22 @@
         self.assertAllClose(knp.Cross()(x1, y2), np.cross(x1, y2))
         if backend.backend() != "torch":
             # API divergence between `torch.cross` and `np.cross`
             # `torch.cross` only allows dim 3, `np.cross` allows dim 2 or 3
             self.assertAllClose(knp.Cross()(x1, y3), np.cross(x1, y3))
             self.assertAllClose(knp.Cross()(x2, y3), np.cross(x2, y3))
 
+        # Test axis is not None
+        self.assertAllClose(
+            knp.cross(x1, y1, axis=-1), np.cross(x1, y1, axis=-1)
+        )
+        self.assertAllClose(
+            knp.Cross(axis=-1)(x1, y1), np.cross(x1, y1, axis=-1)
+        )
+
     def test_einsum(self):
         x = np.arange(24).reshape([2, 3, 4]).astype("float32")
         y = np.arange(24).reshape([2, 4, 3]).astype("float32")
         self.assertAllClose(
             knp.einsum("ijk,lkj->il", x, y),
             np.einsum("ijk,lkj->il", x, y),
         )
@@ -2448,14 +2456,18 @@
             np.linspace(0, 10, 5, endpoint=False),
         )
         self.assertAllClose(knp.Linspace(num=5)(0, 10), np.linspace(0, 10, 5))
         self.assertAllClose(
             knp.Linspace(num=5, endpoint=False)(0, 10),
             np.linspace(0, 10, 5, endpoint=False),
         )
+        self.assertAllClose(
+            knp.Linspace(num=0, endpoint=False)(0, 10),
+            np.linspace(0, 10, 0, endpoint=False),
+        )
 
         start = np.zeros([2, 3, 4])
         stop = np.ones([2, 3, 4])
         self.assertAllClose(
             knp.linspace(start, stop, 5, retstep=True)[0],
             np.linspace(start, stop, 5, retstep=True)[0],
         )
@@ -2655,35 +2667,41 @@
         self.assertAllClose(knp.take(x, 0), np.take(x, 0))
         self.assertAllClose(knp.take(x, 0, axis=1), np.take(x, 0, axis=1))
 
         self.assertAllClose(knp.Take()(x, indices), np.take(x, indices))
         self.assertAllClose(knp.Take()(x, 0), np.take(x, 0))
         self.assertAllClose(knp.Take(axis=1)(x, 0), np.take(x, 0, axis=1))
 
-        # test with multi-dimensional indices
+        # Test with multi-dimensional indices
         rng = np.random.default_rng(0)
         x = rng.standard_normal((2, 3, 4, 5))
         indices = rng.integers(0, 4, (6, 7))
         self.assertAllClose(
-            knp.take(x, indices, axis=2),
-            np.take(x, indices, axis=2),
+            knp.take(x, indices, axis=2), np.take(x, indices, axis=2)
         )
 
-        # test with negative axis
+        # Test with negative axis
         self.assertAllClose(
-            knp.take(x, indices, axis=-2),
-            np.take(x, indices, axis=-2),
+            knp.take(x, indices, axis=-2), np.take(x, indices, axis=-2)
         )
-        # test with axis=None & x.ndim=2
+
+        # Test with axis=None & x.ndim=2
         x = np.array(([1, 2], [3, 4]))
         indices = np.array([2, 3])
         self.assertAllClose(
             knp.take(x, indices, axis=None), np.take(x, indices, axis=None)
         )
 
+        # Test with negative indices
+        x = rng.standard_normal((2, 3, 4, 5))
+        indices = rng.integers(-3, 0, (6, 7))
+        self.assertAllClose(
+            knp.take(x, indices, axis=2), np.take(x, indices, axis=2)
+        )
+
     @parameterized.named_parameters(
         named_product(
             [
                 {"testcase_name": "axis_none", "axis": None},
                 {"testcase_name": "axis_0", "axis": 0},
                 {"testcase_name": "axis_1", "axis": 1},
                 {"testcase_name": "axis_minus1", "axis": -1},
@@ -2740,14 +2758,38 @@
             np.take_along_axis(x, indices, axis=2),
         )
         self.assertAllClose(
             knp.TakeAlongAxis(axis=2)(x, indices),
             np.take_along_axis(x, indices, axis=2),
         )
 
+        # Test with axis=None
+        x = np.arange(12).reshape([1, 1, 3, 4])
+        indices = np.array([1, 2, 3], dtype=np.int32)
+        self.assertAllClose(
+            knp.take_along_axis(x, indices, axis=None),
+            np.take_along_axis(x, indices, axis=None),
+        )
+        self.assertAllClose(
+            knp.TakeAlongAxis(axis=None)(x, indices),
+            np.take_along_axis(x, indices, axis=None),
+        )
+
+        # Test with negative indices
+        x = np.arange(12).reshape([1, 1, 3, 4])
+        indices = np.full([1, 4, 1, 1], -1, dtype=np.int32)
+        self.assertAllClose(
+            knp.take_along_axis(x, indices, axis=2),
+            np.take_along_axis(x, indices, axis=2),
+        )
+        self.assertAllClose(
+            knp.TakeAlongAxis(axis=2)(x, indices),
+            np.take_along_axis(x, indices, axis=2),
+        )
+
     def test_tensordot(self):
         x = np.arange(24).reshape([1, 2, 3, 4]).astype("float32")
         y = np.arange(24).reshape([3, 4, 1, 2]).astype("float32")
         self.assertAllClose(
             knp.tensordot(x, y, axes=2), np.tensordot(x, y, axes=2)
         )
         self.assertAllClose(
@@ -3444,14 +3486,18 @@
 
         x = np.array([[1, 3, 6, 10], [0, 5, 6, 8]])
         self.assertAllClose(knp.diff(x), np.diff(x))
         self.assertAllClose(knp.diff(x, axis=0), np.diff(x, axis=0))
         self.assertAllClose(knp.diff(x, n=2, axis=0), np.diff(x, n=2, axis=0))
         self.assertAllClose(knp.diff(x, n=2, axis=1), np.diff(x, n=2, axis=1))
 
+        # Test n=0
+        x = np.array([1, 2, 4, 7, 0])
+        self.assertAllClose(knp.diff(x, n=0), np.diff(x, n=0))
+
     def test_dot(self):
         x = np.arange(24).reshape([2, 3, 4]).astype("float32")
         y = np.arange(12).reshape([4, 3]).astype("float32")
         z = np.arange(4).astype("float32")
         self.assertAllClose(knp.dot(x, y), np.dot(x, y))
         self.assertAllClose(knp.dot(x, z), np.dot(x, z))
         self.assertAllClose(knp.dot(x, 2), np.dot(x, 2))
@@ -3861,14 +3907,28 @@
         self.assertAllClose(knp.Roll(-1, axis=0)(x), np.roll(x, -1, axis=0))
 
     def test_round(self):
         x = np.array([[1.1, 2.5, 3.9], [3.2, 2.3, 1.8]])
         self.assertAllClose(knp.round(x), np.round(x))
         self.assertAllClose(knp.Round()(x), np.round(x))
 
+        # Test with decimal=1
+        self.assertAllClose(knp.round(x, decimals=1), np.round(x, decimals=1))
+        self.assertAllClose(knp.Round(decimals=1)(x), np.round(x, decimals=1))
+
+        # Test with integers
+        x = np.array([[1, 2, 3], [3, 2, 1]], dtype="int32")
+        self.assertAllClose(knp.round(x, decimals=1), np.round(x, decimals=1))
+        self.assertAllClose(knp.Round(decimals=1)(x), np.round(x, decimals=1))
+
+        # Test with integers and decimal < 0
+        x = np.array([[123, 234, 345], [345, 234, 123]], dtype="int32")
+        self.assertAllClose(knp.round(x, decimals=-1), np.round(x, decimals=-1))
+        self.assertAllClose(knp.Round(decimals=-1)(x), np.round(x, decimals=-1))
+
     def test_sign(self):
         x = np.array([[1, -2, 3], [-3, 2, -1]])
         self.assertAllClose(knp.sign(x), np.sign(x))
         self.assertAllClose(knp.Sign()(x), np.sign(x))
 
     def test_sin(self):
         x = np.array([[1, -2, 3], [-3, 2, -1]])
@@ -4024,14 +4084,22 @@
         self.assertAllClose(knp.Tanh()(x), np.tanh(x))
 
     def test_tile(self):
         x = np.array([[1, 2, 3], [3, 2, 1]])
         self.assertAllClose(knp.tile(x, [2, 3]), np.tile(x, [2, 3]))
         self.assertAllClose(knp.Tile([2, 3])(x), np.tile(x, [2, 3]))
 
+        # If repeats.ndim > x.ndim
+        self.assertAllClose(knp.tile(x, [2, 3, 4]), np.tile(x, [2, 3, 4]))
+        self.assertAllClose(knp.Tile([2, 3, 4])(x), np.tile(x, [2, 3, 4]))
+
+        # If repeats.ndim < x.ndim
+        self.assertAllClose(knp.tile(x, [2]), np.tile(x, [2]))
+        self.assertAllClose(knp.Tile([2])(x), np.tile(x, [2]))
+
     def test_trace(self):
         x = np.arange(24).reshape([1, 2, 3, 4])
         self.assertAllClose(knp.trace(x), np.trace(x))
         self.assertAllClose(
             knp.trace(x, axis1=2, axis2=3),
             np.trace(x, axis1=2, axis2=3),
         )
@@ -4165,14 +4233,27 @@
         self.assertAllClose(
             knp.Correlate(mode="same")(x, y), np.correlate(x, y, mode="same")
         )
         self.assertAllClose(
             knp.Correlate(mode="full")(x, y), np.correlate(x, y, mode="full")
         )
 
+    def test_select(self):
+        x = np.arange(6)
+        condlist = [x < 3, x > 3]
+        choicelist = [x, x**2]
+        y = knp.select(condlist, choicelist, 42)
+        self.assertAllClose(y, [0, 1, 2, 42, 16, 25])
+
+        x = backend.KerasTensor((6,))
+        condlist = [x < 3, x > 3]
+        choicelist = [x, x**2]
+        y = knp.select(condlist, choicelist, 42)
+        self.assertEqual(y.shape, (6,))
+
 
 class NumpyArrayCreateOpsCorrectnessTest(testing.TestCase):
     def test_ones(self):
         self.assertAllClose(knp.ones([2, 3]), np.ones([2, 3]))
         self.assertAllClose(knp.Ones()([2, 3]), np.ones([2, 3]))
 
     def test_zeros(self):
@@ -4182,15 +4263,30 @@
     def test_eye(self):
         self.assertAllClose(knp.eye(3), np.eye(3))
         self.assertAllClose(knp.eye(3, 4), np.eye(3, 4))
         self.assertAllClose(knp.eye(3, 4, 1), np.eye(3, 4, 1))
 
         self.assertAllClose(knp.Eye()(3), np.eye(3))
         self.assertAllClose(knp.Eye()(3, 4), np.eye(3, 4))
-        self.assertAllClose(knp.Eye()(3, 4, 1), np.eye(3, 4, 1))
+        self.assertAllClose(knp.Eye(k=1)(3, 4), np.eye(3, 4, k=1))
+
+        # Test k >= N
+        self.assertAllClose(knp.Eye(k=3)(3), np.eye(3, k=3))
+
+        # Test k > 0 and N >= M
+        self.assertAllClose(knp.Eye(k=1)(3), np.eye(3, k=1))
+
+        # Test k > 0 and N < M and N + k > M
+        self.assertAllClose(knp.Eye(k=2)(3, 4), np.eye(3, 4, k=2))
+
+        # Test k < 0 and M >= N
+        self.assertAllClose(knp.Eye(k=-1)(3), np.eye(3, k=-1))
+
+        # Test k < 0 and M < N and M - k > N
+        self.assertAllClose(knp.Eye(k=-2)(4, 3), np.eye(4, 3, k=-2))
 
     def test_arange(self):
         self.assertAllClose(knp.arange(3), np.arange(3))
         self.assertAllClose(knp.arange(3, 7), np.arange(3, 7))
         self.assertAllClose(knp.arange(3, 7, 2), np.arange(3, 7, 2))
 
         self.assertAllClose(knp.Arange()(3), np.arange(3))
@@ -4224,15 +4320,24 @@
     def test_tri(self):
         self.assertAllClose(knp.tri(3), np.tri(3))
         self.assertAllClose(knp.tri(3, 4), np.tri(3, 4))
         self.assertAllClose(knp.tri(3, 4, 1), np.tri(3, 4, 1))
 
         self.assertAllClose(knp.Tri()(3), np.tri(3))
         self.assertAllClose(knp.Tri()(3, 4), np.tri(3, 4))
-        self.assertAllClose(knp.Tri()(3, 4, 1), np.tri(3, 4, 1))
+        self.assertAllClose(knp.Tri(k=1)(3, 4), np.tri(3, 4, 1))
+
+        # Test k < 0
+        self.assertAllClose(knp.Tri(k=-1)(3), np.tri(3, k=-1))
+
+        # Test -k-1 > N
+        self.assertAllClose(knp.Tri(k=-5)(3), np.tri(3, k=-5))
+
+        # Test k > M
+        self.assertAllClose(knp.Tri(k=4)(3), np.tri(3, k=4))
 
 
 def create_sparse_tensor(x, indices_from=None, start=0, delta=2):
     if indices_from is not None:
         indices = indices_from.indices
     else:
         size = math.prod(x.shape)
@@ -5070,14 +5175,26 @@
         x = knp.ones((1,), dtype=dtype)
         x_jax = jnp.ones((1,), dtype=dtype)
         expected_dtype = standardize_dtype(jnp.max(x_jax).dtype)
 
         self.assertEqual(standardize_dtype(knp.max(x).dtype), expected_dtype)
         self.assertEqual(knp.Max().symbolic_call(x).dtype, expected_dtype)
 
+        # Test with initial
+        initial = 1
+        expected_dtype = standardize_dtype(
+            jnp.max(x_jax, initial=initial).dtype
+        )
+        self.assertEqual(
+            standardize_dtype(knp.max(x, initial=initial).dtype), expected_dtype
+        )
+        self.assertEqual(
+            knp.Max(initial=initial).symbolic_call(x).dtype, expected_dtype
+        )
+
     @parameterized.named_parameters(named_product(dtype=ALL_DTYPES))
     def test_ones(self, dtype):
         import jax.numpy as jnp
 
         expected_dtype = standardize_dtype(jnp.ones([2, 3], dtype=dtype).dtype)
 
         self.assertEqual(
@@ -6041,27 +6158,27 @@
         expected_dtype = standardize_dtype(jnp.eye(3, dtype=dtype).dtype)
 
         self.assertEqual(
             standardize_dtype(knp.eye(3, dtype=dtype).dtype),
             expected_dtype,
         )
         self.assertEqual(
-            standardize_dtype(knp.Eye().symbolic_call(3, dtype=dtype).dtype),
+            standardize_dtype(knp.Eye(dtype=dtype).symbolic_call(3).dtype),
             expected_dtype,
         )
 
         expected_dtype = standardize_dtype(jnp.eye(3, 4, 1, dtype=dtype).dtype)
 
         self.assertEqual(
-            standardize_dtype(knp.eye(3, 4, 1, dtype=dtype).dtype),
+            standardize_dtype(knp.eye(3, 4, k=1, dtype=dtype).dtype),
             expected_dtype,
         )
         self.assertEqual(
             standardize_dtype(
-                knp.Eye().symbolic_call(3, 4, 1, dtype=dtype).dtype
+                knp.Eye(k=1, dtype=dtype).symbolic_call(3, 4).dtype
             ),
             expected_dtype,
         )
 
     @parameterized.named_parameters(named_product(dtype=ALL_DTYPES))
     def test_flip(self, dtype):
         import jax.numpy as jnp
@@ -6739,14 +6856,26 @@
         x = knp.ones((1,), dtype=dtype)
         x_jax = jnp.ones((1,), dtype=dtype)
         expected_dtype = standardize_dtype(jnp.min(x_jax).dtype)
 
         self.assertEqual(standardize_dtype(knp.min(x).dtype), expected_dtype)
         self.assertEqual(knp.Min().symbolic_call(x).dtype, expected_dtype)
 
+        # Test with initial
+        initial = 0
+        expected_dtype = standardize_dtype(
+            jnp.min(x_jax, initial=initial).dtype
+        )
+        self.assertEqual(
+            standardize_dtype(knp.min(x, initial=initial).dtype), expected_dtype
+        )
+        self.assertEqual(
+            knp.Min(initial=initial).symbolic_call(x).dtype, expected_dtype
+        )
+
     @parameterized.named_parameters(
         named_product(dtypes=itertools.combinations(ALL_DTYPES, 2))
     )
     def test_minimum(self, dtypes):
         import jax.numpy as jnp
 
         dtype1, dtype2 = dtypes
@@ -7514,15 +7643,15 @@
         expected_dtype = standardize_dtype(jnp.tri(3, dtype=dtype).dtype)
 
         self.assertEqual(
             standardize_dtype(knp.tri(3, dtype=dtype).dtype),
             expected_dtype,
         )
         self.assertEqual(
-            standardize_dtype(knp.Tri().symbolic_call(3, dtype=dtype).dtype),
+            standardize_dtype(knp.Tri(dtype=dtype).symbolic_call(3).dtype),
             expected_dtype,
         )
 
     @parameterized.named_parameters(named_product(dtype=ALL_DTYPES))
     def test_tril(self, dtype):
         import jax.numpy as jnp
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/operation.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/operation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/operation_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/operation_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/operation_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/operation_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/operation_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/symbolic_arguments.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/symbolic_arguments.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/ops/symbolic_arguments_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/ops/symbolic_arguments_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adadelta.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adadelta_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adadelta_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adafactor.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adafactor_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adafactor_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adagrad.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adagrad_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adagrad_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adam.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adam_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adam_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adamax.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adamax_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adamax_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adamw.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/adamw_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/adamw_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/base_optimizer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/ftrl.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/ftrl_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/ftrl_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/lion.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/lion_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/lion_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/loss_scale_optimizer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/loss_scale_optimizer_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/loss_scale_optimizer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/nadam.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/nadam_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/nadam_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/optimizer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/optimizer_sparse_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/optimizer_sparse_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/optimizer_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/optimizer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/rmsprop.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/rmsprop_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/rmsprop_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/schedules/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/schedules/learning_rate_schedule_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/schedules/learning_rate_schedule_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/sgd.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/optimizers/sgd_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/optimizers/sgd_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/quantizers/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/quantizers/quantizers.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/quantizers/quantizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/quantizers/quantizers_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/quantizers/quantizers_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/random/random.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/random/random_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/random/random_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/random/seed_generator.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/random/seed_generator_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/random/seed_generator_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/regularizers/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/regularizers/regularizers.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/regularizers/regularizers_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/regularizers/regularizers_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/saving/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/saving/object_registration.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/saving/object_registration_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/saving/object_registration_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/saving/saving_api.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/saving/saving_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/saving/saving_api_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/saving/saving_api_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/saving/saving_lib.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/saving/saving_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/saving/saving_lib_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/saving/saving_lib_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/saving/serialization_lib.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/saving/serialization_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,19 @@
             "class_name": "__slice__",
             "config": {
                 "start": serialize_keras_object(obj.start),
                 "stop": serialize_keras_object(obj.stop),
                 "step": serialize_keras_object(obj.step),
             },
         }
+    # Ellipsis is an instance, and ellipsis class is not in global scope.
+    # checking equality also fails elsewhere in the library, so we have
+    # to dynamically get the type.
+    if isinstance(obj, type(Ellipsis)):
+        return {"class_name": "__ellipsis__", "config": {}}
     if isinstance(obj, backend.KerasTensor):
         history = getattr(obj, "_keras_history", None)
         if history:
             history = list(history)
             history[0] = history[0].name
         return {
             "class_name": "__keras_tensor__",
@@ -609,14 +614,16 @@
         return backend.convert_to_tensor(
             inner_config["value"], dtype=inner_config["dtype"]
         )
     if class_name == "__numpy__":
         return np.array(inner_config["value"], dtype=inner_config["dtype"])
     if config["class_name"] == "__bytes__":
         return inner_config["value"].encode("utf-8")
+    if config["class_name"] == "__ellipsis__":
+        return Ellipsis
     if config["class_name"] == "__slice__":
         return slice(
             deserialize_keras_object(
                 inner_config["start"],
                 custom_objects=custom_objects,
                 safe_mode=safe_mode,
             ),
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/saving/serialization_lib_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/saving/serialization_lib_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,18 @@
         model = keras.Model(input, layer)
         serialized, _, reserialized = self.roundtrip(model)
         # Anticipate JSON roundtrip mapping tuples to lists:
         serialized_str = tuples_to_lists_str(serialized)
         reserialized_str = tuples_to_lists_str(reserialized)
         self.assertEqual(serialized_str, reserialized_str)
 
+    def test_serialize_ellipsis(self):
+        _, deserialized, _ = self.roundtrip(Ellipsis)
+        self.assertEqual(..., deserialized)
+
     def test_tensors_and_shapes(self):
         x = ops.random.normal((2, 2), dtype="float64")
         obj = {"x": x}
         _, new_obj, _ = self.roundtrip(obj)
         self.assertAllClose(x, new_obj["x"], atol=1e-5)
 
         obj = {"x.shape": x.shape}
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/testing/test_case.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/testing/test_case.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/testing/test_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/testing/test_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/testing/test_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/compile_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/compile_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/compile_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/compile_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/array_data_adapter_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/array_data_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/array_slicing.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/data_adapter.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/generator_data_adapter_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/generator_data_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/py_dataset_adapter_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/py_dataset_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/epoch_iterator.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/epoch_iterator_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/epoch_iterator_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/trainer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,15 @@
         del x  # The default implementation does not use `x`.
         losses = []
         if self._compile_loss is not None:
             loss = self._compile_loss(y, y_pred, sample_weight)
             if loss is not None:
                 losses.append(loss)
         for loss in self.losses:
-            losses.append(ops.cast(loss, dtype=backend.floatx()))
+            losses.append(ops.sum(ops.cast(loss, dtype=backend.floatx())))
         if backend.backend() != "jax" and len(losses) == 0:
             raise ValueError(
                 "No loss to compute. Provide a `loss` argument in `compile()`."
             )
         if len(losses) == 1:
             total_loss = losses[0]
         elif len(losses) == 0:
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/trainers/trainer_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/trainers/trainer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/tree/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/tree/dmtree_impl.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/tree/dmtree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/tree/optree_impl.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/tree/optree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/tree/tree_api.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/tree/tree_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/tree/tree_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/tree/tree_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/__init__.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/argument_validation.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/audio_dataset_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/audio_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/audio_dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/audio_dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/backend_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/code_stats.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/code_stats_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/code_stats_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/dataset_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/dtype_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/dtype_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/dtype_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/file_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/file_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/file_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/image_dataset_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/image_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/image_dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/image_dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/image_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/io_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/io_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/io_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/jax_layer.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/jax_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/jax_layer_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/jax_layer_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/model_visualization.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/module_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/naming.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/naming_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/naming_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/numerical_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/numerical_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/numerical_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/progbar.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/python_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/python_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/python_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/rng_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/rng_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/rng_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/sequence_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/sequence_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/sequence_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/summary_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/summary_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/summary_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/text_dataset_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/text_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/text_dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/text_dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/tf_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/timeseries_dataset_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/timeseries_dataset_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/timeseries_dataset_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/torch_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/torch_utils_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/torch_utils_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/traceback_utils.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/tracking.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras/src/utils/tracking_test.py` & `keras_nightly-3.3.0.dev2024042003/keras/src/utils/tracking_test.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/keras_nightly.egg-info/PKG-INFO` & `keras_nightly-3.3.0.dev2024042003/keras_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.0.dev2024041903
+Version: 3.3.0.dev2024042003
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.3.0.dev2024041903/keras_nightly.egg-info/SOURCES.txt` & `keras_nightly-3.3.0.dev2024042003/keras_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/pyproject.toml` & `keras_nightly-3.3.0.dev2024042003/pyproject.toml`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.0.dev2024041903/setup.py` & `keras_nightly-3.3.0.dev2024042003/setup.py`

 * *Files identical despite different names*

