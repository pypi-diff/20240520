# Comparing `tmp/baidu_apollo_proto-0.1.0.tar.gz` & `tmp/baidu_apollo_proto-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baidu_apollo_proto-0.1.0.tar", max compression
+gzip compressed data, was "baidu_apollo_proto-0.1.1.tar", max compression
```

## Comparing `baidu_apollo_proto-0.1.0.tar` & `baidu_apollo_proto-0.1.1.tar`

### file list

```diff
@@ -1,677 +1,607 @@
--rw-r--r--   0        0        0       91 2024-05-06 18:51:38.334406 baidu_apollo_proto-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.270670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/__init__.py
--rw-r--r--   0        0        0       45 2024-05-06 18:47:31.270670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.270670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/__init__.py
--rw-r--r--   0        0        0      341 2024-05-06 18:47:31.270670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.270670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/audio/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/audio/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/audio/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/audio/proto/__init__.pyi
--rw-r--r--   0        0        0     5931 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/audio/proto/audio_common_pb2.py
--rw-r--r--   0        0        0     7018 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/audio/proto/audio_conf_pb2.py
--rw-r--r--   0        0        0     7326 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/audio/proto/audio_event_pb2.py
--rw-r--r--   0        0        0     5788 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/audio/proto/audio_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/bridge/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/bridge/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/bridge/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/bridge/proto/__init__.pyi
--rw-r--r--   0        0        0     7353 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/bridge/proto/udp_bridge_remote_info_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/__init__.pyi
--rw-r--r--   0        0        0     5731 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/canbus_conf_pb2.py
--rw-r--r--   0        0        0    84337 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/ch_pb2.py
--rw-r--r--   0        0        0   361381 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/chassis_detail_pb2.py
--rw-r--r--   0        0        0    79319 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/chassis_pb2.py
--rw-r--r--   0        0        0   113739 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/devkit_pb2.py
--rw-r--r--   0        0        0   201961 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/ge3_pb2.py
--rw-r--r--   0        0        0   442211 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/lexus_pb2.py
--rw-r--r--   0        0        0   157770 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/neolix_edu_pb2.py
--rw-r--r--   0        0        0   112905 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/transit_pb2.py
--rw-r--r--   0        0        0     5016 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/vehicle_parameter_pb2.py
--rw-r--r--   0        0        0   189831 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/wey_pb2.py
--rw-r--r--   0        0        0    65589 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/zhongyun_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/__init__.py
--rw-r--r--   0        0        0      143 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/adapters/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/adapters/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/adapters/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/adapters/proto/__init__.pyi
--rw-r--r--   0        0        0    30410 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/adapters/proto/adapter_config_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/configs/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/configs/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/configs/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/configs/proto/__init__.pyi
--rw-r--r--   0        0        0    36272 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/configs/proto/vehicle_config_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/latency_recorder/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/latency_recorder/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/latency_recorder/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/latency_recorder/proto/__init__.pyi
--rw-r--r--   0        0        0    17470 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/latency_recorder/proto/latency_record_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/monitor_log/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/monitor_log/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/monitor_log/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/monitor_log/proto/__init__.pyi
--rw-r--r--   0        0        0    14328 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/monitor_log/proto/monitor_log_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/proto/__init__.pyi
--rw-r--r--   0        0        0     3408 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/proto/direction_pb2.py
--rw-r--r--   0        0        0     6961 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/proto/drive_event_pb2.py
--rw-r--r--   0        0        0     4717 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/proto/drive_state_pb2.py
--rw-r--r--   0        0        0    16099 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/proto/error_code_pb2.py
--rw-r--r--   0        0        0    15182 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/proto/geometry_pb2.py
--rw-r--r--   0        0        0     7527 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/proto/header_pb2.py
--rw-r--r--   0        0        0    37024 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/proto/pnc_point_pb2.py
--rw-r--r--   0        0        0     6129 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/proto/vehicle_signal_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/util/__init__.py
--rw-r--r--   0        0        0       23 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/util/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/util/testdata/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/util/testdata/__init__.pyi
--rw-r--r--   0        0        0     5475 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/util/testdata/simple_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/vehicle_model/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/vehicle_model/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/vehicle_model/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/vehicle_model/proto/__init__.pyi
--rw-r--r--   0        0        0    11270 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/vehicle_model/proto/vehicle_model_config_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/vehicle_state/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/vehicle_state/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/vehicle_state/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/vehicle_state/proto/__init__.pyi
--rw-r--r--   0        0        0    12732 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/vehicle_state/proto/vehicle_state_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/contrib/__init__.py
--rw-r--r--   0        0        0       25 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/contrib/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/__init__.pyi
--rw-r--r--   0        0        0    14209 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/detection2d_pb2.py
--rw-r--r--   0        0        0     3755 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/detection2darray_pb2.py
--rw-r--r--   0        0        0    11266 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/detection3d_pb2.py
--rw-r--r--   0        0        0     3755 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/detection3darray_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/__init__.pyi
--rw-r--r--   0        0        0     5406 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/calibration_table_pb2.py
--rw-r--r--   0        0        0   119179 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/control_cmd_pb2.py
--rw-r--r--   0        0        0    25084 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/control_common_conf_pb2.py
--rw-r--r--   0        0        0    30378 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/control_conf_pb2.py
--rw-r--r--   0        0        0     4381 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/gain_scheduler_conf_pb2.py
--rw-r--r--   0        0        0     4929 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/input_debug_pb2.py
--rw-r--r--   0        0        0    20412 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/lat_controller_conf_pb2.py
--rw-r--r--   0        0        0     4063 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/leadlag_conf_pb2.py
--rw-r--r--   0        0        0     6508 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/local_view_pb2.py
--rw-r--r--   0        0        0    18231 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/lon_controller_conf_pb2.py
--rw-r--r--   0        0        0    19142 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/mpc_controller_conf_pb2.py
--rw-r--r--   0        0        0     8850 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/mrac_conf_pb2.py
--rw-r--r--   0        0        0     5556 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/pad_msg_pb2.py
--rw-r--r--   0        0        0     5897 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/pid_conf_pb2.py
--rw-r--r--   0        0        0     7562 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/preprocessor_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/data/__init__.py
--rw-r--r--   0        0        0       27 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/data/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/data/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/data/proto/__init__.pyi
--rw-r--r--   0        0        0    37510 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/data/proto/frame_pb2.py
--rw-r--r--   0        0        0    32594 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/data/proto/static_info_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/data/tools/__init__.py
--rw-r--r--   0        0        0       29 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/data/tools/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/data/tools/smart_recorder/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/data/tools/smart_recorder/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/data/tools/smart_recorder/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/data/tools/smart_recorder/proto/__init__.pyi
--rw-r--r--   0        0        0     5506 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/data/tools/smart_recorder/proto/smart_recorder_status_pb2.py
--rw-r--r--   0        0        0    11440 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/data/tools/smart_recorder/proto/smart_recorder_triggers_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/__init__.py
--rw-r--r--   0        0        0       29 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/backend/__init__.py
--rw-r--r--   0        0        0       21 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/backend/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/proto/__init__.pyi
--rw-r--r--   0        0        0     3801 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/proto/daemon_cmd_pb2.py
--rw-r--r--   0        0        0     3129 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/proto/daemon_rpt_pb2.py
--rw-r--r--   0        0        0    14055 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/proto/modem_info_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/__init__.pyi
--rw-r--r--   0        0        0     4111 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/camera_update_pb2.py
--rw-r--r--   0        0        0    30122 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/chart_pb2.py
--rw-r--r--   0        0        0    17879 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/data_collection_table_pb2.py
--rw-r--r--   0        0        0    17773 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/hmi_config_pb2.py
--rw-r--r--   0        0        0    49215 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/hmi_mode_pb2.py
--rw-r--r--   0        0        0    18407 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/hmi_status_pb2.py
--rw-r--r--   0        0        0     2142 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/point_cloud_pb2.py
--rw-r--r--   0        0        0    16304 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/preprocess_table_pb2.py
--rw-r--r--   0        0        0   113277 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/simulation_world_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/__init__.py
--rw-r--r--   0        0        0      139 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/camera/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/camera/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/camera/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/camera/proto/__init__.pyi
--rw-r--r--   0        0        0    24718 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/camera/proto/config_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/canbus/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/canbus/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/canbus/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/canbus/proto/__init__.pyi
--rw-r--r--   0        0        0    12311 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/canbus/proto/can_card_parameter_pb2.py
--rw-r--r--   0        0        0     4163 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/canbus/proto/sensor_canbus_conf_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/__init__.pyi
--rw-r--r--   0        0        0    41814 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/config_pb2.py
--rw-r--r--   0        0        0    33208 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/gnss_best_pose_pb2.py
--rw-r--r--   0        0        0    14191 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/gnss_pb2.py
--rw-r--r--   0        0        0    74576 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/gnss_raw_observation_pb2.py
--rw-r--r--   0        0        0    13692 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/gnss_status_pb2.py
--rw-r--r--   0        0        0    14308 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/heading_pb2.py
--rw-r--r--   0        0        0     5514 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/imu_pb2.py
--rw-r--r--   0        0        0    15728 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/ins_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/__init__.pyi
--rw-r--r--   0        0        0     5789 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/config_pb2.py
--rw-r--r--   0        0        0     9720 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/hesai_config_pb2.py
--rw-r--r--   0        0        0     8019 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/hesai_pb2.py
--rw-r--r--   0        0        0     5311 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/lidar_parameter_pb2.py
--rw-r--r--   0        0        0    11250 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/robosense_config_pb2.py
--rw-r--r--   0        0        0     6785 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/robosense_pb2.py
--rw-r--r--   0        0        0    26240 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/velodyne_config_pb2.py
--rw-r--r--   0        0        0    12962 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/velodyne_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/microphone/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/microphone/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/microphone/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/microphone/proto/__init__.pyi
--rw-r--r--   0        0        0     6840 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/microphone/proto/audio_pb2.py
--rw-r--r--   0        0        0    10763 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/microphone/proto/microphone_config_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/__init__.pyi
--rw-r--r--   0        0        0    34082 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/conti_radar_pb2.py
--rw-r--r--   0        0        0   265003 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/delphi_esr_pb2.py
--rw-r--r--   0        0        0    86336 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/mobileye_pb2.py
--rw-r--r--   0        0        0    10243 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/pointcloud_pb2.py
--rw-r--r--   0        0        0    34642 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/racobit_radar_pb2.py
--rw-r--r--   0        0        0    22066 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/radar_pb2.py
--rw-r--r--   0        0        0    26133 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/sensor_image_pb2.py
--rw-r--r--   0        0        0    73970 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/smartereye_pb2.py
--rw-r--r--   0        0        0     3067 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/ultrasonic_radar_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/__init__.py
--rw-r--r--   0        0        0       59 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/conti_radar/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/conti_radar/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/conti_radar/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/conti_radar/proto/__init__.pyi
--rw-r--r--   0        0        0    26377 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/conti_radar/proto/conti_radar_conf_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/racobit_radar/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/racobit_radar/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/racobit_radar/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/racobit_radar/proto/__init__.pyi
--rw-r--r--   0        0        0    25143 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/racobit_radar/proto/racobit_radar_conf_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/ultrasonic_radar/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/ultrasonic_radar/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/ultrasonic_radar/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/ultrasonic_radar/proto/__init__.pyi
--rw-r--r--   0        0        0     7216 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/ultrasonic_radar/proto/ultrasonic_radar_conf_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/smartereye/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/smartereye/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/smartereye/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/smartereye/proto/__init__.pyi
--rw-r--r--   0        0        0    26306 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/smartereye/proto/config_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/tools/__init__.py
--rw-r--r--   0        0        0       31 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/tools/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/tools/image_decompress/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/tools/image_decompress/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/tools/image_decompress/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/tools/image_decompress/proto/__init__.pyi
--rw-r--r--   0        0        0     2149 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/tools/image_decompress/proto/config_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/video/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/video/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/video/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/video/proto/__init__.pyi
--rw-r--r--   0        0        0    20844 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/video/proto/video_h265cfg_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/guardian/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/guardian/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/guardian/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/guardian/proto/__init__.pyi
--rw-r--r--   0        0        0     3602 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/guardian/proto/guardian_conf_pb2.py
--rw-r--r--   0        0        0     3572 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/guardian/proto/guardian_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/__init__.pyi
--rw-r--r--   0        0        0    22890 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/gnss_pnt_result_pb2.py
--rw-r--r--   0        0        0     3357 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/gps_pb2.py
--rw-r--r--   0        0        0     3447 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/imu_pb2.py
--rw-r--r--   0        0        0     3538 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/localization_config_pb2.py
--rw-r--r--   0        0        0    20892 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/localization_pb2.py
--rw-r--r--   0        0        0    43603 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/localization_status_pb2.py
--rw-r--r--   0        0        0    13252 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/measure_pb2.py
--rw-r--r--   0        0        0     8652 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/pose_pb2.py
--rw-r--r--   0        0        0     9639 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/rtk_config_pb2.py
--rw-r--r--   0        0        0     6472 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/sins_pva_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/__init__.py
--rw-r--r--   0        0        0       41 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/__init__.pyi
--rw-r--r--   0        0        0     4119 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_clear_area_pb2.py
--rw-r--r--   0        0        0     4116 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_crosswalk_pb2.py
--rw-r--r--   0        0        0    10081 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_geometry_pb2.py
--rw-r--r--   0        0        0     1927 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_id_pb2.py
--rw-r--r--   0        0        0     6872 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_junction_pb2.py
--rw-r--r--   0        0        0    33595 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_lane_pb2.py
--rw-r--r--   0        0        0    33378 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_overlap_pb2.py
--rw-r--r--   0        0        0     7912 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_parking_space_pb2.py
--rw-r--r--   0        0        0    24567 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_pb2.py
--rw-r--r--   0        0        0    13655 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_pnc_junction_pb2.py
--rw-r--r--   0        0        0    19114 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_road_pb2.py
--rw-r--r--   0        0        0     3763 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_rsu_pb2.py
--rw-r--r--   0        0        0    17405 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_signal_pb2.py
--rw-r--r--   0        0        0     4117 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_speed_bump_pb2.py
--rw-r--r--   0        0        0     5329 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_speed_control_pb2.py
--rw-r--r--   0        0        0     6906 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_stop_sign_pb2.py
--rw-r--r--   0        0        0     4119 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_yield_sign_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/relative_map/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/relative_map/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/relative_map/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/relative_map/proto/__init__.pyi
--rw-r--r--   0        0        0    13726 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/relative_map/proto/navigation_pb2.py
--rw-r--r--   0        0        0     8676 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/relative_map/proto/navigator_config_pb2.py
--rw-r--r--   0        0        0    16130 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/relative_map/proto/relative_map_config_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/tools/__init__.py
--rw-r--r--   0        0        0       30 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/tools/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/proto/__init__.pyi
--rw-r--r--   0        0        0    38508 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/proto/collection_check_message_pb2.py
--rw-r--r--   0        0        0     9393 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/proto/collection_error_code_pb2.py
--rw-r--r--   0        0        0     5174 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/proto/collection_service_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/monitor/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/monitor/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/monitor/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/monitor/proto/__init__.pyi
--rw-r--r--   0        0        0    24463 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/monitor/proto/system_status_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/__init__.py
--rw-r--r--   0        0        0       52 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/camera/__init__.py
--rw-r--r--   0        0        0       38 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/camera/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/camera/app/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/camera/app/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/camera/app/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/camera/app/proto/__init__.pyi
--rw-r--r--   0        0        0    38941 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/camera/app/proto/perception_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/camera/common/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/camera/common/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/camera/common/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/camera/common/proto/__init__.pyi
--rw-r--r--   0        0        0    16546 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/camera/common/proto/object_template_meta_schema_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/camera/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/camera/proto/__init__.pyi
--rw-r--r--   0        0        0    66169 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/camera/proto/yolo_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/fusion/__init__.py
--rw-r--r--   0        0        0       18 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/fusion/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/lidar/__init__.py
--rw-r--r--   0        0        0       23 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/lidar/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/lidar/app/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/lidar/app/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/lidar/app/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/lidar/app/proto/__init__.pyi
--rw-r--r--   0        0        0     4615 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/lidar/app/proto/lidar_obstacle_detection_config_pb2.py
--rw-r--r--   0        0        0     3968 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/lidar/app/proto/lidar_obstacle_tracking_config_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/onboard/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/onboard/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/__init__.pyi
--rw-r--r--   0        0        0    25687 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/fusion_camera_detection_component_pb2.py
--rw-r--r--   0        0        0     6847 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/fusion_component_config_pb2.py
--rw-r--r--   0        0        0    15984 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/lane_perception_component_pb2.py
--rw-r--r--   0        0        0     8426 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/lidar_component_config_pb2.py
--rw-r--r--   0        0        0     4595 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/motion_service_pb2.py
--rw-r--r--   0        0        0     7268 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/radar_component_config_pb2.py
--rw-r--r--   0        0        0    16377 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/trafficlights_perception_component_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/__init__.pyi
--rw-r--r--   0        0        0     3797 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/ccrf_type_fusion_config_pb2.py
--rw-r--r--   0        0        0     5384 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/dst_existence_fusion_config_pb2.py
--rw-r--r--   0        0        0     9917 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/dst_type_fusion_config_pb2.py
--rw-r--r--   0        0        0     5224 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/fused_classifier_config_pb2.py
--rw-r--r--   0        0        0     4237 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/map_manager_config_pb2.py
--rw-r--r--   0        0        0    21526 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/motion_service_pb2.py
--rw-r--r--   0        0        0     4499 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/pbf_tracker_config_pb2.py
--rw-r--r--   0        0        0    41389 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_camera_pb2.py
--rw-r--r--   0        0        0    35522 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_config_schema_pb2.py
--rw-r--r--   0        0        0     6065 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_lane_pb2.py
--rw-r--r--   0        0        0    74709 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_obstacle_pb2.py
--rw-r--r--   0        0        0     7491 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_ultrasonic_pb2.py
--rw-r--r--   0        0        0     9457 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/probabilistic_fusion_config_pb2.py
--rw-r--r--   0        0        0     4484 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/roi_boundary_filter_config_pb2.py
--rw-r--r--   0        0        0   636938 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/rt_pb2.py
--rw-r--r--   0        0        0    12133 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/sensor_meta_schema_pb2.py
--rw-r--r--   0        0        0     2770 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/tracker_config_pb2.py
--rw-r--r--   0        0        0    29561 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/traffic_light_detection_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/__init__.py
--rw-r--r--   0        0        0       19 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/__init__.pyi
--rw-r--r--   0        0        0    34971 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/auto_tuning_model_input_pb2.py
--rw-r--r--   0        0        0    38141 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/auto_tuning_raw_feature_pb2.py
--rw-r--r--   0        0        0    91347 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/decision_pb2.py
--rw-r--r--   0        0        0     7569 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/ipopt_return_status_pb2.py
--rw-r--r--   0        0        0     6012 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/lattice_structure_pb2.py
--rw-r--r--   0        0        0    86626 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/learning_data_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/math/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/math/__init__.pyi
--rw-r--r--   0        0        0     7833 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/math/cos_theta_smoother_config_pb2.py
--rw-r--r--   0        0        0    16221 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/math/fem_pos_deviation_smoother_config_pb2.py
--rw-r--r--   0        0        0    12481 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/math/qp_problem_pb2.py
--rw-r--r--   0        0        0    87356 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/open_space_task_config_pb2.py
--rw-r--r--   0        0        0     5698 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/pad_msg_pb2.py
--rw-r--r--   0        0        0    87377 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/planner_open_space_config_pb2.py
--rw-r--r--   0        0        0   168243 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_config_pb2.py
--rw-r--r--   0        0        0   138187 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_internal_pb2.py
--rw-r--r--   0        0        0    39948 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_pb2.py
--rw-r--r--   0        0        0     9743 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_semantic_map_config_pb2.py
--rw-r--r--   0        0        0     9860 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_stats_pb2.py
--rw-r--r--   0        0        0    69955 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_status_pb2.py
--rw-r--r--   0        0        0    29328 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/reference_line_smoother_config_pb2.py
--rw-r--r--   0        0        0     4994 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/sl_boundary_pb2.py
--rw-r--r--   0        0        0     6589 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/st_drivable_boundary_pb2.py
--rw-r--r--   0        0        0   127062 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/task_config_pb2.py
--rw-r--r--   0        0        0    42482 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/traffic_rule_config_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/__init__.pyi
--rw-r--r--   0        0        0    66099 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/feature_pb2.py
--rw-r--r--   0        0        0     9398 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/fnn_model_base_pb2.py
--rw-r--r--   0        0        0     6177 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/fnn_vehicle_model_pb2.py
--rw-r--r--   0        0        0    47822 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/lane_graph_pb2.py
--rw-r--r--   0        0        0    59580 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/network_layers_pb2.py
--rw-r--r--   0        0        0    11781 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/network_model_pb2.py
--rw-r--r--   0        0        0    25535 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/offline_features_pb2.py
--rw-r--r--   0        0        0    26108 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/prediction_conf_pb2.py
--rw-r--r--   0        0        0    23511 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/prediction_obstacle_pb2.py
--rw-r--r--   0        0        0     5909 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/prediction_point_pb2.py
--rw-r--r--   0        0        0     5247 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/scenario_pb2.py
--rw-r--r--   0        0        0    11980 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/vector_net_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/routing/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/routing/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/routing/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/routing/proto/__init__.pyi
--rw-r--r--   0        0        0     5981 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/routing/proto/poi_pb2.py
--rw-r--r--   0        0        0     8435 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/routing/proto/routing_config_pb2.py
--rw-r--r--   0        0        0    36680 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/routing/proto/routing_pb2.py
--rw-r--r--   0        0        0    18648 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/routing/proto/topo_graph_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/storytelling/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/storytelling/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/storytelling/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/storytelling/proto/__init__.pyi
--rw-r--r--   0        0        0    21807 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/storytelling/proto/story_pb2.py
--rw-r--r--   0        0        0     4553 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/storytelling/proto/storytelling_config_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/task_manager/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/task_manager/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/task_manager/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/task_manager/proto/__init__.pyi
--rw-r--r--   0        0        0     5924 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/task_manager/proto/task_manager_config_pb2.py
--rw-r--r--   0        0        0    18549 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/task_manager/proto/task_manager_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/third_party_perception/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/third_party_perception/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/third_party_perception/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/third_party_perception/proto/__init__.pyi
--rw-r--r--   0        0        0    17334 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/third_party_perception/proto/radar_obstacle_pb2.py
--rw-r--r--   0        0        0     3939 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/third_party_perception/proto/third_party_perception_component_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/__init__.py
--rw-r--r--   0        0        0       56 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/navigator/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/navigator/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/navigator/dbmap/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/navigator/dbmap/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/navigator/dbmap/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/navigator/dbmap/proto/__init__.pyi
--rw-r--r--   0        0        0    18863 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/navigator/dbmap/proto/dbmap_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/prediction/__init__.py
--rw-r--r--   0        0        0       29 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/prediction/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/prediction/data_pipelines/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/prediction/data_pipelines/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/prediction/data_pipelines/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/prediction/data_pipelines/proto/__init__.pyi
--rw-r--r--   0        0        0    47307 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/prediction/data_pipelines/proto/cruise_model_pb2.py
--rw-r--r--   0        0        0    13929 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/prediction/data_pipelines/proto/fnn_model_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/sensor_calibration/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/sensor_calibration/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/sensor_calibration/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/sensor_calibration/proto/__init__.pyi
--rw-r--r--   0        0        0    13399 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/sensor_calibration/proto/extractor_config_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/transform/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/transform/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/transform/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/transform/proto/__init__.pyi
--rw-r--r--   0        0        0     5691 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/transform/proto/static_transform_conf_pb2.py
--rw-r--r--   0        0        0     8909 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/transform/proto/transform_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/__init__.py
--rw-r--r--   0        0        0       20 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/__init__.pyi
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/__init__.pyi
--rw-r--r--   0        0        0    15952 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/fusion_params_pb2.py
--rw-r--r--   0        0        0     5322 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_car_status_pb2.py
--rw-r--r--   0        0        0    10819 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_junction_pb2.py
--rw-r--r--   0        0        0     6130 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_monitor_pb2.py
--rw-r--r--   0        0        0    23335 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_obstacles_pb2.py
--rw-r--r--   0        0        0     7897 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_obu_rsi_pb2.py
--rw-r--r--   0        0        0    19133 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_obu_traffic_light_pb2.py
--rw-r--r--   0        0        0     9397 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_rsi_pb2.py
--rw-r--r--   0        0        0     3258 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_service_car_to_obu_pb2.py
--rw-r--r--   0        0        0     6868 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_service_obu_to_car_pb2.py
--rw-r--r--   0        0        0    18277 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_traffic_light_pb2.py
--rw-r--r--   0        0        0    30751 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_traffic_light_policy_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/__init__.py
--rw-r--r--   0        0        0       45 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/__init__.pyi
--rw-r--r--   0        0        0      178 2024-05-06 18:49:14.513903 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      177 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/__init__.py
--rw-r--r--   0        0        0       26 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/__init__.pyi
--rw-r--r--   0        0        0      186 2024-05-06 18:49:14.513903 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      185 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/__init__.py
--rw-r--r--   0        0        0      412 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/__init__.pyi
--rw-r--r--   0        0        0      198 2024-05-06 18:49:14.513903 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      197 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/audio_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/audio_msgs/__init__.pyi
--rw-r--r--   0        0        0     5953 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/audio_msgs/audio_common_pb2.py
--rw-r--r--   0        0        0     7602 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/audio_msgs/audio_event_pb2.py
--rw-r--r--   0        0        0     6022 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/audio_msgs/audio_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/__init__.pyi
--rw-r--r--   0        0        0      209 2024-05-06 18:49:33.210488 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      208 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     4346 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/__pycache__/drive_state_pb2.cpython-312.pyc
--rw-r--r--   0        0        0    11152 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/__pycache__/error_code_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     7156 2024-05-06 18:49:33.210488 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/__pycache__/geometry_pb2.cpython-310.pyc
--rw-r--r--   0        0        0    11942 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/__pycache__/geometry_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     6402 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/__pycache__/header_pb2.cpython-312.pyc
--rw-r--r--   0        0        0    27084 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/__pycache__/pnc_point_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     3522 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/__pycache__/vehicle_id_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     5437 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/__pycache__/vehicle_signal_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     3428 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/direction_pb2.py
--rw-r--r--   0        0        0     7131 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/drive_event_pb2.py
--rw-r--r--   0        0        0     4770 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/drive_state_pb2.py
--rw-r--r--   0        0        0    16152 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/error_code_pb2.py
--rw-r--r--   0        0        0    15400 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/geometry_pb2.py
--rw-r--r--   0        0        0     7628 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/header_pb2.py
--rw-r--r--   0        0        0    37282 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/pnc_point_pb2.py
--rw-r--r--   0        0        0     3383 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/vehicle_id_pb2.py
--rw-r--r--   0        0        0     6452 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/vehicle_signal_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/chassis_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/chassis_msgs/__init__.pyi
--rw-r--r--   0        0        0      210 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/chassis_msgs/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0    62289 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/chassis_msgs/__pycache__/chassis_pb2.cpython-312.pyc
--rw-r--r--   0        0        0   353927 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/chassis_msgs/chassis_detail_pb2.py
--rw-r--r--   0        0        0    90974 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/chassis_msgs/chassis_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/config_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/config_msgs/__init__.pyi
--rw-r--r--   0        0        0    34037 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/config_msgs/vehicle_config_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/control_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/control_msgs/__init__.pyi
--rw-r--r--   0        0        0   120575 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/control_msgs/control_cmd_pb2.py
--rw-r--r--   0        0        0     5077 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/control_msgs/input_debug_pb2.py
--rw-r--r--   0        0        0     6023 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/control_msgs/pad_msg_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/dreamview_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/dreamview_msgs/__init__.pyi
--rw-r--r--   0        0        0      212 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/dreamview_msgs/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0    22442 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/dreamview_msgs/__pycache__/chart_pb2.cpython-312.pyc
--rw-r--r--   0        0        0    30338 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/dreamview_msgs/chart_pb2.py
--rw-r--r--   0        0        0    36529 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/dreamview_msgs/hmi_status_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/drivers_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/drivers_msgs/__init__.pyi
--rw-r--r--   0        0        0    15211 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/drivers_msgs/can_card_parameter_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/guardian_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/guardian_msgs/__init__.pyi
--rw-r--r--   0        0        0     3729 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/guardian_msgs/guardian_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/__init__.pyi
--rw-r--r--   0        0        0      215 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0    15995 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/__pycache__/localization_pb2.cpython-312.pyc
--rw-r--r--   0        0        0    27664 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/__pycache__/localization_status_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     7292 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/__pycache__/pose_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     3507 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/gps_pb2.py
--rw-r--r--   0        0        0     3620 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/imu_pb2.py
--rw-r--r--   0        0        0    21318 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/localization_pb2.py
--rw-r--r--   0        0        0    43647 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/localization_status_pb2.py
--rw-r--r--   0        0        0     8862 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/pose_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__init__.pyi
--rw-r--r--   0        0        0      207 2024-05-06 18:49:14.513903 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      206 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     2918 2024-05-06 18:49:33.210488 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_clear_area_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     4165 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_clear_area_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     2914 2024-05-06 18:49:48.686973 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_crosswalk_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     4161 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_crosswalk_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     5350 2024-05-06 18:49:33.210488 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_geometry_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     8710 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_geometry_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     1849 2024-05-06 18:49:48.686973 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_id_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2519 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_id_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     3863 2024-05-06 18:49:48.686973 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_junction_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     5869 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_junction_pb2.cpython-312.pyc
--rw-r--r--   0        0        0    14044 2024-05-06 18:49:48.686973 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_lane_pb2.cpython-310.pyc
--rw-r--r--   0        0        0    23584 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_lane_pb2.cpython-312.pyc
--rw-r--r--   0        0        0    14611 2024-05-06 18:49:48.686973 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_overlap_pb2.cpython-310.pyc
--rw-r--r--   0        0        0    26023 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_overlap_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     4369 2024-05-06 18:49:48.690973 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_parking_space_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     6817 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_parking_space_pb2.cpython-312.pyc
--rw-r--r--   0        0        0    11839 2024-05-06 18:49:14.513903 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_pb2.cpython-310.pyc
--rw-r--r--   0        0        0    18603 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     6643 2024-05-06 18:49:48.690973 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_pnc_junction_pb2.cpython-310.pyc
--rw-r--r--   0        0        0    10862 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_pnc_junction_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     8603 2024-05-06 18:49:48.690973 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_road_pb2.cpython-310.pyc
--rw-r--r--   0        0        0    14644 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_road_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     2682 2024-05-06 18:49:48.690973 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_rsu_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     3903 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_rsu_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     7712 2024-05-06 18:49:48.690973 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_signal_pb2.cpython-310.pyc
--rw-r--r--   0        0        0    12832 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_signal_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     2917 2024-05-06 18:49:48.690973 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_speed_bump_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     4164 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_speed_bump_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     3879 2024-05-06 18:49:48.690973 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_stop_sign_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     5888 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_stop_sign_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     2920 2024-05-06 18:49:48.690973 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_yield_sign_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     4167 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__pycache__/map_yield_sign_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     4307 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_clear_area_pb2.py
--rw-r--r--   0        0        0     4304 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_crosswalk_pb2.py
--rw-r--r--   0        0        0    10334 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_geometry_pb2.py
--rw-r--r--   0        0        0     1957 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_id_pb2.py
--rw-r--r--   0        0        0     7060 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_junction_pb2.py
--rw-r--r--   0        0        0    33962 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_lane_pb2.py
--rw-r--r--   0        0        0    33794 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_overlap_pb2.py
--rw-r--r--   0        0        0     8127 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_parking_space_pb2.py
--rw-r--r--   0        0        0    25465 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_pb2.py
--rw-r--r--   0        0        0    13943 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_pnc_junction_pb2.py
--rw-r--r--   0        0        0    19494 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_road_pb2.py
--rw-r--r--   0        0        0     3884 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_rsu_pb2.py
--rw-r--r--   0        0        0    17743 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_signal_pb2.py
--rw-r--r--   0        0        0     4305 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_speed_bump_pb2.py
--rw-r--r--   0        0        0     5449 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_speed_control_pb2.py
--rw-r--r--   0        0        0     7094 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_stop_sign_pb2.py
--rw-r--r--   0        0        0     4307 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_yield_sign_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/monitor_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/monitor_msgs/__init__.pyi
--rw-r--r--   0        0        0    14383 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/monitor_msgs/monitor_log_pb2.py
--rw-r--r--   0        0        0     5539 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/monitor_msgs/smart_recorder_status_pb2.py
--rw-r--r--   0        0        0    24632 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/monitor_msgs/system_status_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/__init__.pyi
--rw-r--r--   0        0        0      213 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0    52045 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/__pycache__/perception_obstacle_pb2.cpython-312.pyc
--rw-r--r--   0        0        0    21191 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/__pycache__/traffic_light_detection_pb2.cpython-312.pyc
--rw-r--r--   0        0        0    41724 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/perception_camera_pb2.py
--rw-r--r--   0        0        0     6241 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/perception_lane_pb2.py
--rw-r--r--   0        0        0    75237 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/perception_obstacle_pb2.py
--rw-r--r--   0        0        0    29683 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/traffic_light_detection_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/__init__.pyi
--rw-r--r--   0        0        0      211 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0    67359 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/__pycache__/decision_pb2.cpython-312.pyc
--rw-r--r--   0        0        0    11157 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/__pycache__/navigation_pb2.cpython-312.pyc
--rw-r--r--   0        0        0    99138 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/__pycache__/planning_internal_pb2.cpython-312.pyc
--rw-r--r--   0        0        0    29012 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/__pycache__/planning_pb2.cpython-312.pyc
--rw-r--r--   0        0        0    12184 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/__pycache__/scenario_type_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     4700 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/__pycache__/sl_boundary_pb2.cpython-312.pyc
--rw-r--r--   0        0        0    92283 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/decision_pb2.py
--rw-r--r--   0        0        0    14052 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/navigation_pb2.py
--rw-r--r--   0        0        0     5670 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/pad_msg_pb2.py
--rw-r--r--   0        0        0   139521 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/planning_internal_pb2.py
--rw-r--r--   0        0        0    40675 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/planning_pb2.py
--rw-r--r--   0        0        0    19310 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/scenario_type_pb2.py
--rw-r--r--   0        0        0     5121 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/sl_boundary_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/__init__.pyi
--rw-r--r--   0        0        0    66923 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/feature_pb2.py
--rw-r--r--   0        0        0    48174 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/lane_graph_pb2.py
--rw-r--r--   0        0        0    23934 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/prediction_obstacle_pb2.py
--rw-r--r--   0        0        0     5953 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/prediction_point_pb2.py
--rw-r--r--   0        0        0     5302 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/scenario_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/routing_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/routing_msgs/__init__.pyi
--rw-r--r--   0        0        0      210 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/routing_msgs/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0    27327 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/routing_msgs/__pycache__/routing_pb2.cpython-312.pyc
--rw-r--r--   0        0        0     6127 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/routing_msgs/poi_pb2.py
--rw-r--r--   0        0        0    37342 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/routing_msgs/routing_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/__init__.pyi
--rw-r--r--   0        0        0    36837 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/conti_radar_pb2.py
--rw-r--r--   0        0        0   265504 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/delphi_esr_pb2.py
--rw-r--r--   0        0        0    33278 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/gnss_best_pose_pb2.py
--rw-r--r--   0        0        0    14369 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/gnss_pb2.py
--rw-r--r--   0        0        0    74616 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/gnss_raw_observation_pb2.py
--rw-r--r--   0        0        0    14401 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/heading_pb2.py
--rw-r--r--   0        0        0     5651 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/imu_pb2.py
--rw-r--r--   0        0        0    15918 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/ins_pb2.py
--rw-r--r--   0        0        0    86885 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/mobileye_pb2.py
--rw-r--r--   0        0        0    10386 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/pointcloud_pb2.py
--rw-r--r--   0        0        0    37471 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/racobit_radar_pb2.py
--rw-r--r--   0        0        0    22343 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/radar_pb2.py
--rw-r--r--   0        0        0    26265 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/sensor_image_pb2.py
--rw-r--r--   0        0        0    74229 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/smartereye_pb2.py
--rw-r--r--   0        0        0     3154 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/ultrasonic_radar_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/__init__.pyi
--rw-r--r--   0        0        0    23963 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/agent_pb2.py
--rw-r--r--   0        0        0   133650 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/grading_condition_pb2.py
--rw-r--r--   0        0        0    10898 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/grading_metric_pb2.py
--rw-r--r--   0        0        0    45292 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/scenario_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/storytelling_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/storytelling_msgs/__init__.pyi
--rw-r--r--   0        0        0    21987 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/storytelling_msgs/story_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/task_manager_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/task_manager_msgs/__init__.pyi
--rw-r--r--   0        0        0    17367 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/task_manager_msgs/task_manager_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/transform_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/transform_msgs/__init__.pyi
--rw-r--r--   0        0        0     9122 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/transform_msgs/transform_pb2.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/v2x_msgs/__init__.py
--rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/v2x_msgs/__init__.pyi
--rw-r--r--   0        0        0    18444 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/v2x_msgs/v2x_traffic_light_pb2.py
--rw-r--r--   0        0        0      386 2024-05-06 18:55:26.261543 baidu_apollo_proto-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      567 1970-01-01 00:00:00.000000 baidu_apollo_proto-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       91 2024-05-06 18:51:38.334406 baidu_apollo_proto-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.270670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/__init__.py
+-rw-r--r--   0        0        0       45 2024-05-06 18:47:31.270670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.270670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/__init__.py
+-rw-r--r--   0        0        0      341 2024-05-06 18:47:31.270670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.270670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/audio/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/audio/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/audio/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/audio/proto/__init__.pyi
+-rw-r--r--   0        0        0     5931 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/audio/proto/audio_common_pb2.py
+-rw-r--r--   0        0        0     7018 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/audio/proto/audio_conf_pb2.py
+-rw-r--r--   0        0        0     7326 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/audio/proto/audio_event_pb2.py
+-rw-r--r--   0        0        0     5788 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/audio/proto/audio_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/bridge/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/bridge/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/bridge/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/bridge/proto/__init__.pyi
+-rw-r--r--   0        0        0     7353 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/bridge/proto/udp_bridge_remote_info_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/__init__.pyi
+-rw-r--r--   0        0        0     5731 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/canbus_conf_pb2.py
+-rw-r--r--   0        0        0    84337 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/ch_pb2.py
+-rw-r--r--   0        0        0   361381 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/chassis_detail_pb2.py
+-rw-r--r--   0        0        0    79319 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/chassis_pb2.py
+-rw-r--r--   0        0        0   113739 2024-05-06 18:47:31.274670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/devkit_pb2.py
+-rw-r--r--   0        0        0   201961 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/ge3_pb2.py
+-rw-r--r--   0        0        0   442211 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/lexus_pb2.py
+-rw-r--r--   0        0        0   157770 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/neolix_edu_pb2.py
+-rw-r--r--   0        0        0   112905 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/transit_pb2.py
+-rw-r--r--   0        0        0     5016 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/vehicle_parameter_pb2.py
+-rw-r--r--   0        0        0   189831 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/wey_pb2.py
+-rw-r--r--   0        0        0    65589 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/zhongyun_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/__init__.py
+-rw-r--r--   0        0        0      143 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/adapters/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/adapters/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/adapters/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/adapters/proto/__init__.pyi
+-rw-r--r--   0        0        0    30410 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/adapters/proto/adapter_config_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/configs/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/configs/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/configs/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/configs/proto/__init__.pyi
+-rw-r--r--   0        0        0    36272 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/configs/proto/vehicle_config_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/latency_recorder/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/latency_recorder/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/latency_recorder/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/latency_recorder/proto/__init__.pyi
+-rw-r--r--   0        0        0    17470 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/latency_recorder/proto/latency_record_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/monitor_log/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/monitor_log/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/monitor_log/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.278670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/monitor_log/proto/__init__.pyi
+-rw-r--r--   0        0        0    14328 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/monitor_log/proto/monitor_log_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/proto/__init__.pyi
+-rw-r--r--   0        0        0     3408 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/proto/direction_pb2.py
+-rw-r--r--   0        0        0     6961 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/proto/drive_event_pb2.py
+-rw-r--r--   0        0        0     4717 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/proto/drive_state_pb2.py
+-rw-r--r--   0        0        0    16099 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/proto/error_code_pb2.py
+-rw-r--r--   0        0        0    15182 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/proto/geometry_pb2.py
+-rw-r--r--   0        0        0     7527 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/proto/header_pb2.py
+-rw-r--r--   0        0        0    37024 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/proto/pnc_point_pb2.py
+-rw-r--r--   0        0        0     6129 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/proto/vehicle_signal_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/util/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/util/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/util/testdata/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/util/testdata/__init__.pyi
+-rw-r--r--   0        0        0     5475 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/util/testdata/simple_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/vehicle_model/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/vehicle_model/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/vehicle_model/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/vehicle_model/proto/__init__.pyi
+-rw-r--r--   0        0        0    11270 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/vehicle_model/proto/vehicle_model_config_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/vehicle_state/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/vehicle_state/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/vehicle_state/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.282670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/vehicle_state/proto/__init__.pyi
+-rw-r--r--   0        0        0    12732 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/vehicle_state/proto/vehicle_state_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/contrib/__init__.py
+-rw-r--r--   0        0        0       25 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/contrib/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/__init__.pyi
+-rw-r--r--   0        0        0    14209 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/detection2d_pb2.py
+-rw-r--r--   0        0        0     3755 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/detection2darray_pb2.py
+-rw-r--r--   0        0        0    11266 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/detection3d_pb2.py
+-rw-r--r--   0        0        0     3755 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/detection3darray_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/__init__.pyi
+-rw-r--r--   0        0        0     5406 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/calibration_table_pb2.py
+-rw-r--r--   0        0        0   119179 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/control_cmd_pb2.py
+-rw-r--r--   0        0        0    25084 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/control_common_conf_pb2.py
+-rw-r--r--   0        0        0    30378 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/control_conf_pb2.py
+-rw-r--r--   0        0        0     4381 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/gain_scheduler_conf_pb2.py
+-rw-r--r--   0        0        0     4929 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/input_debug_pb2.py
+-rw-r--r--   0        0        0    20412 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/lat_controller_conf_pb2.py
+-rw-r--r--   0        0        0     4063 2024-05-06 18:47:31.286670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/leadlag_conf_pb2.py
+-rw-r--r--   0        0        0     6508 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/local_view_pb2.py
+-rw-r--r--   0        0        0    18231 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/lon_controller_conf_pb2.py
+-rw-r--r--   0        0        0    19142 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/mpc_controller_conf_pb2.py
+-rw-r--r--   0        0        0     8850 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/mrac_conf_pb2.py
+-rw-r--r--   0        0        0     5556 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/pad_msg_pb2.py
+-rw-r--r--   0        0        0     5897 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/pid_conf_pb2.py
+-rw-r--r--   0        0        0     7562 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/preprocessor_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/data/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/data/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/data/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/data/proto/__init__.pyi
+-rw-r--r--   0        0        0    37510 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/data/proto/frame_pb2.py
+-rw-r--r--   0        0        0    32594 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/data/proto/static_info_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/data/tools/__init__.py
+-rw-r--r--   0        0        0       29 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/data/tools/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/data/tools/smart_recorder/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/data/tools/smart_recorder/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/data/tools/smart_recorder/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/data/tools/smart_recorder/proto/__init__.pyi
+-rw-r--r--   0        0        0     5506 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/data/tools/smart_recorder/proto/smart_recorder_status_pb2.py
+-rw-r--r--   0        0        0    11440 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/data/tools/smart_recorder/proto/smart_recorder_triggers_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/__init__.py
+-rw-r--r--   0        0        0       29 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/backend/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/backend/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/proto/__init__.pyi
+-rw-r--r--   0        0        0     3801 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/proto/daemon_cmd_pb2.py
+-rw-r--r--   0        0        0     3129 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/proto/daemon_rpt_pb2.py
+-rw-r--r--   0        0        0    14055 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/proto/modem_info_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/__init__.pyi
+-rw-r--r--   0        0        0     4111 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/camera_update_pb2.py
+-rw-r--r--   0        0        0    30122 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/chart_pb2.py
+-rw-r--r--   0        0        0    17879 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/data_collection_table_pb2.py
+-rw-r--r--   0        0        0    17773 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/hmi_config_pb2.py
+-rw-r--r--   0        0        0    49215 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/hmi_mode_pb2.py
+-rw-r--r--   0        0        0    18407 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/hmi_status_pb2.py
+-rw-r--r--   0        0        0     2142 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/point_cloud_pb2.py
+-rw-r--r--   0        0        0    16304 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/preprocess_table_pb2.py
+-rw-r--r--   0        0        0   113277 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/simulation_world_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/__init__.py
+-rw-r--r--   0        0        0      139 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/camera/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/camera/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/camera/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/camera/proto/__init__.pyi
+-rw-r--r--   0        0        0    24718 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/camera/proto/config_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/canbus/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/canbus/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/canbus/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/canbus/proto/__init__.pyi
+-rw-r--r--   0        0        0    12311 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/canbus/proto/can_card_parameter_pb2.py
+-rw-r--r--   0        0        0     4163 2024-05-06 18:47:31.290670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/canbus/proto/sensor_canbus_conf_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/__init__.pyi
+-rw-r--r--   0        0        0    41814 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/config_pb2.py
+-rw-r--r--   0        0        0    33208 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/gnss_best_pose_pb2.py
+-rw-r--r--   0        0        0    14191 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/gnss_pb2.py
+-rw-r--r--   0        0        0    74576 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/gnss_raw_observation_pb2.py
+-rw-r--r--   0        0        0    13692 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/gnss_status_pb2.py
+-rw-r--r--   0        0        0    14308 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/heading_pb2.py
+-rw-r--r--   0        0        0     5514 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/imu_pb2.py
+-rw-r--r--   0        0        0    15728 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/ins_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/__init__.pyi
+-rw-r--r--   0        0        0     5789 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/config_pb2.py
+-rw-r--r--   0        0        0     9720 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/hesai_config_pb2.py
+-rw-r--r--   0        0        0     8019 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/hesai_pb2.py
+-rw-r--r--   0        0        0     5311 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/lidar_parameter_pb2.py
+-rw-r--r--   0        0        0    11250 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/robosense_config_pb2.py
+-rw-r--r--   0        0        0     6785 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/robosense_pb2.py
+-rw-r--r--   0        0        0    26240 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/velodyne_config_pb2.py
+-rw-r--r--   0        0        0    12962 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/velodyne_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/microphone/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/microphone/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/microphone/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/microphone/proto/__init__.pyi
+-rw-r--r--   0        0        0     6840 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/microphone/proto/audio_pb2.py
+-rw-r--r--   0        0        0    10763 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/microphone/proto/microphone_config_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/__init__.pyi
+-rw-r--r--   0        0        0    34082 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/conti_radar_pb2.py
+-rw-r--r--   0        0        0   265003 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/delphi_esr_pb2.py
+-rw-r--r--   0        0        0    86336 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/mobileye_pb2.py
+-rw-r--r--   0        0        0    10243 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/pointcloud_pb2.py
+-rw-r--r--   0        0        0    34642 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/racobit_radar_pb2.py
+-rw-r--r--   0        0        0    22066 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/radar_pb2.py
+-rw-r--r--   0        0        0    26133 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/sensor_image_pb2.py
+-rw-r--r--   0        0        0    73970 2024-05-06 18:47:31.294670 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/smartereye_pb2.py
+-rw-r--r--   0        0        0     3067 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/ultrasonic_radar_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/conti_radar/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/conti_radar/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/conti_radar/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/conti_radar/proto/__init__.pyi
+-rw-r--r--   0        0        0    26377 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/conti_radar/proto/conti_radar_conf_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/racobit_radar/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/racobit_radar/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/racobit_radar/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/racobit_radar/proto/__init__.pyi
+-rw-r--r--   0        0        0    25143 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/racobit_radar/proto/racobit_radar_conf_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/ultrasonic_radar/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/ultrasonic_radar/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/ultrasonic_radar/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/ultrasonic_radar/proto/__init__.pyi
+-rw-r--r--   0        0        0     7216 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/ultrasonic_radar/proto/ultrasonic_radar_conf_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/smartereye/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/smartereye/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/smartereye/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/smartereye/proto/__init__.pyi
+-rw-r--r--   0        0        0    26306 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/smartereye/proto/config_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/tools/__init__.py
+-rw-r--r--   0        0        0       31 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/tools/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/tools/image_decompress/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/tools/image_decompress/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/tools/image_decompress/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/tools/image_decompress/proto/__init__.pyi
+-rw-r--r--   0        0        0     2149 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/tools/image_decompress/proto/config_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/video/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/video/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/video/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/video/proto/__init__.pyi
+-rw-r--r--   0        0        0    20844 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/video/proto/video_h265cfg_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/guardian/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/guardian/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/guardian/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/guardian/proto/__init__.pyi
+-rw-r--r--   0        0        0     3602 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/guardian/proto/guardian_conf_pb2.py
+-rw-r--r--   0        0        0     3572 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/guardian/proto/guardian_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/__init__.pyi
+-rw-r--r--   0        0        0    22890 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/gnss_pnt_result_pb2.py
+-rw-r--r--   0        0        0     3357 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/gps_pb2.py
+-rw-r--r--   0        0        0     3447 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/imu_pb2.py
+-rw-r--r--   0        0        0     3538 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/localization_config_pb2.py
+-rw-r--r--   0        0        0    20892 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/localization_pb2.py
+-rw-r--r--   0        0        0    43603 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/localization_status_pb2.py
+-rw-r--r--   0        0        0    13252 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/measure_pb2.py
+-rw-r--r--   0        0        0     8652 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/pose_pb2.py
+-rw-r--r--   0        0        0     9639 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/rtk_config_pb2.py
+-rw-r--r--   0        0        0     6472 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/sins_pva_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/__init__.py
+-rw-r--r--   0        0        0       41 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.298671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/__init__.pyi
+-rw-r--r--   0        0        0     4119 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_clear_area_pb2.py
+-rw-r--r--   0        0        0     4116 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_crosswalk_pb2.py
+-rw-r--r--   0        0        0    10081 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_geometry_pb2.py
+-rw-r--r--   0        0        0     1927 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_id_pb2.py
+-rw-r--r--   0        0        0     6872 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_junction_pb2.py
+-rw-r--r--   0        0        0    33595 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_lane_pb2.py
+-rw-r--r--   0        0        0    33378 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_overlap_pb2.py
+-rw-r--r--   0        0        0     7912 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_parking_space_pb2.py
+-rw-r--r--   0        0        0    24567 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_pb2.py
+-rw-r--r--   0        0        0    13655 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_pnc_junction_pb2.py
+-rw-r--r--   0        0        0    19114 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_road_pb2.py
+-rw-r--r--   0        0        0     3763 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_rsu_pb2.py
+-rw-r--r--   0        0        0    17405 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_signal_pb2.py
+-rw-r--r--   0        0        0     4117 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_speed_bump_pb2.py
+-rw-r--r--   0        0        0     5329 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_speed_control_pb2.py
+-rw-r--r--   0        0        0     6906 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_stop_sign_pb2.py
+-rw-r--r--   0        0        0     4119 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_yield_sign_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/relative_map/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/relative_map/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/relative_map/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/relative_map/proto/__init__.pyi
+-rw-r--r--   0        0        0    13726 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/relative_map/proto/navigation_pb2.py
+-rw-r--r--   0        0        0     8676 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/relative_map/proto/navigator_config_pb2.py
+-rw-r--r--   0        0        0    16130 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/relative_map/proto/relative_map_config_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/tools/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/tools/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/proto/__init__.pyi
+-rw-r--r--   0        0        0    38508 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/proto/collection_check_message_pb2.py
+-rw-r--r--   0        0        0     9393 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/proto/collection_error_code_pb2.py
+-rw-r--r--   0        0        0     5174 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/proto/collection_service_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/monitor/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/monitor/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/monitor/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/monitor/proto/__init__.pyi
+-rw-r--r--   0        0        0    24463 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/monitor/proto/system_status_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/__init__.py
+-rw-r--r--   0        0        0       52 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/camera/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-06 18:47:31.302671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/camera/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/camera/app/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/camera/app/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/camera/app/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/camera/app/proto/__init__.pyi
+-rw-r--r--   0        0        0    38941 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/camera/app/proto/perception_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/camera/common/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/camera/common/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/camera/common/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/camera/common/proto/__init__.pyi
+-rw-r--r--   0        0        0    16546 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/camera/common/proto/object_template_meta_schema_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/camera/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/camera/proto/__init__.pyi
+-rw-r--r--   0        0        0    66169 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/camera/proto/yolo_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/fusion/__init__.py
+-rw-r--r--   0        0        0       18 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/fusion/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/lidar/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/lidar/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/lidar/app/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/lidar/app/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/lidar/app/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/lidar/app/proto/__init__.pyi
+-rw-r--r--   0        0        0     4615 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/lidar/app/proto/lidar_obstacle_detection_config_pb2.py
+-rw-r--r--   0        0        0     3968 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/lidar/app/proto/lidar_obstacle_tracking_config_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/onboard/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/onboard/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/__init__.pyi
+-rw-r--r--   0        0        0    25687 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/fusion_camera_detection_component_pb2.py
+-rw-r--r--   0        0        0     6847 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/fusion_component_config_pb2.py
+-rw-r--r--   0        0        0    15984 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/lane_perception_component_pb2.py
+-rw-r--r--   0        0        0     8426 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/lidar_component_config_pb2.py
+-rw-r--r--   0        0        0     4595 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/motion_service_pb2.py
+-rw-r--r--   0        0        0     7268 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/radar_component_config_pb2.py
+-rw-r--r--   0        0        0    16377 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/trafficlights_perception_component_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/__init__.pyi
+-rw-r--r--   0        0        0     3797 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/ccrf_type_fusion_config_pb2.py
+-rw-r--r--   0        0        0     5384 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/dst_existence_fusion_config_pb2.py
+-rw-r--r--   0        0        0     9917 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/dst_type_fusion_config_pb2.py
+-rw-r--r--   0        0        0     5224 2024-05-06 18:47:31.306671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/fused_classifier_config_pb2.py
+-rw-r--r--   0        0        0     4237 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/map_manager_config_pb2.py
+-rw-r--r--   0        0        0    21526 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/motion_service_pb2.py
+-rw-r--r--   0        0        0     4499 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/pbf_tracker_config_pb2.py
+-rw-r--r--   0        0        0    41389 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_camera_pb2.py
+-rw-r--r--   0        0        0    35522 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_config_schema_pb2.py
+-rw-r--r--   0        0        0     6065 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_lane_pb2.py
+-rw-r--r--   0        0        0    74709 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_obstacle_pb2.py
+-rw-r--r--   0        0        0     7491 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_ultrasonic_pb2.py
+-rw-r--r--   0        0        0     9457 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/probabilistic_fusion_config_pb2.py
+-rw-r--r--   0        0        0     4484 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/roi_boundary_filter_config_pb2.py
+-rw-r--r--   0        0        0   636938 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/rt_pb2.py
+-rw-r--r--   0        0        0    12133 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/sensor_meta_schema_pb2.py
+-rw-r--r--   0        0        0     2770 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/tracker_config_pb2.py
+-rw-r--r--   0        0        0    29561 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/traffic_light_detection_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/__init__.py
+-rw-r--r--   0        0        0       19 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/__init__.pyi
+-rw-r--r--   0        0        0    34971 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/auto_tuning_model_input_pb2.py
+-rw-r--r--   0        0        0    38141 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/auto_tuning_raw_feature_pb2.py
+-rw-r--r--   0        0        0    91347 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/decision_pb2.py
+-rw-r--r--   0        0        0     7569 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/ipopt_return_status_pb2.py
+-rw-r--r--   0        0        0     6012 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/lattice_structure_pb2.py
+-rw-r--r--   0        0        0    86626 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/learning_data_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/math/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/math/__init__.pyi
+-rw-r--r--   0        0        0     7833 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/math/cos_theta_smoother_config_pb2.py
+-rw-r--r--   0        0        0    16221 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/math/fem_pos_deviation_smoother_config_pb2.py
+-rw-r--r--   0        0        0    12481 2024-05-06 18:47:31.310671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/math/qp_problem_pb2.py
+-rw-r--r--   0        0        0    87356 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/open_space_task_config_pb2.py
+-rw-r--r--   0        0        0     5698 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/pad_msg_pb2.py
+-rw-r--r--   0        0        0    87377 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/planner_open_space_config_pb2.py
+-rw-r--r--   0        0        0   168243 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_config_pb2.py
+-rw-r--r--   0        0        0   138187 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_internal_pb2.py
+-rw-r--r--   0        0        0    39948 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_pb2.py
+-rw-r--r--   0        0        0     9743 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_semantic_map_config_pb2.py
+-rw-r--r--   0        0        0     9860 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_stats_pb2.py
+-rw-r--r--   0        0        0    69955 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_status_pb2.py
+-rw-r--r--   0        0        0    29328 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/reference_line_smoother_config_pb2.py
+-rw-r--r--   0        0        0     4994 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/sl_boundary_pb2.py
+-rw-r--r--   0        0        0     6589 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/st_drivable_boundary_pb2.py
+-rw-r--r--   0        0        0   127062 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/task_config_pb2.py
+-rw-r--r--   0        0        0    42482 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/traffic_rule_config_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/__init__.pyi
+-rw-r--r--   0        0        0    66099 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/feature_pb2.py
+-rw-r--r--   0        0        0     9398 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/fnn_model_base_pb2.py
+-rw-r--r--   0        0        0     6177 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/fnn_vehicle_model_pb2.py
+-rw-r--r--   0        0        0    47822 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/lane_graph_pb2.py
+-rw-r--r--   0        0        0    59580 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/network_layers_pb2.py
+-rw-r--r--   0        0        0    11781 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/network_model_pb2.py
+-rw-r--r--   0        0        0    25535 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/offline_features_pb2.py
+-rw-r--r--   0        0        0    26108 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/prediction_conf_pb2.py
+-rw-r--r--   0        0        0    23511 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/prediction_obstacle_pb2.py
+-rw-r--r--   0        0        0     5909 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/prediction_point_pb2.py
+-rw-r--r--   0        0        0     5247 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/scenario_pb2.py
+-rw-r--r--   0        0        0    11980 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/vector_net_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/routing/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/routing/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/routing/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/routing/proto/__init__.pyi
+-rw-r--r--   0        0        0     5981 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/routing/proto/poi_pb2.py
+-rw-r--r--   0        0        0     8435 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/routing/proto/routing_config_pb2.py
+-rw-r--r--   0        0        0    36680 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/routing/proto/routing_pb2.py
+-rw-r--r--   0        0        0    18648 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/routing/proto/topo_graph_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/storytelling/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/storytelling/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/storytelling/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/storytelling/proto/__init__.pyi
+-rw-r--r--   0        0        0    21807 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/storytelling/proto/story_pb2.py
+-rw-r--r--   0        0        0     4553 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/storytelling/proto/storytelling_config_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/task_manager/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/task_manager/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/task_manager/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/task_manager/proto/__init__.pyi
+-rw-r--r--   0        0        0     5924 2024-05-06 18:47:31.314671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/task_manager/proto/task_manager_config_pb2.py
+-rw-r--r--   0        0        0    18549 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/task_manager/proto/task_manager_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/third_party_perception/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/third_party_perception/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/third_party_perception/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/third_party_perception/proto/__init__.pyi
+-rw-r--r--   0        0        0    17334 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/third_party_perception/proto/radar_obstacle_pb2.py
+-rw-r--r--   0        0        0     3939 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/third_party_perception/proto/third_party_perception_component_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/__init__.py
+-rw-r--r--   0        0        0       56 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/navigator/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/navigator/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/navigator/dbmap/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/navigator/dbmap/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/navigator/dbmap/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/navigator/dbmap/proto/__init__.pyi
+-rw-r--r--   0        0        0    18863 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/navigator/dbmap/proto/dbmap_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/prediction/__init__.py
+-rw-r--r--   0        0        0       29 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/prediction/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/prediction/data_pipelines/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/prediction/data_pipelines/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/prediction/data_pipelines/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/prediction/data_pipelines/proto/__init__.pyi
+-rw-r--r--   0        0        0    47307 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/prediction/data_pipelines/proto/cruise_model_pb2.py
+-rw-r--r--   0        0        0    13929 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/prediction/data_pipelines/proto/fnn_model_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/sensor_calibration/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/sensor_calibration/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/sensor_calibration/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/sensor_calibration/proto/__init__.pyi
+-rw-r--r--   0        0        0    13399 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/sensor_calibration/proto/extractor_config_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/transform/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/transform/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/transform/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/transform/proto/__init__.pyi
+-rw-r--r--   0        0        0     5691 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/transform/proto/static_transform_conf_pb2.py
+-rw-r--r--   0        0        0     8909 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/transform/proto/transform_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/__init__.pyi
+-rw-r--r--   0        0        0    15952 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/fusion_params_pb2.py
+-rw-r--r--   0        0        0     5322 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_car_status_pb2.py
+-rw-r--r--   0        0        0    10819 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_junction_pb2.py
+-rw-r--r--   0        0        0     6130 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_monitor_pb2.py
+-rw-r--r--   0        0        0    23335 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_obstacles_pb2.py
+-rw-r--r--   0        0        0     7897 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_obu_rsi_pb2.py
+-rw-r--r--   0        0        0    19133 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_obu_traffic_light_pb2.py
+-rw-r--r--   0        0        0     9397 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_rsi_pb2.py
+-rw-r--r--   0        0        0     3258 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_service_car_to_obu_pb2.py
+-rw-r--r--   0        0        0     6868 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_service_obu_to_car_pb2.py
+-rw-r--r--   0        0        0    18277 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_traffic_light_pb2.py
+-rw-r--r--   0        0        0    30751 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_traffic_light_policy_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/__init__.py
+-rw-r--r--   0        0        0       45 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/__init__.py
+-rw-r--r--   0        0        0       26 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/__init__.py
+-rw-r--r--   0        0        0      412 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/__init__.pyi
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/audio_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/audio_msgs/__init__.pyi
+-rw-r--r--   0        0        0     5953 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/audio_msgs/audio_common_pb2.py
+-rw-r--r--   0        0        0     7602 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/audio_msgs/audio_event_pb2.py
+-rw-r--r--   0        0        0     6022 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/audio_msgs/audio_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/__init__.pyi
+-rw-r--r--   0        0        0     3428 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/direction_pb2.py
+-rw-r--r--   0        0        0     7131 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/drive_event_pb2.py
+-rw-r--r--   0        0        0     4770 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/drive_state_pb2.py
+-rw-r--r--   0        0        0    16152 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/error_code_pb2.py
+-rw-r--r--   0        0        0    15400 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/geometry_pb2.py
+-rw-r--r--   0        0        0     7628 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/header_pb2.py
+-rw-r--r--   0        0        0    37282 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/pnc_point_pb2.py
+-rw-r--r--   0        0        0     3383 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/vehicle_id_pb2.py
+-rw-r--r--   0        0        0     6452 2024-05-06 18:47:31.318671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/vehicle_signal_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/chassis_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/chassis_msgs/__init__.pyi
+-rw-r--r--   0        0        0   353927 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/chassis_msgs/chassis_detail_pb2.py
+-rw-r--r--   0        0        0    90974 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/chassis_msgs/chassis_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/config_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/config_msgs/__init__.pyi
+-rw-r--r--   0        0        0    34037 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/config_msgs/vehicle_config_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/control_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/control_msgs/__init__.pyi
+-rw-r--r--   0        0        0   120575 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/control_msgs/control_cmd_pb2.py
+-rw-r--r--   0        0        0     5077 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/control_msgs/input_debug_pb2.py
+-rw-r--r--   0        0        0     6023 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/control_msgs/pad_msg_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/dreamview_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/dreamview_msgs/__init__.pyi
+-rw-r--r--   0        0        0    30338 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/dreamview_msgs/chart_pb2.py
+-rw-r--r--   0        0        0    36529 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/dreamview_msgs/hmi_status_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/drivers_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/drivers_msgs/__init__.pyi
+-rw-r--r--   0        0        0    15211 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/drivers_msgs/can_card_parameter_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/guardian_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/guardian_msgs/__init__.pyi
+-rw-r--r--   0        0        0     3729 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/guardian_msgs/guardian_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/__init__.pyi
+-rw-r--r--   0        0        0     3507 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/gps_pb2.py
+-rw-r--r--   0        0        0     3620 2024-05-06 18:47:31.322671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/imu_pb2.py
+-rw-r--r--   0        0        0    21318 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/localization_pb2.py
+-rw-r--r--   0        0        0    43647 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/localization_status_pb2.py
+-rw-r--r--   0        0        0     8862 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/pose_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/__init__.pyi
+-rw-r--r--   0        0        0     4307 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_clear_area_pb2.py
+-rw-r--r--   0        0        0     4304 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_crosswalk_pb2.py
+-rw-r--r--   0        0        0    10334 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_geometry_pb2.py
+-rw-r--r--   0        0        0     1957 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_id_pb2.py
+-rw-r--r--   0        0        0     7060 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_junction_pb2.py
+-rw-r--r--   0        0        0    33962 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_lane_pb2.py
+-rw-r--r--   0        0        0    33794 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_overlap_pb2.py
+-rw-r--r--   0        0        0     8127 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_parking_space_pb2.py
+-rw-r--r--   0        0        0    25465 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_pb2.py
+-rw-r--r--   0        0        0    13943 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_pnc_junction_pb2.py
+-rw-r--r--   0        0        0    19494 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_road_pb2.py
+-rw-r--r--   0        0        0     3884 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_rsu_pb2.py
+-rw-r--r--   0        0        0    17743 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_signal_pb2.py
+-rw-r--r--   0        0        0     4305 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_speed_bump_pb2.py
+-rw-r--r--   0        0        0     5449 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_speed_control_pb2.py
+-rw-r--r--   0        0        0     7094 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_stop_sign_pb2.py
+-rw-r--r--   0        0        0     4307 2024-05-06 18:47:31.326671 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_yield_sign_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/monitor_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/monitor_msgs/__init__.pyi
+-rw-r--r--   0        0        0    14383 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/monitor_msgs/monitor_log_pb2.py
+-rw-r--r--   0        0        0     5539 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/monitor_msgs/smart_recorder_status_pb2.py
+-rw-r--r--   0        0        0    24632 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/monitor_msgs/system_status_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/__init__.pyi
+-rw-r--r--   0        0        0    41724 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/perception_camera_pb2.py
+-rw-r--r--   0        0        0     6241 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/perception_lane_pb2.py
+-rw-r--r--   0        0        0    75237 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/perception_obstacle_pb2.py
+-rw-r--r--   0        0        0    29683 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/traffic_light_detection_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/__init__.pyi
+-rw-r--r--   0        0        0    92283 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/decision_pb2.py
+-rw-r--r--   0        0        0    14052 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/navigation_pb2.py
+-rw-r--r--   0        0        0     5670 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/pad_msg_pb2.py
+-rw-r--r--   0        0        0   139521 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/planning_internal_pb2.py
+-rw-r--r--   0        0        0    40675 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/planning_pb2.py
+-rw-r--r--   0        0        0    19310 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/scenario_type_pb2.py
+-rw-r--r--   0        0        0     5121 2024-05-06 18:47:31.330672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/sl_boundary_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/__init__.pyi
+-rw-r--r--   0        0        0    66923 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/feature_pb2.py
+-rw-r--r--   0        0        0    48174 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/lane_graph_pb2.py
+-rw-r--r--   0        0        0    23934 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/prediction_obstacle_pb2.py
+-rw-r--r--   0        0        0     5953 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/prediction_point_pb2.py
+-rw-r--r--   0        0        0     5302 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/scenario_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/routing_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/routing_msgs/__init__.pyi
+-rw-r--r--   0        0        0     6127 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/routing_msgs/poi_pb2.py
+-rw-r--r--   0        0        0    37342 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/routing_msgs/routing_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/__init__.pyi
+-rw-r--r--   0        0        0    36837 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/conti_radar_pb2.py
+-rw-r--r--   0        0        0   265504 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/delphi_esr_pb2.py
+-rw-r--r--   0        0        0    33278 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/gnss_best_pose_pb2.py
+-rw-r--r--   0        0        0    14369 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/gnss_pb2.py
+-rw-r--r--   0        0        0    74616 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/gnss_raw_observation_pb2.py
+-rw-r--r--   0        0        0    14401 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/heading_pb2.py
+-rw-r--r--   0        0        0     5651 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/imu_pb2.py
+-rw-r--r--   0        0        0    15918 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/ins_pb2.py
+-rw-r--r--   0        0        0    86885 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/mobileye_pb2.py
+-rw-r--r--   0        0        0    10386 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/pointcloud_pb2.py
+-rw-r--r--   0        0        0    37471 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/racobit_radar_pb2.py
+-rw-r--r--   0        0        0    22343 2024-05-06 18:47:31.334672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/radar_pb2.py
+-rw-r--r--   0        0        0    26265 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/sensor_image_pb2.py
+-rw-r--r--   0        0        0    74229 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/smartereye_pb2.py
+-rw-r--r--   0        0        0     3154 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/ultrasonic_radar_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/__init__.pyi
+-rw-r--r--   0        0        0    23963 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/agent_pb2.py
+-rw-r--r--   0        0        0   133650 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/grading_condition_pb2.py
+-rw-r--r--   0        0        0    10898 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/grading_metric_pb2.py
+-rw-r--r--   0        0        0    45292 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/scenario_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/storytelling_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/storytelling_msgs/__init__.pyi
+-rw-r--r--   0        0        0    21987 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/storytelling_msgs/story_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/task_manager_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/task_manager_msgs/__init__.pyi
+-rw-r--r--   0        0        0    17367 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/task_manager_msgs/task_manager_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/transform_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/transform_msgs/__init__.pyi
+-rw-r--r--   0        0        0     9122 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/transform_msgs/transform_pb2.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/v2x_msgs/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/v2x_msgs/__init__.pyi
+-rw-r--r--   0        0        0    18444 2024-05-06 18:47:31.338672 baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/v2x_msgs/v2x_traffic_light_pb2.py
+-rw-r--r--   0        0        0      387 2024-05-19 23:26:52.027478 baidu_apollo_proto-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      562 1970-01-01 00:00:00.000000 baidu_apollo_proto-0.1.1/PKG-INFO
```

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/audio/proto/audio_common_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/audio/proto/audio_common_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/audio/proto/audio_conf_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/audio/proto/audio_conf_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/audio/proto/audio_event_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/audio/proto/audio_event_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/audio/proto/audio_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/audio/proto/audio_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/bridge/proto/udp_bridge_remote_info_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/bridge/proto/udp_bridge_remote_info_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/canbus_conf_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/canbus_conf_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/ch_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/ch_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/chassis_detail_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/chassis_detail_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/chassis_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/chassis_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/devkit_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/devkit_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/ge3_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/ge3_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/lexus_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/lexus_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/neolix_edu_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/neolix_edu_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/transit_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/transit_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/vehicle_parameter_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/vehicle_parameter_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/wey_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/wey_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/canbus/proto/zhongyun_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/canbus/proto/zhongyun_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/adapters/proto/adapter_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/adapters/proto/adapter_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/configs/proto/vehicle_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/configs/proto/vehicle_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/latency_recorder/proto/latency_record_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/latency_recorder/proto/latency_record_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/monitor_log/proto/monitor_log_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/monitor_log/proto/monitor_log_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/proto/direction_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/proto/direction_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/proto/drive_event_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/proto/drive_event_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/proto/drive_state_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/proto/drive_state_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/proto/error_code_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/proto/error_code_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/proto/geometry_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/proto/geometry_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/proto/header_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/proto/header_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/proto/pnc_point_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/proto/pnc_point_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/proto/vehicle_signal_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/proto/vehicle_signal_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/util/testdata/simple_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/util/testdata/simple_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/vehicle_model/proto/vehicle_model_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/vehicle_model/proto/vehicle_model_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/common/vehicle_state/proto/vehicle_state_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/common/vehicle_state/proto/vehicle_state_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/detection2d_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/detection2d_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/detection2darray_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/detection2darray_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/detection3d_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/detection3d_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/detection3darray_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/contrib/lgsvl_msgs/proto/detection3darray_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/calibration_table_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/calibration_table_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/control_cmd_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/control_cmd_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/control_common_conf_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/control_common_conf_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/control_conf_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/control_conf_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/gain_scheduler_conf_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/gain_scheduler_conf_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/input_debug_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/input_debug_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/lat_controller_conf_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/lat_controller_conf_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/leadlag_conf_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/leadlag_conf_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/local_view_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/local_view_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/lon_controller_conf_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/lon_controller_conf_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/mpc_controller_conf_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/mpc_controller_conf_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/mrac_conf_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/mrac_conf_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/pad_msg_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/pad_msg_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/pid_conf_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/pid_conf_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/control/proto/preprocessor_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/control/proto/preprocessor_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/data/proto/frame_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/data/proto/frame_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/data/proto/static_info_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/data/proto/static_info_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/data/tools/smart_recorder/proto/smart_recorder_status_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/data/tools/smart_recorder/proto/smart_recorder_status_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/data/tools/smart_recorder/proto/smart_recorder_triggers_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/data/tools/smart_recorder/proto/smart_recorder_triggers_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/proto/daemon_cmd_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/proto/daemon_cmd_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/proto/daemon_rpt_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/proto/daemon_rpt_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/proto/modem_info_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/backend/teleop/proto/modem_info_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/camera_update_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/camera_update_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/chart_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/chart_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/data_collection_table_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/data_collection_table_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/hmi_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/hmi_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/hmi_mode_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/hmi_mode_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/hmi_status_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/hmi_status_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/point_cloud_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/point_cloud_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/preprocess_table_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/preprocess_table_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/dreamview/proto/simulation_world_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/dreamview/proto/simulation_world_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/camera/proto/config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/camera/proto/config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/canbus/proto/can_card_parameter_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/canbus/proto/can_card_parameter_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/canbus/proto/sensor_canbus_conf_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/canbus/proto/sensor_canbus_conf_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/gnss_best_pose_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/gnss_best_pose_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/gnss_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/gnss_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/gnss_raw_observation_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/gnss_raw_observation_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/gnss_status_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/gnss_status_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/heading_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/heading_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/imu_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/imu_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/ins_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/gnss/proto/ins_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/hesai_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/hesai_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/hesai_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/hesai_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/lidar_parameter_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/lidar_parameter_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/robosense_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/robosense_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/robosense_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/robosense_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/velodyne_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/velodyne_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/velodyne_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/lidar/proto/velodyne_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/microphone/proto/audio_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/microphone/proto/audio_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/microphone/proto/microphone_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/microphone/proto/microphone_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/conti_radar_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/conti_radar_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/delphi_esr_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/delphi_esr_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/mobileye_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/mobileye_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/pointcloud_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/pointcloud_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/racobit_radar_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/racobit_radar_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/radar_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/radar_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/sensor_image_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/sensor_image_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/smartereye_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/smartereye_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/proto/ultrasonic_radar_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/proto/ultrasonic_radar_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/conti_radar/proto/conti_radar_conf_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/conti_radar/proto/conti_radar_conf_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/racobit_radar/proto/racobit_radar_conf_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/racobit_radar/proto/racobit_radar_conf_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/radar/ultrasonic_radar/proto/ultrasonic_radar_conf_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/radar/ultrasonic_radar/proto/ultrasonic_radar_conf_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/smartereye/proto/config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/smartereye/proto/config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/tools/image_decompress/proto/config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/tools/image_decompress/proto/config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/drivers/video/proto/video_h265cfg_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/drivers/video/proto/video_h265cfg_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/guardian/proto/guardian_conf_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/guardian/proto/guardian_conf_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/guardian/proto/guardian_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/guardian/proto/guardian_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/gnss_pnt_result_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/gnss_pnt_result_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/gps_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/gps_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/imu_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/imu_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/localization_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/localization_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/localization_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/localization_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/localization_status_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/localization_status_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/measure_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/measure_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/pose_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/pose_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/rtk_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/rtk_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/localization/proto/sins_pva_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/localization/proto/sins_pva_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_clear_area_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_clear_area_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_crosswalk_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_crosswalk_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_geometry_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_geometry_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_id_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_id_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_junction_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_junction_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_lane_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_lane_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_overlap_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_overlap_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_parking_space_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_parking_space_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_pnc_junction_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_pnc_junction_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_road_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_road_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_rsu_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_rsu_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_signal_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_signal_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_speed_bump_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_speed_bump_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_speed_control_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_speed_control_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_stop_sign_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_stop_sign_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/proto/map_yield_sign_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/proto/map_yield_sign_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/relative_map/proto/navigation_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/relative_map/proto/navigation_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/relative_map/proto/navigator_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/relative_map/proto/navigator_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/relative_map/proto/relative_map_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/relative_map/proto/relative_map_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/proto/collection_check_message_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/proto/collection_check_message_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/proto/collection_error_code_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/proto/collection_error_code_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/proto/collection_service_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/map/tools/map_datachecker/proto/collection_service_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/monitor/proto/system_status_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/monitor/proto/system_status_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/camera/app/proto/perception_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/camera/app/proto/perception_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/camera/common/proto/object_template_meta_schema_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/camera/common/proto/object_template_meta_schema_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/camera/proto/yolo_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/camera/proto/yolo_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/lidar/app/proto/lidar_obstacle_detection_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/lidar/app/proto/lidar_obstacle_detection_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/lidar/app/proto/lidar_obstacle_tracking_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/lidar/app/proto/lidar_obstacle_tracking_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/fusion_camera_detection_component_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/fusion_camera_detection_component_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/fusion_component_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/fusion_component_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/lane_perception_component_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/lane_perception_component_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/lidar_component_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/lidar_component_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/motion_service_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/motion_service_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/radar_component_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/radar_component_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/trafficlights_perception_component_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/onboard/proto/trafficlights_perception_component_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/ccrf_type_fusion_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/ccrf_type_fusion_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/dst_existence_fusion_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/dst_existence_fusion_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/dst_type_fusion_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/dst_type_fusion_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/fused_classifier_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/fused_classifier_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/map_manager_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/map_manager_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/motion_service_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/motion_service_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/pbf_tracker_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/pbf_tracker_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_camera_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_camera_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_config_schema_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_config_schema_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_lane_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_lane_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_obstacle_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_obstacle_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_ultrasonic_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/perception_ultrasonic_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/probabilistic_fusion_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/probabilistic_fusion_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/roi_boundary_filter_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/roi_boundary_filter_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/rt_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/rt_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/sensor_meta_schema_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/sensor_meta_schema_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/tracker_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/tracker_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/perception/proto/traffic_light_detection_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/perception/proto/traffic_light_detection_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/auto_tuning_model_input_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/auto_tuning_model_input_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/auto_tuning_raw_feature_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/auto_tuning_raw_feature_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/decision_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/decision_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/ipopt_return_status_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/ipopt_return_status_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/lattice_structure_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/lattice_structure_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/learning_data_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/learning_data_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/math/cos_theta_smoother_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/math/cos_theta_smoother_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/math/fem_pos_deviation_smoother_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/math/fem_pos_deviation_smoother_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/math/qp_problem_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/math/qp_problem_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/open_space_task_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/open_space_task_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/pad_msg_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/pad_msg_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/planner_open_space_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/planner_open_space_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_internal_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_internal_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_semantic_map_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_semantic_map_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_stats_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_status_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/planning_status_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/reference_line_smoother_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/reference_line_smoother_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/sl_boundary_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/sl_boundary_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/st_drivable_boundary_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/st_drivable_boundary_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/task_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/task_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/planning/proto/traffic_rule_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/planning/proto/traffic_rule_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/feature_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/feature_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/fnn_model_base_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/fnn_model_base_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/fnn_vehicle_model_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/fnn_vehicle_model_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/lane_graph_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/lane_graph_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/network_layers_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/network_layers_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/network_model_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/network_model_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/offline_features_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/offline_features_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/prediction_conf_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/prediction_conf_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/prediction_obstacle_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/prediction_obstacle_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/prediction_point_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/prediction_point_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/scenario_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/scenario_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/prediction/proto/vector_net_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/prediction/proto/vector_net_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/routing/proto/poi_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/routing/proto/poi_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/routing/proto/routing_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/routing/proto/routing_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/routing/proto/routing_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/routing/proto/routing_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/routing/proto/topo_graph_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/routing/proto/topo_graph_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/storytelling/proto/story_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/storytelling/proto/story_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/storytelling/proto/storytelling_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/storytelling/proto/storytelling_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/task_manager/proto/task_manager_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/task_manager/proto/task_manager_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/task_manager/proto/task_manager_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/task_manager/proto/task_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/third_party_perception/proto/radar_obstacle_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/third_party_perception/proto/radar_obstacle_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/third_party_perception/proto/third_party_perception_component_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/third_party_perception/proto/third_party_perception_component_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/navigator/dbmap/proto/dbmap_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/navigator/dbmap/proto/dbmap_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/prediction/data_pipelines/proto/cruise_model_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/prediction/data_pipelines/proto/cruise_model_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/prediction/data_pipelines/proto/fnn_model_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/prediction/data_pipelines/proto/fnn_model_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/tools/sensor_calibration/proto/extractor_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/tools/sensor_calibration/proto/extractor_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/transform/proto/static_transform_conf_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/transform/proto/static_transform_conf_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/transform/proto/transform_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/transform/proto/transform_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/fusion_params_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/fusion_params_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_car_status_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_car_status_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_junction_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_junction_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_monitor_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_monitor_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_obstacles_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_obstacles_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_obu_rsi_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_obu_rsi_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_obu_traffic_light_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_obu_traffic_light_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_rsi_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_rsi_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_service_car_to_obu_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_service_car_to_obu_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_service_obu_to_car_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_service_obu_to_car_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_traffic_light_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_traffic_light_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_traffic_light_policy_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v7/modules/v2x/proto/v2x_traffic_light_policy_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/audio_msgs/audio_common_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/audio_msgs/audio_common_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/audio_msgs/audio_event_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/audio_msgs/audio_event_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/audio_msgs/audio_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/audio_msgs/audio_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/direction_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/direction_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/drive_event_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/drive_event_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/drive_state_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/drive_state_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/error_code_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/error_code_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/geometry_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/geometry_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/header_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/header_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/pnc_point_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/pnc_point_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/vehicle_id_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/vehicle_id_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/vehicle_signal_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/basic_msgs/vehicle_signal_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/chassis_msgs/chassis_detail_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/chassis_msgs/chassis_detail_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/chassis_msgs/chassis_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/chassis_msgs/chassis_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/config_msgs/vehicle_config_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/config_msgs/vehicle_config_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/control_msgs/control_cmd_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/control_msgs/control_cmd_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/control_msgs/input_debug_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/control_msgs/input_debug_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/control_msgs/pad_msg_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/control_msgs/pad_msg_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/dreamview_msgs/chart_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/dreamview_msgs/chart_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/dreamview_msgs/hmi_status_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/dreamview_msgs/hmi_status_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/drivers_msgs/can_card_parameter_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/drivers_msgs/can_card_parameter_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/guardian_msgs/guardian_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/guardian_msgs/guardian_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/gps_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/gps_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/imu_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/imu_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/localization_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/localization_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/localization_status_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/localization_status_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/pose_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/localization_msgs/pose_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_clear_area_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_clear_area_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_crosswalk_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_crosswalk_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_geometry_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_geometry_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_id_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_id_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_junction_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_junction_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_lane_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_lane_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_overlap_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_overlap_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_parking_space_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_parking_space_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_pnc_junction_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_pnc_junction_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_road_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_road_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_rsu_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_rsu_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_signal_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_signal_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_speed_bump_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_speed_bump_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_speed_control_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_speed_control_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_stop_sign_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_stop_sign_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_yield_sign_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/map_msgs/map_yield_sign_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/monitor_msgs/monitor_log_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/monitor_msgs/monitor_log_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/monitor_msgs/smart_recorder_status_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/monitor_msgs/smart_recorder_status_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/monitor_msgs/system_status_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/monitor_msgs/system_status_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/perception_camera_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/perception_camera_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/perception_lane_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/perception_lane_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/perception_obstacle_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/perception_obstacle_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/traffic_light_detection_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/perception_msgs/traffic_light_detection_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/decision_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/decision_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/navigation_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/navigation_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/pad_msg_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/pad_msg_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/planning_internal_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/planning_internal_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/planning_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/planning_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/scenario_type_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/scenario_type_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/sl_boundary_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/planning_msgs/sl_boundary_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/feature_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/feature_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/lane_graph_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/lane_graph_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/prediction_obstacle_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/prediction_obstacle_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/prediction_point_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/prediction_point_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/scenario_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/prediction_msgs/scenario_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/routing_msgs/poi_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/routing_msgs/poi_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/routing_msgs/routing_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/routing_msgs/routing_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/conti_radar_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/conti_radar_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/delphi_esr_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/delphi_esr_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/gnss_best_pose_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/gnss_best_pose_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/gnss_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/gnss_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/gnss_raw_observation_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/gnss_raw_observation_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/heading_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/heading_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/imu_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/imu_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/ins_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/ins_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/mobileye_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/mobileye_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/pointcloud_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/pointcloud_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/racobit_radar_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/racobit_radar_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/radar_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/radar_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/sensor_image_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/sensor_image_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/smartereye_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/smartereye_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/ultrasonic_radar_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/sensor_msgs/ultrasonic_radar_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/agent_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/grading_condition_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/grading_condition_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/grading_metric_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/grading_metric_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/scenario_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/simulation_msgs/scenario_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/storytelling_msgs/story_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/storytelling_msgs/story_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/task_manager_msgs/task_manager_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/task_manager_msgs/task_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/transform_msgs/transform_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/transform_msgs/transform_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/baidu_apollo_proto/proto_v8/modules/common_msgs/v2x_msgs/v2x_traffic_light_pb2.py` & `baidu_apollo_proto-0.1.1/baidu_apollo_proto/proto_v8/modules/common_msgs/v2x_msgs/v2x_traffic_light_pb2.py`

 * *Files identical despite different names*

### Comparing `baidu_apollo_proto-0.1.0/PKG-INFO` & `baidu_apollo_proto-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: baidu-apollo-proto
-Version: 0.1.0
+Version: 0.1.1
 Summary: Compiled protobuff used in Baidu Apollo for Python.
 Author: Yuqi Huai
 Author-email: yhuai@uci.edu
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: protobuf (==3.19.0)
+Requires-Dist: protobuf (==3.19.5)
 Description-Content-Type: text/markdown
 
 # Baidu Apollo Proto
 
 This project compiles protobuf files used by Baidu Apollo for Python.
```

