# Comparing `tmp/rime_sdk-2.8.0rc8.tar.gz` & `tmp/rime_sdk-2.8.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rime_sdk-2.8.0rc8.tar", last modified: Wed Apr 24 08:24:13 2024, max compression
+gzip compressed data, was "rime_sdk-2.8.0rc9.tar", last modified: Tue Apr 30 16:46:52 2024, max compression
```

## Comparing `rime_sdk-2.8.0rc8.tar` & `rime_sdk-2.8.0rc9.tar`

### file list

```diff
@@ -1,600 +1,608 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-24 08:24:13.656007 rime_sdk-2.8.0rc8/
--rw-r--r--   0 runner    (1001) runner    (1001)      566 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/LICENSE
--rw-r--r--   0 runner    (1001) runner    (1001)     1275 2024-04-24 08:24:13.656007 rime_sdk-2.8.0rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      984 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/README.md
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-24 08:24:13.620007 rime_sdk-2.8.0rc8/rime_sdk/
--rw-r--r--   0 runner    (1001) runner    (1001)     1490 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2268 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/authenticator.py
--rw-r--r--   0 runner    (1001) runner    (1001)    71496 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/client.py
--rw-r--r--   0 runner    (1001) runner    (1001)    23353 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/continuous_test.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12282 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/data_collector.py
--rw-r--r--   0 runner    (1001) runner    (1001)      883 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/detection_event.py
--rw-r--r--   0 runner    (1001) runner    (1001)    25623 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/generative_firewall.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3437 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/generative_model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4892 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/image_builder.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-24 08:24:13.620007 rime_sdk-2.8.0rc8/rime_sdk/internal/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/internal/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18386 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/internal/config_parser.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1004 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/internal/constants.py
--rw-r--r--   0 runner    (1001) runner    (1001)      667 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/internal/decorators.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9740 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/internal/file_upload.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1973 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/internal/rest_error_handler.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9361 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/internal/swagger_parser.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2577 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/internal/swagger_utils.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1081 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/internal/test_helpers.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2681 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/internal/throttle_queue.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3570 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/internal/utils.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18764 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/job.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5042 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/monitor.py
--rw-r--r--   0 runner    (1001) runner    (1001)   107184 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/project.py
--rw-r--r--   0 runner    (1001) runner    (1001)    38328 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/registry.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4396 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/schedule.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-24 08:24:13.620007 rime_sdk-2.8.0rc8/rime_sdk/swagger/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-24 08:24:13.620007 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/
--rw-r--r--   0 runner    (1001) runner    (1001)    61236 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-24 08:24:13.620007 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/
--rw-r--r--   0 runner    (1001) runner    (1001)     2411 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)    60690 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5851 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/config_validator_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18207 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    25430 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/data_collector_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11733 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/detection_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    23108 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13964 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    27750 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/file_upload_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    24169 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/firewall_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    23796 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/firewall_instance_manager_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    22695 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    15676 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/generative_model_testing_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    28916 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/image_registry_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    27170 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/integration_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    27728 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/job_reader_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    21865 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18441 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/model_testing_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    35026 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    19932 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    74338 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/project_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    57883 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/registry_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    77856 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/results_reader_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4167 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/rime_info_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    18249 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/schedule_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    40655 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/user_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    25780 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/validation_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    46472 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
--rw-r--r--   0 runner    (1001) runner    (1001)    25179 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8845 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-24 08:24:13.652007 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/
--rw-r--r--   0 runner    (1001) runner    (1001)    58726 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4210 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4369 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3764 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/apigenerativefirewall_list_firewall_instances_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3366 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/apigenerativefirewall_standard_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4328 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6669 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5483 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5103 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3706 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3725 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3435 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8968 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3552 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4503 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3582 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2551 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6687 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
--rw-r--r--   0 runner    (1001) runner    (1001)    17329 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/crossplanetask_cross_plane_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3362 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8011 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4630 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2674 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2695 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7390 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4396 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3292 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6273 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13500 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8080 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4925 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5748 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2705 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5806 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)    14085 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8545 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3410 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)    15539 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4273 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2728 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/detection_event_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2587 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4205 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/detection_resolution.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7745 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2744 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2719 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2670 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4176 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10779 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10808 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_file_security_report.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7556 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_package_url.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7459 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3304 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata_license.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3285 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/fileserver_check_object_exists_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/fileserver_delete_object_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3294 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/fileserver_get_read_object_presigned_link_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3310 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/fileserver_get_upload_object_presigned_link_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3232 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/fileserver_list_objects_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9982 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5075 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3149 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10070 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5158 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7816 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/firewallinstance_firewall_instance_firewall_instance_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2822 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/flagged_substring_request_body_component.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4455 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generative_testing_result_example.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4502 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3679 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5387 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_custom_pii_entity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4675 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_denial_of_service_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2722 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7234 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2844 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5781 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3291 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2896 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_tokenizer.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6773 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_flagged_substring.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3517 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_effective_config_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3686 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_instance_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13926 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_individual_rules_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4144 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3934 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8681 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_off_topic_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4848 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4877 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3752 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_entity_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4895 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5039 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_v2_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2924 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_false_positive_rate.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11874 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2808 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_sensitivity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3447 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_detection_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3934 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5128 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_unknown_external_source_rule_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3869 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_update_firewall_instance_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5046 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7846 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)    14746 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3518 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result_standard_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2667 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5869 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4012 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativetesting_objective_sub_category.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10258 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3408 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3157 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativetesting_threat.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4422 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4103 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2821 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2770 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3403 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3206 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2808 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4550 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5064 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4774 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/job_data_generative_model_test.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3915 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/job_data_scan.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4710 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4752 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/language_detection_details_language_substring.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5481 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4426 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4187 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_file_scan_results_request_file_scan_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3771 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_firewall_instances_request_list_firewall_instances_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4033 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6007 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5102 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5050 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4570 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3633 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6549 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4842 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4373 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3722 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5728 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5076 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3993 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4508 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2674 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13223 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/model_model.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3523 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4142 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2745 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2515 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6262 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4125 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3518 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4963 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12705 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2665 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4511 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2667 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3520 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_transform.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2728 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4020 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5602 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3275 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9399 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/notification_notification.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2774 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2644 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/notification_object_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3594 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4781 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6823 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/pii_detection_details_flagged_entity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4341 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4384 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_activate_schedule_for_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2563 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11026 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3279 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2607 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_deactivate_schedule_for_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2547 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3288 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3190 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4530 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9270 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10554 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12754 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5306 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5738 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3739 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_owner_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)    19393 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_project.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2693 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_project_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5013 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2579 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4180 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_schedule_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3279 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2571 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4380 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4765 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2715 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/protobuf_any.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2574 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6648 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3375 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4050 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4143 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6599 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)    20609 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_params.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2624 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3454 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4688 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5621 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4998 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4224 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_metadata.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3453 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3654 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_open_ai_chat_completion_model_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4161 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5645 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2728 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13267 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3218 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5797 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/repo_metadata_reputation.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5037 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2753 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2559 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9297 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5337 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent_desired_state.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2745 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2606 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8524 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2775 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_attack_objective.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2519 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6159 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13366 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2860 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_config_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4337 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3505 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3389 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4997 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6566 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4077 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6407 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3976 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3303 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3478 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3486 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3314 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_agent_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4200 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7059 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3324 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6750 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3842 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3407 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3481 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4086 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3371 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7230 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3177 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5393 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_schedule_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3324 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_schedule_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5936 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3212 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7061 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3352 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2559 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2535 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2539 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2551 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3371 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2559 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2539 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_schedule_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2567 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5159 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_detailed_upgrade_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2563 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4600 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6332 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6606 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3344 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3130 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_float_list.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3469 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_generative_model_test_progress.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3160 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3462 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3357 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4523 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6063 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3231 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4115 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3631 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3396 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3501 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_file_scan_result_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3265 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3181 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3457 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3122 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3266 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3394 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3365 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3303 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5967 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6275 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3208 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8929 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3381 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3406 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3288 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8541 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4079 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_schedule_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3292 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8955 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4877 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_upgrade_for_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3110 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3147 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4256 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4226 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4316 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3284 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2519 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4368 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3108 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_int_list.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4063 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6446 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_data.py
--rw-r--r--   0 runner    (1001) runner    (1001)    14784 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2865 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2617 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_view.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2611 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_language.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2904 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2770 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5439 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2672 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4968 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4995 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3283 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4835 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11090 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5364 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4580 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5385 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5366 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_firewall_instances_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5847 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4070 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7152 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5064 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4682 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3431 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4796 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5011 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5555 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5033 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4139 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3335 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5758 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2535 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4727 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3583 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4904 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3855 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12972 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2701 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_managed_image_package_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2784 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3900 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_card.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3127 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_task.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4059 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4134 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3697 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_named_double.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2620 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_order.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4197 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3415 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4616 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4108 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3464 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_firewall_agent_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3623 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_firewall_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3320 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4337 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3678 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2575 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2535 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2567 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2691 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2666 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3126 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3976 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_search_spec.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2654 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_severity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5062 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3831 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3226 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5586 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3178 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3194 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5016 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3304 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4870 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3288 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5859 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3336 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3390 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4438 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2547 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3108 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_str_list.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3289 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2741 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3134 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3854 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4448 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_table_column.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2768 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5133 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2718 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9660 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3423 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4811 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2869 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2652 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3911 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2698 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_token_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3172 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_toxicity_threat_category.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5196 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3289 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3481 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3327 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3255 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3425 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3289 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_schedule_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2591 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_upgrade_status_for_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2567 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2523 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2531 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_upgrade_agent_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3156 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_upgrade_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4875 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5335 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_role.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3886 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6815 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3106 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_uuid.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7431 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_workspace.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7167 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7715 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2841 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4741 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4096 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/role_users_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4673 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3900 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3469 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata_model_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4098 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4401 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4797 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6378 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4295 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_activate_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4319 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_deactivate_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6026 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schedule_schedule.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6508 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schedules_schedule_schedule_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6690 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2948 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schemafilescanning_package_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5053 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4051 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5310 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6171 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schemaregistry_model_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4156 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2790 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3993 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2803 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4121 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4121 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4136 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7276 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6259 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4371 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4136 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4187 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10280 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6416 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
--rw-r--r--   0 runner    (1001) runner    (1001)    12809 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4278 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5610 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3485 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9333 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4444 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2764 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6759 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3436 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3799 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_category_results_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3538 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3641 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3358 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5680 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5790 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3496 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5835 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5553 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5086 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5530 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3520 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3382 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     6503 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
--rw-r--r--   0 runner    (1001) runner    (1001)    16800 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7005 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13296 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5304 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13655 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4663 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
--rw-r--r--   0 runner    (1001) runner    (1001)    19373 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11743 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4077 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3410 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/user_private_info.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2634 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/user_role.py
--rw-r--r--   0 runner    (1001) runner    (1001)     7844 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/user_user_detail.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3815 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4140 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4196 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8329 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4326 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13843 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py
--rw-r--r--   0 runner    (1001) runner    (1001)    11044 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
--rw-r--r--   0 runner    (1001) runner    (1001)    10263 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4396 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8198 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
--rw-r--r--   0 runner    (1001) runner    (1001)     8401 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5364 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5380 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body1.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4825 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/validate_request_input.py
--rw-r--r--   0 runner    (1001) runner    (1001)     3641 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/validate_request_output.py
--rw-r--r--   0 runner    (1001) runner    (1001)     9852 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/validate_response_processed_request.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5992 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/validate_response_product_metadata.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5905 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5093 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5189 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4338 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)     4533 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
--rw-r--r--   0 runner    (1001) runner    (1001)    13063 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/rest.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5257 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/test_batch.py
--rw-r--r--   0 runner    (1001) runner    (1001)    17414 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/rime_sdk/test_run.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-24 08:24:13.620007 rime_sdk-2.8.0rc8/rime_sdk.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     1275 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)    41491 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       80 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) runner    (1001)      161 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        9 2024-04-24 08:24:13.000000 rime_sdk-2.8.0rc8/rime_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-04-24 08:24:13.656007 rime_sdk-2.8.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) runner    (1001)     3903 2024-04-24 08:22:40.000000 rime_sdk-2.8.0rc8/setup.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 16:46:52.288008 rime_sdk-2.8.0rc9/
+-rw-r--r--   0 runner    (1001) runner    (1001)      566 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/LICENSE
+-rw-r--r--   0 runner    (1001) runner    (1001)     1275 2024-04-30 16:46:52.288008 rime_sdk-2.8.0rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      984 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/README.md
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 16:46:52.252008 rime_sdk-2.8.0rc9/rime_sdk/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1490 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2268 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/authenticator.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    71496 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/client.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    23353 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/continuous_test.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12282 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/data_collector.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      883 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/detection_event.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    25623 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/generative_firewall.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4118 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/generative_model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4892 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/image_builder.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 16:46:52.252008 rime_sdk-2.8.0rc9/rime_sdk/internal/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/internal/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18386 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/internal/config_parser.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1004 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/internal/constants.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      667 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/internal/decorators.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9740 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/internal/file_upload.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1973 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/internal/rest_error_handler.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9361 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/internal/swagger_parser.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2577 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/internal/swagger_utils.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1081 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/internal/test_helpers.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2681 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/internal/throttle_queue.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3570 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/internal/utils.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18764 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/job.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5042 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) runner    (1001)   107184 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    38328 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/registry.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4396 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/schedule.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 16:46:52.252008 rime_sdk-2.8.0rc9/rime_sdk/swagger/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 16:46:52.252008 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/
+-rw-r--r--   0 runner    (1001) runner    (1001)    62256 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 16:46:52.256008 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/
+-rw-r--r--   0 runner    (1001) runner    (1001)     2411 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    60690 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5851 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/config_validator_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18207 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    25430 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/data_collector_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11733 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/detection_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    23108 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13964 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    27750 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/file_upload_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    24169 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/firewall_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    23796 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/firewall_instance_manager_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    22695 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    15676 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/generative_model_testing_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    28916 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/image_registry_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    27170 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/integration_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    34866 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/job_reader_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    21865 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18441 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/model_testing_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    35026 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    19932 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    74338 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/project_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    57883 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/registry_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    77856 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/results_reader_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4167 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/rime_info_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    18249 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/schedule_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    41129 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/user_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    25780 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/validation_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    46472 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    25179 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8845 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 16:46:52.288008 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/
+-rw-r--r--   0 runner    (1001) runner    (1001)    59746 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4210 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4369 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3764 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/apigenerativefirewall_list_firewall_instances_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3366 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/apigenerativefirewall_standard_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4328 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6669 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5483 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4509 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/code_detection_details_code_substring.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5103 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3706 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3725 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3435 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8968 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3552 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4503 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3582 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2551 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6687 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    17329 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/crossplanetask_cross_plane_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3362 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8011 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4630 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2674 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2695 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7390 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4396 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3292 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6273 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13500 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8080 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4925 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5748 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2705 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5806 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    14085 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8545 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3410 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    15539 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4273 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2728 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/detection_event_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2587 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4205 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/detection_resolution.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7745 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2744 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2719 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2670 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4176 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10779 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10808 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_file_security_report.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7556 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_package_url.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7459 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3304 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata_license.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3285 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/fileserver_check_object_exists_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/fileserver_delete_object_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3294 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/fileserver_get_read_object_presigned_link_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3310 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/fileserver_get_upload_object_presigned_link_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3232 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/fileserver_list_objects_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9982 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5075 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3149 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10070 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5158 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8718 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/firewallinstance_firewall_instance_firewall_instance_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2822 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/flagged_substring_request_body_component.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4455 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generative_testing_result_example.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3958 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_code_detection_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4756 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_code_detection_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5360 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3679 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5387 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_custom_pii_entity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4675 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_denial_of_service_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2722 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3614 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_deployment_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8056 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2844 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5781 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3348 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2896 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_tokenizer.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6773 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_flagged_substring.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3517 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_effective_config_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3686 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_instance_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    14924 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_individual_rules_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4144 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3934 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8681 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_off_topic_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4848 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4877 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3752 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_entity_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4943 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5039 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_v2_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2924 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_false_positive_rate.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12978 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2808 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_sensitivity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3447 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_detection_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3934 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5128 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_unknown_external_source_rule_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3869 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_update_firewall_instance_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5046 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7846 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    14746 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3518 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result_standard_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2667 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7571 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4012 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativetesting_objective_sub_category.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12381 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3408 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3157 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativetesting_threat.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4422 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4103 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2821 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2770 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3403 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3253 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2808 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4550 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5064 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3915 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/job_data_scan.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4710 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4752 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/language_detection_details_language_substring.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5481 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3415 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_api_tokens_request_list_api_tokens_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4426 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4187 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_file_scan_results_request_file_scan_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3771 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_firewall_instances_request_list_firewall_instances_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4033 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6007 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5102 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5050 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4570 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3633 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6549 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4842 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4373 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3722 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5728 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5076 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3993 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4508 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2674 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13223 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/model_model.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3523 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4142 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2745 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2515 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6262 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4125 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3518 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4963 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12705 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2665 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4511 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2667 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3520 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_transform.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2728 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4020 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5602 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3275 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9399 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/notification_notification.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2774 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2644 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/notification_object_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3594 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4781 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6823 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/pii_detection_details_flagged_entity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4341 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4384 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_activate_schedule_for_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2563 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11026 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3279 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2607 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_deactivate_schedule_for_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2547 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3288 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3190 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4530 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9270 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10554 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12754 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5306 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5738 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3739 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_owner_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    19393 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_project.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2693 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_project_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5013 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2579 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4180 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_schedule_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3279 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2571 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4380 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4765 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2715 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/protobuf_any.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2574 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6648 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3375 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4050 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4143 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6599 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    20609 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_params.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2624 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3454 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4688 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5621 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4998 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4224 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_metadata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3453 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3654 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_open_ai_chat_completion_model_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4161 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5645 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2728 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13267 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3218 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5797 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/repo_metadata_reputation.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5037 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2753 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2559 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9297 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_agent.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5337 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_agent_desired_state.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2745 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2606 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_agent_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8524 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2775 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_attack_objective.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3077 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_attack_technique.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2519 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6159 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13366 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2860 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_config_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4337 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3505 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3389 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4997 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6566 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4077 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6407 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3976 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3303 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3478 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3486 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3314 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_firewall_agent_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4200 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_firewall_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7059 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3324 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6750 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3842 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3407 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3481 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4086 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3371 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7230 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3177 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5393 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_schedule_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3324 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_schedule_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5936 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3212 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7061 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3352 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2559 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2535 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2539 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2551 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3371 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2559 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2539 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_schedule_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2567 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5159 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_detailed_upgrade_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2563 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4600 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6332 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6606 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3344 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3130 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_float_list.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4301 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_generative_model_test_progress.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3160 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3462 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3357 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4523 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6063 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3231 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4115 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3631 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3396 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3501 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_file_scan_result_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3265 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3181 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3457 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3122 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3266 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3394 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3365 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3303 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5967 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6275 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3208 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8929 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3381 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3406 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3288 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8541 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4079 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_schedule_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3292 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8955 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4877 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_upgrade_for_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3110 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3147 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4256 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4226 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4316 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3284 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2519 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4368 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3108 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_int_list.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4063 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6458 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_job_data.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5467 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_job_data_generative_model_test.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    14784 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2865 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_job_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2617 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_job_view.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2611 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_language.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2904 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2770 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5439 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2672 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4968 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4995 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3283 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4835 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11090 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5364 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4580 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5385 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5366 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_firewall_instances_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5000 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_gai_test_job_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3848 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_gai_test_jobs_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5847 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4070 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7152 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5064 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4682 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3431 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4796 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5011 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5555 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5033 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4139 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3335 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5758 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2535 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4727 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3583 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4904 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3855 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12972 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2701 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_managed_image_package_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2784 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3900 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_model_card.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3127 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_model_task.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4059 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4134 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3697 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_named_double.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2620 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_order.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4197 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3415 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4616 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4108 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3464 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_firewall_agent_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3623 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_firewall_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3320 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4337 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3678 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2575 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2535 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2567 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2691 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2666 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3126 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3976 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_search_spec.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2527 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2654 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_severity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5062 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3831 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3226 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5586 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3178 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3194 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5016 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3304 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4870 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3288 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5859 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3336 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3390 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4438 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2547 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3108 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_str_list.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3289 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2741 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3134 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3854 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4448 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_table_column.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2768 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5133 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2718 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9660 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3423 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4811 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2869 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2652 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3911 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2747 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_token_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3172 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_toxicity_threat_category.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5196 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3289 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3481 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3327 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3255 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3425 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3289 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_schedule_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2591 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_upgrade_status_for_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2567 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2523 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2543 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2531 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_upgrade_agent_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3156 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_upgrade_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4875 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5335 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_user_role.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3886 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6815 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3106 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_uuid.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2555 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7431 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_workspace.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7167 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7715 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2841 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4741 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4096 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/role_users_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4673 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3900 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3469 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata_model_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4098 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4401 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4797 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6378 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4295 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_activate_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4319 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_deactivate_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6026 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schedule_schedule.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6508 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schedules_schedule_schedule_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6690 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2948 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schemafilescanning_package_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5053 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4051 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5310 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6171 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schemaregistry_model_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4156 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2790 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3993 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2803 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4121 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4121 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4136 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7276 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6259 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4371 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4136 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4187 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10280 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6416 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    12809 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4278 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5610 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3485 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9333 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4444 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2764 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6759 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3436 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3799 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_get_category_results_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3538 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3641 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3358 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5680 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5790 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3496 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5835 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5553 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5086 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5530 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3520 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3382 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     6503 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    16800 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7005 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13296 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5304 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13655 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4663 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    19373 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11743 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4077 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3410 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/user_private_info.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2634 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/user_role.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     7844 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/user_user_detail.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3815 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4140 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4196 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8329 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4326 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13843 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    11044 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    10263 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4396 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8198 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     8401 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5364 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5380 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body1.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4825 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/validate_request_input.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     3641 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/validate_request_output.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     9852 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/validate_response_processed_request.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5992 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/validate_response_product_metadata.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5905 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5093 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5189 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4338 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     4533 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    13063 2024-04-30 16:46:51.000000 rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/rest.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5257 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/test_batch.py
+-rw-r--r--   0 runner    (1001) runner    (1001)    17414 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/rime_sdk/test_run.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2024-04-30 16:46:52.252008 rime_sdk-2.8.0rc9/rime_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1275 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)    42151 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       80 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)      161 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        9 2024-04-30 16:46:52.000000 rime_sdk-2.8.0rc9/rime_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2024-04-30 16:46:52.288008 rime_sdk-2.8.0rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) runner    (1001)     3903 2024-04-30 16:44:54.000000 rime_sdk-2.8.0rc9/setup.py
```

### Comparing `rime_sdk-2.8.0rc8/LICENSE` & `rime_sdk-2.8.0rc9/LICENSE`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/PKG-INFO` & `rime_sdk-2.8.0rc9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime_sdk
-Version: 2.8.0rc8
+Version: 2.8.0rc9
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.8.0rc8/README.md` & `rime_sdk-2.8.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/__init__.py` & `rime_sdk-2.8.0rc9/rime_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/authenticator.py` & `rime_sdk-2.8.0rc9/rime_sdk/authenticator.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/client.py` & `rime_sdk-2.8.0rc9/rime_sdk/client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/continuous_test.py` & `rime_sdk-2.8.0rc9/rime_sdk/continuous_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/data_collector.py` & `rime_sdk-2.8.0rc9/rime_sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/detection_event.py` & `rime_sdk-2.8.0rc9/rime_sdk/detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/generative_firewall.py` & `rime_sdk-2.8.0rc9/rime_sdk/generative_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/generative_model.py` & `rime_sdk-2.8.0rc9/rime_sdk/generative_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from rime_sdk.swagger.swagger_client import (
     ApiClient,
     GenerativeModelTestingApi,
     GenerativetestingGenerativeTestingResult,
     GenerativetestingGetGenerativeModelTestResultsResponse,
     GenerativetestingStartGenerativeModelTestRequest,
     GenerativetestingStartGenerativeModelTestResponse,
+    RimeUUID,
 )
 
 
 class GenerativeModel:
     """The interface to the Generative Model Testing API."""
 
     def __init__(self, api_client: ApiClient):
@@ -27,33 +28,50 @@
     def start_test(
         self,
         url: str,
         endpoint_payload_template: str,
         response_json_path: str,
         http_headers: Optional[dict] = None,
         name: Optional[str] = None,
+        http_auth_integration_id: Optional[str] = None,
+        mutual_tls_integration_id: Optional[str] = None,
     ) -> GenerativeModelTestJob:
         """Start a Generative Model Test.
 
         Args:
             url: The URL to test.
             http_headers: The HTTP headers to use.
             endpoint_payload_template: The endpoint payload template to use.
             response_json_path: The response JSON path to use.
             name: A name to identify your generative test run.
+            http_auth_integration_id: The HTTP Auth Integration ID.
+            mutual_tls_integration_id: The Mutual TLS Integration ID.
 
         Returns:
             GenerativeModelTestJob: The Generative Model Test Job.
         """
+        http_auth_uuid = (
+            RimeUUID(http_auth_integration_id)
+            if http_auth_integration_id is not None
+            else None
+        )
+        mtls_uuid = (
+            RimeUUID(mutual_tls_integration_id)
+            if mutual_tls_integration_id is not None
+            else None
+        )
+
         request = GenerativetestingStartGenerativeModelTestRequest(
             url=url,
             http_headers=http_headers,
             endpoint_payload_template=endpoint_payload_template,
             response_json_path=response_json_path,
             name=name,
+            http_auth_integration_id=http_auth_uuid,
+            mutual_tls_integration_id=mtls_uuid,
         )
         with RESTErrorHandler():
             res: GenerativetestingStartGenerativeModelTestResponse = (
                 GenerativeModelTestingApi(
                     self._api_client
                 ).generative_model_testing_start_generative_model_test(body=request)
             )
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/image_builder.py` & `rime_sdk-2.8.0rc9/rime_sdk/image_builder.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/internal/config_parser.py` & `rime_sdk-2.8.0rc9/rime_sdk/internal/config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/internal/constants.py` & `rime_sdk-2.8.0rc9/rime_sdk/internal/constants.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/internal/decorators.py` & `rime_sdk-2.8.0rc9/rime_sdk/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/internal/file_upload.py` & `rime_sdk-2.8.0rc9/rime_sdk/internal/file_upload.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/internal/rest_error_handler.py` & `rime_sdk-2.8.0rc9/rime_sdk/internal/rest_error_handler.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/internal/swagger_parser.py` & `rime_sdk-2.8.0rc9/rime_sdk/internal/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/internal/swagger_utils.py` & `rime_sdk-2.8.0rc9/rime_sdk/internal/swagger_utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/internal/test_helpers.py` & `rime_sdk-2.8.0rc9/rime_sdk/internal/test_helpers.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/internal/throttle_queue.py` & `rime_sdk-2.8.0rc9/rime_sdk/internal/throttle_queue.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/internal/utils.py` & `rime_sdk-2.8.0rc9/rime_sdk/internal/utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/job.py` & `rime_sdk-2.8.0rc9/rime_sdk/job.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/monitor.py` & `rime_sdk-2.8.0rc9/rime_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/project.py` & `rime_sdk-2.8.0rc9/rime_sdk/project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/registry.py` & `rime_sdk-2.8.0rc9/rime_sdk/registry.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/schedule.py` & `rime_sdk-2.8.0rc9/rime_sdk/schedule.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/__init__.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 from rime_sdk.swagger.swagger_client.models.agent_id_uuid_upgrade_body import AgentIdUuidUpgradeBody
 from rime_sdk.swagger.swagger_client.models.agent_id_uuid_upgrade_body1 import AgentIdUuidUpgradeBody1
 from rime_sdk.swagger.swagger_client.models.apigenerativefirewall_list_firewall_instances_response import ApigenerativefirewallListFirewallInstancesResponse
 from rime_sdk.swagger.swagger_client.models.apigenerativefirewall_standard_info import ApigenerativefirewallStandardInfo
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_category_test_identifier import ArtifactIdentifierCategoryTestIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_subset_test_metric_identifier import ArtifactIdentifierSubsetTestMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_test_case_metric_identifier import ArtifactIdentifierTestCaseMetricIdentifier
+from rime_sdk.swagger.swagger_client.models.code_detection_details_code_substring import CodeDetectionDetailsCodeSubstring
 from rime_sdk.swagger.swagger_client.models.config_generation_category_config_generation_service_response import ConfigGenerationCategoryConfigGenerationServiceResponse
 from rime_sdk.swagger.swagger_client.models.config_generation_profiling_config_generation_service_response import ConfigGenerationProfilingConfigGenerationServiceResponse
 from rime_sdk.swagger.swagger_client.models.config_generation_test_suite_config_generation_service_response import ConfigGenerationTestSuiteConfigGenerationServiceResponse
 from rime_sdk.swagger.swagger_client.models.configvalidator_config_type_body import ConfigvalidatorConfigTypeBody
 from rime_sdk.swagger.swagger_client.models.continuoustests_firewall_id_uuid_body import ContinuoustestsFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.create_agent_request_aws_config import CreateAgentRequestAWSConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_azure_config import CreateAgentRequestAzureConfig
@@ -106,19 +107,22 @@
 from rime_sdk.swagger.swagger_client.models.firewall_firewall_firewall_id_uuid_body import FirewallFirewallFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.firewall_latest_run_info import FirewallLatestRunInfo
 from rime_sdk.swagger.swagger_client.models.firewall_scheduled_ct_info import FirewallScheduledCTInfo
 from rime_sdk.swagger.swagger_client.models.firewall_test_category_severity import FirewallTestCategorySeverity
 from rime_sdk.swagger.swagger_client.models.firewallinstance_firewall_instance_firewall_instance_id_uuid_body import FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody
 from rime_sdk.swagger.swagger_client.models.flagged_substring_request_body_component import FlaggedSubstringRequestBodyComponent
 from rime_sdk.swagger.swagger_client.models.generative_testing_result_example import GenerativeTestingResultExample
+from rime_sdk.swagger.swagger_client.models.generativefirewall_code_detection_details import GenerativefirewallCodeDetectionDetails
+from rime_sdk.swagger.swagger_client.models.generativefirewall_code_detection_rule_config import GenerativefirewallCodeDetectionRuleConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_create_firewall_instance_request import GenerativefirewallCreateFirewallInstanceRequest
 from rime_sdk.swagger.swagger_client.models.generativefirewall_create_firewall_instance_response import GenerativefirewallCreateFirewallInstanceResponse
 from rime_sdk.swagger.swagger_client.models.generativefirewall_custom_pii_entity import GenerativefirewallCustomPiiEntity
 from rime_sdk.swagger.swagger_client.models.generativefirewall_denial_of_service_rule_config import GenerativefirewallDenialOfServiceRuleConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_action import GenerativefirewallFirewallAction
+from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_instance_deployment_config import GenerativefirewallFirewallInstanceDeploymentConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_instance_info import GenerativefirewallFirewallInstanceInfo
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_instance_status import GenerativefirewallFirewallInstanceStatus
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_rule_config import GenerativefirewallFirewallRuleConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_rule_type import GenerativefirewallFirewallRuleType
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_tokenizer import GenerativefirewallFirewallTokenizer
 from rime_sdk.swagger.swagger_client.models.generativefirewall_flagged_substring import GenerativefirewallFlaggedSubstring
 from rime_sdk.swagger.swagger_client.models.generativefirewall_get_firewall_effective_config_response import GenerativefirewallGetFirewallEffectiveConfigResponse
@@ -154,18 +158,18 @@
 from rime_sdk.swagger.swagger_client.models.image_reference_reference_type import ImageReferenceReferenceType
 from rime_sdk.swagger.swagger_client.models.integration_integration_level import IntegrationIntegrationLevel
 from rime_sdk.swagger.swagger_client.models.integration_integration_schema import IntegrationIntegrationSchema
 from rime_sdk.swagger.swagger_client.models.integration_integration_type import IntegrationIntegrationType
 from rime_sdk.swagger.swagger_client.models.integration_variable_sensitivity import IntegrationVariableSensitivity
 from rime_sdk.swagger.swagger_client.models.integrations_integration_id_uuid_body import IntegrationsIntegrationIdUuidBody
 from rime_sdk.swagger.swagger_client.models.job_data_continuous_incremental_test import JobDataContinuousIncrementalTest
-from rime_sdk.swagger.swagger_client.models.job_data_generative_model_test import JobDataGenerativeModelTest
 from rime_sdk.swagger.swagger_client.models.job_data_scan import JobDataScan
 from rime_sdk.swagger.swagger_client.models.job_data_stress_test import JobDataStressTest
 from rime_sdk.swagger.swagger_client.models.language_detection_details_language_substring import LanguageDetectionDetailsLanguageSubstring
+from rime_sdk.swagger.swagger_client.models.list_api_tokens_request_list_api_tokens_query import ListAPITokensRequestListAPITokensQuery
 from rime_sdk.swagger.swagger_client.models.list_agents_request_list_agents_query import ListAgentsRequestListAgentsQuery
 from rime_sdk.swagger.swagger_client.models.list_datasets_request_datasets_query import ListDatasetsRequestDatasetsQuery
 from rime_sdk.swagger.swagger_client.models.list_file_scan_results_request_file_scan_query import ListFileScanResultsRequestFileScanQuery
 from rime_sdk.swagger.swagger_client.models.list_firewall_instances_request_list_firewall_instances_query import ListFirewallInstancesRequestListFirewallInstancesQuery
 from rime_sdk.swagger.swagger_client.models.list_images_request_pip_library_filter import ListImagesRequestPipLibraryFilter
 from rime_sdk.swagger.swagger_client.models.list_metric_identifiers_response_aggregated_metric import ListMetricIdentifiersResponseAggregatedMetric
 from rime_sdk.swagger.swagger_client.models.list_metric_identifiers_response_feature_metric_without_subsets import ListMetricIdentifiersResponseFeatureMetricWithoutSubsets
@@ -259,14 +263,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_actor_role import RimeActorRole
 from rime_sdk.swagger.swagger_client.models.rime_add_users_to_workspace_response import RimeAddUsersToWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_agent import RimeAgent
 from rime_sdk.swagger.swagger_client.models.rime_agent_desired_state import RimeAgentDesiredState
 from rime_sdk.swagger.swagger_client.models.rime_agent_status import RimeAgentStatus
 from rime_sdk.swagger.swagger_client.models.rime_agent_type import RimeAgentType
 from rime_sdk.swagger.swagger_client.models.rime_attack_objective import RimeAttackObjective
+from rime_sdk.swagger.swagger_client.models.rime_attack_technique import RimeAttackTechnique
 from rime_sdk.swagger.swagger_client.models.rime_cancel_job_response import RimeCancelJobResponse
 from rime_sdk.swagger.swagger_client.models.rime_category_metric import RimeCategoryMetric
 from rime_sdk.swagger.swagger_client.models.rime_category_test_result import RimeCategoryTestResult
 from rime_sdk.swagger.swagger_client.models.rime_config_type import RimeConfigType
 from rime_sdk.swagger.swagger_client.models.rime_configure_integration_request_integration_variable import RimeConfigureIntegrationRequestIntegrationVariable
 from rime_sdk.swagger.swagger_client.models.rime_configure_integration_response import RimeConfigureIntegrationResponse
 from rime_sdk.swagger.swagger_client.models.rime_continuous_test_job_progress import RimeContinuousTestJobProgress
@@ -352,14 +357,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_get_validate_predictions_task_status_response import RimeGetValidatePredictionsTaskStatusResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_workspace_response import RimeGetWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_heartbeat_response import RimeHeartbeatResponse
 from rime_sdk.swagger.swagger_client.models.rime_image_reference import RimeImageReference
 from rime_sdk.swagger.swagger_client.models.rime_int_list import RimeIntList
 from rime_sdk.swagger.swagger_client.models.rime_integration_info import RimeIntegrationInfo
 from rime_sdk.swagger.swagger_client.models.rime_job_data import RimeJobData
+from rime_sdk.swagger.swagger_client.models.rime_job_data_generative_model_test import RimeJobDataGenerativeModelTest
 from rime_sdk.swagger.swagger_client.models.rime_job_metadata import RimeJobMetadata
 from rime_sdk.swagger.swagger_client.models.rime_job_type import RimeJobType
 from rime_sdk.swagger.swagger_client.models.rime_job_view import RimeJobView
 from rime_sdk.swagger.swagger_client.models.rime_language import RimeLanguage
 from rime_sdk.swagger.swagger_client.models.rime_license_feature import RimeLicenseFeature
 from rime_sdk.swagger.swagger_client.models.rime_license_limit import RimeLicenseLimit
 from rime_sdk.swagger.swagger_client.models.rime_limit_status import RimeLimitStatus
@@ -369,14 +375,16 @@
 from rime_sdk.swagger.swagger_client.models.rime_list_current_user_roles_response import RimeListCurrentUserRolesResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_datasets_response import RimeListDatasetsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_detection_events_request_query import RimeListDetectionEventsRequestQuery
 from rime_sdk.swagger.swagger_client.models.rime_list_detection_events_response import RimeListDetectionEventsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_enabled_features_response import RimeListEnabledFeaturesResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_file_scan_results_response import RimeListFileScanResultsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_firewall_instances_response import RimeListFirewallInstancesResponse
+from rime_sdk.swagger.swagger_client.models.rime_list_gai_test_job_response import RimeListGAITestJobResponse
+from rime_sdk.swagger.swagger_client.models.rime_list_gai_test_jobs_request_query import RimeListGAITestJobsRequestQuery
 from rime_sdk.swagger.swagger_client.models.rime_list_images_request import RimeListImagesRequest
 from rime_sdk.swagger.swagger_client.models.rime_list_images_response import RimeListImagesResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_jobs_for_project_request_query import RimeListJobsForProjectRequestQuery
 from rime_sdk.swagger.swagger_client.models.rime_list_jobs_for_project_response import RimeListJobsForProjectResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_metric_identifiers_response import RimeListMetricIdentifiersResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_model_cards_response import RimeListModelCardsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_models_response import RimeListModelsResponse
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/__init__.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/agent_manager_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/agent_manager_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/config_validator_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/config_validator_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/data_collector_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/data_collector_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/detection_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/detection_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/feature_flag_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/feature_flag_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/file_scanning_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/file_scanning_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/file_upload_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/file_upload_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/firewall_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/firewall_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/firewall_instance_manager_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/firewall_instance_manager_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/firewall_service_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/firewall_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/generative_model_testing_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/generative_model_testing_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/image_registry_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/image_registry_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/integration_service_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/integration_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/job_reader_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/job_reader_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -412,14 +412,124 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def job_reader_list_gai_test_job(self, workspace_id_uuid, **kwargs):  # noqa: E501
+        """ListGAITestJob is a method to list all GAI test jobs for a given workspace.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.job_reader_list_gai_test_job(workspace_id_uuid, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str workspace_id_uuid: Unique object ID. (required)
+        :param list[str] first_page_query_selected_statuses: Specifies a set of statuses. The query only returns results with a status in the specified set. Specify no statuses to return all results.   - JOB_STATUS_PENDING: Resources have been created for the job but the job has not started yet.  - JOB_STATUS_FAILED: Blanket status for user or system-related job failure.  - JOB_STATUS_REQUESTED: The job descriptor exists but has no resources allocated. Jobs that remain in this status without moving to the PENDING status are at risk of entering the FAILED status.  - JOB_STATUS_CANCELLED: Job has been cancelled. Cancelled jobs cannot be recovered.
+        :param str page_token: The ListJobs query returns a pageToken after the first request.
+        :param str page_size: The maximum number of Job objects to return in a single page.
+        :param str view: Specifies how much information about each job to retrieve.   - JOB_VIEW_BASIC: Server responses only include basic information about the job, including type, status, and some job data.  - JOB_VIEW_FULL: Server responses include all available information about the job, including progress. Has greater performance requirements than the Basic view.
+        :return: RimeListGAITestJobResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.job_reader_list_gai_test_job_with_http_info(workspace_id_uuid, **kwargs)  # noqa: E501
+        else:
+            (data) = self.job_reader_list_gai_test_job_with_http_info(workspace_id_uuid, **kwargs)  # noqa: E501
+            return data
+
+    def job_reader_list_gai_test_job_with_http_info(self, workspace_id_uuid, **kwargs):  # noqa: E501
+        """ListGAITestJob is a method to list all GAI test jobs for a given workspace.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.job_reader_list_gai_test_job_with_http_info(workspace_id_uuid, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str workspace_id_uuid: Unique object ID. (required)
+        :param list[str] first_page_query_selected_statuses: Specifies a set of statuses. The query only returns results with a status in the specified set. Specify no statuses to return all results.   - JOB_STATUS_PENDING: Resources have been created for the job but the job has not started yet.  - JOB_STATUS_FAILED: Blanket status for user or system-related job failure.  - JOB_STATUS_REQUESTED: The job descriptor exists but has no resources allocated. Jobs that remain in this status without moving to the PENDING status are at risk of entering the FAILED status.  - JOB_STATUS_CANCELLED: Job has been cancelled. Cancelled jobs cannot be recovered.
+        :param str page_token: The ListJobs query returns a pageToken after the first request.
+        :param str page_size: The maximum number of Job objects to return in a single page.
+        :param str view: Specifies how much information about each job to retrieve.   - JOB_VIEW_BASIC: Server responses only include basic information about the job, including type, status, and some job data.  - JOB_VIEW_FULL: Server responses include all available information about the job, including progress. Has greater performance requirements than the Basic view.
+        :return: RimeListGAITestJobResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['workspace_id_uuid', 'first_page_query_selected_statuses', 'page_token', 'page_size', 'view']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method job_reader_list_gai_test_job" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'workspace_id_uuid' is set
+        if ('workspace_id_uuid' not in params or
+                params['workspace_id_uuid'] is None):
+            raise ValueError("Missing the required parameter `workspace_id_uuid` when calling `job_reader_list_gai_test_job`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'workspace_id_uuid' in params:
+            path_params['workspaceId.uuid'] = params['workspace_id_uuid']  # noqa: E501
+
+        query_params = []
+        if 'first_page_query_selected_statuses' in params:
+            query_params.append(('firstPageQuery.selectedStatuses', params['first_page_query_selected_statuses']))  # noqa: E501
+            collection_formats['firstPageQuery.selectedStatuses'] = 'multi'  # noqa: E501
+        if 'page_token' in params:
+            query_params.append(('pageToken', params['page_token']))  # noqa: E501
+        if 'page_size' in params:
+            query_params.append(('pageSize', params['page_size']))  # noqa: E501
+        if 'view' in params:
+            query_params.append(('view', params['view']))  # noqa: E501
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['X-Firewall-Api-Key', 'X-Firewall-Auth-Token', 'rime-api-key']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1-beta/jobs/generative/workspaces/{workspaceId.uuid}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RimeListGAITestJobResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def job_reader_list_jobs_for_project(self, project_id_uuid, **kwargs):  # noqa: E501
         """ListJobsForProject  # noqa: E501
 
         Returns a paginated list of jobs for a given project. The list can be filtered by job type and status.  #### Python pagination example:  ```python all_objects = [] # Required for authentication to all methods in the API. headers = {\"rime-api-key\": \"INSERT_API_TOKEN\"} # TODO page_token = \"\" # Initialize query parameters in a dictionary params = {\"INSERT_QUERY_PARAMETER\": \"INSERT_QUERY_VALUE\"} # TODO # Make requests until all results have been returned. while True:     # If the page_token from a previous response is not empty, we need to specify this     # token as a parameter to the next request in order to return the next page.     if page_token != \"\":         params = {\"page_token\": page_token}     res = requests.get(\"INSERT_METHOD_URI\", params=params, headers=headers) # TODO     if res.status_code != 200 :         raise ValueError(res)     res_json = res.json()     all_objects.extend(res_json['INSERT_OBJECT_KEY']) # TODO     page_token = res_json['nextPageToken']     # If all results have been returned, res_json['hasMore'] is false.     if not res_json[\"hasMore\"]:         break ```  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.job_reader_list_jobs_for_project(project_id_uuid, async_req=True)
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/model_card_service_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/model_card_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/model_testing_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/model_testing_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/monitor_service_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/monitor_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/notification_setting_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/notification_setting_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/project_service_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/project_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/registry_service_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/registry_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/results_reader_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/results_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/rime_info_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/rime_info_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/schedule_service_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/schedule_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/user_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/user_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -525,17 +525,18 @@
         List all API tokens for a Workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.user_list_api_tokens(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str page_token: Specifies a page of the list returned by a ListAPITokens query. The ListAPITokens query returns a pageToken when there is more than one page of results.
         :param str page_size: The maximum number of API Token objects to return in a single page.
         :param str workspace_id_uuid: Unique object ID.
+        :param str page_token: Specifies a page of the list returned by a ListAPITokens query. The ListAPITokens query returns a pageToken when there is more than one page of results.
+        :param str first_page_query_token_type: Specifies the type of token. The query filters for results that match the specified type.
         :return: RimeListAPITokensResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.user_list_api_tokens_with_http_info(**kwargs)  # noqa: E501
@@ -549,23 +550,24 @@
         List all API tokens for a Workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.user_list_api_tokens_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
-        :param str page_token: Specifies a page of the list returned by a ListAPITokens query. The ListAPITokens query returns a pageToken when there is more than one page of results.
         :param str page_size: The maximum number of API Token objects to return in a single page.
         :param str workspace_id_uuid: Unique object ID.
+        :param str page_token: Specifies a page of the list returned by a ListAPITokens query. The ListAPITokens query returns a pageToken when there is more than one page of results.
+        :param str first_page_query_token_type: Specifies the type of token. The query filters for results that match the specified type.
         :return: RimeListAPITokensResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['page_token', 'page_size', 'workspace_id_uuid']  # noqa: E501
+        all_params = ['page_size', 'workspace_id_uuid', 'page_token', 'first_page_query_token_type']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -578,20 +580,22 @@
         del params['kwargs']
 
         collection_formats = {}
 
         path_params = {}
 
         query_params = []
-        if 'page_token' in params:
-            query_params.append(('pageToken', params['page_token']))  # noqa: E501
         if 'page_size' in params:
             query_params.append(('pageSize', params['page_size']))  # noqa: E501
         if 'workspace_id_uuid' in params:
             query_params.append(('workspaceId.uuid', params['workspace_id_uuid']))  # noqa: E501
+        if 'page_token' in params:
+            query_params.append(('pageToken', params['page_token']))  # noqa: E501
+        if 'first_page_query_token_type' in params:
+            query_params.append(('firstPageQuery.tokenType', params['first_page_query_token_type']))  # noqa: E501
 
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/validation_service_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/validation_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api/workspace_service_api.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api/workspace_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/api_client.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/configuration.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/__init__.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from rime_sdk.swagger.swagger_client.models.agent_id_uuid_upgrade_body import AgentIdUuidUpgradeBody
 from rime_sdk.swagger.swagger_client.models.agent_id_uuid_upgrade_body1 import AgentIdUuidUpgradeBody1
 from rime_sdk.swagger.swagger_client.models.apigenerativefirewall_list_firewall_instances_response import ApigenerativefirewallListFirewallInstancesResponse
 from rime_sdk.swagger.swagger_client.models.apigenerativefirewall_standard_info import ApigenerativefirewallStandardInfo
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_category_test_identifier import ArtifactIdentifierCategoryTestIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_subset_test_metric_identifier import ArtifactIdentifierSubsetTestMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_test_case_metric_identifier import ArtifactIdentifierTestCaseMetricIdentifier
+from rime_sdk.swagger.swagger_client.models.code_detection_details_code_substring import CodeDetectionDetailsCodeSubstring
 from rime_sdk.swagger.swagger_client.models.config_generation_category_config_generation_service_response import ConfigGenerationCategoryConfigGenerationServiceResponse
 from rime_sdk.swagger.swagger_client.models.config_generation_profiling_config_generation_service_response import ConfigGenerationProfilingConfigGenerationServiceResponse
 from rime_sdk.swagger.swagger_client.models.config_generation_test_suite_config_generation_service_response import ConfigGenerationTestSuiteConfigGenerationServiceResponse
 from rime_sdk.swagger.swagger_client.models.configvalidator_config_type_body import ConfigvalidatorConfigTypeBody
 from rime_sdk.swagger.swagger_client.models.continuoustests_firewall_id_uuid_body import ContinuoustestsFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.create_agent_request_aws_config import CreateAgentRequestAWSConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_azure_config import CreateAgentRequestAzureConfig
@@ -74,19 +75,22 @@
 from rime_sdk.swagger.swagger_client.models.firewall_firewall_firewall_id_uuid_body import FirewallFirewallFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.firewall_latest_run_info import FirewallLatestRunInfo
 from rime_sdk.swagger.swagger_client.models.firewall_scheduled_ct_info import FirewallScheduledCTInfo
 from rime_sdk.swagger.swagger_client.models.firewall_test_category_severity import FirewallTestCategorySeverity
 from rime_sdk.swagger.swagger_client.models.firewallinstance_firewall_instance_firewall_instance_id_uuid_body import FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody
 from rime_sdk.swagger.swagger_client.models.flagged_substring_request_body_component import FlaggedSubstringRequestBodyComponent
 from rime_sdk.swagger.swagger_client.models.generative_testing_result_example import GenerativeTestingResultExample
+from rime_sdk.swagger.swagger_client.models.generativefirewall_code_detection_details import GenerativefirewallCodeDetectionDetails
+from rime_sdk.swagger.swagger_client.models.generativefirewall_code_detection_rule_config import GenerativefirewallCodeDetectionRuleConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_create_firewall_instance_request import GenerativefirewallCreateFirewallInstanceRequest
 from rime_sdk.swagger.swagger_client.models.generativefirewall_create_firewall_instance_response import GenerativefirewallCreateFirewallInstanceResponse
 from rime_sdk.swagger.swagger_client.models.generativefirewall_custom_pii_entity import GenerativefirewallCustomPiiEntity
 from rime_sdk.swagger.swagger_client.models.generativefirewall_denial_of_service_rule_config import GenerativefirewallDenialOfServiceRuleConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_action import GenerativefirewallFirewallAction
+from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_instance_deployment_config import GenerativefirewallFirewallInstanceDeploymentConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_instance_info import GenerativefirewallFirewallInstanceInfo
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_instance_status import GenerativefirewallFirewallInstanceStatus
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_rule_config import GenerativefirewallFirewallRuleConfig
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_rule_type import GenerativefirewallFirewallRuleType
 from rime_sdk.swagger.swagger_client.models.generativefirewall_firewall_tokenizer import GenerativefirewallFirewallTokenizer
 from rime_sdk.swagger.swagger_client.models.generativefirewall_flagged_substring import GenerativefirewallFlaggedSubstring
 from rime_sdk.swagger.swagger_client.models.generativefirewall_get_firewall_effective_config_response import GenerativefirewallGetFirewallEffectiveConfigResponse
@@ -122,18 +126,18 @@
 from rime_sdk.swagger.swagger_client.models.image_reference_reference_type import ImageReferenceReferenceType
 from rime_sdk.swagger.swagger_client.models.integration_integration_level import IntegrationIntegrationLevel
 from rime_sdk.swagger.swagger_client.models.integration_integration_schema import IntegrationIntegrationSchema
 from rime_sdk.swagger.swagger_client.models.integration_integration_type import IntegrationIntegrationType
 from rime_sdk.swagger.swagger_client.models.integration_variable_sensitivity import IntegrationVariableSensitivity
 from rime_sdk.swagger.swagger_client.models.integrations_integration_id_uuid_body import IntegrationsIntegrationIdUuidBody
 from rime_sdk.swagger.swagger_client.models.job_data_continuous_incremental_test import JobDataContinuousIncrementalTest
-from rime_sdk.swagger.swagger_client.models.job_data_generative_model_test import JobDataGenerativeModelTest
 from rime_sdk.swagger.swagger_client.models.job_data_scan import JobDataScan
 from rime_sdk.swagger.swagger_client.models.job_data_stress_test import JobDataStressTest
 from rime_sdk.swagger.swagger_client.models.language_detection_details_language_substring import LanguageDetectionDetailsLanguageSubstring
+from rime_sdk.swagger.swagger_client.models.list_api_tokens_request_list_api_tokens_query import ListAPITokensRequestListAPITokensQuery
 from rime_sdk.swagger.swagger_client.models.list_agents_request_list_agents_query import ListAgentsRequestListAgentsQuery
 from rime_sdk.swagger.swagger_client.models.list_datasets_request_datasets_query import ListDatasetsRequestDatasetsQuery
 from rime_sdk.swagger.swagger_client.models.list_file_scan_results_request_file_scan_query import ListFileScanResultsRequestFileScanQuery
 from rime_sdk.swagger.swagger_client.models.list_firewall_instances_request_list_firewall_instances_query import ListFirewallInstancesRequestListFirewallInstancesQuery
 from rime_sdk.swagger.swagger_client.models.list_images_request_pip_library_filter import ListImagesRequestPipLibraryFilter
 from rime_sdk.swagger.swagger_client.models.list_metric_identifiers_response_aggregated_metric import ListMetricIdentifiersResponseAggregatedMetric
 from rime_sdk.swagger.swagger_client.models.list_metric_identifiers_response_feature_metric_without_subsets import ListMetricIdentifiersResponseFeatureMetricWithoutSubsets
@@ -227,14 +231,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_actor_role import RimeActorRole
 from rime_sdk.swagger.swagger_client.models.rime_add_users_to_workspace_response import RimeAddUsersToWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_agent import RimeAgent
 from rime_sdk.swagger.swagger_client.models.rime_agent_desired_state import RimeAgentDesiredState
 from rime_sdk.swagger.swagger_client.models.rime_agent_status import RimeAgentStatus
 from rime_sdk.swagger.swagger_client.models.rime_agent_type import RimeAgentType
 from rime_sdk.swagger.swagger_client.models.rime_attack_objective import RimeAttackObjective
+from rime_sdk.swagger.swagger_client.models.rime_attack_technique import RimeAttackTechnique
 from rime_sdk.swagger.swagger_client.models.rime_cancel_job_response import RimeCancelJobResponse
 from rime_sdk.swagger.swagger_client.models.rime_category_metric import RimeCategoryMetric
 from rime_sdk.swagger.swagger_client.models.rime_category_test_result import RimeCategoryTestResult
 from rime_sdk.swagger.swagger_client.models.rime_config_type import RimeConfigType
 from rime_sdk.swagger.swagger_client.models.rime_configure_integration_request_integration_variable import RimeConfigureIntegrationRequestIntegrationVariable
 from rime_sdk.swagger.swagger_client.models.rime_configure_integration_response import RimeConfigureIntegrationResponse
 from rime_sdk.swagger.swagger_client.models.rime_continuous_test_job_progress import RimeContinuousTestJobProgress
@@ -320,14 +325,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_get_validate_predictions_task_status_response import RimeGetValidatePredictionsTaskStatusResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_workspace_response import RimeGetWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_heartbeat_response import RimeHeartbeatResponse
 from rime_sdk.swagger.swagger_client.models.rime_image_reference import RimeImageReference
 from rime_sdk.swagger.swagger_client.models.rime_int_list import RimeIntList
 from rime_sdk.swagger.swagger_client.models.rime_integration_info import RimeIntegrationInfo
 from rime_sdk.swagger.swagger_client.models.rime_job_data import RimeJobData
+from rime_sdk.swagger.swagger_client.models.rime_job_data_generative_model_test import RimeJobDataGenerativeModelTest
 from rime_sdk.swagger.swagger_client.models.rime_job_metadata import RimeJobMetadata
 from rime_sdk.swagger.swagger_client.models.rime_job_type import RimeJobType
 from rime_sdk.swagger.swagger_client.models.rime_job_view import RimeJobView
 from rime_sdk.swagger.swagger_client.models.rime_language import RimeLanguage
 from rime_sdk.swagger.swagger_client.models.rime_license_feature import RimeLicenseFeature
 from rime_sdk.swagger.swagger_client.models.rime_license_limit import RimeLicenseLimit
 from rime_sdk.swagger.swagger_client.models.rime_limit_status import RimeLimitStatus
@@ -337,14 +343,16 @@
 from rime_sdk.swagger.swagger_client.models.rime_list_current_user_roles_response import RimeListCurrentUserRolesResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_datasets_response import RimeListDatasetsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_detection_events_request_query import RimeListDetectionEventsRequestQuery
 from rime_sdk.swagger.swagger_client.models.rime_list_detection_events_response import RimeListDetectionEventsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_enabled_features_response import RimeListEnabledFeaturesResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_file_scan_results_response import RimeListFileScanResultsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_firewall_instances_response import RimeListFirewallInstancesResponse
+from rime_sdk.swagger.swagger_client.models.rime_list_gai_test_job_response import RimeListGAITestJobResponse
+from rime_sdk.swagger.swagger_client.models.rime_list_gai_test_jobs_request_query import RimeListGAITestJobsRequestQuery
 from rime_sdk.swagger.swagger_client.models.rime_list_images_request import RimeListImagesRequest
 from rime_sdk.swagger.swagger_client.models.rime_list_images_response import RimeListImagesResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_jobs_for_project_request_query import RimeListJobsForProjectRequestQuery
 from rime_sdk.swagger.swagger_client.models.rime_list_jobs_for_project_response import RimeListJobsForProjectResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_metric_identifiers_response import RimeListMetricIdentifiersResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_model_cards_response import RimeListModelCardsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_models_response import RimeListModelsResponse
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/apigenerativefirewall_list_firewall_instances_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/apigenerativefirewall_list_firewall_instances_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/apigenerativefirewall_standard_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/apigenerativefirewall_standard_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/crossplanetask_cross_plane_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/crossplanetask_cross_plane_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/dataset_dataset.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/dataset_dataset.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/detection_detection_event.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/detection_detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/detection_event_detail.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/detection_event_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/detection_event_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/detection_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/detection_resolution.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/detection_resolution.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_file_security_report.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_file_security_report.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_package_url.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_package_url.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata_license.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata_license.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/fileserver_check_object_exists_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/fileserver_check_object_exists_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/fileserver_delete_object_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/fileserver_delete_object_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/fileserver_get_read_object_presigned_link_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/fileserver_get_read_object_presigned_link_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/fileserver_get_upload_object_presigned_link_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/fileserver_get_upload_object_presigned_link_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/fileserver_list_objects_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/fileserver_list_objects_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/firewall_firewall.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/firewall_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/firewallinstance_firewall_instance_firewall_instance_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/firewallinstance_firewall_instance_firewall_instance_id_uuid_body.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,43 +28,48 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'firewall_instance_id': 'object',
         'config': 'GenerativefirewallFirewallRuleConfig',
         'deployment_status': 'GenerativefirewallFirewallInstanceStatus',
         'description': 'str',
-        'agent_id': 'RimeUUID'
+        'agent_id': 'RimeUUID',
+        'spec': 'GenerativefirewallFirewallInstanceDeploymentConfig'
     }
 
     attribute_map = {
         'firewall_instance_id': 'firewallInstanceId',
         'config': 'config',
         'deployment_status': 'deploymentStatus',
         'description': 'description',
-        'agent_id': 'agentId'
+        'agent_id': 'agentId',
+        'spec': 'spec'
     }
 
-    def __init__(self, firewall_instance_id=None, config=None, deployment_status=None, description=None, agent_id=None):  # noqa: E501
+    def __init__(self, firewall_instance_id=None, config=None, deployment_status=None, description=None, agent_id=None, spec=None):  # noqa: E501
         """FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody - a model defined in Swagger"""  # noqa: E501
         self._firewall_instance_id = None
         self._config = None
         self._deployment_status = None
         self._description = None
         self._agent_id = None
+        self._spec = None
         self.discriminator = None
         if firewall_instance_id is not None:
             self.firewall_instance_id = firewall_instance_id
         if config is not None:
             self.config = config
         if deployment_status is not None:
             self.deployment_status = deployment_status
         if description is not None:
             self.description = description
         if agent_id is not None:
             self.agent_id = agent_id
+        if spec is not None:
+            self.spec = spec
 
     @property
     def firewall_instance_id(self):
         """Gets the firewall_instance_id of this FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody.  # noqa: E501
 
         Unique ID of an object in RIME.  # noqa: E501
 
@@ -167,14 +172,35 @@
 
         :param agent_id: The agent_id of this FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody.  # noqa: E501
         :type: RimeUUID
         """
 
         self._agent_id = agent_id
 
+    @property
+    def spec(self):
+        """Gets the spec of this FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody.  # noqa: E501
+
+
+        :return: The spec of this FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody.  # noqa: E501
+        :rtype: GenerativefirewallFirewallInstanceDeploymentConfig
+        """
+        return self._spec
+
+    @spec.setter
+    def spec(self, spec):
+        """Sets the spec of this FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody.
+
+
+        :param spec: The spec of this FirewallinstanceFirewallInstanceFirewallInstanceIdUuidBody.  # noqa: E501
+        :type: GenerativefirewallFirewallInstanceDeploymentConfig
+        """
+
+        self._spec = spec
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/flagged_substring_request_body_component.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/flagged_substring_request_body_component.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generative_testing_result_example.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generative_testing_result_example.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,31 +25,36 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'config': 'GenerativefirewallFirewallRuleConfig',
-        'description': 'str'
+        'description': 'str',
+        'spec': 'GenerativefirewallFirewallInstanceDeploymentConfig'
     }
 
     attribute_map = {
         'config': 'config',
-        'description': 'description'
+        'description': 'description',
+        'spec': 'spec'
     }
 
-    def __init__(self, config=None, description=None):  # noqa: E501
+    def __init__(self, config=None, description=None, spec=None):  # noqa: E501
         """GenerativefirewallCreateFirewallInstanceRequest - a model defined in Swagger"""  # noqa: E501
         self._config = None
         self._description = None
+        self._spec = None
         self.discriminator = None
         if config is not None:
             self.config = config
         if description is not None:
             self.description = description
+        if spec is not None:
+            self.spec = spec
 
     @property
     def config(self):
         """Gets the config of this GenerativefirewallCreateFirewallInstanceRequest.  # noqa: E501
 
 
         :return: The config of this GenerativefirewallCreateFirewallInstanceRequest.  # noqa: E501
@@ -87,14 +92,35 @@
 
         :param description: The description of this GenerativefirewallCreateFirewallInstanceRequest.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
+    @property
+    def spec(self):
+        """Gets the spec of this GenerativefirewallCreateFirewallInstanceRequest.  # noqa: E501
+
+
+        :return: The spec of this GenerativefirewallCreateFirewallInstanceRequest.  # noqa: E501
+        :rtype: GenerativefirewallFirewallInstanceDeploymentConfig
+        """
+        return self._spec
+
+    @spec.setter
+    def spec(self, spec):
+        """Sets the spec of this GenerativefirewallCreateFirewallInstanceRequest.
+
+
+        :param spec: The spec of this GenerativefirewallCreateFirewallInstanceRequest.  # noqa: E501
+        :type: GenerativefirewallFirewallInstanceDeploymentConfig
+        """
+
+        self._spec = spec
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_custom_pii_entity.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_custom_pii_entity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_denial_of_service_rule_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_denial_of_service_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,43 +28,48 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'firewall_instance_id': 'RimeUUID',
         'config': 'GenerativefirewallFirewallRuleConfig',
         'deployment_status': 'GenerativefirewallFirewallInstanceStatus',
         'description': 'str',
-        'agent_id': 'RimeUUID'
+        'agent_id': 'RimeUUID',
+        'spec': 'GenerativefirewallFirewallInstanceDeploymentConfig'
     }
 
     attribute_map = {
         'firewall_instance_id': 'firewallInstanceId',
         'config': 'config',
         'deployment_status': 'deploymentStatus',
         'description': 'description',
-        'agent_id': 'agentId'
+        'agent_id': 'agentId',
+        'spec': 'spec'
     }
 
-    def __init__(self, firewall_instance_id=None, config=None, deployment_status=None, description=None, agent_id=None):  # noqa: E501
+    def __init__(self, firewall_instance_id=None, config=None, deployment_status=None, description=None, agent_id=None, spec=None):  # noqa: E501
         """GenerativefirewallFirewallInstanceInfo - a model defined in Swagger"""  # noqa: E501
         self._firewall_instance_id = None
         self._config = None
         self._deployment_status = None
         self._description = None
         self._agent_id = None
+        self._spec = None
         self.discriminator = None
         if firewall_instance_id is not None:
             self.firewall_instance_id = firewall_instance_id
         if config is not None:
             self.config = config
         if deployment_status is not None:
             self.deployment_status = deployment_status
         if description is not None:
             self.description = description
         if agent_id is not None:
             self.agent_id = agent_id
+        if spec is not None:
+            self.spec = spec
 
     @property
     def firewall_instance_id(self):
         """Gets the firewall_instance_id of this GenerativefirewallFirewallInstanceInfo.  # noqa: E501
 
 
         :return: The firewall_instance_id of this GenerativefirewallFirewallInstanceInfo.  # noqa: E501
@@ -165,14 +170,35 @@
 
         :param agent_id: The agent_id of this GenerativefirewallFirewallInstanceInfo.  # noqa: E501
         :type: RimeUUID
         """
 
         self._agent_id = agent_id
 
+    @property
+    def spec(self):
+        """Gets the spec of this GenerativefirewallFirewallInstanceInfo.  # noqa: E501
+
+
+        :return: The spec of this GenerativefirewallFirewallInstanceInfo.  # noqa: E501
+        :rtype: GenerativefirewallFirewallInstanceDeploymentConfig
+        """
+        return self._spec
+
+    @spec.setter
+    def spec(self, spec):
+        """Sets the spec of this GenerativefirewallFirewallInstanceInfo.
+
+
+        :param spec: The spec of this GenerativefirewallFirewallInstanceInfo.  # noqa: E501
+        :type: GenerativefirewallFirewallInstanceDeploymentConfig
+        """
+
+        self._spec = spec
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_status.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     FACTUAL_INCONSISTENCY = "FIREWALL_RULE_TYPE_FACTUAL_INCONSISTENCY"
     OFF_TOPIC = "FIREWALL_RULE_TYPE_OFF_TOPIC"
     DENIAL_OF_SERVICE = "FIREWALL_RULE_TYPE_DENIAL_OF_SERVICE"
     INDIRECT_PROMPT_INJECTION = "FIREWALL_RULE_TYPE_INDIRECT_PROMPT_INJECTION"
     UNKNOWN_EXTERNAL_SOURCE = "FIREWALL_RULE_TYPE_UNKNOWN_EXTERNAL_SOURCE"
     LANGUAGE_DETECTION = "FIREWALL_RULE_TYPE_LANGUAGE_DETECTION"
     PROMPT_INJECTION_V2 = "FIREWALL_RULE_TYPE_PROMPT_INJECTION_V2"
+    CODE_DETECTION = "FIREWALL_RULE_TYPE_CODE_DETECTION"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_tokenizer.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_flagged_substring.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_flagged_substring.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_effective_config_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_effective_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_instance_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_instance_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_individual_rules_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_individual_rules_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,42 +33,45 @@
         'pii_detection_output': 'GenerativefirewallPiiDetectionRuleConfig',
         'denial_of_service_input': 'GenerativefirewallDenialOfServiceRuleConfig',
         'denial_of_service_output': 'GenerativefirewallDenialOfServiceRuleConfig',
         'unknown_external_source': 'GenerativefirewallUnknownExternalSourceRuleConfig',
         'language_detection': 'GenerativefirewallLanguageDetectionRuleConfig',
         'prompt_injection_v2': 'GenerativefirewallPromptInjectionV2RuleConfig',
         'toxicity_rule_config_input': 'GenerativefirewallToxicityRuleConfig',
-        'toxicity_rule_config_output': 'GenerativefirewallToxicityRuleConfig'
+        'toxicity_rule_config_output': 'GenerativefirewallToxicityRuleConfig',
+        'code_detection': 'GenerativefirewallCodeDetectionRuleConfig'
     }
 
     attribute_map = {
         'off_topic': 'offTopic',
         'pii_detection_input': 'piiDetectionInput',
         'pii_detection_output': 'piiDetectionOutput',
         'denial_of_service_input': 'denialOfServiceInput',
         'denial_of_service_output': 'denialOfServiceOutput',
         'unknown_external_source': 'unknownExternalSource',
         'language_detection': 'languageDetection',
         'prompt_injection_v2': 'promptInjectionV2',
         'toxicity_rule_config_input': 'toxicityRuleConfigInput',
-        'toxicity_rule_config_output': 'toxicityRuleConfigOutput'
+        'toxicity_rule_config_output': 'toxicityRuleConfigOutput',
+        'code_detection': 'codeDetection'
     }
 
-    def __init__(self, off_topic=None, pii_detection_input=None, pii_detection_output=None, denial_of_service_input=None, denial_of_service_output=None, unknown_external_source=None, language_detection=None, prompt_injection_v2=None, toxicity_rule_config_input=None, toxicity_rule_config_output=None):  # noqa: E501
+    def __init__(self, off_topic=None, pii_detection_input=None, pii_detection_output=None, denial_of_service_input=None, denial_of_service_output=None, unknown_external_source=None, language_detection=None, prompt_injection_v2=None, toxicity_rule_config_input=None, toxicity_rule_config_output=None, code_detection=None):  # noqa: E501
         """GenerativefirewallIndividualRulesConfig - a model defined in Swagger"""  # noqa: E501
         self._off_topic = None
         self._pii_detection_input = None
         self._pii_detection_output = None
         self._denial_of_service_input = None
         self._denial_of_service_output = None
         self._unknown_external_source = None
         self._language_detection = None
         self._prompt_injection_v2 = None
         self._toxicity_rule_config_input = None
         self._toxicity_rule_config_output = None
+        self._code_detection = None
         self.discriminator = None
         if off_topic is not None:
             self.off_topic = off_topic
         if pii_detection_input is not None:
             self.pii_detection_input = pii_detection_input
         if pii_detection_output is not None:
             self.pii_detection_output = pii_detection_output
@@ -82,14 +85,16 @@
             self.language_detection = language_detection
         if prompt_injection_v2 is not None:
             self.prompt_injection_v2 = prompt_injection_v2
         if toxicity_rule_config_input is not None:
             self.toxicity_rule_config_input = toxicity_rule_config_input
         if toxicity_rule_config_output is not None:
             self.toxicity_rule_config_output = toxicity_rule_config_output
+        if code_detection is not None:
+            self.code_detection = code_detection
 
     @property
     def off_topic(self):
         """Gets the off_topic of this GenerativefirewallIndividualRulesConfig.  # noqa: E501
 
 
         :return: The off_topic of this GenerativefirewallIndividualRulesConfig.  # noqa: E501
@@ -293,14 +298,35 @@
 
         :param toxicity_rule_config_output: The toxicity_rule_config_output of this GenerativefirewallIndividualRulesConfig.  # noqa: E501
         :type: GenerativefirewallToxicityRuleConfig
         """
 
         self._toxicity_rule_config_output = toxicity_rule_config_output
 
+    @property
+    def code_detection(self):
+        """Gets the code_detection of this GenerativefirewallIndividualRulesConfig.  # noqa: E501
+
+
+        :return: The code_detection of this GenerativefirewallIndividualRulesConfig.  # noqa: E501
+        :rtype: GenerativefirewallCodeDetectionRuleConfig
+        """
+        return self._code_detection
+
+    @code_detection.setter
+    def code_detection(self, code_detection):
+        """Sets the code_detection of this GenerativefirewallIndividualRulesConfig.
+
+
+        :param code_detection: The code_detection of this GenerativefirewallIndividualRulesConfig.  # noqa: E501
+        :type: GenerativefirewallCodeDetectionRuleConfig
+        """
+
+        self._code_detection = code_detection
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_details.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_rule_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_off_topic_rule_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_off_topic_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_details.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_rule_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_entity_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_entity_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_details.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_details.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'objectives': 'list[RimeAttackObjective]',
-        'techniques': 'list[str]'
+        'techniques': 'list[RimeAttackTechnique]'
     }
 
     attribute_map = {
         'objectives': 'objectives',
         'techniques': 'techniques'
     }
 
@@ -73,26 +73,26 @@
     @property
     def techniques(self):
         """Gets the techniques of this GenerativefirewallPromptInjectionDetails.  # noqa: E501
 
         Attack Techniques represent the technique used in a prompt injection for example: unicode obfuscation, base64 etc. These values may change between versions.  # noqa: E501
 
         :return: The techniques of this GenerativefirewallPromptInjectionDetails.  # noqa: E501
-        :rtype: list[str]
+        :rtype: list[RimeAttackTechnique]
         """
         return self._techniques
 
     @techniques.setter
     def techniques(self, techniques):
         """Sets the techniques of this GenerativefirewallPromptInjectionDetails.
 
         Attack Techniques represent the technique used in a prompt injection for example: unicode obfuscation, base64 etc. These values may change between versions.  # noqa: E501
 
         :param techniques: The techniques of this GenerativefirewallPromptInjectionDetails.  # noqa: E501
-        :type: list[str]
+        :type: list[RimeAttackTechnique]
         """
 
         self._techniques = techniques
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_v2_rule_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_v2_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_false_positive_rate.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_false_positive_rate.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,39 +31,42 @@
         'rule_name': 'str',
         'action': 'GenerativefirewallFirewallAction',
         'risk_category': 'RiskscoreRiskCategoryType',
         'pii_detection_details': 'GenerativefirewallPiiDetectionDetails',
         'language_detection_details': 'GenerativefirewallLanguageDetectionDetails',
         'prompt_injection_details': 'GenerativefirewallPromptInjectionDetails',
         'toxicity_detection_details': 'GenerativefirewallToxicityDetectionDetails',
+        'code_detection_details': 'GenerativefirewallCodeDetectionDetails',
         'rule_eval_metadata': 'RuleOutputRuleEvaluationMetadata',
         'regulatory_standards': 'list[ApigenerativefirewallStandardInfo]'
     }
 
     attribute_map = {
         'rule_name': 'ruleName',
         'action': 'action',
         'risk_category': 'riskCategory',
         'pii_detection_details': 'piiDetectionDetails',
         'language_detection_details': 'languageDetectionDetails',
         'prompt_injection_details': 'promptInjectionDetails',
         'toxicity_detection_details': 'toxicityDetectionDetails',
+        'code_detection_details': 'codeDetectionDetails',
         'rule_eval_metadata': 'ruleEvalMetadata',
         'regulatory_standards': 'regulatoryStandards'
     }
 
-    def __init__(self, rule_name=None, action=None, risk_category=None, pii_detection_details=None, language_detection_details=None, prompt_injection_details=None, toxicity_detection_details=None, rule_eval_metadata=None, regulatory_standards=None):  # noqa: E501
+    def __init__(self, rule_name=None, action=None, risk_category=None, pii_detection_details=None, language_detection_details=None, prompt_injection_details=None, toxicity_detection_details=None, code_detection_details=None, rule_eval_metadata=None, regulatory_standards=None):  # noqa: E501
         """GenerativefirewallRuleOutput - a model defined in Swagger"""  # noqa: E501
         self._rule_name = None
         self._action = None
         self._risk_category = None
         self._pii_detection_details = None
         self._language_detection_details = None
         self._prompt_injection_details = None
         self._toxicity_detection_details = None
+        self._code_detection_details = None
         self._rule_eval_metadata = None
         self._regulatory_standards = None
         self.discriminator = None
         if rule_name is not None:
             self.rule_name = rule_name
         if action is not None:
             self.action = action
@@ -73,14 +76,16 @@
             self.pii_detection_details = pii_detection_details
         if language_detection_details is not None:
             self.language_detection_details = language_detection_details
         if prompt_injection_details is not None:
             self.prompt_injection_details = prompt_injection_details
         if toxicity_detection_details is not None:
             self.toxicity_detection_details = toxicity_detection_details
+        if code_detection_details is not None:
+            self.code_detection_details = code_detection_details
         if rule_eval_metadata is not None:
             self.rule_eval_metadata = rule_eval_metadata
         if regulatory_standards is not None:
             self.regulatory_standards = regulatory_standards
 
     @property
     def rule_name(self):
@@ -226,14 +231,35 @@
         :param toxicity_detection_details: The toxicity_detection_details of this GenerativefirewallRuleOutput.  # noqa: E501
         :type: GenerativefirewallToxicityDetectionDetails
         """
 
         self._toxicity_detection_details = toxicity_detection_details
 
     @property
+    def code_detection_details(self):
+        """Gets the code_detection_details of this GenerativefirewallRuleOutput.  # noqa: E501
+
+
+        :return: The code_detection_details of this GenerativefirewallRuleOutput.  # noqa: E501
+        :rtype: GenerativefirewallCodeDetectionDetails
+        """
+        return self._code_detection_details
+
+    @code_detection_details.setter
+    def code_detection_details(self, code_detection_details):
+        """Sets the code_detection_details of this GenerativefirewallRuleOutput.
+
+
+        :param code_detection_details: The code_detection_details of this GenerativefirewallRuleOutput.  # noqa: E501
+        :type: GenerativefirewallCodeDetectionDetails
+        """
+
+        self._code_detection_details = code_detection_details
+
+    @property
     def rule_eval_metadata(self):
         """Gets the rule_eval_metadata of this GenerativefirewallRuleOutput.  # noqa: E501
 
 
         :return: The rule_eval_metadata of this GenerativefirewallRuleOutput.  # noqa: E501
         :rtype: RuleOutputRuleEvaluationMetadata
         """
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_sensitivity.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_detection_details.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_detection_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_rule_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_unknown_external_source_rule_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_unknown_external_source_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_update_firewall_instance_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_update_firewall_instance_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         'attack_objective': 'RimeAttackObjective',
         'objective_sub_category': 'GenerativetestingObjectiveSubCategory',
         'failing_examples': 'list[GenerativeTestingResultExample]',
         'severity': 'RimeSeverity',
         'owasp_standards': 'list[GenerativetestingGenerativeTestingResultStandardInfo]',
         'nist_standards': 'list[GenerativetestingGenerativeTestingResultStandardInfo]',
         'mitre_standards': 'list[GenerativetestingGenerativeTestingResultStandardInfo]',
-        'attacks_attempted': 'str',
+        'attacks_attempted': 'int',
         'threat': 'GenerativetestingThreat'
     }
 
     attribute_map = {
         'id': 'id',
         'job_id': 'jobId',
         'attack_technique': 'attackTechnique',
@@ -316,26 +316,26 @@
     @property
     def attacks_attempted(self):
         """Gets the attacks_attempted of this GenerativetestingGenerativeTestingResult.  # noqa: E501
 
         The number of attacks prompts attempted for these results.  # noqa: E501
 
         :return: The attacks_attempted of this GenerativetestingGenerativeTestingResult.  # noqa: E501
-        :rtype: str
+        :rtype: int
         """
         return self._attacks_attempted
 
     @attacks_attempted.setter
     def attacks_attempted(self, attacks_attempted):
         """Sets the attacks_attempted of this GenerativetestingGenerativeTestingResult.
 
         The number of attacks prompts attempted for these results.  # noqa: E501
 
         :param attacks_attempted: The attacks_attempted of this GenerativetestingGenerativeTestingResult.  # noqa: E501
-        :type: str
+        :type: int
         """
 
         self._attacks_attempted = attacks_attempted
 
     @property
     def threat(self):
         """Gets the threat of this GenerativetestingGenerativeTestingResult.  # noqa: E501
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result_standard_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result_standard_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_request_query.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,35 +26,45 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'results': 'list[GenerativetestingGenerativeTestingResult]',
         'next_page_token': 'str',
-        'has_more': 'bool'
+        'has_more': 'bool',
+        'job_id': 'RimeUUID',
+        'job_status': 'StatedbJobStatus'
     }
 
     attribute_map = {
         'results': 'results',
         'next_page_token': 'nextPageToken',
-        'has_more': 'hasMore'
+        'has_more': 'hasMore',
+        'job_id': 'jobId',
+        'job_status': 'jobStatus'
     }
 
-    def __init__(self, results=None, next_page_token=None, has_more=None):  # noqa: E501
+    def __init__(self, results=None, next_page_token=None, has_more=None, job_id=None, job_status=None):  # noqa: E501
         """GenerativetestingGetGenerativeModelTestResultsResponse - a model defined in Swagger"""  # noqa: E501
         self._results = None
         self._next_page_token = None
         self._has_more = None
+        self._job_id = None
+        self._job_status = None
         self.discriminator = None
         if results is not None:
             self.results = results
         if next_page_token is not None:
             self.next_page_token = next_page_token
         if has_more is not None:
             self.has_more = has_more
+        if job_id is not None:
+            self.job_id = job_id
+        if job_status is not None:
+            self.job_status = job_status
 
     @property
     def results(self):
         """Gets the results of this GenerativetestingGetGenerativeModelTestResultsResponse.  # noqa: E501
 
         The list of generative testing results.  # noqa: E501
 
@@ -117,14 +127,56 @@
 
         :param has_more: The has_more of this GenerativetestingGetGenerativeModelTestResultsResponse.  # noqa: E501
         :type: bool
         """
 
         self._has_more = has_more
 
+    @property
+    def job_id(self):
+        """Gets the job_id of this GenerativetestingGetGenerativeModelTestResultsResponse.  # noqa: E501
+
+
+        :return: The job_id of this GenerativetestingGetGenerativeModelTestResultsResponse.  # noqa: E501
+        :rtype: RimeUUID
+        """
+        return self._job_id
+
+    @job_id.setter
+    def job_id(self, job_id):
+        """Sets the job_id of this GenerativetestingGetGenerativeModelTestResultsResponse.
+
+
+        :param job_id: The job_id of this GenerativetestingGetGenerativeModelTestResultsResponse.  # noqa: E501
+        :type: RimeUUID
+        """
+
+        self._job_id = job_id
+
+    @property
+    def job_status(self):
+        """Gets the job_status of this GenerativetestingGetGenerativeModelTestResultsResponse.  # noqa: E501
+
+
+        :return: The job_status of this GenerativetestingGetGenerativeModelTestResultsResponse.  # noqa: E501
+        :rtype: StatedbJobStatus
+        """
+        return self._job_status
+
+    @job_status.setter
+    def job_status(self, job_status):
+        """Sets the job_status of this GenerativetestingGetGenerativeModelTestResultsResponse.
+
+
+        :param job_status: The job_status of this GenerativetestingGetGenerativeModelTestResultsResponse.  # noqa: E501
+        :type: StatedbJobStatus
+        """
+
+        self._job_status = job_status
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativetesting_objective_sub_category.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativetesting_objective_sub_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,44 +29,49 @@
     """
     swagger_types = {
         'url': 'str',
         'http_headers': 'dict(str, str)',
         'endpoint_payload_template': 'str',
         'response_json_path': 'str',
         'http_auth_integration_id': 'RimeUUID',
-        'name': 'str'
+        'name': 'str',
+        'mutual_tls_integration_id': 'RimeUUID'
     }
 
     attribute_map = {
         'url': 'url',
         'http_headers': 'httpHeaders',
         'endpoint_payload_template': 'endpointPayloadTemplate',
         'response_json_path': 'responseJsonPath',
         'http_auth_integration_id': 'httpAuthIntegrationId',
-        'name': 'name'
+        'name': 'name',
+        'mutual_tls_integration_id': 'mutualTlsIntegrationId'
     }
 
-    def __init__(self, url=None, http_headers=None, endpoint_payload_template=None, response_json_path=None, http_auth_integration_id=None, name=None):  # noqa: E501
+    def __init__(self, url=None, http_headers=None, endpoint_payload_template=None, response_json_path=None, http_auth_integration_id=None, name=None, mutual_tls_integration_id=None):  # noqa: E501
         """GenerativetestingStartGenerativeModelTestRequest - a model defined in Swagger"""  # noqa: E501
         self._url = None
         self._http_headers = None
         self._endpoint_payload_template = None
         self._response_json_path = None
         self._http_auth_integration_id = None
         self._name = None
+        self._mutual_tls_integration_id = None
         self.discriminator = None
         self.url = url
         if http_headers is not None:
             self.http_headers = http_headers
         self.endpoint_payload_template = endpoint_payload_template
         self.response_json_path = response_json_path
         if http_auth_integration_id is not None:
             self.http_auth_integration_id = http_auth_integration_id
         if name is not None:
             self.name = name
+        if mutual_tls_integration_id is not None:
+            self.mutual_tls_integration_id = mutual_tls_integration_id
 
     @property
     def url(self):
         """Gets the url of this GenerativetestingStartGenerativeModelTestRequest.  # noqa: E501
 
         Parameters for connecting to the user's generative model.  # noqa: E501
 
@@ -110,24 +115,26 @@
 
         self._http_headers = http_headers
 
     @property
     def endpoint_payload_template(self):
         """Gets the endpoint_payload_template of this GenerativetestingStartGenerativeModelTestRequest.  # noqa: E501
 
+        A string template that will be used to create the json payload sent to the LLM endpoint. This template must contain one and only one variable -- prompt_string. This will be replaced at runtime with the prompt used to send to the model.  The template uses \" and \" as the opening and closing delimiters around the prompt_string variable name.  Example: '{ \"prompt\": \"{{prompt_string}}\" }' Example: '{ \"message\": { \"llm_prompt\": \"{{prompt_string}}\" } }'  # noqa: E501
 
         :return: The endpoint_payload_template of this GenerativetestingStartGenerativeModelTestRequest.  # noqa: E501
         :rtype: str
         """
         return self._endpoint_payload_template
 
     @endpoint_payload_template.setter
     def endpoint_payload_template(self, endpoint_payload_template):
         """Sets the endpoint_payload_template of this GenerativetestingStartGenerativeModelTestRequest.
 
+        A string template that will be used to create the json payload sent to the LLM endpoint. This template must contain one and only one variable -- prompt_string. This will be replaced at runtime with the prompt used to send to the model.  The template uses \" and \" as the opening and closing delimiters around the prompt_string variable name.  Example: '{ \"prompt\": \"{{prompt_string}}\" }' Example: '{ \"message\": { \"llm_prompt\": \"{{prompt_string}}\" } }'  # noqa: E501
 
         :param endpoint_payload_template: The endpoint_payload_template of this GenerativetestingStartGenerativeModelTestRequest.  # noqa: E501
         :type: str
         """
         if endpoint_payload_template is None:
             raise ValueError("Invalid value for `endpoint_payload_template`, must not be `None`")  # noqa: E501
 
@@ -198,14 +205,35 @@
 
         :param name: The name of this GenerativetestingStartGenerativeModelTestRequest.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
+    @property
+    def mutual_tls_integration_id(self):
+        """Gets the mutual_tls_integration_id of this GenerativetestingStartGenerativeModelTestRequest.  # noqa: E501
+
+
+        :return: The mutual_tls_integration_id of this GenerativetestingStartGenerativeModelTestRequest.  # noqa: E501
+        :rtype: RimeUUID
+        """
+        return self._mutual_tls_integration_id
+
+    @mutual_tls_integration_id.setter
+    def mutual_tls_integration_id(self, mutual_tls_integration_id):
+        """Sets the mutual_tls_integration_id of this GenerativetestingStartGenerativeModelTestRequest.
+
+
+        :param mutual_tls_integration_id: The mutual_tls_integration_id of this GenerativetestingStartGenerativeModelTestRequest.  # noqa: E501
+        :type: RimeUUID
+        """
+
+        self._mutual_tls_integration_id = mutual_tls_integration_id
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/generativetesting_threat.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/generativetesting_threat.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/googlerpc_status.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_level.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/integration_integration_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/integration_integration_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/integration_integration_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     HUGGINGFACE = "INTEGRATION_TYPE_HUGGINGFACE"
     GCS = "INTEGRATION_TYPE_GCS"
     AZURE_CLIENT_SECRET = "INTEGRATION_TYPE_AZURE_CLIENT_SECRET"
     AZURE_WORKLOAD_IDENTITY = "INTEGRATION_TYPE_AZURE_WORKLOAD_IDENTITY"
     INTERNAL_OPENAI_API_KEY = "INTEGRATION_TYPE_INTERNAL_OPENAI_API_KEY"
     OPENAI_API = "INTEGRATION_TYPE_OPENAI_API"
     HTTP_AUTH = "INTEGRATION_TYPE_HTTP_AUTH"
+    MUTUAL_TLS = "INTEGRATION_TYPE_MUTUAL_TLS"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/job_data_generative_model_test.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_job_data_generative_model_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,114 +11,140 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class JobDataGenerativeModelTest(object):
+class RimeJobDataGenerativeModelTest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'workspace_id': 'RimeUUID',
         'progress': 'RimeGenerativeModelTestProgress',
-        'name': 'str'
+        'name': 'str',
+        'url': 'str'
     }
 
     attribute_map = {
         'workspace_id': 'workspaceId',
         'progress': 'progress',
-        'name': 'name'
+        'name': 'name',
+        'url': 'url'
     }
 
-    def __init__(self, workspace_id=None, progress=None, name=None):  # noqa: E501
-        """JobDataGenerativeModelTest - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, workspace_id=None, progress=None, name=None, url=None):  # noqa: E501
+        """RimeJobDataGenerativeModelTest - a model defined in Swagger"""  # noqa: E501
         self._workspace_id = None
         self._progress = None
         self._name = None
+        self._url = None
         self.discriminator = None
         if workspace_id is not None:
             self.workspace_id = workspace_id
         if progress is not None:
             self.progress = progress
         if name is not None:
             self.name = name
+        if url is not None:
+            self.url = url
 
     @property
     def workspace_id(self):
-        """Gets the workspace_id of this JobDataGenerativeModelTest.  # noqa: E501
+        """Gets the workspace_id of this RimeJobDataGenerativeModelTest.  # noqa: E501
 
 
-        :return: The workspace_id of this JobDataGenerativeModelTest.  # noqa: E501
+        :return: The workspace_id of this RimeJobDataGenerativeModelTest.  # noqa: E501
         :rtype: RimeUUID
         """
         return self._workspace_id
 
     @workspace_id.setter
     def workspace_id(self, workspace_id):
-        """Sets the workspace_id of this JobDataGenerativeModelTest.
+        """Sets the workspace_id of this RimeJobDataGenerativeModelTest.
 
 
-        :param workspace_id: The workspace_id of this JobDataGenerativeModelTest.  # noqa: E501
+        :param workspace_id: The workspace_id of this RimeJobDataGenerativeModelTest.  # noqa: E501
         :type: RimeUUID
         """
 
         self._workspace_id = workspace_id
 
     @property
     def progress(self):
-        """Gets the progress of this JobDataGenerativeModelTest.  # noqa: E501
+        """Gets the progress of this RimeJobDataGenerativeModelTest.  # noqa: E501
 
 
-        :return: The progress of this JobDataGenerativeModelTest.  # noqa: E501
+        :return: The progress of this RimeJobDataGenerativeModelTest.  # noqa: E501
         :rtype: RimeGenerativeModelTestProgress
         """
         return self._progress
 
     @progress.setter
     def progress(self, progress):
-        """Sets the progress of this JobDataGenerativeModelTest.
+        """Sets the progress of this RimeJobDataGenerativeModelTest.
 
 
-        :param progress: The progress of this JobDataGenerativeModelTest.  # noqa: E501
+        :param progress: The progress of this RimeJobDataGenerativeModelTest.  # noqa: E501
         :type: RimeGenerativeModelTestProgress
         """
 
         self._progress = progress
 
     @property
     def name(self):
-        """Gets the name of this JobDataGenerativeModelTest.  # noqa: E501
+        """Gets the name of this RimeJobDataGenerativeModelTest.  # noqa: E501
 
 
-        :return: The name of this JobDataGenerativeModelTest.  # noqa: E501
+        :return: The name of this RimeJobDataGenerativeModelTest.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this JobDataGenerativeModelTest.
+        """Sets the name of this RimeJobDataGenerativeModelTest.
 
 
-        :param name: The name of this JobDataGenerativeModelTest.  # noqa: E501
+        :param name: The name of this RimeJobDataGenerativeModelTest.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
+    @property
+    def url(self):
+        """Gets the url of this RimeJobDataGenerativeModelTest.  # noqa: E501
+
+
+        :return: The url of this RimeJobDataGenerativeModelTest.  # noqa: E501
+        :rtype: str
+        """
+        return self._url
+
+    @url.setter
+    def url(self, url):
+        """Sets the url of this RimeJobDataGenerativeModelTest.
+
+
+        :param url: The url of this RimeJobDataGenerativeModelTest.  # noqa: E501
+        :type: str
+        """
+
+        self._url = url
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
@@ -132,15 +158,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(JobDataGenerativeModelTest, dict):
+        if issubclass(RimeJobDataGenerativeModelTest, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +174,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, JobDataGenerativeModelTest):
+        if not isinstance(other, RimeJobDataGenerativeModelTest):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/job_data_scan.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/job_data_scan.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/language_detection_details_language_substring.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/language_detection_details_language_substring.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_file_scan_results_request_file_scan_query.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_file_scan_results_request_file_scan_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_firewall_instances_request_list_firewall_instances_query.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_firewall_instances_request_list_firewall_instances_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/model_model.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/model_model.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_monitor.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_threshold.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_threshold.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitor_transform.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitor_transform.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/notification_digest_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/notification_digest_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/notification_notification.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/notification_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/notification_notification_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/notification_notification_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/notification_object_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/notification_object_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/pii_detection_details_flagged_entity.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/pii_detection_details_flagged_entity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_activate_schedule_for_project_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_activate_schedule_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_create_project_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_create_project_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_create_project_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_create_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_deactivate_schedule_for_project_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_deactivate_schedule_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_get_project_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_get_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_owner_details.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_project.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_project_status.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_project_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_project_with_details.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_project_with_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_schedule_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_schedule_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_update_project_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_update_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/protobuf_any.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_connection_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_connection_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_params.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_data_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_data_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_metadata.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_open_ai_chat_completion_model_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_open_ai_chat_completion_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_pred_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_pred_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registry_validity_status.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registry_validity_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/repo_metadata_reputation.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/repo_metadata_reputation.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_actor_role.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_actor_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_agent.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent_desired_state.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_agent_desired_state.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent_status.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_agent_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_agent_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_agent_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_attack_objective.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_attack_objective.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_category_metric.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_category_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_config_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_config_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_agent_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_firewall_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_agent_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_firewall_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_schedule_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_schedule_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_schedule_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_schedule_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_schedule_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_schedule_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_detailed_upgrade_status.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_detailed_upgrade_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_failing_row.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_failing_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_feature_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_feature_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_float_list.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_float_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_generative_model_test_progress.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,61 +11,35 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeGenerativeModelTestProgress(object):
+class RimeListWorkspacesRequestQuery(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'attacks_attempted': 'str'
     }
 
     attribute_map = {
-        'attacks_attempted': 'attacksAttempted'
     }
 
-    def __init__(self, attacks_attempted=None):  # noqa: E501
-        """RimeGenerativeModelTestProgress - a model defined in Swagger"""  # noqa: E501
-        self._attacks_attempted = None
+    def __init__(self):  # noqa: E501
+        """RimeListWorkspacesRequestQuery - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
-        if attacks_attempted is not None:
-            self.attacks_attempted = attacks_attempted
-
-    @property
-    def attacks_attempted(self):
-        """Gets the attacks_attempted of this RimeGenerativeModelTestProgress.  # noqa: E501
-
-
-        :return: The attacks_attempted of this RimeGenerativeModelTestProgress.  # noqa: E501
-        :rtype: str
-        """
-        return self._attacks_attempted
-
-    @attacks_attempted.setter
-    def attacks_attempted(self, attacks_attempted):
-        """Sets the attacks_attempted of this RimeGenerativeModelTestProgress.
-
-
-        :param attacks_attempted: The attacks_attempted of this RimeGenerativeModelTestProgress.  # noqa: E501
-        :type: str
-        """
-
-        self._attacks_attempted = attacks_attempted
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeGenerativeModelTestProgress, dict):
+        if issubclass(RimeListWorkspacesRequestQuery, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeGenerativeModelTestProgress):
+        if not isinstance(other, RimeListWorkspacesRequestQuery):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_file_scan_result_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_file_scan_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_schedule_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_schedule_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_upgrade_for_agent_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_upgrade_for_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_image_reference.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_image_reference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_int_list.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_int_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_integration_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_integration_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_data.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_job_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'stress': 'JobDataStressTest',
         'continuous_inc': 'JobDataContinuousIncrementalTest',
         'file_scan': 'JobDataScan',
         'cross_plane_res': 'CrossplanetaskCrossPlaneResponse',
-        'generative_model': 'JobDataGenerativeModelTest'
+        'generative_model': 'RimeJobDataGenerativeModelTest'
     }
 
     attribute_map = {
         'stress': 'stress',
         'continuous_inc': 'continuousInc',
         'file_scan': 'fileScan',
         'cross_plane_res': 'crossPlaneRes',
@@ -148,25 +148,25 @@
 
     @property
     def generative_model(self):
         """Gets the generative_model of this RimeJobData.  # noqa: E501
 
 
         :return: The generative_model of this RimeJobData.  # noqa: E501
-        :rtype: JobDataGenerativeModelTest
+        :rtype: RimeJobDataGenerativeModelTest
         """
         return self._generative_model
 
     @generative_model.setter
     def generative_model(self, generative_model):
         """Sets the generative_model of this RimeJobData.
 
 
         :param generative_model: The generative_model of this RimeJobData.  # noqa: E501
-        :type: JobDataGenerativeModelTest
+        :type: RimeJobDataGenerativeModelTest
         """
 
         self._generative_model = generative_model
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_job_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_job_view.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_job_view.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_language.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_language.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_license_feature.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_license_feature.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_license_limit.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_license_limit.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_limit_status.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_limit_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_firewall_instances_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_firewall_instances_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeListWorkspacesRequestQuery(object):
+class RimeSendRIEmailResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeListWorkspacesRequestQuery - a model defined in Swagger"""  # noqa: E501
+        """RimeSendRIEmailResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeListWorkspacesRequestQuery, dict):
+        if issubclass(RimeSendRIEmailResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeListWorkspacesRequestQuery):
+        if not isinstance(other, RimeSendRIEmailResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_managed_image.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_managed_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_managed_image_package_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_managed_image_package_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_card.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_task.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_model_task.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_named_double.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_named_double.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_order.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_order.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_firewall_agent_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_firewall_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_firewall_agent_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_firewall_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_safe_url.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_safe_url.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_search_spec.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_search_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeSendRIEmailResponse(object):
+class RimeStorePredictionsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeSendRIEmailResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeStorePredictionsResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeSendRIEmailResponse, dict):
+        if issubclass(RimeStorePredictionsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeSendRIEmailResponse):
+        if not isinstance(other, RimeStorePredictionsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_severity.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_str_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,35 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeStorePredictionsResponse(object):
+class RimeStrList(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'values': 'list[str]'
     }
 
     attribute_map = {
+        'values': 'values'
     }
 
-    def __init__(self):  # noqa: E501
-        """RimeStorePredictionsResponse - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, values=None):  # noqa: E501
+        """RimeStrList - a model defined in Swagger"""  # noqa: E501
+        self._values = None
         self.discriminator = None
+        if values is not None:
+            self.values = values
+
+    @property
+    def values(self):
+        """Gets the values of this RimeStrList.  # noqa: E501
+
+
+        :return: The values of this RimeStrList.  # noqa: E501
+        :rtype: list[str]
+        """
+        return self._values
+
+    @values.setter
+    def values(self, values):
+        """Sets the values of this RimeStrList.
+
+
+        :param values: The values of this RimeStrList.  # noqa: E501
+        :type: list[str]
+        """
+
+        self._values = values
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -54,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeStorePredictionsResponse, dict):
+        if issubclass(RimeStrList, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeStorePredictionsResponse):
+        if not isinstance(other, RimeStrList):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_str_list.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,61 +11,41 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeStrList(object):
+class RimeTestType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    STRESS_TESTING_UNSPECIFIED = "TEST_TYPE_STRESS_TESTING_UNSPECIFIED"
+    CONTINUOUS_TESTING = "TEST_TYPE_CONTINUOUS_TESTING"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'values': 'list[str]'
     }
 
     attribute_map = {
-        'values': 'values'
     }
 
-    def __init__(self, values=None):  # noqa: E501
-        """RimeStrList - a model defined in Swagger"""  # noqa: E501
-        self._values = None
+    def __init__(self):  # noqa: E501
+        """RimeTestType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
-        if values is not None:
-            self.values = values
-
-    @property
-    def values(self):
-        """Gets the values of this RimeStrList.  # noqa: E501
-
-
-        :return: The values of this RimeStrList.  # noqa: E501
-        :rtype: list[str]
-        """
-        return self._values
-
-    @values.setter
-    def values(self, values):
-        """Sets the values of this RimeStrList.
-
-
-        :param values: The values of this RimeStrList.  # noqa: E501
-        :type: list[str]
-        """
-
-        self._values = values
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +60,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeStrList, dict):
+        if issubclass(RimeTestType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +76,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeStrList):
+        if not isinstance(other, RimeTestType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_subject_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_subject_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_suggestion.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_suggestion.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_table_column.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_table_column.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_metric.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_test_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/user_role.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,40 +11,42 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeTestType(object):
+class UserRole(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    STRESS_TESTING_UNSPECIFIED = "TEST_TYPE_STRESS_TESTING_UNSPECIFIED"
-    CONTINUOUS_TESTING = "TEST_TYPE_CONTINUOUS_TESTING"
+    UNSPECIFIED = "ROLE_UNSPECIFIED"
+    ADMIN = "ROLE_ADMIN"
+    TRIAL_USER = "ROLE_TRIAL_USER"
+    SUPPORT = "ROLE_SUPPORT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeTestType - a model defined in Swagger"""  # noqa: E501
+        """UserRole - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -60,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeTestType, dict):
+        if issubclass(UserRole, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -76,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeTestType):
+        if not isinstance(other, UserRole):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_time_interval.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_time_interval.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_token_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_token_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     """
     allowed enum values
     """
     UNSPECIFIED = "TOKEN_TYPE_UNSPECIFIED"
     USER = "TOKEN_TYPE_USER"
     INTERNAL_AGENT = "TOKEN_TYPE_INTERNAL_AGENT"
     EXTERNAL_AGENT = "TOKEN_TYPE_EXTERNAL_AGENT"
+    FIREWALL_AGENT = "TOKEN_TYPE_FIREWALL_AGENT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_toxicity_threat_category.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_toxicity_threat_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_schedule_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_schedule_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_upgrade_status_for_agent_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_upgrade_status_for_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_upgrade_agent_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_upgrade_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_upgrade_status.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_upgrade_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_role.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_uuid.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_uuid.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_workspace.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/role_users_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/role_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/role_workspace_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/role_workspace_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata_model_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rule_output_rule_evaluation_metadata_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_activate_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_activate_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_deactivate_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_deactivate_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schedule_schedule.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schedule_schedule.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schedules_schedule_schedule_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schedules_schedule_schedule_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schemafilescanning_package_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schemafilescanning_package_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schemanotification_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schemanotification_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/schemaregistry_model_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/schemaregistry_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/statedb_job_status.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/statedb_job_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_category_results_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_get_category_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/user_private_info.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/user_private_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/user_role.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/rime_attack_technique.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,42 +11,47 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UserRole(object):
+class RimeAttackTechnique(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "ROLE_UNSPECIFIED"
-    ADMIN = "ROLE_ADMIN"
-    TRIAL_USER = "ROLE_TRIAL_USER"
-    SUPPORT = "ROLE_SUPPORT"
+    UNSPECIFIED = "ATTACK_TECHNIQUE_UNSPECIFIED"
+    TASTLE = "ATTACK_TECHNIQUE_TASTLE"
+    SYSTEM_INSTRUCTIONS = "ATTACK_TECHNIQUE_SYSTEM_INSTRUCTIONS"
+    ROLE_PLAY_JAIL_BREAKS = "ATTACK_TECHNIQUE_ROLE_PLAY_JAIL_BREAKS"
+    IGNORE_INSTRUCTIONS = "ATTACK_TECHNIQUE_IGNORE_INSTRUCTIONS"
+    GLITCH_TOKENS = "ATTACK_TECHNIQUE_GLITCH_TOKENS"
+    DRA_JAILBREAK = "ATTACK_TECHNIQUE_DRA_JAILBREAK"
+    DEEP_INCEPTION = "ATTACK_TECHNIQUE_DEEP_INCEPTION"
+    SIMPLE_ADAPTIVE_JAILBREAK = "ATTACK_TECHNIQUE_SIMPLE_ADAPTIVE_JAILBREAK"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """UserRole - a model defined in Swagger"""  # noqa: E501
+        """RimeAttackTechnique - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -62,15 +67,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UserRole, dict):
+        if issubclass(RimeAttackTechnique, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +83,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UserRole):
+        if not isinstance(other, RimeAttackTechnique):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/user_user_detail.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/user_user_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body1.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body1.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/validate_request_input.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/validate_request_input.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/validate_request_output.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/validate_request_output.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/validate_response_processed_request.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/validate_response_processed_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/validate_response_product_metadata.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/validate_response_product_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/swagger/swagger_client/rest.py` & `rime_sdk-2.8.0rc9/rime_sdk/swagger/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/test_batch.py` & `rime_sdk-2.8.0rc9/rime_sdk/test_batch.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk/test_run.py` & `rime_sdk-2.8.0rc9/rime_sdk/test_run.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.8.0rc8/rime_sdk.egg-info/PKG-INFO` & `rime_sdk-2.8.0rc9/rime_sdk.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime-sdk
-Version: 2.8.0rc8
+Version: 2.8.0rc9
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.8.0rc8/rime_sdk.egg-info/SOURCES.txt` & `rime_sdk-2.8.0rc9/rime_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py
 rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py
 rime_sdk/swagger/swagger_client/models/apigenerativefirewall_list_firewall_instances_response.py
 rime_sdk/swagger/swagger_client/models/apigenerativefirewall_standard_info.py
 rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
 rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
 rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
+rime_sdk/swagger/swagger_client/models/code_detection_details_code_substring.py
 rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py
 rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py
 rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py
 rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
 rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
 rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
@@ -128,19 +129,22 @@
 rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
 rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
 rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
 rime_sdk/swagger/swagger_client/models/firewallinstance_firewall_instance_firewall_instance_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/flagged_substring_request_body_component.py
 rime_sdk/swagger/swagger_client/models/generative_testing_result_example.py
+rime_sdk/swagger/swagger_client/models/generativefirewall_code_detection_details.py
+rime_sdk/swagger/swagger_client/models/generativefirewall_code_detection_rule_config.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_request.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_response.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_custom_pii_entity.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_denial_of_service_rule_config.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py
+rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_deployment_config.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_info.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_status.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_config.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_type.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_tokenizer.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_flagged_substring.py
 rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_effective_config_response.py
@@ -176,19 +180,19 @@
 rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
 rime_sdk/swagger/swagger_client/models/integration_integration_level.py
 rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
 rime_sdk/swagger/swagger_client/models/integration_integration_type.py
 rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
 rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
-rime_sdk/swagger/swagger_client/models/job_data_generative_model_test.py
 rime_sdk/swagger/swagger_client/models/job_data_scan.py
 rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
 rime_sdk/swagger/swagger_client/models/language_detection_details_language_substring.py
 rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
+rime_sdk/swagger/swagger_client/models/list_api_tokens_request_list_api_tokens_query.py
 rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
 rime_sdk/swagger/swagger_client/models/list_file_scan_results_request_file_scan_query.py
 rime_sdk/swagger/swagger_client/models/list_firewall_instances_request_list_firewall_instances_query.py
 rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
 rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
 rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
 rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
@@ -281,14 +285,15 @@
 rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
 rime_sdk/swagger/swagger_client/models/rime_agent.py
 rime_sdk/swagger/swagger_client/models/rime_agent_desired_state.py
 rime_sdk/swagger/swagger_client/models/rime_agent_status.py
 rime_sdk/swagger/swagger_client/models/rime_agent_type.py
 rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
 rime_sdk/swagger/swagger_client/models/rime_attack_objective.py
+rime_sdk/swagger/swagger_client/models/rime_attack_technique.py
 rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
 rime_sdk/swagger/swagger_client/models/rime_category_metric.py
 rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
 rime_sdk/swagger/swagger_client/models/rime_config_type.py
 rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
 rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
 rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
@@ -374,14 +379,15 @@
 rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
 rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
 rime_sdk/swagger/swagger_client/models/rime_image_reference.py
 rime_sdk/swagger/swagger_client/models/rime_int_list.py
 rime_sdk/swagger/swagger_client/models/rime_integration_info.py
 rime_sdk/swagger/swagger_client/models/rime_job_data.py
+rime_sdk/swagger/swagger_client/models/rime_job_data_generative_model_test.py
 rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
 rime_sdk/swagger/swagger_client/models/rime_job_type.py
 rime_sdk/swagger/swagger_client/models/rime_job_view.py
 rime_sdk/swagger/swagger_client/models/rime_language.py
 rime_sdk/swagger/swagger_client/models/rime_license_feature.py
 rime_sdk/swagger/swagger_client/models/rime_license_limit.py
 rime_sdk/swagger/swagger_client/models/rime_limit_status.py
@@ -391,14 +397,16 @@
 rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
 rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_firewall_instances_response.py
+rime_sdk/swagger/swagger_client/models/rime_list_gai_test_job_response.py
+rime_sdk/swagger/swagger_client/models/rime_list_gai_test_jobs_request_query.py
 rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
 rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
 rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
```

### Comparing `rime_sdk-2.8.0rc8/setup.py` & `rime_sdk-2.8.0rc9/setup.py`

 * *Files identical despite different names*

