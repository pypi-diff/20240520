# Comparing `tmp/mlfab-0.1.8.tar.gz` & `tmp/mlfab-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlfab-0.1.8.tar", last modified: Fri Mar 15 06:43:37 2024, max compression
+gzip compressed data, was "mlfab-0.1.9.tar", last modified: Wed Apr 17 06:42:00 2024, max compression
```

## Comparing `mlfab-0.1.8.tar` & `mlfab-0.1.9.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:37.423963 mlfab-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-15 06:43:31.000000 mlfab-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-15 06:43:31.000000 mlfab-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-03-15 06:43:37.423963 mlfab-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8128 2024-03-15 06:43:31.000000 mlfab-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:37.403963 mlfab-0.1.8/mlfab/
--rw-r--r--   0 runner    (1001) docker     (127)    24601 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:37.403963 mlfab-0.1.8/mlfab/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/core/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:37.407963 mlfab-0.1.8/mlfab/nn/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/activations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:37.407963 mlfab-0.1.8/mlfab/nn/architectures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/architectures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42793 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/architectures/attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/architectures/bifpn.py
--rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/architectures/monotonic_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/architectures/next_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    25995 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/architectures/rwkv.py
--rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/architectures/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:37.411963 mlfab-0.1.8/mlfab/nn/device/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/device/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/device/metal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:37.411963 mlfab-0.1.8/mlfab/nn/diffusion/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/diffusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/diffusion/consistency.py
--rw-r--r--   0 runner    (1001) docker     (127)    20251 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/diffusion/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/diffusion/ode.py
--rw-r--r--   0 runner    (1001) docker     (127)    13865 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (127)    19486 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (127)    56505 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)    25992 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/lr_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/norms.py
--rw-r--r--   0 runner    (1001) docker     (127)    14960 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (127)    43786 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:37.411963 mlfab-0.1.8/mlfab/nn/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/quantization/fsq.py
--rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/quantization/lfq.py
--rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/quantization/vq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:37.411963 mlfab-0.1.8/mlfab/nn/triton/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (127)    10435 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/triton/monotonic_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)    29357 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/nn/triton/rwkv.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:37.415964 mlfab-0.1.8/mlfab/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:37.415964 mlfab-0.1.8/mlfab/task/launchers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/launchers/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/launchers/multi_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/launchers/single_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    15508 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/launchers/staged.py
--rw-r--r--   0 runner    (1001) docker     (127)    54910 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:37.415964 mlfab-0.1.8/mlfab/task/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/loggers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/loggers/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:37.419963 mlfab-0.1.8/mlfab/task/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/mixins/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/mixins/checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/mixins/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/mixins/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9394 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/mixins/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/mixins/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/mixins/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/mixins/runnable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    23984 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/mixins/train.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/task/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:37.419963 mlfab-0.1.8/mlfab/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:37.423963 mlfab-0.1.8/mlfab/utils/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/utils/data/collate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/utils/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/utils/data/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/utils/data/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    25822 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/utils/experiments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/utils/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-03-15 06:43:31.000000 mlfab-0.1.8/mlfab/utils/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:37.423963 mlfab-0.1.8/mlfab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-03-15 06:43:37.000000 mlfab-0.1.8/mlfab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-03-15 06:43:37.000000 mlfab-0.1.8/mlfab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 06:43:37.000000 mlfab-0.1.8/mlfab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-15 06:43:37.000000 mlfab-0.1.8/mlfab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-15 06:43:37.000000 mlfab-0.1.8/mlfab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-03-15 06:43:31.000000 mlfab-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-15 06:43:37.423963 mlfab-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-15 06:43:31.000000 mlfab-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:43:37.423963 mlfab-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-15 06:43:31.000000 mlfab-0.1.8/tests/test_import_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:42:00.660723 mlfab-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-17 06:41:55.000000 mlfab-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-17 06:41:55.000000 mlfab-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-17 06:42:00.660723 mlfab-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8128 2024-04-17 06:41:55.000000 mlfab-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:42:00.640723 mlfab-0.1.9/mlfab/
+-rw-r--r--   0 runner    (1001) docker     (127)    24601 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:42:00.644723 mlfab-0.1.9/mlfab/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6976 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/core/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:42:00.644723 mlfab-0.1.9/mlfab/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:42:00.648723 mlfab-0.1.9/mlfab/nn/architectures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/architectures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42916 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/architectures/attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6508 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/architectures/bifpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/architectures/monotonic_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/architectures/next_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25985 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/architectures/rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/architectures/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:42:00.648723 mlfab-0.1.9/mlfab/nn/device/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/device/metal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:42:00.648723 mlfab-0.1.9/mlfab/nn/diffusion/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/diffusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11894 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/diffusion/consistency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20251 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/diffusion/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/diffusion/ode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13865 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19486 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5167 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56505 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25992 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/lr_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14683 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/norms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14960 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43786 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:42:00.648723 mlfab-0.1.9/mlfab/nn/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/quantization/fsq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6897 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/quantization/lfq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/quantization/vq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:42:00.652723 mlfab-0.1.9/mlfab/nn/triton/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10435 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/triton/monotonic_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29357 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/nn/triton/rwkv.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:42:00.652723 mlfab-0.1.9/mlfab/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:42:00.652723 mlfab-0.1.9/mlfab/task/launchers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/launchers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/launchers/multi_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/launchers/single_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15508 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/launchers/staged.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54922 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:42:00.656723 mlfab-0.1.9/mlfab/task/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/loggers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/loggers/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:42:00.656723 mlfab-0.1.9/mlfab/task/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/mixins/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/mixins/checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/mixins/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/mixins/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9394 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/mixins/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/mixins/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/mixins/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/mixins/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23982 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/mixins/train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/task/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:42:00.660723 mlfab-0.1.9/mlfab/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:42:00.660723 mlfab-0.1.9/mlfab/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7467 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/utils/data/collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/utils/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/utils/data/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/utils/data/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25822 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/utils/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/utils/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15009 2024-04-17 06:41:55.000000 mlfab-0.1.9/mlfab/utils/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:42:00.660723 mlfab-0.1.9/mlfab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-17 06:42:00.000000 mlfab-0.1.9/mlfab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-17 06:42:00.000000 mlfab-0.1.9/mlfab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 06:42:00.000000 mlfab-0.1.9/mlfab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-17 06:42:00.000000 mlfab-0.1.9/mlfab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-17 06:42:00.000000 mlfab-0.1.9/mlfab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-17 06:41:55.000000 mlfab-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-17 06:42:00.660723 mlfab-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-17 06:41:55.000000 mlfab-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 06:42:00.660723 mlfab-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-17 06:41:55.000000 mlfab-0.1.9/tests/test_import_helper.py
```

### Comparing `mlfab-0.1.8/LICENSE` & `mlfab-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/PKG-INFO` & `mlfab-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlfab
-Version: 0.1.8
+Version: 0.1.9
 Summary: A collection of core machine learning tools
 Home-page: https://github.com/dpshai/mlfab
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mlfab-0.1.8/README.md` & `mlfab-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/__init__.py` & `mlfab-0.1.9/mlfab/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 This file can be maintained by running the update script:
 
 .. code-block:: bash
 
     python -m scripts.update_api --inplace
 """
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 # This list shouldn't be modified by hand; instead, run the update script.
 __all__ = [
     "UserConfig",
     "field",
     "get_data_dir",
     "get_pretrained_models_dir",
```

### Comparing `mlfab-0.1.8/mlfab/core/conf.py` & `mlfab-0.1.9/mlfab/core/conf.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/core/state.py` & `mlfab-0.1.9/mlfab/core/state.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/activations.py` & `mlfab-0.1.9/mlfab/nn/activations.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/architectures/attention.py` & `mlfab-0.1.9/mlfab/nn/architectures/attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -1055,46 +1055,47 @@
             num_layers=num_layers,
             norm=norm,
             use_rotary=use_rotary,
             rotary_base=rotary_base,
         )
         self.proj = nn.Linear(d_model, vocab_size)
 
-    def forward(self, tokens_bt: Tensor, emb_btc: Tensor) -> Tensor:
+    def forward(self, tokens_bt: Tensor, emb_btc: Tensor) -> tuple[Tensor, Tensor]:
         x_btc = self.embeddings(tokens_bt[:, :-1])
         x_btc = torch.cat((self.init_emb.expand(x_btc.size(0), 1, -1), x_btc), dim=1)
         x_btc = x_btc + emb_btc
         x_btc, _ = self.attn(x_btc, is_causal=True)
         logits_btc = self.proj(x_btc)
-        return logits_btc
+        return logits_btc, x_btc
 
     def infer(
         self,
         emb_btc: Tensor,
-        bsz: int = 1,
         sampling_strategy: SamplingStrategy = "top-p",
         k: int | None = None,
         p: float | None = 0.95,
         temperature: float = 1.0,
-    ) -> Tensor:
-        x_b1c: Tensor = self.init_emb.expand(bsz, 1, -1)
+    ) -> tuple[Tensor, Tensor]:
+        x_b1c: Tensor = self.init_emb.expand(emb_btc.size(0), 1, -1)
         x_b1c = x_b1c + emb_btc[:, :1]
         x_b1c, state = self.attn(x_b1c)
         logits_b1l = self.proj(x_b1c)
         tokens_bt = sample_from_logits(logits_b1l, sampling_strategy, k=k, p=p, temperature=temperature)
         tokens_b1 = tokens_bt[:, :1]
 
+        x_list_btc = [x_b1c]
         for t in range(1, emb_btc.size(1)):
             x_b1c = self.embeddings(tokens_b1) + emb_btc[:, t : t + 1]
             x_b1c, state = self.attn(x_b1c, state)
+            x_list_btc.append(x_b1c)
             logits_b1l = self.proj(x_b1c)
             tokens_b1 = sample_from_logits(logits_b1l, sampling_strategy, k=k, p=p, temperature=temperature)
             tokens_bt = torch.cat((tokens_bt, tokens_b1), dim=1)
 
-        return tokens_bt
+        return tokens_bt, torch.cat(x_list_btc, dim=1)
 
 
 T = TypeVar("T", bound=nn.Module)
 
 
 def _get_clones(module: T, num_layers: int) -> list[T]:
     return cast(list[T], nn.ModuleList([copy.deepcopy(module) for _ in range(num_layers)]))
```

### Comparing `mlfab-0.1.8/mlfab/nn/architectures/bifpn.py` & `mlfab-0.1.9/mlfab/nn/architectures/bifpn.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/architectures/monotonic_attention.py` & `mlfab-0.1.9/mlfab/nn/architectures/monotonic_attention.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/architectures/next_token.py` & `mlfab-0.1.9/mlfab/nn/architectures/next_token.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/architectures/rwkv.py` & `mlfab-0.1.9/mlfab/nn/architectures/rwkv.py`

 * *Files 1% similar despite different names*

```diff
@@ -720,21 +720,20 @@
         x_btc, _ = self.rwkv(x_btc)
         logits_btc = self.proj(x_btc)
         return logits_btc
 
     def infer(
         self,
         emb_btc: Tensor,
-        bsz: int = 1,
         sampling_strategy: SamplingStrategy = "top-p",
         k: int | None = None,
         p: float | None = 0.95,
         temperature: float = 1.0,
     ) -> Tensor:
-        x_b1c: Tensor = self.init_emb.expand(bsz, 1, -1)
+        x_b1c: Tensor = self.init_emb.expand(emb_btc.size(0), 1, -1)
         x_b1c = x_b1c + emb_btc[:, :1]
         x_b1c, state = self.rwkv(x_b1c)
         logits_b1l = self.proj(x_b1c)
         tokens_bt = sample_from_logits(logits_b1l, sampling_strategy, k=k, p=p, temperature=temperature)
         tokens_b1 = tokens_bt[:, :1]
 
         for t in range(1, emb_btc.size(1)):
```

### Comparing `mlfab-0.1.8/mlfab/nn/architectures/unet.py` & `mlfab-0.1.9/mlfab/nn/architectures/unet.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/device/auto.py` & `mlfab-0.1.9/mlfab/nn/device/auto.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/device/base.py` & `mlfab-0.1.9/mlfab/nn/device/base.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/device/cpu.py` & `mlfab-0.1.9/mlfab/nn/device/cpu.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/device/gpu.py` & `mlfab-0.1.9/mlfab/nn/device/gpu.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/device/metal.py` & `mlfab-0.1.9/mlfab/nn/device/metal.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/diffusion/consistency.py` & `mlfab-0.1.9/mlfab/nn/diffusion/consistency.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/diffusion/gaussian.py` & `mlfab-0.1.9/mlfab/nn/diffusion/gaussian.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/diffusion/ode.py` & `mlfab-0.1.9/mlfab/nn/diffusion/ode.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/embeddings.py` & `mlfab-0.1.9/mlfab/nn/embeddings.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/functions.py` & `mlfab-0.1.9/mlfab/nn/functions.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/init.py` & `mlfab-0.1.9/mlfab/nn/init.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/kmeans.py` & `mlfab-0.1.9/mlfab/nn/kmeans.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/lora.py` & `mlfab-0.1.9/mlfab/nn/lora.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/losses.py` & `mlfab-0.1.9/mlfab/nn/losses.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/lr_schedulers.py` & `mlfab-0.1.9/mlfab/nn/lr_schedulers.py`

 * *Files 3% similar despite different names*

```diff
@@ -114,36 +114,43 @@
             if not specified.
         min_scale: The minimum learning rate scale.
         decay: Whether to decay the learning rate after warmup.
     """
 
     def __init__(
         self,
-        total_steps: int,
+        total_steps: int | None = None,
         warmup_steps: int | None = None,
         warmup_percent: float = 0.01,
         min_scale: float = 1e-4,
         decay: bool = True,
     ) -> None:
         super().__init__()
 
         if warmup_steps is None:
+            if total_steps is None:
+                raise ValueError(
+                    "If `total_steps` is not specified, then `warmup_steps` cannot be inferred from `warmup_percent`. "
+                    "You should therefore specify the number of warmup steps explicitly."
+                )
             warmup_steps = round(total_steps * warmup_percent)
 
         self.total_steps = total_steps
         self.warmup_steps = warmup_steps
         self.min_scale = min_scale
         self.decay = decay
 
     def get_lr_scale(self, state: State) -> float:
         warmup, total, min_scale = self.warmup_steps, self.total_steps, self.min_scale
         if state.num_steps < warmup:
             return state.num_steps / warmup
         if not self.decay:
             return 1.0
+        if total is None:
+            return 1.0
         if state.num_steps < total:
             return (1 - min_scale) * (total - state.num_steps) / (total - warmup) + min_scale
         return min_scale
 
 
 class CosineLRScheduler(BaseLRScheduler):
     """Defines a cosine learning rate schedule.
@@ -156,34 +163,35 @@
         ramp_up_steps: The number of steps to spend ramping up.
         eta_min: The minimum learning rate scale.
         eta_max: The maximum learning rate scale.
     """
 
     def __init__(
         self,
-        total_steps: int,
+        total_steps: int | None = None,
         num_resets: int = 0,
         phase: int | None = None,
         ramp_up_percent: float = 0.05,
         ramp_up_steps: int | None = None,
         eta_min: float = 0.01,
         eta_max: float = 1.0,
     ) -> None:
         super().__init__()
 
         if phase is None:
+            if total_steps is None:
+                raise ValueError("If `total_steps` is not specified, then `phase` must be specified.")
             phase = int(total_steps / (num_resets + 1))
         if ramp_up_steps is None:
             assert 0.0 <= ramp_up_percent < 1.0
             ramp_up_steps = round(phase * ramp_up_percent)
         else:
             assert ramp_up_steps < phase
 
         self.phase = phase
-        self.total_steps = total_steps
         self.ramp_up_steps = ramp_up_steps
         self.eta_min = eta_min
         self.eta_max = eta_max
 
     def get_lr_scale(self, state: State) -> float:
         phase, ramp_up = self.phase, self.ramp_up_steps
         eta_min, eta_max = self.eta_min, self.eta_max
```

### Comparing `mlfab-0.1.8/mlfab/nn/norms.py` & `mlfab-0.1.9/mlfab/nn/norms.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/optimizers.py` & `mlfab-0.1.9/mlfab/nn/optimizers.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/parallel.py` & `mlfab-0.1.9/mlfab/nn/parallel.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/quantization/fsq.py` & `mlfab-0.1.9/mlfab/nn/quantization/fsq.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/quantization/lfq.py` & `mlfab-0.1.9/mlfab/nn/quantization/lfq.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/quantization/vq.py` & `mlfab-0.1.9/mlfab/nn/quantization/vq.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/triton/__init__.py` & `mlfab-0.1.9/mlfab/nn/triton/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/triton/kmeans.py` & `mlfab-0.1.9/mlfab/nn/triton/kmeans.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/triton/lion.py` & `mlfab-0.1.9/mlfab/nn/triton/lion.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/triton/monotonic_attention.py` & `mlfab-0.1.9/mlfab/nn/triton/monotonic_attention.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/nn/triton/rwkv.py` & `mlfab-0.1.9/mlfab/nn/triton/rwkv.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/base.py` & `mlfab-0.1.9/mlfab/task/base.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/launchers/base.py` & `mlfab-0.1.9/mlfab/task/launchers/base.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/launchers/cli.py` & `mlfab-0.1.9/mlfab/task/launchers/cli.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/launchers/multi_process.py` & `mlfab-0.1.9/mlfab/task/launchers/multi_process.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/launchers/single_process.py` & `mlfab-0.1.9/mlfab/task/launchers/single_process.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/launchers/slurm.py` & `mlfab-0.1.9/mlfab/task/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/launchers/staged.py` & `mlfab-0.1.9/mlfab/task/launchers/staged.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/logger.py` & `mlfab-0.1.9/mlfab/task/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import math
 import re
 import time
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from dataclasses import dataclass
 from types import TracebackType
-from typing import Callable, Iterator, Literal, Self, Sequence, TypeVar, get_args
+from typing import Callable, Iterator, Literal, Self, Sequence, TypeVar, cast, get_args
 
 import torch
 import torch.nn.functional as F
 import torchvision.transforms.functional as V
 from omegaconf import DictConfig
 from PIL import Image, ImageDraw, ImageFont
 from torch import Tensor
@@ -419,15 +419,15 @@
         return image
     if max_num_lines is None:
         max_num_lines = len(text)
     else:
         text = text[:max_num_lines]
     pil_image = V.to_pil_image(image)
     width, height = pil_image.size
-    font: ImageFont.ImageFont = ImageFont.load_default()
+    font = cast(ImageFont.ImageFont, ImageFont.load_default())
     _, _, _, line_height = font.getbbox(text[0])
     new_width, new_height = width, height + line_spacing + max_num_lines * (line_height + line_spacing)
     padded_image = Image.new(pil_image.mode, (new_width, new_height), 255)
     padded_image.paste(pil_image, (0, 0))
     drawer = ImageDraw.Draw(padded_image)
     for i, text_line in enumerate(text):
         text_line_top = height + line_spacing + i * (line_height + line_spacing)
```

### Comparing `mlfab-0.1.8/mlfab/task/loggers/json.py` & `mlfab-0.1.9/mlfab/task/loggers/json.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/loggers/state.py` & `mlfab-0.1.9/mlfab/task/loggers/state.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/loggers/stdout.py` & `mlfab-0.1.9/mlfab/task/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/loggers/tensorboard.py` & `mlfab-0.1.9/mlfab/task/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/mixins/__init__.py` & `mlfab-0.1.9/mlfab/task/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/mixins/artifacts.py` & `mlfab-0.1.9/mlfab/task/mixins/artifacts.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/mixins/checkpointing.py` & `mlfab-0.1.9/mlfab/task/mixins/checkpointing.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/mixins/compile.py` & `mlfab-0.1.9/mlfab/task/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/mixins/cpu_stats.py` & `mlfab-0.1.9/mlfab/task/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/mixins/data_loader.py` & `mlfab-0.1.9/mlfab/task/mixins/data_loader.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/mixins/device.py` & `mlfab-0.1.9/mlfab/task/mixins/device.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/mixins/gpu_stats.py` & `mlfab-0.1.9/mlfab/task/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/mixins/logger.py` & `mlfab-0.1.9/mlfab/task/mixins/logger.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/mixins/mixed_precision.py` & `mlfab-0.1.9/mlfab/task/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/mixins/optimizer.py` & `mlfab-0.1.9/mlfab/task/mixins/optimizer.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/mixins/process.py` & `mlfab-0.1.9/mlfab/task/mixins/process.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/mixins/profiler.py` & `mlfab-0.1.9/mlfab/task/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/mixins/runnable.py` & `mlfab-0.1.9/mlfab/task/mixins/runnable.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/mixins/step_wrapper.py` & `mlfab-0.1.9/mlfab/task/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/mixins/train.py` & `mlfab-0.1.9/mlfab/task/mixins/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,18 +283,18 @@
 
     def get_single_loss(self, loss: Tensor | dict[str, Tensor]) -> tuple[Tensor, list[str]]:
         if isinstance(loss, Tensor):
             if loss.ndim == 0:
                 return loss.unsqueeze(0), ["loss"]
             if loss.ndim == 1:
                 return loss, ["loss"]
-            return loss.sum().unsqueeze(0) / loss.shape[0], ["loss"]
+            return loss.sum().unsqueeze(0) / loss.size(0), ["loss"]
         assert isinstance(loss, dict), f"Single loss should be a scalar or dictionary, not {type(loss)}"
         keys, values = (list(i) for i in zip(*sorted(loss.items())))
-        losses = [v.sum() / v.shape[0] if v.ndim > 0 else v for v in values]
+        losses = [v.sum() / v.size(0) if v.ndim > 0 else v for v in values]
         single_loss = torch.stack(losses, dim=0)
         return single_loss, keys
 
     def get_single_losses(self, losses: Loss) -> list[tuple[Tensor, list[str]]]:
         if isinstance(losses, (Tensor, dict)):
             return [self.get_single_loss(losses)]
         assert isinstance(losses, list), f"Loss should be a scalar, dictionary, or list, not {type(losses)}"
```

### Comparing `mlfab-0.1.8/mlfab/task/script.py` & `mlfab-0.1.9/mlfab/task/script.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/task/task.py` & `mlfab-0.1.9/mlfab/task/task.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/utils/data/collate.py` & `mlfab-0.1.9/mlfab/utils/data/collate.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/utils/data/dataset.py` & `mlfab-0.1.9/mlfab/utils/data/dataset.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/utils/data/error_handling.py` & `mlfab-0.1.9/mlfab/utils/data/error_handling.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/utils/data/transforms.py` & `mlfab-0.1.9/mlfab/utils/data/transforms.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/utils/experiments.py` & `mlfab-0.1.9/mlfab/utils/experiments.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/utils/io.py` & `mlfab-0.1.9/mlfab/utils/io.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/utils/logging.py` & `mlfab-0.1.9/mlfab/utils/logging.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/utils/text.py` & `mlfab-0.1.9/mlfab/utils/text.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab/utils/tokens.py` & `mlfab-0.1.9/mlfab/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/mlfab.egg-info/PKG-INFO` & `mlfab-0.1.9/mlfab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlfab
-Version: 0.1.8
+Version: 0.1.9
 Summary: A collection of core machine learning tools
 Home-page: https://github.com/dpshai/mlfab
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mlfab-0.1.8/mlfab.egg-info/SOURCES.txt` & `mlfab-0.1.9/mlfab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/pyproject.toml` & `mlfab-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mlfab-0.1.8/setup.py` & `mlfab-0.1.9/setup.py`

 * *Files identical despite different names*

