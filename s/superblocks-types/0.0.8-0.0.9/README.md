# Comparing `tmp/superblocks-types-0.0.8.tar.gz` & `tmp/superblocks-types-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superblocks-types-0.0.8.tar", last modified: Tue May 14 13:21:27 2024, max compression
+gzip compressed data, was "superblocks-types-0.0.9.tar", last modified: Tue May 14 13:30:10 2024, max compression
```

## Comparing `superblocks-types-0.0.8.tar` & `superblocks-types-0.0.9.tar`

### file list

```diff
@@ -1,425 +1,425 @@
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.655608 superblocks-types-0.0.8/
--rw-r--r--   0 joeygreco   (501) staff       (20)      699 2024-05-14 13:21:27.655398 superblocks-types-0.0.8/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)     2857 2023-10-13 17:42:57.000000 superblocks-types-0.0.8/README.md
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.487968 superblocks-types-0.0.8/gen/
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.488148 superblocks-types-0.0.8/gen/py/
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.502975 superblocks-types-0.0.8/gen/py/superblocks_types/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.504179 superblocks-types-0.0.8/gen/py/superblocks_types/agent/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/agent/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.505037 superblocks-types-0.0.8/gen/py/superblocks_types/agent/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/agent/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    11137 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/agent/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4561 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/agent/v1/service_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.505380 superblocks-types-0.0.8/gen/py/superblocks_types/ai/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/ai/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.507863 superblocks-types-0.0.8/gen/py/superblocks_types/ai/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/ai/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     8384 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/ai/v1/ai_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/ai/v1/ai_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3037 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/ai/v1/metadata_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/ai/v1/metadata_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4301 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/ai/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     5292 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/ai/v1/service_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1536 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/ai/v1/vector_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/ai/v1/vector_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.508074 superblocks-types-0.0.8/gen/py/superblocks_types/api/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/api/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.512813 superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    39078 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/api_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/api_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2892 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/blocks_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/blocks_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     7250 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/event_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/event_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     8569 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/integration_auth_service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    10697 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/integration_auth_service_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     7424 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/requests_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/requests_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    27067 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    28875 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/service_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.513388 superblocks-types-0.0.8/gen/py/superblocks_types/auth/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/auth/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.514076 superblocks-types-0.0.8/gen/py/superblocks_types/auth/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/auth/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1475 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/auth/v1/auth_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/auth/v1/auth_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.514338 superblocks-types-0.0.8/gen/py/superblocks_types/buf/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/buf/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.516638 superblocks-types-0.0.8/gen/py/superblocks_types/buf/validate/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/buf/validate/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2027 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/buf/validate/expression_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/buf/validate/expression_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.517495 superblocks-types-0.0.8/gen/py/superblocks_types/buf/validate/priv/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/buf/validate/priv/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2014 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/buf/validate/priv/private_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/buf/validate/priv/private_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)   136631 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/buf/validate/validate_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/buf/validate/validate_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.517861 superblocks-types-0.0.8/gen/py/superblocks_types/cache/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/cache/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.518513 superblocks-types-0.0.8/gen/py/superblocks_types/cache/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/cache/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2647 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/cache/v1/cache_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/cache/v1/cache_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.518825 superblocks-types-0.0.8/gen/py/superblocks_types/common/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/common/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.524536 superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1757 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/api_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/api_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3856 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/common_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/common_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2106 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/errors_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/errors_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2113 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/health_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/health_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     5295 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/language_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/language_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3944 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/plugin_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1230 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/utils_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/utils_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.524840 superblocks-types-0.0.8/gen/py/superblocks_types/event/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/event/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.527447 superblocks-types-0.0.8/gen/py/superblocks_types/event/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/event/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3038 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/event/v1/cloudevent_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/event/v1/cloudevent_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     5946 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/event/v1/event_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/event/v1/event_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1826 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/event/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/event/v1/service_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.529300 superblocks-types-0.0.8/gen/py/superblocks_types/event/v2/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/event/v2/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3038 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/event/v2/cloudevent_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/event/v2/cloudevent_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1602 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/event/v2/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4511 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/event/v2/service_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.529647 superblocks-types-0.0.8/gen/py/superblocks_types/google/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/google/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.531048 superblocks-types-0.0.8/gen/py/superblocks_types/google/api/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/google/api/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1587 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/google/api/annotations_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/google/api/annotations_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2485 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/google/api/http_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/google/api/http_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.531331 superblocks-types-0.0.8/gen/py/superblocks_types/intake/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/intake/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.532062 superblocks-types-0.0.8/gen/py/superblocks_types/intake/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/intake/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1350 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/intake/v1/logs_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/intake/v1/logs_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.532777 superblocks-types-0.0.8/gen/py/superblocks_types/integration/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/integration/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.534674 superblocks-types-0.0.8/gen/py/superblocks_types/integration/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/integration/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3686 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/integration/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/integration/v1/service_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.535986 superblocks-types-0.0.8/gen/py/superblocks_types/kafka/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/kafka/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.539701 superblocks-types-0.0.8/gen/py/superblocks_types/kafka/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/kafka/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2054 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/kafka/v1/kafka_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/kafka/v1/kafka_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.541393 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.542348 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/adls/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/adls/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.549192 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/adls/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/adls/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     5366 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/adls/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/adls/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.554519 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/athena/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/athena/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.562029 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/athena/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/athena/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2936 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/athena/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/athena/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.570160 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/bigquery/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/bigquery/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.583502 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/bigquery/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/bigquery/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2878 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/bigquery/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/bigquery/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.589946 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/cockroachdb/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/cockroachdb/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.591884 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/cockroachdb/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/cockroachdb/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2862 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/cockroachdb/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/cockroachdb/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.596405 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/common/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/common/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.599444 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/common/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/common/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     5867 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/common/v1/auth_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/common/v1/auth_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2979 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/common/v1/metadata_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/common/v1/metadata_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     6526 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/common/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/common/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.599778 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/cosmosdb/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/cosmosdb/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.601269 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/cosmosdb/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/cosmosdb/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     6302 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/cosmosdb/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/cosmosdb/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.601721 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/couchbase/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/couchbase/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.602656 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/couchbase/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/couchbase/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4116 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/couchbase/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/couchbase/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.603035 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/custom/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/custom/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.603943 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/custom/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/custom/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1370 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/custom/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/custom/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.604297 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/databricks/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/databricks/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.605146 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/databricks/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/databricks/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2597 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/databricks/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/databricks/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.605520 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/dynamodb/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/dynamodb/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.606613 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/dynamodb/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/dynamodb/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3747 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/dynamodb/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/dynamodb/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.606927 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/email/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/email/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.607659 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/email/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/email/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1932 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/email/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/email/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.607965 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/gcs/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/gcs/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.608733 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/gcs/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/gcs/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2945 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/gcs/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/gcs/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.609020 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/graphql/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/graphql/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.609810 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/graphql/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/graphql/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2004 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/graphql/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/graphql/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.611148 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/gsheets/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/gsheets/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.612129 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/gsheets/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/gsheets/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2609 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/gsheets/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/gsheets/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.612557 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/javascript/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/javascript/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.613406 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/javascript/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/javascript/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1610 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/javascript/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/javascript/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.613777 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/kafka/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/kafka/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.614728 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/kafka/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/kafka/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     9913 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/kafka/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/kafka/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.615097 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mariadb/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mariadb/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.615815 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mariadb/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mariadb/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2834 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mariadb/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mariadb/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.616097 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mongodb/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mongodb/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.616748 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mongodb/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mongodb/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2306 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mongodb/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mongodb/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.617007 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mssql/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mssql/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.617999 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mssql/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mssql/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3139 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mssql/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mssql/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.618274 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mysql/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mysql/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.618967 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mysql/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mysql/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3139 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mysql/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mysql/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.619399 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/ocr/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/ocr/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.620211 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/ocr/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/ocr/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1370 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/ocr/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/ocr/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.620600 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/openai/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/openai/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.621289 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/openai/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/openai/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     7556 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/openai/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/openai/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.621686 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/oracledb/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/oracledb/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.622445 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/oracledb/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/oracledb/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2457 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/oracledb/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/oracledb/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.622733 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/pinecone/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/pinecone/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.623361 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/pinecone/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/pinecone/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3182 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/pinecone/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/pinecone/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.623695 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/postgresql/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/postgresql/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.624323 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/postgresql/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/postgresql/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3173 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/postgresql/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/postgresql/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.624622 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/python/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/python/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.625223 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/python/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/python/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1583 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/python/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/python/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.625499 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/redis/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/redis/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.626408 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/redis/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/redis/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    13985 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/redis/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/redis/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.626684 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/redshift/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/redshift/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.627261 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/redshift/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/redshift/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2756 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/redshift/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/redshift/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.627543 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/restapi/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/restapi/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.628369 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/restapi/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/restapi/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2099 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/restapi/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/restapi/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.628755 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/restapiintegration/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/restapiintegration/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.629405 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/restapiintegration/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/restapiintegration/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2505 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/restapiintegration/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/restapiintegration/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.629705 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/rockset/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/rockset/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.630459 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/rockset/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/rockset/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2800 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/rockset/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/rockset/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.630772 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/s3/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/s3/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.631440 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/s3/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/s3/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2835 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/s3/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/s3/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.631769 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/salesforce/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/salesforce/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.632501 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/salesforce/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/salesforce/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     5285 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/salesforce/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/salesforce/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.633165 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/smtp/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/smtp/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.634079 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/smtp/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/smtp/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2547 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/smtp/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/smtp/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.634387 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/snowflake/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/snowflake/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.635060 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/snowflake/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/snowflake/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2887 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/snowflake/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/snowflake/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.635388 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/workflow/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/workflow/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.636300 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/workflow/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/workflow/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2676 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/workflow/v1/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/workflow/v1/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.637981 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/workflow/v2/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/workflow/v2/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1458 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/workflow/v2/plugin_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/plugins/workflow/v2/plugin_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.638268 superblocks-types-0.0.8/gen/py/superblocks_types/protoc_gen_openapiv2/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/protoc_gen_openapiv2/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.640504 superblocks-types-0.0.8/gen/py/superblocks_types/protoc_gen_openapiv2/options/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/protoc_gen_openapiv2/options/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     2312 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/protoc_gen_openapiv2/options/annotations_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/protoc_gen_openapiv2/options/annotations_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    20165 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/protoc_gen_openapiv2/options/openapiv2_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/protoc_gen_openapiv2/options/openapiv2_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.641315 superblocks-types-0.0.8/gen/py/superblocks_types/secrets/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/secrets/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.642797 superblocks-types-0.0.8/gen/py/superblocks_types/secrets/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/secrets/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     7587 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/secrets/v1/secrets_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/secrets/v1/secrets_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4860 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/secrets/v1/store_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4575 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/secrets/v1/store_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.643274 superblocks-types-0.0.8/gen/py/superblocks_types/security/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/security/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.644955 superblocks-types-0.0.8/gen/py/superblocks_types/security/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/security/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3137 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/security/v1/requests_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/security/v1/requests_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4814 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/security/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4515 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/security/v1/service_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.645321 superblocks-types-0.0.8/gen/py/superblocks_types/store/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/store/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.646960 superblocks-types-0.0.8/gen/py/superblocks_types/store/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/store/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3592 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/store/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     4409 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/store/v1/service_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1667 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/store/v1/store_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/store/v1/store_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.647346 superblocks-types-0.0.8/gen/py/superblocks_types/superblocks/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/superblocks/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.648407 superblocks-types-0.0.8/gen/py/superblocks_types/superblocks/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/superblocks/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1904 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/superblocks/v1/options_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/superblocks/v1/options_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.648777 superblocks-types-0.0.8/gen/py/superblocks_types/syncer/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/syncer/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.650452 superblocks-types-0.0.8/gen/py/superblocks_types/syncer/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/syncer/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     8907 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/syncer/v1/service_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    11798 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/syncer/v1/service_pb2_grpc.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     3378 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/syncer/v1/syncer_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/syncer/v1/syncer_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.650773 superblocks-types-0.0.8/gen/py/superblocks_types/transport/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/transport/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.651691 superblocks-types-0.0.8/gen/py/superblocks_types/transport/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/transport/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    13204 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/transport/v1/transport_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/transport/v1/transport_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.652054 superblocks-types-0.0.8/gen/py/superblocks_types/utils/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/utils/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.652822 superblocks-types-0.0.8/gen/py/superblocks_types/utils/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/utils/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1277 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/utils/v1/utils_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/utils/v1/utils_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.654030 superblocks-types-0.0.8/gen/py/superblocks_types/validate/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/validate/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    15601 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/validate/validate_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/validate/validate_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.654329 superblocks-types-0.0.8/gen/py/superblocks_types/worker/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/worker/__init__.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.655027 superblocks-types-0.0.8/gen/py/superblocks_types/worker/v1/
--rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/worker/v1/__init__.py
--rw-r--r--   0 joeygreco   (501) staff       (20)     1976 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/worker/v1/step_executor_pb2.py
--rw-r--r--   0 joeygreco   (501) staff       (20)    10048 2024-05-14 13:20:28.000000 superblocks-types-0.0.8/gen/py/superblocks_types/worker/v1/step_executor_pb2_grpc.py
-drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:21:27.503965 superblocks-types-0.0.8/gen/py/superblocks_types.egg-info/
--rw-r--r--   0 joeygreco   (501) staff       (20)      699 2024-05-14 13:21:27.000000 superblocks-types-0.0.8/gen/py/superblocks_types.egg-info/PKG-INFO
--rw-r--r--   0 joeygreco   (501) staff       (20)    16191 2024-05-14 13:21:27.000000 superblocks-types-0.0.8/gen/py/superblocks_types.egg-info/SOURCES.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-14 13:21:27.000000 superblocks-types-0.0.8/gen/py/superblocks_types.egg-info/dependency_links.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)       18 2024-05-14 13:21:27.000000 superblocks-types-0.0.8/gen/py/superblocks_types.egg-info/top_level.txt
--rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-14 13:21:27.655724 superblocks-types-0.0.8/setup.cfg
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.152410 superblocks-types-0.0.9/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      699 2024-05-14 13:30:10.152206 superblocks-types-0.0.9/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2857 2023-10-13 17:42:57.000000 superblocks-types-0.0.9/README.md
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.071246 superblocks-types-0.0.9/gen/
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.071428 superblocks-types-0.0.9/gen/py/
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.086675 superblocks-types-0.0.9/gen/py/superblocks_types/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.087649 superblocks-types-0.0.9/gen/py/superblocks_types/agent/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/agent/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.088339 superblocks-types-0.0.9/gen/py/superblocks_types/agent/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/agent/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    11191 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/agent/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4579 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/agent/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.088651 superblocks-types-0.0.9/gen/py/superblocks_types/ai/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/ai/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.091393 superblocks-types-0.0.9/gen/py/superblocks_types/ai/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/ai/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     8456 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/ai/v1/ai_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/ai/v1/ai_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3109 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/ai/v1/metadata_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/ai/v1/metadata_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4409 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/ai/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5328 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/ai/v1/service_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1536 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/ai/v1/vector_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/ai/v1/vector_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.091641 superblocks-types-0.0.9/gen/py/superblocks_types/api/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/api/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.095329 superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    39816 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/api_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/api_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2928 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/blocks_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/blocks_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     7304 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/event_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/event_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     8677 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/integration_auth_service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    10715 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/integration_auth_service_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     7514 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/requests_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/requests_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    27301 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    28911 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.095988 superblocks-types-0.0.9/gen/py/superblocks_types/auth/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/auth/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.096625 superblocks-types-0.0.9/gen/py/superblocks_types/auth/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/auth/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1475 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/auth/v1/auth_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/auth/v1/auth_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.096980 superblocks-types-0.0.9/gen/py/superblocks_types/buf/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/buf/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.099060 superblocks-types-0.0.9/gen/py/superblocks_types/buf/validate/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/buf/validate/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2027 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/buf/validate/expression_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/buf/validate/expression_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.099720 superblocks-types-0.0.9/gen/py/superblocks_types/buf/validate/priv/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/buf/validate/priv/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2014 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/buf/validate/priv/private_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/buf/validate/priv/private_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)   136667 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/buf/validate/validate_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/buf/validate/validate_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.099912 superblocks-types-0.0.9/gen/py/superblocks_types/cache/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/cache/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.100364 superblocks-types-0.0.9/gen/py/superblocks_types/cache/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/cache/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2647 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/cache/v1/cache_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/cache/v1/cache_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.100541 superblocks-types-0.0.9/gen/py/superblocks_types/common/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/common/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.103739 superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1757 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/api_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/api_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3892 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/common_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/common_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2106 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/errors_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/errors_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2113 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/health_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/health_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5295 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/language_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/language_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3944 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/plugin_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1230 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/utils_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/utils_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.103947 superblocks-types-0.0.9/gen/py/superblocks_types/event/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/event/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.105319 superblocks-types-0.0.9/gen/py/superblocks_types/event/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/event/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3038 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/event/v1/cloudevent_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/event/v1/cloudevent_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5982 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/event/v1/event_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/event/v1/event_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1826 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/event/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/event/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.106194 superblocks-types-0.0.9/gen/py/superblocks_types/event/v2/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/event/v2/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3038 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/event/v2/cloudevent_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/event/v2/cloudevent_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1602 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/event/v2/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4511 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/event/v2/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.106410 superblocks-types-0.0.9/gen/py/superblocks_types/google/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/google/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.107483 superblocks-types-0.0.9/gen/py/superblocks_types/google/api/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/google/api/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1605 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/google/api/annotations_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2485 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/google/api/http_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/google/api/http_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.107706 superblocks-types-0.0.9/gen/py/superblocks_types/intake/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/intake/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.108215 superblocks-types-0.0.9/gen/py/superblocks_types/intake/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/intake/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1350 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/intake/v1/logs_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/intake/v1/logs_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.108426 superblocks-types-0.0.9/gen/py/superblocks_types/integration/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/integration/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.108943 superblocks-types-0.0.9/gen/py/superblocks_types/integration/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/integration/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3704 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/integration/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/integration/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.109158 superblocks-types-0.0.9/gen/py/superblocks_types/kafka/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/kafka/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.109661 superblocks-types-0.0.9/gen/py/superblocks_types/kafka/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/kafka/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2054 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/kafka/v1/kafka_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/kafka/v1/kafka_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.109871 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.110025 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/adls/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/adls/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.110544 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/adls/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/adls/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5402 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/adls/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/adls/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.110758 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/athena/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/athena/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.111271 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/athena/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/athena/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2954 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/athena/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/athena/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.111514 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/bigquery/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/bigquery/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.112010 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/bigquery/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/bigquery/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2878 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/bigquery/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/bigquery/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.112219 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/cockroachdb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/cockroachdb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.112698 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/cockroachdb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/cockroachdb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2862 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/cockroachdb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/cockroachdb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.112934 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/common/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/common/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.114407 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/common/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/common/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5867 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/common/v1/auth_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/common/v1/auth_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2979 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/common/v1/metadata_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/common/v1/metadata_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     6544 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/common/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/common/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.114643 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/cosmosdb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/cosmosdb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.115178 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/cosmosdb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/cosmosdb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     6338 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/cosmosdb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/cosmosdb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.115378 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/couchbase/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/couchbase/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.115875 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/couchbase/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/couchbase/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4134 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/couchbase/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/couchbase/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.116073 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/custom/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/custom/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.116522 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/custom/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/custom/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1370 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/custom/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/custom/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.116737 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/databricks/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/databricks/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.117313 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/databricks/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/databricks/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2615 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/databricks/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/databricks/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.117550 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/dynamodb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/dynamodb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.118233 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/dynamodb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/dynamodb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3747 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/dynamodb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/dynamodb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.118481 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/email/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/email/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.118982 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/email/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/email/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1932 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/email/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/email/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.119164 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/gcs/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/gcs/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.119630 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/gcs/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/gcs/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2945 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/gcs/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/gcs/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.119855 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/graphql/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/graphql/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.120363 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/graphql/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/graphql/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2022 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/graphql/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/graphql/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.120559 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/gsheets/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/gsheets/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.121068 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/gsheets/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/gsheets/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2609 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/gsheets/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/gsheets/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.121267 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/javascript/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/javascript/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.121732 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/javascript/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/javascript/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1610 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/javascript/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/javascript/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.121933 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/kafka/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/kafka/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.122649 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/kafka/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/kafka/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     9967 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/kafka/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/kafka/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.122922 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mariadb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mariadb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.123587 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mariadb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mariadb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2834 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mariadb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mariadb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.123856 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mongodb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mongodb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.124528 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mongodb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mongodb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2306 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mongodb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mongodb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.124779 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mssql/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mssql/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.125258 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mssql/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mssql/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3139 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mssql/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mssql/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.125457 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mysql/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mysql/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.126090 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mysql/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mysql/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3139 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mysql/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mysql/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.126316 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/ocr/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/ocr/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.126865 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/ocr/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/ocr/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1370 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/ocr/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/ocr/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.127111 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/openai/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/openai/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.127629 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/openai/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/openai/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     7556 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/openai/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/openai/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.127856 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/oracledb/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/oracledb/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.128400 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/oracledb/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/oracledb/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2475 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/oracledb/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/oracledb/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.128624 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/pinecone/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/pinecone/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.129137 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/pinecone/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/pinecone/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3200 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/pinecone/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/pinecone/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.129348 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/postgresql/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/postgresql/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.129993 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/postgresql/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/postgresql/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3173 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/postgresql/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/postgresql/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.130253 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/python/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/python/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.130878 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/python/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/python/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1583 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/python/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/python/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.131139 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/redis/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/redis/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.131835 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/redis/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/redis/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    14003 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/redis/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/redis/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.132115 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/redshift/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/redshift/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.132697 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/redshift/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/redshift/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2756 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/redshift/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/redshift/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.132955 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/restapi/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/restapi/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.133536 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/restapi/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/restapi/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2117 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/restapi/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/restapi/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.133788 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/restapiintegration/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/restapiintegration/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.134365 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/restapiintegration/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/restapiintegration/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2523 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/restapiintegration/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/restapiintegration/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.134633 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/rockset/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/rockset/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.135201 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/rockset/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/rockset/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2800 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/rockset/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/rockset/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.135474 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/s3/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/s3/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.136051 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/s3/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/s3/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2835 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/s3/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/s3/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.136338 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/salesforce/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/salesforce/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.136832 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/salesforce/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/salesforce/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     5321 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/salesforce/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/salesforce/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.137063 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/smtp/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/smtp/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.137554 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/smtp/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/smtp/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2565 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/smtp/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/smtp/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.137759 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/snowflake/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/snowflake/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.138314 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/snowflake/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/snowflake/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2887 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/snowflake/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/snowflake/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.138521 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/workflow/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/workflow/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.139138 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/workflow/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/workflow/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2694 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/workflow/v1/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/workflow/v1/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.139720 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/workflow/v2/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/workflow/v2/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1476 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/workflow/v2/plugin_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/plugins/workflow/v2/plugin_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.139928 superblocks-types-0.0.9/gen/py/superblocks_types/protoc_gen_openapiv2/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/protoc_gen_openapiv2/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.141281 superblocks-types-0.0.9/gen/py/superblocks_types/protoc_gen_openapiv2/options/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/protoc_gen_openapiv2/options/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     2330 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/protoc_gen_openapiv2/options/annotations_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/protoc_gen_openapiv2/options/annotations_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    20165 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/protoc_gen_openapiv2/options/openapiv2_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/protoc_gen_openapiv2/options/openapiv2_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.141535 superblocks-types-0.0.9/gen/py/superblocks_types/secrets/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/secrets/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.142484 superblocks-types-0.0.9/gen/py/superblocks_types/secrets/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/secrets/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     7641 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/secrets/v1/secrets_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/secrets/v1/secrets_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4950 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/secrets/v1/store_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4593 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/secrets/v1/store_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.142725 superblocks-types-0.0.9/gen/py/superblocks_types/security/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/security/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.143948 superblocks-types-0.0.9/gen/py/superblocks_types/security/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/security/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3155 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/security/v1/requests_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/security/v1/requests_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4886 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/security/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4533 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/security/v1/service_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.144186 superblocks-types-0.0.9/gen/py/superblocks_types/store/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/store/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.145386 superblocks-types-0.0.9/gen/py/superblocks_types/store/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/store/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3664 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/store/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     4427 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/store/v1/service_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1685 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/store/v1/store_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/store/v1/store_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.145667 superblocks-types-0.0.9/gen/py/superblocks_types/superblocks/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/superblocks/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.146350 superblocks-types-0.0.9/gen/py/superblocks_types/superblocks/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/superblocks/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1904 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/superblocks/v1/options_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/superblocks/v1/options_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.146581 superblocks-types-0.0.9/gen/py/superblocks_types/syncer/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/syncer/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.148047 superblocks-types-0.0.9/gen/py/superblocks_types/syncer/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/syncer/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     9033 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/syncer/v1/service_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    11834 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/syncer/v1/service_pb2_grpc.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     3432 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/syncer/v1/syncer_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/syncer/v1/syncer_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.148342 superblocks-types-0.0.9/gen/py/superblocks_types/transport/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/transport/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.149161 superblocks-types-0.0.9/gen/py/superblocks_types/transport/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/transport/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    13384 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/transport/v1/transport_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/transport/v1/transport_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.149485 superblocks-types-0.0.9/gen/py/superblocks_types/utils/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/utils/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.150052 superblocks-types-0.0.9/gen/py/superblocks_types/utils/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/utils/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1277 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/utils/v1/utils_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/utils/v1/utils_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.150814 superblocks-types-0.0.9/gen/py/superblocks_types/validate/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/validate/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    15601 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/validate/validate_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)      159 2024-05-14 13:29:25.000000 superblocks-types-0.0.9/gen/py/superblocks_types/validate/validate_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.151052 superblocks-types-0.0.9/gen/py/superblocks_types/worker/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/worker/__init__.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.151753 superblocks-types-0.0.9/gen/py/superblocks_types/worker/v1/
+-rw-r--r--   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/worker/v1/__init__.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)     1994 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/worker/v1/step_executor_pb2.py
+-rw-r--r--   0 joeygreco   (501) staff       (20)    10084 2024-05-14 13:29:26.000000 superblocks-types-0.0.9/gen/py/superblocks_types/worker/v1/step_executor_pb2_grpc.py
+drwxr-xr-x   0 joeygreco   (501) staff       (20)        0 2024-05-14 13:30:10.087444 superblocks-types-0.0.9/gen/py/superblocks_types.egg-info/
+-rw-r--r--   0 joeygreco   (501) staff       (20)      699 2024-05-14 13:30:10.000000 superblocks-types-0.0.9/gen/py/superblocks_types.egg-info/PKG-INFO
+-rw-r--r--   0 joeygreco   (501) staff       (20)    16191 2024-05-14 13:30:10.000000 superblocks-types-0.0.9/gen/py/superblocks_types.egg-info/SOURCES.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)        1 2024-05-14 13:30:10.000000 superblocks-types-0.0.9/gen/py/superblocks_types.egg-info/dependency_links.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       18 2024-05-14 13:30:10.000000 superblocks-types-0.0.9/gen/py/superblocks_types.egg-info/top_level.txt
+-rw-r--r--   0 joeygreco   (501) staff       (20)       38 2024-05-14 13:30:10.152478 superblocks-types-0.0.9/setup.cfg
```

### Comparing `superblocks-types-0.0.8/PKG-INFO` & `superblocks-types-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-types
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Official Python Types for Superblocks
 Home-page: https://github.com/superblocksteam/types
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks types
 Requires-Python: >=3.10
```

### Comparing `superblocks-types-0.0.8/README.md` & `superblocks-types-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/agent/v1/service_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/agent/v1/service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from common.v1 import common_pb2 as common_dot_v1_dot_common__pb2
-from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from superblocks_types.common.v1 import common_pb2 as common_dot_v1_dot_common__pb2
+from superblocks_types.google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
+from superblocks_types.protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x61gent/v1/service.proto\x12\x08\x61gent.v1\x1a\x16\x63ommon/v1/common.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\"\xc0\x03\n\x13RegistrationRequest\x12Z\n\x0fplugin_versions\x18\x01 \x03(\x0b\x32\x31.agent.v1.RegistrationRequest.PluginVersionsEntryR\x0epluginVersions\x12\x12\n\x04type\x18\x02 \x01(\x05R\x04type\x12;\n\x04tags\x18\x03 \x03(\x0b\x32\'.agent.v1.RegistrationRequest.TagsEntryR\x04tags\x12$\n\x0esigning_key_id\x18\x04 \x01(\tR\x0csigningKeyId\x12\x30\n\x14verification_key_ids\x18\x05 \x03(\tR\x12verificationKeyIds\x1aX\n\x13PluginVersionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x15.agent.v1.VersionListR\x05value:\x02\x38\x01\x1aJ\n\tTagsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x11.agent.v1.TagListR\x05value:\x02\x38\x01\"\xa2\t\n\x14RegistrationResponse\x12P\n\rresponse_meta\x18\x01 \x01(\x0b\x32+.agent.v1.RegistrationResponse.ResponseMetaR\x0cresponseMeta\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.agent.v1.RegistrationResponse.ResponseBodyR\x04\x64\x61ta\x1aZ\n\x0cResponseMeta\x12\x16\n\x06status\x18\x01 \x01(\x05R\x06status\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\x12\x18\n\x07success\x18\x03 \x01(\x08R\x07success\x1a\x9a\x07\n\x0cResponseBody\x12G\n\x05\x61gent\x18\x01 \x01(\x0b\x32\x31.agent.v1.RegistrationResponse.ResponseBody.AgentR\x05\x61gent\x12!\n\x0c\x62illing_plan\x18\x02 \x01(\tR\x0b\x62illingPlan\x12\'\n\x0forganization_id\x18\x03 \x01(\tR\x0eorganizationId\x12+\n\x11organization_name\x18\x04 \x01(\tR\x10organizationName\x1a\xc7\x05\n\x05\x41gent\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x10\n\x03key\x18\x02 \x01(\tR\x03key\x12 \n\x0b\x65nvironment\x18\x03 \x01(\tR\x0b\x65nvironment\x12\x16\n\x06status\x18\x04 \x01(\tR\x06status\x12\x18\n\x07version\x18\x05 \x01(\tR\x07version\x12)\n\x10version_external\x18\x06 \x01(\tR\x0fversionExternal\x12\x8a\x01\n\x19supported_plugin_versions\x18\x07 \x03(\x0b\x32N.agent.v1.RegistrationResponse.ResponseBody.Agent.SupportedPluginVersionsEntryR\x17supportedPluginVersions\x12\x10\n\x03url\x18\x08 \x01(\tR\x03url\x12\x12\n\x04type\x18\t \x01(\x05R\x04type\x12\x34\n\x07updated\x18\n \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07updated\x12\x34\n\x07\x63reated\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12O\n\x04tags\x18\x0c \x03(\x0b\x32;.agent.v1.RegistrationResponse.ResponseBody.Agent.TagsEntryR\x04tags\x1a\x61\n\x1cSupportedPluginVersionsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x15.agent.v1.VersionListR\x05value:\x02\x38\x01\x1aJ\n\tTagsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\'\n\x05value\x18\x02 \x01(\x0b\x32\x11.agent.v1.TagListR\x05value:\x02\x38\x01\")\n\x0bVersionList\x12\x1a\n\x08versions\x18\x01 \x03(\tR\x08versions\"\x1d\n\x07TagList\x12\x12\n\x04tags\x18\x01 \x03(\tR\x04tags\"\xb7\x0b\n\x0f\x41uditLogRequest\x12\x41\n\naudit_logs\x18\x01 \x03(\x0b\x32\".agent.v1.AuditLogRequest.AuditLogR\tauditLogs\x1a\xe0\n\n\x08\x41uditLog\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1b\n\tentity_id\x18\x02 \x01(\tR\x08\x65ntityId\x12V\n\x0b\x65ntity_type\x18\x03 \x01(\x0e\x32\x35.agent.v1.AuditLogRequest.AuditLog.AuditLogEntityTypeR\nentityType\x12\'\n\x0forganization_id\x18\x04 \x01(\tR\x0eorganizationId\x12\x1f\n\x0bis_deployed\x18\x05 \x01(\x08R\nisDeployed\x12\x16\n\x06source\x18\x06 \x01(\tR\x06source\x12\x16\n\x06target\x18\x07 \x01(\tR\x06target\x12H\n\x04type\x18\x08 \x01(\x0e\x32\x34.agent.v1.AuditLogRequest.AuditLog.AuditLogEventTypeR\x04type\x12\x1e\n\x08\x61gent_id\x18\t \x01(\tH\x00R\x07\x61gentId\x88\x01\x01\x12L\n\x06status\x18\n \x01(\x0e\x32/.agent.v1.AuditLogRequest.AuditLog.ApiRunStatusH\x01R\x06status\x88\x01\x01\x12\x19\n\x05\x65rror\x18\x0b \x01(\tH\x02R\x05\x65rror\x88\x01\x01\x12l\n\x14\x61pi_location_context\x18\x0c \x01(\x0b\x32\x35.agent.v1.AuditLogRequest.AuditLog.ApiLocationContextH\x03R\x12\x61piLocationContext\x88\x01\x01\x12K\n\napi_timing\x18\r \x01(\x0b\x32,.agent.v1.AuditLogRequest.AuditLog.ApiTimingR\tapiTiming\x12\x35\n\tuser_type\x18\x0e \x01(\x0e\x32\x13.common.v1.UserTypeH\x04R\x08userType\x88\x01\x01\x12#\n\ntargetName\x18\x0f \x01(\tH\x05R\ntargetName\x88\x01\x01\x1a;\n\x12\x41piLocationContext\x12%\n\x0e\x61pplication_id\x18\x01 \x01(\tR\rapplicationId\x1a@\n\tApiTiming\x12\x14\n\x05start\x18\x01 \x01(\x03R\x05start\x12\x15\n\x03\x65nd\x18\x02 \x01(\x03H\x00R\x03\x65nd\x88\x01\x01\x42\x06\n\x04_end\"e\n\x0c\x41piRunStatus\x12\x1e\n\x1a\x41PI_RUN_STATUS_UNSPECIFIED\x10\x00\x12\x1a\n\x16\x41PI_RUN_STATUS_SUCCESS\x10\x01\x12\x19\n\x15\x41PI_RUN_STATUS_FAILED\x10\x02\"\xcf\x01\n\x12\x41uditLogEntityType\x12%\n!AUDIT_LOG_ENTITY_TYPE_UNSPECIFIED\x10\x00\x12%\n!AUDIT_LOG_ENTITY_TYPE_APPLICATION\x10\x01\x12\"\n\x1e\x41UDIT_LOG_ENTITY_TYPE_WORKFLOW\x10\x02\x12\'\n#AUDIT_LOG_ENTITY_TYPE_SCHEDULED_JOB\x10\x03\x12\x1e\n\x1a\x41UDIT_LOG_ENTITY_TYPE_STEP\x10\x04\"[\n\x11\x41uditLogEventType\x12$\n AUDIT_LOG_EVENT_TYPE_UNSPECIFIED\x10\x00\x12 \n\x1c\x41UDIT_LOG_EVENT_TYPE_API_RUN\x10\x01\x42\x0b\n\t_agent_idB\t\n\x07_statusB\x08\n\x06_errorB\x17\n\x15_api_location_contextB\x0c\n\n_user_typeB\r\n\x0b_targetName2\xe9\x01\n\x0c\x41gentService\x12v\n\x08Register\x12\x1d.agent.v1.RegistrationRequest\x1a\x1e.agent.v1.RegistrationResponse\"+\x92\x41\n*\x08Register\x82\xd3\xe4\x93\x02\x18\"\x13/v1/agents/register:\x01*\x12\x61\n\x05\x41udit\x12\x19.agent.v1.AuditLogRequest\x1a\x16.google.protobuf.Empty\"%\x92\x41\x07*\x05\x41udit\x82\xd3\xe4\x93\x02\x15\"\x10/v2/agents/audit:\x01*BzZ0github.com/superblocksteam/types/gen/go/agent/v1\x92\x41\x45\x12\x1c\n\x15Superblocks Agent API2\x03\x31.0*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'agent.v1.service_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/agent/v1/service_pb2_grpc.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/agent/v1/service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from agent.v1 import service_pb2 as agent_dot_v1_dot_service__pb2
+from superblocks_types.agent.v1 import service_pb2 as agent_dot_v1_dot_service__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
 class AgentServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/ai/v1/ai_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/ai/v1/ai_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from common.v1 import language_pb2 as common_dot_v1_dot_language__pb2
-from common.v1 import utils_pb2 as common_dot_v1_dot_utils__pb2
-from validate import validate_pb2 as validate_dot_validate__pb2
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.common.v1 import language_pb2 as common_dot_v1_dot_language__pb2
+from superblocks_types.common.v1 import utils_pb2 as common_dot_v1_dot_utils__pb2
+from superblocks_types.validate import validate_pb2 as validate_dot_validate__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x61i/v1/ai.proto\x12\x05\x61i.v1\x1a\x18\x63ommon/v1/language.proto\x1a\x15\x63ommon/v1/utils.proto\x1a\x17validate/validate.proto\x1a\x1b\x62uf/validate/validate.proto\x1a\x1cgoogle/protobuf/struct.proto\"T\n\x07Message\x12\x1f\n\x04role\x18\x01 \x01(\x0e\x32\x0b.ai.v1.RoleR\x04role\x12(\n\x07\x63ontent\x18\x02 \x01(\tB\x0e\xfa\x42\x04r\x02\x10\x01\xbaH\x04r\x02\x10\x01R\x07\x63ontent\"\xe0\t\n\x04Task\x12\x32\n\x08optimize\x18\x01 \x01(\x0b\x32\x14.ai.v1.Task.OptimizeH\x00R\x08optimize\x12&\n\x04\x65\x64it\x18\x02 \x01(\x0b\x32\x10.ai.v1.Task.EditH\x00R\x04\x65\x64it\x12/\n\x07\x65xplain\x18\x03 \x01(\x0b\x32\x13.ai.v1.Task.ExplainH\x00R\x07\x65xplain\x12,\n\x06\x63reate\x18\x04 \x01(\x0b\x32\x12.ai.v1.Task.CreateH\x00R\x06\x63reate\x12)\n\x05\x64\x65\x62ug\x18\x05 \x01(\x0b\x32\x11.ai.v1.Task.DebugH\x00R\x05\x64\x65\x62ug\x12\x35\n\ttranspile\x18\x07 \x01(\x0b\x32\x15.ai.v1.Task.TranspileH\x00R\ttranspile\x12&\n\x04mock\x18\x08 \x01(\x0b\x32\x10.ai.v1.Task.MockH\x00R\x04mock\x12(\n\x07history\x18\x06 \x03(\x0b\x32\x0e.ai.v1.MessageR\x07history\x1a\n\n\x08Optimize\x1a\x07\n\x05\x44\x65\x62ug\x1a\x0b\n\tTranspile\x1a\xad\x02\n\x04\x45\x64it\x12\x16\n\x06prompt\x18\x01 \x01(\tR\x06prompt\x12%\n\x06syntax\x18\x02 \x01(\x0e\x32\r.ai.v1.SyntaxR\x06syntax\x12\x18\n\x07snippet\x18\x03 \x01(\tR\x07snippet\x12\x32\n\x07\x63ontext\x18\x04 \x01(\x0b\x32\x18.ai.v1.Task.Edit.ContextR\x07\x63ontext\x1a\x97\x01\n\x07\x43ontext\x12\x35\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.google.protobuf.StructH\x00R\x08metadata\x12\x44\n\x11\x63onfiguration_ids\x18\x02 \x01(\x0b\x32\x15.common.v1.StringListH\x00R\x10\x63onfigurationIdsB\x0f\n\rconfiguration\x1a\x97\x02\n\x06\x43reate\x12\x16\n\x06prompt\x18\x01 \x01(\tR\x06prompt\x12%\n\x06syntax\x18\x02 \x01(\x0e\x32\r.ai.v1.SyntaxR\x06syntax\x12\x34\n\x07\x63ontext\x18\x03 \x01(\x0b\x32\x1a.ai.v1.Task.Create.ContextR\x07\x63ontext\x1a\x97\x01\n\x07\x43ontext\x12\x35\n\x08metadata\x18\x01 \x01(\x0b\x32\x17.google.protobuf.StructH\x00R\x08metadata\x12\x44\n\x11\x63onfiguration_ids\x18\x02 \x01(\x0b\x32\x15.common.v1.StringListH\x00R\x10\x63onfigurationIdsB\x0f\n\rconfiguration\x1a\x97\x01\n\x07\x45xplain\x12%\n\x06syntax\x18\x01 \x01(\x0e\x32\r.ai.v1.SyntaxR\x06syntax\x12\x18\n\x07snippet\x18\x02 \x01(\tR\x07snippet\x12\x1a\n\x08\x63ontents\x18\x03 \x01(\tR\x08\x63ontents\x12/\n\x08language\x18\x04 \x01(\x0e\x32\x13.common.v1.LanguageR\x08language\x1a[\n\x04Mock\x12%\n\x06syntax\x18\x01 \x01(\x0e\x32\r.ai.v1.SyntaxR\x06syntax\x12\x14\n\x05shape\x18\x02 \x01(\tR\x05shape\x12\x16\n\x06prompt\x18\x03 \x01(\tR\x06promptB\x06\n\x04kind*K\n\x03LLM\x12\x13\n\x0fLLM_UNSPECIFIED\x10\x00\x12\x0e\n\nLLM_OPENAI\x10\x01\x12\x11\n\rLLM_ANTHROPIC\x10\x02\x12\x0c\n\x08LLM_MOCK\x10\x03*\x8e\x08\n\x05MODEL\x12\x15\n\x11MODEL_UNSPECIFIED\x10\x00\x12\x1d\n\x19MODEL_ANTHROPIC_CLAUDE_V1\x10\x01\x12\x1f\n\x1bMODEL_ANTHROPIC_CLAUDE_V1_0\x10\x02\x12\x1f\n\x1bMODEL_ANTHROPIC_CLAUDE_V1_2\x10\x03\x12%\n!MODEL_ANTHROPIC_CLAUDE_INSTANT_V1\x10\x04\x12\'\n#MODEL_ANTHROPIC_CLAUDE_INSTANT_V1_0\x10\x05\x12\x1c\n\x18MODEL_OPENAI_GPT432K0314\x10\x06\x12\x1c\n\x18MODEL_OPENAI_GPT432K0613\x10\x1a\x12\x18\n\x14MODEL_OPENAI_GPT432K\x10\x07\x12\x19\n\x15MODEL_OPENAI_GPT40314\x10\x08\x12\x19\n\x15MODEL_OPENAI_GPT40613\x10\x1b\x12\x15\n\x11MODEL_OPENAI_GPT4\x10\t\x12\"\n\x1eMODEL_OPENAI_GPT3_5_TURBO_0301\x10\n\x12\"\n\x1eMODEL_OPENAI_GPT3_5_TURBO_0613\x10\x1c\x12\x1d\n\x19MODEL_OPENAI_GPT3_5_TURBO\x10\x0b\x12!\n\x1dMODEL_OPENAI_GPT3_5_TURBO_16K\x10\x1d\x12&\n\"MODEL_OPENAI_GPT3_5_TURBO_16K_0613\x10\x1e\x12&\n\"MODEL_OPENAI_GPT3_TEXT_DAVINCI_003\x10\x0c\x12&\n\"MODEL_OPENAI_GPT3_TEXT_DAVINCI_002\x10\r\x12$\n MODEL_OPENAI_GPT3_TEXT_CURIE_001\x10\x0e\x12&\n\"MODEL_OPENAI_GPT3_TEXT_BAGGAGE_001\x10\x0f\x12\"\n\x1eMODEL_OPENAI_GPT3_TEXT_ADA_001\x10\x10\x12&\n\"MODEL_OPENAI_GPT3_TEXT_DAVINCI_001\x10\x11\x12+\n\'MODEL_OPENAI_GPT3_DAVINCI_INSTRUCT_BETA\x10\x12\x12\x1d\n\x19MODEL_OPENAI_GPT3_DAVINCI\x10\x13\x12)\n%MODEL_OPENAI_GPT3_CURIE_INSTRUCT_BETA\x10\x14\x12\x1b\n\x17MODEL_OPENAI_GPT3_CURIE\x10\x15\x12\x19\n\x15MODEL_OPENAI_GPT3_ADA\x10\x16\x12\x1d\n\x19MODEL_OPENAI_GPT3_BAGGAGE\x10\x17\x12\x17\n\x13MODEL_MOCK_TIER_ONE\x10\x18\x12\x17\n\x13MODEL_MOCK_TIER_TWO\x10\x19*P\n\x04Role\x12\x14\n\x10ROLE_UNSPECIFIED\x10\x00\x12\r\n\tROLE_USER\x10\x01\x12\x12\n\x0eROLE_ASSISTANT\x10\x02\x12\x0f\n\x0bROLE_SYSTEM\x10\x03*\xd6\x03\n\x06Syntax\x12\x16\n\x12SYNTAX_UNSPECIFIED\x10\x00\x12\x15\n\x11SYNTAX_JAVASCRIPT\x10\x01\x12\x11\n\rSYNTAX_PYTHON\x10\x02\x12\x15\n\x11SYNTAX_POSTGRESQL\x10\x03\x12\x10\n\x0cSYNTAX_MSSQL\x10\x04\x12\x10\n\x0cSYNTAX_MYSQL\x10\x05\x12\x12\n\x0eSYNTAX_MARIADB\x10\x06\x12\x14\n\x10SYNTAX_SNOWFLAKE\x10\x07\x12\x16\n\x12SYNTAX_COCKROACHDB\x10\x08\x12\x12\n\x0eSYNTAX_ROCKSET\x10\t\x12\x13\n\x0fSYNTAX_REDSHIFT\x10\n\x12\x13\n\x0fSYNTAX_BIGQUERY\x10\x0b\x12\x13\n\x0fSYNTAX_DYNAMODB\x10\x0c\x12\x12\n\x0eSYNTAX_MONGODB\x10\r\x12\x12\n\x0eSYNTAX_BINDING\x10\x0e\x12\x0f\n\x0bSYNTAX_JSON\x10\x0f\x12\x0f\n\x0bSYNTAX_HTML\x10\x10\x12\x0e\n\nSYNTAX_API\x10\x11\x12\x19\n\x15SYNTAX_PLUGIN_RESTAPI\x10\x12\x12\x19\n\x15SYNTAX_PLUGIN_GRAPHQL\x10\x13\x12\x13\n\x0fSYNTAX_ORACLEDB\x10\x14\x12\x15\n\x11SYNTAX_DATABRICKS\x10\x15*N\n\x07Persona\x12\x17\n\x13PERSONA_UNSPECIFIED\x10\x00\x12\x15\n\x11PERSONA_DEVELOPER\x10\x01\x12\x13\n\x0fPERSONA_TEACHER\x10\x02\x42/Z-github.com/superblocksteam/types/gen/go/ai/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/ai/v1/metadata_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/ai/v1/metadata_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from plugins.common.v1 import metadata_pb2 as plugins_dot_common_dot_v1_dot_metadata__pb2
-from plugins.kafka.v1 import plugin_pb2 as plugins_dot_kafka_dot_v1_dot_plugin__pb2
-from validate import validate_pb2 as validate_dot_validate__pb2
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.plugins.common.v1 import metadata_pb2 as plugins_dot_common_dot_v1_dot_metadata__pb2
+from superblocks_types.plugins.kafka.v1 import plugin_pb2 as plugins_dot_kafka_dot_v1_dot_plugin__pb2
+from superblocks_types.validate import validate_pb2 as validate_dot_validate__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x61i/v1/metadata.proto\x12\x05\x61i.v1\x1a plugins/common/v1/metadata.proto\x1a\x1dplugins/kafka/v1/plugin.proto\x1a\x17validate/validate.proto\x1a\x1b\x62uf/validate/validate.proto\"\xcc\x06\n\x08Metadata\x12\x43\n\x07mariadb\x18\x01 \x01(\x0b\x32\'.plugins.common.v1.SQLMetadata.MinifiedH\x00R\x07mariadb\x12?\n\x05mssql\x18\x02 \x01(\x0b\x32\'.plugins.common.v1.SQLMetadata.MinifiedH\x00R\x05mssql\x12?\n\x05mysql\x18\x03 \x01(\x0b\x32\'.plugins.common.v1.SQLMetadata.MinifiedH\x00R\x05mysql\x12\x45\n\x08postgres\x18\x04 \x01(\x0b\x32\'.plugins.common.v1.SQLMetadata.MinifiedH\x00R\x08postgres\x12\x43\n\x07rockset\x18\x05 \x01(\x0b\x32\'.plugins.common.v1.SQLMetadata.MinifiedH\x00R\x07rockset\x12G\n\tsnowflake\x18\x06 \x01(\x0b\x32\'.plugins.common.v1.SQLMetadata.MinifiedH\x00R\tsnowflake\x12K\n\x0b\x63ockroachdb\x18\x07 \x01(\x0b\x32\'.plugins.common.v1.SQLMetadata.MinifiedH\x00R\x0b\x63ockroachdb\x12;\n\x05kafka\x18\x08 \x01(\x0b\x32#.plugins.kafka.v1.Metadata.MinifiedH\x00R\x05kafka\x12\x43\n\tconfluent\x18\t \x01(\x0b\x32#.plugins.kafka.v1.Metadata.MinifiedH\x00R\tconfluent\x12\x37\n\x03msk\x18\n \x01(\x0b\x32#.plugins.kafka.v1.Metadata.MinifiedH\x00R\x03msk\x12\x41\n\x08redpanda\x18\x0b \x01(\x0b\x32#.plugins.kafka.v1.Metadata.MinifiedH\x00R\x08redpanda\x12\x45\n\naivenkafka\x18\x0c \x01(\x0b\x32#.plugins.kafka.v1.Metadata.MinifiedH\x00R\naivenkafkaB\x12\n\x06\x63onfig\x12\x08\xf8\x42\x01\xbaH\x02\x08\x01\x42/Z-github.com/superblocksteam/types/gen/go/ai/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ai.v1.metadata_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/ai/v1/service_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/ai/v1/service_pb2.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from ai.v1 import ai_pb2 as ai_dot_v1_dot_ai__pb2
-from common.v1 import health_pb2 as common_dot_v1_dot_health__pb2
-from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from superblocks_types.ai.v1 import ai_pb2 as ai_dot_v1_dot_ai__pb2
+from superblocks_types.common.v1 import health_pb2 as common_dot_v1_dot_health__pb2
+from superblocks_types.google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-from validate import validate_pb2 as validate_dot_validate__pb2
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
+from superblocks_types.validate import validate_pb2 as validate_dot_validate__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x61i/v1/service.proto\x12\x05\x61i.v1\x1a\x0e\x61i/v1/ai.proto\x1a\x16\x63ommon/v1/health.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x17validate/validate.proto\x1a\x1b\x62uf/validate/validate.proto\"M\n\tOverrides\x12\x1c\n\x03llm\x18\x01 \x01(\x0e\x32\n.ai.v1.LLMR\x03llm\x12\"\n\x05model\x18\x02 \x01(\x0e\x32\x0c.ai.v1.MODELR\x05model\"t\n\x11\x43reateTaskRequest\x12/\n\x04task\x18\x01 \x01(\x0b\x32\x0b.ai.v1.TaskB\x0e\xfa\x42\x05\x8a\x01\x02\x10\x01\xbaH\x03\xc8\x01\x01R\x04task\x12.\n\toverrides\x18\x02 \x01(\x0b\x32\x10.ai.v1.OverridesR\toverrides\"s\n\tTaskEvent\x12\x14\n\x05\x63hunk\x18\x01 \x01(\tR\x05\x63hunk\x12\x1c\n\x03llm\x18\x02 \x01(\x0e\x32\n.ai.v1.LLMR\x03llm\x12\"\n\x05model\x18\x03 \x01(\x0e\x32\x0c.ai.v1.MODELR\x05model\x12\x0e\n\x02id\x18\x04 \x01(\tR\x02id2\x8d\x01\n\x0fMetadataService\x12z\n\x06Health\x12\x16.google.protobuf.Empty\x1a\x19.common.v1.HealthResponse\"=\x92\x41\x10*\x0eService Health\x82\xd3\xe4\x93\x02$\x12\r/v1/ai/healthZ\x13\x12\x11/api/v1/ai/health2\x85\x01\n\x0bTaskService\x12v\n\x06\x43reate\x12\x18.ai.v1.CreateTaskRequest\x1a\x10.ai.v1.TaskEvent\">\x92\x41\r*\x0b\x43reate Task\x82\xd3\xe4\x93\x02(\"\x0c/v1/ai/tasks:\x01*Z\x15\"\x10/api/v1/ai/tasks:\x01*0\x01\x42xZ-github.com/superblocksteam/types/gen/go/ai/v1\x92\x41\x46\x12\x1d\n\x16Superblocks AI Service2\x03\x31.0*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'ai.v1.service_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/ai/v1/service_pb2_grpc.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/ai/v1/service_pb2_grpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from ai.v1 import service_pb2 as ai_dot_v1_dot_service__pb2
-from common.v1 import health_pb2 as common_dot_v1_dot_health__pb2
+from superblocks_types.ai.v1 import service_pb2 as ai_dot_v1_dot_service__pb2
+from superblocks_types.common.v1 import health_pb2 as common_dot_v1_dot_health__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
 class MetadataServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/ai/v1/vector_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/ai/v1/vector_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/api_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/api_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,57 +8,57 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from api.v1 import blocks_pb2 as api_dot_v1_dot_blocks__pb2
-from common.v1 import common_pb2 as common_dot_v1_dot_common__pb2
+from superblocks_types.api.v1 import blocks_pb2 as api_dot_v1_dot_blocks__pb2
+from superblocks_types.common.v1 import common_pb2 as common_dot_v1_dot_common__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from plugins.bigquery.v1 import plugin_pb2 as plugins_dot_bigquery_dot_v1_dot_plugin__pb2
-from plugins.cockroachdb.v1 import plugin_pb2 as plugins_dot_cockroachdb_dot_v1_dot_plugin__pb2
-from plugins.couchbase.v1 import plugin_pb2 as plugins_dot_couchbase_dot_v1_dot_plugin__pb2
-from plugins.databricks.v1 import plugin_pb2 as plugins_dot_databricks_dot_v1_dot_plugin__pb2
-from plugins.dynamodb.v1 import plugin_pb2 as plugins_dot_dynamodb_dot_v1_dot_plugin__pb2
-from plugins.email.v1 import plugin_pb2 as plugins_dot_email_dot_v1_dot_plugin__pb2
-from plugins.gcs.v1 import plugin_pb2 as plugins_dot_gcs_dot_v1_dot_plugin__pb2
-from plugins.graphql.v1 import plugin_pb2 as plugins_dot_graphql_dot_v1_dot_plugin__pb2
-from plugins.gsheets.v1 import plugin_pb2 as plugins_dot_gsheets_dot_v1_dot_plugin__pb2
-from plugins.javascript.v1 import plugin_pb2 as plugins_dot_javascript_dot_v1_dot_plugin__pb2
-from plugins.kafka.v1 import plugin_pb2 as plugins_dot_kafka_dot_v1_dot_plugin__pb2
-from plugins.mariadb.v1 import plugin_pb2 as plugins_dot_mariadb_dot_v1_dot_plugin__pb2
-from plugins.mongodb.v1 import plugin_pb2 as plugins_dot_mongodb_dot_v1_dot_plugin__pb2
-from plugins.mssql.v1 import plugin_pb2 as plugins_dot_mssql_dot_v1_dot_plugin__pb2
-from plugins.mysql.v1 import plugin_pb2 as plugins_dot_mysql_dot_v1_dot_plugin__pb2
-from plugins.ocr.v1 import plugin_pb2 as plugins_dot_ocr_dot_v1_dot_plugin__pb2
-from plugins.openai.v1 import plugin_pb2 as plugins_dot_openai_dot_v1_dot_plugin__pb2
-from plugins.oracledb.v1 import plugin_pb2 as plugins_dot_oracledb_dot_v1_dot_plugin__pb2
-from plugins.postgresql.v1 import plugin_pb2 as plugins_dot_postgresql_dot_v1_dot_plugin__pb2
-from plugins.python.v1 import plugin_pb2 as plugins_dot_python_dot_v1_dot_plugin__pb2
-from plugins.redshift.v1 import plugin_pb2 as plugins_dot_redshift_dot_v1_dot_plugin__pb2
-from plugins.restapi.v1 import plugin_pb2 as plugins_dot_restapi_dot_v1_dot_plugin__pb2
-from plugins.restapiintegration.v1 import plugin_pb2 as plugins_dot_restapiintegration_dot_v1_dot_plugin__pb2
-from plugins.rockset.v1 import plugin_pb2 as plugins_dot_rockset_dot_v1_dot_plugin__pb2
-from plugins.s3.v1 import plugin_pb2 as plugins_dot_s3_dot_v1_dot_plugin__pb2
-from plugins.salesforce.v1 import plugin_pb2 as plugins_dot_salesforce_dot_v1_dot_plugin__pb2
-from plugins.smtp.v1 import plugin_pb2 as plugins_dot_smtp_dot_v1_dot_plugin__pb2
-from plugins.snowflake.v1 import plugin_pb2 as plugins_dot_snowflake_dot_v1_dot_plugin__pb2
-from plugins.workflow.v1 import plugin_pb2 as plugins_dot_workflow_dot_v1_dot_plugin__pb2
-from superblocks.v1 import options_pb2 as superblocks_dot_v1_dot_options__pb2
-from validate import validate_pb2 as validate_dot_validate__pb2
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
-from plugins.athena.v1 import plugin_pb2 as plugins_dot_athena_dot_v1_dot_plugin__pb2
-from plugins.redis.v1 import plugin_pb2 as plugins_dot_redis_dot_v1_dot_plugin__pb2
-from plugins.cosmosdb.v1 import plugin_pb2 as plugins_dot_cosmosdb_dot_v1_dot_plugin__pb2
-from plugins.adls.v1 import plugin_pb2 as plugins_dot_adls_dot_v1_dot_plugin__pb2
-from plugins.pinecone.v1 import plugin_pb2 as plugins_dot_pinecone_dot_v1_dot_plugin__pb2
-from plugins.custom.v1 import plugin_pb2 as plugins_dot_custom_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.bigquery.v1 import plugin_pb2 as plugins_dot_bigquery_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.cockroachdb.v1 import plugin_pb2 as plugins_dot_cockroachdb_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.couchbase.v1 import plugin_pb2 as plugins_dot_couchbase_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.databricks.v1 import plugin_pb2 as plugins_dot_databricks_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.dynamodb.v1 import plugin_pb2 as plugins_dot_dynamodb_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.email.v1 import plugin_pb2 as plugins_dot_email_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.gcs.v1 import plugin_pb2 as plugins_dot_gcs_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.graphql.v1 import plugin_pb2 as plugins_dot_graphql_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.gsheets.v1 import plugin_pb2 as plugins_dot_gsheets_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.javascript.v1 import plugin_pb2 as plugins_dot_javascript_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.kafka.v1 import plugin_pb2 as plugins_dot_kafka_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.mariadb.v1 import plugin_pb2 as plugins_dot_mariadb_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.mongodb.v1 import plugin_pb2 as plugins_dot_mongodb_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.mssql.v1 import plugin_pb2 as plugins_dot_mssql_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.mysql.v1 import plugin_pb2 as plugins_dot_mysql_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.ocr.v1 import plugin_pb2 as plugins_dot_ocr_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.openai.v1 import plugin_pb2 as plugins_dot_openai_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.oracledb.v1 import plugin_pb2 as plugins_dot_oracledb_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.postgresql.v1 import plugin_pb2 as plugins_dot_postgresql_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.python.v1 import plugin_pb2 as plugins_dot_python_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.redshift.v1 import plugin_pb2 as plugins_dot_redshift_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.restapi.v1 import plugin_pb2 as plugins_dot_restapi_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.restapiintegration.v1 import plugin_pb2 as plugins_dot_restapiintegration_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.rockset.v1 import plugin_pb2 as plugins_dot_rockset_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.s3.v1 import plugin_pb2 as plugins_dot_s3_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.salesforce.v1 import plugin_pb2 as plugins_dot_salesforce_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.smtp.v1 import plugin_pb2 as plugins_dot_smtp_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.snowflake.v1 import plugin_pb2 as plugins_dot_snowflake_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.workflow.v1 import plugin_pb2 as plugins_dot_workflow_dot_v1_dot_plugin__pb2
+from superblocks_types.superblocks.v1 import options_pb2 as superblocks_dot_v1_dot_options__pb2
+from superblocks_types.validate import validate_pb2 as validate_dot_validate__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.plugins.athena.v1 import plugin_pb2 as plugins_dot_athena_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.redis.v1 import plugin_pb2 as plugins_dot_redis_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.cosmosdb.v1 import plugin_pb2 as plugins_dot_cosmosdb_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.adls.v1 import plugin_pb2 as plugins_dot_adls_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.pinecone.v1 import plugin_pb2 as plugins_dot_pinecone_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.custom.v1 import plugin_pb2 as plugins_dot_custom_dot_v1_dot_plugin__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
-from utils.v1 import utils_pb2 as utils_dot_v1_dot_utils__pb2
+from superblocks_types.utils.v1 import utils_pb2 as utils_dot_v1_dot_utils__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x61pi/v1/api.proto\x12\x06\x61pi.v1\x1a\x13\x61pi/v1/blocks.proto\x1a\x16\x63ommon/v1/common.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a plugins/bigquery/v1/plugin.proto\x1a#plugins/cockroachdb/v1/plugin.proto\x1a!plugins/couchbase/v1/plugin.proto\x1a\"plugins/databricks/v1/plugin.proto\x1a plugins/dynamodb/v1/plugin.proto\x1a\x1dplugins/email/v1/plugin.proto\x1a\x1bplugins/gcs/v1/plugin.proto\x1a\x1fplugins/graphql/v1/plugin.proto\x1a\x1fplugins/gsheets/v1/plugin.proto\x1a\"plugins/javascript/v1/plugin.proto\x1a\x1dplugins/kafka/v1/plugin.proto\x1a\x1fplugins/mariadb/v1/plugin.proto\x1a\x1fplugins/mongodb/v1/plugin.proto\x1a\x1dplugins/mssql/v1/plugin.proto\x1a\x1dplugins/mysql/v1/plugin.proto\x1a\x1bplugins/ocr/v1/plugin.proto\x1a\x1eplugins/openai/v1/plugin.proto\x1a plugins/oracledb/v1/plugin.proto\x1a\"plugins/postgresql/v1/plugin.proto\x1a\x1eplugins/python/v1/plugin.proto\x1a plugins/redshift/v1/plugin.proto\x1a\x1fplugins/restapi/v1/plugin.proto\x1a*plugins/restapiintegration/v1/plugin.proto\x1a\x1fplugins/rockset/v1/plugin.proto\x1a\x1aplugins/s3/v1/plugin.proto\x1a\"plugins/salesforce/v1/plugin.proto\x1a\x1cplugins/smtp/v1/plugin.proto\x1a!plugins/snowflake/v1/plugin.proto\x1a plugins/workflow/v1/plugin.proto\x1a\x1csuperblocks/v1/options.proto\x1a\x17validate/validate.proto\x1a\x1b\x62uf/validate/validate.proto\x1a\x1eplugins/athena/v1/plugin.proto\x1a\x1dplugins/redis/v1/plugin.proto\x1a plugins/cosmosdb/v1/plugin.proto\x1a\x1cplugins/adls/v1/plugin.proto\x1a plugins/pinecone/v1/plugin.proto\x1a\x1eplugins/custom/v1/plugin.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x14utils/v1/utils.proto\"\xde\x01\n\x03\x41pi\x12?\n\x08metadata\x18\x01 \x01(\x0b\x32\x13.common.v1.MetadataB\x0e\xfa\x42\x05\x8a\x01\x02\x10\x01\xbaH\x03\xc8\x01\x01R\x08metadata\x12%\n\x06\x62locks\x18\x02 \x03(\x0b\x32\r.api.v1.BlockR\x06\x62locks\x12)\n\x07trigger\x18\x03 \x01(\x0b\x32\x0f.api.v1.TriggerR\x07trigger\x12\x36\n\tsignature\x18\x04 \x01(\x0b\x32\x13.utils.v1.SignatureH\x00R\tsignature\x88\x01\x01\x42\x0c\n\n_signature\"\xb7\x02\n\x08Profiles\x12,\n\x05modes\x18\x01 \x01(\x0b\x32\x16.api.v1.Profiles.ModesR\x05modes\x1a\xfc\x01\n\x05Modes\x12\x37\n\x06\x65\x64itor\x18\x01 \x01(\x0b\x32\x1f.api.v1.Profiles.Modes.SettingsR\x06\x65\x64itor\x12\x39\n\x07preview\x18\x02 \x01(\x0b\x32\x1f.api.v1.Profiles.Modes.SettingsR\x07preview\x12;\n\x08\x64\x65ployed\x18\x03 \x01(\x0b\x32\x1f.api.v1.Profiles.Modes.SettingsR\x08\x64\x65ployed\x1a\x42\n\x08Settings\x12\x18\n\x07\x64\x65\x66\x61ult\x18\x01 \x01(\tR\x07\x64\x65\x66\x61ult\x12\x1c\n\tavailable\x18\x02 \x03(\tR\tavailable\"\x8e\x0f\n\x07Trigger\x12?\n\x0b\x61pplication\x18\x01 \x01(\x0b\x32\x1b.api.v1.Trigger.ApplicationH\x00R\x0b\x61pplication\x12\x36\n\x08workflow\x18\x02 \x01(\x0b\x32\x18.api.v1.Trigger.WorkflowH\x00R\x08workflow\x12\'\n\x03job\x18\x03 \x01(\x0b\x32\x13.api.v1.Trigger.JobH\x00R\x03job\x1a\xe0\x01\n\x0b\x41pplication\x12=\n\x07options\x18\x01 \x01(\x0b\x32#.api.v1.Trigger.Application.OptionsR\x07options\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02id\x12\x1c\n\x07page_id\x18\x03 \x01(\tH\x00R\x06pageId\x88\x01\x01\x1aX\n\x07Options\x12\x34\n\x14\x65xecute_on_page_load\x18\x01 \x01(\x08H\x00R\x11\x65xecuteOnPageLoad\x88\x01\x01\x42\x17\n\x15_execute_on_page_loadB\n\n\x08_page_id\x1a\x83\x05\n\x08Workflow\x12:\n\x07options\x18\x01 \x01(\x0b\x32 .api.v1.Trigger.Workflow.OptionsR\x07options\x12\x43\n\nparameters\x18\x02 \x01(\x0b\x32#.api.v1.Trigger.Workflow.ParametersR\nparameters\x1a}\n\x07Options\x12,\n\x08profiles\x18\x01 \x01(\x0b\x32\x10.api.v1.ProfilesR\x08profiles\x12/\n\x10\x64\x65ployedCommitId\x18\x02 \x01(\tH\x00R\x10\x64\x65ployedCommitId\x88\x01\x01\x42\x13\n\x11_deployedCommitId\x1a\xf6\x02\n\nParameters\x12\x44\n\x05query\x18\x01 \x03(\x0b\x32..api.v1.Trigger.Workflow.Parameters.QueryEntryR\x05query\x12\x41\n\x04\x62ody\x18\x02 \x03(\x0b\x32-.api.v1.Trigger.Workflow.Parameters.BodyEntryR\x04\x62ody\x1a$\n\nQueryParam\x12\x16\n\x06values\x18\x01 \x03(\tR\x06values\x1ah\n\nQueryEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x44\n\x05value\x18\x02 \x01(\x0b\x32..api.v1.Trigger.Workflow.Parameters.QueryParamR\x05value:\x02\x38\x01\x1aO\n\tBodyEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.ValueR\x05value:\x02\x38\x01\x1a\xed\x06\n\x03Job\x12\x35\n\x07options\x18\x01 \x01(\x0b\x32\x1b.api.v1.Trigger.Job.OptionsR\x07options\x12,\n\tfrequency\x18\x02 \x01(\x05\x42\x0e\xfa\x42\x04\x1a\x02(\x01\xbaH\x04\x1a\x02(\x01R\tfrequency\x12\x38\n\x08interval\x18\x03 \x01(\x0e\x32\x1c.api.v1.Trigger.Job.IntervalR\x08interval\x12\x34\n\x0c\x64\x61y_of_month\x18\x04 \x01(\x05\x42\x12\xfa\x42\x06\x1a\x04\x18 (\x01\xbaH\x06\x1a\x04\x18 (\x01R\ndayOfMonth\x12,\n\x04\x64\x61ys\x18\x05 \x01(\x0b\x32\x18.api.v1.Trigger.Job.DaysR\x04\x64\x61ys\x12.\n\x04time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x04time\x12\'\n\x0ftimezone_locale\x18\x08 \x01(\tR\x0etimezoneLocale\x1a\xb0\x01\n\x07Options\x12,\n\x08profiles\x18\x01 \x01(\x0b\x32\x10.api.v1.ProfilesR\x08profiles\x12\x31\n\x15send_email_on_failure\x18\x02 \x01(\x08R\x12sendEmailOnFailure\x12/\n\x10\x64\x65ployedCommitId\x18\x03 \x01(\tH\x00R\x10\x64\x65ployedCommitId\x88\x01\x01\x42\x13\n\x11_deployedCommitId\x1a\xbe\x01\n\x04\x44\x61ys\x12\x16\n\x06sunday\x18\x01 \x01(\x08R\x06sunday\x12\x16\n\x06monday\x18\x02 \x01(\x08R\x06monday\x12\x18\n\x07tuesday\x18\x03 \x01(\x08R\x07tuesday\x12\x1c\n\twednesday\x18\x04 \x01(\x08R\twednesday\x12\x1a\n\x08thursday\x18\x05 \x01(\x08R\x08thursday\x12\x16\n\x06\x66riday\x18\x06 \x01(\x08R\x06\x66riday\x12\x1a\n\x08saturday\x18\x07 \x01(\x08R\x08saturday\"\x85\x01\n\x08Interval\x12\x18\n\x14INTERVAL_UNSPECIFIED\x10\x00\x12\x13\n\x0fINTERVAL_MINUTE\x10\x01\x12\x11\n\rINTERVAL_HOUR\x10\x02\x12\x10\n\x0cINTERVAL_DAY\x10\x03\x12\x11\n\rINTERVAL_WEEK\x10\x04\x12\x12\n\x0eINTERVAL_MONTH\x10\x05J\x04\x08\x07\x10\x08R\x08\x64\x61ys_utcB\x08\n\x06\x63onfig\"/\n\x06\x42locks\x12%\n\x06\x62locks\x18\x01 \x03(\x0b\x32\r.api.v1.BlockR\x06\x62locks\"\xfe\x16\n\x05\x42lock\x12\"\n\x04name\x18\x01 \x01(\tB\x0e\xfa\x42\x04r\x02\x10\x01\xbaH\x04r\x02\x10\x01R\x04name\x12+\n\x05\x62reak\x18\x02 \x01(\x0b\x32\x13.api.v1.Block.BreakH\x00R\x05\x62reak\x12.\n\x06return\x18\x03 \x01(\x0b\x32\x14.api.v1.Block.ReturnH\x00R\x06return\x12(\n\x04wait\x18\x04 \x01(\x0b\x32\x12.api.v1.Block.WaitH\x00R\x04wait\x12\x34\n\x08parallel\x18\x05 \x01(\x0b\x32\x16.api.v1.Block.ParallelH\x00R\x08parallel\x12=\n\x0b\x63onditional\x18\x06 \x01(\x0b\x32\x19.api.v1.Block.ConditionalH\x00R\x0b\x63onditional\x12(\n\x04loop\x18\x07 \x01(\x0b\x32\x12.api.v1.Block.LoopH\x00R\x04loop\x12\x35\n\ttry_catch\x18\x08 \x01(\x0b\x32\x16.api.v1.Block.TryCatchH\x00R\x08tryCatch\x12\"\n\x04step\x18\t \x01(\x0b\x32\x0c.api.v1.StepH\x00R\x04step\x12\x31\n\tvariables\x18\n \x01(\x0b\x32\x11.api.v1.VariablesH\x00R\tvariables\x12+\n\x05throw\x18\x0b \x01(\x0b\x32\x13.api.v1.Block.ThrowH\x00R\x05throw\x12.\n\x06stream\x18\x0c \x01(\x0b\x32\x14.api.v1.Block.StreamH\x00R\x06stream\x12(\n\x04send\x18\r \x01(\x0b\x32\x12.api.v1.Block.SendH\x00R\x04send\x1a\xa2\x05\n\x08Parallel\x12\x37\n\x06static\x18\x01 \x01(\x0b\x32\x1d.api.v1.Block.Parallel.StaticH\x00R\x06static\x12:\n\x07\x64ynamic\x18\x02 \x01(\x0b\x32\x1e.api.v1.Block.Parallel.DynamicH\x00R\x07\x64ynamic\x12\x42\n\x04wait\x18\x03 \x01(\x0e\x32\x1b.api.v1.Block.Parallel.WaitB\x11\xfa\x42\x05\x82\x01\x02 \x00\xbaH\x06\x82\x01\x03\"\x01\x00R\x04wait\x12)\n\tpool_size\x18\x04 \x01(\x05\x42\x07\xbaH\x04\x1a\x02(\x01H\x01R\x08poolSize\x88\x01\x01\x1a\x92\x01\n\x06Static\x12>\n\x05paths\x18\x01 \x03(\x0b\x32(.api.v1.Block.Parallel.Static.PathsEntryR\x05paths\x1aH\n\nPathsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12$\n\x05value\x18\x02 \x01(\x0b\x32\x0e.api.v1.BlocksR\x05value:\x02\x38\x01\x1a\xbf\x01\n\x07\x44ynamic\x12\x14\n\x05paths\x18\x01 \x01(\tR\x05paths\x12\x46\n\tvariables\x18\x02 \x01(\x0b\x32(.api.v1.Block.Parallel.Dynamic.VariablesR\tvariables\x12%\n\x06\x62locks\x18\x03 \x03(\x0b\x32\r.api.v1.BlockR\x06\x62locks\x1a/\n\tVariables\x12\"\n\x04item\x18\x01 \x01(\tB\x0e\xfa\x42\x04r\x02\x10\x01\xbaH\x04r\x02\x10\x01R\x04item\"9\n\x04Wait\x12\x14\n\x10WAIT_UNSPECIFIED\x10\x00\x12\x0c\n\x08WAIT_ALL\x10\x01\x12\r\n\tWAIT_NONE\x10\x02\x42\x12\n\x06\x63onfig\x12\x08\xf8\x42\x01\xbaH\x02\x08\x01\x42\x0c\n\n_pool_size\x1a\x92\x02\n\x0b\x43onditional\x12\x33\n\x02if\x18\x01 \x01(\x0b\x32#.api.v1.Block.Conditional.ConditionR\x02if\x12<\n\x07\x65lse_if\x18\x02 \x03(\x0b\x32#.api.v1.Block.Conditional.ConditionR\x06\x65lseIf\x12\"\n\x04\x65lse\x18\x03 \x01(\x0b\x32\x0e.api.v1.BlocksR\x04\x65lse\x1al\n\tCondition\x12\x38\n\tcondition\x18\x01 \x01(\tB\x1a\xfa\x42\nr\x08:\x02{{B\x02}}\xbaH\nr\x08:\x02{{B\x02}}R\tcondition\x12%\n\x06\x62locks\x18\x02 \x03(\x0b\x32\r.api.v1.BlockR\x06\x62locks\x1a\xed\x02\n\x04Loop\x12\x30\n\x05range\x18\x01 \x01(\tB\x1a\xfa\x42\nr\x08:\x02{{B\x02}}\xbaH\nr\x08:\x02{{B\x02}}R\x05range\x12+\n\x04type\x18\x02 \x01(\x0e\x32\x17.api.v1.Block.Loop.TypeR\x04type\x12:\n\tvariables\x18\x03 \x01(\x0b\x32\x1c.api.v1.Block.Loop.VariablesR\tvariables\x12%\n\x06\x62locks\x18\x04 \x03(\x0b\x32\r.api.v1.BlockR\x06\x62locks\x1aU\n\tVariables\x12$\n\x05index\x18\x01 \x01(\tB\x0e\xfa\x42\x04r\x02\x10\x01\xbaH\x04r\x02\x10\x01R\x05index\x12\"\n\x04item\x18\x02 \x01(\tB\x0e\xfa\x42\x04r\x02\x10\x01\xbaH\x04r\x02\x10\x01R\x04item\"L\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0c\n\x08TYPE_FOR\x10\x01\x12\x10\n\x0cTYPE_FOREACH\x10\x02\x12\x0e\n\nTYPE_WHILE\x10\x03\x1a\xef\x01\n\x08TryCatch\x12 \n\x03try\x18\x01 \x01(\x0b\x32\x0e.api.v1.BlocksR\x03try\x12$\n\x05\x63\x61tch\x18\x02 \x01(\x0b\x32\x0e.api.v1.BlocksR\x05\x63\x61tch\x12(\n\x07\x66inally\x18\x03 \x01(\x0b\x32\x0e.api.v1.BlocksR\x07\x66inally\x12>\n\tvariables\x18\x04 \x01(\x0b\x32 .api.v1.Block.TryCatch.VariablesR\tvariables\x1a\x31\n\tVariables\x12$\n\x05\x65rror\x18\x01 \x01(\tB\x0e\xfa\x42\x04r\x02\x10\x01\xbaH\x04r\x02\x10\x01R\x05\x65rror\x1a\x41\n\x05\x42reak\x12\x38\n\tcondition\x18\x01 \x01(\tB\x1a\xfa\x42\nr\x08:\x02{{B\x02}}\xbaH\nr\x08:\x02{{B\x02}}R\tcondition\x1a\x38\n\x06Return\x12.\n\x04\x64\x61ta\x18\x01 \x01(\tB\x1a\xfa\x42\nr\x08:\x02{{B\x02}}\xbaH\nr\x08:\x02{{B\x02}}R\x04\x64\x61ta\x1a\x39\n\x05Throw\x12\x30\n\x05\x65rror\x18\x01 \x01(\tB\x1a\xfa\x42\nr\x08:\x02{{B\x02}}\xbaH\nr\x08:\x02{{B\x02}}R\x05\x65rror\x1a@\n\x04Wait\x12\x38\n\tcondition\x18\x01 \x01(\tB\x1a\xfa\x42\nr\x08:\x02{{B\x02}}\xbaH\nr\x08:\x02{{B\x02}}R\tcondition\x1a\xb9\x03\n\x06Stream\x12\x46\n\x07trigger\x18\x01 \x01(\x0b\x32\x1c.api.v1.Block.Stream.TriggerB\x0e\xfa\x42\x05\x8a\x01\x02\x10\x01\xbaH\x03\xc8\x01\x01R\x07trigger\x12(\n\x07process\x18\x02 \x01(\x0b\x32\x0e.api.v1.BlocksR\x07process\x12L\n\tvariables\x18\x03 \x01(\x0b\x32\x1e.api.v1.Block.Stream.VariablesB\x0e\xfa\x42\x05\x8a\x01\x02\x10\x01\xbaH\x03\xc8\x01\x01R\tvariables\x12\x36\n\x07options\x18\x04 \x01(\x0b\x32\x1c.api.v1.Block.Stream.OptionsR\x07options\x1a/\n\tVariables\x12\"\n\x04item\x18\x01 \x01(\tB\x0e\xfa\x42\x04r\x02\x10\x01\xbaH\x04r\x02\x10\x01R\x04item\x1a\x35\n\x07Options\x12*\n\x11\x64isable_auto_send\x18\x01 \x01(\x08R\x0f\x64isableAutoSend\x1aO\n\x07Trigger\x12\"\n\x04name\x18\x01 \x01(\tB\x0e\xfa\x42\x04r\x02\x10\x01\xbaH\x04r\x02\x10\x01R\x04name\x12 \n\x04step\x18\x02 \x01(\x0b\x32\x0c.api.v1.StepR\x04step\x1a\x30\n\x04Send\x12(\n\x07message\x18\x01 \x01(\tB\x0e\xfa\x42\x04r\x02\x10\x01\xbaH\x04r\x02\x10\x01R\x07messageB\x12\n\x06\x63onfig\x12\x08\xf8\x42\x01\xbaH\x02\x08\x01\"\xe0%\n\x04Step\x12 \n\x0bintegration\x18\x01 \x01(\tR\x0bintegration\x12\x33\n\x06python\x18\x02 \x01(\x0b\x32\x19.plugins.python.v1.PluginH\x00R\x06python\x12\x39\n\x08\x62igquery\x18\x03 \x01(\x0b\x32\x1b.plugins.bigquery.v1.PluginH\x00R\x08\x62igquery\x12\x39\n\x08\x64ynamodb\x18\x04 \x01(\x0b\x32\x1b.plugins.dynamodb.v1.PluginH\x00R\x08\x64ynamodb\x12\x30\n\x05\x65mail\x18\x05 \x01(\x0b\x32\x18.plugins.email.v1.PluginH\x00R\x05\x65mail\x12\x36\n\x07graphql\x18\x06 \x01(\x0b\x32\x1a.plugins.graphql.v1.PluginH\x00R\x07graphql\x12L\n\x12graphqlintegration\x18\x07 \x01(\x0b\x32\x1a.plugins.graphql.v1.PluginH\x00R\x12graphqlintegration\x12\x36\n\x07gsheets\x18\x08 \x01(\x0b\x32\x1a.plugins.gsheets.v1.PluginH\x00R\x07gsheets\x12\x36\n\x07mariadb\x18\t \x01(\x0b\x32\x1a.plugins.mariadb.v1.PluginH\x00R\x07mariadb\x12\x30\n\x05mssql\x18\n \x01(\x0b\x32\x18.plugins.mssql.v1.PluginH\x00R\x05mssql\x12\x30\n\x05mysql\x18\x0b \x01(\x0b\x32\x18.plugins.mysql.v1.PluginH\x00R\x05mysql\x12;\n\x08postgres\x18\x0c \x01(\x0b\x32\x1d.plugins.postgresql.v1.PluginH\x00R\x08postgres\x12\x39\n\x08redshift\x18\r \x01(\x0b\x32\x1b.plugins.redshift.v1.PluginH\x00R\x08redshift\x12\x36\n\x07restapi\x18\x0e \x01(\x0b\x32\x1a.plugins.restapi.v1.PluginH\x00R\x07restapi\x12W\n\x12restapiintegration\x18\x0f \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginH\x00R\x12restapiintegration\x12\x36\n\x07rockset\x18\x10 \x01(\x0b\x32\x1a.plugins.rockset.v1.PluginH\x00R\x07rockset\x12\'\n\x02s3\x18\x11 \x01(\x0b\x32\x15.plugins.s3.v1.PluginH\x00R\x02s3\x12<\n\tsnowflake\x18\x12 \x01(\x0b\x32\x1c.plugins.snowflake.v1.PluginH\x00R\tsnowflake\x12\x39\n\x08workflow\x18\x13 \x01(\x0b\x32\x1b.plugins.workflow.v1.PluginH\x00R\x08workflow\x12?\n\njavascript\x18\x14 \x01(\x0b\x32\x1d.plugins.javascript.v1.PluginH\x00R\njavascript\x12\x36\n\x07mongodb\x18\x15 \x01(\x0b\x32\x1a.plugins.mongodb.v1.PluginH\x00R\x07mongodb\x12*\n\x03gcs\x18\x16 \x01(\x0b\x32\x16.plugins.gcs.v1.PluginH\x00R\x03gcs\x12\x33\n\x06openai\x18\x17 \x01(\x0b\x32\x19.plugins.openai.v1.PluginH\x00R\x06openai\x12M\n\x03ocr\x18\x18 \x01(\x0b\x32\x16.plugins.ocr.v1.PluginB\x15\x82\xa6\x1d\x11\x12\x0fsuperblocks-ocrH\x00R\x0fsuperblocks-ocr\x12\x30\n\x05kafka\x18\x19 \x01(\x0b\x32\x18.plugins.kafka.v1.PluginH\x00R\x05kafka\x12\x38\n\tconfluent\x18\x1a \x01(\x0b\x32\x18.plugins.kafka.v1.PluginH\x00R\tconfluent\x12,\n\x03msk\x18\x1b \x01(\x0b\x32\x18.plugins.kafka.v1.PluginH\x00R\x03msk\x12\x36\n\x08redpanda\x18\x1c \x01(\x0b\x32\x18.plugins.kafka.v1.PluginH\x00R\x08redpanda\x12:\n\naivenkafka\x18\x1d \x01(\x0b\x32\x18.plugins.kafka.v1.PluginH\x00R\naivenkafka\x12\x42\n\x0b\x63ockroachdb\x18\x1e \x01(\x0b\x32\x1e.plugins.cockroachdb.v1.PluginH\x00R\x0b\x63ockroachdb\x12]\n\x08\x61irtable\x18\x1f \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x08\x61irtable\x12Y\n\x06notion\x18  \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x06notion\x12_\n\tpagerduty\x18! \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\tpagerduty\x12]\n\x08sendgrid\x18\" \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x08sendgrid\x12W\n\x05slack\x18# \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x05slack\x12\x33\n\x06\x61thena\x18$ \x01(\x0b\x32\x19.plugins.athena.v1.PluginH\x00R\x06\x61thena\x12\x30\n\x05redis\x18% \x01(\x0b\x32\x18.plugins.redis.v1.PluginH\x00R\x05redis\x12W\n\x05\x61sana\x18& \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x05\x61sana\x12Y\n\x06github\x18\' \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x06github\x12-\n\x04smtp\x18( \x01(\x0b\x32\x17.plugins.smtp.v1.PluginH\x00R\x04smtp\x12?\n\nsalesforce\x18) \x01(\x0b\x32\x1d.plugins.salesforce.v1.PluginH\x00R\nsalesforce\x12_\n\tbitbucket\x18* \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\tbitbucket\x12]\n\x08\x63ircleci\x18+ \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x08\x63ircleci\x12W\n\x05\x66ront\x18, \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x05\x66ront\x12]\n\x08intercom\x18- \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x08intercom\x12[\n\x07segment\x18. \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x07segment\x12\x65\n\x0claunchdarkly\x18/ \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x0claunchdarkly\x12[\n\x07\x64ropbox\x18\x30 \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x07\x64ropbox\x12Y\n\x06twilio\x18\x31 \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x06twilio\x12\x63\n\x0bgoogledrive\x18\x32 \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x0bgoogledrive\x12k\n\x0fgoogleanalytics\x18\x33 \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x0fgoogleanalytics\x12S\n\x03\x62ox\x18\x34 \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x03\x62ox\x12[\n\x07hubspot\x18\x35 \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x07hubspot\x12Y\n\x06stripe\x18\x36 \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x06stripe\x12U\n\x04zoom\x18\x37 \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x04zoom\x12U\n\x04jira\x18\x38 \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x04jira\x12[\n\x07zendesk\x18\x39 \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x07zendesk\x12-\n\x04\x61\x64ls\x18: \x01(\x0b\x32\x17.plugins.adls.v1.PluginH\x00R\x04\x61\x64ls\x12S\n\x08pinecone\x18; \x01(\x0b\x32\x1b.plugins.pinecone.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x08pinecone\x12\x39\n\x08\x63osmosdb\x18< \x01(\x0b\x32\x1b.plugins.cosmosdb.v1.PluginH\x00R\x08\x63osmosdb\x12[\n\x07\x64\x61tadog\x18= \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x07\x64\x61tadog\x12U\n\x04xero\x18> \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\x04xero\x12\x39\n\x08oracledb\x18? \x01(\x0b\x32\x1b.plugins.oracledb.v1.PluginH\x00R\x08oracledb\x12g\n\relasticsearch\x18@ \x01(\x0b\x32%.plugins.restapiintegration.v1.PluginB\x18\x82\xa6\x1d\x14\x12\x12restapiintegrationH\x00R\relasticsearch\x12?\n\ndatabricks\x18\x41 \x01(\x0b\x32\x1d.plugins.databricks.v1.PluginH\x00R\ndatabricks\x12<\n\tcouchbase\x18\x42 \x01(\x0b\x32\x1c.plugins.couchbase.v1.PluginH\x00R\tcouchbase\x12\x33\n\x06\x63ustom\x18\x43 \x01(\x0b\x32\x19.plugins.custom.v1.PluginH\x00R\x06\x63ustom:\x06\x82\xb5\x18\x02\x08\x01\x42\x12\n\x06\x63onfig\x12\x08\xf8\x42\x01\xbaH\x02\x08\x01\x42\x30Z.github.com/superblocksteam/types/gen/go/api/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api.v1.api_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/blocks_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/blocks_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from validate import validate_pb2 as validate_dot_validate__pb2
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.validate import validate_pb2 as validate_dot_validate__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x13\x61pi/v1/blocks.proto\x12\x06\x61pi.v1\x1a\x17validate/validate.proto\x1a\x1b\x62uf/validate/validate.proto\"\x9e\x03\n\tVariables\x12.\n\x05items\x18\x01 \x03(\x0b\x32\x18.api.v1.Variables.ConfigR\x05items\x1a\xb7\x01\n\x06\x43onfig\x12\x30\n\x05value\x18\x01 \x01(\tB\x1a\xfa\x42\nr\x08:\x02{{B\x02}}\xbaH\nr\x08:\x02{{B\x02}}R\x05value\x12=\n\x04type\x18\x02 \x01(\x0e\x32\x16.api.v1.Variables.TypeB\x11\xfa\x42\x05\x82\x01\x02 \x00\xbaH\x06\x82\x01\x03\"\x01\x00R\x04type\x12*\n\x04mode\x18\x03 \x01(\x0e\x32\x16.api.v1.Variables.ModeR\x04mode\x12\x10\n\x03key\x18\x04 \x01(\tR\x03key\"f\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x0f\n\x0bTYPE_SIMPLE\x10\x01\x12\x11\n\rTYPE_ADVANCED\x10\x02\x12\x0f\n\x0bTYPE_NATIVE\x10\x03\x12\x13\n\x0fTYPE_FILEPICKER\x10\x04\"?\n\x04Mode\x12\x14\n\x10MODE_UNSPECIFIED\x10\x00\x12\r\n\tMODE_READ\x10\x01\x12\x12\n\x0eMODE_READWRITE\x10\x02\x42\x30Z.github.com/superblocksteam/types/gen/go/api/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api.v1.blocks_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/event_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/event_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from common.v1 import errors_pb2 as common_dot_v1_dot_errors__pb2
+from superblocks_types.common.v1 import errors_pb2 as common_dot_v1_dot_errors__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from validate import validate_pb2 as validate_dot_validate__pb2
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.validate import validate_pb2 as validate_dot_validate__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12\x61pi/v1/event.proto\x12\x06\x61pi.v1\x1a\x16\x63ommon/v1/errors.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a\x1b\x62uf/validate/validate.proto\"l\n\x08Resolved\x12,\n\x05value\x18\x01 \x01(\x0b\x32\x16.google.protobuf.ValueR\x05value\x12\x32\n\x08\x62indings\x18\x02 \x03(\x0b\x32\x16.google.protobuf.ValueR\x08\x62indings\"\x9a\x06\n\x05\x45vent\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x38\n\x04type\x18\x02 \x01(\x0e\x32\x11.api.v1.BlockTypeB\x11\xfa\x42\x05\x82\x01\x02 \x00\xbaH\x06\x82\x01\x03\"\x01\x00R\x04type\x12\x38\n\ttimestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\ttimestamp\x12+\n\x05start\x18\x04 \x01(\x0b\x32\x13.api.v1.Event.StartH\x00R\x05start\x12%\n\x03\x65nd\x18\x05 \x01(\x0b\x32\x11.api.v1.Event.EndH\x00R\x03\x65nd\x12(\n\x04\x64\x61ta\x18\x07 \x01(\x0b\x32\x12.api.v1.Event.DataH\x00R\x04\x64\x61ta\x12\x1b\n\x06parent\x18\x06 \x01(\tH\x01R\x06parent\x88\x01\x01\x12,\n\x0f\x65xecution_index\x18\x08 \x01(\tH\x02R\x0e\x65xecutionIndex\x88\x01\x01\x1a\x34\n\x04\x44\x61ta\x12,\n\x05value\x18\x01 \x01(\x0b\x32\x16.google.protobuf.ValueR\x05value\x1a\x07\n\x05Start\x1a\xd8\x02\n\x03\x45nd\x12\x35\n\x0bperformance\x18\x01 \x01(\x0b\x32\x13.api.v1.PerformanceR\x0bperformance\x12&\n\x06output\x18\x02 \x01(\x0b\x32\x0e.api.v1.OutputR\x06output\x12&\n\x05\x65rror\x18\x03 \x01(\x0b\x32\x10.common.v1.ErrorR\x05\x65rror\x12>\n\x06status\x18\x04 \x01(\x0e\x32\x13.api.v1.BlockStatusB\x11\xfa\x42\x05\x82\x01\x02 \x00\xbaH\x06\x82\x01\x03\"\x01\x00R\x06status\x12;\n\x08resolved\x18\x05 \x03(\x0b\x32\x1f.api.v1.Event.End.ResolvedEntryR\x08resolved\x1aM\n\rResolvedEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12&\n\x05value\x18\x02 \x01(\x0b\x32\x10.api.v1.ResolvedR\x05value:\x02\x38\x01\x42\x07\n\x05\x65ventB\t\n\x07_parentB\x12\n\x10_execution_index\"\xff\x01\n\x0bPerformance\x12\x14\n\x05start\x18\x01 \x01(\x03R\x05start\x12\x16\n\x06\x66inish\x18\x02 \x01(\x03R\x06\x66inish\x12\x14\n\x05total\x18\x03 \x01(\x03R\x05total\x12\x1c\n\texecution\x18\x04 \x01(\x03R\texecution\x12\x1a\n\x08overhead\x18\x05 \x01(\x03R\x08overhead\x12\x37\n\x06\x63ustom\x18\x06 \x03(\x0b\x32\x1f.api.v1.Performance.CustomEntryR\x06\x63ustom\x1a\x39\n\x0b\x43ustomEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\x03R\x05value:\x02\x38\x01\"\xa5\x02\n\x06Output\x12.\n\x06result\x18\x01 \x01(\x0b\x32\x16.google.protobuf.ValueR\x06result\x12\x18\n\x07request\x18\x02 \x01(\tR\x07request\x12\x16\n\x06stdout\x18\x03 \x03(\tR\x06stdout\x12\x16\n\x06stderr\x18\x04 \x03(\tR\x06stderr\x12\x35\n\nrequest_v2\x18\x05 \x01(\x0b\x32\x16.api.v1.Output.RequestR\trequestV2\x1aj\n\x07Request\x12\x18\n\x07summary\x18\x01 \x01(\tR\x07summary\x12\x38\n\x08metadata\x18\x05 \x01(\x0b\x32\x17.google.protobuf.StructH\x00R\x08metadata\x88\x01\x01\x42\x0b\n\t_metadata\"\xad\x01\n\tOutputOld\x12.\n\x06output\x18\x01 \x01(\x0b\x32\x16.google.protobuf.ValueR\x06output\x12\x10\n\x03log\x18\x02 \x03(\tR\x03log\x12\x18\n\x07request\x18\x03 \x01(\tR\x07request\x12\x44\n\x12place_holders_info\x18\x04 \x01(\x0b\x32\x16.google.protobuf.ValueR\x10placeHoldersInfo*a\n\x0b\x42lockStatus\x12\x1c\n\x18\x42LOCK_STATUS_UNSPECIFIED\x10\x00\x12\x1a\n\x16\x42LOCK_STATUS_SUCCEEDED\x10\x01\x12\x18\n\x14\x42LOCK_STATUS_ERRORED\x10\x02*\xbd\x02\n\tBlockType\x12\x1a\n\x16\x42LOCK_TYPE_UNSPECIFIED\x10\x00\x12\x14\n\x10\x42LOCK_TYPE_BREAK\x10\x01\x12\x15\n\x11\x42LOCK_TYPE_RETURN\x10\x02\x12\x13\n\x0f\x42LOCK_TYPE_WAIT\x10\x03\x12\x17\n\x13\x42LOCK_TYPE_PARALLEL\x10\x04\x12\x1a\n\x16\x42LOCK_TYPE_CONDITIONAL\x10\x05\x12\x13\n\x0f\x42LOCK_TYPE_LOOP\x10\x06\x12\x17\n\x13\x42LOCK_TYPE_TRYCATCH\x10\x07\x12\x13\n\x0f\x42LOCK_TYPE_STEP\x10\x08\x12\x18\n\x14\x42LOCK_TYPE_VARIABLES\x10\t\x12\x14\n\x10\x42LOCK_TYPE_THROW\x10\n\x12\x13\n\x0f\x42LOCK_TYPE_SEND\x10\x0b\x12\x15\n\x11\x42LOCK_TYPE_STREAM\x10\x0c\x42\x30Z.github.com/superblocksteam/types/gen/go/api/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api.v1.event_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/integration_auth_service_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/integration_auth_service_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from superblocks_types.google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
-from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-from validate import validate_pb2 as validate_dot_validate__pb2
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
-from plugins.common.v1 import auth_pb2 as plugins_dot_common_dot_v1_dot_auth__pb2
-from common.v1 import common_pb2 as common_dot_v1_dot_common__pb2
+from superblocks_types.protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
+from superblocks_types.validate import validate_pb2 as validate_dot_validate__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.plugins.common.v1 import auth_pb2 as plugins_dot_common_dot_v1_dot_auth__pb2
+from superblocks_types.common.v1 import common_pb2 as common_dot_v1_dot_common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%api/v1/integration_auth_service.proto\x12\x06\x61pi.v1\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x17validate/validate.proto\x1a\x1b\x62uf/validate/validate.proto\x1a\x1cplugins/common/v1/auth.proto\x1a\x16\x63ommon/v1/common.proto\"y\n\x10\x43heckAuthRequest\x12\x37\n\x0eintegration_id\x18\x01 \x01(\tB\x10\xfa\x42\x05r\x03\xb0\x01\x01\xbaH\x05r\x03\xb0\x01\x01R\rintegrationId\x12,\n\x07profile\x18\x02 \x01(\x0b\x32\x12.common.v1.ProfileR\x07profile\"9\n\x11\x43heckAuthResponse\x12$\n\rauthenticated\x18\x01 \x01(\x08R\rauthenticated\"\xc2\x02\n\x0cLoginRequest\x12\x37\n\x0eintegration_id\x18\x01 \x01(\tB\x10\xfa\x42\x05r\x03\xb0\x01\x01\xbaH\x05r\x03\xb0\x01\x01R\rintegrationId\x12,\n\x07profile\x18\x02 \x01(\x0b\x32\x12.common.v1.ProfileR\x07profile\x12\x19\n\x05token\x18\x03 \x01(\tH\x00R\x05token\x88\x01\x01\x12\'\n\x0crefreshToken\x18\x04 \x01(\tH\x01R\x0crefreshToken\x88\x01\x01\x12\x1d\n\x07idToken\x18\x05 \x01(\tH\x02R\x07idToken\x88\x01\x01\x12-\n\x0f\x65xpiryTimestamp\x18\x06 \x01(\x03H\x03R\x0f\x65xpiryTimestamp\x88\x01\x01\x42\x08\n\x06_tokenB\x0f\n\r_refreshTokenB\n\n\x08_idTokenB\x12\n\x10_expiryTimestamp\")\n\rLoginResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\"\xd7\x02\n ExchangeOauthCodeForTokenRequest\x12\x39\n\x0eintegration_id\x18\x01 \x01(\tB\x12\x18\x01\xfa\x42\x05r\x03\xb0\x01\x01\xbaH\x05r\x03\xb0\x01\x01R\rintegrationId\x12,\n\x07profile\x18\x02 \x01(\x0b\x32\x12.common.v1.ProfileR\x07profile\x12\x1f\n\x0b\x61\x63\x63\x65ss_code\x18\x03 \x01(\tR\naccessCode\x12\x1b\n\tauth_type\x18\x04 \x01(\tR\x08\x61uthType\x12O\n\x0b\x61uth_config\x18\x05 \x01(\x0b\x32..plugins.common.v1.OAuth.AuthorizationCodeFlowR\nauthConfig\x12;\n\x10\x63onfiguration_id\x18\x06 \x01(\tB\x10\xfa\x42\x05r\x03\xb0\x01\x01\xbaH\x05r\x03\xb0\x01\x01R\x0f\x63onfigurationId\"\xc1\x01\n RequestOauthPasswordTokenRequest\x12\x37\n\x0eintegration_id\x18\x01 \x01(\tB\x10\xfa\x42\x05r\x03\xb0\x01\x01\xbaH\x05r\x03\xb0\x01\x01R\rintegrationId\x12,\n\x07profile\x18\x02 \x01(\x0b\x32\x12.common.v1.ProfileR\x07profile\x12\x1a\n\x08username\x18\x03 \x01(\tR\x08username\x12\x1a\n\x08password\x18\x04 \x01(\tR\x08password\"\x96\x01\n!RequestOauthPasswordTokenResponse\x12!\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\tR\x0b\x61\x63\x63\x65ssToken\x12#\n\rrefresh_token\x18\x02 \x01(\tR\x0crefreshToken\x12)\n\x10\x65xpiry_timestamp\x18\x03 \x01(\x03R\x0f\x65xpiryTimestamp2\xf4\x04\n\x16IntegrationAuthService\x12i\n\tCheckAuth\x12\x18.api.v1.CheckAuthRequest\x1a\x19.api.v1.CheckAuthResponse\"\'\x92\x41\x0b*\tCheckAuth\x82\xd3\xe4\x93\x02\x13\"\x0e/v1/check-auth:\x01*\x12T\n\x05Login\x12\x14.api.v1.LoginRequest\x1a\x15.api.v1.LoginResponse\"\x1e\x92\x41\x07*\x05Login\x82\xd3\xe4\x93\x02\x0e\"\t/v1/login:\x01*\x12Z\n\x06Logout\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\" \x92\x41\x08*\x06Logout\x82\xd3\xe4\x93\x02\x0f\"\n/v1/logout:\x01*\x12\x99\x01\n\x19\x45xchangeOauthCodeForToken\x12(.api.v1.ExchangeOauthCodeForTokenRequest\x1a\x16.google.protobuf.Empty\":\x92\x41\x1b*\x19\x45xchangeOauthCodeForToken\x82\xd3\xe4\x93\x02\x16\"\x11/v1/exchange-code:\x01*\x12\xa0\x01\n\x19RequestOauthPasswordToken\x12(.api.v1.RequestOauthPasswordTokenRequest\x1a).api.v1.RequestOauthPasswordTokenResponse\".\x92\x41\x0f*\rRequest Token\x82\xd3\xe4\x93\x02\x16\"\x11/v1/request-token:\x01*B0Z.github.com/superblocksteam/types/gen/go/api/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api.v1.integration_auth_service_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/integration_auth_service_pb2_grpc.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/integration_auth_service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from api.v1 import integration_auth_service_pb2 as api_dot_v1_dot_integration__auth__service__pb2
+from superblocks_types.api.v1 import integration_auth_service_pb2 as api_dot_v1_dot_integration__auth__service__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
 class IntegrationAuthServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/requests_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/requests_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from api.v1 import api_pb2 as api_dot_v1_dot_api__pb2
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
-from common.v1 import errors_pb2 as common_dot_v1_dot_errors__pb2
+from superblocks_types.api.v1 import api_pb2 as api_dot_v1_dot_api__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.common.v1 import errors_pb2 as common_dot_v1_dot_errors__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
-from utils.v1 import utils_pb2 as utils_dot_v1_dot_utils__pb2
-from common.v1 import api_pb2 as common_dot_v1_dot_api__pb2
+from superblocks_types.utils.v1 import utils_pb2 as utils_dot_v1_dot_utils__pb2
+from superblocks_types.common.v1 import api_pb2 as common_dot_v1_dot_api__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x61pi/v1/requests.proto\x12\x06\x61pi.v1\x1a\x10\x61pi/v1/api.proto\x1a\x1b\x62uf/validate/validate.proto\x1a\x16\x63ommon/v1/errors.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x14utils/v1/utils.proto\x1a\x13\x63ommon/v1/api.proto\"}\n\x08PatchApi\x12\x1d\n\x03\x61pi\x18\x01 \x01(\x0b\x32\x0b.api.v1.ApiR\x03\x61pi\x12\x1d\n\tcommit_id\x18\x02 \x01(\tH\x00R\x08\x63ommitId\x12!\n\x0b\x62ranch_name\x18\x03 \x01(\tH\x00R\nbranchNameB\x10\n\x07git_ref\x12\x05\xbaH\x02\x08\x01\">\n\x10PatchApisRequest\x12*\n\x07patches\x18\x01 \x03(\x0b\x32\x10.api.v1.PatchApiR\x07patches\"\xcf\x02\n\x11PatchApisResponse\x12<\n\x08statuses\x18\x01 \x03(\x0b\x32 .api.v1.PatchApisResponse.StatusR\x08statuses\x12:\n\x05links\x18\x02 \x03(\x0b\x32$.api.v1.PatchApisResponse.LinksEntryR\x05links\x1au\n\x06Status\x12\x15\n\x06\x61pi_id\x18\x01 \x01(\tR\x05\x61piId\x12\x12\n\x04\x63ode\x18\x02 \x01(\x05R\x04\x63ode\x12\x18\n\x07message\x18\x03 \x01(\tR\x07message\x12&\n\x05\x65rror\x18\x04 \x01(\x0b\x32\x10.common.v1.ErrorR\x05\x65rror\x1aI\n\nLinksEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x0f.common.v1.LinkR\x05value:\x02\x38\x01\"\xa3\x02\n\x1aUpdateApplicationSignature\x12%\n\x0e\x61pplication_id\x18\x01 \x01(\tR\rapplicationId\x12\x1d\n\tcommit_id\x18\x02 \x01(\tH\x00R\x08\x63ommitId\x12!\n\x0b\x62ranch_name\x18\x03 \x01(\tH\x00R\nbranchName\x12\x31\n\tsignature\x18\x04 \x01(\x0b\x32\x13.utils.v1.SignatureR\tsignature\x12\x34\n\x07updated\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07updated\x12!\n\x0cpage_version\x18\x06 \x01(\x05R\x0bpageVersionB\x10\n\x07git_ref\x12\x05\xbaH\x02\x08\x01\"b\n\"UpdateApplicationSignaturesRequest\x12<\n\x07updates\x18\x01 \x03(\x0b\x32\".api.v1.UpdateApplicationSignatureR\x07updates\"\xea\x03\n#UpdateApplicationSignaturesResponse\x12N\n\x08statuses\x18\x01 \x03(\x0b\x32\x32.api.v1.UpdateApplicationSignaturesResponse.StatusR\x08statuses\x12L\n\x05links\x18\x02 \x03(\x0b\x32\x36.api.v1.UpdateApplicationSignaturesResponse.LinksEntryR\x05links\x1a\xd9\x01\n\x06Status\x12%\n\x0e\x61pplication_id\x18\x01 \x01(\tR\rapplicationId\x12\x1d\n\tcommit_id\x18\x02 \x01(\tH\x00R\x08\x63ommitId\x12!\n\x0b\x62ranch_name\x18\x03 \x01(\tH\x00R\nbranchName\x12\x12\n\x04\x63ode\x18\x04 \x01(\x05R\x04\x63ode\x12\x18\n\x07message\x18\x05 \x01(\tR\x07message\x12&\n\x05\x65rror\x18\x06 \x01(\x0b\x32\x10.common.v1.ErrorR\x05\x65rrorB\x10\n\x07git_ref\x12\x05\xbaH\x02\x08\x01\x1aI\n\nLinksEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x0f.common.v1.LinkR\x05value:\x02\x38\x01\"~\n\x0cGenericBatch\x12\x36\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x1a.api.v1.GenericBatch.ItemsB\x06\xbaH\x03\xc8\x01\x01R\x04\x64\x61ta\x1a\x36\n\x05Items\x12-\n\x05items\x18\x01 \x03(\x0b\x32\x17.google.protobuf.StructR\x05items\"H\n\x14GenericBatchResponse\x12\x30\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x14.api.v1.GenericBatchB\x06\xbaH\x03\xc8\x01\x01R\x04\x64\x61taB0Z.github.com/superblocksteam/types/gen/go/api/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api.v1.requests_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/service_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from api.v1 import api_pb2 as api_dot_v1_dot_api__pb2
-from api.v1 import event_pb2 as api_dot_v1_dot_event__pb2
-from common.v1 import common_pb2 as common_dot_v1_dot_common__pb2
-from plugins.cosmosdb.v1 import plugin_pb2 as plugins_dot_cosmosdb_dot_v1_dot_plugin__pb2
-from plugins.adls.v1 import plugin_pb2 as plugins_dot_adls_dot_v1_dot_plugin__pb2
-from store.v1 import store_pb2 as store_dot_v1_dot_store__pb2
-from common.v1 import errors_pb2 as common_dot_v1_dot_errors__pb2
-from common.v1 import health_pb2 as common_dot_v1_dot_health__pb2
-from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from superblocks_types.api.v1 import api_pb2 as api_dot_v1_dot_api__pb2
+from superblocks_types.api.v1 import event_pb2 as api_dot_v1_dot_event__pb2
+from superblocks_types.common.v1 import common_pb2 as common_dot_v1_dot_common__pb2
+from superblocks_types.plugins.cosmosdb.v1 import plugin_pb2 as plugins_dot_cosmosdb_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.adls.v1 import plugin_pb2 as plugins_dot_adls_dot_v1_dot_plugin__pb2
+from superblocks_types.store.v1 import store_pb2 as store_dot_v1_dot_store__pb2
+from superblocks_types.common.v1 import errors_pb2 as common_dot_v1_dot_errors__pb2
+from superblocks_types.common.v1 import health_pb2 as common_dot_v1_dot_health__pb2
+from superblocks_types.google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
-from plugins.kafka.v1 import plugin_pb2 as plugins_dot_kafka_dot_v1_dot_plugin__pb2
-from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-from validate import validate_pb2 as validate_dot_validate__pb2
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.plugins.kafka.v1 import plugin_pb2 as plugins_dot_kafka_dot_v1_dot_plugin__pb2
+from superblocks_types.protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
+from superblocks_types.validate import validate_pb2 as validate_dot_validate__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x61pi/v1/service.proto\x12\x06\x61pi.v1\x1a\x10\x61pi/v1/api.proto\x1a\x12\x61pi/v1/event.proto\x1a\x16\x63ommon/v1/common.proto\x1a plugins/cosmosdb/v1/plugin.proto\x1a\x1cplugins/adls/v1/plugin.proto\x1a\x14store/v1/store.proto\x1a\x16\x63ommon/v1/errors.proto\x1a\x16\x63ommon/v1/health.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1dplugins/kafka/v1/plugin.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x17validate/validate.proto\x1a\x1b\x62uf/validate/validate.proto\"+\n\rHealthRequest\x12\x1a\n\x08\x64\x65tailed\x18\x01 \x01(\x08R\x08\x64\x65tailed\"0\n\x0fValidateRequest\x12\x1d\n\x03\x61pi\x18\x01 \x01(\x0b\x32\x0b.api.v1.ApiR\x03\x61pi\"\x8d\t\n\x0e\x45xecuteRequest\x12\x38\n\x07options\x18\x01 \x01(\x0b\x32\x1e.api.v1.ExecuteRequest.OptionsR\x07options\x12:\n\x06inputs\x18\x02 \x03(\x0b\x32\".api.v1.ExecuteRequest.InputsEntryR\x06inputs\x12\x34\n\ndefinition\x18\x03 \x01(\x0b\x32\x12.api.v1.DefinitionH\x00R\ndefinition\x12\x34\n\x05\x66\x65tch\x18\x04 \x01(\x0b\x32\x1c.api.v1.ExecuteRequest.FetchH\x00R\x05\x66\x65tch\x12\x31\n\x05\x66iles\x18\x05 \x03(\x0b\x32\x1b.api.v1.ExecuteRequest.FileR\x05\x66iles\x12,\n\x07profile\x18\x06 \x01(\x0b\x32\x12.common.v1.ProfileR\x07profile\x1a\x9a\x02\n\x07Options\x12%\n\x0e\x65xclude_output\x18\x01 \x01(\x08R\rexcludeOutput\x12\x32\n\x15include_event_outputs\x18\x02 \x01(\x08R\x13includeEventOutputs\x12%\n\x0einclude_events\x18\x03 \x01(\x08R\rincludeEvents\x12\x14\n\x05start\x18\x04 \x01(\tR\x05start\x12\x12\n\x04stop\x18\x05 \x01(\tR\x04stop\x12)\n\x10include_resolved\x18\x06 \x01(\x08R\x0fincludeResolved\x12\x14\n\x05\x61sync\x18\x07 \x01(\x08R\x05\x61sync\x12\"\n\x05mocks\x18\x08 \x03(\x0b\x32\x0c.api.v1.MockR\x05mocks\x1a\xa1\x02\n\x05\x46\x65tch\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12,\n\x07profile\x18\x02 \x01(\x0b\x32\x12.common.v1.ProfileR\x07profile\x12\x17\n\x04test\x18\x03 \x01(\x08H\x00R\x04test\x88\x01\x01\x12\x19\n\x05token\x18\x04 \x01(\tH\x01R\x05token\x88\x01\x01\x12-\n\tview_mode\x18\x05 \x01(\x0e\x32\x10.api.v1.ViewModeR\x08viewMode\x12 \n\tcommit_id\x18\x06 \x01(\tH\x02R\x08\x63ommitId\x88\x01\x01\x12$\n\x0b\x62ranch_name\x18\x07 \x01(\tH\x03R\nbranchName\x88\x01\x01\x42\x07\n\x05_testB\x08\n\x06_tokenB\x0c\n\n_commit_idB\x0e\n\x0c_branch_name\x1aQ\n\x0bInputsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.ValueR\x05value:\x02\x38\x01\x1a\x8e\x01\n\x04\x46ile\x12\"\n\x0coriginalName\x18\x01 \x01(\tR\x0coriginalName\x12\x16\n\x06\x62uffer\x18\x02 \x01(\x0cR\x06\x62uffer\x12\x1a\n\x08\x65ncoding\x18\x03 \x01(\tR\x08\x65ncoding\x12\x1a\n\x08mimeType\x18\x04 \x01(\tR\x08mimeType\x12\x12\n\x04size\x18\x05 \x01(\tR\x04sizeB\x13\n\x07request\x12\x08\xf8\x42\x01\xbaH\x02\x08\x01\"\xb5\x04\n\nDefinition\x12-\n\x03\x61pi\x18\x01 \x01(\x0b\x32\x0b.api.v1.ApiB\x0e\xfa\x42\x05\x8a\x01\x02\x10\x01\xbaH\x03\xc8\x01\x01R\x03\x61pi\x12H\n\x0cintegrations\x18\x02 \x03(\x0b\x32$.api.v1.Definition.IntegrationsEntryR\x0cintegrations\x12\x37\n\x08metadata\x18\x03 \x01(\x0b\x32\x1b.api.v1.Definition.MetadataR\x08metadata\x12(\n\x06stores\x18\x04 \x01(\x0b\x32\x10.store.v1.StoresR\x06stores\x1a\xf0\x01\n\x08Metadata\x12\x1c\n\trequester\x18\x01 \x01(\tR\trequester\x12\x18\n\x07profile\x18\x02 \x01(\tR\x07profile\x12+\n\x11organization_plan\x18\x03 \x01(\tR\x10organizationPlan\x12+\n\x11organization_name\x18\x04 \x01(\tR\x10organizationName\x12?\n\x0erequester_type\x18\x05 \x01(\x0e\x32\x13.common.v1.UserTypeH\x00R\rrequesterType\x88\x01\x01\x42\x11\n\x0f_requester_type\x1aX\n\x11IntegrationsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x17.google.protobuf.StructR\x05value:\x02\x38\x01\"-\n\rStatusRequest\x12\x1c\n\texecution\x18\x01 \x01(\tR\texecution\"\xe1\x02\n\rAwaitResponse\x12\x1c\n\texecution\x18\x01 \x01(\tR\texecution\x12&\n\x06output\x18\x02 \x01(\x0b\x32\x0e.api.v1.OutputR\x06output\x12(\n\x06\x65rrors\x18\x03 \x03(\x0b\x32\x10.common.v1.ErrorR\x06\x65rrors\x12\x34\n\x06status\x18\x04 \x01(\x0e\x32\x1c.api.v1.AwaitResponse.StatusR\x06status\x12\x35\n\x0bperformance\x18\x05 \x01(\x0b\x32\x13.api.v1.PerformanceR\x0bperformance\x12%\n\x06\x65vents\x18\x06 \x03(\x0b\x32\r.api.v1.EventR\x06\x65vents\"L\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x14\n\x10STATUS_COMPLETED\x10\x01\x12\x14\n\x10STATUS_EXECUTING\x10\x02\"U\n\rAsyncResponse\x12\x1c\n\texecution\x18\x01 \x01(\tR\texecution\x12&\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x10.common.v1.ErrorR\x05\x65rror\"S\n\x0eStreamResponse\x12\x1c\n\texecution\x18\x01 \x01(\tR\texecution\x12#\n\x05\x65vent\x18\x02 \x01(\x0b\x32\r.api.v1.EventR\x05\x65vent\"e\n\rOutputRequest\x12.\n\texecution\x18\x01 \x01(\tB\x10\xfa\x42\x05r\x03\xb0\x01\x01\xbaH\x05r\x03\xb0\x01\x01R\texecution\x12$\n\x05\x62lock\x18\x02 \x01(\tB\x0e\xfa\x42\x04r\x02\x10\x01\xbaH\x04r\x02\x10\x01R\x05\x62lock\"\x91\x01\n\x0eOutputResponse\x12/\n\x08metadata\x18\x01 \x01(\x0b\x32\x13.common.v1.MetadataR\x08metadata\x12&\n\x06output\x18\x02 \x01(\x0b\x32\x0e.api.v1.OutputR\x06output\x12&\n\x05\x65rror\x18\x03 \x01(\x0b\x32\x10.common.v1.ErrorR\x05\x65rror\"-\n\rCancelRequest\x12\x1c\n\texecution\x18\x01 \x01(\tR\texecution\"8\n\x0e\x43\x61ncelResponse\x12&\n\x05\x65rror\x18\x01 \x01(\x0b\x32\x10.common.v1.ErrorR\x05\x65rror\"\xd7\x01\n\x0bTestRequest\x12\x44\n\x11\x64\x61tasource_config\x18\x01 \x01(\x0b\x32\x17.google.protobuf.StructR\x10\x64\x61tasourceConfig\x12)\n\x10integration_type\x18\x02 \x01(\tR\x0fintegrationType\x12)\n\x10\x63onfiguration_id\x18\x03 \x01(\tR\x0f\x63onfigurationId\x12,\n\x07profile\x18\x04 \x01(\x0b\x32\x12.common.v1.ProfileR\x07profile\"\x0e\n\x0cTestResponse\"\xab\x01\n\rDeleteRequest\x12 \n\x0bintegration\x18\x01 \x01(\tR\x0bintegration\x12,\n\x07profile\x18\x02 \x01(\x0b\x32\x12.common.v1.ProfileR\x07profile\x12)\n\x10\x63onfiguration_id\x18\x03 \x01(\tR\x0f\x63onfigurationId\x12\x1f\n\x0bplugin_name\x18\x04 \x01(\tR\npluginName\"\x10\n\x0e\x44\x65leteResponse\"\xe3\x01\n\x08\x46unction\x1a\x65\n\x07Request\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x36\n\nparameters\x18\x03 \x03(\x0b\x32\x16.google.protobuf.ValueR\nparameters\x1ap\n\x08Response\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.ValueR\x05value\x12&\n\x05\x65rror\x18\x03 \x01(\x0b\x32\x10.common.v1.ErrorR\x05\x65rror\"\x84\x01\n\rTwoWayRequest\x12\x32\n\x07\x65xecute\x18\x01 \x01(\x0b\x32\x16.api.v1.ExecuteRequestH\x00R\x07\x65xecute\x12\x37\n\x08\x66unction\x18\x02 \x01(\x0b\x32\x19.api.v1.Function.ResponseH\x00R\x08\x66unctionB\x06\n\x04type\"\x82\x01\n\x0eTwoWayResponse\x12\x30\n\x06stream\x18\x01 \x01(\x0b\x32\x16.api.v1.StreamResponseH\x00R\x06stream\x12\x36\n\x08\x66unction\x18\x02 \x01(\x0b\x32\x18.api.v1.Function.RequestH\x00R\x08\x66unctionB\x06\n\x04type\"\xe2\x03\n\x04Mock\x12\x1f\n\x02on\x18\x01 \x01(\x0b\x32\x0f.api.v1.Mock.OnR\x02on\x12+\n\x06return\x18\x02 \x01(\x0b\x32\x13.api.v1.Mock.ReturnR\x06return\x1a\xbd\x01\n\x06Params\x12.\n\x10integration_type\x18\x01 \x01(\tH\x00R\x0fintegrationType\x88\x01\x01\x12 \n\tstep_name\x18\x02 \x01(\tH\x01R\x08stepName\x88\x01\x01\x12\x33\n\x06inputs\x18\x03 \x01(\x0b\x32\x16.google.protobuf.ValueH\x02R\x06inputs\x88\x01\x01\x42\x13\n\x11_integration_typeB\x0c\n\n_step_nameB\t\n\x07_inputs\x1al\n\x02On\x12\x30\n\x06static\x18\x01 \x01(\x0b\x32\x13.api.v1.Mock.ParamsH\x00R\x06static\x88\x01\x01\x12\x1d\n\x07\x64ynamic\x18\x02 \x01(\tH\x01R\x07\x64ynamic\x88\x01\x01\x42\t\n\x07_staticB\n\n\x08_dynamic\x1a^\n\x06Return\x12\x30\n\x06static\x18\x01 \x01(\x0b\x32\x16.google.protobuf.ValueH\x00R\x06static\x12\x1a\n\x07\x64ynamic\x18\x02 \x01(\tH\x00R\x07\x64ynamicB\x06\n\x04type\"\x82\x01\n\x19MetadataRequestDeprecated\x12 \n\x0bintegration\x18\x01 \x01(\tR\x0bintegration\x12\x15\n\x06\x61pi_id\x18\x02 \x01(\tR\x05\x61piId\x12,\n\x07profile\x18\x03 \x01(\x0b\x32\x12.common.v1.ProfileR\x07profile\"\xa9\x01\n\x0fMetadataRequest\x12 \n\x0bintegration\x18\x01 \x01(\tR\x0bintegration\x12,\n\x07profile\x18\x02 \x01(\x0b\x32\x12.common.v1.ProfileR\x07profile\x12\x46\n\x12step_configuration\x18\x03 \x01(\x0b\x32\x17.google.protobuf.StructR\x11stepConfiguration\"\xd1\n\n\x10MetadataResponse\x12k\n\x18\x64\x61tabase_schema_metadata\x18\x01 \x01(\x0b\x32/.api.v1.MetadataResponse.DatabaseSchemaMetadataH\x00R\x16\x64\x61tabaseSchemaMetadata\x12U\n\x10\x62uckets_metadata\x18\x02 \x01(\x0b\x32(.api.v1.MetadataResponse.BucketsMetadataH\x00R\x0f\x62ucketsMetadata\x12\x32\n\x05kafka\x18\x03 \x01(\x0b\x32\x1a.plugins.kafka.v1.MetadataH\x00R\x05kafka\x12\x42\n\x08\x63osmosdb\x18\x04 \x01(\x0b\x32$.plugins.cosmosdb.v1.Plugin.MetadataH\x00R\x08\x63osmosdb\x12\x36\n\x04\x61\x64ls\x18\x05 \x01(\x0b\x32 .plugins.adls.v1.Plugin.MetadataH\x00R\x04\x61\x64ls\x12\x36\n\x18g_sheets_next_page_token\x18\x06 \x01(\tR\x14gSheetsNextPageToken\x1a\x88\x06\n\x16\x44\x61tabaseSchemaMetadata\x12M\n\x06tables\x18\x01 \x03(\x0b\x32\x35.api.v1.MetadataResponse.DatabaseSchemaMetadata.TableR\x06tables\x12P\n\x07schemas\x18\x02 \x03(\x0b\x32\x36.api.v1.MetadataResponse.DatabaseSchemaMetadata.SchemaR\x07schemas\x1aS\n\x06\x43olumn\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x12\n\x04type\x18\x02 \x01(\tR\x04type\x12!\n\x0c\x65scaped_name\x18\x03 \x01(\tR\x0b\x65scapedName\x1aG\n\x03Key\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x12\n\x04type\x18\x02 \x01(\tR\x04type\x12\x18\n\x07\x63olumns\x18\x03 \x03(\tR\x07\x63olumns\x1a\x34\n\x08Template\x12\x14\n\x05title\x18\x01 \x01(\tR\x05title\x12\x12\n\x04\x62ody\x18\x02 \x01(\tR\x04\x62ody\x1a\xca\x02\n\x05Table\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04type\x18\x02 \x01(\tR\x04type\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12P\n\x07\x63olumns\x18\x04 \x03(\x0b\x32\x36.api.v1.MetadataResponse.DatabaseSchemaMetadata.ColumnR\x07\x63olumns\x12G\n\x04keys\x18\x05 \x03(\x0b\x32\x33.api.v1.MetadataResponse.DatabaseSchemaMetadata.KeyR\x04keys\x12V\n\ttemplates\x18\x06 \x03(\x0b\x32\x38.api.v1.MetadataResponse.DatabaseSchemaMetadata.TemplateR\ttemplates\x12\x16\n\x06schema\x18\x07 \x01(\tR\x06schema\x1a,\n\x06Schema\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x1a$\n\x0e\x42ucketMetadata\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x1aT\n\x0f\x42ucketsMetadata\x12\x41\n\x07\x62uckets\x18\x01 \x03(\x0b\x32\'.api.v1.MetadataResponse.BucketMetadataR\x07\x62ucketsB\n\n\x08metadata\"-\n\x0f\x44ownloadRequest\x12\x1a\n\x08location\x18\x01 \x01(\tR\x08location\"&\n\x10\x44ownloadResponse\x12\x12\n\x04\x64\x61ta\x18\x01 \x01(\x0cR\x04\x64\x61ta\"\xe6\x01\n\x10WorkflowResponse\x12*\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x16.google.protobuf.ValueR\x04\x64\x61ta\x12J\n\rresponse_meta\x18\x02 \x01(\x0b\x32%.api.v1.WorkflowResponse.ResponseMetaR\x0cresponseMeta\x1aZ\n\x0cResponseMeta\x12\x16\n\x06status\x18\x01 \x01(\x05R\x06status\x12\x18\n\x07message\x18\x02 \x01(\tR\x07message\x12\x18\n\x07success\x18\x03 \x01(\x08R\x07success*h\n\x08ViewMode\x12\x19\n\x15VIEW_MODE_UNSPECIFIED\x10\x00\x12\x12\n\x0eVIEW_MODE_EDIT\x10\x01\x12\x15\n\x11VIEW_MODE_PREVIEW\x10\x02\x12\x16\n\x12VIEW_MODE_DEPLOYED\x10\x03\x32q\n\x0fMetadataService\x12^\n\x06Health\x12\x15.api.v1.HealthRequest\x1a\x19.common.v1.HealthResponse\"\"\x92\x41\x10*\x0eService Health\x82\xd3\xe4\x93\x02\t\x12\x07/health2\xbc\x01\n\x11\x44\x65precatedService\x12\xa6\x01\n\x08Workflow\x12\x16.api.v1.ExecuteRequest\x1a\x18.api.v1.WorkflowResponse\"h\x92\x41\x19*\x17Sync Workflow Execution\x82\xd3\xe4\x93\x02\x46\"\x1a/v1/workflows/{fetch.id=*}:\x01*Z%\" /agent/v1/workflows/{fetch.id=*}:\x01*2\xaa\x0b\n\x0f\x45xecutorService\x12\x80\x01\n\x05\x41wait\x12\x16.api.v1.ExecuteRequest\x1a\x15.api.v1.AwaitResponse\"H\x92\x41\x10\x12\x0e\x45xecute an API\x82\xd3\xe4\x93\x02/\"\x0b/v2/execute:\x01*Z\x1d\"\x18/v2/execute/{fetch.id=*}:\x01*\x12\x43\n\x0cTwoWayStream\x12\x15.api.v1.TwoWayRequest\x1a\x16.api.v1.TwoWayResponse\"\x00(\x01\x30\x01\x12\x80\x01\n\x12MetadataDeprecated\x12!.api.v1.MetadataRequestDeprecated\x1a\x18.api.v1.MetadataResponse\"-\x92\x41\x16*\x14Integration Metadata\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v2/metadata\x12o\n\x08Metadata\x12\x17.api.v1.MetadataRequest\x1a\x18.api.v1.MetadataResponse\"0\x92\x41\x16*\x14Integration Metadata\x82\xd3\xe4\x93\x02\x11\"\x0c/v2/metadata:\x01*\x12\x66\n\x04Test\x12\x13.api.v1.TestRequest\x1a\x14.api.v1.TestResponse\"3\x92\x41\x1d*\x1bIntegration Connection Test\x82\xd3\xe4\x93\x02\r\"\x08/v2/test:\x01*\x12j\n\x06\x44\x65lete\x12\x15.api.v1.DeleteRequest\x1a\x16.api.v1.DeleteResponse\"1\x92\x41\x19*\x17\x44\x65lete Integration Hook\x82\xd3\xe4\x93\x02\x0f\"\n/v2/delete:\x01*\x12h\n\x05\x41sync\x12\x16.api.v1.ExecuteRequest\x1a\x15.api.v1.AsyncResponse\"0\x92\x41\x11*\x0f\x41sync Execution\x82\xd3\xe4\x93\x02\x16\"\x11/v2/execute/async:\x01*\x12\x94\x01\n\x06Stream\x12\x16.api.v1.ExecuteRequest\x1a\x16.api.v1.StreamResponse\"X\x92\x41\x12*\x10Stream Execution\x82\xd3\xe4\x93\x02=\"\x12/v2/execute/stream:\x01*Z$\"\x1f/v2/execute/stream/{fetch.id=*}:\x01*0\x01\x12_\n\x06Status\x12\x15.api.v1.StatusRequest\x1a\x15.api.v1.AwaitResponse\"\'\x92\x41\x12*\x10\x45xecution Status\x82\xd3\xe4\x93\x02\x0c\x12\n/v2/status\x12\\\n\x06Output\x12\x15.api.v1.OutputRequest\x1a\x16.api.v1.OutputResponse\"#\x92\x41\x0e*\x0c\x42lock Output\x82\xd3\xe4\x93\x02\x0c\x12\n/v2/output\x12\x64\n\x08\x44ownload\x12\x17.api.v1.DownloadRequest\x1a\x18.api.v1.DownloadResponse\"#\x92\x41\x0f*\rDownload File\x82\xd3\xe4\x93\x02\x0b\x12\t/v2/files0\x01\x12i\n\x06\x43\x61ncel\x12\x15.api.v1.CancelRequest\x1a\x16.api.v1.CancelResponse\"0\x92\x41\x1b*\x19\x43\x61ncel an API\'s Execution\x82\xd3\xe4\x93\x02\x0c\"\n/v2/cancel\x12v\n\x08Validate\x12\x17.api.v1.ValidateRequest\x1a\x16.google.protobuf.Empty\"9\x92\x41\x1f*\x1dValidate an API specification\x82\xd3\xe4\x93\x02\x11\"\x0c/v2/validate:\x01*B\x80\x02Z.github.com/superblocksteam/types/gen/go/api/v1\x92\x41\xcc\x01\x12\x8b\x01\n Superblocks API Executor Service\x12IThis is the contract that the Superblocks Orchestrator component exposes.\"\x17\x1a\x15\x66rank@superblocks.com2\x03\x31.0\x1a\x15\x61gent.superblocks.com*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'api.v1.service_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/api/v1/service_pb2_grpc.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/api/v1/service_pb2_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from api.v1 import service_pb2 as api_dot_v1_dot_service__pb2
-from common.v1 import health_pb2 as common_dot_v1_dot_health__pb2
+from superblocks_types.api.v1 import service_pb2 as api_dot_v1_dot_service__pb2
+from superblocks_types.common.v1 import health_pb2 as common_dot_v1_dot_health__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
 class MetadataServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/auth/v1/auth_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/auth/v1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/buf/validate/expression_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/buf/validate/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/buf/validate/priv/private_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/buf/validate/priv/private_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/buf/validate/validate_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/buf/validate/validate_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from buf.validate import expression_pb2 as buf_dot_validate_dot_expression__pb2
-from buf.validate.priv import private_pb2 as buf_dot_validate_dot_priv_dot_private__pb2
+from superblocks_types.buf.validate import expression_pb2 as buf_dot_validate_dot_expression__pb2
+from superblocks_types.buf.validate.priv import private_pb2 as buf_dot_validate_dot_priv_dot_private__pb2
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x62uf/validate/validate.proto\x12\x0c\x62uf.validate\x1a\x1d\x62uf/validate/expression.proto\x1a\x1f\x62uf/validate/priv/private.proto\x1a google/protobuf/descriptor.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"n\n\x12MessageConstraints\x12\x1f\n\x08\x64isabled\x18\x01 \x01(\x08H\x00R\x08\x64isabled\x88\x01\x01\x12*\n\x03\x63\x65l\x18\x03 \x03(\x0b\x32\x18.buf.validate.ConstraintR\x03\x63\x65lB\x0b\n\t_disabled\"@\n\x10OneofConstraints\x12\x1f\n\x08required\x18\x01 \x01(\x08H\x00R\x08required\x88\x01\x01\x42\x0b\n\t_required\"\xf5\t\n\x10\x46ieldConstraints\x12*\n\x03\x63\x65l\x18\x17 \x03(\x0b\x32\x18.buf.validate.ConstraintR\x03\x63\x65l\x12\x18\n\x07skipped\x18\x18 \x01(\x08R\x07skipped\x12\x1a\n\x08required\x18\x19 \x01(\x08R\x08required\x12!\n\x0cignore_empty\x18\x1a \x01(\x08R\x0bignoreEmpty\x12\x30\n\x05\x66loat\x18\x01 \x01(\x0b\x32\x18.buf.validate.FloatRulesH\x00R\x05\x66loat\x12\x33\n\x06\x64ouble\x18\x02 \x01(\x0b\x32\x19.buf.validate.DoubleRulesH\x00R\x06\x64ouble\x12\x30\n\x05int32\x18\x03 \x01(\x0b\x32\x18.buf.validate.Int32RulesH\x00R\x05int32\x12\x30\n\x05int64\x18\x04 \x01(\x0b\x32\x18.buf.validate.Int64RulesH\x00R\x05int64\x12\x33\n\x06uint32\x18\x05 \x01(\x0b\x32\x19.buf.validate.UInt32RulesH\x00R\x06uint32\x12\x33\n\x06uint64\x18\x06 \x01(\x0b\x32\x19.buf.validate.UInt64RulesH\x00R\x06uint64\x12\x33\n\x06sint32\x18\x07 \x01(\x0b\x32\x19.buf.validate.SInt32RulesH\x00R\x06sint32\x12\x33\n\x06sint64\x18\x08 \x01(\x0b\x32\x19.buf.validate.SInt64RulesH\x00R\x06sint64\x12\x36\n\x07\x66ixed32\x18\t \x01(\x0b\x32\x1a.buf.validate.Fixed32RulesH\x00R\x07\x66ixed32\x12\x36\n\x07\x66ixed64\x18\n \x01(\x0b\x32\x1a.buf.validate.Fixed64RulesH\x00R\x07\x66ixed64\x12\x39\n\x08sfixed32\x18\x0b \x01(\x0b\x32\x1b.buf.validate.SFixed32RulesH\x00R\x08sfixed32\x12\x39\n\x08sfixed64\x18\x0c \x01(\x0b\x32\x1b.buf.validate.SFixed64RulesH\x00R\x08sfixed64\x12-\n\x04\x62ool\x18\r \x01(\x0b\x32\x17.buf.validate.BoolRulesH\x00R\x04\x62ool\x12\x33\n\x06string\x18\x0e \x01(\x0b\x32\x19.buf.validate.StringRulesH\x00R\x06string\x12\x30\n\x05\x62ytes\x18\x0f \x01(\x0b\x32\x18.buf.validate.BytesRulesH\x00R\x05\x62ytes\x12-\n\x04\x65num\x18\x10 \x01(\x0b\x32\x17.buf.validate.EnumRulesH\x00R\x04\x65num\x12\x39\n\x08repeated\x18\x12 \x01(\x0b\x32\x1b.buf.validate.RepeatedRulesH\x00R\x08repeated\x12*\n\x03map\x18\x13 \x01(\x0b\x32\x16.buf.validate.MapRulesH\x00R\x03map\x12*\n\x03\x61ny\x18\x14 \x01(\x0b\x32\x16.buf.validate.AnyRulesH\x00R\x03\x61ny\x12\x39\n\x08\x64uration\x18\x15 \x01(\x0b\x32\x1b.buf.validate.DurationRulesH\x00R\x08\x64uration\x12<\n\ttimestamp\x18\x16 \x01(\x0b\x32\x1c.buf.validate.TimestampRulesH\x00R\ttimestampB\x06\n\x04type\"\xa2\x17\n\nFloatRules\x12u\n\x05\x63onst\x18\x01 \x01(\x02\x42Z\xc2HW\nU\n\x0b\x66loat.const\x1a\x46this != rules.const ? \'value must equal %s\'.format([rules.const]) : \'\'H\x02R\x05\x63onst\x88\x01\x01\x12\xa3\x01\n\x02lt\x18\x02 \x01(\x02\x42\x90\x01\xc2H\x8c\x01\n\x89\x01\n\x08\x66loat.lt\x1a}!has(rules.gte) && !has(rules.gt) && (this.isNan() || this >= rules.lt)? \'value must be less than %s\'.format([rules.lt]) : \'\'H\x00R\x02lt\x12\xb4\x01\n\x03lte\x18\x03 \x01(\x02\x42\x9f\x01\xc2H\x9b\x01\n\x98\x01\n\tfloat.lte\x1a\x8a\x01!has(rules.gte) && !has(rules.gt) && (this.isNan() || this > rules.lte)? \'value must be less than or equal to %s\'.format([rules.lte]) : \'\'H\x00R\x03lte\x12\xf3\x07\n\x02gt\x18\x04 \x01(\x02\x42\xe0\x07\xc2H\xdc\x07\n\x8d\x01\n\x08\x66loat.gt\x1a\x80\x01!has(rules.lt) && !has(rules.lte) && (this.isNan() || this <= rules.gt)? \'value must be greater than %s\'.format([rules.gt]) : \'\'\n\xc3\x01\n\x0b\x66loat.gt_lt\x1a\xb3\x01has(rules.lt) && rules.lt >= rules.gt && (this.isNan() || this >= rules.lt || this <= rules.gt)? \'value must be greater than %s and less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xcd\x01\n\x15\x66loat.gt_lt_exclusive\x1a\xb3\x01has(rules.lt) && rules.lt < rules.gt && (this.isNan() || (rules.lt <= this && this <= rules.gt))? \'value must be greater than %s or less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xd3\x01\n\x0c\x66loat.gt_lte\x1a\xc2\x01has(rules.lte) && rules.lte >= rules.gt && (this.isNan() || this > rules.lte || this <= rules.gt)? \'value must be greater than %s and less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'\n\xdd\x01\n\x16\x66loat.gt_lte_exclusive\x1a\xc2\x01has(rules.lte) && rules.lte < rules.gt && (this.isNan() || (rules.lte < this && this <= rules.gt))? \'value must be greater than %s or less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'H\x01R\x02gt\x12\xbf\x08\n\x03gte\x18\x05 \x01(\x02\x42\xaa\x08\xc2H\xa6\x08\n\x9b\x01\n\tfloat.gte\x1a\x8d\x01!has(rules.lt) && !has(rules.lte) && (this.isNan() || this < rules.gte)? \'value must be greater than or equal to %s\'.format([rules.gte]) : \'\'\n\xd2\x01\n\x0c\x66loat.gte_lt\x1a\xc1\x01has(rules.lt) && rules.lt >= rules.gte && (this.isNan() || this >= rules.lt || this < rules.gte)? \'value must be greater than or equal to %s and less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xdc\x01\n\x16\x66loat.gte_lt_exclusive\x1a\xc1\x01has(rules.lt) && rules.lt < rules.gte && (this.isNan() || (rules.lt <= this && this < rules.gte))? \'value must be greater than or equal to %s or less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xe2\x01\n\rfloat.gte_lte\x1a\xd0\x01has(rules.lte) && rules.lte >= rules.gte && (this.isNan() || this > rules.lte || this < rules.gte)? \'value must be greater than or equal to %s and less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'\n\xec\x01\n\x17\x66loat.gte_lte_exclusive\x1a\xd0\x01has(rules.lte) && rules.lte < rules.gte && (this.isNan() || (rules.lte < this && this < rules.gte))? \'value must be greater than or equal to %s or less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'H\x01R\x03gte\x12y\n\x02in\x18\x06 \x03(\x02\x42i\xc2Hf\nd\n\x08\x66loat.in\x1aX!(this in dyn(rules)[\'in\']) ? \'value must be in list %s\'.format([dyn(rules)[\'in\']]) : \'\'R\x02in\x12}\n\x06not_in\x18\x07 \x03(\x02\x42\x66\xc2Hc\na\n\x0c\x66loat.not_in\x1aQthis in rules.not_in ? \'value must not be in list %s\'.format([rules.not_in]) : \'\'R\x05notIn\x12g\n\x06\x66inite\x18\x08 \x01(\x08\x42O\xc2HL\nJ\n\x0c\x66loat.finite\x1a:this.isNan() || this.isInf() ? \'value must be finite\' : \'\'R\x06\x66initeB\x0b\n\tless_thanB\x0e\n\x0cgreater_thanB\x08\n\x06_const\"\xb3\x17\n\x0b\x44oubleRules\x12v\n\x05\x63onst\x18\x01 \x01(\x01\x42[\xc2HX\nV\n\x0c\x64ouble.const\x1a\x46this != rules.const ? \'value must equal %s\'.format([rules.const]) : \'\'H\x02R\x05\x63onst\x88\x01\x01\x12\xa4\x01\n\x02lt\x18\x02 \x01(\x01\x42\x91\x01\xc2H\x8d\x01\n\x8a\x01\n\tdouble.lt\x1a}!has(rules.gte) && !has(rules.gt) && (this.isNan() || this >= rules.lt)? \'value must be less than %s\'.format([rules.lt]) : \'\'H\x00R\x02lt\x12\xb5\x01\n\x03lte\x18\x03 \x01(\x01\x42\xa0\x01\xc2H\x9c\x01\n\x99\x01\n\ndouble.lte\x1a\x8a\x01!has(rules.gte) && !has(rules.gt) && (this.isNan() || this > rules.lte)? \'value must be less than or equal to %s\'.format([rules.lte]) : \'\'H\x00R\x03lte\x12\xf8\x07\n\x02gt\x18\x04 \x01(\x01\x42\xe5\x07\xc2H\xe1\x07\n\x8e\x01\n\tdouble.gt\x1a\x80\x01!has(rules.lt) && !has(rules.lte) && (this.isNan() || this <= rules.gt)? \'value must be greater than %s\'.format([rules.gt]) : \'\'\n\xc4\x01\n\x0c\x64ouble.gt_lt\x1a\xb3\x01has(rules.lt) && rules.lt >= rules.gt && (this.isNan() || this >= rules.lt || this <= rules.gt)? \'value must be greater than %s and less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xce\x01\n\x16\x64ouble.gt_lt_exclusive\x1a\xb3\x01has(rules.lt) && rules.lt < rules.gt && (this.isNan() || (rules.lt <= this && this <= rules.gt))? \'value must be greater than %s or less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xd4\x01\n\rdouble.gt_lte\x1a\xc2\x01has(rules.lte) && rules.lte >= rules.gt && (this.isNan() || this > rules.lte || this <= rules.gt)? \'value must be greater than %s and less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'\n\xde\x01\n\x17\x64ouble.gt_lte_exclusive\x1a\xc2\x01has(rules.lte) && rules.lte < rules.gt && (this.isNan() || (rules.lte < this && this <= rules.gt))? \'value must be greater than %s or less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'H\x01R\x02gt\x12\xc4\x08\n\x03gte\x18\x05 \x01(\x01\x42\xaf\x08\xc2H\xab\x08\n\x9c\x01\n\ndouble.gte\x1a\x8d\x01!has(rules.lt) && !has(rules.lte) && (this.isNan() || this < rules.gte)? \'value must be greater than or equal to %s\'.format([rules.gte]) : \'\'\n\xd3\x01\n\rdouble.gte_lt\x1a\xc1\x01has(rules.lt) && rules.lt >= rules.gte && (this.isNan() || this >= rules.lt || this < rules.gte)? \'value must be greater than or equal to %s and less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xdd\x01\n\x17\x64ouble.gte_lt_exclusive\x1a\xc1\x01has(rules.lt) && rules.lt < rules.gte && (this.isNan() || (rules.lt <= this && this < rules.gte))? \'value must be greater than or equal to %s or less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xe3\x01\n\x0e\x64ouble.gte_lte\x1a\xd0\x01has(rules.lte) && rules.lte >= rules.gte && (this.isNan() || this > rules.lte || this < rules.gte)? \'value must be greater than or equal to %s and less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'\n\xed\x01\n\x18\x64ouble.gte_lte_exclusive\x1a\xd0\x01has(rules.lte) && rules.lte < rules.gte && (this.isNan() || (rules.lte < this && this < rules.gte))? \'value must be greater than or equal to %s or less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'H\x01R\x03gte\x12z\n\x02in\x18\x06 \x03(\x01\x42j\xc2Hg\ne\n\tdouble.in\x1aX!(this in dyn(rules)[\'in\']) ? \'value must be in list %s\'.format([dyn(rules)[\'in\']]) : \'\'R\x02in\x12~\n\x06not_in\x18\x07 \x03(\x01\x42g\xc2Hd\nb\n\rdouble.not_in\x1aQthis in rules.not_in ? \'value must not be in list %s\'.format([rules.not_in]) : \'\'R\x05notIn\x12h\n\x06\x66inite\x18\x08 \x01(\x08\x42P\xc2HM\nK\n\rdouble.finite\x1a:this.isNan() || this.isInf() ? \'value must be finite\' : \'\'R\x06\x66initeB\x0b\n\tless_thanB\x0e\n\x0cgreater_thanB\x08\n\x06_const\"\xe2\x14\n\nInt32Rules\x12u\n\x05\x63onst\x18\x01 \x01(\x05\x42Z\xc2HW\nU\n\x0bint32.const\x1a\x46this != rules.const ? \'value must equal %s\'.format([rules.const]) : \'\'H\x02R\x05\x63onst\x88\x01\x01\x12\x8e\x01\n\x02lt\x18\x02 \x01(\x05\x42|\xc2Hy\nw\n\x08int32.lt\x1ak!has(rules.gte) && !has(rules.gt) && this >= rules.lt? \'value must be less than %s\'.format([rules.lt]) : \'\'H\x00R\x02lt\x12\xa1\x01\n\x03lte\x18\x03 \x01(\x05\x42\x8c\x01\xc2H\x88\x01\n\x85\x01\n\tint32.lte\x1ax!has(rules.gte) && !has(rules.gt) && this > rules.lte? \'value must be less than or equal to %s\'.format([rules.lte]) : \'\'H\x00R\x03lte\x12\x9b\x07\n\x02gt\x18\x04 \x01(\x05\x42\x88\x07\xc2H\x84\x07\nz\n\x08int32.gt\x1an!has(rules.lt) && !has(rules.lte) && this <= rules.gt? \'value must be greater than %s\'.format([rules.gt]) : \'\'\n\xb3\x01\n\x0bint32.gt_lt\x1a\xa3\x01has(rules.lt) && rules.lt >= rules.gt && (this >= rules.lt || this <= rules.gt)? \'value must be greater than %s and less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xbb\x01\n\x15int32.gt_lt_exclusive\x1a\xa1\x01has(rules.lt) && rules.lt < rules.gt && (rules.lt <= this && this <= rules.gt)? \'value must be greater than %s or less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xc3\x01\n\x0cint32.gt_lte\x1a\xb2\x01has(rules.lte) && rules.lte >= rules.gt && (this > rules.lte || this <= rules.gt)? \'value must be greater than %s and less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'\n\xcb\x01\n\x16int32.gt_lte_exclusive\x1a\xb0\x01has(rules.lte) && rules.lte < rules.gt && (rules.lte < this && this <= rules.gt)? \'value must be greater than %s or less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'H\x01R\x02gt\x12\xe8\x07\n\x03gte\x18\x05 \x01(\x05\x42\xd3\x07\xc2H\xcf\x07\n\x88\x01\n\tint32.gte\x1a{!has(rules.lt) && !has(rules.lte) && this < rules.gte? \'value must be greater than or equal to %s\'.format([rules.gte]) : \'\'\n\xc2\x01\n\x0cint32.gte_lt\x1a\xb1\x01has(rules.lt) && rules.lt >= rules.gte && (this >= rules.lt || this < rules.gte)? \'value must be greater than or equal to %s and less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xca\x01\n\x16int32.gte_lt_exclusive\x1a\xaf\x01has(rules.lt) && rules.lt < rules.gte && (rules.lt <= this && this < rules.gte)? \'value must be greater than or equal to %s or less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xd2\x01\n\rint32.gte_lte\x1a\xc0\x01has(rules.lte) && rules.lte >= rules.gte && (this > rules.lte || this < rules.gte)? \'value must be greater than or equal to %s and less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'\n\xda\x01\n\x17int32.gte_lte_exclusive\x1a\xbe\x01has(rules.lte) && rules.lte < rules.gte && (rules.lte < this && this < rules.gte)? \'value must be greater than or equal to %s or less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'H\x01R\x03gte\x12y\n\x02in\x18\x06 \x03(\x05\x42i\xc2Hf\nd\n\x08int32.in\x1aX!(this in dyn(rules)[\'in\']) ? \'value must be in list %s\'.format([dyn(rules)[\'in\']]) : \'\'R\x02in\x12}\n\x06not_in\x18\x07 \x03(\x05\x42\x66\xc2Hc\na\n\x0cint32.not_in\x1aQthis in rules.not_in ? \'value must not be in list %s\'.format([rules.not_in]) : \'\'R\x05notInB\x0b\n\tless_thanB\x0e\n\x0cgreater_thanB\x08\n\x06_const\"\xe2\x14\n\nInt64Rules\x12u\n\x05\x63onst\x18\x01 \x01(\x03\x42Z\xc2HW\nU\n\x0bint64.const\x1a\x46this != rules.const ? \'value must equal %s\'.format([rules.const]) : \'\'H\x02R\x05\x63onst\x88\x01\x01\x12\x8e\x01\n\x02lt\x18\x02 \x01(\x03\x42|\xc2Hy\nw\n\x08int64.lt\x1ak!has(rules.gte) && !has(rules.gt) && this >= rules.lt? \'value must be less than %s\'.format([rules.lt]) : \'\'H\x00R\x02lt\x12\xa1\x01\n\x03lte\x18\x03 \x01(\x03\x42\x8c\x01\xc2H\x88\x01\n\x85\x01\n\tint64.lte\x1ax!has(rules.gte) && !has(rules.gt) && this > rules.lte? \'value must be less than or equal to %s\'.format([rules.lte]) : \'\'H\x00R\x03lte\x12\x9b\x07\n\x02gt\x18\x04 \x01(\x03\x42\x88\x07\xc2H\x84\x07\nz\n\x08int64.gt\x1an!has(rules.lt) && !has(rules.lte) && this <= rules.gt? \'value must be greater than %s\'.format([rules.gt]) : \'\'\n\xb3\x01\n\x0bint64.gt_lt\x1a\xa3\x01has(rules.lt) && rules.lt >= rules.gt && (this >= rules.lt || this <= rules.gt)? \'value must be greater than %s and less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xbb\x01\n\x15int64.gt_lt_exclusive\x1a\xa1\x01has(rules.lt) && rules.lt < rules.gt && (rules.lt <= this && this <= rules.gt)? \'value must be greater than %s or less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xc3\x01\n\x0cint64.gt_lte\x1a\xb2\x01has(rules.lte) && rules.lte >= rules.gt && (this > rules.lte || this <= rules.gt)? \'value must be greater than %s and less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'\n\xcb\x01\n\x16int64.gt_lte_exclusive\x1a\xb0\x01has(rules.lte) && rules.lte < rules.gt && (rules.lte < this && this <= rules.gt)? \'value must be greater than %s or less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'H\x01R\x02gt\x12\xe8\x07\n\x03gte\x18\x05 \x01(\x03\x42\xd3\x07\xc2H\xcf\x07\n\x88\x01\n\tint64.gte\x1a{!has(rules.lt) && !has(rules.lte) && this < rules.gte? \'value must be greater than or equal to %s\'.format([rules.gte]) : \'\'\n\xc2\x01\n\x0cint64.gte_lt\x1a\xb1\x01has(rules.lt) && rules.lt >= rules.gte && (this >= rules.lt || this < rules.gte)? \'value must be greater than or equal to %s and less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xca\x01\n\x16int64.gte_lt_exclusive\x1a\xaf\x01has(rules.lt) && rules.lt < rules.gte && (rules.lt <= this && this < rules.gte)? \'value must be greater than or equal to %s or less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xd2\x01\n\rint64.gte_lte\x1a\xc0\x01has(rules.lte) && rules.lte >= rules.gte && (this > rules.lte || this < rules.gte)? \'value must be greater than or equal to %s and less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'\n\xda\x01\n\x17int64.gte_lte_exclusive\x1a\xbe\x01has(rules.lte) && rules.lte < rules.gte && (rules.lte < this && this < rules.gte)? \'value must be greater than or equal to %s or less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'H\x01R\x03gte\x12y\n\x02in\x18\x06 \x03(\x03\x42i\xc2Hf\nd\n\x08int64.in\x1aX!(this in dyn(rules)[\'in\']) ? \'value must be in list %s\'.format([dyn(rules)[\'in\']]) : \'\'R\x02in\x12}\n\x06not_in\x18\x07 \x03(\x03\x42\x66\xc2Hc\na\n\x0cint64.not_in\x1aQthis in rules.not_in ? \'value must not be in list %s\'.format([rules.not_in]) : \'\'R\x05notInB\x0b\n\tless_thanB\x0e\n\x0cgreater_thanB\x08\n\x06_const\"\xf2\x14\n\x0bUInt32Rules\x12v\n\x05\x63onst\x18\x01 \x01(\rB[\xc2HX\nV\n\x0cuint32.const\x1a\x46this != rules.const ? \'value must equal %s\'.format([rules.const]) : \'\'H\x02R\x05\x63onst\x88\x01\x01\x12\x8f\x01\n\x02lt\x18\x02 \x01(\rB}\xc2Hz\nx\n\tuint32.lt\x1ak!has(rules.gte) && !has(rules.gt) && this >= rules.lt? \'value must be less than %s\'.format([rules.lt]) : \'\'H\x00R\x02lt\x12\xa2\x01\n\x03lte\x18\x03 \x01(\rB\x8d\x01\xc2H\x89\x01\n\x86\x01\n\nuint32.lte\x1ax!has(rules.gte) && !has(rules.gt) && this > rules.lte? \'value must be less than or equal to %s\'.format([rules.lte]) : \'\'H\x00R\x03lte\x12\xa0\x07\n\x02gt\x18\x04 \x01(\rB\x8d\x07\xc2H\x89\x07\n{\n\tuint32.gt\x1an!has(rules.lt) && !has(rules.lte) && this <= rules.gt? \'value must be greater than %s\'.format([rules.gt]) : \'\'\n\xb4\x01\n\x0cuint32.gt_lt\x1a\xa3\x01has(rules.lt) && rules.lt >= rules.gt && (this >= rules.lt || this <= rules.gt)? \'value must be greater than %s and less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xbc\x01\n\x16uint32.gt_lt_exclusive\x1a\xa1\x01has(rules.lt) && rules.lt < rules.gt && (rules.lt <= this && this <= rules.gt)? \'value must be greater than %s or less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xc4\x01\n\ruint32.gt_lte\x1a\xb2\x01has(rules.lte) && rules.lte >= rules.gt && (this > rules.lte || this <= rules.gt)? \'value must be greater than %s and less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'\n\xcc\x01\n\x17uint32.gt_lte_exclusive\x1a\xb0\x01has(rules.lte) && rules.lte < rules.gt && (rules.lte < this && this <= rules.gt)? \'value must be greater than %s or less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'H\x01R\x02gt\x12\xed\x07\n\x03gte\x18\x05 \x01(\rB\xd8\x07\xc2H\xd4\x07\n\x89\x01\n\nuint32.gte\x1a{!has(rules.lt) && !has(rules.lte) && this < rules.gte? \'value must be greater than or equal to %s\'.format([rules.gte]) : \'\'\n\xc3\x01\n\ruint32.gte_lt\x1a\xb1\x01has(rules.lt) && rules.lt >= rules.gte && (this >= rules.lt || this < rules.gte)? \'value must be greater than or equal to %s and less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xcb\x01\n\x17uint32.gte_lt_exclusive\x1a\xaf\x01has(rules.lt) && rules.lt < rules.gte && (rules.lt <= this && this < rules.gte)? \'value must be greater than or equal to %s or less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xd3\x01\n\x0euint32.gte_lte\x1a\xc0\x01has(rules.lte) && rules.lte >= rules.gte && (this > rules.lte || this < rules.gte)? \'value must be greater than or equal to %s and less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'\n\xdb\x01\n\x18uint32.gte_lte_exclusive\x1a\xbe\x01has(rules.lte) && rules.lte < rules.gte && (rules.lte < this && this < rules.gte)? \'value must be greater than or equal to %s or less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'H\x01R\x03gte\x12z\n\x02in\x18\x06 \x03(\rBj\xc2Hg\ne\n\tuint32.in\x1aX!(this in dyn(rules)[\'in\']) ? \'value must be in list %s\'.format([dyn(rules)[\'in\']]) : \'\'R\x02in\x12~\n\x06not_in\x18\x07 \x03(\rBg\xc2Hd\nb\n\ruint32.not_in\x1aQthis in rules.not_in ? \'value must not be in list %s\'.format([rules.not_in]) : \'\'R\x05notInB\x0b\n\tless_thanB\x0e\n\x0cgreater_thanB\x08\n\x06_const\"\xf2\x14\n\x0bUInt64Rules\x12v\n\x05\x63onst\x18\x01 \x01(\x04\x42[\xc2HX\nV\n\x0cuint64.const\x1a\x46this != rules.const ? \'value must equal %s\'.format([rules.const]) : \'\'H\x02R\x05\x63onst\x88\x01\x01\x12\x8f\x01\n\x02lt\x18\x02 \x01(\x04\x42}\xc2Hz\nx\n\tuint64.lt\x1ak!has(rules.gte) && !has(rules.gt) && this >= rules.lt? \'value must be less than %s\'.format([rules.lt]) : \'\'H\x00R\x02lt\x12\xa2\x01\n\x03lte\x18\x03 \x01(\x04\x42\x8d\x01\xc2H\x89\x01\n\x86\x01\n\nuint64.lte\x1ax!has(rules.gte) && !has(rules.gt) && this > rules.lte? \'value must be less than or equal to %s\'.format([rules.lte]) : \'\'H\x00R\x03lte\x12\xa0\x07\n\x02gt\x18\x04 \x01(\x04\x42\x8d\x07\xc2H\x89\x07\n{\n\tuint64.gt\x1an!has(rules.lt) && !has(rules.lte) && this <= rules.gt? \'value must be greater than %s\'.format([rules.gt]) : \'\'\n\xb4\x01\n\x0cuint64.gt_lt\x1a\xa3\x01has(rules.lt) && rules.lt >= rules.gt && (this >= rules.lt || this <= rules.gt)? \'value must be greater than %s and less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xbc\x01\n\x16uint64.gt_lt_exclusive\x1a\xa1\x01has(rules.lt) && rules.lt < rules.gt && (rules.lt <= this && this <= rules.gt)? \'value must be greater than %s or less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xc4\x01\n\ruint64.gt_lte\x1a\xb2\x01has(rules.lte) && rules.lte >= rules.gt && (this > rules.lte || this <= rules.gt)? \'value must be greater than %s and less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'\n\xcc\x01\n\x17uint64.gt_lte_exclusive\x1a\xb0\x01has(rules.lte) && rules.lte < rules.gt && (rules.lte < this && this <= rules.gt)? \'value must be greater than %s or less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'H\x01R\x02gt\x12\xed\x07\n\x03gte\x18\x05 \x01(\x04\x42\xd8\x07\xc2H\xd4\x07\n\x89\x01\n\nuint64.gte\x1a{!has(rules.lt) && !has(rules.lte) && this < rules.gte? \'value must be greater than or equal to %s\'.format([rules.gte]) : \'\'\n\xc3\x01\n\ruint64.gte_lt\x1a\xb1\x01has(rules.lt) && rules.lt >= rules.gte && (this >= rules.lt || this < rules.gte)? \'value must be greater than or equal to %s and less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xcb\x01\n\x17uint64.gte_lt_exclusive\x1a\xaf\x01has(rules.lt) && rules.lt < rules.gte && (rules.lt <= this && this < rules.gte)? \'value must be greater than or equal to %s or less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xd3\x01\n\x0euint64.gte_lte\x1a\xc0\x01has(rules.lte) && rules.lte >= rules.gte && (this > rules.lte || this < rules.gte)? \'value must be greater than or equal to %s and less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'\n\xdb\x01\n\x18uint64.gte_lte_exclusive\x1a\xbe\x01has(rules.lte) && rules.lte < rules.gte && (rules.lte < this && this < rules.gte)? \'value must be greater than or equal to %s or less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'H\x01R\x03gte\x12z\n\x02in\x18\x06 \x03(\x04\x42j\xc2Hg\ne\n\tuint64.in\x1aX!(this in dyn(rules)[\'in\']) ? \'value must be in list %s\'.format([dyn(rules)[\'in\']]) : \'\'R\x02in\x12~\n\x06not_in\x18\x07 \x03(\x04\x42g\xc2Hd\nb\n\ruint64.not_in\x1aQthis in rules.not_in ? \'value must not be in list %s\'.format([rules.not_in]) : \'\'R\x05notInB\x0b\n\tless_thanB\x0e\n\x0cgreater_thanB\x08\n\x06_const\"\xf2\x14\n\x0bSInt32Rules\x12v\n\x05\x63onst\x18\x01 \x01(\x11\x42[\xc2HX\nV\n\x0csint32.const\x1a\x46this != rules.const ? \'value must equal %s\'.format([rules.const]) : \'\'H\x02R\x05\x63onst\x88\x01\x01\x12\x8f\x01\n\x02lt\x18\x02 \x01(\x11\x42}\xc2Hz\nx\n\tsint32.lt\x1ak!has(rules.gte) && !has(rules.gt) && this >= rules.lt? \'value must be less than %s\'.format([rules.lt]) : \'\'H\x00R\x02lt\x12\xa2\x01\n\x03lte\x18\x03 \x01(\x11\x42\x8d\x01\xc2H\x89\x01\n\x86\x01\n\nsint32.lte\x1ax!has(rules.gte) && !has(rules.gt) && this > rules.lte? \'value must be less than or equal to %s\'.format([rules.lte]) : \'\'H\x00R\x03lte\x12\xa0\x07\n\x02gt\x18\x04 \x01(\x11\x42\x8d\x07\xc2H\x89\x07\n{\n\tsint32.gt\x1an!has(rules.lt) && !has(rules.lte) && this <= rules.gt? \'value must be greater than %s\'.format([rules.gt]) : \'\'\n\xb4\x01\n\x0csint32.gt_lt\x1a\xa3\x01has(rules.lt) && rules.lt >= rules.gt && (this >= rules.lt || this <= rules.gt)? \'value must be greater than %s and less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xbc\x01\n\x16sint32.gt_lt_exclusive\x1a\xa1\x01has(rules.lt) && rules.lt < rules.gt && (rules.lt <= this && this <= rules.gt)? \'value must be greater than %s or less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xc4\x01\n\rsint32.gt_lte\x1a\xb2\x01has(rules.lte) && rules.lte >= rules.gt && (this > rules.lte || this <= rules.gt)? \'value must be greater than %s and less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'\n\xcc\x01\n\x17sint32.gt_lte_exclusive\x1a\xb0\x01has(rules.lte) && rules.lte < rules.gt && (rules.lte < this && this <= rules.gt)? \'value must be greater than %s or less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'H\x01R\x02gt\x12\xed\x07\n\x03gte\x18\x05 \x01(\x11\x42\xd8\x07\xc2H\xd4\x07\n\x89\x01\n\nsint32.gte\x1a{!has(rules.lt) && !has(rules.lte) && this < rules.gte? \'value must be greater than or equal to %s\'.format([rules.gte]) : \'\'\n\xc3\x01\n\rsint32.gte_lt\x1a\xb1\x01has(rules.lt) && rules.lt >= rules.gte && (this >= rules.lt || this < rules.gte)? \'value must be greater than or equal to %s and less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xcb\x01\n\x17sint32.gte_lt_exclusive\x1a\xaf\x01has(rules.lt) && rules.lt < rules.gte && (rules.lt <= this && this < rules.gte)? \'value must be greater than or equal to %s or less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xd3\x01\n\x0esint32.gte_lte\x1a\xc0\x01has(rules.lte) && rules.lte >= rules.gte && (this > rules.lte || this < rules.gte)? \'value must be greater than or equal to %s and less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'\n\xdb\x01\n\x18sint32.gte_lte_exclusive\x1a\xbe\x01has(rules.lte) && rules.lte < rules.gte && (rules.lte < this && this < rules.gte)? \'value must be greater than or equal to %s or less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'H\x01R\x03gte\x12z\n\x02in\x18\x06 \x03(\x11\x42j\xc2Hg\ne\n\tsint32.in\x1aX!(this in dyn(rules)[\'in\']) ? \'value must be in list %s\'.format([dyn(rules)[\'in\']]) : \'\'R\x02in\x12~\n\x06not_in\x18\x07 \x03(\x11\x42g\xc2Hd\nb\n\rsint32.not_in\x1aQthis in rules.not_in ? \'value must not be in list %s\'.format([rules.not_in]) : \'\'R\x05notInB\x0b\n\tless_thanB\x0e\n\x0cgreater_thanB\x08\n\x06_const\"\xf2\x14\n\x0bSInt64Rules\x12v\n\x05\x63onst\x18\x01 \x01(\x12\x42[\xc2HX\nV\n\x0csint64.const\x1a\x46this != rules.const ? \'value must equal %s\'.format([rules.const]) : \'\'H\x02R\x05\x63onst\x88\x01\x01\x12\x8f\x01\n\x02lt\x18\x02 \x01(\x12\x42}\xc2Hz\nx\n\tsint64.lt\x1ak!has(rules.gte) && !has(rules.gt) && this >= rules.lt? \'value must be less than %s\'.format([rules.lt]) : \'\'H\x00R\x02lt\x12\xa2\x01\n\x03lte\x18\x03 \x01(\x12\x42\x8d\x01\xc2H\x89\x01\n\x86\x01\n\nsint64.lte\x1ax!has(rules.gte) && !has(rules.gt) && this > rules.lte? \'value must be less than or equal to %s\'.format([rules.lte]) : \'\'H\x00R\x03lte\x12\xa0\x07\n\x02gt\x18\x04 \x01(\x12\x42\x8d\x07\xc2H\x89\x07\n{\n\tsint64.gt\x1an!has(rules.lt) && !has(rules.lte) && this <= rules.gt? \'value must be greater than %s\'.format([rules.gt]) : \'\'\n\xb4\x01\n\x0csint64.gt_lt\x1a\xa3\x01has(rules.lt) && rules.lt >= rules.gt && (this >= rules.lt || this <= rules.gt)? \'value must be greater than %s and less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xbc\x01\n\x16sint64.gt_lt_exclusive\x1a\xa1\x01has(rules.lt) && rules.lt < rules.gt && (rules.lt <= this && this <= rules.gt)? \'value must be greater than %s or less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xc4\x01\n\rsint64.gt_lte\x1a\xb2\x01has(rules.lte) && rules.lte >= rules.gt && (this > rules.lte || this <= rules.gt)? \'value must be greater than %s and less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'\n\xcc\x01\n\x17sint64.gt_lte_exclusive\x1a\xb0\x01has(rules.lte) && rules.lte < rules.gt && (rules.lte < this && this <= rules.gt)? \'value must be greater than %s or less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'H\x01R\x02gt\x12\xed\x07\n\x03gte\x18\x05 \x01(\x12\x42\xd8\x07\xc2H\xd4\x07\n\x89\x01\n\nsint64.gte\x1a{!has(rules.lt) && !has(rules.lte) && this < rules.gte? \'value must be greater than or equal to %s\'.format([rules.gte]) : \'\'\n\xc3\x01\n\rsint64.gte_lt\x1a\xb1\x01has(rules.lt) && rules.lt >= rules.gte && (this >= rules.lt || this < rules.gte)? \'value must be greater than or equal to %s and less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xcb\x01\n\x17sint64.gte_lt_exclusive\x1a\xaf\x01has(rules.lt) && rules.lt < rules.gte && (rules.lt <= this && this < rules.gte)? \'value must be greater than or equal to %s or less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xd3\x01\n\x0esint64.gte_lte\x1a\xc0\x01has(rules.lte) && rules.lte >= rules.gte && (this > rules.lte || this < rules.gte)? \'value must be greater than or equal to %s and less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'\n\xdb\x01\n\x18sint64.gte_lte_exclusive\x1a\xbe\x01has(rules.lte) && rules.lte < rules.gte && (rules.lte < this && this < rules.gte)? \'value must be greater than or equal to %s or less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'H\x01R\x03gte\x12z\n\x02in\x18\x06 \x03(\x12\x42j\xc2Hg\ne\n\tsint64.in\x1aX!(this in dyn(rules)[\'in\']) ? \'value must be in list %s\'.format([dyn(rules)[\'in\']]) : \'\'R\x02in\x12~\n\x06not_in\x18\x07 \x03(\x12\x42g\xc2Hd\nb\n\rsint64.not_in\x1aQthis in rules.not_in ? \'value must not be in list %s\'.format([rules.not_in]) : \'\'R\x05notInB\x0b\n\tless_thanB\x0e\n\x0cgreater_thanB\x08\n\x06_const\"\x82\x15\n\x0c\x46ixed32Rules\x12w\n\x05\x63onst\x18\x01 \x01(\x07\x42\\\xc2HY\nW\n\rfixed32.const\x1a\x46this != rules.const ? \'value must equal %s\'.format([rules.const]) : \'\'H\x02R\x05\x63onst\x88\x01\x01\x12\x90\x01\n\x02lt\x18\x02 \x01(\x07\x42~\xc2H{\ny\n\nfixed32.lt\x1ak!has(rules.gte) && !has(rules.gt) && this >= rules.lt? \'value must be less than %s\'.format([rules.lt]) : \'\'H\x00R\x02lt\x12\xa3\x01\n\x03lte\x18\x03 \x01(\x07\x42\x8e\x01\xc2H\x8a\x01\n\x87\x01\n\x0b\x66ixed32.lte\x1ax!has(rules.gte) && !has(rules.gt) && this > rules.lte? \'value must be less than or equal to %s\'.format([rules.lte]) : \'\'H\x00R\x03lte\x12\xa5\x07\n\x02gt\x18\x04 \x01(\x07\x42\x92\x07\xc2H\x8e\x07\n|\n\nfixed32.gt\x1an!has(rules.lt) && !has(rules.lte) && this <= rules.gt? \'value must be greater than %s\'.format([rules.gt]) : \'\'\n\xb5\x01\n\rfixed32.gt_lt\x1a\xa3\x01has(rules.lt) && rules.lt >= rules.gt && (this >= rules.lt || this <= rules.gt)? \'value must be greater than %s and less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xbd\x01\n\x17\x66ixed32.gt_lt_exclusive\x1a\xa1\x01has(rules.lt) && rules.lt < rules.gt && (rules.lt <= this && this <= rules.gt)? \'value must be greater than %s or less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xc5\x01\n\x0e\x66ixed32.gt_lte\x1a\xb2\x01has(rules.lte) && rules.lte >= rules.gt && (this > rules.lte || this <= rules.gt)? \'value must be greater than %s and less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'\n\xcd\x01\n\x18\x66ixed32.gt_lte_exclusive\x1a\xb0\x01has(rules.lte) && rules.lte < rules.gt && (rules.lte < this && this <= rules.gt)? \'value must be greater than %s or less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'H\x01R\x02gt\x12\xf2\x07\n\x03gte\x18\x05 \x01(\x07\x42\xdd\x07\xc2H\xd9\x07\n\x8a\x01\n\x0b\x66ixed32.gte\x1a{!has(rules.lt) && !has(rules.lte) && this < rules.gte? \'value must be greater than or equal to %s\'.format([rules.gte]) : \'\'\n\xc4\x01\n\x0e\x66ixed32.gte_lt\x1a\xb1\x01has(rules.lt) && rules.lt >= rules.gte && (this >= rules.lt || this < rules.gte)? \'value must be greater than or equal to %s and less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xcc\x01\n\x18\x66ixed32.gte_lt_exclusive\x1a\xaf\x01has(rules.lt) && rules.lt < rules.gte && (rules.lt <= this && this < rules.gte)? \'value must be greater than or equal to %s or less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xd4\x01\n\x0f\x66ixed32.gte_lte\x1a\xc0\x01has(rules.lte) && rules.lte >= rules.gte && (this > rules.lte || this < rules.gte)? \'value must be greater than or equal to %s and less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'\n\xdc\x01\n\x19\x66ixed32.gte_lte_exclusive\x1a\xbe\x01has(rules.lte) && rules.lte < rules.gte && (rules.lte < this && this < rules.gte)? \'value must be greater than or equal to %s or less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'H\x01R\x03gte\x12{\n\x02in\x18\x06 \x03(\x07\x42k\xc2Hh\nf\n\nfixed32.in\x1aX!(this in dyn(rules)[\'in\']) ? \'value must be in list %s\'.format([dyn(rules)[\'in\']]) : \'\'R\x02in\x12\x7f\n\x06not_in\x18\x07 \x03(\x07\x42h\xc2He\nc\n\x0e\x66ixed32.not_in\x1aQthis in rules.not_in ? \'value must not be in list %s\'.format([rules.not_in]) : \'\'R\x05notInB\x0b\n\tless_thanB\x0e\n\x0cgreater_thanB\x08\n\x06_const\"\x82\x15\n\x0c\x46ixed64Rules\x12w\n\x05\x63onst\x18\x01 \x01(\x06\x42\\\xc2HY\nW\n\rfixed64.const\x1a\x46this != rules.const ? \'value must equal %s\'.format([rules.const]) : \'\'H\x02R\x05\x63onst\x88\x01\x01\x12\x90\x01\n\x02lt\x18\x02 \x01(\x06\x42~\xc2H{\ny\n\nfixed64.lt\x1ak!has(rules.gte) && !has(rules.gt) && this >= rules.lt? \'value must be less than %s\'.format([rules.lt]) : \'\'H\x00R\x02lt\x12\xa3\x01\n\x03lte\x18\x03 \x01(\x06\x42\x8e\x01\xc2H\x8a\x01\n\x87\x01\n\x0b\x66ixed64.lte\x1ax!has(rules.gte) && !has(rules.gt) && this > rules.lte? \'value must be less than or equal to %s\'.format([rules.lte]) : \'\'H\x00R\x03lte\x12\xa5\x07\n\x02gt\x18\x04 \x01(\x06\x42\x92\x07\xc2H\x8e\x07\n|\n\nfixed64.gt\x1an!has(rules.lt) && !has(rules.lte) && this <= rules.gt? \'value must be greater than %s\'.format([rules.gt]) : \'\'\n\xb5\x01\n\rfixed64.gt_lt\x1a\xa3\x01has(rules.lt) && rules.lt >= rules.gt && (this >= rules.lt || this <= rules.gt)? \'value must be greater than %s and less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xbd\x01\n\x17\x66ixed64.gt_lt_exclusive\x1a\xa1\x01has(rules.lt) && rules.lt < rules.gt && (rules.lt <= this && this <= rules.gt)? \'value must be greater than %s or less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xc5\x01\n\x0e\x66ixed64.gt_lte\x1a\xb2\x01has(rules.lte) && rules.lte >= rules.gt && (this > rules.lte || this <= rules.gt)? \'value must be greater than %s and less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'\n\xcd\x01\n\x18\x66ixed64.gt_lte_exclusive\x1a\xb0\x01has(rules.lte) && rules.lte < rules.gt && (rules.lte < this && this <= rules.gt)? \'value must be greater than %s or less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'H\x01R\x02gt\x12\xf2\x07\n\x03gte\x18\x05 \x01(\x06\x42\xdd\x07\xc2H\xd9\x07\n\x8a\x01\n\x0b\x66ixed64.gte\x1a{!has(rules.lt) && !has(rules.lte) && this < rules.gte? \'value must be greater than or equal to %s\'.format([rules.gte]) : \'\'\n\xc4\x01\n\x0e\x66ixed64.gte_lt\x1a\xb1\x01has(rules.lt) && rules.lt >= rules.gte && (this >= rules.lt || this < rules.gte)? \'value must be greater than or equal to %s and less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xcc\x01\n\x18\x66ixed64.gte_lt_exclusive\x1a\xaf\x01has(rules.lt) && rules.lt < rules.gte && (rules.lt <= this && this < rules.gte)? \'value must be greater than or equal to %s or less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xd4\x01\n\x0f\x66ixed64.gte_lte\x1a\xc0\x01has(rules.lte) && rules.lte >= rules.gte && (this > rules.lte || this < rules.gte)? \'value must be greater than or equal to %s and less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'\n\xdc\x01\n\x19\x66ixed64.gte_lte_exclusive\x1a\xbe\x01has(rules.lte) && rules.lte < rules.gte && (rules.lte < this && this < rules.gte)? \'value must be greater than or equal to %s or less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'H\x01R\x03gte\x12{\n\x02in\x18\x06 \x03(\x06\x42k\xc2Hh\nf\n\nfixed64.in\x1aX!(this in dyn(rules)[\'in\']) ? \'value must be in list %s\'.format([dyn(rules)[\'in\']]) : \'\'R\x02in\x12\x7f\n\x06not_in\x18\x07 \x03(\x06\x42h\xc2He\nc\n\x0e\x66ixed64.not_in\x1aQthis in rules.not_in ? \'value must not be in list %s\'.format([rules.not_in]) : \'\'R\x05notInB\x0b\n\tless_thanB\x0e\n\x0cgreater_thanB\x08\n\x06_const\"\x93\x15\n\rSFixed32Rules\x12x\n\x05\x63onst\x18\x01 \x01(\x0f\x42]\xc2HZ\nX\n\x0esfixed32.const\x1a\x46this != rules.const ? \'value must equal %s\'.format([rules.const]) : \'\'H\x02R\x05\x63onst\x88\x01\x01\x12\x91\x01\n\x02lt\x18\x02 \x01(\x0f\x42\x7f\xc2H|\nz\n\x0bsfixed32.lt\x1ak!has(rules.gte) && !has(rules.gt) && this >= rules.lt? \'value must be less than %s\'.format([rules.lt]) : \'\'H\x00R\x02lt\x12\xa4\x01\n\x03lte\x18\x03 \x01(\x0f\x42\x8f\x01\xc2H\x8b\x01\n\x88\x01\n\x0csfixed32.lte\x1ax!has(rules.gte) && !has(rules.gt) && this > rules.lte? \'value must be less than or equal to %s\'.format([rules.lte]) : \'\'H\x00R\x03lte\x12\xaa\x07\n\x02gt\x18\x04 \x01(\x0f\x42\x97\x07\xc2H\x93\x07\n}\n\x0bsfixed32.gt\x1an!has(rules.lt) && !has(rules.lte) && this <= rules.gt? \'value must be greater than %s\'.format([rules.gt]) : \'\'\n\xb6\x01\n\x0esfixed32.gt_lt\x1a\xa3\x01has(rules.lt) && rules.lt >= rules.gt && (this >= rules.lt || this <= rules.gt)? \'value must be greater than %s and less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xbe\x01\n\x18sfixed32.gt_lt_exclusive\x1a\xa1\x01has(rules.lt) && rules.lt < rules.gt && (rules.lt <= this && this <= rules.gt)? \'value must be greater than %s or less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xc6\x01\n\x0fsfixed32.gt_lte\x1a\xb2\x01has(rules.lte) && rules.lte >= rules.gt && (this > rules.lte || this <= rules.gt)? \'value must be greater than %s and less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'\n\xce\x01\n\x19sfixed32.gt_lte_exclusive\x1a\xb0\x01has(rules.lte) && rules.lte < rules.gt && (rules.lte < this && this <= rules.gt)? \'value must be greater than %s or less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'H\x01R\x02gt\x12\xf7\x07\n\x03gte\x18\x05 \x01(\x0f\x42\xe2\x07\xc2H\xde\x07\n\x8b\x01\n\x0csfixed32.gte\x1a{!has(rules.lt) && !has(rules.lte) && this < rules.gte? \'value must be greater than or equal to %s\'.format([rules.gte]) : \'\'\n\xc5\x01\n\x0fsfixed32.gte_lt\x1a\xb1\x01has(rules.lt) && rules.lt >= rules.gte && (this >= rules.lt || this < rules.gte)? \'value must be greater than or equal to %s and less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xcd\x01\n\x19sfixed32.gte_lt_exclusive\x1a\xaf\x01has(rules.lt) && rules.lt < rules.gte && (rules.lt <= this && this < rules.gte)? \'value must be greater than or equal to %s or less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xd5\x01\n\x10sfixed32.gte_lte\x1a\xc0\x01has(rules.lte) && rules.lte >= rules.gte && (this > rules.lte || this < rules.gte)? \'value must be greater than or equal to %s and less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'\n\xdd\x01\n\x1asfixed32.gte_lte_exclusive\x1a\xbe\x01has(rules.lte) && rules.lte < rules.gte && (rules.lte < this && this < rules.gte)? \'value must be greater than or equal to %s or less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'H\x01R\x03gte\x12|\n\x02in\x18\x06 \x03(\x0f\x42l\xc2Hi\ng\n\x0bsfixed32.in\x1aX!(this in dyn(rules)[\'in\']) ? \'value must be in list %s\'.format([dyn(rules)[\'in\']]) : \'\'R\x02in\x12\x80\x01\n\x06not_in\x18\x07 \x03(\x0f\x42i\xc2Hf\nd\n\x0fsfixed32.not_in\x1aQthis in rules.not_in ? \'value must not be in list %s\'.format([rules.not_in]) : \'\'R\x05notInB\x0b\n\tless_thanB\x0e\n\x0cgreater_thanB\x08\n\x06_const\"\x93\x15\n\rSFixed64Rules\x12x\n\x05\x63onst\x18\x01 \x01(\x10\x42]\xc2HZ\nX\n\x0esfixed64.const\x1a\x46this != rules.const ? \'value must equal %s\'.format([rules.const]) : \'\'H\x02R\x05\x63onst\x88\x01\x01\x12\x91\x01\n\x02lt\x18\x02 \x01(\x10\x42\x7f\xc2H|\nz\n\x0bsfixed64.lt\x1ak!has(rules.gte) && !has(rules.gt) && this >= rules.lt? \'value must be less than %s\'.format([rules.lt]) : \'\'H\x00R\x02lt\x12\xa4\x01\n\x03lte\x18\x03 \x01(\x10\x42\x8f\x01\xc2H\x8b\x01\n\x88\x01\n\x0csfixed64.lte\x1ax!has(rules.gte) && !has(rules.gt) && this > rules.lte? \'value must be less than or equal to %s\'.format([rules.lte]) : \'\'H\x00R\x03lte\x12\xaa\x07\n\x02gt\x18\x04 \x01(\x10\x42\x97\x07\xc2H\x93\x07\n}\n\x0bsfixed64.gt\x1an!has(rules.lt) && !has(rules.lte) && this <= rules.gt? \'value must be greater than %s\'.format([rules.gt]) : \'\'\n\xb6\x01\n\x0esfixed64.gt_lt\x1a\xa3\x01has(rules.lt) && rules.lt >= rules.gt && (this >= rules.lt || this <= rules.gt)? \'value must be greater than %s and less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xbe\x01\n\x18sfixed64.gt_lt_exclusive\x1a\xa1\x01has(rules.lt) && rules.lt < rules.gt && (rules.lt <= this && this <= rules.gt)? \'value must be greater than %s or less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xc6\x01\n\x0fsfixed64.gt_lte\x1a\xb2\x01has(rules.lte) && rules.lte >= rules.gt && (this > rules.lte || this <= rules.gt)? \'value must be greater than %s and less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'\n\xce\x01\n\x19sfixed64.gt_lte_exclusive\x1a\xb0\x01has(rules.lte) && rules.lte < rules.gt && (rules.lte < this && this <= rules.gt)? \'value must be greater than %s or less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'H\x01R\x02gt\x12\xf7\x07\n\x03gte\x18\x05 \x01(\x10\x42\xe2\x07\xc2H\xde\x07\n\x8b\x01\n\x0csfixed64.gte\x1a{!has(rules.lt) && !has(rules.lte) && this < rules.gte? \'value must be greater than or equal to %s\'.format([rules.gte]) : \'\'\n\xc5\x01\n\x0fsfixed64.gte_lt\x1a\xb1\x01has(rules.lt) && rules.lt >= rules.gte && (this >= rules.lt || this < rules.gte)? \'value must be greater than or equal to %s and less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xcd\x01\n\x19sfixed64.gte_lt_exclusive\x1a\xaf\x01has(rules.lt) && rules.lt < rules.gte && (rules.lt <= this && this < rules.gte)? \'value must be greater than or equal to %s or less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xd5\x01\n\x10sfixed64.gte_lte\x1a\xc0\x01has(rules.lte) && rules.lte >= rules.gte && (this > rules.lte || this < rules.gte)? \'value must be greater than or equal to %s and less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'\n\xdd\x01\n\x1asfixed64.gte_lte_exclusive\x1a\xbe\x01has(rules.lte) && rules.lte < rules.gte && (rules.lte < this && this < rules.gte)? \'value must be greater than or equal to %s or less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'H\x01R\x03gte\x12|\n\x02in\x18\x06 \x03(\x10\x42l\xc2Hi\ng\n\x0bsfixed64.in\x1aX!(this in dyn(rules)[\'in\']) ? \'value must be in list %s\'.format([dyn(rules)[\'in\']]) : \'\'R\x02in\x12\x80\x01\n\x06not_in\x18\x07 \x03(\x10\x42i\xc2Hf\nd\n\x0fsfixed64.not_in\x1aQthis in rules.not_in ? \'value must not be in list %s\'.format([rules.not_in]) : \'\'R\x05notInB\x0b\n\tless_thanB\x0e\n\x0cgreater_thanB\x08\n\x06_const\"\x8b\x01\n\tBoolRules\x12t\n\x05\x63onst\x18\x01 \x01(\x08\x42Y\xc2HV\nT\n\nbool.const\x1a\x46this != rules.const ? \'value must equal %s\'.format([rules.const]) : \'\'H\x00R\x05\x63onst\x88\x01\x01\x42\x08\n\x06_const\"\xe8$\n\x0bStringRules\x12x\n\x05\x63onst\x18\x01 \x01(\tB]\xc2HZ\nX\n\x0cstring.const\x1aHthis != rules.const ? \'value must equal `%s`\'.format([rules.const]) : \'\'H\x01R\x05\x63onst\x88\x01\x01\x12\x88\x01\n\x03len\x18\x13 \x01(\x04\x42q\xc2Hn\nl\n\nstring.len\x1a^uint(this.size()) != rules.len ? \'value length must be %s characters\'.format([rules.len]) : \'\'H\x02R\x03len\x88\x01\x01\x12\xa6\x01\n\x07min_len\x18\x02 \x01(\x04\x42\x87\x01\xc2H\x83\x01\n\x80\x01\n\x0estring.min_len\x1anuint(this.size()) < rules.min_len ? \'value length must be at least %s characters\'.format([rules.min_len]) : \'\'H\x03R\x06minLen\x88\x01\x01\x12\xa4\x01\n\x07max_len\x18\x03 \x01(\x04\x42\x85\x01\xc2H\x81\x01\n\x7f\n\x0estring.max_len\x1amuint(this.size()) > rules.max_len ? \'value length must be at most %s characters\'.format([rules.max_len]) : \'\'H\x04R\x06maxLen\x88\x01\x01\x12\xaa\x01\n\tlen_bytes\x18\x14 \x01(\x04\x42\x87\x01\xc2H\x83\x01\n\x80\x01\n\x10string.len_bytes\x1aluint(bytes(this).size()) != rules.len_bytes ? \'value length must be %s bytes\'.format([rules.len_bytes]) : \'\'H\x05R\x08lenBytes\x88\x01\x01\x12\xb2\x01\n\tmin_bytes\x18\x04 \x01(\x04\x42\x8f\x01\xc2H\x8b\x01\n\x88\x01\n\x10string.min_bytes\x1atuint(bytes(this).size()) < rules.min_bytes ? \'value length must be at least %s bytes\'.format([rules.min_bytes]) : \'\'H\x06R\x08minBytes\x88\x01\x01\x12\xb1\x01\n\tmax_bytes\x18\x05 \x01(\x04\x42\x8e\x01\xc2H\x8a\x01\n\x87\x01\n\x10string.max_bytes\x1asuint(bytes(this).size()) > rules.max_bytes ? \'value length must be at most %s bytes\'.format([rules.max_bytes]) : \'\'H\x07R\x08maxBytes\x88\x01\x01\x12\x9b\x01\n\x07pattern\x18\x06 \x01(\tB|\xc2Hy\nw\n\x0estring.pattern\x1a\x65!this.matches(rules.pattern) ? \'value does not match regex pattern `%s`\'.format([rules.pattern]) : \'\'H\x08R\x07pattern\x88\x01\x01\x12\x91\x01\n\x06prefix\x18\x07 \x01(\tBt\xc2Hq\no\n\rstring.prefix\x1a^!this.startsWith(rules.prefix) ? \'value does not have prefix `%s`\'.format([rules.prefix]) : \'\'H\tR\x06prefix\x88\x01\x01\x12\x8f\x01\n\x06suffix\x18\x08 \x01(\tBr\xc2Ho\nm\n\rstring.suffix\x1a\\!this.endsWith(rules.suffix) ? \'value does not have suffix `%s`\'.format([rules.suffix]) : \'\'H\nR\x06suffix\x88\x01\x01\x12\x9f\x01\n\x08\x63ontains\x18\t \x01(\tB~\xc2H{\ny\n\x0fstring.contains\x1a\x66!this.contains(rules.contains) ? \'value does not contain substring `%s`\'.format([rules.contains]) : \'\'H\x0bR\x08\x63ontains\x88\x01\x01\x12\xaa\x01\n\x0cnot_contains\x18\x17 \x01(\tB\x81\x01\xc2H~\n|\n\x13string.not_contains\x1a\x65this.contains(rules.not_contains) ? \'value contains substring `%s`\'.format([rules.not_contains]) : \'\'H\x0cR\x0bnotContains\x88\x01\x01\x12z\n\x02in\x18\n \x03(\tBj\xc2Hg\ne\n\tstring.in\x1aX!(this in dyn(rules)[\'in\']) ? \'value must be in list %s\'.format([dyn(rules)[\'in\']]) : \'\'R\x02in\x12~\n\x06not_in\x18\x0b \x03(\tBg\xc2Hd\nb\n\rstring.not_in\x1aQthis in rules.not_in ? \'value must not be in list %s\'.format([rules.not_in]) : \'\'R\x05notIn\x12`\n\x05\x65mail\x18\x0c \x01(\x08\x42H\xc2HE\nC\n\x0cstring.email\x12#value must be a valid email address\x1a\x0ethis.isEmail()H\x00R\x05\x65mail\x12g\n\x08hostname\x18\r \x01(\x08\x42I\xc2HF\nD\n\x0fstring.hostname\x12\x1evalue must be a valid hostname\x1a\x11this.isHostname()H\x00R\x08hostname\x12Q\n\x02ip\x18\x0e \x01(\x08\x42?\xc2H<\n:\n\tstring.ip\x12 value must be a valid IP address\x1a\x0bthis.isIp()H\x00R\x02ip\x12Z\n\x04ipv4\x18\x0f \x01(\x08\x42\x44\xc2HA\n?\n\x0bstring.ipv4\x12\"value must be a valid IPv4 address\x1a\x0cthis.isIp(4)H\x00R\x04ipv4\x12Z\n\x04ipv6\x18\x10 \x01(\x08\x42\x44\xc2HA\n?\n\x0bstring.ipv6\x12\"value must be a valid IPv6 address\x1a\x0cthis.isIp(6)H\x00R\x04ipv6\x12N\n\x03uri\x18\x11 \x01(\x08\x42:\xc2H7\n5\n\nstring.uri\x12\x19value must be a valid URI\x1a\x0cthis.isUri()H\x00R\x03uri\x12\\\n\x07uri_ref\x18\x12 \x01(\x08\x42\x41\xc2H>\n<\n\x0estring.uri_ref\x12\x19value must be a valid URI\x1a\x0fthis.isUriRef()H\x00R\x06uriRef\x12\x82\x01\n\x07\x61\x64\x64ress\x18\x15 \x01(\x08\x42\x66\xc2Hc\na\n\x0estring.address\x12-value must be a valid hostname, or ip address\x1a this.isHostname() || this.isIp()H\x00R\x07\x61\x64\x64ress\x12\xb0\x01\n\x04uuid\x18\x16 \x01(\x08\x42\x99\x01\xc2H\x95\x01\n\x92\x01\n\x0bstring.uuid\x1a\x82\x01!this.matches(\'^[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$\') ? \'value must be a valid UUID\' : \'\'H\x00R\x04uuid\x12\x81\x01\n\x11ip_with_prefixlen\x18\x1a \x01(\x08\x42S\xc2HP\nN\n\x18string.ip_with_prefixlen\x12\x1fvalue must be a valid IP prefix\x1a\x11this.isIpPrefix()H\x00R\x0fipWithPrefixlen\x12\x9e\x01\n\x13ipv4_with_prefixlen\x18\x1b \x01(\x08\x42l\xc2Hi\ng\n\x1astring.ipv4_with_prefixlen\x12\x35value must be a valid IPv4 address with prefix length\x1a\x12this.isIpPrefix(4)H\x00R\x11ipv4WithPrefixlen\x12\x9e\x01\n\x13ipv6_with_prefixlen\x18\x1c \x01(\x08\x42l\xc2Hi\ng\n\x1astring.ipv6_with_prefixlen\x12\x35value must be a valid IPv6 address with prefix length\x1a\x12this.isIpPrefix(6)H\x00R\x11ipv6WithPrefixlen\x12n\n\tip_prefix\x18\x1d \x01(\x08\x42O\xc2HL\nJ\n\x10string.ip_prefix\x12\x1fvalue must be a valid IP prefix\x1a\x15this.isIpPrefix(true)H\x00R\x08ipPrefix\x12y\n\x0bipv4_prefix\x18\x1e \x01(\x08\x42V\xc2HS\nQ\n\x12string.ipv4_prefix\x12!value must be a valid IPv4 prefix\x1a\x18this.isIpPrefix(4, true)H\x00R\nipv4Prefix\x12y\n\x0bipv6_prefix\x18\x1f \x01(\x08\x42V\xc2HS\nQ\n\x12string.ipv6_prefix\x12!value must be a valid IPv6 prefix\x1a\x18this.isIpPrefix(6, true)H\x00R\nipv6Prefix\x12\xac\x04\n\x10well_known_regex\x18\x18 \x01(\x0e\x32\x18.buf.validate.KnownRegexB\xe5\x03\xc2H\xe1\x03\n\xeb\x01\n#string.well_known_regex.header_name\x1a\xc3\x01rules.well_known_regex == 1 && !this.matches(!has(rules.strict) || rules.strict ?\'^:?[0-9a-zA-Z!#$%&\\\'*+-.^_|~\\x60]+$\' :\'^[^\\u0000\\u000A\\u000D]+$\') ? \'value must be a valid HTTP header name\' : \'\'\n\xf0\x01\n$string.well_known_regex.header_value\x1a\xc7\x01rules.well_known_regex == 2 && !this.matches(!has(rules.strict) || rules.strict ?\'^[^\\u0000-\\u0008\\u000A-\\u001F\\u007F]*$\' :\'^[^\\u0000\\u000A\\u000D]*$\') ? \'value must be a valid HTTP header value\' : \'\'H\x00R\x0ewellKnownRegex\x12\x1b\n\x06strict\x18\x19 \x01(\x08H\rR\x06strict\x88\x01\x01\x42\x0c\n\nwell_knownB\x08\n\x06_constB\x06\n\x04_lenB\n\n\x08_min_lenB\n\n\x08_max_lenB\x0c\n\n_len_bytesB\x0c\n\n_min_bytesB\x0c\n\n_max_bytesB\n\n\x08_patternB\t\n\x07_prefixB\t\n\x07_suffixB\x0b\n\t_containsB\x0f\n\r_not_containsB\t\n\x07_strict\"\xda\x0e\n\nBytesRules\x12r\n\x05\x63onst\x18\x01 \x01(\x0c\x42W\xc2HT\nR\n\x0b\x62ytes.const\x1a\x43this != rules.const ? \'value must be %x\'.format([rules.const]) : \'\'H\x01R\x05\x63onst\x88\x01\x01\x12\x82\x01\n\x03len\x18\r \x01(\x04\x42k\xc2Hh\nf\n\tbytes.len\x1aYuint(this.size()) != rules.len ? \'value length must be %s bytes\'.format([rules.len]) : \'\'H\x02R\x03len\x88\x01\x01\x12\x9d\x01\n\x07min_len\x18\x02 \x01(\x04\x42\x7f\xc2H|\nz\n\rbytes.min_len\x1aiuint(this.size()) < rules.min_len ? \'value length must be at least %s bytes\'.format([rules.min_len]) : \'\'H\x03R\x06minLen\x88\x01\x01\x12\x95\x01\n\x07max_len\x18\x03 \x01(\x04\x42w\xc2Ht\nr\n\rbytes.max_len\x1a\x61uint(this.size()) > rules.max_len ? \'value must be at most %s bytes\'.format([rules.max_len]) : \'\'H\x04R\x06maxLen\x88\x01\x01\x12\x9e\x01\n\x07pattern\x18\x04 \x01(\tB\x7f\xc2H|\nz\n\rbytes.pattern\x1ai!string(this).matches(rules.pattern) ? \'value must match regex pattern `%s`\'.format([rules.pattern]) : \'\'H\x05R\x07pattern\x88\x01\x01\x12\x8e\x01\n\x06prefix\x18\x05 \x01(\x0c\x42q\xc2Hn\nl\n\x0c\x62ytes.prefix\x1a\\!this.startsWith(rules.prefix) ? \'value does not have prefix %x\'.format([rules.prefix]) : \'\'H\x06R\x06prefix\x88\x01\x01\x12\x8c\x01\n\x06suffix\x18\x06 \x01(\x0c\x42o\xc2Hl\nj\n\x0c\x62ytes.suffix\x1aZ!this.endsWith(rules.suffix) ? \'value does not have suffix %x\'.format([rules.suffix]) : \'\'H\x07R\x06suffix\x88\x01\x01\x12\x92\x01\n\x08\x63ontains\x18\x07 \x01(\x0c\x42q\xc2Hn\nl\n\x0e\x62ytes.contains\x1aZ!this.contains(rules.contains) ? \'value does not contain %x\'.format([rules.contains]) : \'\'H\x08R\x08\x63ontains\x88\x01\x01\x12\x9b\x01\n\x02in\x18\x08 \x03(\x0c\x42\x8a\x01\xc2H\x86\x01\n\x83\x01\n\x08\x62ytes.in\x1awdyn(rules)[\'in\'].size() > 0 && !(this in dyn(rules)[\'in\']) ? \'value must be in list %s\'.format([dyn(rules)[\'in\']]) : \'\'R\x02in\x12}\n\x06not_in\x18\t \x03(\x0c\x42\x66\xc2Hc\na\n\x0c\x62ytes.not_in\x1aQthis in rules.not_in ? \'value must not be in list %s\'.format([rules.not_in]) : \'\'R\x05notIn\x12r\n\x02ip\x18\n \x01(\x08\x42`\xc2H]\n[\n\x08\x62ytes.ip\x1aOthis.size() != 4 && this.size() != 16 ? \'value must be a valid IP address\' : \'\'H\x00R\x02ip\x12\x65\n\x04ipv4\x18\x0b \x01(\x08\x42O\xc2HL\nJ\n\nbytes.ipv4\x1a<this.size() != 4 ? \'value must be a valid IPv4 address\' : \'\'H\x00R\x04ipv4\x12\x66\n\x04ipv6\x18\x0c \x01(\x08\x42P\xc2HM\nK\n\nbytes.ipv6\x1a=this.size() != 16 ? \'value must be a valid IPv6 address\' : \'\'H\x00R\x04ipv6B\x0c\n\nwell_knownB\x08\n\x06_constB\x06\n\x04_lenB\n\n\x08_min_lenB\n\n\x08_max_lenB\n\n\x08_patternB\t\n\x07_prefixB\t\n\x07_suffixB\x0b\n\t_contains\"\xbc\x03\n\tEnumRules\x12t\n\x05\x63onst\x18\x01 \x01(\x05\x42Y\xc2HV\nT\n\nenum.const\x1a\x46this != rules.const ? \'value must equal %s\'.format([rules.const]) : \'\'H\x00R\x05\x63onst\x88\x01\x01\x12&\n\x0c\x64\x65\x66ined_only\x18\x02 \x01(\x08H\x01R\x0b\x64\x65\x66inedOnly\x88\x01\x01\x12x\n\x02in\x18\x03 \x03(\x05\x42h\xc2He\nc\n\x07\x65num.in\x1aX!(this in dyn(rules)[\'in\']) ? \'value must be in list %s\'.format([dyn(rules)[\'in\']]) : \'\'R\x02in\x12|\n\x06not_in\x18\x04 \x03(\x05\x42\x65\xc2Hb\n`\n\x0b\x65num.not_in\x1aQthis in rules.not_in ? \'value must not be in list %s\'.format([rules.not_in]) : \'\'R\x05notInB\x08\n\x06_constB\x0f\n\r_defined_only\"\xcd\x04\n\rRepeatedRules\x12\xad\x01\n\tmin_items\x18\x01 \x01(\x04\x42\x8a\x01\xc2H\x86\x01\n\x83\x01\n\x12repeated.min_items\x1amuint(this.size()) < rules.min_items ? \'value must contain at least %d item(s)\'.format([rules.min_items]) : \'\'H\x00R\x08minItems\x88\x01\x01\x12\xb1\x01\n\tmax_items\x18\x02 \x01(\x04\x42\x8e\x01\xc2H\x8a\x01\n\x87\x01\n\x12repeated.max_items\x1aquint(this.size()) > rules.max_items ? \'value must contain no more than %s item(s)\'.format([rules.max_items]) : \'\'H\x01R\x08maxItems\x88\x01\x01\x12l\n\x06unique\x18\x03 \x01(\x08\x42O\xc2HL\nJ\n\x0frepeated.unique\x12(repeated value must contain unique items\x1a\rthis.unique()H\x02R\x06unique\x88\x01\x01\x12\x39\n\x05items\x18\x04 \x01(\x0b\x32\x1e.buf.validate.FieldConstraintsH\x03R\x05items\x88\x01\x01\x42\x0c\n\n_min_itemsB\x0c\n\n_max_itemsB\t\n\x07_uniqueB\x08\n\x06_items\"\xf1\x03\n\x08MapRules\x12\x9e\x01\n\tmin_pairs\x18\x01 \x01(\x04\x42|\xc2Hy\nw\n\rmap.min_pairs\x1a\x66uint(this.size()) < rules.min_pairs ? \'map must be at least %d entries\'.format([rules.min_pairs]) : \'\'H\x00R\x08minPairs\x88\x01\x01\x12\x9d\x01\n\tmax_pairs\x18\x02 \x01(\x04\x42{\xc2Hx\nv\n\rmap.max_pairs\x1a\x65uint(this.size()) > rules.max_pairs ? \'map must be at most %d entries\'.format([rules.max_pairs]) : \'\'H\x01R\x08maxPairs\x88\x01\x01\x12\x37\n\x04keys\x18\x04 \x01(\x0b\x32\x1e.buf.validate.FieldConstraintsH\x02R\x04keys\x88\x01\x01\x12;\n\x06values\x18\x05 \x01(\x0b\x32\x1e.buf.validate.FieldConstraintsH\x03R\x06values\x88\x01\x01\x42\x0c\n\n_min_pairsB\x0c\n\n_max_pairsB\x07\n\x05_keysB\t\n\x07_values\"1\n\x08\x41nyRules\x12\x0e\n\x02in\x18\x02 \x03(\tR\x02in\x12\x15\n\x06not_in\x18\x03 \x03(\tR\x05notIn\"\xd2\x16\n\rDurationRules\x12\x93\x01\n\x05\x63onst\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationB]\xc2HZ\nX\n\x0e\x64uration.const\x1a\x46this != rules.const ? \'value must equal %s\'.format([rules.const]) : \'\'H\x02R\x05\x63onst\x88\x01\x01\x12\xac\x01\n\x02lt\x18\x03 \x01(\x0b\x32\x19.google.protobuf.DurationB\x7f\xc2H|\nz\n\x0b\x64uration.lt\x1ak!has(rules.gte) && !has(rules.gt) && this >= rules.lt? \'value must be less than %s\'.format([rules.lt]) : \'\'H\x00R\x02lt\x12\xbf\x01\n\x03lte\x18\x04 \x01(\x0b\x32\x19.google.protobuf.DurationB\x8f\x01\xc2H\x8b\x01\n\x88\x01\n\x0c\x64uration.lte\x1ax!has(rules.gte) && !has(rules.gt) && this > rules.lte? \'value must be less than or equal to %s\'.format([rules.lte]) : \'\'H\x00R\x03lte\x12\xc5\x07\n\x02gt\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationB\x97\x07\xc2H\x93\x07\n}\n\x0b\x64uration.gt\x1an!has(rules.lt) && !has(rules.lte) && this <= rules.gt? \'value must be greater than %s\'.format([rules.gt]) : \'\'\n\xb6\x01\n\x0e\x64uration.gt_lt\x1a\xa3\x01has(rules.lt) && rules.lt >= rules.gt && (this >= rules.lt || this <= rules.gt)? \'value must be greater than %s and less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xbe\x01\n\x18\x64uration.gt_lt_exclusive\x1a\xa1\x01has(rules.lt) && rules.lt < rules.gt && (rules.lt <= this && this <= rules.gt)? \'value must be greater than %s or less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xc6\x01\n\x0f\x64uration.gt_lte\x1a\xb2\x01has(rules.lte) && rules.lte >= rules.gt && (this > rules.lte || this <= rules.gt)? \'value must be greater than %s and less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'\n\xce\x01\n\x19\x64uration.gt_lte_exclusive\x1a\xb0\x01has(rules.lte) && rules.lte < rules.gt && (rules.lte < this && this <= rules.gt)? \'value must be greater than %s or less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'H\x01R\x02gt\x12\x92\x08\n\x03gte\x18\x06 \x01(\x0b\x32\x19.google.protobuf.DurationB\xe2\x07\xc2H\xde\x07\n\x8b\x01\n\x0c\x64uration.gte\x1a{!has(rules.lt) && !has(rules.lte) && this < rules.gte? \'value must be greater than or equal to %s\'.format([rules.gte]) : \'\'\n\xc5\x01\n\x0f\x64uration.gte_lt\x1a\xb1\x01has(rules.lt) && rules.lt >= rules.gte && (this >= rules.lt || this < rules.gte)? \'value must be greater than or equal to %s and less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xcd\x01\n\x19\x64uration.gte_lt_exclusive\x1a\xaf\x01has(rules.lt) && rules.lt < rules.gte && (rules.lt <= this && this < rules.gte)? \'value must be greater than or equal to %s or less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xd5\x01\n\x10\x64uration.gte_lte\x1a\xc0\x01has(rules.lte) && rules.lte >= rules.gte && (this > rules.lte || this < rules.gte)? \'value must be greater than or equal to %s and less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'\n\xdd\x01\n\x1a\x64uration.gte_lte_exclusive\x1a\xbe\x01has(rules.lte) && rules.lte < rules.gte && (rules.lte < this && this < rules.gte)? \'value must be greater than or equal to %s or less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'H\x01R\x03gte\x12\x97\x01\n\x02in\x18\x07 \x03(\x0b\x32\x19.google.protobuf.DurationBl\xc2Hi\ng\n\x0b\x64uration.in\x1aX!(this in dyn(rules)[\'in\']) ? \'value must be in list %s\'.format([dyn(rules)[\'in\']]) : \'\'R\x02in\x12\x9b\x01\n\x06not_in\x18\x08 \x03(\x0b\x32\x19.google.protobuf.DurationBi\xc2Hf\nd\n\x0f\x64uration.not_in\x1aQthis in rules.not_in ? \'value must not be in list %s\'.format([rules.not_in]) : \'\'R\x05notInB\x0b\n\tless_thanB\x0e\n\x0cgreater_thanB\x08\n\x06_const\"\xca\x17\n\x0eTimestampRules\x12\x95\x01\n\x05\x63onst\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampB^\xc2H[\nY\n\x0ftimestamp.const\x1a\x46this != rules.const ? \'value must equal %s\'.format([rules.const]) : \'\'H\x02R\x05\x63onst\x88\x01\x01\x12\xaf\x01\n\x02lt\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x80\x01\xc2H}\n{\n\x0ctimestamp.lt\x1ak!has(rules.gte) && !has(rules.gt) && this >= rules.lt? \'value must be less than %s\'.format([rules.lt]) : \'\'H\x00R\x02lt\x12\xc1\x01\n\x03lte\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x90\x01\xc2H\x8c\x01\n\x89\x01\n\rtimestamp.lte\x1ax!has(rules.gte) && !has(rules.gt) && this > rules.lte? \'value must be less than or equal to %s\'.format([rules.lte]) : \'\'H\x00R\x03lte\x12\x61\n\x06lt_now\x18\x07 \x01(\x08\x42H\xc2HE\nC\n\x10timestamp.lt_now\x1a/this > now ? \'value must be less than now\' : \'\'H\x00R\x05ltNow\x12\xcb\x07\n\x02gt\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\x9c\x07\xc2H\x98\x07\n~\n\x0ctimestamp.gt\x1an!has(rules.lt) && !has(rules.lte) && this <= rules.gt? \'value must be greater than %s\'.format([rules.gt]) : \'\'\n\xb7\x01\n\x0ftimestamp.gt_lt\x1a\xa3\x01has(rules.lt) && rules.lt >= rules.gt && (this >= rules.lt || this <= rules.gt)? \'value must be greater than %s and less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xbf\x01\n\x19timestamp.gt_lt_exclusive\x1a\xa1\x01has(rules.lt) && rules.lt < rules.gt && (rules.lt <= this && this <= rules.gt)? \'value must be greater than %s or less than %s\'.format([rules.gt, rules.lt]) : \'\'\n\xc7\x01\n\x10timestamp.gt_lte\x1a\xb2\x01has(rules.lte) && rules.lte >= rules.gt && (this > rules.lte || this <= rules.gt)? \'value must be greater than %s and less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'\n\xcf\x01\n\x1atimestamp.gt_lte_exclusive\x1a\xb0\x01has(rules.lte) && rules.lte < rules.gt && (rules.lte < this && this <= rules.gt)? \'value must be greater than %s or less than or equal to %s\'.format([rules.gt, rules.lte]) : \'\'H\x01R\x02gt\x12\x98\x08\n\x03gte\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampB\xe7\x07\xc2H\xe3\x07\n\x8c\x01\n\rtimestamp.gte\x1a{!has(rules.lt) && !has(rules.lte) && this < rules.gte? \'value must be greater than or equal to %s\'.format([rules.gte]) : \'\'\n\xc6\x01\n\x10timestamp.gte_lt\x1a\xb1\x01has(rules.lt) && rules.lt >= rules.gte && (this >= rules.lt || this < rules.gte)? \'value must be greater than or equal to %s and less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xce\x01\n\x1atimestamp.gte_lt_exclusive\x1a\xaf\x01has(rules.lt) && rules.lt < rules.gte && (rules.lt <= this && this < rules.gte)? \'value must be greater than or equal to %s or less than %s\'.format([rules.gte, rules.lt]) : \'\'\n\xd6\x01\n\x11timestamp.gte_lte\x1a\xc0\x01has(rules.lte) && rules.lte >= rules.gte && (this > rules.lte || this < rules.gte)? \'value must be greater than or equal to %s and less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'\n\xde\x01\n\x1btimestamp.gte_lte_exclusive\x1a\xbe\x01has(rules.lte) && rules.lte < rules.gte && (rules.lte < this && this < rules.gte)? \'value must be greater than or equal to %s or less than or equal to %s\'.format([rules.gte, rules.lte]) : \'\'H\x01R\x03gte\x12\x64\n\x06gt_now\x18\x08 \x01(\x08\x42K\xc2HH\nF\n\x10timestamp.gt_now\x1a\x32this < now ? \'value must be greater than now\' : \'\'H\x01R\x05gtNow\x12\xc5\x01\n\x06within\x18\t \x01(\x0b\x32\x19.google.protobuf.DurationB\x8c\x01\xc2H\x88\x01\n\x85\x01\n\x10timestamp.within\x1aqthis < now-rules.within || this > now+rules.within ? \'value must be within %s of now\'.format([rules.within]) : \'\'H\x03R\x06within\x88\x01\x01\x42\x0b\n\tless_thanB\x0e\n\x0cgreater_thanB\x08\n\x06_constB\t\n\x07_within*n\n\nKnownRegex\x12\x1b\n\x17KNOWN_REGEX_UNSPECIFIED\x10\x00\x12 \n\x1cKNOWN_REGEX_HTTP_HEADER_NAME\x10\x01\x12!\n\x1dKNOWN_REGEX_HTTP_HEADER_VALUE\x10\x02:_\n\x07message\x12\x1f.google.protobuf.MessageOptions\x18\x87\t \x01(\x0b\x32 .buf.validate.MessageConstraintsR\x07message\x88\x01\x01:W\n\x05oneof\x12\x1d.google.protobuf.OneofOptions\x18\x87\t \x01(\x0b\x32\x1e.buf.validate.OneofConstraintsR\x05oneof\x88\x01\x01:W\n\x05\x66ield\x12\x1d.google.protobuf.FieldOptions\x18\x87\t \x01(\x0b\x32\x1e.buf.validate.FieldConstraintsR\x05\x66ield\x88\x01\x01\x42n\n\x12\x62uild.buf.validateB\rValidateProtoP\x01ZGbuf.build/gen/go/bufbuild/protovalidate/protocolbuffers/go/buf/validateb\x06proto3')
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/cache/v1/cache_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/cache/v1/cache_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/api_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/api_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/common_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/common_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from validate import validate_pb2 as validate_dot_validate__pb2
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.validate import validate_pb2 as validate_dot_validate__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x63ommon/v1/common.proto\x12\tcommon.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a\x1b\x62uf/validate/validate.proto\"\xb6\x01\n\nTimestamps\x12\x34\n\x07\x63reated\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12\x34\n\x07updated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07updated\x12<\n\x0b\x64\x65\x61\x63tivated\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0b\x64\x65\x61\x63tivated\"\xeb\x02\n\x08Metadata\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\"\n\x04name\x18\x03 \x01(\tB\x0e\xfa\x42\x04r\x02\x10\x01\xbaH\x04r\x02\x10\x01R\x04name\x12\x34\n\x0corganization\x18\x04 \x01(\tB\x10\xfa\x42\x05r\x03\xb0\x01\x01\xbaH\x05r\x03\xb0\x01\x01R\x0corganization\x12\x16\n\x06\x66older\x18\x05 \x01(\tR\x06\x66older\x12\x35\n\ntimestamps\x18\x06 \x01(\x0b\x32\x15.common.v1.TimestampsR\ntimestamps\x12\x18\n\x07version\x18\x07 \x01(\tR\x07version\x12\x31\n\x04tags\x18\x08 \x03(\x0b\x32\x1d.common.v1.Metadata.TagsEntryR\x04tags\x1a\x37\n\tTagsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"~\n\x07Profile\x12\x13\n\x02id\x18\x01 \x01(\tH\x00R\x02id\x88\x01\x01\x12\x17\n\x04name\x18\x02 \x01(\tH\x01R\x04name\x88\x01\x01\x12%\n\x0b\x65nvironment\x18\x03 \x01(\tH\x02R\x0b\x65nvironment\x88\x01\x01\x42\x05\n\x03_idB\x07\n\x05_nameB\x0e\n\x0c_environment*X\n\x08UserType\x12\x19\n\x15USER_TYPE_UNSPECIFIED\x10\x00\x12\x19\n\x15USER_TYPE_SUPERBLOCKS\x10\x01\x12\x16\n\x12USER_TYPE_EXTERNAL\x10\x02\x42\x33Z1github.com/superblocksteam/types/gen/go/common/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'common.v1.common_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/errors_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/errors_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/health_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/health_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/language_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/language_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/common/v1/utils_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/common/v1/utils_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/event/v1/cloudevent_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/event/v1/cloudevent_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/event/v1/event_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/event/v1/event_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from api.v1 import event_pb2 as api_dot_v1_dot_event__pb2
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.api.v1 import event_pb2 as api_dot_v1_dot_event__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14\x65vent/v1/event.proto\x12\x08\x65vent.v1\x1a\x12\x61pi/v1/event.proto\x1a\x1b\x62uf/validate/validate.proto\"\xc9\t\n\x0e\x45xecutionEvent\x12w\n\x0c\x65xecution_id\x18\x01 \x01(\tBT\xbaHQrO2M^[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}$R\x0b\x65xecutionId\x12u\n\x0bresource_id\x18\x02 \x01(\tBT\xbaHQrO2M^[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}$R\nresourceId\x12+\n\rresource_name\x18\x03 \x01(\tB\x06\xbaH\x03\xc8\x01\x01R\x0cresourceName\x12;\n\rresource_type\x18\x04 \x01(\x0e\x32\x0e.event.v1.TypeB\x06\xbaH\x03\xc8\x01\x01R\x0cresourceType\x12\x41\n\x10resource_subtype\x18\x05 \x01(\x0e\x32\x11.api.v1.BlockTypeH\x00R\x0fresourceSubtype\x88\x01\x01\x12\x30\n\x06result\x18\x06 \x01(\x0e\x32\x13.api.v1.BlockStatusH\x01R\x06result\x88\x01\x01\x12\x30\n\x06status\x18\x07 \x01(\x0e\x32\x10.event.v1.StatusB\x06\xbaH\x03\xc8\x01\x01R\x06status\x12*\n\x0eintegration_id\x18\x08 \x01(\tH\x02R\rintegrationId\x88\x01\x01\x12.\n\x10integration_type\x18\t \x01(\tH\x03R\x0fintegrationType\x88\x01\x01\x12*\n\x04mode\x18\n \x01(\x0e\x32\x0e.event.v1.ModeB\x06\xbaH\x03\xc8\x01\x01R\x04mode\x12}\n\x0forganization_id\x18\x0b \x01(\tBT\xbaHQrO2M^[a-fA-F0-9]{8}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{4}-[a-fA-F0-9]{12}$R\x0eorganizationId\x12\x1c\n\x07user_id\x18\x0c \x01(\tH\x04R\x06userId\x88\x01\x01\x12\x33\n\x07trigger\x18\r \x01(\x0e\x32\x11.event.v1.TriggerB\x06\xbaH\x03\xc8\x01\x01R\x07trigger\x12 \n\tparent_id\x18\x0e \x01(\tH\x05R\x08parentId\x88\x01\x01\x12$\n\x0bparent_name\x18\x0f \x01(\tH\x06R\nparentName\x88\x01\x01\x12\x34\n\x0bparent_type\x18\x10 \x01(\x0e\x32\x0e.event.v1.TypeH\x07R\nparentType\x88\x01\x01\x12\x35\n\x17is_descendant_of_stream\x18\x11 \x01(\x08R\x14isDescendantOfStream\x12\x1a\n\x06\x61pi_id\x18\x12 \x01(\tH\x08R\x05\x61piId\x88\x01\x01\x42\x13\n\x11_resource_subtypeB\t\n\x07_resultB\x11\n\x0f_integration_idB\x13\n\x11_integration_typeB\n\n\x08_user_idB\x0c\n\n_parent_idB\x0e\n\x0c_parent_nameB\x0e\n\x0c_parent_typeB\t\n\x07_api_id*R\n\x04Mode\x12\x14\n\x10MODE_UNSPECIFIED\x10\x00\x12\x11\n\rMODE_DEPLOYED\x10\x01\x12\x0f\n\x0bMODE_EDITOR\x10\x02\x12\x10\n\x0cMODE_PREVIEW\x10\x03*N\n\x04Type\x12\x14\n\x10TYPE_UNSPECIFIED\x10\x00\x12\x16\n\x12TYPE_EXECUTION_API\x10\x01\x12\x18\n\x14TYPE_EXECUTION_BLOCK\x10\x02*F\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATUS_STARTED\x10\x01\x12\x10\n\x0cSTATUS_ENDED\x10\x02*b\n\x07Trigger\x12\x17\n\x13TRIGGER_UNSPECIFIED\x10\x00\x12\x17\n\x13TRIGGER_APPLICATION\x10\x01\x12\x14\n\x10TRIGGER_WORKFLOW\x10\x02\x12\x0f\n\x0bTRIGGER_JOB\x10\x03\x42\x32Z0github.com/superblocksteam/types/gen/go/event/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'event.v1.event_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/event/v1/service_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/event/v1/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/event/v2/cloudevent_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/event/v2/cloudevent_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/event/v2/service_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/event/v2/service_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/event/v2/service_pb2_grpc.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/event/v2/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/google/api/annotations_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/google/api/annotations_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.api import http_pb2 as google_dot_api_dot_http__pb2
+from superblocks_types.google.api import http_pb2 as google_dot_api_dot_http__pb2
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cgoogle/api/annotations.proto\x12\ngoogle.api\x1a\x15google/api/http.proto\x1a google/protobuf/descriptor.proto:K\n\x04http\x12\x1e.google.protobuf.MethodOptions\x18\xb0\xca\xbc\" \x01(\x0b\x32\x14.google.api.HttpRuleR\x04httpBn\n\x0e\x63om.google.apiB\x10\x41nnotationsProtoP\x01ZAgoogle.golang.org/genproto/googleapis/api/annotations;annotations\xa2\x02\x04GAPIb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/google/api/http_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/intake/v1/logs_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/intake/v1/logs_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/integration/v1/service_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/integration/v1/service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
-from common.v1 import common_pb2 as common_dot_v1_dot_common__pb2
+from superblocks_types.common.v1 import common_pb2 as common_dot_v1_dot_common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cintegration/v1/service.proto\x12\x0eintegration.v1\x1a\x1cgoogle/protobuf/struct.proto\x1a\x16\x63ommon/v1/common.proto\"I\n\x16GetIntegrationResponse\x12/\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x1b.integration.v1.IntegrationR\x04\x64\x61ta\"\xc3\x01\n\x16GetIntegrationsRequest\x12\x31\n\x07profile\x18\x01 \x01(\x0b\x32\x12.common.v1.ProfileH\x00R\x07profile\x88\x01\x01\x12\x10\n\x03ids\x18\x02 \x03(\tR\x03ids\x12-\n\x04kind\x18\x03 \x01(\x0e\x32\x14.integration.v1.KindH\x01R\x04kind\x88\x01\x01\x12\x17\n\x04slug\x18\x04 \x01(\tH\x02R\x04slug\x88\x01\x01\x42\n\n\x08_profileB\x07\n\x05_kindB\x07\n\x05_slug\"J\n\x17GetIntegrationsResponse\x12/\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x1b.integration.v1.IntegrationR\x04\x64\x61ta\"\xdf\x01\n\rConfiguration\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x18\n\x07\x63reated\x18\x02 \x01(\tR\x07\x63reated\x12%\n\x0eintegration_id\x18\x03 \x01(\tR\rintegrationId\x12=\n\rconfiguration\x18\x04 \x01(\x0b\x32\x17.google.protobuf.StructR\rconfiguration\x12\x1d\n\nis_default\x18\x05 \x01(\x08R\tisDefault\x12\x1f\n\x0bprofile_ids\x18\x06 \x03(\tR\nprofileIds\"\xe4\x02\n\x0bIntegration\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x18\n\x07\x63reated\x18\x02 \x01(\tR\x07\x63reated\x12\x18\n\x07updated\x18\x03 \x01(\tR\x07updated\x12\x12\n\x04name\x18\x04 \x01(\tR\x04name\x12\x1b\n\tplugin_id\x18\x05 \x01(\tR\x08pluginId\x12\'\n\x0forganization_id\x18\x06 \x01(\tR\x0eorganizationId\x12.\n\x13\x64\x65mo_integration_id\x18\x07 \x01(\tR\x11\x64\x65moIntegrationId\x12\x45\n\x0e\x63onfigurations\x18\x08 \x03(\x0b\x32\x1d.integration.v1.ConfigurationR\x0e\x63onfigurations\x12,\n\x12is_user_configured\x18\t \x01(\x08R\x10isUserConfigured\x12\x12\n\x04slug\x18\n \x01(\tR\x04slug*>\n\x04Kind\x12\x14\n\x10KIND_UNSPECIFIED\x10\x00\x12\x0f\n\x0bKIND_PLUGIN\x10\x01\x12\x0f\n\x0bKIND_SECRET\x10\x02\x42\x38Z6github.com/superblocksteam/types/gen/go/integration/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'integration.v1.service_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/kafka/v1/kafka_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/kafka/v1/kafka_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/adls/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/adls/v1/plugin_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from plugins.common.v1 import auth_pb2 as plugins_dot_common_dot_v1_dot_auth__pb2
-from plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.common.v1 import auth_pb2 as plugins_dot_common_dot_v1_dot_auth__pb2
+from superblocks_types.plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cplugins/adls/v1/plugin.proto\x12\x0fplugins.adls.v1\x1a\x1cplugins/common/v1/auth.proto\x1a\x1eplugins/common/v1/plugin.proto\"\xc0\r\n\x06Plugin\x12\x17\n\x04name\x18\x01 \x01(\tH\x01R\x04name\x88\x01\x01\x12z\n\x1e\x64ynamic_workflow_configuration\x18\x02 \x01(\x0b\x32/.plugins.common.v1.DynamicWorkflowConfigurationH\x02R\x1c\x64ynamicWorkflowConfiguration\x88\x01\x01\x12\x46\n\nconnection\x18\x03 \x01(\x0b\x32&.plugins.adls.v1.Plugin.AdlsConnectionR\nconnection\x12T\n\x10\x63reate_container\x18\x04 \x01(\x0b\x32\'.plugins.adls.v1.Plugin.CreateContainerH\x00R\x0f\x63reateContainer\x12T\n\x10\x63reate_directory\x18\x05 \x01(\x0b\x32\'.plugins.adls.v1.Plugin.CreateDirectoryH\x00R\x0f\x63reateDirectory\x12T\n\x10rename_directory\x18\x06 \x01(\x0b\x32\'.plugins.adls.v1.Plugin.RenameDirectoryH\x00R\x0frenameDirectory\x12T\n\x10\x64\x65lete_directory\x18\x07 \x01(\x0b\x32\'.plugins.adls.v1.Plugin.DeleteDirectoryH\x00R\x0f\x64\x65leteDirectory\x12g\n\x17list_directory_contents\x18\x08 \x01(\x0b\x32-.plugins.adls.v1.Plugin.ListDirectoryContentsH\x00R\x15listDirectoryContents\x12\x45\n\x0bupload_file\x18\t \x01(\x0b\x32\".plugins.adls.v1.Plugin.UploadFileH\x00R\nuploadFile\x12K\n\rdownload_file\x18\n \x01(\x0b\x32$.plugins.adls.v1.Plugin.DownloadFileH\x00R\x0c\x64ownloadFile\x12\x45\n\x0b\x64\x65lete_file\x18\x0b \x01(\x0b\x32\".plugins.adls.v1.Plugin.DeleteFileH\x00R\ndeleteFile\x1ay\n\x0e\x41\x64lsConnection\x12!\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\tR\x0b\x61\x63\x63ountName\x12\x16\n\x06tenant\x18\x02 \x01(\tR\x06tenant\x12,\n\x04\x61uth\x18\x03 \x01(\x0b\x32\x18.plugins.common.v1.AzureR\x04\x61uth\x1a\x32\n\x0f\x43reateContainer\x12\x1f\n\x0b\x66ile_system\x18\x02 \x01(\tR\nfileSystem\x1a\x46\n\x0f\x43reateDirectory\x12\x1f\n\x0b\x66ile_system\x18\x01 \x01(\tR\nfileSystem\x12\x12\n\x04path\x18\x02 \x01(\tR\x04path\x1a\x61\n\x0fRenameDirectory\x12\x1f\n\x0b\x66ile_system\x18\x01 \x01(\tR\nfileSystem\x12\x12\n\x04path\x18\x02 \x01(\tR\x04path\x12\x19\n\x08new_path\x18\x03 \x01(\tR\x07newPath\x1a\x46\n\x0f\x44\x65leteDirectory\x12\x1f\n\x0b\x66ile_system\x18\x01 \x01(\tR\nfileSystem\x12\x12\n\x04path\x18\x02 \x01(\tR\x04path\x1aL\n\x15ListDirectoryContents\x12\x1f\n\x0b\x66ile_system\x18\x01 \x01(\tR\nfileSystem\x12\x12\n\x04path\x18\x02 \x01(\tR\x04path\x1a[\n\nUploadFile\x12\x1f\n\x0b\x66ile_system\x18\x01 \x01(\tR\nfileSystem\x12\x12\n\x04path\x18\x02 \x01(\tR\x04path\x12\x18\n\x07\x63ontent\x18\x03 \x01(\tR\x07\x63ontent\x1a\x43\n\x0c\x44ownloadFile\x12\x1f\n\x0b\x66ile_system\x18\x01 \x01(\tR\nfileSystem\x12\x12\n\x04path\x18\x02 \x01(\tR\x04path\x1a\x41\n\nDeleteFile\x12\x1f\n\x0b\x66ile_system\x18\x01 \x01(\tR\nfileSystem\x12\x12\n\x04path\x18\x02 \x01(\tR\x04path\x1a-\n\x08Metadata\x12!\n\x0c\x66ile_systems\x18\x01 \x03(\tR\x0b\x66ileSystemsB\r\n\x0b\x61\x64ls_actionB\x07\n\x05_nameB!\n\x1f_dynamic_workflow_configurationB9Z7github.com/superblocksteam/types/gen/go/plugins/adls/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.adls.v1.plugin_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/athena/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/athena/v1/plugin_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1eplugins/athena/v1/plugin.proto\x12\x11plugins.athena.v1\x1a\x1eplugins/common/v1/plugin.proto\"\xce\x04\n\nConnection\x12*\n\x0eworkgroup_name\x18\x01 \x01(\tH\x00R\rworkgroupName\x88\x01\x01\x12=\n\x1boverride_s3_output_location\x18\x02 \x01(\x08R\x18overrideS3OutputLocation\x12\x31\n\x12s3_output_location\x18\x03 \x01(\tH\x01R\x10s3OutputLocation\x88\x01\x01\x12l\n\x19s3_output_location_suffix\x18\x04 \x01(\x0e\x32,.plugins.athena.v1.Connection.DateFolderTypeH\x02R\x16s3OutputLocationSuffix\x88\x01\x01\x12#\n\rdatabase_name\x18\x05 \x01(\tR\x0c\x64\x61tabaseName\x12;\n\naws_config\x18\x06 \x01(\x0b\x32\x1c.plugins.common.v1.AWSConfigR\tawsConfig\"\x89\x01\n\x0e\x44\x61teFolderType\x12 \n\x1c\x44\x41TE_FOLDER_TYPE_UNSPECIFIED\x10\x00\x12\x19\n\x15\x44\x41TE_FOLDER_TYPE_YYYY\x10\x01\x12\x1b\n\x17\x44\x41TE_FOLDER_TYPE_YYYYMM\x10\x02\x12\x1d\n\x19\x44\x41TE_FOLDER_TYPE_YYYYMMDD\x10\x03\x42\x11\n\x0f_workgroup_nameB\x15\n\x13_s3_output_locationB\x1c\n\x1a_s3_output_location_suffix\"\xc2\x02\n\x06Plugin\x12\x17\n\x04name\x18\x01 \x01(\tH\x00R\x04name\x88\x01\x01\x12=\n\nconnection\x18\x02 \x01(\x0b\x32\x1d.plugins.athena.v1.ConnectionR\nconnection\x12\x38\n\x07run_sql\x18\x03 \x01(\x0b\x32\x1f.plugins.common.v1.SQLExecutionR\x06runSql\x12z\n\x1e\x64ynamic_workflow_configuration\x18\x04 \x01(\x0b\x32/.plugins.common.v1.DynamicWorkflowConfigurationH\x01R\x1c\x64ynamicWorkflowConfiguration\x88\x01\x01\x42\x07\n\x05_nameB!\n\x1f_dynamic_workflow_configurationB;Z9github.com/superblocksteam/types/gen/go/plugins/athena/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.athena.v1.plugin_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/bigquery/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/bigquery/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/cockroachdb/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/cockroachdb/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/common/v1/auth_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/common/v1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/common/v1/metadata_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/common/v1/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/common/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/common/v1/plugin_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1eplugins/common/v1/plugin.proto\x12\x11plugins.common.v1\x1a\x1b\x62uf/validate/validate.proto\"\x7f\n\x1c\x44ynamicWorkflowConfiguration\x12\x1d\n\x07\x65nabled\x18\x01 \x01(\x08H\x00R\x07\x65nabled\x88\x01\x01\x12$\n\x0bworkflow_id\x18\x02 \x01(\tH\x01R\nworkflowId\x88\x01\x01\x42\n\n\x08_enabledB\x0e\n\x0c_workflow_id\"\xa7\x02\n\tAWSConfig\x12\x1b\n\x06region\x18\x01 \x01(\tH\x00R\x06region\x88\x01\x01\x12:\n\x04\x61uth\x18\x02 \x01(\x0b\x32!.plugins.common.v1.AWSConfig.AuthH\x01R\x04\x61uth\x88\x01\x01\x1a\xac\x01\n\x04\x41uth\x12\'\n\raccess_key_id\x18\x01 \x01(\tH\x00R\x0b\x61\x63\x63\x65ssKeyId\x88\x01\x01\x12\"\n\nsecret_key\x18\x02 \x01(\tH\x01R\tsecretKey\x88\x01\x01\x12%\n\x0ciam_role_arn\x18\x03 \x01(\tH\x02R\niamRoleArn\x88\x01\x01\x42\x10\n\x0e_access_key_idB\r\n\x0b_secret_keyB\x0f\n\r_iam_role_arnB\t\n\x07_regionB\x07\n\x05_auth\"V\n\x0cSQLExecution\x12\x19\n\x08sql_body\x18\x01 \x01(\tR\x07sqlBody\x12+\n\x11use_parameterized\x18\x02 \x01(\x08R\x10useParameterized\"8\n\x10SQLMappedColumns\x12\x12\n\x04json\x18\x01 \x01(\tR\x04json\x12\x10\n\x03sql\x18\x02 \x01(\tR\x03sql\"\xf0\x03\n\x10SSHConfiguration\x12Z\n\x15\x61uthentication_method\x18\x01 \x01(\x0e\x32 .plugins.common.v1.SSHAuthMethodH\x00R\x14\x61uthenticationMethod\x88\x01\x01\x12\x1d\n\x07\x65nabled\x18\x02 \x01(\x08H\x01R\x07\x65nabled\x88\x01\x01\x12\x17\n\x04host\x18\x03 \x01(\tH\x02R\x04host\x88\x01\x01\x12#\n\npassphrase\x18\x04 \x01(\tH\x03R\npassphrase\x88\x01\x01\x12\x1f\n\x08password\x18\x05 \x01(\tH\x04R\x08password\x88\x01\x01\x12\x17\n\x04port\x18\x06 \x01(\x05H\x05R\x04port\x88\x01\x01\x12$\n\x0bprivate_key\x18\x07 \x01(\tH\x06R\nprivateKey\x88\x01\x01\x12\"\n\npublic_key\x18\x08 \x01(\tH\x07R\tpublicKey\x88\x01\x01\x12\x1f\n\x08username\x18\t \x01(\tH\x08R\x08username\x88\x01\x01\x42\x18\n\x16_authentication_methodB\n\n\x08_enabledB\x07\n\x05_hostB\r\n\x0b_passphraseB\x0b\n\t_passwordB\x07\n\x05_portB\x0e\n\x0c_private_keyB\r\n\x0b_public_keyB\x0b\n\t_username\"\xf6\x04\n\x0bSQLBulkEdit\x12Z\n\rmatching_mode\x18\x01 \x01(\x0e\x32\".plugins.common.v1.SQLMatchingModeB\x0c\xbaH\t\x82\x01\x06\x10\x01\x1a\x02\x01\x02H\x00R\x0cmatchingMode\x88\x01\x01\x12\x1b\n\x06schema\x18\x02 \x01(\tH\x01R\x06schema\x88\x01\x01\x12\x19\n\x05table\x18\x03 \x01(\tH\x02R\x05table\x88\x01\x01\x12&\n\x0cupdated_rows\x18\x04 \x01(\tH\x03R\x0bupdatedRows\x88\x01\x01\x12\x1e\n\x08old_rows\x18\x05 \x01(\tH\x04R\x07oldRows\x88\x01\x01\x12\x1b\n\tfilter_by\x18\x06 \x03(\tR\x08\x66ilterBy\x12W\n\x0cmapping_mode\x18\x07 \x01(\x0e\x32!.plugins.common.v1.SQLMappingModeB\x0c\xbaH\t\x82\x01\x06\x10\x01\x1a\x02\x01\x02H\x05R\x0bmappingMode\x88\x01\x01\x12J\n\x0emapped_columns\x18\x08 \x03(\x0b\x32#.plugins.common.v1.SQLMappedColumnsR\rmappedColumns\x12(\n\rinserted_rows\x18\t \x01(\tH\x06R\x0cinsertedRows\x88\x01\x01\x12&\n\x0c\x64\x65leted_rows\x18\n \x01(\tH\x07R\x0b\x64\x65letedRows\x88\x01\x01\x42\x10\n\x0e_matching_modeB\t\n\x07_schemaB\x08\n\x06_tableB\x0f\n\r_updated_rowsB\x0b\n\t_old_rowsB\x0f\n\r_mapping_modeB\x10\n\x0e_inserted_rowsB\x0f\n\r_deleted_rows*\xba\x01\n\rSSHAuthMethod\x12\x1f\n\x1bSSH_AUTH_METHOD_UNSPECIFIED\x10\x00\x12\x1c\n\x18SSH_AUTH_METHOD_PASSWORD\x10\x01\x12\x1f\n\x1bSSH_AUTH_METHOD_PUB_KEY_RSA\x10\x02\x12#\n\x1fSSH_AUTH_METHOD_PUB_KEY_ED25519\x10\x03\x12$\n SSH_AUTH_METHOD_USER_PRIVATE_KEY\x10\x04*j\n\x0eSQLMappingMode\x12 \n\x1cSQL_MAPPING_MODE_UNSPECIFIED\x10\x00\x12\x19\n\x15SQL_MAPPING_MODE_AUTO\x10\x01\x12\x1b\n\x17SQL_MAPPING_MODE_MANUAL\x10\x02*p\n\x0fSQLMatchingMode\x12!\n\x1dSQL_MATCHING_MODE_UNSPECIFIED\x10\x00\x12\x1a\n\x16SQL_MATCHING_MODE_AUTO\x10\x01\x12\x1e\n\x1aSQL_MATCHING_MODE_ADVANCED\x10\x02*g\n\x0cSQLOperation\x12\x1d\n\x19SQL_OPERATION_UNSPECIFIED\x10\x00\x12\x19\n\x15SQL_OPERATION_RUN_SQL\x10\x01\x12\x1d\n\x19SQL_OPERATION_UPDATE_ROWS\x10\x02\x42;Z9github.com/superblocksteam/types/gen/go/plugins/common/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.common.v1.plugin_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/cosmosdb/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/cosmosdb/v1/plugin_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from plugins.common.v1 import auth_pb2 as plugins_dot_common_dot_v1_dot_auth__pb2
-from plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.common.v1 import auth_pb2 as plugins_dot_common_dot_v1_dot_auth__pb2
+from superblocks_types.plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n plugins/cosmosdb/v1/plugin.proto\x12\x13plugins.cosmosdb.v1\x1a\x1cplugins/common/v1/auth.proto\x1a\x1eplugins/common/v1/plugin.proto\"\x88\x10\n\x06Plugin\x12\x17\n\x04name\x18\x01 \x01(\tH\x01R\x04name\x88\x01\x01\x12z\n\x1e\x64ynamic_workflow_configuration\x18\x02 \x01(\x0b\x32/.plugins.common.v1.DynamicWorkflowConfigurationH\x02R\x1c\x64ynamicWorkflowConfiguration\x88\x01\x01\x12N\n\nconnection\x18\x03 \x01(\x0b\x32..plugins.cosmosdb.v1.Plugin.CosmosDbConnectionR\nconnection\x12\x33\n\x03sql\x18\x05 \x01(\x0b\x32\x1f.plugins.cosmosdb.v1.Plugin.SqlH\x00R\x03sql\x12U\n\x0fpoint_operation\x18\x06 \x01(\x0b\x32*.plugins.cosmosdb.v1.Plugin.PointOperationH\x00R\x0epointOperation\x1a\x8b\x01\n\x12\x43osmosDbConnection\x12\x12\n\x04host\x18\x01 \x01(\tR\x04host\x12\x12\n\x04port\x18\x02 \x01(\x05R\x04port\x12\x1f\n\x0b\x64\x61tabase_id\x18\x03 \x01(\tR\ndatabaseId\x12,\n\x04\x61uth\x18\x04 \x01(\x0b\x32\x18.plugins.common.v1.AzureR\x04\x61uth\x1a\xbf\x02\n\x08Metadata\x12N\n\ncontainers\x18\x01 \x03(\x0b\x32..plugins.cosmosdb.v1.Plugin.Metadata.ContainerR\ncontainers\x1a\xe2\x01\n\tContainer\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12`\n\rpartition_key\x18\x02 \x01(\x0b\x32;.plugins.cosmosdb.v1.Plugin.Metadata.Container.PartitionKeyR\x0cpartitionKey\x1a\x63\n\x0cPartitionKey\x12\x14\n\x05paths\x18\x01 \x03(\tR\x05paths\x12\x12\n\x04kind\x18\x02 \x01(\tR\x04kind\x12\x1d\n\x07version\x18\x03 \x01(\x05H\x00R\x07version\x88\x01\x01\x42\n\n\x08_version\x1a\x86\x02\n\x03Sql\x12I\n\tsingleton\x18\x01 \x01(\x0b\x32).plugins.cosmosdb.v1.Plugin.Sql.SingletonH\x00R\tsingleton\x1a\xa9\x01\n\tSingleton\x12!\n\x0c\x63ontainer_id\x18\x01 \x01(\tR\x0b\x63ontainerId\x12\x14\n\x05query\x18\x02 \x01(\tR\x05query\x12\'\n\x0f\x63ross_partition\x18\x03 \x01(\x08R\x0e\x63rossPartition\x12(\n\rpartition_key\x18\x04 \x01(\tH\x00R\x0cpartitionKey\x88\x01\x01\x42\x10\n\x0e_partition_keyB\x08\n\x06\x61\x63tion\x1a\xf4\x06\n\x0ePointOperation\x12!\n\x0c\x63ontainer_id\x18\x01 \x01(\tR\x0b\x63ontainerId\x12\x45\n\x04read\x18\x02 \x01(\x0b\x32/.plugins.cosmosdb.v1.Plugin.PointOperation.ReadH\x00R\x04read\x12N\n\x07replace\x18\x03 \x01(\x0b\x32\x32.plugins.cosmosdb.v1.Plugin.PointOperation.ReplaceH\x00R\x07replace\x12K\n\x06upsert\x18\x04 \x01(\x0b\x32\x31.plugins.cosmosdb.v1.Plugin.PointOperation.UpsertH\x00R\x06upsert\x12K\n\x06\x64\x65lete\x18\x05 \x01(\x0b\x32\x31.plugins.cosmosdb.v1.Plugin.PointOperation.DeleteH\x00R\x06\x64\x65lete\x12K\n\x06\x63reate\x18\x06 \x01(\x0b\x32\x31.plugins.cosmosdb.v1.Plugin.PointOperation.CreateH\x00R\x06\x63reate\x1aR\n\x04Read\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12(\n\rpartition_key\x18\x03 \x01(\tH\x00R\x0cpartitionKey\x88\x01\x01\x42\x10\n\x0e_partition_key\x1aT\n\x06\x44\x65lete\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12(\n\rpartition_key\x18\x03 \x01(\tH\x00R\x0cpartitionKey\x88\x01\x01\x42\x10\n\x0e_partition_key\x1aY\n\x07Replace\x12\x12\n\x04\x62ody\x18\x01 \x01(\tR\x04\x62ody\x12(\n\rpartition_key\x18\x03 \x01(\tH\x00R\x0cpartitionKey\x88\x01\x01\x42\x10\n\x0e_partition_key\x1aX\n\x06Upsert\x12\x12\n\x04\x62ody\x18\x01 \x01(\tR\x04\x62ody\x12(\n\rpartition_key\x18\x03 \x01(\tH\x00R\x0cpartitionKey\x88\x01\x01\x42\x10\n\x0e_partition_key\x1aX\n\x06\x43reate\x12\x12\n\x04\x62ody\x18\x01 \x01(\tR\x04\x62ody\x12(\n\rpartition_key\x18\x03 \x01(\tH\x00R\x0cpartitionKey\x88\x01\x01\x42\x10\n\x0e_partition_keyB\x08\n\x06\x61\x63tionB\x11\n\x0f\x63osmosdb_actionB\x07\n\x05_nameB!\n\x1f_dynamic_workflow_configurationB=Z;github.com/superblocksteam/types/gen/go/plugins/cosmosdb/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.cosmosdb.v1.plugin_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/couchbase/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/couchbase/v1/plugin_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n!plugins/couchbase/v1/plugin.proto\x12\x14plugins.couchbase.v1\x1a\x1eplugins/common/v1/plugin.proto\"\xb0\n\n\x06Plugin\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12P\n\nconnection\x18\x02 \x01(\x0b\x32\x30.plugins.couchbase.v1.Plugin.CouchbaseConnectionR\nconnection\x12J\n\x08\x65ndpoint\x18\x03 \x01(\x0b\x32..plugins.couchbase.v1.Plugin.CouchbaseEndpointR\x08\x65ndpoint\x12z\n\x1e\x64ynamic_workflow_configuration\x18\x04 \x01(\x0b\x32/.plugins.common.v1.DynamicWorkflowConfigurationH\x01R\x1c\x64ynamicWorkflowConfiguration\x88\x01\x01\x12;\n\x06tunnel\x18\x05 \x01(\x0b\x32#.plugins.common.v1.SSHConfigurationR\x06tunnel\x12:\n\x07run_sql\x18\x06 \x01(\x0b\x32\x1f.plugins.common.v1.SQLExecutionH\x00R\x06runSql\x12\x46\n\x06insert\x18\x07 \x01(\x0b\x32,.plugins.couchbase.v1.Plugin.CouchbaseInsertH\x00R\x06insert\x12=\n\x03get\x18\x08 \x01(\x0b\x32).plugins.couchbase.v1.Plugin.CouchbaseGetH\x00R\x03get\x12\x46\n\x06remove\x18\t \x01(\x0b\x32,.plugins.couchbase.v1.Plugin.CouchbaseRemoveH\x00R\x06remove\x1a;\n\x11\x43ouchbaseEndpoint\x12\x12\n\x04host\x18\x01 \x01(\tR\x04host\x12\x12\n\x04port\x18\x02 \x01(\x05R\x04port\x1aK\n\x13\x43ouchbaseIdentifier\x12\x14\n\x05scope\x18\x01 \x01(\tR\x05scope\x12\x1e\n\ncollection\x18\x02 \x01(\tR\ncollection\x1av\n\x13\x43ouchbaseConnection\x12\x12\n\x04user\x18\x02 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x03 \x01(\tR\x08password\x12\x16\n\x06\x62ucket\x18\x04 \x01(\tR\x06\x62ucket\x12\x17\n\x07use_tls\x18\x05 \x01(\x08R\x06useTls\x1a\x8b\x01\n\x0f\x43ouchbaseInsert\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\x12P\n\nidentifier\x18\x03 \x01(\x0b\x32\x30.plugins.couchbase.v1.Plugin.CouchbaseIdentifierR\nidentifier\x1ar\n\x0c\x43ouchbaseGet\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12P\n\nidentifier\x18\x02 \x01(\x0b\x32\x30.plugins.couchbase.v1.Plugin.CouchbaseIdentifierR\nidentifier\x1au\n\x0f\x43ouchbaseRemove\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12P\n\nidentifier\x18\x02 \x01(\x0b\x32\x30.plugins.couchbase.v1.Plugin.CouchbaseIdentifierR\nidentifierB\x12\n\x10\x63ouchbase_actionB!\n\x1f_dynamic_workflow_configurationB>Z<github.com/superblocksteam/types/gen/go/plugins/couchbase/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.couchbase.v1.plugin_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/custom/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/custom/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/databricks/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/databricks/v1/plugin_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"plugins/databricks/v1/plugin.proto\x12\x15plugins.databricks.v1\x1a\x1eplugins/common/v1/plugin.proto\"\xb8\x05\n\x06Plugin\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12R\n\nconnection\x18\x02 \x01(\x0b\x32\x32.plugins.databricks.v1.Plugin.DatabricksConnectionR\nconnection\x12=\n\toperation\x18\x03 \x01(\x0e\x32\x1f.plugins.common.v1.SQLOperationR\toperation\x12\x38\n\x07run_sql\x18\x04 \x01(\x0b\x32\x1f.plugins.common.v1.SQLExecutionR\x06runSql\x12;\n\tbulk_edit\x18\x05 \x01(\x0b\x32\x1e.plugins.common.v1.SQLBulkEditR\x08\x62ulkEdit\x12z\n\x1e\x64ynamic_workflow_configuration\x18\x06 \x01(\x0b\x32/.plugins.common.v1.DynamicWorkflowConfigurationH\x00R\x1c\x64ynamicWorkflowConfiguration\x88\x01\x01\x1a\xf0\x01\n\x14\x44\x61tabricksConnection\x12,\n\x0f\x64\x65\x66\x61ult_catalog\x18\x01 \x01(\tH\x00R\x0e\x64\x65\x66\x61ultCatalog\x88\x01\x01\x12*\n\x0e\x64\x65\x66\x61ult_schema\x18\x02 \x01(\tH\x01R\rdefaultSchema\x88\x01\x01\x12\x19\n\x08host_url\x18\x03 \x01(\tR\x07hostUrl\x12\x12\n\x04path\x18\x04 \x01(\tR\x04path\x12\x12\n\x04port\x18\x05 \x01(\x05R\x04port\x12\x14\n\x05token\x18\x06 \x01(\tR\x05tokenB\x12\n\x10_default_catalogB\x11\n\x0f_default_schemaB!\n\x1f_dynamic_workflow_configurationB?Z=github.com/superblocksteam/types/gen/go/plugins/databricks/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.databricks.v1.plugin_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/dynamodb/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/dynamodb/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/email/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/email/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/gcs/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/gcs/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/graphql/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/graphql/v1/plugin_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from common.v1 import plugin_pb2 as common_dot_v1_dot_plugin__pb2
+from superblocks_types.common.v1 import plugin_pb2 as common_dot_v1_dot_plugin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fplugins/graphql/v1/plugin.proto\x12\x12plugins.graphql.v1\x1a\x16\x63ommon/v1/plugin.proto\"v\n\x06\x43ustom\x12\x31\n\tvariables\x18\x01 \x01(\x0b\x32\x13.common.v1.PropertyR\tvariables\x12\x39\n\rrequestFormat\x18\x02 \x01(\x0b\x32\x13.common.v1.PropertyR\rrequestFormat\"\xf5\x01\n\x06Plugin\x12\x12\n\x04path\x18\x01 \x01(\tR\x04path\x12-\n\x07headers\x18\x02 \x03(\x0b\x32\x13.common.v1.PropertyR\x07headers\x12\x12\n\x04\x62ody\x18\x03 \x01(\tR\x04\x62ody\x12\x37\n\x06\x63ustom\x18\x04 \x01(\x0b\x32\x1a.plugins.graphql.v1.CustomH\x00R\x06\x63ustom\x88\x01\x01\x12P\n\x13superblocksMetadata\x18\x05 \x01(\x0b\x32\x1e.common.v1.SuperblocksMetadataR\x13superblocksMetadataB\t\n\x07_customB<Z:github.com/superblocksteam/types/gen/go/plugins/graphql/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.graphql.v1.plugin_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/gsheets/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/gsheets/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/javascript/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/javascript/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/kafka/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/kafka/v1/plugin_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
-from validate import validate_pb2 as validate_dot_validate__pb2
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
-from plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
+from superblocks_types.validate import validate_pb2 as validate_dot_validate__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dplugins/kafka/v1/plugin.proto\x12\x10plugins.kafka.v1\x1a\x1cgoogle/protobuf/struct.proto\x1a\x17validate/validate.proto\x1a\x1b\x62uf/validate/validate.proto\x1a\x1eplugins/common/v1/plugin.proto\"\x93\x01\n\x08Metadata\x12/\n\x06topics\x18\x01 \x03(\x0b\x32\x17.plugins.kafka.v1.TopicR\x06topics\x12\x32\n\x07\x62rokers\x18\x02 \x03(\x0b\x32\x18.plugins.kafka.v1.BrokerR\x07\x62rokers\x1a\"\n\x08Minified\x12\x16\n\x06topics\x18\x01 \x03(\tR\x06topics\";\n\x06\x42roker\x12\x17\n\x07node_id\x18\x01 \x01(\x05R\x06nodeId\x12\x18\n\x07\x61\x64\x64ress\x18\x02 \x01(\tR\x07\x61\x64\x64ress\"\x1b\n\x05Topic\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\"A\n\x08Messages\x12\x35\n\x08messages\x18\x01 \x03(\x0b\x32\x19.plugins.kafka.v1.MessageR\x08messages\"\xb0\x03\n\x07Message\x12\x14\n\x05topic\x18\x01 \x01(\tR\x05topic\x12\x1c\n\tpartition\x18\x02 \x01(\x05R\tpartition\x12\x16\n\x06offset\x18\x04 \x01(\x05R\x06offset\x12!\n\ttimestamp\x18\x03 \x01(\tH\x00R\ttimestamp\x88\x01\x01\x12-\n\x03key\x18\x05 \x01(\x0b\x32\x16.google.protobuf.ValueH\x01R\x03key\x88\x01\x01\x12\x31\n\x05value\x18\x06 \x01(\x0b\x32\x16.google.protobuf.ValueH\x02R\x05value\x88\x01\x01\x12\x16\n\x06length\x18\x07 \x01(\x05R\x06length\x12\x1e\n\nattributes\x18\x08 \x01(\x05R\nattributes\x12@\n\x07headers\x18\t \x03(\x0b\x32&.plugins.kafka.v1.Message.HeadersEntryR\x07headers\x1a:\n\x0cHeadersEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x42\x0c\n\n_timestampB\x06\n\x04_keyB\x08\n\x06_value\"\xac\x04\n\x04SASL\x12>\n\tmechanism\x18\x01 \x01(\x0e\x32 .plugins.kafka.v1.SASL.MechanismR\tmechanism\x12\x1f\n\x08username\x18\x02 \x01(\tH\x00R\x08username\x88\x01\x01\x12\x1f\n\x08password\x18\x03 \x01(\tH\x01R\x08password\x88\x01\x01\x12\'\n\raccess_key_id\x18\x04 \x01(\tH\x02R\x0b\x61\x63\x63\x65ssKeyId\x88\x01\x01\x12\"\n\nsecret_key\x18\x05 \x01(\tH\x03R\tsecretKey\x88\x01\x01\x12(\n\rsession_token\x18\x06 \x01(\tH\x04R\x0csessionToken\x88\x01\x01\x12:\n\x16\x61uthorization_identity\x18\x07 \x01(\tH\x05R\x15\x61uthorizationIdentity\x88\x01\x01\"\x86\x01\n\tMechanism\x12\x19\n\x15MECHANISM_UNSPECIFIED\x10\x00\x12\x13\n\x0fMECHANISM_PLAIN\x10\x01\x12\x1a\n\x16MECHANISM_SCRAM_SHA256\x10\x02\x12\x1a\n\x16MECHANISM_SCRAM_SHA512\x10\x03\x12\x11\n\rMECHANISM_AWS\x10\x04\x42\x0b\n\t_usernameB\x0b\n\t_passwordB\x10\n\x0e_access_key_idB\r\n\x0b_secret_keyB\x10\n\x0e_session_tokenB\x19\n\x17_authorization_identity\"q\n\x07\x43luster\x12(\n\x07\x62rokers\x18\x01 \x01(\tB\x0e\xfa\x42\x04r\x02\x10\x01\xbaH\x04r\x02\x10\x01R\x07\x62rokers\x12\x10\n\x03ssl\x18\x02 \x01(\x08R\x03ssl\x12*\n\x04sasl\x18\x03 \x01(\x0b\x32\x16.plugins.kafka.v1.SASLR\x04sasl\"\xa5\x0b\n\x06Plugin\x12\x17\n\x04name\x18\x01 \x01(\tH\x00R\x04name\x88\x01\x01\x12\x39\n\toperation\x18\x02 \x01(\x0e\x32\x1b.plugins.kafka.v1.OperationR\toperation\x12:\n\x07produce\x18\x03 \x01(\x0b\x32 .plugins.kafka.v1.Plugin.ProduceR\x07produce\x12:\n\x07\x63onsume\x18\x04 \x01(\x0b\x32 .plugins.kafka.v1.Plugin.ConsumeR\x07\x63onsume\x12\x33\n\x07\x63luster\x18\x05 \x01(\x0b\x32\x19.plugins.kafka.v1.ClusterR\x07\x63luster\x12W\n\x13superblocksMetadata\x18\x06 \x01(\x0b\x32%.plugins.kafka.v1.SuperblocksMetadataR\x13superblocksMetadata\x12z\n\x1e\x64ynamic_workflow_configuration\x18\x07 \x01(\x0b\x32/.plugins.common.v1.DynamicWorkflowConfigurationH\x01R\x1c\x64ynamicWorkflowConfiguration\x88\x01\x01\x1a\xe6\x03\n\x07\x43onsume\x12L\n\x04\x66rom\x18\x01 \x01(\x0e\x32%.plugins.kafka.v1.Plugin.Consume.FromB\x11\xfa\x42\x05\x82\x01\x02 \x00\xbaH\x06\x82\x01\x03\"\x01\x00R\x04\x66rom\x12\x14\n\x05topic\x18\x02 \x01(\tR\x05topic\x12\x1e\n\x08group_id\x18\x03 \x01(\tH\x00R\x07groupId\x88\x01\x01\x12 \n\tclient_id\x18\x04 \x01(\tH\x01R\x08\x63lientId\x88\x01\x01\x12\x39\n\x04seek\x18\x05 \x01(\x0b\x32%.plugins.kafka.v1.Plugin.Consume.SeekR\x04seek\x12)\n\x10read_uncommitted\x18\x06 \x01(\x08R\x0freadUncommitted\x1a\x62\n\x04Seek\x12$\n\x05topic\x18\x01 \x01(\tB\x0e\xfa\x42\x04r\x02\x10\x01\xbaH\x04r\x02\x10\x01R\x05topic\x12\x16\n\x06offset\x18\x02 \x01(\x05R\x06offset\x12\x1c\n\tpartition\x18\x03 \x01(\x05R\tpartition\"P\n\x04\x46rom\x12\x14\n\x10\x46ROM_UNSPECIFIED\x10\x00\x12\x12\n\x0e\x46ROM_BEGINNING\x10\x01\x12\x0f\n\x0b\x46ROM_LATEST\x10\x02\x12\r\n\tFROM_SEEK\x10\x03\x42\x0b\n\t_group_idB\x0c\n\n_client_id\x1a\xaf\x03\n\x07Produce\x12*\n\x04\x61\x63ks\x18\x01 \x01(\x0e\x32\x16.plugins.kafka.v1.AcksR\x04\x61\x63ks\x12 \n\tclient_id\x18\x02 \x01(\tH\x00R\x08\x63lientId\x88\x01\x01\x12\x1d\n\x07timeout\x18\x03 \x01(\x05H\x01R\x07timeout\x88\x01\x01\x12\x44\n\x0b\x63ompression\x18\x04 \x01(\x0e\x32\x1d.plugins.kafka.v1.CompressionH\x02R\x0b\x63ompression\x88\x01\x01\x12*\n\x0etransaction_id\x18\x05 \x01(\tH\x03R\rtransactionId\x88\x01\x01\x12*\n\x11\x61uto_create_topic\x18\x06 \x01(\x08R\x0f\x61utoCreateTopic\x12\x1e\n\nidempotent\x18\x07 \x01(\x08R\nidempotent\x12 \n\x0btransaction\x18\x08 \x01(\x08R\x0btransaction\x12\x1a\n\x08messages\x18\t \x01(\tR\x08messagesB\x0c\n\n_client_idB\n\n\x08_timeoutB\x0e\n\x0c_compressionB\x11\n\x0f_transaction_idB\x07\n\x05_nameB!\n\x1f_dynamic_workflow_configuration\"\xa9\x01\n\x13SuperblocksMetadata\x12*\n\x0eplugin_version\x18\x01 \x01(\tH\x00R\rpluginVersion\x88\x01\x01\x12\x38\n\x16synced_from_profile_id\x18\x02 \x01(\tH\x01R\x13syncedFromProfileId\x88\x01\x01\x42\x11\n\x0f_plugin_versionB\x19\n\x17_synced_from_profile_id*T\n\tOperation\x12\x19\n\x15OPERATION_UNSPECIFIED\x10\x00\x12\x15\n\x11OPERATION_CONSUME\x10\x01\x12\x15\n\x11OPERATION_PRODUCE\x10\x02*\x83\x01\n\x0b\x43ompression\x12\x1b\n\x17\x43OMPRESSION_UNSPECIFIED\x10\x00\x12\x14\n\x10\x43OMPRESSION_GZIP\x10\x01\x12\x16\n\x12\x43OMPRESSION_SNAPPY\x10\x02\x12\x13\n\x0f\x43OMPRESSION_LZ4\x10\x03\x12\x14\n\x10\x43OMPRESSION_ZSTD\x10\x04*J\n\x04\x41\x63ks\x12\x14\n\x10\x41\x43KS_UNSPECIFIED\x10\x00\x12\r\n\tACKS_NONE\x10\x01\x12\x0f\n\x0b\x41\x43KS_LEADER\x10\x02\x12\x0c\n\x08\x41\x43KS_ALL\x10\x03\x42:Z8github.com/superblocksteam/types/gen/go/plugins/kafka/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.kafka.v1.plugin_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mariadb/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mariadb/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mongodb/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mongodb/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mssql/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mssql/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/mysql/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/mysql/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/ocr/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/ocr/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/openai/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/openai/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/oracledb/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/oracledb/v1/plugin_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n plugins/oracledb/v1/plugin.proto\x12\x13plugins.oracledb.v1\x1a\x1eplugins/common/v1/plugin.proto\"\xfd\x04\n\x06Plugin\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12N\n\nconnection\x18\x02 \x01(\x0b\x32..plugins.oracledb.v1.Plugin.OracleDbConnectionR\nconnection\x12z\n\x1e\x64ynamic_workflow_configuration\x18\x03 \x01(\x0b\x32/.plugins.common.v1.DynamicWorkflowConfigurationH\x00R\x1c\x64ynamicWorkflowConfiguration\x88\x01\x01\x12\x38\n\x07run_sql\x18\x04 \x01(\x0b\x32\x1f.plugins.common.v1.SQLExecutionR\x06runSql\x12;\n\tbulk_edit\x18\x05 \x01(\x0b\x32\x1e.plugins.common.v1.SQLBulkEditR\x08\x62ulkEdit\x12=\n\toperation\x18\x06 \x01(\x0e\x32\x1f.plugins.common.v1.SQLOperationR\toperation\x1a\xb9\x01\n\x12OracleDbConnection\x12\x19\n\x08host_url\x18\x01 \x01(\tR\x07hostUrl\x12\x12\n\x04port\x18\x02 \x01(\x05R\x04port\x12\x12\n\x04user\x18\x03 \x01(\tR\x04user\x12\x1a\n\x08password\x18\x04 \x01(\tR\x08password\x12)\n\x10\x64\x61tabase_service\x18\x05 \x01(\tR\x0f\x64\x61tabaseService\x12\x19\n\x08use_tcps\x18\x06 \x01(\x08R\x07useTcpsB!\n\x1f_dynamic_workflow_configurationB=Z;github.com/superblocksteam/types/gen/go/plugins/oracledb/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.oracledb.v1.plugin_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/pinecone/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/pinecone/v1/plugin_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n plugins/pinecone/v1/plugin.proto\x12\x13plugins.pinecone.v1\x1a\x1eplugins/common/v1/plugin.proto\"\xaf\x06\n\x06Plugin\x12\x17\n\x04name\x18\x01 \x01(\tH\x01R\x04name\x88\x01\x01\x12z\n\x1e\x64ynamic_workflow_configuration\x18\x02 \x01(\x0b\x32/.plugins.common.v1.DynamicWorkflowConfigurationH\x02R\x1c\x64ynamicWorkflowConfiguration\x88\x01\x01\x12\x46\n\nconnection\x18\x03 \x01(\x0b\x32&.plugins.pinecone.v1.Plugin.ConnectionR\nconnection\x12L\n\x0clist_indexes\x18\x04 \x01(\x0b\x32\'.plugins.pinecone.v1.Plugin.ListIndexesH\x00R\x0blistIndexes\x12L\n\x0c\x63reate_index\x18\x05 \x01(\x0b\x32\'.plugins.pinecone.v1.Plugin.CreateIndexH\x00R\x0b\x63reateIndex\x12O\n\rupsert_vector\x18\x06 \x01(\x0b\x32(.plugins.pinecone.v1.Plugin.UpsertVectorH\x00R\x0cupsertVector\x12\x39\n\x05query\x18\x07 \x01(\x0b\x32!.plugins.pinecone.v1.Plugin.QueryH\x00R\x05query\x1aG\n\nConnection\x12 \n\x0b\x65nvironment\x18\x01 \x01(\tR\x0b\x65nvironment\x12\x17\n\x07\x61pi_key\x18\x02 \x01(\tR\x06\x61piKey\x1a\r\n\x0bListIndexes\x1a!\n\x0b\x43reateIndex\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x1a*\n\x0cUpsertVector\x12\x12\n\x03raw\x18\x01 \x01(\tH\x00R\x03rawB\x06\n\x04\x64\x61ta\x1a\x43\n\x05Query\x12\x16\n\x06vector\x18\x01 \x01(\tR\x06vector\x12\x18\n\x05top_k\x18\x02 \x01(\tH\x00R\x04topK\x88\x01\x01\x42\x08\n\x06_top_kB\x08\n\x06\x61\x63tionB\x07\n\x05_nameB!\n\x1f_dynamic_workflow_configurationB=Z;github.com/superblocksteam/types/gen/go/plugins/pinecone/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.pinecone.v1.plugin_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/postgresql/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/postgresql/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/python/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/python/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/redis/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/redis/v1/plugin_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dplugins/redis/v1/plugin.proto\x12\x10plugins.redis.v1\x1a\x1eplugins/common/v1/plugin.proto\"\xe9$\n\x06Plugin\x12\x17\n\x04name\x18\x01 \x01(\tH\x01R\x04name\x88\x01\x01\x12\x43\n\nconnection\x18\x02 \x01(\x0b\x32#.plugins.redis.v1.Plugin.ConnectionR\nconnection\x12\x30\n\x03raw\x18\x03 \x01(\x0b\x32\x1c.plugins.redis.v1.Plugin.RawH\x00R\x03raw\x12\x45\n\nstructured\x18\x04 \x01(\x0b\x32#.plugins.redis.v1.Plugin.StructuredH\x00R\nstructured\x12z\n\x1e\x64ynamic_workflow_configuration\x18\x05 \x01(\x0b\x32/.plugins.common.v1.DynamicWorkflowConfigurationH\x02R\x1c\x64ynamicWorkflowConfiguration\x88\x01\x01\x1az\n\x03Raw\x12\x46\n\tsingleton\x18\x01 \x01(\x0b\x32&.plugins.redis.v1.Plugin.Raw.SingletonH\x00R\tsingleton\x1a!\n\tSingleton\x12\x14\n\x05query\x18\x01 \x01(\tR\x05queryB\x08\n\x06\x61\x63tion\x1a\x8c\x0f\n\nStructured\x12\x30\n\x03get\x18\x06 \x01(\x0b\x32\x1c.plugins.redis.v1.Plugin.GetH\x00R\x03get\x12\x30\n\x03set\x18\x07 \x01(\x0b\x32\x1c.plugins.redis.v1.Plugin.SetH\x00R\x03set\x12\x30\n\x03\x64\x65l\x18\x08 \x01(\x0b\x32\x1c.plugins.redis.v1.Plugin.DelH\x00R\x03\x64\x65l\x12\x33\n\x04keys\x18\t \x01(\x0b\x32\x1d.plugins.redis.v1.Plugin.KeysH\x00R\x04keys\x12\x33\n\x04mget\x18\n \x01(\x0b\x32\x1d.plugins.redis.v1.Plugin.MgetH\x00R\x04mget\x12\x33\n\x04hget\x18\x0b \x01(\x0b\x32\x1d.plugins.redis.v1.Plugin.HgetH\x00R\x04hget\x12\x36\n\x05hmget\x18\x0c \x01(\x0b\x32\x1e.plugins.redis.v1.Plugin.HmgetH\x00R\x05hmget\x12<\n\x07hgetall\x18\r \x01(\x0b\x32 .plugins.redis.v1.Plugin.HgetallH\x00R\x07hgetall\x12\x33\n\x04hset\x18\x0e \x01(\x0b\x32\x1d.plugins.redis.v1.Plugin.HsetH\x00R\x04hset\x12\x39\n\x06hsetnx\x18\x0f \x01(\x0b\x32\x1f.plugins.redis.v1.Plugin.HsetnxH\x00R\x06hsetnx\x12\x33\n\x04hlen\x18\x10 \x01(\x0b\x32\x1d.plugins.redis.v1.Plugin.HlenH\x00R\x04hlen\x12\x33\n\x04hdel\x18\x11 \x01(\x0b\x32\x1d.plugins.redis.v1.Plugin.HdelH\x00R\x04hdel\x12\x36\n\x05hkeys\x18\x12 \x01(\x0b\x32\x1e.plugins.redis.v1.Plugin.HkeysH\x00R\x05hkeys\x12\x36\n\x05hvals\x18\x13 \x01(\x0b\x32\x1e.plugins.redis.v1.Plugin.HvalsH\x00R\x05hvals\x12\x39\n\x06lindex\x18\x14 \x01(\x0b\x32\x1f.plugins.redis.v1.Plugin.LindexH\x00R\x06lindex\x12\x33\n\x04llen\x18\x15 \x01(\x0b\x32\x1d.plugins.redis.v1.Plugin.LlenH\x00R\x04llen\x12\x36\n\x05lpush\x18\x16 \x01(\x0b\x32\x1e.plugins.redis.v1.Plugin.LpushH\x00R\x05lpush\x12\x33\n\x04lrem\x18\x17 \x01(\x0b\x32\x1d.plugins.redis.v1.Plugin.LremH\x00R\x04lrem\x12\x39\n\x06lrange\x18\x18 \x01(\x0b\x32\x1f.plugins.redis.v1.Plugin.LrangeH\x00R\x06lrange\x12\x33\n\x04sadd\x18\x19 \x01(\x0b\x32\x1d.plugins.redis.v1.Plugin.SaddH\x00R\x04sadd\x12\x36\n\x05scard\x18\x1a \x01(\x0b\x32\x1e.plugins.redis.v1.Plugin.ScardH\x00R\x05scard\x12?\n\x08smembers\x18\x1b \x01(\x0b\x32!.plugins.redis.v1.Plugin.SmembersH\x00R\x08smembers\x12\x42\n\tsismember\x18\x1c \x01(\x0b\x32\".plugins.redis.v1.Plugin.SismemberH\x00R\tsismember\x12H\n\x0bsrandmember\x18\x1d \x01(\x0b\x32$.plugins.redis.v1.Plugin.SrandmemberH\x00R\x0bsrandmember\x12\x33\n\x04srem\x18\x1e \x01(\x0b\x32\x1d.plugins.redis.v1.Plugin.SremH\x00R\x04srem\x12\x33\n\x04zadd\x18\x1f \x01(\x0b\x32\x1d.plugins.redis.v1.Plugin.ZaddH\x00R\x04zadd\x12\x36\n\x05zcard\x18  \x01(\x0b\x32\x1e.plugins.redis.v1.Plugin.ZcardH\x00R\x05zcard\x12\x39\n\x06zcount\x18! \x01(\x0b\x32\x1f.plugins.redis.v1.Plugin.ZcountH\x00R\x06zcount\x12\x39\n\x06zrange\x18\" \x01(\x0b\x32\x1f.plugins.redis.v1.Plugin.ZrangeH\x00R\x06zrange\x12\x36\n\x05zrank\x18# \x01(\x0b\x32\x1e.plugins.redis.v1.Plugin.ZrankH\x00R\x05zrank\x12\x33\n\x04zrem\x18$ \x01(\x0b\x32\x1d.plugins.redis.v1.Plugin.ZremH\x00R\x04zrem\x12\x39\n\x06zscore\x18% \x01(\x0b\x32\x1f.plugins.redis.v1.Plugin.ZscoreH\x00R\x06zscore\x12\x39\n\x06\x65xpire\x18& \x01(\x0b\x32\x1f.plugins.redis.v1.Plugin.ExpireH\x00R\x06\x65xpire\x12\x30\n\x03ttl\x18\' \x01(\x0b\x32\x1c.plugins.redis.v1.Plugin.TtlH\x00R\x03ttlB\x08\n\x06\x61\x63tion\x1a\xb8\x03\n\nConnection\x12;\n\x03url\x18\x01 \x01(\x0b\x32\'.plugins.redis.v1.Plugin.Connection.UrlH\x00R\x03url\x12\x44\n\x06\x66ields\x18\x02 \x01(\x0b\x32*.plugins.redis.v1.Plugin.Connection.FieldsH\x00R\x06\x66ields\x1a$\n\x03Url\x12\x1d\n\nurl_string\x18\x01 \x01(\tR\turlString\x1a\xed\x01\n\x06\x46ields\x12\x12\n\x04host\x18\x01 \x01(\tR\x04host\x12\x12\n\x04port\x18\x02 \x01(\x05R\x04port\x12,\n\x0f\x64\x61tabase_number\x18\x03 \x01(\x05H\x00R\x0e\x64\x61tabaseNumber\x88\x01\x01\x12\x1f\n\x08username\x18\x04 \x01(\tH\x01R\x08username\x88\x01\x01\x12\x1f\n\x08password\x18\x05 \x01(\tH\x02R\x08password\x88\x01\x01\x12\x1d\n\nenable_ssl\x18\x06 \x01(\x08R\tenableSslB\x12\n\x10_database_numberB\x0b\n\t_usernameB\x0b\n\t_passwordB\x11\n\x0f\x63onnection_type\x1a\x17\n\x03Get\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x1ai\n\x03Set\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\x12(\n\rexpiration_ms\x18\x03 \x01(\x05H\x00R\x0c\x65xpirationMs\x88\x01\x01\x42\x10\n\x0e_expiration_ms\x1a\x17\n\x03\x44\x65l\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x1a \n\x04Keys\x12\x18\n\x07pattern\x18\x01 \x01(\tR\x07pattern\x1a\x1a\n\x04Mget\x12\x12\n\x04keys\x18\x01 \x01(\tR\x04keys\x1a.\n\x04Hget\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05\x66ield\x18\x02 \x01(\tR\x05\x66ield\x1a\x31\n\x05Hmget\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x16\n\x06\x66ields\x18\x02 \x01(\tR\x06\x66ields\x1a\x1b\n\x07Hgetall\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x1a\x44\n\x04Hset\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05\x66ield\x18\x02 \x01(\tR\x05\x66ield\x12\x14\n\x05value\x18\x03 \x01(\tR\x05value\x1a\x46\n\x06Hsetnx\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05\x66ield\x18\x02 \x01(\tR\x05\x66ield\x12\x14\n\x05value\x18\x03 \x01(\tR\x05value\x1a\x18\n\x04Hlen\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x1a.\n\x04Hdel\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05\x66ield\x18\x02 \x01(\tR\x05\x66ield\x1a\x19\n\x05Hkeys\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x1a\x19\n\x05Hvals\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x1a\x30\n\x06Lindex\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05index\x18\x02 \x01(\x05R\x05index\x1a\x18\n\x04Llen\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x1a/\n\x05Lpush\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\x1a\x44\n\x04Lrem\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05\x63ount\x18\x02 \x01(\x05R\x05\x63ount\x12\x14\n\x05value\x18\x03 \x01(\tR\x05value\x1a\x44\n\x06Lrange\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05start\x18\x02 \x01(\x05R\x05start\x12\x12\n\x04stop\x18\x03 \x01(\x05R\x04stop\x1a\x30\n\x04Sadd\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x16\n\x06member\x18\x02 \x01(\tR\x06member\x1a\x19\n\x05Scard\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x1a\x1c\n\x08Smembers\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x1a\x35\n\tSismember\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x16\n\x06member\x18\x02 \x01(\tR\x06member\x1a\x44\n\x0bSrandmember\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x19\n\x05\x63ount\x18\x02 \x01(\x05H\x00R\x05\x63ount\x88\x01\x01\x42\x08\n\x06_count\x1a\x30\n\x04Srem\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x16\n\x06member\x18\x02 \x01(\tR\x06member\x1a\x46\n\x04Zadd\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05score\x18\x02 \x01(\x01R\x05score\x12\x16\n\x06member\x18\x03 \x01(\tR\x06member\x1a\x19\n\x05Zcard\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x1a>\n\x06Zcount\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x10\n\x03min\x18\x02 \x01(\x01R\x03min\x12\x10\n\x03max\x18\x03 \x01(\x01R\x03max\x1a\x44\n\x06Zrange\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05start\x18\x02 \x01(\x05R\x05start\x12\x12\n\x04stop\x18\x03 \x01(\x05R\x04stop\x1a\x31\n\x05Zrank\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x16\n\x06member\x18\x02 \x01(\tR\x06member\x1a\x30\n\x04Zrem\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x16\n\x06member\x18\x02 \x01(\tR\x06member\x1a\x32\n\x06Zscore\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x16\n\x06member\x18\x02 \x01(\tR\x06member\x1a\xe2\x01\n\x06\x45xpire\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x18\n\x07seconds\x18\x02 \x01(\x05R\x07seconds\x12\x43\n\x06option\x18\x03 \x01(\x0e\x32&.plugins.redis.v1.Plugin.Expire.OptionH\x00R\x06option\x88\x01\x01\"\\\n\x06Option\x12\x16\n\x12OPTION_UNSPECIFIED\x10\x00\x12\r\n\tOPTION_NX\x10\x01\x12\r\n\tOPTION_XX\x10\x02\x12\r\n\tOPTION_GT\x10\x03\x12\r\n\tOPTION_LT\x10\x04\x42\t\n\x07_option\x1a\x17\n\x03Ttl\x12\x10\n\x03key\x18\x01 \x01(\tR\x03keyB\x0e\n\x0c\x63ommand_typeB\x07\n\x05_nameB!\n\x1f_dynamic_workflow_configurationB:Z8github.com/superblocksteam/types/gen/go/plugins/redis/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.redis.v1.plugin_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/redshift/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/redshift/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/restapi/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/restapi/v1/plugin_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from common.v1 import plugin_pb2 as common_dot_v1_dot_plugin__pb2
+from superblocks_types.common.v1 import plugin_pb2 as common_dot_v1_dot_plugin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1fplugins/restapi/v1/plugin.proto\x12\x12plugins.restapi.v1\x1a\x16\x63ommon/v1/plugin.proto\"\xc9\x03\n\x06Plugin\x12\x1e\n\nhttpMethod\x18\x01 \x01(\tR\nhttpMethod\x12\"\n\x0cresponseType\x18\x02 \x01(\tR\x0cresponseType\x12-\n\x07headers\x18\x03 \x03(\x0b\x32\x13.common.v1.PropertyR\x07headers\x12+\n\x06params\x18\x04 \x03(\x0b\x32\x13.common.v1.PropertyR\x06params\x12\x1a\n\x08\x62odyType\x18\x05 \x01(\tR\x08\x62odyType\x12\x12\n\x04\x62ody\x18\x06 \x01(\tR\x04\x62ody\x12/\n\x08\x66ormData\x18\x07 \x03(\x0b\x32\x13.common.v1.PropertyR\x08\x66ormData\x12 \n\x0b\x66ileFormKey\x18\x08 \x01(\tR\x0b\x66ileFormKey\x12\x1a\n\x08\x66ileName\x18\t \x01(\tR\x08\x66ileName\x12\x12\n\x04path\x18\n \x01(\tR\x04path\x12\x1a\n\x08jsonBody\x18\x0b \x01(\tR\x08jsonBody\x12P\n\x13superblocksMetadata\x18\x0c \x01(\x0b\x32\x1e.common.v1.SuperblocksMetadataR\x13superblocksMetadataB<Z:github.com/superblocksteam/types/gen/go/plugins/restapi/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.restapi.v1.plugin_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/restapiintegration/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/restapiintegration/v1/plugin_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from common.v1 import plugin_pb2 as common_dot_v1_dot_plugin__pb2
+from superblocks_types.common.v1 import plugin_pb2 as common_dot_v1_dot_plugin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n*plugins/restapiintegration/v1/plugin.proto\x12\x1dplugins.restapiintegration.v1\x1a\x16\x63ommon/v1/plugin.proto\"\x9c\x05\n\x06Plugin\x12\x1e\n\nhttpMethod\x18\x01 \x01(\tR\nhttpMethod\x12\"\n\x0cresponseType\x18\x02 \x01(\tR\x0cresponseType\x12-\n\x07headers\x18\x03 \x03(\x0b\x32\x13.common.v1.PropertyR\x07headers\x12+\n\x06params\x18\x04 \x03(\x0b\x32\x13.common.v1.PropertyR\x06params\x12\x1a\n\x08\x62odyType\x18\x05 \x01(\tR\x08\x62odyType\x12\x12\n\x04\x62ody\x18\x06 \x01(\tR\x04\x62ody\x12\x1a\n\x08jsonBody\x18\x07 \x01(\tR\x08jsonBody\x12/\n\x08\x66ormData\x18\x08 \x03(\x0b\x32\x13.common.v1.PropertyR\x08\x66ormData\x12 \n\x0b\x66ileFormKey\x18\t \x01(\tR\x0b\x66ileFormKey\x12\x1a\n\x08\x66ileName\x18\n \x01(\tR\x08\x66ileName\x12\x18\n\x07urlBase\x18\x0b \x01(\tR\x07urlBase\x12\x18\n\x07urlPath\x18\x0c \x01(\tR\x07urlPath\x12\x1a\n\x08\x61uthType\x18\r \x01(\tR\x08\x61uthType\x12P\n\x13superblocksMetadata\x18\x0e \x01(\x0b\x32\x1e.common.v1.SuperblocksMetadataR\x13superblocksMetadata\x12$\n\ropenApiAction\x18\x0f \x01(\tR\ropenApiAction\x12&\n\x0eopenApiSpecRef\x18\x10 \x01(\tR\x0eopenApiSpecRef\x12\x31\n\x11openApiTenantName\x18\x11 \x01(\tH\x00R\x11openApiTenantName\x88\x01\x01\x42\x14\n\x12_openApiTenantNameBGZEgithub.com/superblocksteam/types/gen/go/plugins/restapiintegration/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.restapiintegration.v1.plugin_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/rockset/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/rockset/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/s3/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/s3/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/salesforce/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/salesforce/v1/plugin_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from plugins.common.v1 import auth_pb2 as plugins_dot_common_dot_v1_dot_auth__pb2
-from plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.common.v1 import auth_pb2 as plugins_dot_common_dot_v1_dot_auth__pb2
+from superblocks_types.plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"plugins/salesforce/v1/plugin.proto\x12\x15plugins.salesforce.v1\x1a\x1cplugins/common/v1/auth.proto\x1a\x1eplugins/common/v1/plugin.proto\"\xf5\x0c\n\x06Plugin\x12\x17\n\x04name\x18\x01 \x01(\tH\x01R\x04name\x88\x01\x01\x12R\n\nconnection\x18\x02 \x01(\x0b\x32\x32.plugins.salesforce.v1.Plugin.SalesforceConnectionR\nconnection\x12\x38\n\x04soql\x18\x03 \x01(\x0b\x32\".plugins.salesforce.v1.Plugin.SoqlH\x00R\x04soql\x12\x38\n\x04\x63rud\x18\x04 \x01(\x0b\x32\".plugins.salesforce.v1.Plugin.CrudH\x00R\x04\x63rud\x12\x38\n\x04\x62ulk\x18\x05 \x01(\x0b\x32\".plugins.salesforce.v1.Plugin.BulkH\x00R\x04\x62ulk\x12z\n\x1e\x64ynamic_workflow_configuration\x18\x06 \x01(\x0b\x32/.plugins.common.v1.DynamicWorkflowConfigurationH\x02R\x1c\x64ynamicWorkflowConfiguration\x88\x01\x01\x1a\x66\n\x14SalesforceConnection\x12!\n\x0cinstance_url\x18\x01 \x01(\tR\x0binstanceUrl\x12+\n\x04\x61uth\x18\x02 \x01(\x0b\x32\x17.plugins.common.v1.AuthR\x04\x61uth\x1a\xf2\x01\n\x08Metadata\x12G\n\x07objects\x18\x01 \x03(\x0b\x32-.plugins.salesforce.v1.Plugin.Metadata.ObjectR\x07objects\x1a\x9c\x01\n\x06Object\x12K\n\x06\x66ields\x18\x01 \x03(\x0b\x32\x33.plugins.salesforce.v1.Plugin.Metadata.Object.FieldR\x06\x66ields\x1a\x45\n\x05\x46ield\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x14\n\x05label\x18\x02 \x01(\tR\x05label\x12\x12\n\x04type\x18\x03 \x01(\tR\x04type\x1a\xa9\x01\n\x04Soql\x12\x19\n\x08sql_body\x18\x01 \x01(\tR\x07sqlBody\x12\x45\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32-.plugins.salesforce.v1.Plugin.Soql.SoqlActionR\x06\x61\x63tion\"?\n\nSoqlAction\x12\x1b\n\x17SOQL_ACTION_UNSPECIFIED\x10\x00\x12\x14\n\x10SOQL_ACTION_SOQL\x10\x01\x1a\xc2\x02\n\x04\x43rud\x12#\n\rresource_type\x18\x01 \x01(\tR\x0cresourceType\x12\x45\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32-.plugins.salesforce.v1.Plugin.Crud.CrudActionR\x06\x61\x63tion\x12#\n\rresource_body\x18\x03 \x01(\tR\x0cresourceBody\x12\x1f\n\x0bresource_id\x18\x04 \x01(\tR\nresourceId\"\x87\x01\n\nCrudAction\x12\x1b\n\x17\x43RUD_ACTION_UNSPECIFIED\x10\x00\x12\x16\n\x12\x43RUD_ACTION_CREATE\x10\x01\x12\x16\n\x12\x43RUD_ACTION_UPDATE\x10\x02\x12\x16\n\x12\x43RUD_ACTION_DELETE\x10\x03\x12\x14\n\x10\x43RUD_ACTION_READ\x10\x04\x1a\xc4\x02\n\x04\x42ulk\x12#\n\rresource_type\x18\x01 \x01(\tR\x0cresourceType\x12\x45\n\x06\x61\x63tion\x18\x02 \x01(\x0e\x32-.plugins.salesforce.v1.Plugin.Bulk.BulkActionR\x06\x61\x63tion\x12#\n\rresource_body\x18\x03 \x01(\tR\x0cresourceBody\x12\x1f\n\x0b\x65xternal_id\x18\x04 \x01(\tR\nexternalId\"\x89\x01\n\nBulkAction\x12\x1b\n\x17\x42ULK_ACTION_UNSPECIFIED\x10\x00\x12\x16\n\x12\x42ULK_ACTION_CREATE\x10\x01\x12\x16\n\x12\x42ULK_ACTION_UPDATE\x10\x02\x12\x16\n\x12\x42ULK_ACTION_DELETE\x10\x03\x12\x16\n\x12\x42ULK_ACTION_UPSERT\x10\x04\x42\x13\n\x11salesforce_actionB\x07\n\x05_nameB!\n\x1f_dynamic_workflow_configurationB?Z=github.com/superblocksteam/types/gen/go/plugins/salesforce/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.salesforce.v1.plugin_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/smtp/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/smtp/v1/plugin_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.common.v1 import plugin_pb2 as plugins_dot_common_dot_v1_dot_plugin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1cplugins/smtp/v1/plugin.proto\x12\x0fplugins.smtp.v1\x1a\x1eplugins/common/v1/plugin.proto\"\xdd\x04\n\x06Plugin\x12\x17\n\x04name\x18\x01 \x01(\tH\x00R\x04name\x88\x01\x01\x12\x46\n\nconnection\x18\x02 \x01(\x0b\x32&.plugins.smtp.v1.Plugin.SmtpConnectionR\nconnection\x12\x12\n\x04\x66rom\x18\x03 \x01(\tR\x04\x66rom\x12\x19\n\x08reply_to\x18\x04 \x01(\tR\x07replyTo\x12\x0e\n\x02to\x18\x05 \x01(\tR\x02to\x12\x0e\n\x02\x63\x63\x18\x06 \x01(\tR\x02\x63\x63\x12\x10\n\x03\x62\x63\x63\x18\x07 \x01(\tR\x03\x62\x63\x63\x12\x18\n\x07subject\x18\x08 \x01(\tR\x07subject\x12\x12\n\x04\x62ody\x18\t \x01(\tR\x04\x62ody\x12 \n\x0b\x61ttachments\x18\n \x01(\tR\x0b\x61ttachments\x12z\n\x1e\x64ynamic_workflow_configuration\x18\x0b \x01(\x0b\x32/.plugins.common.v1.DynamicWorkflowConfigurationH\x01R\x1c\x64ynamicWorkflowConfiguration\x88\x01\x01\x1a\x98\x01\n\x0eSmtpConnection\x12\x12\n\x04host\x18\x01 \x01(\tR\x04host\x12\x12\n\x04port\x18\x02 \x01(\x05R\x04port\x12\x1a\n\x08username\x18\x03 \x01(\tR\x08username\x12\x1a\n\x08password\x18\x04 \x01(\tR\x08password\x12\x1b\n\x06secure\x18\x05 \x01(\x08H\x00R\x06secure\x88\x01\x01\x42\t\n\x07_secureB\x07\n\x05_nameB!\n\x1f_dynamic_workflow_configurationB9Z7github.com/superblocksteam/types/gen/go/plugins/smtp/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.smtp.v1.plugin_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/snowflake/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/snowflake/v1/plugin_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/workflow/v1/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/workflow/v1/plugin_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from common.v1 import plugin_pb2 as common_dot_v1_dot_plugin__pb2
+from superblocks_types.common.v1 import plugin_pb2 as common_dot_v1_dot_plugin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n plugins/workflow/v1/plugin.proto\x12\x13plugins.workflow.v1\x1a\x16\x63ommon/v1/plugin.proto\"/\n\x05Tuple\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\"\xac\x03\n\x06Plugin\x12\x1a\n\x08workflow\x18\x01 \x01(\tR\x08workflow\x12?\n\x06\x63ustom\x18\x02 \x03(\x0b\x32\'.plugins.workflow.v1.Plugin.CustomEntryR\x06\x63ustom\x12N\n\x0bqueryParams\x18\x03 \x03(\x0b\x32,.plugins.workflow.v1.Plugin.QueryParamsEntryR\x0bqueryParams\x12P\n\x13superblocksMetadata\x18\x0c \x01(\x0b\x32\x1e.common.v1.SuperblocksMetadataR\x13superblocksMetadata\x1aN\n\x0b\x43ustomEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x13.common.v1.PropertyR\x05value:\x02\x38\x01\x1aS\n\x10QueryParamsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12)\n\x05value\x18\x02 \x01(\x0b\x32\x13.common.v1.PropertyR\x05value:\x02\x38\x01\x42=Z;github.com/superblocksteam/types/gen/go/plugins/workflow/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.workflow.v1.plugin_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/plugins/workflow/v2/plugin_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/plugins/workflow/v2/plugin_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from common.v1 import plugin_pb2 as common_dot_v1_dot_plugin__pb2
+from superblocks_types.common.v1 import plugin_pb2 as common_dot_v1_dot_plugin__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n plugins/workflow/v2/plugin.proto\x12\x13plugins.workflow.v2\x1a\x16\x63ommon/v1/plugin.proto\"S\n\x06Plugin\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x39\n\nparameters\x18\x02 \x01(\x0b\x32\x19.common.v1.HttpParametersR\nparametersB=Z;github.com/superblocksteam/types/gen/go/plugins/workflow/v2b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'plugins.workflow.v2.plugin_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/protoc_gen_openapiv2/options/annotations_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/protoc_gen_openapiv2/options/annotations_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
-from protoc_gen_openapiv2.options import openapiv2_pb2 as protoc__gen__openapiv2_dot_options_dot_openapiv2__pb2
+from superblocks_types.protoc_gen_openapiv2.options import openapiv2_pb2 as protoc__gen__openapiv2_dot_options_dot_openapiv2__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n.protoc-gen-openapiv2/options/annotations.proto\x12)grpc.gateway.protoc_gen_openapiv2.options\x1a google/protobuf/descriptor.proto\x1a,protoc-gen-openapiv2/options/openapiv2.proto:~\n\x11openapiv2_swagger\x12\x1c.google.protobuf.FileOptions\x18\x92\x08 \x01(\x0b\x32\x32.grpc.gateway.protoc_gen_openapiv2.options.SwaggerR\x10openapiv2Swagger:\x86\x01\n\x13openapiv2_operation\x12\x1e.google.protobuf.MethodOptions\x18\x92\x08 \x01(\x0b\x32\x34.grpc.gateway.protoc_gen_openapiv2.options.OperationR\x12openapiv2Operation:~\n\x10openapiv2_schema\x12\x1f.google.protobuf.MessageOptions\x18\x92\x08 \x01(\x0b\x32\x31.grpc.gateway.protoc_gen_openapiv2.options.SchemaR\x0fopenapiv2Schema:u\n\ropenapiv2_tag\x12\x1f.google.protobuf.ServiceOptions\x18\x92\x08 \x01(\x0b\x32..grpc.gateway.protoc_gen_openapiv2.options.TagR\x0copenapiv2Tag:~\n\x0fopenapiv2_field\x12\x1d.google.protobuf.FieldOptions\x18\x92\x08 \x01(\x0b\x32\x35.grpc.gateway.protoc_gen_openapiv2.options.JSONSchemaR\x0eopenapiv2FieldBHZFgithub.com/grpc-ecosystem/grpc-gateway/v2/protoc-gen-openapiv2/optionsb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'protoc_gen_openapiv2.options.annotations_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/protoc_gen_openapiv2/options/openapiv2_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/protoc_gen_openapiv2/options/openapiv2_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/secrets/v1/secrets_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/secrets/v1/secrets_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from common.v1 import common_pb2 as common_dot_v1_dot_common__pb2
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
-from plugins.common.v1 import auth_pb2 as plugins_dot_common_dot_v1_dot_auth__pb2
+from superblocks_types.common.v1 import common_pb2 as common_dot_v1_dot_common__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.plugins.common.v1 import auth_pb2 as plugins_dot_common_dot_v1_dot_auth__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18secrets/v1/secrets.proto\x12\nsecrets.v1\x1a\x16\x63ommon/v1/common.proto\x1a\x1b\x62uf/validate/validate.proto\x1a\x1cplugins/common/v1/auth.proto\"s\n\x11\x41wsSecretsManager\x12\x36\n\x04\x61uth\x18\x01 \x01(\x0b\x32\x1a.plugins.common.v1.AwsAuthB\x06\xbaH\x03\xc8\x01\x01R\x04\x61uth\x12\x1b\n\x06prefix\x18\x02 \x01(\tH\x00R\x06prefix\x88\x01\x01\x42\t\n\x07_prefix\"q\n\x10GcpSecretManager\x12\x36\n\x04\x61uth\x18\x01 \x01(\x0b\x32\x1a.plugins.common.v1.GcpAuthB\x06\xbaH\x03\xc8\x01\x01R\x04\x61uth\x12%\n\nproject_id\x18\x02 \x01(\tB\x06\xbaH\x03\xc8\x01\x01R\tprojectId\"\xbf\x04\n\x0eHashicorpVault\x12;\n\x04\x61uth\x18\x01 \x01(\x0b\x32\x1f.secrets.v1.HashicorpVault.AuthB\x06\xbaH\x03\xc8\x01\x01R\x04\x61uth\x12 \n\x07\x61\x64\x64ress\x18\x02 \x01(\tB\x06\xbaH\x03\xc8\x01\x01R\x07\x61\x64\x64ress\x12\x17\n\x04path\x18\x03 \x01(\tH\x00R\x04path\x88\x01\x01\x12!\n\tnamespace\x18\x04 \x01(\tH\x01R\tnamespace\x88\x01\x01\x12<\n\x07version\x18\x05 \x01(\x0e\x32\".secrets.v1.HashicorpVault.VersionR\x07version\x12&\n\x0csecrets_path\x18\x06 \x01(\tH\x02R\x0bsecretsPath\x88\x01\x01\x1a\xbf\x01\n\x04\x41uth\x12\x16\n\x05token\x18\x01 \x01(\tH\x00R\x05token\x12\x44\n\x08\x61pp_role\x18\x02 \x01(\x0b\x32\'.secrets.v1.HashicorpVault.Auth.AppRoleH\x00R\x07\x61ppRole\x1aO\n\x07\x41ppRole\x12\x1f\n\x07role_id\x18\x01 \x01(\tB\x06\xbaH\x03\xc8\x01\x01R\x06roleId\x12#\n\tsecret_id\x18\x02 \x01(\tB\x06\xbaH\x03\xc8\x01\x01R\x08secretIdB\x08\n\x06\x63onfig\"B\n\x07Version\x12\x17\n\x13VERSION_UNSPECIFIED\x10\x00\x12\x0e\n\nVERSION_V1\x10\x01\x12\x0e\n\nVERSION_V2\x10\x02\x42\x07\n\x05_pathB\x0c\n\n_namespaceB\x0f\n\r_secrets_path\"y\n\tMockStore\x12\x33\n\x04\x64\x61ta\x18\x01 \x03(\x0b\x32\x1f.secrets.v1.MockStore.DataEntryR\x04\x64\x61ta\x1a\x37\n\tDataEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xa7\x02\n\x08Provider\x12+\n\x04mock\x18\x01 \x01(\x0b\x32\x15.secrets.v1.MockStoreH\x00R\x04mock\x12O\n\x13\x61ws_secrets_manager\x18\x02 \x01(\x0b\x32\x1d.secrets.v1.AwsSecretsManagerH\x00R\x11\x61wsSecretsManager\x12L\n\x12gcp_secret_manager\x18\x03 \x01(\x0b\x32\x1c.secrets.v1.GcpSecretManagerH\x00R\x10gcpSecretManager\x12\x45\n\x0fhashicorp_vault\x18\x04 \x01(\x0b\x32\x1a.secrets.v1.HashicorpVaultH\x00R\x0ehashicorpVaultB\x08\n\x06\x63onfig\"\xe2\x01\n\x05Store\x12\x37\n\x08metadata\x18\x01 \x01(\x0b\x32\x13.common.v1.MetadataB\x06\xbaH\x03\xc8\x01\x01R\x08metadata\x12\x38\n\x08provider\x18\x02 \x01(\x0b\x32\x14.secrets.v1.ProviderB\x06\xbaH\x03\xc8\x01\x01R\x08provider\x12\x15\n\x03ttl\x18\x03 \x01(\x05H\x00R\x03ttl\x88\x01\x01\x12\x31\n\x10\x63onfiguration_id\x18\x04 \x01(\tB\x06\xbaH\x03\xc8\x01\x01R\x0f\x63onfigurationId\x12\x14\n\x05\x63\x61\x63he\x18\x05 \x01(\x08R\x05\x63\x61\x63heB\x06\n\x04_ttl\"3\n\x07\x44\x65tails\x12\x14\n\x05\x61lias\x18\x01 \x01(\tR\x05\x61lias\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\"e\n\x0cInvalidation\x12\x14\n\x05\x61lias\x18\x01 \x01(\tR\x05\x61lias\x12)\n\x10\x63onfiguration_id\x18\x02 \x01(\tR\x0f\x63onfigurationId\x12\x14\n\x05store\x18\x03 \x01(\tR\x05storeB4Z2github.com/superblocksteam/types/gen/go/secrets/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'secrets.v1.secrets_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/secrets/v1/store_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/secrets/v1/store_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from common.v1 import errors_pb2 as common_dot_v1_dot_errors__pb2
-from common.v1 import common_pb2 as common_dot_v1_dot_common__pb2
-from secrets.v1 import secrets_pb2 as secrets_dot_v1_dot_secrets__pb2
-from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.common.v1 import errors_pb2 as common_dot_v1_dot_errors__pb2
+from superblocks_types.common.v1 import common_pb2 as common_dot_v1_dot_common__pb2
+from superblocks_types.secrets.v1 import secrets_pb2 as secrets_dot_v1_dot_secrets__pb2
+from superblocks_types.google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16secrets/v1/store.proto\x12\nsecrets.v1\x1a\x16\x63ommon/v1/errors.proto\x1a\x16\x63ommon/v1/common.proto\x1a\x18secrets/v1/secrets.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1b\x62uf/validate/validate.proto\"u\n\x11InvalidateRequest\x12\x1d\n\x05store\x18\x01 \x01(\tB\x07\xbaH\x04r\x02\x10\x01R\x05store\x12\x16\n\x06secret\x18\x02 \x01(\tR\x06secret\x12)\n\x10\x63onfiguration_id\x18\x03 \x01(\tR\x0f\x63onfigurationId\"\x98\x01\n\x12InvalidateResponse\x12(\n\x06\x65rrors\x18\x01 \x03(\x0b\x32\x10.common.v1.ErrorR\x06\x65rrors\x12>\n\rinvalidations\x18\x02 \x03(\x0b\x32\x18.secrets.v1.InvalidationR\rinvalidations\x12\x18\n\x07message\x18\x03 \x01(\tR\x07message\"\xad\x01\n\x12ListSecretsRequest\x12\x1d\n\x05store\x18\x01 \x01(\tB\x07\xbaH\x04r\x02\x10\x01R\x05store\x12\x34\n\x07profile\x18\x02 \x01(\x0b\x32\x12.common.v1.ProfileB\x06\xbaH\x03\xc8\x01\x01R\x07profile\x12\x35\n\x08provider\x18\x03 \x01(\x0b\x32\x14.secrets.v1.ProviderH\x00R\x08provider\x88\x01\x01\x42\x0b\n\t_provider\"D\n\x13ListSecretsResponse\x12-\n\x07secrets\x18\x01 \x03(\x0b\x32\x13.secrets.v1.DetailsR\x07secrets2\xcd\x03\n\x0cStoreService\x12\xa6\x02\n\nInvalidate\x12\x1d.secrets.v1.InvalidateRequest\x1a\x1e.secrets.v1.InvalidateResponse\"\xd8\x01\x82\xd3\xe4\x93\x02\xd1\x01\"%/v1/secrets/stores/{store}/invalidate:\x01*ZI\"G/v1/secrets/stores/{store}/configurations/{configuration_id}/invalidateZZ\"X/v1/secrets/stores/{store}/configurations/{configuration_id}/secrets/{secret}/invalidate\x12\x93\x01\n\x0bListSecrets\x12\x1e.secrets.v1.ListSecretsRequest\x1a\x1f.secrets.v1.ListSecretsResponse\"C\x82\xd3\xe4\x93\x02=\x12\x1a/v1/secrets/stores/{store}Z\x1f\"\x1a/v1/secrets/stores/{store}:\x01*B4Z2github.com/superblocksteam/types/gen/go/secrets/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'secrets.v1.store_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/secrets/v1/store_pb2_grpc.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/secrets/v1/store_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from secrets.v1 import store_pb2 as secrets_dot_v1_dot_store__pb2
+from superblocks_types.secrets.v1 import store_pb2 as secrets_dot_v1_dot_store__pb2
 
 
 class StoreServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/security/v1/requests_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/security/v1/requests_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from security.v1 import service_pb2 as security_dot_v1_dot_service__pb2
+from superblocks_types.security.v1 import service_pb2 as security_dot_v1_dot_service__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1asecurity/v1/requests.proto\x12\x0bsecurity.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x19security/v1/service.proto\"O\n\x18ResourcesToResignRequest\x12\x1d\n\nclaimed_by\x18\x01 \x01(\tR\tclaimedBy\x12\x14\n\x05limit\x18\x02 \x01(\x05R\x05limit\"P\n\x19ResourcesToResignResponse\x12\x33\n\tresources\x18\x01 \x03(\x0b\x32\x15.security.v1.ResourceR\tresources\"\xfb\x02\n\x0bKeyRotation\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x36\n\x06status\x18\x02 \x01(\x0e\x32\x1e.security.v1.KeyRotationStatusR\x06status\x12/\n\x13resources_completed\x18\x03 \x01(\x05R\x12resourcesCompleted\x12\'\n\x0fresources_total\x18\x04 \x01(\x05R\x0eresourcesTotal\x12$\n\x0esigning_key_id\x18\x05 \x01(\tR\x0csigningKeyId\x12\x34\n\x07\x63reated\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12\x34\n\x07updated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07updated\x12\x38\n\tcompleted\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcompleted\"U\n\x14KeyRotationsResponse\x12=\n\rkey_rotations\x18\x01 \x03(\x0b\x32\x18.security.v1.KeyRotationR\x0ckeyRotations*\xc2\x01\n\x11KeyRotationStatus\x12#\n\x1fKEY_ROTATION_STATUS_UNSPECIFIED\x10\x00\x12#\n\x1fKEY_ROTATION_STATUS_IN_PROGRESS\x10\x01\x12!\n\x1dKEY_ROTATION_STATUS_COMPLETED\x10\x02\x12\x1e\n\x1aKEY_ROTATION_STATUS_FAILED\x10\x03\x12 \n\x1cKEY_ROTATION_STATUS_CANCELED\x10\x04\x42\x35Z3github.com/superblocksteam/types/gen/go/security/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'security.v1.requests_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/security/v1/service_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/security/v1/service_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from api.v1 import api_pb2 as api_dot_v1_dot_api__pb2
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
-from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from superblocks_types.api.v1 import api_pb2 as api_dot_v1_dot_api__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from utils.v1 import utils_pb2 as utils_dot_v1_dot_utils__pb2
+from superblocks_types.utils.v1 import utils_pb2 as utils_dot_v1_dot_utils__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19security/v1/service.proto\x12\x0bsecurity.v1\x1a\x10\x61pi/v1/api.proto\x1a\x1b\x62uf/validate/validate.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x14utils/v1/utils.proto\"\x89\x04\n\x08Resource\x12\x1f\n\x03\x61pi\x18\x01 \x01(\x0b\x32\x0b.api.v1.ApiH\x00R\x03\x61pi\x12\x39\n\x07literal\x18\x02 \x01(\x0b\x32\x1d.security.v1.Resource.LiteralH\x00R\x07literal\x12\x1d\n\tcommit_id\x18\x03 \x01(\tH\x01R\x08\x63ommitId\x12!\n\x0b\x62ranch_name\x18\x04 \x01(\tH\x01R\nbranchName\x1a\xbb\x02\n\x07Literal\x12*\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x16.google.protobuf.ValueR\x04\x64\x61ta\x12\x36\n\tsignature\x18\x02 \x01(\x0b\x32\x13.utils.v1.SignatureH\x00R\tsignature\x88\x01\x01\x12\x1f\n\x0bresource_id\x18\x03 \x01(\tR\nresourceId\x12\'\n\x0forganization_id\x18\x04 \x01(\tR\x0eorganizationId\x12=\n\x0clast_updated\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0blastUpdated\x12\x12\n\x04type\x18\x06 \x01(\tR\x04type\x12!\n\x0cpage_version\x18\x07 \x01(\x05R\x0bpageVersionB\x0c\n\n_signatureB\x0f\n\x06\x63onfig\x12\x05\xbaH\x02\x08\x01\x42\x10\n\x07git_ref\x12\x05\xbaH\x02\x08\x01\"@\n\x0bSignRequest\x12\x31\n\x08resource\x18\x01 \x01(\x0b\x32\x15.security.v1.ResourceR\x08resource\"A\n\x0cSignResponse\x12\x31\n\tsignature\x18\x01 \x01(\x0b\x32\x13.utils.v1.SignatureR\tsignature\"D\n\rVerifyRequest\x12\x33\n\tresources\x18\x01 \x03(\x0b\x32\x15.security.v1.ResourceR\tresources\"\'\n\x0eVerifyResponse\x12\x15\n\x06key_id\x18\x01 \x01(\tR\x05keyId2\xd2\x01\n\x10SignatureService\x12Z\n\x04Sign\x12\x18.security.v1.SignRequest\x1a\x19.security.v1.SignResponse\"\x1d\x82\xd3\xe4\x93\x02\x17\"\x12/v1/signature/sign:\x01*\x12\x62\n\x06Verify\x12\x1a.security.v1.VerifyRequest\x1a\x1b.security.v1.VerifyResponse\"\x1f\x82\xd3\xe4\x93\x02\x19\"\x14/v1/signature/verify:\x01*B5Z3github.com/superblocksteam/types/gen/go/security/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'security.v1.service_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/security/v1/service_pb2_grpc.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/security/v1/service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from security.v1 import service_pb2 as security_dot_v1_dot_service__pb2
+from superblocks_types.security.v1 import service_pb2 as security_dot_v1_dot_service__pb2
 
 
 class SignatureServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/store/v1/service_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/store/v1/service_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from common.v1 import errors_pb2 as common_dot_v1_dot_errors__pb2
-from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from superblocks_types.common.v1 import errors_pb2 as common_dot_v1_dot_errors__pb2
+from superblocks_types.google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
-from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-from store.v1 import store_pb2 as store_dot_v1_dot_store__pb2
+from superblocks_types.protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
+from superblocks_types.store.v1 import store_pb2 as store_dot_v1_dot_store__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16store/v1/service.proto\x12\x08store.v1\x1a\x16\x63ommon/v1/errors.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x14store/v1/store.proto\"!\n\x0bReadRequest\x12\x12\n\x04keys\x18\x01 \x03(\tR\x04keys\"h\n\x0cReadResponse\x12\x30\n\x07results\x18\x01 \x03(\x0b\x32\x16.google.protobuf.ValueR\x07results\x12&\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x10.common.v1.ErrorR\x05\x65rror\"4\n\x0cWriteRequest\x12$\n\x05pairs\x18\x01 \x03(\x0b\x32\x0e.store.v1.PairR\x05pairs\"]\n\rWriteResponse\x12$\n\x05pairs\x18\x01 \x03(\x0b\x32\x0e.store.v1.PairR\x05pairs\x12&\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x10.common.v1.ErrorR\x05\x65rror2\xbd\x01\n\x0cStoreService\x12S\n\x04Read\x12\x15.store.v1.ReadRequest\x1a\x16.store.v1.ReadResponse\"\x1c\x92\x41\x06*\x04Read\x82\xd3\xe4\x93\x02\r\"\x08/v1/read:\x01*\x12X\n\x05Write\x12\x16.store.v1.WriteRequest\x1a\x17.store.v1.WriteResponse\"\x1e\x92\x41\x07*\x05Write\x82\xd3\xe4\x93\x02\x0e\"\t/v1/write:\x01*BvZ0github.com/superblocksteam/types/gen/go/store/v1\x92\x41\x41\x12\x18\n\x11Superblocks Store2\x03\x31.0*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'store.v1.service_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/store/v1/service_pb2_grpc.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/store/v1/service_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from store.v1 import service_pb2 as store_dot_v1_dot_service__pb2
+from superblocks_types.store.v1 import service_pb2 as store_dot_v1_dot_service__pb2
 
 
 class StoreServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/store/v1/store_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/store/v1/store_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
-from secrets.v1 import secrets_pb2 as secrets_dot_v1_dot_secrets__pb2
+from superblocks_types.secrets.v1 import secrets_pb2 as secrets_dot_v1_dot_secrets__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x14store/v1/store.proto\x12\x08store.v1\x1a\x1cgoogle/protobuf/struct.proto\x1a\x18secrets/v1/secrets.proto\"F\n\x04Pair\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.ValueR\x05value\"5\n\x06Stores\x12+\n\x07secrets\x18\x01 \x03(\x0b\x32\x11.secrets.v1.StoreR\x07secretsB2Z0github.com/superblocksteam/types/gen/go/store/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'store.v1.store_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/superblocks/v1/options_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/superblocks/v1/options_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/syncer/v1/service_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/syncer/v1/service_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from common.v1 import errors_pb2 as common_dot_v1_dot_errors__pb2
-from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
+from superblocks_types.common.v1 import errors_pb2 as common_dot_v1_dot_errors__pb2
+from superblocks_types.google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
-from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
-from syncer.v1 import syncer_pb2 as syncer_dot_v1_dot_syncer__pb2
-from validate import validate_pb2 as validate_dot_validate__pb2
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
-from event.v1 import service_pb2 as event_dot_v1_dot_service__pb2
+from superblocks_types.protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
+from superblocks_types.syncer.v1 import syncer_pb2 as syncer_dot_v1_dot_syncer__pb2
+from superblocks_types.validate import validate_pb2 as validate_dot_validate__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.event.v1 import service_pb2 as event_dot_v1_dot_service__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17syncer/v1/service.proto\x12\tsyncer.v1\x1a\x16\x63ommon/v1/errors.proto\x1a\x1cgoogle/api/annotations.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\x1a\x16syncer/v1/syncer.proto\x1a\x17validate/validate.proto\x1a\x1b\x62uf/validate/validate.proto\x1a\x16\x65vent/v1/service.proto\"H\n\x1fGetConfigurationMetadataRequest\x12%\n\x0eintegration_id\x18\x01 \x01(\tR\rintegrationId\"\x8c\x03\n GetConfigurationMetadataResponse\x12%\n\x0eintegration_id\x18\x01 \x01(\tR\rintegrationId\x12g\n\x0e\x63onfigurations\x18\x02 \x03(\x0b\x32?.syncer.v1.GetConfigurationMetadataResponse.ConfigurationsEntryR\x0e\x63onfigurations\x12)\n\x10integration_type\x18\x03 \x01(\tR\x0fintegrationType\x12\'\n\x0forganization_id\x18\x04 \x01(\tR\x0eorganizationId\x12(\n\x06\x65rrors\x18\x05 \x03(\x0b\x32\x10.common.v1.ErrorR\x06\x65rrors\x1aZ\n\x13\x43onfigurationsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x17.google.protobuf.StructR\x05value:\x02\x38\x01\"6\n\x0bSyncRequest\x12\'\n\x0fintegration_ids\x18\x01 \x03(\tR\x0eintegrationIds\"\xc1\x02\n\x0cSyncResponse\x12`\n\x13integrations_synced\x18\x01 \x03(\x0b\x32/.syncer.v1.SyncResponse.IntegrationsSyncedEntryR\x12integrationsSynced\x12(\n\x06\x65rrors\x18\x02 \x03(\x0b\x32\x10.common.v1.ErrorR\x06\x65rrors\x1a\x39\n\x0bIntegration\x12*\n\x10\x63onfigurationIds\x18\x01 \x03(\tR\x10\x63onfigurationIds\x1aj\n\x17IntegrationsSyncedEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x39\n\x05value\x18\x02 \x01(\x0b\x32#.syncer.v1.SyncResponse.IntegrationR\x05value:\x02\x38\x01\"Z\n\x15UpsertMetadataRequest\x12\x41\n\x08metadata\x18\x01 \x03(\x0b\x32\x13.syncer.v1.MetadataB\x10\xfa\x42\x05\x92\x01\x02\x08\x01\xbaH\x05\x92\x01\x02\x08\x01R\x08metadata\"B\n\x16UpsertMetadataResponse\x12(\n\x06\x65rrors\x18\x01 \x03(\x0b\x32\x10.common.v1.ErrorR\x06\x65rrors\"k\n\x15\x44\x65leteMetadataRequest\x12%\n\x0eintegration_id\x18\x01 \x01(\tR\rintegrationId\x12+\n\x11\x63onfiguration_ids\x18\x02 \x03(\tR\x10\x63onfigurationIds\"B\n\x16\x44\x65leteMetadataResponse\x12(\n\x06\x65rrors\x18\x01 \x03(\x0b\x32\x10.common.v1.ErrorR\x06\x65rrors2\xc6\x03\n\rIntakeService\x12\xa4\x01\n\x0eUpsertMetadata\x12 .syncer.v1.UpsertMetadataRequest\x1a!.syncer.v1.UpsertMetadataResponse\"M\x92\x41\x11*\x0fUpsert Metadata\x82\xd3\xe4\x93\x02\x33\"\x10/api/v1/metadata:\x01*Z\x1c\"\x17/api/v1/syncer/metadata:\x01*\x12\x94\x01\n\x0e\x44\x65leteMetadata\x12 .syncer.v1.DeleteMetadataRequest\x1a!.syncer.v1.DeleteMetadataResponse\"=\x92\x41\x11*\x0f\x44\x65lete Metadata\x82\xd3\xe4\x93\x02#*!/api/v1/metadata/{integration_id}\x12w\n\x0bIngestEvent\x12\x1c.event.v1.IngestEventRequest\x1a\x1d.event.v1.IngestEventResponse\"+\x92\x41\x0f*\rIngest Events\x82\xd3\xe4\x93\x02\x13\"\x0e/api/v1/events:\x01*2\xa3\x01\n\rSyncerService\x12\x91\x01\n\x04Sync\x12\x16.syncer.v1.SyncRequest\x1a\x17.syncer.v1.SyncResponse\"X\x92\x41\x36*4Sync metadata for integrations manually by their IDs\x82\xd3\xe4\x93\x02\x19\"\x14/api/v1/integrations:\x01*2\xef\x01\n\x12IntegrationService\x12\xd8\x01\n\x18GetConfigurationMetadata\x12*.syncer.v1.GetConfigurationMetadataRequest\x1a+.syncer.v1.GetConfigurationMetadataResponse\"c\x92\x41(*&Get integration configuration metadata\x82\xd3\xe4\x93\x02\x32\x12\x30/api/v1/integrations/{integration_id=*}/metadataB\x80\x01Z1github.com/superblocksteam/types/gen/go/syncer/v1\x92\x41J\x12!\n\x1aSuperblocks Syncer Service2\x03\x31.0*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'syncer.v1.service_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/syncer/v1/service_pb2_grpc.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/syncer/v1/service_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from event.v1 import service_pb2 as event_dot_v1_dot_service__pb2
-from syncer.v1 import service_pb2 as syncer_dot_v1_dot_service__pb2
+from superblocks_types.event.v1 import service_pb2 as event_dot_v1_dot_service__pb2
+from superblocks_types.syncer.v1 import service_pb2 as syncer_dot_v1_dot_service__pb2
 
 
 class IntakeServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/syncer/v1/syncer_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/syncer/v1/syncer_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from ai.v1 import metadata_pb2 as ai_dot_v1_dot_metadata__pb2
+from superblocks_types.ai.v1 import metadata_pb2 as ai_dot_v1_dot_metadata__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
-from validate import validate_pb2 as validate_dot_validate__pb2
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.validate import validate_pb2 as validate_dot_validate__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16syncer/v1/syncer.proto\x12\tsyncer.v1\x1a\x14\x61i/v1/metadata.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17validate/validate.proto\x1a\x1b\x62uf/validate/validate.proto\"\x82\x03\n\x08Metadata\x12\x39\n\x10\x63onfiguration_id\x18\x01 \x01(\tB\x0e\xfa\x42\x04r\x02\x10\x01\xbaH\x04r\x02\x10\x01R\x0f\x63onfigurationId\x12\x35\n\x0eintegration_id\x18\x02 \x01(\tB\x0e\xfa\x42\x04r\x02\x10\x01\xbaH\x04r\x02\x10\x01R\rintegrationId\x12\x42\n\x0craw_metadata\x18\x03 \x01(\x0b\x32\x0f.ai.v1.MetadataB\x0e\xfa\x42\x05\x8a\x01\x02\x10\x01\xbaH\x03\xc8\x01\x01R\x0brawMetadata\x12L\n\x14updated_datetime_utc\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x12updatedDatetimeUtc\x12\x39\n\x10integration_type\x18\x05 \x01(\tB\x0e\xfa\x42\x04r\x02\x10\x01\xbaH\x04r\x02\x10\x01R\x0fintegrationType\x12\x37\n\x0forganization_id\x18\x06 \x01(\tB\x0e\xfa\x42\x04r\x02\x10\x01\xbaH\x04r\x02\x10\x01R\x0eorganizationIdB3Z1github.com/superblocksteam/types/gen/go/syncer/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'syncer.v1.syncer_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/transport/v1/transport_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/transport/v1/transport_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from api.v1 import api_pb2 as api_dot_v1_dot_api__pb2
-from api.v1 import blocks_pb2 as api_dot_v1_dot_blocks__pb2
-from api.v1 import service_pb2 as api_dot_v1_dot_service__pb2
-from common.v1 import errors_pb2 as common_dot_v1_dot_errors__pb2
+from superblocks_types.api.v1 import api_pb2 as api_dot_v1_dot_api__pb2
+from superblocks_types.api.v1 import blocks_pb2 as api_dot_v1_dot_blocks__pb2
+from superblocks_types.api.v1 import service_pb2 as api_dot_v1_dot_service__pb2
+from superblocks_types.common.v1 import errors_pb2 as common_dot_v1_dot_errors__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
-from plugins.kafka.v1 import plugin_pb2 as plugins_dot_kafka_dot_v1_dot_plugin__pb2
-from plugins.cosmosdb.v1 import plugin_pb2 as plugins_dot_cosmosdb_dot_v1_dot_plugin__pb2
-from plugins.adls.v1 import plugin_pb2 as plugins_dot_adls_dot_v1_dot_plugin__pb2
-from validate import validate_pb2 as validate_dot_validate__pb2
-from buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
-from store.v1 import store_pb2 as store_dot_v1_dot_store__pb2
+from superblocks_types.plugins.kafka.v1 import plugin_pb2 as plugins_dot_kafka_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.cosmosdb.v1 import plugin_pb2 as plugins_dot_cosmosdb_dot_v1_dot_plugin__pb2
+from superblocks_types.plugins.adls.v1 import plugin_pb2 as plugins_dot_adls_dot_v1_dot_plugin__pb2
+from superblocks_types.validate import validate_pb2 as validate_dot_validate__pb2
+from superblocks_types.buf.validate import validate_pb2 as buf_dot_validate_dot_validate__pb2
+from superblocks_types.store.v1 import store_pb2 as store_dot_v1_dot_store__pb2
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1ctransport/v1/transport.proto\x12\x0ctransport.v1\x1a\x10\x61pi/v1/api.proto\x1a\x13\x61pi/v1/blocks.proto\x1a\x14\x61pi/v1/service.proto\x1a\x16\x63ommon/v1/errors.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1dplugins/kafka/v1/plugin.proto\x1a plugins/cosmosdb/v1/plugin.proto\x1a\x1cplugins/adls/v1/plugin.proto\x1a\x17validate/validate.proto\x1a\x1b\x62uf/validate/validate.proto\x1a\x14store/v1/store.proto\x1a\x19google/protobuf/any.proto\"\xdc\x04\n\x0bPerformance\x12\x14\n\x05\x65rror\x18\x01 \x01(\x08R\x05\x65rror\x12O\n\x10plugin_execution\x18\x02 \x01(\x0b\x32$.transport.v1.Performance.ObservableR\x0fpluginExecution\x12I\n\rqueue_request\x18\x03 \x01(\x0b\x32$.transport.v1.Performance.ObservableR\x0cqueueRequest\x12K\n\x0equeue_response\x18\x04 \x01(\x0b\x32$.transport.v1.Performance.ObservableR\rqueueResponse\x12J\n\x0ekv_store_fetch\x18\x05 \x01(\x0b\x32$.transport.v1.Performance.ObservableR\x0ckvStoreFetch\x12H\n\rkv_store_push\x18\x06 \x01(\x0b\x32$.transport.v1.Performance.ObservableR\x0bkvStorePush\x12:\n\x05total\x18\x07 \x01(\x0b\x32$.transport.v1.Performance.ObservableR\x05total\x1a|\n\nObservable\x12\x14\n\x05start\x18\x01 \x01(\x01R\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\x01R\x03\x65nd\x12\x14\n\x05value\x18\x03 \x01(\x01R\x05value\x12\x14\n\x05\x62ytes\x18\x04 \x01(\x01R\x05\x62ytes\x12\x1a\n\x08\x65stimate\x18\x05 \x01(\x01R\x08\x65stimate\"t\n\x08Variable\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12*\n\x04type\x18\x02 \x01(\x0e\x32\x16.api.v1.Variables.TypeR\x04type\x12*\n\x04mode\x18\x03 \x01(\x0e\x32\x16.api.v1.Variables.ModeR\x04mode\"\xe4\x01\n\rObservability\x12\x19\n\x08trace_id\x18\x01 \x01(\tR\x07traceId\x12\x17\n\x07span_id\x18\x02 \x01(\tR\x06spanId\x12\x42\n\x07\x62\x61ggage\x18\x03 \x03(\x0b\x32(.transport.v1.Observability.BaggageEntryR\x07\x62\x61ggage\x12\x1f\n\x0btrace_flags\x18\x04 \x01(\x0cR\ntraceFlags\x1a:\n\x0c\x42\x61ggageEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\x96\x0f\n\x07Request\x12\x14\n\x05inbox\x18\x01 \x01(\tR\x05inbox\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.transport.v1.Request.DataR\x04\x64\x61ta\x12\x14\n\x05topic\x18\x03 \x01(\tR\x05topic\x1a\xae\x0e\n\x04\x44\x61ta\x12\x39\n\x06pinned\x18\x01 \x01(\x0b\x32!.transport.v1.Request.Data.PinnedR\x06pinned\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.transport.v1.Request.Data.DataR\x04\x64\x61ta\x1a\xb1\x02\n\x06Pinned\x12\x16\n\x06\x62ucket\x18\x01 \x01(\tR\x06\x62ucket\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12\x18\n\x07version\x18\x03 \x01(\tR\x07version\x12\x14\n\x05\x65vent\x18\x04 \x01(\tR\x05\x65vent\x12L\n\x07\x63\x61rrier\x18\x05 \x03(\x0b\x32..transport.v1.Request.Data.Pinned.CarrierEntryB\x02\x18\x01R\x07\x63\x61rrier\x12\x41\n\robservability\x18\x06 \x01(\x0b\x32\x1b.transport.v1.ObservabilityR\robservability\x1a:\n\x0c\x43\x61rrierEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\x1a\x81\x0b\n\x04\x44\x61ta\x12;\n\x05props\x18\x01 \x01(\x0b\x32%.transport.v1.Request.Data.Data.PropsR\x05props\x12\x37\n\x08\x64_config\x18\x02 \x01(\x0b\x32\x17.google.protobuf.StructH\x00R\x07\x64\x43onfig\x88\x01\x01\x12\x37\n\x08\x61_config\x18\x03 \x01(\x0b\x32\x17.google.protobuf.StructH\x01R\x07\x61\x43onfig\x88\x01\x01\x12=\n\x06quotas\x18\x04 \x01(\x0b\x32%.transport.v1.Request.Data.Data.QuotaR\x06quotas\x1a\xb7\x08\n\x05Props\x12J\n\x14\x61\x63tion_configuration\x18\x01 \x01(\x0b\x32\x17.google.protobuf.StructR\x13\x61\x63tionConfiguration\x12R\n\x18\x64\x61tasource_configuration\x18\x02 \x01(\x0b\x32\x17.google.protobuf.StructR\x17\x64\x61tasourceConfiguration\x12\x63\n!redacted_datasource_configuration\x18\x03 \x01(\x0b\x32\x17.google.protobuf.StructR\x1fredactedDatasourceConfiguration\x12!\n\x0c\x65xecution_id\x18\x04 \x01(\tR\x0b\x65xecutionId\x12\x1b\n\tstep_name\x18\x05 \x01(\tR\x08stepName\x12 \n\x0b\x65nvironment\x18\x06 \x01(\tR\x0b\x65nvironment\x12P\n\x0c\x62inding_keys\x18\x07 \x03(\x0b\x32-.transport.v1.Request.Data.Data.Props.BindingR\x0b\x62indingKeys\x12R\n\tvariables\x18\x08 \x03(\x0b\x32\x34.transport.v1.Request.Data.Data.Props.VariablesEntryR\tvariables\x12%\n\rfileServerUrl\x18\t \x01(\tR\x0e$fileServerUrl\x12@\n\x05\x66iles\x18\n \x03(\x0b\x32*.transport.v1.Request.Data.Data.Props.FileR\x05\x66iles\x12\x16\n\x06render\x18\x0b \x01(\x08R\x06render\x12\x18\n\x07version\x18\x0c \x01(\tR\x07version\x1a/\n\x07\x42inding\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x12\n\x04type\x18\x02 \x01(\tR\x04type\x1a\xfe\x01\n\x04\x46ile\x12\x1c\n\tfieldname\x18\x01 \x01(\tR\tfieldname\x12\"\n\x0coriginalname\x18\x02 \x01(\tR\x0coriginalname\x12\x1a\n\x08\x65ncoding\x18\x03 \x01(\tR\x08\x65ncoding\x12\x1a\n\x08mimetype\x18\x04 \x01(\tR\x08mimetype\x12\x12\n\x04size\x18\x05 \x01(\x03R\x04size\x12 \n\x0b\x64\x65stination\x18\x06 \x01(\tR\x0b\x64\x65stination\x12\x1a\n\x08\x66ilename\x18\x07 \x01(\tR\x08\x66ilename\x12\x12\n\x04path\x18\x08 \x01(\tR\x04path\x12\x16\n\x06\x62uffer\x18\t \x01(\x0cR\x06\x62uffer\x1aT\n\x0eVariablesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12,\n\x05value\x18\x02 \x01(\x0b\x32\x16.transport.v1.VariableR\x05value:\x02\x38\x01\x1a\x37\n\x05Quota\x12\x12\n\x04size\x18\x01 \x01(\x05R\x04size\x12\x1a\n\x08\x64uration\x18\x02 \x01(\x05R\x08\x64urationB\x0b\n\t_d_configB\x0b\n\t_a_config\"\xb1\x06\n\x08Response\x12/\n\x04\x64\x61ta\x18\x01 \x01(\x0b\x32\x1b.transport.v1.Response.DataR\x04\x64\x61ta\x12(\n\x06pinned\x18\x02 \x01(\x0b\x32\x10.common.v1.ErrorR\x06pinned\x1a\xc9\x05\n\x04\x44\x61ta\x12\x31\n\x06pinned\x18\x01 \x01(\x0b\x32\x19.transport.v1.PerformanceR\x06pinned\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .transport.v1.Response.Data.DataR\x04\x64\x61ta\x1a\xd7\x04\n\x04\x44\x61ta\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\"\n\x03\x65rr\x18\x02 \x01(\x0b\x32\x10.common.v1.ErrorR\x03\x65rr\x12Q\n\tdb_schema\x18\x03 \x01(\x0b\x32/.api.v1.MetadataResponse.DatabaseSchemaMetadataH\x00R\x08\x64\x62Schema\x88\x01\x01\x12\x41\n\x07\x62uckets\x18\x04 \x03(\x0b\x32\'.api.v1.MetadataResponse.BucketMetadataR\x07\x62uckets\x12\x35\n\x05kafka\x18\x05 \x01(\x0b\x32\x1a.plugins.kafka.v1.MetadataH\x01R\x05kafka\x88\x01\x01\x12\x45\n\x08\x63osmosdb\x18\x06 \x01(\x0b\x32$.plugins.cosmosdb.v1.Plugin.MetadataH\x02R\x08\x63osmosdb\x88\x01\x01\x12\x39\n\x04\x61\x64ls\x18\x07 \x01(\x0b\x32 .plugins.adls.v1.Plugin.MetadataH\x03R\x04\x61\x64ls\x88\x01\x01\x12\x35\n\x08\x64ynamodb\x18\x08 \x01(\x0b\x32\x14.google.protobuf.AnyH\x04R\x08\x64ynamodb\x88\x01\x01\x12;\n\x18g_sheets_next_page_token\x18\t \x01(\tH\x05R\x14gSheetsNextPageToken\x88\x01\x01\x42\x0c\n\n_db_schemaB\x08\n\x06_kafkaB\x0b\n\t_cosmosdbB\x07\n\x05_adlsB\x0b\n\t_dynamodbB\x1b\n\x19_g_sheets_next_page_token\"\xc0\x03\n\x05\x46\x65tch\x12-\n\x03\x61pi\x18\x01 \x01(\x0b\x32\x0b.api.v1.ApiB\x0e\xfa\x42\x05\x8a\x01\x02\x10\x01\xbaH\x03\xc8\x01\x01R\x03\x61pi\x12I\n\x0cintegrations\x18\x02 \x03(\x0b\x32%.transport.v1.Fetch.IntegrationsEntryR\x0cintegrations\x12H\n\x08metadata\x18\x03 \x01(\x0b\x32\x1c.transport.v1.Fetch.MetadataB\x0e\xfa\x42\x05\x8a\x01\x02\x10\x01\xbaH\x03\xc8\x01\x01R\x08metadata\x12(\n\x06stores\x18\x04 \x01(\x0b\x32\x10.store.v1.StoresR\x06stores\x1ao\n\x08Metadata\x12\x1c\n\trequester\x18\x01 \x01(\tR\trequester\x12\x18\n\x07profile\x18\x02 \x01(\tR\x07profile\x12+\n\x11organization_plan\x18\x03 \x01(\tR\x10organizationPlan\x1aX\n\x11IntegrationsEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12-\n\x05value\x18\x02 \x01(\x0b\x32\x17.google.protobuf.StructR\x05value:\x02\x38\x01\">\n\x14\x46\x65tchScheduleJobResp\x12&\n\x04\x61pis\x18\x01 \x03(\x0b\x32\x12.api.v1.DefinitionR\x04\x61pisB6Z4github.com/superblocksteam/types/gen/go/transport/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/utils/v1/utils_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/utils/v1/utils_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/validate/validate_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/worker/v1/step_executor_pb2.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/worker/v1/step_executor_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from transport.v1 import transport_pb2 as transport_dot_v1_dot_transport__pb2
+from superblocks_types.transport.v1 import transport_pb2 as transport_dot_v1_dot_transport__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1dworker/v1/step_executor.proto\x12\tworker.v1\x1a\x1ctransport/v1/transport.proto\"#\n\x0bStringValue\x12\x14\n\x05value\x18\x01 \x01(\tR\x05value2\xd3\x02\n\x13StepExecutorService\x12;\n\x06Stream\x12\x15.transport.v1.Request\x1a\x16.worker.v1.StringValue\"\x00\x30\x01\x12:\n\x07\x45xecute\x12\x15.transport.v1.Request\x1a\x16.transport.v1.Response\"\x00\x12;\n\x08Metadata\x12\x15.transport.v1.Request\x1a\x16.transport.v1.Response\"\x00\x12\x41\n\x0eTestConnection\x12\x15.transport.v1.Request\x1a\x16.transport.v1.Response\"\x00\x12\x43\n\x10\x44\x65leteDatasource\x12\x15.transport.v1.Request\x1a\x16.transport.v1.Response\"\x00\x42\x33Z1github.com/superblocksteam/types/gen/go/worker/v1b\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'worker.v1.step_executor_pb2', _globals)
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types/worker/v1/step_executor_pb2_grpc.py` & `superblocks-types-0.0.9/gen/py/superblocks_types/worker/v1/step_executor_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from transport.v1 import transport_pb2 as transport_dot_v1_dot_transport__pb2
-from worker.v1 import step_executor_pb2 as worker_dot_v1_dot_step__executor__pb2
+from superblocks_types.transport.v1 import transport_pb2 as transport_dot_v1_dot_transport__pb2
+from superblocks_types.worker.v1 import step_executor_pb2 as worker_dot_v1_dot_step__executor__pb2
 
 
 class StepExecutorServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types.egg-info/PKG-INFO` & `superblocks-types-0.0.9/gen/py/superblocks_types.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superblocks-types
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Official Python Types for Superblocks
 Home-page: https://github.com/superblocksteam/types
 Author: Joey Greco
 Author-email: joeyagreco@gmail.com
 License: MIT
 Keywords: superblocks types
 Requires-Python: >=3.10
```

### Comparing `superblocks-types-0.0.8/gen/py/superblocks_types.egg-info/SOURCES.txt` & `superblocks-types-0.0.9/gen/py/superblocks_types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

