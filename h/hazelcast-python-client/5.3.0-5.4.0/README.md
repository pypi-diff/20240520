# Comparing `tmp/hazelcast-python-client-5.3.0.tar.gz` & `tmp/hazelcast_python_client-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hazelcast-python-client-5.3.0.tar", last modified: Mon Jun 12 14:29:20 2023, max compression
+gzip compressed data, was "hazelcast_python_client-5.4.0.tar", last modified: Fri May 17 10:02:34 2024, max compression
```

## Comparing `hazelcast-python-client-5.3.0.tar` & `hazelcast_python_client-5.4.0.tar`

### file list

```diff
@@ -1,382 +1,383 @@
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:20.059892 hazelcast-python-client-5.3.0/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    11358 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/LICENSE.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       47 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/MANIFEST.in
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     8829 2023-06-12 14:29:20.059892 hazelcast-python-client-5.3.0/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     7578 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/README.rst
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:19.989891 hazelcast-python-client-5.3.0/hazelcast/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      246 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    16433 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/aggregator.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    22523 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/client.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    13634 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/cluster.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     6168 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/compact.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    72382 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/config.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    38921 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/connection.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    14181 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/core.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    17582 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/cp.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    16593 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/db.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     4502 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/discovery.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    15384 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/errors.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     9302 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/future.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1650 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/hash.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    16602 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/invocation.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3385 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/lifecycle.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    11857 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/listener.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    12904 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/metrics.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    10787 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/near_cache.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     5420 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/partition.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    23360 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/predicate.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3225 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/projection.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:19.999891 hazelcast-python-client-5.3.0/hazelcast/protocol/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     4297 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    25744 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/builtin.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     9174 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/client_message.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:20.049892 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1098 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_add_and_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1257 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_alter_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      888 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_apply_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1270 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_compare_and_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1098 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_get_and_add_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1118 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_get_and_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      910 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1341 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_apply_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1168 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_compare_and_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1084 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_contains_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      835 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1223 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1819 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_add_cluster_view_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1677 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_add_distributed_object_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3002 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_authentication_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2963 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_authentication_custom_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      547 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_create_proxy_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      547 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_destroy_proxy_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      893 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_fetch_schema_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_get_distributed_objects_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1267 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_local_backup_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      401 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_ping_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      921 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_remove_distributed_object_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      601 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_send_all_schemas_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      649 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_send_schema_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      895 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_statistics_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1314 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_await_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1105 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_count_down_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      909 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_get_count_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      909 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_get_round_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1098 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_try_set_count_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      678 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_group_create_cp_group_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      700 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_group_destroy_cp_object_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1036 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_session_close_session_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1429 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_session_create_session_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      821 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_session_generate_thread_id_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      809 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_session_heartbeat_session_codec.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:20.049892 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1289 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/address_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1150 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/anchor_data_list_holder_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1549 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/bitmap_index_options_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      905 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/distributed_object_info_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1424 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/endpoint_qualifier_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1919 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/error_holder_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1375 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/field_descriptor_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      762 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/hazelcast_json_value_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1918 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/index_config_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2704 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/member_info_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1844 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/member_version_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2940 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/paging_predicate_holder_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1627 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/raft_group_id_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1044 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/schema_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     4880 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/simple_entry_view_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1925 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/sql_column_metadata_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2157 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/sql_error_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2434 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/sql_query_id_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1729 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/stack_trace_element_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      780 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/executor_service_is_shutdown_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      495 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/executor_service_shutdown_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1168 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/executor_service_submit_to_member_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      994 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/executor_service_submit_to_partition_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1553 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/fenced_lock_get_lock_ownership_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1475 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/fenced_lock_lock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1644 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/fenced_lock_try_lock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1478 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/fenced_lock_unlock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1397 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/flake_id_generator_new_id_batch_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      972 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1157 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_all_with_index_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2002 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      833 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_with_index_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      495 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_clear_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      964 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_compare_and_remove_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      964 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_compare_and_retain_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      963 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_contains_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      874 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_contains_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      712 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_get_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      944 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      870 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_index_of_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      779 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_is_empty_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      712 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_iterator_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      870 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_last_index_of_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      955 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_list_iterator_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1016 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_remove_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      945 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_remove_with_index_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      991 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      775 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1079 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_sub_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2696 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_entry_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2738 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_entry_listener_to_key_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2786 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_entry_listener_to_key_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2750 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_entry_listener_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      634 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_index_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      684 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_interceptor_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3168 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_near_cache_invalidation_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      755 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_aggregate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      803 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_aggregate_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      493 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_clear_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1075 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_contains_key_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      872 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_contains_value_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      849 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_delete_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1121 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_entries_with_paging_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      772 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_entries_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      718 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_entry_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      493 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_evict_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1076 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_evict_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      785 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_execute_on_all_keys_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1067 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_execute_on_key_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      910 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_execute_on_keys_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      833 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_execute_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      493 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_flush_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      863 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_force_unlock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      850 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_get_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1006 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1355 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_get_entry_view_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      777 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_is_empty_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      868 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_is_locked_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      710 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_key_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1113 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_key_set_with_paging_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      764 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_key_set_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      834 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_load_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1014 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_load_given_keys_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1161 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_lock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      784 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_project_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      832 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_project_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1003 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1181 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1181 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_if_absent_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1340 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_if_absent_with_max_idle_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1023 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_transient_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1340 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_transient_with_max_idle_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1340 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_with_max_idle_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      590 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1007 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1014 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_entry_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1116 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_if_same_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      814 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_interceptor_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1047 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_replace_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1166 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_replace_if_same_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1023 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1046 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_set_ttl_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1340 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_set_with_max_idle_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      773 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1552 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_try_lock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1270 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_try_put_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1230 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_try_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1027 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_unlock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      710 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_values_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1113 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_values_with_paging_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      764 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_values_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2512 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_add_entry_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2554 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_add_entry_listener_to_key_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      495 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_clear_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1117 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_contains_entry_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1077 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_contains_key_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      874 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_contains_value_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      720 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_entry_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      865 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_force_unlock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1019 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      870 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_is_locked_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      712 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_key_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1163 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_lock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      746 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_put_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1118 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_put_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1020 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1118 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_remove_entry_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1016 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_remove_entry_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      775 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1554 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_try_lock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1029 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_unlock_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1073 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_value_count_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      712 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_values_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1842 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/pn_counter_add_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1487 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/pn_counter_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      777 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/pn_counter_get_configured_replica_count_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      970 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_add_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2002 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_add_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      495 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_clear_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      970 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_compare_and_remove_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      970 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_compare_and_retain_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      970 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_contains_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_contains_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      971 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_drain_to_max_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      780 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_is_empty_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      713 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_iterator_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1107 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_offer_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      702 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_peek_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      992 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_poll_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      590 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_put_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      776 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_remaining_capacity_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1016 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_remove_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      776 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      702 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_take_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2322 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2364 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_to_key_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2412 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_to_key_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2376 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      495 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_clear_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      870 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_contains_key_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      874 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_contains_value_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      720 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_entry_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      743 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      779 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_is_empty_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      712 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_key_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      689 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_put_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1019 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_put_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      744 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1016 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_remove_entry_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      775 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      712 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_values_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1206 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_add_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1109 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_add_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      778 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_capacity_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      778 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_head_sequence_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2019 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_read_many_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      963 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_read_one_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      778 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_remaining_capacity_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      778 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      778 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_tail_sequence_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1799 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_acquire_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      909 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_available_permits_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1630 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_change_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1474 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_drain_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      791 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_get_semaphore_type_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1108 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_init_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1630 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_release_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      972 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_add_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_add_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2002 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_add_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      495 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_clear_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      964 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_compare_and_remove_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      964 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_compare_and_retain_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      962 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_contains_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_contains_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      713 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_get_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      780 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_is_empty_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      875 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1016 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_remove_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      776 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      537 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/sql_close_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2720 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/sql_execute_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1308 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/sql_fetch_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1763 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/topic_add_message_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      683 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/topic_publish_all_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      594 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/topic_publish_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1016 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/topic_remove_message_listener_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      860 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transaction_commit_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1413 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transaction_create_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      860 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transaction_rollback_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1231 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_list_add_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1231 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_list_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1134 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_list_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1227 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_contains_key_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1000 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_delete_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1158 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1158 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_get_for_update_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1136 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_is_empty_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1127 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_key_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1181 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_key_set_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1332 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_put_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1198 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_put_if_absent_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1158 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1267 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_remove_if_same_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1198 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_replace_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1323 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_replace_if_same_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1040 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_set_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1132 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1127 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_values_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1181 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_values_with_predicate_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1169 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_get_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1267 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_put_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1169 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1267 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_remove_entry_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1132 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1223 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_value_count_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1385 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_offer_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1272 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_peek_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1272 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_poll_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1134 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_size_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1118 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_take_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1231 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_set_add_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1231 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_set_remove_codec.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1134 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_set_size_codec.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:20.049892 hazelcast-python-client-5.3.0/hazelcast/proxy/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3366 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     8853 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/base.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:20.049892 hazelcast-python-client-5.3.0/hazelcast/proxy/cp/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2777 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/cp/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    12255 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/cp/atomic_long.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    13673 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/cp/atomic_reference.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     7013 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/cp/count_down_latch.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    20531 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/cp/fenced_lock.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    26238 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/cp/semaphore.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     6450 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/executor.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     7363 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/flake_id_generator.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    22954 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/list.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    91050 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/map.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    28442 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/multi_map.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    14045 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/pn_counter.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    19223 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/queue.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    30702 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/reliable_topic.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    20727 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/replicated_map.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    18381 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/ringbuffer.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    12795 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/set.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     5301 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/topic.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2495 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_list.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    16519 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_map.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     5995 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_multi_map.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3983 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_queue.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2450 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_set.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    19104 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/reactor.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      924 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/security.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:20.059892 hazelcast-python-client-5.3.0/hazelcast/serialization/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      139 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    79208 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/api.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1166 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/bits.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    85139 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/compact.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     2556 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/data.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     7609 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/input.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     3964 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/objects.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     9182 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/output.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:20.059892 hazelcast-python-client-5.3.0/hazelcast/serialization/portable/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       48 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/portable/__init__.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    26041 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/portable/classdef.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     6619 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/portable/context.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    24966 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/portable/reader.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     4427 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/portable/serializer.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    17762 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/portable/writer.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1343 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/serialization_const.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    10152 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/serializer.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    21275 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/service.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     4129 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/serialization/util.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    48167 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/sql.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    14211 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/statistics.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     9670 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/transaction.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)      385 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/types.py
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    11858 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/hazelcast/util.py
-drwxr-xr-x   0 ec2-user  (1000) ec2-user  (1000)        0 2023-06-12 14:29:20.059892 hazelcast-python-client-5.3.0/hazelcast_python_client.egg-info/
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     8829 2023-06-12 14:29:19.000000 hazelcast-python-client-5.3.0/hazelcast_python_client.egg-info/PKG-INFO
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)    18352 2023-06-12 14:29:19.000000 hazelcast-python-client-5.3.0/hazelcast_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)        1 2023-06-12 14:29:19.000000 hazelcast-python-client-5.3.0/hazelcast_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       16 2023-06-12 14:29:19.000000 hazelcast-python-client-5.3.0/hazelcast_python_client.egg-info/requires.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       10 2023-06-12 14:29:19.000000 hazelcast-python-client-5.3.0/hazelcast_python_client.egg-info/top_level.txt
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)       38 2023-06-12 14:29:20.059892 hazelcast-python-client-5.3.0/setup.cfg
--rw-r--r--   0 ec2-user  (1000) ec2-user  (1000)     1984 2023-06-12 14:28:16.000000 hazelcast-python-client-5.3.0/setup.py
+drwxrwxr-x   0 yuce      (1000) yuce      (1000)        0 2024-05-17 10:02:34.701533 hazelcast_python_client-5.4.0/
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    11358 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/LICENSE.txt
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)       47 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/MANIFEST.in
+-rw-r--r--   0 yuce      (1000) yuce      (1000)     8917 2024-05-17 10:02:34.701533 hazelcast_python_client-5.4.0/PKG-INFO
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     7595 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/README.rst
+drwxrwxr-x   0 yuce      (1000) yuce      (1000)        0 2024-05-17 10:02:34.569531 hazelcast_python_client-5.4.0/hazelcast/
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      246 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/__init__.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    16433 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/aggregator.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    20114 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/asyncore.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    22520 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/client.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    13634 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/cluster.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     6168 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/compact.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    72376 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/config.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    38921 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/connection.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    14181 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/core.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    17582 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/cp.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    16593 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/db.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     4478 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/discovery.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    15384 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/errors.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     9302 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/future.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1650 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/hash.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    16602 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/invocation.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     3385 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/lifecycle.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    11857 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/listener.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    12904 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/metrics.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    10787 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/near_cache.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     5420 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/partition.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    23360 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/predicate.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     3225 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/projection.py
+drwxrwxr-x   0 yuce      (1000) yuce      (1000)        0 2024-05-17 10:02:34.573531 hazelcast_python_client-5.4.0/hazelcast/protocol/
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     4297 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/__init__.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    25744 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/builtin.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     9174 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/client_message.py
+drwxrwxr-x   0 yuce      (1000) yuce      (1000)        0 2024-05-17 10:02:34.665532 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)        0 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/__init__.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1098 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_long_add_and_get_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1257 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_long_alter_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      888 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_long_apply_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1270 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_long_compare_and_set_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1098 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_long_get_and_add_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1118 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_long_get_and_set_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      910 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_long_get_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1341 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_ref_apply_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1168 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_ref_compare_and_set_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1084 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_ref_contains_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      835 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_ref_get_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1223 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_ref_set_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1819 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_add_cluster_view_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1677 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_add_distributed_object_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     3002 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_authentication_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2963 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_authentication_custom_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      547 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_create_proxy_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      547 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_destroy_proxy_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      893 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_fetch_schema_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      689 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_get_distributed_objects_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1267 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_local_backup_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      401 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_ping_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      921 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_remove_distributed_object_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      601 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_send_all_schemas_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      649 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_send_schema_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      895 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_statistics_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1314 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/count_down_latch_await_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1105 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/count_down_latch_count_down_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      909 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/count_down_latch_get_count_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      909 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/count_down_latch_get_round_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1098 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/count_down_latch_try_set_count_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      678 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/cp_group_create_cp_group_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      700 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/cp_group_destroy_cp_object_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1036 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/cp_session_close_session_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1429 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/cp_session_create_session_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      821 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/cp_session_generate_thread_id_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      809 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/cp_session_heartbeat_session_codec.py
+drwxrwxr-x   0 yuce      (1000) yuce      (1000)        0 2024-05-17 10:02:34.673532 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)        0 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/__init__.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1289 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/address_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1150 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/anchor_data_list_holder_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1549 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/bitmap_index_options_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      905 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/distributed_object_info_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1424 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/endpoint_qualifier_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1919 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/error_holder_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1375 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/field_descriptor_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      762 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/hazelcast_json_value_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1918 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/index_config_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2704 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/member_info_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1844 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/member_version_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2940 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/paging_predicate_holder_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1627 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/raft_group_id_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1044 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/schema_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     4880 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/simple_entry_view_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1925 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/sql_column_metadata_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2157 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/sql_error_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2434 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/sql_query_id_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1729 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/stack_trace_element_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      780 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/executor_service_is_shutdown_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      495 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/executor_service_shutdown_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1168 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/executor_service_submit_to_member_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      994 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/executor_service_submit_to_partition_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1553 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/fenced_lock_get_lock_ownership_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1475 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/fenced_lock_lock_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1644 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/fenced_lock_try_lock_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1478 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/fenced_lock_unlock_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1397 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/flake_id_generator_new_id_batch_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      972 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_add_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1157 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_add_all_with_index_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      875 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_add_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2002 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_add_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      833 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_add_with_index_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      495 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_clear_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      964 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_compare_and_remove_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      964 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_compare_and_retain_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      963 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_contains_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      874 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_contains_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      712 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_get_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      944 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_get_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      870 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_index_of_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      779 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_is_empty_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      712 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_iterator_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      870 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_last_index_of_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      955 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_list_iterator_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      875 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_remove_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1016 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_remove_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      945 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_remove_with_index_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      991 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_set_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      775 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_size_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1079 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_sub_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2696 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_add_entry_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2738 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_add_entry_listener_to_key_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2786 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_add_entry_listener_to_key_with_predicate_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2750 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_add_entry_listener_with_predicate_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      634 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_add_index_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      684 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_add_interceptor_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     3168 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_add_near_cache_invalidation_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      755 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_aggregate_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      803 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_aggregate_with_predicate_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      493 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_clear_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1075 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_contains_key_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      872 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_contains_value_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      849 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_delete_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1121 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_entries_with_paging_predicate_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      772 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_entries_with_predicate_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      718 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_entry_set_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      493 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_evict_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1076 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_evict_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      785 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_execute_on_all_keys_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1067 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_execute_on_key_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      910 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_execute_on_keys_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      833 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_execute_with_predicate_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      493 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_flush_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      863 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_force_unlock_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      850 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_get_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1006 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_get_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1355 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_get_entry_view_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      777 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_is_empty_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      868 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_is_locked_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      710 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_key_set_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1113 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_key_set_with_paging_predicate_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      764 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_key_set_with_predicate_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      834 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_load_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1014 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_load_given_keys_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1161 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_lock_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      784 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_project_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      832 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_project_with_predicate_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1003 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_put_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1181 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_put_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1181 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_put_if_absent_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1340 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_put_if_absent_with_max_idle_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1023 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_put_transient_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1340 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_put_transient_with_max_idle_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1340 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_put_with_max_idle_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      590 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_remove_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1007 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_remove_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1014 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_remove_entry_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1116 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_remove_if_same_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      814 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_remove_interceptor_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1047 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_replace_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1166 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_replace_if_same_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1023 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_set_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1046 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_set_ttl_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1340 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_set_with_max_idle_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      773 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_size_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1552 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_try_lock_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1270 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_try_put_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1230 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_try_remove_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1027 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_unlock_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      710 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_values_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1113 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_values_with_paging_predicate_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      764 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_values_with_predicate_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2512 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_add_entry_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2554 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_add_entry_listener_to_key_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      495 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_clear_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1117 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_contains_entry_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1077 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_contains_key_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      874 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_contains_value_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      720 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_entry_set_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      865 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_force_unlock_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1019 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_get_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      870 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_is_locked_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      712 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_key_set_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1163 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_lock_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      746 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_put_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1118 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_put_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1020 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_remove_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1118 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_remove_entry_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1016 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_remove_entry_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      775 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_size_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1554 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_try_lock_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1029 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_unlock_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1073 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_value_count_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      712 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_values_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1842 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/pn_counter_add_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1487 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/pn_counter_get_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      777 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/pn_counter_get_configured_replica_count_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      970 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_add_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2002 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_add_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      495 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_clear_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      970 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_compare_and_remove_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      970 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_compare_and_retain_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      970 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_contains_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      875 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_contains_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      971 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_drain_to_max_size_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      780 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_is_empty_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      713 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_iterator_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1107 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_offer_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      702 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_peek_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      992 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_poll_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      590 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_put_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      776 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_remaining_capacity_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      875 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_remove_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1016 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_remove_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      776 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_size_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      702 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_take_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2322 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2364 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_to_key_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2412 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_to_key_with_predicate_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2376 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_with_predicate_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      495 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_clear_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      870 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_contains_key_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      874 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_contains_value_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      720 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_entry_set_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      743 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_get_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      779 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_is_empty_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      712 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_key_set_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      689 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_put_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1019 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_put_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      744 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_remove_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1016 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_remove_entry_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      775 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_size_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      712 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_values_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1206 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/ringbuffer_add_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1109 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/ringbuffer_add_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      778 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/ringbuffer_capacity_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      778 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/ringbuffer_head_sequence_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2019 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/ringbuffer_read_many_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      963 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/ringbuffer_read_one_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      778 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/ringbuffer_remaining_capacity_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      778 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/ringbuffer_size_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      778 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/ringbuffer_tail_sequence_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1799 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/semaphore_acquire_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      909 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/semaphore_available_permits_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1630 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/semaphore_change_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1474 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/semaphore_drain_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      791 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/semaphore_get_semaphore_type_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1108 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/semaphore_init_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1630 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/semaphore_release_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      972 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_add_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      875 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_add_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2002 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_add_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      495 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_clear_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      964 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_compare_and_remove_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      964 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_compare_and_retain_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      962 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_contains_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      875 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_contains_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      713 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_get_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      780 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_is_empty_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      875 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_remove_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1016 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_remove_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      776 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_size_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      537 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/sql_close_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2720 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/sql_execute_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1308 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/sql_fetch_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1763 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/topic_add_message_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      683 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/topic_publish_all_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      594 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/topic_publish_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1016 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/topic_remove_message_listener_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      860 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transaction_commit_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1413 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transaction_create_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      860 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transaction_rollback_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1231 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_list_add_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1231 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_list_remove_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1134 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_list_size_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1227 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_contains_key_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1000 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_delete_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1158 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_get_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1158 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_get_for_update_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1136 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_is_empty_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1127 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_key_set_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1181 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_key_set_with_predicate_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1332 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_put_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1198 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_put_if_absent_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1158 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_remove_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1267 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_remove_if_same_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1198 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_replace_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1323 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_replace_if_same_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1040 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_set_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1132 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_size_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1127 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_values_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1181 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_values_with_predicate_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1169 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_multi_map_get_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1267 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_multi_map_put_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1169 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_multi_map_remove_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1267 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_multi_map_remove_entry_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1132 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_multi_map_size_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1223 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_multi_map_value_count_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1385 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_queue_offer_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1272 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_queue_peek_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1272 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_queue_poll_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1134 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_queue_size_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1118 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_queue_take_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1231 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_set_add_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1231 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_set_remove_codec.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1134 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_set_size_codec.py
+drwxrwxr-x   0 yuce      (1000) yuce      (1000)        0 2024-05-17 10:02:34.685532 hazelcast_python_client-5.4.0/hazelcast/proxy/
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     3366 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/__init__.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     8853 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/base.py
+drwxrwxr-x   0 yuce      (1000) yuce      (1000)        0 2024-05-17 10:02:34.689532 hazelcast_python_client-5.4.0/hazelcast/proxy/cp/
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2777 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/cp/__init__.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    12255 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/cp/atomic_long.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    13673 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/cp/atomic_reference.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     7013 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/cp/count_down_latch.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    20531 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/cp/fenced_lock.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    26238 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/cp/semaphore.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     6450 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/executor.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     7363 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/flake_id_generator.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    22954 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/list.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    91050 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/map.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    28442 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/multi_map.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    14045 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/pn_counter.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    19223 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/queue.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    30981 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/reliable_topic.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    20727 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/replicated_map.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    18381 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/ringbuffer.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    12795 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/set.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     5301 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/topic.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2495 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/transactional_list.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    16519 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/transactional_map.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     5995 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/transactional_multi_map.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     3983 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/transactional_queue.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2450 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/proxy/transactional_set.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    19191 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/reactor.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      924 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/security.py
+drwxrwxr-x   0 yuce      (1000) yuce      (1000)        0 2024-05-17 10:02:34.693533 hazelcast_python_client-5.4.0/hazelcast/serialization/
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      139 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/serialization/__init__.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    79208 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/serialization/api.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1166 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/serialization/bits.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    85139 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/serialization/compact.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2556 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/serialization/data.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     7609 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/serialization/input.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     3964 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/serialization/objects.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     9182 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/serialization/output.py
+drwxrwxr-x   0 yuce      (1000) yuce      (1000)        0 2024-05-17 10:02:34.697533 hazelcast_python_client-5.4.0/hazelcast/serialization/portable/
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)       48 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/serialization/portable/__init__.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    26041 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/serialization/portable/classdef.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     6619 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/serialization/portable/context.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    24966 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/serialization/portable/reader.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     4427 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/serialization/portable/serializer.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    17762 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/serialization/portable/writer.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     1343 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/serialization/serialization_const.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    10152 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/serialization/serializer.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    21275 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/serialization/service.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     4129 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/serialization/util.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    48167 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/sql.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    14211 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/statistics.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     9670 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/transaction.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)      385 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/types.py
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    11858 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/hazelcast/util.py
+drwxrwxr-x   0 yuce      (1000) yuce      (1000)        0 2024-05-17 10:02:34.701533 hazelcast_python_client-5.4.0/hazelcast_python_client.egg-info/
+-rw-r--r--   0 yuce      (1000) yuce      (1000)     8917 2024-05-17 10:02:34.000000 hazelcast_python_client-5.4.0/hazelcast_python_client.egg-info/PKG-INFO
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)    18374 2024-05-17 10:02:34.000000 hazelcast_python_client-5.4.0/hazelcast_python_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)        1 2024-05-17 10:02:34.000000 hazelcast_python_client-5.4.0/hazelcast_python_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)       16 2024-05-17 10:02:34.000000 hazelcast_python_client-5.4.0/hazelcast_python_client.egg-info/requires.txt
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)       10 2024-05-17 10:02:34.000000 hazelcast_python_client-5.4.0/hazelcast_python_client.egg-info/top_level.txt
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)       38 2024-05-17 10:02:34.701533 hazelcast_python_client-5.4.0/setup.cfg
+-rw-rw-r--   0 yuce      (1000) yuce      (1000)     2034 2024-05-17 09:41:13.000000 hazelcast_python_client-5.4.0/setup.py
```

### Comparing `hazelcast-python-client-5.3.0/LICENSE.txt` & `hazelcast_python_client-5.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/PKG-INFO` & `hazelcast_python_client-5.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: hazelcast-python-client
-Version: 5.3.0
+Version: 5.4.0
 Summary: Hazelcast Python Client
 Home-page: https://github.com/hazelcast/hazelcast-python-client
 Author: Hazelcast Inc. Developers
 Author-email: hazelcast@googlegroups.com
 License: Apache 2.0
 Keywords: hazelcast,hazelcast client,In-Memory Data Grid,Distributed Computing
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: stats
 License-File: LICENSE.txt
+Provides-Extra: stats
+Requires-Dist: psutil; extra == "stats"
 
 Hazelcast Python Client
 =======================
 
 .. image:: https://img.shields.io/pypi/v/hazelcast-python-client
     :target: https://pypi.org/project/hazelcast-python-client/
     :alt: PyPI
@@ -168,15 +169,15 @@
    Map data locally in the memory of the client, called **Near Cache**
 -  Additional data structures and simple messaging constructs such as
    **Set**, **MultiMap**, **Queue**, **Topic**
 -  Cluster-wide unique ID generator, called **FlakeIdGenerator**
 -  Distributed, CRDT based counter, called **PNCounter**
 -  Distributed concurrency primitives from CP Subsystem such as
    **FencedLock**, **Semaphore**, **AtomicLong**
--  Integration with `Hazelcast Viridian <https://viridian.hazelcast.com/>`__
+-  Integration with `Hazelcast Cloud <https://cloud.hazelcast.com/>`__
 -  Support for serverless and traditional web service architectures with
    **Unisocket** and **Smart** operation modes
 -  Ability to listen to client lifecycle, cluster state, and distributed
    data structure events
 -  and `many
    more <https://hazelcast.com/clients/python/#client-features>`__
 
@@ -186,17 +187,14 @@
 You can use the following channels for your questions and
 development/usage issues:
 
 -  `GitHub
    repository <https://github.com/hazelcast/hazelcast-python-client/issues/new>`__
 -  `Documentation <https://hazelcast.readthedocs.io>`__
 -  `Slack <https://slack.hazelcast.com>`__
--  `Google Groups <https://groups.google.com/g/hazelcast>`__
--  `Stack
-   Overflow <https://stackoverflow.com/questions/tagged/hazelcast>`__
 
 Contributing
 ------------
 
 We encourage any type of contribution in the form of issue reports or
 pull requests.
 
@@ -240,16 +238,16 @@
 
 Testing
 ^^^^^^^
 
 In order to test Hazelcast Python client locally, you will need the
 following:
 
--  Java 8 or newer
--  Maven
+-  `Supported Java virtual machine <https://docs.hazelcast.com/hazelcast/latest/deploy/versioning-compatibility#supported-java-virtual-machines>`
+-  `Apache Maven <https://maven.apache.org/>`
 
 Following commands starts the tests:
 
 .. code:: bash
 
     python run_tests.py
 
@@ -264,9 +262,7 @@
 Copyright
 ---------
 
 Copyright (c) 2008-2023, Hazelcast, Inc. All Rights Reserved.
 
 Visit `hazelcast.com <https://hazelcast.com>`__ for more
 information.
-
-
```

### Comparing `hazelcast-python-client-5.3.0/README.rst` & `hazelcast_python_client-5.4.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
    Map data locally in the memory of the client, called **Near Cache**
 -  Additional data structures and simple messaging constructs such as
    **Set**, **MultiMap**, **Queue**, **Topic**
 -  Cluster-wide unique ID generator, called **FlakeIdGenerator**
 -  Distributed, CRDT based counter, called **PNCounter**
 -  Distributed concurrency primitives from CP Subsystem such as
    **FencedLock**, **Semaphore**, **AtomicLong**
--  Integration with `Hazelcast Viridian <https://viridian.hazelcast.com/>`__
+-  Integration with `Hazelcast Cloud <https://cloud.hazelcast.com/>`__
 -  Support for serverless and traditional web service architectures with
    **Unisocket** and **Smart** operation modes
 -  Ability to listen to client lifecycle, cluster state, and distributed
    data structure events
 -  and `many
    more <https://hazelcast.com/clients/python/#client-features>`__
 
@@ -157,17 +157,14 @@
 You can use the following channels for your questions and
 development/usage issues:
 
 -  `GitHub
    repository <https://github.com/hazelcast/hazelcast-python-client/issues/new>`__
 -  `Documentation <https://hazelcast.readthedocs.io>`__
 -  `Slack <https://slack.hazelcast.com>`__
--  `Google Groups <https://groups.google.com/g/hazelcast>`__
--  `Stack
-   Overflow <https://stackoverflow.com/questions/tagged/hazelcast>`__
 
 Contributing
 ------------
 
 We encourage any type of contribution in the form of issue reports or
 pull requests.
 
@@ -211,16 +208,16 @@
 
 Testing
 ^^^^^^^
 
 In order to test Hazelcast Python client locally, you will need the
 following:
 
--  Java 8 or newer
--  Maven
+-  `Supported Java virtual machine <https://docs.hazelcast.com/hazelcast/latest/deploy/versioning-compatibility#supported-java-virtual-machines>`
+-  `Apache Maven <https://maven.apache.org/>`
 
 Following commands starts the tests:
 
 .. code:: bash
 
     python run_tests.py
```

### Comparing `hazelcast-python-client-5.3.0/hazelcast/aggregator.py` & `hazelcast_python_client-5.4.0/hazelcast/aggregator.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/client.py` & `hazelcast_python_client-5.4.0/hazelcast/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,15 +526,15 @@
         cluster_members = config.cluster_members
         address_list_provided = len(cluster_members) > 0
         cloud_discovery_token = config.cloud_discovery_token
         cloud_enabled = cloud_discovery_token is not None
         if address_list_provided and cloud_enabled:
             raise IllegalStateError(
                 "Only one discovery method can be enabled at a time. "
-                "Cluster members given explicitly: %s, Hazelcast Viridian enabled: %s"
+                "Cluster members given explicitly: %s, Hazelcast Cloud enabled: %s"
                 % (address_list_provided, cloud_enabled)
             )
 
         if cloud_enabled:
             connection_timeout = self._get_connection_timeout(config)
             return HazelcastCloudAddressProvider(cloud_discovery_token, connection_timeout)
```

### Comparing `hazelcast-python-client-5.3.0/hazelcast/cluster.py` & `hazelcast_python_client-5.4.0/hazelcast/cluster.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/compact.py` & `hazelcast_python_client-5.4.0/hazelcast/compact.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/config.py` & `hazelcast_python_client-5.4.0/hazelcast/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -658,17 +658,17 @@
         if not isinstance(value, bool):
             raise TypeError("ssl_check_hostname must be a boolean")
 
         self._ssl_check_hostname = value
 
     @property
     def cloud_discovery_token(self) -> typing.Optional[str]:
-        """Discovery token of the Hazelcast Viridian cluster.
+        """Discovery token of the Hazelcast Cloud cluster.
 
-        When this value is set, Hazelcast Viridian discovery is enabled.
+        When this value is set, Hazelcast Cloud discovery is enabled.
         """
         return self._cloud_discovery_token
 
     @cloud_discovery_token.setter
     def cloud_discovery_token(self, value: str) -> None:
         if not isinstance(value, str):
             raise TypeError("cloud_discovery_token must be a string")
```

### Comparing `hazelcast-python-client-5.3.0/hazelcast/connection.py` & `hazelcast_python_client-5.4.0/hazelcast/connection.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/core.py` & `hazelcast_python_client-5.4.0/hazelcast/core.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/cp.py` & `hazelcast_python_client-5.4.0/hazelcast/cp.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/db.py` & `hazelcast_python_client-5.4.0/hazelcast/db.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/discovery.py` & `hazelcast_python_client-5.4.0/hazelcast/discovery.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,34 +7,34 @@
 from hazelcast.core import AddressHelper
 
 _logger = logging.getLogger(__name__)
 
 
 class HazelcastCloudAddressProvider:
     """Provides initial addresses for client to find and connect to a node
-    and resolves private IP addresses of Hazelcast Viridian service.
+    and resolves private IP addresses of Hazelcast Cloud service.
     """
 
     def __init__(self, token, connection_timeout):
         self.cloud_discovery = HazelcastCloudDiscovery(token, connection_timeout)
         self._private_to_public = dict()
 
     def load_addresses(self):
-        """Loads member addresses from Hazelcast Viridian endpoint.
+        """Loads member addresses from Hazelcast Cloud endpoint.
 
         Returns:
             tuple[list[hazelcast.core.Address], list[hazelcast.core.Address]]: The possible member addresses
                 as primary addresses to connect to.
         """
         try:
             nodes = self.cloud_discovery.discover_nodes()
             # Every private address is primary
             return list(nodes.keys()), []
         except Exception as e:
-            _logger.warning("Failed to load addresses from Hazelcast Viridian: %s", e)
+            _logger.warning("Failed to load addresses from Hazelcast Cloud: %s", e)
         return [], []
 
     def translate(self, address):
         """Translates the given address to another address specific to network or service.
 
         Args:
             address (hazelcast.core.Address): Private address to be translated
@@ -54,35 +54,35 @@
         return self._private_to_public.get(address, None)
 
     def refresh(self):
         """Refreshes the internal lookup table if necessary."""
         try:
             self._private_to_public = self.cloud_discovery.discover_nodes()
         except Exception as e:
-            _logger.warning("Failed to load addresses from Hazelcast Viridian: %s", e)
+            _logger.warning("Failed to load addresses from Hazelcast Cloud: %s", e)
 
 
 class HazelcastCloudDiscovery:
-    """Service that discovers nodes via Hazelcast Viridian.
-    https://api.viridian.hazelcast.com/cluster/discovery?token=<TOKEN>
+    """Service that discovers nodes via Hazelcast Cloud.
+    https://api.cloud.hazelcast.com/cluster/discovery?token=<TOKEN>
     """
 
-    _CLOUD_URL_BASE = "api.viridian.hazelcast.com"
+    _CLOUD_URL_BASE = "api.cloud.hazelcast.com"
     _CLOUD_URL_PATH = "/cluster/discovery?token="
     _PRIVATE_ADDRESS_PROPERTY = "private-address"
     _PUBLIC_ADDRESS_PROPERTY = "public-address"
 
     def __init__(self, token, connection_timeout):
         self._url = self._CLOUD_URL_PATH + token
         self._connection_timeout = connection_timeout
         # Default context operates only on TLSv1+, checks certificates,hostname and validity
         self._ctx = ssl.create_default_context()
 
     def discover_nodes(self):
-        """Discovers nodes from Hazelcast Viridian.
+        """Discovers nodes from Hazelcast Cloud.
 
         Returns:
             dict[hazelcast.core.Address, hazelcast.core.Address]: Dictionary that maps private
                 addresses to public addresses.
         """
         try:
             https_connection = HTTPSConnection(
```

### Comparing `hazelcast-python-client-5.3.0/hazelcast/errors.py` & `hazelcast_python_client-5.4.0/hazelcast/errors.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/future.py` & `hazelcast_python_client-5.4.0/hazelcast/future.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/hash.py` & `hazelcast_python_client-5.4.0/hazelcast/hash.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/invocation.py` & `hazelcast_python_client-5.4.0/hazelcast/invocation.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/lifecycle.py` & `hazelcast_python_client-5.4.0/hazelcast/lifecycle.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/listener.py` & `hazelcast_python_client-5.4.0/hazelcast/listener.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/metrics.py` & `hazelcast_python_client-5.4.0/hazelcast/metrics.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/near_cache.py` & `hazelcast_python_client-5.4.0/hazelcast/near_cache.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/partition.py` & `hazelcast_python_client-5.4.0/hazelcast/partition.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/predicate.py` & `hazelcast_python_client-5.4.0/hazelcast/predicate.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/projection.py` & `hazelcast_python_client-5.4.0/hazelcast/projection.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/__init__.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/builtin.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/builtin.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/client_message.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/client_message.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_add_and_get_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_long_add_and_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_alter_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_long_alter_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_apply_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_long_apply_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_compare_and_set_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_long_compare_and_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_get_and_add_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_long_get_and_add_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_get_and_set_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_long_get_and_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_long_get_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_long_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_apply_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_ref_apply_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_compare_and_set_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_ref_compare_and_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_contains_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_ref_contains_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_get_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_ref_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/atomic_ref_set_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/atomic_ref_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_add_cluster_view_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_add_cluster_view_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_add_distributed_object_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_add_distributed_object_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_authentication_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_authentication_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_authentication_custom_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_authentication_custom_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_create_proxy_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_create_proxy_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_destroy_proxy_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_destroy_proxy_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_fetch_schema_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_fetch_schema_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_get_distributed_objects_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_get_distributed_objects_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_local_backup_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_local_backup_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_remove_distributed_object_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_remove_distributed_object_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_send_all_schemas_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_send_all_schemas_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_send_schema_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_send_schema_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/client_statistics_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/client_statistics_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_await_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/count_down_latch_await_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_count_down_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/count_down_latch_count_down_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_get_count_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/count_down_latch_get_count_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_get_round_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/count_down_latch_get_round_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/count_down_latch_try_set_count_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/count_down_latch_try_set_count_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_group_create_cp_group_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/cp_group_create_cp_group_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_group_destroy_cp_object_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/cp_group_destroy_cp_object_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_session_close_session_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/cp_session_close_session_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_session_create_session_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/cp_session_create_session_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_session_generate_thread_id_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/cp_session_generate_thread_id_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/cp_session_heartbeat_session_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/cp_session_heartbeat_session_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/address_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/address_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/anchor_data_list_holder_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/anchor_data_list_holder_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/bitmap_index_options_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/bitmap_index_options_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/distributed_object_info_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/distributed_object_info_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/endpoint_qualifier_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/endpoint_qualifier_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/error_holder_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/error_holder_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/field_descriptor_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/field_descriptor_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/hazelcast_json_value_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/hazelcast_json_value_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/index_config_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/index_config_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/member_info_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/member_info_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/member_version_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/member_version_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/paging_predicate_holder_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/paging_predicate_holder_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/raft_group_id_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/raft_group_id_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/schema_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/schema_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/simple_entry_view_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/simple_entry_view_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/sql_column_metadata_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/sql_column_metadata_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/sql_error_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/sql_error_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/sql_query_id_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/sql_query_id_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/custom/stack_trace_element_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/custom/stack_trace_element_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/executor_service_is_shutdown_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/executor_service_is_shutdown_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/executor_service_submit_to_member_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/executor_service_submit_to_member_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/executor_service_submit_to_partition_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/executor_service_submit_to_partition_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/fenced_lock_get_lock_ownership_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/fenced_lock_get_lock_ownership_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/fenced_lock_lock_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/fenced_lock_lock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/fenced_lock_try_lock_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/fenced_lock_try_lock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/fenced_lock_unlock_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/fenced_lock_unlock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/flake_id_generator_new_id_batch_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/flake_id_generator_new_id_batch_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_add_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_all_with_index_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_add_all_with_index_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_add_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_add_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_add_with_index_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_add_with_index_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_compare_and_remove_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_compare_and_remove_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_compare_and_retain_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_compare_and_retain_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_contains_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_contains_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_contains_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_contains_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_get_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_get_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_get_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_index_of_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_index_of_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_is_empty_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_is_empty_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_iterator_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_iterator_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_last_index_of_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_last_index_of_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_list_iterator_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_list_iterator_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_remove_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_remove_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_remove_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_remove_with_index_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_remove_with_index_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_set_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_size_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/list_sub_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/list_sub_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_entry_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_add_entry_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_entry_listener_to_key_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_add_entry_listener_to_key_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_entry_listener_to_key_with_predicate_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_add_entry_listener_to_key_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_entry_listener_with_predicate_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_add_entry_listener_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_index_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_add_index_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_interceptor_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_add_interceptor_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_add_near_cache_invalidation_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_add_near_cache_invalidation_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_aggregate_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_aggregate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_aggregate_with_predicate_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_aggregate_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_contains_key_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_contains_key_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_contains_value_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_contains_value_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_delete_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_delete_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_entries_with_paging_predicate_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_entries_with_paging_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_entries_with_predicate_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_entries_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_entry_set_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_entry_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_evict_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_evict_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_execute_on_all_keys_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_execute_on_all_keys_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_execute_on_key_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_execute_on_key_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_execute_on_keys_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_execute_on_keys_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_execute_with_predicate_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_execute_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_force_unlock_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_force_unlock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_get_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_get_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_get_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_get_entry_view_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_get_entry_view_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_is_empty_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_is_empty_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_is_locked_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_is_locked_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_key_set_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_key_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_key_set_with_paging_predicate_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_key_set_with_paging_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_key_set_with_predicate_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_key_set_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_load_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_load_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_load_given_keys_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_load_given_keys_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_lock_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_lock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_project_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_project_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_project_with_predicate_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_project_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_put_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_put_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_if_absent_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_put_if_absent_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_if_absent_with_max_idle_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_put_if_absent_with_max_idle_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_transient_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_put_transient_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_transient_with_max_idle_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_put_transient_with_max_idle_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_put_with_max_idle_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_put_with_max_idle_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_remove_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_entry_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_remove_entry_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_if_same_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_remove_if_same_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_remove_interceptor_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_remove_interceptor_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_replace_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_replace_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_replace_if_same_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_replace_if_same_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_set_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_set_ttl_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_set_ttl_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_set_with_max_idle_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_set_with_max_idle_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_size_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_try_lock_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_try_lock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_try_put_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_try_put_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_try_remove_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_try_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_unlock_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_unlock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_values_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_values_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_values_with_paging_predicate_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_values_with_paging_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/map_values_with_predicate_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/map_values_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_add_entry_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_add_entry_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_add_entry_listener_to_key_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_add_entry_listener_to_key_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_contains_entry_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_contains_entry_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_contains_key_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_contains_key_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_contains_value_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_contains_value_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_entry_set_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_entry_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_force_unlock_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_force_unlock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_get_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_is_locked_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_is_locked_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_key_set_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_key_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_lock_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_lock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_put_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_put_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_put_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_put_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_remove_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_remove_entry_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_remove_entry_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_remove_entry_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_remove_entry_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_size_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_try_lock_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_try_lock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_unlock_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_unlock_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_value_count_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_value_count_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/multi_map_values_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/multi_map_values_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/pn_counter_add_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/pn_counter_add_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/pn_counter_get_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/pn_counter_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/pn_counter_get_configured_replica_count_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/pn_counter_get_configured_replica_count_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_add_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_add_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_add_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_add_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_compare_and_remove_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_compare_and_remove_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_compare_and_retain_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_compare_and_retain_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_contains_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_contains_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_contains_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_contains_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_drain_to_max_size_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_drain_to_max_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_is_empty_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_is_empty_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_iterator_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_iterator_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_offer_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_offer_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_peek_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_peek_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_poll_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_poll_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_put_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_put_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_remaining_capacity_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_remaining_capacity_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_remove_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_remove_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_remove_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_size_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/queue_take_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/queue_take_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_to_key_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_to_key_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_to_key_with_predicate_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_to_key_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_with_predicate_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_add_entry_listener_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_contains_key_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_contains_key_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_contains_value_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_contains_value_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_entry_set_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_entry_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_get_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_is_empty_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_is_empty_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_key_set_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_key_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_put_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_put_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_put_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_put_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_remove_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_remove_entry_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_remove_entry_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_size_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/replicated_map_values_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/replicated_map_values_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_add_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/ringbuffer_add_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_add_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/ringbuffer_add_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_capacity_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/ringbuffer_capacity_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_head_sequence_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/ringbuffer_head_sequence_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_read_many_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/ringbuffer_read_many_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_read_one_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/ringbuffer_read_one_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_remaining_capacity_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/ringbuffer_remaining_capacity_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_size_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/ringbuffer_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/ringbuffer_tail_sequence_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/ringbuffer_tail_sequence_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_acquire_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/semaphore_acquire_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_available_permits_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/semaphore_available_permits_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_change_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/semaphore_change_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_drain_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/semaphore_drain_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_get_semaphore_type_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/semaphore_get_semaphore_type_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_init_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/semaphore_init_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/semaphore_release_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/semaphore_release_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_add_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_add_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_add_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_add_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_add_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_add_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_compare_and_remove_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_compare_and_remove_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_compare_and_retain_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_compare_and_retain_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_contains_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_contains_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_contains_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_contains_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_get_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_get_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_is_empty_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_is_empty_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_remove_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_remove_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_remove_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/set_size_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/set_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/sql_close_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/sql_close_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/sql_execute_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/sql_execute_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/sql_fetch_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/sql_fetch_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/topic_add_message_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/topic_add_message_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/topic_publish_all_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/topic_publish_all_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/topic_publish_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/topic_publish_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/topic_remove_message_listener_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/topic_remove_message_listener_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transaction_commit_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transaction_commit_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transaction_create_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transaction_create_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transaction_rollback_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transaction_rollback_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_list_add_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_list_add_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_list_remove_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_list_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_list_size_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_list_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_contains_key_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_contains_key_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_delete_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_delete_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_get_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_get_for_update_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_get_for_update_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_is_empty_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_is_empty_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_key_set_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_key_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_key_set_with_predicate_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_key_set_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_put_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_put_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_put_if_absent_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_put_if_absent_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_remove_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_remove_if_same_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_remove_if_same_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_replace_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_replace_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_replace_if_same_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_replace_if_same_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_set_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_set_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_size_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_values_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_values_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_map_values_with_predicate_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_map_values_with_predicate_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_get_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_multi_map_get_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_put_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_multi_map_put_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_remove_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_multi_map_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_remove_entry_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_multi_map_remove_entry_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_size_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_multi_map_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_multi_map_value_count_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_multi_map_value_count_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_offer_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_queue_offer_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_peek_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_queue_peek_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_poll_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_queue_poll_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_size_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_queue_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_queue_take_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_queue_take_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_set_add_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_set_add_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_set_remove_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_set_remove_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/protocol/codec/transactional_set_size_codec.py` & `hazelcast_python_client-5.4.0/hazelcast/protocol/codec/transactional_set_size_codec.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/__init__.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/base.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/base.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/cp/__init__.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/cp/__init__.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/cp/atomic_long.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/cp/atomic_long.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/cp/atomic_reference.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/cp/atomic_reference.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/cp/count_down_latch.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/cp/count_down_latch.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/cp/fenced_lock.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/cp/fenced_lock.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/cp/semaphore.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/cp/semaphore.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/executor.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/executor.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/flake_id_generator.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/flake_id_generator.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/list.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/list.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/map.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/map.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/multi_map.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/multi_map.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/pn_counter.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/pn_counter.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/queue.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/queue.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/reliable_topic.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/reliable_topic.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,14 +146,21 @@
 
         Returns:
             ``True`` if the ReliableMessageListener should terminate itself,
             ``False`` if it should keep on running.
         """
         raise NotImplementedError("is_terminal")
 
+    def on_cancel(self) -> None:
+        """
+        Called when the ReliableMessageListener is cancelled. This can happen
+        when the listener is unregistered or cancelled due to an exception or during shutdown.
+        """
+        pass
+
 
 class _MessageRunner:
     def __init__(
         self,
         registration_id,
         listener,
         ringbuffer,
@@ -207,14 +214,15 @@
 
     def cancel(self):
         """Sets the cancelled flag and removes
         the runner registration.
         """
         self._cancelled = True
         self._runners.pop(self._registration_id, None)
+        self._listener.on_cancel()
 
     def _handle_next_batch(self, future):
         """Handles the result of the read_many request from
         the ringbuffer.
 
         Args:
             future (hazelcast.future.Future):
```

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/replicated_map.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/replicated_map.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/ringbuffer.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/ringbuffer.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/set.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/set.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/topic.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/topic.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_list.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/transactional_list.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_map.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/transactional_map.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_multi_map.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/transactional_multi_map.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_queue.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/transactional_queue.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/proxy/transactional_set.py` & `hazelcast_python_client-5.4.0/hazelcast/proxy/transactional_set.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/reactor.py` & `hazelcast_python_client-5.4.0/hazelcast/reactor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-import asyncore
+try:
+    import asyncore
+except ImportError:
+    import hazelcast.asyncore as asyncore  # type: ignore
 import errno
 import io
 import logging
 import os
 import select
 import socket
 import ssl
```

### Comparing `hazelcast-python-client-5.3.0/hazelcast/security.py` & `hazelcast_python_client-5.4.0/hazelcast/security.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/serialization/api.py` & `hazelcast_python_client-5.4.0/hazelcast/serialization/api.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/serialization/bits.py` & `hazelcast_python_client-5.4.0/hazelcast/serialization/bits.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/serialization/compact.py` & `hazelcast_python_client-5.4.0/hazelcast/serialization/compact.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/serialization/data.py` & `hazelcast_python_client-5.4.0/hazelcast/serialization/data.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/serialization/input.py` & `hazelcast_python_client-5.4.0/hazelcast/serialization/input.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/serialization/objects.py` & `hazelcast_python_client-5.4.0/hazelcast/serialization/objects.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/serialization/output.py` & `hazelcast_python_client-5.4.0/hazelcast/serialization/output.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/serialization/portable/classdef.py` & `hazelcast_python_client-5.4.0/hazelcast/serialization/portable/classdef.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/serialization/portable/context.py` & `hazelcast_python_client-5.4.0/hazelcast/serialization/portable/context.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/serialization/portable/reader.py` & `hazelcast_python_client-5.4.0/hazelcast/serialization/portable/reader.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/serialization/portable/serializer.py` & `hazelcast_python_client-5.4.0/hazelcast/serialization/portable/serializer.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/serialization/portable/writer.py` & `hazelcast_python_client-5.4.0/hazelcast/serialization/portable/writer.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/serialization/serialization_const.py` & `hazelcast_python_client-5.4.0/hazelcast/serialization/serialization_const.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/serialization/serializer.py` & `hazelcast_python_client-5.4.0/hazelcast/serialization/serializer.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/serialization/service.py` & `hazelcast_python_client-5.4.0/hazelcast/serialization/service.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/serialization/util.py` & `hazelcast_python_client-5.4.0/hazelcast/serialization/util.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/sql.py` & `hazelcast_python_client-5.4.0/hazelcast/sql.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/statistics.py` & `hazelcast_python_client-5.4.0/hazelcast/statistics.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/transaction.py` & `hazelcast_python_client-5.4.0/hazelcast/transaction.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast/util.py` & `hazelcast_python_client-5.4.0/hazelcast/util.py`

 * *Files identical despite different names*

### Comparing `hazelcast-python-client-5.3.0/hazelcast_python_client.egg-info/PKG-INFO` & `hazelcast_python_client-5.4.0/hazelcast_python_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: hazelcast-python-client
-Version: 5.3.0
+Version: 5.4.0
 Summary: Hazelcast Python Client
 Home-page: https://github.com/hazelcast/hazelcast-python-client
 Author: Hazelcast Inc. Developers
 Author-email: hazelcast@googlegroups.com
 License: Apache 2.0
 Keywords: hazelcast,hazelcast client,In-Memory Data Grid,Distributed Computing
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: stats
 License-File: LICENSE.txt
+Provides-Extra: stats
+Requires-Dist: psutil; extra == "stats"
 
 Hazelcast Python Client
 =======================
 
 .. image:: https://img.shields.io/pypi/v/hazelcast-python-client
     :target: https://pypi.org/project/hazelcast-python-client/
     :alt: PyPI
@@ -168,15 +169,15 @@
    Map data locally in the memory of the client, called **Near Cache**
 -  Additional data structures and simple messaging constructs such as
    **Set**, **MultiMap**, **Queue**, **Topic**
 -  Cluster-wide unique ID generator, called **FlakeIdGenerator**
 -  Distributed, CRDT based counter, called **PNCounter**
 -  Distributed concurrency primitives from CP Subsystem such as
    **FencedLock**, **Semaphore**, **AtomicLong**
--  Integration with `Hazelcast Viridian <https://viridian.hazelcast.com/>`__
+-  Integration with `Hazelcast Cloud <https://cloud.hazelcast.com/>`__
 -  Support for serverless and traditional web service architectures with
    **Unisocket** and **Smart** operation modes
 -  Ability to listen to client lifecycle, cluster state, and distributed
    data structure events
 -  and `many
    more <https://hazelcast.com/clients/python/#client-features>`__
 
@@ -186,17 +187,14 @@
 You can use the following channels for your questions and
 development/usage issues:
 
 -  `GitHub
    repository <https://github.com/hazelcast/hazelcast-python-client/issues/new>`__
 -  `Documentation <https://hazelcast.readthedocs.io>`__
 -  `Slack <https://slack.hazelcast.com>`__
--  `Google Groups <https://groups.google.com/g/hazelcast>`__
--  `Stack
-   Overflow <https://stackoverflow.com/questions/tagged/hazelcast>`__
 
 Contributing
 ------------
 
 We encourage any type of contribution in the form of issue reports or
 pull requests.
 
@@ -240,16 +238,16 @@
 
 Testing
 ^^^^^^^
 
 In order to test Hazelcast Python client locally, you will need the
 following:
 
--  Java 8 or newer
--  Maven
+-  `Supported Java virtual machine <https://docs.hazelcast.com/hazelcast/latest/deploy/versioning-compatibility#supported-java-virtual-machines>`
+-  `Apache Maven <https://maven.apache.org/>`
 
 Following commands starts the tests:
 
 .. code:: bash
 
     python run_tests.py
 
@@ -264,9 +262,7 @@
 Copyright
 ---------
 
 Copyright (c) 2008-2023, Hazelcast, Inc. All Rights Reserved.
 
 Visit `hazelcast.com <https://hazelcast.com>`__ for more
 information.
-
-
```

### Comparing `hazelcast-python-client-5.3.0/hazelcast_python_client.egg-info/SOURCES.txt` & `hazelcast_python_client-5.4.0/hazelcast_python_client.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
 setup.py
 hazelcast/__init__.py
 hazelcast/aggregator.py
+hazelcast/asyncore.py
 hazelcast/client.py
 hazelcast/cluster.py
 hazelcast/compact.py
 hazelcast/config.py
 hazelcast/connection.py
 hazelcast/core.py
 hazelcast/cp.py
```

### Comparing `hazelcast-python-client-5.3.0/setup.py` & `hazelcast_python_client-5.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     license="Apache 2.0",
     keywords="hazelcast,hazelcast client,In-Memory Data Grid,Distributed Computing",
     packages=find_packages(
         exclude=["benchmarks", "examples", "examples.*", "docs", "docs.*", "tests", "tests.*"]
```

