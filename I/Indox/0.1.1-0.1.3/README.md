# Comparing `tmp/Indox-0.1.1.tar.gz` & `tmp/indox-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Indox-0.1.1.tar", last modified: Wed May  8 13:36:50 2024, max compression
+gzip compressed data, was "indox-0.1.3.tar", last modified: Mon May 20 10:10:44 2024, max compression
```

## Comparing `Indox-0.1.1.tar` & `indox-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,57 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 13:36:50.042721 Indox-0.1.1/
-drwxrwxrwx   0        0        0        0 2024-05-08 13:36:49.925356 Indox-0.1.1/Indox/
--rw-rw-rw-   0        0        0     3548 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/Embedding.py
--rw-rw-rw-   0        0        0     2453 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/Graph.py
--rw-rw-rw-   0        0        0    12884 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/Indox.py
--rw-rw-rw-   0        0        0     5666 2024-05-08 13:25:13.000000 Indox-0.1.1/Indox/QAModels.py
--rw-rw-rw-   0        0        0    12574 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/Splitter.py
--rw-rw-rw-   0        0        0     2959 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/Summary.py
--rw-rw-rw-   0        0        0       66 2024-05-08 13:01:56.000000 Indox-0.1.1/Indox/__init__.py
--rw-rw-rw-   0        0        0      593 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/clean.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:36:50.022400 Indox-0.1.1/Indox/cluster/
--rw-rw-rw-   0        0        0     6348 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/cluster/Clustering.py
--rw-rw-rw-   0        0        0     4685 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/cluster/EmbedClusterSummarize.py
--rw-rw-rw-   0        0        0        0 2024-05-08 13:08:42.000000 Indox-0.1.1/Indox/cluster/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:36:50.037432 Indox-0.1.1/Indox/metrics/
--rw-rw-rw-   0        0        0        0 2024-05-08 13:08:54.000000 Indox-0.1.1/Indox/metrics/__init__.py
--rw-rw-rw-   0        0        0     4114 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/metrics/metrics.py
--rw-rw-rw-   0        0        0    10055 2024-05-08 13:08:27.000000 Indox-0.1.1/Indox/metrics/unieval.py
--rw-rw-rw-   0        0        0     8837 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/utils.py
--rw-rw-rw-   0        0        0     5358 2024-05-08 10:23:44.000000 Indox-0.1.1/Indox/vectorstore.py
-drwxrwxrwx   0        0        0        0 2024-05-08 13:36:49.952967 Indox-0.1.1/Indox.egg-info/
--rw-rw-rw-   0        0        0      685 2024-05-08 13:36:49.000000 Indox-0.1.1/Indox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2024-05-08 13:36:49.000000 Indox-0.1.1/Indox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 13:36:49.000000 Indox-0.1.1/Indox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      440 2024-05-08 13:36:49.000000 Indox-0.1.1/Indox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-08 13:36:49.000000 Indox-0.1.1/Indox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2024-05-08 10:23:44.000000 Indox-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      685 2024-05-08 13:36:50.037432 Indox-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     8204 2024-05-08 10:23:44.000000 Indox-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-08 13:36:50.043746 Indox-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1023 2024-05-08 13:36:43.000000 Indox-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.672964 indox-0.1.3/
+drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.643278 indox-0.1.3/Indox/
+drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.656961 indox-0.1.3/Indox/DataLoaderSplitter/
+drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.660961 indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/
+-rw-rw-rw-   0        0        0     6348 2024-05-11 13:44:58.000000 indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/Clustering.py
+-rw-rw-rw-   0        0        0     2074 2024-05-13 06:41:26.000000 indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/Embed.py
+-rw-rw-rw-   0        0        0     4781 2024-05-13 08:12:00.000000 indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/EmbedClusterSummarize.py
+-rw-rw-rw-   0        0        0     2856 2024-05-13 06:27:35.000000 indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/Summary.py
+-rw-rw-rw-   0        0        0       35 2024-05-14 14:02:48.000000 indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/__init__.py
+-rw-rw-rw-   0        0        0     4078 2024-05-14 14:21:32.000000 indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/split.py
+-rw-rw-rw-   0        0        0     6425 2024-05-13 08:09:25.000000 indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.661961 indox-0.1.3/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/
+-rw-rw-rw-   0        0        0       45 2024-05-14 14:02:48.000000 indox-0.1.3/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/__init__.py
+-rw-rw-rw-   0        0        0     2453 2024-05-15 14:05:13.000000 indox-0.1.3/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/loader.py
+-rw-rw-rw-   0        0        0     3596 2024-05-15 08:19:59.000000 indox-0.1.3/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/split.py
+-rw-rw-rw-   0        0        0      108 2024-05-14 14:18:27.000000 indox-0.1.3/Indox/DataLoaderSplitter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.662961 indox-0.1.3/Indox/Embeddings/
+-rw-rw-rw-   0        0        0       67 2024-05-12 16:34:51.000000 indox-0.1.3/Indox/Embeddings/__init__.py
+-rw-rw-rw-   0        0        0      495 2024-05-12 16:34:51.000000 indox-0.1.3/Indox/Embeddings/embedding_models.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.665960 indox-0.1.3/Indox/Evaluation/
+-rw-rw-rw-   0        0        0       28 2024-05-13 12:54:42.000000 indox-0.1.3/Indox/Evaluation/__init__.py
+-rw-rw-rw-   0        0        0     7715 2024-05-19 08:29:16.000000 indox-0.1.3/Indox/Evaluation/eval.py
+-rw-rw-rw-   0        0        0     2906 2024-05-13 12:39:30.000000 indox-0.1.3/Indox/Evaluation/metrics.py
+-rw-rw-rw-   0        0        0     4719 2024-05-19 08:29:16.000000 indox-0.1.3/Indox/Evaluation/similarity.py
+-rw-rw-rw-   0        0        0    10059 2024-05-13 12:39:30.000000 indox-0.1.3/Indox/Evaluation/unieval.py
+-rw-rw-rw-   0        0        0     2453 2024-05-11 13:44:58.000000 indox-0.1.3/Indox/Graph.py
+-rw-rw-rw-   0        0        0     8869 2024-05-16 15:16:32.000000 indox-0.1.3/Indox/Indox.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.665960 indox-0.1.3/Indox/QaModels/
+drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.666962 indox-0.1.3/Indox/QaModels/Dspy_Cot/
+-rw-rw-rw-   0        0        0       27 2024-05-12 15:50:15.000000 indox-0.1.3/Indox/QaModels/Dspy_Cot/__init__.py
+-rw-rw-rw-   0        0        0     2654 2024-05-13 14:07:14.000000 indox-0.1.3/Indox/QaModels/Dspy_Cot/dspy.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.667963 indox-0.1.3/Indox/QaModels/Mistral/
+-rw-rw-rw-   0        0        0       30 2024-05-12 15:50:15.000000 indox-0.1.3/Indox/QaModels/Mistral/__init__.py
+-rw-rw-rw-   0        0        0     2756 2024-05-12 15:50:15.000000 indox-0.1.3/Indox/QaModels/Mistral/mistral.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.668963 indox-0.1.3/Indox/QaModels/OpenAi/
+-rw-rw-rw-   0        0        0       30 2024-05-12 15:50:15.000000 indox-0.1.3/Indox/QaModels/OpenAi/__init__.py
+-rw-rw-rw-   0        0        0     2232 2024-05-15 14:01:50.000000 indox-0.1.3/Indox/QaModels/OpenAi/openai.py
+-rw-rw-rw-   0        0        0       95 2024-05-14 13:59:17.000000 indox-0.1.3/Indox/QaModels/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.669963 indox-0.1.3/Indox/Splitter/
+-rw-rw-rw-   0        0        0       60 2024-05-15 04:55:56.000000 indox-0.1.3/Indox/Splitter/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-05-14 14:16:18.000000 indox-0.1.3/Indox/Splitter/semantic_text_splitter.py
+-rw-rw-rw-   0        0        0       66 2024-05-12 15:34:14.000000 indox-0.1.3/Indox/__init__.py
+-rw-rw-rw-   0        0        0      960 2024-05-14 11:18:39.000000 indox-0.1.3/Indox/config.yaml
+-rw-rw-rw-   0        0        0     2738 2024-05-15 06:17:01.000000 indox-0.1.3/Indox/utils.py
+-rw-rw-rw-   0        0        0     8896 2024-05-13 14:07:14.000000 indox-0.1.3/Indox/vectorstore.py
+-rw-rw-rw-   0        0        0     2562 2024-05-16 15:16:32.000000 indox-0.1.3/Indox/visualization.py
+drwxrwxrwx   0        0        0        0 2024-05-20 10:10:44.670963 indox-0.1.3/Indox.egg-info/
+-rw-rw-rw-   0        0        0     8261 2024-05-20 10:10:44.000000 indox-0.1.3/Indox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1391 2024-05-20 10:10:44.000000 indox-0.1.3/Indox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 10:10:44.000000 indox-0.1.3/Indox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      274 2024-05-20 10:10:44.000000 indox-0.1.3/Indox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-20 10:10:44.000000 indox-0.1.3/Indox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2024-05-11 13:44:58.000000 indox-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     8261 2024-05-20 10:10:44.671964 indox-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6916 2024-05-20 09:59:26.000000 indox-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-20 10:10:44.672964 indox-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1307 2024-05-20 10:10:06.000000 indox-0.1.3/setup.py
```

### Comparing `Indox-0.1.1/Indox/Embedding.py` & `indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/Embed.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,12 @@
 import numpy as np
-from .cluster.Clustering import perform_clustering
 import pandas as pd
 from typing import List
-from .utils import read_config
-from langchain_community.embeddings import HuggingFaceEmbeddings
-from langchain_openai import OpenAIEmbeddings
-import os
 
-
-def embedding_model():
-    """
-    Retrieve the embedding model based on the configuration settings.
-
-    Returns:
-    - embeddings: An instance of the appropriate embeddings model as specified in the configuration.
-
-    Raises:
-    - KeyError: If the `embedding_model` key is missing in the configuration.
-    - ValueError: If the specified embedding model name isn't recognized.
-
-    Notes:
-    - The function relies on the `read_config` method to determine which model to use.
-    - The function currently supports 'openai' and 'sbert' as embedding models.
-    """
-    # Load configuration settings
-    config = read_config()
-
-    # Verify the embedding model type from the configuration
-    embedding_model_name = config['embedding_model'].lower()
-
-    if embedding_model_name == 'openai':
-        model = "text-embedding-3-small"
-        embeddings = OpenAIEmbeddings(model=model, openai_api_key=os.environ["OPENAI_API_KEY"])
-        return embeddings
-    elif embedding_model_name == 'sbert':
-        embeddings = HuggingFaceEmbeddings(model_name="multi-qa-mpnet-base-cos-v1")
-        return embeddings
-    else:
-        raise ValueError(f"Unrecognized embedding model specified in the configuration: {embedding_model_name}")
+from .Clustering import perform_clustering
 
 
 def embed(texts: List[str], embeddings) -> np.ndarray:
     """
     Generate embeddings for a list of text documents using a provided embeddings object.
 
     Parameters:
@@ -53,16 +18,15 @@
     """
     text_embeddings = embeddings.embed_documents(texts)
 
     text_embeddings_np = np.array(text_embeddings)
     return text_embeddings_np
 
 
-def embed_cluster_texts(texts: List[str], embeddings) -> pd.DataFrame:
-    config = read_config()
+def embed_cluster_texts(texts: List[str], embeddings, dim, threshold) -> pd.DataFrame:
     """
     Embeds and clusters a list of texts using a provided embeddings object, returning a DataFrame with texts, their embeddings, and cluster labels.
 
     This function combines embedding generation and clustering into a single step. It assumes the existence
     of a previously defined `perform_clustering` function that performs clustering on the embeddings.
 
     Parameters:
@@ -73,15 +37,15 @@
     - pandas.DataFrame: A DataFrame containing the original texts, their embeddings, and the assigned cluster labels.
     """
     text_embeddings_np = embed(
         texts, embeddings
     )  # Generate embeddings using the provided embeddings object
     cluster_labels = perform_clustering(
         text_embeddings_np,
-        config["clustering"]["dim"],
-        config["clustering"]["threshold"],
+        dim=dim,
+        threshold=threshold,
     )  # Perform clustering on the embeddings
     df = pd.DataFrame()  # Initialize a DataFrame to store the results
     df["text"] = texts  # Store original texts
     df["embd"] = list(text_embeddings_np)  # Store embeddings as a list in the DataFrame
     df["cluster"] = cluster_labels  # Store cluster labels
     return df
```

### Comparing `Indox-0.1.1/Indox/Graph.py` & `indox-0.1.3/Indox/Graph.py`

 * *Files identical despite different names*

### Comparing `Indox-0.1.1/Indox/Summary.py` & `indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/Summary.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from openai import OpenAI
-from .utils import read_config
+from ...utils import read_config
 from transformers import pipeline
 import logging
 
 
-# logging.basicConfig(
-#     format="%(asctime)s - %(levelname)s - %(message)s", level=logging.INFO
-# )
+
 
 
 def summarize(context):
     """
     Summarizes the given context using either OpenAI's GPT-3.5 model or a Hugging Face model based on the configuration.
 
     Args:
```

### Comparing `Indox-0.1.1/Indox/cluster/Clustering.py` & `indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/Clustering.py`

 * *Files identical despite different names*

### Comparing `Indox-0.1.1/Indox/cluster/EmbedClusterSummarize.py` & `indox-0.1.3/Indox/DataLoaderSplitter/ClusteredSplit/EmbedClusterSummarize.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from typing import List, Tuple, Optional, Any, Dict
+from typing import List
 import pandas as pd
-from ..Embedding import embed_cluster_texts
-from ..Summary import summarize
-from ..clean import remove_stopwords_chunk
+from .Embed import embed_cluster_texts
+from .Summary import summarize
+from .utils import rechunk
+from ..utils.clean import remove_stopwords_chunk
+
 
 def embed_cluster_summarize_texts(
-        texts: List[str], embeddings, level: int, re_chunk=False, max_chunk: int = 100):
+        texts: List[str], embeddings, dim, threshold, level: int, re_chunk=False, max_chunk: int = 100):
     """
     Embeds, clusters, and summarizes a list of texts. This function first generates embeddings for the texts,
     clusters them based on similarity, expands the cluster assignments for easier processing, and then summarizes
     the content within each cluster.
 
     Parameters:
     - texts: A list of text documents to be processed.
@@ -21,15 +23,15 @@
       1. The first DataFrame (`df_clusters`) includes the original texts, their embeddings, and cluster assignments.
       2. The second DataFrame (`df_summary`) contains summaries for each cluster, the specified level of detail,
          and the cluster identifiers.
     """
     input_tokens_all = 0
     output_tokens_all = 0
     # Embed and cluster the texts, resulting in a DataFrame with 'text', 'embd', and 'cluster' columns
-    df_clusters = embed_cluster_texts(texts, embeddings)
+    df_clusters = embed_cluster_texts(texts, embeddings, dim, threshold)
 
     # Expand DataFrame entries to document-cluster pairings for straightforward processing
     expanded_list = [
         {"text": row["text"], "embd": row["embd"], "cluster": cluster}
         for index, row in df_clusters.iterrows()
         for cluster in row["cluster"]
     ]
@@ -55,41 +57,42 @@
             "summaries": summaries,
             "level": [level] * len(summaries),
             "cluster": list(all_clusters),
         }
     )
 
     if re_chunk:
-        from ..Splitter import rechunk
         df_summary = rechunk(df_summary=df_summary, max_chunk=max_chunk)
 
     return df_clusters, df_summary, input_tokens_all, output_tokens_all
 
 
-def recursive_embed_cluster_summarize(texts: List[str], embeddings, level: int = 1, n_levels: int = 3,
-                                      re_chunk=False, max_chunk: int = 100, remove_sword=False):
+def recursive_embed_cluster_summarize(texts: List[str], embeddings, dim, threshold, max_chunk: int = 100,
+                                      level: int = 1,
+                                      n_levels: int = 3,
+                                      re_chunk=False, remove_sword=False):
     """
     Recursively embeds, clusters, and summarizes texts up to a specified level or until
     the number of unique clusters becomes 1, storing the results at each level using a specified embeddings object.
 
     Parameters:
     - texts: List[str], texts to be processed.
     - embeddings: An object capable of generating embeddings, must have an `embed_documents` method.
     - level: int, current recursion level (starts at 1).
     - n_levels: int, maximum depth of recursion.
 
     """
-    if remove_sword == True:
+    if remove_sword:
         texts = remove_stopwords_chunk(texts)
 
     results = {}
 
     # Perform embedding, clustering, and summarization for the current level
     df_clusters, df_summary, input_tokens, output_tokens = \
-        embed_cluster_summarize_texts(texts, embeddings,
+        embed_cluster_summarize_texts(texts, embeddings, dim, threshold,
                                       level, re_chunk=re_chunk,
                                       max_chunk=max_chunk)
     input_tokens_all = input_tokens
     output_tokens_all = output_tokens
     # Store the results of the current level
     results[level] = (df_clusters, df_summary)
```

### Comparing `Indox-0.1.1/Indox/metrics/unieval.py` & `indox-0.1.3/Indox/Evaluation/unieval.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,14 +177,15 @@
                 eval_scores[i]['overall'] = np.mean(list(eval_scores[i].values()))
 
         # if print_result == True:
         #     print_scores(eval_scores)
 
         return eval_scores
 
+
 def add_question(dimension, output, src=None, ref=None, context=None):
     """
         Add questions to generate input in Bool-QA format for UniEval.
 
         dimension: specific dimension to be evaluated
         src: source input for different NLG tasks. For example, source document for summarization
              and dialogue history for dialogue response generation.
@@ -211,8 +212,8 @@
         elif dimension == 'understandability':
             cur_input = 'question: Is this an understandable response in the dialogue? </s> response: ' + output[i]
         else:
             raise NotImplementedError(
                 'The input format for this dimension is still undefined. Please customize it first.')
 
         input_with_question.append(cur_input)
-    return input_with_question
+    return input_with_question
```

### Comparing `Indox-0.1.1/README.md` & `indox-0.1.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # inDox: Advanced Search and Retrieval Augmentation Generative
 
-## Overview
-This project, **inDox**, leverages advanced clustering techniques provided by **Raptor** alongside the efficient retrieval capabilities of **pgvector** and other vector stores. It is designed to allow users to interact with and visualize data within a PostgreSQL database effectively. The solution involves segmenting text data into manageable chunks, enhancing retrieval through a custom model, and providing an intuitive interface for querying and retrieving relevant information.
+**Indox Retrieval Augmentation** is an innovative application designed to streamline information extraction from a wide
+range of document types, including text files, PDF, HTML, Markdown, and LaTeX. Whether structured or unstructured, Indox
+provides users with a powerful toolset to efficiently extract relevant data.
+
+Indox Retrieval Augmentation is an innovative application designed to streamline information extraction from a wide
+range of document types, including text files, PDF, HTML, Markdown, and LaTeX. Whether structured or unstructured, Indox
+provides users with a powerful toolset to efficiently extract relevant data. One of its key features is the ability to
+intelligently cluster primary chunks to form more robust groupings, enhancing the quality and relevance of the extracted
+information.
+With a focus on adaptability and user-centric design, Indox aims to deliver future-ready functionality with more
+features planned for upcoming releases. Join us in exploring how Indox can revolutionize your document processing
+workflow, bringing clarity and organization to your data retrieval needs.
 
 ## Prerequisites
+
 Before running this project, ensure that you have the following installed:
+
 - **Python 3.8+**: Required for running the Python backend.
 - **PostgreSQL**: Needed if you wish to store your data in a PostgreSQL database.
 - **OpenAI API Key**: Necessary if you are using the OpenAI embedding model.
+- **HuggingFace API Key**: Necessary if you are using the HuggingFace llms.
 
 Ensure your system also meets these requirements:
+
 - Access to environmental variables for handling sensitive information like API keys.
 - Suitable hardware capable of supporting intensive computational tasks.
 
-## Optional Libraries and Enhancements
-### Unstructured Data Handling
-For those looking to process unstructured data such as PDF, HTML, Markdown, LaTeX, and plain text files.
-
-### Additional Clustering Layer
-- If the `unstructured` library is not used, you can opt to add an extra clustering layer specifically optimized for structured PDFs or text files to enhance data handling.
-
-### PostgreSQL with pgVector
-- **Required Version**: Make sure to use PostgreSQL versions that are compatible with `pgvector`. We recommend PostgreSQL 12 or newer to ensure full compatibility with all features.
-
-
-
 ## Installation
 
 Clone the repository and navigate to the directory:
 
 ```bash
 git clone https://github.com/osllmai/inDox.git
 cd inDox
@@ -39,160 +41,167 @@
 ```bash
 pip install -r requirements.txt
 ```
 
 ## Configuration
 
 ### Environment Variables
-Set your `OPENAI_API_KEY` in your environment variables for secure access.
+
+Set your `OPENAI_API_KEY` or `HF_API_KEY` in your environment variables for secure access.
 
 ### Database Setup
-Ensure your PostgreSQL database is up and running, and accessible from your application. (if you are going to use pgvector as your vectorstore)
+
+Ensure your PostgreSQL database is up and running, and accessible from your application. This is necessary if you plan to use pgvector as your vector store.
+
+Alternatively, you can use Chroma or Faiss as your vector store. Make sure to specify your choice and the necessary configurations in the config.yaml file.
 
 ## Usage
 
 ### Preparing Your Data
 
 1. **Define the File Path**: Specify the path to your text or PDF file.
 2. **Load Embedding Models**: Initialize your embedding model from OpenAI's selection of pre-trained models.
 
-## Config Setup
-Before launching your first instance of **inDox**, it's crucial to properly configure the QA model and the embedding model. This configuration is done through the `IRA.config` YAML file.
+# Quick Start 
+
+## Import Indox Package
 
+Import the necessary classes from the Indox package.
 
+``` python
+from Indox import IndoxRetrievalAugmentation
+```
 
+### Initialize Indox
 
-## Initialize the Retrieval System
+Create an instance of IndoxRetrievalAugmentation.
 
-```python
-from Indox import IndoxRetrievalAugmentation
-IRA = IndoxRetrievalAugmentation()
+``` python
+Indox = IndoxRetrievalAugmentation()
 ```
+## Initial Configuration
 
-### Initial Configuration
-- **Configuration File**: Ensure you locate and modify the `IRA.config` YAML file according to your needs before starting the application. 
+- **Configuration File**: Ensure you locate and modify the `Indox.config` YAML file according to your needs before
+  starting the application.
 
 ## Dynamic Configuration Changes
+
 For changes that need to be applied after the initial setup or during runtime:
+
 - **Modifying Configurations**: Use the following Python snippet to update your settings dynamically:
   ```python
-  IRA.config["your_setting_that_need_to_change"] = "new_setting"
-  IRA.initialize()
-
+  Indox.config["your_setting_that_need_to_change"] = "new_setting"
+  Indox.update_config()
 
 ## Configuration Details
-Here's a breakdown of the config dictionary and its properties:
 
-### Clustering
-- `dim`: Specifies the dimension of clustering.
-- `threshold`: Lower thresholds mean more samples will be clustered together; higher thresholds increase the number of clusters but decrease their size.
+Here's a breakdown of the config dictionary and its properties:
 
 ### PostgreSQL
-- `conn_string`: Your PostgreSQL database credentials.
 
-### QA Model
-- `temperature`: Controls the diversity of the QA model's responses. Higher values increase diversity but also the risk of nonsensical outputs; lower values decrease diversity and reduce risks.
+- `conn_string`: Your PostgreSQL database credentials.
 
 ### Summary Model
+
 - `max_tokens`: Maximum token count the summary model can generate.
 - `min_len`: Minimum token count the summary model generates.
-- `model_name`: Default is `gpt-3.5-turbo-0125`, but it can be replaced with any Hugging Face model supporting the summarization pipeline.
-
-### Embedding Model
-- The default embedding model is OpenAI embeddings. Optionally, "SBert" can be used:
-  ```python
-  {"embedding_model": "SBert"}
-
-### Splitter
-Options include `raptor-text-splitter` and `semantic-text-splitter`.
-
-### Considerations for Re-Chunking
-
-- **Using `unstructured` Library**: Setting `re_chunk` to `True` disables the use of the `unstructured` library due to compatibility issues.
-- **Extra Clustering Layer**: If `re_chunk` is set to `True` and the user opts for an additional clustering layer, re-chunking is applied to the outputs of the summary model. However, it is crucial to note that if the summary model's output is less than 500 tokens, re-chunking is not recommended due to potential inefficiency and lack of necessity.
-
-### Generate Chunks
-
-```python
-documents = IRA.create_chunks(file_path=html, max_chunk_size=200, content_type=None,
-                                             unstructured=False, re_chunk= False, remove_sword=False)
-print("Documents:", documents)
-```
-
-  
-- The re_chunk argument in the create_chunks function of IRA object, specifies whether to perform re-chunking of the data:
-False: Chunking occurs only at the start of the process.
-True: Chunking happens after each summarization process.
-
-- The `max_chunk_size` parameter specifies the maximum number of tokens in each chunk.
-- Using the `unstructured` library, users can add files in PDF, HTML, Markdown, LaTeX, or plain text formats. In this scenario, chunking is performed using the `chunk_by_title` method from the `unstructured` library, which organizes the content by titles within the document.
-- The remove_sword specifies if the stop words are going to be removed or not.
+- `model_name`: Default is `gpt-3.5-turbo-0125`, but it can be replaced with any Hugging Face model supporting the
+  summarization pipeline.
 
 ### PostgreSQL Setup with pgvector
 
 If you want to use PostgreSQL for vector storage, you should perform the following steps:
 
-1. **Install pgvector**: To install `pgvector` on your PostgreSQL server, follow the detailed installation instructions available on the official pgvector GitHub repository:
+1. **Install pgvector**: To install `pgvector` on your PostgreSQL server, follow the detailed installation instructions
+   available on the official pgvector GitHub repository:
    [pgvector Installation Instructions](https://github.com/pgvector/pgvector)
 
 2. **Add Vector Extension**:
    Connect to your PostgreSQL database and execute the following SQL command to create the `pgvector` extension:
 
    ```sql
    -- Connect to your database
    psql -U username -d database_name
 
    -- Run inside your psql terminal
    CREATE EXTENSION vector;
    # Replace the placeholders with your actual PostgreSQL credentials and details
 
+Additionally, for those interested in exploring other vector database options, you can consider using **Chroma** or *
+*Faiss**. These provide alternative approaches to vector storage and retrieval that may better suit specific use cases
+or performance requirements.
+
+### Importing QA and Embedding Models
+
+``` python
+from Indox.QaModels import OpenAiQA
+```
+
+``` python
+from Indox.Embeddings import OpenAiEmbedding
+```
+
+
+``` python
+openai_qa = OpenAiQA(api_key=OPENAI_API_KEY,model="gpt-3.5-turbo-0125")
+openai_embeddings = OpenAiEmbedding(model="text-embedding-3-small",openai_api_key=OPENAI_API_KEY)
+```
+
+## Modifying Configuration Settings
 
-Additionally, for those interested in exploring other vector database options, you can consider using **Chroma** or **Faiss**. These provide alternative approaches to vector storage and retrieval that may better suit specific use cases or performance requirements.
+To change a configuration setting, you can directly modify the
+`Indox.config` dictionary. Here is an example of how you can update a
+configuration setting:
 
-### Next, you need to connect to the vectorstore
+``` python
+# Example of modifying a configuration setting
+Indox.config["old_config"] = "new_config"
 
-```python
-indox.connect_to_vectorstore(collection_name='your_collection_name')
+# Applying the updated configuration
+Indox.update_config()
 ```
 
-### Store in vectorstore
 
-```python
-# you need to set your database credentials in th config.yaml file
-indox.store_in_vectorstore(chunks=documents)
+We take advantage of the `unstructured` library to load
+documents and split them into chunks by title. This method helps in
+organizing thme document into manageable sections for further
+processing.
+
+``` python
+from Indox.DataLoaderSplitter import UnstructuredLoadAndSplit
 ```
 
+``` python
+docs_unstructured = UnstructuredLoadAndSplit(file_path=file_path)
+```
 
-### Querying
+    Starting processing...
+    End Chunking process.
 
-Lastly, we can use the IRA and asnwer to queries using answer_question function from IRA object.
+Storing document chunks in a vector store is crucial for enabling
+efficient retrieval and search operations. By converting text data into
+vector representations and storing them in a vector store, you can
+perform rapid similarity searches and other vector-based operations.
 
-```python
-response = IRA.answer_question(query="your query?!", top_k=5, document_relevancy_filter=False)
-print("Responses:", response[0])
-print("Retrieve chunks and scores:", response[1])
+``` python
+Indox.connect_to_vectorstore(collection_name="sample",embeddings=openai_embeddings)
+Indox.store_in_vectorstore(chunks=docs_unstructured)
 ```
-- the top_k argument speficies how many similar documents will be returned from vectorstore.
-- the document_relevancy_filter argument: if set to True, filters out irrelevant documents in the top_k documents.
-### Roadmap
 
-- [x] vector stores
-   - [x] pgvector
-   - [x] chromadb  
-   - [x] faiss
+## Quering
 
-- [x] summary models
-   - [x] openai chatgpt
-   - [x] huggingface models
+``` python
+query = "your query!!??"
+```
 
-- [x] embedding models
-   - [x] openai embeddings
-   - [x] sentence transformer embeddings
+``` python
+response_openai = Indox.answer_question(query=query,qa_model=openai_qa)
+```
 
-- [x] chunking strategies
-   - [x] semantic chunking
+``` python
+answer = response_openai[0]
+```
 
-- [x] add unstructured support
+``` python
+context, score = response_openai[1]
+```
 
-- [x] add simple RAG support
-      
-- [ ] cleaning pipeline
```

