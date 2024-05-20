# Comparing `tmp/llm2vec-0.1.6.tar.gz` & `tmp/llm2vec-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm2vec-0.1.6.tar", last modified: Wed May  8 16:29:59 2024, max compression
+gzip compressed data, was "llm2vec-0.1.7.tar", last modified: Mon May 20 19:52:11 2024, max compression
```

## Comparing `llm2vec-0.1.6.tar` & `llm2vec-0.1.7.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-08 16:29:59.721398 llm2vec-0.1.6/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1067 2024-04-08 21:09:47.000000 llm2vec-0.1.6/LICENSE
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    12628 2024-05-08 16:29:59.721661 llm2vec-0.1.6/PKG-INFO
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    12178 2024-05-08 16:25:06.000000 llm2vec-0.1.6/README.md
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-08 16:29:59.703822 llm2vec-0.1.6/llm2vec/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       29 2024-04-16 16:56:44.000000 llm2vec-0.1.6/llm2vec/__init__.py
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-08 16:29:59.711660 llm2vec-0.1.6/llm2vec/dataset/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6148 2024-05-08 16:25:06.000000 llm2vec-0.1.6/llm2vec/dataset/E5Data.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       26 2024-04-30 22:31:54.000000 llm2vec-0.1.6/llm2vec/dataset/__init__.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1123 2024-04-30 22:31:54.000000 llm2vec-0.1.6/llm2vec/dataset/dataset.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      723 2024-04-30 22:31:54.000000 llm2vec-0.1.6/llm2vec/dataset/utils.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     2417 2024-04-30 22:31:54.000000 llm2vec-0.1.6/llm2vec/experiment_utils.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    16774 2024-05-08 16:25:06.000000 llm2vec-0.1.6/llm2vec/llm2vec.py
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-08 16:29:59.715280 llm2vec-0.1.6/llm2vec/loss/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1478 2024-04-30 22:31:54.000000 llm2vec-0.1.6/llm2vec/loss/HardNegativeNLLLoss.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       52 2024-04-30 22:31:54.000000 llm2vec-0.1.6/llm2vec/loss/__init__.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     3080 2024-04-30 22:31:54.000000 llm2vec-0.1.6/llm2vec/loss/loss_utils.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      289 2024-04-30 22:31:54.000000 llm2vec-0.1.6/llm2vec/loss/utils.py
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-08 16:29:59.720316 llm2vec-0.1.6/llm2vec/models/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      130 2024-04-16 16:56:44.000000 llm2vec-0.1.6/llm2vec/models/__init__.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7620 2024-04-16 16:56:44.000000 llm2vec-0.1.6/llm2vec/models/attn_mask_utils.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7760 2024-04-30 22:31:54.000000 llm2vec-0.1.6/llm2vec/models/bidirectional_llama.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    10368 2024-04-17 17:32:47.000000 llm2vec-0.1.6/llm2vec/models/bidirectional_mistral.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       22 2024-05-08 16:29:50.000000 llm2vec-0.1.6/llm2vec/version.py
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-08 16:29:59.708107 llm2vec-0.1.6/llm2vec.egg-info/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    12628 2024-05-08 16:29:59.000000 llm2vec-0.1.6/llm2vec.egg-info/PKG-INFO
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      661 2024-05-08 16:29:59.000000 llm2vec-0.1.6/llm2vec.egg-info/SOURCES.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-05-08 16:29:59.000000 llm2vec-0.1.6/llm2vec.egg-info/dependency_links.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-16 16:57:16.000000 llm2vec-0.1.6/llm2vec.egg-info/not-zip-safe
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       74 2024-05-08 16:29:59.000000 llm2vec-0.1.6/llm2vec.egg-info/requires.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        8 2024-05-08 16:29:59.000000 llm2vec-0.1.6/llm2vec.egg-info/top_level.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       79 2024-05-08 16:29:59.722725 llm2vec-0.1.6/setup.cfg
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1089 2024-04-17 17:32:47.000000 llm2vec-0.1.6/setup.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-20 19:52:11.350339 llm2vec-0.1.7/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1067 2024-04-08 21:09:47.000000 llm2vec-0.1.7/LICENSE
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    14785 2024-05-20 19:52:11.350859 llm2vec-0.1.7/PKG-INFO
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    14335 2024-05-20 19:39:21.000000 llm2vec-0.1.7/README.md
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-20 19:52:11.328401 llm2vec-0.1.7/llm2vec/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       29 2024-04-16 16:56:44.000000 llm2vec-0.1.7/llm2vec/__init__.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-20 19:52:11.339303 llm2vec-0.1.7/llm2vec/dataset/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6148 2024-05-08 16:25:06.000000 llm2vec-0.1.7/llm2vec/dataset/E5Data.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1368 2024-05-20 19:39:21.000000 llm2vec-0.1.7/llm2vec/dataset/Wiki1M.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       53 2024-05-20 19:39:21.000000 llm2vec-0.1.7/llm2vec/dataset/__init__.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1137 2024-05-20 19:39:21.000000 llm2vec-0.1.7/llm2vec/dataset/dataset.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      778 2024-05-20 19:39:21.000000 llm2vec-0.1.7/llm2vec/dataset/utils.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     2417 2024-04-30 22:31:54.000000 llm2vec-0.1.7/llm2vec/experiment_utils.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    16796 2024-05-20 19:39:21.000000 llm2vec-0.1.7/llm2vec/llm2vec.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-20 19:52:11.343390 llm2vec-0.1.7/llm2vec/loss/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1478 2024-04-30 22:31:54.000000 llm2vec-0.1.7/llm2vec/loss/HardNegativeNLLLoss.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       52 2024-04-30 22:31:54.000000 llm2vec-0.1.7/llm2vec/loss/__init__.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     3080 2024-04-30 22:31:54.000000 llm2vec-0.1.7/llm2vec/loss/loss_utils.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      289 2024-04-30 22:31:54.000000 llm2vec-0.1.7/llm2vec/loss/utils.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-20 19:52:11.348430 llm2vec-0.1.7/llm2vec/models/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      130 2024-04-16 16:56:44.000000 llm2vec-0.1.7/llm2vec/models/__init__.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7620 2024-04-16 16:56:44.000000 llm2vec-0.1.7/llm2vec/models/attn_mask_utils.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7774 2024-05-20 19:39:21.000000 llm2vec-0.1.7/llm2vec/models/bidirectional_llama.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    10368 2024-04-17 17:32:47.000000 llm2vec-0.1.7/llm2vec/models/bidirectional_mistral.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       22 2024-05-20 19:51:17.000000 llm2vec-0.1.7/llm2vec/version.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-20 19:52:11.333543 llm2vec-0.1.7/llm2vec.egg-info/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    14785 2024-05-20 19:52:11.000000 llm2vec-0.1.7/llm2vec.egg-info/PKG-INFO
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      687 2024-05-20 19:52:11.000000 llm2vec-0.1.7/llm2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-05-20 19:52:11.000000 llm2vec-0.1.7/llm2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-16 16:57:16.000000 llm2vec-0.1.7/llm2vec.egg-info/not-zip-safe
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       74 2024-05-20 19:52:11.000000 llm2vec-0.1.7/llm2vec.egg-info/requires.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        8 2024-05-20 19:52:11.000000 llm2vec-0.1.7/llm2vec.egg-info/top_level.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       79 2024-05-20 19:52:11.352866 llm2vec-0.1.7/setup.cfg
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1089 2024-04-17 17:32:47.000000 llm2vec-0.1.7/setup.py
```

### Comparing `llm2vec-0.1.6/LICENSE` & `llm2vec-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.6/PKG-INFO` & `llm2vec-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,16 @@
-Metadata-Version: 2.1
-Name: llm2vec
-Version: 0.1.6
-Summary: The official llm2vec library
-Home-page: https://github.com/McGill-NLP/llm2vec
-Author: McGill NLP
-Author-email: parishad.behnamghader@mila.quebec
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # *LLM2Vec: Large Language Models Are Secretly Powerful Text Encoders* 
 
+
 [![arxiv](https://img.shields.io/badge/arXiv-2404.05961-b31b1b.svg)](https://arxiv.org/abs/2404.05961)
 [![PyPi](https://img.shields.io/pypi/v/llm2vec)](https://pypi.org/project/llm2vec/)
 [![HF Link](https://img.shields.io/badge/HF%20Models-LLM2Vec-FFD21E.svg)](https://huggingface.co/collections/McGill-NLP/llm2vec-660e14f536b3c8d10b3f1c34)
-
-
-
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/McGill-NLP/llm2vec/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/badge/llm2vec)](https://pepy.tech/project/llm2vec)
 
 LLM2Vec is a simple recipe to convert decoder-only LLMs into text encoders. It consists of 3 simple steps: 1) enabling bidirectional attention, 2) training with masked next token prediction, and 3) unsupervised contrastive learning. The model can be further fine-tuned to achieve state-of-the-art performance.
 
 <p align="center">
   <img src="https://github.com/McGill-NLP/llm2vec/assets/12207571/48efd48a-431b-4625-8e0f-248a442e3839" width="75%" alt="LLM2Vec_figure1"/>
 </p>
 
@@ -49,37 +35,37 @@
 
 ## Getting Started
 LLM2Vec class is a wrapper on top of HuggingFace models to support enabling bidirectionality in decoder-only LLMs, sequence encoding and pooling operations. The steps below showcase an example on how to use the library.
 
 ### Preparing the model
 Initializing LLM2Vec model using pretrained LLMs is straightforward. The `from_pretrained` method of LLM2Vec takes a base model identifier/path and an optional PEFT model identifier/path. All HuggingFace model loading arguments can be passed to `from_pretrained` method. By default, the models are loaded with bidirectional connections enabled. This can be turned off by passing `enable_bidirectional=False` to the `from_pretrained` method.
 
-Here, we first initialize the Mistral MNTP base model and load the unsupervised-trained LoRA weights (trained with SimCSE objective and wiki corpus).
+Here, we first initialize the Llama-3 MNTP base model and load the unsupervised-trained LoRA weights (trained with SimCSE objective and wiki corpus).
 
 ```python
 import torch
 from llm2vec import LLM2Vec
 
 l2v = LLM2Vec.from_pretrained(
-    "McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp",
-    peft_model_name_or_path="McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp-unsup-simcse",
+    "McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp",
+    peft_model_name_or_path="McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-unsup-simcse",
     device_map="cuda" if torch.cuda.is_available() else "cpu",
     torch_dtype=torch.bfloat16,
 )
 ```
 
 We can also load the model with supervised-trained LoRA weights (trained with contrastive learning and public E5 data) by changing the `peft_model_name_or_path`.
 
 ```python
 import torch
 from llm2vec import LLM2Vec
 
 l2v = LLM2Vec.from_pretrained(
-    "McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp",
-    peft_model_name_or_path="McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp-supervised",
+    "McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp",
+    peft_model_name_or_path="McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-supervised",
     device_map="cuda" if torch.cuda.is_available() else "cpu",
     torch_dtype=torch.bfloat16,
 )
 ```
 
 By default the LLM2Vec model uses the `mean` pooling strategy. You can change the pooling strategy by passing the `pooling_mode` argument to the `from_pretrained` method. Similarly, you can change the maximum sequence length by passing the `max_length` argument (default is 512).
 
@@ -107,16 +93,16 @@
 # Compute cosine similarity
 q_reps_norm = torch.nn.functional.normalize(q_reps, p=2, dim=1)
 d_reps_norm = torch.nn.functional.normalize(d_reps, p=2, dim=1)
 cos_sim = torch.mm(q_reps_norm, d_reps_norm.transpose(0, 1))
 
 print(cos_sim)
 """
-tensor([[0.5485, 0.0551],
-        [0.0565, 0.5425]])
+tensor([[0.6470, 0.1619],
+        [0.0786, 0.5844]])
 """
 ```
 
 More examples of classification, clustering, sentence similarity etc are present in [examples](examples) directory.
 
 ## Model List
 
@@ -128,68 +114,112 @@
 
 \* State-of-the-art on MTEB among models trained on public data
 
 \*\* Unsupervised state-of-the-art on MTEB
 
 ## Training 
 ### MNTP training
-To train the model with Masked Next Token Prediction (MNTP), you can use the `experiments/run_mntp.py` script. It is adapted from HuggingFace Masked Language Modeling (MLM) [script](https://github.com/huggingface/transformers/blob/51bcadc10a569847b93a30dbe3a077037ae63bad/examples/pytorch/language-modeling/run_mlm.py). To train the Mistral-7B model with MNTP, run the following command:
+To train the model with Masked Next Token Prediction (MNTP), you can use the `experiments/run_mntp.py` script. It is adapted from HuggingFace Masked Language Modeling (MLM) [script](https://github.com/huggingface/transformers/blob/51bcadc10a569847b93a30dbe3a077037ae63bad/examples/pytorch/language-modeling/run_mlm.py). To train the Meta-Llama-3-8B model with MNTP, run the following command:
 
 ```bash
-python experiments/run_mntp.py train_configs/mntp/Mistral.json
+python experiments/run_mntp.py train_configs/mntp/MetaLlama3.json
 ```
 
-The Mistral training configuration [file](train_configs/mntp/Mistral.json) contains all the training hyperparameters and configurations used in our paper. 
+The Meta-Llama-3-8B training configuration [file](train_configs/mntp/MetaLlama3.json) contains all the training hyperparameters and configurations used in our paper. 
 ```json
 {
-    "model_name_or_path": "mistralai/Mistral-7B-Instruct-v0.2",
+    "model_name_or_path": "meta-llama/Meta-Llama-3-8B-Instruct",
     "dataset_name": "wikitext",
     "dataset_config_name": "wikitext-103-raw-v1",
     "mask_token_type": "blank",
-    "data_collator_type": "all_mask",
-    "mlm_probability": 0.8,
+    "data_collator_type": "default",
+    "mlm_probability": 0.2,
     "lora_r": 16,
     "gradient_checkpointing": true,
     "torch_dtype": "bfloat16",
     "attn_implementation": "flash_attention_2"
     // ....
 }
 ```
 
-Similar configurations are also available for[Meta-Llama-3-8B](train_configs/mntp/MetaLlama3.json), [Llama-2-7B](train_configs/mntp/Llama2.json), and [Sheared-Llama-1.3B](train_configs/mntp/Sheared-Llama.json) models.
+Similar configurations are also available for[Mistral-7B](train_configs/mntp/Mistral.json), [Llama-2-7B](train_configs/mntp/Llama2.json), and [Sheared-Llama-1.3B](train_configs/mntp/Sheared-Llama.json) models.
 
 ### Unsupervised contrastive training (SimCSE)
-COMING SOON
+For SimCSE training, we replicated the training procedure from [SimCSE](https://arxiv.org/abs/2104.08821) paper. For training, we use the dataset 1 million sentences from English Wikipedia released by the authors. It can be downloaded using the following command:
+
+```bash
+wget https://huggingface.co/datasets/princeton-nlp/datasets-for-simcse/resolve/main/wiki1m_for_simcse.txt
+```
+
+To use the training script with pre-set configurations, the downloaded file should be placed in the `cache` directory. The directory layout should be as follows:
+
+```
+cache
+└── wiki1m_for_simcse.txt
+```
+If the dataset is placed in a different directory, please change the dataset_file_path in the training configuration accordingly.
+
+To train the Meta-Llama-3-8B model with SimCSE, run the following command:
+
+```bash
+python experiments/run_simcse.py train_configs/simcse/MetaLlama3.json
+```
+
+The Meta-Llama-3-8B training configuration [file](train_configs/simcse/MetaLlama3.json) contains all the training hyperparameters and configurations used in our paper. 
+```json
+{
+    "model_name_or_path": "meta-llama/Meta-Llama-3-8B-Instruct",
+    "peft_model_name_or_path": "McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp",
+    "simcse_dropout": 0.3,
+    "bidirectional": true,
+    "pooling_mode": "mean",
+    "dataset_name": "Wiki1M",
+    "dataset_file_path": "cache/wiki1m_for_simcse.txt",
+    "learning_rate": 3e-5,
+    "loss_scale": 20,
+    "per_device_train_batch_size": 128,
+    "max_seq_length": 128,
+    "stop_after_n_steps": 1000,
+    "lora_r": 16,
+    "gradient_checkpointing": true,
+    "torch_dtype": "bfloat16",
+    "attn_implementation": "flash_attention_2",
+    // ....
+}
+```
+
+Similar configurations are also available for [Mistral](train_configs/simcse/Mistral.json), [Llama-2-7B](train_configs/simcse/Llama2.json), and [Sheared-Llama-1.3B](train_configs/simcse/Sheared-Llama.json) models.
 
 ### Supervised contrastive training
 For supervised contrastive training, we use the public portion of dataset used in [Improving Text Embeddings with Large Language Models](https://arxiv.org/abs/2401.00368), curated by authors of [Repetition Improves Language Model Embeddings](https://arxiv.org/abs/2402.15449). The dataset can be downloaded from the [GitHub page of Echo embeddings repository](https://github.com/jakespringer/echo-embeddings#training). To use the training script, the downloaded dataset should be placed in the `cache` directory. The directory layout should be as follows:
 
 ```
 cache
+|── wiki1m_for_simcse.txt
 └── echo-data
     ├── allnli_split1.jsonl
     ├── allnli_split2.jsonl
     ├── allnli.jsonl
     ├── dureader.jsonl
     ...
 ```
 If the dataset is placed in a different directory, please change the `dataset_file_path` in the training configuration accordingly. 
 
-To train the Mistral-7B model with supervised contrastive learning, run the following command:
+To train the Meta-Llama-3-8B model with supervised contrastive learning, run the following command:
 
 ```bash
-torchrun --nproc_per_node=8 experiments/run_supervised.py train_configs/supervised/Mistral.json
+torchrun --nproc_per_node=8 experiments/run_supervised.py train_configs/supervised/MetaLlama3.json
 ```
 The number of GPUs can be changed by modifying the `--nproc_per_node` argument.
 
-The Mistral training configuration [file](train_configs/supervised/Mistral.json) contains all the training hyperparameters and configurations used in our paper. 
+The Meta-Llama-3-8B training configuration [file](train_configs/supervised/MetaLlama3.json) contains all the training hyperparameters and configurations used in our paper. 
 ```json
 {
-    "model_name_or_path": "mistralai/Mistral-7B-Instruct-v0.2",
-    "peft_model_name_or_path": "McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp",
+    "model_name_or_path": "meta-llama/Meta-Llama-3-8B-Instruct",
+    "peft_model_name_or_path": "McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp",
     "bidirectional": true,
     "pooling_mode": "mean",
     "dataset_name": "E5",
     "dataset_file_path": "cache/echo-data",
     "learning_rate": 2e-4,
     "num_train_epochs": 3,
     "warmup_steps": 300,
@@ -197,15 +227,15 @@
     "lora_r": 16,
     "gradient_checkpointing": true,
     "torch_dtype": "bfloat16",
     "attn_implementation": "flash_attention_2"
     // ....
 }
 ```
-Similar configurations are also available for [Meta-Llama-3-8B](train_configs/supervised/MetaLlama3.json), [Llama-2-7B](train_configs/supervised/Llama2.json), and [Sheared-Llama-1.3B](train_configs/supervised/Sheared-Llama.json) models.
+Similar configurations are also available for [Mistral](train_configs/supervised/Mistral.json), [Llama-2-7B](train_configs/supervised/Llama2.json), and [Sheared-Llama-1.3B](train_configs/supervised/Sheared-Llama.json) models.
 
 
 ### Word-level tasks training
 
 To tune the model for word-level tasks, we define a classifier on top of the models, and only train the classifier weights. The code is adapted from HuggingFace token classification [example](https://huggingface.co/docs/transformers/en/tasks/token_classification). To train and test the classifier for Llama-2-7B MNTP model on `pos_tags` task, run the following command:
 ```bash
 python experiments/run_word_task.py train_configs/word-task/Llama2-bi-mntp.json
```

### Comparing `llm2vec-0.1.6/README.md` & `llm2vec-0.1.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,31 @@
+Metadata-Version: 2.1
+Name: llm2vec
+Version: 0.1.7
+Summary: The official llm2vec library
+Home-page: https://github.com/McGill-NLP/llm2vec
+Author: McGill NLP
+Author-email: parishad.behnamghader@mila.quebec
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 # *LLM2Vec: Large Language Models Are Secretly Powerful Text Encoders* 
 
+
 [![arxiv](https://img.shields.io/badge/arXiv-2404.05961-b31b1b.svg)](https://arxiv.org/abs/2404.05961)
 [![PyPi](https://img.shields.io/pypi/v/llm2vec)](https://pypi.org/project/llm2vec/)
 [![HF Link](https://img.shields.io/badge/HF%20Models-LLM2Vec-FFD21E.svg)](https://huggingface.co/collections/McGill-NLP/llm2vec-660e14f536b3c8d10b3f1c34)
-
-
-
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/McGill-NLP/llm2vec/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/badge/llm2vec)](https://pepy.tech/project/llm2vec)
 
 LLM2Vec is a simple recipe to convert decoder-only LLMs into text encoders. It consists of 3 simple steps: 1) enabling bidirectional attention, 2) training with masked next token prediction, and 3) unsupervised contrastive learning. The model can be further fine-tuned to achieve state-of-the-art performance.
 
 <p align="center">
   <img src="https://github.com/McGill-NLP/llm2vec/assets/12207571/48efd48a-431b-4625-8e0f-248a442e3839" width="75%" alt="LLM2Vec_figure1"/>
 </p>
 
@@ -34,37 +50,37 @@
 
 ## Getting Started
 LLM2Vec class is a wrapper on top of HuggingFace models to support enabling bidirectionality in decoder-only LLMs, sequence encoding and pooling operations. The steps below showcase an example on how to use the library.
 
 ### Preparing the model
 Initializing LLM2Vec model using pretrained LLMs is straightforward. The `from_pretrained` method of LLM2Vec takes a base model identifier/path and an optional PEFT model identifier/path. All HuggingFace model loading arguments can be passed to `from_pretrained` method. By default, the models are loaded with bidirectional connections enabled. This can be turned off by passing `enable_bidirectional=False` to the `from_pretrained` method.
 
-Here, we first initialize the Mistral MNTP base model and load the unsupervised-trained LoRA weights (trained with SimCSE objective and wiki corpus).
+Here, we first initialize the Llama-3 MNTP base model and load the unsupervised-trained LoRA weights (trained with SimCSE objective and wiki corpus).
 
 ```python
 import torch
 from llm2vec import LLM2Vec
 
 l2v = LLM2Vec.from_pretrained(
-    "McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp",
-    peft_model_name_or_path="McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp-unsup-simcse",
+    "McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp",
+    peft_model_name_or_path="McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-unsup-simcse",
     device_map="cuda" if torch.cuda.is_available() else "cpu",
     torch_dtype=torch.bfloat16,
 )
 ```
 
 We can also load the model with supervised-trained LoRA weights (trained with contrastive learning and public E5 data) by changing the `peft_model_name_or_path`.
 
 ```python
 import torch
 from llm2vec import LLM2Vec
 
 l2v = LLM2Vec.from_pretrained(
-    "McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp",
-    peft_model_name_or_path="McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp-supervised",
+    "McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp",
+    peft_model_name_or_path="McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-supervised",
     device_map="cuda" if torch.cuda.is_available() else "cpu",
     torch_dtype=torch.bfloat16,
 )
 ```
 
 By default the LLM2Vec model uses the `mean` pooling strategy. You can change the pooling strategy by passing the `pooling_mode` argument to the `from_pretrained` method. Similarly, you can change the maximum sequence length by passing the `max_length` argument (default is 512).
 
@@ -92,16 +108,16 @@
 # Compute cosine similarity
 q_reps_norm = torch.nn.functional.normalize(q_reps, p=2, dim=1)
 d_reps_norm = torch.nn.functional.normalize(d_reps, p=2, dim=1)
 cos_sim = torch.mm(q_reps_norm, d_reps_norm.transpose(0, 1))
 
 print(cos_sim)
 """
-tensor([[0.5485, 0.0551],
-        [0.0565, 0.5425]])
+tensor([[0.6470, 0.1619],
+        [0.0786, 0.5844]])
 """
 ```
 
 More examples of classification, clustering, sentence similarity etc are present in [examples](examples) directory.
 
 ## Model List
 
@@ -113,68 +129,112 @@
 
 \* State-of-the-art on MTEB among models trained on public data
 
 \*\* Unsupervised state-of-the-art on MTEB
 
 ## Training 
 ### MNTP training
-To train the model with Masked Next Token Prediction (MNTP), you can use the `experiments/run_mntp.py` script. It is adapted from HuggingFace Masked Language Modeling (MLM) [script](https://github.com/huggingface/transformers/blob/51bcadc10a569847b93a30dbe3a077037ae63bad/examples/pytorch/language-modeling/run_mlm.py). To train the Mistral-7B model with MNTP, run the following command:
+To train the model with Masked Next Token Prediction (MNTP), you can use the `experiments/run_mntp.py` script. It is adapted from HuggingFace Masked Language Modeling (MLM) [script](https://github.com/huggingface/transformers/blob/51bcadc10a569847b93a30dbe3a077037ae63bad/examples/pytorch/language-modeling/run_mlm.py). To train the Meta-Llama-3-8B model with MNTP, run the following command:
 
 ```bash
-python experiments/run_mntp.py train_configs/mntp/Mistral.json
+python experiments/run_mntp.py train_configs/mntp/MetaLlama3.json
 ```
 
-The Mistral training configuration [file](train_configs/mntp/Mistral.json) contains all the training hyperparameters and configurations used in our paper. 
+The Meta-Llama-3-8B training configuration [file](train_configs/mntp/MetaLlama3.json) contains all the training hyperparameters and configurations used in our paper. 
 ```json
 {
-    "model_name_or_path": "mistralai/Mistral-7B-Instruct-v0.2",
+    "model_name_or_path": "meta-llama/Meta-Llama-3-8B-Instruct",
     "dataset_name": "wikitext",
     "dataset_config_name": "wikitext-103-raw-v1",
     "mask_token_type": "blank",
-    "data_collator_type": "all_mask",
-    "mlm_probability": 0.8,
+    "data_collator_type": "default",
+    "mlm_probability": 0.2,
     "lora_r": 16,
     "gradient_checkpointing": true,
     "torch_dtype": "bfloat16",
     "attn_implementation": "flash_attention_2"
     // ....
 }
 ```
 
-Similar configurations are also available for[Meta-Llama-3-8B](train_configs/mntp/MetaLlama3.json), [Llama-2-7B](train_configs/mntp/Llama2.json), and [Sheared-Llama-1.3B](train_configs/mntp/Sheared-Llama.json) models.
+Similar configurations are also available for[Mistral-7B](train_configs/mntp/Mistral.json), [Llama-2-7B](train_configs/mntp/Llama2.json), and [Sheared-Llama-1.3B](train_configs/mntp/Sheared-Llama.json) models.
 
 ### Unsupervised contrastive training (SimCSE)
-COMING SOON
+For SimCSE training, we replicated the training procedure from [SimCSE](https://arxiv.org/abs/2104.08821) paper. For training, we use the dataset 1 million sentences from English Wikipedia released by the authors. It can be downloaded using the following command:
+
+```bash
+wget https://huggingface.co/datasets/princeton-nlp/datasets-for-simcse/resolve/main/wiki1m_for_simcse.txt
+```
+
+To use the training script with pre-set configurations, the downloaded file should be placed in the `cache` directory. The directory layout should be as follows:
+
+```
+cache
+└── wiki1m_for_simcse.txt
+```
+If the dataset is placed in a different directory, please change the dataset_file_path in the training configuration accordingly.
+
+To train the Meta-Llama-3-8B model with SimCSE, run the following command:
+
+```bash
+python experiments/run_simcse.py train_configs/simcse/MetaLlama3.json
+```
+
+The Meta-Llama-3-8B training configuration [file](train_configs/simcse/MetaLlama3.json) contains all the training hyperparameters and configurations used in our paper. 
+```json
+{
+    "model_name_or_path": "meta-llama/Meta-Llama-3-8B-Instruct",
+    "peft_model_name_or_path": "McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp",
+    "simcse_dropout": 0.3,
+    "bidirectional": true,
+    "pooling_mode": "mean",
+    "dataset_name": "Wiki1M",
+    "dataset_file_path": "cache/wiki1m_for_simcse.txt",
+    "learning_rate": 3e-5,
+    "loss_scale": 20,
+    "per_device_train_batch_size": 128,
+    "max_seq_length": 128,
+    "stop_after_n_steps": 1000,
+    "lora_r": 16,
+    "gradient_checkpointing": true,
+    "torch_dtype": "bfloat16",
+    "attn_implementation": "flash_attention_2",
+    // ....
+}
+```
+
+Similar configurations are also available for [Mistral](train_configs/simcse/Mistral.json), [Llama-2-7B](train_configs/simcse/Llama2.json), and [Sheared-Llama-1.3B](train_configs/simcse/Sheared-Llama.json) models.
 
 ### Supervised contrastive training
 For supervised contrastive training, we use the public portion of dataset used in [Improving Text Embeddings with Large Language Models](https://arxiv.org/abs/2401.00368), curated by authors of [Repetition Improves Language Model Embeddings](https://arxiv.org/abs/2402.15449). The dataset can be downloaded from the [GitHub page of Echo embeddings repository](https://github.com/jakespringer/echo-embeddings#training). To use the training script, the downloaded dataset should be placed in the `cache` directory. The directory layout should be as follows:
 
 ```
 cache
+|── wiki1m_for_simcse.txt
 └── echo-data
     ├── allnli_split1.jsonl
     ├── allnli_split2.jsonl
     ├── allnli.jsonl
     ├── dureader.jsonl
     ...
 ```
 If the dataset is placed in a different directory, please change the `dataset_file_path` in the training configuration accordingly. 
 
-To train the Mistral-7B model with supervised contrastive learning, run the following command:
+To train the Meta-Llama-3-8B model with supervised contrastive learning, run the following command:
 
 ```bash
-torchrun --nproc_per_node=8 experiments/run_supervised.py train_configs/supervised/Mistral.json
+torchrun --nproc_per_node=8 experiments/run_supervised.py train_configs/supervised/MetaLlama3.json
 ```
 The number of GPUs can be changed by modifying the `--nproc_per_node` argument.
 
-The Mistral training configuration [file](train_configs/supervised/Mistral.json) contains all the training hyperparameters and configurations used in our paper. 
+The Meta-Llama-3-8B training configuration [file](train_configs/supervised/MetaLlama3.json) contains all the training hyperparameters and configurations used in our paper. 
 ```json
 {
-    "model_name_or_path": "mistralai/Mistral-7B-Instruct-v0.2",
-    "peft_model_name_or_path": "McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp",
+    "model_name_or_path": "meta-llama/Meta-Llama-3-8B-Instruct",
+    "peft_model_name_or_path": "McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp",
     "bidirectional": true,
     "pooling_mode": "mean",
     "dataset_name": "E5",
     "dataset_file_path": "cache/echo-data",
     "learning_rate": 2e-4,
     "num_train_epochs": 3,
     "warmup_steps": 300,
@@ -182,15 +242,15 @@
     "lora_r": 16,
     "gradient_checkpointing": true,
     "torch_dtype": "bfloat16",
     "attn_implementation": "flash_attention_2"
     // ....
 }
 ```
-Similar configurations are also available for [Meta-Llama-3-8B](train_configs/supervised/MetaLlama3.json), [Llama-2-7B](train_configs/supervised/Llama2.json), and [Sheared-Llama-1.3B](train_configs/supervised/Sheared-Llama.json) models.
+Similar configurations are also available for [Mistral](train_configs/supervised/Mistral.json), [Llama-2-7B](train_configs/supervised/Llama2.json), and [Sheared-Llama-1.3B](train_configs/supervised/Sheared-Llama.json) models.
 
 
 ### Word-level tasks training
 
 To tune the model for word-level tasks, we define a classifier on top of the models, and only train the classifier weights. The code is adapted from HuggingFace token classification [example](https://huggingface.co/docs/transformers/en/tasks/token_classification). To train and test the classifier for Llama-2-7B MNTP model on `pos_tags` task, run the following command:
 ```bash
 python experiments/run_word_task.py train_configs/word-task/Llama2-bi-mntp.json
```

### Comparing `llm2vec-0.1.6/llm2vec/dataset/E5Data.py` & `llm2vec-0.1.7/llm2vec/dataset/E5Data.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.6/llm2vec/dataset/dataset.py` & `llm2vec-0.1.7/llm2vec/dataset/dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import torch
 
 @dataclass
 class DataSample:
     id_: int
     query: str
     positive: str
-    negative: str
-    task_name: str
+    negative: str = None
+    task_name: str = None
 
 class TrainSample:
     """
     Structure for one input example with texts, the label and a unique id
     """
     def __init__(self, guid: str = '', texts: List[str] = None,  label: Union[int, float] = 0):
         """
```

### Comparing `llm2vec-0.1.6/llm2vec/experiment_utils.py` & `llm2vec-0.1.7/llm2vec/experiment_utils.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.6/llm2vec/llm2vec.py` & `llm2vec-0.1.7/llm2vec/llm2vec.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,15 @@
         return text
 
     def tokenize(self, texts):
         texts_2 = []
         original_texts = []
         for text in texts:
             t = text.split("!@#$%^&*()")
-            texts_2.append(t[1])
+            texts_2.append(t[1] if len(t) > 1 else "")
             original_texts.append("".join(t))
 
         original = self.tokenizer(
             original_texts,
             return_tensors="pt",
             padding=True,
             truncation=True,
```

### Comparing `llm2vec-0.1.6/llm2vec/loss/HardNegativeNLLLoss.py` & `llm2vec-0.1.7/llm2vec/loss/HardNegativeNLLLoss.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.6/llm2vec/loss/loss_utils.py` & `llm2vec-0.1.7/llm2vec/loss/loss_utils.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.6/llm2vec/models/attn_mask_utils.py` & `llm2vec-0.1.7/llm2vec/models/attn_mask_utils.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.6/llm2vec/models/bidirectional_llama.py` & `llm2vec-0.1.7/llm2vec/models/bidirectional_llama.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,21 +109,21 @@
 
     def _update_causal_mask(self, attention_mask, input_tensor, cache_position, past_seen_tokens=None):
         if self.config._attn_implementation == "flash_attention_2":
             if attention_mask is not None and 0.0 in attention_mask:
                 return attention_mask
             return None
 
-        if is_transformers_attn_greater_or_equal_4_40() and self.config._attn_implementation == "sdpa":
-            # For SDPA, when possible, we will rely on its `is_causal` argument instead of its `attn_mask` argument,
-            # in order to dispatch on Flash Attention 2.
-            if AttentionMaskConverter._ignore_causal_mask_sdpa(
-                attention_mask, inputs_embeds=input_tensor, past_key_values_length=past_seen_tokens
-            ):
-                return None
+        # if is_transformers_attn_greater_or_equal_4_40() and self.config._attn_implementation == "sdpa":
+        #     # For SDPA, when possible, we will rely on its `is_causal` argument instead of its `attn_mask` argument,
+        #     # in order to dispatch on Flash Attention 2.
+        #     if AttentionMaskConverter._ignore_causal_mask_sdpa(
+        #         attention_mask, inputs_embeds=input_tensor, past_key_values_length=past_seen_tokens
+        #     ):
+        #         return None
 
         dtype, device = input_tensor.dtype, input_tensor.device
         min_dtype = torch.finfo(dtype).min
         sequence_length = input_tensor.shape[1]
         if hasattr(
             getattr(self.layers[0], "self_attn", {}), "past_key_value"
         ):  # static cache
```

### Comparing `llm2vec-0.1.6/llm2vec/models/bidirectional_mistral.py` & `llm2vec-0.1.7/llm2vec/models/bidirectional_mistral.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.6/llm2vec.egg-info/PKG-INFO` & `llm2vec-0.1.7/llm2vec.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: llm2vec
-Version: 0.1.6
+Version: 0.1.7
 Summary: The official llm2vec library
 Home-page: https://github.com/McGill-NLP/llm2vec
 Author: McGill NLP
 Author-email: parishad.behnamghader@mila.quebec
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+
 # *LLM2Vec: Large Language Models Are Secretly Powerful Text Encoders* 
 
+
 [![arxiv](https://img.shields.io/badge/arXiv-2404.05961-b31b1b.svg)](https://arxiv.org/abs/2404.05961)
 [![PyPi](https://img.shields.io/pypi/v/llm2vec)](https://pypi.org/project/llm2vec/)
 [![HF Link](https://img.shields.io/badge/HF%20Models-LLM2Vec-FFD21E.svg)](https://huggingface.co/collections/McGill-NLP/llm2vec-660e14f536b3c8d10b3f1c34)
-
-
-
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/McGill-NLP/llm2vec/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/badge/llm2vec)](https://pepy.tech/project/llm2vec)
 
 LLM2Vec is a simple recipe to convert decoder-only LLMs into text encoders. It consists of 3 simple steps: 1) enabling bidirectional attention, 2) training with masked next token prediction, and 3) unsupervised contrastive learning. The model can be further fine-tuned to achieve state-of-the-art performance.
 
 <p align="center">
   <img src="https://github.com/McGill-NLP/llm2vec/assets/12207571/48efd48a-431b-4625-8e0f-248a442e3839" width="75%" alt="LLM2Vec_figure1"/>
 </p>
 
@@ -49,37 +50,37 @@
 
 ## Getting Started
 LLM2Vec class is a wrapper on top of HuggingFace models to support enabling bidirectionality in decoder-only LLMs, sequence encoding and pooling operations. The steps below showcase an example on how to use the library.
 
 ### Preparing the model
 Initializing LLM2Vec model using pretrained LLMs is straightforward. The `from_pretrained` method of LLM2Vec takes a base model identifier/path and an optional PEFT model identifier/path. All HuggingFace model loading arguments can be passed to `from_pretrained` method. By default, the models are loaded with bidirectional connections enabled. This can be turned off by passing `enable_bidirectional=False` to the `from_pretrained` method.
 
-Here, we first initialize the Mistral MNTP base model and load the unsupervised-trained LoRA weights (trained with SimCSE objective and wiki corpus).
+Here, we first initialize the Llama-3 MNTP base model and load the unsupervised-trained LoRA weights (trained with SimCSE objective and wiki corpus).
 
 ```python
 import torch
 from llm2vec import LLM2Vec
 
 l2v = LLM2Vec.from_pretrained(
-    "McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp",
-    peft_model_name_or_path="McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp-unsup-simcse",
+    "McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp",
+    peft_model_name_or_path="McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-unsup-simcse",
     device_map="cuda" if torch.cuda.is_available() else "cpu",
     torch_dtype=torch.bfloat16,
 )
 ```
 
 We can also load the model with supervised-trained LoRA weights (trained with contrastive learning and public E5 data) by changing the `peft_model_name_or_path`.
 
 ```python
 import torch
 from llm2vec import LLM2Vec
 
 l2v = LLM2Vec.from_pretrained(
-    "McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp",
-    peft_model_name_or_path="McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp-supervised",
+    "McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp",
+    peft_model_name_or_path="McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp-supervised",
     device_map="cuda" if torch.cuda.is_available() else "cpu",
     torch_dtype=torch.bfloat16,
 )
 ```
 
 By default the LLM2Vec model uses the `mean` pooling strategy. You can change the pooling strategy by passing the `pooling_mode` argument to the `from_pretrained` method. Similarly, you can change the maximum sequence length by passing the `max_length` argument (default is 512).
 
@@ -107,16 +108,16 @@
 # Compute cosine similarity
 q_reps_norm = torch.nn.functional.normalize(q_reps, p=2, dim=1)
 d_reps_norm = torch.nn.functional.normalize(d_reps, p=2, dim=1)
 cos_sim = torch.mm(q_reps_norm, d_reps_norm.transpose(0, 1))
 
 print(cos_sim)
 """
-tensor([[0.5485, 0.0551],
-        [0.0565, 0.5425]])
+tensor([[0.6470, 0.1619],
+        [0.0786, 0.5844]])
 """
 ```
 
 More examples of classification, clustering, sentence similarity etc are present in [examples](examples) directory.
 
 ## Model List
 
@@ -128,68 +129,112 @@
 
 \* State-of-the-art on MTEB among models trained on public data
 
 \*\* Unsupervised state-of-the-art on MTEB
 
 ## Training 
 ### MNTP training
-To train the model with Masked Next Token Prediction (MNTP), you can use the `experiments/run_mntp.py` script. It is adapted from HuggingFace Masked Language Modeling (MLM) [script](https://github.com/huggingface/transformers/blob/51bcadc10a569847b93a30dbe3a077037ae63bad/examples/pytorch/language-modeling/run_mlm.py). To train the Mistral-7B model with MNTP, run the following command:
+To train the model with Masked Next Token Prediction (MNTP), you can use the `experiments/run_mntp.py` script. It is adapted from HuggingFace Masked Language Modeling (MLM) [script](https://github.com/huggingface/transformers/blob/51bcadc10a569847b93a30dbe3a077037ae63bad/examples/pytorch/language-modeling/run_mlm.py). To train the Meta-Llama-3-8B model with MNTP, run the following command:
 
 ```bash
-python experiments/run_mntp.py train_configs/mntp/Mistral.json
+python experiments/run_mntp.py train_configs/mntp/MetaLlama3.json
 ```
 
-The Mistral training configuration [file](train_configs/mntp/Mistral.json) contains all the training hyperparameters and configurations used in our paper. 
+The Meta-Llama-3-8B training configuration [file](train_configs/mntp/MetaLlama3.json) contains all the training hyperparameters and configurations used in our paper. 
 ```json
 {
-    "model_name_or_path": "mistralai/Mistral-7B-Instruct-v0.2",
+    "model_name_or_path": "meta-llama/Meta-Llama-3-8B-Instruct",
     "dataset_name": "wikitext",
     "dataset_config_name": "wikitext-103-raw-v1",
     "mask_token_type": "blank",
-    "data_collator_type": "all_mask",
-    "mlm_probability": 0.8,
+    "data_collator_type": "default",
+    "mlm_probability": 0.2,
     "lora_r": 16,
     "gradient_checkpointing": true,
     "torch_dtype": "bfloat16",
     "attn_implementation": "flash_attention_2"
     // ....
 }
 ```
 
-Similar configurations are also available for[Meta-Llama-3-8B](train_configs/mntp/MetaLlama3.json), [Llama-2-7B](train_configs/mntp/Llama2.json), and [Sheared-Llama-1.3B](train_configs/mntp/Sheared-Llama.json) models.
+Similar configurations are also available for[Mistral-7B](train_configs/mntp/Mistral.json), [Llama-2-7B](train_configs/mntp/Llama2.json), and [Sheared-Llama-1.3B](train_configs/mntp/Sheared-Llama.json) models.
 
 ### Unsupervised contrastive training (SimCSE)
-COMING SOON
+For SimCSE training, we replicated the training procedure from [SimCSE](https://arxiv.org/abs/2104.08821) paper. For training, we use the dataset 1 million sentences from English Wikipedia released by the authors. It can be downloaded using the following command:
+
+```bash
+wget https://huggingface.co/datasets/princeton-nlp/datasets-for-simcse/resolve/main/wiki1m_for_simcse.txt
+```
+
+To use the training script with pre-set configurations, the downloaded file should be placed in the `cache` directory. The directory layout should be as follows:
+
+```
+cache
+└── wiki1m_for_simcse.txt
+```
+If the dataset is placed in a different directory, please change the dataset_file_path in the training configuration accordingly.
+
+To train the Meta-Llama-3-8B model with SimCSE, run the following command:
+
+```bash
+python experiments/run_simcse.py train_configs/simcse/MetaLlama3.json
+```
+
+The Meta-Llama-3-8B training configuration [file](train_configs/simcse/MetaLlama3.json) contains all the training hyperparameters and configurations used in our paper. 
+```json
+{
+    "model_name_or_path": "meta-llama/Meta-Llama-3-8B-Instruct",
+    "peft_model_name_or_path": "McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp",
+    "simcse_dropout": 0.3,
+    "bidirectional": true,
+    "pooling_mode": "mean",
+    "dataset_name": "Wiki1M",
+    "dataset_file_path": "cache/wiki1m_for_simcse.txt",
+    "learning_rate": 3e-5,
+    "loss_scale": 20,
+    "per_device_train_batch_size": 128,
+    "max_seq_length": 128,
+    "stop_after_n_steps": 1000,
+    "lora_r": 16,
+    "gradient_checkpointing": true,
+    "torch_dtype": "bfloat16",
+    "attn_implementation": "flash_attention_2",
+    // ....
+}
+```
+
+Similar configurations are also available for [Mistral](train_configs/simcse/Mistral.json), [Llama-2-7B](train_configs/simcse/Llama2.json), and [Sheared-Llama-1.3B](train_configs/simcse/Sheared-Llama.json) models.
 
 ### Supervised contrastive training
 For supervised contrastive training, we use the public portion of dataset used in [Improving Text Embeddings with Large Language Models](https://arxiv.org/abs/2401.00368), curated by authors of [Repetition Improves Language Model Embeddings](https://arxiv.org/abs/2402.15449). The dataset can be downloaded from the [GitHub page of Echo embeddings repository](https://github.com/jakespringer/echo-embeddings#training). To use the training script, the downloaded dataset should be placed in the `cache` directory. The directory layout should be as follows:
 
 ```
 cache
+|── wiki1m_for_simcse.txt
 └── echo-data
     ├── allnli_split1.jsonl
     ├── allnli_split2.jsonl
     ├── allnli.jsonl
     ├── dureader.jsonl
     ...
 ```
 If the dataset is placed in a different directory, please change the `dataset_file_path` in the training configuration accordingly. 
 
-To train the Mistral-7B model with supervised contrastive learning, run the following command:
+To train the Meta-Llama-3-8B model with supervised contrastive learning, run the following command:
 
 ```bash
-torchrun --nproc_per_node=8 experiments/run_supervised.py train_configs/supervised/Mistral.json
+torchrun --nproc_per_node=8 experiments/run_supervised.py train_configs/supervised/MetaLlama3.json
 ```
 The number of GPUs can be changed by modifying the `--nproc_per_node` argument.
 
-The Mistral training configuration [file](train_configs/supervised/Mistral.json) contains all the training hyperparameters and configurations used in our paper. 
+The Meta-Llama-3-8B training configuration [file](train_configs/supervised/MetaLlama3.json) contains all the training hyperparameters and configurations used in our paper. 
 ```json
 {
-    "model_name_or_path": "mistralai/Mistral-7B-Instruct-v0.2",
-    "peft_model_name_or_path": "McGill-NLP/LLM2Vec-Mistral-7B-Instruct-v2-mntp",
+    "model_name_or_path": "meta-llama/Meta-Llama-3-8B-Instruct",
+    "peft_model_name_or_path": "McGill-NLP/LLM2Vec-Meta-Llama-3-8B-Instruct-mntp",
     "bidirectional": true,
     "pooling_mode": "mean",
     "dataset_name": "E5",
     "dataset_file_path": "cache/echo-data",
     "learning_rate": 2e-4,
     "num_train_epochs": 3,
     "warmup_steps": 300,
@@ -197,15 +242,15 @@
     "lora_r": 16,
     "gradient_checkpointing": true,
     "torch_dtype": "bfloat16",
     "attn_implementation": "flash_attention_2"
     // ....
 }
 ```
-Similar configurations are also available for [Meta-Llama-3-8B](train_configs/supervised/MetaLlama3.json), [Llama-2-7B](train_configs/supervised/Llama2.json), and [Sheared-Llama-1.3B](train_configs/supervised/Sheared-Llama.json) models.
+Similar configurations are also available for [Mistral](train_configs/supervised/Mistral.json), [Llama-2-7B](train_configs/supervised/Llama2.json), and [Sheared-Llama-1.3B](train_configs/supervised/Sheared-Llama.json) models.
 
 
 ### Word-level tasks training
 
 To tune the model for word-level tasks, we define a classifier on top of the models, and only train the classifier weights. The code is adapted from HuggingFace token classification [example](https://huggingface.co/docs/transformers/en/tasks/token_classification). To train and test the classifier for Llama-2-7B MNTP model on `pos_tags` task, run the following command:
 ```bash
 python experiments/run_word_task.py train_configs/word-task/Llama2-bi-mntp.json
```

### Comparing `llm2vec-0.1.6/setup.py` & `llm2vec-0.1.7/setup.py`

 * *Files identical despite different names*

