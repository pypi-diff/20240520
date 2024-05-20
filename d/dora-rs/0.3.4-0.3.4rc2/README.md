# Comparing `tmp/dora_rs-0.3.4.tar.gz` & `tmp/dora_rs-0.3.4rc2.tar.gz`

## Comparing `dora_rs-0.3.4.tar` & `dora_rs-0.3.4rc2.tar`

### file list

```diff
@@ -1,120 +1,120 @@
--rw-r--r--   0     1001      127      549 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/python/operator/Cargo.toml
--rw-r--r--   0     1001      127     8166 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/python/operator/src/lib.rs
--rw-r--r--   0     1001      127      424 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/Cargo.toml
--rw-r--r--   0     1001      127    13680 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/lib.rs
--rw-r--r--   0     1001      127     4140 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/qos.rs
--rw-r--r--   0     1001      127      729 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/deserialize/array.rs
--rw-r--r--   0     1001      127     6330 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/deserialize/mod.rs
--rw-r--r--   0     1001      127     4726 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/deserialize/primitive.rs
--rw-r--r--   0     1001      127     6326 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/deserialize/sequence.rs
--rw-r--r--   0     1001      127     1154 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/deserialize/string.rs
--rw-r--r--   0     1001      127     4263 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/mod.rs
--rw-r--r--   0     1001      127     9390 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/serialize/array.rs
--rw-r--r--   0     1001      127     9481 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/serialize/defaults.rs
--rw-r--r--   0     1001      127     7776 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/serialize/mod.rs
--rw-r--r--   0     1001      127     3086 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/serialize/primitive.rs
--rw-r--r--   0     1001      127     9552 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/serialize/sequence.rs
--rw-r--r--   0     1001      127    11898 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/test_utils.py
--rw-r--r--   0     1001      127      461 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/rust/operator/types/Cargo.toml
--rw-r--r--   0     1001      127     4949 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/rust/operator/types/src/lib.rs
--rw-r--r--   0     1001      127      323 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/arrow-convert/Cargo.toml
--rw-r--r--   0     1001      127     5495 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/arrow-convert/src/from_impls.rs
--rw-r--r--   0     1001      127     3744 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/arrow-convert/src/into_impls.rs
--rw-r--r--   0     1001      127      485 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/arrow-convert/src/lib.rs
--rw-r--r--   0     1001      127      583 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/telemetry/tracing/Cargo.toml
--rw-r--r--   0     1001      127     1620 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/telemetry/tracing/src/lib.rs
--rw-r--r--   0     1001      127     2388 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/telemetry/tracing/src/telemetry.rs
--rw-r--r--   0     1001      127     1431 2024-05-20 16:38:59.000000 dora_rs-0.3.4/binaries/runtime/Cargo.toml
--rw-r--r--   0     1001      127    13120 2024-05-20 16:38:59.000000 dora_rs-0.3.4/binaries/runtime/src/lib.rs
--rw-r--r--   0     1001      127     4296 2024-05-20 16:38:59.000000 dora_rs-0.3.4/binaries/runtime/src/operator/channel.rs
--rw-r--r--   0     1001      127     2639 2024-05-20 16:38:59.000000 dora_rs-0.3.4/binaries/runtime/src/operator/mod.rs
--rw-r--r--   0     1001      127    15299 2024-05-20 16:38:59.000000 dora_rs-0.3.4/binaries/runtime/src/operator/python.rs
--rw-r--r--   0     1001      127    10280 2024-05-20 16:38:59.000000 dora_rs-0.3.4/binaries/runtime/src/operator/shared_lib.rs
--rw-r--r--   0     1001      127      451 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/message/Cargo.toml
--rw-r--r--   0     1001      127     4262 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/message/src/lib.rs
--rw-r--r--   0     1001      127     1213 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/Cargo.toml
--rw-r--r--   0     1001      127     1483 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/build.rs
--rw-r--r--   0     1001      127      276 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/src/_core/mod.rs
--rw-r--r--   0     1001      127     4114 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/src/_core/sequence.rs
--rw-r--r--   0     1001      127     5540 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/src/_core/string.rs
--rw-r--r--   0     1001      127     2337 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/src/_core/traits.rs
--rw-r--r--   0     1001      127      262 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/src/lib.rs
--rw-r--r--   0     1001      127      593 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/shared-memory-server/Cargo.toml
--rw-r--r--   0     1001      127     3249 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/shared-memory-server/src/bin/bench.rs
--rw-r--r--   0     1001      127     7343 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/shared-memory-server/src/channel.rs
--rw-r--r--   0     1001      127     2058 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/shared-memory-server/src/lib.rs
--rw-r--r--   0     1001      127      322 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/Cargo.toml
--rw-r--r--   0     1001      127      787 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/build.rs
--rw-r--r--   0     1001      127    11235 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/lib.rs
--rw-r--r--   0     1001      127     3703 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/action.rs
--rw-r--r--   0     1001      127     2848 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/constant.rs
--rw-r--r--   0     1001      127      776 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/error.rs
--rw-r--r--   0     1001      127     2257 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/ident.rs
--rw-r--r--   0     1001      127     9397 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/literal.rs
--rw-r--r--   0     1001      127     4376 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/member.rs
--rw-r--r--   0     1001      127     4024 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/message.rs
--rw-r--r--   0     1001      127      191 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/mod.rs
--rw-r--r--   0     1001      127     3354 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/package.rs
--rw-r--r--   0     1001      127     2607 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/service.rs
--rw-r--r--   0     1001      127    10878 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/types.rs
--rw-r--r--   0     1001      127     7208 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/types/action.rs
--rw-r--r--   0     1001      127     1910 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/types/constant.rs
--rw-r--r--   0     1001      127     4429 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/types/member.rs
--rw-r--r--   0     1001      127    20805 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/types/message.rs
--rw-r--r--   0     1001      127      299 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/types/mod.rs
--rw-r--r--   0     1001      127     3790 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/types/package.rs
--rw-r--r--   0     1001      127    12149 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/types/primitives.rs
--rw-r--r--   0     1001      127     3382 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/types/sequences.rs
--rw-r--r--   0     1001      127    11907 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/types/service.rs
--rw-r--r--   0     1001      127      100 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/action/Fibonacci.action
--rw-r--r--   0     1001      127     1271 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Arrays.msg
--rw-r--r--   0     1001      127      240 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BasicTypes.msg
--rw-r--r--   0     1001      127     1346 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BoundedSequences.msg
--rw-r--r--   0     1001      127      315 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Constants.msg
--rw-r--r--   0     1001      127      315 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Defaults.msg
--rw-r--r--   0     1001      127        0 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Empty.msg
--rw-r--r--   0     1001      127      484 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/MultiNested.msg
--rw-r--r--   0     1001      127       29 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Nested.msg
--rw-r--r--   0     1001      127      591 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Strings.msg
--rw-r--r--   0     1001      127     1255 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/UnboundedSequences.msg
--rw-r--r--   0     1001      127      415 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/WStrings.msg
--rw-r--r--   0     1001      127     2282 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Arrays.srv
--rw-r--r--   0     1001      127      524 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/BasicTypes.srv
--rw-r--r--   0     1001      127        4 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Empty.srv
--rw-r--r--   0     1001      127      561 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/telemetry/metrics/Cargo.toml
--rw-r--r--   0     1001      127     1828 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/telemetry/metrics/src/lib.rs
--rw-r--r--   0     1001      127      665 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/core/Cargo.toml
--rw-r--r--   0     1001      127     9127 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/core/src/config.rs
--rw-r--r--   0     1001      127      922 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/core/src/coordinator_messages.rs
--rw-r--r--   0     1001      127     7006 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/core/src/daemon_messages.rs
--rw-r--r--   0     1001      127    11553 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/core/src/descriptor/mod.rs
--rw-r--r--   0     1001      127     7331 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/core/src/descriptor/validate.rs
--rw-r--r--   0     1001      127     7349 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/core/src/descriptor/visualize.rs
--rw-r--r--   0     1001      127     2397 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/core/src/lib.rs
--rw-r--r--   0     1001      127     2170 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/core/src/topics.rs
--rw-r--r--   0     1001      127      733 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/rust/node/Cargo.toml
--rw-r--r--   0     1001      127     2429 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/rust/node/src/daemon_connection/mod.rs
--rw-r--r--   0     1001      127     2149 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/rust/node/src/daemon_connection/tcp.rs
--rw-r--r--   0     1001      127     3457 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/rust/node/src/event_stream/event.rs
--rw-r--r--   0     1001      127     3100 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/rust/node/src/event_stream/merged.rs
--rw-r--r--   0     1001      127     8375 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/rust/node/src/event_stream/mod.rs
--rw-r--r--   0     1001      127     9280 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/rust/node/src/event_stream/thread.rs
--rw-r--r--   0     1001      127      764 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/rust/node/src/lib.rs
--rw-r--r--   0     1001      127     2553 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/rust/node/src/node/arrow_utils.rs
--rw-r--r--   0     1001      127     3654 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/rust/node/src/node/control_channel.rs
--rw-r--r--   0     1001      127     5795 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/rust/node/src/node/drop_stream.rs
--rw-r--r--   0     1001      127    14339 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/rust/node/src/node/mod.rs
--rw-r--r--   0     1001      127      452 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/download/Cargo.toml
--rw-r--r--   0     1001      127     1285 2024-05-20 16:38:59.000000 dora_rs-0.3.4/libraries/extensions/download/src/lib.rs
--rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 dora_rs-0.3.4/apis/python/node/Cargo.toml
--rw-r--r--   0     1001      127      339 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/python/node/README.md
--rw-r--r--   0     1001      127      723 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/python/node/dora/__init__.py
--rw-r--r--   0     1001      127     8499 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/python/node/dora/__init__.pyi
--rw-r--r--   0     1001      127    17717 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/python/node/generate_stubs.py
--rw-r--r--   0     1001      127     8051 2024-05-20 16:38:59.000000 dora_rs-0.3.4/apis/python/node/src/lib.rs
--rw-r--r--   0     1001      127   262765 2024-05-20 16:38:59.000000 dora_rs-0.3.4/Cargo.lock
--rw-r--r--   0        0        0     3875 1970-01-01 00:00:00.000000 dora_rs-0.3.4/Cargo.toml
--rw-r--r--   0        0        0      272 1970-01-01 00:00:00.000000 dora_rs-0.3.4/pyproject.toml
--rw-r--r--   0     1001      127      723 2024-05-20 16:38:59.000000 dora_rs-0.3.4/dora/__init__.py
--rw-r--r--   0     1001      127     8499 2024-05-20 16:38:59.000000 dora_rs-0.3.4/dora/__init__.pyi
--rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 dora_rs-0.3.4/PKG-INFO
+-rw-r--r--   0     1001      127      549 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/python/operator/Cargo.toml
+-rw-r--r--   0     1001      127     8166 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/python/operator/src/lib.rs
+-rw-r--r--   0     1001      127     1213 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/Cargo.toml
+-rw-r--r--   0     1001      127     1483 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/build.rs
+-rw-r--r--   0     1001      127      276 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/src/_core/mod.rs
+-rw-r--r--   0     1001      127     4114 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/src/_core/sequence.rs
+-rw-r--r--   0     1001      127     5540 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/src/_core/string.rs
+-rw-r--r--   0     1001      127     2337 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/src/_core/traits.rs
+-rw-r--r--   0     1001      127      262 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/src/lib.rs
+-rw-r--r--   0     1001      127      665 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/core/Cargo.toml
+-rw-r--r--   0     1001      127     9127 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/core/src/config.rs
+-rw-r--r--   0     1001      127      922 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/core/src/coordinator_messages.rs
+-rw-r--r--   0     1001      127     7006 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/core/src/daemon_messages.rs
+-rw-r--r--   0     1001      127    11553 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/core/src/descriptor/mod.rs
+-rw-r--r--   0     1001      127     7331 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/core/src/descriptor/validate.rs
+-rw-r--r--   0     1001      127     7349 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/core/src/descriptor/visualize.rs
+-rw-r--r--   0     1001      127     2397 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/core/src/lib.rs
+-rw-r--r--   0     1001      127     2170 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/core/src/topics.rs
+-rw-r--r--   0     1001      127      452 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/download/Cargo.toml
+-rw-r--r--   0     1001      127     1285 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/download/src/lib.rs
+-rw-r--r--   0     1001      127      561 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/telemetry/metrics/Cargo.toml
+-rw-r--r--   0     1001      127     1828 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/telemetry/metrics/src/lib.rs
+-rw-r--r--   0     1001      127      322 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/Cargo.toml
+-rw-r--r--   0     1001      127      787 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/build.rs
+-rw-r--r--   0     1001      127    11235 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/lib.rs
+-rw-r--r--   0     1001      127     3703 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/action.rs
+-rw-r--r--   0     1001      127     2848 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/constant.rs
+-rw-r--r--   0     1001      127      776 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/error.rs
+-rw-r--r--   0     1001      127     2257 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/ident.rs
+-rw-r--r--   0     1001      127     9397 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/literal.rs
+-rw-r--r--   0     1001      127     4376 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/member.rs
+-rw-r--r--   0     1001      127     4024 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/message.rs
+-rw-r--r--   0     1001      127      191 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/mod.rs
+-rw-r--r--   0     1001      127     3354 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/package.rs
+-rw-r--r--   0     1001      127     2607 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/service.rs
+-rw-r--r--   0     1001      127    10878 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/types.rs
+-rw-r--r--   0     1001      127     7208 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/action.rs
+-rw-r--r--   0     1001      127     1910 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/constant.rs
+-rw-r--r--   0     1001      127     4429 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/member.rs
+-rw-r--r--   0     1001      127    20805 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/message.rs
+-rw-r--r--   0     1001      127      299 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/mod.rs
+-rw-r--r--   0     1001      127     3790 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/package.rs
+-rw-r--r--   0     1001      127    12149 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/primitives.rs
+-rw-r--r--   0     1001      127     3382 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/sequences.rs
+-rw-r--r--   0     1001      127    11907 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/service.rs
+-rw-r--r--   0     1001      127      100 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/action/Fibonacci.action
+-rw-r--r--   0     1001      127     1271 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Arrays.msg
+-rw-r--r--   0     1001      127      240 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BasicTypes.msg
+-rw-r--r--   0     1001      127     1346 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BoundedSequences.msg
+-rw-r--r--   0     1001      127      315 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Constants.msg
+-rw-r--r--   0     1001      127      315 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Defaults.msg
+-rw-r--r--   0     1001      127        0 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Empty.msg
+-rw-r--r--   0     1001      127      484 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/MultiNested.msg
+-rw-r--r--   0     1001      127       29 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Nested.msg
+-rw-r--r--   0     1001      127      591 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Strings.msg
+-rw-r--r--   0     1001      127     1255 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/UnboundedSequences.msg
+-rw-r--r--   0     1001      127      415 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/WStrings.msg
+-rw-r--r--   0     1001      127     2282 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Arrays.srv
+-rw-r--r--   0     1001      127      524 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/BasicTypes.srv
+-rw-r--r--   0     1001      127        4 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Empty.srv
+-rw-r--r--   0     1001      127      733 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/Cargo.toml
+-rw-r--r--   0     1001      127     2429 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/daemon_connection/mod.rs
+-rw-r--r--   0     1001      127     2149 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/daemon_connection/tcp.rs
+-rw-r--r--   0     1001      127     3457 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/event_stream/event.rs
+-rw-r--r--   0     1001      127     3100 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/event_stream/merged.rs
+-rw-r--r--   0     1001      127     8375 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/event_stream/mod.rs
+-rw-r--r--   0     1001      127     9280 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/event_stream/thread.rs
+-rw-r--r--   0     1001      127      764 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/lib.rs
+-rw-r--r--   0     1001      127     2553 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/node/arrow_utils.rs
+-rw-r--r--   0     1001      127     3654 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/node/control_channel.rs
+-rw-r--r--   0     1001      127     5795 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/node/drop_stream.rs
+-rw-r--r--   0     1001      127    14339 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/node/src/node/mod.rs
+-rw-r--r--   0     1001      127      583 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/telemetry/tracing/Cargo.toml
+-rw-r--r--   0     1001      127     1620 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/telemetry/tracing/src/lib.rs
+-rw-r--r--   0     1001      127     2388 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/telemetry/tracing/src/telemetry.rs
+-rw-r--r--   0     1001      127      424 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/Cargo.toml
+-rw-r--r--   0     1001      127    13680 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/lib.rs
+-rw-r--r--   0     1001      127     4140 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/qos.rs
+-rw-r--r--   0     1001      127      729 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/array.rs
+-rw-r--r--   0     1001      127     6330 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/mod.rs
+-rw-r--r--   0     1001      127     4726 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/primitive.rs
+-rw-r--r--   0     1001      127     6326 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/sequence.rs
+-rw-r--r--   0     1001      127     1154 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/string.rs
+-rw-r--r--   0     1001      127     4263 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/mod.rs
+-rw-r--r--   0     1001      127     9390 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/array.rs
+-rw-r--r--   0     1001      127     9481 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/defaults.rs
+-rw-r--r--   0     1001      127     7776 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/mod.rs
+-rw-r--r--   0     1001      127     3086 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/primitive.rs
+-rw-r--r--   0     1001      127     9552 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/sequence.rs
+-rw-r--r--   0     1001      127    11898 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/test_utils.py
+-rw-r--r--   0     1001      127     1431 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/binaries/runtime/Cargo.toml
+-rw-r--r--   0     1001      127    13120 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/binaries/runtime/src/lib.rs
+-rw-r--r--   0     1001      127     4296 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/binaries/runtime/src/operator/channel.rs
+-rw-r--r--   0     1001      127     2639 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/binaries/runtime/src/operator/mod.rs
+-rw-r--r--   0     1001      127    15299 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/binaries/runtime/src/operator/python.rs
+-rw-r--r--   0     1001      127    10280 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/binaries/runtime/src/operator/shared_lib.rs
+-rw-r--r--   0     1001      127      461 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/operator/types/Cargo.toml
+-rw-r--r--   0     1001      127     4949 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/rust/operator/types/src/lib.rs
+-rw-r--r--   0     1001      127      323 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/arrow-convert/Cargo.toml
+-rw-r--r--   0     1001      127     5495 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/arrow-convert/src/from_impls.rs
+-rw-r--r--   0     1001      127     3744 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/arrow-convert/src/into_impls.rs
+-rw-r--r--   0     1001      127      485 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/arrow-convert/src/lib.rs
+-rw-r--r--   0     1001      127      451 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/message/Cargo.toml
+-rw-r--r--   0     1001      127     4262 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/message/src/lib.rs
+-rw-r--r--   0     1001      127      593 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/shared-memory-server/Cargo.toml
+-rw-r--r--   0     1001      127     3249 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/shared-memory-server/src/bin/bench.rs
+-rw-r--r--   0     1001      127     7343 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/shared-memory-server/src/channel.rs
+-rw-r--r--   0     1001      127     2058 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/libraries/shared-memory-server/src/lib.rs
+-rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 dora_rs-0.3.4rc2/apis/python/node/Cargo.toml
+-rw-r--r--   0     1001      127      339 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/python/node/README.md
+-rw-r--r--   0     1001      127      723 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/python/node/dora/__init__.py
+-rw-r--r--   0     1001      127     8425 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/python/node/dora/__init__.pyi
+-rw-r--r--   0     1001      127    17717 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/python/node/generate_stubs.py
+-rw-r--r--   0     1001      127     7897 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/apis/python/node/src/lib.rs
+-rw-r--r--   0     1001      127   262901 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/Cargo.lock
+-rw-r--r--   0        0        0     3955 1970-01-01 00:00:00.000000 dora_rs-0.3.4rc2/Cargo.toml
+-rw-r--r--   0        0        0      272 1970-01-01 00:00:00.000000 dora_rs-0.3.4rc2/pyproject.toml
+-rw-r--r--   0     1001      127      723 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/dora/__init__.py
+-rw-r--r--   0     1001      127     8425 2024-05-17 14:11:34.000000 dora_rs-0.3.4rc2/dora/__init__.pyi
+-rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 dora_rs-0.3.4rc2/PKG-INFO
```

### Comparing `dora_rs-0.3.4/apis/python/operator/Cargo.toml` & `dora_rs-0.3.4rc2/apis/python/operator/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/apis/python/operator/src/lib.rs` & `dora_rs-0.3.4rc2/apis/python/operator/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/lib.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/qos.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/qos.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/deserialize/array.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/array.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/deserialize/mod.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/deserialize/primitive.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/primitive.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/deserialize/sequence.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/sequence.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/deserialize/string.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/deserialize/string.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/mod.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/serialize/array.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/array.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/serialize/defaults.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/defaults.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/serialize/mod.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/serialize/primitive.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/primitive.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/src/typed/serialize/sequence.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/src/typed/serialize/sequence.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/python/test_utils.py` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/python/test_utils.py`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/apis/rust/operator/types/src/lib.rs` & `dora_rs-0.3.4rc2/apis/rust/operator/types/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/arrow-convert/src/from_impls.rs` & `dora_rs-0.3.4rc2/libraries/arrow-convert/src/from_impls.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/arrow-convert/src/into_impls.rs` & `dora_rs-0.3.4rc2/libraries/arrow-convert/src/into_impls.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/telemetry/tracing/Cargo.toml` & `dora_rs-0.3.4rc2/libraries/extensions/telemetry/tracing/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/telemetry/tracing/src/lib.rs` & `dora_rs-0.3.4rc2/libraries/extensions/telemetry/tracing/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/telemetry/tracing/src/telemetry.rs` & `dora_rs-0.3.4rc2/libraries/extensions/telemetry/tracing/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/binaries/runtime/Cargo.toml` & `dora_rs-0.3.4rc2/binaries/runtime/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/binaries/runtime/src/lib.rs` & `dora_rs-0.3.4rc2/binaries/runtime/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/binaries/runtime/src/operator/channel.rs` & `dora_rs-0.3.4rc2/binaries/runtime/src/operator/channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/binaries/runtime/src/operator/mod.rs` & `dora_rs-0.3.4rc2/binaries/runtime/src/operator/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/binaries/runtime/src/operator/python.rs` & `dora_rs-0.3.4rc2/binaries/runtime/src/operator/python.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/binaries/runtime/src/operator/shared_lib.rs` & `dora_rs-0.3.4rc2/binaries/runtime/src/operator/shared_lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/message/src/lib.rs` & `dora_rs-0.3.4rc2/libraries/message/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/Cargo.toml` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/build.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/build.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/src/_core/sequence.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/src/_core/sequence.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/src/_core/string.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/src/_core/string.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/src/_core/traits.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/src/_core/traits.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/shared-memory-server/Cargo.toml` & `dora_rs-0.3.4rc2/libraries/shared-memory-server/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/shared-memory-server/src/bin/bench.rs` & `dora_rs-0.3.4rc2/libraries/shared-memory-server/src/bin/bench.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/shared-memory-server/src/channel.rs` & `dora_rs-0.3.4rc2/libraries/shared-memory-server/src/channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/shared-memory-server/src/lib.rs` & `dora_rs-0.3.4rc2/libraries/shared-memory-server/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/build.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/build.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/lib.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/action.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/action.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/constant.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/constant.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/error.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/error.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/ident.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/ident.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/literal.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/literal.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/member.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/member.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/message.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/message.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/package.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/package.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/service.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/service.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/parser/types.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/parser/types.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/types/action.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/action.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/types/constant.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/constant.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/types/member.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/member.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/types/message.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/message.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/types/package.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/package.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/types/primitives.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/primitives.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/types/sequences.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/sequences.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/src/types/service.rs` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/src/types/service.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Arrays.msg` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Arrays.msg`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BoundedSequences.msg` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/BoundedSequences.msg`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Strings.msg` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/Strings.msg`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/UnboundedSequences.msg` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/msg/UnboundedSequences.msg`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Arrays.srv` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/Arrays.srv`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/BasicTypes.srv` & `dora_rs-0.3.4rc2/libraries/extensions/ros2-bridge/msg-gen/test_msgs/srv/BasicTypes.srv`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/telemetry/metrics/Cargo.toml` & `dora_rs-0.3.4rc2/libraries/extensions/telemetry/metrics/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/telemetry/metrics/src/lib.rs` & `dora_rs-0.3.4rc2/libraries/extensions/telemetry/metrics/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/core/Cargo.toml` & `dora_rs-0.3.4rc2/libraries/core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/core/src/config.rs` & `dora_rs-0.3.4rc2/libraries/core/src/config.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/core/src/coordinator_messages.rs` & `dora_rs-0.3.4rc2/libraries/core/src/coordinator_messages.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/core/src/daemon_messages.rs` & `dora_rs-0.3.4rc2/libraries/core/src/daemon_messages.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/core/src/descriptor/mod.rs` & `dora_rs-0.3.4rc2/libraries/core/src/descriptor/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/core/src/descriptor/validate.rs` & `dora_rs-0.3.4rc2/libraries/core/src/descriptor/validate.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/core/src/descriptor/visualize.rs` & `dora_rs-0.3.4rc2/libraries/core/src/descriptor/visualize.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/core/src/lib.rs` & `dora_rs-0.3.4rc2/libraries/core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/core/src/topics.rs` & `dora_rs-0.3.4rc2/libraries/core/src/topics.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/apis/rust/node/Cargo.toml` & `dora_rs-0.3.4rc2/apis/rust/node/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/apis/rust/node/src/daemon_connection/mod.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/daemon_connection/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/apis/rust/node/src/daemon_connection/tcp.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/daemon_connection/tcp.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/apis/rust/node/src/event_stream/event.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/event_stream/event.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/apis/rust/node/src/event_stream/merged.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/event_stream/merged.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/apis/rust/node/src/event_stream/mod.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/event_stream/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/apis/rust/node/src/event_stream/thread.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/event_stream/thread.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/apis/rust/node/src/lib.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/apis/rust/node/src/node/arrow_utils.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/node/arrow_utils.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/apis/rust/node/src/node/control_channel.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/node/control_channel.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/apis/rust/node/src/node/drop_stream.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/node/drop_stream.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/apis/rust/node/src/node/mod.rs` & `dora_rs-0.3.4rc2/apis/rust/node/src/node/mod.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/libraries/extensions/download/src/lib.rs` & `dora_rs-0.3.4rc2/libraries/extensions/download/src/lib.rs`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/apis/python/node/Cargo.toml` & `dora_rs-0.3.4rc2/apis/python/node/Cargo.toml`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/apis/python/node/dora/__init__.py` & `dora_rs-0.3.4rc2/apis/python/node/dora/__init__.py`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/apis/python/node/dora/__init__.pyi` & `dora_rs-0.3.4rc2/apis/python/node/dora/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -35,17 +35,14 @@
 ```"""
 
     def dataflow_descriptor(self) -> dict:
         """Returns the full dataflow descriptor that this node is part of.
 
 This method returns the parsed dataflow YAML file."""
 
-    def dataflow_id(self) -> str:
-        """Returns the dataflow id."""
-
     def merge_external_events(self, subscription: dora.Ros2Subscription) -> None:
         """Merge an external event stream with dora main loop.
 This currently only work with ROS2."""
 
     def next(self, timeout: float=None) -> dora.PyEvent:
         """`.next()` gives you the next input that the node has received.
 It blocks until the next event becomes available.
```

### Comparing `dora_rs-0.3.4/apis/python/node/generate_stubs.py` & `dora_rs-0.3.4rc2/apis/python/node/generate_stubs.py`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/apis/python/node/src/lib.rs` & `dora_rs-0.3.4rc2/apis/python/node/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -150,21 +150,14 @@
     /// This method returns the parsed dataflow YAML file.
     ///
     /// :rtype: dict
     pub fn dataflow_descriptor(&self, py: Python) -> pythonize::Result<PyObject> {
         pythonize::pythonize(py, self.node.dataflow_descriptor())
     }
 
-    /// Returns the dataflow id.
-    ///
-    /// :rtype: str
-    pub fn dataflow_id(&self) -> String {
-        self.node.dataflow_id().to_string()
-    }
-
     /// Merge an external event stream with dora main loop.
     /// This currently only work with ROS2.
     ///
     /// :type subscription: dora.Ros2Subscription
     /// :rtype: None
     pub fn merge_external_events(
         &mut self,
```

### Comparing `dora_rs-0.3.4/Cargo.lock` & `dora_rs-0.3.4rc2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1052,28 +1052,28 @@
  "unicode-width",
  "walkdir",
  "wild",
 ]
 
 [[package]]
 name = "benchmark-example-node"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "benchmark-example-sink"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-node-api",
  "eyre",
  "tracing",
  "tracing-subscriber",
 ]
 
@@ -1696,23 +1696,23 @@
  "strum 0.26.2",
  "strum_macros 0.26.2",
  "unicode-width",
 ]
 
 [[package]]
 name = "communication-layer-pub-sub"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "flume 0.10.14",
  "zenoh",
 ]
 
 [[package]]
 name = "communication-layer-request-reply"
-version = "0.3.4"
+version = "0.3.4-rc2"
 
 [[package]]
 name = "concurrent-queue"
 version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f057a694a54f12365049b0958a1685bb52d567f5593b355fbf685838e873d400"
 dependencies = [
@@ -2237,23 +2237,23 @@
 checksum = "ef5282ad69563b5fc40319526ba27e0e7363d552a896f0297d54f767717f9b95"
 dependencies = [
  "litrs",
 ]
 
 [[package]]
 name = "dora-arrow-convert"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "arrow",
  "eyre",
 ]
 
 [[package]]
 name = "dora-cli"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "bat",
  "clap 4.4.6",
  "communication-layer-request-reply",
  "ctrlc",
  "dora-coordinator",
  "dora-core",
@@ -2276,15 +2276,15 @@
  "tracing",
  "uuid",
  "webbrowser",
 ]
 
 [[package]]
 name = "dora-coordinator"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "ctrlc",
  "dora-core",
  "dora-tracing",
  "eyre",
  "futures",
  "futures-concurrency",
@@ -2294,15 +2294,15 @@
  "tokio-stream",
  "tracing",
  "uuid",
 ]
 
 [[package]]
 name = "dora-core"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "aligned-vec",
  "dora-message",
  "eyre",
  "once_cell",
  "serde",
  "serde-with-expand-env",
@@ -2311,15 +2311,15 @@
  "tracing",
  "uuid",
  "which",
 ]
 
 [[package]]
 name = "dora-daemon"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "aligned-vec",
  "async-trait",
  "bincode",
  "ctrlc",
  "dora-arrow-convert",
  "dora-core",
@@ -2340,15 +2340,15 @@
  "tracing-opentelemetry",
  "uuid",
  "which",
 ]
 
 [[package]]
 name = "dora-download"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "eyre",
  "reqwest",
  "tokio",
  "tracing",
 ]
 
@@ -2368,37 +2368,37 @@
  "tokio-stream",
  "tracing",
  "uuid",
 ]
 
 [[package]]
 name = "dora-message"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "arrow-data",
  "arrow-schema",
  "eyre",
  "serde",
  "uhlc",
 ]
 
 [[package]]
 name = "dora-metrics"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "eyre",
  "opentelemetry 0.22.0",
  "opentelemetry-otlp",
  "opentelemetry-system-metrics",
  "opentelemetry_sdk 0.22.1",
 ]
 
 [[package]]
 name = "dora-node-api"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "aligned-vec",
  "arrow",
  "bincode",
  "dora-arrow-convert",
  "dora-core",
  "dora-tracing",
@@ -2412,25 +2412,25 @@
  "shared_memory_extended",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "dora-node-api-c"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "arrow-array",
  "dora-node-api",
  "eyre",
  "tracing",
 ]
 
 [[package]]
 name = "dora-node-api-cxx"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "cxx",
  "cxx-build",
  "dora-node-api",
  "dora-ros2-bridge",
  "dora-ros2-bridge-msg-gen",
  "eyre",
@@ -2439,15 +2439,15 @@
  "rust-format",
  "serde",
  "serde-big-array",
 ]
 
 [[package]]
 name = "dora-node-api-python"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "arrow",
  "dora-node-api",
  "dora-operator-api-python",
  "dora-ros2-bridge-python",
  "dora-runtime",
  "eyre",
@@ -2456,84 +2456,84 @@
  "pyo3",
  "pythonize",
  "serde_yaml 0.8.26",
 ]
 
 [[package]]
 name = "dora-operator-api"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-arrow-convert",
  "dora-operator-api-macros",
  "dora-operator-api-types",
 ]
 
 [[package]]
 name = "dora-operator-api-c"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-operator-api-types",
 ]
 
 [[package]]
 name = "dora-operator-api-cxx"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "cxx",
  "cxx-build",
  "dora-operator-api",
 ]
 
 [[package]]
 name = "dora-operator-api-macros"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "dora-operator-api-python"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "aligned-vec",
  "arrow",
  "arrow-schema",
  "dora-node-api",
  "eyre",
  "flume 0.10.14",
  "pyo3",
  "serde_yaml 0.8.26",
 ]
 
 [[package]]
 name = "dora-operator-api-types"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "arrow",
  "dora-arrow-convert",
  "safer-ffi",
 ]
 
 [[package]]
 name = "dora-record"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "chrono",
  "dora-node-api",
  "dora-tracing",
  "eyre",
  "parquet",
  "tokio",
 ]
 
 [[package]]
 name = "dora-rerun"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-node-api",
  "eyre",
  "ndarray",
  "rerun",
  "tokio",
 ]
@@ -2589,15 +2589,15 @@
  "pyo3",
  "serde",
  "serde_assert",
 ]
 
 [[package]]
 name = "dora-runtime"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "aligned-vec",
  "arrow",
  "dora-core",
  "dora-download",
  "dora-metrics",
  "dora-node-api",
@@ -2616,15 +2616,15 @@
  "tokio-stream",
  "tracing",
  "tracing-opentelemetry",
 ]
 
 [[package]]
 name = "dora-tracing"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "eyre",
  "opentelemetry 0.18.0",
  "opentelemetry-jaeger",
  "tracing",
  "tracing-opentelemetry",
  "tracing-subscriber",
@@ -4822,33 +4822,33 @@
  "net2",
  "winapi 0.2.8",
  "ws2_32-sys",
 ]
 
 [[package]]
 name = "multiple-daemons-example-node"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
 ]
 
 [[package]]
 name = "multiple-daemons-example-operator"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-operator-api",
 ]
 
 [[package]]
 name = "multiple-daemons-example-sink"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-node-api",
  "eyre",
 ]
 
 [[package]]
 name = "naga"
@@ -7863,34 +7863,34 @@
  "smallvec",
  "subtle",
  "zeroize",
 ]
 
 [[package]]
 name = "rust-dataflow-example-node"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-node-api",
  "eyre",
  "futures",
  "rand",
  "tokio",
 ]
 
 [[package]]
 name = "rust-dataflow-example-sink"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-node-api",
  "eyre",
 ]
 
 [[package]]
 name = "rust-dataflow-example-status-node"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-node-api",
  "eyre",
 ]
 
 [[package]]
 name = "rust-format"
@@ -7901,15 +7901,15 @@
  "prettyplease 0.1.25",
  "proc-macro2",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "rust-ros2-dataflow-example-node"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "dora-node-api",
  "dora-ros2-bridge",
  "eyre",
  "futures",
  "futures-timer",
  "rand",
@@ -8383,15 +8383,15 @@
 checksum = "f40ca3c46823713e0d4209592e8d6e826aa57e928f09752619fc696c499637f6"
 dependencies = [
  "lazy_static",
 ]
 
 [[package]]
 name = "shared-memory-server"
-version = "0.3.4"
+version = "0.3.4-rc2"
 dependencies = [
  "bincode",
  "eyre",
  "raw_sync_2",
  "serde",
  "shared_memory_extended",
  "tracing",
```

### Comparing `dora_rs-0.3.4/Cargo.toml` & `dora_rs-0.3.4rc2/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [workspace]
 members = ["apis/python/node", "apis/rust/*", "libraries/extensions/telemetry/*"]
 
 [workspace.package]
 # Make sure to also bump `apis/node/python/__init__.py` version.
-version = "0.3.4"
+version = "0.3.4-rc2"
 description = "`dora` goal is to be a low latency, composable, and distributed data flow."
 documentation = "https://dora.carsmos.ai"
 license = "Apache-2.0"
 
 [workspace.dependencies]
-dora-node-api = { version = "0.3.4", path = "apis/rust/node", default-features = false }
-dora-node-api-python = { version = "0.3.4", path = "apis/python/node", default-features = false }
-dora-operator-api = { version = "0.3.4", path = "apis/rust/operator", default-features = false }
-dora-operator-api-macros = { version = "0.3.4", path = "apis/rust/operator/macros" }
-dora-operator-api-types = { version = "0.3.4", path = "apis/rust/operator/types" }
-dora-operator-api-python = { version = "0.3.4", path = "apis/python/operator" }
-dora-operator-api-c = { version = "0.3.4", path = "apis/c/operator" }
-dora-node-api-c = { version = "0.3.4", path = "apis/c/node" }
-dora-core = { version = "0.3.4", path = "libraries/core" }
-dora-arrow-convert = { version = "0.3.4", path = "libraries/arrow-convert" }
-dora-tracing = { version = "0.3.4", path = "libraries/extensions/telemetry/tracing" }
-dora-metrics = { version = "0.3.4", path = "libraries/extensions/telemetry/metrics" }
-dora-download = { version = "0.3.4", path = "libraries/extensions/download" }
-shared-memory-server = { version = "0.3.4", path = "libraries/shared-memory-server" }
-communication-layer-request-reply = { version = "0.3.4", path = "libraries/communication-layer/request-reply" }
-dora-message = { version = "0.3.4", path = "libraries/message" }
-dora-runtime = { version = "0.3.4", path = "binaries/runtime" }
-dora-daemon = { version = "0.3.4", path = "binaries/daemon" }
-dora-coordinator = { version = "0.3.4", path = "binaries/coordinator" }
+dora-node-api = { version = "0.3.4-rc2", path = "apis/rust/node", default-features = false }
+dora-node-api-python = { version = "0.3.4-rc2", path = "apis/python/node", default-features = false }
+dora-operator-api = { version = "0.3.4-rc2", path = "apis/rust/operator", default-features = false }
+dora-operator-api-macros = { version = "0.3.4-rc2", path = "apis/rust/operator/macros" }
+dora-operator-api-types = { version = "0.3.4-rc2", path = "apis/rust/operator/types" }
+dora-operator-api-python = { version = "0.3.4-rc2", path = "apis/python/operator" }
+dora-operator-api-c = { version = "0.3.4-rc2", path = "apis/c/operator" }
+dora-node-api-c = { version = "0.3.4-rc2", path = "apis/c/node" }
+dora-core = { version = "0.3.4-rc2", path = "libraries/core" }
+dora-arrow-convert = { version = "0.3.4-rc2", path = "libraries/arrow-convert" }
+dora-tracing = { version = "0.3.4-rc2", path = "libraries/extensions/telemetry/tracing" }
+dora-metrics = { version = "0.3.4-rc2", path = "libraries/extensions/telemetry/metrics" }
+dora-download = { version = "0.3.4-rc2", path = "libraries/extensions/download" }
+shared-memory-server = { version = "0.3.4-rc2", path = "libraries/shared-memory-server" }
+communication-layer-request-reply = { version = "0.3.4-rc2", path = "libraries/communication-layer/request-reply" }
+dora-message = { version = "0.3.4-rc2", path = "libraries/message" }
+dora-runtime = { version = "0.3.4-rc2", path = "binaries/runtime" }
+dora-daemon = { version = "0.3.4-rc2", path = "binaries/daemon" }
+dora-coordinator = { version = "0.3.4-rc2", path = "binaries/coordinator" }
 dora-ros2-bridge = { path = "libraries/extensions/ros2-bridge" }
 dora-ros2-bridge-msg-gen = { path = "libraries/extensions/ros2-bridge/msg-gen" }
 dora-ros2-bridge-python = { path = "libraries/extensions/ros2-bridge/python" }
 arrow = "48.0.0"
 arrow-schema = "48.0.0"
 arrow-data = "48.0.0"
 arrow-array = "48.0.0"
```

### Comparing `dora_rs-0.3.4/dora/__init__.py` & `dora_rs-0.3.4rc2/dora/__init__.py`

 * *Files identical despite different names*

### Comparing `dora_rs-0.3.4/dora/__init__.pyi` & `dora_rs-0.3.4rc2/dora/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -35,17 +35,14 @@
 ```"""
 
     def dataflow_descriptor(self) -> dict:
         """Returns the full dataflow descriptor that this node is part of.
 
 This method returns the parsed dataflow YAML file."""
 
-    def dataflow_id(self) -> str:
-        """Returns the dataflow id."""
-
     def merge_external_events(self, subscription: dora.Ros2Subscription) -> None:
         """Merge an external event stream with dora main loop.
 This currently only work with ROS2."""
 
     def next(self, timeout: float=None) -> dora.PyEvent:
         """`.next()` gives you the next input that the node has received.
 It blocks until the next event becomes available.
```

### Comparing `dora_rs-0.3.4/PKG-INFO` & `dora_rs-0.3.4rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dora-rs
-Version: 0.3.4
+Version: 0.3.4rc2
 Requires-Dist: pyarrow
 Summary: `dora` goal is to be a low latency, composable, and distributed data flow.
 License: Apache-2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 This crate corresponds to the Node API for Dora.
```

