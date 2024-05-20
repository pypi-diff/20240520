# Comparing `tmp/Indox-0.1.1.tar.gz` & `tmp/indox-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Indox-0.1.1.tar", last modified: Wed May  8 13:36:50 2024, max compression
+gzip compressed data, was "indox-0.1.2.tar", last modified: Mon May 20 09:40:53 2024, max compression
```

## Comparing `Indox-0.1.1.tar` & `indox-0.1.2.tar`

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
+drwxrwxrwx   0        0        0        0 2024-05-20 09:40:53.693103 indox-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-05-20 09:40:53.373793 indox-0.1.2/Indox/
+drwxrwxrwx   0        0        0        0 2024-05-20 09:40:53.401616 indox-0.1.2/Indox/DataLoaderSplitter/
+drwxrwxrwx   0        0        0        0 2024-05-20 09:40:53.492179 indox-0.1.2/Indox/DataLoaderSplitter/ClusteredSplit/
+-rw-rw-rw-   0        0        0     6348 2024-05-11 13:44:58.000000 indox-0.1.2/Indox/DataLoaderSplitter/ClusteredSplit/Clustering.py
+-rw-rw-rw-   0        0        0     2074 2024-05-13 06:41:26.000000 indox-0.1.2/Indox/DataLoaderSplitter/ClusteredSplit/Embed.py
+-rw-rw-rw-   0        0        0     4781 2024-05-13 08:12:00.000000 indox-0.1.2/Indox/DataLoaderSplitter/ClusteredSplit/EmbedClusterSummarize.py
+-rw-rw-rw-   0        0        0     2856 2024-05-13 06:27:35.000000 indox-0.1.2/Indox/DataLoaderSplitter/ClusteredSplit/Summary.py
+-rw-rw-rw-   0        0        0       35 2024-05-14 14:02:48.000000 indox-0.1.2/Indox/DataLoaderSplitter/ClusteredSplit/__init__.py
+-rw-rw-rw-   0        0        0     4078 2024-05-14 14:21:32.000000 indox-0.1.2/Indox/DataLoaderSplitter/ClusteredSplit/split.py
+-rw-rw-rw-   0        0        0     6425 2024-05-13 08:09:25.000000 indox-0.1.2/Indox/DataLoaderSplitter/ClusteredSplit/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:40:53.552854 indox-0.1.2/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/
+-rw-rw-rw-   0        0        0       45 2024-05-14 14:02:48.000000 indox-0.1.2/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/__init__.py
+-rw-rw-rw-   0        0        0     2453 2024-05-15 14:05:13.000000 indox-0.1.2/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/loader.py
+-rw-rw-rw-   0        0        0     3596 2024-05-15 08:19:59.000000 indox-0.1.2/Indox/DataLoaderSplitter/UnstructuredLoadAndSplit/split.py
+-rw-rw-rw-   0        0        0      108 2024-05-14 14:18:27.000000 indox-0.1.2/Indox/DataLoaderSplitter/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:40:53.563770 indox-0.1.2/Indox/Embeddings/
+-rw-rw-rw-   0        0        0       67 2024-05-12 16:34:51.000000 indox-0.1.2/Indox/Embeddings/__init__.py
+-rw-rw-rw-   0        0        0      495 2024-05-12 16:34:51.000000 indox-0.1.2/Indox/Embeddings/embedding_models.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:40:53.627041 indox-0.1.2/Indox/Evaluation/
+-rw-rw-rw-   0        0        0       28 2024-05-13 12:54:42.000000 indox-0.1.2/Indox/Evaluation/__init__.py
+-rw-rw-rw-   0        0        0     7715 2024-05-19 08:29:16.000000 indox-0.1.2/Indox/Evaluation/eval.py
+-rw-rw-rw-   0        0        0     2906 2024-05-13 12:39:30.000000 indox-0.1.2/Indox/Evaluation/metrics.py
+-rw-rw-rw-   0        0        0     4719 2024-05-19 08:29:16.000000 indox-0.1.2/Indox/Evaluation/similarity.py
+-rw-rw-rw-   0        0        0    10059 2024-05-13 12:39:30.000000 indox-0.1.2/Indox/Evaluation/unieval.py
+-rw-rw-rw-   0        0        0     2453 2024-05-11 13:44:58.000000 indox-0.1.2/Indox/Graph.py
+-rw-rw-rw-   0        0        0     8869 2024-05-16 15:16:32.000000 indox-0.1.2/Indox/Indox.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:40:53.633061 indox-0.1.2/Indox/QaModels/
+drwxrwxrwx   0        0        0        0 2024-05-20 09:40:53.644609 indox-0.1.2/Indox/QaModels/Dspy_Cot/
+-rw-rw-rw-   0        0        0       27 2024-05-12 15:50:15.000000 indox-0.1.2/Indox/QaModels/Dspy_Cot/__init__.py
+-rw-rw-rw-   0        0        0     2654 2024-05-13 14:07:14.000000 indox-0.1.2/Indox/QaModels/Dspy_Cot/dspy.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:40:53.657081 indox-0.1.2/Indox/QaModels/Mistral/
+-rw-rw-rw-   0        0        0       30 2024-05-12 15:50:15.000000 indox-0.1.2/Indox/QaModels/Mistral/__init__.py
+-rw-rw-rw-   0        0        0     2756 2024-05-12 15:50:15.000000 indox-0.1.2/Indox/QaModels/Mistral/mistral.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:40:53.668136 indox-0.1.2/Indox/QaModels/OpenAi/
+-rw-rw-rw-   0        0        0       30 2024-05-12 15:50:15.000000 indox-0.1.2/Indox/QaModels/OpenAi/__init__.py
+-rw-rw-rw-   0        0        0     2232 2024-05-15 14:01:50.000000 indox-0.1.2/Indox/QaModels/OpenAi/openai.py
+-rw-rw-rw-   0        0        0       95 2024-05-14 13:59:17.000000 indox-0.1.2/Indox/QaModels/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:40:53.690128 indox-0.1.2/Indox/Splitter/
+-rw-rw-rw-   0        0        0       60 2024-05-15 04:55:56.000000 indox-0.1.2/Indox/Splitter/__init__.py
+-rw-rw-rw-   0        0        0      377 2024-05-14 14:16:18.000000 indox-0.1.2/Indox/Splitter/semantic_text_splitter.py
+-rw-rw-rw-   0        0        0       66 2024-05-12 15:34:14.000000 indox-0.1.2/Indox/__init__.py
+-rw-rw-rw-   0        0        0      960 2024-05-14 11:18:39.000000 indox-0.1.2/Indox/config.yaml
+-rw-rw-rw-   0        0        0     2738 2024-05-15 06:17:01.000000 indox-0.1.2/Indox/utils.py
+-rw-rw-rw-   0        0        0     8896 2024-05-13 14:07:14.000000 indox-0.1.2/Indox/vectorstore.py
+-rw-rw-rw-   0        0        0     2562 2024-05-16 15:16:32.000000 indox-0.1.2/Indox/visualization.py
+drwxrwxrwx   0        0        0        0 2024-05-20 09:40:53.691101 indox-0.1.2/Indox.egg-info/
+-rw-rw-rw-   0        0        0     5920 2024-05-20 09:40:52.000000 indox-0.1.2/Indox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1391 2024-05-20 09:40:53.000000 indox-0.1.2/Indox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 09:40:52.000000 indox-0.1.2/Indox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      274 2024-05-20 09:40:52.000000 indox-0.1.2/Indox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-20 09:40:52.000000 indox-0.1.2/Indox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2024-05-11 13:44:58.000000 indox-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5920 2024-05-20 09:40:53.691101 indox-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4575 2024-05-20 08:20:02.000000 indox-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-20 09:40:53.693103 indox-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1307 2024-05-20 08:16:33.000000 indox-0.1.2/setup.py
```

### Comparing `Indox-0.1.1/Indox/Embedding.py` & `indox-0.1.2/Indox/DataLoaderSplitter/ClusteredSplit/Embed.py`

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

### Comparing `Indox-0.1.1/Indox/Graph.py` & `indox-0.1.2/Indox/Graph.py`

 * *Files identical despite different names*

### Comparing `Indox-0.1.1/Indox/Summary.py` & `indox-0.1.2/Indox/DataLoaderSplitter/ClusteredSplit/Summary.py`

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

### Comparing `Indox-0.1.1/Indox/cluster/Clustering.py` & `indox-0.1.2/Indox/DataLoaderSplitter/ClusteredSplit/Clustering.py`

 * *Files identical despite different names*

### Comparing `Indox-0.1.1/Indox/cluster/EmbedClusterSummarize.py` & `indox-0.1.2/Indox/DataLoaderSplitter/ClusteredSplit/EmbedClusterSummarize.py`

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

### Comparing `Indox-0.1.1/Indox/metrics/unieval.py` & `indox-0.1.2/Indox/Evaluation/unieval.py`

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

