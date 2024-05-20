# Comparing `tmp/rnaformer-1.3.1.tar.gz` & `tmp/rnaformer-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnaformer-1.3.1.tar", last modified: Sat May 18 10:55:18 2024, max compression
+gzip compressed data, was "rnaformer-1.3.2.tar", last modified: Mon May 20 13:20:31 2024, max compression
```

## Comparing `rnaformer-1.3.1.tar` & `rnaformer-1.3.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:55:18.523375 rnaformer-1.3.1/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)    11347 2024-04-10 11:44:16.000000 rnaformer-1.3.1/LICENSE
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      124 2024-04-17 13:09:53.000000 rnaformer-1.3.1/MANIFEST.in
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     5692 2024-05-18 10:55:18.523375 rnaformer-1.3.1/PKG-INFO
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4381 2024-04-22 14:37:55.000000 rnaformer-1.3.1/README.md
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:55:18.519375 rnaformer-1.3.1/RNAformer/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-17 13:15:35.000000 rnaformer-1.3.1/RNAformer/__init__.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:55:18.519375 rnaformer-1.3.1/RNAformer/model/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3594 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/model/RNAformer.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2020 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/model/RNAformer_block.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      755 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/model/RNAformer_stack.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/model/__init__.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:55:18.523375 rnaformer-1.3.1/RNAformer/module/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/module/__init__.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)    13307 2024-04-22 14:11:45.000000 rnaformer-1.3.1/RNAformer/module/axial_attention.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      940 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/module/axial_dropout.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3788 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/module/embedding.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3371 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/module/feed_forward.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:55:18.523375 rnaformer-1.3.1/RNAformer/pl_module/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/pl_module/__init__.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)    11243 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/pl_module/datamodule_rna.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     9104 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/pl_module/rna_folding_trainer.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:55:18.523375 rnaformer-1.3.1/RNAformer/utils/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      164 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/utils/__init__.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4062 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/utils/configuration.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:55:18.523375 rnaformer-1.3.1/RNAformer/utils/data/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/utils/data/__init__.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     5800 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/utils/data/rna.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     6566 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/utils/eval_predictions.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      890 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/utils/folder_manager.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3656 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/utils/group_parameters.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:55:18.523375 rnaformer-1.3.1/RNAformer/utils/handler/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/utils/handler/__init__.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2145 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/utils/handler/base_handler.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3478 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/utils/handler/checkpoint.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     1480 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/utils/handler/folder.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2461 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/utils/instantiate.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3780 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/utils/logger.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:55:18.523375 rnaformer-1.3.1/RNAformer/utils/optim/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/utils/optim/__init__.py
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     1067 2024-04-10 11:44:16.000000 rnaformer-1.3.1/RNAformer/utils/optim/lr_schedule.py
-drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-18 10:55:18.523375 rnaformer-1.3.1/RNAformer.egg-info/
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     5692 2024-05-18 10:55:18.000000 rnaformer-1.3.1/RNAformer.egg-info/PKG-INFO
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2129 2024-05-18 10:55:18.000000 rnaformer-1.3.1/RNAformer.egg-info/SOURCES.txt
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)        1 2024-05-18 10:55:18.000000 rnaformer-1.3.1/RNAformer.egg-info/dependency_links.txt
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      273 2024-05-18 10:55:18.000000 rnaformer-1.3.1/RNAformer.egg-info/requires.txt
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)       10 2024-05-18 10:55:18.000000 rnaformer-1.3.1/RNAformer.egg-info/top_level.txt
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)     1184 2024-05-18 10:55:14.000000 rnaformer-1.3.1/pyproject.toml
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)       38 2024-05-18 10:55:18.523375 rnaformer-1.3.1/setup.cfg
--rw-r--r--   0 koeksalr (19891) bioinf    (1065)      286 2024-04-22 14:37:48.000000 rnaformer-1.3.1/setup.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-20 13:20:31.577628 rnaformer-1.3.2/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)    11347 2024-04-10 11:44:16.000000 rnaformer-1.3.2/LICENSE
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      124 2024-04-17 13:09:53.000000 rnaformer-1.3.2/MANIFEST.in
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     5676 2024-05-20 13:20:31.577628 rnaformer-1.3.2/PKG-INFO
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4365 2024-05-20 13:03:33.000000 rnaformer-1.3.2/README.md
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-20 13:20:31.573629 rnaformer-1.3.2/RNAformer/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-17 13:15:35.000000 rnaformer-1.3.2/RNAformer/__init__.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-20 13:20:31.573629 rnaformer-1.3.2/RNAformer/model/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3594 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/model/RNAformer.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2020 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/model/RNAformer_block.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      755 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/model/RNAformer_stack.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/model/__init__.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-20 13:20:31.573629 rnaformer-1.3.2/RNAformer/module/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/module/__init__.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)    13307 2024-04-22 14:11:45.000000 rnaformer-1.3.2/RNAformer/module/axial_attention.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      940 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/module/axial_dropout.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3788 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/module/embedding.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3371 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/module/feed_forward.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-20 13:20:31.573629 rnaformer-1.3.2/RNAformer/pl_module/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/pl_module/__init__.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)    11243 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/pl_module/datamodule_rna.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     9104 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/pl_module/rna_folding_trainer.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-20 13:20:31.573629 rnaformer-1.3.2/RNAformer/utils/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      164 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/utils/__init__.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     4062 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/utils/configuration.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-20 13:20:31.577628 rnaformer-1.3.2/RNAformer/utils/data/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/utils/data/__init__.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     5800 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/utils/data/rna.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     6566 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/utils/eval_predictions.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      890 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/utils/folder_manager.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3656 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/utils/group_parameters.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-20 13:20:31.577628 rnaformer-1.3.2/RNAformer/utils/handler/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/utils/handler/__init__.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2145 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/utils/handler/base_handler.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3478 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/utils/handler/checkpoint.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     1480 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/utils/handler/folder.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2461 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/utils/instantiate.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     3780 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/utils/logger.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-20 13:20:31.577628 rnaformer-1.3.2/RNAformer/utils/optim/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        0 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/utils/optim/__init__.py
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     1067 2024-04-10 11:44:16.000000 rnaformer-1.3.2/RNAformer/utils/optim/lr_schedule.py
+drwxr-xr-x   0 koeksalr (19891) bioinf    (1065)        0 2024-05-20 13:20:31.577628 rnaformer-1.3.2/RNAformer.egg-info/
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     5676 2024-05-20 13:20:31.000000 rnaformer-1.3.2/RNAformer.egg-info/PKG-INFO
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     2129 2024-05-20 13:20:31.000000 rnaformer-1.3.2/RNAformer.egg-info/SOURCES.txt
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)        1 2024-05-20 13:20:31.000000 rnaformer-1.3.2/RNAformer.egg-info/dependency_links.txt
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      273 2024-05-20 13:20:31.000000 rnaformer-1.3.2/RNAformer.egg-info/requires.txt
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)       10 2024-05-20 13:20:31.000000 rnaformer-1.3.2/RNAformer.egg-info/top_level.txt
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)     1184 2024-05-20 13:18:48.000000 rnaformer-1.3.2/pyproject.toml
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)       38 2024-05-20 13:20:31.577628 rnaformer-1.3.2/setup.cfg
+-rw-r--r--   0 koeksalr (19891) bioinf    (1065)      854 2024-05-20 13:18:46.000000 rnaformer-1.3.2/setup.py
```

### Comparing `rnaformer-1.3.1/LICENSE` & `rnaformer-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/PKG-INFO` & `rnaformer-1.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RNAformer
-Version: 1.3.1
+Version: 1.3.2
 Summary: RNAformer: a simple single-sequence-based deep learning model for RNA secondary structure prediction.
 Author: Frederic Runge, Rolf Backofen, Frank Hutter
 Author-email: "Joerg K.H. Franke" <frankej@cs.uni-freiburg.de>, Ryan Koeksal <koeksalr@informatik.uni-freiburg.de>
 Maintainer-email: Ryan Koeksal <koeksalr@informatik.uni-freiburg.de>, "Joerg K.H. Franke" <frankej@cs.uni-freiburg.de>
 Project-URL: Homepage, https://github.com/automl/RNAformer
 Project-URL: Issues, https://github.com/automl/RNAformer/issues
 Classifier: Programming Language :: Python :: 3
@@ -101,28 +101,28 @@
 
 ## Model Checkpoints
 
 Please find here the state dictionaries and configs for the models used in the paper: 
 
 RNAformer 32M from the biophysical model experiment:
 ```
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_state_dict_biophysical.pth
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_config_biophysical.yml
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_state_dict_biophysical.pth
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_config_biophysical.yml
 ```
 
 RNAformer 32M from the bprna model experiment:
 ```
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_state_dict_bprna.pth
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_config_bprna.yml
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_state_dict_bprna.pth
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_config_bprna.yml
 ```
 
 RNAformer 32M from the intra family finetuning experiment:
 ```
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_state_dict_intra_family_finetuned.pth
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_config_intra_family_finetuned.yml
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_state_dict_intra_family_finetuned.pth
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_config_intra_family_finetuned.yml
 ```
 
 RNAformer 32M from the inter family finetuning experiment:
 ```
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_state_dict_inter_family_finetuned.pth
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_config_inter_family_finetuned.yml
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_state_dict_inter_family_finetuned.pth
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_config_inter_family_finetuned.yml
 ```
```

### Comparing `rnaformer-1.3.1/README.md` & `rnaformer-1.3.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -65,28 +65,28 @@
 
 ## Model Checkpoints
 
 Please find here the state dictionaries and configs for the models used in the paper: 
 
 RNAformer 32M from the biophysical model experiment:
 ```
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_state_dict_biophysical.pth
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_config_biophysical.yml
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_state_dict_biophysical.pth
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_config_biophysical.yml
 ```
 
 RNAformer 32M from the bprna model experiment:
 ```
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_state_dict_bprna.pth
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_config_bprna.yml
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_state_dict_bprna.pth
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_config_bprna.yml
 ```
 
 RNAformer 32M from the intra family finetuning experiment:
 ```
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_state_dict_intra_family_finetuned.pth
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_config_intra_family_finetuned.yml
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_state_dict_intra_family_finetuned.pth
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_config_intra_family_finetuned.yml
 ```
 
 RNAformer 32M from the inter family finetuning experiment:
 ```
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_state_dict_inter_family_finetuned.pth
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_config_inter_family_finetuned.yml
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_state_dict_inter_family_finetuned.pth
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_config_inter_family_finetuned.yml
 ```
```

### Comparing `rnaformer-1.3.1/RNAformer/model/RNAformer.py` & `rnaformer-1.3.2/RNAformer/model/RNAformer.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/model/RNAformer_block.py` & `rnaformer-1.3.2/RNAformer/model/RNAformer_block.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/model/RNAformer_stack.py` & `rnaformer-1.3.2/RNAformer/model/RNAformer_stack.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/module/axial_attention.py` & `rnaformer-1.3.2/RNAformer/module/axial_attention.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/module/axial_dropout.py` & `rnaformer-1.3.2/RNAformer/module/axial_dropout.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/module/embedding.py` & `rnaformer-1.3.2/RNAformer/module/embedding.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/module/feed_forward.py` & `rnaformer-1.3.2/RNAformer/module/feed_forward.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/pl_module/datamodule_rna.py` & `rnaformer-1.3.2/RNAformer/pl_module/datamodule_rna.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/pl_module/rna_folding_trainer.py` & `rnaformer-1.3.2/RNAformer/pl_module/rna_folding_trainer.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/utils/configuration.py` & `rnaformer-1.3.2/RNAformer/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/utils/data/rna.py` & `rnaformer-1.3.2/RNAformer/utils/data/rna.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/utils/eval_predictions.py` & `rnaformer-1.3.2/RNAformer/utils/eval_predictions.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/utils/folder_manager.py` & `rnaformer-1.3.2/RNAformer/utils/folder_manager.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/utils/group_parameters.py` & `rnaformer-1.3.2/RNAformer/utils/group_parameters.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/utils/handler/base_handler.py` & `rnaformer-1.3.2/RNAformer/utils/handler/base_handler.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/utils/handler/checkpoint.py` & `rnaformer-1.3.2/RNAformer/utils/handler/checkpoint.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/utils/handler/folder.py` & `rnaformer-1.3.2/RNAformer/utils/handler/folder.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/utils/instantiate.py` & `rnaformer-1.3.2/RNAformer/utils/instantiate.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/utils/logger.py` & `rnaformer-1.3.2/RNAformer/utils/logger.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer/utils/optim/lr_schedule.py` & `rnaformer-1.3.2/RNAformer/utils/optim/lr_schedule.py`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/RNAformer.egg-info/PKG-INFO` & `rnaformer-1.3.2/RNAformer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RNAformer
-Version: 1.3.1
+Version: 1.3.2
 Summary: RNAformer: a simple single-sequence-based deep learning model for RNA secondary structure prediction.
 Author: Frederic Runge, Rolf Backofen, Frank Hutter
 Author-email: "Joerg K.H. Franke" <frankej@cs.uni-freiburg.de>, Ryan Koeksal <koeksalr@informatik.uni-freiburg.de>
 Maintainer-email: Ryan Koeksal <koeksalr@informatik.uni-freiburg.de>, "Joerg K.H. Franke" <frankej@cs.uni-freiburg.de>
 Project-URL: Homepage, https://github.com/automl/RNAformer
 Project-URL: Issues, https://github.com/automl/RNAformer/issues
 Classifier: Programming Language :: Python :: 3
@@ -101,28 +101,28 @@
 
 ## Model Checkpoints
 
 Please find here the state dictionaries and configs for the models used in the paper: 
 
 RNAformer 32M from the biophysical model experiment:
 ```
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_state_dict_biophysical.pth
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_config_biophysical.yml
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_state_dict_biophysical.pth
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_config_biophysical.yml
 ```
 
 RNAformer 32M from the bprna model experiment:
 ```
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_state_dict_bprna.pth
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_config_bprna.yml
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_state_dict_bprna.pth
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_config_bprna.yml
 ```
 
 RNAformer 32M from the intra family finetuning experiment:
 ```
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_state_dict_intra_family_finetuned.pth
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_config_intra_family_finetuned.yml
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_state_dict_intra_family_finetuned.pth
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_config_intra_family_finetuned.yml
 ```
 
 RNAformer 32M from the inter family finetuning experiment:
 ```
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_state_dict_inter_family_finetuned.pth
-https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/datasets/RNAformer_32M_config_inter_family_finetuned.yml
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_state_dict_inter_family_finetuned.pth
+https://ml.informatik.uni-freiburg.de/research-artifacts/RNAformer/models/RNAformer_32M_config_inter_family_finetuned.yml
 ```
```

### Comparing `rnaformer-1.3.1/RNAformer.egg-info/SOURCES.txt` & `rnaformer-1.3.2/RNAformer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rnaformer-1.3.1/pyproject.toml` & `rnaformer-1.3.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "RNAformer"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
   { name="Joerg K.H. Franke", email="frankej@cs.uni-freiburg.de" },
   { name="Frederic Runge"},
   { name="Ryan Koeksal", email="koeksalr@informatik.uni-freiburg.de" },
   { name="Rolf Backofen"},
   { name="Frank Hutter"},
 ]
```

