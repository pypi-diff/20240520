# Comparing `tmp/danling-0.3.5.tar.gz` & `tmp/danling-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danling-0.3.5.tar", last modified: Thu May  9 10:48:18 2024, max compression
+gzip compressed data, was "danling-0.3.6.tar", last modified: Mon May 20 13:02:08 2024, max compression
```

## Comparing `danling-0.3.5.tar` & `danling-0.3.6.tar`

### file list

```diff
@@ -1,150 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.411428 danling-0.3.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.379428 danling-0.3.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-09 10:48:14.000000 danling-0.3.5/.github/merge_rules.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.379428 danling-0.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-09 10:48:14.000000 danling-0.3.5/.github/workflows/push.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-05-09 10:48:14.000000 danling-0.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-09 10:48:14.000000 danling-0.3.5/.pre-commit-config.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)       88 2024-05-09 10:48:14.000000 danling-0.3.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.379428 danling-0.3.5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-09 10:48:14.000000 danling-0.3.5/LICENSES/LICENSE.AGPL
--rwxr-xr-x   0 runner    (1001) docker     (127)    11357 2024-05-09 10:48:14.000000 danling-0.3.5/LICENSES/LICENSE.Apache
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-09 10:48:14.000000 danling-0.3.5/LICENSES/LICENSE.BSD
--rwxr-xr-x   0 runner    (1001) docker     (127)    18092 2024-05-09 10:48:14.000000 danling-0.3.5/LICENSES/LICENSE.GPLv2
--rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-05-09 10:48:14.000000 danling-0.3.5/LICENSES/LICENSE.GPLv3
--rwxr-xr-x   0 runner    (1001) docker     (127)     1083 2024-05-09 10:48:14.000000 danling-0.3.5/LICENSES/LICENSE.MIT
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-09 10:48:14.000000 danling-0.3.5/LICENSES/LICENSE.Unlicense
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-09 10:48:18.411428 danling-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-09 10:48:14.000000 danling-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-09 10:48:14.000000 danling-0.3.5/anaconda-project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.379428 danling-0.3.5/danling/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-09 10:48:14.000000 danling-0.3.5/danling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 10:48:18.000000 danling-0.3.5/danling/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.383428 danling-0.3.5/danling/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-09 10:48:14.000000 danling-0.3.5/danling/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9609 2024-05-09 10:48:14.000000 danling-0.3.5/danling/metrics/average_meter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-09 10:48:14.000000 danling-0.3.5/danling/metrics/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    21784 2024-05-09 10:48:14.000000 danling-0.3.5/danling/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-09 10:48:14.000000 danling-0.3.5/danling/metrics/multitask.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-09 10:48:14.000000 danling-0.3.5/danling/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.383428 danling-0.3.5/danling/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.383428 danling-0.3.5/danling/modules/mlp/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/mlp/dense.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/mlp/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.383428 danling-0.3.5/danling/modules/transformer/
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.383428 danling-0.3.5/danling/modules/transformer/attention/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/attention/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11127 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/attention/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/attention/simple_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.387428 danling-0.3.5/danling/modules/transformer/ffn/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/ffn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/ffn/fcn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.387428 danling-0.3.5/danling/modules/transformer/pos_embed/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/pos_embed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-09 10:48:14.000000 danling-0.3.5/danling/modules/transformer/pos_embed/pos_embed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.387428 danling-0.3.5/danling/optim/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-09 10:48:14.000000 danling-0.3.5/danling/optim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.387428 danling-0.3.5/danling/optim/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-09 10:48:14.000000 danling-0.3.5/danling/optim/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7624 2024-05-09 10:48:14.000000 danling-0.3.5/danling/optim/lr_scheduler/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-09 10:48:14.000000 danling-0.3.5/danling/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.387428 danling-0.3.5/danling/runner/
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-09 10:48:14.000000 danling-0.3.5/danling/runner/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-09 10:48:14.000000 danling-0.3.5/danling/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19827 2024-05-09 10:48:14.000000 danling-0.3.5/danling/runner/accelerate_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    44104 2024-05-09 10:48:14.000000 danling-0.3.5/danling/runner/base_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-09 10:48:14.000000 danling-0.3.5/danling/runner/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     6133 2024-05-09 10:48:14.000000 danling-0.3.5/danling/runner/state.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-09 10:48:14.000000 danling-0.3.5/danling/runner/torch_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-09 10:48:14.000000 danling-0.3.5/danling/runner/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.387428 danling-0.3.5/danling/tensors/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-09 10:48:14.000000 danling-0.3.5/danling/tensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-09 10:48:14.000000 danling-0.3.5/danling/tensors/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    44356 2024-05-09 10:48:14.000000 danling-0.3.5/danling/tensors/nested_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-09 10:48:14.000000 danling-0.3.5/danling/tensors/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-09 10:48:14.000000 danling-0.3.5/danling/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.391428 danling-0.3.5/danling/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-09 10:48:14.000000 danling-0.3.5/danling/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-09 10:48:14.000000 danling-0.3.5/danling/utils/basex.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-09 10:48:14.000000 danling-0.3.5/danling/utils/contextmanagers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-05-09 10:48:14.000000 danling-0.3.5/danling/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-09 10:48:14.000000 danling-0.3.5/danling/utils/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-09 10:48:14.000000 danling-0.3.5/danling/utils/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.407428 danling-0.3.5/danling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-09 10:48:18.000000 danling-0.3.5/danling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-05-09 10:48:18.000000 danling-0.3.5/danling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 10:48:18.000000 danling-0.3.5/danling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-09 10:48:18.000000 danling-0.3.5/danling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-09 10:48:18.000000 danling-0.3.5/danling.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.375428 danling-0.3.5/demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.391428 danling-0.3.5/demo/vision/
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-09 10:48:14.000000 danling-0.3.5/demo/vision/torch_mnist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.391428 danling-0.3.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.391428 danling-0.3.5/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/CNAME
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.391428 danling-0.3.5/docs/docs/blog/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/blog/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/manifest.webmanifest
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.391428 danling-0.3.5/docs/docs/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/metrics/average_meter.md
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/metrics/metrics.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.391428 danling-0.3.5/docs/docs/optim/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/optim/lr_scheduler.md
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/package.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.391428 danling-0.3.5/docs/docs/runner/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/runner/accelerate_runner.md
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/runner/base_runner.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/runner/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/runner/state.md
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/runner/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.395428 danling-0.3.5/docs/docs/tensors/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/tensors/nested_tensor.md
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/tensors/pn_tensor.md
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/tensors/torch_func_registry.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.395428 danling-0.3.5/docs/docs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/utils/basex.md
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/utils/contextmanagers.md
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/utils/decorators.md
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-09 10:48:14.000000 danling-0.3.5/docs/docs/utils/io.md
--rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-09 10:48:14.000000 danling-0.3.5/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.395428 danling-0.3.5/docs/overrides/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.375428 danling-0.3.5/docs/overrides/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.395428 danling-0.3.5/docs/overrides/assets/css/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/assets/css/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/assets/css/fonts.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.407428 danling-0.3.5/docs/overrides/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   213368 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/assets/fonts/CascadiaCodePL.woff2
--rw-r--r--   0 runner    (1001) docker     (127)  8530056 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/assets/fonts/HYQiHei.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   118704 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/assets/fonts/HelveticaNowDisplay.otf
--rw-r--r--   0 runner    (1001) docker     (127)   656232 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/assets/fonts/HelveticaWorld.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.407428 danling-0.3.5/docs/overrides/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/assets/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    21972 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/assets/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.407428 danling-0.3.5/docs/overrides/javascripts/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/javascripts/shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-09 10:48:14.000000 danling-0.3.5/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-09 10:48:14.000000 danling-0.3.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-09 10:48:14.000000 danling-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-09 10:48:14.000000 danling-0.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 10:48:18.411428 danling-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 10:48:14.000000 danling-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.375428 danling-0.3.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.407428 danling-0.3.5/tests/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)    16380 2024-05-09 10:48:14.000000 danling-0.3.5/tests/metrics/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.407428 danling-0.3.5/tests/optim/
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-05-09 10:48:14.000000 danling-0.3.5/tests/optim/test_lr_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.407428 danling-0.3.5/tests/runner/
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-09 10:48:14.000000 danling-0.3.5/tests/runner/test_base_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-09 10:48:14.000000 danling-0.3.5/tests/runner/test_torch_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.407428 danling-0.3.5/tests/tensors/
--rw-r--r--   0 runner    (1001) docker     (127)     9983 2024-05-09 10:48:14.000000 danling-0.3.5/tests/tensors/test_nested_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 10:48:18.407428 danling-0.3.5/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-09 10:48:14.000000 danling-0.3.5/tests/utils/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-09 10:48:14.000000 danling-0.3.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.081216 danling-0.3.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.053216 danling-0.3.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-20 13:02:04.000000 danling-0.3.6/.github/merge_rules.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.053216 danling-0.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-20 13:02:04.000000 danling-0.3.6/.github/workflows/push.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-05-20 13:02:04.000000 danling-0.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-20 13:02:04.000000 danling-0.3.6/.pre-commit-config.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)       88 2024-05-20 13:02:04.000000 danling-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-20 13:02:04.000000 danling-0.3.6/LICENSE.header
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.053216 danling-0.3.6/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-20 13:02:04.000000 danling-0.3.6/LICENSES/LICENSE.AGPL
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11357 2024-05-20 13:02:04.000000 danling-0.3.6/LICENSES/LICENSE.Apache
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-20 13:02:04.000000 danling-0.3.6/LICENSES/LICENSE.BSD
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18092 2024-05-20 13:02:04.000000 danling-0.3.6/LICENSES/LICENSE.GPLv2
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35149 2024-05-20 13:02:04.000000 danling-0.3.6/LICENSES/LICENSE.GPLv3
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1083 2024-05-20 13:02:04.000000 danling-0.3.6/LICENSES/LICENSE.MIT
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-20 13:02:04.000000 danling-0.3.6/LICENSES/LICENSE.Unlicense
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-20 13:02:08.081216 danling-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-20 13:02:04.000000 danling-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-20 13:02:04.000000 danling-0.3.6/anaconda-project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.053216 danling-0.3.6/danling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-20 13:02:04.000000 danling-0.3.6/danling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 13:02:07.000000 danling-0.3.6/danling/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.057216 danling-0.3.6/danling/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-20 13:02:04.000000 danling-0.3.6/danling/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-05-20 13:02:04.000000 danling-0.3.6/danling/metrics/average_meter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-05-20 13:02:04.000000 danling-0.3.6/danling/metrics/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22358 2024-05-20 13:02:04.000000 danling-0.3.6/danling/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-20 13:02:04.000000 danling-0.3.6/danling/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.057216 danling-0.3.6/danling/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-20 13:02:04.000000 danling-0.3.6/danling/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.057216 danling-0.3.6/danling/modules/mlp/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-20 13:02:04.000000 danling-0.3.6/danling/modules/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-20 13:02:04.000000 danling-0.3.6/danling/modules/mlp/dense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-05-20 13:02:04.000000 danling-0.3.6/danling/modules/mlp/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.057216 danling-0.3.6/danling/modules/transformer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-20 13:02:04.000000 danling-0.3.6/danling/modules/transformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.057216 danling-0.3.6/danling/modules/transformer/attention/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-20 13:02:04.000000 danling-0.3.6/danling/modules/transformer/attention/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-05-20 13:02:04.000000 danling-0.3.6/danling/modules/transformer/attention/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-20 13:02:04.000000 danling-0.3.6/danling/modules/transformer/attention/simple_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-20 13:02:04.000000 danling-0.3.6/danling/modules/transformer/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-20 13:02:04.000000 danling-0.3.6/danling/modules/transformer/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.057216 danling-0.3.6/danling/modules/transformer/ffn/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-20 13:02:04.000000 danling-0.3.6/danling/modules/transformer/ffn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-20 13:02:04.000000 danling-0.3.6/danling/modules/transformer/ffn/fcn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.057216 danling-0.3.6/danling/modules/transformer/pos_embed/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-20 13:02:04.000000 danling-0.3.6/danling/modules/transformer/pos_embed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-05-20 13:02:04.000000 danling-0.3.6/danling/modules/transformer/pos_embed/pos_embed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.057216 danling-0.3.6/danling/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-20 13:02:04.000000 danling-0.3.6/danling/optim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.057216 danling-0.3.6/danling/optim/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-20 13:02:04.000000 danling-0.3.6/danling/optim/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-05-20 13:02:04.000000 danling-0.3.6/danling/optim/lr_scheduler/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-20 13:02:04.000000 danling-0.3.6/danling/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.061216 danling-0.3.6/danling/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-20 13:02:04.000000 danling-0.3.6/danling/runner/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-20 13:02:04.000000 danling-0.3.6/danling/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20423 2024-05-20 13:02:04.000000 danling-0.3.6/danling/runner/accelerate_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44776 2024-05-20 13:02:04.000000 danling-0.3.6/danling/runner/base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-20 13:02:04.000000 danling-0.3.6/danling/runner/defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6729 2024-05-20 13:02:04.000000 danling-0.3.6/danling/runner/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-20 13:02:04.000000 danling-0.3.6/danling/runner/torch_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-20 13:02:04.000000 danling-0.3.6/danling/runner/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.061216 danling-0.3.6/danling/tensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-20 13:02:04.000000 danling-0.3.6/danling/tensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-05-20 13:02:04.000000 danling-0.3.6/danling/tensors/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44952 2024-05-20 13:02:04.000000 danling-0.3.6/danling/tensors/nested_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-20 13:02:04.000000 danling-0.3.6/danling/tensors/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-20 13:02:04.000000 danling-0.3.6/danling/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.061216 danling-0.3.6/danling/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-20 13:02:04.000000 danling-0.3.6/danling/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-05-20 13:02:04.000000 danling-0.3.6/danling/utils/basex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-20 13:02:04.000000 danling-0.3.6/danling/utils/contextmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-20 13:02:04.000000 danling-0.3.6/danling/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-20 13:02:04.000000 danling-0.3.6/danling/utils/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-05-20 13:02:04.000000 danling-0.3.6/danling/utils/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.081216 danling-0.3.6/danling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-20 13:02:07.000000 danling-0.3.6/danling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3208 2024-05-20 13:02:08.000000 danling-0.3.6/danling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:02:07.000000 danling-0.3.6/danling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-20 13:02:07.000000 danling-0.3.6/danling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 13:02:07.000000 danling-0.3.6/danling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.049216 danling-0.3.6/demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.061216 danling-0.3.6/demo/vision/
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-20 13:02:04.000000 danling-0.3.6/demo/vision/torch_mnist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.061216 danling-0.3.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.061216 danling-0.3.6/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/CNAME
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.061216 danling-0.3.6/docs/docs/blog/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/blog/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/manifest.webmanifest
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.061216 danling-0.3.6/docs/docs/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/metrics/average_meter.md
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/metrics/metrics.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.065216 danling-0.3.6/docs/docs/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/optim/lr_scheduler.md
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/package.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.065216 danling-0.3.6/docs/docs/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/runner/accelerate_runner.md
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/runner/base_runner.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/runner/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/runner/state.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/runner/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.065216 danling-0.3.6/docs/docs/tensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/tensors/nested_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/tensors/pn_tensor.md
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/tensors/torch_func_registry.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.065216 danling-0.3.6/docs/docs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/utils/basex.md
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/utils/contextmanagers.md
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/utils/decorators.md
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-20 13:02:04.000000 danling-0.3.6/docs/docs/utils/io.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5460 2024-05-20 13:02:04.000000 danling-0.3.6/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.065216 danling-0.3.6/docs/overrides/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.049216 danling-0.3.6/docs/overrides/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.065216 danling-0.3.6/docs/overrides/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-20 13:02:04.000000 danling-0.3.6/docs/overrides/assets/css/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-20 13:02:04.000000 danling-0.3.6/docs/overrides/assets/css/fonts.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.077216 danling-0.3.6/docs/overrides/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   213368 2024-05-20 13:02:04.000000 danling-0.3.6/docs/overrides/assets/fonts/CascadiaCodePL.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)  8530056 2024-05-20 13:02:04.000000 danling-0.3.6/docs/overrides/assets/fonts/HYQiHei.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   118704 2024-05-20 13:02:04.000000 danling-0.3.6/docs/overrides/assets/fonts/HelveticaNowDisplay.otf
+-rw-r--r--   0 runner    (1001) docker     (127)   656232 2024-05-20 13:02:04.000000 danling-0.3.6/docs/overrides/assets/fonts/HelveticaWorld.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.077216 danling-0.3.6/docs/overrides/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     8116 2024-05-20 13:02:04.000000 danling-0.3.6/docs/overrides/assets/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    21972 2024-05-20 13:02:04.000000 danling-0.3.6/docs/overrides/assets/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.077216 danling-0.3.6/docs/overrides/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-20 13:02:04.000000 danling-0.3.6/docs/overrides/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-20 13:02:04.000000 danling-0.3.6/docs/overrides/javascripts/shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-05-20 13:02:04.000000 danling-0.3.6/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-20 13:02:04.000000 danling-0.3.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-20 13:02:04.000000 danling-0.3.6/licensing.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-20 13:02:04.000000 danling-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-20 13:02:04.000000 danling-0.3.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:02:08.081216 danling-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 13:02:04.000000 danling-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.049216 danling-0.3.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.077216 danling-0.3.6/tests/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)    16976 2024-05-20 13:02:04.000000 danling-0.3.6/tests/metrics/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.077216 danling-0.3.6/tests/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)     5731 2024-05-20 13:02:04.000000 danling-0.3.6/tests/optim/test_lr_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.077216 danling-0.3.6/tests/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-20 13:02:04.000000 danling-0.3.6/tests/runner/test_base_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-20 13:02:04.000000 danling-0.3.6/tests/runner/test_torch_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.081216 danling-0.3.6/tests/tensors/
+-rw-r--r--   0 runner    (1001) docker     (127)    10579 2024-05-20 13:02:04.000000 danling-0.3.6/tests/tensors/test_nested_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:02:08.081216 danling-0.3.6/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-20 13:02:04.000000 danling-0.3.6/tests/utils/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-20 13:02:04.000000 danling-0.3.6/tox.ini
```

### Comparing `danling-0.3.5/.github/workflows/push.yaml` & `danling-0.3.6/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/.gitignore` & `danling-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/.pre-commit-config.yaml` & `danling-0.3.6/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
       - id: check-xml
       - id: check-toml
       - id: check-yaml
         files: danling
       - id: debug-statements
         exclude: danling/utils/contextmanagers.py
       - id: end-of-file-fixer
+        exclude: LICENSE.header
       - id: fix-byte-order-marker
       - id: fix-encoding-pragma
         args: ["--remove"]
       - id: mixed-line-ending
         args: ["--fix=lf"]
       - id: requirements-txt-fixer
       - id: trailing-whitespace
```

### Comparing `danling-0.3.5/LICENSES/LICENSE.AGPL` & `danling-0.3.6/LICENSES/LICENSE.AGPL`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/LICENSES/LICENSE.Apache` & `danling-0.3.6/LICENSES/LICENSE.Apache`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/LICENSES/LICENSE.BSD` & `danling-0.3.6/LICENSES/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/LICENSES/LICENSE.GPLv2` & `danling-0.3.6/LICENSES/LICENSE.GPLv2`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/LICENSES/LICENSE.GPLv3` & `danling-0.3.6/LICENSES/LICENSE.GPLv3`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/LICENSES/LICENSE.MIT` & `danling-0.3.6/LICENSES/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/LICENSES/LICENSE.Unlicense` & `danling-0.3.6/LICENSES/LICENSE.Unlicense`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/PKG-INFO` & `danling-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.3.5
+Version: 0.3.6
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR AGPL-3.0-or-later OR GPL-2.0-or-later OR BSD-4-Clause OR MIT OR Apache-2.0
         
 Project-URL: documentation, https://danling.org
 Project-URL: homepage, https://danling.org
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: LICENSE.header
 Requires-Dist: cached-property; python_version < "3.8"
 Requires-Dist: chanfig>=0.0.96
 Requires-Dist: gitpython
 Requires-Dist: lazy-imports
 Requires-Dist: strenum; python_version < "3.11"
 Requires-Dist: tqdm
 Provides-Extra: jax
```

### Comparing `danling-0.3.5/README.md` & `danling-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/anaconda-project.yml` & `danling-0.3.6/anaconda-project.yml`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/danling/metrics/average_meter.py` & `danling-0.3.6/danling/metrics/average_meter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,32 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 from __future__ import annotations
 
 from typing import Any, Dict
 
-from chanfig import NestedDict
+from chanfig import FlatDict, NestedDict
 from torch import distributed as dist
 
-from .multitask import MultiTaskDict
-from .utils import get_world_size
+from .utils import MetricsDict, MultiTaskDict, get_world_size
 
 
 class AverageMeter:
     r"""
     Computes and stores the average and current value.
 
     Attributes:
@@ -140,18 +156,115 @@
     def avg(self):
         return self.average()
 
     def __format__(self, format_spec) -> str:
         return f"{self.val.__format__(format_spec)} ({self.avg.__format__(format_spec)})"
 
 
-class MultiTaskAverageMeter(MultiTaskDict):
+class AverageMeters(MetricsDict):
+    """
+    Examples:
+        >>> meters = AverageMeters()
+        >>> meters.update({"loss": 0.6, "auroc": 0.7, "r2": 0.8})
+        >>> print(f"{meters:.4f}")
+        loss: 0.6000 (0.6000)
+        auroc: 0.7000 (0.7000)
+        r2: 0.8000 (0.8000)
+        >>> meters.update({"loss": {"value": 0.9, "n": 1}})
+        >>> print(f"{meters:.4f}")
+        loss: 0.9000 (0.7500)
+        auroc: 0.7000 (0.7000)
+        r2: 0.8000 (0.8000)
+        >>> meters.sum.dict()
+        {'loss': 1.5, 'auroc': 0.7, 'r2': 0.8}
+        >>> meters.count.dict()
+        {'loss': 2, 'auroc': 1, 'r2': 1}
+        >>> meters.reset()
+        >>> print(f"{meters:.4f}")
+        loss: 0.0000 (nan)
+        auroc: 0.0000 (nan)
+        r2: 0.0000 (nan)
+    """
+
+    def __init__(self, *args, default_factory=AverageMeter, **kwargs) -> None:
+        super().__init__(*args, default_factory=default_factory, **kwargs)
+
+    @property
+    def sum(self) -> FlatDict[str, float]:
+        return FlatDict({key: meter.sum for key, meter in self.all_items()})
+
+    @property
+    def count(self) -> FlatDict[str, int]:
+        return FlatDict({key: meter.count for key, meter in self.all_items()})
+
+    def update(self, values: Dict, *, n: int = 1) -> None:  # pylint: disable=W0237
+        r"""
+        Updates the average and current value in all meters.
+
+        Args:
+            values: Dict of values to be added to the average.
+            n: Number of values to be added.
+
+        Raises:
+            ValueError: If the value is not an instance of (int, float, Mapping).
+
+        Examples:
+            >>> meters = AverageMeters()
+            >>> meters.update({"loss": 0.6, "auroc": 0.7, "r2": 0.8})
+            >>> meters.sum.dict()
+            {'loss': 0.6, 'auroc': 0.7, 'r2': 0.8}
+            >>> meters.count.dict()
+            {'loss': 1, 'auroc': 1, 'r2': 1}
+            >>> meters.update({"loss": {"value": 0.9, "n": 1}})
+            >>> meters.sum.dict()
+            {'loss': 1.5, 'auroc': 0.7, 'r2': 0.8}
+            >>> meters.count.dict()
+            {'loss': 2, 'auroc': 1, 'r2': 1}
+            >>> meters.update({"loss": 0.8, "auroc": 0.9, "r2": 0.8})
+            >>> meters.sum.dict()
+            {'loss': 2.3, 'auroc': 1.6, 'r2': 1.6}
+            >>> meters.count.dict()
+            {'loss': 3, 'auroc': 2, 'r2': 2}
+            >>> meters.update({"auroc": 0.7, "r2": 0.7})
+            >>> meters.sum.dict()
+            {'loss': 2.3, 'auroc': 2.3, 'r2': 2.3}
+            >>> meters.count.dict()
+            {'loss': 3, 'auroc': 3, 'r2': 3}
+            >>> meters.update({"dataset1": {"cls.auroc": 0.9}, "dataset1.reg.r2": 0.8, "dataset2.r2": 0.9})
+            Traceback (most recent call last):
+            ValueError: Expected values to be int, float, or a flat dictionary, but got <class 'dict'>
+            This is likely due to nested dictionary in the values.
+            Nested dictionaries cannot be processed due to the method's design, which uses Mapping to pass both value and count ('n'). Ensure your input is a flat dictionary or a single value.
+            >>> meters.update(dict(loss=""))
+            Traceback (most recent call last):
+            ValueError: Expected values to be int, float, or a flat dictionary, but got <class 'str'>
+        """  # noqa: E501
+
+        for meter, value in values.items():
+            if isinstance(value, (int, float)):
+                self[meter].update(value, n)
+            elif isinstance(value, Dict):
+                value.setdefault("n", n)
+                try:
+                    self[meter].update(**value)
+                except TypeError:
+                    raise ValueError(
+                        f"Expected values to be int, float, or a flat dictionary, but got {type(value)}\n"
+                        "This is likely due to nested dictionary in the values.\n"
+                        "Nested dictionaries cannot be processed due to the method's design, which uses Mapping "
+                        "to pass both value and count ('n'). Ensure your input is a flat dictionary or a single value."
+                    ) from None
+            else:
+                raise ValueError(f"Expected values to be int, float, or a flat dictionary, but got {type(value)}")
+
+
+class MultiTaskAverageMeters(MultiTaskDict):
     """
     Examples:
-        >>> meters = MultiTaskAverageMeter()
+        >>> meters = MultiTaskAverageMeters()
         >>> meters.update({"loss": 0.6, "dataset1.cls.auroc": 0.7, "dataset1.reg.r2": 0.8, "dataset2.r2": 0.9})
         >>> print(f"{meters:.4f}")
         loss: 0.6000 (0.6000)
         dataset1.cls.auroc: 0.7000 (0.7000)
         dataset1.reg.r2: 0.8000 (0.8000)
         dataset2.r2: 0.9000 (0.9000)
         >>> meters.update({"loss": {"value": 0.9, "n": 1}})
@@ -166,15 +279,15 @@
         {'loss': 2, 'dataset1': {'cls': {'auroc': 1}, 'reg': {'r2': 1}}, 'dataset2': {'r2': 1}}
         >>> meters.reset()
         >>> print(f"{meters:.4f}")
         loss: 0.0000 (nan)
         dataset1.cls.auroc: 0.0000 (nan)
         dataset1.reg.r2: 0.0000 (nan)
         dataset2.r2: 0.0000 (nan)
-        >>> meters = MultiTaskAverageMeter(return_average=True)
+        >>> meters = MultiTaskAverageMeters(return_average=True)
         >>> meters.update({"loss": 0.6, "dataset1.a.auroc": 0.7, "dataset1.b.auroc": 0.8, "dataset2.auroc": 0.9})
         >>> print(f"{meters:.4f}")
         loss: 0.6000 (0.6000)
         dataset1.a.auroc: 0.7000 (0.7000)
         dataset1.b.auroc: 0.8000 (0.8000)
         dataset2.auroc: 0.9000 (0.9000)
         >>> meters.update({"loss": 0.9, "dataset1.a.auroc": 0.8, "dataset1.b.auroc": 0.9, "dataset2.auroc": 1.0})
@@ -201,15 +314,15 @@
             values: Dict of values to be added to the average.
             n: Number of values to be added.
 
         Raises:
             ValueError: If the value is not an instance of (int, float, Mapping).
 
         Examples:
-            >>> meters = MultiTaskAverageMeter()
+            >>> meters = MultiTaskAverageMeters()
             >>> meters.update({"loss": 0.6, "dataset1.cls.auroc": 0.7, "dataset1.reg.r2": 0.8, "dataset2.r2": 0.9})
             >>> meters.sum.dict()
             {'loss': 0.6, 'dataset1': {'cls': {'auroc': 0.7}, 'reg': {'r2': 0.8}}, 'dataset2': {'r2': 0.9}}
             >>> meters.count.dict()
             {'loss': 1, 'dataset1': {'cls': {'auroc': 1}, 'reg': {'r2': 1}}, 'dataset2': {'r2': 1}}
             >>> meters.update({"loss": {"value": 0.9, "n": 1}})
             >>> meters.sum.dict()
@@ -249,14 +362,14 @@
                         "This is likely due to nested dictionary in the values.\n"
                         "Nested dictionaries cannot be processed due to the method's design, which uses Mapping "
                         "to pass both value and count ('n'). Ensure your input is a flat dictionary or a single value."
                     ) from None
             else:
                 raise ValueError(f"Expected values to be int, float, or a flat dictionary, but got {type(value)}")
 
-    # eval hack, as the default_factory must not be set to make `NestedDict` happy
+    # evil hack, as the default_factory must not be set to make `NestedDict` happy
     # this have some side effects, it will break attribute style intermediate nested dict auto creation
     # but everything has a price
     def get(self, name: Any, default=None) -> Any:
         if not name.startswith("_") and not name.endswith("_"):
             return self.setdefault(name, AverageMeter())
         return super().get(name, default)
```

### Comparing `danling-0.3.5/danling/metrics/functional.py` & `danling-0.3.6/danling/metrics/functional.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 # pylint: disable=redefined-builtin
 from __future__ import annotations
 
 import torch
 from lazy_imports import try_import
 from torch import Tensor
```

### Comparing `danling-0.3.5/danling/metrics/metrics.py` & `danling-0.3.6/danling/metrics/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 # pylint: disable=redefined-builtin
 from __future__ import annotations
 
 from collections.abc import Mapping
 from math import nan
 from typing import Any, Callable, Iterable
 
@@ -9,16 +26,15 @@
 from chanfig import DefaultDict, FlatDict
 from torch import Tensor
 from torch import distributed as dist
 from torcheval.metrics import Metric
 
 from danling.tensors import NestedTensor
 
-from .multitask import MultiTaskDict
-from .utils import flist, get_world_size
+from .utils import MultiTaskDict, flist, get_world_size
 
 try:
     from typing import Self  # type: ignore[attr-defined]
 except ImportError:
     from typing_extensions import Self
```

### Comparing `danling-0.3.5/danling/modules/transformer/attention/multihead_attention.py` & `danling-0.3.6/danling/modules/transformer/attention/multihead_attention.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 import warnings
 from typing import Optional, Tuple
 
 import torch
 import torch.nn.functional as F
 from torch import Tensor, nn
```

### Comparing `danling-0.3.5/danling/modules/transformer/attention/simple_attention.py` & `danling-0.3.6/danling/modules/transformer/attention/simple_attention.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 import warnings
 from typing import Optional, Tuple
 
 import torch
 import torch.nn.functional as F
 from torch import Tensor, nn
```

### Comparing `danling-0.3.5/danling/modules/transformer/decoder.py` & `danling-0.3.6/danling/modules/transformer/decoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 from functools import partial
 from typing import Any, Dict, Optional, Tuple, Type
 
 import torch
 from torch import Tensor, nn
 from torch.utils.checkpoint import checkpoint
```

### Comparing `danling-0.3.5/danling/modules/transformer/encoder.py` & `danling-0.3.6/danling/modules/transformer/encoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 from functools import partial
 from typing import Any, Dict, Optional, Tuple, Type
 
 import torch
 from torch import Tensor, nn
 from torch.utils.checkpoint import checkpoint
```

### Comparing `danling-0.3.5/danling/modules/transformer/pos_embed/pos_embed.py` & `danling-0.3.6/danling/modules/transformer/pos_embed/pos_embed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 import math
 from typing import Optional
 
 import torch
 from torch import Tensor, nn
```

### Comparing `danling-0.3.5/danling/optim/lr_scheduler/lr_scheduler.py` & `danling-0.3.6/danling/optim/lr_scheduler/lr_scheduler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 from math import cos, pi
 from typing import List, Optional
 from warnings import warn
 
 from torch.optim import Optimizer, lr_scheduler
```

### Comparing `danling-0.3.5/danling/runner/README.md` & `danling-0.3.6/danling/runner/README.md`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/danling/runner/accelerate_runner.py` & `danling-0.3.6/danling/runner/accelerate_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 from __future__ import annotations
 
 import os
 import random
 from collections.abc import Callable, Mapping
 from contextlib import suppress
 from time import time
```

### Comparing `danling-0.3.5/danling/runner/base_runner.py` & `danling-0.3.6/danling/runner/base_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,48 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 # pylint: disable=redefined-builtin, keyword-arg-before-vararg
 from __future__ import annotations
 
 import logging
 import logging.config
 import os
 import random
 import shutil
 from collections.abc import Callable, Mapping, Sequence
 from math import ceil
 from sys import version_info
-from typing import Any, Dict
+from typing import TYPE_CHECKING, Any, Dict
 from uuid import UUID, uuid5
 from warnings import warn
 
 from chanfig import Config, FlatDict, NestedDict, Variable
 
-from danling.metrics import AverageMeter, Metrics, MultiTaskAverageMeter
+from danling.metrics import AverageMeter, AverageMeters
 from danling.typing import File, PathStr
 from danling.utils import catch, ensure_dir, load, save
 
+if TYPE_CHECKING:
+    from danling.metrics import Metrics
+
 try:
     from functools import cached_property
 except ImportError:
     from cached_property import cached_property  # type: ignore
 
 try:
     from numpy import random as np_random
@@ -131,17 +151,17 @@
         rank (int, property): Process index of all processes.
         local_rank (int, property): Process index of local processes.
         distributed (bool, property): If runner is running in distributed mode.
         is_main_process (bool, property): If current process is the main process of all processes.
         is_local_main_process (bool, property): If current process is the main process of local processes.
 
     Attributes: logging:
-        meters (MultiTaskAverageMeter): Average meters.
-            Initialised to `MultiTaskAverageMeter` by default.
-        metrics (Metrics): Metrics for evaluating.
+        meters (AverageMeters | MultiTaskAverageMeters): Average meters.
+            Initialised to `AverageMeters` by default.
+        metrics (Metrics | MultiTaskMetrics | None): Metrics for evaluating.
         logger:
         writer:
 
     See Also:
         [`RunnerState`][danling.runner.runner_state.RunnerState]: The runeer base that stores runtime information.
         [`BaseRunner`][danling.runner.BaseRunner]: The base runner class.
     """
@@ -161,30 +181,30 @@
 
     datasets: FlatDict
     datasamplers: FlatDict
     dataloaders: FlatDict
     split: str
 
     results: NestedDict
-    meters: MultiTaskAverageMeter
+    meters: AverageMeters
     metrics: Metrics | None = None
     logger: logging.Logger | None = None
     writer: Any | None = None
 
     def __init__(self, config: NestedDict) -> None:
         self.timestamp = get_time_str()
         if "datasets" not in self.__dict__:
             self.datasets = FlatDict()
         if "datasamplers" not in self.__dict__:
             self.datasamplers = FlatDict()
         if "dataloaders" not in self.__dict__:
             self.dataloaders = FlatDict()
         if "results" not in self.__dict__:
             self.results = NestedDict()
-        self.meters = MultiTaskAverageMeter()
+        self.meters = AverageMeters()
         self._mode = RunnerMode.train  # type: ignore[assignment]
         # must init state at last to avoid name conflicts
         self._state = RunnerState(config)
         self.inited = True
         self.init_distributed()
         if self.state.seed is not None:
             self.set_seed()
```

### Comparing `danling-0.3.5/danling/runner/state.py` & `danling-0.3.6/danling/runner/state.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 from __future__ import annotations
 
 from random import randint
 from typing import Optional
 from uuid import UUID, uuid5
 
 from chanfig import NestedDict
```

### Comparing `danling-0.3.5/danling/tensors/functional.py` & `danling-0.3.6/danling/tensors/functional.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 from collections.abc import Sequence
 from typing import Tuple
 
 import torch
 from torch import Tensor
```

### Comparing `danling-0.3.5/danling/tensors/nested_tensor.py` & `danling-0.3.6/danling/tensors/nested_tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 # pylint: disable=protected-access
 from __future__ import annotations
 
 from typing import Any, Callable, Iterable, Mapping, Sequence, SupportsFloat
 
 import torch
 from torch import Tensor
```

### Comparing `danling-0.3.5/danling/utils/decorators.py` & `danling-0.3.6/danling/utils/decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 from __future__ import annotations
 
 import traceback
 from functools import lru_cache, wraps
 from inspect import isfunction
 from os import makedirs
 from os.path import abspath
```

### Comparing `danling-0.3.5/danling/utils/io.py` & `danling-0.3.6/danling/utils/io.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 import json
 import os
 import pickle
 from typing import Any, Dict, List
 
 import yaml
 from chanfig import FlatDict
@@ -107,15 +124,15 @@
     if extension in YAML:
         with open(file) as fp:
             return yaml.load(fp, *args, **kwargs)  # type: ignore
     if extension in PICKLE:
         with open(file, "rb") as fp:
             return pickle.load(fp, *args, **kwargs)  # type: ignore
     if extension in PANDAS_SUPPORTED:
-        load_pandas(file, *args, **kwargs)
+        return load_pandas(file, *args, **kwargs)
     raise ValueError(f"Tying to load {file!r} with unsupported extension={extension!r}")
 
 
 def load_pandas(file: PathStr, *args: List[Any], **kwargs: Dict[str, Any]) -> Any:
     r"""
     Load any pandas data file with supported extensions.
     """
```

### Comparing `danling-0.3.5/danling.egg-info/PKG-INFO` & `danling-0.3.6/danling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danling
-Version: 0.3.5
+Version: 0.3.6
 Summary: Scaffold for experienced Machine Learning Researchers
 Author-email: Zhiyuan Chen <this@zyc.ai>
 Maintainer-email: Zhiyuan Chen <this@zyc.ai>
 License: Unlicense OR AGPL-3.0-or-later OR GPL-2.0-or-later OR BSD-4-Clause OR MIT OR Apache-2.0
         
 Project-URL: documentation, https://danling.org
 Project-URL: homepage, https://danling.org
@@ -22,14 +22,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+License-File: LICENSE.header
 Requires-Dist: cached-property; python_version < "3.8"
 Requires-Dist: chanfig>=0.0.96
 Requires-Dist: gitpython
 Requires-Dist: lazy-imports
 Requires-Dist: strenum; python_version < "3.11"
 Requires-Dist: tqdm
 Provides-Extra: jax
```

### Comparing `danling-0.3.5/danling.egg-info/SOURCES.txt` & `danling-0.3.6/danling.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 .gitignore
 .pre-commit-config.yaml
 LICENSE
+LICENSE.header
 README.md
 anaconda-project.yml
+licensing.sh
 pyproject.toml
 requirements.txt
 setup.py
 tox.ini
 .github/merge_rules.yaml
 .github/workflows/push.yaml
 LICENSES/LICENSE.AGPL
@@ -25,15 +27,14 @@
 danling.egg-info/dependency_links.txt
 danling.egg-info/requires.txt
 danling.egg-info/top_level.txt
 danling/metrics/__init__.py
 danling/metrics/average_meter.py
 danling/metrics/functional.py
 danling/metrics/metrics.py
-danling/metrics/multitask.py
 danling/metrics/utils.py
 danling/modules/__init__.py
 danling/modules/mlp/__init__.py
 danling/modules/mlp/dense.py
 danling/modules/mlp/mlp.py
 danling/modules/transformer/__init__.py
 danling/modules/transformer/decoder.py
```

### Comparing `danling-0.3.5/docs/mkdocs.yml` & `danling-0.3.6/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/docs/overrides/assets/fonts/CascadiaCodePL.woff2` & `danling-0.3.6/docs/overrides/assets/fonts/CascadiaCodePL.woff2`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/docs/overrides/assets/fonts/HYQiHei.ttf` & `danling-0.3.6/docs/overrides/assets/fonts/HYQiHei.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/docs/overrides/assets/fonts/HelveticaNowDisplay.otf` & `danling-0.3.6/docs/overrides/assets/fonts/HelveticaNowDisplay.otf`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/docs/overrides/assets/fonts/HelveticaWorld.ttf` & `danling-0.3.6/docs/overrides/assets/fonts/HelveticaWorld.ttf`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/docs/overrides/assets/images/favicon.ico` & `danling-0.3.6/docs/overrides/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/docs/overrides/assets/images/logo.png` & `danling-0.3.6/docs/overrides/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/docs/overrides/main.html` & `danling-0.3.6/docs/overrides/main.html`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/pyproject.toml` & `danling-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `danling-0.3.5/tests/metrics/test_metrics.py` & `danling-0.3.6/tests/metrics/test_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 import os
 import random
 
 import pytest
 import torch
 from torch import distributed as dist
 from torch.multiprocessing import spawn
```

### Comparing `danling-0.3.5/tests/optim/test_lr_scheduler.py` & `danling-0.3.6/tests/optim/test_lr_scheduler.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 import torch
 from torch import optim
 
 from danling.optim import LRScheduler
 
 # fmt: off
 LR_LINEAR_NUMERICAL_100 = [0.198, 0.392, 0.582, 0.768, 0.95, 0.9401, 0.9301, 0.9201, 0.9101, 0.9001, 0.8901, 0.8801, 0.8701, 0.8601, 0.8501, 0.8402, 0.8302, 0.8202, 0.8102, 0.8002, 0.7902, 0.7802, 0.7702, 0.7602, 0.7502, 0.7403, 0.7303, 0.7203, 0.7103, 0.7003, 0.6903, 0.6803, 0.6703, 0.6603, 0.6503, 0.6404, 0.6304, 0.6204, 0.6104, 0.6004, 0.5904, 0.5804, 0.5704, 0.5604, 0.5504, 0.5405, 0.5305, 0.5205, 0.5105, 0.5005, 0.4905, 0.4805, 0.4705, 0.4605, 0.4505, 0.4406, 0.4306, 0.4206, 0.4106, 0.4006, 0.3906, 0.3806, 0.3706, 0.3606, 0.3506, 0.3407, 0.3307, 0.3207, 0.3107, 0.3007, 0.2907, 0.2807, 0.2707, 0.2607, 0.2507, 0.2408, 0.2308, 0.2208, 0.2108, 0.2008, 0.1813, 0.1627, 0.1452, 0.1287, 0.1131, 0.0986, 0.0851, 0.0725, 0.061, 0.0505, 0.0409, 0.0324, 0.0248, 0.0183, 0.0127, 0.0082, 0.0046, 0.0021, 0.0005, 0.0]  # noqa
```

### Comparing `danling-0.3.5/tests/tensors/test_nested_tensor.py` & `danling-0.3.6/tests/tensors/test_nested_tensor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+# DanLing
+# Copyright (C) 2022-Present  DanLing
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the following licenses:
+# - The Unlicense
+# - GNU Affero General Public License v3.0 or later
+# - GNU General Public License v2.0 or later
+# - BSD 4-Clause "Original" or "Old" License
+# - MIT License
+# - Apache License 2.0
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
+# See the LICENSE file for more details.
+
 import random
 
 import pytest
 import torch
 
 from danling.tensors import NestedTensor
 from danling.tensors.nested_tensor import NestedTensorFuncWrapper
```

