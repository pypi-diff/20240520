# Comparing `tmp/toc_trade_pb_v2-0.1.8.tar.gz` & `tmp/toc_trade_pb_v2-0.1.9.tar.gz`

## Comparing `toc_trade_pb_v2-0.1.8.tar` & `toc_trade_pb_v2-0.1.9.tar`

### file list

```diff
@@ -1,113 +1,113 @@
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/CHANGELOG.md
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/CONTRIBUTING.md
--rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/Makefile
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go.mod
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go.sum
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/package-lock.json
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/package.json
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/pubspec.lock
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/pubspec.yaml
--rwxr-xr-x   0        0        0      504 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/.chglog/CHANGELOG.tpl.md
--rwxr-xr-x   0        0        0      528 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/.chglog/config.yml
--rw-r--r--   0        0        0    20644 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/app.pb.go
--rw-r--r--   0        0        0    35785 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/basic.pb.go
--rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/basic_grpc.pb.go
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/entity.pb.go
--rw-r--r--   0        0        0    31727 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/history.pb.go
--rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/history_grpc.pb.go
--rw-r--r--   0        0        0    48055 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/mq.pb.go
--rw-r--r--   0        0        0    39615 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/realtime.pb.go
--rw-r--r--   0        0        0    16341 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/realtime_grpc.pb.go
--rw-r--r--   0        0        0    12403 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/subscribe.pb.go
--rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/subscribe_grpc.pb.go
--rw-r--r--   0        0        0    73958 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/trade.pb.go
--rw-r--r--   0        0        0    31982 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/go/pb/trade_grpc.pb.go
--rw-r--r--   0        0        0    16456 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/app/app.pb.dart
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/app/app.pbenum.dart
--rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/app/app.pbjson.dart
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/app/app.pbserver.dart
--rw-r--r--   0        0        0    33911 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/basic.pb.dart
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/basic.pbenum.dart
--rw-r--r--   0        0        0    10360 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/basic.pbjson.dart
--rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/basic.pbserver.dart
--rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/entity.pb.dart
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/entity.pbenum.dart
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/entity.pbjson.dart
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/entity.pbserver.dart
--rw-r--r--   0        0        0    30778 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/history.pb.dart
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/history.pbenum.dart
--rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/history.pbjson.dart
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/history.pbserver.dart
--rw-r--r--   0        0        0    46124 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/mq.pb.dart
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/mq.pbenum.dart
--rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/mq.pbjson.dart
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/mq.pbserver.dart
--rw-r--r--   0        0        0    36869 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/realtime.pb.dart
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/realtime.pbenum.dart
--rw-r--r--   0        0        0    11581 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/realtime.pbjson.dart
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/realtime.pbserver.dart
--rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/subscribe.pb.dart
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/subscribe.pbenum.dart
--rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/subscribe.pbjson.dart
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/subscribe.pbserver.dart
--rw-r--r--   0        0        0    69695 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/trade.pb.dart
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/trade.pbenum.dart
--rw-r--r--   0        0        0    20594 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/trade.pbjson.dart
--rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/forwarder/trade.pbserver.dart
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/google/protobuf/empty.pb.dart
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/google/protobuf/empty.pbenum.dart
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/google/protobuf/empty.pbjson.dart
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/lib/google/protobuf/empty.pbserver.dart
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/protos/v3/app/app.proto
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/protos/v3/forwarder/basic.proto
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/protos/v3/forwarder/entity.proto
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/protos/v3/forwarder/history.proto
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/protos/v3/forwarder/mq.proto
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/protos/v3/forwarder/realtime.proto
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/protos/v3/forwarder/subscribe.proto
--rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/protos/v3/forwarder/trade.proto
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/app/__init__.py
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/app/app_pb2.py
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/app/app_pb2.pyi
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/app/app_pb2_grpc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/__init__.py
--rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/basic_pb2.py
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/basic_pb2.pyi
--rw-r--r--   0        0        0    12888 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/basic_pb2_grpc.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/entity_pb2.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/entity_pb2.pyi
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/entity_pb2_grpc.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/history_pb2.py
--rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/history_pb2.pyi
--rw-r--r--   0        0        0     9478 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/history_pb2_grpc.py
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/mq_pb2.py
--rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/mq_pb2.pyi
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/mq_pb2_grpc.py
--rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/realtime_pb2.py
--rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/realtime_pb2.pyi
--rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/realtime_pb2_grpc.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/subscribe_pb2.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/subscribe_pb2.pyi
--rw-r--r--   0        0        0    20666 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/subscribe_pb2_grpc.py
--rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/trade_pb2.py
--rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/trade_pb2.pyi
--rw-r--r--   0        0        0    35687 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/trade_pb2_grpc.py
--rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/scripts/gomod_update.sh
--rwxr-xr-x   0        0        0      249 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/scripts/modify_py_import.sh
--rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/scripts/update_dependency.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/tests/.gitkeep
--rw-r--r--   0        0        0    22978 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/ts/app/app.ts
--rw-r--r--   0        0        0    46501 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/ts/forwarder/basic.ts
--rw-r--r--   0        0        0     7734 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/ts/forwarder/entity.ts
--rw-r--r--   0        0        0    38023 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/ts/forwarder/history.ts
--rw-r--r--   0        0        0    75768 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/ts/forwarder/mq.ts
--rw-r--r--   0        0        0    52979 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/ts/forwarder/realtime.ts
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/ts/forwarder/subscribe.ts
--rw-r--r--   0        0        0    91499 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/ts/forwarder/trade.ts
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/ts/google/protobuf/empty.ts
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/LICENSE
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/README.md
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/.markdownlint.yaml
+-rw-r--r--   0        0        0     2517 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/Makefile
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/go.mod
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/go.sum
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/package-lock.json
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/package.json
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/pubspec.lock
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/pubspec.yaml
+-rwxr-xr-x   0        0        0      504 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0        0        0      528 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/.chglog/config.yml
+-rw-r--r--   0        0        0    20644 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/golang/pb/app.pb.go
+-rw-r--r--   0        0        0    35785 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/golang/pb/basic.pb.go
+-rw-r--r--   0        0        0    13116 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/golang/pb/basic_grpc.pb.go
+-rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/golang/pb/entity.pb.go
+-rw-r--r--   0        0        0    31727 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/golang/pb/history.pb.go
+-rw-r--r--   0        0        0     9586 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/golang/pb/history_grpc.pb.go
+-rw-r--r--   0        0        0    48055 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/golang/pb/mq.pb.go
+-rw-r--r--   0        0        0    39615 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/golang/pb/realtime.pb.go
+-rw-r--r--   0        0        0    16341 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/golang/pb/realtime_grpc.pb.go
+-rw-r--r--   0        0        0    12403 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/golang/pb/subscribe.pb.go
+-rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/golang/pb/subscribe_grpc.pb.go
+-rw-r--r--   0        0        0    73958 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/golang/pb/trade.pb.go
+-rw-r--r--   0        0        0    31982 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/golang/pb/trade_grpc.pb.go
+-rw-r--r--   0        0        0    16456 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/app/app.pb.dart
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/app/app.pbenum.dart
+-rw-r--r--   0        0        0     4982 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/app/app.pbjson.dart
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/app/app.pbserver.dart
+-rw-r--r--   0        0        0    33911 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/basic.pb.dart
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/basic.pbenum.dart
+-rw-r--r--   0        0        0    10360 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/basic.pbjson.dart
+-rw-r--r--   0        0        0     2743 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/basic.pbserver.dart
+-rw-r--r--   0        0        0     7044 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/entity.pb.dart
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/entity.pbenum.dart
+-rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/entity.pbjson.dart
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/entity.pbserver.dart
+-rw-r--r--   0        0        0    30778 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/history.pb.dart
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/history.pbenum.dart
+-rw-r--r--   0        0        0     9075 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/history.pbjson.dart
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/history.pbserver.dart
+-rw-r--r--   0        0        0    46124 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/mq.pb.dart
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/mq.pbenum.dart
+-rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/mq.pbjson.dart
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/mq.pbserver.dart
+-rw-r--r--   0        0        0    36869 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/realtime.pb.dart
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/realtime.pbenum.dart
+-rw-r--r--   0        0        0    11581 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/realtime.pbjson.dart
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/realtime.pbserver.dart
+-rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/subscribe.pb.dart
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/subscribe.pbenum.dart
+-rw-r--r--   0        0        0     4132 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/subscribe.pbjson.dart
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/subscribe.pbserver.dart
+-rw-r--r--   0        0        0    69695 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/trade.pb.dart
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/trade.pbenum.dart
+-rw-r--r--   0        0        0    20594 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/trade.pbjson.dart
+-rw-r--r--   0        0        0     5909 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/forwarder/trade.pbserver.dart
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/google/protobuf/empty.pb.dart
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/google/protobuf/empty.pbenum.dart
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/google/protobuf/empty.pbjson.dart
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/lib/google/protobuf/empty.pbserver.dart
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/protos/v3/app/app.proto
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/protos/v3/forwarder/basic.proto
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/protos/v3/forwarder/entity.proto
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/protos/v3/forwarder/history.proto
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/protos/v3/forwarder/mq.proto
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/protos/v3/forwarder/realtime.proto
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/protos/v3/forwarder/subscribe.proto
+-rw-r--r--   0        0        0     7471 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/protos/v3/forwarder/trade.proto
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/app/__init__.py
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/app/app_pb2.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/app/app_pb2.pyi
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/app/app_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/__init__.py
+-rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/basic_pb2.py
+-rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/basic_pb2.pyi
+-rw-r--r--   0        0        0    12888 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/basic_pb2_grpc.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/entity_pb2.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/entity_pb2.pyi
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/history_pb2.py
+-rw-r--r--   0        0        0     4671 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/history_pb2.pyi
+-rw-r--r--   0        0        0     9478 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/history_pb2_grpc.py
+-rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/mq_pb2.py
+-rw-r--r--   0        0        0    11050 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/mq_pb2.pyi
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/mq_pb2_grpc.py
+-rw-r--r--   0        0        0     5324 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/realtime_pb2.py
+-rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/realtime_pb2.pyi
+-rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/subscribe_pb2.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/subscribe_pb2.pyi
+-rw-r--r--   0        0        0    20666 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py
+-rw-r--r--   0        0        0     8576 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/trade_pb2.py
+-rw-r--r--   0        0        0    11691 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/trade_pb2.pyi
+-rw-r--r--   0        0        0    35687 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/trade_pb2_grpc.py
+-rwxr-xr-x   0        0        0      250 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/scripts/gomod_update.sh
+-rwxr-xr-x   0        0        0      337 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/scripts/modify_py_import.sh
+-rwxr-xr-x   0        0        0      197 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/scripts/update_dependency.sh
+-rw-r--r--   0        0        0    22978 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/typescript/app/app.ts
+-rw-r--r--   0        0        0    46501 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/typescript/forwarder/basic.ts
+-rw-r--r--   0        0        0     7734 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/typescript/forwarder/entity.ts
+-rw-r--r--   0        0        0    38023 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/typescript/forwarder/history.ts
+-rw-r--r--   0        0        0    75768 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/typescript/forwarder/mq.ts
+-rw-r--r--   0        0        0    52979 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/typescript/forwarder/realtime.ts
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/typescript/forwarder/subscribe.ts
+-rw-r--r--   0        0        0    91499 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/typescript/forwarder/trade.ts
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/typescript/google/protobuf/empty.ts
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/LICENSE
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/README.md
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 toc_trade_pb_v2-0.1.9/PKG-INFO
```

### Comparing `toc_trade_pb_v2-0.1.8/CHANGELOG.md` & `toc_trade_pb_v2-0.1.9/CHANGELOG.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,25 @@
 # CHANGELOG
 
+## [v0.1.9](https://github.com/ToC-Taiwan/toc-machine-trading-fe/compare/v0.1.7...v0.1.9)
+
+> 2024-05-20
+
+### Code Refactoring (1)
+
+* split layout by language
+
+## [v0.1.7](https://github.com/ToC-Taiwan/toc-machine-trading-fe/compare/v0.1.4...v0.1.7)
+
+> 2024-05-19
+
+### Features (1)
+
+* add dart pre-compiled files
+
 ## [v0.1.4](https://github.com/ToC-Taiwan/toc-machine-trading-fe/compare/v0.1.0...v0.1.4)
 
 > 2024-05-18
 
 ### Features (1)
 
 * add ts, modify python generated import
```

### Comparing `toc_trade_pb_v2-0.1.8/CONTRIBUTING.md` & `toc_trade_pb_v2-0.1.9/CONTRIBUTING.md`

 * *Files 17% similar despite different names*

```diff
@@ -35,17 +35,21 @@
 
 ```sh
 brew tap git-chglog/git-chglog
 brew install git-chglog
 ```
 
 ```sh
-COMMIT_HASH=053ff921b22726015638934803fa228113f58bf1
-VERSION=0.1.8
+COMMIT_HASH=06b7f9b9def32e770d980ac3ba2e5177333441c9
+VERSION=0.1.9
 git tag -a v$VERSION $COMMIT_HASH -m $VERSION
+git-chglog -o CHANGELOG.md
+```
+
+```sh
 git push -u origin --all
 git push -u origin --tags
 ```
 
 ### Find ignored files
 
 ```sh
```

### Comparing `toc_trade_pb_v2-0.1.8/Makefile` & `toc_trade_pb_v2-0.1.9/Makefile`

 * *Files 24% similar despite different names*

```diff
@@ -2,72 +2,69 @@
 PIP=$(shell which pip3)
 PROTOC_PATH=$(shell which protoc)
 PROTOC_INCLUDE_PATH=$(shell dirname $(shell dirname "$(PROTOC_PATH)"))
 
 compile: compile-go compile-py compile-ts compile-dart
 
 compile-go:
-	@rm -rf go && mkdir -p go
+	@rm -rf golang && mkdir -p golang
 	@$(PROTOC_PATH) \
-	--go_out=go \
-	--go-grpc_out=go \
+	--go_out=golang \
+	--go-grpc_out=golang \
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
-	@rm -rf py/toc_trade_pb && mkdir -p py/toc_trade_pb
+	@rm -rf python/toc_trade_pb && mkdir -p python/toc_trade_pb
 	@$(PYTHON) -m grpc_tools.protoc \
-	--grpc_python_out=py/toc_trade_pb \
-	--python_out=pyi_out:py/toc_trade_pb \
+	--grpc_python_out=python/toc_trade_pb \
+	--python_out=pyi_out:python/toc_trade_pb \
 	--proto_path=protos/v3 \
 	./protos/v3/*/*.proto
 
-	@./scripts/modify_py_import.sh
-	@touch py/toc_trade_pb/__init__.py
-	@touch py/toc_trade_pb/app/__init__.py
-	@touch py/toc_trade_pb/forwarder/__init__.py
+	@./scripts/modify_py_import.sh python/toc_trade_pb
+	@touch python/toc_trade_pb/__init__.py
+	@touch python/toc_trade_pb/app/__init__.py
+	@touch python/toc_trade_pb/forwarder/__init__.py
 
 compile-ts:
-	@rm -rf ts && mkdir -p ts
+	@rm -rf typescript && mkdir -p typescript
 	@$(PROTOC_PATH) \
 	--proto_path=protos/v3 \
     --ts_opt=no_grpc \
     --ts_opt=no_namespace \
-    --ts_out=ts \
+    --ts_out=typescript \
 	./protos/v3/*/*.proto
 
 build-py: check
 	@rm -rf dist
 	@$(PYTHON) -m build
 
 upload-py: check build-py
 ifeq ($(PYPI_TOKEN),)
 	$(error "PYPI_TOKEN first")
 endif
 	@$(PYTHON) -m twine upload --repository pypi -p $(PYPI_TOKEN) dist/*
 
-clean: ## clear virtual environment
+clean:
 	@rm -rf venv
 
-venv: clean ## create virtual environment
+venv: clean
 	@$(PYTHON) -m venv venv
 
 check: ## check environment
 ifneq ($(PYTHON),$(PWD)/venv/bin/python3)
 	$(error "Please run 'make venv' first")
 endif
 	@echo "Venv python version: $(shell $(PYTHON) --version | awk '{print $$2}')"
 	@echo "Python path: $(PYTHON)"
 	@$(PIP) install -U --no-warn-script-location --no-cache-dir grpcio-tools protobuf build twine
-
-help: ## display this help screen
-	@awk 'BEGIN {FS = ":.*##"; printf "\nUsage:\n  make \033[36m<target>\033[0m\n"} /^[a-zA-Z_-]+:.*?##/ { printf "  \033[36m%-30s\033[0m %s\n", $$1, $$2 } /^##@/ { printf "\n\033[1m%s\033[0m\n", substr($$0, 5) } ' $(MAKEFILE_LIST)
```

### Comparing `toc_trade_pb_v2-0.1.8/go.sum` & `toc_trade_pb_v2-0.1.9/go.sum`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/package-lock.json` & `toc_trade_pb_v2-0.1.9/package-lock.json`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/package.json` & `toc_trade_pb_v2-0.1.9/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'version'": "'0.1.9'"}*

```diff
@@ -14,9 +14,9 @@
     ],
     "license": "MIT",
     "name": "@chindada/toc-trade-protobuf",
     "repository": {
         "type": "git",
         "url": "git+https://github.com/ToC-Taiwan/toc-trade-protobuf.git"
     },
-    "version": "0.1.8"
+    "version": "0.1.9"
 }
```

### Comparing `toc_trade_pb_v2-0.1.8/pubspec.lock` & `toc_trade_pb_v2-0.1.9/pubspec.lock`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/.chglog/config.yml` & `toc_trade_pb_v2-0.1.9/.chglog/config.yml`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/go/pb/app.pb.go` & `toc_trade_pb_v2-0.1.9/golang/pb/app.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/go/pb/basic.pb.go` & `toc_trade_pb_v2-0.1.9/golang/pb/basic.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/go/pb/basic_grpc.pb.go` & `toc_trade_pb_v2-0.1.9/golang/pb/basic_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/go/pb/entity.pb.go` & `toc_trade_pb_v2-0.1.9/golang/pb/entity.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/go/pb/history.pb.go` & `toc_trade_pb_v2-0.1.9/golang/pb/history.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/go/pb/history_grpc.pb.go` & `toc_trade_pb_v2-0.1.9/golang/pb/history_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/go/pb/mq.pb.go` & `toc_trade_pb_v2-0.1.9/golang/pb/mq.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/go/pb/realtime.pb.go` & `toc_trade_pb_v2-0.1.9/golang/pb/realtime.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/go/pb/realtime_grpc.pb.go` & `toc_trade_pb_v2-0.1.9/golang/pb/realtime_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/go/pb/subscribe.pb.go` & `toc_trade_pb_v2-0.1.9/golang/pb/subscribe.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/go/pb/subscribe_grpc.pb.go` & `toc_trade_pb_v2-0.1.9/golang/pb/subscribe_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/go/pb/trade.pb.go` & `toc_trade_pb_v2-0.1.9/golang/pb/trade.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/go/pb/trade_grpc.pb.go` & `toc_trade_pb_v2-0.1.9/golang/pb/trade_grpc.pb.go`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/app/app.pb.dart` & `toc_trade_pb_v2-0.1.9/lib/app/app.pb.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/app/app.pbenum.dart` & `toc_trade_pb_v2-0.1.9/lib/app/app.pbenum.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/app/app.pbjson.dart` & `toc_trade_pb_v2-0.1.9/lib/app/app.pbjson.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/basic.pb.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/basic.pb.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/basic.pbjson.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/basic.pbjson.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/basic.pbserver.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/basic.pbserver.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/entity.pb.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/entity.pb.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/entity.pbjson.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/entity.pbjson.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/history.pb.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/history.pb.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/history.pbjson.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/history.pbjson.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/history.pbserver.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/history.pbserver.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/mq.pb.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/mq.pb.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/mq.pbenum.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/mq.pbenum.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/mq.pbjson.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/mq.pbjson.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/realtime.pb.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/realtime.pb.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/realtime.pbjson.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/realtime.pbjson.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/realtime.pbserver.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/realtime.pbserver.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/subscribe.pb.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/subscribe.pb.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/subscribe.pbjson.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/subscribe.pbjson.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/subscribe.pbserver.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/subscribe.pbserver.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/trade.pb.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/trade.pb.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/trade.pbjson.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/trade.pbjson.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/forwarder/trade.pbserver.dart` & `toc_trade_pb_v2-0.1.9/lib/forwarder/trade.pbserver.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/google/protobuf/empty.pb.dart` & `toc_trade_pb_v2-0.1.9/lib/google/protobuf/empty.pb.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/lib/google/protobuf/empty.pbjson.dart` & `toc_trade_pb_v2-0.1.9/lib/google/protobuf/empty.pbjson.dart`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/protos/v3/app/app.proto` & `toc_trade_pb_v2-0.1.9/protos/v3/app/app.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/protos/v3/forwarder/basic.proto` & `toc_trade_pb_v2-0.1.9/protos/v3/forwarder/basic.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/protos/v3/forwarder/history.proto` & `toc_trade_pb_v2-0.1.9/protos/v3/forwarder/history.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/protos/v3/forwarder/mq.proto` & `toc_trade_pb_v2-0.1.9/protos/v3/forwarder/mq.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/protos/v3/forwarder/realtime.proto` & `toc_trade_pb_v2-0.1.9/protos/v3/forwarder/realtime.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/protos/v3/forwarder/subscribe.proto` & `toc_trade_pb_v2-0.1.9/protos/v3/forwarder/subscribe.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/protos/v3/forwarder/trade.proto` & `toc_trade_pb_v2-0.1.9/protos/v3/forwarder/trade.proto`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/app/app_pb2.py` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/app/app_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/app/app_pb2.pyi` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/app/app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/app/app_pb2_grpc.py` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/app/app_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/basic_pb2.py` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/basic_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/basic_pb2.pyi` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/basic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/basic_pb2_grpc.py` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/basic_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/entity_pb2.py` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/entity_pb2.pyi` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/entity_pb2_grpc.py` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/entity_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/history_pb2.py` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/history_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/history_pb2.pyi` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/history_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/history_pb2_grpc.py` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/history_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/mq_pb2.py` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/mq_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/mq_pb2.pyi` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/mq_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/mq_pb2_grpc.py` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/mq_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/realtime_pb2.py` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/realtime_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/realtime_pb2.pyi` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/realtime_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/realtime_pb2_grpc.py` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/realtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/subscribe_pb2.py` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/subscribe_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/subscribe_pb2.pyi` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/subscribe_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/subscribe_pb2_grpc.py` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/subscribe_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/trade_pb2.py` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/trade_pb2.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/trade_pb2.pyi` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/trade_pb2.pyi`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/py/toc_trade_pb/forwarder/trade_pb2_grpc.py` & `toc_trade_pb_v2-0.1.9/python/toc_trade_pb/forwarder/trade_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/ts/app/app.ts` & `toc_trade_pb_v2-0.1.9/typescript/app/app.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/ts/forwarder/basic.ts` & `toc_trade_pb_v2-0.1.9/typescript/forwarder/basic.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/ts/forwarder/entity.ts` & `toc_trade_pb_v2-0.1.9/typescript/forwarder/entity.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/ts/forwarder/history.ts` & `toc_trade_pb_v2-0.1.9/typescript/forwarder/history.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/ts/forwarder/mq.ts` & `toc_trade_pb_v2-0.1.9/typescript/forwarder/mq.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/ts/forwarder/realtime.ts` & `toc_trade_pb_v2-0.1.9/typescript/forwarder/realtime.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/ts/forwarder/subscribe.ts` & `toc_trade_pb_v2-0.1.9/typescript/forwarder/subscribe.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/ts/forwarder/trade.ts` & `toc_trade_pb_v2-0.1.9/typescript/forwarder/trade.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/ts/google/protobuf/empty.ts` & `toc_trade_pb_v2-0.1.9/typescript/google/protobuf/empty.ts`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/LICENSE` & `toc_trade_pb_v2-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `toc_trade_pb_v2-0.1.8/pyproject.toml` & `toc_trade_pb_v2-0.1.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "toc-trade-pb-v2"
-version = "0.1.8"
+version = "0.1.9"
 authors = [{ name = "Tim Hsu", email = "maochindada@gmail.com" }]
 description = "Pre-compiled Python protobuf files for ToC Trade"
 readme = "README.md"
 requires-python = ">=3.11"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
+classifiers = ["Programming Language :: Python :: 3"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["py/toc_trade_pb"]
 
 [project.urls]
 Homepage = "https://github.com/ToC-Taiwan/toc-trade-protobuf"
 Issues = "https://github.com/ToC-Taiwan/toc-trade-protobuf/issues"
```

