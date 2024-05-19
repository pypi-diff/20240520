# Comparing `tmp/flwr_nightly-1.9.0.dev20240517.tar.gz` & `tmp/flwr_nightly-1.9.0.dev20240519.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.9.0.dev20240517.tar", max compression
+gzip compressed data, was "flwr_nightly-1.9.0.dev20240519.tar", max compression
```

## Comparing `flwr_nightly-1.9.0.dev20240517.tar` & `flwr_nightly-1.9.0.dev20240519.tar`

### file list

```diff
@@ -1,226 +1,231 @@
--rw-r--r--   0        0        0    11358 2024-05-17 23:05:25.047979 flwr_nightly-1.9.0.dev20240517/LICENSE
--rw-r--r--   0        0        0    12915 2024-05-17 23:05:25.047979 flwr_nightly-1.9.0.dev20240517/README.md
--rw-r--r--   0        0        0     5831 2024-05-17 23:05:37.368088 flwr_nightly-1.9.0.dev20240517/pyproject.toml
--rw-r--r--   0        0        0      937 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/__init__.py
--rw-r--r--   0        0        0      720 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/__init__.py
--rw-r--r--   0        0        0     1141 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/app.py
--rw-r--r--   0        0        0     5106 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/build.py
--rw-r--r--   0        0        0     4899 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/config_utils.py
--rw-r--r--   0        0        0     2215 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/example.py
--rw-r--r--   0        0        0      789 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/__init__.py
--rw-r--r--   0        0        0     6168 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/new.py
--rw-r--r--   0        0        0      725 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/__init__.py
--rw-r--r--   0        0        0     3078 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/.gitignore.tpl
--rw-r--r--   0        0        0      668 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/README.md.tpl
--rw-r--r--   0        0        0      729 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/__init__.py
--rw-r--r--   0        0        0      736 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/__init__.py
--rw-r--r--   0        0        0       21 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
--rw-r--r--   0        0        0     1450 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/client.hf.py.tpl
--rw-r--r--   0        0        0     2113 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/client.mlx.py.tpl
--rw-r--r--   0        0        0      521 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
--rw-r--r--   0        0        0     1172 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
--rw-r--r--   0        0        0     2801 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl
--rw-r--r--   0        0        0     1280 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
--rw-r--r--   0        0        0      338 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/server.hf.py.tpl
--rw-r--r--   0        0        0      272 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/server.mlx.py.tpl
--rw-r--r--   0        0        0      248 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
--rw-r--r--   0        0        0      593 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
--rw-r--r--   0        0        0      341 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/server.sklearn.py.tpl
--rw-r--r--   0        0        0      579 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
--rw-r--r--   0        0        0     2857 2024-05-17 23:05:25.459983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/task.hf.py.tpl
--rw-r--r--   0        0        0     2598 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/task.mlx.py.tpl
--rw-r--r--   0        0        0     3684 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
--rw-r--r--   0        0        0     1044 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/task.tensorflow.py.tpl
--rw-r--r--   0        0        0      676 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/pyproject.hf.toml.tpl
--rw-r--r--   0        0        0      585 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/pyproject.mlx.toml.tpl
--rw-r--r--   0        0        0      523 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
--rw-r--r--   0        0        0      592 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
--rw-r--r--   0        0        0      572 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl
--rw-r--r--   0        0        0      571 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
--rw-r--r--   0        0        0      789 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/run/__init__.py
--rw-r--r--   0        0        0     2334 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/run/run.py
--rw-r--r--   0        0        0     4119 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/utils.py
--rw-r--r--   0        0        0     1268 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    22313 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     8183 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     8636 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/client_app.py
--rw-r--r--   0        0        0     7435 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      735 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     8993 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      752 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     4903 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/grpc_rere_client/client_interceptor.py
--rw-r--r--   0        0        0     9597 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0     2404 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/heartbeat.py
--rw-r--r--   0        0        0      719 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     6553 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1824 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     1143 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/mod/__init__.py
--rw-r--r--   0        0        0     5415 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/mod/centraldp_mods.py
--rw-r--r--   0        0        0     2624 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/mod/comms_mods.py
--rw-r--r--   0        0        0     4982 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/mod/localdp_mod.py
--rw-r--r--   0        0        0      849 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/mod/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     1095 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
--rw-r--r--   0        0        0    19699 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
--rw-r--r--   0        0        0     1226 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/mod/utils.py
--rw-r--r--   0        0        0     1778 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/node_state.py
--rw-r--r--   0        0        0     2195 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/node_state_tests.py
--rw-r--r--   0        0        0    10283 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      735 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0    11520 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0      865 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/supernode/__init__.py
--rw-r--r--   0        0        0     9052 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/supernode/app.py
--rw-r--r--   0        0        0     1006 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/typing.py
--rw-r--r--   0        0        0     3721 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1882 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     2424 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0     1313 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/context.py
--rw-r--r--   0        0        0      891 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     6113 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/differential_privacy.py
--rw-r--r--   0        0        0     1074 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/differential_privacy_constants.py
--rw-r--r--   0        0        0     2004 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     2812 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/exit_handlers.py
--rw-r--r--   0        0        0     2460 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     7107 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0    13896 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/message.py
--rw-r--r--   0        0        0     4961 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/object_ref.py
--rw-r--r--   0        0        0     2095 2024-05-17 23:05:25.463983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0     1385 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/pyproject.py
--rw-r--r--   0        0        0     1054 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/record/__init__.py
--rw-r--r--   0        0        0     4652 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/record/configsrecord.py
--rw-r--r--   0        0        0     1393 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/record/conversion_utils.py
--rw-r--r--   0        0        0     3923 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/record/metricsrecord.py
--rw-r--r--   0        0        0     4838 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/record/parametersrecord.py
--rw-r--r--   0        0        0     5056 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/record/recordset.py
--rw-r--r--   0        0        0     3879 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/record/typeddict.py
--rw-r--r--   0        0        0    13798 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/recordset_compat.py
--rw-r--r--   0        0        0    11707 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/retry_invoker.py
--rw-r--r--   0        0        0      731 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/secure_aggregation/__init__.py
--rw-r--r--   0        0        0      738 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/secure_aggregation/crypto/__init__.py
--rw-r--r--   0        0        0     2792 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/secure_aggregation/crypto/shamir.py
--rw-r--r--   0        0        0     4707 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
--rw-r--r--   0        0        0     3026 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
--rw-r--r--   0        0        0     2310 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/secure_aggregation/quantization.py
--rw-r--r--   0        0        0     2183 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
--rw-r--r--   0        0        0     3221 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
--rw-r--r--   0        0        0    22250 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7865 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     4382 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      666 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      683 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     3207 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     5016 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     7304 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     2022 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     1084 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/error_pb2.py
--rw-r--r--   0        0        0      734 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/error_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/error_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/error_pb2_grpc.pyi
--rw-r--r--   0        0        0     5018 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     9161 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0    10605 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2811 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1081 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     6009 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/recordset_pb2.py
--rw-r--r--   0        0        0    14161 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/recordset_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/recordset_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/recordset_pb2_grpc.pyi
--rw-r--r--   0        0        0     2472 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4320 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0     9781 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1716 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    28913 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6127 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2399 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0      892 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/compat/__init__.py
--rw-r--r--   0        0        0     3421 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/compat/app.py
--rw-r--r--   0        0        0     3468 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/compat/app_utils.py
--rw-r--r--   0        0        0     5444 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/compat/driver_client_proxy.py
--rw-r--r--   0        0        0     1766 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/compat/legacy_context.py
--rw-r--r--   0        0        0     1061 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      862 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     5090 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/driver/driver.py
--rw-r--r--   0        0        0    11832 2024-05-17 23:05:25.467983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/driver/grpc_driver.py
--rw-r--r--   0        0        0     5063 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/history.py
--rw-r--r--   0        0        0     5972 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/run_serverapp.py
--rw-r--r--   0        0        0    17565 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/server.py
--rw-r--r--   0        0        0     4402 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/server_app.py
--rw-r--r--   0        0        0     1349 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/server_config.py
--rw-r--r--   0        0        0     2836 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0    13468 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     6532 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/bulyan.py
--rw-r--r--   0        0        0    17406 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/dp_adaptive_clipping.py
--rw-r--r--   0        0        0    12853 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/dp_fixed_clipping.py
--rw-r--r--   0        0        0     4877 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     7219 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5900 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6505 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     6763 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11799 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9784 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8132 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2704 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5242 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     6862 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5890 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     6080 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedxgb_bagging.py
--rw-r--r--   0        0        0     5607 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedxgb_cyclic.py
--rw-r--r--   0        0        0     4047 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     6801 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6285 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10150 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7543 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      707 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/__init__.py
--rw-r--r--   0        0        0      712 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/driver/__init__.py
--rw-r--r--   0        0        0     1932 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/driver/driver_grpc.py
--rw-r--r--   0        0        0     4791 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/driver/driver_servicer.py
--rw-r--r--   0        0        0      711 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/__init__.py
--rw-r--r--   0        0        0      735 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     5993 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6458 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4887 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11932 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0      758 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     3387 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0     7691 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py
--rw-r--r--   0        0        0      731 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     3622 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      735 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     7621 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0      783 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/vce/__init__.py
--rw-r--r--   0        0        0     1466 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
--rw-r--r--   0        0        0     2260 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
--rw-r--r--   0        0        0     6545 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
--rw-r--r--   0        0        0    12456 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/vce/vce_api.py
--rw-r--r--   0        0        0     1003 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/state/__init__.py
--rw-r--r--   0        0        0    12750 2024-05-17 23:05:25.471983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/state/in_memory_state.py
--rw-r--r--   0        0        0    28528 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/state/sqlite_state.py
--rw-r--r--   0        0        0     7989 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/state/state.py
--rw-r--r--   0        0        0     1654 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/state/state_factory.py
--rw-r--r--   0        0        0     2207 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/state/utils.py
--rw-r--r--   0        0        0      913 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/typing.py
--rw-r--r--   0        0        0      908 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5485 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     5301 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0      902 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/workflow/__init__.py
--rw-r--r--   0        0        0     1082 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/workflow/constant.py
--rw-r--r--   0        0        0    13227 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/workflow/default_workflows.py
--rw-r--r--   0        0        0      880 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/workflow/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     5838 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
--rw-r--r--   0        0        0    29038 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
--rw-r--r--   0        0        0     1348 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0    14380 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      734 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0    19367 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/simulation/ray_transport/ray_actor.py
--rw-r--r--   0        0        0     6738 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0     2392 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/simulation/ray_transport/utils.py
--rw-r--r--   0        0        0    16006 2024-05-17 23:05:25.475983 flwr_nightly-1.9.0.dev20240517/src/py/flwr/simulation/run_simulation.py
--rw-r--r--   0        0        0    15302 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240517/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-05-19 23:05:33.074234 flwr_nightly-1.9.0.dev20240519/LICENSE
+-rw-r--r--   0        0        0    12915 2024-05-19 23:05:33.074234 flwr_nightly-1.9.0.dev20240519/README.md
+-rw-r--r--   0        0        0     5831 2024-05-19 23:05:48.782432 flwr_nightly-1.9.0.dev20240519/pyproject.toml
+-rw-r--r--   0        0        0      937 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0      720 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/__init__.py
+-rw-r--r--   0        0        0     1141 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/app.py
+-rw-r--r--   0        0        0     5106 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/build.py
+-rw-r--r--   0        0        0     4899 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/config_utils.py
+-rw-r--r--   0        0        0     2215 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/example.py
+-rw-r--r--   0        0        0      789 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/__init__.py
+-rw-r--r--   0        0        0     6223 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/new.py
+-rw-r--r--   0        0        0      725 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/__init__.py
+-rw-r--r--   0        0        0     3078 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/.gitignore.tpl
+-rw-r--r--   0        0        0      668 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/README.md.tpl
+-rw-r--r--   0        0        0      729 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/__init__.py
+-rw-r--r--   0        0        0      736 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
+-rw-r--r--   0        0        0     1450 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/client.hf.py.tpl
+-rw-r--r--   0        0        0     1434 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/client.jax.py.tpl
+-rw-r--r--   0        0        0     2113 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/client.mlx.py.tpl
+-rw-r--r--   0        0        0      521 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
+-rw-r--r--   0        0        0     1172 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
+-rw-r--r--   0        0        0     2801 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl
+-rw-r--r--   0        0        0     1280 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
+-rw-r--r--   0        0        0      338 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/server.hf.py.tpl
+-rw-r--r--   0        0        0      246 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/server.jax.py.tpl
+-rw-r--r--   0        0        0      272 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/server.mlx.py.tpl
+-rw-r--r--   0        0        0      248 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
+-rw-r--r--   0        0        0      593 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
+-rw-r--r--   0        0        0      341 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/server.sklearn.py.tpl
+-rw-r--r--   0        0        0      579 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
+-rw-r--r--   0        0        0     2857 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/task.hf.py.tpl
+-rw-r--r--   0        0        0     1519 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/task.jax.py.tpl
+-rw-r--r--   0        0        0     2598 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/task.mlx.py.tpl
+-rw-r--r--   0        0        0     3684 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
+-rw-r--r--   0        0        0     1044 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/task.tensorflow.py.tpl
+-rw-r--r--   0        0        0      676 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/pyproject.hf.toml.tpl
+-rw-r--r--   0        0        0      568 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/pyproject.jax.toml.tpl
+-rw-r--r--   0        0        0      585 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/pyproject.mlx.toml.tpl
+-rw-r--r--   0        0        0      523 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
+-rw-r--r--   0        0        0      592 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
+-rw-r--r--   0        0        0      572 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl
+-rw-r--r--   0        0        0      571 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
+-rw-r--r--   0        0        0      789 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/run/__init__.py
+-rw-r--r--   0        0        0     2334 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/run/run.py
+-rw-r--r--   0        0        0     4119 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/utils.py
+-rw-r--r--   0        0        0     1268 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    22313 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     8183 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     8636 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/client_app.py
+-rw-r--r--   0        0        0     7435 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      735 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     8993 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      752 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     4903 2024-05-19 23:05:33.490239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/grpc_rere_client/client_interceptor.py
+-rw-r--r--   0        0        0     9597 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0     2404 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/heartbeat.py
+-rw-r--r--   0        0        0      719 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6553 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1824 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     1143 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/mod/__init__.py
+-rw-r--r--   0        0        0     5415 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/mod/centraldp_mods.py
+-rw-r--r--   0        0        0     2624 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/mod/comms_mods.py
+-rw-r--r--   0        0        0     4982 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/mod/localdp_mod.py
+-rw-r--r--   0        0        0      849 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/mod/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     1095 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
+-rw-r--r--   0        0        0    19699 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
+-rw-r--r--   0        0        0     1226 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/mod/utils.py
+-rw-r--r--   0        0        0     1778 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/node_state.py
+-rw-r--r--   0        0        0     2195 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/node_state_tests.py
+-rw-r--r--   0        0        0    10283 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      735 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0    11520 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0      865 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/supernode/__init__.py
+-rw-r--r--   0        0        0     9052 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/supernode/app.py
+-rw-r--r--   0        0        0     1006 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/typing.py
+-rw-r--r--   0        0        0     3721 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1882 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     2424 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0     1313 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/context.py
+-rw-r--r--   0        0        0      891 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     6113 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/differential_privacy.py
+-rw-r--r--   0        0        0     1074 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/differential_privacy_constants.py
+-rw-r--r--   0        0        0     2004 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     2812 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/exit_handlers.py
+-rw-r--r--   0        0        0     2460 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     7107 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0    13896 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/message.py
+-rw-r--r--   0        0        0     4961 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/object_ref.py
+-rw-r--r--   0        0        0     2095 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0     1385 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/pyproject.py
+-rw-r--r--   0        0        0     1054 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/record/__init__.py
+-rw-r--r--   0        0        0     4652 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/record/configsrecord.py
+-rw-r--r--   0        0        0     1393 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/record/conversion_utils.py
+-rw-r--r--   0        0        0     3923 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/record/metricsrecord.py
+-rw-r--r--   0        0        0     4838 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/record/parametersrecord.py
+-rw-r--r--   0        0        0     5056 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/record/recordset.py
+-rw-r--r--   0        0        0     3879 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/record/typeddict.py
+-rw-r--r--   0        0        0    13798 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/recordset_compat.py
+-rw-r--r--   0        0        0    11707 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/retry_invoker.py
+-rw-r--r--   0        0        0      731 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0      738 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/secure_aggregation/crypto/__init__.py
+-rw-r--r--   0        0        0     2792 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/secure_aggregation/crypto/shamir.py
+-rw-r--r--   0        0        0     4707 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
+-rw-r--r--   0        0        0     3026 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
+-rw-r--r--   0        0        0     2310 2024-05-19 23:05:33.494239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/secure_aggregation/quantization.py
+-rw-r--r--   0        0        0     2183 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
+-rw-r--r--   0        0        0     3221 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
+-rw-r--r--   0        0        0    22250 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7865 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     4382 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      666 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      683 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     3207 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     5016 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     7304 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     2022 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1084 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/error_pb2.py
+-rw-r--r--   0        0        0      734 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/error_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/error_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/error_pb2_grpc.pyi
+-rw-r--r--   0        0        0     5018 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     9161 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0    10605 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2811 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1081 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6009 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/recordset_pb2.py
+-rw-r--r--   0        0        0    14161 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/recordset_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/recordset_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/recordset_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2472 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4320 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9781 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1716 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    28913 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6127 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2399 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0      892 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/compat/__init__.py
+-rw-r--r--   0        0        0     3421 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/compat/app.py
+-rw-r--r--   0        0        0     3468 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/compat/app_utils.py
+-rw-r--r--   0        0        0     5444 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/compat/driver_client_proxy.py
+-rw-r--r--   0        0        0     1766 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/compat/legacy_context.py
+-rw-r--r--   0        0        0     1061 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      886 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     5090 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/driver/driver.py
+-rw-r--r--   0        0        0    11832 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/driver/grpc_driver.py
+-rw-r--r--   0        0        0     6490 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/driver/inmemory_driver.py
+-rw-r--r--   0        0        0     5063 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0     5972 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/run_serverapp.py
+-rw-r--r--   0        0        0    17821 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0     4402 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/server_app.py
+-rw-r--r--   0        0        0     1349 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/server_config.py
+-rw-r--r--   0        0        0     2836 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0    13468 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     6532 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/bulyan.py
+-rw-r--r--   0        0        0    17406 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/dp_adaptive_clipping.py
+-rw-r--r--   0        0        0    12853 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/dp_fixed_clipping.py
+-rw-r--r--   0        0        0     4877 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     7219 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5900 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6505 2024-05-19 23:05:33.498239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     6763 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11799 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9784 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8132 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2704 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5242 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     6862 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5890 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     6080 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedxgb_bagging.py
+-rw-r--r--   0        0        0     5607 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedxgb_cyclic.py
+-rw-r--r--   0        0        0     4047 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     6801 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6285 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10150 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7543 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      707 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/__init__.py
+-rw-r--r--   0        0        0      712 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/driver/__init__.py
+-rw-r--r--   0        0        0     1932 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/driver/driver_grpc.py
+-rw-r--r--   0        0        0     4791 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/driver/driver_servicer.py
+-rw-r--r--   0        0        0      711 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/__init__.py
+-rw-r--r--   0        0        0      735 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     5993 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6458 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4887 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11932 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0      758 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     3387 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0     7691 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py
+-rw-r--r--   0        0        0      731 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     3622 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      735 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     7621 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0      783 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/vce/__init__.py
+-rw-r--r--   0        0        0     1466 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
+-rw-r--r--   0        0        0     2260 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
+-rw-r--r--   0        0        0     6722 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
+-rw-r--r--   0        0        0    12456 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/vce/vce_api.py
+-rw-r--r--   0        0        0     1003 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/state/__init__.py
+-rw-r--r--   0        0        0    12750 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/state/in_memory_state.py
+-rw-r--r--   0        0        0    28528 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/state/sqlite_state.py
+-rw-r--r--   0        0        0     7989 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/state/state.py
+-rw-r--r--   0        0        0     1654 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/state/state_factory.py
+-rw-r--r--   0        0        0     2207 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/state/utils.py
+-rw-r--r--   0        0        0      913 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/typing.py
+-rw-r--r--   0        0        0      908 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5485 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     5301 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0      902 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/workflow/__init__.py
+-rw-r--r--   0        0        0     1082 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/workflow/constant.py
+-rw-r--r--   0        0        0    14003 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/workflow/default_workflows.py
+-rw-r--r--   0        0        0      880 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/workflow/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     5838 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
+-rw-r--r--   0        0        0    29038 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
+-rw-r--r--   0        0        0     1348 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0    14380 2024-05-19 23:05:33.502239 flwr_nightly-1.9.0.dev20240519/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      734 2024-05-19 23:05:33.506240 flwr_nightly-1.9.0.dev20240519/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0    19367 2024-05-19 23:05:33.506240 flwr_nightly-1.9.0.dev20240519/src/py/flwr/simulation/ray_transport/ray_actor.py
+-rw-r--r--   0        0        0     6738 2024-05-19 23:05:33.506240 flwr_nightly-1.9.0.dev20240519/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0     2392 2024-05-19 23:05:33.506240 flwr_nightly-1.9.0.dev20240519/src/py/flwr/simulation/ray_transport/utils.py
+-rw-r--r--   0        0        0    15098 2024-05-19 23:05:33.506240 flwr_nightly-1.9.0.dev20240519/src/py/flwr/simulation/run_simulation.py
+-rw-r--r--   0        0        0    15302 1970-01-01 00:00:00.000000 flwr_nightly-1.9.0.dev20240519/PKG-INFO
```

### Comparing `flwr_nightly-1.9.0.dev20240517/LICENSE` & `flwr_nightly-1.9.0.dev20240519/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/README.md` & `flwr_nightly-1.9.0.dev20240519/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/pyproject.toml` & `flwr_nightly-1.9.0.dev20240519/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.9.0.dev20240517"
+version = "1.9.0.dev20240519"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.ai>"]
 readme = "README.md"
 homepage = "https://flower.ai"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.ai"
```

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/app.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/build.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/build.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/config_utils.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/example.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/example.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/new.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/new.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 class MlFramework(str, Enum):
     """Available frameworks."""
 
     NUMPY = "NumPy"
     PYTORCH = "PyTorch"
     TENSORFLOW = "TensorFlow"
+    JAX = "JAX"
     HUGGINGFACE = "HF"
     MLX = "MLX"
     SKLEARN = "sklearn"
 
 
 class TemplateNotFound(Exception):
     """Raised when template does not exist."""
@@ -151,14 +152,15 @@
             "template": f"app/code/client.{framework_str}.py.tpl"
         },
     }
 
     # Depending on the framework, generate task.py file
     frameworks_with_tasks = [
         MlFramework.PYTORCH.value.lower(),
+        MlFramework.JAX.value.lower(),
         MlFramework.HUGGINGFACE.value.lower(),
         MlFramework.MLX.value.lower(),
         MlFramework.TENSORFLOW.value.lower(),
     ]
     if framework_str in frameworks_with_tasks:
         files[f"{import_name}/task.py"] = {
             "template": f"app/code/task.{framework_str}.py.tpl"
```

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/.gitignore.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/.gitignore.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/README.md.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/README.md.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/client.hf.py.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/client.hf.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/client.mlx.py.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/client.mlx.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/client.sklearn.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/task.hf.py.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/task.hf.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/task.mlx.py.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/task.mlx.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/code/task.tensorflow.py.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/code/task.tensorflow.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/pyproject.hf.toml.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/pyproject.hf.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/pyproject.mlx.toml.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/pyproject.mlx.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/pyproject.sklearn.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/run/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/run/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/run/run.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/run/run.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/cli/utils.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/cli/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/app.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/client.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/client_app.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/client_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/grpc_rere_client/client_interceptor.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/grpc_rere_client/client_interceptor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/heartbeat.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/heartbeat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/mod/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/mod/centraldp_mods.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/mod/centraldp_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/mod/comms_mods.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/mod/comms_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/mod/localdp_mod.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/mod/localdp_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/mod/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/mod/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/mod/utils.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/mod/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/node_state.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/node_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/node_state_tests.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/node_state_tests.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/rest_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/supernode/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/supernode/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/supernode/app.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/supernode/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/client/typing.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/client/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/address.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/constant.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/context.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/date.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/differential_privacy.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/differential_privacy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/differential_privacy_constants.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/differential_privacy_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/dp.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/exit_handlers.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/exit_handlers.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/grpc.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/logger.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/message.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/message.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/object_ref.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/object_ref.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/parameter.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/pyproject.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/pyproject.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/record/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/record/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/record/configsrecord.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/record/configsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/record/conversion_utils.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/record/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/record/metricsrecord.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/record/metricsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/record/parametersrecord.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/record/parametersrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/record/recordset.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/record/recordset.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/record/typeddict.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/record/typeddict.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/recordset_compat.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/recordset_compat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/retry_invoker.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/retry_invoker.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/secure_aggregation/crypto/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/secure_aggregation/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/secure_aggregation/crypto/shamir.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/secure_aggregation/crypto/shamir.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/secure_aggregation/quantization.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/secure_aggregation/quantization.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/secure_aggregation/secaggplus_constants.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/secure_aggregation/secaggplus_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/secure_aggregation/secaggplus_utils.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/secure_aggregation/secaggplus_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/serde.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/typing.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/common/version.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/error_pb2.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/error_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/error_pb2.pyi` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/recordset_pb2.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/recordset_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/recordset_pb2.pyi` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/recordset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/app.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/compat/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/compat/app.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/compat/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/compat/app_utils.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/compat/app_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/compat/driver_client_proxy.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/compat/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/compat/legacy_context.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/compat/legacy_context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/criterion.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,15 @@
-# Copyright 2022 Flower Labs GmbH. All Rights Reserved.
+# Copyright 2024 Flower Labs GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Flower driver SDK."""
-
-
-from .driver import Driver
-from .grpc_driver import GrpcDriver, GrpcDriverHelper
-
-__all__ = [
-    "Driver",
-    "GrpcDriver",
-    "GrpcDriverHelper",
-]
+"""Flower SuperLink."""
```

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/driver/driver.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/driver/grpc_driver.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/driver/grpc_driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/history.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/run_serverapp.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/run_serverapp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/server.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,22 @@
         # Get initial parameters from one of the clients
         log(INFO, "Requesting initial parameters from one random client")
         random_client = self._client_manager.sample(1)[0]
         ins = GetParametersIns(config={})
         get_parameters_res = random_client.get_parameters(
             ins=ins, timeout=timeout, group_id=server_round
         )
-        log(INFO, "Received initial parameters from one random client")
+        if get_parameters_res.status.code == Code.OK:
+            log(INFO, "Received initial parameters from one random client")
+        else:
+            log(
+                WARN,
+                "Failed to receive initial parameters from the client."
+                " Empty initial parameters will be used.",
+            )
         return get_parameters_res.parameters
 
 
 def reconnect_clients(
     client_instructions: List[Tuple[ClientProxy, ReconnectIns]],
     max_workers: Optional[int],
     timeout: Optional[float],
```

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/server_app.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/server_app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/server_config.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/server_config.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/bulyan.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/bulyan.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/dp_adaptive_clipping.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/dp_adaptive_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/dp_fixed_clipping.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/dp_fixed_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedxgb_bagging.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedxgb_bagging.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedxgb_cyclic.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedxgb_cyclic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# Copyright 2024 Flower Labs GmbH. All Rights Reserved.
+# Copyright 2020 Flower Labs GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Flower SuperLink."""
+"""Ray-based Flower ClientProxy implementation."""
```

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/driver/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/driver/driver_grpc.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/driver/driver_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/driver/driver_servicer.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/grpc_rere/server_interceptor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/message_handler/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/vce/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/vce/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/vce/backend/backend.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/vce/backend/backend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,20 @@
         if not pathlib.Path(work_dir).exists():
             raise ValueError(f"Specified work_dir {work_dir} does not exist.")
 
         # Init ray and append working dir if needed
         runtime_env = (
             self._configure_runtime_env(work_dir=work_dir) if work_dir else None
         )
-        if backend_config.get("silent", False):
+
+        if backend_config.get("mute_logging", False):
+            init_ray(
+                logging_level=WARNING, log_to_driver=False, runtime_env=runtime_env
+            )
+        elif backend_config.get("silent", False):
             init_ray(logging_level=WARNING, log_to_driver=True, runtime_env=runtime_env)
         else:
             init_ray(runtime_env=runtime_env)
 
         # Validate client resources
         self.client_resources_key = "client_resources"
```

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/fleet/vce/vce_api.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/fleet/vce/vce_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/state/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/state/in_memory_state.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/state/sqlite_state.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/state/state.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/state/state_factory.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/superlink/state/utils.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/superlink/state/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/typing.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/workflow/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/workflow/constant.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/workflow/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/workflow/default_workflows.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/workflow/default_workflows.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,30 @@
 # ==============================================================================
 """Legacy default workflows."""
 
 
 import io
 import timeit
 from logging import INFO, WARN
-from typing import Optional, cast
+from typing import List, Optional, Tuple, Union, cast
 
 import flwr.common.recordset_compat as compat
-from flwr.common import ConfigsRecord, Context, GetParametersIns, ParametersRecord, log
+from flwr.common import (
+    Code,
+    ConfigsRecord,
+    Context,
+    EvaluateRes,
+    FitRes,
+    GetParametersIns,
+    ParametersRecord,
+    log,
+)
 from flwr.common.constant import MessageType, MessageTypeLegacy
 
+from ..client_proxy import ClientProxy
 from ..compat.app_utils import start_update_client_manager_thread
 from ..compat.legacy_context import LegacyContext
 from ..driver import Driver
 from ..typing import Workflow
 from .constant import MAIN_CONFIGS_RECORD, MAIN_PARAMS_RECORD, Key
 
 
@@ -132,15 +142,22 @@
                     message_type=MessageTypeLegacy.GET_PARAMETERS,
                     dst_node_id=random_client.node_id,
                     group_id="0",
                 )
             ]
         )
         msg = list(messages)[0]
-        if msg.has_content():
+
+        if (
+            msg.has_content()
+            and compat._extract_status_from_recordset(  # pylint: disable=W0212
+                "getparametersres", msg.content
+            ).code
+            == Code.OK
+        ):
             log(INFO, "Received initial parameters from one random client")
             paramsrecord = next(iter(msg.content.parameters_records.values()))
         else:
             log(
                 WARN,
                 "Failed to receive initial parameters from the client."
                 " Empty initial parameters will be used.",
@@ -253,26 +270,28 @@
         INFO,
         "aggregate_fit: received %s results and %s failures",
         len(messages) - num_failures,
         num_failures,
     )
 
     # Aggregate training results
-    results = [
-        (
-            node_id_to_proxy[msg.metadata.src_node_id],
-            compat.recordset_to_fitres(msg.content, False),
-        )
-        for msg in messages
-        if msg.has_content()
-    ]
-    failures = [Exception(msg.error) for msg in messages if msg.has_error()]
-    aggregated_result = context.strategy.aggregate_fit(
-        current_round, results, failures  # type: ignore
-    )
+    results: List[Tuple[ClientProxy, FitRes]] = []
+    failures: List[Union[Tuple[ClientProxy, FitRes], BaseException]] = []
+    for msg in messages:
+        if msg.has_content():
+            proxy = node_id_to_proxy[msg.metadata.src_node_id]
+            fitres = compat.recordset_to_fitres(msg.content, False)
+            if fitres.status.code == Code.OK:
+                results.append((proxy, fitres))
+            else:
+                failures.append((proxy, fitres))
+        else:
+            failures.append(Exception(msg.error))
+
+    aggregated_result = context.strategy.aggregate_fit(current_round, results, failures)
     parameters_aggregated, metrics_aggregated = aggregated_result
 
     # Update the parameters and write history
     if parameters_aggregated:
         paramsrecord = compat.parameters_to_parametersrecord(
             parameters_aggregated, True
         )
@@ -337,25 +356,29 @@
         INFO,
         "aggregate_evaluate: received %s results and %s failures",
         len(messages) - num_failures,
         num_failures,
     )
 
     # Aggregate the evaluation results
-    results = [
-        (
-            node_id_to_proxy[msg.metadata.src_node_id],
-            compat.recordset_to_evaluateres(msg.content),
-        )
-        for msg in messages
-        if msg.has_content()
-    ]
-    failures = [Exception(msg.error) for msg in messages if msg.has_error()]
+    results: List[Tuple[ClientProxy, EvaluateRes]] = []
+    failures: List[Union[Tuple[ClientProxy, EvaluateRes], BaseException]] = []
+    for msg in messages:
+        if msg.has_content():
+            proxy = node_id_to_proxy[msg.metadata.src_node_id]
+            evalres = compat.recordset_to_evaluateres(msg.content)
+            if evalres.status.code == Code.OK:
+                results.append((proxy, evalres))
+            else:
+                failures.append((proxy, evalres))
+        else:
+            failures.append(Exception(msg.error))
+
     aggregated_result = context.strategy.aggregate_evaluate(
-        current_round, results, failures  # type: ignore
+        current_round, results, failures
     )
 
     loss_aggregated, metrics_aggregated = aggregated_result
 
     # Write history
     if loss_aggregated is not None:
         context.history.add_loss_distributed(
```

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/workflow/secure_aggregation/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/workflow/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/simulation/app.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/simulation/ray_transport/ray_actor.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/simulation/ray_transport/ray_actor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/simulation/ray_transport/utils.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/simulation/ray_transport/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.9.0.dev20240517/src/py/flwr/simulation/run_simulation.py` & `flwr_nightly-1.9.0.dev20240519/src/py/flwr/simulation/run_simulation.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,24 +20,21 @@
 import logging
 import threading
 import traceback
 from logging import DEBUG, ERROR, INFO, WARNING
 from time import sleep
 from typing import Dict, Optional
 
-import grpc
-
 from flwr.client import ClientApp
 from flwr.common import EventType, event, log
 from flwr.common.logger import set_logger_propagation, update_console_handler
 from flwr.common.typing import ConfigsRecordValues
-from flwr.server.driver import Driver, GrpcDriver
+from flwr.server.driver import Driver, InMemoryDriver
 from flwr.server.run_serverapp import run
 from flwr.server.server_app import ServerApp
-from flwr.server.superlink.driver.driver_grpc import run_driver_api_grpc
 from flwr.server.superlink.fleet import vce
 from flwr.server.superlink.state import StateFactory
 from flwr.simulation.ray_transport.utils import (
     enable_tf_gpu_growth as enable_gpu_growth,
 )
 
 
@@ -52,15 +49,14 @@
     _run_simulation(
         server_app_attr=args.server_app,
         client_app_attr=args.client_app,
         num_supernodes=args.num_supernodes,
         backend_name=args.backend,
         backend_config=backend_config_dict,
         app_dir=args.app_dir,
-        driver_api_address=args.driver_api_address,
         enable_tf_gpu_growth=args.enable_tf_gpu_growth,
         verbose_logging=args.verbose,
     )
 
 
 # Entry point from Python session (script or notebook)
 # pylint: disable=too-many-arguments
@@ -173,15 +169,14 @@
 
 
 # pylint: disable=too-many-locals
 def _main_loop(
     num_supernodes: int,
     backend_name: str,
     backend_config_stream: str,
-    driver_api_address: str,
     app_dir: str,
     enable_tf_gpu_growth: bool,
     client_app: Optional[ClientApp] = None,
     client_app_attr: Optional[str] = None,
     server_app: Optional[ServerApp] = None,
     server_app_attr: Optional[str] = None,
 ) -> None:
@@ -190,29 +185,19 @@
     Everything runs on the main thread or a separate one, depening on whether the main
     thread already contains a running Asyncio event loop. This is the case if running
     the Simulation Engine on a Jupyter/Colab notebook.
     """
     # Initialize StateFactory
     state_factory = StateFactory(":flwr-in-memory-state:")
 
-    # Start Driver API
-    driver_server: grpc.Server = run_driver_api_grpc(
-        address=driver_api_address,
-        state_factory=state_factory,
-        certificates=None,
-    )
-
     f_stop = asyncio.Event()
     serverapp_th = None
     try:
         # Initialize Driver
-        driver = GrpcDriver(
-            driver_service_address=driver_api_address,
-            root_certificates=None,
-        )
+        driver = InMemoryDriver(state_factory)
 
         # Get and run ServerApp thread
         serverapp_th = run_serverapp_th(
             server_app_attr=server_app_attr,
             server_app=server_app,
             driver=driver,
             app_dir=app_dir,
@@ -235,17 +220,14 @@
 
     except Exception as ex:
         log(ERROR, "An exception occurred !! %s", ex)
         log(ERROR, traceback.format_exc())
         raise RuntimeError("An error was encountered. Ending simulation.") from ex
 
     finally:
-        # Stop Driver
-        driver_server.stop(grace=0)
-        driver.close()
         # Trigger stop event
         f_stop.set()
 
         event(EventType.RUN_SUPERLINK_LEAVE)
         if serverapp_th:
             serverapp_th.join()
 
@@ -258,15 +240,14 @@
     client_app: Optional[ClientApp] = None,
     server_app: Optional[ServerApp] = None,
     backend_name: str = "ray",
     backend_config: Optional[Dict[str, ConfigsRecordValues]] = None,
     client_app_attr: Optional[str] = None,
     server_app_attr: Optional[str] = None,
     app_dir: str = "",
-    driver_api_address: str = "0.0.0.0:9091",
     enable_tf_gpu_growth: bool = False,
     verbose_logging: bool = False,
 ) -> None:
     r"""Launch the Simulation Engine.
 
     Parameters
     ----------
@@ -298,17 +279,14 @@
         A path to a `ServerApp` module to be loaded: For example: `server:app` or
         `project.package.module:wrapper.app`."
 
     app_dir : str
         Add specified directory to the PYTHONPATH and load `ClientApp` from there.
         (Default: current working directory.)
 
-    driver_api_address : str (default: "0.0.0.0:9091")
-        Driver API (gRPC) server address (IPv4, IPv6, or a domain name)
-
     enable_tf_gpu_growth : bool (default: False)
         A boolean to indicate whether to enable GPU growth on the main thread. This is
         desirable if you make use of a TensorFlow model on your `ServerApp` while
         having your `ClientApp` running on the same GPU. Without enabling this, you
         might encounter an out-of-memory error becasue TensorFlow by default allocates
         all GPU memory. Read mor about how `tf.config.experimental.set_memory_growth()`
         works in the TensorFlow documentation: https://www.tensorflow.org/api/stable.
@@ -338,15 +316,14 @@
     backend_config_stream = json.dumps(backend_config)
 
     simulation_engine_th = None
     args = (
         num_supernodes,
         backend_name,
         backend_config_stream,
-        driver_api_address,
         app_dir,
         enable_tf_gpu_growth,
         client_app,
         client_app_attr,
         server_app,
         server_app_attr,
     )
@@ -396,20 +373,14 @@
     parser.add_argument(
         "--num-supernodes",
         type=int,
         required=True,
         help="Number of simulated SuperNodes.",
     )
     parser.add_argument(
-        "--driver-api-address",
-        default="0.0.0.0:9091",
-        type=str,
-        help="For example: `server:app` or `project.package.module:wrapper.app`",
-    )
-    parser.add_argument(
         "--backend",
         default="ray",
         type=str,
         help="Simulation backend that executes the ClientApp.",
     )
     parser.add_argument(
         "--backend-config",
```

### Comparing `flwr_nightly-1.9.0.dev20240517/PKG-INFO` & `flwr_nightly-1.9.0.dev20240519/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.9.0.dev20240517
+Version: 1.9.0.dev20240519
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.ai
 License: Apache-2.0
 Keywords: flower,fl,federated learning,federated analytics,federated evaluation,machine learning
 Author: The Flower Authors
 Author-email: hello@flower.ai
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240517 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.9.0.dev20240519 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.ai
 License: Apache-2.0 Keywords: flower,fl,federated learning,federated
 analytics,federated evaluation,machine learning Author: The Flower Authors
 Author-email: hello@flower.ai Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
```

