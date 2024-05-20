# Comparing `tmp/vital-ai-vitalsigns-0.1.8.tar.gz` & `tmp/vital-ai-vitalsigns-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vital-ai-vitalsigns-0.1.8.tar", last modified: Tue May  7 19:59:43 2024, max compression
+gzip compressed data, was "vital-ai-vitalsigns-0.1.9.tar", last modified: Tue May  7 21:05:31 2024, max compression
```

## Comparing `vital-ai-vitalsigns-0.1.8.tar` & `vital-ai-vitalsigns-0.1.9.tar`

### file list

```diff
@@ -1,315 +1,315 @@
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.999418 vital-ai-vitalsigns-0.1.8/
--rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.8/LICENSE
--rw-r--r--   0 hadfield   (501) staff       (20)      707 2024-05-07 19:59:42.999149 vital-ai-vitalsigns-0.1.8/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)       25 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.8/README.md
--rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-07 19:59:42.999471 vital-ai-vitalsigns-0.1.8/setup.cfg
--rw-r--r--   0 hadfield   (501) staff       (20)     1141 2024-05-07 17:44:32.000000 vital-ai-vitalsigns-0.1.8/setup.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.946107 vital-ai-vitalsigns-0.1.8/test/
--rw-r--r--   0 hadfield   (501) staff       (20)      489 2024-05-02 22:13:47.000000 vital-ai-vitalsigns-0.1.8/test/test_embedding_model.py
--rw-r--r--   0 hadfield   (501) staff       (20)     2254 2024-05-07 18:10:12.000000 vital-ai-vitalsigns-0.1.8/test/test_graph_collection.py
--rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 17:51:38.000000 vital-ai-vitalsigns-0.1.8/test/test_package_discovery.py
--rw-r--r--   0 hadfield   (501) staff       (20)     2809 2024-05-07 18:01:11.000000 vital-ai-vitalsigns-0.1.8/test/test_query_builder.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.946335 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.947941 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/collection/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:00:36.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/collection/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)    11636 2024-05-07 18:14:44.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/collection/graph_collection.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:49:20.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/collection/networkx_collection_impl.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1030 2024-05-03 21:08:09.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/collection/rdf_collection_impl.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1961 2024-05-07 18:29:23.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/collection/vector_collection_impl.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.948187 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/embedding/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:22:30.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/embedding/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)     2608 2024-05-07 14:39:23.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/embedding/embedding_model.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.949109 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/impl/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 18:25:32.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/impl/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)     2401 2024-05-07 13:32:41.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/impl/vitalsigns_impl.py
--rw-r--r--   0 hadfield   (501) staff       (20)      269 2024-03-19 17:21:02.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/impl/vitalsigns_package.py
--rw-r--r--   0 hadfield   (501) staff       (20)     5439 2024-05-07 13:01:47.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/impl/vitalsigns_registry.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.952210 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/
--rw-r--r--   0 hadfield   (501) staff       (20)       47 2024-03-19 21:49:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/BaseDomainOntology.py
--rw-r--r--   0 hadfield   (501) staff       (20)     5214 2024-05-07 14:40:38.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/GraphObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1843 2024-05-04 18:11:27.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/VITAL_Edge.py
--rw-r--r--   0 hadfield   (501) staff       (20)      338 2024-03-17 20:11:18.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/VITAL_Edge.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1690 2024-05-04 18:13:01.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/VITAL_GraphContainerObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      310 2024-03-17 20:11:39.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/VITAL_GraphContainerObject.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1868 2024-05-04 18:13:13.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/VITAL_HyperEdge.py
--rw-r--r--   0 hadfield   (501) staff       (20)      354 2024-03-17 20:11:44.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/VITAL_HyperEdge.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1657 2024-05-04 18:13:26.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/VITAL_HyperNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      298 2024-03-17 20:11:51.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/VITAL_HyperNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1642 2024-05-04 18:11:50.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/VITAL_Node.py
--rw-r--r--   0 hadfield   (501) staff       (20)      294 2024-03-17 20:11:57.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/VITAL_Node.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.952540 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/classproperties/
--rw-r--r--   0 hadfield   (501) staff       (20)      250 2024-05-03 23:34:11.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/classproperties/ClassProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-03 22:18:04.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/classproperties/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.953100 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/datatype/
--rw-r--r--   0 hadfield   (501) staff       (20)      241 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/datatype/GeoLocation.py
--rw-r--r--   0 hadfield   (501) staff       (20)       23 2024-05-03 17:43:23.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/datatype/Truth.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/datatype/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.956200 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/
--rw-r--r--   0 hadfield   (501) staff       (20)      549 2024-05-07 13:21:09.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/BooleanProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      741 2024-05-07 13:24:30.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/DateTimeProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      683 2024-05-07 13:27:08.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/DoubleProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      680 2024-05-07 13:27:16.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/FloatProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      552 2024-05-03 20:22:16.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/GeoLocationProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      897 2024-05-03 20:45:02.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/IProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      676 2024-05-07 13:28:26.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/IntegerProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      724 2024-05-07 13:28:37.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/LongProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      355 2024-05-03 20:22:44.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/MultiValueProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      446 2024-05-07 13:31:15.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/OtherProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      675 2024-05-07 13:30:16.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/StringProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      540 2024-05-03 20:26:30.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/TruthProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)      669 2024-05-07 13:30:29.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/URIProperty.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.956669 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/trait/
--rw-r--r--   0 hadfield   (501) staff       (20)      701 2024-05-07 13:02:48.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/trait/PropertyTrait.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/trait/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.958138 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/query/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:00:23.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/query/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)      351 2024-05-03 22:16:06.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/query/property_constraint.py
--rw-r--r--   0 hadfield   (501) staff       (20)      293 2024-05-03 18:45:19.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/query/result_element.py
--rw-r--r--   0 hadfield   (501) staff       (20)      522 2024-05-03 18:46:27.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/query/result_list.py
--rw-r--r--   0 hadfield   (501) staff       (20)     2456 2024-05-04 14:04:22.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/query/vital_graph_query.py
--rw-r--r--   0 hadfield   (501) staff       (20)      565 2024-05-04 14:04:22.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/query/vital_query.py
--rw-r--r--   0 hadfield   (501) staff       (20)      889 2024-05-04 14:12:47.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/query/vital_select_query.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.958509 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/query_impl/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:01:10.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/query_impl/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:02:54.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/query_impl/sparql_query_impl.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:03:29.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/query_impl/weaviate_vector_query_impl.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.958892 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/service/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:50:18.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/service/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)       29 2024-05-07 17:57:40.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/service/base_service.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.959258 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/service/graph/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:52:56.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/service/graph/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:53:52.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/service/graph/graph_service.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:55:42.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/service/graph/name_graph.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:54:28.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/service/graph/virtuoso_service.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.959605 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/service/vector/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:52:44.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/service/vector/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:56:03.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/service/vector/vector_namespace.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:54:05.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/service/vector/vector_service.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:54:54.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/service/vector/weaviate_service.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:50:40.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/service/vital_segment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      109 2024-05-07 17:57:56.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/service/vital_service.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.959786 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/utils/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-02 19:19:42.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/utils/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)       30 2024-05-02 19:20:23.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/utils/uri_generator.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.960030 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-07 17:36:13.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.960466 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/client/
--rw-r--r--   0 hadfield   (501) staff       (20)       61 2024-05-07 17:37:01.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/client/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)     2832 2024-05-07 17:38:00.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/client/client.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.961733 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/db/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:15:12.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/db/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)    12405 2024-05-07 18:22:54.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/db/base.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.962486 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/db/executors/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:15:33.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/db/executors/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)     5628 2024-05-07 18:21:44.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/db/executors/hnsw_indexer.py
--rw-r--r--   0 hadfield   (501) staff       (20)     4847 2024-05-07 19:57:42.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/db/executors/inmemory_exact_indexer.py
--rw-r--r--   0 hadfield   (501) staff       (20)     4207 2024-05-07 17:31:35.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/db/executors/typed_executor.py
--rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-07 17:29:49.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/db/hnsw_vectordb.py
--rw-r--r--   0 hadfield   (501) staff       (20)      276 2024-05-07 17:30:02.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/db/inmemory_exact_vectordb.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1600 2024-05-07 17:30:22.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/db/service.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.964437 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/utils/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:16:37.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/utils/__init__.py
--rw-r--r--   0 hadfield   (501) staff       (20)      850 2024-05-07 17:24:00.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/utils/create_doc_type.py
--rw-r--r--   0 hadfield   (501) staff       (20)      734 2024-05-07 17:23:28.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/utils/pass_parameters.py
--rw-r--r--   0 hadfield   (501) staff       (20)     4157 2024-05-07 17:38:56.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/utils/push_to_hubble.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1471 2024-05-07 17:22:19.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/utils/sort_matches_by_score.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-07 17:22:38.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/utils/unify_input_output.py
--rw-r--r--   0 hadfield   (501) staff       (20)      894 2024-05-04 18:08:26.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vitalsigns.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.947204 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns.egg-info/
--rw-r--r--   0 hadfield   (501) staff       (20)      707 2024-05-07 19:59:42.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns.egg-info/PKG-INFO
--rw-r--r--   0 hadfield   (501) staff       (20)    15634 2024-05-07 19:59:42.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns.egg-info/SOURCES.txt
--rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-07 19:59:42.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns.egg-info/dependency_links.txt
--rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-07 19:59:42.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns.egg-info/entry_points.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       94 2024-05-07 19:59:42.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns.egg-info/requires.txt
--rw-r--r--   0 hadfield   (501) staff       (20)       45 2024-05-07 19:59:42.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns.egg-info/top_level.txt
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.964691 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.986222 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/
--rw-r--r--   0 hadfield   (501) staff       (20)     1476 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/AggregationResult.py
--rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/AggregationResult.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2083 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/DatabaseConnection.py
--rw-r--r--   0 hadfield   (501) staff       (20)      309 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/DatabaseConnection.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1551 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Dataset.py
--rw-r--r--   0 hadfield   (501) staff       (20)      186 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Dataset.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/DomainModel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      360 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/DomainModel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/DomainOntology.py
--rw-r--r--   0 hadfield   (501) staff       (20)     1273 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_SameAs.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_SameAs.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1285 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasApp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasApp.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasAuthKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasAuthKey.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasChildCategory.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasChildCategory.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasChildDomainModel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasChildDomainModel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1288 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasDbConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasDbConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasIndexConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasIndexConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasOrganization.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasOrganization.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasParentDomainModel.py
--rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasParentDomainModel.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasProvisioning.py
--rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasProvisioning.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasSegment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasSegment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasSession.py
--rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasSession.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1309 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasTransaction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasTransaction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/GraphMatch.py
--rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/GraphMatch.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1664 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/RDFStatement.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/RDFStatement.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1381 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SparqlAskResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SparqlAskResponse.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SparqlBinding.py
--rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SparqlBinding.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1531 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SparqlDatabaseConnection.py
--rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SparqlDatabaseConnection.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SparqlUpdateResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SparqlUpdateResponse.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1414 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SqlDatabaseConnection.py
--rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SqlDatabaseConnection.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1307 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SqlResultRow.py
--rw-r--r--   0 hadfield   (501) staff       (20)      168 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SqlResultRow.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1382 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SqlUpdateResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SqlUpdateResponse.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1353 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/URIReference.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/URIReference.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_Category.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_Category.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1256 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_Event.py
--rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_Event.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1279 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_GraphQuery.py
--rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_GraphQuery.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1276 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_PathQuery.py
--rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_PathQuery.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1483 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_PayloadNode.py
--rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_PayloadNode.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_PeerEdge.py
--rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_PeerEdge.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1358 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_Query.py
--rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_Query.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1282 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_SelectQuery.py
--rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_SelectQuery.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1277 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_TaxonomyEdge.py
--rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_TaxonomyEdge.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1343 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalApp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalApp.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1353 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalAuthKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalAuthKey.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1379 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalOrganization.py
--rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalOrganization.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1274 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalProvisioning.py
--rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalProvisioning.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1458 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalSegment.py
--rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalSegment.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1294 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceAdminKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceAdminKey.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1951 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceAllegrographConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      305 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceAllegrographConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     2419 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      414 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1540 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceIndexedDBConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceIndexedDBConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1279 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceKey.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1435 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceLuceneDiskConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceLuceneDiskConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1342 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceLuceneMemoryConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceLuceneMemoryConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceMockConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceMockConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1423 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServicePrimeConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServicePrimeConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1291 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceRootKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceRootKey.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceSaaSConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceSaaSConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1423 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceSparkConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceSparkConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1923 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceSqlConfig.py
--rw-r--r--   0 hadfield   (501) staff       (20)      294 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceSqlConfig.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1555 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalSession.py
--rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalSession.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)     1482 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalTransaction.py
--rw-r--r--   0 hadfield   (501) staff       (20)      173 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalTransaction.pyi
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/__init__.py
-drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 19:59:42.998844 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/
--rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_URIProp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasAggregationType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasAppID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasBackwardCompVersion.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasCatalogName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasConfigString.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasConnectionError.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasConnectionState.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasDatabase.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasDateRetrieved.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasDbType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasDefaultPackageValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasDefaultSegmentName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasDomainOWL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasDomainOWLHash.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasEdgeDestination.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasEdgeSource.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasEndpointType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasEndpointURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasGraphQueries.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasHyperEdgeDestination.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasHyperEdgeSource.py
--rw-r--r--   0 hadfield   (501) staff       (20)      193 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasKey.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasListIndex.py
--rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasOntologyIRI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasOrganizationID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasPassword.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasPoolInitialSize.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasPoolMaxTotal.py
--rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasPreferredImportVersions.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasProvenance.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasQueryString.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasRdfContext.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasRdfObject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasRdfPredicate.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasRdfSubject.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasRepositoryName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasRootPath.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasSegmentID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasSelectQueries.py
--rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasSerializedJSON.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasSerializedRDF.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasServerURL.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasSessionID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasSessionType.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasSourceName.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasSourceUrl.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasTargetAppID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasTargetOrganizationID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasTimestamp.py
--rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasTransactionID.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasTransactionState.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasURIRef.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasUpdateTime.py
--rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasUpdatedRowsCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasUpdatedTriplesCount.py
--rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasUriGenerationStrategy.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasUsername.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasValue.py
--rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasVersionIRI.py
--rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_hasVersionInfo.py
--rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_isActive.py
--rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_isPositiveResponse.py
--rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_isPreferred.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_isPrimary.py
--rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_isReadOnly.py
--rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_types.py
--rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/Property_vitaltype.py
--rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/properties/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.249184 vital-ai-vitalsigns-0.1.9/
+-rw-r--r--   0 hadfield   (501) staff       (20)    11357 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.9/LICENSE
+-rw-r--r--   0 hadfield   (501) staff       (20)      707 2024-05-07 21:05:31.248950 vital-ai-vitalsigns-0.1.9/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)       25 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.9/README.md
+-rw-r--r--   0 hadfield   (501) staff       (20)       38 2024-05-07 21:05:31.249228 vital-ai-vitalsigns-0.1.9/setup.cfg
+-rw-r--r--   0 hadfield   (501) staff       (20)     1141 2024-05-07 21:05:20.000000 vital-ai-vitalsigns-0.1.9/setup.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.195421 vital-ai-vitalsigns-0.1.9/test/
+-rw-r--r--   0 hadfield   (501) staff       (20)      489 2024-05-02 22:13:47.000000 vital-ai-vitalsigns-0.1.9/test/test_embedding_model.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2254 2024-05-07 18:10:12.000000 vital-ai-vitalsigns-0.1.9/test/test_graph_collection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 17:51:38.000000 vital-ai-vitalsigns-0.1.9/test/test_package_discovery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2809 2024-05-07 18:01:11.000000 vital-ai-vitalsigns-0.1.9/test/test_query_builder.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.195780 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.197373 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/collection/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:00:36.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/collection/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)    11636 2024-05-07 18:14:44.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/collection/graph_collection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:49:20.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/collection/networkx_collection_impl.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1030 2024-05-03 21:08:09.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/collection/rdf_collection_impl.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1961 2024-05-07 18:29:23.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/collection/vector_collection_impl.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.197582 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/embedding/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:22:30.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/embedding/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2608 2024-05-07 14:39:23.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/embedding/embedding_model.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.198535 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/impl/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 18:25:32.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/impl/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2401 2024-05-07 13:32:41.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/impl/vitalsigns_impl.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      269 2024-03-19 17:21:02.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/impl/vitalsigns_package.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     5439 2024-05-07 13:01:47.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/impl/vitalsigns_registry.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.201727 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/
+-rw-r--r--   0 hadfield   (501) staff       (20)       47 2024-03-19 21:49:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/BaseDomainOntology.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     5214 2024-05-07 14:40:38.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/GraphObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1843 2024-05-04 18:11:27.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/VITAL_Edge.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      338 2024-03-17 20:11:18.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/VITAL_Edge.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1690 2024-05-04 18:13:01.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/VITAL_GraphContainerObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      310 2024-03-17 20:11:39.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/VITAL_GraphContainerObject.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1868 2024-05-04 18:13:13.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/VITAL_HyperEdge.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      354 2024-03-17 20:11:44.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/VITAL_HyperEdge.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1657 2024-05-04 18:13:26.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/VITAL_HyperNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      298 2024-03-17 20:11:51.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/VITAL_HyperNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1642 2024-05-04 18:11:50.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/VITAL_Node.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      294 2024-03-17 20:11:57.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/VITAL_Node.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.202040 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/classproperties/
+-rw-r--r--   0 hadfield   (501) staff       (20)      250 2024-05-03 23:34:11.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/classproperties/ClassProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-03 22:18:04.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/classproperties/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.202582 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/datatype/
+-rw-r--r--   0 hadfield   (501) staff       (20)      241 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/datatype/GeoLocation.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       23 2024-05-03 17:43:23.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/datatype/Truth.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/datatype/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.205805 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/
+-rw-r--r--   0 hadfield   (501) staff       (20)      549 2024-05-07 13:21:09.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/BooleanProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      741 2024-05-07 13:24:30.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/DateTimeProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      683 2024-05-07 13:27:08.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/DoubleProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      680 2024-05-07 13:27:16.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/FloatProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      552 2024-05-03 20:22:16.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/GeoLocationProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      897 2024-05-03 20:45:02.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/IProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      676 2024-05-07 13:28:26.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/IntegerProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      724 2024-05-07 13:28:37.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/LongProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      355 2024-05-03 20:22:44.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/MultiValueProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      446 2024-05-07 13:31:15.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/OtherProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      675 2024-05-07 13:30:16.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/StringProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      540 2024-05-03 20:26:30.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/TruthProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      669 2024-05-07 13:30:29.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/URIProperty.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.206152 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/trait/
+-rw-r--r--   0 hadfield   (501) staff       (20)      701 2024-05-07 13:02:48.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/trait/PropertyTrait.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-03-17 18:00:51.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/trait/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.208132 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/query/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:00:23.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/query/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      351 2024-05-03 22:16:06.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/query/property_constraint.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      293 2024-05-03 18:45:19.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/query/result_element.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      522 2024-05-03 18:46:27.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/query/result_list.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2456 2024-05-04 14:04:22.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/query/vital_graph_query.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      565 2024-05-04 14:04:22.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/query/vital_query.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      889 2024-05-04 14:12:47.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/query/vital_select_query.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.208540 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/query_impl/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:01:10.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/query_impl/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:02:54.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/query_impl/sparql_query_impl.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-01 15:03:29.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/query_impl/weaviate_vector_query_impl.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.209194 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/service/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:50:18.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/service/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       29 2024-05-07 17:57:40.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/service/base_service.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.209825 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/service/graph/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:52:56.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/service/graph/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:53:52.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/service/graph/graph_service.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:55:42.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/service/graph/name_graph.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:54:28.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/service/graph/virtuoso_service.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.210190 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/service/vector/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:52:44.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/service/vector/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:56:03.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/service/vector/vector_namespace.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:54:05.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/service/vector/vector_service.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:54:54.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/service/vector/weaviate_service.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:50:40.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/service/vital_segment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      109 2024-05-07 17:57:56.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/service/vital_service.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.210382 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/utils/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-02 19:19:42.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/utils/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)       30 2024-05-02 19:20:23.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/utils/uri_generator.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.210636 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-07 17:36:13.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.211072 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/client/
+-rw-r--r--   0 hadfield   (501) staff       (20)       61 2024-05-07 17:37:01.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/client/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     2832 2024-05-07 17:38:00.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/client/client.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.212203 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/db/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:15:12.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/db/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)    12405 2024-05-07 18:22:54.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/db/base.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.213064 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/db/executors/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:15:33.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/db/executors/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     5628 2024-05-07 18:21:44.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/db/executors/hnsw_indexer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     5762 2024-05-07 21:04:48.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/db/executors/inmemory_exact_indexer.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     4207 2024-05-07 17:31:35.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/db/executors/typed_executor.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      240 2024-05-07 17:29:49.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/db/hnsw_vectordb.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      276 2024-05-07 17:30:02.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/db/inmemory_exact_vectordb.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1600 2024-05-07 17:30:22.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/db/service.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.214521 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/utils/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-07 17:16:37.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/utils/__init__.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      850 2024-05-07 17:24:00.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/utils/create_doc_type.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      734 2024-05-07 17:23:28.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/utils/pass_parameters.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     4157 2024-05-07 17:38:56.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/utils/push_to_hubble.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1471 2024-05-07 17:22:19.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/utils/sort_matches_by_score.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1322 2024-05-07 17:22:38.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/utils/unify_input_output.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      894 2024-05-04 18:08:26.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vitalsigns.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.196575 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns.egg-info/
+-rw-r--r--   0 hadfield   (501) staff       (20)      707 2024-05-07 21:05:31.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns.egg-info/PKG-INFO
+-rw-r--r--   0 hadfield   (501) staff       (20)    15634 2024-05-07 21:05:31.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns.egg-info/SOURCES.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)        1 2024-05-07 21:05:31.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns.egg-info/dependency_links.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)      116 2024-05-07 21:05:31.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns.egg-info/entry_points.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       94 2024-05-07 21:05:31.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns.egg-info/requires.txt
+-rw-r--r--   0 hadfield   (501) staff       (20)       45 2024-05-07 21:05:31.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns.egg-info/top_level.txt
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.214659 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.236674 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/
+-rw-r--r--   0 hadfield   (501) staff       (20)     1476 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/AggregationResult.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/AggregationResult.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2083 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/DatabaseConnection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      309 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/DatabaseConnection.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1551 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Dataset.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      186 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Dataset.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/DomainModel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      360 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/DomainModel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/DomainOntology.py
+-rw-r--r--   0 hadfield   (501) staff       (20)     1273 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_SameAs.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_SameAs.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1285 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasApp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasApp.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasAuthKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasAuthKey.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasChildCategory.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasChildCategory.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasChildDomainModel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      149 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasChildDomainModel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1288 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasDbConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      141 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasDbConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasIndexConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      144 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasIndexConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasOrganization.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasOrganization.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1315 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasParentDomainModel.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      150 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasParentDomainModel.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1312 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasProvisioning.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      157 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasProvisioning.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasSegment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasSegment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1297 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasSession.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      152 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasSession.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1309 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasTransaction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      156 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasTransaction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1301 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/GraphMatch.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      166 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/GraphMatch.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1664 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/RDFStatement.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/RDFStatement.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1381 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SparqlAskResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      148 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SparqlAskResponse.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1310 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SparqlBinding.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      169 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SparqlBinding.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1531 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SparqlDatabaseConnection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      206 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SparqlDatabaseConnection.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1394 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SparqlUpdateResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      153 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SparqlUpdateResponse.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1414 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SqlDatabaseConnection.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SqlDatabaseConnection.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1307 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SqlResultRow.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      168 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SqlResultRow.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1382 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SqlUpdateResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      147 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SqlUpdateResponse.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1353 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/URIReference.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/URIReference.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_Category.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_Category.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1256 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_Event.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      119 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_Event.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1279 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_GraphQuery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      132 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_GraphQuery.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1276 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_PathQuery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      131 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_PathQuery.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1483 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_PayloadNode.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      172 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_PayloadNode.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1265 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_PeerEdge.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      122 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_PeerEdge.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1358 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_Query.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      136 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_Query.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1282 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_SelectQuery.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      133 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_SelectQuery.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1277 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_TaxonomyEdge.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      126 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_TaxonomyEdge.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1343 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalApp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      127 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalApp.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1353 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalAuthKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      129 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalAuthKey.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1379 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalOrganization.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      145 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalOrganization.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1274 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalProvisioning.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      125 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalProvisioning.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1458 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalSegment.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      158 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalSegment.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1294 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceAdminKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      139 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceAdminKey.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1951 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceAllegrographConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      305 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceAllegrographConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     2419 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      414 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1540 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceIndexedDBConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceIndexedDBConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1279 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      134 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceKey.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1435 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceLuceneDiskConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      179 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceLuceneDiskConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1342 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceLuceneMemoryConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      167 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceLuceneMemoryConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceMockConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceMockConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1423 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServicePrimeConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServicePrimeConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1291 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceRootKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      138 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceRootKey.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1318 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceSaaSConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      159 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceSaaSConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1423 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceSparkConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceSparkConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1923 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceSqlConfig.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      294 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceSqlConfig.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1555 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalSession.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      177 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalSession.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)     1482 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalTransaction.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      173 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalTransaction.pyi
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/__init__.py
+drwxr-xr-x   0 hadfield   (501) staff       (20)        0 2024-05-07 21:05:31.248621 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/
+-rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_URIProp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasAggregationType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasAppID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasBackwardCompVersion.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasCatalogName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasConfigString.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasConnectionError.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasConnectionState.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasDatabase.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasDateRetrieved.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasDbType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasDefaultPackageValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      223 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasDefaultSegmentName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasDomainOWL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasDomainOWLHash.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasEdgeDestination.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasEdgeSource.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasEndpointType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasEndpointURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasGraphQueries.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasHyperEdgeDestination.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasHyperEdgeSource.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      193 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasKey.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasListIndex.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      195 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasOntologyIRI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasOrganizationID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasPassword.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasPoolInitialSize.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasPoolMaxTotal.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      233 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasPreferredImportVersions.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasProvenance.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasQueryString.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasRdfContext.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasRdfObject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      211 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasRdfPredicate.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasRdfSubject.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasRepositoryName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasRootPath.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasSegmentID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasSelectQueries.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      215 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasSerializedJSON.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasSerializedRDF.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasServerURL.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasSessionID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasSessionType.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasSourceName.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasSourceUrl.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasTargetAppID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      227 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasTargetOrganizationID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      205 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasTimestamp.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      213 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasTransactionID.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasTransactionState.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasURIRef.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasUpdateTime.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      219 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasUpdatedRowsCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      225 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasUpdatedTriplesCount.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      229 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasUriGenerationStrategy.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasUsername.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasValue.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      207 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasVersionIRI.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      209 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_hasVersionInfo.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      197 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_isActive.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      217 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_isPositiveResponse.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      203 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_isPreferred.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_isPrimary.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      201 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_isReadOnly.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      191 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_types.py
+-rw-r--r--   0 hadfield   (501) staff       (20)      199 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/Property_vitaltype.py
+-rw-r--r--   0 hadfield   (501) staff       (20)        0 2024-05-04 17:21:21.000000 vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/properties/__init__.py
```

### Comparing `vital-ai-vitalsigns-0.1.8/LICENSE` & `vital-ai-vitalsigns-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/PKG-INFO` & `vital-ai-vitalsigns-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vital-ai-vitalsigns
-Version: 0.1.8
+Version: 0.1.9
 Summary: VitalSigns knowledge graph bindings
 Home-page: https://github.com/vital-ai/vital-vitalsigns-python
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `vital-ai-vitalsigns-0.1.8/setup.py` & `vital-ai-vitalsigns-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vital-ai-vitalsigns',
-    version='0.1.8',
+    version='0.1.9',
     author='Marc Hadfield',
     author_email='marc@vital.ai',
     description='VitalSigns knowledge graph bindings',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vital-ai/vital-vitalsigns-python',
     packages=find_packages(exclude=["test"]),
```

### Comparing `vital-ai-vitalsigns-0.1.8/test/test_graph_collection.py` & `vital-ai-vitalsigns-0.1.9/test/test_graph_collection.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/test/test_query_builder.py` & `vital-ai-vitalsigns-0.1.9/test/test_query_builder.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/collection/graph_collection.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/collection/graph_collection.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/collection/rdf_collection_impl.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/collection/rdf_collection_impl.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/collection/vector_collection_impl.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/collection/vector_collection_impl.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/embedding/embedding_model.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/embedding/embedding_model.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/impl/vitalsigns_impl.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/impl/vitalsigns_impl.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/impl/vitalsigns_registry.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/impl/vitalsigns_registry.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/GraphObject.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/GraphObject.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/VITAL_Edge.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/VITAL_Edge.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/VITAL_GraphContainerObject.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/VITAL_GraphContainerObject.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/VITAL_HyperEdge.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/VITAL_HyperEdge.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/VITAL_HyperNode.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/VITAL_HyperNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/VITAL_Node.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/VITAL_Node.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/BooleanProperty.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/BooleanProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/DateTimeProperty.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/DateTimeProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/DoubleProperty.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/DoubleProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/FloatProperty.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/FloatProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/GeoLocationProperty.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/GeoLocationProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/IProperty.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/IProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/IntegerProperty.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/IntegerProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/LongProperty.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/LongProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/StringProperty.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/StringProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/TruthProperty.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/TruthProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/properties/URIProperty.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/properties/URIProperty.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/model/trait/PropertyTrait.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/model/trait/PropertyTrait.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/query/result_list.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/query/result_list.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/query/vital_graph_query.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/query/vital_graph_query.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/query/vital_query.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/query/vital_query.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/query/vital_select_query.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/query/vital_select_query.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/client/client.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/client/client.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/db/base.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/db/base.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/db/executors/hnsw_indexer.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/db/executors/hnsw_indexer.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/db/executors/inmemory_exact_indexer.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/db/executors/inmemory_exact_indexer.py`

 * *Files 12% similar despite different names*

```diff
@@ -63,27 +63,54 @@
         params = parameters or {}
         if '__results__' in params:
             params.pop('__results__')
 
         if class_uri is None:
             ret = self._indexer.find_batched(docs, search_field=search_field, **params)
         else:
-            filtered = self._indexer.filter(
-                filter_query={'ClassURI': {'$eq': class_uri}},
-                limit=self._indexer.num_docs())
-            ret = self._indexer.find_batched(filtered, search_field=search_field, **params)
+            # filtered = self._indexer.filter(
+            #    filter_query={'ClassURI': {'$eq': class_uri}},
+            #    limit=self._indexer.num_docs())
 
+            # this is not a batch case
+            query = (self._indexer.build_query()
+                     .filter(filter_query={'ClassURI': {'$eq': class_uri}})
+                     .find(query=docs[0], search_field=search_field, limit=1000)
+                     .build())
+
+            # ret = self._indexer.find_batched(docs, search_field=search_field, **params)
+
+            ret = self._indexer.execute_query(query)
+            # self.logger.info(f'Results {ret}')
+
+            # for d in ret:
+            #    self.logger.info(f'{d}')
+
+            matched_documents = ret.documents
+            matched_scores = ret.scores
+
+            output_doc = self._output_schema(**docs[0].dict())
+            output_doc.matches = matched_documents
+            output_doc.scores = matched_scores
+            res.append(output_doc)
+            return res
+
+        # batch case
         matched_documents = ret.documents
         matched_scores = ret.scores
 
         # not true for filtered?
         # assert len(docs) == len(matched_documents) == len(matched_scores)
 
         for query, matches, scores in zip(docs, matched_documents, matched_scores):
             output_doc = self._output_schema(**query.dict())
+            # self.logger.info(f'{query}')
+            # self.logger.info(f'{matches}')
+            # self.logger.info(f'{scores}')
+
             output_doc.matches = matches
             output_doc.scores = scores.tolist()
             res.append(output_doc)
         return res
 
     @requests(on='/search')
     def search(self, docs, *args, **kwargs):
```

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/db/executors/typed_executor.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/db/executors/typed_executor.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/db/service.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/db/service.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/utils/create_doc_type.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/utils/create_doc_type.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/utils/pass_parameters.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/utils/pass_parameters.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/utils/push_to_hubble.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/utils/push_to_hubble.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/utils/sort_matches_by_score.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/utils/sort_matches_by_score.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vectordb/utils/unify_input_output.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vectordb/utils/unify_input_output.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns/vitalsigns.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns/vitalsigns.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns.egg-info/PKG-INFO` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vital-ai-vitalsigns
-Version: 0.1.8
+Version: 0.1.9
 Summary: VitalSigns knowledge graph bindings
 Home-page: https://github.com/vital-ai/vital-vitalsigns-python
 Author: Marc Hadfield
 Author-email: marc@vital.ai
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns.egg-info/SOURCES.txt` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/AggregationResult.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/AggregationResult.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/DatabaseConnection.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/DatabaseConnection.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Dataset.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Dataset.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/DomainModel.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/DomainModel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_SameAs.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_SameAs.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasApp.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasApp.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasAuthKey.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasAuthKey.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasChildCategory.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasChildCategory.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasChildDomainModel.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasChildDomainModel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasDbConfig.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasDbConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasIndexConfig.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasIndexConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasOrganization.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasOrganization.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasParentDomainModel.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasParentDomainModel.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasProvisioning.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasProvisioning.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasSegment.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasSegment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasSession.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasSession.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/Edge_hasTransaction.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/Edge_hasTransaction.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/GraphMatch.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/GraphMatch.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/RDFStatement.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/RDFStatement.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SparqlAskResponse.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SparqlAskResponse.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SparqlBinding.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SparqlBinding.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SparqlDatabaseConnection.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SparqlDatabaseConnection.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SparqlUpdateResponse.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SparqlUpdateResponse.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SqlDatabaseConnection.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SqlDatabaseConnection.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SqlResultRow.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SqlResultRow.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/SqlUpdateResponse.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/SqlUpdateResponse.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/URIReference.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/URIReference.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_Category.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_Category.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_Event.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_Event.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_GraphQuery.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_GraphQuery.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_PathQuery.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_PathQuery.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_PayloadNode.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_PayloadNode.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_PeerEdge.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_PeerEdge.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_Query.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_Query.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_SelectQuery.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_SelectQuery.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VITAL_TaxonomyEdge.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VITAL_TaxonomyEdge.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalApp.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalApp.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalAuthKey.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalAuthKey.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalOrganization.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalOrganization.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalProvisioning.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalProvisioning.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalSegment.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalSegment.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceAdminKey.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceAdminKey.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceAllegrographConfig.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceAllegrographConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceConfig.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceIndexedDBConfig.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceIndexedDBConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceKey.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceKey.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceLuceneDiskConfig.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceLuceneDiskConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceLuceneMemoryConfig.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceLuceneMemoryConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceMockConfig.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceMockConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServicePrimeConfig.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServicePrimeConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceRootKey.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceRootKey.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceSaaSConfig.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceSaaSConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceSparkConfig.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceSparkConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalServiceSqlConfig.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalServiceSqlConfig.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalSession.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalSession.py`

 * *Files identical despite different names*

### Comparing `vital-ai-vitalsigns-0.1.8/vital_ai_vitalsigns_core/model/VitalTransaction.py` & `vital-ai-vitalsigns-0.1.9/vital_ai_vitalsigns_core/model/VitalTransaction.py`

 * *Files identical despite different names*

