# Comparing `tmp/gs_engine-0.27.0-py2.py3-none-macosx_12_0_x86_64.whl.zip` & `tmp/gs_engine-0.28.0a20240520-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,11 @@
-Zip file size: 13046 bytes, number of entries: 13
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-29 15:12 graphscope_runtime/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-29 15:12 gs_engine-0.27.0.dist-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-29 15:12 graphscope.runtime/
--rw-r--r--  2.0 unx      694 b- defN 24-Mar-29 12:40 graphscope_runtime/__init__.py
--rw-rw-r--  2.0 unx      804 b- defN 24-Mar-29 15:12 gs_engine-0.27.0.dist-info/RECORD
--rw-r--r--  2.0 unx      140 b- defN 24-Mar-29 15:03 gs_engine-0.27.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-Mar-29 15:03 gs_engine-0.27.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx    23170 b- defN 24-Mar-29 15:03 gs_engine-0.27.0.dist-info/METADATA
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-29 15:12 graphscope.runtime/conf/
--rw-r--r--  2.0 unx     1573 b- defN 24-Mar-29 12:40 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      398 b- defN 24-Mar-29 12:40 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      593 b- defN 24-Mar-29 12:40 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx      204 b- defN 24-Mar-29 12:40 graphscope.runtime/conf/log4rs.yml
-13 files, 27595 bytes uncompressed, 11174 bytes compressed:  59.5%
+Zip file size: 12698 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      398 b- defN 24-May-20 19:01 graphscope.runtime/conf/executor.vineyard.properties
+-rw-r--r--  2.0 unx      593 b- defN 24-May-20 19:01 graphscope.runtime/conf/frontend.vineyard.properties
+-rw-r--r--  2.0 unx     1573 b- defN 24-May-20 19:01 graphscope.runtime/conf/log4j2.xml
+-rw-r--r--  2.0 unx      204 b- defN 24-May-20 19:01 graphscope.runtime/conf/log4rs.yml
+-rw-r--r--  2.0 unx      694 b- defN 24-May-20 19:01 graphscope_runtime/__init__.py
+-rw-r--r--  2.0 unx    23359 b- defN 24-May-20 20:02 gs_engine-0.28.0a20240520.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-May-20 20:02 gs_engine-0.28.0a20240520.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-May-20 20:02 gs_engine-0.28.0a20240520.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      831 b- defN 24-May-20 20:02 gs_engine-0.28.0a20240520.dist-info/RECORD
+9 files, 27781 bytes uncompressed, 11236 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -1,40 +1,28 @@
-Filename: graphscope_runtime/
-Comment: 
-
-Filename: gs_engine-0.27.0.dist-info/
-Comment: 
-
-Filename: graphscope.runtime/
-Comment: 
-
-Filename: graphscope_runtime/__init__.py
-Comment: 
-
-Filename: gs_engine-0.27.0.dist-info/RECORD
+Filename: graphscope.runtime/conf/executor.vineyard.properties
 Comment: 
 
-Filename: gs_engine-0.27.0.dist-info/WHEEL
+Filename: graphscope.runtime/conf/frontend.vineyard.properties
 Comment: 
 
-Filename: gs_engine-0.27.0.dist-info/top_level.txt
+Filename: graphscope.runtime/conf/log4j2.xml
 Comment: 
 
-Filename: gs_engine-0.27.0.dist-info/METADATA
+Filename: graphscope.runtime/conf/log4rs.yml
 Comment: 
 
-Filename: graphscope.runtime/conf/
+Filename: graphscope_runtime/__init__.py
 Comment: 
 
-Filename: graphscope.runtime/conf/log4j2.xml
+Filename: gs_engine-0.28.0a20240520.dist-info/METADATA
 Comment: 
 
-Filename: graphscope.runtime/conf/executor.vineyard.properties
+Filename: gs_engine-0.28.0a20240520.dist-info/WHEEL
 Comment: 
 
-Filename: graphscope.runtime/conf/frontend.vineyard.properties
+Filename: gs_engine-0.28.0a20240520.dist-info/top_level.txt
 Comment: 
 
-Filename: graphscope.runtime/conf/log4rs.yml
+Filename: gs_engine-0.28.0a20240520.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=store
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## Comparing `gs_engine-0.27.0.dist-info/METADATA` & `gs_engine-0.28.0a20240520.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-engine
-Version: 0.27.0
+Version: 0.28.0a20240520
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -44,14 +44,15 @@
 🎉 See our ongoing [GraphScope Flex](https://github.com/alibaba/GraphScope/tree/main/flex): a LEGO-inspired, modular, and user-friendly GraphScope evolution. 🎉
 
 GraphScope is a unified distributed graph computing platform that provides a one-stop environment for performing diverse graph operations on a cluster of computers through a user-friendly Python interface. GraphScope makes multi-staged processing of large-scale graph data on compute clusters simply by combining several important pieces of Alibaba technology: including [GRAPE](https://github.com/alibaba/libgrape-lite), [MaxGraph](interactive_engine/), and [Graph-Learn](https://github.com/alibaba/graph-learn) (GL) for analytics, interactive, and graph neural networks (GNN) computation, respectively, and the [Vineyard](https://github.com/v6d-io/v6d) store that offers efficient in-memory data transfers.
 
 Visit our website at [graphscope.io](https://graphscope.io) to learn more.
 
 ## Latest News
+- [25/03/2024] 🙌🏻 We donated the graph file format [GraphAr](https://graphar.apache.org/) to [Apache Software Foundation](https://www.apache.org/) as an Incubating Project. 
 - [05/02/2024] 🎉 GraphScope Flex [paper](https://arxiv.org/abs/2312.12107) was accepted by [SIGMOD 2024](https://2024.sigmod.org/) Industry Track. See you in 🇨🇱!
 - [19/12/2023] 📑 A paper introducing GraphScope Flex released on [arXiv.org](https://arxiv.org/abs/2312.12107).
 - [20/07/2023] 🏆 GraphScope achieved record-breaking results on the [LDBC Social Network Benchmark Interactive workload](https://ldbcouncil.org/benchmarks/snb-interactive/), with a 2.45× higher throughput on SF300 than the previous record holder! 🏆
 - [04/07/2023] 🚀 GraphScope Flex tech preview released with [v0.23.0](https://github.com/alibaba/GraphScope/releases/tag/v0.23.0).
   
 ## Table of Contents
```

