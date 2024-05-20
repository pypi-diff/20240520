# Comparing `tmp/superlinked-3.9.1.tar.gz` & `tmp/superlinked-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superlinked-3.9.1.tar", max compression
+gzip compressed data, was "superlinked-4.0.1.tar", max compression
```

## Comparing `superlinked-3.9.1.tar` & `superlinked-4.0.1.tar`

### file list

```diff
@@ -1,171 +1,228 @@
--rw-r--r--   0        0        0    11354 2024-03-20 12:30:06.973285 superlinked-3.9.1/LICENSE
--rw-r--r--   0        0        0    28655 2024-03-20 12:30:06.973285 superlinked-3.9.1/NOTICE
--rw-r--r--   0        0        0     6382 2024-03-20 12:30:06.973285 superlinked-3.9.1/PYPI_README.md
--rw-r--r--   0        0        0     5333 2024-03-20 12:32:07.438558 superlinked-3.9.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/__init__.py
--rw-r--r--   0        0        0     5228 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/evaluation/charts/recency_plotter.py
--rw-r--r--   0        0        0     5593 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/evaluation/vector_sampler.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/calculation/__init__.py
--rw-r--r--   0        0        0     1410 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/calculation/vector_similarity.py
--rw-r--r--   0        0        0      682 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/const.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/__init__.py
--rw-r--r--   0        0        0     3270 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/aggregation_node.py
--rw-r--r--   0        0        0      940 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/chunking_node.py
--rw-r--r--   0        0        0     1857 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/comparison_filter_node.py
--rw-r--r--   0        0        0     2431 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/concatenation_node.py
--rw-r--r--   0        0        0      890 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/constant_node.py
--rw-r--r--   0        0        0     4571 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/context.py
--rw-r--r--   0        0        0     5016 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/dag.py
--rw-r--r--   0        0        0     1242 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/dag_effect.py
--rw-r--r--   0        0        0     3149 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/event_aggregation_node.py
--rw-r--r--   0        0        0      945 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/exception.py
--rw-r--r--   0        0        0     1795 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/index_node.py
--rw-r--r--   0        0        0     1119 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/named_function_node.py
--rw-r--r--   0        0        0     3263 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/node.py
--rw-r--r--   0        0        0     1313 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/number_embedding_node.py
--rw-r--r--   0        0        0     1331 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/number_similarity_node.py
--rw-r--r--   0        0        0     1818 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/period_time.py
--rw-r--r--   0        0        0      897 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/persistence_params.py
--rw-r--r--   0        0        0     1403 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/recency_node.py
--rw-r--r--   0        0        0     1015 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/resolved_schema_reference.py
--rw-r--r--   0        0        0     2019 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/schema_dag.py
--rw-r--r--   0        0        0     1111 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/schema_field_node.py
--rw-r--r--   0        0        0     1241 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/schema_object_reference.py
--rw-r--r--   0        0        0     1329 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/dag/text_embedding_node.py
--rw-r--r--   0        0        0     4120 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/data_types.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/embedding/__init__.py
--rw-r--r--   0        0        0     5317 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/embedding/chunking_util.py
--rw-r--r--   0        0        0     1850 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/embedding/number_embedding.py
--rw-r--r--   0        0        0     1848 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/embedding/number_similarity_embedding.py
--rw-r--r--   0        0        0     4364 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/embedding/recency_embedding.py
--rw-r--r--   0        0        0     1274 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/embedding/sentence_transformer_embedding.py
--rw-r--r--   0        0        0     1143 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/exception.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/interface/__init__.py
--rw-r--r--   0        0        0     5715 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/interface/comparison_operand.py
--rw-r--r--   0        0        0      841 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/interface/comparison_operation_type.py
--rw-r--r--   0        0        0      718 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/interface/has_length.py
--rw-r--r--   0        0        0      836 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/interface/has_multiplier.py
--rw-r--r--   0        0        0      825 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/interface/weighted.py
--rw-r--r--   0        0        0     1307 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/observable.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/parser/__init__.py
--rw-r--r--   0        0        0     5873 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/parser/data_parser.py
--rw-r--r--   0        0        0     4800 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/parser/dataframe_parser.py
--rw-r--r--   0        0        0      814 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/parser/exception.py
--rw-r--r--   0        0        0     4379 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/parser/json_parser.py
--rw-r--r--   0        0        0     1354 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/parser/parsed_schema.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/__init__.py
--rw-r--r--   0        0        0     1072 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/event_schema.py
--rw-r--r--   0        0        0     1964 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/event_schema_object.py
--rw-r--r--   0        0        0     1014 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/exception.py
--rw-r--r--   0        0        0      627 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/general_type.py
--rw-r--r--   0        0        0     1392 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/id_schema_object.py
--rw-r--r--   0        0        0     1178 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/schema.py
--rw-r--r--   0        0        0     3147 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/schema_decorator.py
--rw-r--r--   0        0        0     3209 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/schema_factory.py
--rw-r--r--   0        0        0     4804 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/schema_object.py
--rw-r--r--   0        0        0     2962 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/schema_reference.py
--rw-r--r--   0        0        0      686 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/schema_type.py
--rw-r--r--   0        0        0     3201 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/schema/schema_validator.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/source/__init__.py
--rw-r--r--   0        0        0      857 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/source/source.py
--rw-r--r--   0        0        0      647 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/source/types.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/storage/__init__.py
--rw-r--r--   0        0        0      683 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/storage/persistence_type.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.025286 superlinked-3.9.1/superlinked/framework/common/util/__init__.py
--rw-r--r--   0        0        0     2591 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/common/util/class_helper.py
--rw-r--r--   0        0        0     2074 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/common/util/dot_separated_path_util.py
--rw-r--r--   0        0        0      707 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/common/util/immutable_model.py
--rw-r--r--   0        0        0     1058 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/common/util/named_function_evaluator.py
--rw-r--r--   0        0        0      886 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/common/util/schema_util.py
--rw-r--r--   0        0        0      907 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/common/util/time_util.py
--rw-r--r--   0        0        0     4383 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/common/util/type_validator.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/compiler/__init__.py
--rw-r--r--   0        0        0     3305 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/compiler/online_schema_dag_compiler.py
--rw-r--r--   0        0        0      108 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/__init__.py
--rw-r--r--   0        0        0      221 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/__init__.py
--rw-r--r--   0        0        0      719 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/exception.py
--rw-r--r--   0        0        0     4378 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/executor.py
--rw-r--r--   0        0        0      124 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/in_memory/__init__.py
--rw-r--r--   0        0        0     6524 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py
--rw-r--r--   0        0        0      119 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/query/__init__.py
--rw-r--r--   0        0        0     5732 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/query/query_executor.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/rest/__init__.py
--rw-r--r--   0        0        0     1532 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/rest/rest_configuration.py
--rw-r--r--   0        0        0      818 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/rest/rest_descriptor.py
--rw-r--r--   0        0        0     4110 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/rest/rest_executor.py
--rw-r--r--   0        0        0     3236 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/executor/rest/rest_handler.py
--rw-r--r--   0        0        0      176 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/index/__init__.py
--rw-r--r--   0        0        0     1776 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/index/effect.py
--rw-r--r--   0        0        0    10209 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/index/index.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/index/util/__init__.py
--rw-r--r--   0        0        0     1516 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/index/util/aggregation_effect_group.py
--rw-r--r--   0        0        0     2448 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/index/util/aggregation_node_util.py
--rw-r--r--   0        0        0     6203 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py
--rw-r--r--   0        0        0     2557 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py
--rw-r--r--   0        0        0     3673 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/index/util/event_aggregation_node_util.py
--rw-r--r--   0        0        0      192 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/__init__.py
--rw-r--r--   0        0        0     1137 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/param.py
--rw-r--r--   0        0        0     2772 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/param_evaluator.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/predicate/__init__.py
--rw-r--r--   0        0        0      756 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/predicate/binary_op.py
--rw-r--r--   0        0        0     1517 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/predicate/binary_predicate.py
--rw-r--r--   0        0        0      924 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py
--rw-r--r--   0        0        0     1124 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/predicate/query_predicate.py
--rw-r--r--   0        0        0    11202 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/query.py
--rw-r--r--   0        0        0     6223 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/query_filters.py
--rw-r--r--   0        0        0     7954 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/query_vector_factory.py
--rw-r--r--   0        0        0     3329 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/query_weighting.py
--rw-r--r--   0        0        0     1890 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/query/result.py
--rw-r--r--   0        0        0      213 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/source/__init__.py
--rw-r--r--   0        0        0     2773 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/source/in_memory_source.py
--rw-r--r--   0        0        0     1987 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/source/rest_source.py
--rw-r--r--   0        0        0     1144 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/source/source.py
--rw-r--r--   0        0        0      183 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/space/__init__.py
--rw-r--r--   0        0        0      781 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/space/exception.py
--rw-r--r--   0        0        0     8004 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/space/number_space.py
--rw-r--r--   0        0        0     7301 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/space/recency_space.py
--rw-r--r--   0        0        0     2218 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/space/space.py
--rw-r--r--   0        0        0     1275 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/space/space_field_set.py
--rw-r--r--   0        0        0     4414 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/dsl/space/text_similarity_space.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/evaluator/__init__.py
--rw-r--r--   0        0        0     1016 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/evaluator/dag_evaluator.py
--rw-r--r--   0        0        0     4650 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/evaluator/online_dag_evaluator.py
--rw-r--r--   0        0        0     2278 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/evaluator/query_dag_evaluator.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/__init__.py
--rw-r--r--   0        0        0     4791 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/default_online_node.py
--rw-r--r--   0        0        0     1129 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/evaluation_result.py
--rw-r--r--   0        0        0      831 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/exception.py
--rw-r--r--   0        0        0     5312 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_aggregation_node.py
--rw-r--r--   0        0        0     3825 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_chunking_node.py
--rw-r--r--   0        0        0     2528 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_comparison_filter_node.py
--rw-r--r--   0        0        0     5093 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_concatenation_node.py
--rw-r--r--   0        0        0     2209 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_constant_node.py
--rw-r--r--   0        0        0     8871 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_event_aggregation_node.py
--rw-r--r--   0        0        0     3927 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_index_node.py
--rw-r--r--   0        0        0     2506 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_named_function_node.py
--rw-r--r--   0        0        0     3821 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_node.py
--rw-r--r--   0        0        0     3840 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_number_embedding_node.py
--rw-r--r--   0        0        0     3725 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_number_similarity_node.py
--rw-r--r--   0        0        0     2877 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_recency_node.py
--rw-r--r--   0        0        0     3718 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_schema_dag.py
--rw-r--r--   0        0        0     3609 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_schema_field_node.py
--rw-r--r--   0        0        0     2530 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/dag/online_text_embedding_node.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/source/__init__.py
--rw-r--r--   0        0        0     3313 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/source/in_memory_data_processor.py
--rw-r--r--   0        0        0     1479 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/source/in_memory_object_writer.py
--rw-r--r--   0        0        0     1549 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/source/in_memory_source.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/store_manager/__init__.py
--rw-r--r--   0        0        0     5813 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/online/store_manager/evaluation_result_store_manager.py
--rw-r--r--   0        0        0        0 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/storage/__init__.py
--rw-r--r--   0        0        0     2512 2024-03-20 12:30:07.029286 superlinked-3.9.1/superlinked/framework/storage/entity.py
--rw-r--r--   0        0        0     1936 2024-03-20 12:30:07.033286 superlinked-3.9.1/superlinked/framework/storage/entity_store.py
--rw-r--r--   0        0        0     4750 2024-03-20 12:30:07.033286 superlinked-3.9.1/superlinked/framework/storage/entity_store_manager.py
--rw-r--r--   0        0        0     1304 2024-03-20 12:30:07.033286 superlinked-3.9.1/superlinked/framework/storage/field.py
--rw-r--r--   0        0        0     7925 2024-03-20 12:30:07.033286 superlinked-3.9.1/superlinked/framework/storage/in_memory_entity_store.py
--rw-r--r--   0        0        0     1126 2024-03-20 12:30:07.033286 superlinked-3.9.1/superlinked/framework/storage/in_memory_object_store.py
--rw-r--r--   0        0        0     1125 2024-03-20 12:30:07.033286 superlinked-3.9.1/superlinked/framework/storage/object_store.py
--rw-r--r--   0        0        0     1570 2024-03-20 12:30:07.033286 superlinked-3.9.1/superlinked/framework/storage/object_store_manager.py
--rw-r--r--   0        0        0     9446 1970-01-01 00:00:00.000000 superlinked-3.9.1/PKG-INFO
+-rw-r--r--   0        0        0    11354 2024-05-20 11:16:57.453673 superlinked-4.0.1/LICENSE
+-rw-r--r--   0        0        0    28655 2024-05-20 11:16:57.453673 superlinked-4.0.1/NOTICE
+-rw-r--r--   0        0        0     6840 2024-05-20 11:16:57.453673 superlinked-4.0.1/PYPI_README.md
+-rw-r--r--   0        0        0     3698 2024-05-20 11:20:02.165106 superlinked-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/evaluation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/evaluation/charts/__init__.py
+-rw-r--r--   0        0        0     5601 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/evaluation/charts/recency_plotter.py
+-rw-r--r--   0        0        0     8077 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/evaluation/vector_sampler.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/calculation/__init__.py
+-rw-r--r--   0        0        0      742 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/calculation/distance_metric.py
+-rw-r--r--   0        0        0     1621 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/calculation/vector_similarity.py
+-rw-r--r--   0        0        0      805 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/const.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/__init__.py
+-rw-r--r--   0        0        0     3624 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/aggregation_node.py
+-rw-r--r--   0        0        0     2280 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/categorical_similarity_node.py
+-rw-r--r--   0        0        0     1515 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/chunking_node.py
+-rw-r--r--   0        0        0     2089 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/comparison_filter_node.py
+-rw-r--r--   0        0        0     2586 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/concatenation_node.py
+-rw-r--r--   0        0        0     1093 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/constant_node.py
+-rw-r--r--   0        0        0     4985 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/context.py
+-rw-r--r--   0        0        0     1846 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/custom_node.py
+-rw-r--r--   0        0        0     5923 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/dag.py
+-rw-r--r--   0        0        0     1338 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/dag_effect.py
+-rw-r--r--   0        0        0     3664 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/event_aggregation_node.py
+-rw-r--r--   0        0        0     1004 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/exception.py
+-rw-r--r--   0        0        0     2023 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/index_node.py
+-rw-r--r--   0        0        0     1415 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/named_function_node.py
+-rw-r--r--   0        0        0     4465 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/node.py
+-rw-r--r--   0        0        0     2414 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/number_embedding_node.py
+-rw-r--r--   0        0        0     2368 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/number_similarity_node.py
+-rw-r--r--   0        0        0     1620 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/period_time.py
+-rw-r--r--   0        0        0      897 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/persistence_params.py
+-rw-r--r--   0        0        0     2449 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/recency_node.py
+-rw-r--r--   0        0        0     1128 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/resolved_schema_reference.py
+-rw-r--r--   0        0        0     2019 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/schema_dag.py
+-rw-r--r--   0        0        0     1384 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/schema_field_node.py
+-rw-r--r--   0        0        0     1378 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/schema_object_reference.py
+-rw-r--r--   0        0        0     2062 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/dag/text_embedding_node.py
+-rw-r--r--   0        0        0     8036 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/data_types.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/embedding/__init__.py
+-rw-r--r--   0        0        0     5281 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/embedding/categorical_similarity_embedding.py
+-rw-r--r--   0        0        0     5890 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/embedding/chunking_util.py
+-rw-r--r--   0        0        0     1576 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/embedding/custom_embedding.py
+-rw-r--r--   0        0        0     1280 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/embedding/embedding.py
+-rw-r--r--   0        0        0     3138 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/embedding/number_embedding.py
+-rw-r--r--   0        0        0     2383 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/embedding/number_similarity_embedding.py
+-rw-r--r--   0        0        0     7995 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/embedding/recency_embedding.py
+-rw-r--r--   0        0        0     2134 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/embedding/sentence_transformer_embedding.py
+-rw-r--r--   0        0        0     1250 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/exception.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/interface/__init__.py
+-rw-r--r--   0        0        0     5851 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/interface/comparison_operand.py
+-rw-r--r--   0        0        0      841 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/interface/comparison_operation_type.py
+-rw-r--r--   0        0        0      808 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/interface/has_aggregation.py
+-rw-r--r--   0        0        0      718 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/interface/has_length.py
+-rw-r--r--   0        0        0      836 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/interface/has_multiplier.py
+-rw-r--r--   0        0        0      940 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/interface/weighted.py
+-rw-r--r--   0        0        0     1322 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/observable.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/parser/__init__.py
+-rw-r--r--   0        0        0     5879 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/parser/data_parser.py
+-rw-r--r--   0        0        0     4806 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/parser/dataframe_parser.py
+-rw-r--r--   0        0        0      814 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/parser/exception.py
+-rw-r--r--   0        0        0     4379 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/parser/json_parser.py
+-rw-r--r--   0        0        0     1354 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/parser/parsed_schema.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/__init__.py
+-rw-r--r--   0        0        0     1072 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/event_schema.py
+-rw-r--r--   0        0        0     1964 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/event_schema_object.py
+-rw-r--r--   0        0        0     1014 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/exception.py
+-rw-r--r--   0        0        0      627 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/general_type.py
+-rw-r--r--   0        0        0     1392 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/id_schema_object.py
+-rw-r--r--   0        0        0     1178 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/schema.py
+-rw-r--r--   0        0        0     3189 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/schema_decorator.py
+-rw-r--r--   0        0        0     3209 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/schema_factory.py
+-rw-r--r--   0        0        0     5687 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/schema_object.py
+-rw-r--r--   0        0        0     3170 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/schema_reference.py
+-rw-r--r--   0        0        0      686 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/schema_type.py
+-rw-r--r--   0        0        0     3201 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/schema/schema_validator.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.497673 superlinked-4.0.1/superlinked/framework/common/source/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/source/source.py
+-rw-r--r--   0        0        0      647 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/source/types.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/space/__init__.py
+-rw-r--r--   0        0        0     4398 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/space/aggregation.py
+-rw-r--r--   0        0        0     2121 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/space/normalization.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/entity.py
+-rw-r--r--   0        0        0      878 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/entity_data.py
+-rw-r--r--   0        0        0      696 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/entity_id.py
+-rw-r--r--   0        0        0      627 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/exception.py
+-rw-r--r--   0        0        0     1516 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/field.py
+-rw-r--r--   0        0        0     2535 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/field_data.py
+-rw-r--r--   0        0        0      733 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/field_data_type.py
+-rw-r--r--   0        0        0     3213 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/field_encoder.py
+-rw-r--r--   0        0        0      746 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/persistence_type.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/search_index_creation/__init__.py
+-rw-r--r--   0        0        0     1216 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/search_index_creation/index_field_descriptor.py
+-rw-r--r--   0        0        0      671 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/search_index_creation/search_algorithm.py
+-rw-r--r--   0        0        0      692 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/search_index_creation/vector_component_precision.py
+-rw-r--r--   0        0        0     2306 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/vdb_connector.py
+-rw-r--r--   0        0        0     1075 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage/vdb_knn_search_params.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage_manager/__init__.py
+-rw-r--r--   0        0        0     6065 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage_manager/entity_builder.py
+-rw-r--r--   0        0        0     2143 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage_manager/field_type_converter.py
+-rw-r--r--   0        0        0     1059 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage_manager/knn_search_params.py
+-rw-r--r--   0        0        0      769 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage_manager/node_result_params.py
+-rw-r--r--   0        0        0    13379 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage_manager/storage_manager.py
+-rw-r--r--   0        0        0     1462 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/storage_manager/storage_naming.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/collection_util.py
+-rw-r--r--   0        0        0     2074 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/dot_separated_path_util.py
+-rw-r--r--   0        0        0      707 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/immutable_model.py
+-rw-r--r--   0        0        0     1058 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/named_function_evaluator.py
+-rw-r--r--   0        0        0      886 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/schema_util.py
+-rw-r--r--   0        0        0     1642 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/string_util.py
+-rw-r--r--   0        0        0      907 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/time_util.py
+-rw-r--r--   0        0        0     1189 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/type_util.py
+-rw-r--r--   0        0        0     4383 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/common/util/type_validator.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/compiler/__init__.py
+-rw-r--r--   0        0        0     2556 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/compiler/online_schema_dag_compiler.py
+-rw-r--r--   0        0        0      108 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/data_loader/__init__.py
+-rw-r--r--   0        0        0      726 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/data_loader/data_loader.py
+-rw-r--r--   0        0        0      221 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/__init__.py
+-rw-r--r--   0        0        0      719 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/exception.py
+-rw-r--r--   0        0        0     4281 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/executor.py
+-rw-r--r--   0        0        0      124 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/in_memory/__init__.py
+-rw-r--r--   0        0        0     7300 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py
+-rw-r--r--   0        0        0      119 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/query/__init__.py
+-rw-r--r--   0        0        0     6478 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/query/query_executor.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/rest/__init__.py
+-rw-r--r--   0        0        0     1540 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/rest/rest_configuration.py
+-rw-r--r--   0        0        0      818 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/rest/rest_descriptor.py
+-rw-r--r--   0        0        0     4395 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/rest/rest_executor.py
+-rw-r--r--   0        0        0     3236 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/executor/rest/rest_handler.py
+-rw-r--r--   0        0        0      176 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/index/__init__.py
+-rw-r--r--   0        0        0     1904 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/index/effect.py
+-rw-r--r--   0        0        0    10985 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/index/index.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/index/util/__init__.py
+-rw-r--r--   0        0        0     1516 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/index/util/aggregation_effect_group.py
+-rw-r--r--   0        0        0     2448 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/index/util/aggregation_node_util.py
+-rw-r--r--   0        0        0     6203 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py
+-rw-r--r--   0        0        0     2557 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py
+-rw-r--r--   0        0        0     3673 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/index/util/event_aggregation_node_util.py
+-rw-r--r--   0        0        0      192 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/__init__.py
+-rw-r--r--   0        0        0     1183 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/param.py
+-rw-r--r--   0        0        0     3798 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/param_evaluator.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/predicate/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/predicate/binary_op.py
+-rw-r--r--   0        0        0     1521 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/predicate/binary_predicate.py
+-rw-r--r--   0        0        0      924 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py
+-rw-r--r--   0        0        0     1128 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/predicate/query_predicate.py
+-rw-r--r--   0        0        0    13173 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/query.py
+-rw-r--r--   0        0        0     6223 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/query_filters.py
+-rw-r--r--   0        0        0     6990 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/query_vector_factory.py
+-rw-r--r--   0        0        0     3329 2024-05-20 11:16:57.501673 superlinked-4.0.1/superlinked/framework/dsl/query/query_weighting.py
+-rw-r--r--   0        0        0     2457 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/query/result.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/registry/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/registry/exception.py
+-rw-r--r--   0        0        0     1984 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/registry/superlinked_registry.py
+-rw-r--r--   0        0        0      214 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/source/__init__.py
+-rw-r--r--   0        0        0     2773 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/source/in_memory_source.py
+-rw-r--r--   0        0        0     1987 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/source/rest_source.py
+-rw-r--r--   0        0        0     1144 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/source/source.py
+-rw-r--r--   0        0        0      183 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/space/__init__.py
+-rw-r--r--   0        0        0     7539 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/space/categorical_similarity_space.py
+-rw-r--r--   0        0        0     5569 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/space/custom_space.py
+-rw-r--r--   0        0        0      856 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/space/exception.py
+-rw-r--r--   0        0        0     8215 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/space/number_space.py
+-rw-r--r--   0        0        0     8516 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/space/recency_space.py
+-rw-r--r--   0        0        0     2732 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/space/space.py
+-rw-r--r--   0        0        0     1275 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/space/space_field_set.py
+-rw-r--r--   0        0        0     4804 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/dsl/space/text_similarity_space.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/evaluator/__init__.py
+-rw-r--r--   0        0        0     1043 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/evaluator/dag_evaluator.py
+-rw-r--r--   0        0        0     5222 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/evaluator/online_dag_evaluator.py
+-rw-r--r--   0        0        0     2237 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/evaluator/query_dag_evaluator.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/new_storage/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/new_storage/in_memory/__init__.py
+-rw-r--r--   0        0        0      787 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/new_storage/in_memory/exception.py
+-rw-r--r--   0        0        0     6127 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/new_storage/in_memory/in_memory_knn_search.py
+-rw-r--r--   0        0        0     6408 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/new_storage/in_memory/in_memory_vdb.py
+-rw-r--r--   0        0        0      921 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/new_storage/in_memory/index_config.py
+-rw-r--r--   0        0        0     1305 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/new_storage/in_memory/json_codec.py
+-rw-r--r--   0        0        0     1562 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/new_storage/in_memory/object_serializer.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/__init__.py
+-rw-r--r--   0        0        0      801 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/batched_chunk_input_item.py
+-rw-r--r--   0        0        0     7597 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/default_online_node.py
+-rw-r--r--   0        0        0     1129 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/evaluation_result.py
+-rw-r--r--   0        0        0      768 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/exception.py
+-rw-r--r--   0        0        0     6395 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_aggregation_node.py
+-rw-r--r--   0        0        0     3288 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_categorical_similarity_node.py
+-rw-r--r--   0        0        0     3540 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_chunking_node.py
+-rw-r--r--   0        0        0     2330 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_comparison_filter_node.py
+-rw-r--r--   0        0        0     5148 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_concatenation_node.py
+-rw-r--r--   0        0        0     2115 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_constant_node.py
+-rw-r--r--   0        0        0     3435 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_custom_node.py
+-rw-r--r--   0        0        0     8157 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_event_aggregation_node.py
+-rw-r--r--   0        0        0     4135 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_index_node.py
+-rw-r--r--   0        0        0     2434 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_named_function_node.py
+-rw-r--r--   0        0        0     4996 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_node.py
+-rw-r--r--   0        0        0     5773 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_node_registry.py
+-rw-r--r--   0        0        0     3162 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_number_embedding_node.py
+-rw-r--r--   0        0        0     3272 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_number_similarity_node.py
+-rw-r--r--   0        0        0     2796 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_recency_node.py
+-rw-r--r--   0        0        0     3732 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_schema_dag.py
+-rw-r--r--   0        0        0     3509 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_schema_field_node.py
+-rw-r--r--   0        0        0     3338 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/online_text_embedding_node.py
+-rw-r--r--   0        0        0      794 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/parent_results.py
+-rw-r--r--   0        0        0     1322 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/dag/parent_validator.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/source/__init__.py
+-rw-r--r--   0        0        0     3486 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/source/in_memory_data_processor.py
+-rw-r--r--   0        0        0     1539 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/source/in_memory_object_writer.py
+-rw-r--r--   0        0        0     1752 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/source/in_memory_source.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/store_manager/__init__.py
+-rw-r--r--   0        0        0     5707 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/online/store_manager/evaluation_result_store_manager.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/__init__.py
+-rw-r--r--   0        0        0     2587 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/entity.py
+-rw-r--r--   0        0        0     1936 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/entity_store.py
+-rw-r--r--   0        0        0     4966 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/entity_store_manager.py
+-rw-r--r--   0        0        0     1304 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/field.py
+-rw-r--r--   0        0        0     8076 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/in_memory_entity_store.py
+-rw-r--r--   0        0        0     1209 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/in_memory_object_store.py
+-rw-r--r--   0        0        0     1125 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/object_store.py
+-rw-r--r--   0        0        0     1570 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/object_store_manager.py
+-rw-r--r--   0        0        0     3317 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/framework/storage/persistable_dict.py
+-rw-r--r--   0        0        0        0 2024-05-20 11:16:57.505673 superlinked-4.0.1/superlinked/py.typed
+-rw-r--r--   0        0        0     8320 1970-01-01 00:00:00.000000 superlinked-4.0.1/PKG-INFO
```

### Comparing `superlinked-3.9.1/LICENSE` & `superlinked-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/NOTICE` & `superlinked-4.0.1/NOTICE`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/PYPI_README.md` & `superlinked-4.0.1/PYPI_README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,55 +1,36 @@
 # Superlinked 
 
-Superlinked is a declarative Python SDK that enables you to turn complex data into vectors, in a way that fits the modern data stack and works with your favorite Vector Databases.
+Superlinked is a compute framework for your information retrieval and feature engineering systems, focused on turning complex data into vector embeddings within your RAG, Search, RecSys and Analytics stack.
 
-3 key areas of focus:
-
-1. Custom embedding model creation that fits your complex data entities.
-1. ETL for your vector index for both streaming and batch use-cases.
-1. Vector-native query language that helps you convert hybrid search queries to pure vector queries.
+Our current release allows you to explore our computational model in simple scripts and python notebooks, our next major release will focus on helping you run Superlinked in production, with built-in data infra and vector database integrations.
 
 Visit [Superlinked](https://superlinked.com/) for more information about the company behind this product and our other initiatives.
 
-## Use-cases
-
-- **RAG**: [HR Knowledgebase](https://github.com/superlinked/superlinked/blob/main/notebook/rag_hr_knowledgebase.ipynb)
-- **Semantic Search**: [Movie Recommendations](https://github.com/superlinked/superlinked/blob/main/notebook/semantic_search_netflix_titles.ipynb), [Business News](https://github.com/superlinked/superlinked/blob/main/notebook/semantic_search_news.ipynb)
-- **Recommendation Systems**: [E-commerce](https://github.com/superlinked/superlinked/blob/main/notebook/recommendations_e_commerce.ipynb)
-- **Analytics**: [User Acquisition](https://github.com/superlinked/superlinked/blob/main/notebook/analytics_user_acquisition.ipynb)
-
-You can check a full list of examples [here](https://github.com/superlinked/superlinked/tree/main/notebook).
+If you like what we do, give us a star! ⭐
 
-## Reference
+The screenshot below shows how to build multimodal vectors from your data & define weights at query time to avoid postprocessing & rerank requirements.
 
-1. Describe your data using Python classes with the [@schema](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/common/schema/schema.md) decorator.
-2. Describe your vector embeddings from building blocks with [Spaces](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/space/index.md).
-3. Combine your embeddings into a queryable [Index](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/index/index.m.md).
-4. Define your search with dynamic parameters and weights as a [Query](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/query/query.md).
-5. Load your data using a [Source](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/source/index.md).
-6. Define your transformations with a [Parser](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/common/parser) (e.g.: from [`pd.DataFrame`](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/common/parser/dataframe_parser.md)). 
-7. Run your configuration with an [Executor](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/executor/in_memory/in_memory_executor.md).
+![If the image does not render, you can check the notebook here: https://github.com/superlinked/superlinked/blob/main/notebook/recommendations_e_commerce.ipynb](https://storage.googleapis.com/superlinked-public-assets/notebook.png)
 
-You can check a list of our [features](https://github.com/superlinked/superlinked/tree/main/notebook/feature) or head to our [documentation](https://github.com/superlinked/superlinked/tree/main/docs).
-  
 ## Try it out
 
 Example on how to use Superlinked to experiment with the semantic search use-case. 
 
-### Pre-requisities
+### Pre-requisites
 
 #### In a notebook
 
 Install the superlinked library: 
 ```
 %pip install superlinked
 ```
 
 #### As a script 
-Ensure your python version is 3.10.x.
+Ensure your python version is at least 3.10.x but not newer than 3.12.
 
 ```commandline
 $> python -V
 Python 3.10.9
 ```
 
 If your python version is not `3.10.x` you might use [pyenv](https://github.com/pyenv/pyenv) to install it. 
@@ -73,15 +54,15 @@
 from superlinked.framework.dsl.index.index import Index
 from superlinked.framework.dsl.query.param import Param
 from superlinked.framework.dsl.query.query import Query
 from superlinked.framework.dsl.source.in_memory_source import InMemorySource
 from superlinked.framework.dsl.executor.in_memory.in_memory_executor import InMemoryExecutor
 
 
-@schema # Desribe your schemas.
+@schema # Describe your schemas.
 class Document:
     id: IdField  # Each schema should have exactly one `IdField`.
     body: String # Use `String` for text fields.
 
 document = Document()
 
 relevance_space = TextSimilaritySpace(text=document.body, model="sentence-transformers/all-mpnet-base-v2") # Select your semantic embedding model.
@@ -99,16 +80,39 @@
 source.put([{"id": "sunny_day", "body": "Today is a sunny day"}])
 
 print(app.query(query, query_text="Who is a positive friend?")) # Run your query.
 ```
 
 Ready to go to production? We are launching our first Vector DB connectors soon! [Tell us which Vector DB we should support!](https://github.com/superlinked/superlinked/discussions/41)
 
+## Use-cases
+
+- **RAG**: [HR Knowledgebase](https://github.com/superlinked/superlinked/blob/main/notebook/rag_hr_knowledgebase.ipynb)
+- **Semantic Search**: [Movies](https://github.com/superlinked/superlinked/blob/main/notebook/semantic_search_netflix_titles.ipynb), [Business News](https://github.com/superlinked/superlinked/blob/main/notebook/semantic_search_news.ipynb)
+- **Recommendation Systems**: [E-commerce](https://github.com/superlinked/superlinked/blob/main/notebook/recommendations_e_commerce.ipynb)
+- **Analytics**: [User Acquisition](https://github.com/superlinked/superlinked/blob/main/notebook/analytics_user_acquisition.ipynb)
+
+You can check a full list of examples [here](https://github.com/superlinked/superlinked/tree/main/notebook).
+
+## Reference
+
+1. Describe your data using Python classes with the [@schema](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/common/schema/schema.md) decorator.
+2. Describe your vector embeddings from building blocks with [Spaces](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/space/index.md).
+3. Combine your embeddings into a queryable [Index](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/index/index.m.md).
+4. Define your search with dynamic parameters and weights as a [Query](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/query/query.md).
+5. Load your data using a [Source](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/source/index.md).
+6. Define your transformations with a [Parser](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/common/parser) (e.g.: from [`pd.DataFrame`](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/common/parser/dataframe_parser.md)). 
+7. Run your configuration with an [Executor](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/executor/in_memory/in_memory_executor.md).
+
+You can check a list of our [features](https://github.com/superlinked/superlinked/tree/main/notebook/feature) or head to our [documentation](https://github.com/superlinked/superlinked/tree/main/docs).
+  
 ## Articles
 
-- [Vector DB Comparison](https://superlinked.com/vector-db-comparison/): Open-source collaboritve comparison of vector databases by Superlinked.
+- [Vector DB Comparison](https://superlinked.com/vector-db-comparison/): Open-source collaborative comparison of vector databases by Superlinked.
 - [Vector Hub](https://superlinked.com/vectorhub/): VectorHub is a free and open-sourced learning hub for people interested in adding vector retrieval to their ML stack
 
 ## Support
 
-If you encounter any challanges during your experiments, feel free to create an [issue](https://github.com/superlinked/superlinked/issues/new?assignees=ClaireSuperlinked&labels=bug&projects=&template=bug_report.md&title=), request a [feature](https://github.com/superlinked/superlinked/issues/new?assignees=ClaireSuperlinked&labels=enhancement&projects=&template=feature_request.md&title=) or to [start a discussion](https://github.com/superlinked/superlinked/discussions/new/choose).
+If you encounter any challenges during your experiments, feel free to create an [issue](https://github.com/superlinked/superlinked/issues/new?assignees=ClaireSuperlinked&labels=bug&projects=&template=bug_report.md&title=), request a [feature](https://github.com/superlinked/superlinked/issues/new?assignees=ClaireSuperlinked&labels=enhancement&projects=&template=feature_request.md&title=) or to [start a discussion](https://github.com/superlinked/superlinked/discussions/new/choose).
 Make sure to group your feedback in separate issues and discussions by topic. Thank you for your feedback!
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `superlinked-3.9.1/superlinked/evaluation/charts/recency_plotter.py` & `superlinked-4.0.1/superlinked/evaluation/charts/recency_plotter.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,78 +15,87 @@
 import datetime
 from typing import Mapping
 
 import altair as alt
 import numpy as np
 import pandas as pd
 
+from superlinked.framework.common.calculation.distance_metric import DistanceMetric
 from superlinked.framework.common.calculation.vector_similarity import (
-    SimilarityMethod,
     VectorSimilarityCalculator,
 )
 from superlinked.framework.common.dag.context import (
     ContextValue,
     ExecutionContext,
     ExecutionEnvironment,
 )
 from superlinked.framework.common.data_types import Vector
-from superlinked.framework.common.embedding.recency_embedding import RecencyEmbedding
+from superlinked.framework.common.embedding.recency_embedding import (
+    RecencyEmbedding,
+    calculate_recency_normalization,
+)
 from superlinked.framework.dsl.space.recency_space import RecencySpace
 
 
 class RecencyPlotter:
     """
     A helper class used to plot recency scores.
     """
 
     def __init__(
         self,
         recency_space: RecencySpace,
         vector_similarity_calculator: VectorSimilarityCalculator = VectorSimilarityCalculator(
-            SimilarityMethod.INNER_PRODUCT
+            DistanceMetric.INNER_PRODUCT
         ),
         negative_filter_time_period_showcase_multiplier: float = 1.1,
         context_data: Mapping[str, Mapping[str, ContextValue]] | None = None,
     ) -> None:
         """
-        Sets up the RecencyPlotter object. Provide it with a space, and observe the score of time points calculated back from `now`.
+        Sets up the RecencyPlotter object. Provide it with a space, and observe the score
+        of time points calculated back from `now`.
 
         Args:
             recency_space (RecencySpace): An instance of RecencySpace class.
-            negative_filter_time_period_showcase_multiplier (float): A multiplier to adjust the time frame for showcasing negative filter area.
-                1.1 means 10% of the largest period time is additionally presented in the chart. Default value tends to work nicely.
+            negative_filter_time_period_showcase_multiplier (float): A multiplier to adjust
+            the time frame for showcasing negative filter area.
+                1.1 means 10% of the largest period time is additionally presented in the
+                chart. Default value tends to work nicely.
         """
-        self._embedding: RecencyEmbedding = RecencyEmbedding(
+        self.context: ExecutionContext = ExecutionContext.from_context_data(
+            context_data, environment=ExecutionEnvironment.IN_MEMORY
+        )
+        normalization = calculate_recency_normalization(recency_space.period_time_list)
+        self._embedding = RecencyEmbedding(
             period_time_list=recency_space.period_time_list,
+            normalization=normalization,
+            time_period_hour_offset=recency_space.time_period_hour_offset,
             negative_filter=recency_space.negative_filter,
         )
         self._negative_filter_time_period_showcase_multiplier = (
             negative_filter_time_period_showcase_multiplier
         )
         self.vector_similarity_calculator = vector_similarity_calculator
-        self.context: ExecutionContext = ExecutionContext.from_context_data(
-            context_data, environment=ExecutionEnvironment.IN_MEMORY
-        )
 
     def __generate_recency_scores(
         self, oldest_ts_to_plot: int, now_ts: int, num_points: int
     ) -> pd.DataFrame:
         plot_timestamps: np.ndarray = np.linspace(
             start=oldest_ts_to_plot, stop=now_ts, num=num_points
         )
         recency_vectors: list[Vector] = [
-            self._embedding.calc_recency_vector(plot_ts, now_ts, False)
+            self._embedding.calc_recency_vector(plot_ts, self.context)
             for plot_ts in plot_timestamps
         ]
 
-        now_vector: Vector = self._embedding.calc_recency_vector(now_ts, now_ts, True)
+        now_vector: Vector = self._embedding.calc_recency_vector(
+            now_ts, ExecutionContext(ExecutionEnvironment.QUERY)
+        )
         recency_scores: list[float] = [
-            self.vector_similarity_calculator.calculate_similarity(
-                now_vector.value, vec.value
-            )
+            self.vector_similarity_calculator.calculate_similarity(now_vector, vec)
             for vec in recency_vectors
         ]
         date_labels: list[datetime.datetime] = [
             datetime.datetime.fromtimestamp(ts) for ts in plot_timestamps
         ]
         return pd.DataFrame({"date": date_labels, "score": recency_scores})
 
@@ -106,15 +115,17 @@
             height (int, optional): The height of the chart. Defaults to 380.
             chart_point_size (int, optional): The size of the points on the chart. Defaults to 10.
 
         Returns:
             alt.Chart: A Chart object with plotted recency scores.
         """
         now_ts: int = self.context.now()
-        max_period_time_ts: int = int(self._embedding.max_period_time.total_seconds())
+        max_period_time_ts: int = int(
+            self._embedding.max_period_time.period_time.total_seconds()
+        )
         oldest_ts_to_plot: int = int(
             now_ts
             - (
                 max_period_time_ts
                 * self._negative_filter_time_period_showcase_multiplier
             )
         )
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/const.py` & `superlinked-4.0.1/superlinked/framework/dsl/registry/exception.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,10 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-ONLINE_DAG_NODE_MODULE = "superlinked.framework.online.dag"
-MAX_DAG_DEPTH = 20
-DEFAULT_WEIGHT = 1.0
+
+class DuplicateElementException(Exception):
+    pass
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/aggregation_node.py` & `superlinked-4.0.1/superlinked/framework/common/dag/aggregation_node.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import cast
+from typing import Any, cast
 
 from typing_extensions import override
 
 from superlinked.framework.common.dag.dag_effect import DagEffect
 from superlinked.framework.common.dag.exception import ParentCountException
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.dag.persistence_params import PersistenceParams
@@ -32,16 +32,16 @@
         self,
         weighted_parents: list[Weighted[Node[Vector]]],
         dag_effects: set[DagEffect],
     ) -> None:
         super().__init__(
             [weighted_parent.item for weighted_parent in weighted_parents],
             persistence_params=PersistenceParams(persist_parent_evaluation_result=True),
+            dag_effects=dag_effects,
         )
-        self.dag_effects = dag_effects
         self.__validate_parents()
         self.weighted_parents = weighted_parents
         # All parents are of the same length as it was validated earlier.
         self.__length = cast(HasLength, self.parents[0]).length
 
     def __validate_parents(self) -> None:
         if len(self.parents) == 0:
@@ -63,15 +63,26 @@
             )
 
     @property
     def length(self) -> int:
         return self.__length
 
     @override
+    def _get_node_id_parameters(self) -> dict[str, Any]:
+        weighted_parents = [
+            {"node_id": parent.item.node_id, "weight": parent.weight}
+            for parent in self.weighted_parents
+        ]
+        return {
+            "weighted_parents": weighted_parents,
+            "dag_effects": self.dag_effects,
+        }
+
     @property
+    @override
     def persist_evaluation_result(self) -> bool:
         # Aggregation node's parents are always persisted, no need for double persistence.
         return False
 
     @override
     def project_parents_to_schema(self, schema: SchemaObject) -> list[Node]:
         if schema in self.schemas:
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/chunking_node.py` & `superlinked-4.0.1/superlinked/framework/common/interface/has_length.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,20 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from superlinked.framework.common.dag.node import Node
+from abc import ABC, abstractmethod
 
 
-class ChunkingNode(Node[str]):
-    def __init__(
-        self,
-        parent: Node[str],
-        chunk_size: int | None = None,
-        chunk_overlap: int | None = None,
-    ) -> None:
-        super().__init__([parent])
-        self.chunk_size = chunk_size
-        self.chunk_overlap = chunk_overlap
+class HasLength(ABC):
+    @property
+    @abstractmethod
+    def length(self) -> int:
+        pass
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/comparison_filter_node.py` & `superlinked-4.0.1/superlinked/framework/common/dag/comparison_filter_node.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import Any
+
 from typing_extensions import override
 
 from superlinked.framework.common.dag.dag_effect import DagEffect
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.dag.schema_field_node import SchemaFieldNode
 from superlinked.framework.common.exception import InitializationException
 from superlinked.framework.common.interface.comparison_operand import (
@@ -36,12 +38,19 @@
                 f"{self.class_name}'s parent and operand must be the same."
             )
         super().__init__([parent])
         if dag_effects is not None:
             self.dag_effects = dag_effects
         self.comparison_operation = comparison_operation
 
-    @override
     @property
+    @override
     def persist_evaluation_result(self) -> bool:
-        # ComparisonFilterNode's result is bool, curently it cannot be persisted.
+        # ComparisonFilterNode's result is bool, currently it cannot be persisted.
         return False
+
+    @override
+    def _get_node_id_parameters(self) -> dict[str, Any]:
+        return {
+            "comparison_operation": self.comparison_operation,
+            "dag_effects": self.dag_effects,
+        }
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/concatenation_node.py` & `superlinked-4.0.1/superlinked/framework/common/dag/concatenation_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import cast
+from typing import Any, cast
 
 from typing_extensions import override
 
 from superlinked.framework.common.const import DEFAULT_WEIGHT
 from superlinked.framework.common.dag.dag_effect import DagEffect
 from superlinked.framework.common.dag.exception import ParentCountException
 from superlinked.framework.common.dag.node import Node
@@ -49,14 +49,20 @@
             )
 
     @property
     def length(self) -> int:
         return self.__length
 
     @override
+    def _get_node_id_parameters(self) -> dict[str, Any]:
+        return {
+            "default_weight": self.default_weight,
+        }
+
+    @override
     def project_parents_to_schema(self, schema: SchemaObject) -> list[Node]:
         if schema in self.schemas:
             return self.parents
         return []
 
     def project_parents_for_dag_effect(self, dag_effect: DagEffect) -> list[Node]:
         if dag_effect in self.dag_effects:
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/constant_node.py` & `superlinked-4.0.1/superlinked/framework/common/dag/constant_node.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import Any
+
+from typing_extensions import override
+
 from superlinked.framework.common.dag.node import NDT, Node
 from superlinked.framework.common.schema.schema_object import SchemaObject
 
 
 class ConstantNode(Node[NDT]):
     def __init__(self, value: NDT, schema: SchemaObject) -> None:
         super().__init__([], schemas={schema})
         self.value = value
+
+    @override
+    def _get_node_id_parameters(self) -> dict[str, Any]:
+        return {"schemas": self.schemas, "value": str(self.value)}
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/context.py` & `superlinked-4.0.1/superlinked/framework/common/dag/context.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from collections import defaultdict
-from enum import Enum
+from enum import Enum, auto
 from typing import Mapping, TypeVar, cast
 
 from typing_extensions import Self, TypeAlias
 
 from superlinked.framework.common.exception import (
     NotImplementedException,
     QueryException,
@@ -33,52 +33,62 @@
 CONTEXT_COMMON_NOW = "now"
 SPACE_WEIGHT_PARAM_NAME = "weight"
 
 
 class ExecutionEnvironment(Enum):
     IN_MEMORY = 1
     QUERY = 2
+    BATCH = 3
+
+
+class NowStrategy(Enum):
+    SYSTEM_TIME = auto()
+    CONTEXT_TIME = auto()
+    CONTEXT_OR_SYSTEM_TIME = auto()
 
 
 class ExecutionContext:
     def __init__(
         self,
         environment: ExecutionEnvironment,
+        now_strategy: NowStrategy = NowStrategy.CONTEXT_OR_SYSTEM_TIME,
         data: Mapping[str, Mapping[str, ContextValue]] | None = None,
     ) -> None:
         self.__environment = environment
+        self.__now_strategy = now_strategy
         self.__data: dict[str, dict[str, ContextValue]] = defaultdict(dict)
         if data:
             self.update_data(data)
 
     def update_data(self, data: Mapping[str, Mapping[str, ContextValue]]) -> Self:
         for key, sub_map in data.items():
             self.__data[key].update(sub_map)
         return self
 
     def now(self) -> int:
-        match self.__environment:
-            case ExecutionEnvironment.IN_MEMORY:
+        match self.__now_strategy:
+            case NowStrategy.CONTEXT_OR_SYSTEM_TIME:
                 return (
                     self.__data_now() or time_util.now()
                 )  # ingestion uses system time for in_memory executor if it is not overridden
-            case ExecutionEnvironment.QUERY:
+            case NowStrategy.CONTEXT_TIME:
                 now = self.__data_now()
                 if now is None:
                     raise QueryException(
                         (
                             f"Environment's '{CONTEXT_COMMON}.{CONTEXT_COMMON_NOW}' ",
                             "property should always be initialized for query contexts",
                         )
                     )
-
                 return now
+            case NowStrategy.SYSTEM_TIME:
+                return time_util.now()
             case _:
                 raise NotImplementedException(
-                    f"Now is not defined for environment type: {self.__environment}"
+                    f"Unknown now strategy: {self.__now_strategy}"
                 )
 
     @property
     def environment(self) -> ExecutionEnvironment:
         return self.__environment
 
     @property
@@ -125,13 +135,14 @@
         return self.has_environment(ExecutionEnvironment.QUERY)
 
     @classmethod
     def from_context_data(
         cls,
         context_data: Mapping[str, Mapping[str, ContextValue]] | None,
         environment: ExecutionEnvironment,
+        now_strategy: NowStrategy = NowStrategy.CONTEXT_OR_SYSTEM_TIME,
     ) -> ExecutionContext:
         return (
-            cls(environment)
+            cls(environment, now_strategy)
             if context_data is None
-            else cls(environment).update_data(context_data)
+            else cls(environment, now_strategy).update_data(context_data)
         )
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/dag.py` & `superlinked-4.0.1/superlinked/framework/common/dag/dag.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,52 +8,61 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from beartype.typing import Sequence
+
 from superlinked.framework.common.dag.dag_effect import DagEffect
+from superlinked.framework.common.dag.exception import InvalidDagException
+from superlinked.framework.common.dag.index_node import IndexNode
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.dag.schema_dag import SchemaDag
 from superlinked.framework.common.exception import (
+    DuplicateNodeIdException,
     InvalidDagEffectException,
     InvalidSchemaException,
 )
 from superlinked.framework.common.schema.schema_object import SchemaObject
 
 
 class Dag:
     def __init__(
         self, nodes: list[Node], dag_effects: list[DagEffect] | None = None
     ) -> None:
         self.nodes = nodes
+        self._index_node = self.__init_index_node(self.nodes)
+        self.__check_for_node_id_duplication()
         self.dag_effects = dag_effects or []
-        self.__node_id_schema_map: dict[str, set[SchemaObject]] = (
+        node_id_schema_map: dict[str, set[SchemaObject]] = (
             self.__init_node_id_schema_map(self.nodes)
         )
-        self.__node_id_dag_effect_map: dict[str, set[DagEffect]] = (
+        node_id_dag_effect_map: dict[str, set[DagEffect]] = (
             self.__init_node_id_dag_effect_map(self.nodes)
         )
-        self.__schemas: set[SchemaObject] = self.__init_schemas(
-            self.__node_id_schema_map
-        )
+        self.__schemas: set[SchemaObject] = self.__init_schemas(node_id_schema_map)
         self.__schema_dag_map: dict[SchemaObject, SchemaDag] = (
-            self.__init_schema_schema_dag_map(self.__schemas, self.__node_id_schema_map)
+            self.__init_schema_schema_dag_map(self.__schemas, node_id_schema_map)
         )
         self.__dag_effect_dag_map: dict[DagEffect, SchemaDag] = (
             self.__init_dag_effect_schema_dag_map(
-                self.dag_effects, self.__node_id_dag_effect_map
+                self.dag_effects, node_id_dag_effect_map
             )
         )
 
     @property
     def schemas(self) -> set[SchemaObject]:
         return self.__schemas
 
+    @property
+    def index_node(self) -> IndexNode:
+        return self._index_node
+
     def project_to_schema(self, schema: SchemaObject) -> SchemaDag:
         if (dag := self.__schema_dag_map.get(schema)) is not None:
             return dag
         raise InvalidSchemaException(
             f"SchemaDag for the given schema ({schema._base_class_name}) doesn't exist."
         )
 
@@ -61,14 +70,21 @@
         if (dag := self.__dag_effect_dag_map.get(dag_effect)) is not None:
             return dag
         raise InvalidDagEffectException(
             f"SchemaDag for the given dag effect ({dag_effect} "
             + f"- {dag_effect.event_schema._base_class_name}) doesn't exist."
         )
 
+    def __init_index_node(self, nodes: Sequence[Node]) -> IndexNode:
+        if index_node := next(
+            (node for node in nodes if isinstance(node, IndexNode)), None
+        ):
+            return index_node
+        raise InvalidDagException("Dag doesn't have an IndexNode.")
+
     def __init_node_id_schema_map(
         self, nodes: list[Node]
     ) -> dict[str, set[SchemaObject]]:
         return {node.node_id: node.schemas for node in nodes}
 
     def __init_node_id_dag_effect_map(
         self, nodes: list[Node]
@@ -129,7 +145,14 @@
             for node in filtered_nodes
             for parent in node.project_parents_for_dag_effect(dag_effect)
         )
         return SchemaDag(
             dag_effect.event_schema,
             list(projected_parents.union(filtered_nodes)),
         )
+
+    def __check_for_node_id_duplication(self) -> None:
+        node_ids = set()
+        for node in self.nodes:
+            if node.node_id in node_ids:
+                raise DuplicateNodeIdException(f"Node id: {node} is duplicated!")
+            node_ids.add(node._node_id)
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/dag_effect.py` & `superlinked-4.0.1/superlinked/framework/common/dag/dag_effect.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,11 +24,11 @@
 class DagEffect:
     resolved_affected_schema_reference: ResolvedSchemaReference
     resolved_affecting_schema_reference: ResolvedSchemaReference
     event_schema: EventSchemaObject
 
     def __str__(self) -> str:
         return (
-            f"{self.resolved_affected_schema_reference}:"
-            + f"{self.resolved_affecting_schema_reference}:"
-            + f"{self.event_schema._schema_name}"
+            f"{self.__class__.__name__}(resolved_affected_schema_reference={self.resolved_affected_schema_reference}, "
+            f"resolved_affecting_schema_reference={self.resolved_affecting_schema_reference}, "
+            f"event_schema={self.event_schema})"
         )
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/event_aggregation_node.py` & `superlinked-4.0.1/superlinked/framework/common/dag/event_aggregation_node.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import cast
+from typing import Any, cast
 
 from typing_extensions import override
 
 from superlinked.framework.common.dag.comparison_filter_node import ComparisonFilterNode
 from superlinked.framework.common.dag.dag_effect import DagEffect
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.dag.persistence_params import PersistenceParams
@@ -64,14 +64,29 @@
         self.__length = cast(HasLength, self.parents[0]).length
 
     @property
     def length(self) -> int:
         return self.__length
 
     @override
+    def _get_node_id_parameters(self) -> dict[str, Any]:
+        filters = [
+            {"node_id": filter_.item.node_id, "weight": filter_.weight}
+            for filter_ in self.filters
+        ]
+        return {
+            "dag_effects": self.dag_effects,
+            "schemas": self.schemas,
+            "event_schema": self.event_schema,
+            "affected_schema": self.affected_schema,
+            "affecting_schema": self.affecting_schema,
+            "filters": filters,
+        }
+
+    @override
     def project_parents_to_schema(self, schema: SchemaObject) -> list[Node]:
         if schema == self.event_schema:
             return self.parents
         return []
 
     def project_parents_for_dag_effect(self, dag_effect: DagEffect) -> list[Node]:
         if dag_effect in self.dag_effects:
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/exception.py` & `superlinked-4.0.1/superlinked/framework/common/dag/exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 
 from superlinked.framework.common.exception import (
     InitializationException,
     ValidationException,
 )
 
 
+class InvalidDagException(ValidationException):
+    pass
+
+
 class LeafNodeCountException(ValidationException):
     pass
 
 
 class LeafNodeTypeException(ValidationException):
     pass
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/index_node.py` & `superlinked-4.0.1/superlinked/framework/common/dag/index_node.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import cast
+from typing import Any, cast
+
+from typing_extensions import override
 
 from superlinked.framework.common.dag.exception import ParentCountException
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.dag.persistence_params import PersistenceParams
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.storage.persistence_type import PersistenceType
@@ -24,24 +26,30 @@
 
 class IndexNode(Node[Vector], HasLength):
     def __init__(
         self,
         parents: set[Node[Vector]],
     ) -> None:
         super().__init__(
-            list(self.__validate_parents(parents)),
+            self.__validate_and_order_parents(parents),
             persistence_params=PersistenceParams(
                 persist_evaluation_result=True, persistence_type=PersistenceType.VECTOR
             ),
         )
         self.__length = cast(HasLength, self.parents[0]).length
 
-    def __validate_parents(self, parents: set[Node[Vector]]) -> set[Node[Vector]]:
+    def __validate_and_order_parents(
+        self, parents: set[Node[Vector]]
+    ) -> list[Node[Vector]]:
         if len(parents) == 0:
             raise ParentCountException(
                 f"{self.class_name} must have at least 1 parent."
             )
-        return parents
+        return sorted(parents, key=lambda parent: parent.node_id)
 
     @property
     def length(self) -> int:
         return self.__length
+
+    @override
+    def _get_node_id_parameters(self) -> dict[str, Any]:
+        return {"length": self.length}
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/named_function_node.py` & `superlinked-4.0.1/superlinked/framework/common/dag/named_function_node.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import Any
+
+from typing_extensions import override
+
 from superlinked.framework.common.dag.node import NDT, Node
 from superlinked.framework.common.schema.schema_object import SchemaObject
 from superlinked.framework.common.util.named_function_evaluator import NamedFunction
 
 
 class NamedFunctionNode(Node[NDT]):
     def __init__(
@@ -23,7 +27,15 @@
         named_function: NamedFunction,
         schema: SchemaObject,
         return_type: type[NDT],
     ) -> None:
         super().__init__([], schemas={schema})
         self.named_function = named_function
         self.return_type = return_type
+
+    @override
+    def _get_node_id_parameters(self) -> dict[str, Any]:
+        return {
+            "schemas": self.schemas,
+            "named_function": self.named_function,
+            "return_type": self.return_type,
+        }
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/node.py` & `superlinked-4.0.1/superlinked/framework/online/source/in_memory_data_processor.py`

 * *Files 27% similar despite different names*

```diff
@@ -8,85 +8,76 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from __future__ import annotations
-
-import uuid
-from abc import ABC
-from typing import Generic, TypeVar
-
+from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.dag_effect import DagEffect
-from superlinked.framework.common.dag.persistence_params import PersistenceParams
-from superlinked.framework.common.schema.schema_object import SchemaObject
-from superlinked.framework.common.storage.persistence_type import PersistenceType
+from superlinked.framework.common.exception import InvalidDagEffectException
+from superlinked.framework.common.observable import Subscriber
+from superlinked.framework.common.parser.parsed_schema import ParsedSchema
+from superlinked.framework.dsl.index.index import Index
+from superlinked.framework.evaluator.online_dag_evaluator import OnlineDagEvaluator
 
-# NodeDataType
-NDT = TypeVar("NDT")
-# NodeType
-NT = TypeVar("NT", bound="Node")
 
+class InMemoryDataProcessor(Subscriber[ParsedSchema]):
+    MAX_SAVE_DEPTH = 10
 
-class Node(Generic[NDT], ABC):
     def __init__(
+        self, evaluator: OnlineDagEvaluator, context: ExecutionContext, index: Index
+    ) -> None:
+        super().__init__()
+        self.evaluator = evaluator
+        self.context = context
+        self.effect_schemas = set(index._effect_schemas)
+        self._schema_type_schema_mapper = index._schema_type_schema_mapper
+        self._dag_effects = index._dag_effects
+
+    def update(self, messages: list[ParsedSchema]) -> None:
+        regular_msgs: list[ParsedSchema] = []
+        for message in messages:
+            if message.schema in self.effect_schemas:
+                self._process_event(message)
+            else:
+                regular_msgs.append(message)
+        if regular_msgs:
+            self.evaluator.evaluate(regular_msgs, self.context)
+
+    def _process_event(
         self,
-        parents: list[Node],
-        schemas: set[SchemaObject] | None = None,
-        dag_effects: set[DagEffect] | None = None,
-        persistence_params: PersistenceParams | None = None,
+        event_parsed_schema: ParsedSchema,
     ) -> None:
-        self.children: list[Node] = []
-        self.parents = parents
-        self._node_id = (
-            f"{self.class_name}-{str(uuid.uuid4())}"
-            f'({"|".join([parent.node_id for parent in self.parents])})'
-        )
-        self.schemas: set[SchemaObject] = (schemas or set()).union(
-            {schema for parent in parents for schema in parent.schemas}
-            if parents
-            else set()
-        )
-        self.dag_effects: set[DagEffect] = (dag_effects or set()).union(
-            {dag_effect for parent in parents for dag_effect in parent.dag_effects}
-            if parents
-            else set()
-        )
-        self._persistence_params = persistence_params or PersistenceParams()
-        for parent in self.parents:
-            parent._append_child(self)
-
-    def _append_child(self, child: Node) -> None:
-        self.children.append(child)
-        self._persistence_params.persist_evaluation_result |= (
-            child._persistence_params.persist_parent_evaluation_result
+        effect_parsed_schema_map = self._map_event_parsed_schema_by_dag_effects(
+            event_parsed_schema
         )
+        for effect, parsed_schema in effect_parsed_schema_map.items():
+            self.evaluator.evaluate_by_dag_effect(parsed_schema, self.context, effect)
 
-    @property
-    def node_id(self) -> str:
-        return self._node_id
-
-    @property
-    def class_name(self) -> str:
-        return self.__class__.__name__
-
-    @property
-    def persist_evaluation_result(self) -> bool:
-        return self._persistence_params.persist_evaluation_result
-
-    @property
-    def persistence_type(self) -> PersistenceType:
-        return self._persistence_params.persistence_type
-
-    def project_parents_to_schema(self, schema: SchemaObject) -> list[Node]:
-        if schema in self.schemas:
-            return [parent for parent in self.parents if schema in parent.schemas]
-        return []
-
-    def project_parents_for_dag_effect(self, dag_effect: DagEffect) -> list[Node]:
-        if dag_effect in self.dag_effects:
-            return [
-                parent for parent in self.parents if dag_effect in parent.dag_effects
+    def _map_event_parsed_schema_by_dag_effects(
+        self, event_parsed_schema: ParsedSchema
+    ) -> dict[DagEffect, ParsedSchema]:
+        active_effects = [
+            effect
+            for effect in self._dag_effects
+            if effect.event_schema == event_parsed_schema.schema
+        ]
+        effect_parsed_schema_map = dict[DagEffect, ParsedSchema]()
+        for effect in active_effects:
+            affected_schema_ids = [
+                reference.value
+                for reference in event_parsed_schema.fields
+                if reference.schema_field
+                == effect.resolved_affected_schema_reference.reference_field
+                and reference.value is not None
             ]
-        return []
+            if len(affected_schema_ids) > 1:
+                raise InvalidDagEffectException(f"DagEffect: {effect}")
+            if affected_schema_ids:
+                effect_parsed_schema_map[effect] = ParsedSchema(
+                    effect.resolved_affected_schema_reference.schema,
+                    affected_schema_ids[0],
+                    [],
+                    event_parsed_schema,
+                )
+        return effect_parsed_schema_map
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/number_embedding_node.py` & `superlinked-4.0.1/superlinked/framework/common/embedding/custom_embedding.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,31 +8,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from superlinked.framework.common.dag.node import Node
+import numpy as np
+import numpy.typing as npt
+from typing_extensions import override
+
+from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.data_types import Vector
-from superlinked.framework.common.embedding.number_embedding import (
-    Mode,
-    NumberEmbedding,
-)
+from superlinked.framework.common.embedding.embedding import Embedding
 from superlinked.framework.common.interface.has_length import HasLength
+from superlinked.framework.common.space.normalization import Normalization
+
 
+class CustomEmbedding(Embedding[npt.NDArray[np.float64]], HasLength):
+    def __init__(self, length: int, normalization: Normalization) -> None:
+        self.__length: int = length
+        self._normalization: Normalization = normalization
 
-class NumberEmbeddingNode(Node[Vector], HasLength):
-    def __init__(
+    @override
+    def embed(
         self,
-        parent: Node[float | int],
-        min_value: float,
-        max_value: float,
-        mode: Mode,
-        negative_filter: float,
-    ) -> None:
-        super().__init__([parent])
-        self.embedding = NumberEmbedding(min_value, max_value, mode, negative_filter)
+        input_: npt.NDArray[np.float64],
+        context: ExecutionContext,  # pylint: disable=unused-argument
+    ) -> Vector:
+        return Vector(input_).normalize(self._normalization.norm(input_))
 
     @property
     def length(self) -> int:
-        return self.embedding.length
+        return self.__length
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/number_similarity_node.py` & `superlinked-4.0.1/superlinked/framework/evaluator/dag_evaluator.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,31 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from superlinked.framework.common.dag.node import Node
-from superlinked.framework.common.data_types import Vector
-from superlinked.framework.common.embedding.number_similarity_embedding import (
-    NumberSimilarityEmbedding,
-)
-from superlinked.framework.common.interface.has_length import HasLength
+from abc import ABC, abstractmethod
+from typing import Generic, TypeVar
 
+from superlinked.framework.common.dag.context import ExecutionContext
+from superlinked.framework.common.parser.parsed_schema import ParsedSchema
 
-class NumberSimilarityNode(Node[Vector], HasLength):
-    def __init__(
-        self,
-        parent: Node[float | int],
-        min_value: float,
-        max_value: float,
-        negative_filter: float,
-    ) -> None:
-        super().__init__([parent])
-        self.embedding = NumberSimilarityEmbedding(
-            min_value, max_value, negative_filter
-        )
+# Dag evaluation result type
+DERT = TypeVar("DERT")
 
-    @property
-    def length(self) -> int:
-        return self.embedding.length
+
+class DagEvaluator(ABC, Generic[DERT]):
+    @abstractmethod
+    def evaluate(
+        self, parsed_schemas: list[ParsedSchema], context: ExecutionContext
+    ) -> list[DERT]:
+        pass
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/period_time.py` & `superlinked-4.0.1/superlinked/framework/common/dag/period_time.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,36 +8,35 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from dataclasses import dataclass, field
 from datetime import timedelta
 
 from superlinked.framework.common.const import DEFAULT_WEIGHT
 
 
+@dataclass(frozen=True)
 class PeriodTime:
     """
     A class representing a period time parameter.
     Attributes:
         period_time (timedelta): Oldest item the parameter will differentiate. Older items will have
             0 or `negative_filter` recency_score.
         weight (float): Defaults to 1.0. Useful to tune different period_times against each other.
     """
 
-    def __init__(self, period_time: timedelta, weight: float = DEFAULT_WEIGHT) -> None:
+    period_time: timedelta = field(init=True)
+    weight: float = field(default=DEFAULT_WEIGHT, init=True)
+
+    def __post_init__(self) -> None:
         """
-        Initialize the PeriodTime.
-        Args:
-            period_time (timedelta): Oldest item the parameter will differentiate.
-                Older items will have 0 or `negative_filter` recency_score.
-            weight (float, optional): Defaults to 1.0. Useful to tune different period_times against each other.
+        Validate the PeriodTime after initialization.
         """
-        if int(period_time.total_seconds()) <= 0:
+        if int(self.period_time.total_seconds()) <= 0:
             raise ValueError(
                 f"Period_time parameter must be a positive time period, at least 1 seconds. "
-                f"Got {period_time.__str__()} which is {int(period_time.total_seconds())} seconds."
+                f"Got {self.period_time.__str__()} which is {int(self.period_time.total_seconds())} seconds."
             )
-        self.period_time = period_time
-        self.weight = weight
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/persistence_params.py` & `superlinked-4.0.1/superlinked/framework/common/dag/persistence_params.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/recency_node.py` & `superlinked-4.0.1/superlinked/framework/common/util/named_function_evaluator.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,30 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from superlinked.framework.common.dag.node import Node
-from superlinked.framework.common.dag.period_time import PeriodTime
-from superlinked.framework.common.data_types import Vector
-from superlinked.framework.common.embedding.recency_embedding import RecencyEmbedding
-from superlinked.framework.common.interface.has_length import HasLength
-
-
-class RecencyNode(Node[Vector], HasLength):
-    def __init__(
-        self,
-        parent: Node[int],
-        period_time_list: list[PeriodTime],
-        negative_filter: float = 0.0,
-    ) -> None:
-        super().__init__([parent])
-        self.embedding: RecencyEmbedding = RecencyEmbedding(
-            period_time_list=period_time_list,
-            negative_filter=negative_filter,
-        )
-
-    @property
-    def length(self) -> int:
-        return self.embedding.length
+from enum import Enum
+from typing import Any
+
+from superlinked.framework.common.dag.context import ExecutionContext
+
+
+class NamedFunction(Enum):
+    NOW = "now"
+
+
+class NamedFunctionEvaluator:
+    def evaluate(self, named_function: NamedFunction, context: ExecutionContext) -> Any:
+        match named_function:
+            case NamedFunction.NOW:
+                return self.__now(context)
+
+    def __now(self, context: ExecutionContext) -> int:
+        return context.now()
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/resolved_schema_reference.py` & `superlinked-4.0.1/superlinked/framework/common/dag/resolved_schema_reference.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,8 +21,11 @@
 @dataclass(frozen=True)
 class ResolvedSchemaReference:
     schema: IdSchemaObject
     reference_field: SchemaReference
     multiplier: float
 
     def __str__(self) -> str:
-        return f"{self.schema._schema_name}:{self.multiplier}"
+        return (
+            f"{self.__class__.__name__}(schema={self.schema}, multiplier={self.multiplier}, "
+            f"reference_field={self.reference_field})"
+        )
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/schema_dag.py` & `superlinked-4.0.1/superlinked/framework/common/dag/schema_dag.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/schema_field_node.py` & `superlinked-4.0.1/superlinked/framework/common/source/source.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Generic
 
-from superlinked.framework.common.dag.dag_effect import DagEffect
-from superlinked.framework.common.dag.node import Node
-from superlinked.framework.common.schema.schema_object import SFT, SchemaField
+from superlinked.framework.common.schema.id_schema_object import IdSchemaObjectT
+from superlinked.framework.common.source.types import SourceTypeT
 
 
-class SchemaFieldNode(Generic[SFT], Node[SFT]):
-    def __init__(
-        self, schema_field: SchemaField[SFT], dag_effects: set[DagEffect] | None = None
-    ) -> None:
-        super().__init__([], schemas={schema_field.schema_obj}, dag_effects=dag_effects)
-        self.schema_field = schema_field
+class Source(Generic[IdSchemaObjectT, SourceTypeT]):
+    def __init__(self) -> None:
+        pass
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/schema_object_reference.py` & `superlinked-4.0.1/superlinked/framework/common/dag/schema_object_reference.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,7 +23,10 @@
     ) -> None:
         if not isinstance(schema, reference_field._referenced_schema):
             raise InitializationException(
                 f"{self.__class__.__name__}'s schema is not the referenced schema."
             )
         self.schema = schema
         self.reference_field = reference_field
+
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__}(schema={self.schema}, reference_field={self.reference_field})"
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/dag/text_embedding_node.py` & `superlinked-4.0.1/superlinked/framework/new_storage/in_memory/json_codec.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,28 +8,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from superlinked.framework.common.dag.node import Node
+import json
+from typing import Any
+
+import numpy as np
+
 from superlinked.framework.common.data_types import Vector
-from superlinked.framework.common.embedding.sentence_transformer_embedding import (
-    SentenceTransformerEmbedding,
-)
-from superlinked.framework.common.interface.has_length import HasLength
-
-
-class TextEmbeddingNode(Node[Vector], HasLength):
-    def __init__(self, parent: Node[str], model_name: str) -> None:
-        super().__init__([parent])
-        self.model_name = model_name
-        self.post_init()
-
-    def post_init(self) -> None:
-        self.embedding = SentenceTransformerEmbedding(self.model_name)
-        self.__length = self.embedding.length
-
-    @property
-    def length(self) -> int:
-        return self.__length
+
+
+class JsonEncoder(json.JSONEncoder):
+    def default(self, o: object) -> dict[str, str | list]:
+        if isinstance(o, Vector):
+            return {"type": "__Vector__", "value": o.value.tolist()}
+        return super().default(o)
+
+
+class JsonDecoder(json.JSONDecoder):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super().__init__(object_hook=self.decode_dict, *args, **kwargs)
+
+    def decode_dict(self, dct: dict[str, Any]) -> Vector | dict[str, Any]:
+        if "type" in dct and dct["type"] == "__Vector__":
+            return Vector(np.array(dct["value"]))
+        return dct
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/embedding/chunking_util.py` & `superlinked-4.0.1/superlinked/framework/common/embedding/chunking_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,18 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Callable
 
-DEFAULT_CHUNK_SIZE = 250
-DEFAULT_CHUNK_OVERLAP = 20
+DEFAULT_CHUNK_SIZE: int = 250
+DEFAULT_CHUNK_OVERLAP: int = 20
+DEFAULT_REMOVE_SPLIT_CHARS: list[str] = ["\n"]
+DEFAULT_ADDITIONAL_SPLIT_CHARS: list[str] = [".", "!", "?"]
 
 
 class Chunker:
     @staticmethod
     def _split_text_keep_sep(
         text: str, separator: str, keep_sep: bool = True
     ) -> list[str]:
@@ -41,21 +43,24 @@
     def _split(
         self,
         text: str,
         chunk_size: int,
         remove_splitter_chars: list[str] | None = None,
         additional_splitter_chars: list[str] | None = None,
     ) -> list[str]:
-        """Break text into logical splits that are smaller than chunk size.
-        NOTE: the splits contain the separators.
+        """
+        Break text into logical splits that are smaller than chunk size.
+        NOTE: the splits
+            - do not contain the separators if separator in remove_splitter_chars
+            - contain the separators if separator in additional_splitter_chars.
         """
         if remove_splitter_chars is None:
-            remove_splitter_chars = ["\n"]
+            remove_splitter_chars = DEFAULT_REMOVE_SPLIT_CHARS
         if additional_splitter_chars is None:
-            additional_splitter_chars = [".", "!", "?"]
+            additional_splitter_chars = DEFAULT_ADDITIONAL_SPLIT_CHARS
         splits_to_process: list[str] = [text]
         new_splits: list[str] = []
         split_fns: list[Callable[[str], list[str]]] = [
             self._split_by_sep(sep, keep_sep=False) for sep in remove_splitter_chars
         ] + [
             self._split_by_sep(sep, keep_sep=True)
             for sep in additional_splitter_chars + [" "]
@@ -125,19 +130,29 @@
         chunk = "".join(cur_chunk).strip()
         if chunk:
             chunks.append(chunk)
 
         return [" ".join(chunk.split()) for chunk in chunks]
 
     def chunk_text(
-        self, text: str, chunk_size: int | None = None, chunk_overlap: int | None = None
+        self,
+        text: str,
+        chunk_size: int | None = None,
+        chunk_overlap: int | None = None,
+        split_chars_keep: list[str] | None = None,
+        split_chars_remove: list[str] | None = None,
     ) -> list[str]:
         if not text:
             return []
         chunk_size = DEFAULT_CHUNK_SIZE if chunk_size is None else chunk_size
         chunk_overlap = (
             DEFAULT_CHUNK_OVERLAP if chunk_overlap is None else chunk_overlap
         )
-        splits = self._split(text=text, chunk_size=chunk_size)
+        splits = self._split(
+            text=text,
+            chunk_size=chunk_size,
+            remove_splitter_chars=split_chars_keep,
+            additional_splitter_chars=split_chars_remove,
+        )
         return self._merge(
             splits=splits, chunk_size=chunk_size, chunk_overlap=chunk_overlap
         )
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/embedding/number_similarity_embedding.py` & `superlinked-4.0.1/superlinked/framework/common/embedding/number_embedding.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,45 +8,83 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import math
+from enum import Enum
 
+import numpy as np
+from typing_extensions import override
+
+from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.data_types import Vector
+from superlinked.framework.common.embedding.embedding import Embedding
 from superlinked.framework.common.interface.has_length import HasLength
+from superlinked.framework.common.space.normalization import Normalization
+
+
+class Mode(Enum):
+    MAXIMUM = "maximum"
+    MINIMUM = "minimum"
+    SIMILAR = "similar"
 
 
-class NumberSimilarityEmbedding(HasLength):
+class NumberEmbedding(Embedding[float], HasLength):
     def __init__(
-        self, min_value: float, max_value: float, negative_filter: float
+        self,
+        min_value: float,
+        max_value: float,
+        mode: Mode,
+        negative_filter: float,
+        normalization: Normalization,
     ) -> None:
-        self.__length = 3
-        self.__circle_size_in_rad = math.pi / 2
-        self.min_value = min_value
-        self.max_value = max_value
-        self.negative_filter = negative_filter
-
-    def transform(self, input_number: float, is_query: bool) -> Vector:
-        if input_number < self.min_value or input_number > self.max_value:
-            return Vector([0.0, 0.0, self.negative_filter])
-
-        constrained_input: float = min(
-            max(self.min_value, input_number), self.max_value
-        )
-        normalized_input = (constrained_input - self.min_value) / (
-            self.max_value - self.min_value
+        self.__length = 1
+        self._min_value = min_value
+        self._max_value = max_value
+        self._mode = mode
+        self._negative_filter = float(negative_filter)
+        self._normalization = normalization
+
+    @override
+    def embed(
+        self,
+        input_: float,
+        context: ExecutionContext,  # pylint: disable=unused-argument
+    ) -> Vector:
+        constrained_input: float = min(max(self._min_value, input_), self._max_value)
+        transformed_number: float = (constrained_input - self._min_value) / (
+            self._max_value - self._min_value
         )
-        angle_in_radians = normalized_input * self.__circle_size_in_rad
-        return Vector(
-            [
-                math.sin(angle_in_radians),
-                math.cos(angle_in_radians),
-                1.0 if is_query else 0.0,
-            ]
+        if self._mode == Mode.MINIMUM:
+            transformed_number = 1 - transformed_number
+        if transformed_number <= 0:
+            transformed_number = self._negative_filter
+        vector_input = np.array([transformed_number])
+        vector = Vector(vector_input)
+        return vector.normalize(self._normalization.norm(vector_input))
+
+    @override
+    def inverse_embed(
+        self,
+        vector: Vector,
+        context: ExecutionContext,  # pylint: disable=unused-argument
+    ) -> float:
+        """
+        This function might seem complex,
+        but it essentially performs the inverse operation of the embed function.
+        """
+        denormalized = self._normalization.denormalize(vector)
+        transformed_number = denormalized.value[0]
+        if transformed_number == self._negative_filter:
+            transformed_number = -1
+        if self._mode == Mode.MINIMUM:
+            transformed_number = 1 - transformed_number
+        transformed_number = (
+            transformed_number * (self._max_value - self._min_value) + self._min_value
         )
+        return transformed_number
 
     @property
     def length(self) -> int:
         return self.__length
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/embedding/sentence_transformer_embedding.py` & `superlinked-4.0.1/superlinked/framework/common/storage_manager/knn_search_params.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,29 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import cast
+from dataclasses import dataclass
 
-import numpy as np
-from sentence_transformers import SentenceTransformer
+from beartype.typing import Sequence
 
 from superlinked.framework.common.data_types import Vector
-from superlinked.framework.common.interface.has_length import HasLength
+from superlinked.framework.common.interface.comparison_operand import (
+    ComparisonOperation,
+)
+from superlinked.framework.common.schema.schema_object import SchemaField
 
 
-class SentenceTransformerEmbedding(HasLength):
-    def __init__(self, model_name: str) -> None:
-        self.model = SentenceTransformer(model_name)
-        self.__length = self.model.get_sentence_embedding_dimension()
-
-    def transform(self, text: str) -> Vector:
-        return Vector(
-            list(cast(np.ndarray, self.model.encode(text)).astype(np.float32).tolist())
-        )
-
-    @property
-    def length(self) -> int:
-        return self.__length
+@dataclass
+class KnnSearchParams:
+    vector: Vector
+    limit: int
+    filters: Sequence[ComparisonOperation[SchemaField]] | None = None
+    radius: float | None = None
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/exception.py` & `superlinked-4.0.1/superlinked/framework/common/exception.py`

 * *Files 19% similar despite different names*

```diff
@@ -29,14 +29,18 @@
     pass
 
 
 class MismatchingDimensionException(Exception):
     pass
 
 
+class NegativeFilterException(Exception):
+    pass
+
+
 class NotImplementedException(Exception):
     pass
 
 
 class ParseException(Exception):
     pass
 
@@ -51,7 +55,11 @@
 
 class SchemaMismatchException(Exception):
     pass
 
 
 class ValidationException(Exception):
     pass
+
+
+class DuplicateNodeIdException(Exception):
+    pass
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/interface/comparison_operand.py` & `superlinked-4.0.1/superlinked/framework/common/interface/comparison_operand.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,90 +23,90 @@
 
 COT = TypeVar("COT", bound="ComparisonOperand")
 
 
 class ComparisonOperand(ABC, Generic[COT]):
     def __init__(self, _: type[COT]) -> None:
         super().__init__()
-        self.__original_operation_mapping: dict[
+        self.__built_in_operation_mapping: dict[
             ComparisonOperationType, Callable[[ComparisonOperand[COT], object], bool]
         ] = {
-            ComparisonOperationType.EQUAL: self._original_equal,
-            ComparisonOperationType.NOT_EQUAL: self._original_not_equal,
-            ComparisonOperationType.GREATER_THAN: self._original_greater_than,
-            ComparisonOperationType.LESS_THAN: self._original_less_than,
-            ComparisonOperationType.GREATER_EQUAL: self._original_greater_equal,
-            ComparisonOperationType.LESS_EQUAL: self._original_less_equal,
+            ComparisonOperationType.EQUAL: self._built_in_equal,
+            ComparisonOperationType.NOT_EQUAL: self._built_in_not_equal,
+            ComparisonOperationType.GREATER_THAN: self._built_in_greater_than,
+            ComparisonOperationType.LESS_THAN: self._built_in_less_than,
+            ComparisonOperationType.GREATER_EQUAL: self._built_in_greater_equal,
+            ComparisonOperationType.LESS_EQUAL: self._built_in_less_equal,
         }
 
     @property
-    def _original_operation_mapping(
+    def _built_in_operation_mapping(
         self,
     ) -> dict[
         ComparisonOperationType, Callable[[ComparisonOperand[COT], object], bool]
     ]:
-        return self.__original_operation_mapping
+        return self.__built_in_operation_mapping
 
-    def _get_original_operation(
+    def _get_built_in_operation(
         self, operation_type: ComparisonOperationType
     ) -> Callable[[ComparisonOperand[COT], object], bool]:
-        return self.__original_operation_mapping[operation_type]
+        return self.__built_in_operation_mapping[operation_type]
 
     def __eq__(self, __value: object) -> ComparisonOperation[COT]:  # type: ignore[override]
         return ComparisonOperation(ComparisonOperationType.EQUAL, self, __value)
 
     @staticmethod
     @abstractmethod
-    def _original_equal(
+    def _built_in_equal(
         left_operand: ComparisonOperand[COT], right_operand: object
     ) -> bool:
         pass
 
     def __ne__(self, __value: object) -> ComparisonOperation[COT]:  # type: ignore[override]
         return ComparisonOperation(ComparisonOperationType.NOT_EQUAL, self, __value)
 
     @staticmethod
     @abstractmethod
-    def _original_not_equal(
+    def _built_in_not_equal(
         left_operand: ComparisonOperand[COT], right_operand: object
     ) -> bool:
         pass
 
     def __gt__(self, __value: object) -> ComparisonOperation[COT]:  # type: ignore[override]
         return ComparisonOperation(ComparisonOperationType.GREATER_THAN, self, __value)
 
     @staticmethod
-    def _original_greater_than(
+    def _built_in_greater_than(
         left_operand: ComparisonOperand[COT], right_operand: object
     ) -> bool:
         raise NotImplementedError()
 
     def __lt__(self, __value: object) -> ComparisonOperation[COT]:  # type: ignore[override]
         return ComparisonOperation(ComparisonOperationType.LESS_THAN, self, __value)
 
     @staticmethod
-    def _original_less_than(
+    def _built_in_less_than(
         left_operand: ComparisonOperand[COT], right_operand: object
     ) -> bool:
         raise NotImplementedError()
 
     def __ge__(self, __value: object) -> ComparisonOperation[COT]:  # type: ignore[override]
         return ComparisonOperation(ComparisonOperationType.GREATER_EQUAL, self, __value)
 
     @staticmethod
-    def _original_greater_equal(
+    def _built_in_greater_equal(
         left_operand: ComparisonOperand[COT], right_operand: object
     ) -> bool:
         raise NotImplementedError()
 
     def __le__(self, __value: object) -> ComparisonOperation[COT]:  # type: ignore[override]
         return ComparisonOperation(ComparisonOperationType.LESS_EQUAL, self, __value)
 
     @staticmethod
-    def _original_less_equal(
+    def _built_in_less_equal(
         left_operand: ComparisonOperand[COT], right_operand: object
     ) -> bool:
         raise NotImplementedError()
 
 
 class ComparisonOperation(Generic[COT]):
     def __init__(
@@ -116,18 +116,21 @@
         other: object,
     ) -> None:
         self._op = op
         self._operand = operand
         self._other = other
 
     def __bool__(self) -> bool:
-        return self._operand._get_original_operation(self._op)(
+        return self._operand._get_built_in_operation(self._op)(
             self._operand, self._other
         )
 
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__}(op={self._op}, operand={self._operand}, other={self._other})"
+
     def evaluate(self, value: Any) -> bool:
         match self._op:
             case ComparisonOperationType.EQUAL:
                 return self.__evaluate_eq(value)
 
             case ComparisonOperationType.NOT_EQUAL:
                 return self.__evaluate_ne(value)
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/interface/comparison_operation_type.py` & `superlinked-4.0.1/superlinked/framework/common/interface/comparison_operation_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/common/interface/has_length.py` & `superlinked-4.0.1/superlinked/framework/common/schema/general_type.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from abc import ABC, abstractmethod
+from typing import TypeVar
 
-
-class HasLength(ABC):
-    @property
-    @abstractmethod
-    def length(self) -> int:
-        pass
+T = TypeVar("T")
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/interface/has_multiplier.py` & `superlinked-4.0.1/superlinked/framework/common/interface/has_multiplier.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/common/interface/weighted.py` & `superlinked-4.0.1/superlinked/framework/common/util/immutable_model.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,19 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from dataclasses import dataclass
-from typing import Generic, TypeVar
+from pydantic import BaseModel, ConfigDict
 
-from superlinked.framework.common.const import DEFAULT_WEIGHT
 
-WT = TypeVar("WT")
-
-
-@dataclass
-class Weighted(Generic[WT]):
-    item: WT
-    weight: float = DEFAULT_WEIGHT
+class ImmutableBaseModel(BaseModel):
+    model_config = ConfigDict(frozen=True)
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/observable.py` & `superlinked-4.0.1/superlinked/framework/common/observable.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 
 
 class Subscriber(ABC, Generic[PM]):
     def __init__(self) -> None:
         pass
 
     @abstractmethod
-    def update(self, message: PM) -> None:
+    def update(self, messages: list[PM]) -> None:
         pass
 
 
 class Publisher(Generic[PM]):
     def __init__(self) -> None:
         self.subscribers: list[Subscriber] = []
 
     def register(self, subscriber: Subscriber[PM]) -> None:
         self.subscribers.append(subscriber)
 
     def unregister(self, subscriber: Subscriber[PM]) -> None:
         self.subscribers.remove(subscriber)
 
-    def _dispatch(self, message: PM) -> None:
+    def _dispatch(self, messages: list[PM]) -> None:
         for subscriber in self.subscribers:
-            subscriber.update(message)
+            subscriber.update(messages)
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/parser/data_parser.py` & `superlinked-4.0.1/superlinked/framework/common/parser/data_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         return self._marshal(parsed_schemas)
 
     def __validate_mapping_against_schema(
         self, schema: IdSchemaObjectT, mapping: Mapping[SchemaField, str] | None
     ) -> None:
         if not mapping:
             return
-        schema_fields = schema._get_schema_fields() + [schema.id]
+        schema_fields = list(schema._get_schema_fields()) + [schema.id]
         if invalid_keys := [key for key in mapping.keys() if key not in schema_fields]:
             invalid_key_names = [
                 f"{key.schema_obj._base_class_name}.{key.name}" for key in invalid_keys
             ]
             raise InvalidMappingException(
                 f"{invalid_key_names} don't belong to the {schema._base_class_name} schema."
             )
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/parser/dataframe_parser.py` & `superlinked-4.0.1/superlinked/framework/common/parser/dataframe_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     ) -> None:
         super().__init__(schema, mapping)
         self._id_name = self.mapping.get(self._schema.id, self._schema.id.name)
 
     def _get_column_name_to_schema_field_mapping(self) -> dict[str, SchemaField]:
         reverse_mapping: dict[str, SchemaField] = {
             self.mapping.get(field, field.name) if self.mapping else field.name: field
-            for field in self._schema._get_schema_fields() + [self._schema.id]
+            for field in list(self._schema._get_schema_fields()) + [self._schema.id]
         }
         return reverse_mapping
 
     def unmarshal(self, data: pd.DataFrame) -> list[ParsedSchema]:
         """
         Parses the given DataFrame into a list of ParsedSchema objects according to the defined schema and mapping.
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/parser/exception.py` & `superlinked-4.0.1/superlinked/framework/common/parser/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/common/parser/json_parser.py` & `superlinked-4.0.1/superlinked/framework/common/parser/json_parser.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/common/parser/parsed_schema.py` & `superlinked-4.0.1/superlinked/framework/common/parser/parsed_schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/common/schema/event_schema.py` & `superlinked-4.0.1/superlinked/framework/common/schema/event_schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/common/schema/event_schema_object.py` & `superlinked-4.0.1/superlinked/framework/common/schema/event_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/common/schema/exception.py` & `superlinked-4.0.1/superlinked/framework/common/schema/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/common/schema/general_type.py` & `superlinked-4.0.1/superlinked/framework/common/source/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import TypeVar
 
-T = TypeVar("T")
+SourceTypeT = TypeVar("SourceTypeT")
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/schema/id_schema_object.py` & `superlinked-4.0.1/superlinked/framework/common/schema/id_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/common/schema/schema.py` & `superlinked-4.0.1/superlinked/framework/common/schema/schema.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/common/schema/schema_decorator.py` & `superlinked-4.0.1/superlinked/framework/common/schema/schema_decorator.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import inspect
 from typing import Any, TypeAlias, cast
 
+from beartype.typing import Sequence
+
 from superlinked.framework.common.schema.event_schema_object import EventSchemaObject
 from superlinked.framework.common.schema.general_type import T
 from superlinked.framework.common.schema.id_schema_object import IdField, IdSchemaObject
 from superlinked.framework.common.schema.schema_object import (
     SchemaField,
     SchemaFieldDescriptor,
 )
@@ -61,15 +63,15 @@
             def __init__(self) -> None:
                 super().__init__(schema_cls, schema_name, id_field_name)
                 self._schema_fields = [
                     self._init_field(schema_field_descriptor)
                     for schema_field_descriptor in schema_field_descriptors
                 ]
 
-            def _get_schema_fields(self) -> list[SchemaField]:
+            def _get_schema_fields(self) -> Sequence[SchemaField]:
                 """Returns all declared SchemaFields. Does not include the mandatory "id" field."""
                 return self._schema_fields
 
         return cast(
             type[Decorated],
             type("DecoratedType", (Decorated, schema_cls), {}),
         )
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/schema/schema_factory.py` & `superlinked-4.0.1/superlinked/framework/common/schema/schema_factory.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/common/schema/schema_reference.py` & `superlinked-4.0.1/superlinked/framework/common/schema/schema_reference.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,20 @@
         HasMultiplier.__init__(self)
         if not issubclass(referenced_schema, IdSchemaObject):
             raise InvalidSchemaTypeException(
                 f"referenced_schema ({referenced_schema}) id not a subclass of IdSchemaObject"
             )
         self.__referenced_schema: type[IdSchemaObject] = referenced_schema
 
+    def __str__(self) -> str:
+        return (
+            f"{self.__class__.__name__}(name={self.name}, schema_obj={self.schema_obj}, "
+            f"referenced_schema={self._referenced_schema})"
+        )
+
     @property
     def _referenced_schema(self) -> type[IdSchemaObject]:
         return self.__referenced_schema
 
     def __mul__(self, other: float | int) -> MultipliedSchemaReference:
         return MultipliedSchemaReference(self) * other
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/schema/schema_type.py` & `superlinked-4.0.1/superlinked/framework/common/schema/schema_type.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/common/schema/schema_validator.py` & `superlinked-4.0.1/superlinked/framework/common/schema/schema_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/common/source/source.py` & `superlinked-4.0.1/superlinked/framework/online/dag/parent_results.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,16 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Generic
+from superlinked.framework.online.dag.evaluation_result import SingleEvaluationResult
+from superlinked.framework.online.dag.online_node import OnlineNode
 
-from superlinked.framework.common.schema.id_schema_object import IdSchemaObjectT
-from superlinked.framework.common.source.types import SourceTypeT
-
-
-class Source(Generic[IdSchemaObjectT, SourceTypeT]):
-    def __init__(self) -> None:
-        pass
+ParentResults = dict[OnlineNode, SingleEvaluationResult]
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/source/types.py` & `superlinked-4.0.1/superlinked/framework/common/storage/search_index_creation/search_algorithm.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,10 +8,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TypeVar
+from enum import Enum
 
-SourceTypeT = TypeVar("SourceTypeT")
+
+class SearchAlgorithm(Enum):
+    FLAT = "FLAT"
+    HNSW = "HNSW"
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/storage/persistence_type.py` & `superlinked-4.0.1/superlinked/framework/common/storage/exception.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,13 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from enum import Enum
 
-
-class PersistenceType(Enum):
-    VECTOR = "vector"
-    PROPERTY = "property"
+class EncoderException(Exception):
+    pass
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/util/dot_separated_path_util.py` & `superlinked-4.0.1/superlinked/framework/common/util/dot_separated_path_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/common/util/immutable_model.py` & `superlinked-4.0.1/superlinked/framework/common/calculation/distance_metric.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,12 +8,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from pydantic import BaseModel, ConfigDict
+from enum import Enum
 
 
-class ImmutableBaseModel(BaseModel):
-    model_config = ConfigDict(frozen=True)
+class DistanceMetric(Enum):
+    EUCLIDEAN = "EUCLIDEAN"
+    INNER_PRODUCT = "INNER_PRODUCT"
+    COSINE_SIMILARITY = "COSINE_SIMILARITY"
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/util/named_function_evaluator.py` & `superlinked-4.0.1/superlinked/framework/common/util/schema_util.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,25 +8,19 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from enum import Enum
-from typing import Any
+import inspect
+from typing import get_origin
 
-from superlinked.framework.common.dag.context import ExecutionContext
+from superlinked.framework.common.schema.general_type import T
 
 
-class NamedFunction(Enum):
-    NOW = "now"
-
-
-class NamedFunctionEvaluator:
-    def evaluate(self, named_function: NamedFunction, context: ExecutionContext) -> Any:
-        match named_function:
-            case NamedFunction.NOW:
-                return self.__now(context)
-
-    def __now(self, context: ExecutionContext) -> int:
-        return context.now()
+class SchemaUtil:
+    @staticmethod
+    def if_not_class_get_origin(type_: type[T]) -> type | None:
+        if inspect.isclass(type_):
+            return type_
+        return get_origin(type_)
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/util/schema_util.py` & `superlinked-4.0.1/superlinked/framework/common/storage_manager/node_result_params.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,19 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import inspect
-from typing import get_origin
+from dataclasses import dataclass
+from typing import Any
 
-from superlinked.framework.common.schema.general_type import T
 
-
-class SchemaUtil:
-    @staticmethod
-    def if_not_class_get_origin(type_: type[T]) -> type | None:
-        if inspect.isclass(type_):
-            return type_
-        return get_origin(type_)
+@dataclass
+class NodeResultParams:
+    result: Any
+    origin_id: str | None = None
+    node_data: dict[str, Any] | None = None
```

### Comparing `superlinked-3.9.1/superlinked/framework/common/util/time_util.py` & `superlinked-4.0.1/superlinked/framework/common/util/time_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/common/util/type_validator.py` & `superlinked-4.0.1/superlinked/framework/common/util/type_validator.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/compiler/online_schema_dag_compiler.py` & `superlinked-4.0.1/superlinked/framework/compiler/online_schema_dag_compiler.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,53 +8,46 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from superlinked.framework.common.const import ONLINE_DAG_NODE_MODULE
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.dag.schema_dag import SchemaDag
-from superlinked.framework.common.exception import NotImplementedException
-from superlinked.framework.common.util.class_helper import ClassHelper
 from superlinked.framework.online.dag.online_node import OnlineNode
+from superlinked.framework.online.dag.online_node_registry import OnlineNodeRegistry
 from superlinked.framework.online.dag.online_schema_dag import OnlineSchemaDag
 from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
     EvaluationResultStoreManager,
 )
 
 
 class OnlineSchemaDagCompiler:
-    online_node_class_mapper: dict[type[Node], type[OnlineNode]] = {
-        c.get_node_type(): c
-        for c in ClassHelper.get_subclasses(OnlineNode, ONLINE_DAG_NODE_MODULE)  # type: ignore
-    }
-
     def __init__(
         self, nodes: set[Node], store_compilation_results: bool = True
     ) -> None:
         self.__nodes = nodes
         self.__store_compilation_results = store_compilation_results
         self.__compiled_nodes: dict[str, OnlineNode] = {}
+        self.__online_node_registry = OnlineNodeRegistry()
 
     def compile_node(
         self,
         node: Node,
         evaluation_result_store_manager: EvaluationResultStoreManager,
     ) -> OnlineNode:
         if compiled_node := self.__compiled_nodes.get(node.node_id):
             return compiled_node
         compiled_parents = [
             self.compile_node(parent, evaluation_result_store_manager)
             for parent in node.parents
             if parent in self.__nodes
         ]
-        online_node_class = OnlineSchemaDagCompiler.find_online_node_class(type(node))
-        compiled_node = online_node_class.from_node(
+        compiled_node = self.__online_node_registry.init_online_node(
             node, compiled_parents, evaluation_result_store_manager
         )
         self.__compiled_nodes[node.node_id] = compiled_node
         return compiled_node
 
     def compile_schema_dag(
         self,
@@ -64,18 +57,7 @@
         compiled_nodes: list[OnlineNode] = [
             self.compile_node(node, evaluation_result_store_manager)
             for node in dag.nodes
         ]
         if not self.__store_compilation_results:
             self.__compiled_nodes = {}
         return OnlineSchemaDag(dag.schema, compiled_nodes)
-
-    @staticmethod
-    def find_online_node_class(node_class: type[Node]) -> type[OnlineNode]:
-        online_node_class = OnlineSchemaDagCompiler.online_node_class_mapper.get(
-            node_class
-        )
-        if online_node_class is None:
-            raise NotImplementedException(
-                f"Not implemented Node type: {node_class.__name__}"
-            )
-        return online_node_class
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/executor/exception.py` & `superlinked-4.0.1/superlinked/framework/dsl/executor/exception.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/executor/executor.py` & `superlinked-4.0.1/superlinked/framework/dsl/executor/executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import Annotated, Generic, TypeVar, get_args
+from typing import Annotated, Generic, TypeVar
 
 from beartype.typing import Sequence
 from typing_extensions import Self
 
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.util.time_util import now
+from superlinked.framework.common.util.type_util import get_single_generic_type
 from superlinked.framework.common.util.type_validator import TypeValidator
 from superlinked.framework.dsl.index.index import Index
 from superlinked.framework.dsl.source.source import SourceT
 from superlinked.framework.storage.entity_store import EntityStore
 from superlinked.framework.storage.entity_store_manager import EntityStoreManager
 from superlinked.framework.storage.object_store import ObjectStore
 from superlinked.framework.storage.object_store_manager import ObjectStoreManager
@@ -104,23 +105,20 @@
 
         Args:
             sources (list[SourceT]): The list of sources.
             indices (list[Index]): The list of indices.
             context (Mapping[str, Mapping[str, Any]]): The context mapping.
         """
         TypeValidator.validate_list_item_type(
-            sources, self.__get_generic_type(), "sources"
+            sources, get_single_generic_type(self), "sources"
         )
         self._sources = sources
         self._indices = indices
         self._context = context
 
-    def __get_generic_type(self) -> type[SourceT]:
-        return get_args(self.__class__.__orig_bases__[0])[0]  # type: ignore[attr-defined] # pylint: disable=no-member
-
     @property
     def context(self) -> ExecutionContext:
         """
         Get the context.
 
         Returns:
             Mapping[str, Mapping[str, Any]]: The context mapping.
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py` & `superlinked-4.0.1/superlinked/framework/dsl/executor/in_memory/in_memory_executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from typing import Any, Mapping
+from typing import Any, Mapping, cast
 
 from beartype.typing import Sequence
 
 from superlinked.framework.common.dag.context import (
     ContextValue,
     ExecutionContext,
     ExecutionEnvironment,
@@ -37,21 +37,22 @@
     InMemoryDataProcessor,
 )
 from superlinked.framework.online.source.in_memory_object_writer import (
     InMemoryObjectWriter,
 )
 from superlinked.framework.storage.in_memory_entity_store import InMemoryEntityStore
 from superlinked.framework.storage.in_memory_object_store import InMemoryObjectStore
+from superlinked.framework.storage.persistable_dict import ObjectReader, ObjectWriter
 
 
 class InMemoryExecutor(Executor[InMemorySource]):
     """
     In-memory implementation of the Executor class. Supply it with the sources through which
     your data is received, and the indices indicating the desired vector spaces, and the executor will
-    create the spaces optimised for search.
+    create the spaces optimized for search.
 
     Attributes:
         sources (list[InMemorySource]): List of in-memory sources.
         indices (list[Index]): List of indices.
     """
 
     def __init__(
@@ -128,14 +129,26 @@
             source._source.register(self._object_writer)
         for data_processor, index in zip(
             self._data_processors, self._executor._indices
         ):
             for source in self.__filter_index_sources(index, self._executor._sources):
                 source._source.register(data_processor)
 
+    def restore(self, reader: ObjectReader) -> None:
+        node_ids = [index._node_id for index in self.executor._indices]
+        app_identifier = "_".join(node_ids)
+        cast(InMemoryObjectStore, self._object_store).restore(reader, app_identifier)
+        cast(InMemoryEntityStore, self._entity_store).restore(reader, app_identifier)
+
+    def persist(self, writer: ObjectWriter) -> None:
+        node_ids = [index._node_id for index in self.executor._indices]
+        app_identifier = "_".join(node_ids)
+        cast(InMemoryObjectStore, self._object_store).persist(writer, app_identifier)
+        cast(InMemoryEntityStore, self._entity_store).persist(writer, app_identifier)
+
     def query(self, query_obj: QueryObj, **params: Any) -> Result:
         """
         Execute a query. Example:
         ```
         query = (
             Query(relevance_index, weights=[{"relevance_space": Param("relevance_weight")}])
             .find(paragraph)
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/executor/query/query_executor.py` & `superlinked-4.0.1/superlinked/framework/dsl/executor/query/query_executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from typing import Any
 
 from superlinked.framework.common.dag.context import (
     CONTEXT_COMMON,
     CONTEXT_COMMON_NOW,
     ExecutionContext,
     ExecutionEnvironment,
+    NowStrategy,
 )
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.exception import QueryException
 from superlinked.framework.common.util import time_util
 from superlinked.framework.dsl.executor.executor import App
 from superlinked.framework.dsl.query.param_evaluator import ParamEvaluator
 from superlinked.framework.dsl.query.query import QueryObj
@@ -68,21 +69,26 @@
         Returns:
             Result: The result of the query execution that can be inspected and post-proceseed.
 
         Raises:
             QueryException: If the query index is not amongst the executor's indices.
         """
         self.__check_executor_has_index()
-        entities: list[Entity] = self._knn(self._get_query_vector(params))
+        param_evaluator = ParamEvaluator(params)
+        limit = param_evaluator.evaluate_limit_param(self.query_obj.limit_)
+        radius = param_evaluator.evaluate_radius_param(self.query_obj.radius_)
+        # TODO FAI-1838 use self.query_obj.hard_filters in self._knn_search
+        entities: list[Entity] = self._knn(
+            self._get_query_vector(param_evaluator), limit, radius
+        )
         return Result(
             self.query_obj.schema, self._map_entities_to_result_entries(entities)
         )
 
-    def _get_query_vector(self, params: dict[str, Any]) -> Vector:
-        param_evaluator = ParamEvaluator(params)
+    def _get_query_vector(self, param_evaluator: ParamEvaluator) -> Vector:
         query_filters = self._create_query_filters(param_evaluator)
         space_weight_map = self.__get_space_weight_map(param_evaluator)
         return self.query_vector_factory.produce_vector(
             self.query_obj.index._node_id,
             query_filters,
             space_weight_map,
             self.query_obj.schema,
@@ -90,28 +96,32 @@
         )
 
     def _create_query_filters(self, param_evaluator: ParamEvaluator) -> QueryFilters:
         return QueryFilters(self.query_obj.filters, param_evaluator)
 
     def _create_query_context_base(self) -> ExecutionContext:
         eval_context = ExecutionContext(
-            environment=ExecutionEnvironment.QUERY, data=self.app.executor.context.data
+            environment=ExecutionEnvironment.QUERY,
+            data=self.app.executor.context.data,
+            now_strategy=NowStrategy.CONTEXT_TIME,
         )
         eval_context.update_data(
             {CONTEXT_COMMON: {CONTEXT_COMMON_NOW: self.__query_now()}}
         )
         return eval_context
 
-    def _knn(self, vector: Vector) -> list[Entity]:
+    def _knn(
+        self, vector: Vector, limit: int | None, radius: float | None
+    ) -> list[Entity]:
         return self.app.entity_store_manager.knn(
             self.query_obj.index._node_id,
             vector,
             self.query_obj.schema._schema_name,
-            self.query_obj.limit_,
-            self.query_obj.radius_,
+            limit,
+            radius,
         )
 
     def _map_entities_to_result_entries(
         self, entities: list[Entity]
     ) -> list[ResultEntry]:
         return [
             ResultEntry(
@@ -142,9 +152,22 @@
         self, param_evaluator: ParamEvaluator
     ) -> dict[Space, float]:
         return {
             space: param_evaluator.evaluate_weight_param(weight_obj)
             for space, weight_obj in self.query_obj.builder.space_weight_map.items()
         }
 
-    def __query_now(self) -> int:
+    def __check_now(
+        self,
+    ) -> int:
         return self.query_obj._override_now or time_util.now()
+
+    def __query_now(self) -> int:
+        now_ = self.__check_now()
+        if now_ is not None:
+            return now_
+        raise QueryException(
+            (
+                f"Environment's '{CONTEXT_COMMON}.{CONTEXT_COMMON_NOW}' ",
+                "property should always be initialized for query contexts",
+            )
+        )
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/executor/rest/rest_configuration.py` & `superlinked-4.0.1/superlinked/framework/dsl/executor/rest/rest_configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from attr import dataclass
+from dataclasses import dataclass
+
 from pydantic import model_validator
 
 from superlinked.framework.common.util.immutable_model import ImmutableBaseModel
 from superlinked.framework.dsl.executor.rest.rest_descriptor import RestDescriptor
 from superlinked.framework.dsl.query.query import QueryObj
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/executor/rest/rest_descriptor.py` & `superlinked-4.0.1/superlinked/framework/dsl/executor/rest/rest_descriptor.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/executor/rest/rest_executor.py` & `superlinked-4.0.1/superlinked/framework/dsl/executor/rest/rest_executor.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from __future__ import annotations
 
 from typing import Mapping
 
 from superlinked.framework.common.dag.context import ContextValue
 from superlinked.framework.dsl.executor.executor import App, Executor
 from superlinked.framework.dsl.executor.in_memory.in_memory_executor import (
+    InMemoryApp,
     InMemoryExecutor,
 )
 from superlinked.framework.dsl.executor.rest.rest_configuration import (
     RestEndpointConfiguration,
     RestQuery,
 )
 from superlinked.framework.dsl.executor.rest.rest_handler import RestHandler
@@ -102,14 +103,24 @@
             self.__online_app,
             executor._sources,
             executor._queries,
             executor._endpoint_configuration,
         )
 
     @property
+    def online_app(self) -> InMemoryApp:
+        """
+        Property that returns the InMemoryApp instance associated with the RestApp.
+
+        Returns:
+            InMemoryApp: An instance of InMemoryApp.
+        """
+        return self.__online_app
+
+    @property
     def handler(self) -> RestHandler:
         """
         Property that returns the RestHandler instance associated with the RestApp.
 
         Returns:
             RestHandler: An instance of RestHandler.
         """
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/executor/rest/rest_handler.py` & `superlinked-4.0.1/superlinked/framework/dsl/executor/rest/rest_handler.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/index/effect.py` & `superlinked-4.0.1/superlinked/framework/dsl/index/effect.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,9 +39,12 @@
 
     space: Space
     affected_schema_reference: SchemaReference
     affecting_schema_reference: SchemaReference | MultipliedSchemaReference
     filter_: ComparisonOperation[SchemaField]
 
     def __str__(self) -> str:
-        result = f"{self.space}:{self.affected_schema_reference}:{self.affecting_schema_reference}:{self.filter_}"
-        return result
+        return (
+            f"{self.__class__.__name__}(space={self.space}, filter={self.filter_}, "
+            f"affected_schema_reference={self.affected_schema_reference}, "
+            f"affecting_schema_reference={self.affecting_schema_reference})"
+        )
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/index/index.py` & `superlinked-4.0.1/superlinked/framework/dsl/index/index.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Annotated, Sequence
+from typing import Annotated
+
+from beartype.typing import Sequence
 
 from superlinked.framework.common.const import MAX_DAG_DEPTH
 from superlinked.framework.common.dag.concatenation_node import ConcatenationNode
 from superlinked.framework.common.dag.dag import Dag
 from superlinked.framework.common.dag.dag_effect import DagEffect
 from superlinked.framework.common.dag.index_node import IndexNode
 from superlinked.framework.common.dag.node import Node
@@ -24,55 +26,62 @@
 from superlinked.framework.common.exception import (
     InitializationException,
     RecursionException,
     ValidationException,
 )
 from superlinked.framework.common.schema.event_schema_object import EventSchemaObject
 from superlinked.framework.common.schema.id_schema_object import IdSchemaObject
-from superlinked.framework.common.schema.schema_object import SchemaObject
+from superlinked.framework.common.schema.schema_object import SchemaField, SchemaObject
 from superlinked.framework.common.util.type_validator import TypeValidator
 from superlinked.framework.dsl.index.effect import Effect
 from superlinked.framework.dsl.index.util.aggregation_effect_group import (
     AggregationEffectGroup,
 )
 from superlinked.framework.dsl.index.util.aggregation_node_util import (
     AggregationNodeUtil,
 )
 from superlinked.framework.dsl.index.util.effect_with_referenced_schema_object import (
     EffectWithReferencedSchemaObject,
 )
 from superlinked.framework.dsl.space.space import Space
 
+ValidatedSpaceList = Annotated[list[Space], TypeValidator.list_validator(Space)]
+ValidatedSchemaFieldList = Annotated[
+    list[SchemaField], TypeValidator.list_validator(SchemaField)
+]
+ValidatedEffectList = Annotated[list[Effect], TypeValidator.list_validator(Effect)]
+
 
-class Index:
+class Index:  # pylint: disable=too-many-instance-attributes
     """
     An index is an abstraction which represents a collection of spaces that will enable us to query our data.
     """
 
     @TypeValidator.wrap
     def __init__(
         self,
-        spaces: Space | Annotated[list[Space], TypeValidator.list_validator(Space)],
-        effects: (
-            Annotated[list[Effect], TypeValidator.list_validator(Effect)] | None
-        ) = None,
+        spaces: Space | ValidatedSpaceList,
+        fields: SchemaField | ValidatedSchemaFieldList | None = None,
+        effects: ValidatedEffectList | None = None,
     ) -> None:
         """
         Initialize the Index.
 
         Args:
             spaces (Space | list[Space]): The space or list of spaces.
+            fields (SchemaField | list[SchemaField]): The field or list of fields to be indexed.
             effects (list[Effect]): A list of conditional interactions within a `Space`.
             Defaults to None.
 
         Raises:
             InitializationException: If no spaces are provided.
         """
         self.__spaces = self.__init_spaces(spaces)
         self.__space_schemas = self.__init_node_schemas(self.__spaces)
+        self.__fields = self.__init_fields(fields)
         effects_with_schema = self.__init_effects_with_schema(effects, self.__spaces)
         self.__effect_schemas = self.__init_effect_schemas(effects_with_schema)
         self.__node = self.__init_index_node(self.__spaces, effects_with_schema)
         self.__dag_effects = self.__init_dag_effects(effects_with_schema)
         self.__dag = self.__init_dag(self.__node, self.__dag_effects)
         self.__schema_type_schema_mapper = self.__init_schema_type_schema_mapper(
             effects_with_schema
@@ -87,14 +96,18 @@
         return self.__effect_schemas
 
     @property
     def _node(self) -> IndexNode:
         return self.__node
 
     @property
+    def _fields(self) -> Sequence[SchemaField]:
+        return self.__fields
+
+    @property
     def _node_id(self) -> str:
         return self.__node.node_id
 
     @property
     def _dag_effects(self) -> list[DagEffect]:
         return self.__dag_effects
 
@@ -144,14 +157,23 @@
             schema
             for space in validated_spaces
             for node in space._get_all_leaf_nodes()
             for schema in node.schemas
             if not (schema in seen or seen_add(schema))
         ]
 
+    def __init_fields(
+        self, fields: SchemaField | Sequence[SchemaField] | None
+    ) -> Sequence[SchemaField]:
+        if fields is None:
+            return []
+        if not isinstance(fields, Sequence):
+            return [fields]
+        return fields
+
     def __init_effects_with_schema(
         self, effects: list[Effect] | None, spaces: list[Space]
     ) -> list[EffectWithReferencedSchemaObject]:
         if effects is None:
             effects = []
         self.__validate_effects(effects, spaces)
         return [
@@ -190,35 +212,33 @@
         effects: list[EffectWithReferencedSchemaObject],
     ) -> IndexNode:
         index_parents = set[Node[Vector]]()
         for schema in self.__space_schemas:
             if len(spaces) == 1:
                 space = spaces[0]
                 index_parents.add(
-                    self.__init_parent_for_index_or_concatenation(
-                        space, schema, effects
-                    )
+                    self.__init_parent_for_index_or_aggregation(space, schema, effects)
                 )
             else:
                 concatenation_node_parents: list[Node[Vector]] = []
                 for space in spaces:
                     concatenation_node_parents.append(
-                        self.__init_parent_for_index_or_concatenation(
+                        self.__init_parent_for_index_or_aggregation(
                             space, schema, effects
                         )
                     )
                 index_parents.add(ConcatenationNode(concatenation_node_parents))
         return IndexNode(index_parents)
 
     def __init_dag_effects(
         self, effects_with_schema: list[EffectWithReferencedSchemaObject]
     ) -> list[DagEffect]:
         return [effect.dag_effect for effect in effects_with_schema]
 
-    def __init_parent_for_index_or_concatenation(
+    def __init_parent_for_index_or_aggregation(
         self,
         space: Space,
         schema: SchemaObject,
         effects: list[EffectWithReferencedSchemaObject],
     ) -> Node[Vector]:
         filtered_effects = Index.__filter_effects_by_space_and_schema(
             effects=effects,
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/index/util/aggregation_effect_group.py` & `superlinked-4.0.1/superlinked/framework/dsl/index/util/aggregation_effect_group.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/index/util/aggregation_node_util.py` & `superlinked-4.0.1/superlinked/framework/dsl/index/util/aggregation_node_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py` & `superlinked-4.0.1/superlinked/framework/dsl/index/util/effect_with_referenced_schema_object.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py` & `superlinked-4.0.1/superlinked/framework/dsl/index/util/event_aggregation_effect_group.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/index/util/event_aggregation_node_util.py` & `superlinked-4.0.1/superlinked/framework/dsl/index/util/event_aggregation_node_util.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/query/param.py` & `superlinked-4.0.1/superlinked/framework/dsl/query/param.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,8 +31,9 @@
             name (str): The name of the parameter.
         """
         self.name = name
 
 
 ParamInputType: TypeAlias = str | int | float | bool | None
 ParamType: TypeAlias = ParamInputType | Param
-FloatParamType: TypeAlias = float | Param
+NumericParamType: TypeAlias = float | int | Param
+IntParamType: TypeAlias = int | Param
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/query/param_evaluator.py` & `superlinked-4.0.1/superlinked/framework/dsl/query/param_evaluator.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any
 
 from superlinked.framework.common.const import DEFAULT_WEIGHT
 from superlinked.framework.common.exception import QueryException
-from superlinked.framework.dsl.query.param import FloatParamType, Param
+from superlinked.framework.dsl.query.param import IntParamType, NumericParamType, Param
 from superlinked.framework.dsl.query.predicate.binary_predicate import BinaryPredicate
 from superlinked.framework.dsl.query.predicate.evaluated_binary_predicate import (
     EvaluatedBinaryPredicate,
 )
 
 # Exclude from documentation.
 __pdoc__ = {}
@@ -37,26 +37,57 @@
     ) -> list[EvaluatedBinaryPredicate]:
         return [
             self._evaluate_binary_predicate(query_filter) for query_filter in filters
         ]
 
     def evaluate_weight_param(
         self,
-        param: FloatParamType,
+        param: NumericParamType,
         default: float = DEFAULT_WEIGHT,
     ) -> float:
-        value = self._evaluate_param(param, default)
+        value = self.evaluate_numeric_param(param, "Weight", default)
         if value is None:
             return default
+        return value
+
+    def evaluate_radius_param(
+        self,
+        param: NumericParamType | None,
+    ) -> float | None:
+        value = self.evaluate_numeric_param(param, "Radius")
+        if value is not None and (value > 1 or value < 0):
+            raise ValueError(
+                f"Not a valid Radius value ({value}). It should be between 0 and 1."
+            )
+        return value
+
+    def evaluate_numeric_param(
+        self,
+        param: NumericParamType | None,
+        param_name: str,
+        default: float | None = None,
+    ) -> float | None:
+        value = self._evaluate_param(param, default)
         if isinstance(value, (float, int)):
             return float(value)
+        if value is None:
+            return value
         raise QueryException(
-            f"Weight should be numeric, got {value.__class__.__name__}"
+            f"{param_name} should be numeric, got {value.__class__.__name__}"
         )
 
+    def evaluate_limit_param(
+        self,
+        param: IntParamType | None,
+    ) -> int | None:
+        value = self._evaluate_param(param)
+        if value is None or isinstance(value, int):
+            return value
+        raise QueryException(f"Limit should be int, got {value.__class__.__name__}")
+
     def _evaluate_binary_predicate(
         self, predicate: BinaryPredicate
     ) -> EvaluatedBinaryPredicate:
         return EvaluatedBinaryPredicate(
             predicate,
             self.evaluate_weight_param(predicate.weight_param),
             self._evaluate_param(predicate.right_param),
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/query/predicate/binary_op.py` & `superlinked-4.0.1/superlinked/framework/dsl/query/predicate/binary_op.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/query/predicate/binary_predicate.py` & `superlinked-4.0.1/superlinked/framework/dsl/query/predicate/binary_predicate.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.schema.schema_object import SchemaField
-from superlinked.framework.dsl.query.param import FloatParamType, Param
+from superlinked.framework.dsl.query.param import NumericParamType, Param
 from superlinked.framework.dsl.query.predicate.binary_op import BinaryOp
 from superlinked.framework.dsl.query.predicate.query_predicate import QueryPredicate
 
 # Exclude from documentation.
 __pdoc__ = {}
 __pdoc__["BinaryPredicate"] = False
 
 
 class BinaryPredicate(QueryPredicate[BinaryOp]):
     def __init__(
         self,
         op: BinaryOp,
         left_param: SchemaField,
         right_param: Param | str | int | float | None,
-        weight: FloatParamType,
+        weight: NumericParamType,
         left_param_node: Node | None = None,
     ) -> None:
         super().__init__(op=op, params=[left_param, right_param], weight_param=weight)
         self.left_param = left_param
         self.right_param = right_param
         self.left_param_node = left_param_node
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py` & `superlinked-4.0.1/superlinked/framework/dsl/query/predicate/evaluated_binary_predicate.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/query/predicate/query_predicate.py` & `superlinked-4.0.1/superlinked/framework/dsl/query/predicate/query_predicate.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 # limitations under the License.
 
 from dataclasses import dataclass
 from enum import Enum
 from typing import Generic, TypeVar
 
 from superlinked.framework.common.schema.schema_object import SchemaField
-from superlinked.framework.dsl.query.param import FloatParamType, Param
+from superlinked.framework.dsl.query.param import NumericParamType, Param
 
 # Exclude from documentation.
 __pdoc__ = {}
 __pdoc__["QueryPredicate"] = False
 
 # Operation type
 OPT = TypeVar("OPT", bound=Enum)
 
 
 @dataclass(frozen=True)
 class QueryPredicate(Generic[OPT]):
     op: OPT
     params: list[SchemaField | Param | str | int | float | None]
-    weight_param: FloatParamType
+    weight_param: NumericParamType
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/query/query.py` & `superlinked-4.0.1/superlinked/framework/dsl/query/query.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,42 +17,62 @@
 from typing import Annotated, TypedDict, cast
 
 from superlinked.framework.common.const import DEFAULT_WEIGHT
 from superlinked.framework.common.exception import (
     InvalidSchemaException,
     QueryException,
 )
+from superlinked.framework.common.interface.comparison_operand import (
+    ComparisonOperation,
+)
+from superlinked.framework.common.interface.comparison_operation_type import (
+    ComparisonOperationType,
+)
 from superlinked.framework.common.schema.id_schema_object import IdSchemaObject
 from superlinked.framework.common.schema.schema import T
+from superlinked.framework.common.schema.schema_object import SchemaField
+from superlinked.framework.common.util.type_util import get_single_generic_type
 from superlinked.framework.common.util.type_validator import TypeValidator
 from superlinked.framework.dsl.index.index import Index
-from superlinked.framework.dsl.query.param import FloatParamType, ParamType
+from superlinked.framework.dsl.query.param import (
+    IntParamType,
+    NumericParamType,
+    Param,
+    ParamType,
+)
 from superlinked.framework.dsl.query.predicate.binary_op import BinaryOp
 from superlinked.framework.dsl.query.predicate.binary_predicate import BinaryPredicate
 from superlinked.framework.dsl.query.predicate.query_predicate import QueryPredicate
 from superlinked.framework.dsl.space.space import Space
 from superlinked.framework.dsl.space.space_field_set import SpaceFieldSet
 
 # Exclude from documentation.
 __pdoc__ = {}
 __pdoc__["QueryObjInternalProperty"] = False
 
 
+VALID_HARD_FILTER_TYPES = [
+    ComparisonOperationType.EQUAL,
+    ComparisonOperationType.NOT_EQUAL,
+]
+
+
 class QueryObjInternalProperty(TypedDict, total=False):
     """Only intended for self initialization inside QueryObj functions, not for external initialization"""
 
     filters: list[QueryPredicate]
-    limit: int | None
-    radius: float | None
+    limit: IntParamType | None
+    radius: NumericParamType | None
+    hard_filters: list[ComparisonOperation[SchemaField]]
     override_now: int | None
     filtered_spaces: set[Space]
 
 
 @TypeValidator.wrap
-class QueryObj:
+class QueryObj:  # pylint: disable=too-many-instance-attributes
     """
     A class representing a query object. Use .with_vector to run queries using a stored
     vector, or use .similar for queries where you supply the query at query-time. Or combine
     them, or even combine multiple .similar to supply different queries for each space in the
     Index.
 
     Attributes:
@@ -74,14 +94,17 @@
             schema (IdSchemaObject): The schema object.
         """
         self.builder = builder
         self.schema = cast(IdSchemaObject, schema)
         if not internal_property:
             internal_property = {}
         self.filters = internal_property.get("filters", list[QueryPredicate]())
+        self.hard_filters = internal_property.get(
+            "hard_filters", list[ComparisonOperation[SchemaField]]()
+        )
         self.limit_ = internal_property.get("limit")
         self.radius_ = internal_property.get("radius")
         # by default now in queries is the system time, but it can be overridden for testing/reproducible notebooks
         self._override_now = internal_property.get("override_now")
         self.__filtered_spaces = internal_property.get("filtered_spaces", set[Space]())
 
     @property
@@ -94,26 +117,26 @@
     def override_now(self, now: int) -> QueryObj:
         return self.__alter({"override_now": now})
 
     def similar(
         self,
         field_set: SpaceFieldSet,
         param: ParamType,
-        weight: FloatParamType = DEFAULT_WEIGHT,
+        weight: NumericParamType = DEFAULT_WEIGHT,
     ) -> QueryObj:
         """
         Add a 'similar' clause to the query. Similar queries compile query inputs (like query text) into vectors
         using a space and then use the query_vector (weighted with weight param) to search
         in the referenced space of the index.
 
         Args:
             field_set (SpaceFieldSet): The referenced space.
             param (ParamType): The parameter. Basically the query itself. It can be a fixed value,
             or a placeholder (Param) for later substitution.
-            weight (FloatParamType, optional): The weight. Defaults to 1.0.
+            weight (NumericParamType, optional): The weight. Defaults to 1.0.
 
         Returns:
             Self: The query object itself.
 
         Raises:
             QueryException: If the space is already bound in the query.
             InvalidSchemaException: If the schema is not in the similarity field's schema types.
@@ -139,57 +162,53 @@
             return self.__alter(
                 {"filters": filters, "filtered_spaces": filtered_spaces}
             )
         raise InvalidSchemaException(
             f"'find' ({type(self.schema)}) is not in similarity field's schema types."
         )
 
-    def limit(self, limit: int | None) -> QueryObj:
+    def limit(self, limit: IntParamType | None) -> QueryObj:
         """
         Set a limit to the number of results returned by the query.
         If the limit is None, a result set based on all elements in the index will be returned.
 
         Args:
-            limit (int | None): The maximum number of results to return. If None, all results are returned.
+            limit (IntParamType | None): The maximum number of results to return. If None, all results are returned.
 
         Returns:
             Self: The query object itself.
         """
         return self.__alter({"limit": limit})
 
-    def radius(self, radius: float) -> QueryObj:
+    def radius(self, radius: NumericParamType | None) -> QueryObj:
         """
         Set a radius for the search in the query. The radius is a float value that
         determines the maximum distance to the input vector in the search.
         A lower radius value means that the enforced maximum distance is lower,
         therefore closer vectors are returned only.
         A radius of 0.05 means the lowest cosine similarity of items returned to the query vector is 0.95.
         The valid range is between 0 and 1. Otherwise it will raise ValueError.
 
         Args:
-            radius (float): The maximum distance of the returned items from the query vector.
+            radius (NumericParamType | None): The maximum distance of the returned items from the query vector.
+            If None, all results are returned.
 
         Returns:
             Self: The query object itself.
 
         Raises:
             ValueError: If the radius is not between 0 and 1.
         """
-        if radius > 1 or radius < 0:
-            raise ValueError(
-                f"Not a valid radius value ({radius}). It should be between 0 and 1."
-            )
-
         return self.__alter({"radius": radius})
 
     def with_vector(
         self,
         schema_obj: IdSchemaObject | T,
         id_param: ParamType,
-        weight: FloatParamType = DEFAULT_WEIGHT,
+        weight: NumericParamType = DEFAULT_WEIGHT,
     ) -> QueryObj:
         """
         Add a 'with_vector' clause to the query. This fetches an object with id_param
         from the db and uses the vector of that item for search purposes. Weighting
         happens at the space level (and if there is also a .similar query present,
         this part has weight=1 compared to the weight set at .similar for the query
         vector).
@@ -212,14 +231,44 @@
                 left_param=schema_obj.id,
                 right_param=id_param,
                 weight=weight,
             )
         )
         return self.__alter({"filters": filters})
 
+    def filter(
+        self, comparison_operation: ComparisonOperation[SchemaField]
+    ) -> QueryObj:
+        """
+        Add a 'filter' clause to the query. This filters the results from the db
+        to only contain items based on the filtering input.
+        E.g:
+        filter(color_schema.color == "blue")
+        filter(color_schema.color == Param("color_param"))
+        filter(color_schema.color != "red")
+
+        Args:
+            comparison_operation ComparisonOperation[SchemaField]: The comparison operation.
+
+        Returns:
+            Self: The query object itself.
+        """
+        if comparison_operation._op not in VALID_HARD_FILTER_TYPES:
+            raise QueryException(
+                f"Unsupported filter operation: {comparison_operation._op}."
+            )
+        allowed_types = [Param, get_single_generic_type(comparison_operation._operand)]
+        if type(comparison_operation._other) not in allowed_types:
+            raise QueryException(
+                f"Unsupported filter operand type: {comparison_operation._other.__class__.__name__}."
+            )
+        hard_filters = self.hard_filters.copy()
+        hard_filters.append(comparison_operation)
+        return self.__alter({"hard_filters": hard_filters})
+
     def __is_indexed_space(self, space: Space) -> bool:
         return self.builder.index.has_space(space)
 
     def __is_space_bound(self, space: Space) -> bool:
         return space in self.__filtered_spaces
 
     def __alter(self, properties: QueryObjInternalProperty) -> QueryObj:
@@ -241,35 +290,35 @@
 class Query:
     """
     A class representing a query. Build queries using Params as placeholders for weights or query text,
     and supply their value later on when executing a query.
 
     Attributes:
         index (Index): The index.
-        space_weight_map (Mapping[Space, FloatParamType] | None): The mapping of spaces to weights.
+        space_weight_map (Mapping[Space, NumericParamType] | None): The mapping of spaces to weights.
     """
 
     @TypeValidator.wrap
     def __init__(
         self,
         index: Index,
         weights: (
             Annotated[
-                dict[Space, FloatParamType],
-                TypeValidator.dict_validator(Space, FloatParamType),
+                dict[Space, NumericParamType],
+                TypeValidator.dict_validator(Space, NumericParamType),
             ]
             | None
         ) = None,
     ) -> None:
         """
         Initialize the Query.
 
         Args:
             index (Index): The index to be used for the query.
-            weights (Mapping[Space, FloatParamType] | None, optional): The mapping of spaces to weights.
+            weights (Mapping[Space, NumericParamType] | None, optional): The mapping of spaces to weights.
                 Defaults to None, which is equal weight for each space.
         """
         self.index = index
 
         self._queries: list[QueryObj] = []
         self.space_weight_map = weights or {}
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/query/query_filters.py` & `superlinked-4.0.1/superlinked/framework/dsl/query/query_filters.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/query/query_vector_factory.py` & `superlinked-4.0.1/superlinked/framework/dsl/query/query_vector_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from functools import reduce
 from math import sqrt
 from typing import cast
 
 from superlinked.framework.common.dag.context import (
     ExecutionContext,
     ExecutionEnvironment,
+    NowStrategy,
 )
 from superlinked.framework.common.dag.dag import Dag
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.exception import QueryException
 from superlinked.framework.common.parser.parsed_schema import (
     ParsedSchema,
     ParsedSchemaField,
@@ -64,51 +65,31 @@
         looks_like_vector: Vector | None = self._get_looks_like_vector(
             index_node_id, query_filters
         )
         # Generate vector from SIMILAR filters.
         similar_vector: Vector | None = self._get_similar_vector(
             schema, query_filters, context_base
         )
-        # Apply additional weights.
-        vectors: list[Vector | None] = self._apply_vector_weights(
-            looks_like_vector, similar_vector, query_filters
-        )
+        weight_sum = query_filters._get_weight_abs_sum()
         # Aggregate them.
-        vector: Vector = QueryVectorFactory._combine_vectors(vectors)
+        vector: Vector = QueryVectorFactory._combine_vectors(
+            [looks_like_vector, similar_vector], weight_sum
+        )
         # Re-weight by space weights.
         space_node_id_weight_map: dict[str, float] = (
             self.__get_node_id_weight_map_from_space_weight_map(
                 schema, global_space_weight_map
             )
         )
         query_context = self._create_query_context(
             context_base, space_node_id_weight_map
         )
         vector = self._evaluator.re_weight_vector(schema, vector, query_context)
         return vector
 
-    def _apply_vector_weights(
-        self,
-        looks_like_vector: Vector | None,
-        similar_vector: Vector | None,
-        query_filters: QueryFilters,
-    ) -> list[Vector | None]:
-        weight_sum = query_filters._get_weight_abs_sum()
-
-        if looks_like_vector is not None:
-            looks_like_vector = looks_like_vector / weight_sum
-
-        if similar_vector is not None:
-            similar_vector_coefficient = self._get_similar_coefficient(query_filters)
-            if similar_vector_coefficient != 0:
-                similar_vector = similar_vector * similar_vector_coefficient
-                similar_vector = similar_vector / weight_sum
-
-        return [looks_like_vector, similar_vector]
-
     def _get_looks_like_vector(
         self,
         index_node_id: str,
         query_filters: QueryFilters,
     ) -> Vector | None:
         if looks_like_filter := query_filters.looks_like_filter:
             # search by the vector of the referenced entity
@@ -142,36 +123,27 @@
             )
             parsed_schema_fields = (
                 self._build_parsed_schema_fields(query_filters)
                 if similar_filters
                 else []
             )
             parsed_schema = ParsedSchema(schema, "", parsed_schema_fields)
-            evaluation = self._evaluator.evaluate(parsed_schema, query_context)
+            evaluation = self._evaluator.evaluate_single(parsed_schema, query_context)
             return evaluation.main.value
         return None
 
-    def _get_similar_coefficient(
-        self,
-        query_filters: QueryFilters,
-    ) -> float:
-        weights = [filter_.weight for filter_ in query_filters.similar_filters]
-        weight_sum = sum(weights)
-        if weight_sum != 0:
-            weight_pow_sum = sum(weight**2 for weight in weights)
-            return weight_sum / sqrt(weight_pow_sum)
-        return 0
-
     def _create_query_context(
         self,
         context_base: ExecutionContext,
         node_id_weight_map: dict[str, float],
     ) -> ExecutionContext:
         eval_context = ExecutionContext(
-            environment=ExecutionEnvironment.QUERY, data=context_base.data
+            environment=ExecutionEnvironment.QUERY,
+            data=context_base.data,
+            now_strategy=NowStrategy.CONTEXT_TIME,
         )
         eval_context.update_data(
             self._query_weighting.get_node_weights(node_id_weight_map)
         )
         return eval_context
 
     @staticmethod
@@ -191,19 +163,20 @@
             ParsedSchemaField.from_schema_field(
                 filter_.predicate.left_param, filter_.value
             )
             for filter_ in query_filters.similar_filters
         ]
 
     @staticmethod
-    def _combine_vectors(
-        vectors: list[Vector | None],
-    ) -> Vector:
-        if non_none_vectors := [vector for vector in vectors if vector]:
-            return reduce(lambda a, b: a.aggregate(b), non_none_vectors).normalize()
+    def _combine_vectors(vectors: list[Vector | None], weight_sum: float) -> Vector:
+        if non_none_vectors := [
+            vector for vector in vectors if vector and not vector.is_empty
+        ]:
+            aggregation = reduce(lambda a, b: a.aggregate(b), non_none_vectors)
+            return aggregation.normalize(sqrt(weight_sum))
         raise QueryException("No implemented OP provided for the query")
 
     @staticmethod
     def __get_node_id_weight_map_from_filters(
         query_filters: QueryFilters,
     ) -> dict[str, float]:
         return {
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/query/query_weighting.py` & `superlinked-4.0.1/superlinked/framework/dsl/query/query_weighting.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/query/result.py` & `superlinked-4.0.1/superlinked/framework/dsl/query/result.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from dataclasses import dataclass
 from typing import Any
 
+from pandas import DataFrame
+
 from superlinked.framework.common.schema.id_schema_object import IdSchemaObject
 from superlinked.framework.storage.entity import Entity
 
 
 @dataclass(frozen=True)
 class ResultEntry:
     """
@@ -45,12 +47,25 @@
         schema (IdSchemaObject): The schema of the result.
         entries (list[ResultEntry]): A list of result entries.
     """
 
     schema: IdSchemaObject
     entries: list[ResultEntry]
 
+    def to_pandas(self) -> DataFrame:
+        """
+        Converts the query result entries into a pandas DataFrame.
+
+        Each row in the DataFrame corresponds to a single entity in the result, with
+        columns representing the fields of the stored objects.
+
+        Returns:
+            DataFrame: A pandas DataFrame where each row represents a result entity, and
+                each column corresponds to the fields of the stored objects.
+        """
+        return DataFrame([entry.stored_object for entry in self.entries])
+
     def __str__(self) -> str:
         return "\n".join(
             f"#{i+1} id:{entry.entity.id_.object_id}, object:{entry.stored_object}"
             for i, entry in enumerate(self.entries)
         )
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/source/in_memory_source.py` & `superlinked-4.0.1/superlinked/framework/dsl/source/in_memory_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     @property
     def _source(self) -> CommonInMemorySource:
         return self.__source
 
     def put(self, data: list[SourceTypeT]) -> None:
         """
-        Put data into the InMemorySource. This operation can take time as the vectorisation
+        Put data into the InMemorySource. This operation can take time as the vectorization
         of your data happens here.
 
         Args:
             data (list[SourceTypeT]): The data to put.
         """
         for item in data:
             self.__source.put(item)
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/source/rest_source.py` & `superlinked-4.0.1/superlinked/framework/dsl/source/rest_source.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/source/source.py` & `superlinked-4.0.1/superlinked/framework/dsl/source/source.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/space/exception.py` & `superlinked-4.0.1/superlinked/framework/online/dag/exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from superlinked.framework.common.exception import ValidationException
+from superlinked.framework.common.exception import DagEvaluationException
 
 
-class NoDefaultNodeException(ValidationException):
+class ChunkException(DagEvaluationException):
     pass
 
 
-class InvalidSpaceParamException(ValidationException):
+class ValueNotProvidedException(Exception):
     pass
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/space/number_space.py` & `superlinked-4.0.1/superlinked/framework/dsl/space/number_space.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,24 +8,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import cast
+from typing import Mapping, cast
+
+from typing_extensions import override
 
 from superlinked.framework.common.dag.constant_node import ConstantNode
 from superlinked.framework.common.dag.node import Node
-from superlinked.framework.common.dag.number_embedding_node import NumberEmbeddingNode
+from superlinked.framework.common.dag.number_embedding_node import (
+    NumberEmbeddingNode,
+    NumberEmbeddingParams,
+)
 from superlinked.framework.common.dag.number_similarity_node import NumberSimilarityNode
 from superlinked.framework.common.dag.schema_field_node import SchemaFieldNode
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.embedding.number_embedding import Mode
 from superlinked.framework.common.schema.schema_object import Number, SchemaObject
+from superlinked.framework.common.space.aggregation import InputAggregationMode
 from superlinked.framework.dsl.space.exception import (
     InvalidSpaceParamException,
     NoDefaultNodeException,
 )
 from superlinked.framework.dsl.space.space import Space
 from superlinked.framework.dsl.space.space_field_set import SpaceFieldSet
 
@@ -43,134 +49,126 @@
             It is a SchemaFieldObject not regular python ints or floats.
         min_value (float | int): This represents the minimum boundary. Any number lower than
             this will be considered as this minimum value. It can be either a float or an integer.
         max_value (float | int): This represents the maximum boundary. Any number higher than
             this will be considered as this maximum value. It can be either a float or an integer.
         mode (Mode): The mode of the number embedding. Possible values are: maximum, minimum and similar.
             Similar mode expects a .similar on the query, otherwise it will default to maximum.
+        aggregation_mode (InputAggregationMode): The  aggregation mode of the number embedding.
+                Possible values are: maximum, minimum and average.
         negative_filter (float): This is a value that will be set for everything that is equal or
             lower than the min_value. It can be a float. It defaults to 0 (No effect)
 
     Raises:
         InvalidSpaceParamException: If multiple fields of the same schema are in the same space.
             Or the min_value is bigger than the max value, or the negative filter bigger than 0
         InvalidSchemaException: If there's no node corresponding to a given schema.
 
     """
 
-    def __init__(
+    def __init__(  # pylint: disable=too-many-arguments
         self,
         number: Number | list[Number],
         min_value: float | int,
         max_value: float | int,
         mode: Mode,
+        aggregation_mode: InputAggregationMode = InputAggregationMode.INPUT_AVERAGE,
         negative_filter: float = 0.0,
     ) -> None:
         """
         Initializes the NumberSpace object.
 
         Attributes:
             number (SpaceFieldSet): A set of Number objects.
                 These are SchemaFieldObjects not regular python ints or floats.
             min_value (float | int): This represents the minimum boundary. Any number lower than
                 this will be considered as this minimum value. It can be either a float or an integer.
             max_value (float | int): This represents the maximum boundary. Any number higher than
                 this will be considered as this maximum value. It can be either a float or an integer.
             mode (Mode): The mode of the number embedding. Possible values are: maximum, minimum and similar.
                 Similar mode expects a .similar on the query, otherwise it will default to maximum.
+            aggregation_mode (InputAggregationMode): The  aggregation mode of the number embedding.
+                Possible values are: maximum, minimum and average.
             negative_filter (float): This is a value that will be set for everything that is equal or
                 lower than the min_value. It can be a float. It defaults to 0 (No effect)
 
          Raises:
             InvalidSpaceParamException: If multiple fields of the same schema are in the same space.
                 Or the min_value is bigger than the max value, or the negative filter bigger than 0
             InvalidSchemaException: If there's no node corresponding to a given schema.
         """
         super().__init__(number, Number)
         self.__validate_parameters(min_value, max_value, negative_filter)
-        self.min_value: float = float(min_value)
-        self.max_value: float = float(max_value)
-        self.mode: Mode = mode
-        self.negative_filter: float = negative_filter
+        self.aggregation_mode = aggregation_mode
+        self.embedding_params = NumberEmbeddingParams(
+            min_value=float(min_value),
+            max_value=float(max_value),
+            mode=mode,
+            negative_filter=negative_filter,
+        )
         number_node_map = {
-            num: self.__create_node_by_mode(
-                SchemaFieldNode(num),
-                float(self.min_value),
-                float(self.max_value),
-                self.mode,
-                self.negative_filter,
-            )
-            for num in self._field_set
+            num: self.__create_node(SchemaFieldNode(num)) for num in self._field_set
         }
         self.number = SpaceFieldSet(self, set(number_node_map.keys()))
         self.__schema_node_map: dict[SchemaObject, Node] = {
             schema_field.schema_obj: node
             for schema_field, node in number_node_map.items()
         }
         self.default_constant_node_input: int | float | None
-        match self.mode:
+        match mode:
             case Mode.MAXIMUM:
-                self.default_constant_node_input = self.max_value
+                self.default_constant_node_input = max_value
             case Mode.MINIMUM:
-                self.default_constant_node_input = self.min_value
+                self.default_constant_node_input = min_value
             case Mode.SIMILAR:
                 self.default_constant_node_input = None
             case _:
-                raise ValueError(f"Unknown mode: {self.mode}")
+                raise ValueError(f"Unknown mode: {mode}")
 
-    def _get_node(self, schema: SchemaObject) -> Node[Vector]:
-        if node := self.__schema_node_map.get(schema):
-            return node
-        return self.__create_default_node(schema)
+    @property
+    def _node_by_schema(self) -> Mapping[SchemaObject, Node[Vector]]:
+        return self.__schema_node_map
 
-    def _get_all_leaf_nodes(self) -> set[Node[Vector]]:
-        return set(self.__schema_node_map.values())
-
-    def __create_node_by_mode(
+    def __create_node(
         self,
         schema_field_node: SchemaFieldNode,
-        min_value: float,
-        max_value: float,
-        mode: Mode,
-        negative_filter: float,
     ) -> Node:
         return (
             NumberSimilarityNode(
-                schema_field_node, min_value, max_value, negative_filter
-            )
-            if mode == Mode.SIMILAR
-            else NumberEmbeddingNode(
-                schema_field_node, min_value, max_value, mode, negative_filter
+                schema_field_node,
+                self.embedding_params.min_value,
+                self.embedding_params.max_value,
+                self.embedding_params.negative_filter,
+                self.aggregation_mode,
             )
+            if self.embedding_params.mode == Mode.SIMILAR
+            else NumberEmbeddingNode(schema_field_node, self.embedding_params)
         )
 
     def __validate_parameters(
         self, min_value: float | int, max_value: float | int, negative_filter: float
     ) -> None:
         if min_value >= max_value:
             raise InvalidSpaceParamException(
                 f"The maximum value ({max_value}) should be greater than the minimum value ({min_value})."
             )
         if negative_filter > 0:
             raise InvalidSpaceParamException(
                 f"The negative filter value should not be more than 0. Value is: {negative_filter}"
             )
 
-    def __create_default_node(self, schema: SchemaObject) -> NumberEmbeddingNode:
-        if self.mode is Mode.SIMILAR:
+    @override
+    def _handle_node_not_present(self, schema: SchemaObject) -> NumberEmbeddingNode:
+        if self.embedding_params.mode is Mode.SIMILAR:
             raise NoDefaultNodeException(
                 "Number Space with SIMILAR Mode do not have a default value, a .similar "
                 "clause is needed in the query."
             )
         constant_node = cast(
             Node, ConstantNode(value=self.default_constant_node_input, schema=schema)
         )
 
         number_embedding_node = NumberEmbeddingNode(
-            parent=constant_node,
-            min_value=self.min_value,
-            max_value=self.max_value,
-            mode=self.mode,
-            negative_filter=self.negative_filter,
+            constant_node, self.embedding_params
         )
         self.__schema_node_map[schema] = number_embedding_node
         return number_embedding_node
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/space/recency_space.py` & `superlinked-4.0.1/superlinked/framework/dsl/space/recency_space.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,35 +10,40 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 from datetime import timedelta
-from typing import cast
+from typing import Mapping, cast
+
+from typing_extensions import override
 
 from superlinked.framework.common.dag.named_function_node import NamedFunctionNode
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.dag.period_time import PeriodTime
 from superlinked.framework.common.dag.recency_node import RecencyNode
 from superlinked.framework.common.dag.schema_field_node import SchemaFieldNode
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.schema.schema_object import (
     SchemaField,
     SchemaObject,
     Timestamp,
 )
+from superlinked.framework.common.space.aggregation import InputAggregationMode
 from superlinked.framework.common.util.named_function_evaluator import NamedFunction
 from superlinked.framework.dsl.space.space import Space
 from superlinked.framework.dsl.space.space_field_set import SpaceFieldSet
 
 logger = logging.getLogger()
 
+DEFAULT_PERIOD_TIME = PeriodTime(period_time=timedelta(days=14))
+
 
-class RecencySpace(Space):
+class RecencySpace(Space):  # pylint: disable=too-many-instance-attributes
     """
     Recency space encodes timestamp type data measured in seconds and in unix timestamp format.
     Recency space is utilised to encode how recent items are. Use period_time_list
     to mark the time periods of interest.
     Items older than the largest period_time are going to have uniform recency score. (0 or negative_filter if set)
     You can use multiple period_times to give additional emphasis to sub time periods.
     Like using 2 days and 5 days gives extra emphasis to the first 2 days. The extent of which can be controlled with
@@ -49,70 +54,78 @@
     Negative_filter is useful for effectively filtering out entities that are older than the oldest period time.
     You can think of the value of negative_filter as it offsets that amount of similarity stemming from other
     spaces in the index. For example setting it -1 would offset any text similarity that has weight 1 - effectively
     filtering out all old items however similar they are in terms of their text.
 
     Attributes:
         timestamp (SpaceFieldSet): A set of Timestamp objects. The actual data is expected to be unix timestamps
-        in seconds.
-        It is a SchemaFieldObject not regular python ints or floats.
+            in seconds.
+            It is a SchemaFieldObject not regular python ints or floats.
+        time_period_hour_offset (timedelta): Starting period time will be set to this hour.
+            Day will be the next day of context.now(). Defaults to timedelta(hours=0).
         period_time_list (list[PeriodTime] | None): A list of period time parameters.
-        Weights default to 1. Period time to 14 days.
-        timestamp (SpaceFieldSet): A set of Timestamp objects.
-        It is a SchemaFieldObject, not regular python ints or floats.
-        period_time_list (list[PeriodTimeParam] | None): A list of period time parameters.
-        Weights default to 1.0.
-        negative_filter (float): The recency score of items that are older than the oldest period time. Default to 0.0.
+            Weights default to 1. Period time to 14 days.
+        aggregation_mode (InputAggregationMode): The  aggregation mode of the number embedding.
+            Possible values are: maximum, minimum and average. Defaults to InputAggregationMode.INPUT_AVERAGE.
+        negative_filter (float): The recency score of items that are older than the oldest period time. Defaults to 0.0.
     """
 
     def __init__(
         self,
         timestamp: Timestamp | list[Timestamp],
+        time_period_hour_offset: timedelta = timedelta(hours=0),
         period_time_list: list[PeriodTime] | PeriodTime | None = None,
+        aggregation_mode: InputAggregationMode = InputAggregationMode.INPUT_AVERAGE,
         negative_filter: float = 0.0,
     ) -> None:
         """
         Initialize the RecencySpace.
 
         Args:
-            timestamp (Timestamp | list[Timestamp]): A timestamp or a list of timestamps.
-            period_time_list (list[PeriodTime] | None, optional): A list of period time parameters.
-            Defaults to None.
-            negative_filter (float): The recency score attributed to items older than the largest period_time value.
-            Defaults to 0.0.
+            timestamp (SpaceFieldSet): A set of Timestamp objects. The actual data is expected to be unix timestamps
+                in seconds.
+                It is a SchemaFieldObject not regular python ints or floats.
+            time_period_hour_offset (timedelta): Starting period time will be set to this hour.
+                Day will be the next day of context.now(). Defaults to timedelta(hours=0).
+            period_time_list (list[PeriodTime] | None): A list of period time parameters.
+                Weights default to 1. Period time to 14 days.
+            aggregation_mode (InputAggregationMode): The  aggregation mode of the number embedding.
+                Possible values are: maximum, minimum and average. Defaults to InputAggregationMode.INPUT_AVERAGE.
+            negative_filter (float): The recency score of items that are older than the oldest period time.
+                Defaults to 0.0.
         """
         super().__init__(timestamp, Timestamp)
         self.timestamp = SpaceFieldSet(self, cast(set[SchemaField], self._field_set))
         self.period_time_list: list[PeriodTime] = (
             period_time_list
             if isinstance(period_time_list, list)
             else (
                 [period_time_list]
                 if period_time_list is not None
-                else [PeriodTime(period_time=timedelta(days=14))]
+                else [DEFAULT_PERIOD_TIME]
             )
         )
         self.negative_filter = negative_filter
+        self.time_period_hour_offset = time_period_hour_offset
+        self.__aggregation_mode: InputAggregationMode = aggregation_mode
         self.__run_parameter_checks()
         self.__schema_node_map: dict[SchemaObject, RecencyNode] = {
             field.schema_obj: RecencyNode(
                 SchemaFieldNode(field),
+                self.time_period_hour_offset,
                 self.period_time_list,
+                self.__aggregation_mode,
                 self.negative_filter,
             )
             for field in self.timestamp.fields
         }
 
-    def _get_node(self, schema: SchemaObject) -> Node[Vector]:
-        if (node := self.__schema_node_map.get(schema)) is not None:
-            return node
-        return self.__create_default_node(schema)
-
-    def _get_all_leaf_nodes(self) -> set[Node[Vector]]:
-        return set(self.__schema_node_map.values())
+    @property
+    def _node_by_schema(self) -> Mapping[SchemaObject, Node[Vector]]:
+        return self.__schema_node_map
 
     def __run_parameter_checks(self) -> None:
         if self.negative_filter > 0:
             sum_weights: float = sum(param.weight for param in self.period_time_list)
 
             max_period_time: timedelta = max(
                 param.period_time for param in self.period_time_list
@@ -141,14 +154,19 @@
                 "recency score curves. Use with caution. \n"
                 "To better understand your recency scores use RecencyPlotter."
                 "It can be imported from `superlinked.evaluation.charts.recency_plotter`. \n"
                 "Check an example notebook at: https://github.com/superlinked/superlinked/blob/main"
                 "/notebook/combining_recency_and_relevance.ipynb. "
             )
 
-    def __create_default_node(self, schema: SchemaObject) -> RecencyNode:
+    @override
+    def _handle_node_not_present(self, schema: SchemaObject) -> RecencyNode:
         named_function_node = NamedFunctionNode(NamedFunction.NOW, schema, int)
         recency_node = RecencyNode(
-            named_function_node, self.period_time_list, self.negative_filter
+            named_function_node,
+            self.time_period_hour_offset,
+            self.period_time_list,
+            self.__aggregation_mode,
+            self.negative_filter,
         )
         self.__schema_node_map[schema] = recency_node
         return recency_node
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/space/space.py` & `superlinked-4.0.1/superlinked/framework/dsl/space/space.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import TypeVar
+from typing import Mapping, TypeVar
 
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.data_types import Vector
-from superlinked.framework.common.schema.schema_object import SchemaField, SchemaObjectT
+from superlinked.framework.common.exception import InvalidSchemaException
+from superlinked.framework.common.schema.schema_object import SchemaField, SchemaObject
 from superlinked.framework.common.util.type_validator import TypeValidator
 from superlinked.framework.dsl.space.exception import InvalidSpaceParamException
 
 # SpaceInputType
 SIT = TypeVar("SIT", bound=SchemaField)
 
 
@@ -48,14 +49,23 @@
             for schema in schema_list
             if schema_list.count(schema) > 1
         ]:
             raise InvalidSpaceParamException(
                 f"Duplicates schemas in the same space are not allowed. Duplicates: {duplicates}"
             )
 
+    @property
     @abstractmethod
-    def _get_node(self, schema: SchemaObjectT) -> Node[Vector]:
-        pass
+    def _node_by_schema(self) -> Mapping[SchemaObject, Node[Vector]]: ...
+
+    def _get_node(self, schema: SchemaObject) -> Node[Vector]:
+        if node := self._node_by_schema.get(schema):
+            return node
+        return self._handle_node_not_present(schema)
+
+    def _handle_node_not_present(self, schema: SchemaObject) -> Node[Vector]:
+        raise InvalidSchemaException(
+            f"There's no node corresponding to this schema: {schema._schema_name}"
+        )
 
-    @abstractmethod
     def _get_all_leaf_nodes(self) -> set[Node[Vector]]:
-        pass
+        return set(self._node_by_schema.values())
```

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/space/space_field_set.py` & `superlinked-4.0.1/superlinked/framework/dsl/space/space_field_set.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/dsl/space/text_similarity_space.py` & `superlinked-4.0.1/superlinked/framework/dsl/space/text_similarity_space.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,22 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import cast
+from typing import Mapping, cast
 
 from superlinked.framework.common.dag.chunking_node import ChunkingNode
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.dag.schema_field_node import SchemaFieldNode
 from superlinked.framework.common.dag.text_embedding_node import TextEmbeddingNode
 from superlinked.framework.common.data_types import Vector
-from superlinked.framework.common.exception import InvalidSchemaException
 from superlinked.framework.common.schema.schema_object import SchemaObject, String
 from superlinked.framework.common.util.type_validator import TypeValidator
 from superlinked.framework.dsl.space.space import Space
 from superlinked.framework.dsl.space.space_field_set import SpaceFieldSet
 
 TextInput = String | ChunkingNode
 
@@ -65,42 +64,54 @@
         if isinstance(text, String):
             return text
         if isinstance(text, SchemaFieldNode):
             return cast(String, text.schema_field)
         return self.__get_root(text.parents[0])
 
     def __generate_embedding_node(
-        self, text: TextInput, model: str
+        self,
+        text: TextInput,
+        model: str,
     ) -> TextEmbeddingNode:
         if isinstance(text, ChunkingNode):
             return TextEmbeddingNode(text, model)
         return TextEmbeddingNode(SchemaFieldNode(text), model)
 
-    def _get_node(self, schema: SchemaObject) -> Node[Vector]:
-        if node := self.__schema_node_map.get(schema):
-            return node
-        raise InvalidSchemaException(
-            f"There's no node corresponding to this schema: {schema._schema_name}"
-        )
-
-    def _get_all_leaf_nodes(self) -> set[Node[Vector]]:
-        return set(self.__schema_node_map.values())
+    @property
+    def _node_by_schema(self) -> Mapping[SchemaObject, Node[Vector]]:
+        return self.__schema_node_map
 
 
 @TypeValidator.wrap
 def chunk(
-    text: String, chunk_size: int | None = None, chunk_overlap: int | None = None
+    text: String,
+    chunk_size: int | None = None,
+    chunk_overlap: int | None = None,
+    split_chars_keep: list[str] | None = None,
+    split_chars_remove: list[str] | None = None,
 ) -> ChunkingNode:
     """
     Create smaller chunks from the given text, a String SchemaFieldObject. It is helpful when you search
     for more granular information in your text corpus. It is recommended to try different chunk_sizes to
     find what fits best your use-case. Chunking respects word boundaries.
 
     Args:
-        text (String): The text to chunk.
-        chunk_size (int | None, optional): The maximum size of each chunk in characters. Defaults to None.
-        chunk_overlap (int | None, optional): The maximum overlap between chunks in characters. Defaults to None.
+        text (String): The String field the text of which is to be chunked.
+        chunk_size (int | None, optional): The maximum size of each chunk in characters. Defaults to None, which means
+        effectively using 250.
+        chunk_overlap (int | None, optional): The maximum overlap between chunks in characters. Defaults to None, which
+        means effectively using {}.
+        split_chars_keep: Characters to split at, but also keep in the text. Should be characters that can signal
+        meaningful breakpoints in the text. Effectively defaults to ["!", "?", "."].
+        split_chars_remove: Characters to split at and remove from the text. Should be characters that can signal
+        meaningful breakpoints in the text. Effectively defaults to ["\n"].
 
     Returns:
         ChunkingNode: The chunking node.
     """
-    return ChunkingNode(SchemaFieldNode(text), chunk_size, chunk_overlap)
+    return ChunkingNode(
+        SchemaFieldNode(text),
+        chunk_size,
+        chunk_overlap,
+        split_chars_keep,
+        split_chars_remove,
+    )
```

### Comparing `superlinked-3.9.1/superlinked/framework/evaluator/dag_evaluator.py` & `superlinked-4.0.1/superlinked/framework/common/interface/weighted.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,21 +8,22 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from abc import ABC, abstractmethod
+from dataclasses import dataclass
 from typing import Generic, TypeVar
 
-from superlinked.framework.common.dag.context import ExecutionContext
-from superlinked.framework.common.parser.parsed_schema import ParsedSchema
+from superlinked.framework.common.const import DEFAULT_WEIGHT
 
-# Dag evaluation result type
-DERT = TypeVar("DERT")
+WT = TypeVar("WT")
 
 
-class DagEvaluator(ABC, Generic[DERT]):
-    @abstractmethod
-    def evaluate(self, parsed_schema: ParsedSchema, context: ExecutionContext) -> DERT:
-        pass
+@dataclass
+class Weighted(Generic[WT]):
+    item: WT
+    weight: float = DEFAULT_WEIGHT
+
+    def __str__(self) -> str:
+        return f"{self.__class__.__name__}(item={self.item}, weight={self.weight})"
```

### Comparing `superlinked-3.9.1/superlinked/framework/evaluator/online_dag_evaluator.py` & `superlinked-4.0.1/superlinked/framework/evaluator/online_dag_evaluator.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from superlinked.framework.common.dag.dag_effect import DagEffect
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.exception import (
     InvalidDagEffectException,
     InvalidSchemaException,
 )
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
+from superlinked.framework.common.schema.id_schema_object import IdSchemaObject
 from superlinked.framework.common.schema.schema_object import SchemaObject
 from superlinked.framework.compiler.online_schema_dag_compiler import (
     OnlineSchemaDagCompiler,
 )
 from superlinked.framework.evaluator.dag_evaluator import DagEvaluator
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.online_schema_dag import OnlineSchemaDag
@@ -54,41 +55,50 @@
         )
         self._dag_effect_online_schema_dag_mapper = (
             self.__init_dag_effect_online_schema_dag_mapper(
                 self._dag, self._evaluation_result_store_manager
             )
         )
 
+    def __get_single_schema(self, parsed_schemas: list[ParsedSchema]) -> IdSchemaObject:
+        unique_schemas: set[IdSchemaObject] = {
+            parsed_schema.schema for parsed_schema in parsed_schemas
+        }
+        if len(unique_schemas) != 1:
+            raise InvalidSchemaException(
+                f"Multiple schemas ({[s._schema_name for s in unique_schemas]}) present in the index."
+            )
+        return next(iter(unique_schemas))
+
     def evaluate(
         self,
-        parsed_schema: ParsedSchema,
+        parsed_schemas: list[ParsedSchema],
         context: ExecutionContext,
-    ) -> EvaluationResult[Vector]:
+    ) -> list[EvaluationResult[Vector]]:
+        index_schema = self.__get_single_schema(parsed_schemas)
         if (
-            online_schema_dag := self._schema_online_schema_dag_mapper.get(
-                parsed_schema.schema
-            )
+            online_schema_dag := self._schema_online_schema_dag_mapper.get(index_schema)
         ) is not None:
-            return online_schema_dag.evaluate(parsed_schema, context)
+            return online_schema_dag.evaluate(parsed_schemas, context)
         raise InvalidSchemaException(
-            f"Schema ({parsed_schema.schema._schema_name}) isn't present in the index."
+            f"Schema ({index_schema._schema_name}) isn't present in the index."
         )
 
     def evaluate_by_dag_effect(
         self,
         parsed_schema: ParsedSchema,
         context: ExecutionContext,
         dag_effect: DagEffect,
     ) -> EvaluationResult[Vector]:
         if (
             online_schema_dag := self._dag_effect_online_schema_dag_mapper.get(
                 dag_effect
             )
         ) is not None:
-            return online_schema_dag.evaluate(parsed_schema, context)
+            return online_schema_dag.evaluate([parsed_schema], context)[0]
         raise InvalidDagEffectException(
             f"DagEffect ({dag_effect}) isn't present in the index."
         )
 
     def __init_schema_online_schema_dag_mapper(
         self,
         schemas: set[SchemaObject],
```

### Comparing `superlinked-3.9.1/superlinked/framework/evaluator/query_dag_evaluator.py` & `superlinked-4.0.1/superlinked/framework/evaluator/query_dag_evaluator.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,36 +8,34 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.exception import (
     DagEvaluationException,
     InvalidSchemaException,
 )
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
 from superlinked.framework.common.schema.schema_object import SchemaObject
 from superlinked.framework.evaluator.online_dag_evaluator import OnlineDagEvaluator
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 
 
 class QueryDagEvaluator(OnlineDagEvaluator):
-    @override
-    def evaluate(
+    def evaluate_single(
         self,
         parsed_schema: ParsedSchema,
         context: ExecutionContext,
     ) -> EvaluationResult[Vector]:
-        result = super().evaluate(parsed_schema, context)
+        result = super().evaluate([parsed_schema], context)[0]
         QueryDagEvaluator.__check_evaluation(result)
         return result
 
     @staticmethod
     def __check_evaluation(evaluation: EvaluationResult[Vector]) -> None:
         if len(evaluation.chunks) > 0:
             raise DagEvaluationException(
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/dag/evaluation_result.py` & `superlinked-4.0.1/superlinked/framework/online/dag/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/online/dag/exception.py` & `superlinked-4.0.1/superlinked/framework/dsl/space/exception.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from superlinked.framework.common.exception import DagEvaluationException
+from superlinked.framework.common.exception import ValidationException
 
 
-class ParentCountException(DagEvaluationException):
+class NoDefaultNodeException(ValidationException):
     pass
 
 
-class ChunkException(DagEvaluationException):
+class InvalidSpaceParamException(ValidationException):
     pass
 
 
-class ValueNotProvidedException(Exception):
+class InvalidAggregationStrategyException(ValidationException):
     pass
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/dag/online_aggregation_node.py` & `superlinked-4.0.1/superlinked/framework/online/dag/online_aggregation_node.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,83 +10,112 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from functools import reduce
 from typing import cast
 
+from beartype.typing import Sequence
+from typing_extensions import override
+
 from superlinked.framework.common.dag.aggregation_node import AggregationNode
 from superlinked.framework.common.dag.context import ExecutionContext
+from superlinked.framework.common.dag.exception import ParentCountException
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.exception import (
     MismatchingDimensionException,
     ValidationException,
 )
+from superlinked.framework.common.interface.has_aggregation import HasAggregation
 from superlinked.framework.common.interface.has_length import HasLength
+from superlinked.framework.common.space.aggregation import Aggregation
 from superlinked.framework.online.dag.default_online_node import DefaultOnlineNode
 from superlinked.framework.online.dag.evaluation_result import SingleEvaluationResult
-from superlinked.framework.online.dag.exception import ParentCountException
 from superlinked.framework.online.dag.online_node import OnlineNode
+from superlinked.framework.online.dag.parent_validator import ParentValidationType
 from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
     EvaluationResultStoreManager,
 )
 
 
 class OnlineAggregationNode(DefaultOnlineNode[AggregationNode, Vector], HasLength):
     def __init__(
         self,
         node: AggregationNode,
         parents: list[OnlineNode],
         evaluation_result_store_manager: EvaluationResultStoreManager,
     ) -> None:
-        super().__init__(node, parents, evaluation_result_store_manager)
+        super().__init__(
+            node,
+            parents,
+            evaluation_result_store_manager,
+            ParentValidationType.AT_LEAST_ONE_PARENT,
+        )
         OnlineAggregationNode.__validate_parents(parents)
 
-    @classmethod
-    def from_node(
-        cls,
-        node: AggregationNode,
-        parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
-    ) -> OnlineAggregationNode:
-        return cls(node, parents, evaluation_result_store_manager)
-
-    @classmethod
-    def get_node_type(cls) -> type[AggregationNode]:
-        return AggregationNode
-
     @property
     def length(self) -> int:
         return self.node.length
 
     @classmethod
     def __validate_parents(cls, parents: list[OnlineNode]) -> None:
-        if len(parents) == 0:
-            raise ParentCountException(f"{cls.__name__} must have at least 1 parent.")
         length = cast(HasLength, parents[0]).length
         if any(
             parent for parent in parents if cast(HasLength, parent).length != length
         ):
             raise ValidationException(
                 f"{cls.__name__} must have parents with the same length."
             )
 
+    @override
+    def _evaluate_singles(
+        self,
+        parent_results: list[dict[OnlineNode, SingleEvaluationResult]],
+        context: ExecutionContext,
+    ) -> Sequence[Vector | None]:
+        return [
+            self._evaluate_single(parent_result, context)
+            for parent_result in parent_results
+        ]
+
     def _evaluate_single(
         self,
         parent_results: dict[OnlineNode, SingleEvaluationResult],
         context: ExecutionContext,
     ) -> Vector:
         self._check_evaluation_inputs(parent_results)
         weighted_vectors = self._get_weighted_vectors(parent_results)
-        aggregation = reduce(lambda a, b: a.aggregate(b), weighted_vectors)
-        return aggregation.normalize()
+        return self.__get_aggregation(parent_results).aggregate(
+            weighted_vectors, context
+        )
+
+    def __get_aggregation(
+        self, parent_results: dict[OnlineNode, SingleEvaluationResult]
+    ) -> Aggregation:
+        aggregations: list[Aggregation] = [
+            online_node.node.aggregation
+            for online_node in parent_results.keys()
+            if isinstance(online_node.node, HasAggregation)
+        ]
+        if not aggregations:
+            raise ValidationException("No Aggregation set.")
+        if not all(
+            aggregation.normalization == aggregations[0].normalization
+            for aggregation in aggregations
+        ):
+            aggregation_class_names = [
+                str(aggregation.__class__) for aggregation in aggregations
+            ]
+            raise ValidationException(
+                f"Cannot aggregate with different Aggregations: {str(aggregation_class_names)}."
+            )
+        return aggregations[0]
 
     def _check_evaluation_inputs(
         self,
         parent_results: dict[OnlineNode, SingleEvaluationResult],
     ) -> None:
         invalid_type_result_types = [
             result.__class__.__name__
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/dag/online_chunking_node.py` & `superlinked-4.0.1/superlinked/framework/online/dag/online_chunking_node.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,81 +18,77 @@
 
 from typing_extensions import override
 
 from superlinked.framework.common.dag.chunking_node import ChunkingNode
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.embedding.chunking_util import Chunker
-from superlinked.framework.common.exception import (
-    DagEvaluationException,
-    InitializationException,
-)
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.exception import ChunkException
 from superlinked.framework.online.dag.online_node import OnlineNode
+from superlinked.framework.online.dag.parent_validator import ParentValidationType
 from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
     EvaluationResultStoreManager,
 )
 
 
 class OnlineChunkingNode(OnlineNode[ChunkingNode, str]):
     def __init__(
         self,
         node: ChunkingNode,
-        parent: OnlineNode[Node[str], str],
+        parents: list[OnlineNode[Node[str], str]],
         evaluation_result_store_manager: EvaluationResultStoreManager,
     ) -> None:
-        super().__init__(node, [parent], evaluation_result_store_manager)
-
-    @classmethod
-    def from_node(
-        cls,
-        node: ChunkingNode,
-        parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
-    ) -> OnlineChunkingNode:
-        if len(parents) != 1:
-            raise InitializationException(f"{cls.__name__} must have exactly 1 parent.")
-        return cls(node, parents[0], evaluation_result_store_manager)
-
-    @classmethod
-    def get_node_type(cls) -> type[ChunkingNode]:
-        return ChunkingNode
+        super().__init__(
+            node,
+            parents,
+            evaluation_result_store_manager,
+            ParentValidationType.EXACTLY_ONE_PARENT,
+        )
 
     def __chunk(
-        self, text: str, chunk_size: int | None, chunk_overlap: int | None
+        self,
+        text: str,
+        chunk_size: int | None,
+        chunk_overlap: int | None,
+        split_chars_keep: list[str] | None = None,
+        split_chars_remove: list[str] | None = None,
     ) -> list[str]:
         chunker = Chunker()
-        return chunker.chunk_text(text, chunk_size, chunk_overlap)
+        return chunker.chunk_text(
+            text, chunk_size, chunk_overlap, split_chars_keep, split_chars_remove
+        )
 
     @override
     def evaluate_self(
         self,
+        parsed_schemas: list[ParsedSchema],
+        context: ExecutionContext,
+    ) -> list[EvaluationResult[str]]:
+        return [self.evaluate_self_single(schema, context) for schema in parsed_schemas]
+
+    def evaluate_self_single(
+        self,
         parsed_schema: ParsedSchema,
         context: ExecutionContext,
     ) -> EvaluationResult[str]:
-        if len(self.parents) != 1:
-            stored_result = self.load_stored_result(
-                parsed_schema.id_, parsed_schema.schema
-            )
-            if stored_result is None:
-                raise DagEvaluationException(
-                    f"{self.class_name} doesn't have a stored result."
-                )
-            return EvaluationResult(self._get_single_evaluation_result(stored_result))
         input_: EvaluationResult[str] = cast(
             OnlineNode[Node[str], str], self.parents[0]
-        ).evaluate_next(parsed_schema, context)
+        ).evaluate_next_single(parsed_schema, context)
         if len(input_.chunks) > 0:
             # We can just log a warning and proceed with input_.main.
             raise ChunkException(f"{self.class_name} cannot have a chunked input.")
         input_value = input_.main.value
         chunk_inputs = self.__chunk(
-            input_value, self.node.chunk_size, self.node.chunk_overlap
+            input_value,
+            self.node.chunk_size,
+            self.node.chunk_overlap,
+            self.node.split_chars_keep,
+            self.node.split_chars_remove,
         )
         main = self._get_single_evaluation_result(input_value)
         chunks = [
             self._get_single_evaluation_result(chunk_input)
             for chunk_input in chunk_inputs
         ]
         return EvaluationResult(main, chunks)
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/dag/online_comparison_filter_node.py` & `superlinked-4.0.1/superlinked/framework/online/dag/online_comparison_filter_node.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,51 +10,51 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from beartype.typing import Sequence
+from typing_extensions import override
+
 from superlinked.framework.common.dag.comparison_filter_node import ComparisonFilterNode
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.online.dag.default_online_node import DefaultOnlineNode
 from superlinked.framework.online.dag.evaluation_result import SingleEvaluationResult
-from superlinked.framework.online.dag.exception import ParentCountException
 from superlinked.framework.online.dag.online_node import OnlineNode
+from superlinked.framework.online.dag.parent_validator import ParentValidationType
 from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
     EvaluationResultStoreManager,
 )
 
 
 class OnlineComparisonFilterNode(DefaultOnlineNode[ComparisonFilterNode, bool]):
     def __init__(
         self,
         node: ComparisonFilterNode,
-        parent: OnlineNode,
+        parents: list[OnlineNode],
         evaluation_result_store_manager: EvaluationResultStoreManager,
     ) -> None:
-        super().__init__(node, [parent], evaluation_result_store_manager)
+        super().__init__(
+            node,
+            parents,
+            evaluation_result_store_manager,
+            ParentValidationType.EXACTLY_ONE_PARENT,
+        )
 
-    @classmethod
-    def from_node(
-        cls,
-        node: ComparisonFilterNode,
-        parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
-    ) -> OnlineComparisonFilterNode:
-        if len(parents) != 1:
-            raise ParentCountException(f"{cls.__name__} must have exactly 1 parent.")
-        return cls(node, parents[0], evaluation_result_store_manager)
-
-    @classmethod
-    def get_node_type(cls) -> type[ComparisonFilterNode]:
-        return ComparisonFilterNode
+    @override
+    def _evaluate_singles(
+        self,
+        parent_results: list[dict[OnlineNode, SingleEvaluationResult]],
+        context: ExecutionContext,
+    ) -> Sequence[bool | None]:
+        return [
+            self._evaluate_single(parent_result) for parent_result in parent_results
+        ]
 
     def _evaluate_single(
         self,
         parent_results: dict[OnlineNode, SingleEvaluationResult],
-        context: ExecutionContext,
-    ) -> bool | None:
-        if len(parent_results) != 1:
-            raise ParentCountException(f"{self.class_name} must have exactly 1 parent.")
+    ) -> bool:
         parent_result: SingleEvaluationResult = list(parent_results.values())[0]
         return self.node.comparison_operation.evaluate(parent_result.value)
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/dag/online_concatenation_node.py` & `superlinked-4.0.1/superlinked/framework/online/dag/online_concatenation_node.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,106 +10,115 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from math import sqrt
 from typing import cast
 
+from beartype.typing import Sequence
+from typing_extensions import override
+
 from superlinked.framework.common.dag.concatenation_node import ConcatenationNode
 from superlinked.framework.common.dag.context import (
     SPACE_WEIGHT_PARAM_NAME,
     ExecutionContext,
 )
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.exception import ValidationException
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.online.dag.default_online_node import DefaultOnlineNode
 from superlinked.framework.online.dag.evaluation_result import SingleEvaluationResult
-from superlinked.framework.online.dag.exception import ParentCountException
 from superlinked.framework.online.dag.online_node import OnlineNode
+from superlinked.framework.online.dag.parent_validator import ParentValidationType
 from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
     EvaluationResultStoreManager,
 )
 
 
 class OnlineConcatenationNode(DefaultOnlineNode[ConcatenationNode, Vector], HasLength):
     def __init__(
         self,
         node: ConcatenationNode,
         parents: list[OnlineNode],
         evaluation_result_store_manager: EvaluationResultStoreManager,
     ) -> None:
-        super().__init__(node, parents, evaluation_result_store_manager)
-
-    @classmethod
-    def from_node(
-        cls,
-        node: ConcatenationNode,
-        parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
-    ) -> OnlineConcatenationNode:
-        if len(parents) == 0:
-            raise ParentCountException(f"{cls.__name__} must have at least 1 parent.")
-        return cls(node, parents, evaluation_result_store_manager)
-
-    @classmethod
-    def get_node_type(cls) -> type[ConcatenationNode]:
-        return ConcatenationNode
+        super().__init__(
+            node,
+            parents,
+            evaluation_result_store_manager,
+            ParentValidationType.AT_LEAST_ONE_PARENT,
+        )
 
     @property
     def length(self) -> int:
         return self.node.length
 
-    def _evaluate_single(
+    @override
+    def _evaluate_singles(
         self,
-        parent_results: dict[OnlineNode, SingleEvaluationResult],
+        parent_results: list[dict[OnlineNode, SingleEvaluationResult]],
         context: ExecutionContext,
-    ) -> Vector:
+    ) -> Sequence[Vector | None]:
         self.__check_evaluation_inputs(parent_results)
-        vector = sum(
-            [
-                self.__apply_vector_weight(result.value, parent.node_id, context)
-                for parent, result in parent_results.items()
-            ],
-            Vector([]),
-        )
-        return vector if context.is_query_context() else vector.normalize()
+        vectors = [
+            sum(
+                [
+                    self.__apply_vector_weight(result.value, parent.node_id, context)
+                    for parent, result in parent_result.items()
+                ],
+                Vector([]),
+            )
+            for parent_result in parent_results
+        ]
+        weight_sum = self._get_weight_abs_sum(context)
+        return [
+            (
+                vector
+                if context.is_query_context()
+                else vector.normalize(sqrt(weight_sum))
+            )
+            for vector in vectors
+        ]
 
     def re_weight_vector(
         self,
         vector: Vector,
         context: ExecutionContext,
     ) -> Vector:
-        if len(self.parents) == 0:
-            raise ParentCountException(
-                f"{self.class_name} must have at least 1 parent."
-            )
         parts = self._split_vector(vector)
         vector = sum(
             [
                 self.__apply_vector_weight(part, parent.node_id, context)
                 for part, parent in zip(parts, self.parents)
             ],
             Vector([]),
         )
-        return vector.normalize()
+        weight_sum = self._get_weight_abs_sum(context)
+        return vector.normalize(sqrt(weight_sum))
+
+    def _get_weight_abs_sum(
+        self,
+        context: ExecutionContext,
+    ) -> float:
+        return sum(
+            abs(self.__get_weight_of_node(parent.node_id, context))
+            for parent in self.parents
+        )
 
     def __check_evaluation_inputs(
         self,
-        parent_results: dict[OnlineNode, SingleEvaluationResult],
+        parent_results: list[dict[OnlineNode, SingleEvaluationResult]],
     ) -> None:
-        if len(parent_results.items()) == 0:
-            raise ParentCountException(
-                f"{self.class_name} must have at least 1 parent."
-            )
         invalid_results = [
             result
-            for _, result in parent_results.items()
+            for parent_result in parent_results
+            for result in parent_result.values()
             if not isinstance(result.value, Vector)
         ]
         if len(invalid_results) != 0:
             raise ValidationException(
                 f"{self.class_name} can only process `Vector` inputs."
             )
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/dag/online_constant_node.py` & `superlinked-4.0.1/superlinked/framework/online/dag/online_constant_node.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,48 +10,50 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from typing_extensions import override
+
 from superlinked.framework.common.dag.constant_node import ConstantNode
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.node import NDT
-from superlinked.framework.common.exception import InitializationException
-from superlinked.framework.online.dag.default_online_node import DefaultOnlineNode
-from superlinked.framework.online.dag.evaluation_result import SingleEvaluationResult
+from superlinked.framework.common.parser.parsed_schema import ParsedSchema
+from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.online_node import OnlineNode
+from superlinked.framework.online.dag.parent_validator import ParentValidationType
 from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
     EvaluationResultStoreManager,
 )
 
 
-class OnlineConstantNode(DefaultOnlineNode[ConstantNode[NDT], NDT]):
+class OnlineConstantNode(OnlineNode[ConstantNode[NDT], NDT]):
     def __init__(
         self,
         node: ConstantNode,
+        parents: list[OnlineNode],
         evaluation_result_store_manager: EvaluationResultStoreManager,
     ) -> None:
-        super().__init__(node, [], evaluation_result_store_manager)
+        super().__init__(
+            node,
+            parents,
+            evaluation_result_store_manager,
+            ParentValidationType.NO_PARENTS,
+        )
 
-    @classmethod
-    def from_node(
-        cls,
-        node: ConstantNode,
-        parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
-    ) -> OnlineConstantNode:
-        if len(parents) != 0:
-            raise InitializationException(f"{cls.__name__} cannot have parents.")
-        return cls(node, evaluation_result_store_manager)
-
-    @classmethod
-    def get_node_type(cls) -> type[ConstantNode]:
-        return ConstantNode
+    @override
+    def evaluate_self(
+        self,
+        parsed_schemas: list[ParsedSchema],
+        context: ExecutionContext,
+    ) -> list[EvaluationResult[NDT]]:
+        result = EvaluationResult(
+            self._get_single_evaluation_result(self._evaluate_single())
+        )
+        return [result for _ in parsed_schemas]
 
     def _evaluate_single(
         self,
-        parent_results: dict[OnlineNode, SingleEvaluationResult],
-        context: ExecutionContext,
-    ) -> NDT | None:
+    ) -> NDT:
         return self.node.value
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/dag/online_event_aggregation_node.py` & `superlinked-4.0.1/superlinked/framework/online/dag/online_event_aggregation_node.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,48 +10,41 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from dataclasses import dataclass
-
 from typing_extensions import override
 
 from superlinked.framework.common.const import DEFAULT_WEIGHT
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.event_aggregation_node import EventAggregationNode
+from superlinked.framework.common.dag.exception import ParentCountException
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.exception import (
     DagEvaluationException,
     ValidationException,
 )
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
 from superlinked.framework.common.schema.schema_object import SchemaObject
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
-from superlinked.framework.online.dag.exception import ParentCountException
 from superlinked.framework.online.dag.online_comparison_filter_node import (
     OnlineComparisonFilterNode,
 )
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
     EvaluationResultStoreManager,
 )
 
 
 class OnlineEventAggregationNode(OnlineNode[EventAggregationNode, Vector], HasLength):
     EFFECT_COUNT_KEY = "effect_count"
 
-    @dataclass
-    class EventEffect:
-        aggregation: Vector
-        effect_count: int
-
     def __init__(
         self,
         node: EventAggregationNode,
         parents: list[OnlineNode],
         evaluation_result_store_manager: EvaluationResultStoreManager,
     ) -> None:
         super().__init__(node, parents, evaluation_result_store_manager)
@@ -82,63 +75,56 @@
                 filter_.weight
                 for filter_ in self.node.filters
                 if filter_.item == parent.node
             ),
             DEFAULT_WEIGHT,
         )
 
-    @classmethod
-    def from_node(
-        cls,
-        node: EventAggregationNode,
-        parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
-    ) -> OnlineEventAggregationNode:
-        return cls(node, parents, evaluation_result_store_manager)
-
-    @classmethod
-    def get_node_type(cls) -> type[EventAggregationNode]:
-        return EventAggregationNode
-
     @property
     def length(self) -> int:
         return self.node.length
 
     @override
     def evaluate_self(
         self,
+        parsed_schemas: list[ParsedSchema],
+        context: ExecutionContext,
+    ) -> list[EvaluationResult[Vector]]:
+        return [self.evaluate_self_single(schema, context) for schema in parsed_schemas]
+
+    def evaluate_self_single(
+        self,
         parsed_schema: ParsedSchema,
         context: ExecutionContext,
     ) -> EvaluationResult[Vector]:
         self.__check_schema_validity(parsed_schema.schema)
         stored_result = (
             self.load_stored_result(parsed_schema.id_, parsed_schema.schema)
             or Vector.empty_vector()
         )
         if (
             parsed_schema.event_parsed_schema is None
             or self.node.event_schema != parsed_schema.event_parsed_schema.schema
             or self.input_to_aggregate is None
         ):
             return EvaluationResult(self._get_single_evaluation_result(stored_result))
-        previous_result = stored_result
-        event_effect = self._process_event(parsed_schema.event_parsed_schema, context)
-
+        event_effects = self._process_event(parsed_schema.event_parsed_schema, context)
         previous_effect_count = self.__load_effect_count(
             parsed_schema.id_, parsed_schema.schema
         )
-        accumulated_previous_result = (
-            Vector.empty_vector()
+        previous_results = (
+            [Vector.empty_vector()]
             if previous_effect_count == 0
-            else (previous_result * previous_effect_count)
+            else ([stored_result] * previous_effect_count)
         )
-        new_effect_count = previous_effect_count + event_effect.effect_count
+        new_effect_count = previous_effect_count + len(event_effects)
         vector = (
-            (accumulated_previous_result.aggregate(event_effect.aggregation))
-            / new_effect_count
+            self.input_to_aggregate.node.aggregation.aggregate(
+                previous_results + event_effects, context
+            )
             if new_effect_count
             else Vector.empty_vector()
         )
         self.__store_effect_count(
             parsed_schema.id_, parsed_schema.schema, new_effect_count
         )
         result = self._get_single_evaluation_result(vector)
@@ -152,57 +138,51 @@
                 + f"got {schema._base_class_name}"
             )
 
     def _process_event(
         self,
         event_parsed_schema: ParsedSchema,
         context: ExecutionContext,
-    ) -> EventEffect:
+    ) -> list[Vector]:
         if self.input_to_aggregate is None:
             raise DagEvaluationException(
                 f"{self.class_name} must have an input to aggregate."
             )
 
         affecting_parsed_schema = self._map_event_schema_to_affecting_schema(
             event_parsed_schema
         )
-        parent_result = self.input_to_aggregate.evaluate_next(
+        parent_result = self.input_to_aggregate.evaluate_next_single(
             affecting_parsed_schema, context
         ).main.value
         if not isinstance(parent_result, Vector):
             raise DagEvaluationException(
                 "parent_to_aggregate's evaluation result must be of type Vector"
                 + f", got {type(parent_result)}"
             )
-        event_effect = self._aggregate_event_effect(
+        event_effects = self._aggregate_event_effect(
             event_parsed_schema, parent_result, context
         )
-        return event_effect
+        return event_effects
 
     def _aggregate_event_effect(
         self,
         event_parsed_schema: ParsedSchema,
         affecting_vector: Vector,
         context: ExecutionContext,
-    ) -> EventEffect:
-        aggregated_vector: Vector = Vector.empty_vector()
-        effect_count = 0
-        if not affecting_vector.is_empty:
-            for filter_parent, weight in self.weighted_filter_parents.items():
-                filter_result = filter_parent.evaluate_next(
-                    event_parsed_schema,
-                    context,
-                )
-                if filter_result.main.value:
-                    weighted_affecting_vector = affecting_vector * weight
-                    aggregated_vector = aggregated_vector.aggregate(
-                        weighted_affecting_vector
-                    )
-                    effect_count += 1
-        return OnlineEventAggregationNode.EventEffect(aggregated_vector, effect_count)
+    ) -> list[Vector]:
+        if affecting_vector.is_empty:
+            return []
+        return [
+            affecting_vector * weight
+            for filter_parent, weight in self.weighted_filter_parents.items()
+            if filter_parent.evaluate_next_single(
+                event_parsed_schema, context
+            ).main.value
+        ]
 
     def _map_event_schema_to_affecting_schema(
         self, event_parsed_schema: ParsedSchema
     ) -> ParsedSchema:
         return next(
             ParsedSchema(self.node.affecting_schema.schema, field.value, [])
             for field in event_parsed_schema.fields
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/dag/online_index_node.py` & `superlinked-4.0.1/superlinked/framework/online/dag/online_index_node.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 from __future__ import annotations
 
 from typing import cast
 
 from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
+from superlinked.framework.common.dag.exception import ParentCountException
 from superlinked.framework.common.dag.index_node import IndexNode
 from superlinked.framework.common.dag.node import Node
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
 from superlinked.framework.common.schema.schema_object import SchemaObject
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
-from superlinked.framework.online.dag.exception import ParentCountException
 from superlinked.framework.online.dag.online_concatenation_node import (
     OnlineConcatenationNode,
 )
 from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
     EvaluationResultStoreManager,
 )
@@ -45,56 +45,59 @@
     ) -> None:
         super().__init__(node, parents, evaluation_result_store_manager)
 
     @property
     def length(self) -> int:
         return self.node.length
 
-    @classmethod
-    def from_node(
-        cls,
-        node: IndexNode,
-        parents: list[OnlineNode[Node[Vector], Vector]],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
-    ) -> OnlineIndexNode:
-        return cls(node, parents, evaluation_result_store_manager)
-
-    @classmethod
-    def get_node_type(cls) -> type[IndexNode]:
-        return IndexNode
-
     def get_parent_for_schema(self, schema: SchemaObject) -> OnlineNode:
         active_parents = [
             parent
             for parent in self.parents
             if schema in cast(Node, parent.node).schemas
         ]
         if len(active_parents) != 1:
             raise ParentCountException(
                 f"{self.class_name} must have exactly 1 parent per schema, got {len(active_parents)}"
             )
         return active_parents[0]
 
+    def __get_parent_for_parsed_schemas(
+        self, parsed_schemas: list[ParsedSchema]
+    ) -> OnlineNode:
+        active_parents = set(
+            self.get_parent_for_schema(parsed_schema.schema)
+            for parsed_schema in parsed_schemas
+        )
+        if len(active_parents) != 1:
+            raise ParentCountException(
+                f"{self.class_name} must have exactly 1 parent per schema, got {len(active_parents)}"
+            )
+        return cast(OnlineNode[Node[Vector], Vector], next(iter(active_parents)))
+
     @override
     def evaluate_self(
         self,
-        parsed_schema: ParsedSchema,
+        parsed_schemas: list[ParsedSchema],
         context: ExecutionContext,
-    ) -> EvaluationResult[Vector]:
-        active_parent = self.get_parent_for_schema(parsed_schema.schema)
-        parent = cast(OnlineNode[Node[Vector], Vector], active_parent)
-        parent_result: EvaluationResult[Vector] = parent.evaluate_next(
-            parsed_schema, context
+    ) -> list[EvaluationResult[Vector]]:
+        parent: OnlineNode = self.__get_parent_for_parsed_schemas(parsed_schemas)
+        parent_results: list[EvaluationResult[Vector]] = parent.evaluate_next(
+            parsed_schemas, context
         )
-        main = self._get_single_evaluation_result(parent_result.main.value)
-        chunks = [
-            self._get_single_evaluation_result(chunk_result.value)
-            for chunk_result in parent_result.chunks
+        return [
+            EvaluationResult(
+                self._get_single_evaluation_result(parent_result.main.value),
+                [
+                    self._get_single_evaluation_result(chunk_result.value)
+                    for chunk_result in parent_result.chunks
+                ],
+            )
+            for parent_result in parent_results
         ]
-        return EvaluationResult(main, chunks)
 
     def _re_weight_vector(
         self,
         schema: SchemaObject,
         vector: Vector,
         context: ExecutionContext,
     ) -> Vector:
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/dag/online_named_function_node.py` & `superlinked-4.0.1/superlinked/framework/online/dag/online_named_function_node.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,55 +12,58 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from typing import cast
 
+from typing_extensions import override
+
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.named_function_node import NamedFunctionNode
 from superlinked.framework.common.dag.node import NDT
-from superlinked.framework.common.exception import InitializationException
+from superlinked.framework.common.parser.parsed_schema import ParsedSchema
 from superlinked.framework.common.util.named_function_evaluator import (
     NamedFunctionEvaluator,
 )
-from superlinked.framework.online.dag.default_online_node import DefaultOnlineNode
-from superlinked.framework.online.dag.evaluation_result import SingleEvaluationResult
+from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.online_node import OnlineNode
+from superlinked.framework.online.dag.parent_validator import ParentValidationType
 from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
     EvaluationResultStoreManager,
 )
 
 
-class OnlineNamedFunctionNode(DefaultOnlineNode[NamedFunctionNode[NDT], NDT]):
+class OnlineNamedFunctionNode(OnlineNode[NamedFunctionNode[NDT], NDT]):
     def __init__(
         self,
         node: NamedFunctionNode,
+        parents: list[OnlineNode],
         evaluation_result_store_manager: EvaluationResultStoreManager,
     ) -> None:
-        super().__init__(node, [], evaluation_result_store_manager)
+        super().__init__(
+            node,
+            parents,
+            evaluation_result_store_manager,
+            ParentValidationType.NO_PARENTS,
+        )
 
-    @classmethod
-    def from_node(
-        cls,
-        node: NamedFunctionNode,
-        parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
-    ) -> OnlineNamedFunctionNode:
-        if len(parents) != 0:
-            raise InitializationException(f"{cls.__name__} cannot have parents.")
-        return cls(node, evaluation_result_store_manager)
-
-    @classmethod
-    def get_node_type(cls) -> type[NamedFunctionNode]:
-        return NamedFunctionNode
+    @override
+    def evaluate_self(
+        self,
+        parsed_schemas: list[ParsedSchema],
+        context: ExecutionContext,
+    ) -> list[EvaluationResult[NDT]]:
+        result = EvaluationResult(
+            self._get_single_evaluation_result(self._evaluate_single(context))
+        )
+        return [result for _ in parsed_schemas]
 
     def _evaluate_single(
         self,
-        parent_results: dict[OnlineNode, SingleEvaluationResult],
         context: ExecutionContext,
-    ) -> NDT | None:
+    ) -> NDT:
         result = cast(
             NDT,
             NamedFunctionEvaluator().evaluate(self.node.named_function, context),
         )
         return result
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/dag/online_node.py` & `superlinked-4.0.1/superlinked/framework/online/dag/online_text_embedding_node.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,114 +10,80 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from abc import ABC, ABCMeta, abstractmethod
-from typing import Generic, TypeVar
+from typing import cast
 
-from typing_extensions import Self
+from beartype.typing import Sequence
+from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
-from superlinked.framework.common.dag.node import NDT, NT
+from superlinked.framework.common.dag.text_embedding_node import TextEmbeddingNode
+from superlinked.framework.common.data_types import Vector
+from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
-from superlinked.framework.common.schema.schema_object import SchemaObject
+from superlinked.framework.online.dag.default_online_node import DefaultOnlineNode
 from superlinked.framework.online.dag.evaluation_result import (
     EvaluationResult,
     SingleEvaluationResult,
 )
+from superlinked.framework.online.dag.online_node import OnlineNode
 from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
     EvaluationResultStoreManager,
 )
 
-ONT = TypeVar("ONT", bound="OnlineNode")
 
-
-class OnlineNode(ABC, Generic[NT, NDT], metaclass=ABCMeta):
+class OnlineTextEmbeddingNode(DefaultOnlineNode[TextEmbeddingNode, Vector], HasLength):
     def __init__(
         self,
-        node: NT,
+        node: TextEmbeddingNode,
         parents: list[OnlineNode],
         evaluation_result_store_manager: EvaluationResultStoreManager,
     ) -> None:
-        self.node = node
-        self.children: list[OnlineNode] = []
-        self.parents = parents
-        self.evaluation_result_store_manager = evaluation_result_store_manager
-        for parent in self.parents:
-            parent.children.append(self)
-
-    @property
-    def class_name(self) -> str:
-        return self.__class__.__name__
+        super().__init__(node, parents, evaluation_result_store_manager)
 
     @property
-    def node_id(self) -> str:
-        return self.node.node_id
-
-    def _get_single_evaluation_result(self, value: NDT) -> SingleEvaluationResult[NDT]:
-        return SingleEvaluationResult(self.node_id, value)
-
-    @classmethod
-    @abstractmethod
-    def from_node(
-        cls,
-        node: NT,
-        parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
-    ) -> Self:
-        pass
-
-    @classmethod
-    @abstractmethod
-    def get_node_type(cls) -> type[NT]:
-        pass
+    def length(self) -> int:
+        return self.node.length
 
-    def evaluate_next(
-        self,
-        parsed_schema: ParsedSchema,
-        context: ExecutionContext,
-    ) -> EvaluationResult[NDT]:
-        result = self.evaluate_self(parsed_schema, context)
-        if self.node.persist_evaluation_result:
-            self.persist(result, parsed_schema, context)
-        return result
-
-    @abstractmethod
+    @override
     def evaluate_self(
         self,
-        parsed_schema: ParsedSchema,
+        parsed_schemas: list[ParsedSchema],
         context: ExecutionContext,
-    ) -> EvaluationResult[NDT]:
-        pass
+    ) -> list[EvaluationResult[Vector]]:
+        if self._is_query_without_similar_clause(parsed_schemas, context):
+            vector = Vector([0] * self.node.length)
+            return [
+                EvaluationResult(self._get_single_evaluation_result(vector))
+                for _ in parsed_schemas
+            ]
+        return super().evaluate_self(parsed_schemas, context)
 
-    def persist(
+    @override
+    def _evaluate_singles(
         self,
-        result: EvaluationResult[NDT],
-        parsed_schema: ParsedSchema,
+        parent_results: list[dict[OnlineNode, SingleEvaluationResult]],
         context: ExecutionContext,
-    ) -> None:
-        if context.is_query_context():
-            return
-        self.evaluation_result_store_manager.save_result(
-            result,
-            parsed_schema.id_,
-            parsed_schema.schema._schema_name,
-            self.node.persistence_type,
-        )
-
-    def load_stored_result(
-        self, main_object_id: str, schema: SchemaObject
-    ) -> NDT | None:
-        stored_value: SingleEvaluationResult | None = (
-            self.evaluation_result_store_manager.load_single_result(
-                main_object_id,
-                self.node_id,
-                schema._schema_name,
-                self.node.persistence_type,
+    ) -> Sequence[Vector | None]:
+        none_indices = [
+            i for i, parent_result in enumerate(parent_results) if not parent_result
+        ]
+        non_none_parent_results = [
+            parent_result for parent_result in parent_results if parent_result
+        ]
+        input_ = list(
+            map(
+                lambda parent_result: list(parent_result.values())[0].value,
+                non_none_parent_results,
             )
         )
-        if stored_value:
-            return stored_value.value
-        return None
+        embedded_texts = cast(list[Vector | None], self.__embed_texts(input_))
+        for i in none_indices:
+            embedded_texts.insert(i, None)
+        return embedded_texts
+
+    def __embed_texts(self, texts: list[str]) -> list[Vector]:
+        return self.node.embedding.embed_multiple(texts)
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/dag/online_number_embedding_node.py` & `superlinked-4.0.1/superlinked/framework/online/dag/online_number_similarity_node.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,81 +16,66 @@
 
 from typing import cast
 
 from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.node import Node
-from superlinked.framework.common.dag.number_embedding_node import NumberEmbeddingNode
+from superlinked.framework.common.dag.number_similarity_node import NumberSimilarityNode
 from superlinked.framework.common.data_types import Vector
-from superlinked.framework.common.exception import DagEvaluationException
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
-from superlinked.framework.online.dag.exception import ParentCountException
 from superlinked.framework.online.dag.online_node import OnlineNode
+from superlinked.framework.online.dag.parent_validator import ParentValidationType
 from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
     EvaluationResultStoreManager,
 )
 
 
-class OnlineNumberEmbeddingNode(OnlineNode[NumberEmbeddingNode, Vector], HasLength):
+class OnlineNumberSimilarityNode(OnlineNode[NumberSimilarityNode, Vector], HasLength):
     def __init__(
         self,
-        node: NumberEmbeddingNode,
+        node: NumberSimilarityNode,
         parents: list[OnlineNode],
         evaluation_result_store_manager: EvaluationResultStoreManager,
     ) -> None:
-        super().__init__(node, parents, evaluation_result_store_manager)
-
-    @classmethod
-    def from_node(
-        cls,
-        node: NumberEmbeddingNode,
-        parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
-    ) -> OnlineNumberEmbeddingNode:
-        if len(parents) > 1:
-            raise ParentCountException(
-                f"{cls.__name__} cannot have more than one parents, got {len(parents)}."
-            )
-        return cls(node, parents, evaluation_result_store_manager)
-
-    @classmethod
-    def get_node_type(cls) -> type[NumberEmbeddingNode]:
-        return NumberEmbeddingNode
+        super().__init__(
+            node,
+            parents,
+            evaluation_result_store_manager,
+            ParentValidationType.LESS_THAN_TWO_PARENTS,
+        )
 
     @property
     def length(self) -> int:
         return self.node.length
 
     @override
     def evaluate_self(
         self,
+        parsed_schemas: list[ParsedSchema],
+        context: ExecutionContext,
+    ) -> list[EvaluationResult[Vector]]:
+        if self._is_query_without_similar_clause(parsed_schemas, context):
+            vector = Vector([0] * self.node.length)
+            return [
+                EvaluationResult(self._get_single_evaluation_result(vector))
+                for _ in parsed_schemas
+            ]
+        return [self.evaluate_self_single(schema, context) for schema in parsed_schemas]
+
+    def evaluate_self_single(
+        self,
         parsed_schema: ParsedSchema,
         context: ExecutionContext,
     ) -> EvaluationResult[Vector]:
-        if context.is_query_context():
-            vector = Vector([1.0] * self.node.length)
-            return EvaluationResult(self._get_single_evaluation_result(vector))
-
-        if len(self.parents) > 1:
-            raise ParentCountException(
-                f"{self.__class__.__name__} cannot have more than one parents, got {len(self.parents)}."
-            )
-
         if len(self.parents) == 0:
-            stored_result = self.load_stored_result(
-                parsed_schema.id_, parsed_schema.schema
-            )
-            if stored_result is None:
-                raise DagEvaluationException(
-                    f"{self.class_name} doesn't have a stored result."
-                )
+            stored_result = self.load_stored_result_or_raise_exception(parsed_schema)
             return EvaluationResult(self._get_single_evaluation_result(stored_result))
 
         input_: EvaluationResult[float | int] = cast(
             OnlineNode[Node[float | int], float | int], self.parents[0]
-        ).evaluate_next(parsed_schema, context)
-        transformed_input_value = self.node.embedding.transform(input_.main.value)
+        ).evaluate_next_single(parsed_schema, context)
+        transformed_input_value = self.node.embedding.embed(input_.main.value, context)
         main = self._get_single_evaluation_result(transformed_input_value)
         return EvaluationResult(main)
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/dag/online_number_similarity_node.py` & `superlinked-4.0.1/superlinked/framework/online/dag/online_custom_node.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,83 +12,76 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from typing import cast
 
+import numpy as np
+import numpy.typing as npt
 from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
+from superlinked.framework.common.dag.custom_node import CustomVectorEmbeddingNode
 from superlinked.framework.common.dag.node import Node
-from superlinked.framework.common.dag.number_similarity_node import NumberSimilarityNode
 from superlinked.framework.common.data_types import Vector
-from superlinked.framework.common.exception import DagEvaluationException
+from superlinked.framework.common.exception import ValidationException
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
-from superlinked.framework.online.dag.exception import ParentCountException
 from superlinked.framework.online.dag.online_node import OnlineNode
+from superlinked.framework.online.dag.parent_validator import ParentValidationType
 from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
     EvaluationResultStoreManager,
 )
 
 
-class OnlineNumberSimilarityNode(OnlineNode[NumberSimilarityNode, Vector], HasLength):
+class OnlineCustomVectorEmbeddingNode(
+    OnlineNode[CustomVectorEmbeddingNode, Vector], HasLength
+):
     def __init__(
         self,
-        node: NumberSimilarityNode,
+        node: CustomVectorEmbeddingNode,
         parents: list[OnlineNode],
         evaluation_result_store_manager: EvaluationResultStoreManager,
     ) -> None:
-        super().__init__(node, parents, evaluation_result_store_manager)
-
-    @classmethod
-    def from_node(
-        cls,
-        node: NumberSimilarityNode,
-        parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
-    ) -> OnlineNumberSimilarityNode:
-        if len(parents) > 1:
-            raise ParentCountException(
-                f"{cls.__name__} cannot have more than one parents, got {len(parents)}."
-            )
-        return cls(node, parents, evaluation_result_store_manager)
-
-    @classmethod
-    def get_node_type(cls) -> type[NumberSimilarityNode]:
-        return NumberSimilarityNode
+        super().__init__(
+            node,
+            parents,
+            evaluation_result_store_manager,
+            ParentValidationType.LESS_THAN_TWO_PARENTS,
+        )
 
     @property
     def length(self) -> int:
         return self.node.length
 
     @override
     def evaluate_self(
         self,
+        parsed_schemas: list[ParsedSchema],
+        context: ExecutionContext,
+    ) -> list[EvaluationResult[Vector]]:
+        return [self.evaluate_self_single(schema, context) for schema in parsed_schemas]
+
+    def evaluate_self_single(
+        self,
         parsed_schema: ParsedSchema,
         context: ExecutionContext,
     ) -> EvaluationResult[Vector]:
-        if len(self.parents) > 1:
-            raise ParentCountException(
-                f"{self.__class__.__name__} cannot have more than one parents, got {len(self.parents)}."
-            )
-
         if len(self.parents) == 0:
-            stored_result = self.load_stored_result(
-                parsed_schema.id_, parsed_schema.schema
-            )
-            if stored_result is None:
-                raise DagEvaluationException(
-                    f"{self.class_name} doesn't have a stored result."
-                )
+            stored_result = self.load_stored_result_or_raise_exception(parsed_schema)
             return EvaluationResult(self._get_single_evaluation_result(stored_result))
 
-        input_: EvaluationResult[float | int] = cast(
-            OnlineNode[Node[float | int], float | int], self.parents[0]
-        ).evaluate_next(parsed_schema, context)
-        transformed_input_value = self.node.embedding.transform(
-            input_.main.value, context.is_query_context()
-        )
+        input_: EvaluationResult[npt.NDArray[np.float64]] = cast(
+            OnlineNode[Node[Vector], npt.NDArray[np.float64]], self.parents[0]
+        ).evaluate_next_single(parsed_schema, context)
+        input_value = input_.main.value
+        if len(input_value) != self.length:
+            raise ValidationException(
+                f"{self.class_name} can only process `Vector` inputs"
+                + f" of size {self.length}"
+                + f", got {len(input_value)}"
+            )
+        transformed_input_value = self.node.embedding.embed(input_value, context)
         main = self._get_single_evaluation_result(transformed_input_value)
         return EvaluationResult(main)
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/dag/online_recency_node.py` & `superlinked-4.0.1/superlinked/framework/online/dag/online_recency_node.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,66 +10,66 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from beartype.typing import Sequence
+from typing_extensions import override
+
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.recency_node import RecencyNode
 from superlinked.framework.common.data_types import Vector
-from superlinked.framework.common.exception import InitializationException
 from superlinked.framework.common.interface.has_length import HasLength
 from superlinked.framework.online.dag.default_online_node import DefaultOnlineNode
 from superlinked.framework.online.dag.evaluation_result import SingleEvaluationResult
 from superlinked.framework.online.dag.online_node import OnlineNode
+from superlinked.framework.online.dag.parent_validator import ParentValidationType
 from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
     EvaluationResultStoreManager,
 )
 
 DAY_IN_SECONDS: int = 24 * 60 * 60
 
 
 class OnlineRecencyNode(DefaultOnlineNode[RecencyNode, Vector], HasLength):
     def __init__(
         self,
         node: RecencyNode,
-        parent: OnlineNode,
-        evaluation_result_store_manager: EvaluationResultStoreManager,
-    ) -> None:
-        super().__init__(node, [parent], evaluation_result_store_manager)
-
-    @classmethod
-    def from_node(
-        cls,
-        node: RecencyNode,
         parents: list[OnlineNode],
         evaluation_result_store_manager: EvaluationResultStoreManager,
-    ) -> OnlineRecencyNode:
-        if len(parents) != 1:
-            raise InitializationException(f"{cls.__name__} must have exactly 1 parent.")
-        return cls(node, parents[0], evaluation_result_store_manager)
-
-    @classmethod
-    def get_node_type(cls) -> type[RecencyNode]:
-        return RecencyNode
+    ) -> None:
+        super().__init__(
+            node,
+            parents,
+            evaluation_result_store_manager,
+            ParentValidationType.EXACTLY_ONE_PARENT,
+        )
 
     @property
     def length(self) -> int:
         return self.node.embedding.length
 
+    @override
+    def _evaluate_singles(
+        self,
+        parent_results: list[dict[OnlineNode, SingleEvaluationResult]],
+        context: ExecutionContext,
+    ) -> Sequence[Vector | None]:
+        return [
+            self._evaluate_single(parent_result, context)
+            for parent_result in parent_results
+        ]
+
     def _evaluate_single(
         self,
         parent_results: dict[OnlineNode, SingleEvaluationResult],
         context: ExecutionContext,
     ) -> Vector | None:
         if len(parent_results.items()) != 1:
             return None
         input_ = list(parent_results.values())[0]
         return self._calc_recency(input_.value, context)
 
     def _calc_recency(self, created_at: int, context: ExecutionContext) -> Vector:
-        time_period_start: int = context.now()
-
-        return self.node.embedding.calc_recency_vector(
-            created_at, time_period_start, context.is_query_context()
-        )
+        return self.node.embedding.calc_recency_vector(created_at, context)
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/dag/online_schema_dag.py` & `superlinked-4.0.1/superlinked/framework/online/dag/online_schema_dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,18 +54,18 @@
 
     @property
     def leaf_node(self) -> OnlineIndexNode:
         return self.__leaf_node
 
     def evaluate(
         self,
-        parsed_schema: ParsedSchema,
+        parsed_schemas: list[ParsedSchema],
         context: ExecutionContext,
-    ) -> EvaluationResult[Vector]:
-        return self.leaf_node.evaluate_next(parsed_schema, context)
+    ) -> list[EvaluationResult[Vector]]:
+        return self.leaf_node.evaluate_next(parsed_schemas, context)
 
     def __validate(self, schema: SchemaObject, nodes: list[OnlineNode]) -> None:
         class_name = self.__class__.__name__
         leaf_nodes = [node for node in nodes if len(node.children) == 0]
         if len(leaf_nodes) != 1:
             raise LeafNodeCountException(
                 f"{class_name} must have exactly one leaf Node."
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/dag/online_schema_field_node.py` & `superlinked-4.0.1/superlinked/framework/online/dag/online_schema_field_node.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,54 +16,52 @@
 
 from typing import Generic, cast
 
 from typing_extensions import override
 
 from superlinked.framework.common.dag.context import ExecutionContext
 from superlinked.framework.common.dag.schema_field_node import SchemaFieldNode
-from superlinked.framework.common.exception import InitializationException
 from superlinked.framework.common.parser.parsed_schema import (
     ParsedSchema,
     ParsedSchemaField,
 )
 from superlinked.framework.common.schema.schema_object import SFT, Timestamp
 from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.exception import ValueNotProvidedException
 from superlinked.framework.online.dag.online_node import OnlineNode
+from superlinked.framework.online.dag.parent_validator import ParentValidationType
 from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
     EvaluationResultStoreManager,
 )
 
 
 class OnlineSchemaFieldNode(Generic[SFT], OnlineNode[SchemaFieldNode, SFT]):
     def __init__(
         self,
         node: SchemaFieldNode,
-        evaluation_result_store_manager: EvaluationResultStoreManager,
-    ) -> None:
-        super().__init__(node, [], evaluation_result_store_manager)
-
-    @classmethod
-    def from_node(
-        cls,
-        node: SchemaFieldNode,
         parents: list[OnlineNode],
         evaluation_result_store_manager: EvaluationResultStoreManager,
-    ) -> OnlineSchemaFieldNode:
-        if len(parents) != 0:
-            raise InitializationException(f"{cls.__name__} cannot have parents.")
-        return cls(node, evaluation_result_store_manager)
-
-    @classmethod
-    def get_node_type(cls) -> type[SchemaFieldNode]:
-        return SchemaFieldNode
+    ) -> None:
+        super().__init__(
+            node,
+            parents,
+            evaluation_result_store_manager,
+            ParentValidationType.NO_PARENTS,
+        )
 
     @override
     def evaluate_self(
         self,
+        parsed_schemas: list[ParsedSchema],
+        context: ExecutionContext,
+    ) -> list[EvaluationResult[SFT]]:
+        return [self.evaluate_self_single(schema, context) for schema in parsed_schemas]
+
+    def evaluate_self_single(
+        self,
         parsed_schema: ParsedSchema,
         context: ExecutionContext,
     ) -> EvaluationResult[SFT]:
         parsed_nodes: list[ParsedSchemaField] = [
             field
             for field in parsed_schema.fields
             if field.schema_field == self.node.schema_field
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/dag/online_text_embedding_node.py` & `superlinked-4.0.1/superlinked/framework/online/dag/online_number_embedding_node.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,57 +10,70 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
+from typing import cast
+
+from typing_extensions import override
+
 from superlinked.framework.common.dag.context import ExecutionContext
-from superlinked.framework.common.dag.text_embedding_node import TextEmbeddingNode
+from superlinked.framework.common.dag.node import Node
+from superlinked.framework.common.dag.number_embedding_node import NumberEmbeddingNode
 from superlinked.framework.common.data_types import Vector
 from superlinked.framework.common.interface.has_length import HasLength
-from superlinked.framework.online.dag.default_online_node import DefaultOnlineNode
-from superlinked.framework.online.dag.evaluation_result import SingleEvaluationResult
+from superlinked.framework.common.parser.parsed_schema import ParsedSchema
+from superlinked.framework.online.dag.evaluation_result import EvaluationResult
 from superlinked.framework.online.dag.online_node import OnlineNode
+from superlinked.framework.online.dag.parent_validator import ParentValidationType
 from superlinked.framework.online.store_manager.evaluation_result_store_manager import (
     EvaluationResultStoreManager,
 )
 
 
-class OnlineTextEmbeddingNode(DefaultOnlineNode[TextEmbeddingNode, Vector], HasLength):
+class OnlineNumberEmbeddingNode(OnlineNode[NumberEmbeddingNode, Vector], HasLength):
     def __init__(
         self,
-        node: TextEmbeddingNode,
+        node: NumberEmbeddingNode,
         parents: list[OnlineNode],
         evaluation_result_store_manager: EvaluationResultStoreManager,
     ) -> None:
-        super().__init__(node, parents, evaluation_result_store_manager)
+        super().__init__(
+            node,
+            parents,
+            evaluation_result_store_manager,
+            ParentValidationType.LESS_THAN_TWO_PARENTS,
+        )
 
     @property
     def length(self) -> int:
         return self.node.length
 
-    @classmethod
-    def from_node(
-        cls,
-        node: TextEmbeddingNode,
-        parents: list[OnlineNode],
-        evaluation_result_store_manager: EvaluationResultStoreManager,
-    ) -> OnlineTextEmbeddingNode:
-        return cls(node, parents, evaluation_result_store_manager)
-
-    @classmethod
-    def get_node_type(cls) -> type[TextEmbeddingNode]:
-        return TextEmbeddingNode
-
-    def _evaluate_single(
+    @override
+    def evaluate_self(
         self,
-        parent_results: dict[OnlineNode, SingleEvaluationResult],
+        parsed_schemas: list[ParsedSchema],
         context: ExecutionContext,
-    ) -> Vector | None:
-        if len(parent_results.items()) != 1:
-            return None
-        input_ = list(parent_results.values())[0]
-        return self.__embed_text(input_.value).normalize()
+    ) -> list[EvaluationResult[Vector]]:
+        return [self.evaluate_self_single(schema, context) for schema in parsed_schemas]
 
-    def __embed_text(self, text: str) -> Vector:
-        return self.node.embedding.transform(text)
+    def evaluate_self_single(
+        self,
+        parsed_schema: ParsedSchema,
+        context: ExecutionContext,
+    ) -> EvaluationResult[Vector]:
+        if context.is_query_context():
+            vector = Vector([1.0] * self.node.length)
+            return EvaluationResult(self._get_single_evaluation_result(vector))
+
+        if len(self.parents) == 0:
+            stored_result = self.load_stored_result_or_raise_exception(parsed_schema)
+            return EvaluationResult(self._get_single_evaluation_result(stored_result))
+
+        input_: EvaluationResult[float | int] = cast(
+            OnlineNode[Node[float | int], float | int], self.parents[0]
+        ).evaluate_next_single(parsed_schema, context)
+        transformed_input_value = self.node.embedding.embed(input_.main.value, context)
+        main = self._get_single_evaluation_result(transformed_input_value)
+        return EvaluationResult(main)
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/source/in_memory_object_writer.py` & `superlinked-4.0.1/superlinked/framework/online/source/in_memory_object_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,13 +23,14 @@
 
 
 class InMemoryObjectWriter(Subscriber[ParsedSchema]):
     def __init__(self, object_store_manager: ObjectStoreManager[Json]) -> None:
         super().__init__()
         self.__object_store_manager = object_store_manager
 
-    def update(self, message: ParsedSchema) -> None:
-        parser = JsonParser(message.schema)
-        data = parser.marshal(message)
-        data_id = DataId(message.schema._schema_name, message.id_)
-        for data_element in data:
-            self.__object_store_manager.save(data_id, data_element)
+    def update(self, messages: list[ParsedSchema]) -> None:
+        for message in messages:
+            parser = JsonParser(message.schema)
+            data = parser.marshal(message)
+            data_id = DataId(message.schema._schema_name, message.id_)
+            for data_element in data:
+                self.__object_store_manager.save(data_id, data_element)
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/source/in_memory_source.py` & `superlinked-4.0.1/superlinked/framework/online/source/in_memory_source.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,28 +12,32 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
 from typing import Generic
 
+from superlinked.framework.common.const import INMEMORY_PUT_CHUNK_SIZE
 from superlinked.framework.common.observable import Publisher
 from superlinked.framework.common.parser.data_parser import DataParser
 from superlinked.framework.common.parser.parsed_schema import ParsedSchema
 from superlinked.framework.common.schema.id_schema_object import IdSchemaObjectT
 from superlinked.framework.common.source.source import Source
 from superlinked.framework.common.source.types import SourceTypeT
+from superlinked.framework.common.util.collection_util import chunk_list
 
 
 class InMemorySource(
     Generic[IdSchemaObjectT, SourceTypeT],
     Publisher[ParsedSchema],
     Source[IdSchemaObjectT, SourceTypeT],
 ):
     def __init__(self, parser: DataParser[IdSchemaObjectT, SourceTypeT]) -> None:
         super().__init__()
         self.parser = parser
 
     def put(self, data: SourceTypeT) -> None:
         parsed_schemas: list[ParsedSchema] = self.parser.unmarshal(data)
-        for parsed_schema in parsed_schemas:
-            self._dispatch(parsed_schema)
+        for batch in chunk_list(
+            data=parsed_schemas, chunk_size=INMEMORY_PUT_CHUNK_SIZE
+        ):
+            self._dispatch(batch)
```

### Comparing `superlinked-3.9.1/superlinked/framework/online/store_manager/evaluation_result_store_manager.py` & `superlinked-4.0.1/superlinked/framework/online/store_manager/evaluation_result_store_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,35 +116,33 @@
         )
         self.store_manager.set_property(
             entity_id,
             EvaluationResultStoreManager._get_metadata_property_key(args.key),
             args.metadata,
         )
 
-    def load_single_result(
+    def load_stored_result(
         self,
         main_object_id: str,
         node_id: str,
         schema_name: str,
         persistence_type: PersistenceType,
-    ) -> SingleEvaluationResult | None:
+    ) -> Any | None:
         entity_id = EvaluationResultStoreManager._create_entity_id(
             main_object_id, node_id, schema_name
         )
         stored_result: Any
         match persistence_type:
             case PersistenceType.VECTOR:
                 stored_result = self.store_manager.get_vector(entity_id)
             case PersistenceType.PROPERTY:
                 stored_result = self.store_manager.get_property(
                     entity_id, EvaluationResultStoreManager.RESULT_KEY
                 )
-        if not stored_result:
-            return None
-        return SingleEvaluationResult(node_id, stored_result)
+        return stored_result
 
     def load_result_meta(
         self,
         main_object_id: str,
         schema_name: str,
         node_id: str,
         key: str,
```

### Comparing `superlinked-3.9.1/superlinked/framework/storage/entity.py` & `superlinked-4.0.1/superlinked/framework/storage/entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,7 +83,10 @@
             and __value.id_ == self.id_
             and __value.__to_str_dict() == self.__to_str_dict()
             and (__value.origin_id or "") == (self.origin_id or "")
         )
 
     def __hash__(self) -> int:
         return hash((self.id_, frozenset(self.__to_str_dict()), (self.origin_id or "")))
+
+    def is_chunk(self) -> bool:
+        return self.origin_id is not None
```

### Comparing `superlinked-3.9.1/superlinked/framework/storage/entity_store.py` & `superlinked-4.0.1/superlinked/framework/storage/entity_store.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/storage/entity_store_manager.py` & `superlinked-4.0.1/superlinked/framework/storage/entity_store_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,19 +47,24 @@
         field = self.store.get_field(entity_id, EntityStoreManager.VECTOR_KEY)
         if not isinstance(field, VectorField):
             raise ValueError(
                 f"Field at id ({str(entity_id)}) is not a vector but {type(field)}"
             )
         return field.vector
 
-    def get_entities(self, node_id: str, schema: str) -> list[Entity]:
-        filter_fields = {
-            EntityStoreManager.NODE_ID_KEY: TextField(node_id),
-            EntityStoreManager.SCHEMA_NAME_KEY: TextField(schema),
-        }
+    def get_entities(
+        self, node_id: str = None, schema: str = None, object_id: str = None
+    ) -> list[Entity]:
+        filter_fields = {}
+        if node_id:
+            filter_fields[EntityStoreManager.NODE_ID_KEY] = TextField(node_id)
+        if schema:
+            filter_fields[EntityStoreManager.SCHEMA_NAME_KEY] = TextField(schema)
+        if object_id:
+            filter_fields[EntityStoreManager.OBJECT_ID_KEY] = TextField(object_id)
         return self.store.get_entities(filter_fields)
 
     def set_property(
         self,
         entity_id: EntityId,
         key: str,
         value: str,
```

### Comparing `superlinked-3.9.1/superlinked/framework/storage/field.py` & `superlinked-4.0.1/superlinked/framework/storage/field.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/superlinked/framework/storage/in_memory_entity_store.py` & `superlinked-4.0.1/superlinked/framework/storage/in_memory_entity_store.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,81 +14,82 @@
 
 from __future__ import annotations
 
 from collections import defaultdict
 from collections.abc import Mapping
 from typing import cast
 
+from superlinked.framework.common.calculation.distance_metric import DistanceMetric
 from superlinked.framework.common.calculation.vector_similarity import (
-    SimilarityMethod,
     VectorSimilarityCalculator,
 )
 from superlinked.framework.storage.entity import Entity, EntityId
 from superlinked.framework.storage.entity_store import EntityStore
 from superlinked.framework.storage.field import Field, TextField, VectorField
+from superlinked.framework.storage.persistable_dict import PersistableDict
 
 
-class InMemoryEntityStore(EntityStore):
+class InMemoryEntityStore(EntityStore, PersistableDict):
     """
     Store and retrieve vector and text values.
 
     Disclaimer: Use this module to test on small number of vectors and vector dimensions.
     It behaves reasonably (<1s) for 10k vectors with 1k dimensions each, when performing KNN.
     """
 
     ORIGIN_ID_KEY = "__origin_id__"
     ITEMS_KEY = "__items__"
     SIMILARITY_KEY = "__similarity__"
 
     def __init__(
         self,
         vector_similarity_calculator: VectorSimilarityCalculator = VectorSimilarityCalculator(
-            SimilarityMethod.INNER_PRODUCT
+            DistanceMetric.INNER_PRODUCT
         ),
     ) -> None:
-        self.entities: defaultdict[str, dict[str, Field]] = defaultdict(lambda: {})
+        super().__init__(dict_value=defaultdict(dict))
         self.vector_similarity_calculator = vector_similarity_calculator
 
     def set_field(self, entity_id: EntityId, key: str, value: Field) -> None:
         row_id: str = InMemoryEntityStore._get_row_id_from_entity_id(entity_id)
-        entity = self.entities[row_id]
+        entity = self._dict[row_id]
         entity.update({key: value})
 
     def get_field(self, entity_id: EntityId, key: str) -> Field | None:
         row_id: str = InMemoryEntityStore._get_row_id_from_entity_id(entity_id)
-        entity = self.entities[row_id]
+        entity = self._dict[row_id]
         return entity.get(key)
 
     def set_origin_id(self, entity_id: EntityId, origin_id: EntityId) -> None:
         row_id: str = InMemoryEntityStore._get_row_id_from_entity_id(entity_id)
-        entity = self.entities[row_id]
+        entity = self._dict[row_id]
         entity.update(
             {
                 InMemoryEntityStore.ORIGIN_ID_KEY: TextField(
                     InMemoryEntityStore._get_row_id_from_entity_id(origin_id)
                 )
             }
         )
 
     def get_origin_id(self, entity_id: EntityId) -> EntityId | None:
         row_id: str = InMemoryEntityStore._get_row_id_from_entity_id(entity_id)
-        entity = self.entities[row_id]
+        entity = self._dict[row_id]
         origin_id_field: Field | None = entity.get(InMemoryEntityStore.ORIGIN_ID_KEY)
         if origin_id_field and isinstance(origin_id_field, TextField):
             return InMemoryEntityStore._get_entity_id_from_row_id(origin_id_field.value)
         return None
 
     def set_entity(self, entity: Entity) -> None:
         row_id: str = InMemoryEntityStore._get_row_id_from_entity_id(entity.id_)
-        entity_ = self.entities[row_id]
+        entity_ = self._dict[row_id]
         entity_.update(entity._items)
 
     def get_entity(self, entity_id: EntityId) -> Entity:
         row_id: str = InMemoryEntityStore._get_row_id_from_entity_id(entity_id)
-        entity = self.entities[row_id]
+        entity = self._dict[row_id]
         origin_id_field: Field | None = entity.get(InMemoryEntityStore.ORIGIN_ID_KEY)
         return Entity(
             entity_id,
             entity,
             (
                 InMemoryEntityStore._get_entity_id_from_row_id(origin_id_field.value)
                 if origin_id_field
@@ -98,40 +99,42 @@
         )
 
     def get_entities(
         self, key_value_filter: Mapping[str, Field] | None = None
     ) -> list[Entity]:
         return [
             self.get_entity(InMemoryEntityStore._get_entity_id_from_row_id(k))
-            for k, v in self.entities.items()
+            for k, v in self._dict.items()
             if InMemoryEntityStore._is_subset(v, key_value_filter)
         ]
 
     def knn(
         self,
         key: str,
         vector: VectorField,
         key_value_filter: Mapping[str, Field] | None = None,
         limit: int | None = None,
         radius: float | None = None,
     ) -> list[Entity]:
         filtered_entities: dict[str, dict] = {
             k: {InMemoryEntityStore.ITEMS_KEY: v}
-            for k, v in self.entities.items()
+            for k, v in self._dict.items()
             if InMemoryEntityStore._is_subset(v, key_value_filter)
         }
 
         InMemoryEntityStore._validate_entities(filtered_entities, key, vector)
 
         for k, v in filtered_entities.items():
-            actual_vector = cast(VectorField, v[InMemoryEntityStore.ITEMS_KEY][key])
+            comparison_vector_field = cast(
+                VectorField, v[InMemoryEntityStore.ITEMS_KEY][key]
+            )
             filtered_entities[k].update(
                 {
                     InMemoryEntityStore.SIMILARITY_KEY: self.vector_similarity_calculator.calculate_similarity(
-                        actual_vector.value, vector.value
+                        comparison_vector_field.vector, vector.vector
                     )
                 }
             )
 
         sorted_entities = sorted(
             {
                 k: v
```

### Comparing `superlinked-3.9.1/superlinked/framework/storage/in_memory_object_store.py` & `superlinked-4.0.1/superlinked/framework/storage/object_store_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,23 +10,38 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 
-from superlinked.framework.common.data_types import Json
-from superlinked.framework.storage.object_store import ObjectStore
+from dataclasses import dataclass
+from typing import Generic
 
+from superlinked.framework.storage.object_store import ObjectStore, ObjectTypeT
 
-class InMemoryObjectStore(ObjectStore[Json]):
-    def __init__(self) -> None:
-        self.__store: dict[str, Json] = {}
 
-    def save(self, row_id: str, data: Json) -> None:
-        self.__store[row_id] = data
+@dataclass
+class DataId:
+    schema_id: str
+    object_id: str
 
-    def load(self, row_id: str) -> Json | None:
-        return self.__store.get(row_id)
+    def __str__(self) -> str:
+        return f"{self.schema_id}:{self.object_id}"
 
-    def load_all(self) -> list[Json]:
-        return list(self.__store.values())
+
+class ObjectStoreManager(Generic[ObjectTypeT]):
+    def __init__(self, store: ObjectStore[ObjectTypeT]) -> None:
+        self.__store = store
+
+    def save(self, data_id: DataId, data: ObjectTypeT) -> None:
+        self.__store.save(ObjectStoreManager._get_row_id_from_data_id(data_id), data)
+
+    def load(self, data_id: DataId) -> ObjectTypeT | None:
+        return self.__store.load(ObjectStoreManager._get_row_id_from_data_id(data_id))
+
+    def load_all(self) -> list[ObjectTypeT]:
+        return self.__store.load_all()
+
+    @staticmethod
+    def _get_row_id_from_data_id(data_id: DataId) -> str:
+        return f"{data_id.schema_id}:{data_id.object_id}"
```

### Comparing `superlinked-3.9.1/superlinked/framework/storage/object_store.py` & `superlinked-4.0.1/superlinked/framework/storage/object_store.py`

 * *Files identical despite different names*

### Comparing `superlinked-3.9.1/PKG-INFO` & `superlinked-4.0.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,111 +1,69 @@
 Metadata-Version: 2.1
 Name: superlinked
-Version: 3.9.1
+Version: 4.0.1
 Summary: The Superlinked vector computing library
 License: Apache-2.0
 Author: Superlinked Release
 Author-email: release@superlinked.com
-Requires-Python: >=3.10,<3.11
+Requires-Python: >=3.10,<=3.12.3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Provides-Extra: batch
-Provides-Extra: deployment-executor
-Provides-Extra: deployment-poller
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: interactive
 Provides-Extra: profiler
-Requires-Dist: accelerate (==0.27.2) ; extra == "interactive"
-Requires-Dist: adlfs (==2023.12.0) ; extra == "deployment-executor"
+Requires-Dist: accelerate (>=0.27.2,<0.28.0) ; extra == "interactive"
 Requires-Dist: altair (==5.2.0) ; extra == "interactive"
 Requires-Dist: beartype (>=0.17.2,<0.18.0)
-Requires-Dist: boto3 (==1.34.13) ; extra == "deployment-poller"
-Requires-Dist: boto3-stubs[s3] (==1.34.13) ; extra == "deployment-poller"
-Requires-Dist: cerberus (==1.3.5) ; extra == "deployment-executor" or extra == "deployment-poller"
-Requires-Dist: dask[complete,distributed] (==2024.1.0) ; extra == "deployment-executor"
-Requires-Dist: deltalake (==0.15.1) ; extra == "deployment-executor"
-Requires-Dist: fastapi (==0.109.0) ; extra == "deployment-executor"
-Requires-Dist: fastapi-restful (>=0.5.0,<0.6.0) ; extra == "deployment-executor"
-Requires-Dist: fsspec (==2023.12.2) ; extra == "deployment-executor"
 Requires-Dist: furl (>=2.1.3,<3.0.0)
-Requires-Dist: gcsfs (==2023.12.2.post1) ; extra == "deployment-executor"
-Requires-Dist: google-auth (==2.26.1) ; extra == "deployment-poller"
-Requires-Dist: google-cloud-storage (==2.14.0) ; extra == "deployment-poller"
 Requires-Dist: graphviz (>=0.20.1,<0.21.0) ; extra == "profiler"
-Requires-Dist: httpx (==0.26.0) ; extra == "deployment-executor"
-Requires-Dist: inject (>=5.2.0,<6.0.0) ; extra == "deployment-executor"
-Requires-Dist: ipywidgets (==8.1.2) ; extra == "interactive"
+Requires-Dist: ipywidgets (>=8.1.2,<9.0.0) ; extra == "interactive"
 Requires-Dist: jupyter (>=1.0.0,<2.0.0) ; extra == "interactive" or extra == "profiler"
-Requires-Dist: numpy (==1.22.4)
-Requires-Dist: pandas (>=2.2.1,<3.0.0)
+Requires-Dist: numpy (>=1.25.2)
+Requires-Dist: pandas (==2.0.3)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
-Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0) ; extra == "deployment-executor"
-Requires-Dist: pyspark (==3.5.0) ; extra == "batch"
-Requires-Dist: pyyaml (==6.0.1) ; extra == "deployment-poller"
-Requires-Dist: requests (==2.27.1) ; extra == "deployment-poller"
-Requires-Dist: s3fs (==2023.12.2) ; extra == "deployment-executor"
 Requires-Dist: sentence-transformers (==2.2.2)
 Requires-Dist: snakeviz (>=2.2.0,<2.3.0) ; extra == "profiler"
-Requires-Dist: supervisor (==4.2.5) ; extra == "deployment-executor"
-Requires-Dist: transformers (==4.38.2) ; extra == "interactive"
-Requires-Dist: typing-inspect (>=0.9.0,<0.10.0) ; extra == "deployment-executor"
-Requires-Dist: typing_extensions (>=3.10.0.2) ; extra == "deployment-executor"
-Requires-Dist: umap-learn (==0.5.5) ; extra == "interactive"
-Requires-Dist: uvicorn (==0.15.0) ; extra == "deployment-executor"
+Requires-Dist: transformers (>=4.38.2,<5.0.0) ; extra == "interactive"
+Requires-Dist: typing_extensions (>=3.10.0.2)
+Requires-Dist: umap-learn (>=0.5.5,<0.6.0) ; extra == "interactive"
 Requires-Dist: yelp-gprof2dot (>=1.2.0,<1.3.0) ; extra == "profiler"
 Description-Content-Type: text/markdown
 
 # Superlinked 
 
-Superlinked is a declarative Python SDK that enables you to turn complex data into vectors, in a way that fits the modern data stack and works with your favorite Vector Databases.
+Superlinked is a compute framework for your information retrieval and feature engineering systems, focused on turning complex data into vector embeddings within your RAG, Search, RecSys and Analytics stack.
 
-3 key areas of focus:
-
-1. Custom embedding model creation that fits your complex data entities.
-1. ETL for your vector index for both streaming and batch use-cases.
-1. Vector-native query language that helps you convert hybrid search queries to pure vector queries.
+Our current release allows you to explore our computational model in simple scripts and python notebooks, our next major release will focus on helping you run Superlinked in production, with built-in data infra and vector database integrations.
 
 Visit [Superlinked](https://superlinked.com/) for more information about the company behind this product and our other initiatives.
 
-## Use-cases
-
-- **RAG**: [HR Knowledgebase](https://github.com/superlinked/superlinked/blob/main/notebook/rag_hr_knowledgebase.ipynb)
-- **Semantic Search**: [Movie Recommendations](https://github.com/superlinked/superlinked/blob/main/notebook/semantic_search_netflix_titles.ipynb), [Business News](https://github.com/superlinked/superlinked/blob/main/notebook/semantic_search_news.ipynb)
-- **Recommendation Systems**: [E-commerce](https://github.com/superlinked/superlinked/blob/main/notebook/recommendations_e_commerce.ipynb)
-- **Analytics**: [User Acquisition](https://github.com/superlinked/superlinked/blob/main/notebook/analytics_user_acquisition.ipynb)
-
-You can check a full list of examples [here](https://github.com/superlinked/superlinked/tree/main/notebook).
+If you like what we do, give us a star! ⭐
 
-## Reference
+The screenshot below shows how to build multimodal vectors from your data & define weights at query time to avoid postprocessing & rerank requirements.
 
-1. Describe your data using Python classes with the [@schema](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/common/schema/schema.md) decorator.
-2. Describe your vector embeddings from building blocks with [Spaces](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/space/index.md).
-3. Combine your embeddings into a queryable [Index](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/index/index.m.md).
-4. Define your search with dynamic parameters and weights as a [Query](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/query/query.md).
-5. Load your data using a [Source](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/source/index.md).
-6. Define your transformations with a [Parser](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/common/parser) (e.g.: from [`pd.DataFrame`](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/common/parser/dataframe_parser.md)). 
-7. Run your configuration with an [Executor](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/executor/in_memory/in_memory_executor.md).
+![If the image does not render, you can check the notebook here: https://github.com/superlinked/superlinked/blob/main/notebook/recommendations_e_commerce.ipynb](https://storage.googleapis.com/superlinked-public-assets/notebook.png)
 
-You can check a list of our [features](https://github.com/superlinked/superlinked/tree/main/notebook/feature) or head to our [documentation](https://github.com/superlinked/superlinked/tree/main/docs).
-  
 ## Try it out
 
 Example on how to use Superlinked to experiment with the semantic search use-case. 
 
-### Pre-requisities
+### Pre-requisites
 
 #### In a notebook
 
 Install the superlinked library: 
 ```
 %pip install superlinked
 ```
 
 #### As a script 
-Ensure your python version is 3.10.x.
+Ensure your python version is at least 3.10.x but not newer than 3.12.
 
 ```commandline
 $> python -V
 Python 3.10.9
 ```
 
 If your python version is not `3.10.x` you might use [pyenv](https://github.com/pyenv/pyenv) to install it. 
@@ -129,15 +87,15 @@
 from superlinked.framework.dsl.index.index import Index
 from superlinked.framework.dsl.query.param import Param
 from superlinked.framework.dsl.query.query import Query
 from superlinked.framework.dsl.source.in_memory_source import InMemorySource
 from superlinked.framework.dsl.executor.in_memory.in_memory_executor import InMemoryExecutor
 
 
-@schema # Desribe your schemas.
+@schema # Describe your schemas.
 class Document:
     id: IdField  # Each schema should have exactly one `IdField`.
     body: String # Use `String` for text fields.
 
 document = Document()
 
 relevance_space = TextSimilaritySpace(text=document.body, model="sentence-transformers/all-mpnet-base-v2") # Select your semantic embedding model.
@@ -155,17 +113,40 @@
 source.put([{"id": "sunny_day", "body": "Today is a sunny day"}])
 
 print(app.query(query, query_text="Who is a positive friend?")) # Run your query.
 ```
 
 Ready to go to production? We are launching our first Vector DB connectors soon! [Tell us which Vector DB we should support!](https://github.com/superlinked/superlinked/discussions/41)
 
+## Use-cases
+
+- **RAG**: [HR Knowledgebase](https://github.com/superlinked/superlinked/blob/main/notebook/rag_hr_knowledgebase.ipynb)
+- **Semantic Search**: [Movies](https://github.com/superlinked/superlinked/blob/main/notebook/semantic_search_netflix_titles.ipynb), [Business News](https://github.com/superlinked/superlinked/blob/main/notebook/semantic_search_news.ipynb)
+- **Recommendation Systems**: [E-commerce](https://github.com/superlinked/superlinked/blob/main/notebook/recommendations_e_commerce.ipynb)
+- **Analytics**: [User Acquisition](https://github.com/superlinked/superlinked/blob/main/notebook/analytics_user_acquisition.ipynb)
+
+You can check a full list of examples [here](https://github.com/superlinked/superlinked/tree/main/notebook).
+
+## Reference
+
+1. Describe your data using Python classes with the [@schema](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/common/schema/schema.md) decorator.
+2. Describe your vector embeddings from building blocks with [Spaces](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/space/index.md).
+3. Combine your embeddings into a queryable [Index](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/index/index.m.md).
+4. Define your search with dynamic parameters and weights as a [Query](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/query/query.md).
+5. Load your data using a [Source](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/source/index.md).
+6. Define your transformations with a [Parser](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/common/parser) (e.g.: from [`pd.DataFrame`](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/common/parser/dataframe_parser.md)). 
+7. Run your configuration with an [Executor](https://github.com/superlinked/superlinked/blob/main/docs/superlinked/framework/dsl/executor/in_memory/in_memory_executor.md).
+
+You can check a list of our [features](https://github.com/superlinked/superlinked/tree/main/notebook/feature) or head to our [documentation](https://github.com/superlinked/superlinked/tree/main/docs).
+  
 ## Articles
 
-- [Vector DB Comparison](https://superlinked.com/vector-db-comparison/): Open-source collaboritve comparison of vector databases by Superlinked.
+- [Vector DB Comparison](https://superlinked.com/vector-db-comparison/): Open-source collaborative comparison of vector databases by Superlinked.
 - [Vector Hub](https://superlinked.com/vectorhub/): VectorHub is a free and open-sourced learning hub for people interested in adding vector retrieval to their ML stack
 
 ## Support
 
-If you encounter any challanges during your experiments, feel free to create an [issue](https://github.com/superlinked/superlinked/issues/new?assignees=ClaireSuperlinked&labels=bug&projects=&template=bug_report.md&title=), request a [feature](https://github.com/superlinked/superlinked/issues/new?assignees=ClaireSuperlinked&labels=enhancement&projects=&template=feature_request.md&title=) or to [start a discussion](https://github.com/superlinked/superlinked/discussions/new/choose).
+If you encounter any challenges during your experiments, feel free to create an [issue](https://github.com/superlinked/superlinked/issues/new?assignees=ClaireSuperlinked&labels=bug&projects=&template=bug_report.md&title=), request a [feature](https://github.com/superlinked/superlinked/issues/new?assignees=ClaireSuperlinked&labels=enhancement&projects=&template=feature_request.md&title=) or to [start a discussion](https://github.com/superlinked/superlinked/discussions/new/choose).
 Make sure to group your feedback in separate issues and discussions by topic. Thank you for your feedback!
 
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

