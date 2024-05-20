# Comparing `tmp/lakehouse_engine-1.19.0-py3-none-any.whl.zip` & `tmp/lakehouse_engine-1.20.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,200 +1,205 @@
-Zip file size: 265495 bytes, number of entries: 198
--rw-r--r--  2.0 unx      474 b- defN 24-Mar-14 11:12 lakehouse_engine/__init__.py
--rw-r--r--  2.0 unx    11338 b- defN 24-Mar-14 11:12 lakehouse_engine/engine.py
--rw-r--r--  2.0 unx       62 b- defN 24-Mar-14 11:12 lakehouse_engine/algorithms/__init__.py
--rw-r--r--  2.0 unx     5527 b- defN 24-Mar-14 11:12 lakehouse_engine/algorithms/algorithm.py
--rw-r--r--  2.0 unx    23776 b- defN 24-Mar-14 11:12 lakehouse_engine/algorithms/data_loader.py
--rw-r--r--  2.0 unx     6163 b- defN 24-Mar-14 11:12 lakehouse_engine/algorithms/dq_validator.py
--rw-r--r--  2.0 unx      539 b- defN 24-Mar-14 11:12 lakehouse_engine/algorithms/exceptions.py
--rw-r--r--  2.0 unx    12407 b- defN 24-Mar-14 11:12 lakehouse_engine/algorithms/reconciliator.py
--rw-r--r--  2.0 unx     5887 b- defN 24-Mar-14 11:12 lakehouse_engine/algorithms/sensor.py
--rw-r--r--  2.0 unx       73 b- defN 24-Mar-14 11:12 lakehouse_engine/configs/__init__.py
--rw-r--r--  2.0 unx       29 b- defN 24-Mar-14 11:12 lakehouse_engine/configs/engine.yaml
--rw-r--r--  2.0 unx       63 b- defN 24-Mar-14 11:12 lakehouse_engine/core/__init__.py
--rw-r--r--  2.0 unx     8750 b- defN 24-Mar-14 11:12 lakehouse_engine/core/dbfs_file_manager.py
--rw-r--r--  2.0 unx    31043 b- defN 24-Mar-14 11:12 lakehouse_engine/core/definitions.py
--rw-r--r--  2.0 unx     4088 b- defN 24-Mar-14 11:12 lakehouse_engine/core/exec_env.py
--rw-r--r--  2.0 unx      445 b- defN 24-Mar-14 11:12 lakehouse_engine/core/executable.py
--rw-r--r--  2.0 unx     1903 b- defN 24-Mar-14 11:12 lakehouse_engine/core/file_manager.py
--rw-r--r--  2.0 unx    21478 b- defN 24-Mar-14 11:12 lakehouse_engine/core/s3_file_manager.py
--rw-r--r--  2.0 unx    13664 b- defN 24-Mar-14 11:12 lakehouse_engine/core/sensor_manager.py
--rw-r--r--  2.0 unx    10171 b- defN 24-Mar-14 11:12 lakehouse_engine/core/table_manager.py
--rw-r--r--  2.0 unx       82 b- defN 24-Mar-14 11:12 lakehouse_engine/dq_processors/__init__.py
--rw-r--r--  2.0 unx     7265 b- defN 24-Mar-14 11:12 lakehouse_engine/dq_processors/assistant.py
--rw-r--r--  2.0 unx    23551 b- defN 24-Mar-14 11:12 lakehouse_engine/dq_processors/dq_factory.py
--rw-r--r--  2.0 unx      302 b- defN 24-Mar-14 11:12 lakehouse_engine/dq_processors/exceptions.py
--rw-r--r--  2.0 unx     8904 b- defN 24-Mar-14 11:12 lakehouse_engine/dq_processors/validator.py
--rw-r--r--  2.0 unx       83 b- defN 24-Mar-14 11:12 lakehouse_engine/dq_processors/custom_expectations/__init__.py
--rw-r--r--  2.0 unx     7066 b- defN 24-Mar-14 11:12 lakehouse_engine/dq_processors/custom_expectations/expect_column_pair_a_to_be_smaller_or_equal_than_b.py
--rw-r--r--  2.0 unx     7958 b- defN 24-Mar-14 11:12 lakehouse_engine/dq_processors/custom_expectations/expect_column_values_to_be_date_not_older_than.py
--rw-r--r--  2.0 unx     6647 b- defN 24-Mar-14 11:12 lakehouse_engine/dq_processors/custom_expectations/expect_multicolumn_column_a_must_equal_b_or_c.py
--rw-r--r--  2.0 unx    14618 b- defN 24-Mar-14 11:12 lakehouse_engine/dq_processors/custom_expectations/expect_queried_column_agg_value_to_be.py
--rw-r--r--  2.0 unx       85 b- defN 24-Mar-14 11:12 lakehouse_engine/io/__init__.py
--rw-r--r--  2.0 unx      687 b- defN 24-Mar-14 11:12 lakehouse_engine/io/exceptions.py
--rw-r--r--  2.0 unx      797 b- defN 24-Mar-14 11:12 lakehouse_engine/io/reader.py
--rw-r--r--  2.0 unx     2285 b- defN 24-Mar-14 11:12 lakehouse_engine/io/reader_factory.py
--rw-r--r--  2.0 unx     4720 b- defN 24-Mar-14 11:12 lakehouse_engine/io/writer.py
--rw-r--r--  2.0 unx     2885 b- defN 24-Mar-14 11:12 lakehouse_engine/io/writer_factory.py
--rw-r--r--  2.0 unx       51 b- defN 24-Mar-14 11:12 lakehouse_engine/io/readers/__init__.py
--rw-r--r--  2.0 unx      718 b- defN 24-Mar-14 11:12 lakehouse_engine/io/readers/dataframe_reader.py
--rw-r--r--  2.0 unx     2334 b- defN 24-Mar-14 11:12 lakehouse_engine/io/readers/file_reader.py
--rw-r--r--  2.0 unx     2448 b- defN 24-Mar-14 11:12 lakehouse_engine/io/readers/jdbc_reader.py
--rw-r--r--  2.0 unx      862 b- defN 24-Mar-14 11:12 lakehouse_engine/io/readers/kafka_reader.py
--rw-r--r--  2.0 unx      734 b- defN 24-Mar-14 11:12 lakehouse_engine/io/readers/query_reader.py
--rw-r--r--  2.0 unx     7205 b- defN 24-Mar-14 11:12 lakehouse_engine/io/readers/sap_b4_reader.py
--rw-r--r--  2.0 unx     7299 b- defN 24-Mar-14 11:12 lakehouse_engine/io/readers/sap_bw_reader.py
--rw-r--r--  2.0 unx     5445 b- defN 24-Mar-14 11:12 lakehouse_engine/io/readers/sftp_reader.py
--rw-r--r--  2.0 unx     1300 b- defN 24-Mar-14 11:12 lakehouse_engine/io/readers/table_reader.py
--rw-r--r--  2.0 unx       67 b- defN 24-Mar-14 11:12 lakehouse_engine/io/writers/__init__.py
--rw-r--r--  2.0 unx     4361 b- defN 24-Mar-14 11:12 lakehouse_engine/io/writers/console_writer.py
--rw-r--r--  2.0 unx     7476 b- defN 24-Mar-14 11:12 lakehouse_engine/io/writers/dataframe_writer.py
--rw-r--r--  2.0 unx     7752 b- defN 24-Mar-14 11:12 lakehouse_engine/io/writers/delta_merge_writer.py
--rw-r--r--  2.0 unx     3888 b- defN 24-Mar-14 11:12 lakehouse_engine/io/writers/file_writer.py
--rw-r--r--  2.0 unx     3074 b- defN 24-Mar-14 11:12 lakehouse_engine/io/writers/jdbc_writer.py
--rw-r--r--  2.0 unx     3679 b- defN 24-Mar-14 11:12 lakehouse_engine/io/writers/kafka_writer.py
--rw-r--r--  2.0 unx     5820 b- defN 24-Mar-14 11:12 lakehouse_engine/io/writers/table_writer.py
--rw-r--r--  2.0 unx       87 b- defN 24-Mar-14 11:12 lakehouse_engine/terminators/__init__.py
--rw-r--r--  2.0 unx     4557 b- defN 24-Mar-14 11:12 lakehouse_engine/terminators/cdf_processor.py
--rw-r--r--  2.0 unx     5332 b- defN 24-Mar-14 11:12 lakehouse_engine/terminators/dataset_optimizer.py
--rw-r--r--  2.0 unx     3873 b- defN 24-Mar-14 11:12 lakehouse_engine/terminators/notifier.py
--rw-r--r--  2.0 unx     2934 b- defN 24-Mar-14 11:12 lakehouse_engine/terminators/notifier_factory.py
--rw-r--r--  2.0 unx     2126 b- defN 24-Mar-14 11:12 lakehouse_engine/terminators/sensor_terminator.py
--rw-r--r--  2.0 unx      456 b- defN 24-Mar-14 11:12 lakehouse_engine/terminators/spark_terminator.py
--rw-r--r--  2.0 unx     1990 b- defN 24-Mar-14 11:12 lakehouse_engine/terminators/terminator_factory.py
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-14 11:12 lakehouse_engine/terminators/notifiers/__init__.py
--rw-r--r--  2.0 unx     6683 b- defN 24-Mar-14 11:12 lakehouse_engine/terminators/notifiers/email_notifier.py
--rw-r--r--  2.0 unx     1494 b- defN 24-Mar-14 11:12 lakehouse_engine/terminators/notifiers/notification_templates.py
--rw-r--r--  2.0 unx       72 b- defN 24-Mar-14 11:12 lakehouse_engine/transformers/__init__.py
--rw-r--r--  2.0 unx      895 b- defN 24-Mar-14 11:12 lakehouse_engine/transformers/aggregators.py
--rw-r--r--  2.0 unx     3325 b- defN 24-Mar-14 11:12 lakehouse_engine/transformers/column_creators.py
--rw-r--r--  2.0 unx    15223 b- defN 24-Mar-14 11:12 lakehouse_engine/transformers/column_reshapers.py
--rw-r--r--  2.0 unx     4866 b- defN 24-Mar-14 11:12 lakehouse_engine/transformers/condensers.py
--rw-r--r--  2.0 unx     1260 b- defN 24-Mar-14 11:12 lakehouse_engine/transformers/custom_transformers.py
--rw-r--r--  2.0 unx     2168 b- defN 24-Mar-14 11:12 lakehouse_engine/transformers/data_maskers.py
--rw-r--r--  2.0 unx     5331 b- defN 24-Mar-14 11:12 lakehouse_engine/transformers/date_transformers.py
--rw-r--r--  2.0 unx      341 b- defN 24-Mar-14 11:12 lakehouse_engine/transformers/exceptions.py
--rw-r--r--  2.0 unx     6359 b- defN 24-Mar-14 11:12 lakehouse_engine/transformers/filters.py
--rw-r--r--  2.0 unx     3624 b- defN 24-Mar-14 11:12 lakehouse_engine/transformers/joiners.py
--rw-r--r--  2.0 unx     1555 b- defN 24-Mar-14 11:12 lakehouse_engine/transformers/null_handlers.py
--rw-r--r--  2.0 unx     1926 b- defN 24-Mar-14 11:12 lakehouse_engine/transformers/optimizers.py
--rw-r--r--  2.0 unx     1240 b- defN 24-Mar-14 11:12 lakehouse_engine/transformers/regex_transformers.py
--rw-r--r--  2.0 unx     1817 b- defN 24-Mar-14 11:12 lakehouse_engine/transformers/repartitioners.py
--rw-r--r--  2.0 unx     5889 b- defN 24-Mar-14 11:12 lakehouse_engine/transformers/transformer_factory.py
--rw-r--r--  2.0 unx     1956 b- defN 24-Mar-14 11:12 lakehouse_engine/transformers/unions.py
--rw-r--r--  2.0 unx      918 b- defN 24-Mar-14 11:12 lakehouse_engine/transformers/watermarker.py
--rw-r--r--  2.0 unx       25 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/__init__.py
--rw-r--r--  2.0 unx     1636 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/databricks_utils.py
--rw-r--r--  2.0 unx     4950 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/engine_usage_stats.py
--rw-r--r--  2.0 unx     4691 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/expectations_utils.py
--rw-r--r--  2.0 unx     1079 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/file_utils.py
--rw-r--r--  2.0 unx     2864 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/logging_handler.py
--rw-r--r--  2.0 unx     6594 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/schema_utils.py
--rw-r--r--  2.0 unx     7327 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/sql_parser_utils.py
--rw-r--r--  2.0 unx       32 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/configs/__init__.py
--rw-r--r--  2.0 unx     3444 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/configs/config_utils.py
--rw-r--r--  2.0 unx       36 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/extraction/__init__.py
--rw-r--r--  2.0 unx    15419 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/extraction/jdbc_extraction_utils.py
--rw-r--r--  2.0 unx    11821 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/extraction/sap_b4_extraction_utils.py
--rw-r--r--  2.0 unx    14221 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/extraction/sap_bw_extraction_utils.py
--rw-r--r--  2.0 unx    18533 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/extraction/sftp_extraction_utils.py
--rw-r--r--  2.0 unx       50 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/storage/__init__.py
--rw-r--r--  2.0 unx     1473 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/storage/dbfs_storage.py
--rw-r--r--  2.0 unx      774 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/storage/file_storage.py
--rw-r--r--  2.0 unx     3232 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/storage/file_storage_functions.py
--rw-r--r--  2.0 unx     1280 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/storage/local_fs_storage.py
--rw-r--r--  2.0 unx     1298 b- defN 24-Mar-14 11:12 lakehouse_engine/utils/storage/s3_storage.py
--rw-r--r--  2.0 unx    12260 b- defN 24-Mar-14 11:12 lakehouse_engine-1.19.0.data/data/requirements/requirements_os.lock
--rw-r--r--  2.0 unx      356 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/__init__.py
--rw-r--r--  2.0 unx       35 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/__init__.py
--rw-r--r--  2.0 unx       65 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/append_load_from_jdbc_with_permissive_mode/__init__.py
--rw-r--r--  2.0 unx       48 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/append_load_with_failfast/__init__.py
--rw-r--r--  2.0 unx       70 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/batch_delta_load_init_delta_backfill_with_merge/__init__.py
--rw-r--r--  2.0 unx       42 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/custom_transformer/__init__.py
--rw-r--r--  2.0 unx       48 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/extract_from_sap_b4_adso/__init__.py
--rw-r--r--  2.0 unx       46 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/extract_from_sap_bw_dso/__init__.py
--rw-r--r--  2.0 unx       41 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/extract_from_sftp/__init__.py
--rw-r--r--  2.0 unx       53 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/extract_using_jdbc_connection/__init__.py
--rw-r--r--  2.0 unx       42 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/filtered_full_load/__init__.py
--rw-r--r--  2.0 unx       64 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/filtered_full_load_with_selective_replace/__init__.py
--rw-r--r--  2.0 unx       58 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/flatten_schema_and_explode_columns/__init__.py
--rw-r--r--  2.0 unx       33 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/full_load/__init__.py
--rw-r--r--  2.0 unx       43 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/read_from_dataframe/__init__.py
--rw-r--r--  2.0 unx       60 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/streaming_append_load_with_malformed/__init__.py
--rw-r--r--  2.0 unx       61 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/streaming_append_load_with_terminator/__init__.py
--rw-r--r--  2.0 unx       77 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/streaming_delta_load_with_group_and_rank_condensation/__init__.py
--rw-r--r--  2.0 unx       82 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/streaming_delta_with_late_arriving_and_out_of_order_events/__init__.py
--rw-r--r--  2.0 unx       48 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/write_and_read_dataframe/__init__.py
--rw-r--r--  2.0 unx       40 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_loader/write_to_console/__init__.py
--rw-r--r--  2.0 unx       36 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_quality/__init__.py
--rw-r--r--  2.0 unx       43 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_quality/custom_expectations/__init__.py
--rw-r--r--  2.0 unx       46 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_quality/data_quality_validator/__init__.py
--rw-r--r--  2.0 unx       39 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_quality/minimal_example/__init__.py
--rw-r--r--  2.0 unx       35 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_quality/result_sink/__init__.py
--rw-r--r--  2.0 unx       35 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_quality/row_tagging/__init__.py
--rw-r--r--  2.0 unx       43 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/data_quality/validations_failing/__init__.py
--rw-r--r--  2.0 unx       37 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/reconciliator/__init__.py
--rw-r--r--  2.0 unx       30 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/sensor/__init__.py
--rw-r--r--  2.0 unx       35 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/sensor/delta_table/__init__.py
--rw-r--r--  2.0 unx       51 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/sensor/delta_upstream_sensor_table/__init__.py
--rw-r--r--  2.0 unx       28 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/sensor/file/__init__.py
--rw-r--r--  2.0 unx       34 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/sensor/jdbc_table/__init__.py
--rw-r--r--  2.0 unx       29 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/sensor/kafka/__init__.py
--rw-r--r--  2.0 unx       33 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/sensor/sap_bw_b4/__init__.py
--rw-r--r--  2.0 unx       44 b- defN 24-Mar-14 11:12 lakehouse_engine_usage/sensor/update_sensor_status/__init__.py
--rw-r--r--  2.0 unx       21 b- defN 24-Mar-14 11:12 tests/__init__.py
--rw-r--r--  2.0 unx     1968 b- defN 24-Mar-14 11:12 tests/conftest.py
--rw-r--r--  2.0 unx       54 b- defN 24-Mar-14 11:12 tests/configs/__init__.py
--rw-r--r--  2.0 unx       89 b- defN 24-Mar-14 11:12 tests/feature/__init__.py
--rw-r--r--  2.0 unx     6329 b- defN 24-Mar-14 11:12 tests/feature/test_append_load.py
--rw-r--r--  2.0 unx    22498 b- defN 24-Mar-14 11:12 tests/feature/test_data_quality.py
--rw-r--r--  2.0 unx    17643 b- defN 24-Mar-14 11:12 tests/feature/test_dq_validator.py
--rw-r--r--  2.0 unx     7928 b- defN 24-Mar-14 11:12 tests/feature/test_engine_usage_stats.py
--rw-r--r--  2.0 unx    17735 b- defN 24-Mar-14 11:12 tests/feature/test_extract_from_sap_b4.py
--rw-r--r--  2.0 unx    23508 b- defN 24-Mar-14 11:12 tests/feature/test_extract_from_sap_bw.py
--rw-r--r--  2.0 unx    10590 b- defN 24-Mar-14 11:12 tests/feature/test_file_manager.py
--rw-r--r--  2.0 unx     9124 b- defN 24-Mar-14 11:12 tests/feature/test_file_manager_dbfs.py
--rw-r--r--  2.0 unx    11234 b- defN 24-Mar-14 11:12 tests/feature/test_file_manager_s3.py
--rw-r--r--  2.0 unx     2499 b- defN 24-Mar-14 11:12 tests/feature/test_full_load.py
--rw-r--r--  2.0 unx     4573 b- defN 24-Mar-14 11:12 tests/feature/test_jdbc_reader.py
--rw-r--r--  2.0 unx     4116 b- defN 24-Mar-14 11:12 tests/feature/test_materialize_cdf.py
--rw-r--r--  2.0 unx    16028 b- defN 24-Mar-14 11:12 tests/feature/test_notification.py
--rw-r--r--  2.0 unx    14219 b- defN 24-Mar-14 11:12 tests/feature/test_reconciliation.py
--rw-r--r--  2.0 unx    20111 b- defN 24-Mar-14 11:12 tests/feature/test_schema_evolution.py
--rw-r--r--  2.0 unx    16396 b- defN 24-Mar-14 11:12 tests/feature/test_sensors.py
--rw-r--r--  2.0 unx    19193 b- defN 24-Mar-14 11:12 tests/feature/test_sftp_reader.py
--rw-r--r--  2.0 unx     9422 b- defN 24-Mar-14 11:12 tests/feature/test_table_manager.py
--rw-r--r--  2.0 unx    14023 b- defN 24-Mar-14 11:12 tests/feature/test_writers.py
--rw-r--r--  2.0 unx       64 b- defN 24-Mar-14 11:12 tests/feature/custom_expectations/__init__.py
--rw-r--r--  2.0 unx     9212 b- defN 24-Mar-14 11:12 tests/feature/custom_expectations/test_custom_expectations.py
--rw-r--r--  2.0 unx     3823 b- defN 24-Mar-14 11:12 tests/feature/custom_expectations/test_expectation_validity.py
--rw-r--r--  2.0 unx       89 b- defN 24-Mar-14 11:12 tests/feature/data_loader_custom_transformer/__init__.py
--rw-r--r--  2.0 unx     4060 b- defN 24-Mar-14 11:12 tests/feature/data_loader_custom_transformer/test_data_loader_custom_transformer_calculate_kpi.py
--rw-r--r--  2.0 unx     7613 b- defN 24-Mar-14 11:12 tests/feature/data_loader_custom_transformer/test_data_loader_custom_transformer_delta_load.py
--rw-r--r--  2.0 unx       32 b- defN 24-Mar-14 11:12 tests/feature/delta_load/__init__.py
--rw-r--r--  2.0 unx     5343 b- defN 24-Mar-14 11:12 tests/feature/delta_load/test_delta_load_group_and_rank.py
--rw-r--r--  2.0 unx     3481 b- defN 24-Mar-14 11:12 tests/feature/delta_load/test_delta_load_merge_options.py
--rw-r--r--  2.0 unx     9547 b- defN 24-Mar-14 11:12 tests/feature/delta_load/test_delta_load_record_mode_cdc.py
--rw-r--r--  2.0 unx       37 b- defN 24-Mar-14 11:12 tests/feature/transformations/__init__.py
--rw-r--r--  2.0 unx     4310 b- defN 24-Mar-14 11:12 tests/feature/transformations/test_chain_transformations.py
--rw-r--r--  2.0 unx     1947 b- defN 24-Mar-14 11:12 tests/feature/transformations/test_column_creators.py
--rw-r--r--  2.0 unx     2625 b- defN 24-Mar-14 11:12 tests/feature/transformations/test_column_reshapers.py
--rw-r--r--  2.0 unx     1999 b- defN 24-Mar-14 11:12 tests/feature/transformations/test_data_maskers.py
--rw-r--r--  2.0 unx     1816 b- defN 24-Mar-14 11:12 tests/feature/transformations/test_date_transformers.py
--rw-r--r--  2.0 unx     3319 b- defN 24-Mar-14 11:12 tests/feature/transformations/test_drop_duplicate_rows.py
--rw-r--r--  2.0 unx     3029 b- defN 24-Mar-14 11:12 tests/feature/transformations/test_joiners.py
--rw-r--r--  2.0 unx     2298 b- defN 24-Mar-14 11:12 tests/feature/transformations/test_multiple_transformations.py
--rw-r--r--  2.0 unx     1863 b- defN 24-Mar-14 11:12 tests/feature/transformations/test_null_handlers.py
--rw-r--r--  2.0 unx     3489 b- defN 24-Mar-14 11:12 tests/feature/transformations/test_optimizers.py
--rw-r--r--  2.0 unx     1996 b- defN 24-Mar-14 11:12 tests/feature/transformations/test_regex_transformers.py
--rw-r--r--  2.0 unx     4981 b- defN 24-Mar-14 11:12 tests/feature/transformations/test_unions.py
--rw-r--r--  2.0 unx     6275 b- defN 24-Mar-14 11:12 tests/feature/transformations/test_watermarker.py
--rw-r--r--  2.0 unx       23 b- defN 24-Mar-14 11:12 tests/utils/__init__.py
--rw-r--r--  2.0 unx     6959 b- defN 24-Mar-14 11:12 tests/utils/dataframe_helpers.py
--rw-r--r--  2.0 unx     1960 b- defN 24-Mar-14 11:12 tests/utils/exec_env_helpers.py
--rw-r--r--  2.0 unx     1513 b- defN 24-Mar-14 11:12 tests/utils/local_storage.py
--rw-r--r--  2.0 unx    11339 b- defN 24-Mar-14 11:13 lakehouse_engine-1.19.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    24843 b- defN 24-Mar-14 11:13 lakehouse_engine-1.19.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-14 11:13 lakehouse_engine-1.19.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       46 b- defN 24-Mar-14 11:13 lakehouse_engine-1.19.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    20783 b- defN 24-Mar-14 11:13 lakehouse_engine-1.19.0.dist-info/RECORD
-198 files, 913809 bytes uncompressed, 231103 bytes compressed:  74.7%
+Zip file size: 294885 bytes, number of entries: 203
+-rw-r--r--  2.0 unx      474 b- defN 24-May-20 15:04 lakehouse_engine/__init__.py
+-rw-r--r--  2.0 unx    14690 b- defN 24-May-20 15:04 lakehouse_engine/engine.py
+-rw-r--r--  2.0 unx       62 b- defN 24-May-20 15:04 lakehouse_engine/algorithms/__init__.py
+-rw-r--r--  2.0 unx     5527 b- defN 24-May-20 15:04 lakehouse_engine/algorithms/algorithm.py
+-rw-r--r--  2.0 unx    23776 b- defN 24-May-20 15:04 lakehouse_engine/algorithms/data_loader.py
+-rw-r--r--  2.0 unx     6163 b- defN 24-May-20 15:04 lakehouse_engine/algorithms/dq_validator.py
+-rw-r--r--  2.0 unx      539 b- defN 24-May-20 15:04 lakehouse_engine/algorithms/exceptions.py
+-rw-r--r--  2.0 unx    34132 b- defN 24-May-20 15:04 lakehouse_engine/algorithms/gab.py
+-rw-r--r--  2.0 unx    12407 b- defN 24-May-20 15:04 lakehouse_engine/algorithms/reconciliator.py
+-rw-r--r--  2.0 unx     5887 b- defN 24-May-20 15:04 lakehouse_engine/algorithms/sensor.py
+-rw-r--r--  2.0 unx       73 b- defN 24-May-20 15:04 lakehouse_engine/configs/__init__.py
+-rw-r--r--  2.0 unx       29 b- defN 24-May-20 15:04 lakehouse_engine/configs/engine.yaml
+-rw-r--r--  2.0 unx       63 b- defN 24-May-20 15:04 lakehouse_engine/core/__init__.py
+-rw-r--r--  2.0 unx     8750 b- defN 24-May-20 15:04 lakehouse_engine/core/dbfs_file_manager.py
+-rw-r--r--  2.0 unx    50454 b- defN 24-May-20 15:04 lakehouse_engine/core/definitions.py
+-rw-r--r--  2.0 unx     4088 b- defN 24-May-20 15:04 lakehouse_engine/core/exec_env.py
+-rw-r--r--  2.0 unx      445 b- defN 24-May-20 15:04 lakehouse_engine/core/executable.py
+-rw-r--r--  2.0 unx     2440 b- defN 24-May-20 15:04 lakehouse_engine/core/file_manager.py
+-rw-r--r--  2.0 unx    32419 b- defN 24-May-20 15:04 lakehouse_engine/core/gab_manager.py
+-rw-r--r--  2.0 unx    19747 b- defN 24-May-20 15:04 lakehouse_engine/core/gab_sql_generator.py
+-rw-r--r--  2.0 unx    21478 b- defN 24-May-20 15:04 lakehouse_engine/core/s3_file_manager.py
+-rw-r--r--  2.0 unx    13664 b- defN 24-May-20 15:04 lakehouse_engine/core/sensor_manager.py
+-rw-r--r--  2.0 unx    10571 b- defN 24-May-20 15:04 lakehouse_engine/core/table_manager.py
+-rw-r--r--  2.0 unx       82 b- defN 24-May-20 15:04 lakehouse_engine/dq_processors/__init__.py
+-rw-r--r--  2.0 unx     7265 b- defN 24-May-20 15:04 lakehouse_engine/dq_processors/assistant.py
+-rw-r--r--  2.0 unx    26871 b- defN 24-May-20 15:04 lakehouse_engine/dq_processors/dq_factory.py
+-rw-r--r--  2.0 unx      302 b- defN 24-May-20 15:04 lakehouse_engine/dq_processors/exceptions.py
+-rw-r--r--  2.0 unx     8904 b- defN 24-May-20 15:04 lakehouse_engine/dq_processors/validator.py
+-rw-r--r--  2.0 unx       83 b- defN 24-May-20 15:04 lakehouse_engine/dq_processors/custom_expectations/__init__.py
+-rw-r--r--  2.0 unx     7066 b- defN 24-May-20 15:04 lakehouse_engine/dq_processors/custom_expectations/expect_column_pair_a_to_be_smaller_or_equal_than_b.py
+-rw-r--r--  2.0 unx     7958 b- defN 24-May-20 15:04 lakehouse_engine/dq_processors/custom_expectations/expect_column_values_to_be_date_not_older_than.py
+-rw-r--r--  2.0 unx     6627 b- defN 24-May-20 15:04 lakehouse_engine/dq_processors/custom_expectations/expect_multicolumn_column_a_must_equal_b_or_c.py
+-rw-r--r--  2.0 unx    14618 b- defN 24-May-20 15:04 lakehouse_engine/dq_processors/custom_expectations/expect_queried_column_agg_value_to_be.py
+-rw-r--r--  2.0 unx       85 b- defN 24-May-20 15:04 lakehouse_engine/io/__init__.py
+-rw-r--r--  2.0 unx      687 b- defN 24-May-20 15:04 lakehouse_engine/io/exceptions.py
+-rw-r--r--  2.0 unx      797 b- defN 24-May-20 15:04 lakehouse_engine/io/reader.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-May-20 15:04 lakehouse_engine/io/reader_factory.py
+-rw-r--r--  2.0 unx     4720 b- defN 24-May-20 15:04 lakehouse_engine/io/writer.py
+-rw-r--r--  2.0 unx     2885 b- defN 24-May-20 15:04 lakehouse_engine/io/writer_factory.py
+-rw-r--r--  2.0 unx       51 b- defN 24-May-20 15:04 lakehouse_engine/io/readers/__init__.py
+-rw-r--r--  2.0 unx      718 b- defN 24-May-20 15:04 lakehouse_engine/io/readers/dataframe_reader.py
+-rw-r--r--  2.0 unx     2334 b- defN 24-May-20 15:04 lakehouse_engine/io/readers/file_reader.py
+-rw-r--r--  2.0 unx     2448 b- defN 24-May-20 15:04 lakehouse_engine/io/readers/jdbc_reader.py
+-rw-r--r--  2.0 unx      862 b- defN 24-May-20 15:04 lakehouse_engine/io/readers/kafka_reader.py
+-rw-r--r--  2.0 unx      734 b- defN 24-May-20 15:04 lakehouse_engine/io/readers/query_reader.py
+-rw-r--r--  2.0 unx     7205 b- defN 24-May-20 15:04 lakehouse_engine/io/readers/sap_b4_reader.py
+-rw-r--r--  2.0 unx     7299 b- defN 24-May-20 15:04 lakehouse_engine/io/readers/sap_bw_reader.py
+-rw-r--r--  2.0 unx     5445 b- defN 24-May-20 15:04 lakehouse_engine/io/readers/sftp_reader.py
+-rw-r--r--  2.0 unx     1300 b- defN 24-May-20 15:04 lakehouse_engine/io/readers/table_reader.py
+-rw-r--r--  2.0 unx       67 b- defN 24-May-20 15:04 lakehouse_engine/io/writers/__init__.py
+-rw-r--r--  2.0 unx     4361 b- defN 24-May-20 15:04 lakehouse_engine/io/writers/console_writer.py
+-rw-r--r--  2.0 unx     7516 b- defN 24-May-20 15:04 lakehouse_engine/io/writers/dataframe_writer.py
+-rw-r--r--  2.0 unx     7752 b- defN 24-May-20 15:04 lakehouse_engine/io/writers/delta_merge_writer.py
+-rw-r--r--  2.0 unx     3888 b- defN 24-May-20 15:04 lakehouse_engine/io/writers/file_writer.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-May-20 15:04 lakehouse_engine/io/writers/jdbc_writer.py
+-rw-r--r--  2.0 unx     3679 b- defN 24-May-20 15:04 lakehouse_engine/io/writers/kafka_writer.py
+-rw-r--r--  2.0 unx     5820 b- defN 24-May-20 15:04 lakehouse_engine/io/writers/table_writer.py
+-rw-r--r--  2.0 unx       87 b- defN 24-May-20 15:04 lakehouse_engine/terminators/__init__.py
+-rw-r--r--  2.0 unx     4557 b- defN 24-May-20 15:04 lakehouse_engine/terminators/cdf_processor.py
+-rw-r--r--  2.0 unx     5332 b- defN 24-May-20 15:04 lakehouse_engine/terminators/dataset_optimizer.py
+-rw-r--r--  2.0 unx     3873 b- defN 24-May-20 15:04 lakehouse_engine/terminators/notifier.py
+-rw-r--r--  2.0 unx     2934 b- defN 24-May-20 15:04 lakehouse_engine/terminators/notifier_factory.py
+-rw-r--r--  2.0 unx     2126 b- defN 24-May-20 15:04 lakehouse_engine/terminators/sensor_terminator.py
+-rw-r--r--  2.0 unx      456 b- defN 24-May-20 15:04 lakehouse_engine/terminators/spark_terminator.py
+-rw-r--r--  2.0 unx     1990 b- defN 24-May-20 15:04 lakehouse_engine/terminators/terminator_factory.py
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 15:04 lakehouse_engine/terminators/notifiers/__init__.py
+-rw-r--r--  2.0 unx     6683 b- defN 24-May-20 15:04 lakehouse_engine/terminators/notifiers/email_notifier.py
+-rw-r--r--  2.0 unx     1494 b- defN 24-May-20 15:04 lakehouse_engine/terminators/notifiers/notification_templates.py
+-rw-r--r--  2.0 unx       72 b- defN 24-May-20 15:04 lakehouse_engine/transformers/__init__.py
+-rw-r--r--  2.0 unx      895 b- defN 24-May-20 15:04 lakehouse_engine/transformers/aggregators.py
+-rw-r--r--  2.0 unx     3325 b- defN 24-May-20 15:04 lakehouse_engine/transformers/column_creators.py
+-rw-r--r--  2.0 unx    15361 b- defN 24-May-20 15:04 lakehouse_engine/transformers/column_reshapers.py
+-rw-r--r--  2.0 unx     4866 b- defN 24-May-20 15:04 lakehouse_engine/transformers/condensers.py
+-rw-r--r--  2.0 unx     1260 b- defN 24-May-20 15:04 lakehouse_engine/transformers/custom_transformers.py
+-rw-r--r--  2.0 unx     2168 b- defN 24-May-20 15:04 lakehouse_engine/transformers/data_maskers.py
+-rw-r--r--  2.0 unx     5331 b- defN 24-May-20 15:04 lakehouse_engine/transformers/date_transformers.py
+-rw-r--r--  2.0 unx      341 b- defN 24-May-20 15:04 lakehouse_engine/transformers/exceptions.py
+-rw-r--r--  2.0 unx     6359 b- defN 24-May-20 15:04 lakehouse_engine/transformers/filters.py
+-rw-r--r--  2.0 unx     3624 b- defN 24-May-20 15:04 lakehouse_engine/transformers/joiners.py
+-rw-r--r--  2.0 unx     1555 b- defN 24-May-20 15:04 lakehouse_engine/transformers/null_handlers.py
+-rw-r--r--  2.0 unx     1926 b- defN 24-May-20 15:04 lakehouse_engine/transformers/optimizers.py
+-rw-r--r--  2.0 unx     1240 b- defN 24-May-20 15:04 lakehouse_engine/transformers/regex_transformers.py
+-rw-r--r--  2.0 unx     1817 b- defN 24-May-20 15:04 lakehouse_engine/transformers/repartitioners.py
+-rw-r--r--  2.0 unx     5889 b- defN 24-May-20 15:04 lakehouse_engine/transformers/transformer_factory.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-May-20 15:04 lakehouse_engine/transformers/unions.py
+-rw-r--r--  2.0 unx      918 b- defN 24-May-20 15:04 lakehouse_engine/transformers/watermarker.py
+-rw-r--r--  2.0 unx       25 b- defN 24-May-20 15:04 lakehouse_engine/utils/__init__.py
+-rw-r--r--  2.0 unx     1636 b- defN 24-May-20 15:04 lakehouse_engine/utils/databricks_utils.py
+-rw-r--r--  2.0 unx     5632 b- defN 24-May-20 15:04 lakehouse_engine/utils/engine_usage_stats.py
+-rw-r--r--  2.0 unx     4691 b- defN 24-May-20 15:04 lakehouse_engine/utils/expectations_utils.py
+-rw-r--r--  2.0 unx     1079 b- defN 24-May-20 15:04 lakehouse_engine/utils/file_utils.py
+-rw-r--r--  2.0 unx    22848 b- defN 24-May-20 15:04 lakehouse_engine/utils/gab_utils.py
+-rw-r--r--  2.0 unx     2864 b- defN 24-May-20 15:04 lakehouse_engine/utils/logging_handler.py
+-rw-r--r--  2.0 unx     6935 b- defN 24-May-20 15:04 lakehouse_engine/utils/schema_utils.py
+-rw-r--r--  2.0 unx     7327 b- defN 24-May-20 15:04 lakehouse_engine/utils/sql_parser_utils.py
+-rw-r--r--  2.0 unx       32 b- defN 24-May-20 15:04 lakehouse_engine/utils/configs/__init__.py
+-rw-r--r--  2.0 unx     3866 b- defN 24-May-20 15:04 lakehouse_engine/utils/configs/config_utils.py
+-rw-r--r--  2.0 unx       36 b- defN 24-May-20 15:04 lakehouse_engine/utils/extraction/__init__.py
+-rw-r--r--  2.0 unx    15419 b- defN 24-May-20 15:04 lakehouse_engine/utils/extraction/jdbc_extraction_utils.py
+-rw-r--r--  2.0 unx    11821 b- defN 24-May-20 15:04 lakehouse_engine/utils/extraction/sap_b4_extraction_utils.py
+-rw-r--r--  2.0 unx    14221 b- defN 24-May-20 15:04 lakehouse_engine/utils/extraction/sap_bw_extraction_utils.py
+-rw-r--r--  2.0 unx    18533 b- defN 24-May-20 15:04 lakehouse_engine/utils/extraction/sftp_extraction_utils.py
+-rw-r--r--  2.0 unx       50 b- defN 24-May-20 15:04 lakehouse_engine/utils/storage/__init__.py
+-rw-r--r--  2.0 unx     1525 b- defN 24-May-20 15:04 lakehouse_engine/utils/storage/dbfs_storage.py
+-rw-r--r--  2.0 unx      774 b- defN 24-May-20 15:04 lakehouse_engine/utils/storage/file_storage.py
+-rw-r--r--  2.0 unx     4212 b- defN 24-May-20 15:04 lakehouse_engine/utils/storage/file_storage_functions.py
+-rw-r--r--  2.0 unx     1280 b- defN 24-May-20 15:04 lakehouse_engine/utils/storage/local_fs_storage.py
+-rw-r--r--  2.0 unx     1422 b- defN 24-May-20 15:04 lakehouse_engine/utils/storage/s3_storage.py
+-rw-r--r--  2.0 unx    12351 b- defN 24-May-20 15:04 lakehouse_engine-1.20.0.data/data/requirements/requirements_os.lock
+-rw-r--r--  2.0 unx      356 b- defN 24-May-20 15:04 lakehouse_engine_usage/__init__.py
+-rw-r--r--  2.0 unx       35 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/__init__.py
+-rw-r--r--  2.0 unx       65 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/append_load_from_jdbc_with_permissive_mode/__init__.py
+-rw-r--r--  2.0 unx       48 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/append_load_with_failfast/__init__.py
+-rw-r--r--  2.0 unx       70 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/batch_delta_load_init_delta_backfill_with_merge/__init__.py
+-rw-r--r--  2.0 unx       42 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/custom_transformer/__init__.py
+-rw-r--r--  2.0 unx       48 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/extract_from_sap_b4_adso/__init__.py
+-rw-r--r--  2.0 unx       46 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/extract_from_sap_bw_dso/__init__.py
+-rw-r--r--  2.0 unx       41 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/extract_from_sftp/__init__.py
+-rw-r--r--  2.0 unx       53 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/extract_using_jdbc_connection/__init__.py
+-rw-r--r--  2.0 unx       42 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/filtered_full_load/__init__.py
+-rw-r--r--  2.0 unx       64 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/filtered_full_load_with_selective_replace/__init__.py
+-rw-r--r--  2.0 unx       58 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/flatten_schema_and_explode_columns/__init__.py
+-rw-r--r--  2.0 unx       33 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/full_load/__init__.py
+-rw-r--r--  2.0 unx       43 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/read_from_dataframe/__init__.py
+-rw-r--r--  2.0 unx       60 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/streaming_append_load_with_malformed/__init__.py
+-rw-r--r--  2.0 unx       61 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/streaming_append_load_with_terminator/__init__.py
+-rw-r--r--  2.0 unx       77 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/streaming_delta_load_with_group_and_rank_condensation/__init__.py
+-rw-r--r--  2.0 unx       82 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/streaming_delta_with_late_arriving_and_out_of_order_events/__init__.py
+-rw-r--r--  2.0 unx       48 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/write_and_read_dataframe/__init__.py
+-rw-r--r--  2.0 unx       40 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_loader/write_to_console/__init__.py
+-rw-r--r--  2.0 unx       36 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_quality/__init__.py
+-rw-r--r--  2.0 unx       43 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_quality/custom_expectations/__init__.py
+-rw-r--r--  2.0 unx       46 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_quality/data_quality_validator/__init__.py
+-rw-r--r--  2.0 unx       39 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_quality/minimal_example/__init__.py
+-rw-r--r--  2.0 unx       35 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_quality/result_sink/__init__.py
+-rw-r--r--  2.0 unx       35 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_quality/row_tagging/__init__.py
+-rw-r--r--  2.0 unx       43 b- defN 24-May-20 15:04 lakehouse_engine_usage/data_quality/validations_failing/__init__.py
+-rw-r--r--  2.0 unx       37 b- defN 24-May-20 15:04 lakehouse_engine_usage/reconciliator/__init__.py
+-rw-r--r--  2.0 unx       30 b- defN 24-May-20 15:04 lakehouse_engine_usage/sensor/__init__.py
+-rw-r--r--  2.0 unx       35 b- defN 24-May-20 15:04 lakehouse_engine_usage/sensor/delta_table/__init__.py
+-rw-r--r--  2.0 unx       51 b- defN 24-May-20 15:04 lakehouse_engine_usage/sensor/delta_upstream_sensor_table/__init__.py
+-rw-r--r--  2.0 unx       28 b- defN 24-May-20 15:04 lakehouse_engine_usage/sensor/file/__init__.py
+-rw-r--r--  2.0 unx       34 b- defN 24-May-20 15:04 lakehouse_engine_usage/sensor/jdbc_table/__init__.py
+-rw-r--r--  2.0 unx       29 b- defN 24-May-20 15:04 lakehouse_engine_usage/sensor/kafka/__init__.py
+-rw-r--r--  2.0 unx       33 b- defN 24-May-20 15:04 lakehouse_engine_usage/sensor/sap_bw_b4/__init__.py
+-rw-r--r--  2.0 unx       44 b- defN 24-May-20 15:04 lakehouse_engine_usage/sensor/update_sensor_status/__init__.py
+-rw-r--r--  2.0 unx       21 b- defN 24-May-20 15:04 tests/__init__.py
+-rw-r--r--  2.0 unx     1968 b- defN 24-May-20 15:04 tests/conftest.py
+-rw-r--r--  2.0 unx       54 b- defN 24-May-20 15:04 tests/configs/__init__.py
+-rw-r--r--  2.0 unx       89 b- defN 24-May-20 15:04 tests/feature/__init__.py
+-rw-r--r--  2.0 unx     6329 b- defN 24-May-20 15:04 tests/feature/test_append_load.py
+-rw-r--r--  2.0 unx    26259 b- defN 24-May-20 15:04 tests/feature/test_data_quality.py
+-rw-r--r--  2.0 unx    17643 b- defN 24-May-20 15:04 tests/feature/test_dq_validator.py
+-rw-r--r--  2.0 unx     7943 b- defN 24-May-20 15:04 tests/feature/test_engine_usage_stats.py
+-rw-r--r--  2.0 unx    17735 b- defN 24-May-20 15:04 tests/feature/test_extract_from_sap_b4.py
+-rw-r--r--  2.0 unx    23508 b- defN 24-May-20 15:04 tests/feature/test_extract_from_sap_bw.py
+-rw-r--r--  2.0 unx    10590 b- defN 24-May-20 15:04 tests/feature/test_file_manager.py
+-rw-r--r--  2.0 unx     9124 b- defN 24-May-20 15:04 tests/feature/test_file_manager_dbfs.py
+-rw-r--r--  2.0 unx    11234 b- defN 24-May-20 15:04 tests/feature/test_file_manager_s3.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-20 15:04 tests/feature/test_full_load.py
+-rw-r--r--  2.0 unx    13799 b- defN 24-May-20 15:04 tests/feature/test_gab.py
+-rw-r--r--  2.0 unx     4573 b- defN 24-May-20 15:04 tests/feature/test_jdbc_reader.py
+-rw-r--r--  2.0 unx     4116 b- defN 24-May-20 15:04 tests/feature/test_materialize_cdf.py
+-rw-r--r--  2.0 unx    16028 b- defN 24-May-20 15:04 tests/feature/test_notification.py
+-rw-r--r--  2.0 unx    14219 b- defN 24-May-20 15:04 tests/feature/test_reconciliation.py
+-rw-r--r--  2.0 unx    20111 b- defN 24-May-20 15:04 tests/feature/test_schema_evolution.py
+-rw-r--r--  2.0 unx    16396 b- defN 24-May-20 15:04 tests/feature/test_sensors.py
+-rw-r--r--  2.0 unx    19193 b- defN 24-May-20 15:04 tests/feature/test_sftp_reader.py
+-rw-r--r--  2.0 unx     9422 b- defN 24-May-20 15:04 tests/feature/test_table_manager.py
+-rw-r--r--  2.0 unx    14023 b- defN 24-May-20 15:04 tests/feature/test_writers.py
+-rw-r--r--  2.0 unx       64 b- defN 24-May-20 15:04 tests/feature/custom_expectations/__init__.py
+-rw-r--r--  2.0 unx     9212 b- defN 24-May-20 15:04 tests/feature/custom_expectations/test_custom_expectations.py
+-rw-r--r--  2.0 unx     3850 b- defN 24-May-20 15:04 tests/feature/custom_expectations/test_expectation_validity.py
+-rw-r--r--  2.0 unx       89 b- defN 24-May-20 15:04 tests/feature/data_loader_custom_transformer/__init__.py
+-rw-r--r--  2.0 unx     4060 b- defN 24-May-20 15:04 tests/feature/data_loader_custom_transformer/test_data_loader_custom_transformer_calculate_kpi.py
+-rw-r--r--  2.0 unx     7613 b- defN 24-May-20 15:04 tests/feature/data_loader_custom_transformer/test_data_loader_custom_transformer_delta_load.py
+-rw-r--r--  2.0 unx       32 b- defN 24-May-20 15:04 tests/feature/delta_load/__init__.py
+-rw-r--r--  2.0 unx     5343 b- defN 24-May-20 15:04 tests/feature/delta_load/test_delta_load_group_and_rank.py
+-rw-r--r--  2.0 unx     3481 b- defN 24-May-20 15:04 tests/feature/delta_load/test_delta_load_merge_options.py
+-rw-r--r--  2.0 unx     9547 b- defN 24-May-20 15:04 tests/feature/delta_load/test_delta_load_record_mode_cdc.py
+-rw-r--r--  2.0 unx       37 b- defN 24-May-20 15:04 tests/feature/transformations/__init__.py
+-rw-r--r--  2.0 unx     4310 b- defN 24-May-20 15:04 tests/feature/transformations/test_chain_transformations.py
+-rw-r--r--  2.0 unx     1947 b- defN 24-May-20 15:04 tests/feature/transformations/test_column_creators.py
+-rw-r--r--  2.0 unx     2625 b- defN 24-May-20 15:04 tests/feature/transformations/test_column_reshapers.py
+-rw-r--r--  2.0 unx     1999 b- defN 24-May-20 15:04 tests/feature/transformations/test_data_maskers.py
+-rw-r--r--  2.0 unx     1816 b- defN 24-May-20 15:04 tests/feature/transformations/test_date_transformers.py
+-rw-r--r--  2.0 unx     3319 b- defN 24-May-20 15:04 tests/feature/transformations/test_drop_duplicate_rows.py
+-rw-r--r--  2.0 unx     3029 b- defN 24-May-20 15:04 tests/feature/transformations/test_joiners.py
+-rw-r--r--  2.0 unx     2298 b- defN 24-May-20 15:04 tests/feature/transformations/test_multiple_transformations.py
+-rw-r--r--  2.0 unx     1863 b- defN 24-May-20 15:04 tests/feature/transformations/test_null_handlers.py
+-rw-r--r--  2.0 unx     3489 b- defN 24-May-20 15:04 tests/feature/transformations/test_optimizers.py
+-rw-r--r--  2.0 unx     1996 b- defN 24-May-20 15:04 tests/feature/transformations/test_regex_transformers.py
+-rw-r--r--  2.0 unx     4981 b- defN 24-May-20 15:04 tests/feature/transformations/test_unions.py
+-rw-r--r--  2.0 unx     6275 b- defN 24-May-20 15:04 tests/feature/transformations/test_watermarker.py
+-rw-r--r--  2.0 unx       23 b- defN 24-May-20 15:04 tests/utils/__init__.py
+-rw-r--r--  2.0 unx     6959 b- defN 24-May-20 15:04 tests/utils/dataframe_helpers.py
+-rw-r--r--  2.0 unx     1960 b- defN 24-May-20 15:04 tests/utils/exec_env_helpers.py
+-rw-r--r--  2.0 unx     1513 b- defN 24-May-20 15:04 tests/utils/local_storage.py
+-rw-r--r--  2.0 unx    11339 b- defN 24-May-20 15:05 lakehouse_engine-1.20.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    24847 b- defN 24-May-20 15:05 lakehouse_engine-1.20.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-20 15:05 lakehouse_engine-1.20.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       46 b- defN 24-May-20 15:05 lakehouse_engine-1.20.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    21245 b- defN 24-May-20 15:05 lakehouse_engine-1.20.0.dist-info/RECORD
+203 files, 1070893 bytes uncompressed, 259769 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -15,14 +15,17 @@
 
 Filename: lakehouse_engine/algorithms/dq_validator.py
 Comment: 
 
 Filename: lakehouse_engine/algorithms/exceptions.py
 Comment: 
 
+Filename: lakehouse_engine/algorithms/gab.py
+Comment: 
+
 Filename: lakehouse_engine/algorithms/reconciliator.py
 Comment: 
 
 Filename: lakehouse_engine/algorithms/sensor.py
 Comment: 
 
 Filename: lakehouse_engine/configs/__init__.py
@@ -45,14 +48,20 @@
 
 Filename: lakehouse_engine/core/executable.py
 Comment: 
 
 Filename: lakehouse_engine/core/file_manager.py
 Comment: 
 
+Filename: lakehouse_engine/core/gab_manager.py
+Comment: 
+
+Filename: lakehouse_engine/core/gab_sql_generator.py
+Comment: 
+
 Filename: lakehouse_engine/core/s3_file_manager.py
 Comment: 
 
 Filename: lakehouse_engine/core/sensor_manager.py
 Comment: 
 
 Filename: lakehouse_engine/core/table_manager.py
@@ -258,14 +267,17 @@
 
 Filename: lakehouse_engine/utils/expectations_utils.py
 Comment: 
 
 Filename: lakehouse_engine/utils/file_utils.py
 Comment: 
 
+Filename: lakehouse_engine/utils/gab_utils.py
+Comment: 
+
 Filename: lakehouse_engine/utils/logging_handler.py
 Comment: 
 
 Filename: lakehouse_engine/utils/schema_utils.py
 Comment: 
 
 Filename: lakehouse_engine/utils/sql_parser_utils.py
@@ -306,15 +318,15 @@
 
 Filename: lakehouse_engine/utils/storage/local_fs_storage.py
 Comment: 
 
 Filename: lakehouse_engine/utils/storage/s3_storage.py
 Comment: 
 
-Filename: lakehouse_engine-1.19.0.data/data/requirements/requirements_os.lock
+Filename: lakehouse_engine-1.20.0.data/data/requirements/requirements_os.lock
 Comment: 
 
 Filename: lakehouse_engine_usage/__init__.py
 Comment: 
 
 Filename: lakehouse_engine_usage/data_loader/__init__.py
 Comment: 
@@ -462,14 +474,17 @@
 
 Filename: tests/feature/test_file_manager_s3.py
 Comment: 
 
 Filename: tests/feature/test_full_load.py
 Comment: 
 
+Filename: tests/feature/test_gab.py
+Comment: 
+
 Filename: tests/feature/test_jdbc_reader.py
 Comment: 
 
 Filename: tests/feature/test_materialize_cdf.py
 Comment: 
 
 Filename: tests/feature/test_notification.py
@@ -573,23 +588,23 @@
 
 Filename: tests/utils/exec_env_helpers.py
 Comment: 
 
 Filename: tests/utils/local_storage.py
 Comment: 
 
-Filename: lakehouse_engine-1.19.0.dist-info/LICENSE.txt
+Filename: lakehouse_engine-1.20.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: lakehouse_engine-1.19.0.dist-info/METADATA
+Filename: lakehouse_engine-1.20.0.dist-info/METADATA
 Comment: 
 
-Filename: lakehouse_engine-1.19.0.dist-info/WHEEL
+Filename: lakehouse_engine-1.20.0.dist-info/WHEEL
 Comment: 
 
-Filename: lakehouse_engine-1.19.0.dist-info/top_level.txt
+Filename: lakehouse_engine-1.20.0.dist-info/top_level.txt
 Comment: 
 
-Filename: lakehouse_engine-1.19.0.dist-info/RECORD
+Filename: lakehouse_engine-1.20.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lakehouse_engine/engine.py

```diff
@@ -1,166 +1,167 @@
 """Contract of the lakehouse engine with all the available functions to be executed."""
 from typing import List, Optional, OrderedDict
 
 from lakehouse_engine.algorithms.data_loader import DataLoader
 from lakehouse_engine.algorithms.dq_validator import DQValidator
+from lakehouse_engine.algorithms.gab import GAB
 from lakehouse_engine.algorithms.reconciliator import Reconciliator
 from lakehouse_engine.algorithms.sensor import Sensor, SensorStatus
-from lakehouse_engine.core.definitions import SAPLogchain, TerminatorSpec
+from lakehouse_engine.core.definitions import (
+    CollectEngineUsage,
+    DQDefaults,
+    SAPLogchain,
+    TerminatorSpec,
+)
 from lakehouse_engine.core.exec_env import ExecEnv
 from lakehouse_engine.core.file_manager import FileManagerFactory
 from lakehouse_engine.core.sensor_manager import SensorUpstreamManager
 from lakehouse_engine.core.table_manager import TableManager
+from lakehouse_engine.dq_processors.dq_factory import DQFactory
 from lakehouse_engine.terminators.notifier_factory import NotifierFactory
 from lakehouse_engine.terminators.sensor_terminator import SensorTerminator
 from lakehouse_engine.utils.configs.config_utils import ConfigUtils
 from lakehouse_engine.utils.engine_usage_stats import EngineUsageStats
 
 
 def load_data(
     acon_path: Optional[str] = None,
     acon: Optional[dict] = None,
-    collect_engine_usage: bool = None,
+    collect_engine_usage: str = CollectEngineUsage.PROD_ONLY.value,
     spark_confs: dict = None,
 ) -> Optional[OrderedDict]:
     """Load data using the DataLoader algorithm.
 
     Args:
         acon_path: path of the acon (algorithm configuration) file.
         acon: acon provided directly through python code (e.g., notebooks or other
             apps).
-        collect_engine_usage: a boolean that enables or disables the collection and
-                storage of Lakehouse usage statistics.
+        collect_engine_usage: Lakehouse usage statistics collection strategy.
         spark_confs: optional dictionary with the spark confs to be used when collecting
             the engine usage.
     """
     acon = ConfigUtils.get_acon(acon_path, acon)
     ExecEnv.get_or_create(app_name="data_loader", config=acon.get("exec_env", None))
     EngineUsageStats.store_engine_usage(
         acon, load_data.__name__, collect_engine_usage, spark_confs
     )
     return DataLoader(acon).execute()
 
 
 def execute_reconciliation(
     acon_path: Optional[str] = None,
     acon: Optional[dict] = None,
-    collect_engine_usage: bool = None,
+    collect_engine_usage: str = CollectEngineUsage.PROD_ONLY.value,
     spark_confs: dict = None,
 ) -> None:
     """Execute the Reconciliator algorithm.
 
     Args:
         acon_path: path of the acon (algorithm configuration) file.
         acon: acon provided directly through python code (e.g., notebooks or other
             apps).
-        collect_engine_usage: whether we want to enable the collection and storage of
-            lakehouse engine usage stats or not.
+        collect_engine_usage: Lakehouse usage statistics collection strategy.
         spark_confs: optional dictionary with the spark confs to be used when collecting
             the engine usage.
     """
     acon = ConfigUtils.get_acon(acon_path, acon)
     ExecEnv.get_or_create(app_name="reconciliator", config=acon.get("exec_env", None))
     EngineUsageStats.store_engine_usage(
         acon, execute_reconciliation.__name__, collect_engine_usage, spark_confs
     )
     Reconciliator(acon).execute()
 
 
 def execute_dq_validation(
     acon_path: Optional[str] = None,
     acon: Optional[dict] = None,
-    collect_engine_usage: bool = None,
+    collect_engine_usage: str = CollectEngineUsage.PROD_ONLY.value,
     spark_confs: dict = None,
 ) -> None:
     """Execute the DQValidator algorithm.
 
     Args:
         acon_path: path of the acon (algorithm configuration) file.
         acon: acon provided directly through python code (e.g., notebooks or other
             apps).
-        collect_engine_usage: whether we want to enable the collection and storage of
-            lakehouse engine usage stats or not.
+        collect_engine_usage: Lakehouse usage statistics collection strategy.
         spark_confs: optional dictionary with the spark confs to be used when collecting
             the engine usage.
     """
     acon = ConfigUtils.get_acon(acon_path, acon)
     ExecEnv.get_or_create(app_name="dq_validator", config=acon.get("exec_env", None))
     EngineUsageStats.store_engine_usage(
         acon, execute_dq_validation.__name__, collect_engine_usage, spark_confs
     )
     DQValidator(acon).execute()
 
 
 def manage_table(
     acon_path: Optional[str] = None,
     acon: Optional[dict] = None,
-    collect_engine_usage: bool = None,
+    collect_engine_usage: str = CollectEngineUsage.PROD_ONLY.value,
     spark_confs: dict = None,
 ) -> None:
     """Manipulate tables/views using Table Manager algorithm.
 
     Args:
         acon_path: path of the acon (algorithm configuration) file.
         acon: acon provided directly through python code (e.g., notebooks
             or other apps).
-        collect_engine_usage: whether we want to enable the collection and storage of
-            lakehouse engine usage stats or not.
+        collect_engine_usage: Lakehouse usage statistics collection strategy.
         spark_confs: optional dictionary with the spark confs to be used when collecting
             the engine usage.
     """
     acon = ConfigUtils.get_acon(acon_path, acon)
     ExecEnv.get_or_create(app_name="manage_table", config=acon.get("exec_env", None))
     EngineUsageStats.store_engine_usage(
         acon, manage_table.__name__, collect_engine_usage, spark_confs
     )
     TableManager(acon).get_function()
 
 
 def manage_files(
     acon_path: Optional[str] = None,
     acon: Optional[dict] = None,
-    collect_engine_usage: bool = None,
+    collect_engine_usage: str = CollectEngineUsage.PROD_ONLY.value,
     spark_confs: dict = None,
 ) -> None:
     """Manipulate s3 files using File Manager algorithm.
 
     Args:
         acon_path: path of the acon (algorithm configuration) file.
         acon: acon provided directly through python code (e.g., notebooks
             or other apps).
-        collect_engine_usage: whether we want to enable the collection and storage of
-            lakehouse engine usage stats or not.
+        collect_engine_usage: Lakehouse usage statistics collection strategy.
         spark_confs: optional dictionary with the spark confs to be used when collecting
             the engine usage.
     """
     acon = ConfigUtils.get_acon(acon_path, acon)
     ExecEnv.get_or_create(app_name="manage_files", config=acon.get("exec_env", None))
     EngineUsageStats.store_engine_usage(
         acon, manage_files.__name__, collect_engine_usage, spark_confs
     )
     FileManagerFactory.execute_function(configs=acon)
 
 
 def execute_sensor(
     acon_path: Optional[str] = None,
     acon: Optional[dict] = None,
-    collect_engine_usage: bool = None,
+    collect_engine_usage: str = CollectEngineUsage.PROD_ONLY.value,
     spark_confs: dict = None,
 ) -> bool:
     """Execute a sensor based on a Sensor Algorithm Configuration.
 
     A sensor is useful to check if an upstream system has new data.
 
     Args:
         acon_path: path of the acon (algorithm configuration) file.
         acon: acon provided directly through python code (e.g., notebooks
             or other apps).
-        collect_engine_usage: whether we want to enable the collection and storage of
-            lakehouse engine usage stats or not.
+        collect_engine_usage: Lakehouse usage statistics collection strategy.
         spark_confs: optional dictionary with the spark confs to be used when collecting
             the engine usage.
     """
     acon = ConfigUtils.get_acon(acon_path, acon)
     ExecEnv.get_or_create(app_name="execute_sensor", config=acon.get("exec_env", None))
     EngineUsageStats.store_engine_usage(
         acon, execute_sensor.__name__, collect_engine_usage, spark_confs
@@ -288,7 +289,83 @@
     """
     notifier = NotifierFactory.get_notifier(
         spec=TerminatorSpec(function="notify", args=args)
     )
 
     notifier.create_notification()
     notifier.send_notification()
+
+
+def build_data_docs(
+    store_backend: str = DQDefaults.STORE_BACKEND.value,
+    local_fs_root_dir: str = None,
+    data_docs_local_fs: str = None,
+    data_docs_prefix: str = DQDefaults.DATA_DOCS_PREFIX.value,
+    bucket: str = None,
+    data_docs_bucket: str = None,
+    expectations_store_prefix: str = DQDefaults.EXPECTATIONS_STORE_PREFIX.value,
+    validations_store_prefix: str = DQDefaults.VALIDATIONS_STORE_PREFIX.value,
+    checkpoint_store_prefix: str = DQDefaults.CHECKPOINT_STORE_PREFIX.value,
+) -> None:
+    """Build Data Docs for the project.
+
+    This function does a full build of data docs based on all the great expectations
+    checkpoints in the specified location, getting all history of run/validations
+    executed and results.
+
+    Args:
+        store_backend: which store_backend to use (e.g. s3 or file_system).
+        local_fs_root_dir: path of the root directory. Note: only applicable
+            for store_backend file_system
+        data_docs_local_fs: path of the root directory. Note: only applicable
+            for store_backend file_system.
+        data_docs_prefix: prefix where to store data_docs' data.
+        bucket: the bucket name to consider for the store_backend
+            (store DQ artefacts). Note: only applicable for store_backend s3.
+        data_docs_bucket: the bucket name for data docs only. When defined,
+            it will supersede bucket parameter.
+            Note: only applicable for store_backend s3.
+        expectations_store_prefix: prefix where to store expectations' data.
+            Note: only applicable for store_backend s3.
+        validations_store_prefix: prefix where to store validations' data.
+            Note: only applicable for store_backend s3.
+        checkpoint_store_prefix: prefix where to store checkpoints' data.
+            Note: only applicable for store_backend s3.
+    """
+    DQFactory.build_data_docs(
+        store_backend=store_backend,
+        local_fs_root_dir=local_fs_root_dir,
+        data_docs_local_fs=data_docs_local_fs,
+        data_docs_prefix=data_docs_prefix,
+        bucket=bucket,
+        data_docs_bucket=data_docs_bucket,
+        expectations_store_prefix=expectations_store_prefix,
+        validations_store_prefix=validations_store_prefix,
+        checkpoint_store_prefix=checkpoint_store_prefix,
+    )
+
+
+def execute_gab(
+    acon_path: Optional[str] = None,
+    acon: Optional[dict] = None,
+    collect_engine_usage: str = CollectEngineUsage.PROD_ONLY.value,
+    spark_confs: dict = None,
+) -> None:
+    """Execute the gold asset builder based on a GAB Algorithm Configuration.
+
+    GaB is useful to build your gold assets with predefined functions for recurrent
+    periods.
+
+    Args:
+        acon_path: path of the acon (algorithm configuration) file.
+        acon: acon provided directly through python code (e.g., notebooks
+            or other apps).
+        collect_engine_usage: Lakehouse usage statistics collection strategy.
+        spark_confs: optional dictionary with the spark confs to be used when collecting
+            the engine usage.
+    """
+    acon = ConfigUtils.get_acon(acon_path, acon)
+    ExecEnv.get_or_create(app_name="execute_gab", config=acon.get("exec_env", None))
+    EngineUsageStats.store_engine_usage(
+        acon, execute_gab.__name__, collect_engine_usage, spark_confs
+    )
+    GAB(acon).execute()
```

## lakehouse_engine/core/definitions.py

```diff
@@ -1,39 +1,58 @@
 """Definitions of standard values and structures for core components."""
 from dataclasses import dataclass
+from datetime import datetime
 from enum import Enum
-from typing import List, Optional
+from typing import List, Optional, Union
 
 from pyspark.sql import DataFrame
 from pyspark.sql.types import (
     ArrayType,
     BooleanType,
     StringType,
     StructField,
     StructType,
     TimestampType,
 )
 
 
+class CollectEngineUsage(Enum):
+    """Options for collecting engine usage stats.
+
+    - enabled, enables the collection and storage of Lakehouse Engine
+    usage statistics for any environment.
+    - prod_only, enables the collection and storage of Lakehouse Engine
+    usage statistics for production environment only.
+    - disabled, disables the collection and storage of Lakehouse Engine
+    usage statistics, for all environments.
+    """
+
+    ENABLED = "enabled"
+    PROD_ONLY = "prod_only"
+    DISABLED = "disabled"
+
+
 @dataclass
 class EngineConfig(object):
     """Definitions that can come from the Engine Config file.
 
     - dq_bucket: S3 bucket used to store data quality related artifacts.
     - notif_disallowed_email_servers: email servers not allowed to be used
         for sending notifications.
-    - engine_usage_path: path where the engine usage stats are stored.
+    - engine_usage_path: path where the engine prod usage stats are stored.
+    - engine_dev_usage_path: path where the engine dev usage stats are stored.
     - collect_engine_usage: whether to enable the collection of lakehouse
         engine usage stats or not.
     """
 
     dq_bucket: Optional[str] = None
     notif_disallowed_email_servers: Optional[list] = None
     engine_usage_path: Optional[str] = None
-    collect_engine_usage: bool = True
+    engine_dev_usage_path: Optional[str] = None
+    collect_engine_usage: str = CollectEngineUsage.ENABLED.value
 
 
 class EngineStats(Enum):
     """Definitions for collection of Lakehouse Engine Stats.
 
     .. note::
         Note: whenever the value comes from a key inside a Spark Config
@@ -253,14 +272,15 @@
         providing a table name in the form of `<db>.<table>`.
     - query: sql query to execute and return the dataframe. Use it if you do not want to
         read from a file system nor from a table, but rather from a sql query instead.
     - schema: dict representation of a schema of the input (e.g., Spark struct type
         schema).
     - schema_path: path to a file with a representation of a schema of the input (e.g.,
         Spark struct type schema).
+    - disable_dbfs_retry: optional flag to disable file storage dbfs.
     - with_filepath: if we want to include the path of the file that is being read. Only
         works with the file reader (batch and streaming modes are supported).
     - options: dict with other relevant options according to the execution
         environment (e.g., spark) possible sources.
     - calculate_upper_bound: when to calculate upper bound to extract from SAP BW
         or not.
     - calc_upper_bound_schema: specific schema for the calculated upper_bound.
@@ -275,14 +295,15 @@
     df_name: Optional[DataFrame] = None
     db_table: Optional[str] = None
     location: Optional[str] = None
     query: Optional[str] = None
     enforce_schema_from_table: Optional[str] = None
     schema: Optional[dict] = None
     schema_path: Optional[str] = None
+    disable_dbfs_retry: bool = False
     with_filepath: bool = False
     options: Optional[dict] = None
     jdbc_args: Optional[dict] = None
     calculate_upper_bound: bool = False
     calc_upper_bound_schema: Optional[str] = None
     generate_predicates: bool = False
     predicates_add_null: bool = True
@@ -377,21 +398,20 @@
     - local_fs_root_dir - path of the root directory. Note: only applicable for
         store_backend file_system.
     - data_docs_local_fs - the path for data docs only for store_backend
         file_system.
     - bucket - the bucket name to consider for the store_backend (store DQ artefacts).
         Note: only applicable for store_backend s3.
     - data_docs_bucket - the bucket name for data docs only. When defined, it will
-        supersede bucket parameter.
+        supersede bucket parameter. Note: only applicable for store_backend s3.
     - expectations_store_prefix - prefix where to store expectations' data. Note: only
         applicable for store_backend s3.
     - validations_store_prefix - prefix where to store validations' data. Note: only
         applicable for store_backend s3.
-    - data_docs_prefix - prefix where to store data_docs' data. Note: only applicable
-        for store_backend s3.
+    - data_docs_prefix - prefix where to store data_docs' data.
     - checkpoint_store_prefix - prefix where to store checkpoints' data. Note: only
         applicable for store_backend s3.
     - data_asset_name - name of the data asset to consider when configuring the great
         expectations' data source.
     - expectation_suite_name - name to consider for great expectations' suite.
     - assistant_options - additional options to pass to the DQ assistant processor.
     - result_sink_db_table - db.table_name indicating the database and table in which
@@ -809,7 +829,524 @@
     PARAGRAPH = "\n"
     STAR = "*"
 
     MULTIPLE_LINE_COMMENT = [
         OPENING_MULTIPLE_LINE_COMMENT,
         CLOSING_MULTIPLE_LINE_COMMENT,
     ]
+
+
+class GABDefaults(Enum):
+    """Defaults used on the GAB process."""
+
+    DATE_FORMAT = "%Y-%m-%d"
+    DIMENSIONS_DEFAULT_COLUMNS = ["from_date", "to_date"]
+    DEFAULT_DIMENSION_CALENDAR_TABLE = "dim_calendar"
+    DEFAULT_LOOKUP_QUERY_BUILDER_TABLE = "lkp_query_builder"
+
+
+class GABStartOfWeek(Enum):
+    """Representation of start of week values on GAB."""
+
+    SUNDAY = "S"
+    MONDAY = "M"
+
+    @classmethod
+    def get_start_of_week(cls) -> dict:
+        """Get the start of week enum as a dict.
+
+        Returns:
+            dict containing all enum entries as `{name:value}`.
+        """
+        return {
+            start_of_week.name: start_of_week.value
+            for start_of_week in list(GABStartOfWeek)
+        }
+
+    @classmethod
+    def get_values(cls) -> set[str]:
+        """Get the start of week enum values as set.
+
+        Returns:
+            set containing all possible values `{value}`.
+        """
+        return {start_of_week.value for start_of_week in list(GABStartOfWeek)}
+
+
+@dataclass
+class GABSpec(object):
+    """Gab Specification.
+
+    query_label_filter: query use-case label to execute.
+    queue_filter: queue to execute the job.
+    cadence_filter: selected cadences to build the asset.
+    target_database: target database to write.
+    curr_date: current date.
+    start_date: period start date.
+    end_date: period end date.
+    rerun_flag: rerun flag.
+    target_table: target table to write.
+    source_database: source database.
+    gab_base_path: base path to read the use cases.
+    lookup_table: gab configuration table.
+    calendar_table: gab calendar table.
+    """
+
+    query_label_filter: list[str]
+    queue_filter: list[str]
+    cadence_filter: list[str]
+    target_database: str
+    current_date: datetime
+    start_date: datetime
+    end_date: datetime
+    rerun_flag: str
+    target_table: str
+    source_database: str
+    gab_base_path: str
+    lookup_table: str
+    calendar_table: str
+
+    @classmethod
+    def create_from_acon(cls, acon: dict):  # type: ignore
+        """Create GabSpec from acon.
+
+        Args:
+            acon: gab ACON.
+        """
+        lookup_table = f"{acon['source_database']}." + (
+            acon.get(
+                "lookup_table", GABDefaults.DEFAULT_LOOKUP_QUERY_BUILDER_TABLE.value
+            )
+        )
+
+        calendar_table = f"{acon['source_database']}." + (
+            acon.get(
+                "calendar_table", GABDefaults.DEFAULT_DIMENSION_CALENDAR_TABLE.value
+            )
+        )
+
+        def format_date(date_to_format: Union[datetime, str]) -> datetime:
+            if isinstance(date_to_format, str):
+                return datetime.strptime(date_to_format, GABDefaults.DATE_FORMAT.value)
+            else:
+                return date_to_format
+
+        return cls(
+            query_label_filter=acon["query_label_filter"],
+            queue_filter=acon["queue_filter"],
+            cadence_filter=acon["cadence_filter"],
+            target_database=acon["target_database"],
+            current_date=datetime.now(),
+            start_date=format_date(acon["start_date"]),
+            end_date=format_date(acon["end_date"]),
+            rerun_flag=acon["rerun_flag"],
+            target_table=acon["target_table"],
+            source_database=acon["source_database"],
+            gab_base_path=acon["gab_base_path"],
+            lookup_table=lookup_table,
+            calendar_table=calendar_table,
+        )
+
+
+class GABCadence(Enum):
+    """Representation of the supported cadences on GAB."""
+
+    DAY = 1
+    WEEK = 2
+    MONTH = 3
+    QUARTER = 4
+    YEAR = 5
+
+    @classmethod
+    def get_ordered_cadences(cls) -> dict:
+        """Get the cadences ordered by the value.
+
+        Returns:
+            dict containing ordered cadences as `{name:value}`.
+        """
+        cadences = list(GABCadence)
+        return {
+            cadence.name: cadence.value
+            for cadence in sorted(cadences, key=lambda gab_cadence: gab_cadence.value)
+        }
+
+    @classmethod
+    def get_cadences(cls) -> set[str]:
+        """Get the cadences values as set.
+
+        Returns:
+            set containing all possible cadence values as `{value}`.
+        """
+        return {cadence.name for cadence in list(GABCadence)}
+
+    @classmethod
+    def order_cadences(cls, cadences_to_order: list[str]) -> list[str]:
+        """Order a list of cadences by value.
+
+        Returns:
+            ordered set containing the received cadences.
+        """
+        return sorted(
+            cadences_to_order,
+            key=lambda item: cls.get_ordered_cadences().get(item),  # type: ignore
+        )
+
+
+class GABKeys:
+    """Constants used to update pre-configured gab dict key."""
+
+    JOIN_SELECT = "join_select"
+    PROJECT_START = "project_start"
+    PROJECT_END = "project_end"
+
+
+class GABReplaceableKeys:
+    """Constants used to replace pre-configured gab dict values."""
+
+    CADENCE = "${cad}"
+    DATE_COLUMN = "${date_column}"
+    CONFIG_WEEK_START = "${config_week_start}"
+    RECONCILIATION_CADENCE = "${rec_cadence}"
+
+
+class GABCombinedConfiguration(Enum):
+    """GAB combined configuration.
+
+    Based on the use case configuration return the values to override in the SQL file.
+    This enum aims to exhaustively map each combination of `cadence`, `reconciliation`,
+        `week_start` and `snap_flag` return the corresponding values `join_select`,
+        `project_start` and `project_end` to replace this values in the stages SQL file.
+
+    Return corresponding configuration (join_select, project_start, project_end) for
+        each combination (cadence x recon x week_start x snap_flag).
+    """
+
+    _PROJECT_DATE_COLUMN_TRUNCATED_BY_CADENCE = (
+        "date(date_trunc('${cad}',${date_column}))"
+    )
+    _DEFAULT_PROJECT_START = "df_cal.cadence_start_date"
+    _DEFAULT_PROJECT_END = "df_cal.cadence_end_date"
+
+    COMBINED_CONFIGURATION = {
+        # Combination of:
+        # - cadence: `DAY`
+        # - reconciliation_window: `DAY`, `WEEK`, `MONTH`, `QUARTER`, `YEAR`
+        # - week_start: `S`, `M`
+        # - snapshot_flag: `Y`, `N`
+        1: {
+            "cadence": GABCadence.DAY.name,
+            "recon": GABCadence.get_cadences(),
+            "week_start": GABStartOfWeek.get_values(),
+            "snap_flag": {"Y", "N"},
+            "join_select": "",
+            "project_start": _PROJECT_DATE_COLUMN_TRUNCATED_BY_CADENCE,
+            "project_end": _PROJECT_DATE_COLUMN_TRUNCATED_BY_CADENCE,
+        },
+        # Combination of:
+        # - cadence: `WEEK`
+        # - reconciliation_window: `DAY`
+        # - week_start: `S`, `M`
+        # - snapshot_flag: `Y`
+        2: {
+            "cadence": GABCadence.WEEK.name,
+            "recon": GABCadence.DAY.name,
+            "week_start": GABStartOfWeek.get_values(),
+            "snap_flag": "Y",
+            "join_select": """
+            select distinct case
+                when '${config_week_start}' = 'Monday' then weekstart_mon
+                when '${config_week_start}' = 'Sunday' then weekstart_sun
+            end as cadence_start_date,
+            calendar_date as cadence_end_date
+        """,
+            "project_start": _DEFAULT_PROJECT_START,
+            "project_end": _DEFAULT_PROJECT_END,
+        },
+        # Combination of:
+        # - cadence: `WEEK`
+        # - reconciliation_window: `DAY, `MONTH`, `QUARTER`, `YEAR`
+        # - week_start: `M`
+        # - snapshot_flag: `Y`, `N`
+        3: {
+            "cadence": GABCadence.WEEK.name,
+            "recon": {
+                GABCadence.DAY.name,
+                GABCadence.MONTH.name,
+                GABCadence.QUARTER.name,
+                GABCadence.YEAR.name,
+            },
+            "week_start": "M",
+            "snap_flag": {"Y", "N"},
+            "join_select": """
+            select distinct case
+                when '${config_week_start}'  = 'Monday' then weekstart_mon
+                when '${config_week_start}' = 'Sunday' then weekstart_sun
+            end as cadence_start_date,
+            case
+                when '${config_week_start}' = 'Monday' then weekend_mon
+                when '${config_week_start}' = 'Sunday' then weekend_sun
+            end as cadence_end_date""",
+            "project_start": _DEFAULT_PROJECT_START,
+            "project_end": _DEFAULT_PROJECT_END,
+        },
+        4: {
+            "cadence": GABCadence.MONTH.name,
+            "recon": GABCadence.DAY.name,
+            "week_start": GABStartOfWeek.get_values(),
+            "snap_flag": "Y",
+            "join_select": """
+            select distinct month_start as cadence_start_date,
+            calendar_date as cadence_end_date
+        """,
+            "project_start": _DEFAULT_PROJECT_START,
+            "project_end": _DEFAULT_PROJECT_END,
+        },
+        5: {
+            "cadence": GABCadence.MONTH.name,
+            "recon": GABCadence.WEEK.name,
+            "week_start": GABStartOfWeek.MONDAY.value,
+            "snap_flag": "Y",
+            "join_select": """
+            select distinct month_start as cadence_start_date,
+            case
+                when date(
+                    date_trunc('MONTH',add_months(calendar_date, 1))
+                )-1 < weekend_mon
+                    then date(date_trunc('MONTH',add_months(calendar_date, 1)))-1
+                else weekend_mon
+            end as cadence_end_date""",
+            "project_start": _DEFAULT_PROJECT_START,
+            "project_end": _DEFAULT_PROJECT_END,
+        },
+        6: {
+            "cadence": GABCadence.MONTH.name,
+            "recon": GABCadence.WEEK.name,
+            "week_start": GABStartOfWeek.SUNDAY.value,
+            "snap_flag": "Y",
+            "join_select": """
+            select distinct month_start as cadence_start_date,
+            case
+                when date(
+                    date_trunc('MONTH',add_months(calendar_date, 1))
+                )-1 < weekend_sun
+                    then date(date_trunc('MONTH',add_months(calendar_date, 1)))-1
+                else weekend_sun
+            end as cadence_end_date""",
+            "project_start": _DEFAULT_PROJECT_START,
+            "project_end": _DEFAULT_PROJECT_END,
+        },
+        7: {
+            "cadence": GABCadence.MONTH.name,
+            "recon": GABCadence.get_cadences(),
+            "week_start": GABStartOfWeek.get_values(),
+            "snap_flag": {"Y", "N"},
+            "join_select": "",
+            "project_start": _PROJECT_DATE_COLUMN_TRUNCATED_BY_CADENCE,
+            "project_end": "date(date_trunc('MONTH',add_months(${date_column}, 1)))-1",
+        },
+        8: {
+            "cadence": GABCadence.QUARTER.name,
+            "recon": GABCadence.DAY.name,
+            "week_start": GABStartOfWeek.get_values(),
+            "snap_flag": "Y",
+            "join_select": """
+            select distinct quarter_start as cadence_start_date,
+            calendar_date as cadence_end_date
+        """,
+            "project_start": _DEFAULT_PROJECT_START,
+            "project_end": _DEFAULT_PROJECT_END,
+        },
+        9: {
+            "cadence": GABCadence.QUARTER.name,
+            "recon": GABCadence.WEEK.name,
+            "week_start": GABStartOfWeek.MONDAY.value,
+            "snap_flag": "Y",
+            "join_select": """
+            select distinct quarter_start as cadence_start_date,
+            case
+                when weekend_mon > date(
+                    date_trunc('QUARTER',add_months(calendar_date, 3))
+                )-1
+                    then date(date_trunc('QUARTER',add_months(calendar_date, 3)))-1
+                else weekend_mon
+            end as cadence_end_date""",
+            "project_start": _DEFAULT_PROJECT_START,
+            "project_end": _DEFAULT_PROJECT_END,
+        },
+        10: {
+            "cadence": GABCadence.QUARTER.name,
+            "recon": GABCadence.WEEK.name,
+            "week_start": GABStartOfWeek.SUNDAY.value,
+            "snap_flag": "Y",
+            "join_select": """
+            select distinct quarter_start as cadence_start_date,
+            case
+                when weekend_sun > date(
+                    date_trunc('QUARTER',add_months(calendar_date, 3))
+                )-1
+                    then date(date_trunc('QUARTER',add_months(calendar_date, 3)))-1
+                else weekend_sun
+            end as cadence_end_date""",
+            "project_start": _DEFAULT_PROJECT_START,
+            "project_end": _DEFAULT_PROJECT_END,
+        },
+        11: {
+            "cadence": GABCadence.QUARTER.name,
+            "recon": GABCadence.MONTH.name,
+            "week_start": GABStartOfWeek.get_values(),
+            "snap_flag": "Y",
+            "join_select": """
+            select distinct quarter_start as cadence_start_date,
+            month_end as cadence_end_date
+        """,
+            "project_start": _DEFAULT_PROJECT_START,
+            "project_end": _DEFAULT_PROJECT_END,
+        },
+        12: {
+            "cadence": GABCadence.QUARTER.name,
+            "recon": GABCadence.YEAR.name,
+            "week_start": GABStartOfWeek.get_values(),
+            "snap_flag": "N",
+            "join_select": "",
+            "project_start": _PROJECT_DATE_COLUMN_TRUNCATED_BY_CADENCE,
+            "project_end": """
+            date(
+                date_trunc(
+                    '${cad}',add_months(date(date_trunc('${cad}',${date_column})), 3)
+                )
+            )-1
+        """,
+        },
+        13: {
+            "cadence": GABCadence.QUARTER.name,
+            "recon": GABCadence.get_cadences(),
+            "week_start": GABStartOfWeek.get_values(),
+            "snap_flag": "N",
+            "join_select": "",
+            "project_start": _PROJECT_DATE_COLUMN_TRUNCATED_BY_CADENCE,
+            "project_end": """
+            date(
+                date_trunc(
+                    '${cad}',add_months( date(date_trunc('${cad}',${date_column})), 3)
+                )
+            )-1
+        """,
+        },
+        14: {
+            "cadence": GABCadence.YEAR.name,
+            "recon": GABCadence.WEEK.name,
+            "week_start": GABStartOfWeek.MONDAY.value,
+            "snap_flag": "Y",
+            "join_select": """
+            select distinct year_start as cadence_start_date,
+            case
+                when weekend_mon > date(
+                    date_trunc('YEAR',add_months(calendar_date, 12))
+                )-1
+                    then date(date_trunc('YEAR',add_months(calendar_date, 12)))-1
+                else weekend_mon
+            end as cadence_end_date""",
+            "project_start": _DEFAULT_PROJECT_START,
+            "project_end": _DEFAULT_PROJECT_END,
+        },
+        15: {
+            "cadence": GABCadence.YEAR.name,
+            "recon": GABCadence.WEEK.name,
+            "week_start": GABStartOfWeek.SUNDAY.value,
+            "snap_flag": "Y",
+            "join_select": """
+            select distinct year_start as cadence_start_date,
+            case
+                when weekend_sun > date(
+                    date_trunc('YEAR',add_months(calendar_date, 12))
+                )-1
+                    then date(date_trunc('YEAR',add_months(calendar_date, 12)))-1
+                else weekend_sun
+            end as cadence_end_date""",
+            "project_start": _DEFAULT_PROJECT_START,
+            "project_end": _DEFAULT_PROJECT_END,
+        },
+        16: {
+            "cadence": GABCadence.YEAR.name,
+            "recon": GABCadence.get_cadences(),
+            "week_start": GABStartOfWeek.get_values(),
+            "snap_flag": "N",
+            "inverse_flag": "Y",
+            "join_select": "",
+            "project_start": _PROJECT_DATE_COLUMN_TRUNCATED_BY_CADENCE,
+            "project_end": """
+            date(
+                date_trunc(
+                    '${cad}',add_months(date(date_trunc('${cad}',${date_column})), 12)
+                )
+            )-1
+        """,
+        },
+        17: {
+            "cadence": GABCadence.YEAR.name,
+            "recon": {
+                GABCadence.DAY.name,
+                GABCadence.MONTH.name,
+                GABCadence.QUARTER.name,
+            },
+            "week_start": GABStartOfWeek.get_values(),
+            "snap_flag": "Y",
+            "join_select": """
+            select distinct year_start as cadence_start_date,
+            case
+                when '${rec_cadence}' = 'DAY' then calendar_date
+                when '${rec_cadence}' = 'MONTH' then month_end
+                when '${rec_cadence}' = 'QUARTER' then quarter_end
+            end as cadence_end_date
+        """,
+            "project_start": _DEFAULT_PROJECT_START,
+            "project_end": _DEFAULT_PROJECT_END,
+        },
+        18: {
+            "cadence": GABCadence.get_cadences(),
+            "recon": GABCadence.get_cadences(),
+            "week_start": GABStartOfWeek.get_values(),
+            "snap_flag": {"Y", "N"},
+            "join_select": """
+            select distinct
+            case
+                when '${cad}' = 'WEEK' and '${config_week_start}' = 'Monday'
+                    then weekstart_mon
+                when  '${cad}' = 'WEEK' and '${config_week_start}' = 'Sunday'
+                    then weekstart_sun
+                else
+                    date(date_trunc('${cad}',calendar_date))
+            end as cadence_start_date,
+            case
+                when '${cad}' = 'WEEK' and '${config_week_start}' = 'Monday'
+                    then weekend_mon
+                when  '${cad}' = 'WEEK' and '${config_week_start}' = 'Sunday'
+                    then weekend_sun
+                when '${cad}' = 'DAY'
+                    then date(date_trunc('${cad}',calendar_date))
+                when '${cad}' = 'MONTH'
+                    then date(
+                        date_trunc(
+                            'MONTH',
+                            add_months(date(date_trunc('${cad}',calendar_date)), 1)
+                        )
+                    )-1
+                when '${cad}' = 'QUARTER'
+                    then date(
+                        date_trunc(
+                            'QUARTER',
+                            add_months(date(date_trunc('${cad}',calendar_date)) , 3)
+                        )
+                    )-1
+                when '${cad}' = 'YEAR'
+                    then date(
+                        date_trunc(
+                            'YEAR',
+                            add_months(date(date_trunc('${cad}',calendar_date)), 12)
+                        )
+                    )-1
+            end as cadence_end_date
+        """,
+            "project_start": _DEFAULT_PROJECT_START,
+            "project_end": _DEFAULT_PROJECT_END,
+        },
+    }
```

## lakehouse_engine/core/file_manager.py

```diff
@@ -1,11 +1,12 @@
 """Module for abstract representation of a file manager system."""
 from abc import ABC, abstractmethod
 from typing import Any
 
+from lakehouse_engine.algorithms.exceptions import RestoreTypeNotFoundException
 from lakehouse_engine.utils.storage.file_storage_functions import FileStorageFunctions
 
 
 class FileManager(ABC):  # noqa: B024
     """Abstract file manager class."""
 
     def __init__(self, configs: dict):
@@ -50,11 +51,24 @@
 
     @staticmethod
     def execute_function(configs: dict) -> Any:
         """Get a specific File Manager and function to execute."""
         from lakehouse_engine.core.dbfs_file_manager import DBFSFileManager
         from lakehouse_engine.core.s3_file_manager import S3FileManager
 
-        if FileStorageFunctions.is_boto3_configured():
+        disable_dbfs_retry = (
+            configs["disable_dbfs_retry"]
+            if "disable_dbfs_retry" in configs.keys()
+            else False
+        )
+
+        if disable_dbfs_retry:
             S3FileManager(configs).get_function()
+        elif FileStorageFunctions.is_boto3_configured():
+            try:
+                S3FileManager(configs).get_function()
+            except (ValueError, NotImplementedError, RestoreTypeNotFoundException):
+                raise
+            except Exception:
+                DBFSFileManager(configs).get_function()
         else:
             DBFSFileManager(configs).get_function()
```

## lakehouse_engine/core/table_manager.py

```diff
@@ -53,15 +53,20 @@
         else:
             raise NotImplementedError(
                 f"The requested function {self.function} is not implemented."
             )
 
     def create(self) -> None:
         """Create a new table or view on metastore."""
-        sql = ConfigUtils.read_sql(self.configs["path"])
+        disable_dbfs_retry = (
+            self.configs["disable_dbfs_retry"]
+            if "disable_dbfs_retry" in self.configs.keys()
+            else False
+        )
+        sql = ConfigUtils.read_sql(self.configs["path"], disable_dbfs_retry)
         try:
             sql_commands = SQLParserUtils().split_sql_commands(
                 sql_commands=sql,
                 delimiter=self.configs.get("delimiter", ";"),
                 advanced_parser=self.configs.get("advanced_parser", False),
             )
             for command in sql_commands:
@@ -181,15 +186,20 @@
 
     def execute_multiple_sql_files(self) -> None:
         """Execute multiple statements in multiple sql files.
 
         In this function the path to the files is separated by comma.
         """
         for table_metadata_file in self.configs["path"].split(","):
-            sql = ConfigUtils.read_sql(table_metadata_file.strip())
+            disable_dbfs_retry = (
+                self.configs["disable_dbfs_retry"]
+                if "disable_dbfs_retry" in self.configs.keys()
+                else False
+            )
+            sql = ConfigUtils.read_sql(table_metadata_file.strip(), disable_dbfs_retry)
             sql_commands = SQLParserUtils().split_sql_commands(
                 sql_commands=sql,
                 delimiter=self.configs.get("delimiter", ";"),
                 advanced_parser=self.configs.get("advanced_parser", False),
             )
             for command in sql_commands:
                 if command.strip():
```

## lakehouse_engine/dq_processors/dq_factory.py

```diff
@@ -4,21 +4,21 @@
 from datetime import datetime, timezone
 from json import dumps, loads
 from typing import Any, Dict, List, Optional, OrderedDict, Tuple, Union
 
 from great_expectations.checkpoint.types.checkpoint_result import CheckpointResult
 from great_expectations.core.batch import RuntimeBatchRequest
 from great_expectations.data_context import EphemeralDataContext
+from great_expectations.data_context.data_context.context_factory import get_context
 from great_expectations.data_context.types.base import (
     AnonymizedUsageStatisticsConfig,
     DataContextConfig,
     FilesystemStoreBackendDefaults,
     S3StoreBackendDefaults,
 )
-from great_expectations.util import get_context
 from pyspark.sql import DataFrame
 from pyspark.sql.functions import (
     array,
     col,
     dayofmonth,
     explode,
     from_json,
@@ -132,14 +132,79 @@
             raise TypeError(
                 f"Type of Data Quality '{dq_spec.dq_type}' is not supported."
             )
 
         return data
 
     @classmethod
+    def build_data_docs(
+        cls,
+        store_backend: str = DQDefaults.STORE_BACKEND.value,
+        local_fs_root_dir: str = None,
+        data_docs_local_fs: str = None,
+        data_docs_prefix: str = DQDefaults.DATA_DOCS_PREFIX.value,
+        bucket: str = None,
+        data_docs_bucket: str = None,
+        expectations_store_prefix: str = DQDefaults.EXPECTATIONS_STORE_PREFIX.value,
+        validations_store_prefix: str = DQDefaults.VALIDATIONS_STORE_PREFIX.value,
+        checkpoint_store_prefix: str = DQDefaults.CHECKPOINT_STORE_PREFIX.value,
+    ) -> None:
+        """Build Data Docs for the project.
+
+        This function does a full build of data docs based on all the great expectations
+        checkpoints in the specified location, getting all history of run/validations
+        executed and results.
+
+        Args:
+            store_backend: which store_backend to use (e.g. s3 or file_system).
+            local_fs_root_dir: path of the root directory. Note: only applicable
+                for store_backend file_system
+            data_docs_local_fs: path of the root directory. Note: only applicable
+                for store_backend file_system.
+            data_docs_prefix: prefix where to store data_docs' data.
+            bucket: the bucket name to consider for the store_backend
+                (store DQ artefacts). Note: only applicable for store_backend s3.
+            data_docs_bucket: the bucket name for data docs only. When defined,
+                it will supersede bucket parameter.
+                Note: only applicable for store_backend s3.
+            expectations_store_prefix: prefix where to store expectations' data.
+                Note: only applicable for store_backend s3.
+            validations_store_prefix: prefix where to store validations' data.
+                Note: only applicable for store_backend s3.
+            checkpoint_store_prefix: prefix where to store checkpoints' data.
+                Note: only applicable for store_backend s3.
+        """
+        if store_backend == DQDefaults.STORE_BACKEND.value:
+            dq_spec = DQSpec(
+                spec_id="dq_validator",
+                input_id="dq",
+                dq_type=DQType.VALIDATOR.value,
+                store_backend=DQDefaults.STORE_BACKEND.value,
+                data_docs_prefix=data_docs_prefix,
+                bucket=bucket,
+                data_docs_bucket=data_docs_bucket,
+                expectations_store_prefix=expectations_store_prefix,
+                validations_store_prefix=validations_store_prefix,
+                checkpoint_store_prefix=checkpoint_store_prefix,
+            )
+        elif store_backend == DQDefaults.FILE_SYSTEM_STORE.value:
+            dq_spec = DQSpec(
+                spec_id="dq_validator",
+                input_id="dq",
+                dq_type=DQType.VALIDATOR.value,
+                store_backend=DQDefaults.FILE_SYSTEM_STORE.value,
+                local_fs_root_dir=local_fs_root_dir,
+                data_docs_local_fs=data_docs_local_fs,
+                data_docs_prefix=data_docs_prefix,
+            )
+        context = get_context(project_config=cls._get_data_context_config(dq_spec))
+        cls._LOGGER.info("The data docs were rebuilt")
+        context.build_data_docs()
+
+    @classmethod
     def _check_critical_functions_tags(cls, failed_expectations: List[Any]) -> list:
         critical_failure = []
 
         for expectation in failed_expectations:
             meta = expectation["meta"]
             if meta and (
                 ("notes" in meta.keys() and "Critical function" in meta["notes"])
```

## lakehouse_engine/dq_processors/custom_expectations/expect_multicolumn_column_a_must_equal_b_or_c.py

```diff
@@ -51,18 +51,15 @@
                 & (column_list[2].rlike(validation_regex_c))
                 & (column_list[0] == column_list[2])
             )
         )
 
 
 class ExpectMulticolumnColumnAMustEqualBOrC(MulticolumnMapExpectation):
-    """MultiColumn Expectation.
-
-    Expect that the column 'a' is equal to 'b' when this is
-    not empty; otherwise 'a' must be equal to 'c'.
+    """Expect that the column 'a' is equal to 'b' when this is not empty; otherwise 'a' must be equal to 'c'.
 
     Args:
         column_list: The column names to evaluate.
 
     Keyword Args:
         - ignore_row_if: default to "never".
         - result_format:  Which output mode to use:
@@ -73,15 +70,15 @@
            Default set to True.
         - catch_exceptions: If True, then catch exceptions
            and include them as part of the result object.
            Default set to False.
 
     Returns:
         An ExpectationSuiteValidationResult.
-    """
+    """  # noqa: E501
 
     examples = [
         {
             "dataset_name": "Test Dataset",
             "data": [
                 {
                     "data": {
```

## lakehouse_engine/io/writers/dataframe_writer.py

```diff
@@ -98,15 +98,16 @@
         """
         app_id = ExecEnv.SESSION.getActiveSession().conf.get("spark.app.id")
         stream_df_view_name = f"`{app_id}_{output_spec.spec_id}`"
         DataFrameWriter._logger.info("Drop temp view if exists")
 
         if DataFrameWriter._table_exists(stream_df_view_name):
             # Cleaning global temp view to not maintain state and impact other acon runs
-            ExecEnv.SESSION.catalog.dropGlobalTempView(stream_df_view_name.strip("`"))
+            view_name = stream_df_view_name.strip("`")
+            ExecEnv.SESSION.sql(f"DROP VIEW global_temp.`{view_name}`")
 
         df_writer = df.writeStream.trigger(**Writer.get_streaming_trigger(output_spec))
 
         if (
             output_spec.streaming_micro_batch_transformers
             or output_spec.streaming_micro_batch_dq_processors
         ):
```

## lakehouse_engine/transformers/column_reshapers.py

```diff
@@ -323,36 +323,38 @@
     def from_json(
         cls,
         input_col: str,
         schema_path: Optional[str] = None,
         schema: Optional[dict] = None,
         json_options: Optional[dict] = None,
         drop_all_cols: bool = False,
+        disable_dbfs_retry: bool = False,
     ) -> Callable:
         """Convert a json string into a json column (struct).
 
         The new json column can be added to the existing columns (default) or it can
         replace all the others, being the only one to output. The new column gets the
         same name as the original one suffixed with '_json'.
 
         Args:
             input_col: dict with columns and respective target names.
             schema_path: path to the StructType schema (spark schema).
             schema: dict with the StructType schema (spark schema).
             json_options: options to parse the json value.
             drop_all_cols: whether to drop all the input columns or not.
                 Defaults to False.
+            disable_dbfs_retry: optional flag to disable file storage dbfs.
 
         Returns:
             A function to be called in .transform() spark function.
         """
 
         def inner(df: DataFrame) -> DataFrame:
             if schema_path:
-                json_schema = SchemaUtils.from_file(schema_path)
+                json_schema = SchemaUtils.from_file(schema_path, disable_dbfs_retry)
             elif schema:
                 json_schema = SchemaUtils.from_dict(schema)
             else:
                 raise WrongArgumentsException(
                     "A file or dict schema needs to be provided."
                 )
```

## lakehouse_engine/utils/engine_usage_stats.py

```diff
@@ -2,15 +2,15 @@
 import ast
 import json
 import re
 from datetime import datetime
 from typing import Dict
 from urllib.parse import urlparse
 
-from lakehouse_engine.core.definitions import EngineStats
+from lakehouse_engine.core.definitions import CollectEngineUsage, EngineStats
 from lakehouse_engine.core.exec_env import ExecEnv
 from lakehouse_engine.utils.configs.config_utils import ConfigUtils
 from lakehouse_engine.utils.logging_handler import LoggingHandler
 from lakehouse_engine.utils.storage.file_storage_functions import FileStorageFunctions
 
 
 class EngineUsageStats(object):
@@ -19,69 +19,84 @@
     _LOGGER = LoggingHandler(__name__).get_logger()
 
     @classmethod
     def store_engine_usage(
         cls,
         acon: dict,
         func_name: str,
-        collect_engine_usage: bool = None,
+        collect_engine_usage: str = None,
         spark_confs: dict = None,
     ) -> None:
         """Collects and store Lakehouse Engine usage statistics.
 
         These statistics include the acon and other relevant information, such as
         the lakehouse engine version and the functions/algorithms being used.
 
         Args:
             acon: acon dictionary file.
             func_name: function name that called this log acon.
-            collect_engine_usage: a boolean that enables or disables the collection and
-                storage of Lakehouse usage statistics.
+            collect_engine_usage: Lakehouse usage statistics collection strategy.
             spark_confs: optional dictionary with the spark confs to be used when
                 collecting the engine usage.
         """
         try:
-            engine_usage_path = ExecEnv.ENGINE_CONFIG.engine_usage_path
-
             if (
-                collect_engine_usage or ExecEnv.ENGINE_CONFIG.collect_engine_usage
-            ) and engine_usage_path is not None:
+                collect_engine_usage
+                in [
+                    CollectEngineUsage.ENABLED.value,
+                    CollectEngineUsage.PROD_ONLY.value,
+                ]
+                or ExecEnv.ENGINE_CONFIG.collect_engine_usage
+                in CollectEngineUsage.ENABLED.value
+            ):
                 start_timestamp = datetime.now()
                 timestamp_str = start_timestamp.strftime("%Y%m%d%H%M%S")
 
                 usage_stats: Dict = {"acon": ConfigUtils.remove_sensitive_info(acon)}
                 EngineUsageStats.get_spark_conf_values(usage_stats, spark_confs)
 
-                usage_stats["function"] = func_name
-                usage_stats["engine_version"] = ConfigUtils.get_engine_version()
-                usage_stats["start_timestamp"] = start_timestamp
-                usage_stats["year"] = start_timestamp.year
-                usage_stats["month"] = start_timestamp.month
-                run_id_extracted = re.search("run-([1-9]\\w+)", usage_stats["run_id"])
-                usage_stats["run_id"] = (
-                    run_id_extracted.group(1) if run_id_extracted else ""
-                )
-
-                log_file_name = f"eng_usage_{func_name}_{timestamp_str}.json"
-
-                usage_stats_str = json.dumps(usage_stats, default=str)
-
-                url = urlparse(
-                    f"{engine_usage_path}/{usage_stats['dp_name']}/"
-                    f"{start_timestamp.year}/{start_timestamp.month}/{log_file_name}",
-                    allow_fragments=False,
-                )
-
-                try:
-                    FileStorageFunctions.write_payload(
-                        engine_usage_path, url, usage_stats_str
+                engine_usage_path = None
+                if usage_stats["environment"] == "prod":
+                    engine_usage_path = ExecEnv.ENGINE_CONFIG.engine_usage_path
+                elif collect_engine_usage != CollectEngineUsage.PROD_ONLY.value:
+                    engine_usage_path = ExecEnv.ENGINE_CONFIG.engine_dev_usage_path
+
+                if engine_usage_path is not None:
+                    usage_stats["function"] = func_name
+                    usage_stats["engine_version"] = ConfigUtils.get_engine_version()
+                    usage_stats["start_timestamp"] = start_timestamp
+                    usage_stats["year"] = start_timestamp.year
+                    usage_stats["month"] = start_timestamp.month
+                    run_id_extracted = re.search(
+                        "run-([1-9]\\w+)", usage_stats["run_id"]
+                    )
+                    usage_stats["run_id"] = (
+                        run_id_extracted.group(1) if run_id_extracted else ""
                     )
-                    cls._LOGGER.info("Storing Lakehouse Engine usage statistics")
-                except FileNotFoundError as e:
-                    cls._LOGGER.error(f"Could not write engine stats into file: {e}.")
+
+                    log_file_name = f"eng_usage_{func_name}_{timestamp_str}.json"
+
+                    usage_stats_str = json.dumps(usage_stats, default=str)
+
+                    url = urlparse(
+                        f"{engine_usage_path}/{usage_stats['dp_name']}/"
+                        f"{start_timestamp.year}/{start_timestamp.month}/"
+                        f"{log_file_name}",
+                        allow_fragments=False,
+                    )
+
+                    try:
+                        FileStorageFunctions.write_payload(
+                            engine_usage_path, url, usage_stats_str
+                        )
+                        cls._LOGGER.info("Storing Lakehouse Engine usage statistics")
+                    except FileNotFoundError as e:
+                        cls._LOGGER.error(
+                            f"Could not write engine stats into file: {e}."
+                        )
         except Exception as e:
             cls._LOGGER.error(
                 "Failed while collecting the lakehouse engine stats: "
                 f"Unexpected {e=}, {type(e)=}."
             )
 
     @classmethod
```

## lakehouse_engine/utils/schema_utils.py

```diff
@@ -13,40 +13,42 @@
 
 class SchemaUtils(object):
     """Schema utils that help retrieve and manage schemas of dataframes."""
 
     _logger: Logger = LoggingHandler(__name__).get_logger()
 
     @staticmethod
-    def from_file(file_path: str) -> StructType:
+    def from_file(file_path: str, disable_dbfs_retry: bool = False) -> StructType:
         """Get a spark schema from a file (spark StructType json file) in a file system.
 
         Args:
             file_path: path of the file in a file system. [Check here](
                 https://spark.apache.org/docs/latest/api/java/org/apache/spark/sql/types/StructType.html).
-
-
+            disable_dbfs_retry: optional flag to disable file storage dbfs.
 
         Returns:
             Spark schema struct type.
         """
-        return StructType.fromJson(FileStorageFunctions.read_json(file_path))
+        return StructType.fromJson(
+            FileStorageFunctions.read_json(file_path, disable_dbfs_retry)
+        )
 
     @staticmethod
-    def from_file_to_dict(file_path: str) -> Any:
+    def from_file_to_dict(file_path: str, disable_dbfs_retry: bool = False) -> Any:
         """Get a dict with the spark schema from a file in a file system.
 
         Args:
             file_path: path of the file in a file system. [Check here](
                 https://spark.apache.org/docs/latest/api/java/org/apache/spark/sql/types/StructType.html).
+            disable_dbfs_retry: optional flag to disable file storage dbfs.
 
         Returns:
              Spark schema in a dict.
         """
-        return FileStorageFunctions.read_json(file_path)
+        return FileStorageFunctions.read_json(file_path, disable_dbfs_retry)
 
     @staticmethod
     def from_dict(struct_type: dict) -> StructType:
         """Get a spark schema from a dict.
 
         Args:
             struct_type: dict containing a spark schema structure. [Check here](
@@ -87,15 +89,17 @@
         if input_spec.enforce_schema_from_table:
             cls._logger.info(
                 f"Reading schema from table: {input_spec.enforce_schema_from_table}"
             )
             return SchemaUtils.from_table_schema(input_spec.enforce_schema_from_table)
         elif input_spec.schema_path:
             cls._logger.info(f"Reading schema from file: {input_spec.schema_path}")
-            return SchemaUtils.from_file(input_spec.schema_path)
+            return SchemaUtils.from_file(
+                input_spec.schema_path, input_spec.disable_dbfs_retry
+            )
         elif input_spec.schema:
             cls._logger.info(
                 f"Reading schema from configuration file: {input_spec.schema}"
             )
             return SchemaUtils.from_dict(input_spec.schema)
         else:
             cls._logger.info("No schema was provided... skipping enforce schema")
```

## lakehouse_engine/utils/configs/config_utils.py

```diff
@@ -25,26 +25,30 @@
     ]
 
     @classmethod
     def get_acon(
         cls,
         acon_path: Optional[str] = None,
         acon: Optional[dict] = None,
+        disable_dbfs_retry: bool = False,
     ) -> dict:
         """Get acon based on a filesystem path or on a dict.
 
         Args:
             acon_path: path of the acon (algorithm configuration) file.
             acon: acon provided directly through python code (e.g., notebooks
                 or other apps).
+            disable_dbfs_retry: optional flag to disable file storage dbfs.
 
         Returns:
             Dict representation of an acon.
         """
-        acon = acon if acon else ConfigUtils.read_json_acon(acon_path)
+        acon = (
+            acon if acon else ConfigUtils.read_json_acon(acon_path, disable_dbfs_retry)
+        )
         cls._LOGGER.info(f"Read Algorithm Configuration: {str(acon)}")
         return acon
 
     @staticmethod
     def get_config(package: str = "lakehouse_engine.configs") -> Any:
         """Get the lakehouse engine configuration file.
 
@@ -66,36 +70,38 @@
             version = pkg_resources.get_distribution("lakehouse-engine").version
         except pkg_resources.DistributionNotFound:
             cls._LOGGER.info("Could not identify Lakehouse Engine version.")
             version = ""
         return str(version)
 
     @staticmethod
-    def read_json_acon(path: str) -> Any:
+    def read_json_acon(path: str, disable_dbfs_retry: bool = False) -> Any:
         """Read an acon (algorithm configuration) file.
 
         Args:
             path: path to the acon file.
+            disable_dbfs_retry: optional flag to disable file storage dbfs.
 
         Returns:
             The acon file content as a dict.
         """
-        return FileStorageFunctions.read_json(path)
+        return FileStorageFunctions.read_json(path, disable_dbfs_retry)
 
     @staticmethod
-    def read_sql(path: str) -> Any:
+    def read_sql(path: str, disable_dbfs_retry: bool = False) -> Any:
         """Read a DDL file in Spark SQL format from a cloud object storage system.
 
         Args:
             path: path to the SQL file.
+            disable_dbfs_retry: optional flag to disable file storage dbfs.
 
         Returns:
             Content of the SQL file.
         """
-        return FileStorageFunctions.read_sql(path)
+        return FileStorageFunctions.read_sql(path, disable_dbfs_retry)
 
     @classmethod
     def remove_sensitive_info(
         cls, dict_to_replace: Union[dict, list]
     ) -> Union[dict, list]:
         """Remove sensitive info from a dictionary.
```

## lakehouse_engine/utils/storage/dbfs_storage.py

```diff
@@ -22,15 +22,15 @@
 
         Returns:
             File payload/content.
         """
         from lakehouse_engine.core.exec_env import ExecEnv
 
         str_url = urlunparse(url)
-        cls._LOGGER.info(f"Reading from file: {str_url}")
+        cls._LOGGER.info(f"Trying with dbfs_storage: Reading from file: {str_url}")
         return DatabricksUtils.get_db_utils(ExecEnv.SESSION).fs.head(
             str_url, cls._MAX_INT
         )
 
     @classmethod
     def write_payload_to_file(cls, url: ParseResult, content: str) -> None:
         """Write payload into a file.
@@ -38,9 +38,9 @@
         Args:
             url: url of the file.
             content: content to write into the file.
         """
         from lakehouse_engine.core.exec_env import ExecEnv
 
         str_url = urlunparse(url)
-        cls._LOGGER.info(f"Writing into file: {str_url}")
+        cls._LOGGER.info(f"Trying with dbfs_storage: Writing into file: {str_url}")
         DatabricksUtils.get_db_utils(ExecEnv.SESSION).fs.put(str_url, content, True)
```

## lakehouse_engine/utils/storage/file_storage_functions.py

```diff
@@ -11,77 +11,97 @@
 from lakehouse_engine.utils.storage.s3_storage import S3Storage
 
 
 class FileStorageFunctions(ABC):  # noqa: B024
     """Class for common file storage functions."""
 
     @classmethod
-    def read_json(cls, path: str) -> Any:
+    def read_json(cls, path: str, disable_dbfs_retry: bool = False) -> Any:
         """Read a json file.
 
         The file should be in a supported file system (e.g., s3, dbfs or
         local filesystem).
 
         Args:
             path: path to the json file.
+            disable_dbfs_retry: optional flag to disable file storage dbfs.
 
         Returns:
             Dict with json file content.
         """
         url = urlparse(path, allow_fragments=False)
-        if url.scheme == "s3" and cls.is_boto3_configured():
+        if disable_dbfs_retry:
             return json.load(S3Storage.get_file_payload(url))
+        elif url.scheme == "s3" and cls.is_boto3_configured():
+            try:
+                return json.load(S3Storage.get_file_payload(url))
+            except Exception:
+                return json.loads(DBFSStorage.get_file_payload(url))
         elif url.scheme == "file":
             return json.load(LocalFSStorage.get_file_payload(url))
         elif url.scheme in ["dbfs", "s3"]:
             return json.loads(DBFSStorage.get_file_payload(url))
         else:
             raise NotImplementedError(
                 f"File storage protocol not implemented for {path}."
             )
 
     @classmethod
-    def read_sql(cls, path: str) -> Any:
+    def read_sql(cls, path: str, disable_dbfs_retry: bool = False) -> Any:
         """Read a sql file.
 
         The file should be in a supported file system (e.g., s3, dbfs or local
         filesystem).
 
         Args:
             path: path to the sql file.
+            disable_dbfs_retry: optional flag to disable file storage dbfs.
 
         Returns:
             Content of the SQL file.
         """
         url = urlparse(path, allow_fragments=False)
-        if url.scheme == "s3" and cls.is_boto3_configured():
+        if disable_dbfs_retry:
             return S3Storage.get_file_payload(url).read().decode("utf-8")
+        elif url.scheme == "s3" and cls.is_boto3_configured():
+            try:
+                return S3Storage.get_file_payload(url).read().decode("utf-8")
+            except Exception:
+                return DBFSStorage.get_file_payload(url)
         elif url.scheme == "file":
             return LocalFSStorage.get_file_payload(url).read()
         elif url.scheme in ["dbfs", "s3"]:
             return DBFSStorage.get_file_payload(url)
         else:
             raise NotImplementedError(
                 f"Object storage protocol not implemented for {path}."
             )
 
     @classmethod
-    def write_payload(cls, path: str, url: ParseResult, content: str) -> None:
+    def write_payload(
+        cls, path: str, url: ParseResult, content: str, disable_dbfs_retry: bool = False
+    ) -> None:
         """Write payload into a file.
 
         The file should be in a supported file system (e.g., s3, dbfs or local
         filesystem).
 
         Args:
             path: path to validate the file type.
             url: url of the file.
             content: content to write into the file.
+            disable_dbfs_retry: optional flag to disable file storage dbfs.
         """
-        if path.startswith("s3://") and cls.is_boto3_configured():
+        if disable_dbfs_retry:
             S3Storage.write_payload_to_file(url, content)
+        elif path.startswith("s3://") and cls.is_boto3_configured():
+            try:
+                S3Storage.write_payload_to_file(url, content)
+            except Exception:
+                DBFSStorage.write_payload_to_file(url, content)
         elif path.startswith(("s3://", "dbfs:/")):
             DBFSStorage.write_payload_to_file(url, content)
         else:
             LocalFSStorage.write_payload_to_file(url, content)
 
     @staticmethod
     def is_boto3_configured() -> bool:
```

## lakehouse_engine/utils/storage/s3_storage.py

```diff
@@ -21,22 +21,28 @@
             url: url of the file.
 
         Returns:
             File payload/content.
         """
         s3 = boto3.resource("s3")
         obj = s3.Object(url.netloc, url.path.lstrip("/"))
-        cls._LOGGER.info(f"Reading from file: {url.scheme}://{url.netloc}{url.path}")
+        cls._LOGGER.info(
+            f"Trying with s3_storage: "
+            f"Reading from file: {url.scheme}://{url.netloc}{url.path}"
+        )
         return obj.get()["Body"]
 
     @classmethod
     def write_payload_to_file(cls, url: ParseResult, content: str) -> None:
         """Write payload into a file.
 
         Args:
             url: url of the file.
             content: content to write into the file.
         """
         s3 = boto3.resource("s3")
         obj = s3.Object(url.netloc, url.path.lstrip("/"))
-        cls._LOGGER.info(f"Writing into file: {url.scheme}://{url.netloc}{url.path}")
+        cls._LOGGER.info(
+            f"Trying with s3_storage: "
+            f"Writing into file: {url.scheme}://{url.netloc}{url.path}"
+        )
         obj.put(Body=content)
```

## tests/feature/test_data_quality.py

```diff
@@ -1,8 +1,10 @@
 """Test data quality process in different types of data loads."""
+import shutil
+from os import stat
 from os.path import exists
 from typing import Any
 
 import pytest
 from pyspark.sql import DataFrame
 from pyspark.sql.functions import (
     array_sort,
@@ -12,15 +14,15 @@
     schema_of_json,
     transform,
 )
 
 from lakehouse_engine.core.definitions import DQDefaults, DQFunctionSpec, DQSpec
 from lakehouse_engine.dq_processors.dq_factory import DQFactory
 from lakehouse_engine.dq_processors.exceptions import DQValidationsFailedException
-from lakehouse_engine.engine import load_data
+from lakehouse_engine.engine import build_data_docs, load_data
 from lakehouse_engine.utils.schema_utils import SchemaUtils
 from tests.conftest import (
     FEATURE_RESOURCES,
     LAKEHOUSE_FEATURE_CONTROL,
     LAKEHOUSE_FEATURE_IN,
     LAKEHOUSE_FEATURE_OUT,
 )
@@ -615,7 +617,89 @@
                             "",
                         ),
                     ),
                 ),
             ),
         ),
     )
+
+
+@pytest.mark.parametrize(
+    "scenario",
+    [
+        {
+            "scenario_name": "without_data_docs_local_fs",
+            "local_fs_root_dir": f"{TEST_LAKEHOUSE_OUT.replace('file://', '')}/"
+            f"load_with_dq_validator/no_transformers/dq",
+            "data_docs_local_fs": None,
+            "data_docs_prefix": DQDefaults.DATA_DOCS_PREFIX.value,
+        },
+        {
+            "scenario_name": "with_data_docs_local_fs",
+            "local_fs_root_dir": f"{TEST_LAKEHOUSE_OUT.replace('file://', '')}/"
+            f"validator",
+            "data_docs_local_fs": f"{TEST_LAKEHOUSE_OUT.replace('file://', '')}/"
+            f"validator/data_docs",
+            "data_docs_prefix": DQDefaults.DATA_DOCS_PREFIX.value,
+        },
+    ],
+)
+def test_build_data_docs(scenario: dict, caplog: Any) -> None:
+    """Test the data quality build data docs process.
+
+    The tests executed intend to validate if the build of data docs is
+    done successfully. It is expected that data docs are built considering
+    all the history of checkpoints, even when changing store_backend s3 to
+    file_system. The build of data docs should enable all the runs/validations,
+    that are stored in the path specified, to be available in data docs
+    website, with all the history of runs/validations.
+
+    These tests enable to validate if the build of data docs is done
+    correctly when adding an extra checkpoint, having a specific
+    data_docs_local_fs or using the default value:
+    - without_data_docs_local_fs: data quality is stored in file_system
+    and for this test local_fs_root_dir is specified and data_docs_local_fs
+    and data_docs_prefix have the default value.
+    - with_data_docs_local_fs: data quality is stored in file_system
+    and for this test local_fs_root_dir and data_docs_local_fs are specified
+    and data_docs_prefix have the default value.
+
+    Args:
+        scenario: scenario to test.
+        caplog: captured log.
+    """
+    if scenario["data_docs_local_fs"]:
+        data_docs_location = (
+            f'{scenario["data_docs_local_fs"]}/{scenario["data_docs_prefix"]}index.html'
+        )
+    else:
+        data_docs_location = (
+            f'{scenario["local_fs_root_dir"]}/{scenario["data_docs_prefix"]}index.html'
+        )
+    file_stats_before = stat(data_docs_location)
+    if scenario["scenario_name"] == "without_data_docs_local_fs":
+        checkpoint_name = "20240409-143548-dq_validator-sales_source-checkpoint"
+        shutil.copytree(
+            src=f'{TEST_RESOURCES.replace("/app/", "")}/build_data_docs/'
+            f'{scenario["scenario_name"]}/{checkpoint_name}',
+            dst=f'{scenario["local_fs_root_dir"].replace("/app/", "")}/uncommitted/'
+            f"validations/dq_validator-sales_source-validator/{checkpoint_name}",
+        )
+    elif scenario["scenario_name"] == "with_data_docs_local_fs":
+        checkpoint_name = "20240410-080323-dq_success-sales_orders-checkpoint"
+        shutil.copytree(
+            src=f'{TEST_RESOURCES.replace("/app/", "")}/build_data_docs/'
+            f'{scenario["scenario_name"]}/{checkpoint_name}',
+            dst=f'{scenario["local_fs_root_dir"].replace("/app/", "")}/uncommitted/'
+            f"validations/dq_success-sales_orders-validator/{checkpoint_name}",
+        )
+
+    build_data_docs(
+        store_backend=DQDefaults.FILE_SYSTEM_STORE.value,
+        local_fs_root_dir=scenario["local_fs_root_dir"],
+        data_docs_local_fs=scenario["data_docs_local_fs"],
+        data_docs_prefix=scenario["data_docs_prefix"],
+    )
+
+    file_stats_after = stat(data_docs_location)
+    assert "The data docs were rebuilt" in caplog.text
+    assert file_stats_before.st_size < file_stats_after.st_size
```

## tests/feature/test_engine_usage_stats.py

```diff
@@ -124,15 +124,15 @@
         f"{TEST_RESOURCES}/{scenario}/data/control.json",
         f"{TEST_LAKEHOUSE_CONTROL}/{scenario}/data/",
     )
 
     load_data(
         acon=_get_test_acon(scenario),
         spark_confs={"dp_name": "dp_name"},
-        collect_engine_usage=True,
+        collect_engine_usage="enabled",
     )
 
     _prepare_and_compare_dfs(scenario)
 
 
 @pytest.mark.parametrize("scenario", ["table_manager"])
 def test_table_manager(scenario: str) -> None:
@@ -152,15 +152,15 @@
     acon = {
         "function": "execute_sql",
         "sql": "select 1",
         "exec_env": {"dp_name": scenario},
     }
 
     manage_table(
-        acon=acon, spark_confs={"dp_name": "dp_name"}, collect_engine_usage=True
+        acon=acon, spark_confs={"dp_name": "dp_name"}, collect_engine_usage="enabled"
     )
 
     _prepare_and_compare_dfs(scenario)
 
 
 @pytest.mark.parametrize("scenario", ["dq_validator"])
 def test_dq_validator(scenario: str) -> None:
@@ -210,15 +210,15 @@
                 },
             ],
         },
         "exec_env": {"dp_name": scenario},
     }
 
     execute_dq_validation(
-        acon=acon, spark_confs={"dp_name": "dp_name"}, collect_engine_usage=True
+        acon=acon, spark_confs={"dp_name": "dp_name"}, collect_engine_usage="enabled"
     )
 
     _prepare_and_compare_dfs(scenario)
 
 
 def _prepare_and_compare_dfs(scenario: str) -> None:
     """Prepare DF and compare test and control dataframes.
```

## tests/feature/custom_expectations/test_expectation_validity.py

```diff
@@ -1,8 +1,9 @@
 """Module with the validation code for the custom expectations."""
+import copy
 import importlib
 import re
 
 import pytest
 
 from lakehouse_engine.core.definitions import DQDefaults
 
@@ -84,15 +85,15 @@
 
 def _process_diagnostics_output(diagnostics_output: str) -> None:
     """Processes the output from the expectation diagnostics.
 
     Args:
         diagnostics_output: the output from the diagnostics command.
     """
-    validations = DIAGNOSTICS_VALIDATIONS
+    validations = copy.deepcopy(DIAGNOSTICS_VALIDATIONS)
     for line in str(diagnostics_output).split("\n"):
         if CHECKMARK in line:
             for validation in validations:
                 if re.match(validation, line):
                     validations.remove(validation)
                     break
```

## Comparing `lakehouse_engine-1.19.0.data/data/requirements/requirements_os.lock` & `lakehouse_engine-1.20.0.data/data/requirements/requirements_os.lock`

 * *Files 1% similar despite different names*

```diff
@@ -376,16 +376,18 @@
     # via nbconvert
 paramiko==3.4.0
     # via -r cicd/requirements.txt
 parso==0.8.3
     # via jedi
 patsy==0.5.3
     # via statsmodels
-pendulum==2.1.2
-    # via microsoft-kiota-serialization-json
+pendulum==3.0.0
+    # via
+    #   -r cicd/requirements.txt
+    #   microsoft-kiota-serialization-json
 pexpect==4.8.0
     # via ipython
 phik==0.12.3
     # via ydata-profiling
 pickleshare==0.7.5
     # via ipython
 pillow==10.1.0
@@ -442,22 +444,21 @@
     #   botocore
     #   great-expectations
     #   jupyter-client
     #   matplotlib
     #   microsoft-kiota-serialization-text
     #   pandas
     #   pendulum
+    #   time-machine
 python-json-logger==2.0.7
     # via jupyter-events
 pytz==2023.3.post1
     # via
     #   great-expectations
     #   pandas
-pytzdata==2020.1
-    # via pendulum
 pywavelets==1.4.1
     # via imagehash
 pyyaml==6.0.1
     # via
     #   -r cicd/requirements.txt
     #   jupyter-events
     #   ydata-profiling
@@ -530,14 +531,16 @@
     # via microsoft-kiota-abstractions
 tangled-up-in-unicode==0.2.0
     # via visions
 terminado==0.18.0
     # via
     #   jupyter-server
     #   jupyter-server-terminals
+time-machine==2.13.0
+    # via pendulum
 tinycss2==1.2.1
     # via nbconvert
 tomli==2.0.1
     # via jupyterlab
 toolz==0.12.0
     # via altair
 tornado==6.4
@@ -581,15 +584,17 @@
     #   azure-core
     #   great-expectations
     #   ipython
     #   opentelemetry-sdk
     #   pydantic
     #   typeguard
 tzdata==2023.3
-    # via pandas
+    # via
+    #   pandas
+    #   pendulum
 tzlocal==5.1
     # via great-expectations
 uri-template==1.3.0
     # via jsonschema
 urllib3==1.26.17
     # via
     #   botocore
```

## Comparing `lakehouse_engine-1.19.0.dist-info/LICENSE.txt` & `lakehouse_engine-1.20.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `lakehouse_engine-1.19.0.dist-info/METADATA` & `lakehouse_engine-1.20.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakehouse-engine
-Version: 1.19.0
+Version: 1.20.0
 Summary: A Spark framework serving as the engine for several lakehouse algorithms and data flows.
 Home-page: https://adidas.github.io/lakehouse-engine-docs/lakehouse_engine.html
 Author: Adidas Lakehouse Foundations Team
 Author-email: software.engineering@adidas.com
 Project-URL: Source Code, https://adidas.github.io/lakehouse-engine
 Project-URL: Documentation, https://adidas.github.io/lakehouse-engine-docs/lakehouse_engine.html
 Project-URL: Issues, https://github.com/adidas/lakehouse-engine/issues
@@ -129,15 +129,15 @@
 Requires-Dist: overrides ==7.6.0
 Requires-Dist: packaging ==23.2
 Requires-Dist: pandas ==2.0.3
 Requires-Dist: pandocfilters ==1.5.1
 Requires-Dist: paramiko ==3.4.0
 Requires-Dist: parso ==0.8.3
 Requires-Dist: patsy ==0.5.3
-Requires-Dist: pendulum ==2.1.2
+Requires-Dist: pendulum ==3.0.0
 Requires-Dist: pexpect ==4.8.0
 Requires-Dist: phik ==0.12.3
 Requires-Dist: pickleshare ==0.7.5
 Requires-Dist: pillow ==10.1.0
 Requires-Dist: platformdirs ==4.1.0
 Requires-Dist: portalocker ==2.8.2
 Requires-Dist: prometheus-client ==0.19.0
@@ -152,15 +152,14 @@
 Requires-Dist: pyjwt[crypto] ==2.8.0
 Requires-Dist: pynacl ==1.5.0
 Requires-Dist: pyparsing ==3.1.1
 Requires-Dist: pyspark ==3.4.1
 Requires-Dist: python-dateutil ==2.8.2
 Requires-Dist: python-json-logger ==2.0.7
 Requires-Dist: pytz ==2023.3.post1
-Requires-Dist: pytzdata ==2020.1
 Requires-Dist: pywavelets ==1.4.1
 Requires-Dist: pyyaml ==6.0.1
 Requires-Dist: pyzmq ==25.1.2
 Requires-Dist: referencing ==0.30.2
 Requires-Dist: requests ==2.31.0
 Requires-Dist: rfc3339-validator ==0.1.4
 Requires-Dist: rfc3986-validator ==0.1.1
@@ -175,14 +174,15 @@
 Requires-Dist: sniffio ==1.3.0
 Requires-Dist: soupsieve ==2.5
 Requires-Dist: stack-data ==0.6.3
 Requires-Dist: statsmodels ==0.14.0
 Requires-Dist: std-uritemplate ==0.0.43
 Requires-Dist: tangled-up-in-unicode ==0.2.0
 Requires-Dist: terminado ==0.18.0
+Requires-Dist: time-machine ==2.13.0
 Requires-Dist: tinycss2 ==1.2.1
 Requires-Dist: tomli ==2.0.1
 Requires-Dist: toolz ==0.12.0
 Requires-Dist: tornado ==6.4
 Requires-Dist: tqdm ==4.66.1
 Requires-Dist: traitlets ==5.11.2
 Requires-Dist: typeguard ==4.1.5
```

## Comparing `lakehouse_engine-1.19.0.dist-info/RECORD` & `lakehouse_engine-1.20.0.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 lakehouse_engine/__init__.py,sha256=UNAIviNRi0OCr1uT1z8iGS1-__9shlPV8kP3rOmI_Es,474
-lakehouse_engine/engine.py,sha256=Y0-yJtvUmInYCh0l2wyhMfbPKlm69gmg6dFjJmfMM1A,11338
+lakehouse_engine/engine.py,sha256=wUi9QYcJMJRGOp1RPFCkA4XwhzInCRbgK3Qijot34E0,14690
 lakehouse_engine/algorithms/__init__.py,sha256=V78ZLqCZ0wgUmLuuMLs0WhyX3PmaNhOBdfoQ2Ql2irw,62
 lakehouse_engine/algorithms/algorithm.py,sha256=SdyhET7fjYolwjeFRoq_nroGpesxGx3FMEIXjBKqSqQ,5527
 lakehouse_engine/algorithms/data_loader.py,sha256=ClxXsoxbqOVL2G_wPlksX3tFU-qi4QjSobmqwifMfj4,23776
 lakehouse_engine/algorithms/dq_validator.py,sha256=ELhWWQeZP3Pc5lxfFHTG_uPLPzDUexjr8ej2nQfKN4w,6163
 lakehouse_engine/algorithms/exceptions.py,sha256=LzfvAQllM518O2lUqDRsEfJzRuapzP_imVsiOfSIpkA,539
+lakehouse_engine/algorithms/gab.py,sha256=9wW7AQP6xYuLbRHkqs9WZwrWhkG0QkwvzpbnwlxV0QI,34132
 lakehouse_engine/algorithms/reconciliator.py,sha256=ob3iHOgR-MSLp8gjTW0s-J131pN3f0dfyKtl59TxBX4,12407
 lakehouse_engine/algorithms/sensor.py,sha256=yeN7WoUl60LQyu-vOjBHEVOm7bBNFa7DwUaV358kpu0,5887
 lakehouse_engine/configs/__init__.py,sha256=g8qwCRM1_9z6DhQnC0vfptk0IP9GrhqqLX3IyISTXJQ,73
 lakehouse_engine/configs/engine.yaml,sha256=t_FMUburp2fN60tpZlITvSYHQH-Q_UkF3_yTWrfqFNA,29
 lakehouse_engine/core/__init__.py,sha256=0x60VJkynFTtnnQKv91oYnDh9q1vPEDny0Arfc7yRps,63
 lakehouse_engine/core/dbfs_file_manager.py,sha256=hoqMmNH6qqALMCYhdcR4pHezNnnLn76QIfg9Y5grs78,8750
-lakehouse_engine/core/definitions.py,sha256=n19HtscksDY2FhLrvlOoJJ70IEULSIcoTst5FQN5ZqI,31043
+lakehouse_engine/core/definitions.py,sha256=Wldig41KYwMi4exnBB6bnQXAE4WZlwxlJcYK_YUlocU,50454
 lakehouse_engine/core/exec_env.py,sha256=6re-wQkbtjqLBIKYabL1afBLo-0BpcCfveEaL9uuIzQ,4088
 lakehouse_engine/core/executable.py,sha256=G25WggJI7Iibx5nqfYIx0aipkh0ZWfYKnkXYjmGiIbA,445
-lakehouse_engine/core/file_manager.py,sha256=HiTGK8jS1B1msbQO5PmPKpn6OU_fEXNDwm-eKtPgmcI,1903
+lakehouse_engine/core/file_manager.py,sha256=btMA29eBMv62aANSuAQyY79OVrx6P_g7p4CdcflxNyk,2440
+lakehouse_engine/core/gab_manager.py,sha256=CTBCrnb8JWCEpNuQmMM8g4XJ141N2J7vLQdSXXLBa8E,32419
+lakehouse_engine/core/gab_sql_generator.py,sha256=QgEuNgh4JvXTjyhQfrvWvyjI0oGaIU1obuJOWvJy0F8,19747
 lakehouse_engine/core/s3_file_manager.py,sha256=o0B5hzLYpXWvt8-_cxEMQcbQawGIIeAD29vQt9ad9lA,21478
 lakehouse_engine/core/sensor_manager.py,sha256=dT0JUd1ioj-qPgFvbApMRLMm43G6o4nL2DpcAkvf8k4,13664
-lakehouse_engine/core/table_manager.py,sha256=VM95PNFIvPfm7lvs4SaG_m1b6HJ0UrXG27Hir2WM6gk,10171
+lakehouse_engine/core/table_manager.py,sha256=A-31m4EXmqnI_girGhsfcmeWL6JpW5LGeMamo6HkUIo,10571
 lakehouse_engine/dq_processors/__init__.py,sha256=Dgkruh3esEkE3F30e4UkmnLiXr3pM6_-VAsHfQhj3XE,82
 lakehouse_engine/dq_processors/assistant.py,sha256=s2puJjI-nZAe_6wDFjJN8gB2jaEuEmnBtsH8oSTmJk4,7265
-lakehouse_engine/dq_processors/dq_factory.py,sha256=FPRToumoYpaZqhcilyA3Lred6WF8VULSyV07CdDQy_4,23551
+lakehouse_engine/dq_processors/dq_factory.py,sha256=mCwMZdg5GC9Ix6VfaOnSCdQlUTypStXkKSRmefODl_s,26871
 lakehouse_engine/dq_processors/exceptions.py,sha256=5Q13A7XzX4KnIHIpAAbGeTUIEOPXGf5n3L8Tz8U_55s,302
 lakehouse_engine/dq_processors/validator.py,sha256=pZd-w0Daki1e2JUGl4OZYcNCuQ7CZbNh0doSLmG0Ngs,8904
 lakehouse_engine/dq_processors/custom_expectations/__init__.py,sha256=MhvDiMOJ77YVrx9xpAczZbQiB37AR-mQ-3uX8MwnwjY,83
 lakehouse_engine/dq_processors/custom_expectations/expect_column_pair_a_to_be_smaller_or_equal_than_b.py,sha256=912omTucNHdLmXFv8yFz13yN6oMFOpV0paKpb4tdGHc,7066
 lakehouse_engine/dq_processors/custom_expectations/expect_column_values_to_be_date_not_older_than.py,sha256=jqWOAUCpu6QykVbCXa3WzTWh4wLJVjdVOBdfbC8-ukM,7958
-lakehouse_engine/dq_processors/custom_expectations/expect_multicolumn_column_a_must_equal_b_or_c.py,sha256=SqITipGVeUAqCTKKAz44a6bXSs9bk5QlMFu4vG8T_DM,6647
+lakehouse_engine/dq_processors/custom_expectations/expect_multicolumn_column_a_must_equal_b_or_c.py,sha256=Tpy4yochamk7DJ1dacB1J8YrgXW3N4-KawhNoxPsYOA,6627
 lakehouse_engine/dq_processors/custom_expectations/expect_queried_column_agg_value_to_be.py,sha256=CydGLMz6gtFaRINzS16Fhy5c7usxCk3TU02NXnGstaU,14618
 lakehouse_engine/io/__init__.py,sha256=lBmTVI52wsaOh5YIWwsN_Iw7vHv-FnnX4Kcurs-bncU,85
 lakehouse_engine/io/exceptions.py,sha256=a6UGS1MvI0ckeEFp2NIOpla6Aq05SrEkQIuOM0DTRKU,687
 lakehouse_engine/io/reader.py,sha256=xbaL7GCfjxQ4ExZnXnHm6ORqi2MRZYKO1yllJ4ZNbjk,797
 lakehouse_engine/io/reader_factory.py,sha256=YIpR3sdkjCBrwlA0J1_y3Kwtn9ri4kxP5Z3kl1JgXu4,2285
 lakehouse_engine/io/writer.py,sha256=_5KkxjS1wQETdvlZGd85HP3wKX_pc-c-YZ62EpplPKw,4720
 lakehouse_engine/io/writer_factory.py,sha256=XdFPTPUn_-mTLz5NEcYLbstsL_bAS0ynLZsO1rBppFs,2885
@@ -42,15 +45,15 @@
 lakehouse_engine/io/readers/query_reader.py,sha256=-xSmpuH42TufnPGxjsx0aAeEF2ANRvd0posOJcQAyzg,734
 lakehouse_engine/io/readers/sap_b4_reader.py,sha256=RmyVZxl8OkJhgJ2W1MdN3tXLdQ13kF2R2fET5_El3xU,7205
 lakehouse_engine/io/readers/sap_bw_reader.py,sha256=H2YtIbDXAHZ8SnEvQ1UGX5XuoFIaAsE89NUhtcMkT94,7299
 lakehouse_engine/io/readers/sftp_reader.py,sha256=IqYrmG7IICLpzxZWYlRxG9hBiHJKngBd9dJ6gXFdBXU,5445
 lakehouse_engine/io/readers/table_reader.py,sha256=IVnJ98a7xlmpjJ--cQ2XAoG6QXntlWa6DwZfRvn0Wuk,1300
 lakehouse_engine/io/writers/__init__.py,sha256=wQhLOlOrUIZthbiOwEI2fftjED21eVoxqAh_kQ7owJs,67
 lakehouse_engine/io/writers/console_writer.py,sha256=hOCXJg194NIx28ppJg1X2I60A7i3jStRV3apbM1rgiE,4361
-lakehouse_engine/io/writers/dataframe_writer.py,sha256=C5t9hVoGxxBYgEkkMNJjgrNrG4XcDxqNyA9GznPduZw,7476
+lakehouse_engine/io/writers/dataframe_writer.py,sha256=EMv1Atzdm0R2D-R4MbzXfMjBkC8atGnsGK_0zun06DY,7516
 lakehouse_engine/io/writers/delta_merge_writer.py,sha256=TExZI0Sg0jEjcWG6PPPZaMC5ODrqxlL4RkKB8APCSsQ,7752
 lakehouse_engine/io/writers/file_writer.py,sha256=53d5UOgU1d18DhXXHGackUgDui-1Y1xDgbsIdOL3twg,3888
 lakehouse_engine/io/writers/jdbc_writer.py,sha256=AhKAsUTaIiwUrh1x0cjSArb0dEnVgKJ6ozAutKqYEOg,3074
 lakehouse_engine/io/writers/kafka_writer.py,sha256=H9nHcW0TKid7w60TMRQSh7lpuMVXr0hZMXmPNaYj6Ig,3679
 lakehouse_engine/io/writers/table_writer.py,sha256=3ruMkFP3yuG1tOkEZRuVaQPC_LSJJ0ymdT7Ob64QXaU,5820
 lakehouse_engine/terminators/__init__.py,sha256=hUS_kq0qIOwoV0zpKYy700CWc0bA_5BafZ8Lm8PvN34,87
 lakehouse_engine/terminators/cdf_processor.py,sha256=0zRvCNR7P2Z8y2v51xjQn4xK4JTP7v6oOdDW1vrBSos,4557
@@ -62,15 +65,15 @@
 lakehouse_engine/terminators/terminator_factory.py,sha256=5mn21smu5MJZ9DB0QUlIf2XgtgDfFOONey-kjVKAfv8,1990
 lakehouse_engine/terminators/notifiers/__init__.py,sha256=50B5KJmkZADsBJEAFnN8r55mEq4jglmN62eKePZoGTE,28
 lakehouse_engine/terminators/notifiers/email_notifier.py,sha256=zCvcNUN-ru62GRoI5xEdTSvlfT1URmIuKSxgkv-MoEI,6683
 lakehouse_engine/terminators/notifiers/notification_templates.py,sha256=N8HZUzaA_-6hV5Iv2kpy1m7qdSensWZJWbZ3k9UKBDU,1494
 lakehouse_engine/transformers/__init__.py,sha256=G_fSJ-ZOknDj7mbVJx-ULzzxs4zkrOENUKvjSQR--jI,72
 lakehouse_engine/transformers/aggregators.py,sha256=Wf7ivHGaXSM86lr8Aiu0aKb4KrVh0NbpnKLnQ_8LJR8,895
 lakehouse_engine/transformers/column_creators.py,sha256=IXNOgZUI-4cvQ_rabKYoEG6_cGTyytXXLhyssAahCCY,3325
-lakehouse_engine/transformers/column_reshapers.py,sha256=BrDMTs2ihC1fgnj7U203P0L9I7JepdprnXh1kGeK06U,15223
+lakehouse_engine/transformers/column_reshapers.py,sha256=wl3-lvpp-hOAinwpoohbBGXBHOVley4LyiPDGj3Pusw,15361
 lakehouse_engine/transformers/condensers.py,sha256=k7fiuBaIMKmZRH3akHsLxGyVqHqH_i69FlbSb8hMJL8,4866
 lakehouse_engine/transformers/custom_transformers.py,sha256=sC9XWV9kYXFjvQHS0REfD9DjIMOHk0d6r-lD931W0vU,1260
 lakehouse_engine/transformers/data_maskers.py,sha256=HBqU9sn3Q5odPVTBofQoz9BVnHEya4mV6HJ2N-uBm8I,2168
 lakehouse_engine/transformers/date_transformers.py,sha256=NlpxGc-Ug2nowdIjY70GJRzhzoKJPktj0bipKCtSrY4,5331
 lakehouse_engine/transformers/exceptions.py,sha256=C-voRlbcDds7V3Qk07XPlGdX_9y1AOj3ZciIoB0iHV0,341
 lakehouse_engine/transformers/filters.py,sha256=BzGwXBhrG2auccEnGgbWk5WMWf3FD-4DluFYUe-qL5E,6359
 lakehouse_engine/transformers/joiners.py,sha256=LhriYZNlG8aD4wvea-HNIFOZRa9B3vxqfxBbe-jFxkI,3624
@@ -79,34 +82,35 @@
 lakehouse_engine/transformers/regex_transformers.py,sha256=zgrGsWEWHBHByXy93rVfSzbwfo-2y1QQ0nnbTSzhxaQ,1240
 lakehouse_engine/transformers/repartitioners.py,sha256=Xw50sSiL8uX_hOopH0ldR4vJdQ5GdckFREyu_KZ5GQk,1817
 lakehouse_engine/transformers/transformer_factory.py,sha256=Be6dZfOPwZvrLZsH6OZ8GX92Cd1pQ6TSnJlbIguQXR8,5889
 lakehouse_engine/transformers/unions.py,sha256=eRzscQzlIXqdX5hs2ZsCQQ7rGC4YvM9f57g8ZVRGyH4,1956
 lakehouse_engine/transformers/watermarker.py,sha256=RGwS3zRGc3p57qsqks4gx8gxnUUxmvL5UMo6BxK74vU,918
 lakehouse_engine/utils/__init__.py,sha256=ghksXfMwMaYno0t9ZZ5dGf9R49_IfwhT5BHXiUVVU6A,25
 lakehouse_engine/utils/databricks_utils.py,sha256=Y8G8KuU2SQeFaw0tMttpumEK6HC-7WrWYxaGGhqypGE,1636
-lakehouse_engine/utils/engine_usage_stats.py,sha256=6z6uEOi2kG49NGHXMiZT9PeXmv8AB1Pvr1lrEV6Jsc8,4950
+lakehouse_engine/utils/engine_usage_stats.py,sha256=K6ZkO-IuBMhEKANIC6PDDp6PR_1pXhpXWRl9AHnQiSI,5632
 lakehouse_engine/utils/expectations_utils.py,sha256=CmYgJJ9HF8o-S8bPtRp3zaPpq3CS30zDeWRp8w9b5y0,4691
 lakehouse_engine/utils/file_utils.py,sha256=J-x3NIH3RbtxbSV-sRq37iHR7Fw_5mCs_snpME0X2sY,1079
+lakehouse_engine/utils/gab_utils.py,sha256=7JgAJ4Qi5DRvQ98vM0uAwkgnWSJ03v5cMU1NwM8DhqQ,22848
 lakehouse_engine/utils/logging_handler.py,sha256=gG1ipddbZwm1OxkWGwZDDpGX67nrdwEvDDUqSM-50Bg,2864
-lakehouse_engine/utils/schema_utils.py,sha256=M31Fri7H5Y2b78LtKc4jqbr38SuYnTqRRSzWPKVvj2I,6594
+lakehouse_engine/utils/schema_utils.py,sha256=Y0r0znyrQ38MR0V0IZ5ImCRJsZjTlNmhHnq1fYDN7LM,6935
 lakehouse_engine/utils/sql_parser_utils.py,sha256=b1BbnXvYcXa4NVEA9XsQWWxe0IVe7fh1FGXmYjzcDWk,7327
 lakehouse_engine/utils/configs/__init__.py,sha256=ZppvpKhFNhT7B949O63K7mZWHphDuOlOztsx4lLw7OM,32
-lakehouse_engine/utils/configs/config_utils.py,sha256=6x44ohk-OGWxg8qFqi2h9C6__OZrSReq5NnDrcJZrvI,3444
+lakehouse_engine/utils/configs/config_utils.py,sha256=2QdgTf1JrXMxceShLLEBhbBhWoAkW1Czx2UNaoPrbZI,3866
 lakehouse_engine/utils/extraction/__init__.py,sha256=14GeiFc3DNmAIaaI6OZDZIH43YIPRguSfpG0unAgb3c,36
 lakehouse_engine/utils/extraction/jdbc_extraction_utils.py,sha256=p5LH6e_qombeM3-mb1PNkDsATNJ9y5kugRhc-gTQ5X0,15419
 lakehouse_engine/utils/extraction/sap_b4_extraction_utils.py,sha256=GIUguZuSfJNLwVwsgivKRouA1Z7SGJLdUlzXeaw2tt4,11821
 lakehouse_engine/utils/extraction/sap_bw_extraction_utils.py,sha256=oeJKUyYxduLbhDK7PjMSkS_3la72PxJnz9Os9fYNV2o,14221
 lakehouse_engine/utils/extraction/sftp_extraction_utils.py,sha256=1z0qP2h7oArBFWHd5e7FuX25RLPIPlevDQsmX7LjEsc,18533
 lakehouse_engine/utils/storage/__init__.py,sha256=Pw5_47oC5ywPpfo1U6djLYeTPnm4D9IbIuL_vxHLpi8,50
-lakehouse_engine/utils/storage/dbfs_storage.py,sha256=ukDyDxy-u4d5aXqhXSmiXQ7yGFmADfq1Gi0N-_tZPs4,1473
+lakehouse_engine/utils/storage/dbfs_storage.py,sha256=Lf8HjUjVYj5Oyog1liOA2ImX0hxZaXrNfLh6NkHBZKc,1525
 lakehouse_engine/utils/storage/file_storage.py,sha256=NZk3fNIF1tPzclmsjOwv0NAUa7EovuIDoJxJ6TaMrZo,774
-lakehouse_engine/utils/storage/file_storage_functions.py,sha256=Fah_wADDiGtT6xPabdICM5rXojDATolfREzDkC_VkhA,3232
+lakehouse_engine/utils/storage/file_storage_functions.py,sha256=qR-3_ajPJPGhazlUTj5-8OMNl7pJ4YfcnBJ7XptLDdo,4212
 lakehouse_engine/utils/storage/local_fs_storage.py,sha256=1Z3loLKV5w0POeiw3LDTKxkAjAJJgwgwBHaNQ0jL0YI,1280
-lakehouse_engine/utils/storage/s3_storage.py,sha256=WyWS21EoGRUyq7zbx0HJ7K3714J95o6rL23liJghNMI,1298
-lakehouse_engine-1.19.0.data/data/requirements/requirements_os.lock,sha256=nAW_2w3OaEJaOIhAJjXzduGs0IpiEgnwtVvZCEWrV5w,12260
+lakehouse_engine/utils/storage/s3_storage.py,sha256=gh7xI7PXCPxgwMD-FfqXpKMFFCPAnSfLVGpU79okzEg,1422
+lakehouse_engine-1.20.0.data/data/requirements/requirements_os.lock,sha256=uFX1Zu-18_EFOmS3PIND5P6JiqvdzTqHliiM1GtgXYk,12351
 lakehouse_engine_usage/__init__.py,sha256=cpUdXUuZ2vL1Z_gAWtqBDSPbFIoKPZhFpicct0ujiHA,356
 lakehouse_engine_usage/data_loader/__init__.py,sha256=ves-R-ByBDABs7O9u1ee3jraMhxG9hIwLVVjDgSvJC8,35
 lakehouse_engine_usage/data_loader/append_load_from_jdbc_with_permissive_mode/__init__.py,sha256=OBYnOld9RxB_glxVZUihoPVY030wyKsixZXxqGFiA8I,65
 lakehouse_engine_usage/data_loader/append_load_with_failfast/__init__.py,sha256=k7QceuiqU-1XYOzNXK2NFgMGzkyK9_Qbc2sGanWytSE,48
 lakehouse_engine_usage/data_loader/batch_delta_load_init_delta_backfill_with_merge/__init__.py,sha256=KXNHTcb7eq5VXjjTsAI8sW75KVCsfRcdOqZkOCgN9zQ,70
 lakehouse_engine_usage/data_loader/custom_transformer/__init__.py,sha256=koaapHPS_IZo5V4HNfjvSA_F9ZWESL12DPt2NbVUH4Y,42
 lakehouse_engine_usage/data_loader/extract_from_sap_b4_adso/__init__.py,sha256=yFdkvig301fTmvTGhkFLTfv6u5s55YuCvc8DsHX0hFs,48
@@ -141,35 +145,36 @@
 lakehouse_engine_usage/sensor/sap_bw_b4/__init__.py,sha256=NlDtkwOqMyme4it9TgUVDnGcUU2a4GHjFPXakwfnl2g,33
 lakehouse_engine_usage/sensor/update_sensor_status/__init__.py,sha256=f7A7BWu_RgCkYly5WETjzufoTIUO9GAXskx2H0Z5B-Q,44
 tests/__init__.py,sha256=xqsJPT1QR2TH_5GYK8tiHp-Lb29chxGsr147MWoLAZw,21
 tests/conftest.py,sha256=aIdKAmYDbXTJleI_-NpZcw5lLSeUN-lUtRI9EtlDYLo,1968
 tests/configs/__init__.py,sha256=9CXMq3gm_ebjcm9aE-Iy9Nfh-B9Ot07RlNIJGgQtrUs,54
 tests/feature/__init__.py,sha256=2D7R0mr8_VM5g5Dmtg1Y0YQ_My3udCkL3PdEDBcaJfg,89
 tests/feature/test_append_load.py,sha256=dBBY6RDbE1aly0w86Pwyep7zynBlONiIMfMVZaBpYWk,6329
-tests/feature/test_data_quality.py,sha256=ixTYAnTaf09MPyaxpt1OP-9w_F1IrWfUthdAPYshnmA,22498
+tests/feature/test_data_quality.py,sha256=_fGaCM25f15wFoLuYNf_wXiBqqcykRIPgnCM290ca58,26259
 tests/feature/test_dq_validator.py,sha256=dNA0eos9MsbngxdvNEIice_0H0ZdIeSxd1oWPBI8Sjg,17643
-tests/feature/test_engine_usage_stats.py,sha256=RAwffWfwz-Z_x-mLEQFYuHR27uN8wVn5vEhTzG79am0,7928
+tests/feature/test_engine_usage_stats.py,sha256=XrYHqoavOx1pa6hB4xsvsj3pK5hC4Mck3MJRhEw1xO0,7943
 tests/feature/test_extract_from_sap_b4.py,sha256=mCeuR13uPHV_eluzY6ScKci2hypHNmKXFiub1Mp928k,17735
 tests/feature/test_extract_from_sap_bw.py,sha256=XU-t07gjGPP-WSYyHDUjemBicFzemzVakTWdIOAABJE,23508
 tests/feature/test_file_manager.py,sha256=fzBJUR1sQ0_dUp7s3CpWFQaXUw09RuTgxZ86_-S6Xtg,10590
 tests/feature/test_file_manager_dbfs.py,sha256=cFK_jKGEZUXEQXGtL3M-RFie3gADx_WrJ3DVYjNe-e0,9124
 tests/feature/test_file_manager_s3.py,sha256=Jh3QTs537vs1tsbUkAuTtlzmsJ1BQGckobGocGXzUlQ,11234
 tests/feature/test_full_load.py,sha256=LJUA5chULgOV9M_M86TrbTyW6jkdTyfUEyqk1pT_JgE,2499
+tests/feature/test_gab.py,sha256=zwFT8FRy5sso1BseBqGR_8JOoMBZk7NwiOxeJtq21Ik,13799
 tests/feature/test_jdbc_reader.py,sha256=_um1taKAOotI42ph2sGlx-N6Qqkz6K-4bcgI7mnc-dA,4573
 tests/feature/test_materialize_cdf.py,sha256=wiphaQaQYhTNKJNEiFT1CcIFPHUjli2m8Y467O7jKnI,4116
 tests/feature/test_notification.py,sha256=IRv8Rnl0GZyd_PLdCzE0OC2VXFOH8zUx574hEIFdOOo,16028
 tests/feature/test_reconciliation.py,sha256=RQgosAuRKHFSpcET-2gA3VAvmJRiKFJsuFzzJFeipXQ,14219
 tests/feature/test_schema_evolution.py,sha256=Dlj-MyZ-a4pJXQIngGHJqdOHf5pNnnf144B2IlOXW_g,20111
 tests/feature/test_sensors.py,sha256=FS3_xh4wIx2s2Xc5j4GwmQTPKrkfTCglk-XvPDH61SY,16396
 tests/feature/test_sftp_reader.py,sha256=HyfqTBc2rksicPExfPnFG4_ZTWwigY52hzbrQ9n2yyw,19193
 tests/feature/test_table_manager.py,sha256=p8xC1cq0HDnsJzpjfrUg0f1iC1QHCIbSngzmuBQMQ3U,9422
 tests/feature/test_writers.py,sha256=0y3tUqnhS2P65B5ZOYwdY0uTFa3IdipsA5LO0dMJBsE,14023
 tests/feature/custom_expectations/__init__.py,sha256=VVFbYWc7AIDndDqeiqq6QSOEsVFA7WolgcIS4SOQfk4,64
 tests/feature/custom_expectations/test_custom_expectations.py,sha256=_JayetKRgMzDLomwv7Op15jTouYPMxCwWtw1mPTgrXg,9212
-tests/feature/custom_expectations/test_expectation_validity.py,sha256=VoeylfgbK1uJaCChCXoFZZdI3nOfaxSKVIwrIwce6gI,3823
+tests/feature/custom_expectations/test_expectation_validity.py,sha256=QbhbSrudI3XePfBw1FpzhCjU_IxbdoAaSLeg2y45Q5U,3850
 tests/feature/data_loader_custom_transformer/__init__.py,sha256=cfzl2Nsa14EH5zo6Jw732gG7dIFoUHf-iwdRnFTp5zk,89
 tests/feature/data_loader_custom_transformer/test_data_loader_custom_transformer_calculate_kpi.py,sha256=KYCRiDeK1IPGuJWlgKgV5HiDdYUhGRw0Sefki2XmFU4,4060
 tests/feature/data_loader_custom_transformer/test_data_loader_custom_transformer_delta_load.py,sha256=O0epYvdNbFDfrTx1Obl6__-vvVbs0vJVwneQehIclrU,7613
 tests/feature/delta_load/__init__.py,sha256=AIHHVMIyr7WXAOjPTa0oSjVQNAW63cvmM0Qzg4ZOjnE,32
 tests/feature/delta_load/test_delta_load_group_and_rank.py,sha256=1HJZi0dBFdrjR8lhym7N_48wIRcW1pGayIzHO_2MO8U,5343
 tests/feature/delta_load/test_delta_load_merge_options.py,sha256=HSPwmBljY2t7a-ccQ9sGF-3_uFrfhkdrdYc9uFcUAaY,3481
 tests/feature/delta_load/test_delta_load_record_mode_cdc.py,sha256=ZFSXGM8Q5MxiTEedLaYUNfVaXqOhxPi44Pbx2l1QgU8,9547
@@ -187,12 +192,12 @@
 tests/feature/transformations/test_regex_transformers.py,sha256=CHd36rg-rtFJPco8Bj61524ztoJ2Ya3ge3UUfbBej3U,1996
 tests/feature/transformations/test_unions.py,sha256=AGjDOH_qPE2a3irvw9RsGwYBM3igbUl5xSjP7QIicKo,4981
 tests/feature/transformations/test_watermarker.py,sha256=3d391-D2VzC0bi_06h23KqHW5Pzr_pEgaNcAZpkXmC8,6275
 tests/utils/__init__.py,sha256=nUnqAIcMWyNNDRX30xRT754S9qPlhiY0mcwfrwMY-uA,23
 tests/utils/dataframe_helpers.py,sha256=PWG2gKBh7XtQI9JzAmyPBqnknnnVOz0JzCmXLw5-2gM,6959
 tests/utils/exec_env_helpers.py,sha256=bb30NzLRXUI2pXdQ0W3PqiSJCVBuAdCsXsGZZz1drS4,1960
 tests/utils/local_storage.py,sha256=Wc9xDuXbWjpFZL-DNNFHg9naWDpBi13c80FWxJLO3UI,1513
-lakehouse_engine-1.19.0.dist-info/LICENSE.txt,sha256=gwVdeUQ_58ZvOu-89Kpkea4u5R0o2Op9Z64yowWgyvw,11339
-lakehouse_engine-1.19.0.dist-info/METADATA,sha256=9Ap_lOa7vXcfJpwmGsIF927PS6TWK3U0Jrv8bDTrxPw,24843
-lakehouse_engine-1.19.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-lakehouse_engine-1.19.0.dist-info/top_level.txt,sha256=GlWVGoEAFp0EcxYphWf0KrVIu6xS7Qg3FvImZii9l1M,46
-lakehouse_engine-1.19.0.dist-info/RECORD,,
+lakehouse_engine-1.20.0.dist-info/LICENSE.txt,sha256=gwVdeUQ_58ZvOu-89Kpkea4u5R0o2Op9Z64yowWgyvw,11339
+lakehouse_engine-1.20.0.dist-info/METADATA,sha256=MbWyRWvtis4YaWW9ElfURmseOTKGrhq1Cp7n0ifEIS4,24847
+lakehouse_engine-1.20.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+lakehouse_engine-1.20.0.dist-info/top_level.txt,sha256=GlWVGoEAFp0EcxYphWf0KrVIu6xS7Qg3FvImZii9l1M,46
+lakehouse_engine-1.20.0.dist-info/RECORD,,
```

