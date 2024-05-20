# Comparing `tmp/spaceone-core-2.0.84.tar.gz` & `tmp/spaceone-core-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaceone-core-2.0.84.tar", last modified: Mon May 20 00:33:52 2024, max compression
+gzip compressed data, was "spaceone-core-2.0.9.tar", last modified: Wed Nov  1 08:35:45 2023, max compression
```

## Comparing `spaceone-core-2.0.84.tar` & `spaceone-core-2.0.9.tar`

### file list

```diff
@@ -1,134 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.678866 spaceone-core-2.0.84/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-20 00:33:52.678866 spaceone-core-2.0.84/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 00:33:52.678866 spaceone-core-2.0.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.666866 spaceone-core-2.0.84/spaceone/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.666866 spaceone-core-2.0.84/spaceone/core/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.666866 spaceone-core-2.0.84/spaceone/core/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.666866 spaceone-core-2.0.84/spaceone/core/auth/jwt/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/auth/jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/auth/jwt/jwt_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.666866 spaceone-core-2.0.84/spaceone/core/cache/
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/cache/base_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/cache/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/cache/redis_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.666866 spaceone-core-2.0.84/spaceone/core/config/
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/config/default_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.666866 spaceone-core-2.0.84/spaceone/core/connector/
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5024 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/connector/space_connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.670866 spaceone-core-2.0.84/spaceone/core/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/fastapi/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.670866 spaceone-core-2.0.84/spaceone/core/fastapi/extension/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/fastapi/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/fastapi/extension/health.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/fastapi/extension/reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/fastapi/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.670866 spaceone-core-2.0.84/spaceone/core/handler/
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/handler/authentication_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/handler/authorization_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/handler/mutation_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/locator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.670866 spaceone-core-2.0.84/spaceone/core/logger/
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/logger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.670866 spaceone-core-2.0.84/spaceone/core/logger/filters/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/logger/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/logger/filters/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/logger/filters/exclude.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/logger/filters/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/logger/filters/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/logger/filters/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/logger/filters/traceback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/logger/filters/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.670866 spaceone-core-2.0.84/spaceone/core/model/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/model/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.670866 spaceone-core-2.0.84/spaceone/core/model/mongo_model/
--rw-r--r--   0 runner    (1001) docker     (127)    51641 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/model/mongo_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/model/mongo_model/filter_operator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/model/mongo_model/stat_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.670866 spaceone-core-2.0.84/spaceone/core/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/opentelemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/opentelemetry/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/opentelemetry/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.674866 spaceone-core-2.0.84/spaceone/core/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/plugin/plugin_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/plugin/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.674866 spaceone-core-2.0.84/spaceone/core/pygrpc/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/pygrpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/pygrpc/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/pygrpc/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.674866 spaceone-core-2.0.84/spaceone/core/pygrpc/extension/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/pygrpc/extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/pygrpc/extension/grpc_health.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/pygrpc/extension/server_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/pygrpc/message_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/pygrpc/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.674866 spaceone-core-2.0.84/spaceone/core/queue/
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/queue/redis_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.674866 spaceone-core-2.0.84/spaceone/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/scheduler/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/scheduler/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/scheduler/task_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/scheduler/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.674866 spaceone-core-2.0.84/spaceone/core/service/
--rw-r--r--   0 runner    (1001) docker     (127)     9434 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/service/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.674866 spaceone-core-2.0.84/spaceone/core/skeleton/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/skeleton/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.674866 spaceone-core-2.0.84/spaceone/core/skeleton/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/skeleton/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/skeleton/conf/global_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.674866 spaceone-core-2.0.84/spaceone/core/skeleton/connector/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/skeleton/connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.674866 spaceone-core-2.0.84/spaceone/core/skeleton/error/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/skeleton/error/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.674866 spaceone-core-2.0.84/spaceone/core/skeleton/info/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/skeleton/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/skeleton/info/helloworld_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.678866 spaceone-core-2.0.84/spaceone/core/skeleton/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/skeleton/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.678866 spaceone-core-2.0.84/spaceone/core/skeleton/interface/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/skeleton/interface/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/skeleton/interface/grpc/helloworld.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.678866 spaceone-core-2.0.84/spaceone/core/skeleton/interface/rest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/skeleton/interface/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.678866 spaceone-core-2.0.84/spaceone/core/skeleton/interface/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/skeleton/interface/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.678866 spaceone-core-2.0.84/spaceone/core/skeleton/manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/skeleton/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/skeleton/manager/helloworld_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.678866 spaceone-core-2.0.84/spaceone/core/skeleton/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/skeleton/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.678866 spaceone-core-2.0.84/spaceone/core/skeleton/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/skeleton/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/skeleton/service/helloworld_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.678866 spaceone-core-2.0.84/spaceone/core/unittest/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/unittest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/unittest/result.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/unittest/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    14890 2024-05-20 00:33:40.000000 spaceone-core-2.0.84/spaceone/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:33:52.678866 spaceone-core-2.0.84/spaceone_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-20 00:33:52.000000 spaceone-core-2.0.84/spaceone_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-20 00:33:52.000000 spaceone-core-2.0.84/spaceone_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 00:33:52.000000 spaceone-core-2.0.84/spaceone_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-20 00:33:52.000000 spaceone-core-2.0.84/spaceone_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 00:33:52.000000 spaceone-core-2.0.84/spaceone_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-20 00:33:52.000000 spaceone-core-2.0.84/spaceone_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 00:33:52.000000 spaceone-core-2.0.84/spaceone_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.033508 spaceone-core-2.0.9/spaceone/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.033508 spaceone-core-2.0.9/spaceone/core/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.033508 spaceone-core-2.0.9/spaceone/core/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.033508 spaceone-core-2.0.9/spaceone/core/auth/jwt/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/auth/jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/auth/jwt/jwt_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.033508 spaceone-core-2.0.9/spaceone/core/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/cache/base_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/cache/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/cache/redis_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8486 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.033508 spaceone-core-2.0.9/spaceone/core/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/config/default_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.033508 spaceone-core-2.0.9/spaceone/core/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/connector/space_connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7722 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.033508 spaceone-core-2.0.9/spaceone/core/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/fastapi/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.033508 spaceone-core-2.0.9/spaceone/core/fastapi/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/fastapi/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/fastapi/extension/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/fastapi/extension/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/fastapi/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/handler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/handler/authentication_api_key_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/handler/authentication_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/handler/authorization_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/handler/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/handler/mutation_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/locator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/logger/
+-rw-r--r--   0 runner    (1001) docker     (127)     4792 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/logger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/logger/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/logger/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/logger/filters/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/logger/filters/exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/logger/filters/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/logger/filters/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/logger/filters/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/logger/filters/traceback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/logger/filters/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/model/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/model/mongo_model/
+-rw-r--r--   0 runner    (1001) docker     (127)    45629 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/model/mongo_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/model/mongo_model/filter_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8532 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/model/mongo_model/stat_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/opentelemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/opentelemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/opentelemetry/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/opentelemetry/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/pygrpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/pygrpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/pygrpc/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/pygrpc/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/pygrpc/extension/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/pygrpc/extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/pygrpc/extension/grpc_health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/pygrpc/extension/server_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6468 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/pygrpc/message_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/pygrpc/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/queue/redis_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/scheduler/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/scheduler/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/scheduler/task_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/scheduler/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/service/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10721 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/service/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10237 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/service/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/skeleton/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/skeleton/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/conf/global_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/skeleton/connector/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/skeleton/error/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.037508 spaceone-core-2.0.9/spaceone/core/skeleton/info/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/info/helloworld_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/spaceone/core/skeleton/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/spaceone/core/skeleton/interface/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/interface/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/interface/grpc/helloworld.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/spaceone/core/skeleton/interface/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/interface/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/spaceone/core/skeleton/interface/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/interface/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/spaceone/core/skeleton/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/manager/helloworld_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/spaceone/core/skeleton/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/spaceone/core/skeleton/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/skeleton/service/helloworld_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/spaceone/core/unittest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/unittest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/unittest/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/unittest/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14475 2023-11-01 08:35:29.000000 spaceone-core-2.0.9/spaceone/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 08:35:45.041508 spaceone-core-2.0.9/spaceone_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2023-11-01 08:35:44.000000 spaceone-core-2.0.9/spaceone_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2023-11-01 08:35:44.000000 spaceone-core-2.0.9/spaceone_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-01 08:35:44.000000 spaceone-core-2.0.9/spaceone_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-01 08:35:44.000000 spaceone-core-2.0.9/spaceone_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-01 08:35:44.000000 spaceone-core-2.0.9/spaceone_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2023-11-01 08:35:44.000000 spaceone-core-2.0.9/spaceone_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-01 08:35:44.000000 spaceone-core-2.0.9/spaceone_core.egg-info/top_level.txt
```

### Comparing `spaceone-core-2.0.84/setup.py` & `spaceone-core-2.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,17 +71,14 @@
         # CLI packages
         'click',
 
         # model packages
         'pydantic',
         'mongoengine',
 
-        # AWS packages
-        'boto3',
-
         # test framework packages
         'unittest-xml-reporting',
         'factory-boy',
         'mongomock',
 
         # tracing packages
         'opentelemetry-api',
```

### Comparing `spaceone-core-2.0.84/spaceone/core/auth/jwt/__init__.py` & `spaceone-core-2.0.9/spaceone/core/auth/jwt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from spaceone.core.auth import Authenticator
 from spaceone.core.auth.jwt.jwt_util import JWTUtil
 from spaceone.core.error import *
 
 
 class JWTAuthenticator(Authenticator):
+
     def __init__(self, key):
         self._key = key
 
     def validate(self, token, options=None):
         if not self._key:
-            raise ERROR_AUTHENTICATE_FAILURE(message="Decode key is not set.")
+            raise ERROR_AUTHENTICATE_FAILURE(message='Decode key is not set.')
 
         if not isinstance(token, (str, bytes)):
-            raise ERROR_AUTHENTICATE_FAILURE(message="Invalid token format.")
+            raise ERROR_AUTHENTICATE_FAILURE(message='Invalid token format.')
 
         if options is None:
             options = {}
 
         try:
             payload = JWTUtil.decode(token, self._key, options=options)
         except Exception:
-            raise ERROR_AUTHENTICATE_FAILURE(message="Token is invalid or expired.")
+            raise ERROR_AUTHENTICATE_FAILURE(message='Token is invalid or expired.')
 
         return payload
```

### Comparing `spaceone-core-2.0.84/spaceone/core/auth/jwt/jwt_util.py` & `spaceone-core-2.0.9/spaceone/core/auth/jwt/jwt_util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,30 @@
 import json
 from jwcrypto import jwk
 from jose import jwt
 
 
 class JWTUtil:
+
     @staticmethod
-    def generate_jwk(key_type="RSA", size=2048):
+    def generate_jwk(key_type='RSA', size=2048):
         key = jwk.JWK.generate(kty=key_type, size=size)
         private_jwk = json.loads(key.export_private())
         public_jwk = json.loads(key.export_public())
         return private_jwk, public_jwk
 
     @staticmethod
-    def encode(payload: dict, private_jwk: dict, algorithm="RS256") -> str:
+    def encode(payload: dict, private_jwk: dict, algorithm='RS256') -> str:
         return jwt.encode(payload, key=private_jwk, algorithm=algorithm)
 
     @staticmethod
-    def decode(token: str, public_jwk: dict, algorithm="RS256", options=None) -> dict:
+    def decode(token: str, public_jwk: dict, algorithm='RS256', options=None) -> dict:
         if options is None:
             options = {}
 
-        options["verify_aud"] = options.get("verify_aud", False)
+        options['verify_aud'] = options.get('verify_aud', False)
 
         return jwt.decode(token, key=public_jwk, algorithms=algorithm, options=options)
 
     @staticmethod
     def unverified_decode(token: str) -> dict:
         return jwt.get_unverified_claims(token)
-
-    @staticmethod
-    def get_value_from_token(token: str, key: str, default: any = None) -> any:
-        try:
-            return JWTUtil.unverified_decode(token).get(key, default)
-        except Exception as e:
-            return default
```

### Comparing `spaceone-core-2.0.84/spaceone/core/cache/__init__.py` & `spaceone-core-2.0.9/spaceone/core/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/cache/base_cache.py` & `spaceone-core-2.0.9/spaceone/core/cache/base_cache.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/cache/local_cache.py` & `spaceone-core-2.0.9/spaceone/core/cache/local_cache.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/cache/redis_cache.py` & `spaceone-core-2.0.9/spaceone/core/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/config/__init__.py` & `spaceone-core-2.0.9/spaceone/core/config/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,35 +6,25 @@
 from spaceone.core.config import default_conf
 
 _REMOTE_URL = []
 _GLOBAL = {}
 _LOGGER = logging.getLogger(__name__)
 
 
-def init_conf(package: str, port: int = None, host: str = None, grpc_app_path: str = None,
-              rest_app_path: str = None, plugin_app_path: str = None):
+def init_conf(package, **kwargs):
     set_default_conf()
 
     _GLOBAL['PACKAGE'] = package
     _GLOBAL['SERVICE'] = package.rsplit('.', 1)[-1:][0]
 
-    if host:
-        _GLOBAL['HOST'] = host
+    if 'host' in kwargs:
+        _GLOBAL['HOST'] = kwargs['HOST']
 
-    if port:
-        _GLOBAL['PORT'] = port
-
-    if grpc_app_path:
-        _GLOBAL['GRPC_APP_PATH'] = grpc_app_path
-
-    if rest_app_path:
-        _GLOBAL['REST_APP_PATH'] = rest_app_path
-
-    if plugin_app_path:
-        _GLOBAL['PLUGIN_APP_PATH'] = plugin_app_path
+    if 'port' in kwargs:
+        _GLOBAL['PORT'] = kwargs['port']
 
 
 def set_default_conf():
     for key, value in vars(default_conf).items():
         if not key.startswith('__'):
             _GLOBAL[key] = value
 
@@ -43,33 +33,32 @@
     return _GLOBAL['PACKAGE']
 
 
 def get_service():
     return _GLOBAL['SERVICE']
 
 
+def get_handler(name):
+    return _GLOBAL.get('HANDLERS', {}).get(name, {})
+
+
 def get_connector(name):
     return _GLOBAL.get('CONNECTORS', {}).get(name, {})
 
 
-def set_service_config(global_conf_path: str = None):
+def set_service_config():
     """
-    Get config from service
+    Get config from service ({package}.conf.global_conf)
     """
 
     package = _GLOBAL['PACKAGE']
     if package is None:
         raise ValueError(f'Package is undefined.')
 
-    global_conf_path = global_conf_path or _GLOBAL['GLOBAL_CONF_PATH']
-    global_conf_path = global_conf_path.format(package=package)
-
-    module_path, fromlist = global_conf_path.split(':')
-    global_module = __import__(module_path, fromlist=[fromlist])
-
+    global_module = __import__(f'{package}.conf.global_conf', fromlist=['global_conf'])
     for key, value in vars(global_module).items():
         if not key.startswith('__'):
             if key in _GLOBAL:
                 if isinstance(value, dict):
                     _GLOBAL[key] = utils.deep_merge(value, _GLOBAL[key])
                 else:
                     _GLOBAL[key] = value
@@ -154,13 +143,14 @@
 
         if port:
             conf['port'] = port
 
         c = consul.Consul(**conf)
         index, data = c.kv.get(key)
         if data:
+            print(data)
             json_str = data['Value'].decode('utf-8')
             return utils.load_json(json_str)
 
         return {}
     except Exception as e:
         raise Exception(f'Consul Call Error: {e}')
```

### Comparing `spaceone-core-2.0.84/spaceone/core/config/default_conf.py` & `spaceone-core-2.0.9/spaceone/core/config/default_conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,32 +5,25 @@
 # Server Configuration
 PORT = 50051
 HOST = '127.0.0.1'
 
 MAX_WORKERS = 100
 MAX_MESSAGE_LENGTH = 1024 * 1024 * 1024
 
-# Global Configuration
-GLOBAL_CONF_PATH = '{package}.conf.global_conf:global_conf'
-
 # Unit Test Configuration
 MOCK_MODE = False
 
 # gRPC Configuration
-GRPC_APP_PATH = '{package}.interface.grpc:app'
-
 # gRPC Extension APIs
 GRPC_EXTENSION_SERVICERS = {
     'spaceone.core.pygrpc.extension.grpc_health': ['GRPCHealth'],
     'spaceone.core.pygrpc.extension.server_info': ['ServerInfo']
 }
 
 # REST Configuration
-REST_APP_PATH = '{package}.interface.rest:app'
-
 # REST Application Options
 REST_TITLE = ''
 REST_DESCRIPTION = ''
 REST_CONTACT = {}
 
 # REST Middlewares
 REST_MIDDLEWARES = []
@@ -44,26 +37,32 @@
 ]
 
 # REST Uvicorn Options
 UVICORN_OPTIONS = {
     'factory': True
 }
 
-# Plugin Configuration
-PLUGIN_APP_PATH = '{package}.main:app'
 
 # Handler Configuration
 HANDLERS = {
     'authentication': [],
     'authorization': [],
     'mutation': [],
     'event': []
 }
 
+HANDLER_EXCLUDE_APIS = {
+    'authentication': [],
+    'authorization': [],
+    'mutation': [],
+    'event': []
+}
+
 # Logging Configuration
+ENABLE_STACK_INFO = False
 LOG = {}
 
 # OpenTelemetry Configuration
 OTEL = {
     'endpoint': None
 }
```

### Comparing `spaceone-core-2.0.84/spaceone/core/connector/space_connector.py` & `spaceone-core-2.0.9/spaceone/core/connector/space_connector.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,156 +1,129 @@
 import types
 import logging
-from typing import Any, List, Tuple
 from google.protobuf.json_format import MessageToDict
 from opentelemetry.trace.propagation.tracecontext import TraceContextTextMapPropagator
 
+from spaceone.core import config as global_config
 from spaceone.core.connector import BaseConnector
 from spaceone.core import pygrpc
 from spaceone.core.utils import parse_grpc_endpoint
-from spaceone.core.pygrpc.client import GRPCClient
 from spaceone.core.error import *
 
 __all__ = ["SpaceConnector"]
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class SpaceConnector(BaseConnector):
-    name = "SpaceConnector"
 
-    def __init__(
-        self,
-        *args,
-        service: str = None,
-        endpoint: str = None,
-        token: str = None,
-        return_type: str = "dict",
-        **kwargs,
-    ):
+    def __init__(self, return_type: str = 'dict', service: str = None, endpoint: str = None, *args, **kwargs):
         super().__init__(*args, **kwargs)
+
+        self._mock_mode = global_config.get_global('MOCK_MODE', False)
         self._service = service
         self._endpoint = endpoint
-        self._token = token
         self._return_type = return_type
-
-        self._client = None
-        self._endpoints: dict = self.config.get("endpoints", {})
-
+        self._token = kwargs.get('token')
+        self._endpoints = self.config.get('endpoints', {})
         self._verify()
-        self._init_client()
+
+        if self._mock_mode is False:
+            self._init_client()
 
     @property
-    def client(self) -> GRPCClient:
+    def client(self):
         return self._client
 
-    def dispatch(self, method: str, params: dict = None, **kwargs) -> Any:
+    def dispatch(self, method: str, params: dict = None, **kwargs):
         return self._call_api(method, params, **kwargs)
 
-    def _call_api(
-        self,
-        method: str,
-        params: dict = None,
-        token: str = None,
-        x_domain_id: str = None,
-        x_workspace_id: str = None,
-    ) -> Any:
+    def _call_api(self, method: str, params: dict = None, **kwargs):
+        token = kwargs.get('token')
+
+        self._check_mock_mode(method)
+
         resource, verb = self._parse_method(method)
         self._check_method(resource, verb)
 
         params = params or {}
-        metadata = self._get_connection_metadata(token, x_domain_id, x_workspace_id)
+        kwargs['metadata'] = self._get_connection_metadata(token)
 
-        response_or_iterator = getattr(getattr(self._client, resource), verb)(
-            params, metadata=metadata
-        )
+        response_or_iterator = getattr(getattr(self._client, resource), verb)(params, **kwargs)
 
-        if self._return_type == "dict":
+        if self._return_type == 'dict':
             if isinstance(response_or_iterator, types.GeneratorType):
                 return self._generate_response(response_or_iterator)
             else:
                 return self._change_message(response_or_iterator)
         else:
             return response_or_iterator
 
-    def _verify(self) -> None:
-        if self._service:
+    def _check_mock_mode(self, method):
+        if self._mock_mode:
+            raise ERROR_CONNECTOR(connector='SpaceConnector',
+                                  reason=f'Dispatch cannot be executed in mock mode. '
+                                         f'(endpoint = {self._get_endpoint()}, method = {method})')
+
+    def _verify(self):
+        if self._endpoint:
+            pass
+        elif self._service:
             if not isinstance(self._endpoints, dict):
-                raise ERROR_CONNECTOR_CONFIGURATION(connector="SpaceConnector")
+                raise ERROR_CONNECTOR_CONFIGURATION(connector='SpaceConnector')
 
             if self._service not in self._endpoints:
-                raise ERROR_CONNECTOR_LOAD(
-                    connector="SpaceConnector",
-                    reason=f"{self._service} endpoint is undefined.",
-                )
-
-        elif not self._endpoint:
-            raise ERROR_CONNECTOR_LOAD(
-                connector="SpaceConnector", reason="service or endpoint is required."
-            )
+                raise ERROR_CONNECTOR_LOAD(connector='SpaceConnector', reason=f'{self._service} endpoint is undefined.')
+        else:
+            raise ERROR_CONNECTOR_LOAD(connector='SpaceConnector', reason='service or endpoint is required.')
 
-    def _init_client(self) -> None:
+    def _init_client(self):
         endpoint = self._get_endpoint()
         e = parse_grpc_endpoint(endpoint)
-        self._client: GRPCClient = pygrpc.client(
-            endpoint=e["endpoint"],
-            ssl_enabled=e["ssl_enabled"],
-            max_message_length=1024 * 1024 * 256,
-        )
+        self._client = pygrpc.client(endpoint=e['endpoint'], ssl_enabled=e['ssl_enabled'],
+                                     max_message_length=1024 * 1024 * 256)
 
     @staticmethod
-    def _change_message(message) -> dict:
+    def _change_message(message):
         return MessageToDict(message, preserving_proto_field_name=True)
 
     def _generate_response(self, response_iterator):
         for response in response_iterator:
             yield self._change_message(response)
 
-    def _get_connection_metadata(
-        self, token: str = None, x_domain_id: str = None, x_workspace_id: str = None
-    ) -> List[Tuple]:
+    def _get_connection_metadata(self, token=None):
         metadata = []
 
         if token:
-            metadata.append(("token", token))
+            metadata.append(('token', token))
         elif self._token:
-            metadata.append(("token", self._token))
-        elif token := self.transaction.meta.get("token"):
-            metadata.append(("token", token))
-
-        if x_domain_id:
-            metadata.append(("x_domain_id", x_domain_id))
-
-        if x_workspace_id:
-            metadata.append(("x_workspace_id", x_workspace_id))
+            metadata.append(('token', self._token))
+        elif token := self.transaction.meta.get('token'):
+            metadata.append(('token', token))
 
         carrier = {}
         TraceContextTextMapPropagator().inject(carrier)
 
-        if traceparent := carrier.get("traceparent"):
-            metadata.append(("traceparent", traceparent))
+        if traceparent := carrier.get('traceparent'):
+            metadata.append(('traceparent', traceparent))
 
         return metadata
 
-    def _parse_method(self, method: str) -> Tuple[str, str]:
+    def _parse_method(self, method):
         try:
-            resource, verb = method.split(".")
+            resource, verb = method.split('.')
         except Exception:
-            raise ERROR_CONNECTOR(
-                connector="SpaceConnector",
-                reason=f"Method is invalid. (endpoint = {self._get_endpoint()}, method = {method})",
-            )
+            raise ERROR_CONNECTOR(connector='SpaceConnector',
+                                  reason=f'Method is invalid. (endpoint = {self._get_endpoint()}, method = {method})')
 
         return resource, verb
 
-    def _check_method(self, resource: str, verb: str) -> None:
+    def _check_method(self, resource, verb):
         supported_verb = self._client.api_resources.get(resource)
 
         if supported_verb is None or verb not in supported_verb:
-            raise ERROR_CONNECTOR(
-                connector="SpaceConnector",
-                reason=f"Method not supported. "
-                f"(endpoint = {self._get_endpoint()}, method = {resource}.{verb})",
-            )
+            raise ERROR_CONNECTOR(connector='SpaceConnector',
+                                  reason=f'Method not supported. (endpoint = {self._get_endpoint()}, '
+                                         f'method = {resource}.{verb})')
 
-    def _get_endpoint(self) -> str:
+    def _get_endpoint(self):
         return self._endpoint or self._endpoints[self._service]
```

### Comparing `spaceone-core-2.0.84/spaceone/core/error.py` & `spaceone-core-2.0.9/spaceone/core/error.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 class ERROR_BASE(Exception):
-    _status_code = "INTERNAL"
-    _error_code = "ERROR_BASE"
-    _message = "Base Error Class"
+    _status_code = 'INTERNAL'
+    _error_code = 'ERROR_BASE'
+    _message = 'Base Error Class'
     _meta = {}
 
     def __init__(self, _error_code=None, _meta=None, **kwargs):
         if isinstance(_meta, dict):
             self._meta = _meta
 
         if _error_code:
             self._error_code = _error_code.strip()
         else:
             self._error_code = self.__class__.__name__
 
         try:
             self._message = self.message.format(**kwargs)
         except Exception:
-            raise ERROR_MESSAGE_FORMAT(
-                error_class=self.__class__.__name__, key=str(kwargs)
-            )
+            raise ERROR_MESSAGE_FORMAT(error_class=self.__class__.__name__, key=str(kwargs))
 
     @property
     def message(self):
         return self._message
 
     @property
     def error_code(self):
@@ -45,255 +43,231 @@
         return self._meta
 
     @meta.setter
     def meta(self, key, value):
         self._meta[key] = value
 
     def _repr(self):
-        return (
-            "\n"
-            f"\terror_code = {self._error_code}\n"
-            f"\tstatus_code = {self._status_code}\n"
-            f"\tmessage = {self._message}"
-        )
+        return ('\n'
+                f'\terror_code = {self._error_code}\n'
+                f'\tstatus_code = {self._status_code}\n'
+                f'\tmessage = {self._message}')
 
     def __repr__(self):
         return self._repr()
 
     def __str__(self):
         return self._repr()
 
 
 class ERROR_INVALID_ARGUMENT(ERROR_BASE):
-    _status_code = "INVALID_ARGUMENT"
-    _message = "Argument is invalid."
-
-
-class ERROR_REQUIRED_X_DOMAIN_ID(ERROR_INVALID_ARGUMENT):
-    _message = "System token requires 'x_domain_id' in metadata."
+    _status_code = 'INVALID_ARGUMENT'
+    _message = 'Argument is invalid.'
 
 
 class ERROR_REQUIRED_PARAMETER(ERROR_INVALID_ARGUMENT):
-    _message = "Required parameter. (key = {key})"
+    _message = 'Required parameter. (key = {key})'
 
 
 class ERROR_INVALID_PARAMETER_TYPE(ERROR_INVALID_ARGUMENT):
-    _message = "Parameter type is invalid. (key = {key}, type = {type})"
+    _message = 'Parameter type is invalid. (key = {key}, type = {type})'
 
 
 class ERROR_INVALID_PARAMETER(ERROR_INVALID_ARGUMENT):
-    _message = "Parameter is invalid. (key = {key}, reason = {reason})"
+    _message = 'Parameter is invalid. (key = {key}, reason = {reason})'
 
 
 class ERROR_NOT_FOUND(ERROR_INVALID_ARGUMENT):
-    _status_code = "NOT_FOUND"
-    _message = "Resource cannot be found or access is denied. ({key} = {value})"
+    _status_code = 'NOT_FOUND'
+    _message = 'Value not found. ({key} = {value})'
 
 
 class ERROR_NOT_UNIQUE(ERROR_INVALID_ARGUMENT):
-    _status_code = "ALREADY_EXISTS"
-    _message = "Tried to save duplicate unique key. ({key} = {value})"
+    _status_code = 'ALREADY_EXISTS'
+    _message = 'Tried to save duplicate unique key. ({key} = {value})'
 
 
 class ERROR_SAVE_UNIQUE_VALUES(ERROR_NOT_UNIQUE):
-    _message = "Tried to save duplicate unique values. (keys = {keys})"
+    _message = 'Tried to save duplicate unique values. (keys = {keys})'
 
 
 class ERROR_EXIST_RESOURCE(ERROR_INVALID_ARGUMENT):
-    _message = "'{child}' resources is existed in {parent}."
+    _message = '\'{child}\' resources is existed in {parent}.'
 
 
 class ERROR_OPERATOR_VALUE_TYPE(ERROR_INVALID_ARGUMENT):
-    _message = (
-        "The value of '{operator} operator' does not support list type. ({condition})"
-    )
+    _message = 'The value of \'{operator} operator\' does not support list type. ({condition})'
 
 
 class ERROR_OPERATOR_LIST_VALUE_TYPE(ERROR_INVALID_ARGUMENT):
-    _message = "The value of '{operator} operator' must be a list type. ({condition})"
+    _message = 'The value of \'{operator} operator\' must be a list type. ({condition})'
 
 
 class ERROR_OPERATOR_DICT_VALUE_TYPE(ERROR_INVALID_ARGUMENT):
-    _message = (
-        "The value of '{operator} operator' must be a dictionary type. ({condition})"
-    )
+    _message = 'The value of \'{operator} operator\' must be a dictionary type. ({condition})'
 
 
 class ERROR_OPERATOR_BOOLEAN_TYPE(ERROR_INVALID_ARGUMENT):
-    _message = (
-        "The value of '{operator} operator' must be a boolean type. ({condition})"
-    )
+    _message = 'The value of \'{operator} operator\' must be a boolean type. ({condition})'
 
 
 class ERROR_INVALID_FORMAT(ERROR_INVALID_ARGUMENT):
-    _message = "Value format is invalid. ({key} = {value} ! {rule})"
+    _message = 'Value format is invalid. ({key} = {value} ! {rule})'
 
 
 class ERROR_JSON_FORMAT(ERROR_INVALID_ARGUMENT):
-    _message = "JSON format is invalid. ({key} = {value})"
+    _message = 'JSON format is invalid. ({key} = {value})'
 
 
 class ERROR_AUTHENTICATE_FAILURE(ERROR_INVALID_ARGUMENT):
-    _status_code = "UNAUTHENTICATED"
-    _message = "Authenticate failure. (message = {message})"
+    _status_code = 'UNAUTHENTICATED'
+    _message = 'Authenticate failure. (message = {message})'
 
 
 class ERROR_PERMISSION_DENIED(ERROR_INVALID_ARGUMENT):
-    _status_code = "PERMISSION_DENIED"
-    _message = "Permission denied."
+    _status_code = 'PERMISSION_DENIED'
+    _message = 'Permission denied.'
 
 
 class ERROR_UNKNOWN(ERROR_BASE):
-    _status_code = "INTERNAL"
-    _message = "{message}"
+    _status_code = 'INTERNAL'
+    _message = '{message}'
 
 
 class ERROR_REQUEST_TIMEOUT(ERROR_UNKNOWN):
-    _status_code = "DEADLINE_EXCEEDED"
-    _message = "Request timeout!"
+    _status_code = 'DEADLINE_EXCEEDED'
+    _message = 'Request timeout!'
 
 
 class ERROR_TRANSACTION_STATUS(ERROR_UNKNOWN):
-    _message = "Transaction status is incorrect. (status = {status})"
+    _message = 'Transaction status is incorrect. (status = {status})'
 
 
 class ERROR_UNSUPPORTED_API(ERROR_UNKNOWN):
-    _message = "Call Unsupported API. (reason = {reason})"
+    _message = 'Call Unsupported API. (reason = {reason})'
 
 
 class ERROR_CONFIGURATION(ERROR_UNKNOWN):
-    _message = "Configuration is invalid. (key = {key})"
+    _message = 'Configuration is invalid. (key = {key})'
 
 
 class ERROR_DB_ENGINE_UNDEFINE(ERROR_CONFIGURATION):
-    _message = "Database engine is undefined. (alias = {alias})"
+    _message = 'Database engine is undefined. (alias = {alias})'
 
 
 class ERROR_CACHE_CONFIGURATION(ERROR_CONFIGURATION):
-    _message = "Cache is not configured. (alias = {alias})"
+    _message = 'Cache is not configured. (alias = {alias})'
 
 
 class ERROR_CACHE_ENGINE_UNDEFINE(ERROR_CONFIGURATION):
-    _message = "Cache engine is undefined. (alias = {alias})"
+    _message = 'Cache engine is undefined. (alias = {alias})'
 
 
 class ERROR_CONNECTOR_CONFIGURATION(ERROR_CONFIGURATION):
-    _message = "Connector configuration is invalid. (backend = {backend})"
+    _message = 'Connector configuration is invalid. (backend = {backend})'
 
 
 class ERROR_GRPC_CONFIGURATION(ERROR_CONFIGURATION):
-    _message = "gRPC client configuration is invalid. ({endpoint}/{service}/{method})"
+    _message = 'gRPC client configuration is invalid. ({endpoint}/{service}/{method})'
 
 
 class ERROR_HANDLER_CONFIGURATION(ERROR_CONFIGURATION):
-    _message = (
-        "Handler configuration is invalid. (handler = {handler}, reason = {reason})"
-    )
+    _message = 'Handler configuration is invalid. (handler = {handler})'
 
 
 class ERROR_CONNECTOR_CONFIGURATION(ERROR_CONFIGURATION):
-    _message = "Connector configuration is invalid. (connector = {connector}, reason = {reason})"
+    _message = 'Connector configuration is invalid. (connector = {connector})'
 
 
 class ERROR_LOG_CONFIG(ERROR_CONFIGURATION):
-    _message = "Log configuration is invalid. (reason = {reason})"
+    _message = 'Log configuration is invalid. (reason = {reason})'
 
 
 class ERROR_WRONG_CONFIGURATION(ERROR_CONFIGURATION):
-    _message = "Configuration is invalid. ({key})"
+    _message = 'Configuration is invalid. ({key})'
 
 
 class ERROR_DB_QUERY(ERROR_UNKNOWN):
-    _message = "Database query failed. (reason = {reason})"
+    _message = 'Database query failed. (reason = {reason})'
 
 
 class ERROR_CACHE_OPTION(ERROR_UNKNOWN):
-    _message = (
-        "Does not support the cache option. (method = {method}, option = {option})"
-    )
+    _message = 'Does not support the cache option. (method = {method}, option = {option})'
 
 
 class ERROR_CACHE_TIMEOUT(ERROR_UNKNOWN):
-    _message = "Cache timeout error. (config = {config})"
+    _message = 'Cache timeout error. (config = {config})'
 
 
 class ERROR_CACHE_ENCODE(ERROR_UNKNOWN):
-    _message = "Cache data encoding failed. (reason = {reason})"
+    _message = 'Cache data encoding failed. (reason = {reason})'
 
 
 class ERROR_CACHE_DECODE(ERROR_UNKNOWN):
-    _message = "Cache data decoding failed. (reason = {reason})"
+    _message = 'Cache data decoding failed. (reason = {reason})'
 
 
 class ERROR_CACHEABLE_VALUE_TYPE(ERROR_UNKNOWN):
-    _message = "The value of cache.cacheable must be a dict type."
+    _message = 'The value of cache.cacheable must be a dict type.'
 
 
 class ERROR_INTERNAL_API(ERROR_UNKNOWN):
-    _message = "{message}"
+    _message = '{message}'
 
 
 class ERROR_UNAVAILAVBLE(ERROR_UNKNOWN):
-    _status_code = "UNAVAILABLE"
-    _message = "Server is unavailable. (reason = {reason})"
+    _status_code = 'UNAVAILABLE'
+    _message = 'Server is unavailable. (reason = {reason})'
 
 
 class ERROR_QUEUE_PUT(ERROR_UNAVAILAVBLE):
-    _message = "Queue data put failed. (reason = {reason})"
+    _message = 'Queue data put failed. (reason = {reason})'
 
 
 class ERROR_QUEUE_GET(ERROR_UNAVAILAVBLE):
-    _message = "Queue data get failed. (reason = {reason})"
+    _message = 'Queue data get failed. (reason = {reason})'
 
 
 class ERROR_GRPC_CONNECTION(ERROR_UNAVAILAVBLE):
-    _status_code = "UNAVAILABLE"
-    _message = "Server is unavailable. (channel = {channel}, message = {message})"
+    _status_code = 'UNAVAILABLE'
+    _message = 'Server is unavailable. (channel = {channel}, message = {message})'
 
 
 class ERROR_GRPC_TLS_HANDSHAKE(ERROR_GRPC_CONNECTION):
-    _message = "TLS handshake failed. (reason = {reason})"
+    _message = 'TLS handshake failed. (reason = {reason})'
 
 
 class ERROR_HANDLER(ERROR_UNKNOWN):
-    _message = "'{handler_type} handler' import failed. (reason = {reason})"
+    _message = '\'{handler_type} handler\' import failed. (reason = {reason})'
 
 
 class ERROR_CONNECTOR(ERROR_UNKNOWN):
-    _message = "'{connector} handler' import failed. (reason = {reason})"
+    _message = '\'{connector} handler\' import failed. (reason = {reason})'
 
 
 class ERROR_CONNECTOR_LOAD(ERROR_CONNECTOR):
-    _message = "Failed to load connector. (connector = {connector}, reason = {reason})"
+    _message = 'Failed to load connector. (connector = {connector}, reason = {reason})'
 
 
 class ERROR_LOCATOR(ERROR_UNKNOWN):
-    _message = "'{name}' load failed. (reason = {reason})"
+    _message = '\'{name}\' load failed. (reason = {reason})'
 
 
 class ERROR_TASK_LOCATOR(ERROR_LOCATOR):
-    _message = "Call locator failure. (locator = {locator}, name = {name})"
+    _message = 'Call locator failure. locator: {locator}, name: {name}'
 
 
 class ERROR_TASK_METHOD(ERROR_UNKNOWN):
-    _message = "Call method failure. (name = {name}, method = {method})"
+    _message = 'Call method failure. name: {name}, method: {method}, params: {params}'
 
 
 class ERROR_NOT_IMPLEMENTED(ERROR_UNKNOWN):
-    _status_code = "UNIMPLEMENTED"
-    _message = "Not implemented."
+    _status_code = 'UNIMPLEMENTED'
+    _message = 'Not implemented, {name}'
 
 
 class ERROR_MESSAGE_FORMAT(ERROR_UNKNOWN):
-    _message = (
-        "Error message format is invalid. (error_class = {error_class}, key = {key})"
-    )
+    _message = 'Error message format is invalid. (error_class={error_class}, key={key})'
 
 
 class ERROR_CACHE_KEY_FORMAT(ERROR_UNKNOWN):
-    _message = "Cache key format is invalid. (key = {key})"
-
-
-class ERROR_SERVICE_ACCOUNT_CANNOT_BE_DELETED_WITH_EXISTING_APP(ERROR_INVALID_ARGUMENT):
-    _status_code = "INVALID_OPERATION"
-    _message = """Service Account cannot be deleted as long as an associated App exists. 
-    Please delete the App before deleting the Service Account. (error_class = {error_class}, key = {key})"""
+    _message = 'Cache key format is invalid. (key={key})'
```

### Comparing `spaceone-core-2.0.84/spaceone/core/fastapi/api.py` & `spaceone-core-2.0.9/spaceone/core/fastapi/api.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/fastapi/extension/reflection.py` & `spaceone-core-2.0.9/spaceone/core/fastapi/extension/reflection.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/fastapi/server.py` & `spaceone-core-2.0.9/spaceone/core/fastapi/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,17 +130,15 @@
 def fast_api_app():
     app = _init_fast_api()
     app = _add_middlewares(app)
     app = _include_routers(app)
     return app
 
 
-def serve(app_path: str = None):
+def serve():
     conf = config.get_global()
-    app_path = conf['REST_APP_PATH']
-
     uvicorn_options = conf.get('UVICORN_OPTIONS', {})
 
     _LOGGER.info(f'Start REST Server ({config.get_service()}): '
                  f'host={conf["HOST"]} port={conf["PORT"]} options={uvicorn_options}')
 
     uvicorn.run('spaceone.core.fastapi.server:fast_api_app', host=conf['HOST'], port=conf['PORT'], **uvicorn_options)
```

### Comparing `spaceone-core-2.0.84/spaceone/core/handler/mutation_handler.py` & `spaceone-core-2.0.9/spaceone/core/handler/mutation_handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,62 @@
 import logging
 from spaceone.core.handler import BaseMutationHandler
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class SpaceONEMutationHandler(BaseMutationHandler):
+
     def request(self, params):
-        user_role_type: str = self.transaction.get_meta("authorization.role_type")
-        domain_id: str = self.transaction.get_meta("authorization.domain_id")
-        workspace_id: str = self.transaction.get_meta("authorization.workspace_id")
-        user_projects: list = self.transaction.get_meta("authorization.projects")
-        user_id: str = self.transaction.get_meta("authorization.user_id")
-        set_user_id: str = self.transaction.get_meta("authorization.set_user_id")
-        injected_params: dict = self.transaction.get_meta("authorization.injected_params")
-
-        if user_role_type == "SYSTEM_TOKEN":
-            if domain_id:
-                params["domain_id"] = domain_id
-
-            if workspace_id:
-                params["workspace_id"] = workspace_id
-
-        elif user_role_type == "DOMAIN_ADMIN":
-            params["domain_id"] = domain_id
-        elif user_role_type == "WORKSPACE_OWNER":
-            params["domain_id"] = domain_id
-            params["workspace_id"] = workspace_id
-        elif user_role_type == "WORKSPACE_MEMBER":
-            params["domain_id"] = domain_id
-            params["workspace_id"] = workspace_id
-            params["user_projects"] = user_projects
-        elif user_role_type == "USER":
-            params["domain_id"] = domain_id
+        scope = self.transaction.get_meta('authorization.scope')
+        role_type = self.transaction.get_meta('authorization.role_type')
+
+        domain_id = self.transaction.get_meta('domain_id') or params.get('domain_id')
+
+        if role_type and role_type != 'SYSTEM':
+            if scope == 'DOMAIN':
+                params = self._apply_domain_scope(params, role_type, domain_id)
+            elif scope == 'PROJECT':
+                params = self._apply_project_scope(params, role_type, domain_id)
+            elif scope == 'USER':
+                params = self._apply_user_scope(params, role_type, domain_id)
+            elif scope == 'DOMAIN_OR_PROJECT':
+                params = self._apply_domain_or_project_scope(params, role_type, domain_id)
+            elif scope == 'PUBLIC_OR_DOMAIN':
+                params = self._apply_public_or_domain_scope(params, role_type, domain_id)
+
+        return params
+
+    def _apply_domain_scope(self, params, role_type, domain_id):
+        params['domain_id'] = domain_id
+        return params
+
+    def _apply_project_scope(self, params, role_type, domain_id):
+        params['domain_id'] = domain_id
+
+        if role_type == 'PROJECT':
+            params['user_projects'] = self.transaction.get_meta('authorization.projects')
+            params['user_project_groups'] = self.transaction.get_meta('authorization.project_groups')
 
-        if set_user_id:
-            params["user_id"] = user_id
+        return params
+
+    def _apply_user_scope(self, params, role_type, domain_id):
+        params['domain_id'] = domain_id
+
+        if role_type in ['PROJECT', 'USER']:
+            params['user_id'] = self.transaction.get_meta('user_id')
+
+        return params
+
+    def _apply_domain_or_project_scope(self, params, role_type, domain_id):
+        params['domain_id'] = domain_id
+
+        if role_type == 'PROJECT':
+            params['user_projects'] = self.transaction.get_meta('authorization.projects') + [None]
+            params['user_project_groups'] = self.transaction.get_meta('authorization.project_groups') + [None]
+
+        return params
 
-        if injected_params:
-            params.update(injected_params)
+    def _apply_public_or_domain_scope(self, params, role_type, domain_id):
+        params['user_domains'] = [domain_id, None]
 
         return params
```

### Comparing `spaceone-core-2.0.84/spaceone/core/locator.py` & `spaceone-core-2.0.9/spaceone/core/locator.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,105 +3,110 @@
 from spaceone.core import config
 from spaceone.core.error import *
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def _get_module(package, target):
-    return __import__(f"{package}.{target}", fromlist=[f"{target}"])
+    return __import__(f'{package}.{target}', fromlist=[f'{target}'])
 
 
 class Locator(object):
     @staticmethod
     def get_service(name_or_object: [str, object], metadata: dict = None, **kwargs):
         metadata = metadata or {}
         package = config.get_package()
 
         if isinstance(name_or_object, str):
-            service_module = _get_module(package, "service")
+            service_module = _get_module(package, 'service')
             return getattr(service_module, name_or_object)(metadata=metadata, **kwargs)
         else:
             return name_or_object(metadata=metadata, **kwargs)
 
     @staticmethod
     def get_manager(name_or_object: [str, object], **kwargs):
         package = config.get_package()
         try:
             if isinstance(name_or_object, str):
-                manager_module = _get_module(package, "manager")
+                manager_module = _get_module(package, 'manager')
                 return getattr(manager_module, name_or_object)(**kwargs)
             else:
                 return name_or_object(**kwargs)
 
         except ERROR_BASE as e:
             raise e
 
         except Exception as e:
-            raise ERROR_LOCATOR(
-                name=name_or_object, reason=e, _meta={"type": "manager"}
-            )
+            raise ERROR_LOCATOR(name=name_or_object, reason=e, _meta={'type': 'manager'})
 
     @staticmethod
     def get_info(name_or_object: [str, object], *args, **kwargs):
         package = config.get_package()
         try:
             if isinstance(name_or_object, str):
-                info_module = _get_module(package, "info")
+                info_module = _get_module(package, 'info')
                 return getattr(info_module, name_or_object)(*args, **kwargs)
             else:
                 return name_or_object(*args, **kwargs)
 
         except ERROR_BASE as e:
             raise e
 
         except Exception as e:
-            raise ERROR_LOCATOR(name=name_or_object, reason=e, _meta={"type": "info"})
+            raise ERROR_LOCATOR(name=name_or_object, reason=e, _meta={'type': 'info'})
 
     @staticmethod
     def get_model(name_or_object: [str, object]):
         package = config.get_package()
         try:
             if isinstance(name_or_object, str):
-                model_module = _get_module(package, "model")
+                model_module = _get_module(package, 'model')
                 return getattr(model_module, name_or_object)
             else:
                 return name_or_object
 
         except ERROR_BASE as e:
             raise e
 
         except Exception as e:
-            raise ERROR_LOCATOR(
-                name=f"{name_or_object} Model", reason=e, _meta={"type": "model"}
-            )
+            raise ERROR_LOCATOR(name=f'{name_or_object} Model', reason=e, _meta={'type': 'model'})
 
     @staticmethod
     def get_connector(name_or_object: [str, object], **kwargs):
         package = config.get_package()
 
         try:
             if isinstance(name_or_object, str):
                 connector_conf = config.get_connector(name_or_object)
-                backend = connector_conf.get("backend")
+                backend = connector_conf.get('backend')
 
                 if backend:
-                    connector_module_path, connector_name = backend.rsplit(":", 1)
-                    connector_module = __import__(
-                        connector_module_path, fromlist=[connector_name]
-                    )
+                    connector_module_path, name_or_object = backend.rsplit('.', 1)
+                    connector_module = __import__(connector_module_path, fromlist=[name_or_object])
                 else:
-                    connector_module = _get_module(package, "connector")
-                    connector_name = name_or_object
+                    connector_module = _get_module(package, 'connector')
 
-                return getattr(connector_module, connector_name)(
-                    connector_name=name_or_object, **kwargs
-                )
+                return getattr(connector_module, name_or_object)(**kwargs)
             else:
                 return name_or_object(**kwargs)
 
         except ERROR_BASE as e:
             raise e
 
         except Exception as e:
-            raise ERROR_LOCATOR(
-                name=name_or_object, reason=e, _meta={"type": "connector"}
-            )
+            raise ERROR_LOCATOR(name=name_or_object, reason=e, _meta={'type': 'connector'})
+
+    @staticmethod
+    def get_manager(name_or_object: [str, object], **kwargs):
+        package = config.get_package()
+        try:
+            if isinstance(name_or_object, str):
+                manager_module = _get_module(package, 'manager')
+                return getattr(manager_module, name_or_object)(**kwargs)
+            else:
+                return name_or_object(**kwargs)
+
+        except ERROR_BASE as e:
+            raise e
+
+        except Exception as e:
+            raise ERROR_LOCATOR(name=name_or_object, reason=e, _meta={'type': 'manager'})
```

### Comparing `spaceone-core-2.0.84/spaceone/core/logger/__init__.py` & `spaceone-core-2.0.9/spaceone/core/logger/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,158 +3,169 @@
 import copy
 
 from spaceone.core import config
 from spaceone.core.error import *
 from spaceone.core.utils import *
 from spaceone.core.logger.filters import *
 
-__all__ = ["set_logger"]
+__all__ = ['set_logger']
 
-DEFAULT_LOGGER = "spaceone"
+DEFAULT_LOGGER = 'spaceone'
 
 HANDLER_DEFAULT_CONSOLE = {
-    "class": "logging.StreamHandler",
-    "formatter": "standard",
-    "filters": ["transaction", "masking", "exclude", "parameter", "traceback"],
+    'class': 'logging.StreamHandler',
+    'formatter': 'standard',
+    'filters': ['transaction', 'masking', 'exclude', 'parameter', 'traceback']
 }
 
 HANDLER_DEFAULT_FILE = {
-    "class": "logging.handlers.RotatingFileHandler",
-    "filename": "",
-    "filters": [
-        "transaction",
-        "masking",
-        "exclude",
-        "error_message",
-        "parameter_log",
-        "message",
-        "traceback_log",
-    ],
-    "formatter": "file",
-    "maxBytes": 10485760,  # 10 MB
-    "backupCount": 10,
+    'class': 'logging.handlers.RotatingFileHandler',
+    'filename': '',
+    'filters': ['transaction', 'masking', 'exclude', 'error_message', 'parameter_log', 'message', 'traceback_log'],
+    'formatter': 'file',
+    'maxBytes': 10485760,  # 10 MB
+    'backupCount': 10
 }
 
 HANDLER_DEFAULT_TMPL = {
-    "console": HANDLER_DEFAULT_CONSOLE,
-    "file": HANDLER_DEFAULT_FILE,
+    'console': HANDLER_DEFAULT_CONSOLE,
+    'file': HANDLER_DEFAULT_FILE
 }
 
 FORMATTER_DEFAULT_TMPL = {
-    "standard": {
-        "format": "%(asctime)s.%(msecs)03dZ [%(levelname)s] %(trace_id)s %(domain_id)s %(audience)s %(role_type)s %(workspace_id)s %(tnx_method)s (%(filename)s:%(lineno)d) %(message)s %(params)s %(traceback)s",
-        "datefmt": "%Y-%m-%dT%H:%M:%S",
-    },
-    "file": {
-        "format": '{"time": "%(asctime)s.%(msecs)03dZ", "level": "%(levelname)s", "peer": "%(peer)s", "trace_id": "%(trace_id)s", "domain_id": "%(domain_id)s", "audience": "%(audience)s", "role_type": "%(role_type)s", "tnx_method": "%(tnx_method)s", "file_name": "%(filename)s", "line": %(lineno)d, "parameter": %(params_log)s, "message": %(msg_dump)s, "error": { "code": "%(error_code)s", "message": "%(error_message)s", "traceback": %(traceback_log)s }}',
-        "datefmt": "%Y-%m-%dT%H:%M:%S",
+    'standard': {
+        'format': '%(asctime)s.%(msecs)03dZ [%(levelname)s] %(trace_id)s %(domain_id)s %(user_id)s %(tnx_method)s (%(filename)s:%(lineno)d) %(message)s %(params)s %(traceback)s',
+        'datefmt': '%Y-%m-%dT%H:%M:%S',
     },
+    'file': {
+        'format': '{"time": "%(asctime)s.%(msecs)03dZ", "level": "%(levelname)s", "peer": "%(peer)s", "trace_id": "%(trace_id)s", "domain_id": "%(domain_id)s", "user_id": "%(user_id)s", "tnx_method": "%(tnx_method)s", "file_name": "%(filename)s", "line": %(lineno)d, "parameter": %(params_log)s, "message": %(msg_dump)s, "error": { "code": "%(error_code)s", "message": "%(error_message)s", "traceback": %(traceback_log)s }}',
+        'datefmt': '%Y-%m-%dT%H:%M:%S',
+    }
 }
 
 FILTER_DEFAULT_TMPL = {
-    "masking": {"()": MaskingFilter, "rules": {}},
-    "transaction": {"()": TransactionFilter},
-    "traceback": {"()": TracebackFilter},
-    "traceback_log": {"()": TracebackLogFilter},
-    "parameter": {"()": ParameterFilter},
-    "parameter_log": {"()": ParameterLogFilter},
-    "error_message": {"()": ErrorFilter},
-    "message": {"()": MessageJsonFilter},
-    "exclude": {
-        "()": ExcludeFilter,
-        "rules": {
-            "tnx_method": [],
-        },
+    'masking': {
+        '()': MaskingFilter,
+        'rules': {}
     },
+    'transaction': {
+        '()': TransactionFilter
+    },
+    'traceback': {
+        '()': TracebackFilter
+    },
+    'traceback_log': {
+        '()': TracebackLogFilter
+    },
+    'parameter': {
+        '()': ParameterFilter
+    },
+    'parameter_log': {
+        '()': ParameterLogFilter
+    },
+    'error_message': {
+        '()': ErrorFilter
+    },
+    'message': {
+        '()': MessageJsonFilter
+    },
+    'exclude': {
+        '()': ExcludeFilter,
+        'rules': {
+            'tnx_method': [],
+        }
+    }
 }
 
 _LOGGER = {
-    "version": 1,
-    "formatters": {},
-    "filters": {},
-    "handlers": {"console": HANDLER_DEFAULT_CONSOLE},
-    "loggers": {},
+    'version': 1,
+    'formatters': {},
+    'filters': {},
+    'handlers': {
+        'console': HANDLER_DEFAULT_CONSOLE
+    },
+    'loggers': {}
 }
 
-LOGGER_DEFAULT_TMPL = {"level": "DEBUG", "propagate": True, "handlers": ["console"]}
+LOGGER_DEFAULT_TMPL = {
+    'level': 'DEBUG',
+    'propagate': True,
+    'handlers': ['console']
+}
 
 
 def set_logger(transaction=None):
     _set_config(transaction)
     logging.config.dictConfig(_LOGGER)
 
 
 def _set_default_logger(default_logger):
-    _LOGGER["loggers"] = {default_logger: LOGGER_DEFAULT_TMPL}
-    _LOGGER["formatters"] = FORMATTER_DEFAULT_TMPL
+    _LOGGER['loggers'] = {default_logger: LOGGER_DEFAULT_TMPL}
+    _LOGGER['formatters'] = FORMATTER_DEFAULT_TMPL
 
 
 def _set_loggers(loggers):
     for _logger in loggers:
-        _LOGGER["loggers"][_logger] = deep_merge(
-            loggers[_logger], copy.deepcopy(LOGGER_DEFAULT_TMPL)
-        )
+        _LOGGER['loggers'][_logger] = deep_merge(loggers[_logger], copy.deepcopy(LOGGER_DEFAULT_TMPL))
 
 
 def _set_transaction_filter(transaction):
     if transaction:
-        _LOGGER["filters"]["transaction"]["transaction"] = transaction
+        _LOGGER['filters']['transaction']['transaction'] = transaction
 
 
 def _set_handlers(handlers):
     for _handler in handlers:
         _default = copy.deepcopy(HANDLER_DEFAULT_TMPL)
 
-        if "type" in handlers[_handler]:
-            if handlers[_handler]["type"] not in HANDLER_DEFAULT_TMPL:
-                raise ERROR_LOG_CONFIG(reason="Logger handler type is not supported")
+        if 'type' in handlers[_handler]:
+            if handlers[_handler]['type'] not in HANDLER_DEFAULT_TMPL:
+                raise ERROR_LOG_CONFIG(reason='Logger handler type is not supported')
 
-            _default = copy.deepcopy(HANDLER_DEFAULT_TMPL[handlers[_handler]["type"]])
+            _default = copy.deepcopy(HANDLER_DEFAULT_TMPL[handlers[_handler]['type']])
 
         _default = deep_merge(handlers[_handler], _default)
 
-        if "type" in _default:
-            del _default["type"]
+        if 'type' in _default:
+            del _default['type']
 
-        _LOGGER["handlers"][_handler] = _default
+        _LOGGER['handlers'][_handler] = _default
 
 
 def _set_formatters(formatters):
     for _formatter in formatters:
         _default = {}
 
-        if "type" in formatters[_formatter]:
-            if formatters[_formatter]["type"] not in FORMATTER_DEFAULT_TMPL:
-                raise ERROR_LOG_CONFIG(reason="Logger formatter type is not supported")
+        if 'type' in formatters[_formatter]:
+            if formatters[_formatter]['type'] not in FORMATTER_DEFAULT_TMPL:
+                raise ERROR_LOG_CONFIG(reason='Logger formatter type is not supported')
 
-            _default = copy.deepcopy(
-                FORMATTER_DEFAULT_TMPL[formatters[_formatter]["type"]]
-            )
+            _default = copy.deepcopy(FORMATTER_DEFAULT_TMPL[formatters[_formatter]['type']])
 
-        _default = deep_merge(formatters[_formatter]["args"], _default)
+        _default = deep_merge(formatters[_formatter]['args'], _default)
 
-        if "type" in _default:
-            del _default["type"]
+        if 'type' in _default:
+            del _default['type']
 
-        _LOGGER["formatters"][_formatter] = _default
+        _LOGGER['formatters'][_formatter] = _default
 
 
 def _set_filters(filters):
-    _LOGGER["filters"] = deep_merge(filters, copy.deepcopy(FILTER_DEFAULT_TMPL))
+    _LOGGER['filters'] = deep_merge(filters, copy.deepcopy(FILTER_DEFAULT_TMPL))
 
 
 def _set_config(transaction):
-    global_log_conf = config.get_global("LOG", {})
+    global_log_conf = config.get_global('LOG', {})
 
     _set_default_logger(DEFAULT_LOGGER)
 
-    if "loggers" in global_log_conf:
-        _set_loggers(global_log_conf["loggers"])
+    if 'loggers' in global_log_conf:
+        _set_loggers(global_log_conf['loggers'])
 
-    if "handlers" in global_log_conf:
-        _set_handlers(global_log_conf["handlers"])
+    if 'handlers' in global_log_conf:
+        _set_handlers(global_log_conf['handlers'])
 
-    if "formatters" in global_log_conf:
-        _set_formatters(global_log_conf["formatters"])
+    if 'formatters' in global_log_conf:
+        _set_formatters(global_log_conf['formatters'])
 
-    _set_filters(global_log_conf.get("filters", {}))
+    _set_filters(global_log_conf.get('filters', {}))
     _set_transaction_filter(transaction)
```

### Comparing `spaceone-core-2.0.84/spaceone/core/logger/filters/masking.py` & `spaceone-core-2.0.9/spaceone/core/logger/filters/masking.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,39 @@
+# -*- coding: utf-8 -*-
 import logging
 import copy
 import json
 from fnmatch import fnmatch
 
 
 class MaskingFilter(logging.Filter):
     def __init__(self, rules):
         self.rules = rules
 
     def filter(self, record):
-        tnx_method = getattr(record, "tnx_method", None)
-        parameter = getattr(record, "parameter", None)
+        tnx_method = getattr(record, 'tnx_method', None)
+        parameter = getattr(record, 'parameter', None)
 
         if tnx_method and parameter:
             record.parameter = self._check_masking(tnx_method, parameter)
         return True
 
     def _check_masking(self, tnx_method, params):
         masking_parameter = copy.deepcopy(params)
 
         if tnx_method in self.rules:
             return self._masking(masking_parameter, self.rules[tnx_method])
 
-        """
+        '''
         masking_parameter = copy.deepcopy(params)
         
         for _rule in self.rules:
             if fnmatch(tnx_method, _rule):
                 masking_parameter = self._masking(masking_parameter, self.rules[_rule])
-        """
+        '''
         return masking_parameter
 
     @staticmethod
     def _masking(parameter, patterns):
         for _p in parameter:
             if _p in patterns:
                 parameter[_p] = "********"
```

### Comparing `spaceone-core-2.0.84/spaceone/core/logger/filters/parameter.py` & `spaceone-core-2.0.9/spaceone/core/logger/filters/parameter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,27 @@
+# -*- coding: utf-8 -*-
 import logging
 import json
 
 
 class ParameterFilter(logging.Filter):
     def filter(self, record):
-        params = getattr(record, "parameter", None)
+        params = getattr(record, 'parameter', None)
 
         if params is None:
-            record.params = ""
+            record.params = ''
         else:
             record.params = json.dumps(params)
 
         return True
 
 
 class ParameterLogFilter(logging.Filter):
     def filter(self, record):
-        params = getattr(record, "parameter", None)
+        params = getattr(record, 'parameter', None)
 
-        if params is None or params == "":
-            record.params_log = "{}"
+        if params is None or params == '':
+            record.params_log = '{}'
         else:
             record.params_log = json.dumps(params)
 
         return True
```

### Comparing `spaceone-core-2.0.84/spaceone/core/logger/filters/traceback.py` & `spaceone-core-2.0.9/spaceone/core/logger/filters/traceback.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
+# -*- coding: utf-8 -*-
 import logging
 
 
 class TracebackFilter(logging.Filter):
     def filter(self, record):
-        _traceback = getattr(record, "traceback", None)
+        _traceback = getattr(record, 'traceback', None)
 
         if _traceback is None or _traceback == "":
-            record.traceback = ""
+            record.traceback = ''
         else:
-            record.traceback = (
-                _traceback.replace("\\n", "\n").replace('\\"', '"').replace("\\t", "\t")
-            )
+            record.traceback = _traceback.replace('\\n', '\n').replace('\\"', '\"').replace('\\t', '\t')
 
         return True
 
 
 class TracebackLogFilter(logging.Filter):
     def filter(self, record):
-        _traceback = getattr(record, "traceback", None)
+        _traceback = getattr(record, 'traceback', None)
 
         if _traceback is None or _traceback == "":
             record.traceback_log = '""'
         else:
             record.traceback_log = _traceback
 
-        return True
+        return True
```

### Comparing `spaceone-core-2.0.84/spaceone/core/model/mongo_model/__init__.py` & `spaceone-core-2.0.9/spaceone/core/model/mongo_model/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,197 +1,201 @@
 import bson
 import re
 import logging
 import certifi
 import copy
 from datetime import datetime, date
 from dateutil.relativedelta import relativedelta
-from functools import reduce, partial
-from mongoengine import (
-    EmbeddedDocumentField,
-    EmbeddedDocument,
-    Document,
-    QuerySet,
-    register_connection,
-)
+from functools import reduce
+from mongoengine import EmbeddedDocumentField, EmbeddedDocument, Document, QuerySet, register_connection
 from mongoengine.fields import DateField, DateTimeField, ComplexDateTimeField
 from pymongo import ReadPreference
 from mongoengine.errors import *
 from spaceone.core import config
 from spaceone.core import utils
 from spaceone.core.error import *
 from spaceone.core.model.base_model import BaseModel
 from spaceone.core.model.mongo_model.filter_operator import FILTER_OPERATORS
-from spaceone.core.model.mongo_model.stat_operator import (
-    STAT_GROUP_OPERATORS,
-    STAT_PROJECT_OPERATORS,
-)
+from spaceone.core.model.mongo_model.stat_operator import STAT_GROUP_OPERATORS, STAT_PROJECT_OPERATORS
 
-_REFERENCE_ERROR_FORMAT = r"Could not delete document \((\w+)\.\w+ refers to it\)"
+_REFERENCE_ERROR_FORMAT = r'Could not delete document \((\w+)\.\w+ refers to it\)'
 _MONGO_INIT_MODELS = []
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def _raise_reference_error(class_name, message):
     m = re.findall(_REFERENCE_ERROR_FORMAT, message)
     if len(m) > 0:
         raise ERROR_EXIST_RESOURCE(parent=class_name, child=m[0])
 
 
 class MongoCustomQuerySet(QuerySet):
+
     def last(self):
-        return self.order_by("-id").first()
+        return self.order_by('-id').first()
 
     def update(self, *args, **kwargs):
         if len(args) > 0 and isinstance(args[0], dict):
             kwargs.update(args[0])
         super().update(**kwargs)
 
     def increment(self, key, amount=1):
-        key = key.replace(".", "__")
-        inc_data = {f"inc__{key}": amount}
+        key = key.replace('.', '__')
+        inc_data = {
+            f'inc__{key}': amount
+        }
 
         super().update(**inc_data)
 
     def decrement(self, key, amount=1):
-        key = key.replace(".", "__")
-        dec_data = {f"dec__{key}": amount}
+        key = key.replace('.', '__')
+        dec_data = {
+            f'dec__{key}': amount
+        }
 
         super().update(**dec_data)
 
     def set_data(self, key, data):
-        key = key.replace(".", "__")
-        set_data = {f"set__{key}": data}
+        key = key.replace('.', '__')
+        set_data = {
+            f'set__{key}': data
+        }
 
         super().update(**set_data)
 
     def unset_data(self, *keys):
         unset_data = {}
 
         for key in keys:
-            key = key.replace(".", "__")
-            unset_data[f"unset__{key}"] = 1
+            key = key.replace('.', '__')
+            unset_data[f'unset__{key}'] = 1
 
         super().update(**unset_data)
 
     def append(self, key, data):
-        key = key.replace(".", "__")
-        append_data = {f"push__{key}": data}
+        key = key.replace('.', '__')
+        append_data = {
+            f'push__{key}': data
+        }
 
         super().update(**append_data)
 
     def remove(self, key, data):
-        key = key.replace(".", "__")
-        remove_data = {f"pull__{key}": data}
+        key = key.replace('.', '__')
+        remove_data = {
+            f'pull__{key}': data
+        }
         super().update(**remove_data)
 
 
 class MongoModel(Document, BaseModel):
+
     auto_create_index = True
     meta = {
-        "abstract": True,
-        "queryset_class": MongoCustomQuerySet,
-        "auto_create_index": False,
+        'abstract': True,
+        'queryset_class': MongoCustomQuerySet,
+        'auto_create_index': False
     }
 
     @classmethod
-    def init(cls, create_index: bool = True) -> None:
+    def init(cls):
         global_conf = config.get_global()
-        databases = global_conf.get("DATABASES", {})
-        db_name_prefix = global_conf.get("DATABASE_NAME_PREFIX", "")
+        databases = global_conf.get('DATABASES', {})
+        db_name_prefix = global_conf.get('DATABASE_NAME_PREFIX', '')
 
-        if not global_conf.get("MOCK_MODE", False):
+        if not global_conf.get('MOCK_MODE', False):
             for alias, db_conf in databases.items():
                 is_connect = cls._connect(alias, db_conf, db_name_prefix)
                 if is_connect:
-                    package_path = config.get_package()
-                    model_path = config.get_global("DATABASE_MODEL_PATH", "model")
-                    __import__(f"{package_path}.{model_path}", fromlist=["*"])
-
-                    for model in cls.__subclasses__():
-                        if create_index:
+                    for model in cls.get_inherited_models():
+                        if (model != cls
+                                and issubclass(model, MongoModel)
+                                and model not in _MONGO_INIT_MODELS):
+                            model.auto_create_index = global_conf.get('DATABASE_AUTO_CREATE_INDEX', True)
                             model._create_index()
-                        model._load_default_meta()
+                            model._load_default_meta()
+
+                            _MONGO_INIT_MODELS.append(model)
 
     @classmethod
-    def _connect(cls, alias: str, db_conf: dict, db_name_prefix: str) -> bool:
+    def _connect(cls, alias: str, db_conf: dict, db_name_prefix: str):
         is_connect = False
         db_conf = copy.deepcopy(db_conf)
-        engine = db_conf.get("engine")
-        host = db_conf.get("host")
-        db = db_conf.get("db")
-        username = db_conf.get("username")
+        engine = db_conf.get('engine')
+        host = db_conf.get('host')
+        db = db_conf.get('db')
+        username = db_conf.get('username')
 
         if engine is None:
             raise ERROR_DB_ENGINE_UNDEFINE(alias=alias)
-        del db_conf["engine"]
+        del db_conf['engine']
 
-        if engine == "MongoModel":
+        if engine == 'MongoModel':
             if host and db and username:
-                if "read_preference" in db_conf:
-                    read_preference = getattr(
-                        ReadPreference, db_conf["read_preference"], None
-                    )
+                if 'read_preference' in db_conf:
+                    read_preference = getattr(ReadPreference, db_conf['read_preference'], None)
                     if read_preference:
-                        db_conf["read_preference"] = read_preference
+                        db_conf['read_preference'] = read_preference
                     else:
-                        del db_conf["read_preference"]
+                        del db_conf['read_preference']
 
-                db_name: str = db_conf.get("db", "")
-                db_conf["db"] = f"{db_name_prefix}{db_name}"
+                db_name: str = db_conf.get('db', '')
+                db_conf['db'] = f'{db_name_prefix}{db_name}'
 
-                host: str = str(db_conf.get("host", "")).strip()
-                if host.startswith("mongodb+srv://"):
-                    db_conf["tlsCAFile"] = certifi.where()
+                host: str = str(db_conf.get('host', '')).strip()
+                if host.startswith('mongodb+srv://'):
+                    db_conf['tlsCAFile'] = certifi.where()
 
                 register_connection(alias, **db_conf)
                 is_connect = True
-                _LOGGER.debug(f"Create MongoDB Connection: {alias}")
+                _LOGGER.debug(f'Create MongoDB Connection: {alias}')
+            else:
+                _LOGGER.warning(f'MongoDB is not configured. (alias = {alias})')
 
         return is_connect
 
     @classmethod
     def _load_default_meta(cls):
-        cls._meta["datetime_fields"] = []
+        cls._meta['datetime_fields'] = []
         for name, field in cls._fields.items():
             if isinstance(field, DateField):
-                cls._meta["datetime_fields"].append(name)
+                cls._meta['datetime_fields'].append(name)
             elif isinstance(field, DateTimeField):
-                cls._meta["datetime_fields"].append(name)
+                cls._meta['datetime_fields'].append(name)
             elif isinstance(field, ComplexDateTimeField):
-                cls._meta["datetime_fields"].append(name)
+                cls._meta['datetime_fields'].append(name)
 
     @classmethod
-    def _create_index(cls) -> None:
+    def _create_index(cls):
         if cls.auto_create_index:
-            indexes = cls._meta.get("indexes", [])
-            unique_fields = cls._get_unique_fields()
+            indexes = cls._meta.get('indexes', [])
 
-            if len(indexes) > 0 or len(unique_fields) > 0:
-                total_index_count = len(indexes) + len(unique_fields)
+            if len(indexes) > 0:
+                _LOGGER.debug(f'Create MongoDB Indexes ({cls.__name__} Model: {len(indexes)} Indexes)')
 
-                _LOGGER.debug(
-                    f"Create MongoDB Indexes ({cls.__name__} Model: {total_index_count} Indexes)"
-                )
+                unique_fields = cls._get_unique_fields()
 
                 for unique_field in unique_fields:
                     try:
-                        cls.create_index({"fields": unique_field, "unique": True})
+                        cls.create_index({
+                            'fields': unique_field,
+                            'unique': True
+                        })
 
                     except Exception as e:
-                        _LOGGER.error(f"Unique Index Creation Failure: {e}")
+                        _LOGGER.error(f'Unique Index Creation Failure: {e}')
 
                 for index in indexes:
                     try:
                         cls.create_index(index)
 
                     except Exception as e:
-                        if e.code != 85:  # 85: IndexOptionsConflict
-                            _LOGGER.error(f"Index Creation Failure: {e}")
+                        if e.code != 85: # 85: IndexOptionsConflict
+                            _LOGGER.error(f'Index Creation Failure: {e}')
 
     @classmethod
     def _get_unique_fields(cls):
         unique_fields = []
         for name, field in cls._fields.items():
             if field.unique:
                 if isinstance(field.unique_with, str):
@@ -200,170 +204,154 @@
                     unique_fields.append([field.name] + field.unique_with)
                 else:
                     unique_fields.append([field.name])
 
         return unique_fields
 
     @classmethod
-    def _trim_value(cls, value: any) -> any:
-        if isinstance(value, str):
-            return value.strip()
-        elif isinstance(value, dict):
-            changed_value = {}
-            for k, v in value.items():
-                if isinstance(k, str):
-                    k = k.strip()
-                if isinstance(v, str):
-                    v = v.strip()
-                changed_value[k] = cls._trim_value(v)
-
-            return changed_value
-        else:
-            return value
-
-    @classmethod
     def create(cls, data):
         create_data = {}
 
         for name, field in cls._fields.items():
             if name in data:
                 create_data[name] = data[name]
             else:
-                generate_id = getattr(field, "generate_id", None)
+                generate_id = getattr(field, 'generate_id', None)
                 if generate_id:
                     create_data[name] = utils.generate_id(generate_id)
 
-                if getattr(field, "auto_now", False):
+                if getattr(field, 'auto_now', False):
                     create_data[name] = datetime.utcnow()
-                elif getattr(field, "auto_now_add", False):
+                elif getattr(field, 'auto_now_add', False):
                     create_data[name] = datetime.utcnow()
 
         for unique_field in cls._get_unique_fields():
             conditions = {}
             for f in unique_field:
                 conditions[f] = data.get(f)
             vos = cls.filter(**conditions)
             if vos.count() > 0:
                 raise ERROR_SAVE_UNIQUE_VALUES(keys=unique_field)
 
-        for key, value in create_data.items():
-            create_data[key] = cls._trim_value(value)
-
         try:
             new_vo = cls(**create_data).save()
         except Exception as e:
             raise ERROR_DB_QUERY(reason=e)
 
         return new_vo
 
     def update(self, data):
         updatable_fields = self._meta.get(
-            "updatable_fields",
-            list(
+            'updatable_fields', list(
                 filter(
-                    lambda x: x != self._meta.get("id_field", "id"), self._fields.keys()
+                    lambda x: x != self._meta.get('id_field', 'id'), self._fields.keys()
                 )
-            ),
+            )
         )
 
         for name, field in self._fields.items():
-            if getattr(field, "auto_now", False):
+            if getattr(field, 'auto_now', False):
                 if name not in data.keys():
                     data[name] = datetime.utcnow()
 
         for unique_field in self._get_unique_fields():
-            conditions = {"pk__ne": self.pk}
+            conditions = {'pk__ne': self.pk}
             for f in unique_field:
                 conditions[f] = data.get(f)
 
             vos = self.filter(**conditions)
             if vos.count() > 0:
                 raise ERROR_SAVE_UNIQUE_VALUES(keys=unique_field)
 
         for key in list(data.keys()):
             if key not in updatable_fields:
                 del data[key]
 
         if data != {}:
-            for key, value in data.items():
-                data[key] = self._trim_value(value)
-
             try:
                 super().update(**data)
                 self.reload()
             except Exception as e:
                 raise ERROR_DB_QUERY(reason=e)
 
         return self
 
-    def delete(self, *args):
+    def delete(self):
         try:
-            super().delete(*args)
+            super().delete()
         except OperationError as e:
             _raise_reference_error(self.__class__.__name__, str(e))
             raise ERROR_DB_QUERY(reason=e)
         except Exception as e:
             raise ERROR_DB_QUERY(reason=e)
 
     def terminate(self):
         super().delete()
 
     def increment(self, key, amount=1):
-        key = key.replace(".", "__")
-        inc_data = {f"inc__{key}": amount}
+        key = key.replace('.', '__')
+        inc_data = {
+            f'inc__{key}': amount
+        }
 
         super().update(**inc_data)
         self.reload()
         return self
 
     def decrement(self, key, amount=1):
-        key = key.replace(".", "__")
-        dec_data = {f"dec__{key}": amount}
+        key = key.replace('.', '__')
+        dec_data = {
+            f'dec__{key}': amount
+        }
 
         super().update(**dec_data)
         self.reload()
         return self
 
     def set_data(self, key, data):
-        key = key.replace(".", "__")
-        set_data = {f"set__{key}": data}
+        key = key.replace('.', '__')
+        set_data = {
+            f'set__{key}': data
+        }
 
         super().update(**set_data)
         self.reload()
         return self
 
     def unset_data(self, *keys):
         unset_data = {}
 
         for key in keys:
-            key = key.replace(".", "__")
-            unset_data[f"unset__{key}"] = 1
+            key = key.replace('.', '__')
+            unset_data[f'unset__{key}'] = 1
 
         super().update(**unset_data)
         self.reload()
         return self
 
-    def append(self, key, data) -> Document:
-        key = key.replace(".", "__")
+    def append(self, key, data):
+        key = key.replace('.', '__')
         append_data = {}
 
-        field = getattr(self._fields.get(key, {}), "field", None)
+        field = getattr(self._fields.get(key, {}), 'field', None)
         if field and isinstance(field, EmbeddedDocumentField):
             reference_model = field.document_type_obj
-            append_data[f"push__{key}"] = reference_model(**data)
+            append_data[f'push__{key}'] = reference_model(**data)
         else:
-            append_data[f"push__{key}"] = data
+            append_data[f'push__{key}'] = data
 
         super().update(**append_data)
         self.reload()
         return self
 
     def remove(self, key, data):
-        key = key.replace(".", "__")
-        remove_data = {f"pull__{key}": data}
+        key = key.replace('.', '__')
+        remove_data = {
+            f'pull__{key}': data
+        }
         super().update(**remove_data)
         self.reload()
         return self
 
     @classmethod
     def get(cls, only=None, **conditions):
         vos = cls.filter(**conditions)
@@ -384,167 +372,133 @@
         return vos.first()
 
     @classmethod
     def filter(cls, **conditions):
         change_conditions = {}
         for key, value in conditions.items():
             if isinstance(value, list):
-                change_conditions[f"{key}__in"] = value
+                change_conditions[f'{key}__in'] = value
             else:
                 change_conditions[key] = value
 
         return cls.objects.filter(**change_conditions)
 
-    def to_dict(self) -> dict:
-        return dict(self.to_mongo())
+    def to_dict(self):
+        return self.to_mongo()
 
     @classmethod
     def _get_target_objects(cls, target):
         if target:
             read_preference = getattr(ReadPreference, target, None)
             if read_preference:
                 return cls.objects.read_preference(read_preference)
 
         return cls.objects
 
     @staticmethod
     def _check_operator_value(is_multiple, operator, value, condition):
         if is_multiple:
             if not isinstance(value, list):
-                raise ERROR_OPERATOR_LIST_VALUE_TYPE(
-                    operator=operator, condition=condition
-                )
+                raise ERROR_OPERATOR_LIST_VALUE_TYPE(operator=operator, condition=condition)
 
         else:
             if isinstance(value, list):
                 raise ERROR_OPERATOR_VALUE_TYPE(operator=operator, condition=condition)
 
     @classmethod
     def _check_reference_field(cls, key):
-        ref_keys = cls._meta.get("reference_query_keys", {}).keys()
+        ref_keys = cls._meta.get('reference_query_keys', {}).keys()
         if key in ref_keys:
             return False
         else:
             return True
 
     @classmethod
     def _get_reference_model(cls, key):
-        for ref_key, ref_conf in cls._meta.get("reference_query_keys", {}).items():
-            if key.startswith(ref_key) and key[len(ref_key)] == ".":
+        for ref_key, ref_conf in cls._meta.get('reference_query_keys', {}).items():
+            if key.startswith(ref_key) and key[len(ref_key)] == '.':
                 if isinstance(ref_conf, dict):
-                    ref_model = ref_conf.get("model")
-                    foreign_key = ref_conf.get("foreign_key")
+                    ref_model = ref_conf.get('model')
+                    foreign_key = ref_conf.get('foreign_key')
                 else:
                     ref_model = ref_conf
                     foreign_key = None
 
-                ref_query_key = key.replace(f"{ref_key}.", "")
-                if ref_model == "self":
+                ref_query_key = key.replace(f'{ref_key}.', '')
+                if ref_model == 'self':
                     ref_model = cls
 
                 return ref_model, ref_key, ref_query_key, foreign_key
 
         return None, None, None, None
 
     @classmethod
-    def _change_reference_condition(cls, key, value, operator, reference_filter=None):
+    def _change_reference_condition(cls, key, value, operator):
         ref_model, ref_key, ref_query_key, foreign_key = cls._get_reference_model(key)
         if ref_model:
             if value is None:
                 return ref_key, value, operator
             else:
-                if operator == "not":
-                    _filter = [{"k": ref_query_key, "v": value, "o": "eq"}]
-                elif operator == "not_in":
-                    _filter = [{"k": ref_query_key, "v": value, "o": "in"}]
-                else:
-                    _filter = [{"k": ref_query_key, "v": value, "o": operator}]
-                if reference_filter:
-                    for key, value in reference_filter.items():
-                        if value:
-                            _filter.append({"k": key, "v": value, "o": "eq"})
-
-                ref_vos, total_count = ref_model.query(filter=_filter)
+                ref_vos, total_count = ref_model.query(
+                    filter=[{'k': ref_query_key, 'v': value, 'o': operator}])
 
                 if foreign_key:
                     ref_values = []
                     for ref_vo in ref_vos:
                         ref_value = getattr(ref_vo, foreign_key)
                         if ref_value:
                             ref_values.append(ref_value)
                 else:
                     ref_values = list(ref_vos)
-
-                if operator in ["not", "not_in"]:
-                    return ref_key, ref_values, "not_in"
-                else:
-                    return ref_key, ref_values, "in"
+                return ref_key, ref_values, 'in'
 
         else:
             return key, value, operator
 
     @classmethod
-    def _make_condition(cls, condition, reference_filter=None):
-        key = condition.get("key", condition.get("k"))
-        value = condition.get("value", condition.get("v"))
-        operator = condition.get("operator", condition.get("o"))
-        change_query_keys = cls._meta.get("change_query_keys", {})
+    def _make_condition(cls, condition):
+        key = condition.get('key', condition.get('k'))
+        value = condition.get('value', condition.get('v'))
+        operator = condition.get('operator', condition.get('o'))
+        change_query_keys = cls._meta.get('change_query_keys', {})
 
         if operator not in FILTER_OPERATORS:
-            raise ERROR_DB_QUERY(
-                reason=f"Filter operator is not supported. (operator = "
-                f"{FILTER_OPERATORS.keys()})"
-            )
+            raise ERROR_DB_QUERY(reason=f'Filter operator is not supported. (operator = '
+                                        f'{FILTER_OPERATORS.keys()})')
 
         resolver, mongo_operator, is_multiple = FILTER_OPERATORS.get(operator)
 
         cls._check_operator_value(is_multiple, operator, value, condition)
 
         if key and operator:
             if key in change_query_keys:
                 key = change_query_keys[key]
 
-            if operator not in ["regex", "regex_in"]:
+            if operator not in ['regex', 'regex_in']:
                 if cls._check_reference_field(key):
-                    key, value, operator = cls._change_reference_condition(
-                        key, value, operator, reference_filter
-                    )
+                    key, value, operator = cls._change_reference_condition(key, value, operator)
 
                     resolver, mongo_operator, is_multiple = FILTER_OPERATORS[operator]
 
-                key = key.replace(".", "__")
+                key = key.replace('.', '__')
 
             return resolver(key, value, mongo_operator, is_multiple)
         else:
-            raise ERROR_DB_QUERY(
-                reason="Filter condition should have key, value and operator."
-            )
+            raise ERROR_DB_QUERY(reason='Filter condition should have key, value and operator.')
 
     @classmethod
-    def _make_filter(cls, filter, filter_or, reference_filter):
+    def _make_filter(cls, filter, filter_or):
         _filter = None
         _filter_or = None
 
         if len(filter) > 0:
-            _filter = reduce(
-                lambda x, y: x & y,
-                map(
-                    partial(cls._make_condition, reference_filter=reference_filter),
-                    filter,
-                ),
-            )
+            _filter = reduce(lambda x, y: x & y, map(cls._make_condition, filter))
 
         if len(filter_or) > 0:
-            _filter_or = reduce(
-                lambda x, y: x | y,
-                map(
-                    partial(cls._make_condition, reference_filter=reference_filter),
-                    filter_or,
-                ),
-            )
+            _filter_or = reduce(lambda x, y: x | y, map(cls._make_condition, filter_or))
 
         if _filter and _filter_or:
             _filter = _filter & _filter_or
         else:
             _filter = _filter or _filter_or
 
         return _filter
@@ -553,223 +507,128 @@
     def _remove_duplicate_only_keys(cls, only):
         changed_only = []
         duplicated_only = []
         for key in only:
             exists = False
 
             for changed_key in changed_only:
-                if key == changed_key or key.startswith(f"{changed_key}."):
+                if key == changed_key or key.startswith(f'{changed_key}.'):
                     exists = True
-                elif changed_key.startswith(f"{key}."):
+                elif changed_key.startswith(f'{key}.'):
                     duplicated_only.append(changed_key)
 
             if exists is False:
                 changed_only.append(key)
 
         if len(duplicated_only) > 0:
             changed_only = list(set(changed_only) - set(duplicated_only))
 
         return changed_only
 
-    @staticmethod
-    def _make_unwind_project_stage(only: list):
-        project_fields = []
-        for key in only:
-            project_fields.append(
-                {
-                    "key": key,
-                    "name": key,
-                }
-            )
-
-        return {
-            "project": {
-                "exclude_keys": False,
-                "only_keys": False,
-                "fields": project_fields,
-            }
-        }
-
     @classmethod
-    def _stat_with_unwind(
-        cls,
-        unwind: list,
-        only: list = None,
-        filter: list = None,
-        filter_or: list = None,
-        sort: list = None,
-        page: dict = None,
-        target: str = None,
-    ):
-        if only is None:
-            raise ERROR_DB_QUERY(reason="unwind option requires only option.")
-
-        if not isinstance(unwind, dict):
-            raise ERROR_DB_QUERY(reason="unwind option should be dict type.")
-
-        if "path" not in unwind:
-            raise ERROR_DB_QUERY(reason="unwind option should have path key.")
-
-        unwind_path = unwind["path"]
-        unwind_filter = unwind.get("filter")
+    def query(cls, *args, only=None, exclude=None, all_fields=False, filter=None, filter_or=None,
+              sort=None, page=None, minimal=False, count_only=False, target=None, **kwargs):
 
-        aggregate = [{"unwind": {"path": unwind_path}}]
+        if filter is None:
+            filter = []
 
-        if unwind_filter:
-            aggregate.append({"match": {"filter": unwind_filter}})
+        if filter_or is None:
+            filter_or = []
 
-        # Add project stage
-        project_fields = []
-        for key in only:
-            project_fields.append(
-                {
-                    "key": key,
-                    "name": key,
-                }
-            )
-
-        aggregate.append(
-            {
-                "project": {
-                    "exclude_keys": True,
-                    "only_keys": True,
-                    "fields": project_fields,
-                }
-            }
-        )
-
-        # Add sort stage
-        if sort:
-            aggregate.append({"sort": sort})
-
-        response = cls.stat(
-            aggregate=aggregate,
-            filter=filter,
-            filter_or=filter_or,
-            page=page,
-            tageet=target,
-            allow_disk_use=True,
-        )
-
-        try:
-            vos = []
-            total_count = response.get("total_count", 0)
-            for result in response.get("results", []):
-                unwind_data = utils.get_dict_value(result, unwind_path)
-                result = utils.change_dict_value(result, unwind_path, [unwind_data])
+        if sort is None:
+            sort = {}
 
-                vo = cls(**result)
-                vos.append(vo)
-        except Exception as e:
-            raise ERROR_DB_QUERY(reason=f"Failed to convert unwind result: {e}")
-
-        return vos, total_count
+        if page is None:
+            page = {}
 
-    @classmethod
-    def query(
-        cls,
-        *args,
-        only=None,
-        exclude=None,
-        filter=None,
-        filter_or=None,
-        sort=None,
-        page=None,
-        minimal=False,
-        count_only=False,
-        unwind=None,
-        reference_filter=None,
-        target=None,
-        **kwargs,
-    ):
-        filter = filter or []
-        filter_or = filter_or or []
-        sort = sort or []
-        page = page or {}
-
-        if unwind:
-            return cls._stat_with_unwind(
-                unwind, only, filter, filter_or, sort, page, target
-            )
-
-        else:
-            _order_by = []
-            minimal_fields = cls._meta.get("minimal_fields")
+        _order_by = []
+        minimal_fields = cls._meta.get('minimal_fields')
 
-            _filter = cls._make_filter(filter, filter_or, reference_filter)
+        _filter = cls._make_filter(filter, filter_or)
 
-            for sort_option in sort:
-                if sort_option.get("desc", False):
-                    _order_by.append(f'-{sort_option["key"]}')
+        if 'key' in sort:
+            if sort.get('desc', False):
+                _order_by.append(f'-{sort["key"]}')
+            else:
+                _order_by.append(f'{sort["key"]}')
+        elif 'keys' in sort:
+            for s in sort['keys']:
+                if s.get('desc', False):
+                    _order_by.append(f'-{s["key"]}')
                 else:
-                    _order_by.append(f'{sort_option["key"]}')
+                    _order_by.append(f'{s["key"]}')
 
-            try:
-                vos = cls._get_target_objects(target).filter(_filter)
+        try:
+            vos = cls._get_target_objects(target).filter(_filter)
+
+            if len(_order_by) > 0:
+                vos = vos.order_by(*_order_by)
 
+            if only:
                 if len(_order_by) > 0:
-                    vos = vos.order_by(*_order_by)
+                    ordering = _order_by
+                else:
+                    ordering = cls._meta.get('ordering')
 
-                if only:
-                    if len(_order_by) > 0:
-                        ordering = _order_by
-                    else:
-                        ordering = cls._meta.get("ordering")
+                for key in ordering:
+                    if key.startswith('+') or key.startswith('-'):
+                        key = key[1:]
+                    if key not in only:
+                        only.append(key)
 
-                    for key in ordering:
-                        if key.startswith("+") or key.startswith("-"):
-                            key = key[1:]
-                        if key not in only:
-                            only.append(key)
+                only = cls._remove_duplicate_only_keys(only)
+                vos = vos.only(*only)
 
-                    only = cls._remove_duplicate_only_keys(only)
-                    vos = vos.only(*only)
+            if exclude:
+                vos = vos.exclude(*exclude)
 
-                if exclude:
-                    vos = vos.exclude(*exclude)
+            if minimal and minimal_fields:
+                vos = vos.only(*minimal_fields)
 
-                if minimal and minimal_fields:
-                    vos = vos.only(*minimal_fields)
+            if all_fields:
+                vos = vos.all_fields()
 
-                total_count = vos.count()
+            total_count = vos.count()
 
-                if count_only:
-                    vos = []
+            if count_only:
+                vos = []
 
-                else:
-                    if "limit" in page and page["limit"] > 0:
-                        start = page.get("start", 1)
-                        if start < 1:
-                            start = 1
+            else:
+                if 'limit' in page and page['limit'] > 0:
+                    start = page.get('start', 1)
+                    if start < 1:
+                        start = 1
 
-                        vos = vos[start - 1 : start + page["limit"] - 1]
+                    vos = vos[start - 1:start + page['limit'] - 1]
 
-                return vos, total_count
+            return vos, total_count
 
-            except Exception as e:
-                raise ERROR_DB_QUERY(reason=e)
+        except Exception as e:
+            raise ERROR_DB_QUERY(reason=e)
 
     @classmethod
     def _check_well_known_type(cls, value):
-        if isinstance(value, bson.objectid.ObjectId):
+        if isinstance(value, datetime):
+            return f'{value.isoformat()}Z'
+        elif isinstance(value, bson.objectid.ObjectId):
             return str(value)
         elif isinstance(value, Document):
             return str(value.id)
         elif isinstance(value, EmbeddedDocument):
             return dict(value.to_mongo())
         else:
             return value
 
     @classmethod
     def _make_aggregate_values(cls, cursor):
         values = []
         for row in cursor:
             data = {}
             for key, value in row.items():
-                if key == "_id" and isinstance(row[key], dict):
+                if key == '_id' and isinstance(row[key], dict):
                     for group_key, group_value in row[key].items():
                         data[group_key] = cls._check_well_known_type(group_value)
                 else:
                     data[key] = cls._check_well_known_type(value)
 
             values.append(data)
 
@@ -784,420 +643,379 @@
         return changed_values
 
     @classmethod
     def _make_sub_conditions(cls, sub_conditions, _before_group_keys):
         and_sub_conditions = []
 
         for sub_condition in sub_conditions:
-            key = sub_condition.get("key", sub_condition.get("k"))
-            value = sub_condition.get("value", sub_condition.get("v"))
-            operator = sub_condition.get("operator", sub_condition.get("o"))
+            key = sub_condition.get('key', sub_condition.get('k'))
+            value = sub_condition.get('value', sub_condition.get('v'))
+            operator = sub_condition.get('operator', sub_condition.get('o'))
 
             if key is None:
                 raise ERROR_DB_QUERY(
-                    reason=f"'aggregate.group.fields.conditions.key' condition requires a key: {sub_condition}"
-                )
+                    reason=f"'aggregate.group.fields.conditions.key' condition requires a key: {sub_condition}")
 
             if value is None:
                 raise ERROR_DB_QUERY(
-                    reason=f"'aggregate.group.fields.conditions.value' condition requires a value: {sub_condition}"
-                )
+                    reason=f"'aggregate.group.fields.conditions.value' condition requires a value: {sub_condition}")
 
             if operator is None:
                 raise ERROR_DB_QUERY(
-                    reason=f"'aggregate.group.fields.conditions.operator' condition requires a operator: {sub_condition}"
-                )
+                    reason=f"'aggregate.group.fields.conditions.operator' condition requires a operator: {sub_condition}")
 
-            _SUPPORTED_OPERATOR = ["eq", "not", "gt", "gte", "lt", "lte"]
+            _SUPPORTED_OPERATOR = ['eq', 'not', 'gt', 'gte', 'lt', 'lte']
 
             if operator not in _SUPPORTED_OPERATOR:
                 raise ERROR_DB_QUERY(
                     reason=f"'aggregate.group.fields.conditions.operator' condition's {operator} operator is not "
-                    f"supported. (supported_operator = {_SUPPORTED_OPERATOR})"
-                )
+                           f"supported. (supported_operator = {_SUPPORTED_OPERATOR})")
 
             if key in _before_group_keys:
-                key = f"_id.{key}"
+                key = f'_id.{key}'
 
-            and_sub_conditions.append({f"${operator}": [f"${key}", value]})
+            and_sub_conditions.append(
+                {
+                    f'${operator}': [f'${key}', value]
+                }
+            )
 
-        return {"$and": and_sub_conditions}
+        return {
+            '$and': and_sub_conditions
+        }
 
     @classmethod
     def _get_group_fields(cls, condition, _before_group_keys):
-        key = condition.get("key", condition.get("k"))
-        name = condition.get("name", condition.get("n"))
-        operator = condition.get("operator", condition.get("o"))
-        sub_conditions = condition.get("conditions")
-        sub_fields = condition.get("fields") or []
-        data_type = condition.get("data_type")
+        key = condition.get('key', condition.get('k'))
+        name = condition.get('name', condition.get('n'))
+        operator = condition.get('operator', condition.get('o'))
+        sub_conditions = condition.get('conditions')
+        sub_fields = condition.get('fields') or []
+        data_type = condition.get('data_type')
 
         if operator not in STAT_GROUP_OPERATORS:
-            raise ERROR_DB_QUERY(
-                reason=f"'aggregate.group.fields' condition's {operator} operator is not supported. "
-                f"(supported_operator = {list(STAT_GROUP_OPERATORS.keys())})"
-            )
+            raise ERROR_DB_QUERY(reason=f"'aggregate.group.fields' condition's {operator} operator is not supported. "
+                                        f"(supported_operator = {list(STAT_GROUP_OPERATORS.keys())})")
 
         if name is None:
-            raise ERROR_DB_QUERY(
-                reason=f"'aggregate.group.fields' condition requires a name: {condition}"
-            )
+            raise ERROR_DB_QUERY(reason=f"'aggregate.group.fields' condition requires a name: {condition}")
 
         if key in _before_group_keys:
-            key = f"_id.{key}"
+            key = f'_id.{key}'
 
         for sub_field in sub_fields:
-            f_key = sub_field.get("key", sub_field.get("k"))
-            f_name = sub_field.get("name", sub_field.get("n"))
+            f_key = sub_field.get('key', sub_field.get('k'))
+            f_name = sub_field.get('name', sub_field.get('n'))
 
             if f_key is None:
-                raise ERROR_DB_QUERY(
-                    reason=f"'aggregate.group.fields.fields' condition requires a key: {condition}"
-                )
+                raise ERROR_DB_QUERY(reason=f"'aggregate.group.fields.fields' condition requires a key: {condition}")
 
             if f_name is None:
-                raise ERROR_DB_QUERY(
-                    reason=f"'aggregate.group.fields.fields' condition requires a name: {condition}"
-                )
+                raise ERROR_DB_QUERY(reason=f"'aggregate.group.fields.fields' condition requires a name: {condition}")
 
             if f_key in _before_group_keys:
-                sub_field["key"] = f"_id.{f_key}"
+                sub_field['key'] = f'_id.{f_key}'
 
         if sub_conditions:
-            sub_conditions = cls._make_sub_conditions(
-                sub_conditions, _before_group_keys
-            )
+            sub_conditions = cls._make_sub_conditions(sub_conditions, _before_group_keys)
 
         return key, name, operator, sub_fields, sub_conditions, data_type
 
     @classmethod
     def _get_group_keys(cls, condition, _before_group_keys):
-        key = condition.get("key", condition.get("k"))
-        name = condition.get("name", condition.get("n"))
-        date_format = condition.get("date_format")
+        key = condition.get('key', condition.get('k'))
+        name = condition.get('name', condition.get('n'))
+        date_format = condition.get('date_format')
 
         if key is None:
-            raise ERROR_DB_QUERY(
-                reason=f"'aggregate.group.keys' condition requires a key: {condition}"
-            )
+            raise ERROR_DB_QUERY(reason=f"'aggregate.group.keys' condition requires a key: {condition}")
 
         if name is None:
-            raise ERROR_DB_QUERY(
-                reason=f"'aggregate.group.keys' condition requires a name: {condition}"
-            )
+            raise ERROR_DB_QUERY(reason=f"'aggregate.group.keys' condition requires a name: {condition}")
 
         if key in _before_group_keys:
-            key = f"_id.{key}"
+            key = f'_id.{key}'
 
         if date_format:
-            if date_format == "year":
-                rule = {"$year": f"${key}"}
-            elif date_format == "month":
-                rule = {"$month": f"${key}"}
-            elif date_format == "day":
-                rule = {"$dayOfMonth": f"${key}"}
+            if date_format == 'year':
+                rule = {
+                    '$year': f'${key}'
+                }
+            elif date_format == 'month':
+                rule = {
+                    '$month': f'${key}'
+                }
+            elif date_format == 'day':
+                rule = {
+                    '$dayOfMonth': f'${key}'
+                }
             else:
-                rule = {"$dateToString": {"format": date_format, "date": f"${key}"}}
+                rule = {
+                    '$dateToString': {
+                        'format': date_format,
+                        'date': f'${key}'
+                    }
+                }
         else:
-            rule = f"${key}"
+            rule = f'${key}'
 
         return name, rule
 
     @classmethod
     def _make_group_rule(cls, options, _before_group_keys):
         _group_keys = []
-        _group_rule = {"$group": {"_id": {}}}
-        _keys = options.get("keys", [])
-        _fields = options.get("fields", [])
+        _group_rule = {
+            '$group': {
+                '_id': {}
+            }
+        }
+        _keys = options.get('keys', [])
+        _fields = options.get('fields', [])
 
         if len(_keys) == 0 and len(_fields) == 0:
-            raise ERROR_REQUIRED_PARAMETER(
-                key="aggregate.group.keys || aggregate.group.fields"
-            )
+            raise ERROR_REQUIRED_PARAMETER(key='aggregate.group.keys || aggregate.group.fields')
 
         for condition in _keys:
             name, rule = cls._get_group_keys(condition, _before_group_keys)
-            _group_rule["$group"]["_id"][name] = rule
+            _group_rule['$group']['_id'][name] = rule
             _group_keys.append(name)
 
         for condition in _fields:
-            (
-                key,
-                name,
-                operator,
-                sub_fields,
-                sub_conditions,
-                data_type,
-            ) = cls._get_group_fields(condition, _before_group_keys)
-
-            rule = STAT_GROUP_OPERATORS[operator](
-                condition,
-                key,
-                operator,
-                name,
-                data_type,
-                sub_conditions,
-                sub_fields,
-                cls._meta["datetime_fields"],
-            )
-            _group_rule["$group"].update(rule)
+            key, name, operator, sub_fields, sub_conditions, data_type = \
+                cls._get_group_fields(condition, _before_group_keys)
+
+            rule = STAT_GROUP_OPERATORS[operator](condition, key, operator, name, data_type, sub_conditions, sub_fields,
+                                                  cls._meta['datetime_fields'])
+            _group_rule['$group'].update(rule)
 
         return _group_rule, _group_keys
 
     @classmethod
     def _get_project_fields(cls, condition):
-        key = condition.get("key", condition.get("k"))
-        name = condition.get("name", condition.get("n"))
-        operator = condition.get("operator", condition.get("o"))
-        fields = condition.get("fields", condition.get("f"))
+        key = condition.get('key', condition.get('k'))
+        name = condition.get('name', condition.get('n'))
+        operator = condition.get('operator', condition.get('o'))
+        fields = condition.get('fields', condition.get('f'))
 
         if operator and operator not in STAT_PROJECT_OPERATORS:
-            raise ERROR_DB_QUERY(
-                reason=f"'aggregate.project.fields' condition's {operator} operator is not supported. "
-                f"(supported_operator = {list(STAT_PROJECT_OPERATORS.keys())})"
-            )
+            raise ERROR_DB_QUERY(reason=f"'aggregate.project.fields' condition's {operator} operator is not supported. "
+                                        f"(supported_operator = {list(STAT_PROJECT_OPERATORS.keys())})")
 
         if name is None:
-            raise ERROR_DB_QUERY(
-                reason=f"'aggregate.project.fields' condition requires a name: {condition}"
-            )
+            raise ERROR_DB_QUERY(reason=f"'aggregate.project.fields' condition requires a name: {condition}")
 
         return key, name, operator, fields
 
     @classmethod
     def _make_project_rule(cls, options, _group_keys):
         _rules = []
-        _fields = options.get("fields", [])
-        _exclude_keys = options.get("exclude_keys", False)
-        _only_keys = options.get("only_keys", False)
-        _project_rule = {"$project": {}}
+        _fields = options.get('fields', [])
+        _exclude_keys = options.get('exclude_keys', False)
+        _project_rule = {
+            '$project': {
+            }
+        }
 
         if len(_fields) == 0:
-            raise ERROR_REQUIRED_PARAMETER(key="aggregate.project.fields")
+            raise ERROR_REQUIRED_PARAMETER(key='aggregate.project.fields')
 
         for condition in _fields:
             key, name, operator, fields = cls._get_project_fields(condition)
 
             if operator:
-                rule = STAT_PROJECT_OPERATORS[operator](
-                    condition, key, operator, name, fields, _group_keys
-                )
-                _project_rule["$project"].update(rule)
+                rule = STAT_PROJECT_OPERATORS[operator](condition, key, operator, name, fields, _group_keys)
+                _project_rule['$project'].update(rule)
             else:
                 if key in _group_keys:
-                    key = f"_id.{key}"
+                    key = f'_id.{key}'
 
-                if _only_keys:
-                    _project_rule["$project"][name] = 1
-                else:
-                    _project_rule["$project"][name] = f"${key}"
+                _project_rule['$project'][name] = f'${key}'
 
         if _exclude_keys:
-            _project_rule["$project"]["_id"] = 0
+            _project_rule['$project']['_id'] = 0
             _group_keys = []
 
         return _project_rule, _group_keys
 
     @classmethod
     def _make_unwind_rule(cls, options):
-        if "path" not in options:
-            raise ERROR_REQUIRED_PARAMETER(key="aggregate.unwind.path")
+        if 'path' not in options:
+            raise ERROR_REQUIRED_PARAMETER(key='aggregate.unwind.path')
 
-        return {"$unwind": f"${options['path']}"}
+        return {
+            '$unwind': f"${options['path']}"
+        }
 
     @classmethod
     def _make_count_rule(cls, options):
-        if "name" not in options:
-            raise ERROR_REQUIRED_PARAMETER(key="aggregate.count.name")
+        if 'name' not in options:
+            raise ERROR_REQUIRED_PARAMETER(key='aggregate.count.name')
 
-        return {"$count": options["name"]}
+        return {
+            '$count': options['name']
+        }
 
     @classmethod
     def _make_sort_rule(cls, options, _group_keys):
+        key = options.get('key')
+        desc = options.get('desc', False)
+        keys = options.get('keys')
+
         order_by = {}
 
-        for sort_option in options:
-            if sort_option["key"] in _group_keys:
-                sort_key = f'_id.{sort_option["key"]}'
+        if key:
+            if key in _group_keys:
+                sort_key = f'_id.{key}'
             else:
-                sort_key = sort_option["key"]
+                sort_key = key
+
+            order_by[sort_key] = -1 if desc else 1
+
+        elif keys:
+            for k in keys:
+                if k['key'] in _group_keys:
+                    sort_key = f'_id.{k["key"]}'
+                else:
+                    sort_key = k['key']
 
-            order_by[sort_key] = -1 if sort_option.get("desc", False) else 1
+                order_by[sort_key] = -1 if k.get('desc', False) else 1
 
-        return {"$sort": order_by}
+        else:
+            raise ERROR_REQUIRED_PARAMETER(key='aggregate.sort.key')
+
+        return {
+            '$sort': order_by
+        }
 
     @classmethod
     def _make_limit_rule(cls, options):
-        return {"$limit": options}
+        return {
+            '$limit': options
+        }
 
     @classmethod
     def _make_skip_rule(cls, options):
-        return {"$skip": options}
-
-    @classmethod
-    def _make_match_rule(cls, options):
-        match_options = {"$and": []}
-
-        for condition in options.get("filter", []):
-            key = condition.get("key", condition.get("k"))
-            value = condition.get("value", condition.get("v"))
-            operator = condition.get("operator", condition.get("o"))
-
-            if not (key and value and operator):
-                raise ERROR_REQUIRED_PARAMETER(key="aggregate.match.filter")
-
-            if operator == "eq":
-                match_options["$and"].append({key: value})
-            elif operator == "not":
-                match_options["$and"].append({key: {"$ne": value}})
-            elif operator == "in":
-                match_options["$and"].append({key: {"$in": value}})
-            elif operator == "not_in":
-                match_options["$and"].append({key: {"$nin": value}})
-            elif operator == "contain":
-                match_options["$and"].append({key: {"$regex": f".*{value}.*"}})
-            elif operator == "not_contain":
-                match_options["$and"].append(
-                    {key: {"$not": {"$regex": f".*{value}.*"}}}
-                )
-            elif operator == "contain_in":
-                match_options["$and"].append(
-                    {"$or": [{key: {"$regex": f".*{v}.*"}} for v in value]}
-                )
-            elif operator == "not_contain_in":
-                match_options["$and"].append(
-                    {"$nor": [{key: {"$regex": f".*{v}.*"}} for v in value]}
-                )
-            else:
-                raise ERROR_DB_QUERY(reason=f"Unsupported operator: {operator}")
-
-        return {"$match": match_options}
+        return {
+            '$skip': options
+        }
 
     @classmethod
     def _make_aggregate_rules(cls, aggregate):
         _aggregate_rules = []
         _group_keys = []
 
         if not isinstance(aggregate, list):
-            raise ERROR_INVALID_PARAMETER_TYPE(key="aggregate", type="list")
+            raise ERROR_INVALID_PARAMETER_TYPE(key='aggregate', type='list')
 
         for stage in aggregate:
-            if "unwind" in stage:
-                rule = cls._make_unwind_rule(stage["unwind"])
+            if 'unwind' in stage:
+                rule = cls._make_unwind_rule(stage['unwind'])
                 _aggregate_rules.append(rule)
-            elif "group" in stage:
-                rule, group_keys = cls._make_group_rule(stage["group"], _group_keys)
+            elif 'group' in stage:
+                rule, group_keys = cls._make_group_rule(stage['group'], _group_keys)
                 _aggregate_rules.append(rule)
                 _group_keys += group_keys
-            elif "count" in stage:
-                rule = cls._make_count_rule(stage["count"])
+            elif 'count' in stage:
+                rule = cls._make_count_rule(stage['count'])
                 _aggregate_rules.append(rule)
-            elif "sort" in stage:
-                rule = cls._make_sort_rule(stage["sort"], _group_keys)
+            elif 'sort' in stage:
+                rule = cls._make_sort_rule(stage['sort'], _group_keys)
                 _aggregate_rules.append(rule)
-            elif "project" in stage:
-                rule, _group_keys = cls._make_project_rule(
-                    stage["project"], _group_keys
-                )
+            elif 'project' in stage:
+                rule, _group_keys = cls._make_project_rule(stage['project'], _group_keys)
                 _aggregate_rules.append(rule)
-            elif "limit" in stage:
-                rule = cls._make_limit_rule(stage["limit"])
+            elif 'limit' in stage:
+                rule = cls._make_limit_rule(stage['limit'])
                 _aggregate_rules.append(rule)
-            elif "skip" in stage:
-                rule = cls._make_skip_rule(stage["skip"])
-                _aggregate_rules.append(rule)
-            elif "match" in stage:
-                rule = cls._make_match_rule(stage["match"])
+            elif 'skip' in stage:
+                rule = cls._make_skip_rule(stage['skip'])
                 _aggregate_rules.append(rule)
             else:
-                raise ERROR_REQUIRED_PARAMETER(
-                    key="aggregate.unwind or aggregate.group or "
-                    "aggregate.count or aggregate.sort or "
-                    "aggregate.project or aggregate.limit or "
-                    "aggregate.skip"
-                )
+                raise ERROR_REQUIRED_PARAMETER(key='aggregate.unwind or aggregate.group or '
+                                                   'aggregate.count or aggregate.sort or '
+                                                   'aggregate.project or aggregate.limit or '
+                                                   'aggregate.skip')
 
         return _aggregate_rules
 
     @classmethod
     def _stat_aggregate(cls, vos, aggregate, page, allow_disk_use):
         result = {}
         pipeline = []
         _aggregate_rules = cls._make_aggregate_rules(aggregate)
 
         for rule in _aggregate_rules:
             pipeline.append(rule)
 
-        if "limit" in page and page["limit"] > 0:
-            limit = page["limit"]
-            start = page.get("start", 1)
+        if 'limit' in page and page['limit'] > 0:
+            limit = page['limit']
+            start = page.get('start', 1)
             start = 1 if start < 1 else start
 
-            result["total_count"] = 0
-            cursor = vos.aggregate(pipeline + [{"$count": "total_count"}])
+            result['total_count'] = 0
+            cursor = vos.aggregate(pipeline + [{'$count': 'total_count'}])
             for c in cursor:
-                result["total_count"] = c["total_count"]
+                result['total_count'] = c['total_count']
                 break
 
             if start > 1:
-                pipeline.append({"$skip": start - 1})
-
-            pipeline.append({"$limit": limit})
+                pipeline.append({
+                    '$skip': start - 1
+                })
+
+            pipeline.append({
+                '$limit': limit
+            })
 
         if allow_disk_use:
-            _LOGGER.debug(f"[_stat_aggregate] allow_disk_use: {allow_disk_use}")
+            _LOGGER.debug(f'[_stat_aggregate] allow_disk_use: {allow_disk_use}')
             cursor = vos.aggregate(pipeline, allowDiskUse=True)
         else:
             cursor = vos.aggregate(pipeline)
-        result["results"] = cls._make_aggregate_values(cursor)
+        result['results'] = cls._make_aggregate_values(cursor)
         return result
 
     @classmethod
     def _stat_distinct(cls, vos, distinct, page):
         result = {}
         values = vos.distinct(distinct)
 
         try:
             values.sort()
         except Exception:
             pass
 
-        if "limit" in page and page["limit"] > 0:
-            start = page.get("start", 1)
+        if 'limit' in page and page['limit'] > 0:
+            start = page.get('start', 1)
             if start < 1:
                 start = 1
 
-            result["total_count"] = len(values)
-            values = values[start - 1 : start + page["limit"] - 1]
+            result['total_count'] = len(values)
+            values = values[start - 1:start + page['limit'] - 1]
 
-        result["results"] = cls._make_distinct_values(values)
+        result['results'] = cls._make_distinct_values(values)
         return result
 
     @classmethod
-    def stat(
-        cls,
-        *args,
-        aggregate=None,
-        distinct=None,
-        filter=None,
-        filter_or=None,
-        page=None,
-        reference_filter=None,
-        target="SECONDARY_PREFERRED",
-        allow_disk_use=False,
-        **kwargs,
-    ):
-        filter = filter or []
-        filter_or = filter_or or []
-        page = page or {}
+    def stat(cls, *args, aggregate=None, distinct=None, filter=None, filter_or=None, page=None,
+             target='SECONDARY_PREFERRED', allow_disk_use=False, **kwargs):
+
+        if filter is None:
+            filter = []
+
+        if filter_or is None:
+            filter_or = []
+
+        if page is None:
+            page = {}
 
         if not (aggregate or distinct):
-            raise ERROR_REQUIRED_PARAMETER(key="aggregate")
+            raise ERROR_REQUIRED_PARAMETER(key='aggregate')
 
-        _filter = cls._make_filter(filter, filter_or, reference_filter)
+        _filter = cls._make_filter(filter, filter_or)
 
         try:
             vos = cls._get_target_objects(target).filter(_filter)
 
             if aggregate:
                 return cls._stat_aggregate(vos, aggregate, page, allow_disk_use)
 
@@ -1209,352 +1027,360 @@
                 e = ERROR_UNKNOWN(message=str(e))
 
             raise ERROR_DB_QUERY(reason=e.message)
 
     @classmethod
     def _check_field_group(cls, field_group):
         for key in field_group:
-            if key.startswith("_total_"):
-                raise ERROR_INVALID_PARAMETER(
-                    key="field_group",
-                    reason="Field group keys cannot contain _total_ characters.",
-                )
+            if key.startswith('_total_'):
+                raise ERROR_INVALID_PARAMETER(key='field_group',
+                                              reason='Field group keys cannot contain _total_ characters.')
 
     @classmethod
     def _make_group_keys(cls, group_by, date_field, granularity=None):
         group_keys = []
-        for group_option in group_by:
-            if isinstance(group_option, dict):
-                key = group_option.get("key")
-                name = group_option.get("name")
-
-                if not (key and name):
-                    raise ERROR_INVALID_PARAMETER(
-                        key="group_by",
-                        reason="group_by option requires a key and name.",
-                    )
-            elif isinstance(group_option, str):
-                key = group_option
-                name = key.rsplit(".", 1)[-1:][0]
-            else:
-                raise ERROR_INVALID_PARAMETER(
-                    key="group_by",
-                    reason="group_by option should be dict or str type.",
-                )
-
-            group_keys.append({"key": key, "name": name})
-
-        if granularity and granularity in ["DAILY", "MONTHLY", "YEARLY"]:
-            group_keys.append({"key": date_field, "name": "date"})
+        for key in group_by:
+            name = key.rsplit('.', 1)[-1:][0]
+            group_keys.append({
+                'key': key,
+                'name': name
+            })
+
+        if granularity and granularity in ['DAILY', 'MONTHLY', 'YEARLY']:
+            group_keys.append({
+                'key': date_field,
+                'name': 'date'
+            })
 
         return group_keys
 
     @classmethod
     def _make_group_fields(cls, fields):
         group_fields = []
         for name, condition in fields.items():
             cls._check_condition(condition)
-            operator = condition["operator"]
-            key = condition.get("key")
-            fields = condition.get("fields")
-            data_type = condition.get("data_type")
-
-            group_field = {"name": name, "operator": operator, "data_type": data_type}
+            operator = condition['operator']
+            key = condition.get('key')
+            fields = condition.get('fields')
+            data_type = condition.get('data_type')
+
+            group_field = {
+                'name': name,
+                'operator': operator,
+                'data_type': data_type
+            }
 
-            if operator != "count":
-                group_field["key"] = key
+            if operator != 'count':
+                group_field['key'] = key
 
-            if operator == "push" and fields:
+            if operator == 'push' and fields:
                 push_fields = []
                 for key, value in fields.items():
-                    push_fields.append({"key": value, "name": key})
+                    push_fields.append({
+                        'key': value,
+                        'name': key
+                    })
 
-                group_field["fields"] = push_fields
+                group_field['fields'] = push_fields
 
             group_fields.append(group_field)
 
         return group_fields
 
     @classmethod
     def _check_condition(cls, condition):
-        key = condition.get("key")
-        operator = condition.get("operator")
-        fields = condition.get("fields", [])
+        key = condition.get('key')
+        operator = condition.get('operator')
+        fields = condition.get('fields', [])
 
         if operator is None:
-            raise ERROR_REQUIRED_PARAMETER(key="query.fields.operator")
+            raise ERROR_REQUIRED_PARAMETER(key='query.fields.operator')
 
         # Check Operator
-        if operator not in ["count", "push"] and key is None:
-            raise ERROR_REQUIRED_PARAMETER(key="query.fields.key")
+        if operator not in ['count', 'push'] and key is None:
+            raise ERROR_REQUIRED_PARAMETER(key='query.fields.key')
 
-        if operator == "push" and not key and len(fields) == 0:
-            raise ERROR_REQUIRED_PARAMETER(key="query.fields.fields")
+        if operator == 'push' and not key and len(fields) == 0:
+            raise ERROR_REQUIRED_PARAMETER(key='query.fields.fields')
 
     @classmethod
     def _make_field_group_keys(cls, group_keys, field_group):
         field_group_keys = []
-        for group_option in group_keys:
-            key = group_option["name"]
-            name = group_option["name"]
+        for group_key in group_keys:
+            key = group_key['key'].rsplit('.', 1)[-1:][0]
+            name = group_key['name']
             if name not in field_group:
-                if name == "date":
-                    field_group_keys.append({"key": "date", "name": "date"})
+                if name == 'date':
+                    field_group_keys.append({
+                        'key': 'date',
+                        'name': 'date'
+                    })
                 else:
-                    field_group_keys.append({"key": key, "name": name})
+                    field_group_keys.append({
+                        'key': key,
+                        'name': name
+                    })
 
         return field_group_keys
 
     @classmethod
     def _make_field_group_fields(cls, group_fields, field_group):
         field_group_fields = []
         for group_field in group_fields:
-            field_name = group_field["name"]
-            operator = group_field["operator"]
+            field_name = group_field['name']
+            operator = group_field['operator']
 
-            if operator in ["sum", "average", "max", "min", "count"]:
-                field_group_fields.append(
-                    {
-                        "key": field_name,
-                        "name": f"_total_{field_name}",
-                        "operator": "sum" if operator == "count" else operator,
-                    }
-                )
-
-            field_group_fields.append(
-                {
-                    "name": field_name,
-                    "operator": "push",
-                    "fields": cls._make_field_group_push_fields(
-                        field_name, field_group
-                    ),
-                }
-            )
+            if operator in ['sum', 'average', 'max', 'min', 'count']:
+                field_group_fields.append({
+                    'key': field_name,
+                    'name': f'_total_{field_name}',
+                    'operator': 'sum' if operator == 'count' else operator
+                })
+
+            field_group_fields.append({
+                'name': field_name,
+                'operator': 'push',
+                'fields': cls._make_field_group_push_fields(field_name, field_group)
+            })
 
         return field_group_fields
 
     @classmethod
     def _make_field_group_push_fields(cls, field_name, field_group):
-        push_fields = [{"name": "value", "key": field_name}]
+        push_fields = [
+            {
+                'name': 'value',
+                'key': field_name
+            }
+        ]
 
         for field_group_key in field_group:
-            push_fields.append({"name": field_group_key, "key": field_group_key})
+            push_fields.append({
+                'name': field_group_key,
+                'key': field_group_key
+            })
 
         return push_fields
 
     @classmethod
     def _make_field_group_query(cls, group_keys, group_fields, field_group):
         field_group_query = {
-            "group": {
-                "keys": cls._make_field_group_keys(group_keys, field_group),
-                "fields": cls._make_field_group_fields(group_fields, field_group),
+            'group': {
+                'keys': cls._make_field_group_keys(group_keys, field_group),
+                'fields': cls._make_field_group_fields(group_fields, field_group)
             }
         }
 
         return [field_group_query]
 
     @classmethod
     def _make_select_query(cls, select):
-        select_query = {"project": {"fields": [], "exclude_keys": True}}
+        select_query = {
+            'project': {
+                'fields': [],
+                'exclude_keys': True
+            }
+        }
 
-        supported_operator = ["add", "subtract", "multiply", "divide", "size", "sum"]
+        supported_operator = ['add', 'subtract', 'multiply', 'divide', 'size', 'sum']
 
         for name, condition in select.items():
             if isinstance(condition, str):
-                select_query["project"]["fields"].append(
-                    {"name": name, "key": condition}
-                )
+                select_query['project']['fields'].append({
+                    'name': name,
+                    'key': condition
+                })
             elif isinstance(condition, dict):
-                operator = condition.get("operator")
-                key = condition.get("key")
-                fields = condition.get("fields")
+                operator = condition.get('operator')
+                key = condition.get('key')
+                fields = condition.get('fields')
 
                 if operator not in supported_operator:
-                    raise ERROR_INVALID_PARAMETER(
-                        key="query.select.operator",
-                        reason=f"supported_operator = {supported_operator}",
-                    )
+                    raise ERROR_INVALID_PARAMETER(key='query.select.operator',
+                                                  reason=f'supported_operator = {supported_operator}')
 
                 if key:
-                    select_query["project"]["fields"].append(
-                        {"name": name, "operator": operator, "key": key}
-                    )
+                    select_query['project']['fields'].append({
+                        'name': name,
+                        'operator': operator,
+                        'key': key
+                    })
                 elif fields:
-                    select_query["project"]["fields"].append(
-                        {"name": name, "operator": operator, "fields": fields}
-                    )
+                    select_query['project']['fields'].append({
+                        'name': name,
+                        'operator': operator,
+                        'fields': fields
+                    })
                 else:
-                    raise ERROR_REQUIRED_PARAMETER(key="query.select.fields")
+                    raise ERROR_REQUIRED_PARAMETER(key='query.select.fields')
 
         return [select_query]
 
     @classmethod
     def _make_sort_query(cls, sort, group_fields, has_field_group):
-        sort_query = {"sort": []}
+        sort_query = {
+            'sort': {
+                'keys': []
+            }
+        }
         if has_field_group:
             group_field_names = []
             for group_field in group_fields:
-                group_field_names.append(group_field["name"])
+                group_field_names.append(group_field['name'])
 
             for condition in sort:
-                key = condition.get("key")
-                desc = condition.get("desc", False)
+                key = condition.get('key')
+                desc = condition.get('desc', False)
 
                 if key in group_field_names:
-                    key = f"_total_{key}"
+                    key = f'_total_{key}'
 
-                sort_query["sort"].append({"key": key, "desc": desc})
+                sort_query['sort']['keys'].append({
+                    'key': key,
+                    'desc': desc
+                })
         else:
-            sort_query["sort"] = sort
+            sort_query['sort']['keys'] = sort
 
         return [sort_query]
 
     @classmethod
     def _make_page_query(cls, page):
         page_query = []
-        start = page.get("start")
-        limit = page.get("limit")
+        start = page.get('start')
+        limit = page.get('limit')
 
         if limit:
             if start:
-                page_query.append({"skip": start - 1})
-
-            page_query.append({"limit": limit + 1})
+                page_query.append({
+                    'skip': start - 1
+                })
+
+            page_query.append({
+                'limit': limit + 1
+            })
 
         return page_query
 
     @classmethod
     def _make_date_filter(cls, date_field, key, operator):
-        return [{"k": date_field, "v": key, "o": operator}]
+        return [{
+            'k': date_field,
+            'v': key,
+            'o': operator
+        }]
 
     @classmethod
     def _parse_start_and_end_time(cls, key, value) -> date:
         if isinstance(value, date):
             return value
         elif isinstance(value, datetime):
             return value.date()
         elif isinstance(value, str):
+
             if len(value) == 4:
-                date_format = "%Y"
-                date_type = "YYYY"
+                date_format = '%Y'
+                date_type = 'YYYY'
             elif len(value) == 7:
-                date_format = "%Y-%m"
-                date_type = "YYYY-MM"
+                date_format = '%Y-%m'
+                date_type = 'YYYY-MM'
             else:
-                date_format = "%Y-%m-%d"
-                date_type = "YYYY-MM-DD"
+                date_format = '%Y-%m-%d'
+                date_type = 'YYYY-MM-DD'
 
             try:
                 dt = datetime.strptime(value, date_format).date()
 
-                if date_type == "YYYY":
-                    if key == "start":
+                if date_type == 'YYYY':
+                    if key == 'start':
                         return datetime(dt.year, 1, 1)
                     else:
                         return datetime(dt.year, 1, 1) + relativedelta(years=1)
-                elif date_type == "YYYY-MM":
-                    if key == "start":
+                elif date_type == 'YYYY-MM':
+                    if key == 'start':
                         return datetime(dt.year, dt.month, 1)
                     else:
                         return datetime(dt.year, dt.month, 1) + relativedelta(months=1)
                 else:
-                    if key == "start":
+                    if key == 'start':
                         return datetime(dt.year, dt.month, dt.day)
                     else:
-                        return datetime(dt.year, dt.month, dt.day) + relativedelta(
-                            days=1
-                        )
+                        return datetime(dt.year, dt.month, dt.day) + relativedelta(days=1)
 
             except Exception as e:
                 raise ERROR_INVALID_PARAMETER_TYPE(key=key, type=date_type)
         else:
-            raise ERROR_INVALID_PARAMETER(
-                key=key, reason=f"{key} option should be datetime or str"
-            )
+            raise ERROR_INVALID_PARAMETER(key=key, reason=f'{key} option should be datetime or str')
 
     @classmethod
     def _convert_date_value(cls, date_value, date_field_format):
         if isinstance(date_field_format, str):
             return date_value.strftime(date_field_format)
         else:
             return date_value
 
     @classmethod
-    def analyze(
-        cls,
-        *args,
-        granularity=None,
-        fields=None,
-        select=None,
-        group_by=None,
-        field_group=None,
-        filter=None,
-        filter_or=None,
-        page=None,
-        sort=None,
-        start=None,
-        end=None,
-        date_field="date",
-        date_field_format="%Y-%m-%d",
-        reference_filter=None,
-        target="SECONDARY_PREFERRED",
-        allow_disk_use=False,
-        **kwargs,
-    ):
+    def analyze(cls, *args, granularity=None, fields=None, select=None, group_by=None, field_group=None,
+                filter=None, filter_or=None, page=None, sort=None, start=None, end=None,
+                date_field='date', date_field_format='%Y-%m-%d', target='SECONDARY_PREFERRED',
+                allow_disk_use=False, **kwargs):
+
         if fields is None:
-            raise ERROR_REQUIRED_PARAMETER(key="fields")
+            raise ERROR_REQUIRED_PARAMETER(key='fields')
 
         filter = filter or []
         filter_or = filter_or or []
         group_by = group_by or []
         sort = sort or []
         page = page or {}
         field_group = field_group or []
         cls._check_field_group(field_group)
         has_field_group = len(field_group) > 0
-        page_limit = page.get("limit")
+        page_limit = page.get('limit')
 
         if start:
-            start_time: date = cls._parse_start_and_end_time("start", start)
+            start_time: date = cls._parse_start_and_end_time('start', start)
             start_value = cls._convert_date_value(start_time, date_field_format)
-            filter += cls._make_date_filter(date_field, start_value, "gte")
+            filter += cls._make_date_filter(date_field, start_value, 'gte')
 
         if end:
-            end_time: date = cls._parse_start_and_end_time("end", end)
+            end_time: date = cls._parse_start_and_end_time('end', end)
             end_value = cls._convert_date_value(end_time, date_field_format)
-            filter += cls._make_date_filter(date_field, end_value, "lt")
+            filter += cls._make_date_filter(date_field, end_value, 'lt')
 
         group_keys = cls._make_group_keys(group_by, date_field, granularity)
         group_fields = cls._make_group_fields(fields)
 
         query = {
-            "filter": filter,
-            "filter_or": filter_or,
-            "aggregate": [{"group": {"keys": group_keys, "fields": group_fields}}],
-            "target": target,
-            "allow_disk_use": allow_disk_use,
-            "reference_filter": reference_filter,
+            'filter': filter,
+            'filter_or': filter_or,
+            'aggregate': [
+                {
+                    'group': {
+                        'keys': group_keys,
+                        'fields': group_fields
+                    }
+                }
+            ],
+            'target': target,
+            'allow_disk_use': allow_disk_use
         }
 
         if select:
-            query["aggregate"] += cls._make_select_query(select)
+            query['aggregate'] += cls._make_select_query(select)
 
         if has_field_group:
-            query["aggregate"] += cls._make_field_group_query(
-                group_keys, group_fields, field_group
-            )
+            query['aggregate'] += cls._make_field_group_query(group_keys, group_fields, field_group)
 
         if len(sort) > 0:
-            query["aggregate"] += cls._make_sort_query(
-                sort, group_fields, has_field_group
-            )
+            query['aggregate'] += cls._make_sort_query(sort, group_fields, has_field_group)
 
         if page:
-            query["aggregate"] += cls._make_page_query(page)
+            query['aggregate'] += cls._make_page_query(page)
 
         response = cls.stat(**query)
 
         if page_limit:
-            response["more"] = len(response["results"]) > page_limit
-            response["results"] = response["results"][:page_limit]
+            response['more'] = len(response['results']) > page_limit
+            response['results'] = response['results'][:page_limit]
 
         return response
```

### Comparing `spaceone-core-2.0.84/spaceone/core/model/mongo_model/filter_operator.py` & `spaceone-core-2.0.9/spaceone/core/model/mongo_model/filter_operator.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/model/mongo_model/stat_operator.py` & `spaceone-core-2.0.9/spaceone/core/model/mongo_model/stat_operator.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/opentelemetry/metrics.py` & `spaceone-core-2.0.9/spaceone/core/opentelemetry/metrics.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/opentelemetry/tracer.py` & `spaceone-core-2.0.9/spaceone/core/opentelemetry/tracer.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/pygrpc/client.py` & `spaceone-core-2.0.9/spaceone/core/pygrpc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 import logging
 import types
 import grpc
 from google.protobuf.json_format import ParseDict
 from google.protobuf.message_factory import MessageFactory
 from google.protobuf.descriptor_pool import DescriptorPool
 from google.protobuf.descriptor import ServiceDescriptor, MethodDescriptor
@@ -179,15 +180,15 @@
             setattr(self, method_name, channel.unary_unary(
                 method_key,
                 request_serializer=request_message_desc.SerializeToString,
                 response_deserializer=response_message_desc.FromString
             ))
 
 
-class GRPCClient(object):
+class _GRPCClient(object):
 
     def __init__(self, channel, options, channel_key):
         self._request_map = {}
         self._api_resources = {}
 
         self._reflection_db = ProtoReflectionDescriptorDatabase(channel)
         self._desc_pool = DescriptorPool(self._reflection_db)
@@ -255,15 +256,15 @@
 
         try:
             grpc.channel_ready_future(channel).result(timeout=3)
         except Exception as e:
             raise ERROR_GRPC_CONNECTION(channel=endpoint, message='Channel is not ready.')
 
         try:
-            _GRPC_CHANNEL[endpoint] = GRPCClient(channel, client_opts, endpoint)
+            _GRPC_CHANNEL[endpoint] = _GRPCClient(channel, client_opts, endpoint)
         except Exception as e:
             if hasattr(e, 'details'):
                 raise ERROR_GRPC_CONNECTION(channel=endpoint, message=e.details())
             else:
                 raise ERROR_GRPC_CONNECTION(channel=endpoint, message=str(e))
 
     return _GRPC_CHANNEL[endpoint]
```

### Comparing `spaceone-core-2.0.84/spaceone/core/pygrpc/extension/grpc_health.py` & `spaceone-core-2.0.9/spaceone/core/pygrpc/extension/grpc_health.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/pygrpc/extension/server_info.py` & `spaceone-core-2.0.9/spaceone/core/pygrpc/extension/server_info.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/pygrpc/server.py` & `spaceone-core-2.0.9/spaceone/core/pygrpc/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,25 +72,24 @@
         self.server.add_insecure_port(f'[::]:{self._port}')
         _LOGGER.info(f'Start gRPC Server ({self._service}): '
                      f'port={self._port}, max_workers={self._max_workers}')
         self.server.start()
         self.server.wait_for_termination()
 
 
-def _get_grpc_app() -> GRPCServer:
-    package: str = config.get_package()
-    app_path: str = config.get_global('GRPC_APP_PATH')
-    app_path = app_path.format(package=package)
-    module_path, app_name = app_path.split(':')
+def _get_app(app_path: str) -> GRPCServer:
+    package_path = config.get_package()
+    app_module_path, app_name = app_path.split(':')
+    module_path = f'{package_path}.{app_module_path}'
 
     try:
         app_module = __import__(module_path, fromlist=[app_name])
 
         if not hasattr(app_module, 'app'):
-            raise ImportError(f'App is not defined. (app_path = {package}.{app_path})')
+            raise ImportError(f'App is not defined. (app_path = {package_path}.{app_path})')
 
         return getattr(app_module, 'app')
     except Exception as e:
         raise ImportError(f'Cannot import app: {e}')
 
 
 def _import_module(module_path, servicer_name):
@@ -99,15 +98,15 @@
         module = __import__(module_path, fromlist=[servicer_name])
     except Exception as e:
         _LOGGER.warning(f'[_import_module] Cannot import grpc servicer module. (reason = {e})', exc_info=True)
 
     return module
 
 
-def add_extension_services(app):
+def _add_extension_services(app):
     ext_proto_conf = config.get_global('GRPC_EXTENSION_SERVICERS', {})
     for module_path, servicer_names in ext_proto_conf.items():
         for servicer_name in servicer_names:
             if api_module := _import_module(module_path, servicer_name):
                 if hasattr(api_module, servicer_name):
                     servicer_cls = getattr(api_module, servicer_name)
 
@@ -115,11 +114,11 @@
                 else:
                     _LOGGER.warning(f'[_add_services] Failed to add service. '
                                     f'(module_path={module_path}, servicer_name={servicer_name})')
 
     return app
 
 
-def serve():
-    app = _get_grpc_app()
-    app = add_extension_services(app)
+def serve(app_path: str):
+    app = _get_app(app_path)
+    app = _add_extension_services(app)
     app.run()
```

### Comparing `spaceone-core-2.0.84/spaceone/core/queue/__init__.py` & `spaceone-core-2.0.9/spaceone/core/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/queue/redis_queue.py` & `spaceone-core-2.0.9/spaceone/core/queue/redis_queue.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/scheduler/scheduler.py` & `spaceone-core-2.0.9/spaceone/core/scheduler/scheduler.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,60 +24,61 @@
         self.global_config = config.get_global()
         super().__init__()
 
     def push_task(self):
         # Create Task
         try:
             tasks = self.create_task()
-            _LOGGER.debug(f"[push_task] task: {len(tasks)}")
+            _LOGGER.debug(f'[push_task] task: {len(tasks)}')
         except Exception as e:
-            _LOGGER.error(f"[push_task] error create_task: {e}")
+            _LOGGER.error(f'[push_task] error create_task: {e}')
             tasks = []
 
         for task in tasks:
             try:
                 validate(task, schema=SPACEONE_TASK_SCHEMA)
                 json_task = json.dumps(task)
-                _LOGGER.debug(f"[push_task] Task schema: {self._remove_metadata(task)}")
+                _LOGGER.debug(f'[push_task] Task schema: {self._remove_metadata(task)}')
                 queue.put(self.queue, json_task)
             except Exception as e:
-                _LOGGER.debug(f"[push_task] Task schema: {task}, {e}")
+                print(e)
+                _LOGGER.debug(f'[push_task] Task schema: {task}, {e}')
 
     def run(self):
-        NotImplementedError("scheduler.run is not implemented")
+        NotImplementedError('scheduler.run is not implemented')
 
     def create_task(self):
-        NotImplementedError("scheduler.create_task is not implemented")
+        NotImplementedError('scheduler.create_task is not implemented')
 
     def _remove_metadata(self, task):
         copied_task = copy.deepcopy(task)
         change_stages = []
-        for stage in copied_task.get("stages", []):
-            if "metadata" in stage:
-                stage["metadata"] = "*****"
+        for stage in copied_task.get('stages', []):
+            if 'metadata' in stage:
+                stage['metadata'] = '*****'
             change_stages.append(stage)
 
-        copied_task["stages"] = change_stages
+        copied_task['stages'] = change_stages
         return copied_task
 
 
 class IntervalScheduler(BaseScheduler):
     def __init__(self, queue, interval):
         super().__init__(queue)
         self.config = self.parse_config(interval)
 
     def parse_config(self, expr):
-        """expr
-        format: integer (second)
+        """ expr
+          format: integer (second)
         """
         try:
             if isinstance(expr, int):
                 return int(expr)
         except Exception as e:
-            _LOGGER.error(f"[parse_config] Wrong configraiton, {e}")
+            _LOGGER.error(f'[parse_config] Wrong configraiton, {e}')
 
     def run(self):
         config.set_global_force(**self.global_config)
 
         # Enable logging configuration
         set_logger()
 
@@ -89,30 +90,29 @@
 
 class HourlyScheduler(BaseScheduler):
     """
     HourlyScheduler starts every HH:00
     If you want to start at different minutes
     send minute like ':15' meaning every 15 minute
     """
-
-    def __init__(self, queue, interval=1, minute=":00"):
+    def __init__(self, queue, interval=1, minute=':00'):
         super().__init__(queue)
         self.config = self.parse_config(interval)
         self.minute = minute
 
     def parse_config(self, expr):
-        """expr
-        format: integer (hour)
+        """ expr
+          format: integer (hour)
         """
         try:
             if isinstance(expr, int):
                 return int(expr)
         except Exception as e:
-            _LOGGER.error(f"[parse_config] Wrong configuration, {e}")
-            raise ERROR_CONFIGURATION(key="interval")
+            _LOGGER.error(f'[parse_config] Wrong configuration, {e}')
+            raise ERROR_CONFIGURATION(key='interval')
 
     def run(self):
         config.set_global_force(**self.global_config)
 
         # Enable logging configuration
         set_logger()
 
@@ -123,23 +123,22 @@
             time.sleep(1)
 
 
 class CronScheduler(BaseScheduler):
     """
     cronjob: min hour day month week
     """
-
     def __init__(self, queue, rule):
         super().__init__(queue)
         self.config = self.parse_config(rule)
 
     def parse_config(self, expr):
-        """exprd
-        format: min hour day month week
-        * * * * *
+        """ exprd
+          format: min hour day month week
+          * * * * *
         """
         # TODO: verify format
         return expr
 
     def run(self):
         config.set_global_force(**self.global_config)
```

### Comparing `spaceone-core-2.0.84/spaceone/core/scheduler/server.py` & `spaceone-core-2.0.9/spaceone/core/scheduler/server.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/scheduler/task_schema.py` & `spaceone-core-2.0.9/spaceone/core/scheduler/task_schema.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/scheduler/worker.py` & `spaceone-core-2.0.9/spaceone/core/scheduler/worker.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import copy
 import json
 import random
 import string
 import logging
 
 from multiprocessing import Process
 
@@ -11,97 +10,91 @@
 from spaceone.core.logger import set_logger
 from spaceone.core.error import ERROR_TASK_LOCATOR, ERROR_TASK_METHOD
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def randomString(stringLength=8):
-    """Generate a random string of fixed length"""
+    """Generate a random string of fixed length """
     letters = string.ascii_lowercase
-    return "".join(random.sample(letters, stringLength))
+    return ''.join(random.sample(letters, stringLength))
 
 
 class SingleTask:
+
     def __init__(self, single_task: dict):
-        self.locator = single_task["locator"]
-        self.name = single_task["name"]
-        self.metadata = single_task["metadata"]
-        self.method = single_task["method"]
-        self.params = single_task["params"]
+        self.locator = single_task['locator']
+        self.name = single_task['name']
+        self.metadata = single_task['metadata']
+        self.method = single_task['method']
+        self.params = single_task['params']
         self._locator = Locator()
 
     def execute(self):
-        """Run method"""
+        """ Run method
+        """
         try:
-            if self.locator == "SERVICE":
+            if self.locator == 'SERVICE':
                 caller = self._locator.get_service(self.name, self.metadata)
-            elif self.locator == "MANAGER":
+            elif self.locator == 'MANAGER':
                 caller = self._locator.get_manager(self.name)
 
         except Exception as e:
-            _LOGGER.debug(f"[SingleTask.execute] locator error: {e}")
+            _LOGGER.debug(f'[SingleTask] fail at locator {e}')
             raise ERROR_TASK_LOCATOR(locator=self.locator, name=self.name)
 
         try:
-            _LOGGER.debug(
-                f"[SingleTask.execute] (REQUEST) => {self.name}.{self.method}"
-            )
+            _LOGGER.debug(f'[SingleTask] request: {self.name}.{self.method} {self.params}')
             method = getattr(caller, self.method)
             resp = method(**self.params)
-            _LOGGER.debug(f"[SingleTask.execute] (RESPONSE) => SUCCESS")
+            _LOGGER.debug(f'[SingleTask] response: {resp}')
             return resp
         except Exception as e:
-            _LOGGER.error(
-                f"[SingleTask.execute] Fail to execute method ({self.method}): {e}",
-                exc_info=True,
-            )
-            raise ERROR_TASK_METHOD(name=self.name, method=self.method)
+            _LOGGER.error(f'[SingleTask] fail to execute method: {self.method}, params: {self.params}, {e}')
+            raise ERROR_TASK_METHOD(name=self.name, method=self.method, params=self.params)
 
 
 class SpaceoneTask:
     def __init__(self, task: dict):
         self.task = task
-        self.name = task.get("name", "")
-        self.version = task.get("version", "v1")
-        self.execution_engine = task.get("executionEngine", "BaseWorker")
-        self.stages = task.get("stages")
-        self.stop_on_failure = task.get("stop_on_failure", True)
+        self.name = task.get('name', "")
+        self.version = task.get('version', 'v1')
+        self.execution_engine = task.get('executionEngine', 'BaseWorker')
+        self.stages = task.get('stages')
+        self.stop_on_failure = task.get('stop_on_failure', True)
 
     def execute(self):
-        """Run stage"""
+        """ Run stage
+        """
         self.tasks = []
         for stage in self.stages:
             try:
                 single_task = SingleTask(stage)
                 single_task.execute()
             except Exception as e:
-                stage_log = copy.deepcopy(stage)
-                stage_log["metadata"] = "*****"
-                _LOGGER.error(
-                    f"[SpaceoneTask] fail to parse {stage_log}, {e}", exc_info=True
-                )
+                _LOGGER.error(f'[SpaceoneTask] fail to parse {stage}, {e}')
                 if self.stop_on_failure:
-                    _LOGGER.debug(
-                        f"[SpaceoneTask] stop task, since stop on failure is enabled"
-                    )
+                    _LOGGER.debug(f'[SpaceoneTask] stop task, since stop on failure is enabled')
                     break
 
 
 class BaseWorker(Process):
+
     def __init__(self, queue, **kwargs):
-        self._name_ = "worker-%s" % randomString()
+        self._name_ = 'worker-%s' % randomString()
         self.queue = queue
-        _LOGGER.debug(f"[BaseWorker] BaseWorker name  : {self._name_}")
-        _LOGGER.debug(f"[BaseWorker] BaseWorker queue : {self.queue}")
+        _LOGGER.debug(f'[BaseWorker] BaseWorker name  : {self._name_}')
+        _LOGGER.debug(f'[BaseWorker] BaseWorker queue : {self.queue}')
 
         self.global_config = config.get_global()
         super().__init__()
 
     def run(self):
-        """Infinite Loop"""
+        """ Infinite Loop
+        """
         config.set_global_force(**self.global_config)
 
         # Enable logging configuration
         set_logger()
 
         while True:
             # Read from Queue
@@ -109,11 +102,11 @@
             try:
                 json_task = json.loads(binary_task.decode())
                 task = SpaceoneTask(json_task)
                 # Run task
                 task.execute()
 
             except Exception as e:
-                _LOGGER.error(
-                    f"[{self._name_}] failed to decode task: {binary_task}, {e}"
-                )
+                _LOGGER.error(f'[{self._name_}] failed to decode task: {binary_task}, {e}')
                 continue
+
+
```

### Comparing `spaceone-core-2.0.84/spaceone/core/service/utils.py` & `spaceone-core-2.0.9/spaceone/core/service/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,125 +1,41 @@
 import re
 import functools
-import types
-from typing import Union
 from dateutil.parser import parse
-from datetime import datetime, date
-from typing import get_type_hints
-from pydantic import ValidationError, BaseModel
+from datetime import datetime
+from dateutil.relativedelta import relativedelta
 
 from spaceone.core import utils
 from spaceone.core.error import *
 
-__all__ = [
-    "convert_model",
-    "change_value_by_rule",
-    "change_only_key",
-    "check_required",
-    "set_query_page_limit",
-    "append_query_filter",
-    "change_tag_filter",
-    "append_keyword_filter",
-    "change_timestamp_value",
-    "change_date_value",
-    "change_timestamp_filter",
-]
-
-
-def _raise_pydantic_error(e: ValidationError):
-    for error in e.errors():
-        if error["type"] == "value_error.missing":
-            raise ERROR_REQUIRED_PARAMETER(key=", ".join(error["loc"]))
-        elif error["type"].startswith("type_error"):
-            raise ERROR_INVALID_PARAMETER_TYPE(
-                key=", ".join(error["loc"]), type=error["type"].split(".")[1]
-            )
-        else:
-            raise ERROR_INVALID_PARAMETER(
-                key=", ".join(error["loc"]), reason=error["msg"]
-            )
-
-
-def _generate_response(response_iterator: types.GeneratorType) -> types.GeneratorType:
-    for response in response_iterator:
-        if isinstance(response, BaseModel):
-            response = response.dict()
-
-        yield response
-
-
-def convert_model(func) -> callable:
-    @functools.wraps(func)
-    def wrapped_func(self, params: dict) -> Union[dict, types.GeneratorType]:
-        type_hints = get_type_hints(func)
-        params_hint = type_hints.get("params")
-
-        if params_hint and isinstance(params, dict):
-            try:
-                params = params_hint(**params)
-            except ValidationError as e:
-                _raise_pydantic_error(e)
-
-        response_or_iterator = func(self, params)
-
-        if isinstance(response_or_iterator, types.GeneratorType):
-            return _generate_response(response_or_iterator)
-        else:
-            if isinstance(response_or_iterator, BaseModel):
-                response_or_iterator = response_or_iterator.dict()
-
-        return response_or_iterator
-
-    return wrapped_func
-
-
-def change_value_by_rule(rule: str, param_key: str, value: any = None) -> any:
-    def wrapper(func: callable) -> callable:
-        @functools.wraps(func)
-        def wrapped_func(cls, params: dict) -> Union[dict, types.GeneratorType]:
-            if param_value := params.get(param_key):
-                if rule == "APPEND":
-                    if isinstance(param_value, list):
-                        param_value.append(value)
-                    else:
-                        param_value = [param_value, value]
-
-                params[param_key] = param_value
-
-            return func(cls, params)
-
-        return wrapped_func
-
-    return wrapper
-
 
-def change_only_key(change_rule, key_path="only") -> callable:
+def change_only_key(change_rule, key_path='only'):
     def wrapper(func):
         @functools.wraps(func)
         def wrapped_func(cls, params):
             only_keys = change_rule.keys()
             only = utils.get_dict_value(params, key_path, [])
             new_only = []
             for key in only:
-                key_match = key.split(".", 1)[0]
+                key_match = key.split('.', 1)[0]
                 if key_match in only_keys:
                     if change_rule[key_match] not in new_only:
                         new_only.append(change_rule[key_match])
                 else:
                     new_only.append(key)
 
             utils.change_dict_value(params, key_path, new_only)
             return func(cls, params)
 
         return wrapped_func
 
     return wrapper
 
 
-def check_required(required_keys) -> callable:
+def check_required(required_keys):
     def wrapper(func):
         @functools.wraps(func)
         def wrapped_func(cls, params):
             for key in required_keys:
                 value = utils.get_dict_value(params, key)
                 if value is None:
                     raise ERROR_REQUIRED_PARAMETER(key=key)
@@ -127,197 +43,199 @@
             return func(cls, params)
 
         return wrapped_func
 
     return wrapper
 
 
-def set_query_page_limit(default_limit) -> callable:
+def set_query_page_limit(default_limit):
     def wrapper(func):
         @functools.wraps(func)
         def wrapped_func(cls, params):
-            query = params.get("query", {})
-            query["page"] = query.get("page", {})
-            page_limit = query["page"].get("limit", 1000)
+            query = params.get('query', {})
+            query['page'] = query.get('page', {})
+            page_limit = query['page'].get('limit', 1000)
 
             if page_limit > default_limit:
                 page_limit = default_limit
 
-            query["page"]["limit"] = page_limit
-            params["query"] = query
+            query['page']['limit'] = page_limit
+            params['query'] = query
 
             return func(cls, params)
 
         return wrapped_func
 
     return wrapper
 
 
-def append_query_filter(filter_keys) -> callable:
+def append_query_filter(filter_keys):
     def wrapper(func):
         @functools.wraps(func)
         def wrapped_func(cls, params):
-            query = params.get("query", {})
-            query["filter"] = query.get("filter", [])
+            query = params.get('query', {})
+            query['filter'] = query.get('filter', [])
 
             for key in filter_keys:
                 if key in params:
                     if isinstance(params[key], list):
-                        query["filter"].append({"k": key, "v": params[key], "o": "in"})
+                        query['filter'].append({'k': key, 'v': params[key], 'o': 'in'})
                     else:
-                        query["filter"].append({"k": key, "v": params[key], "o": "eq"})
+                        query['filter'].append({'k': key, 'v': params[key], 'o': 'eq'})
 
-            params["query"] = query
+            params['query'] = query
 
             return func(cls, params)
 
         return wrapped_func
 
     return wrapper
 
 
-def change_tag_filter(tag_key="tags") -> callable:
+def change_tag_filter(tag_key='tags'):
     def wrapper(func):
         @functools.wraps(func)
         def wrapped_func(cls, params):
-            params["query"] = params.get("query", {})
+            params['query'] = params.get('query', {})
             change_filter = []
-            for condition in params["query"].get("filter", []):
-                key = condition.get("key", condition.get("k"))
-                if key and key.startswith(f"{tag_key}."):
-                    value = condition.get("value", condition.get("v"))
-                    operator = condition.get("operator", condition.get("o"))
-                    tag_key_split = key.split(".", 1)
-                    change_filter.append(
-                        {
-                            "key": "tags",
-                            "value": {
-                                "key": tag_key_split[1],
-                                "value": _change_match_query(
-                                    operator, value, condition
-                                ),
-                            },
-                            "operator": "match",
-                        }
-                    )
+            for condition in params['query'].get('filter', []):
+                key = condition.get('key', condition.get('k'))
+                if key and key.startswith(f'{tag_key}.'):
+                    value = condition.get('value', condition.get('v'))
+                    operator = condition.get('operator', condition.get('o'))
+                    tag_key_split = key.split('.', 1)
+                    change_filter.append({
+                        'key': 'tags',
+                        'value': {
+                            'key': tag_key_split[1],
+                            'value': _change_match_query(operator, value, condition)
+                        },
+                        'operator': 'match'
+                    })
                 else:
                     change_filter.append(condition)
 
-            if "only" in params["query"]:
+            if 'only' in params['query']:
                 change_only = []
-                for key in params["query"].get("only", []):
-                    if key.startswith("tags.") and "tags" not in change_only:
-                        change_only.append("tags")
+                for key in params['query'].get('only', []):
+                    if key.startswith('tags.') and 'tags' not in change_only:
+                        change_only.append('tags')
                     else:
                         change_only.append(key)
 
-                params["query"]["only"] = change_only
+                params['query']['only'] = change_only
 
-            params["query"]["filter"] = change_filter
+            params['query']['filter'] = change_filter
             return func(cls, params)
 
         return wrapped_func
 
     return wrapper
 
 
-def _change_match_query(operator, value, condition) -> callable:
-    if operator == "eq":
+def _change_match_query(operator, value, condition):
+    if operator == 'eq':
         return value
-    elif operator == "not":
-        return {"$ne": value}
-    elif operator == "in":
+    elif operator == 'not':
+        return {
+            '$ne': value
+        }
+    elif operator == 'in':
         if not isinstance(value, list):
             raise ERROR_OPERATOR_LIST_VALUE_TYPE(operator=operator, condition=condition)
 
-        return {"$in": value}
-    elif operator == "not_in":
+        return {
+            '$in': value
+        }
+    elif operator == 'not_in':
         if not isinstance(value, list):
             raise ERROR_OPERATOR_LIST_VALUE_TYPE(operator=operator, condition=condition)
 
-        return {"$nin": value}
-    elif operator == "contain":
+        return {
+            '$nin': value
+        }
+    elif operator == 'contain':
         return re.compile(value, re.IGNORECASE)
-    elif operator == "not_contain":
-        return {"$not": re.compile(value, re.IGNORECASE)}
-    elif operator == "contain_in":
+    elif operator == 'not_contain':
+        return {
+            '$not': re.compile(value, re.IGNORECASE)
+        }
+    elif operator == 'contain_in':
         if not isinstance(value, list):
             raise ERROR_OPERATOR_LIST_VALUE_TYPE(operator=operator, condition=condition)
 
-        return {"$in": value}
-    elif operator == "not_contain_in":
+        return {
+            '$in': value
+        }
+    elif operator == 'not_contain_in':
         if not isinstance(value, list):
             raise ERROR_OPERATOR_LIST_VALUE_TYPE(operator=operator, condition=condition)
 
-        return {"$nin": value}
+        return {
+            '$nin': value
+        }
     else:
-        raise ERROR_DB_QUERY(reason="Filter operator is not supported.")
+        raise ERROR_DB_QUERY(reason='Filter operator is not supported.')
 
 
-def append_keyword_filter(keywords=None) -> callable:
+def append_keyword_filter(keywords=None):
     if keywords is None:
         keywords = []
 
     def wrapper(func):
         @functools.wraps(func)
         def wrapped_func(cls, params):
-            query = params.get("query", {})
-            if "keyword" in query:
-                query["filter_or"] = query.get("filter_or", [])
+            query = params.get('query', {})
+            if 'keyword' in query:
+                query['filter_or'] = query.get('filter_or', [])
 
-                keyword = query["keyword"].strip()
+                keyword = query['keyword'].strip()
                 if len(keyword) > 0:
                     for key in keywords:
-                        query["filter_or"].append(
-                            {
-                                "k": key,
-                                "v": list(filter(None, keyword.split(" "))),
-                                "o": "contain_in",
-                            }
-                        )
+                        query['filter_or'].append({
+                            'k': key,
+                            'v': list(filter(None, keyword.split(' '))),
+                            'o': 'contain_in'
+                        })
 
-                del query["keyword"]
-                params["query"] = query
+                del query['keyword']
+                params['query'] = query
 
             return func(cls, params)
 
         return wrapped_func
 
     return wrapper
 
 
-def change_timestamp_value(
-    timestamp_keys=None, timestamp_format="google_timestamp"
-) -> callable:
+def change_timestamp_value(timestamp_keys=None, timestamp_format='google_timestamp'):
     if timestamp_keys is None:
         timestamp_keys = []
 
     def wrapper(func):
         @functools.wraps(func)
         def wrapped_func(cls, params):
             change_params = {}
 
             for key, value in params.items():
                 if key in timestamp_keys:
                     if not _is_null(value):
-                        value = _convert_datetime_from_timestamp(
-                            value, key, timestamp_format
-                        )
+                        value = _convert_datetime_from_timestamp(value, key, timestamp_format)
                         change_params[key] = value
                 else:
                     change_params[key] = value
 
             return func(cls, change_params)
 
         return wrapped_func
 
     return wrapper
 
 
-def change_date_value(date_keys=None, date_format="%Y-%m-%d") -> callable:
+def change_date_value(date_keys=None, date_format='%Y-%m-%d'):
     if date_keys is None:
         date_keys = []
 
     def wrapper(func):
         @functools.wraps(func)
         def wrapped_func(cls, params):
             change_params = {}
@@ -333,90 +251,84 @@
             return func(cls, change_params)
 
         return wrapped_func
 
     return wrapper
 
 
-def change_timestamp_filter(
-    filter_keys=None, timestamp_format="google_timestamp"
-) -> callable:
+def change_timestamp_filter(filter_keys=None, timestamp_format='google_timestamp'):
     if filter_keys is None:
         filter_keys = []
 
     def wrapper(func):
         @functools.wraps(func)
         def wrapped_func(cls, params):
-            query = params.get("query", {})
-            query_filter = query.get("filter")
-            query_filter_or = query.get("filter_or")
+            query = params.get('query', {})
+            query_filter = query.get('filter')
+            query_filter_or = query.get('filter_or')
             if query_filter:
-                query["filter"] = _change_timestamp_condition(
-                    query_filter, filter_keys, "filter", timestamp_format
-                )
+                query['filter'] = _change_timestamp_condition(query_filter, filter_keys,
+                                                              'filter', timestamp_format)
 
             if query_filter_or:
-                query["filter_or"] = _change_timestamp_condition(
-                    query_filter_or, filter_keys, "filter_or", timestamp_format
-                )
+                query['filter_or'] = _change_timestamp_condition(query_filter_or, filter_keys,
+                                                                 'filter_or', timestamp_format)
 
-            params["query"] = query
+            params['query'] = query
 
             return func(cls, params)
 
         return wrapped_func
 
     return wrapper
 
 
-def _is_null(value) -> bool:
-    if value is None or str(value).strip() == "":
+def _is_null(value):
+    if value is None or str(value).strip() == '':
         return True
 
     return False
 
 
-def _change_timestamp_condition(
-    query_filter, filter_keys, filter_type, timestamp_format
-) -> list:
+def _change_timestamp_condition(query_filter, filter_keys, filter_type, timestamp_format):
     change_filter = []
 
     for condition in query_filter:
-        key = condition.get("k") or condition.get("key")
-        value = condition.get("v") or condition.get("value")
-        operator = condition.get("o") or condition.get("operator")
+        key = condition.get('k') or condition.get('key')
+        value = condition.get('v') or condition.get('value')
+        operator = condition.get('o') or condition.get('operator')
 
         if key in filter_keys:
-            value = _convert_datetime_from_timestamp(
-                value, f"query.{filter_type}.{key}", timestamp_format
-            )
+            value = _convert_datetime_from_timestamp(value, f'query.{filter_type}.{key}', timestamp_format)
 
-        change_filter.append({"key": key, "value": value, "operator": operator})
+        change_filter.append({
+            'key': key,
+            'value': value,
+            'operator': operator
+        })
 
     return change_filter
 
 
-def _convert_datetime_from_timestamp(timestamp, key, timestamp_format) -> datetime:
-    type_message = (
-        "google.protobuf.Timestamp({seconds: <second>, nanos: <nano second>})"
-    )
+def _convert_datetime_from_timestamp(timestamp, key, timestamp_format):
+    type_message = 'google.protobuf.Timestamp({seconds: <second>, nanos: <nano second>})'
 
     try:
-        if timestamp_format == "iso8601":
-            type_message = "ISO 8601(YYYY-MM-DDThh:mm:ssTZD)"
+        if timestamp_format == 'iso8601':
+            type_message = 'ISO 8601(YYYY-MM-DDThh:mm:ssTZD)'
             return parse(timestamp)
         else:
-            seconds = timestamp["seconds"]
-            nanos = timestamp.get("nanos")
+            seconds = timestamp['seconds']
+            nanos = timestamp.get('nanos')
 
             # TODO: change nanoseconds to timestamp
 
             return datetime.utcfromtimestamp((int(seconds)))
     except Exception as e:
         raise ERROR_INVALID_PARAMETER_TYPE(key=key, type=type_message)
 
 
-def _convert_date_from_string(date_str, key, date_format) -> date:
+def _convert_date_from_string(date_str, key, date_format):
     try:
         return datetime.strptime(date_str, date_format).date()
     except Exception as e:
         raise ERROR_INVALID_PARAMETER_TYPE(key=key, type=date_format)
```

### Comparing `spaceone-core-2.0.84/spaceone/core/skeleton/conf/global_conf.py` & `spaceone-core-2.0.9/spaceone/core/skeleton/conf/global_conf.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/skeleton/interface/grpc/helloworld.py` & `spaceone-core-2.0.9/spaceone/core/skeleton/interface/grpc/helloworld.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/token.py` & `spaceone-core-2.0.9/spaceone/core/token.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/unittest/result.py` & `spaceone-core-2.0.9/spaceone/core/unittest/result.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/unittest/runner.py` & `spaceone-core-2.0.9/spaceone/core/unittest/runner.py`

 * *Files identical despite different names*

### Comparing `spaceone-core-2.0.84/spaceone/core/utils.py` & `spaceone-core-2.0.9/spaceone/core/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,71 +1,70 @@
+import os
 import re
 import time
 import random
 import string
 import secrets
+import sys
 import datetime
 import yaml
 import json
 import hashlib
 import urllib
+import pkg_resources
 
 from urllib.parse import urlparse
 from dateutil.parser import isoparse
 from typing import Tuple
 from pathlib import Path
 from typing import Union
 
 YAML_LOADER = yaml.Loader
 YAML_LOADER.add_implicit_resolver(
-    "tag:yaml.org,2002:float",
-    re.compile(
-        """^(?:
+    u'tag:yaml.org,2002:float',
+    re.compile(u'''^(?:
      [-+]?(?:[0-9][0-9_]*)\\.[0-9_]*(?:[eE][-+]?[0-9]+)?
     |[-+]?(?:[0-9][0-9_]*)(?:[eE][-+]?[0-9]+)
     |\\.[0-9_]+(?:[eE][-+][0-9]+)?
     |[-+]?[0-9][0-9_]*(?::[0-5]?[0-9])+\\.[0-9_]*
     |[-+]?\\.(?:inf|Inf|INF)
-    |\\.(?:nan|NaN|NAN))$""",
-        re.X,
-    ),
-    list("-+0123456789."),
-)
+    |\\.(?:nan|NaN|NAN))$''', re.X),
+    list(u'-+0123456789.'))
 
 
-def generate_id(prefix: str = "id", nbytes: int = 6) -> str:
+def generate_id(prefix: str = 'id', nbytes: int = 6) -> str:
     random_id = secrets.token_hex(nbytes)
-    return f"{prefix}-{random_id}"
+    return f'{prefix}-{random_id}'
 
 
 def generate_trace_id() -> int:
     return random.getrandbits(128)
 
 
 def generate_secret(nbytes: int = 32) -> str:
     return secrets.token_urlsafe(nbytes)
 
 
 def generate_password(length: int = 8) -> str:
     # create alphanumerical from string constants
-    printable = f"{string.ascii_letters}{string.digits}"
+    printable = f'{string.ascii_letters}{string.digits}'
 
     # convert printable from string to list and shuffle
     printable = list(printable)
     random.shuffle(printable)
 
     # generate random password and convert to string
     random_password = random.choices(printable, k=length)
 
     # Append one lowercase and one uppercase and one number characters
     random_password.append(random.choices(list(string.ascii_lowercase))[0])
     random_password.append(random.choices(list(string.ascii_uppercase))[0])
     random_password.append(random.choices(list(string.digits))[0])
 
-    random_password = "".join(random_password)
+    random_password = ''.join(random_password)
     return random_password
 
 
 def random_string(nbytes: int = 6) -> str:
     return secrets.token_hex(nbytes)
 
 
@@ -74,140 +73,140 @@
     p.mkdir(parents=True, exist_ok=True)
 
 
 def dump_json(data, indent=None, sort_keys=False) -> str:
     try:
         return json.dumps(data, indent=indent, sort_keys=sort_keys, ensure_ascii=False)
     except Exception as e:
-        raise ValueError(f"JSON Dump Error: {str(e)}")
+        raise ValueError(f'JSON Dump Error: {str(e)}')
 
 
 def save_json_to_file(data, json_file: str, indent=None, sort_keys=False):
     try:
         json_str = dump_json(data, indent, sort_keys)
-        with open(json_file, "w") as f:
+        with open(json_file, 'w') as f:
             f.write(json_str)
             f.close()
     except Exception as e:
-        raise ValueError(f"JSON Save Error: {str(e)}")
+        raise ValueError(f'JSON Save Error: {str(e)}')
 
 
 def load_json(json_str: str) -> dict:
     try:
         return json.loads(json_str)
     except Exception:
-        raise ValueError(f"JSON Load Error: {json_str}")
+        raise ValueError(f'JSON Load Error: {json_str}')
 
 
 def load_json_from_file(json_file: str) -> dict:
     try:
-        with open(json_file, "r") as f:
+        with open(json_file, 'r') as f:
             return load_json(f.read())
     except Exception:
-        raise Exception(f"JSON Load Error: {json_file}")
+        raise Exception(f'JSON Load Error: {json_file}')
 
 
 def dump_yaml(data: dict) -> str:
     try:
         return yaml.dump(data, allow_unicode=True)
     except Exception as e:
-        raise ValueError(f"YAML Dump Error: {str(e)}")
+        raise ValueError(f'YAML Dump Error: {str(e)}')
 
 
 def save_yaml_to_file(data: dict, yaml_file: str):
     try:
         yaml_str = dump_yaml(data)
-        with open(yaml_file, "w") as f:
+        with open(yaml_file, 'w') as f:
             f.write(yaml_str)
             f.close()
     except Exception as e:
-        raise ValueError(f"YAML Save Error: {str(e)}")
+        raise ValueError(f'YAML Save Error: {str(e)}')
 
 
 def load_yaml(yaml_str: str) -> dict:
     try:
         return yaml.load(yaml_str, Loader=YAML_LOADER)
     except Exception:
-        raise ValueError(f"YAML Load Error: {yaml_str}")
+        raise ValueError(f'YAML Load Error: {yaml_str}')
 
 
 def load_yaml_from_file(yaml_file: str) -> dict:
     try:
-        with open(yaml_file, "r") as f:
+        with open(yaml_file, 'r') as f:
             return load_yaml(f.read())
     except Exception:
-        raise Exception(f"YAML Load Error: {yaml_file}")
+        raise Exception(f'YAML Load Error: {yaml_file}')
 
 
 def load_yaml_from_url(url: str) -> dict:
     try:
         f = urllib.urlopen(url)
         return load_yaml(f.read())
     except Exception as e:
-        raise Exception(f"Http call error: {url}. e={e}")
+        raise Exception(f'Http call error: {url}. e={e}')
 
 
 def parse_endpoint(endpoint: str) -> dict:
     try:
         o = urlparse(endpoint)
     except Exception:
-        raise ValueError(f"Endpoint is invalid. ({endpoint})")
+        raise ValueError(f'Endpoint is invalid. ({endpoint})')
 
-    return {"scheme": o.scheme, "hostname": o.hostname, "port": o.port, "path": o.path}
+    return {
+        'scheme': o.scheme,
+        'hostname': o.hostname,
+        'port': o.port,
+        'path': o.path
+    }
 
 
 def parse_grpc_endpoint(endpoint: str) -> dict:
     try:
         endpoint_info = parse_endpoint(endpoint)
 
-        if endpoint_info["scheme"] not in ["grpc", "grpc+ssl"]:
-            raise ValueError(
-                f"Unsupported protocol. (supported_protocol=grpc|grpc+ssl, endpoint={endpoint})"
-            )
+        if endpoint_info['scheme'] not in ['grpc', 'grpc+ssl']:
+            raise ValueError(f'Unsupported protocol. (supported_protocol=grpc|grpc+ssl, endpoint={endpoint})')
 
     except Exception:
-        raise ValueError(f"gRPC Endpoint is invalid. (endpoint={endpoint})")
+        raise ValueError(f'gRPC Endpoint is invalid. (endpoint={endpoint})')
 
-    if endpoint_info["scheme"] == "grpc+ssl":
+    if endpoint_info['scheme'] == 'grpc+ssl':
         ssl_enabled = True
     else:
         ssl_enabled = False
 
     return {
-        "endpoint": f'{endpoint_info["hostname"]}:{endpoint_info["port"]}',
-        "ssl_enabled": ssl_enabled,
+        'endpoint': f'{endpoint_info["hostname"]}:{endpoint_info["port"]}',
+        'ssl_enabled': ssl_enabled
     }
 
 
 def parse_grpc_uri(uri: str) -> dict:
     try:
         endpoint_info = parse_endpoint(uri)
 
-        if endpoint_info["scheme"] not in ["grpc", "grpc+ssl"]:
-            raise ValueError(
-                f"Unsupported protocol. (supported_protocol=grpc|grpc+ssl, uri={uri})"
-            )
-
-        version, service, method = filter(
-            lambda x: x.strip() != "", endpoint_info["path"].split("/")
-        )
+        if endpoint_info['scheme'] not in ['grpc', 'grpc+ssl']:
+            raise ValueError(f'Unsupported protocol. (supported_protocol=grpc|grpc+ssl, uri={uri})')
+
+        version, service, method = \
+            filter(lambda x: x.strip() != '', endpoint_info['path'].split('/'))
     except Exception:
-        raise ValueError(f"gRPC URI is invalid. (uri={uri})")
+        raise ValueError(f'gRPC URI is invalid. (uri={uri})')
 
-    if endpoint_info["scheme"] == "grpc+ssl":
+    if endpoint_info['scheme'] == 'grpc+ssl':
         ssl_enabled = True
     else:
         ssl_enabled = False
 
     return {
-        "endpoint": f'{endpoint_info["hostname"]}:{endpoint_info["port"]}',
-        "version": version,
-        "service": service,
-        "method": method,
-        "ssl_enabled": ssl_enabled,
+        'endpoint': f'{endpoint_info["hostname"]}:{endpoint_info["port"]}',
+        'version': version,
+        'service': service,
+        'method': method,
+        'ssl_enabled': ssl_enabled
     }
 
 
 def deep_merge(from_dict: dict, into_dict: dict) -> dict:
     for key, value in from_dict.items():
         if isinstance(value, dict):
             node = into_dict.setdefault(key, {})
@@ -217,130 +216,121 @@
 
     return into_dict
 
 
 def parse_timediff_query(query: str) -> datetime:
     try:
         time_info, include_operator = _parse_timediff_from_regex(query)
-        base_dt = _convert_base_time(time_info["base_time"])
+        base_dt = _convert_base_time(time_info['base_time'])
         if include_operator:
-            time_delta = _convert_time_delta(
-                time_info["time_delta_number"], time_info["time_delta_unit"]
-            )
-            if time_info["operator"] == "+":
+            time_delta = _convert_time_delta(time_info['time_delta_number'], time_info['time_delta_unit'])
+            if time_info['operator'] == '+':
                 return base_dt + time_delta
             else:
                 return base_dt - time_delta
         else:
             return base_dt
     except Exception as e:
-        raise ValueError(f"Timediff format is invalid. (value={query})")
+        raise ValueError(f'Timediff format is invalid. (value={query})')
 
 
-def _convert_time_delta(
-    time_delta_number: str, time_delta_unit: str
-) -> datetime.timedelta:
+def _convert_time_delta(time_delta_number: str, time_delta_unit: str) -> datetime.timedelta:
     _time_delta_map = {
-        "s": "seconds",
-        "m": "minutes",
-        "h": "hours",
-        "d": "days",
-        "w": "weeks",
+        's': 'seconds',
+        'm': 'minutes',
+        'h': 'hours',
+        'd': 'days',
+        'w': 'weeks'
     }
 
-    time_delta_params = {_time_delta_map[time_delta_unit]: int(time_delta_number)}
+    time_delta_params = {
+        _time_delta_map[time_delta_unit]: int(time_delta_number)
+    }
 
     return datetime.timedelta(**time_delta_params)
 
 
 def _convert_base_time(time_str: str) -> datetime:
     now = datetime.datetime.utcnow()
-    if time_str == "now":
+    if time_str == 'now':
         return now
-    elif time_str == "now/d":
+    elif time_str == 'now/d':
         return datetime.datetime.combine(now.date(), datetime.time(0))
-    elif time_str == "now/w":
+    elif time_str == 'now/w':
         today = datetime.datetime.combine(now.date(), datetime.time(0))
         return today - datetime.timedelta(days=now.date().weekday())
-    elif time_str == "now/m":
+    elif time_str == 'now/m':
         today = datetime.datetime.combine(now.date(), datetime.time(0))
         return today.replace(day=1)
 
 
 def _parse_timediff_from_regex(query: str) -> Tuple[dict, bool]:
-    p = (
-        r"^\s?(?P<base_time>now(\/[dwm])?)\s?"
-        r"(?P<operator>[+|-])\s?"
-        r"(?P<time_delta_number>\d+)"
-        r"(?P<time_delta_unit>[s|m|h|d|w])\s?$"
-    )
+    p = r'^\s?(?P<base_time>now(\/[dwm])?)\s?' \
+        r'(?P<operator>[+|-])\s?' \
+        r'(?P<time_delta_number>\d+)' \
+        r'(?P<time_delta_unit>[s|m|h|d|w])\s?$'
     rule = re.compile(p)
     match = rule.match(query)
     if match:
         return match.groupdict(), True
     else:
-        if query.strip() not in ["now", "now/d", "now/w", "now/m"]:
-            raise ValueError(f"Timediff format is invalid. (value={query})")
+        if query.strip() not in ['now', 'now/d', 'now/w', 'now/m']:
+            raise ValueError(f'Timediff format is invalid. (value={query})')
 
-        return {"base_time": query.strip()}, False
+        return {'base_time': query.strip()}, False
 
 
 def get_dict_value(data: dict, dotted_key: str, default_value: any = None):
-    if "." in dotted_key:
+    if '.' in dotted_key:
         key, rest = dotted_key.split(".", 1)
 
         if isinstance(data, dict) and key in data:
             if isinstance(data[key], list):
-                list_values = []
-                for value in data[key]:
-                    list_values.append(get_dict_value(value, rest, default_value))
-
-                return list_values
-
+                return get_list_values(data[key], rest, default_value)
             else:
                 return get_dict_value(data[key], rest, default_value)
 
         else:
             return default_value
     else:
         if isinstance(data, dict):
             return data.get(dotted_key, default_value)
         else:
             return default_value
 
 
 def get_list_values(values: list, dotted_key: str, default_value: any = None):
-    match_option = "contain"
+    match_option = 'contain'
     if len(dotted_key) > 1 and dotted_key[0] == "?":
         condition = True
         try:
-            cond_option, rest = dotted_key[1:].split("=>", 1)
-            cond_key, cond_value = cond_option.split(":", 1)
+            cond_option, rest = dotted_key[1:].split('=>', 1)
+            cond_key, cond_value = cond_option.split(':', 1)
         except Exception as e:
             # Syntax Error
             return default_value
 
-        if cond_value[:1] == "=":
-            match_option = "eq"
+        if cond_value[:1] == '=':
+            match_option = 'eq'
             cond_value = cond_value[1:]
 
-        elif cond_value[:1] == "!":
-            match_option = "not"
+        elif cond_value[:1] == '!':
+            match_option = 'not'
             cond_value = cond_value[1:]
 
     else:
         try:
             # Get value by index
-            if "." in dotted_key:
-                index, rest = dotted_key.split(".", 1)
+            if '.' in dotted_key:
+                index, rest = dotted_key.split('.', 1)
                 index = int(index)
                 if index >= len(values):
                     return default_value
                 else:
-                    if rest.strip() != "" and isinstance(values[index], dict):
+                    if rest.strip() != '' and isinstance(values[index], dict):
                         return get_dict_value(values[index], rest, default_value)
                     else:
                         values = values[index]
             else:
                 return values[int(dotted_key)]
 
         except Exception:
@@ -349,18 +339,16 @@
         condition = False
         cond_key = None
         cond_value = None
 
     results = []
     for value in values:
         # Get value from condition
-        if not isinstance(value, dict) or (
-            condition
-            and not _check_condition(match_option, value[cond_key], cond_value)
-        ):
+        if not isinstance(value, dict) \
+                or (condition and not _check_condition(match_option, value[cond_key], cond_value)):
             continue
 
         # Get value from dict key
         result = get_dict_value(value, rest, default_value)
 
         if result:
             if isinstance(result, list):
@@ -377,76 +365,62 @@
         return results
 
 
 def _check_condition(match_option: str, val1, val2):
     val1 = str(val1).lower()
     val2 = str(val2).lower()
 
-    if match_option == "eq":
+    if match_option == 'eq':
         if val1 == val2:
             return True
 
-    elif match_option == "not":
+    elif match_option == 'not':
         if val1.find(val2) < 0:
             return True
 
     else:
         if val1.find(val2) >= 0:
             return True
 
     return False
 
 
-def change_dict_value(
-    data: dict, dotted_key: str, change_value, change_type="value"
-) -> dict:
+def change_dict_value(data: dict, dotted_key: str, change_value, change_type='value') -> dict:
     # change_value = func or value(any type)
-    if "." in dotted_key:
-        key, rest = dotted_key.split(".", 1)
+    if '.' in dotted_key:
+        key, rest = dotted_key.split('.', 1)
         if key in data:
-            if rest.startswith("[]") and isinstance(data[key], list):
+            if rest.startswith('[]') and isinstance(data[key], list):
                 list_data = []
                 for sub_data in data[key]:
-                    if rest.strip() == "[]":
-                        list_data.append(
-                            _change_value_by_type(change_type, sub_data, change_value)
-                        )
+                    if rest.strip() == '[]':
+                        list_data.append(_change_value_by_type(change_type, sub_data, change_value))
                     else:
-                        sub_rest = rest.split(".", 1)[1]
-                        list_data.append(
-                            change_dict_value(
-                                sub_data, sub_rest, change_value, change_type
-                            )
-                        )
+                        sub_rest = rest.split('.', 1)[1]
+                        list_data.append(change_dict_value(sub_data, sub_rest, change_value, change_type))
                 data[key] = list_data
             elif isinstance(data[key], dict):
-                data[key] = change_dict_value(
-                    data[key], rest, change_value, change_type
-                )
+                data[key] = change_dict_value(data[key], rest, change_value, change_type)
     else:
         if dotted_key in data:
-            data[dotted_key] = _change_value_by_type(
-                change_type, data[dotted_key], change_value
-            )
+            data[dotted_key] = _change_value_by_type(change_type, data[dotted_key], change_value)
 
     return data
 
 
 def _change_value_by_type(change_type, original_value, change_value):
-    if change_type == "value":
+    if change_type == 'value':
         return change_value
-    elif change_type == "func":
+    elif change_type == 'func':
         return change_value(original_value)
     else:
         return original_value
 
 
-def date_to_string(
-    value: datetime.date, date_format: str = "%Y-%m-%d"
-) -> Union[str, None]:
+def date_to_string(value: datetime.date, date_format: str = '%Y-%m-%d') -> Union[str, None]:
     if isinstance(value, datetime.date):
         return value.strftime(date_format)
 
     return None
 
 
 def datetime_to_iso8601(value: datetime.datetime) -> Union[str, None]:
@@ -458,15 +432,15 @@
 
 
 def iso8601_to_datetime(value: str) -> Union[datetime.datetime, None]:
     if isinstance(value, str):
         try:
             return isoparse(value)
         except Exception as e:
-            raise ValueError(f"Datetime(ISO8601) format is invalid. (value={value})")
+            raise ValueError(f'Datetime(ISO8601) format is invalid. (value={value})')
 
     return None
 
 
 def iso8601_to_timestamp(value: str) -> Union[int, None]:
     dt = iso8601_to_datetime(value)
     if dt:
@@ -475,27 +449,30 @@
     return None
 
 
 def tags_to_dict(tags: list) -> Union[dict, None]:
     if isinstance(tags, list):
         dict_value = {}
         for tag in tags:
-            dict_value[tag["key"]] = tag["value"]
+            dict_value[tag['key']] = tag['value']
 
         return dict_value
 
     else:
         return None
 
 
 def dict_to_tags(dict_value: dict) -> list:
     tags = []
     if isinstance(dict_value, dict):
         for key, value in dict_value.items():
-            tags.append({"key": key, "value": value})
+            tags.append({
+                'key': key,
+                'value': value
+            })
 
     return tags
 
 
 def dict_to_hash(dict_value: dict) -> str:
     """MD5 hash of a dictionary."""
     dhash = hashlib.md5()
@@ -506,22 +483,20 @@
 
 def string_to_hash(str_value: str) -> str:
     """MD5 hash of a String."""
     dhash = hashlib.md5(str_value.encode("utf-8"))
     return dhash.hexdigest()
 
 
-def change_dict_with_dot_notation(dict_value: dict, key="", dots=None) -> dict:
+def change_dict_with_dot_notation(dict_value: dict, key='', dots=None) -> dict:
     if dots is None:
         dots = {}
     if isinstance(dict_value, dict):
-        for k, v in dict_value.items():
-            change_dict_with_dot_notation(
-                dict_value[k], f"{key}.{k}" if key else k, dots
-            )
+        for (k, v) in dict_value.items():
+            change_dict_with_dot_notation(dict_value[k], f'{key}.{k}' if key else k, dots)
     else:
         dots[key] = dict_value
     return dots
 
 
-if __name__ == "__main__":
+if __name__ == '__main__':
     pass
```

### Comparing `spaceone-core-2.0.84/spaceone_core.egg-info/SOURCES.txt` & `spaceone-core-2.0.9/spaceone_core.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,18 @@
 spaceone/core/fastapi/__init__.py
 spaceone/core/fastapi/api.py
 spaceone/core/fastapi/server.py
 spaceone/core/fastapi/extension/__init__.py
 spaceone/core/fastapi/extension/health.py
 spaceone/core/fastapi/extension/reflection.py
 spaceone/core/handler/__init__.py
+spaceone/core/handler/authentication_api_key_handler.py
 spaceone/core/handler/authentication_handler.py
 spaceone/core/handler/authorization_handler.py
+spaceone/core/handler/event_handler.py
 spaceone/core/handler/mutation_handler.py
 spaceone/core/logger/__init__.py
 spaceone/core/logger/filters/__init__.py
 spaceone/core/logger/filters/error.py
 spaceone/core/logger/filters/exclude.py
 spaceone/core/logger/filters/masking.py
 spaceone/core/logger/filters/message.py
@@ -43,17 +45,14 @@
 spaceone/core/model/base_model.py
 spaceone/core/model/mongo_model/__init__.py
 spaceone/core/model/mongo_model/filter_operator.py
 spaceone/core/model/mongo_model/stat_operator.py
 spaceone/core/opentelemetry/__init__.py
 spaceone/core/opentelemetry/metrics.py
 spaceone/core/opentelemetry/tracer.py
-spaceone/core/plugin/__init__.py
-spaceone/core/plugin/plugin_conf.py
-spaceone/core/plugin/server.py
 spaceone/core/pygrpc/__init__.py
 spaceone/core/pygrpc/api.py
 spaceone/core/pygrpc/client.py
 spaceone/core/pygrpc/message_type.py
 spaceone/core/pygrpc/server.py
 spaceone/core/pygrpc/extension/__init__.py
 spaceone/core/pygrpc/extension/grpc_health.py
@@ -62,14 +61,15 @@
 spaceone/core/queue/redis_queue.py
 spaceone/core/scheduler/__init__.py
 spaceone/core/scheduler/scheduler.py
 spaceone/core/scheduler/server.py
 spaceone/core/scheduler/task_schema.py
 spaceone/core/scheduler/worker.py
 spaceone/core/service/__init__.py
+spaceone/core/service/service.py
 spaceone/core/service/utils.py
 spaceone/core/skeleton/__init__.py
 spaceone/core/skeleton/conf/__init__.py
 spaceone/core/skeleton/conf/global_conf.py
 spaceone/core/skeleton/connector/__init__.py
 spaceone/core/skeleton/error/__init__.py
 spaceone/core/skeleton/info/__init__.py
```

