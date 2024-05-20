# Comparing `tmp/jaxonmodels-0.1.2.tar.gz` & `tmp/jaxonmodels-0.1.3.tar.gz`

## Comparing `jaxonmodels-0.1.2.tar` & `jaxonmodels-0.1.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/pyrightconfig.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/examples/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/examples/examples.requirements.txt
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/examples/train_lstm.py
--rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/examples/train_resnet.py
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/examples/train_rnn.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/commons/__init__.py
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/commons/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/layers/__init__.py
--rw-r--r--   0        0        0    16144 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/layers/mha.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/layers/rope_embeddings.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/layers/selective_state_space_models.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/rnns/rnn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/ssm/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/ssm/mamba/__init__.py
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/ssm/mamba/mamba.py
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/ssm/mamba/model_args.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/transformers/__init__.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/transformers/kira/README.md
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/transformers/kira/__init__.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/transformers/kira/generate.py
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/transformers/kira/kira.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/transformers/kira/model_args.py
--rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/transformers/kira/train.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/transformers/llama/__init__.py
--rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/transformers/llama/llama2.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/transformers/llama/model_args.py
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/transformers/llama/tokenizer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/utils/__init__.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/utils/boto_client.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/vision/__init__.py
--rw-r--r--   0        0        0    11887 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/vision/resnet.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/jaxonmodels/vision/vgg.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/LICENSE
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/README.md
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 jaxonmodels-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/pyrightconfig.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/examples/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/examples/examples.requirements.txt
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/examples/train_lstm.py
+-rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/examples/train_resnet.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/examples/train_rnn.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/commons/__init__.py
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/commons/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/layers/__init__.py
+-rw-r--r--   0        0        0    16144 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/layers/mha.py
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/layers/rope_embeddings.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/layers/selective_state_space_models.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/rnns/rnn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/ssm/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/ssm/mamba/__init__.py
+-rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/ssm/mamba/mamba.py
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/ssm/mamba/model_args.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/transformers/__init__.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/transformers/kira/README.md
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/transformers/kira/__init__.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/transformers/kira/generate.py
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/transformers/kira/kira.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/transformers/kira/model_args.py
+-rw-r--r--   0        0        0     2345 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/transformers/kira/train.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/transformers/llama/__init__.py
+-rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/transformers/llama/llama3.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/transformers/llama/model_args.py
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/transformers/llama/tokenizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/utils/__init__.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/utils/boto_client.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/vision/__init__.py
+-rw-r--r--   0        0        0    11887 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/vision/resnet.py
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/jaxonmodels/vision/vgg.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/LICENSE
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/README.md
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 jaxonmodels-0.1.3/PKG-INFO
```

### Comparing `jaxonmodels-0.1.2/examples/train_resnet.py` & `jaxonmodels-0.1.3/examples/train_resnet.py`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/examples/train_rnn.py` & `jaxonmodels-0.1.3/examples/train_rnn.py`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/jaxonmodels/commons/utils.py` & `jaxonmodels-0.1.3/jaxonmodels/commons/utils.py`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/jaxonmodels/layers/mha.py` & `jaxonmodels-0.1.3/jaxonmodels/layers/mha.py`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/jaxonmodels/layers/rope_embeddings.py` & `jaxonmodels-0.1.3/jaxonmodels/layers/rope_embeddings.py`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/jaxonmodels/layers/selective_state_space_models.py` & `jaxonmodels-0.1.3/jaxonmodels/layers/selective_state_space_models.py`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/jaxonmodels/rnns/rnn.py` & `jaxonmodels-0.1.3/jaxonmodels/rnns/rnn.py`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/jaxonmodels/ssm/mamba/mamba.py` & `jaxonmodels-0.1.3/jaxonmodels/ssm/mamba/mamba.py`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/jaxonmodels/ssm/mamba/model_args.py` & `jaxonmodels-0.1.3/jaxonmodels/ssm/mamba/model_args.py`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/jaxonmodels/transformers/kira/README.md` & `jaxonmodels-0.1.3/jaxonmodels/transformers/kira/README.md`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/jaxonmodels/transformers/kira/generate.py` & `jaxonmodels-0.1.3/jaxonmodels/transformers/kira/generate.py`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/jaxonmodels/transformers/kira/kira.py` & `jaxonmodels-0.1.3/jaxonmodels/transformers/kira/kira.py`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/jaxonmodels/transformers/kira/train.py` & `jaxonmodels-0.1.3/jaxonmodels/transformers/kira/train.py`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/jaxonmodels/transformers/llama/llama2.py` & `jaxonmodels-0.1.3/jaxonmodels/transformers/llama/llama3.py`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/jaxonmodels/transformers/llama/model_args.py` & `jaxonmodels-0.1.3/jaxonmodels/transformers/llama/model_args.py`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/jaxonmodels/transformers/llama/tokenizer.py` & `jaxonmodels-0.1.3/jaxonmodels/transformers/llama/tokenizer.py`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/jaxonmodels/utils/boto_client.py` & `jaxonmodels-0.1.3/jaxonmodels/utils/boto_client.py`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/jaxonmodels/vision/resnet.py` & `jaxonmodels-0.1.3/jaxonmodels/vision/resnet.py`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/jaxonmodels/vision/vgg.py` & `jaxonmodels-0.1.3/jaxonmodels/vision/vgg.py`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/.gitignore` & `jaxonmodels-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/LICENSE` & `jaxonmodels-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxonmodels-0.1.2/pyproject.toml` & `jaxonmodels-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jaxonmodels"
-version = "0.1.2"
+version = "0.1.3"
 description = "JAX models for deep learning"
 readme = "README.md"
 requires-python = "~=3.10"
 license = { file = "LICENSE" }
 authors = [{ name = "Artur A. Galstyan", email = "mail@arturgalstyan.dev" }]
 dependencies = [
     "jax",
```

### Comparing `jaxonmodels-0.1.2/PKG-INFO` & `jaxonmodels-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jaxonmodels
-Version: 0.1.2
+Version: 0.1.3
 Summary: JAX models for deep learning
 Author-email: "Artur A. Galstyan" <mail@arturgalstyan.dev>
 License: MIT License
         
         Copyright (c) 2024 Artur A. Galstyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

