# Comparing `tmp/keras_nightly-3.3.3.dev2024050903.tar.gz` & `tmp/keras_nightly-3.3.3.dev2024051103.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras_nightly-3.3.3.dev2024050903.tar", last modified: Thu May  9 03:21:29 2024, max compression
+gzip compressed data, was "keras_nightly-3.3.3.dev2024051103.tar", last modified: Sat May 11 03:20:26 2024, max compression
```

## Comparing `keras_nightly-3.3.3.dev2024050903.tar` & `keras_nightly-3.3.3.dev2024051103.tar`

### file list

```diff
@@ -1,698 +1,698 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.851182 keras_nightly-3.3.3.dev2024050903/
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-09 03:21:29.851182 keras_nightly-3.3.3.dev2024050903/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.751181 keras_nightly-3.3.3.dev2024050903/keras/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.751181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.751181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.755181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/layers/
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.759181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/preprocessing/text/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/preprocessing/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/api/
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-09 03:21:25.000000 keras_nightly-3.3.3.dev2024050903/keras/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/api/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/activations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/api/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/applications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/api/applications/convnext/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/applications/convnext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/api/applications/densenet/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/applications/densenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/api/applications/efficientnet/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/applications/efficientnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/api/applications/efficientnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.763181 keras_nightly-3.3.3.dev2024050903/keras/api/applications/imagenet_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/applications/inception_resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/applications/inception_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/applications/inception_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/applications/mobilenet/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/applications/mobilenet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/applications/mobilenet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/applications/mobilenet_v3/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/applications/nasnet/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/applications/nasnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/applications/resnet/
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/applications/resnet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/applications/resnet50/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/applications/resnet50/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/applications/resnet_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/applications/vgg16/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/applications/vgg16/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/applications/vgg19/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/applications/vgg19/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/applications/xception/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/applications/xception/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/backend/
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/callbacks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/datasets/boston_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/datasets/california_housing/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/datasets/california_housing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/datasets/cifar10/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/datasets/cifar10/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/datasets/cifar100/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/datasets/cifar100/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/datasets/fashion_mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.767181 keras_nightly-3.3.3.dev2024050903/keras/api/datasets/imdb/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/datasets/imdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/datasets/mnist/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/datasets/mnist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/datasets/reuters/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/datasets/reuters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/dtype_policies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/export/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/initializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/legacy/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/mixed_precision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/models/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/ops/
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/ops/image/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/ops/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/ops/linalg/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/ops/linalg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/ops/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/ops/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/ops/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/ops/numpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/optimizers/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/optimizers/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/optimizers/schedules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/preprocessing/image/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/preprocessing/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.771181 keras_nightly-3.3.3.dev2024050903/keras/api/preprocessing/sequence/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.775181 keras_nightly-3.3.3.dev2024050903/keras/api/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.775181 keras_nightly-3.3.3.dev2024050903/keras/api/random/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/random/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.775181 keras_nightly-3.3.3.dev2024050903/keras/api/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/regularizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.775181 keras_nightly-3.3.3.dev2024050903/keras/api/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/saving/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.775181 keras_nightly-3.3.3.dev2024050903/keras/api/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/tree/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.775181 keras_nightly-3.3.3.dev2024050903/keras/api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.775181 keras_nightly-3.3.3.dev2024050903/keras/api/utils/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/api/utils/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.775181 keras_nightly-3.3.3.dev2024050903/keras/src/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.775181 keras_nightly-3.3.3.dev2024050903/keras/src/activations/
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/activations/activations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/api_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.779181 keras_nightly-3.3.3.dev2024050903/keras/src/applications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24919 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/applications/convnext.py
--rw-r--r--   0 runner    (1001) docker     (127)    16848 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/applications/densenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    25274 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/applications/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    40460 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/applications/inception_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/applications/mobilenet.py
--rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    30694 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/applications/nasnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    19006 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/applications/resnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/applications/resnet_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9110 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/applications/vgg16.py
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/applications/vgg19.py
--rw-r--r--   0 runner    (1001) docker     (127)    12705 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/applications/xception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.779181 keras_nightly-3.3.3.dev2024050903/keras/src/backend/
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.779181 keras_nightly-3.3.3.dev2024050903/keras/src/backend/common/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17099 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/common/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/common/global_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/common/name_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/common/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/exports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.783182 keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    29008 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    31232 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.783182 keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/image.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    30670 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    28249 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.787181 keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6161 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    28490 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    78825 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.791182 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17887 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    27099 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)    48117 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.791182 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.795182 keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/callback_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/terminate_on_nan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.795182 keras_nightly-3.3.3.dev2024050903/keras/src/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/constraints/constraints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.795182 keras_nightly-3.3.3.dev2024050903/keras/src/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/datasets/boston_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/datasets/california_housing.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/datasets/cifar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/datasets/cifar10.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/datasets/cifar100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/datasets/imdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/datasets/mnist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/datasets/reuters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.799182 keras_nightly-3.3.3.dev2024050903/keras/src/distribution/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/distribution/distribution_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.799182 keras_nightly-3.3.3.dev2024050903/keras/src/dtype_policies/
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/dtype_policies/dtype_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.799182 keras_nightly-3.3.3.dev2024050903/keras/src/export/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33588 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/export/export_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.799182 keras_nightly-3.3.3.dev2024050903/keras/src/initializers/
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/initializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/initializers/initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/initializers/random_initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.799182 keras_nightly-3.3.3.dev2024050903/keras/src/layers/
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.799182 keras_nightly-3.3.3.dev2024050903/keras/src/layers/activations/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/activations/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/activations/elu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/activations/prelu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/activations/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/activations/softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.803182 keras_nightly-3.3.3.dev2024050903/keras/src/layers/attention/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/attention/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    28502 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/attention/multi_head_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.803182 keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17263 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/separable_conv2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.807182 keras_nightly-3.3.3.dev2024050903/keras/src/layers/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25496 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/core/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    42280 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 runner    (1001) docker     (127)    17463 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/core/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/core/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/core/input_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/core/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/core/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/input_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    64221 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.807182 keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/average.py
--rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/maximum.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/minimum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/multiply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.807182 keras_nightly-3.3.3.dev2024050903/keras/src/layers/normalization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/normalization/unit_normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.811182 keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/max_pooling3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.815182 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 runner    (1001) docker     (127)    17728 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.815182 keras_nightly-3.3.3.dev2024050903/keras/src/layers/regularization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/regularization/spatial_dropout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.819182 keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/zero_padding3d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.823182 keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13235 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    28138 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/gru.py
--rw-r--r--   0 runner    (1001) docker     (127)    26982 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/time_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.823182 keras_nightly-3.3.3.dev2024050903/keras/src/legacy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/legacy/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/legacy/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/legacy/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.823182 keras_nightly-3.3.3.dev2024050903/keras/src/legacy/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.827182 keras_nightly-3.3.3.dev2024050903/keras/src/legacy/saving/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.827182 keras_nightly-3.3.3.dev2024050903/keras/src/losses/
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/losses/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)    69039 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/losses/losses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.827182 keras_nightly-3.3.3.dev2024050903/keras/src/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/metrics/regression_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.831182 keras_nightly-3.3.3.dev2024050903/keras/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/models/cloning.py
--rw-r--r--   0 runner    (1001) docker     (127)    30043 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/models/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    22763 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/models/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/models/sequential.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/models/variable_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.831182 keras_nightly-3.3.3.dev2024050903/keras/src/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27019 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/ops/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    15626 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/ops/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    37642 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/ops/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/ops/linalg.py
--rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/ops/math.py
--rw-r--r--   0 runner    (1001) docker     (127)    67512 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/ops/nn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (127)   196510 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/ops/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/ops/operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/ops/operation_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/ops/symbolic_arguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.835182 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/adadelta.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/adafactor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/adamax.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)    40536 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/ftrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/nadam.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/rmsprop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.835182 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/schedules/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.835182 keras_nightly-3.3.3.dev2024050903/keras/src/quantizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/quantizers/quantizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.835182 keras_nightly-3.3.3.dev2024050903/keras/src/random/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/random/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/random/seed_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.839182 keras_nightly-3.3.3.dev2024050903/keras/src/regularizers/
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/regularizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/regularizers/regularizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.839182 keras_nightly-3.3.3.dev2024050903/keras/src/saving/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/saving/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/saving/keras_saveable.py
--rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/saving/object_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/saving/saving_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26931 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/saving/saving_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)    29052 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/saving/serialization_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.839182 keras_nightly-3.3.3.dev2024050903/keras/src/testing/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28114 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/testing/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/testing/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.839182 keras_nightly-3.3.3.dev2024050903/keras/src/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25904 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/trainers/compile_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.843182 keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    46479 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/trainers/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.843182 keras_nightly-3.3.3.dev2024050903/keras/src/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/tree/dmtree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/tree/optree_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/tree/tree_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.847182 keras_nightly-3.3.3.dev2024050903/keras/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/argument_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/code_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/dtype_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/file_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16629 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/jax_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/jax_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/model_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/numerical_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/progbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/python_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/rng_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/summary_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/traceback_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-09 03:19:49.000000 keras_nightly-3.3.3.dev2024050903/keras/src/utils/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-09 03:21:27.000000 keras_nightly-3.3.3.dev2024050903/keras/src/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 03:21:29.851182 keras_nightly-3.3.3.dev2024050903/keras_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-09 03:21:29.000000 keras_nightly-3.3.3.dev2024050903/keras_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20419 2024-05-09 03:21:29.000000 keras_nightly-3.3.3.dev2024050903/keras_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 03:21:29.000000 keras_nightly-3.3.3.dev2024050903/keras_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-09 03:21:29.000000 keras_nightly-3.3.3.dev2024050903/keras_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 03:21:29.000000 keras_nightly-3.3.3.dev2024050903/keras_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 03:21:29.851182 keras_nightly-3.3.3.dev2024050903/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-09 03:21:27.000000 keras_nightly-3.3.3.dev2024050903/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.909350 keras_nightly-3.3.3.dev2024051103/
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-11 03:20:26.909350 keras_nightly-3.3.3.dev2024051103/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4789 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.805350 keras_nightly-3.3.3.dev2024051103/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.805350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.805350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.805350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.805350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.805350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.805350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.805350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.805350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.805350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.805350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.805350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.805350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.805350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.805350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     6684 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.809350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.813351 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/preprocessing/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/preprocessing/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-11 03:20:22.000000 keras_nightly-3.3.3.dev2024051103/keras/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/api/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/activations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/api/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/applications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/api/applications/convnext/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/applications/convnext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/api/applications/densenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/applications/densenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/api/applications/efficientnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/applications/efficientnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/api/applications/efficientnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/api/applications/imagenet_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/api/applications/inception_resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/api/applications/inception_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/applications/inception_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/api/applications/mobilenet/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/applications/mobilenet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/api/applications/mobilenet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/api/applications/mobilenet_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.817350 keras_nightly-3.3.3.dev2024051103/keras/api/applications/nasnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/applications/nasnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/applications/resnet/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/applications/resnet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/applications/resnet50/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/applications/resnet50/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/applications/resnet_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/applications/vgg16/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/applications/vgg16/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/applications/vgg19/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/applications/vgg19/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/applications/xception/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/applications/xception/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/callbacks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/datasets/boston_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/datasets/california_housing/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/datasets/california_housing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/datasets/cifar10/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/datasets/cifar10/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/datasets/cifar100/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/datasets/cifar100/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/datasets/fashion_mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/datasets/imdb/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/datasets/imdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/datasets/mnist/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/datasets/mnist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/datasets/reuters/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/datasets/reuters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.821350 keras_nightly-3.3.3.dev2024051103/keras/api/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/dtype_policies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/export/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/initializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     9963 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/legacy/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/mixed_precision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)     9036 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/ops/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/ops/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/ops/linalg/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/ops/linalg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/ops/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/ops/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/ops/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     5772 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/ops/numpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/optimizers/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/optimizers/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/optimizers/schedules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/preprocessing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/preprocessing/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/preprocessing/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/preprocessing/sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.825350 keras_nightly-3.3.3.dev2024051103/keras/api/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.829350 keras_nightly-3.3.3.dev2024051103/keras/api/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/random/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.829350 keras_nightly-3.3.3.dev2024051103/keras/api/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/regularizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.829350 keras_nightly-3.3.3.dev2024051103/keras/api/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/saving/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.829350 keras_nightly-3.3.3.dev2024051103/keras/api/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/tree/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.829350 keras_nightly-3.3.3.dev2024051103/keras/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.829350 keras_nightly-3.3.3.dev2024051103/keras/api/utils/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/api/utils/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.829350 keras_nightly-3.3.3.dev2024051103/keras/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.829350 keras_nightly-3.3.3.dev2024051103/keras/src/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/activations/activations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/api_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.833351 keras_nightly-3.3.3.dev2024051103/keras/src/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25014 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/applications/convnext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16902 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/applications/densenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25341 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/applications/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40735 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16034 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15581 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/applications/inception_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17168 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/applications/mobilenet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17934 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23521 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30917 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/applications/nasnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/applications/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9173 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/applications/vgg16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9494 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/applications/vgg19.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12766 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/applications/xception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.833351 keras_nightly-3.3.3.dev2024051103/keras/src/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.833351 keras_nightly-3.3.3.dev2024051103/keras/src/backend/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17099 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9808 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/common/global_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/common/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/exports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.837350 keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12083 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14746 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29008 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31232 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13804 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36259 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.841350 keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13086 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10586 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30670 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28249 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10738 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.845350 keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13708 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14197 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28490 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78825 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34600 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32268 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33111 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.845350 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17887 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14001 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15073 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27099 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48117 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.849350 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8292 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13704 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17577 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.853350 keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18488 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26393 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/terminate_on_nan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.853350 keras_nightly-3.3.3.dev2024051103/keras/src/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/constraints/constraints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.853350 keras_nightly-3.3.3.dev2024051103/keras/src/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/datasets/california_housing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/datasets/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/datasets/cifar10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2914 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/datasets/cifar100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/datasets/imdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/datasets/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/datasets/reuters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.853350 keras_nightly-3.3.3.dev2024051103/keras/src/distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31207 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/distribution/distribution_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.853350 keras_nightly-3.3.3.dev2024051103/keras/src/dtype_policies/
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12920 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/dtype_policies/dtype_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.853350 keras_nightly-3.3.3.dev2024051103/keras/src/export/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33588 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/export/export_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.857350 keras_nightly-3.3.3.dev2024051103/keras/src/initializers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/initializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/initializers/initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23462 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/initializers/random_initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.857350 keras_nightly-3.3.3.dev2024051103/keras/src/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.857350 keras_nightly-3.3.3.dev2024051103/keras/src/layers/activations/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/activations/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/activations/elu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/activations/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/activations/softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.857350 keras_nightly-3.3.3.dev2024051103/keras/src/layers/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/attention/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17952 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28502 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/attention/multi_head_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.861350 keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17263 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10695 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11617 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12643 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5672 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5895 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/separable_conv2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.865350 keras_nightly-3.3.3.dev2024051103/keras/src/layers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25496 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/core/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42280 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17463 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/core/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/core/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8989 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/core/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9849 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/input_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64221 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.865350 keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/average.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10795 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6708 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.865350 keras_nightly-3.3.3.dev2024051103/keras/src/layers/normalization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8534 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/normalization/unit_normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.869350 keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4127 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/max_pooling3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.873350 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14572 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13145 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29613 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8317 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10936 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18458 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13920 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6463 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10820 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17728 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27820 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.877350 keras_nightly-3.3.3.dev2024051103/keras/src/layers/regularization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7300 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/regularization/spatial_dropout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.877350 keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/zero_padding3d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.881350 keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13235 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27242 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8294 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8287 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28138 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26982 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19159 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17537 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4943 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/time_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.881350 keras_nightly-3.3.3.dev2024051103/keras/src/legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70241 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/legacy/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/legacy/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/legacy/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.881350 keras_nightly-3.3.3.dev2024051103/keras/src/legacy/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65545 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11172 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11110 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.885350 keras_nightly-3.3.3.dev2024051103/keras/src/legacy/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7296 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22750 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21808 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.885350 keras_nightly-3.3.3.dev2024051103/keras/src/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6013 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/losses/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69039 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/losses/losses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.885350 keras_nightly-3.3.3.dev2024051103/keras/src/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     7198 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15604 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61579 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26976 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10692 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19818 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/metrics/regression_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.889350 keras_nightly-3.3.3.dev2024051103/keras/src/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15386 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/models/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30043 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/models/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22763 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13067 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/models/sequential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/models/variable_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.889350 keras_nightly-3.3.3.dev2024051103/keras/src/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27019 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/ops/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15626 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/ops/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37642 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/ops/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21256 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/ops/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30618 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/ops/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67512 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/ops/nn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)   196510 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/ops/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10608 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/ops/operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/ops/operation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/ops/symbolic_arguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.893350 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/adamax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40536 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11553 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/nadam.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6003 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/rmsprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.893350 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/schedules/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35507 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.893350 keras_nightly-3.3.3.dev2024051103/keras/src/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/quantizers/quantizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.893350 keras_nightly-3.3.3.dev2024051103/keras/src/random/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/random/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/random/seed_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.897350 keras_nightly-3.3.3.dev2024051103/keras/src/regularizers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/regularizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11799 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/regularizers/regularizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.897350 keras_nightly-3.3.3.dev2024051103/keras/src/saving/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/saving/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/saving/keras_saveable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7358 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/saving/object_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9737 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/saving/saving_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26931 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/saving/saving_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29052 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/saving/serialization_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.897350 keras_nightly-3.3.3.dev2024051103/keras/src/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28114 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/testing/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6197 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/testing/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.897350 keras_nightly-3.3.3.dev2024051103/keras/src/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25904 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/trainers/compile_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.901350 keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9717 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20556 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46479 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/trainers/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.901350 keras_nightly-3.3.3.dev2024051103/keras/src/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/tree/dmtree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/tree/optree_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9397 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/tree/tree_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.905350 keras_nightly-3.3.3.dev2024051103/keras/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/argument_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/code_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28554 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16371 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/file_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16629 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26570 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/jax_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/jax_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16107 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/model_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/progbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/python_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/rng_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14512 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/summary_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10675 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4630 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8997 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8980 2024-05-11 03:19:08.000000 keras_nightly-3.3.3.dev2024051103/keras/src/utils/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-11 03:20:24.000000 keras_nightly-3.3.3.dev2024051103/keras/src/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 03:20:26.909350 keras_nightly-3.3.3.dev2024051103/keras_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-11 03:20:26.000000 keras_nightly-3.3.3.dev2024051103/keras_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20419 2024-05-11 03:20:26.000000 keras_nightly-3.3.3.dev2024051103/keras_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 03:20:26.000000 keras_nightly-3.3.3.dev2024051103/keras_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-11 03:20:26.000000 keras_nightly-3.3.3.dev2024051103/keras_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 03:20:26.000000 keras_nightly-3.3.3.dev2024051103/keras_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 03:20:26.909350 keras_nightly-3.3.3.dev2024051103/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-11 03:20:24.000000 keras_nightly-3.3.3.dev2024051103/setup.py
```

### Comparing `keras_nightly-3.3.3.dev2024050903/PKG-INFO` & `keras_nightly-3.3.3.dev2024051103/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.3.dev2024050903
+Version: 3.3.3.dev2024051103
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.3.3.dev2024050903/README.md` & `keras_nightly-3.3.3.dev2024051103/README.md`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/activations/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/convnext/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/backend/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/callbacks/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/config/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/constraints/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/distribution/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/dtype_policies/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/initializers/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/layers/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/losses/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/metrics/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/mixed_precision/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/ops/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/ops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from keras.src.ops.core import vectorized_map
 from keras.src.ops.core import while_loop
 from keras.src.ops.linalg import cholesky
 from keras.src.ops.linalg import det
 from keras.src.ops.linalg import eig
 from keras.src.ops.linalg import eigh
 from keras.src.ops.linalg import inv
+from keras.src.ops.linalg import lstsq
 from keras.src.ops.linalg import lu_factor
 from keras.src.ops.linalg import norm
 from keras.src.ops.linalg import qr
 from keras.src.ops.linalg import solve
 from keras.src.ops.linalg import solve_triangular
 from keras.src.ops.linalg import svd
 from keras.src.ops.math import erf
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/ops/linalg/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,13 +5,14 @@
 """
 
 from keras.src.ops.linalg import cholesky
 from keras.src.ops.linalg import det
 from keras.src.ops.linalg import eig
 from keras.src.ops.linalg import eigh
 from keras.src.ops.linalg import inv
+from keras.src.ops.linalg import lstsq
 from keras.src.ops.linalg import lu_factor
 from keras.src.ops.linalg import norm
 from keras.src.ops.linalg import qr
 from keras.src.ops.linalg import solve
 from keras.src.ops.linalg import solve_triangular
 from keras.src.ops.linalg import svd
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/ops/nn/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/ops/numpy/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/optimizers/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/preprocessing/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/preprocessing/image/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/preprocessing/image/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/quantizers/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/random/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/regularizers/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/saving/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/tree/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/_tf_keras/keras/utils/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/activations/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/applications/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/applications/convnext/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/applications/efficientnet/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/applications/efficientnet_v2/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/backend/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/callbacks/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/config/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/constraints/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/distribution/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/dtype_policies/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/initializers/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/layers/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/losses/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/metrics/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/mixed_precision/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/ops/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/ops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from keras.src.ops.core import vectorized_map
 from keras.src.ops.core import while_loop
 from keras.src.ops.linalg import cholesky
 from keras.src.ops.linalg import det
 from keras.src.ops.linalg import eig
 from keras.src.ops.linalg import eigh
 from keras.src.ops.linalg import inv
+from keras.src.ops.linalg import lstsq
 from keras.src.ops.linalg import lu_factor
 from keras.src.ops.linalg import norm
 from keras.src.ops.linalg import qr
 from keras.src.ops.linalg import solve
 from keras.src.ops.linalg import solve_triangular
 from keras.src.ops.linalg import svd
 from keras.src.ops.math import erf
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/ops/linalg/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/ops/linalg/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,13 +5,14 @@
 """
 
 from keras.src.ops.linalg import cholesky
 from keras.src.ops.linalg import det
 from keras.src.ops.linalg import eig
 from keras.src.ops.linalg import eigh
 from keras.src.ops.linalg import inv
+from keras.src.ops.linalg import lstsq
 from keras.src.ops.linalg import lu_factor
 from keras.src.ops.linalg import norm
 from keras.src.ops.linalg import qr
 from keras.src.ops.linalg import solve
 from keras.src.ops.linalg import solve_triangular
 from keras.src.ops.linalg import svd
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/ops/nn/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/ops/numpy/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/optimizers/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/optimizers/legacy/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/optimizers/schedules/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/quantizers/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/random/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/regularizers/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/saving/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/tree/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/api/utils/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/activations/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/activations/activations.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/api_export.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/applications/convnext.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/applications/convnext.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,14 +127,15 @@
         ImageNet classes).
     classifier_activation: A `str` or callable. The activation function to use
         on the "top" layer. Ignored unless `include_top=True`. Set
         `classifier_activation=None` to return the logits of the "top" layer.
         Defaults to `"softmax"`.
         When loading pretrained weights, `classifier_activation` can only
         be `None` or `"softmax"`.
+    name: The name of the model (string).
 
 Returns:
     A model instance.
 """
 
 
 class StochasticDepth(Layer):
@@ -329,36 +330,37 @@
 
 def ConvNeXt(
     depths,
     projection_dims,
     drop_path_rate=0.0,
     layer_scale_init_value=1e-6,
     default_size=224,
-    model_name="convnext",
+    name="convnext",
     include_preprocessing=True,
     include_top=True,
     weights=None,
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    weights_name=None,
 ):
     """Instantiates ConvNeXt architecture given specific configuration.
 
     Args:
         depths: An iterable containing depths for each individual stages.
         projection_dims: An iterable containing output number of channels of
         each individual stages.
         drop_path_rate: Stochastic depth probability. If 0.0, then stochastic
             depth won't be used.
         layer_scale_init_value: Layer scale coefficient. If 0.0, layer scaling
             won't be used.
         default_size: Default input image size.
-        model_name: An optional name for the model.
+        name: An optional name for the model.
         include_preprocessing: boolean denoting whther to
             include preprocessing in the model.
             When `weights="imagenet"` this should always be `True`.
             But for other models (e.g., randomly initialized) you should set it
             to `False` and apply preprocessing to data accordingly.
         include_top: Boolean denoting whether to include classification
             head to the model.
@@ -436,52 +438,52 @@
     x = inputs
     if include_preprocessing:
         channel_axis = (
             3 if backend.image_data_format() == "channels_last" else 1
         )
         num_channels = input_shape[channel_axis - 1]
         if num_channels == 3:
-            x = PreStem(name=model_name)(x)
+            x = PreStem(name=name)(x)
 
     # Stem block.
     stem = Sequential(
         [
             layers.Conv2D(
                 projection_dims[0],
                 kernel_size=4,
                 strides=4,
-                name=model_name + "_stem_conv",
+                name=name + "_stem_conv",
             ),
             layers.LayerNormalization(
-                epsilon=1e-6, name=model_name + "_stem_layernorm"
+                epsilon=1e-6, name=name + "_stem_layernorm"
             ),
         ],
-        name=model_name + "_stem",
+        name=name + "_stem",
     )
 
     # Downsampling blocks.
     downsample_layers = []
     downsample_layers.append(stem)
 
     num_downsample_layers = 3
     for i in range(num_downsample_layers):
         downsample_layer = Sequential(
             [
                 layers.LayerNormalization(
                     epsilon=1e-6,
-                    name=model_name + "_downsampling_layernorm_" + str(i),
+                    name=name + "_downsampling_layernorm_" + str(i),
                 ),
                 layers.Conv2D(
                     projection_dims[i + 1],
                     kernel_size=2,
                     strides=2,
-                    name=model_name + "_downsampling_conv_" + str(i),
+                    name=name + "_downsampling_conv_" + str(i),
                 ),
             ],
-            name=model_name + "_downsampling_block_" + str(i),
+            name=name + "_downsampling_block_" + str(i),
         )
         downsample_layers.append(downsample_layer)
 
     # Stochastic depth schedule.
     # This is referred from the original ConvNeXt codebase:
     # https://github.com/facebookresearch/ConvNeXt/blob/main/models/convnext.py#L86
     depth_drop_rates = [
@@ -495,44 +497,44 @@
     for i in range(num_convnext_blocks):
         x = downsample_layers[i](x)
         for j in range(depths[i]):
             x = ConvNeXtBlock(
                 projection_dim=projection_dims[i],
                 drop_path_rate=depth_drop_rates[cur + j],
                 layer_scale_init_value=layer_scale_init_value,
-                name=model_name + f"_stage_{i}_block_{j}",
+                name=name + f"_stage_{i}_block_{j}",
             )(x)
         cur += depths[i]
 
     if include_top:
         imagenet_utils.validate_activation(classifier_activation, weights)
         x = Head(
             num_classes=classes,
             classifier_activation=classifier_activation,
-            name=model_name,
+            name=name,
         )(x)
 
     else:
         if pooling == "avg":
             x = layers.GlobalAveragePooling2D()(x)
         elif pooling == "max":
             x = layers.GlobalMaxPooling2D()(x)
         x = layers.LayerNormalization(epsilon=1e-6)(x)
 
-    model = Functional(inputs=inputs, outputs=x, name=model_name)
+    model = Functional(inputs=inputs, outputs=x, name=name)
 
     # Load weights.
     if weights == "imagenet":
         if include_top:
             file_suffix = ".h5"
-            file_hash = WEIGHTS_HASHES[model_name][0]
+            file_hash = WEIGHTS_HASHES[weights_name][0]
         else:
             file_suffix = "_notop.h5"
-            file_hash = WEIGHTS_HASHES[model_name][1]
-        file_name = model_name + file_suffix
+            file_hash = WEIGHTS_HASHES[weights_name][1]
+        file_name = name + file_suffix
         weights_path = file_utils.get_file(
             file_name,
             BASE_WEIGHTS_PATH + file_name,
             cache_subdir="models",
             file_hash=file_hash,
         )
         model.load_weights(weights_path)
@@ -548,31 +550,32 @@
 @keras_export(
     [
         "keras.applications.convnext.ConvNeXtTiny",
         "keras.applications.ConvNeXtTiny",
     ]
 )
 def ConvNeXtTiny(
-    model_name="convnext_tiny",
     include_top=True,
     include_preprocessing=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="convnext_tiny",
 ):
     return ConvNeXt(
+        weights_name="convnext_tiny",
         depths=MODEL_CONFIGS["tiny"]["depths"],
         projection_dims=MODEL_CONFIGS["tiny"]["projection_dims"],
         drop_path_rate=0.0,
         layer_scale_init_value=1e-6,
         default_size=MODEL_CONFIGS["tiny"]["default_size"],
-        model_name=model_name,
+        name=name,
         include_top=include_top,
         include_preprocessing=include_preprocessing,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
@@ -583,31 +586,32 @@
 @keras_export(
     [
         "keras.applications.convnext.ConvNeXtSmall",
         "keras.applications.ConvNeXtSmall",
     ]
 )
 def ConvNeXtSmall(
-    model_name="convnext_small",
     include_top=True,
     include_preprocessing=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="convnext_small",
 ):
     return ConvNeXt(
+        weights_name="convnext_small",
         depths=MODEL_CONFIGS["small"]["depths"],
         projection_dims=MODEL_CONFIGS["small"]["projection_dims"],
         drop_path_rate=0.0,
         layer_scale_init_value=1e-6,
         default_size=MODEL_CONFIGS["small"]["default_size"],
-        model_name=model_name,
+        name=name,
         include_top=include_top,
         include_preprocessing=include_preprocessing,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
@@ -618,31 +622,32 @@
 @keras_export(
     [
         "keras.applications.convnext.ConvNeXtBase",
         "keras.applications.ConvNeXtBase",
     ]
 )
 def ConvNeXtBase(
-    model_name="convnext_base",
     include_top=True,
     include_preprocessing=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="convnext_base",
 ):
     return ConvNeXt(
+        weights_name="convnext_base",
         depths=MODEL_CONFIGS["base"]["depths"],
         projection_dims=MODEL_CONFIGS["base"]["projection_dims"],
         drop_path_rate=0.0,
         layer_scale_init_value=1e-6,
         default_size=MODEL_CONFIGS["base"]["default_size"],
-        model_name=model_name,
+        name=name,
         include_top=include_top,
         include_preprocessing=include_preprocessing,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
@@ -653,31 +658,32 @@
 @keras_export(
     [
         "keras.applications.convnext.ConvNeXtLarge",
         "keras.applications.ConvNeXtLarge",
     ]
 )
 def ConvNeXtLarge(
-    model_name="convnext_large",
     include_top=True,
     include_preprocessing=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="convnext_large",
 ):
     return ConvNeXt(
+        weights_name="convnext_large",
         depths=MODEL_CONFIGS["large"]["depths"],
         projection_dims=MODEL_CONFIGS["large"]["projection_dims"],
         drop_path_rate=0.0,
         layer_scale_init_value=1e-6,
         default_size=MODEL_CONFIGS["large"]["default_size"],
-        model_name=model_name,
+        name=name,
         include_top=include_top,
         include_preprocessing=include_preprocessing,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
@@ -688,31 +694,32 @@
 @keras_export(
     [
         "keras.applications.convnext.ConvNeXtXLarge",
         "keras.applications.ConvNeXtXLarge",
     ]
 )
 def ConvNeXtXLarge(
-    model_name="convnext_xlarge",
     include_top=True,
     include_preprocessing=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="convnext_xlarge",
 ):
     return ConvNeXt(
+        weights_name="convnext_xlarge",
         depths=MODEL_CONFIGS["xlarge"]["depths"],
         projection_dims=MODEL_CONFIGS["xlarge"]["projection_dims"],
         drop_path_rate=0.0,
         layer_scale_init_value=1e-6,
         default_size=MODEL_CONFIGS["xlarge"]["default_size"],
-        model_name=model_name,
+        name=name,
         include_top=include_top,
         include_preprocessing=include_preprocessing,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/applications/densenet.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/applications/densenet.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="densenet",
 ):
     """Instantiates the DenseNet architecture.
 
     Reference:
     - [Densely Connected Convolutional Networks](
         https://arxiv.org/abs/1608.06993) (CVPR 2017)
 
@@ -172,14 +173,15 @@
             if no `weights` argument is specified.
         classifier_activation: A `str` or callable.
             The activation function to use
             on the "top" layer. Ignored unless `include_top=True`. Set
             `classifier_activation=None` to return the logits of the "top"
             layer. When loading pretrained weights, `classifier_activation`
             can only be `None` or `"softmax"`.
+        name: The name of the model (string).
 
     Returns:
         A model instance.
     """
     if backend.image_data_format() == "channels_first":
         raise ValueError(
             "DenseNet does not support the `channels_first` image data "
@@ -257,22 +259,15 @@
     # any potential predecessors of `input_tensor`.
     if input_tensor is not None:
         inputs = operation_utils.get_source_inputs(input_tensor)
     else:
         inputs = img_input
 
     # Create model.
-    if blocks == [6, 12, 24, 16]:
-        model = Functional(inputs, x, name="densenet121")
-    elif blocks == [6, 12, 32, 32]:
-        model = Functional(inputs, x, name="densenet169")
-    elif blocks == [6, 12, 48, 32]:
-        model = Functional(inputs, x, name="densenet201")
-    else:
-        model = Functional(inputs, x, name="densenet")
+    model = Functional(inputs, x, name=name)
 
     # Load weights.
     if weights == "imagenet":
         if include_top:
             if blocks == [6, 12, 24, 16]:
                 weights_path = file_utils.get_file(
                     "densenet121_weights_tf_dim_ordering_tf_kernels.h5",
@@ -333,25 +328,27 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="densenet121",
 ):
     """Instantiates the Densenet121 architecture."""
     return DenseNet(
         [6, 12, 24, 16],
         include_top,
         weights,
         input_tensor,
         input_shape,
         pooling,
         classes,
         classifier_activation,
+        name=name,
     )
 
 
 @keras_export(
     [
         "keras.applications.densenet.DenseNet169",
         "keras.applications.DenseNet169",
@@ -361,25 +358,27 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="densenet169",
 ):
     """Instantiates the Densenet169 architecture."""
     return DenseNet(
         [6, 12, 32, 32],
         include_top,
         weights,
         input_tensor,
         input_shape,
         pooling,
         classes,
         classifier_activation,
+        name=name,
     )
 
 
 @keras_export(
     [
         "keras.applications.densenet.DenseNet201",
         "keras.applications.DenseNet201",
@@ -389,25 +388,27 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="densenet201",
 ):
     """Instantiates the Densenet201 architecture."""
     return DenseNet(
         [6, 12, 48, 32],
         include_top,
         weights,
         input_tensor,
         input_shape,
         pooling,
         classes,
         classifier_activation,
+        name=name,
     )
 
 
 @keras_export("keras.applications.densenet.preprocess_input")
 def preprocess_input(x, data_format=None):
     return imagenet_utils.preprocess_input(
         x, data_format=data_format, mode="torch"
@@ -438,48 +439,49 @@
 
 Note: each Keras Application expects a specific kind of input preprocessing.
 For DenseNet, call `keras.applications.densenet.preprocess_input`
 on your inputs before passing them to the model.
 
 Args:
     include_top: whether to include the fully-connected
-    layer at the top of the network.
+        layer at the top of the network.
     weights: one of `None` (random initialization),
-    `"imagenet"` (pre-training on ImageNet),
-    or the path to the weights file to be loaded.
-    input_tensor: optional Keras tensor
-    (i.e. output of `layers.Input()`)
-    to use as image input for the model.
+        `"imagenet"` (pre-training on ImageNet),
+        or the path to the weights file to be loaded.
+        input_tensor: optional Keras tensor
+        (i.e. output of `layers.Input()`)
+        to use as image input for the model.
     input_shape: optional shape tuple, only to be specified
-    if `include_top` is False (otherwise the input shape
-    has to be `(224, 224, 3)` (with `'channels_last'` data format)
-    or `(3, 224, 224)` (with `'channels_first'` data format).
-    It should have exactly 3 inputs channels,
-    and width and height should be no smaller than 32.
-    E.g. `(200, 200, 3)` would be one valid value.
+        if `include_top` is False (otherwise the input shape
+        has to be `(224, 224, 3)` (with `'channels_last'` data format)
+        or `(3, 224, 224)` (with `'channels_first'` data format).
+        It should have exactly 3 inputs channels,
+        and width and height should be no smaller than 32.
+        E.g. `(200, 200, 3)` would be one valid value.
     pooling: Optional pooling mode for feature extraction
-    when `include_top` is `False`.
-    - `None` means that the output of the model will be
-        the 4D tensor output of the
-        last convolutional block.
-    - `avg` means that global average pooling
-        will be applied to the output of the
-        last convolutional block, and thus
-        the output of the model will be a 2D tensor.
-    - `max` means that global max pooling will
-        be applied.
+        when `include_top` is `False`.
+        - `None` means that the output of the model will be
+            the 4D tensor output of the
+            last convolutional block.
+        - `avg` means that global average pooling
+            will be applied to the output of the
+            last convolutional block, and thus
+            the output of the model will be a 2D tensor.
+        - `max` means that global max pooling will
+            be applied.
     classes: optional number of classes to classify images
-    into, only to be specified if `include_top` is `True`, and
-    if no `weights` argument is specified.
+        into, only to be specified if `include_top` is `True`, and
+        if no `weights` argument is specified.
     classifier_activation: A `str` or callable.
-    The activation function to use
-    on the "top" layer. Ignored unless `include_top=True`. Set
-    `classifier_activation=None` to return the logits
-    of the "top" layer. When loading pretrained weights,
-    `classifier_activation` can only be `None` or `"softmax"`.
+        The activation function to use
+        on the "top" layer. Ignored unless `include_top=True`. Set
+        `classifier_activation=None` to return the logits
+        of the "top" layer. When loading pretrained weights,
+        `classifier_activation` can only be `None` or `"softmax"`.
+    name: The name of the model (string).
 
 Returns:
     A Keras model instance.
 """
 
 setattr(DenseNet121, "__doc__", DenseNet121.__doc__ + DOC)
 setattr(DenseNet169, "__doc__", DenseNet169.__doc__ + DOC)
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/applications/efficientnet.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/applications/efficientnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,14 +191,15 @@
         ImageNet classes there are. Defaults to `1000`.
     classifier_activation: A `str` or callable. The activation function to use
         on the "top" layer. Ignored unless `include_top=True`. Set
         `classifier_activation=None` to return the logits of the "top" layer.
         Defaults to `'softmax'`.
         When loading pretrained weights, `classifier_activation` can only
         be `None` or `"softmax"`.
+    name: The name of the model (string).
 
 Returns:
     A model instance.
 """
 
 
 IMAGENET_STDDEV_RGB = [0.229, 0.224, 0.225]
@@ -209,35 +210,36 @@
     depth_coefficient,
     default_size,
     dropout_rate=0.2,
     drop_connect_rate=0.2,
     depth_divisor=8,
     activation="swish",
     blocks_args="default",
-    model_name="efficientnet",
+    name="efficientnet",
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    weights_name=None,
 ):
     """Instantiates the EfficientNet architecture.
 
     Args:
       width_coefficient: float, scaling coefficient for network width.
       depth_coefficient: float, scaling coefficient for network depth.
       default_size: integer, default input image size.
       dropout_rate: float, dropout rate before final classifier layer.
       drop_connect_rate: float, dropout rate at skip connections.
       depth_divisor: integer, a unit of network width.
       activation: activation function.
       blocks_args: list of dicts, parameters to construct block modules.
-      model_name: string, model name.
+      name: string, model name.
       include_top: whether to include the fully-connected
           layer at the top of the network.
       weights: one of `None` (random initialization),
             'imagenet' (pre-training on ImageNet),
             or the path to the weights file to be loaded.
       input_tensor: optional Keras tensor
           (i.e. output of `layers.Input()`)
@@ -407,25 +409,25 @@
     # any potential predecessors of `input_tensor`.
     if input_tensor is not None:
         inputs = operation_utils.get_source_inputs(input_tensor)
     else:
         inputs = img_input
 
     # Create model.
-    model = Functional(inputs, x, name=model_name)
+    model = Functional(inputs, x, name=name)
 
     # Load weights.
     if weights == "imagenet":
         if include_top:
             file_suffix = ".h5"
-            file_hash = WEIGHTS_HASHES[model_name[-2:]][0]
+            file_hash = WEIGHTS_HASHES[weights_name][0]
         else:
             file_suffix = "_notop.h5"
-            file_hash = WEIGHTS_HASHES[model_name[-2:]][1]
-        file_name = model_name + file_suffix
+            file_hash = WEIGHTS_HASHES[weights_name][1]
+        file_name = name + file_suffix
         weights_path = file_utils.get_file(
             file_name,
             BASE_WEIGHTS_PATH + file_name,
             cache_subdir="models",
             file_hash=file_hash,
         )
         model.load_weights(weights_path)
@@ -559,30 +561,30 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
-    **kwargs,
+    name="efficientnetb0",
 ):
     return EfficientNet(
         1.0,
         1.0,
         224,
         0.2,
-        model_name="efficientnetb0",
+        name=name,
         include_top=include_top,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
         classifier_activation=classifier_activation,
-        **kwargs,
+        weights_name="b0",
     )
 
 
 @keras_export(
     [
         "keras.applications.efficientnet.EfficientNetB1",
         "keras.applications.EfficientNetB1",
@@ -592,30 +594,30 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
-    **kwargs,
+    name="efficientnetb1",
 ):
     return EfficientNet(
         1.0,
         1.1,
         240,
         0.2,
-        model_name="efficientnetb1",
+        name=name,
         include_top=include_top,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
         classifier_activation=classifier_activation,
-        **kwargs,
+        weights_name="b1",
     )
 
 
 @keras_export(
     [
         "keras.applications.efficientnet.EfficientNetB2",
         "keras.applications.EfficientNetB2",
@@ -625,30 +627,30 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
-    **kwargs,
+    name="efficientnetb2",
 ):
     return EfficientNet(
         1.1,
         1.2,
         260,
         0.3,
-        model_name="efficientnetb2",
+        name=name,
         include_top=include_top,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
         classifier_activation=classifier_activation,
-        **kwargs,
+        weights_name="b2",
     )
 
 
 @keras_export(
     [
         "keras.applications.efficientnet.EfficientNetB3",
         "keras.applications.EfficientNetB3",
@@ -658,30 +660,30 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
-    **kwargs,
+    name="efficientnetb3",
 ):
     return EfficientNet(
         1.2,
         1.4,
         300,
         0.3,
-        model_name="efficientnetb3",
+        name=name,
         include_top=include_top,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
         classifier_activation=classifier_activation,
-        **kwargs,
+        weights_name="b3",
     )
 
 
 @keras_export(
     [
         "keras.applications.efficientnet.EfficientNetB4",
         "keras.applications.EfficientNetB4",
@@ -691,30 +693,30 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
-    **kwargs,
+    name="efficientnetb4",
 ):
     return EfficientNet(
         1.4,
         1.8,
         380,
         0.4,
-        model_name="efficientnetb4",
+        name=name,
         include_top=include_top,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
         classifier_activation=classifier_activation,
-        **kwargs,
+        weights_name="b4",
     )
 
 
 @keras_export(
     [
         "keras.applications.efficientnet.EfficientNetB5",
         "keras.applications.EfficientNetB5",
@@ -724,30 +726,30 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
-    **kwargs,
+    name="efficientnetb5",
 ):
     return EfficientNet(
         1.6,
         2.2,
         456,
         0.4,
-        model_name="efficientnetb5",
+        name=name,
         include_top=include_top,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
         classifier_activation=classifier_activation,
-        **kwargs,
+        weights_name="b5",
     )
 
 
 @keras_export(
     [
         "keras.applications.efficientnet.EfficientNetB6",
         "keras.applications.EfficientNetB6",
@@ -757,30 +759,30 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
-    **kwargs,
+    name="efficientnetb6",
 ):
     return EfficientNet(
         1.8,
         2.6,
         528,
         0.5,
-        model_name="efficientnetb6",
+        name=name,
         include_top=include_top,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
         classifier_activation=classifier_activation,
-        **kwargs,
+        weights_name="b6",
     )
 
 
 @keras_export(
     [
         "keras.applications.efficientnet.EfficientNetB7",
         "keras.applications.EfficientNetB7",
@@ -790,30 +792,30 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
-    **kwargs,
+    name="efficientnetb7",
 ):
     return EfficientNet(
         2.0,
         3.1,
         600,
         0.5,
-        model_name="efficientnetb7",
+        name=name,
         include_top=include_top,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
         classifier_activation=classifier_activation,
-        **kwargs,
+        weights_name="b7",
     )
 
 
 EfficientNetB0.__doc__ = BASE_DOCSTRING.format(name="EfficientNetB0")
 EfficientNetB1.__doc__ = BASE_DOCSTRING.format(name="EfficientNetB1")
 EfficientNetB2.__doc__ = BASE_DOCSTRING.format(name="EfficientNetB2")
 EfficientNetB3.__doc__ = BASE_DOCSTRING.format(name="EfficientNetB3")
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/applications/efficientnet_v2.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/applications/efficientnet_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -575,14 +575,15 @@
         ImageNet classes).
     classifier_activation: A string or callable. The activation function to use
         on the "top" layer. Ignored unless `include_top=True`. Set
         `classifier_activation=None` to return the logits of the "top" layer.
         Defaults to `"softmax"`.
         When loading pretrained weights, `classifier_activation` can only
         be `None` or `"softmax"`.
+    name: The name of the model (string).
 
 Returns:
     A model instance.
 """
 
 
 def round_filters(filters, width_coefficient, min_depth, depth_divisor):
@@ -826,23 +827,24 @@
     dropout_rate=0.2,
     drop_connect_rate=0.2,
     depth_divisor=8,
     min_depth=8,
     bn_momentum=0.9,
     activation="swish",
     blocks_args="default",
-    model_name="efficientnetv2",
+    name="efficientnetv2",
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
     include_preprocessing=True,
+    weights_name=None,
 ):
     """Instantiates the EfficientNetV2 architecture using given scaling
     coefficients.
 
     Args:
         width_coefficient: float, scaling coefficient for network width.
         depth_coefficient: float, scaling coefficient for network depth.
@@ -850,15 +852,15 @@
         dropout_rate: float, dropout rate before final classifier layer.
         drop_connect_rate: float, dropout rate at skip connections.
         depth_divisor: integer, a unit of network width.
         min_depth: integer, minimum number of filters.
         bn_momentum: float. Momentum parameter for Batch Normalization layers.
         activation: activation function.
         blocks_args: list of dicts, parameters to construct block modules.
-        model_name: string, model name.
+        name: string, model name.
         include_top: whether to include the fully-connected layer at the top of
             the network.
         weights: one of `None` (random initialization), `"imagenet"`
             (pre-training on ImageNet),
             or the path to the weights file to be loaded.
         input_tensor: optional Keras tensor (i.e. output of `layers.Input()`) or
             numpy array to use as image input for the model.
@@ -884,15 +886,15 @@
             Defaults to `True`.
 
     Returns:
         A model instance.
     """
 
     if blocks_args == "default":
-        blocks_args = DEFAULT_BLOCKS_ARGS[model_name]
+        blocks_args = DEFAULT_BLOCKS_ARGS[name]
 
     if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
             "`None` (random initialization), `imagenet` "
             "(pre-training on ImageNet), "
             "or the path to the weights file to be loaded."
@@ -927,15 +929,15 @@
 
     x = img_input
 
     if include_preprocessing:
         # Apply original V1 preprocessing for Bx variants
         # if number of channels allows it
         num_channels = input_shape[bn_axis - 1]
-        if model_name.split("-")[-1].startswith("b") and num_channels == 3:
+        if name.split("-")[-1].startswith("b") and num_channels == 3:
             x = layers.Rescaling(scale=1.0 / 255)(x)
             x = layers.Normalization(
                 mean=[0.485, 0.456, 0.406],
                 variance=[0.229**2, 0.224**2, 0.225**2],
                 axis=bn_axis,
             )(x)
         else:
@@ -1053,25 +1055,25 @@
     # any potential predecessors of `input_tensor`.
     if input_tensor is not None:
         inputs = operation_utils.get_source_inputs(input_tensor)
     else:
         inputs = img_input
 
     # Create model.
-    model = Functional(inputs, x, name=model_name)
+    model = Functional(inputs, x, name=name)
 
     # Load weights.
     if weights == "imagenet":
         if include_top:
             file_suffix = ".h5"
-            file_hash = WEIGHTS_HASHES[model_name[-2:]][0]
+            file_hash = WEIGHTS_HASHES[weights_name][0]
         else:
             file_suffix = "_notop.h5"
-            file_hash = WEIGHTS_HASHES[model_name[-2:]][1]
-        file_name = model_name + file_suffix
+            file_hash = WEIGHTS_HASHES[weights_name][1]
+        file_name = name + file_suffix
         weights_path = file_utils.get_file(
             file_name,
             BASE_WEIGHTS_PATH + file_name,
             cache_subdir="models",
             file_hash=file_hash,
         )
         model.load_weights(weights_path)
@@ -1092,28 +1094,30 @@
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
     include_preprocessing=True,
+    name="efficientnetv2-b0",
 ):
     return EfficientNetV2(
         width_coefficient=1.0,
         depth_coefficient=1.0,
         default_size=224,
-        model_name="efficientnetv2-b0",
+        name=name,
         include_top=include_top,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
         classifier_activation=classifier_activation,
         include_preprocessing=include_preprocessing,
+        weights_name="b0",
     )
 
 
 @keras_export(
     [
         "keras.applications.efficientnet_v2.EfficientNetV2B1",
         "keras.applications.EfficientNetV2B1",
@@ -1124,28 +1128,30 @@
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
     include_preprocessing=True,
+    name="efficientnetv2-b1",
 ):
     return EfficientNetV2(
         width_coefficient=1.0,
         depth_coefficient=1.1,
         default_size=240,
-        model_name="efficientnetv2-b1",
+        name=name,
         include_top=include_top,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
         classifier_activation=classifier_activation,
         include_preprocessing=include_preprocessing,
+        weights_name="b1",
     )
 
 
 @keras_export(
     [
         "keras.applications.efficientnet_v2.EfficientNetV2B2",
         "keras.applications.EfficientNetV2B2",
@@ -1156,28 +1162,30 @@
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
     include_preprocessing=True,
+    name="efficientnetv2-b2",
 ):
     return EfficientNetV2(
         width_coefficient=1.1,
         depth_coefficient=1.2,
         default_size=260,
-        model_name="efficientnetv2-b2",
+        name=name,
         include_top=include_top,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
         classifier_activation=classifier_activation,
         include_preprocessing=include_preprocessing,
+        weights_name="b2",
     )
 
 
 @keras_export(
     [
         "keras.applications.efficientnet_v2.EfficientNetV2B3",
         "keras.applications.EfficientNetV2B3",
@@ -1188,28 +1196,30 @@
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
     include_preprocessing=True,
+    name="efficientnetv2-b3",
 ):
     return EfficientNetV2(
         width_coefficient=1.2,
         depth_coefficient=1.4,
         default_size=300,
-        model_name="efficientnetv2-b3",
+        name=name,
         include_top=include_top,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
         classifier_activation=classifier_activation,
         include_preprocessing=include_preprocessing,
+        weights_name="b3",
     )
 
 
 @keras_export(
     [
         "keras.applications.efficientnet_v2.EfficientNetV2S",
         "keras.applications.EfficientNetV2S",
@@ -1220,28 +1230,30 @@
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
     include_preprocessing=True,
+    name="efficientnetv2-s",
 ):
     return EfficientNetV2(
         width_coefficient=1.0,
         depth_coefficient=1.0,
         default_size=384,
-        model_name="efficientnetv2-s",
+        name=name,
         include_top=include_top,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
         classifier_activation=classifier_activation,
         include_preprocessing=include_preprocessing,
+        weights_name="-s",
     )
 
 
 @keras_export(
     [
         "keras.applications.efficientnet_v2.EfficientNetV2M",
         "keras.applications.EfficientNetV2M",
@@ -1252,28 +1264,30 @@
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
     include_preprocessing=True,
+    name="efficientnetv2-m",
 ):
     return EfficientNetV2(
         width_coefficient=1.0,
         depth_coefficient=1.0,
         default_size=480,
-        model_name="efficientnetv2-m",
+        name=name,
         include_top=include_top,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
         classifier_activation=classifier_activation,
         include_preprocessing=include_preprocessing,
+        weights_name="-m",
     )
 
 
 @keras_export(
     [
         "keras.applications.efficientnet_v2.EfficientNetV2L",
         "keras.applications.EfficientNetV2L",
@@ -1284,28 +1298,30 @@
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
     include_preprocessing=True,
+    name="efficientnetv2-l",
 ):
     return EfficientNetV2(
         width_coefficient=1.0,
         depth_coefficient=1.0,
         default_size=480,
-        model_name="efficientnetv2-l",
+        name=name,
         include_top=include_top,
         weights=weights,
         input_tensor=input_tensor,
         input_shape=input_shape,
         pooling=pooling,
         classes=classes,
         classifier_activation=classifier_activation,
         include_preprocessing=include_preprocessing,
+        weights_name="-l",
     )
 
 
 EfficientNetV2B0.__doc__ = BASE_DOCSTRING.format(name="EfficientNetV2B0")
 EfficientNetV2B1.__doc__ = BASE_DOCSTRING.format(name="EfficientNetV2B1")
 EfficientNetV2B2.__doc__ = BASE_DOCSTRING.format(name="EfficientNetV2B2")
 EfficientNetV2B3.__doc__ = BASE_DOCSTRING.format(name="EfficientNetV2B3")
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/applications/imagenet_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/applications/inception_resnet_v2.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/applications/inception_resnet_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="inception_resnet_v2",
 ):
     """Instantiates the Inception-ResNet v2 architecture.
 
     Reference:
     - [Inception-v4, Inception-ResNet and the Impact of
        Residual Connections on Learning](https://arxiv.org/abs/1602.07261)
       (AAAI 2017)
@@ -84,14 +85,15 @@
             and if no `weights` argument is specified.
         classifier_activation: A `str` or callable.
             The activation function to use on the "top" layer.
             Ignored unless `include_top=True`.
             Set `classifier_activation=None` to return the logits
             of the "top" layer. When loading pretrained weights,
             `classifier_activation` can only be `None` or `"softmax"`.
+        name: The name of the model (string).
 
     Returns:
         A model instance.
     """
     if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
@@ -209,15 +211,15 @@
     # any potential predecessors of `input_tensor`.
     if input_tensor is not None:
         inputs = operation_utils.get_source_inputs(input_tensor)
     else:
         inputs = img_input
 
     # Create model.
-    model = Functional(inputs, x, name="inception_resnet_v2")
+    model = Functional(inputs, x, name=name)
 
     # Load weights.
     if weights == "imagenet":
         if include_top:
             fname = "inception_resnet_v2_weights_tf_dim_ordering_tf_kernels.h5"
             weights_path = file_utils.get_file(
                 fname,
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/applications/inception_v3.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/applications/inception_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="inception_v3",
 ):
     """Instantiates the Inception v3 architecture.
 
     Reference:
     - [Rethinking the Inception Architecture for Computer Vision](
         http://arxiv.org/abs/1512.00567) (CVPR 2016)
 
@@ -87,14 +88,15 @@
             into, only to be specified if `include_top` is `True`, and
             if no `weights` argument is specified. Defaults to 1000.
         classifier_activation: A `str` or callable. The activation function
             to use on the "top" layer. Ignored unless `include_top=True`.
             Set `classifier_activation=None` to return the logits of the "top"
             layer. When loading pretrained weights, `classifier_activation`
             can only be `None` or `"softmax"`.
+        name: The name of the model (string).
 
     Returns:
         A model instance.
     """
     if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
@@ -349,15 +351,15 @@
     # Ensure that the model takes into account
     # any potential predecessors of `input_tensor`.
     if input_tensor is not None:
         inputs = operation_utils.get_source_inputs(input_tensor)
     else:
         inputs = img_input
     # Create model.
-    model = Functional(inputs, x, name="inception_v3")
+    model = Functional(inputs, x, name=name)
 
     # Load weights.
     if weights == "imagenet":
         if include_top:
             weights_path = file_utils.get_file(
                 "inception_v3_weights_tf_dim_ordering_tf_kernels.h5",
                 WEIGHTS_PATH,
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/applications/mobilenet.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/applications/mobilenet_v2.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/applications/mobilenet_v3.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/applications/nasnet.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/applications/nasnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     pooling=None,
     classes=1000,
     default_size=None,
     classifier_activation="softmax",
+    name="NASNet",
 ):
     """Instantiates a NASNet model.
 
     Reference:
     - [Learning Transferable Architectures for Scalable Image Recognition](
         https://arxiv.org/abs/1707.07012) (CVPR 2018)
 
@@ -101,14 +102,15 @@
         default_size: Specifies the default image size of the model
         classifier_activation: A `str` or callable.
             The activation function to use on the "top" layer.
             Ignored unless `include_top=True`.
             Set `classifier_activation=None` to return the logits
             of the "top" layer. When loading pretrained weights,
             `classifier_activation` can only be `None` or `"softmax"`.
+        name: The name of the model (string).
 
     Returns:
         A model instance.
     """
     if backend.image_data_format() == "channels_first":
         raise ValueError(
             "NASNet does not support the `channels_first` image data "
@@ -175,16 +177,16 @@
             img_input = layers.Input(tensor=input_tensor, shape=input_shape)
         else:
             img_input = input_tensor
 
     if penultimate_filters % (24 * (filter_multiplier**2)) != 0:
         raise ValueError(
             "For NASNet-A models, the `penultimate_filters` must be a multiple "
-            "of 24 * (`filter_multiplier` ** 2). Current value: %d"
-            % penultimate_filters
+            "of 24 * (`filter_multiplier` ** 2). "
+            f"Current value: {penultimate_filters}"
         )
 
     channel_dim = 1 if backend.image_data_format() == "channels_first" else -1
     filters = penultimate_filters // 24
 
     x = layers.Conv2D(
         stem_block_filters,
@@ -205,45 +207,45 @@
         x, p, filters // (filter_multiplier**2), block_id="stem_1"
     )
     x, p = _reduction_a_cell(
         x, p, filters // filter_multiplier, block_id="stem_2"
     )
 
     for i in range(num_blocks):
-        x, p = _normal_a_cell(x, p, filters, block_id="%d" % (i))
+        x, p = _normal_a_cell(x, p, filters, block_id=f"{i}")
 
     x, p0 = _reduction_a_cell(
-        x, p, filters * filter_multiplier, block_id="reduce_%d" % (num_blocks)
+        x, p, filters * filter_multiplier, block_id=f"reduce_{num_blocks}"
     )
 
     p = p0 if not skip_reduction else p
 
     for i in range(num_blocks):
         x, p = _normal_a_cell(
             x,
             p,
             filters * filter_multiplier,
-            block_id="%d" % (num_blocks + i + 1),
+            block_id=f"{num_blocks + i + 1}",
         )
 
     x, p0 = _reduction_a_cell(
         x,
         p,
         filters * filter_multiplier**2,
-        block_id="reduce_%d" % (2 * num_blocks),
+        block_id=f"reduce_{2 * num_blocks}",
     )
 
     p = p0 if not skip_reduction else p
 
     for i in range(num_blocks):
         x, p = _normal_a_cell(
             x,
             p,
             filters * filter_multiplier**2,
-            block_id="%d" % (2 * num_blocks + i + 1),
+            block_id=f"{2 * num_blocks + i + 1}",
         )
 
     x = layers.Activation("relu")(x)
 
     if include_top:
         x = layers.GlobalAveragePooling2D()(x)
         imagenet_utils.validate_activation(classifier_activation, weights)
@@ -259,15 +261,15 @@
     # Ensure that the model takes into account
     # any potential predecessors of `input_tensor`.
     if input_tensor is not None:
         inputs = operation_utils.get_source_inputs(input_tensor)
     else:
         inputs = img_input
 
-    model = Functional(inputs, x, name="NASNet")
+    model = Functional(inputs, x, name=name)
 
     # Load weights.
     if weights == "imagenet":
         if default_size == 224:  # mobile version
             if include_top:
                 weights_path = file_utils.get_file(
                     "nasnet_mobile.h5",
@@ -320,14 +322,15 @@
     input_shape=None,
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="nasnet_mobile",
 ):
     """Instantiates a Mobile NASNet model in ImageNet mode.
 
     Reference:
     - [Learning Transferable Architectures for Scalable Image Recognition](
         https://arxiv.org/abs/1707.07012) (CVPR 2018)
 
@@ -370,14 +373,15 @@
             into, only to be specified if `include_top` is `True`, and
             if no `weights` argument is specified.
         classifier_activation: A `str` or callable. The activation function to
             use on the "top" layer. Ignored unless `include_top=True`. Set
             `classifier_activation=None` to return the logits of the "top"
             layer.  When loading pretrained weights, `classifier_activation` can
             only be `None` or `"softmax"`.
+        name: The name of the model (string).
 
     Returns:
         A Keras model instance.
     """
     if backend.backend() == "torch":
         raise ValueError(
             "NASNetMobile is not available with the torch backend "
@@ -396,14 +400,15 @@
         include_top=include_top,
         weights=weights,
         input_tensor=input_tensor,
         pooling=pooling,
         classes=classes,
         default_size=224,
         classifier_activation=classifier_activation,
+        name=name,
     )
 
 
 @keras_export(
     [
         "keras.applications.nasnet.NASNetLarge",
         "keras.applications.NASNetLarge",
@@ -413,14 +418,15 @@
     input_shape=None,
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="nasnet_large",
 ):
     """Instantiates a NASNet model in ImageNet mode.
 
     Reference:
     - [Learning Transferable Architectures for Scalable Image Recognition](
         https://arxiv.org/abs/1707.07012) (CVPR 2018)
 
@@ -463,14 +469,15 @@
             into, only to be specified if `include_top` is `True`, and
             if no `weights` argument is specified.
         classifier_activation: A `str` or callable. The activation function to
             use on the "top" layer. Ignored unless `include_top=True`. Set
             `classifier_activation=None` to return the logits of the "top"
             layer.  When loading pretrained weights, `classifier_activation`
             can only be `None` or `"softmax"`.
+        name: The name of the model (string).
 
     Returns:
         A Keras model instance.
     """
     return NASNet(
         input_shape,
         penultimate_filters=4032,
@@ -481,14 +488,15 @@
         include_top=include_top,
         weights=weights,
         input_tensor=input_tensor,
         pooling=pooling,
         classes=classes,
         default_size=331,
         classifier_activation=classifier_activation,
+        name=name,
     )
 
 
 def _separable_conv_block(
     ip, filters, kernel_size=(3, 3), strides=(1, 1), block_id=None
 ):
     """Adds 2 blocks of [relu-separable conv-batchnorm].
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/applications/resnet.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/applications/resnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,33 +45,34 @@
 }
 
 
 def ResNet(
     stack_fn,
     preact,
     use_bias,
-    model_name="resnet",
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="resnet",
+    weights_name=None,
 ):
     """Instantiates the ResNet, ResNetV2, and ResNeXt architecture.
 
     Args:
         stack_fn: A function that returns output tensor for the
             stacked residual blocks.
         preact: Whether to use pre-activation or not. `True` for ResNetV2,
             `False` for ResNet and ResNeXt.
         use_bias: Whether to use biases for convolutional layers or not.
             `True` for ResNet and ResNetV2, `False` for ResNeXt.
-        model_name: Name of the model.
+        name: Name of the model.
         include_top: Whether to include the fully-connected
             layer at the top of the network.
         weights: One of `None` (random initialization),
             `"imagenet"` (pre-training on ImageNet),
             or the path to the weights file to be loaded.
         input_tensor: Optional Keras tensor (i.e. output of `layers.Input()`)
             to use as image input for the model.
@@ -96,14 +97,15 @@
             and if no `weights` argument is specified.
         classifier_activation: A `str` or callable. The activation
             function to use on the "top" layer. Ignored unless
             `include_top=True`. Set `classifier_activation=None` to
             return the logits of the "top" layer. When loading
             pretrained weights, `classifier_activation` can only be
             `None` or `"softmax"`.
+        name: The name of the model (string).
 
     Returns:
         A Model instance.
     """
 
     if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
@@ -185,26 +187,26 @@
     # any potential predecessors of `input_tensor`.
     if input_tensor is not None:
         inputs = operation_utils.get_source_inputs(input_tensor)
     else:
         inputs = img_input
 
     # Create model.
-    model = Functional(inputs, x, name=model_name)
+    model = Functional(inputs, x, name=name)
 
     # Load weights.
-    if (weights == "imagenet") and (model_name in WEIGHTS_HASHES):
+    if (weights == "imagenet") and (weights_name in WEIGHTS_HASHES):
         if include_top:
-            file_name = model_name + "_weights_tf_dim_ordering_tf_kernels.h5"
-            file_hash = WEIGHTS_HASHES[model_name][0]
+            file_name = weights_name + "_weights_tf_dim_ordering_tf_kernels.h5"
+            file_hash = WEIGHTS_HASHES[weights_name][0]
         else:
             file_name = (
-                model_name + "_weights_tf_dim_ordering_tf_kernels_notop.h5"
+                weights_name + "_weights_tf_dim_ordering_tf_kernels_notop.h5"
             )
-            file_hash = WEIGHTS_HASHES[model_name][1]
+            file_hash = WEIGHTS_HASHES[weights_name][1]
         weights_path = file_utils.get_file(
             file_name,
             BASE_WEIGHTS_PATH + file_name,
             cache_subdir="models",
             file_hash=file_hash,
         )
         model.load_weights(weights_path)
@@ -390,34 +392,36 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="resnet50",
 ):
     """Instantiates the ResNet50 architecture."""
 
     def stack_fn(x):
         x = stack_residual_blocks_v1(x, 64, 3, stride1=1, name="conv2")
         x = stack_residual_blocks_v1(x, 128, 4, name="conv3")
         x = stack_residual_blocks_v1(x, 256, 6, name="conv4")
         return stack_residual_blocks_v1(x, 512, 3, name="conv5")
 
     return ResNet(
         stack_fn,
-        False,
-        True,
-        "resnet50",
-        include_top,
-        weights,
-        input_tensor,
-        input_shape,
-        pooling,
-        classes,
+        preact=False,
+        use_bias=True,
+        weights_name="resnet50",
+        name=name,
+        include_top=include_top,
+        weights=weights,
+        input_tensor=input_tensor,
+        input_shape=input_shape,
+        pooling=pooling,
+        classes=classes,
         classifier_activation=classifier_activation,
     )
 
 
 @keras_export(
     [
         "keras.applications.resnet.ResNet101",
@@ -428,34 +432,36 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="resnet101",
 ):
     """Instantiates the ResNet101 architecture."""
 
     def stack_fn(x):
         x = stack_residual_blocks_v1(x, 64, 3, stride1=1, name="conv2")
         x = stack_residual_blocks_v1(x, 128, 4, name="conv3")
         x = stack_residual_blocks_v1(x, 256, 23, name="conv4")
         return stack_residual_blocks_v1(x, 512, 3, name="conv5")
 
     return ResNet(
         stack_fn,
-        False,
-        True,
-        "resnet101",
-        include_top,
-        weights,
-        input_tensor,
-        input_shape,
-        pooling,
-        classes,
+        preact=False,
+        use_bias=True,
+        name=name,
+        weights_name="resnet101",
+        include_top=include_top,
+        weights=weights,
+        input_tensor=input_tensor,
+        input_shape=input_shape,
+        pooling=pooling,
+        classes=classes,
         classifier_activation=classifier_activation,
     )
 
 
 @keras_export(
     [
         "keras.applications.resnet.ResNet152",
@@ -466,34 +472,36 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="resnet152",
 ):
     """Instantiates the ResNet152 architecture."""
 
     def stack_fn(x):
         x = stack_residual_blocks_v1(x, 64, 3, stride1=1, name="conv2")
         x = stack_residual_blocks_v1(x, 128, 8, name="conv3")
         x = stack_residual_blocks_v1(x, 256, 36, name="conv4")
         return stack_residual_blocks_v1(x, 512, 3, name="conv5")
 
     return ResNet(
         stack_fn,
-        False,
-        True,
-        "resnet152",
-        include_top,
-        weights,
-        input_tensor,
-        input_shape,
-        pooling,
-        classes,
+        preact=False,
+        use_bias=True,
+        name=name,
+        weights_name="resnet152",
+        include_top=include_top,
+        weights=weights,
+        input_tensor=input_tensor,
+        input_shape=input_shape,
+        pooling=pooling,
+        classes=classes,
         classifier_activation=classifier_activation,
     )
 
 
 @keras_export(
     [
         "keras.applications.resnet50.preprocess_input",
@@ -568,14 +576,15 @@
         specified if `include_top` is `True`, and if no `weights` argument is
         specified.
     classifier_activation: A `str` or callable. The activation function to
         use on the "top" layer. Ignored unless `include_top=True`. Set
         `classifier_activation=None` to return the logits of the "top" layer.
         When loading pretrained weights, `classifier_activation` can only
         be `None` or `"softmax"`.
+    name: The name of the model (string).
 
 Returns:
     A Model instance.
 """
 
 setattr(ResNet50, "__doc__", ResNet50.__doc__ + DOC)
 setattr(ResNet101, "__doc__", ResNet101.__doc__ + DOC)
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/applications/resnet_v2.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/applications/resnet_v2.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="resnet50v2",
 ):
     """Instantiates the ResNet50V2 architecture."""
 
     def stack_fn(x):
         x = resnet.stack_residual_blocks_v2(x, 64, 3, name="conv2")
         x = resnet.stack_residual_blocks_v2(x, 128, 4, name="conv3")
         x = resnet.stack_residual_blocks_v2(x, 256, 6, name="conv4")
@@ -28,21 +29,22 @@
             x, 512, 3, stride1=1, name="conv5"
         )
 
     return resnet.ResNet(
         stack_fn,
         True,
         True,
-        "resnet50v2",
-        include_top,
-        weights,
-        input_tensor,
-        input_shape,
-        pooling,
-        classes,
+        name=name,
+        weights_name="resnet50v2",
+        include_top=include_top,
+        weights=weights,
+        input_tensor=input_tensor,
+        input_shape=input_shape,
+        pooling=pooling,
+        classes=classes,
         classifier_activation=classifier_activation,
     )
 
 
 @keras_export(
     [
         "keras.applications.ResNet101V2",
@@ -53,14 +55,15 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="resnet101v2",
 ):
     """Instantiates the ResNet101V2 architecture."""
 
     def stack_fn(x):
         x = resnet.stack_residual_blocks_v2(x, 64, 3, name="conv2")
         x = resnet.stack_residual_blocks_v2(x, 128, 4, name="conv3")
         x = resnet.stack_residual_blocks_v2(x, 256, 23, name="conv4")
@@ -68,21 +71,22 @@
             x, 512, 3, stride1=1, name="conv5"
         )
 
     return resnet.ResNet(
         stack_fn,
         True,
         True,
-        "resnet101v2",
-        include_top,
-        weights,
-        input_tensor,
-        input_shape,
-        pooling,
-        classes,
+        name=name,
+        weights_name="resnet101v2",
+        include_top=include_top,
+        weights=weights,
+        input_tensor=input_tensor,
+        input_shape=input_shape,
+        pooling=pooling,
+        classes=classes,
         classifier_activation=classifier_activation,
     )
 
 
 @keras_export(
     [
         "keras.applications.ResNet152V2",
@@ -93,14 +97,15 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="resnet152v2",
 ):
     """Instantiates the ResNet152V2 architecture."""
 
     def stack_fn(x):
         x = resnet.stack_residual_blocks_v2(x, 64, 3, name="conv2")
         x = resnet.stack_residual_blocks_v2(x, 128, 8, name="conv3")
         x = resnet.stack_residual_blocks_v2(x, 256, 36, name="conv4")
@@ -108,21 +113,22 @@
             x, 512, 3, stride1=1, name="conv5"
         )
 
     return resnet.ResNet(
         stack_fn,
         True,
         True,
-        "resnet152v2",
-        include_top,
-        weights,
-        input_tensor,
-        input_shape,
-        pooling,
-        classes,
+        name=name,
+        weights_name="resnet152v2",
+        include_top=include_top,
+        weights=weights,
+        input_tensor=input_tensor,
+        input_shape=input_shape,
+        pooling=pooling,
+        classes=classes,
         classifier_activation=classifier_activation,
     )
 
 
 @keras_export("keras.applications.resnet_v2.preprocess_input")
 def preprocess_input(x, data_format=None):
     return imagenet_utils.preprocess_input(
@@ -187,14 +193,15 @@
         specified if `include_top` is `True`, and if no `weights` argument is
         specified.
     classifier_activation: A `str` or callable. The activation function to
         use on the "top" layer. Ignored unless `include_top=True`. Set
         `classifier_activation=None` to return the logits of the "top" layer.
         When loading pretrained weights, `classifier_activation` can only
         be `None` or `"softmax"`.
+    name: The name of the model (string).
 
 Returns:
     A Model instance.
 """
 
 setattr(ResNet50V2, "__doc__", ResNet50V2.__doc__ + DOC)
 setattr(ResNet101V2, "__doc__", ResNet101V2.__doc__ + DOC)
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/applications/vgg16.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/applications/vgg16.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="vgg16",
 ):
     """Instantiates the VGG16 model.
 
     Reference:
     - [Very Deep Convolutional Networks for Large-Scale Image Recognition](
     https://arxiv.org/abs/1409.1556) (ICLR 2015)
 
@@ -82,17 +83,18 @@
             into, only to be specified if `include_top` is `True`, and
             if no `weights` argument is specified.
         classifier_activation: A `str` or callable. The activation function to
             use on the "top" layer. Ignored unless `include_top=True`. Set
             `classifier_activation=None` to return the logits of the "top"
             layer.  When loading pretrained weights, `classifier_activation`
             can only be `None` or `"softmax"`.
+        name: The name of the model (string).
 
     Returns:
-        A model instance.
+        A `Model` instance.
     """
     if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
             "`None` (random initialization), 'imagenet' "
             "(pre-training on ImageNet), "
             "or the path to the weights file to be loaded.  Received: "
@@ -197,15 +199,15 @@
     # any potential predecessors of `input_tensor`.
     if input_tensor is not None:
         inputs = operation_utils.get_source_inputs(input_tensor)
     else:
         inputs = img_input
 
     # Create model.
-    model = Functional(inputs, x, name="vgg16")
+    model = Functional(inputs, x, name=name)
 
     # Load weights.
     if weights == "imagenet":
         if include_top:
             weights_path = file_utils.get_file(
                 "vgg16_weights_tf_dim_ordering_tf_kernels.h5",
                 WEIGHTS_PATH,
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/applications/vgg19.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/applications/vgg19.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="vgg19",
 ):
     """Instantiates the VGG19 model.
 
     Reference:
     - [Very Deep Convolutional Networks for Large-Scale Image Recognition](
     https://arxiv.org/abs/1409.1556) (ICLR 2015)
 
@@ -82,14 +83,15 @@
             into, only to be specified if `include_top` is `True`, and
             if no `weights` argument is specified.
         classifier_activation: A `str` or callable. The activation function to
             use on the "top" layer. Ignored unless `include_top=True`. Set
             `classifier_activation=None` to return the logits of the "top"
             layer.  When loading pretrained weights, `classifier_activation` can
             only be `None` or `"softmax"`.
+        name: The name of the model (string).
 
     Returns:
         A model instance.
     """
     if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
@@ -205,15 +207,15 @@
     # any potential predecessors of `input_tensor`.
     if input_tensor is not None:
         inputs = operation_utils.get_source_inputs(input_tensor)
     else:
         inputs = img_input
 
     # Create model.
-    model = Functional(inputs, x, name="vgg19")
+    model = Functional(inputs, x, name=name)
 
     # Load weights.
     if weights == "imagenet":
         if include_top:
             weights_path = file_utils.get_file(
                 "vgg19_weights_tf_dim_ordering_tf_kernels.h5",
                 WEIGHTS_PATH,
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/applications/xception.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/applications/xception.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     include_top=True,
     weights="imagenet",
     input_tensor=None,
     input_shape=None,
     pooling=None,
     classes=1000,
     classifier_activation="softmax",
+    name="xception",
 ):
     """Instantiates the Xception architecture.
 
     Reference:
     - [Xception: Deep Learning with Depthwise Separable Convolutions](
         https://arxiv.org/abs/1610.02357) (CVPR 2017)
 
@@ -82,14 +83,15 @@
             into, only to be specified if `include_top` is `True`, and
             if no `weights` argument is specified.
         classifier_activation: A `str` or callable. The activation function to
             use on the "top" layer. Ignored unless `include_top=True`. Set
             `classifier_activation=None` to return the logits of the "top"
             layer.  When loading pretrained weights, `classifier_activation` can
             only be `None` or `"softmax"`.
+        name: The name of the model (string).
 
     Returns:
         A model instance.
     """
     if not (weights in {"imagenet", None} or file_utils.exists(weights)):
         raise ValueError(
             "The `weights` argument should be either "
@@ -304,15 +306,15 @@
     # Ensure that the model takes into account
     # any potential predecessors of `input_tensor`.
     if input_tensor is not None:
         inputs = operation_utils.get_source_inputs(input_tensor)
     else:
         inputs = img_input
     # Create model.
-    model = Functional(inputs, x, name="xception")
+    model = Functional(inputs, x, name=name)
 
     # Load weights.
     if weights == "imagenet":
         if include_top:
             weights_path = file_utils.get_file(
                 "xception_weights_tf_dim_ordering_tf_kernels.h5",
                 WEIGHTS_PATH,
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/common/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/common/backend_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/common/dtypes.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/common/dtypes.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/common/global_state.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/common/global_state.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/common/keras_tensor.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/common/name_scope.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/common/name_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/common/stateless_scope.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/common/variables.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/common/variables.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/config.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/exports.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/core.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/distribution_lib.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/image.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/linalg.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/linalg.py`

 * *Files 16% similar despite different names*

```diff
@@ -77,7 +77,13 @@
 
 def solve_triangular(a, b, lower=False):
     return jsp.linalg.solve_triangular(a, b, lower=lower)
 
 
 def svd(x, full_matrices=True, compute_uv=True):
     return jnp.linalg.svd(x, full_matrices=full_matrices, compute_uv=compute_uv)
+
+
+def lstsq(a, b, rcond=None):
+    a = convert_to_tensor(a)
+    b = convert_to_tensor(b)
+    return jnp.linalg.lstsq(a, b, rcond=rcond)[0]
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/math.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/nn.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/numpy.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/optimizer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/random.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/rnn.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/sparse.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/jax/trainer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/jax/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/core.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/image.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/linalg.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/linalg.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,7 +76,13 @@
         b = np.expand_dims(b, axis=-1)
         return _vectorized_solve_triangular(a, b).squeeze(axis=-1)
     return _vectorized_solve_triangular(a, b)
 
 
 def svd(x, full_matrices=True, compute_uv=True):
     return np.linalg.svd(x, full_matrices=full_matrices, compute_uv=compute_uv)
+
+
+def lstsq(a, b, rcond=None):
+    a = convert_to_tensor(a)
+    b = convert_to_tensor(b)
+    return np.linalg.lstsq(a, b, rcond=rcond)[0]
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/math.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/nn.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/numpy.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/random.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/rnn.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/numpy/trainer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/numpy/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/core.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,22 +144,30 @@
     tensor values when the shape is unknown (this is tf specific, as dynamic
     shapes do not apply in other backends).
     """
     if isinstance(x, KerasTensor):
         return x.shape
     if not tf.is_tensor(x):
         x = tf.convert_to_tensor(x)
-    dynamic = tf.shape(x)
     if x.shape == tf.TensorShape(None):
         raise ValueError(
             "All tensors passed to `ops.shape` must have a statically known "
             f"rank. Received: x={x} with unknown rank."
         )
-    static = x.shape.as_list()
-    return tuple(dynamic[i] if s is None else s for i, s in enumerate(static))
+    shape = x.shape.as_list()
+    dynamic = tf.shape(x)
+    for i in range(len(shape)):
+        if shape[i] is None:
+            try:
+                shape[i] = dynamic[i]
+            except:
+                # With RaggedTensors, accessing a ragged dimension will fail,
+                # we leave it as None.
+                pass
+    return tuple(shape)
 
 
 def cast(x, dtype):
     dtype = standardize_dtype(dtype)
     if isinstance(x, tf.SparseTensor):
         x_shape = x.shape
         x = tf.cast(x, dtype)
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/distribution_lib.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/image.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/layer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/linalg.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/linalg.py`

 * *Files 11% similar despite different names*

```diff
@@ -185,7 +185,48 @@
 
 
 def svd(x, full_matrices=True, compute_uv=True):
     s, u, v = tf.linalg.svd(
         x, full_matrices=full_matrices, compute_uv=compute_uv
     )
     return u, s, tf.linalg.adjoint(v)
+
+
+def lstsq(a, b, rcond=None):
+    a = convert_to_tensor(a)
+    b = convert_to_tensor(b)
+    if a.shape[0] != b.shape[0]:
+        raise ValueError("Leading dimensions of input arrays must match")
+    b_orig_ndim = b.ndim
+    if b_orig_ndim == 1:
+        b = b[:, None]
+    if a.ndim != 2:
+        raise TypeError(
+            f"{a.ndim}-dimensional array given. "
+            "Array must be two-dimensional"
+        )
+    if b.ndim != 2:
+        raise TypeError(
+            f"{b.ndim}-dimensional array given. "
+            "Array must be one or two-dimensional"
+        )
+    m, n = a.shape
+    dtype = a.dtype
+    eps = tf.experimental.numpy.finfo(dtype).eps
+    if a.shape == ():
+        s = tf.zeros(0, dtype=a.dtype)
+        x = tf.zeros((n, *b.shape[1:]), dtype=a.dtype)
+    else:
+        if rcond is None:
+            rcond = eps * max(n, m)
+        else:
+            rcond = tf.where(rcond < 0, eps, rcond)
+        u, s, vt = svd(a, full_matrices=False)
+        mask = s >= tf.convert_to_tensor(rcond, dtype=s.dtype) * s[0]
+        safe_s = tf.cast(tf.where(mask, s, 1), dtype=a.dtype)
+        s_inv = tf.where(mask, 1 / safe_s, 0)[:, tf.newaxis]
+        u_t_b = tf.matmul(tf.transpose(tf.math.conj(u)), b)
+        x = tf.matmul(tf.transpose(tf.math.conj(vt)), s_inv * u_t_b)
+
+    if b_orig_ndim == 1:
+        x = tf.reshape(x, [-1])
+    return x
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/math.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/nn.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/numpy.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/optimizer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/random.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/rnn.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/sparse.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/sparse.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/trackable.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/tensorflow/trainer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/tensorflow/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/core.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/image.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/layer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/linalg.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/linalg.py`

 * *Files 18% similar despite different names*

```diff
@@ -68,7 +68,13 @@
 
 def svd(x, full_matrices=True, compute_uv=True):
     if not compute_uv:
         raise NotImplementedError(
             "`compute_uv=False` is not supported for torch backend."
         )
     return torch.linalg.svd(x, full_matrices=full_matrices)
+
+
+def lstsq(a, b, rcond=None):
+    a = convert_to_tensor(a)
+    b = convert_to_tensor(b)
+    return torch.linalg.lstsq(a, b, rcond=rcond)[0]
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/math.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/nn.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/numpy.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_adam.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_lion.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/random.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/rnn.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/backend/torch/trainer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/backend/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/backup_and_restore.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/callback.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/callback_list.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/csv_logger.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/early_stopping.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/history.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/lambda_callback.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/learning_rate_scheduler.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/model_checkpoint.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/progbar_logger.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/remote_monitor.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/swap_ema_weights.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/tensorboard.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/callbacks/terminate_on_nan.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/constraints/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/constraints/constraints.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/datasets/boston_housing.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/datasets/california_housing.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/datasets/cifar.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/datasets/cifar10.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/datasets/cifar100.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/datasets/fashion_mnist.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/datasets/imdb.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/datasets/mnist.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/datasets/reuters.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/distribution/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/distribution/distribution_lib.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/dtype_policies/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/dtype_policies/dtype_policy.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/dtype_policies/dtype_policy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/export/export_lib.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/export/export_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/initializers/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/initializers/constant_initializers.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/initializers/initializer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/initializers/random_initializers.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/activations/activation.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/activations/elu.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/activations/leaky_relu.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/activations/prelu.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/activations/relu.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/activations/softmax.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/attention/additive_attention.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/attention/attention.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/attention/grouped_query_attention.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/attention/multi_head_attention.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/base_conv.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/base_conv_transpose.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/base_separable_conv.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/conv1d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/conv1d_transpose.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/conv2d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/conv2d_transpose.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/conv3d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/conv3d_transpose.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/separable_conv1d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/convolutional/separable_conv2d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/core/dense.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/core/dense.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/core/einsum_dense.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/core/einsum_dense.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/core/embedding.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/core/embedding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/core/identity.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/core/input_layer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/core/lambda_layer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/core/masking.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/core/wrapper.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/input_spec.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/input_spec.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/layer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/add.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/average.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/base_merge.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/concatenate.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/dot.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/maximum.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/minimum.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/multiply.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/merging/subtract.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/normalization/batch_normalization.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/normalization/group_normalization.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/normalization/layer_normalization.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/normalization/spectral_normalization.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/normalization/unit_normalization.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/average_pooling1d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/average_pooling2d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/average_pooling3d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/base_global_pooling.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/base_pooling.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/global_average_pooling1d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/global_average_pooling2d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/global_average_pooling3d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/global_max_pooling1d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/global_max_pooling2d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/global_max_pooling3d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/max_pooling1d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/max_pooling2d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/pooling/max_pooling3d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/category_encoding.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/center_crop.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/discretization.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/feature_space.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/feature_space.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/hashed_crossing.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/hashing.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/index_lookup.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/integer_lookup.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/normalization.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/random_brightness.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/random_contrast.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/random_crop.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/random_flip.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/random_rotation.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/random_translation.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/random_zoom.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/rescaling.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/resizing.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/string_lookup.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/string_lookup.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/text_vectorization.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/preprocessing/tf_data_layer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/regularization/activity_regularization.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/regularization/alpha_dropout.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/regularization/dropout.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/regularization/gaussian_dropout.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/regularization/gaussian_noise.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/regularization/spatial_dropout.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/cropping1d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/cropping2d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/cropping3d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/flatten.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/permute.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/repeat_vector.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/reshape.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/up_sampling1d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/up_sampling2d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/up_sampling3d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/zero_padding1d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/zero_padding2d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/reshaping/zero_padding3d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/bidirectional.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/conv_lstm.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/conv_lstm1d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/conv_lstm2d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/conv_lstm3d.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/gru.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/lstm.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/rnn.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/simple_rnn.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/layers/rnn/time_distributed.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/legacy/backend.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/legacy/layers.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/legacy/losses.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/legacy/preprocessing/image.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/legacy/preprocessing/sequence.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/legacy/preprocessing/text.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/legacy/saving/json_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/legacy/saving/legacy_h5_format.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/legacy/saving/saving_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/legacy/saving/serialization.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/losses/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/losses/loss.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/losses/loss.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/losses/losses.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/losses/losses.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/metrics/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/metrics/accuracy_metrics.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/metrics/confusion_metrics.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/metrics/f_score_metrics.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/metrics/hinge_metrics.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/metrics/iou_metrics.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/metrics/metric.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/metrics/metrics_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/metrics/probabilistic_metrics.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/metrics/reduction_metrics.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/metrics/reduction_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/metrics/regression_metrics.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/models/cloning.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/models/cloning.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/models/functional.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/models/functional.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/models/model.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/models/model.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/models/sequential.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/models/sequential.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/models/variable_mapping.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/models/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/ops/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/ops/core.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/ops/core.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/ops/function.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/ops/function.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/ops/image.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/ops/image.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/ops/linalg.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/ops/linalg.py`

 * *Files 3% similar despite different names*

```diff
@@ -589,14 +589,91 @@
 
 def _svd(x, full_matrices=True, compute_uv=True):
     x = backend.convert_to_tensor(x)
     _assert_2d(x)
     return backend.linalg.svd(x, full_matrices, compute_uv)
 
 
+class Lstsq(Operation):
+    def __init__(self, rcond=None):
+        super().__init__()
+        self.rcond = rcond
+
+    def call(self, a, b):
+        return backend.linalg.lstsq(a, b, rcond=self.rcond)
+
+    def compute_output_spec(self, a, b):
+        if len(a.shape) != 2:
+            raise ValueError(
+                "Expected a to have rank 2. " f"Received: a.shape={a.shape}"
+            )
+        if len(b.shape) not in (1, 2):
+            raise ValueError(
+                "Expected b to have rank 1 or 2. "
+                f"Received: b.shape={b.shape}"
+            )
+        m, n = a.shape
+        if b.shape[0] != m:
+            raise ValueError(
+                "Expected b.shape[0] to be equal to "
+                "a.shape[0]. Received: "
+                f"a.shape={a.shape}, b.shape={b.shape}"
+            )
+        if len(b.shape) == 2:
+            k = b.shape[1]
+            x = KerasTensor((n, k), dtype=a.dtype)
+        else:
+            x = KerasTensor((n,), dtype=a.dtype)
+        return x
+
+
+@keras_export(["keras.ops.lstsq", "keras.ops.linalg.lstsq"])
+def lstsq(a, b, rcond=None):
+    """Return the least-squares solution to a linear matrix equation.
+
+    Computes the vector x that approximately solves the equation
+    `a @ x = b`. The equation may be under-, well-, or over-determined
+    (i.e., the number of linearly independent rows of a can be less than,
+    equal to, or greater than its number of linearly independent columns).
+    If a is square and of full rank, then `x` (but for round-off error)
+    is the exact solution of the equation. Else, `x` minimizes the
+    L2 norm of `b - a * x`.
+
+    If there are multiple minimizing solutions,
+    the one with the smallest L2 norm  is returned.
+
+    Args:
+        a: "Coefficient" matrix of shape `(M, N)`.
+        b: Ordinate or "dependent variable" values,
+            of shape `(M,)` or `(M, K)`.
+            If `b` is two-dimensional, the least-squares solution
+            is calculated for each of the K columns of `b`.
+        rcond: Cut-off ratio for small singular values of `a`.
+            For the purposes of rank determination,
+            singular values are treated as zero if they are
+            smaller than rcond times the largest
+            singular value of `a`.
+
+    Returns:
+        Tensor with shape `(N,)` or `(N, K)` containing
+        the least-squares solutions.
+
+    **NOTE:** The output differs from `numpy.linalg.lstsq`.
+    NumPy returns a tuple with four elements, the first of which
+    being the least-squares solutions and the others
+    being essentially never used.
+    Keras only returns the first value. This is done both
+    to ensure consistency across backends (which cannot be achieved
+    for the other values) and to simplify the API.
+    """
+    if any_symbolic_tensors((a, b)):
+        return Lstsq(rcond=rcond).symbolic_call(a, b)
+    return backend.linalg.lstsq(a, b, rcond=rcond)
+
+
 def _assert_1d(*arrays):
     for a in arrays:
         if a.ndim < 1:
             raise ValueError(
                 "Expected input to have rank >= 1. "
                 "Received scalar input {a}."
             )
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/ops/math.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/ops/nn.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/ops/nn.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/ops/node.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/ops/numpy.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/ops/numpy.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/ops/operation.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/ops/operation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/ops/operation_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/ops/symbolic_arguments.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/ops/symbolic_arguments.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/adadelta.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/adadelta.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/adafactor.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/adagrad.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/adam.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/adamax.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/adamax.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/adamw.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/base_optimizer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/ftrl.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/lion.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/loss_scale_optimizer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/nadam.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/optimizer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/rmsprop.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/schedules/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/optimizers/sgd.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/quantizers/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/quantizers/quantizers.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/quantizers/quantizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/random/random.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/random/seed_generator.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/regularizers/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/regularizers/regularizers.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/saving/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/saving/keras_saveable.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/saving/keras_saveable.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/saving/object_registration.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/saving/saving_api.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/saving/saving_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/saving/saving_lib.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/saving/saving_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/saving/serialization_lib.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/testing/test_case.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/testing/test_case.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/testing/test_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/trainers/compile_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/trainers/compile_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/array_slicing.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/data_adapter.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/trainers/epoch_iterator.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/trainers/trainer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/tree/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/tree/dmtree_impl.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/tree/dmtree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/tree/optree_impl.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/tree/optree_impl.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/tree/tree_api.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/tree/tree_api.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/__init__.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/argument_validation.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/audio_dataset_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/audio_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/backend_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/code_stats.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/dataset_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/dtype_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/file_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/image_dataset_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/image_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/image_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/io_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/jax_layer.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/jax_layer.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/model_visualization.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/module_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/naming.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/numerical_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/progbar.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/python_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/rng_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/sequence_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/summary_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/text_dataset_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/text_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/tf_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/timeseries_dataset_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/torch_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/traceback_utils.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras/src/utils/tracking.py` & `keras_nightly-3.3.3.dev2024051103/keras/src/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/keras_nightly.egg-info/PKG-INFO` & `keras_nightly-3.3.3.dev2024051103/keras_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras-nightly
-Version: 3.3.3.dev2024050903
+Version: 3.3.3.dev2024051103
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keras_nightly-3.3.3.dev2024050903/keras_nightly.egg-info/SOURCES.txt` & `keras_nightly-3.3.3.dev2024051103/keras_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keras_nightly-3.3.3.dev2024050903/setup.py` & `keras_nightly-3.3.3.dev2024051103/setup.py`

 * *Files identical despite different names*

