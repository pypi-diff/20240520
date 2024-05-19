# Comparing `tmp/toc_trade_pb_v2-0.1.7.tar.gz` & `tmp/toc_trade_pb_v2-0.1.8.tar.gz`

## Comparing `toc_trade_pb_v2-0.1.7.tar` & `toc_trade_pb_v2-0.1.8.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/CHANGELOG.md
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/CONTRIBUTING.md
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/Makefile
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/go.mod
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/go.sum
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/package-lock.json
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/package.json
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/pubspec.lock
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/pubspec.yaml
--rwxr-xr-x   0        0        0      504 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/.chglog/CHANGELOG.tpl.md
--rwxr-xr-x   0        0        0      528 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/.chglog/config.yml
--rw-r--r--   0        0        0    16456 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/app/app.pb.dart
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/app/app.pbenum.dart
--rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/app/app.pbjson.dart
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/app/app.pbserver.dart
--rw-r--r--   0        0        0    33911 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/basic.pb.dart
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/basic.pbenum.dart
--rw-r--r--   0        0        0    10360 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/basic.pbjson.dart
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/basic.pbserver.dart
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/entity.pb.dart
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/entity.pbenum.dart
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/entity.pbjson.dart
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/entity.pbserver.dart
--rw-r--r--   0        0        0    30778 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/history.pb.dart
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/history.pbenum.dart
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/history.pbjson.dart
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/history.pbserver.dart
--rw-r--r--   0        0        0    46124 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/mq.pb.dart
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/mq.pbenum.dart
--rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/mq.pbjson.dart
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/mq.pbserver.dart
--rw-r--r--   0        0        0    36869 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/realtime.pb.dart
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/realtime.pbenum.dart
--rw-r--r--   0        0        0    11581 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/realtime.pbjson.dart
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/realtime.pbserver.dart
--rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/subscribe.pb.dart
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/subscribe.pbenum.dart
--rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/subscribe.pbjson.dart
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/subscribe.pbserver.dart
--rw-r--r--   0        0        0    69695 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/trade.pb.dart
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/trade.pbenum.dart
--rw-r--r--   0        0        0    20594 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/trade.pbjson.dart
--rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/forwarder/trade.pbserver.dart
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/google/protobuf/empty.pb.dart
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/google/protobuf/empty.pbenum.dart
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/google/protobuf/empty.pbjson.dart
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/lib/google/protobuf/empty.pbserver.dart
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/protos/v3/app/app.proto
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/protos/v3/forwarder/basic.proto
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/protos/v3/forwarder/entity.proto
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/protos/v3/forwarder/history.proto
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/protos/v3/forwarder/mq.proto
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/protos/v3/forwarder/realtime.proto
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/protos/v3/forwarder/subscribe.proto
--rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/protos/v3/forwarder/trade.proto
--rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/scripts/gomod_update.sh
--rwxr-xr-x   0        0        0      257 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/scripts/modify_py_import.sh
--rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/scripts/update_dependency.sh
--rw-r--r--   0        0        0    20644 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/app.pb.go
--rw-r--r--   0        0        0    35785 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/basic.pb.go
--rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/basic_grpc.pb.go
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/entity.pb.go
--rw-r--r--   0        0        0    31727 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/history.pb.go
--rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/history_grpc.pb.go
--rw-r--r--   0        0        0    48055 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/mq.pb.go
--rw-r--r--   0        0        0    39615 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/realtime.pb.go
--rw-r--r--   0        0        0    16341 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/realtime_grpc.pb.go
--rw-r--r--   0        0        0    12403 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/subscribe.pb.go
--rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/subscribe_grpc.pb.go
--rw-r--r--   0        0        0    73958 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/trade.pb.go
--rw-r--r--   0        0        0    31982 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/golang/pb/trade_grpc.pb.go
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/app/__init__.py
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/app/app_pb2.py
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/app/app_pb2.pyi
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/app/app_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/__init__.py
--rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/basic_pb2.py
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/basic_pb2.pyi
--rw-r--r--   0        0        0    12888 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/basic_pb2_grpc.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/entity_pb2.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/entity_pb2.pyi
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/entity_pb2_grpc.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/history_pb2.py
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/history_pb2.pyi
--rw-r--r--   0        0        0     9478 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/history_pb2_grpc.py
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/mq_pb2.py
--rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/mq_pb2.pyi
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/mq_pb2_grpc.py
--rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/realtime_pb2.py
--rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/realtime_pb2.pyi
--rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/subscribe_pb2.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/subscribe_pb2.pyi
--rw-r--r--   0        0        0    20666 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py
--rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/trade_pb2.py
--rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/trade_pb2.pyi
--rw-r--r--   0        0        0    35687 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/trade_pb2_grpc.py
--rw-r--r--   0        0        0    22978 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/ts/app/app.ts
--rw-r--r--   0        0        0    46501 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/ts/forwarder/basic.ts
--rw-r--r--   0        0        0     7734 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/ts/forwarder/entity.ts
--rw-r--r--   0        0        0    38023 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/ts/forwarder/history.ts
--rw-r--r--   0        0        0    75768 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/ts/forwarder/mq.ts
--rw-r--r--   0        0        0    52979 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/ts/forwarder/realtime.ts
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/ts/forwarder/subscribe.ts
--rw-r--r--   0        0        0    91499 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/ts/forwarder/trade.ts
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/src/ts/google/protobuf/empty.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/tests/.gitkeep
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/LICENSE
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/README.md
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/CHANGELOG.md
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/Makefile
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go.mod
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go.sum
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/package-lock.json
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/package.json
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/pubspec.lock
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/pubspec.yaml
+-rwxr-xr-x   0        0        0      504 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0        0        0      528 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/.chglog/config.yml
+-rw-r--r--   0        0        0    20644 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/app.pb.go
+-rw-r--r--   0        0        0    35785 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/basic.pb.go
+-rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/basic_grpc.pb.go
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/entity.pb.go
+-rw-r--r--   0        0        0    31727 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/history.pb.go
+-rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/history_grpc.pb.go
+-rw-r--r--   0        0        0    48055 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/mq.pb.go
+-rw-r--r--   0        0        0    39615 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/realtime.pb.go
+-rw-r--r--   0        0        0    16341 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/realtime_grpc.pb.go
+-rw-r--r--   0        0        0    12403 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/subscribe.pb.go
+-rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/subscribe_grpc.pb.go
+-rw-r--r--   0        0        0    73958 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/trade.pb.go
+-rw-r--r--   0        0        0    31982 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/trade_grpc.pb.go
+-rw-r--r--   0        0        0    16456 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/app/app.pb.dart
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/app/app.pbenum.dart
+-rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/app/app.pbjson.dart
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/app/app.pbserver.dart
+-rw-r--r--   0        0        0    33911 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/basic.pb.dart
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/basic.pbenum.dart
+-rw-r--r--   0        0        0    10360 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/basic.pbjson.dart
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/basic.pbserver.dart
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/entity.pb.dart
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/entity.pbenum.dart
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/entity.pbjson.dart
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/entity.pbserver.dart
+-rw-r--r--   0        0        0    30778 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/history.pb.dart
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/history.pbenum.dart
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/history.pbjson.dart
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/history.pbserver.dart
+-rw-r--r--   0        0        0    46124 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/mq.pb.dart
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/mq.pbenum.dart
+-rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/mq.pbjson.dart
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/mq.pbserver.dart
+-rw-r--r--   0        0        0    36869 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/realtime.pb.dart
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/realtime.pbenum.dart
+-rw-r--r--   0        0        0    11581 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/realtime.pbjson.dart
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/realtime.pbserver.dart
+-rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/subscribe.pb.dart
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/subscribe.pbenum.dart
+-rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/subscribe.pbjson.dart
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/subscribe.pbserver.dart
+-rw-r--r--   0        0        0    69695 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/trade.pb.dart
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/trade.pbenum.dart
+-rw-r--r--   0        0        0    20594 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/trade.pbjson.dart
+-rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/trade.pbserver.dart
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/google/protobuf/empty.pb.dart
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/google/protobuf/empty.pbenum.dart
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/google/protobuf/empty.pbjson.dart
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/google/protobuf/empty.pbserver.dart
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/protos/v3/app/app.proto
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/protos/v3/forwarder/basic.proto
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/protos/v3/forwarder/entity.proto
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/protos/v3/forwarder/history.proto
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/protos/v3/forwarder/mq.proto
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/protos/v3/forwarder/realtime.proto
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/protos/v3/forwarder/subscribe.proto
+-rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/protos/v3/forwarder/trade.proto
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/app/__init__.py
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/app/app_pb2.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/app/app_pb2.pyi
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/app/app_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/__init__.py
+-rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/basic_pb2.py
+-rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/basic_pb2.pyi
+-rw-r--r--   0        0        0    12888 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/basic_pb2_grpc.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/entity_pb2.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/entity_pb2.pyi
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/history_pb2.py
+-rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/history_pb2.pyi
+-rw-r--r--   0        0        0     9478 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/history_pb2_grpc.py
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/mq_pb2.py
+-rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/mq_pb2.pyi
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/mq_pb2_grpc.py
+-rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/realtime_pb2.py
+-rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/realtime_pb2.pyi
+-rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/realtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/subscribe_pb2.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/subscribe_pb2.pyi
+-rw-r--r--   0        0        0    20666 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/subscribe_pb2_grpc.py
+-rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/trade_pb2.py
+-rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/trade_pb2.pyi
+-rw-r--r--   0        0        0    35687 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/trade_pb2_grpc.py
+-rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/scripts/gomod_update.sh
+-rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/scripts/modify_py_import.sh
+-rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/scripts/update_dependency.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/tests/.gitkeep
+-rw-r--r--   0        0        0    22978 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/ts/app/app.ts
+-rw-r--r--   0        0        0    46501 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/ts/forwarder/basic.ts
+-rw-r--r--   0        0        0     7734 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/ts/forwarder/entity.ts
+-rw-r--r--   0        0        0    38023 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/ts/forwarder/history.ts
+-rw-r--r--   0        0        0    75768 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/ts/forwarder/mq.ts
+-rw-r--r--   0        0        0    52979 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/ts/forwarder/realtime.ts
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/ts/forwarder/subscribe.ts
+-rw-r--r--   0        0        0    91499 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/ts/forwarder/trade.ts
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/ts/google/protobuf/empty.ts
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/LICENSE
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/README.md
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/PKG-INFO
```

### Comparing `toc_trade_pb_v2-0.1.7/CHANGELOG.md` & `toc_trade_pb_v2-0.1.8/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/CONTRIBUTING.md` & `toc_trade_pb_v2-0.1.8/CONTRIBUTING.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ```sh
 brew tap git-chglog/git-chglog
 brew install git-chglog
 ```
 
 ```sh
 COMMIT_HASH=053ff921b22726015638934803fa228113f58bf1
-VERSION=0.1.7
+VERSION=0.1.8
 git tag -a v$VERSION $COMMIT_HASH -m $VERSION
 git push -u origin --all
 git push -u origin --tags
 ```
 
 ### Find ignored files
```

### Comparing `toc_trade_pb_v2-0.1.7/Makefile` & `toc_trade_pb_v2-0.1.8/Makefile`

 * *Files 13% similar despite different names*

```diff
@@ -2,51 +2,51 @@
 PIP=$(shell which pip3)
 PROTOC_PATH=$(shell which protoc)
 PROTOC_INCLUDE_PATH=$(shell dirname $(shell dirname "$(PROTOC_PATH)"))
 
 compile: compile-go compile-py compile-ts compile-dart
 
 compile-go:
-	@rm -rf src/golang && mkdir -p src/golang
+	@rm -rf go && mkdir -p go
 	@$(PROTOC_PATH) \
-	--go_out=src/golang \
-	--go-grpc_out=src/golang \
+	--go_out=go \
+	--go-grpc_out=go \
 	--proto_path=protos/v3 \
 	./protos/v3/*/*.proto
 	@. ./scripts/gomod_update.sh
 
 compile-dart:
 	@rm -rf lib && mkdir -p lib
 	@dart pub global activate --overwrite protoc_plugin
 	@$(PROTOC_PATH) \
 	--dart_out=lib \
 	--proto_path=protos/v3 \
 	./protos/v3/*/*.proto \
 	$(PROTOC_INCLUDE_PATH)/include/google/protobuf/empty.proto
 
 compile-py: check
-	@rm -rf src/python/toc_trade_pb && mkdir -p src/python/toc_trade_pb
+	@rm -rf py/toc_trade_pb && mkdir -p py/toc_trade_pb
 	@$(PYTHON) -m grpc_tools.protoc \
-	--grpc_python_out=src/python/toc_trade_pb \
-	--python_out=pyi_out:src/python/toc_trade_pb \
+	--grpc_python_out=py/toc_trade_pb \
+	--python_out=pyi_out:py/toc_trade_pb \
 	--proto_path=protos/v3 \
 	./protos/v3/*/*.proto
 
 	@./scripts/modify_py_import.sh
-	@touch src/python/toc_trade_pb/__init__.py
-	@touch src/python/toc_trade_pb/app/__init__.py
-	@touch src/python/toc_trade_pb/forwarder/__init__.py
+	@touch py/toc_trade_pb/__init__.py
+	@touch py/toc_trade_pb/app/__init__.py
+	@touch py/toc_trade_pb/forwarder/__init__.py
 
 compile-ts:
-	@rm -rf src/ts && mkdir -p src/ts
+	@rm -rf ts && mkdir -p ts
 	@$(PROTOC_PATH) \
 	--proto_path=protos/v3 \
     --ts_opt=no_grpc \
     --ts_opt=no_namespace \
-    --ts_out=src/ts \
+    --ts_out=ts \
 	./protos/v3/*/*.proto
 
 build-py: check
 	@rm -rf dist
 	@$(PYTHON) -m build
 
 upload-py: check build-py
```

### Comparing `toc_trade_pb_v2-0.1.7/go.sum` & `toc_trade_pb_v2-0.1.8/go.sum`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/package-lock.json` & `toc_trade_pb_v2-0.1.8/package-lock.json`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/package.json` & `toc_trade_pb_v2-0.1.8/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.1.8'"}*

```diff
@@ -14,9 +14,9 @@
     ],
     "license": "MIT",
     "name": "@chindada/toc-trade-protobuf",
     "repository": {
         "type": "git",
         "url": "git+https://github.com/ToC-Taiwan/toc-trade-protobuf.git"
     },
-    "version": "0.1.7"
+    "version": "0.1.8"
 }
```

### Comparing `toc_trade_pb_v2-0.1.7/pubspec.lock` & `toc_trade_pb_v2-0.1.8/pubspec.lock`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/.chglog/config.yml` & `toc_trade_pb_v2-0.1.8/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/app/app.pb.dart` & `toc_trade_pb_v2-0.1.8/lib/app/app.pb.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/app/app.pbenum.dart` & `toc_trade_pb_v2-0.1.8/lib/app/app.pbenum.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/app/app.pbjson.dart` & `toc_trade_pb_v2-0.1.8/lib/app/app.pbjson.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/basic.pb.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/basic.pb.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/basic.pbjson.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/basic.pbjson.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/basic.pbserver.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/basic.pbserver.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/entity.pb.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/entity.pb.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/entity.pbjson.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/entity.pbjson.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/history.pb.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/history.pb.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/history.pbjson.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/history.pbjson.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/history.pbserver.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/history.pbserver.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/mq.pb.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/mq.pb.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/mq.pbenum.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/mq.pbenum.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/mq.pbjson.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/mq.pbjson.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/realtime.pb.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/realtime.pb.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/realtime.pbjson.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/realtime.pbjson.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/realtime.pbserver.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/realtime.pbserver.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/subscribe.pb.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/subscribe.pb.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/subscribe.pbjson.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/subscribe.pbjson.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/subscribe.pbserver.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/subscribe.pbserver.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/trade.pb.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/trade.pb.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/trade.pbjson.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/trade.pbjson.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/forwarder/trade.pbserver.dart` & `toc_trade_pb_v2-0.1.8/lib/forwarder/trade.pbserver.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/google/protobuf/empty.pb.dart` & `toc_trade_pb_v2-0.1.8/lib/google/protobuf/empty.pb.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/lib/google/protobuf/empty.pbjson.dart` & `toc_trade_pb_v2-0.1.8/lib/google/protobuf/empty.pbjson.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/protos/v3/app/app.proto` & `toc_trade_pb_v2-0.1.8/protos/v3/app/app.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/protos/v3/forwarder/basic.proto` & `toc_trade_pb_v2-0.1.8/protos/v3/forwarder/basic.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/protos/v3/forwarder/history.proto` & `toc_trade_pb_v2-0.1.8/protos/v3/forwarder/history.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/protos/v3/forwarder/mq.proto` & `toc_trade_pb_v2-0.1.8/protos/v3/forwarder/mq.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/protos/v3/forwarder/realtime.proto` & `toc_trade_pb_v2-0.1.8/protos/v3/forwarder/realtime.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/protos/v3/forwarder/subscribe.proto` & `toc_trade_pb_v2-0.1.8/protos/v3/forwarder/subscribe.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/protos/v3/forwarder/trade.proto` & `toc_trade_pb_v2-0.1.8/protos/v3/forwarder/trade.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/golang/pb/app.pb.go` & `toc_trade_pb_v2-0.1.8/go/pb/app.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/golang/pb/basic.pb.go` & `toc_trade_pb_v2-0.1.8/go/pb/basic.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/golang/pb/basic_grpc.pb.go` & `toc_trade_pb_v2-0.1.8/go/pb/basic_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/golang/pb/entity.pb.go` & `toc_trade_pb_v2-0.1.8/go/pb/entity.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/golang/pb/history.pb.go` & `toc_trade_pb_v2-0.1.8/go/pb/history.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/golang/pb/history_grpc.pb.go` & `toc_trade_pb_v2-0.1.8/go/pb/history_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/golang/pb/mq.pb.go` & `toc_trade_pb_v2-0.1.8/go/pb/mq.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/golang/pb/realtime.pb.go` & `toc_trade_pb_v2-0.1.8/go/pb/realtime.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/golang/pb/realtime_grpc.pb.go` & `toc_trade_pb_v2-0.1.8/go/pb/realtime_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/golang/pb/subscribe.pb.go` & `toc_trade_pb_v2-0.1.8/go/pb/subscribe.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/golang/pb/subscribe_grpc.pb.go` & `toc_trade_pb_v2-0.1.8/go/pb/subscribe_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/golang/pb/trade.pb.go` & `toc_trade_pb_v2-0.1.8/go/pb/trade.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/golang/pb/trade_grpc.pb.go` & `toc_trade_pb_v2-0.1.8/go/pb/trade_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/app/app_pb2.py` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/app/app_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/app/app_pb2.pyi` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/app/app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/app/app_pb2_grpc.py` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/app/app_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/basic_pb2.py` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/basic_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/basic_pb2.pyi` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/basic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/basic_pb2_grpc.py` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/basic_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/entity_pb2.py` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/entity_pb2.pyi` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/entity_pb2_grpc.py` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/entity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/history_pb2.py` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/history_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/history_pb2.pyi` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/history_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/history_pb2_grpc.py` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/history_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/mq_pb2.py` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/mq_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/mq_pb2.pyi` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/mq_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/mq_pb2_grpc.py` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/mq_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/realtime_pb2.py` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/realtime_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/realtime_pb2.pyi` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/realtime_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/realtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/subscribe_pb2.py` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/subscribe_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/subscribe_pb2.pyi` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/subscribe_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/subscribe_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/trade_pb2.py` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/trade_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/trade_pb2.pyi` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/trade_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/python/toc_trade_pb/forwarder/trade_pb2_grpc.py` & `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/trade_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/ts/app/app.ts` & `toc_trade_pb_v2-0.1.8/ts/app/app.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/ts/forwarder/basic.ts` & `toc_trade_pb_v2-0.1.8/ts/forwarder/basic.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/ts/forwarder/entity.ts` & `toc_trade_pb_v2-0.1.8/ts/forwarder/entity.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/ts/forwarder/history.ts` & `toc_trade_pb_v2-0.1.8/ts/forwarder/history.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/ts/forwarder/mq.ts` & `toc_trade_pb_v2-0.1.8/ts/forwarder/mq.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/ts/forwarder/realtime.ts` & `toc_trade_pb_v2-0.1.8/ts/forwarder/realtime.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/ts/forwarder/subscribe.ts` & `toc_trade_pb_v2-0.1.8/ts/forwarder/subscribe.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/ts/forwarder/trade.ts` & `toc_trade_pb_v2-0.1.8/ts/forwarder/trade.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/src/ts/google/protobuf/empty.ts` & `toc_trade_pb_v2-0.1.8/ts/google/protobuf/empty.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/LICENSE` & `toc_trade_pb_v2-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.7/pyproject.toml` & `toc_trade_pb_v2-0.1.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "toc-trade-pb-v2"
-version = "0.1.7"
+version = "0.1.8"
 authors = [{ name = "Tim Hsu", email = "maochindada@gmail.com" }]
 description = "Pre-compiled Python protobuf files for ToC Trade"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.hatch.build.targets.wheel]
-packages = [
-    "src/python/toc_trade_pb",
-    "src/python/toc_trade_pb/app",
-    "src/python/toc_trade_pb/forwarder",
-]
+packages = ["py/toc_trade_pb"]
 
 [project.urls]
 Homepage = "https://github.com/ToC-Taiwan/toc-trade-protobuf"
 Issues = "https://github.com/ToC-Taiwan/toc-trade-protobuf/issues"
```

### Comparing `toc_trade_pb_v2-0.1.7/PKG-INFO` & `toc_trade_pb_v2-0.1.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: toc-trade-pb-v2
-Version: 0.1.7
+Version: 0.1.8
 Summary: Pre-compiled Python protobuf files for ToC Trade
 Project-URL: Homepage, https://github.com/ToC-Taiwan/toc-trade-protobuf
 Project-URL: Issues, https://github.com/ToC-Taiwan/toc-trade-protobuf/issues
 Author-email: Tim Hsu <maochindada@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

