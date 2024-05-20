# Comparing `tmp/codefly_cli-0.0.8.tar.gz` & `tmp/codefly_cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codefly_cli-0.0.8.tar", max compression
+gzip compressed data, was "codefly_cli-0.0.9.tar", max compression
```

## Comparing `codefly_cli-0.0.8.tar` & `codefly_cli-0.0.9.tar`

### file list

```diff
@@ -1,133 +1,133 @@
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.8/codefly_cli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 14:08:31.584555 codefly_cli-0.0.8/codefly_cli/actions/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.8/codefly_cli/actions/v0/__init__.py
--rw-r--r--   0        0        0     2004 2024-05-16 14:53:37.499836 codefly_cli-0.0.8/codefly_cli/actions/v0/module_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499681 codefly_cli-0.0.8/codefly_cli/actions/v0/module_pb2_grpc.py
--rw-r--r--   0        0        0     2009 2024-05-16 14:53:37.499220 codefly_cli-0.0.8/codefly_cli/actions/v0/organization_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499510 codefly_cli-0.0.8/codefly_cli/actions/v0/organization_pb2_grpc.py
--rw-r--r--   0        0        0     3743 2024-05-16 14:53:37.499953 codefly_cli-0.0.8/codefly_cli/actions/v0/service_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499899 codefly_cli-0.0.8/codefly_cli/actions/v0/service_pb2_grpc.py
--rw-r--r--   0        0        0     2588 2024-05-16 14:53:37.499937 codefly_cli-0.0.8/codefly_cli/actions/v0/workspace_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499877 codefly_cli-0.0.8/codefly_cli/actions/v0/workspace_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-05-13 14:08:31.584555 codefly_cli-0.0.8/codefly_cli/base/__init__.py
--rw-r--r--   0        0        0      194 2024-05-13 14:09:42.444829 codefly_cli-0.0.8/codefly_cli/base/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.8/codefly_cli/base/v0/__init__.py
--rw-r--r--   0        0        0      197 2024-05-13 13:43:44.892103 codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1676 2024-05-18 18:07:17.078576 codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/agent_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1855 2024-05-18 18:07:17.085209 codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/configuration_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     3371 2024-05-18 18:07:17.076349 codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/endpoint_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1615 2024-05-18 18:07:17.101736 codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/environment_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1791 2024-05-18 18:07:17.072066 codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/module_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1950 2024-05-18 18:07:17.103610 codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/network_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1704 2024-05-18 18:07:17.087333 codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/scope_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2613 2024-05-18 18:07:17.074126 codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/service_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1701 2024-05-18 18:07:17.098860 codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/spec_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2168 2024-05-18 18:07:16.996487 codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/workspace_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2399 2024-05-16 14:53:37.499708 codefly_cli-0.0.8/codefly_cli/base/v0/agent_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499646 codefly_cli-0.0.8/codefly_cli/base/v0/agent_pb2_grpc.py
--rw-r--r--   0        0        0     2500 2024-05-16 14:53:37.499461 codefly_cli-0.0.8/codefly_cli/base/v0/configuration_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499745 codefly_cli-0.0.8/codefly_cli/base/v0/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     5828 2024-05-16 14:53:37.500444 codefly_cli-0.0.8/codefly_cli/base/v0/endpoint_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.500443 codefly_cli-0.0.8/codefly_cli/base/v0/endpoint_pb2_grpc.py
--rw-r--r--   0        0        0     2169 2024-05-16 14:53:37.500330 codefly_cli-0.0.8/codefly_cli/base/v0/environment_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.500340 codefly_cli-0.0.8/codefly_cli/base/v0/environment_pb2_grpc.py
--rw-r--r--   0        0        0     2402 2024-05-16 14:53:37.500972 codefly_cli-0.0.8/codefly_cli/base/v0/module_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501854 codefly_cli-0.0.8/codefly_cli/base/v0/module_pb2_grpc.py
--rw-r--r--   0        0        0     2768 2024-05-16 14:53:37.501436 codefly_cli-0.0.8/codefly_cli/base/v0/network_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501580 codefly_cli-0.0.8/codefly_cli/base/v0/network_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2024-05-16 14:53:37.501802 codefly_cli-0.0.8/codefly_cli/base/v0/organization_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501756 codefly_cli-0.0.8/codefly_cli/base/v0/organization_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2024-05-16 14:53:37.501624 codefly_cli-0.0.8/codefly_cli/base/v0/scope_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501786 codefly_cli-0.0.8/codefly_cli/base/v0/scope_pb2_grpc.py
--rw-r--r--   0        0        0     4669 2024-05-16 14:53:37.501891 codefly_cli-0.0.8/codefly_cli/base/v0/service_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.502450 codefly_cli-0.0.8/codefly_cli/base/v0/service_pb2_grpc.py
--rw-r--r--   0        0        0     2414 2024-05-16 14:53:37.501961 codefly_cli-0.0.8/codefly_cli/base/v0/spec_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.502506 codefly_cli-0.0.8/codefly_cli/base/v0/spec_pb2_grpc.py
--rw-r--r--   0        0        0     3318 2024-05-16 14:53:37.502732 codefly_cli-0.0.8/codefly_cli/base/v0/workspace_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.503340 codefly_cli-0.0.8/codefly_cli/base/v0/workspace_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.8/codefly_cli/buf/__init__.py
--rw-r--r--   0        0        0      193 2024-05-13 13:47:20.622712 codefly_cli-0.0.8/codefly_cli/buf/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1849 2024-05-10 18:40:43.954080 codefly_cli-0.0.8/codefly_cli/buf/validate/BUILD.bazel
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.8/codefly_cli/buf/validate/__init__.py
--rw-r--r--   0        0        0      202 2024-05-13 13:47:20.623558 codefly_cli-0.0.8/codefly_cli/buf/validate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1735 2024-05-18 18:07:17.059629 codefly_cli-0.0.8/codefly_cli/buf/validate/__pycache__/expression_pb2.cpython-310.pyc
--rw-r--r--   0        0        0   105220 2024-05-18 18:07:17.056893 codefly_cli-0.0.8/codefly_cli/buf/validate/__pycache__/validate_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     4027 2024-05-10 18:40:43.958003 codefly_cli-0.0.8/codefly_cli/buf/validate/expression.proto
--rw-r--r--   0        0        0     2292 2024-05-16 14:53:37.503962 codefly_cli-0.0.8/codefly_cli/buf/validate/expression_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.503883 codefly_cli-0.0.8/codefly_cli/buf/validate/expression_pb2_grpc.py
--rw-r--r--   0        0        0     1064 2024-05-10 18:40:43.969884 codefly_cli-0.0.8/codefly_cli/buf/validate/priv/BUILD.bazel
--rw-r--r--   0        0        0        0 2024-05-10 18:40:43.949057 codefly_cli-0.0.8/codefly_cli/buf/validate/priv/__init__.py
--rw-r--r--   0        0        0      207 2024-05-11 14:39:48.143074 codefly_cli-0.0.8/codefly_cli/buf/validate/priv/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1833 2024-05-18 18:07:17.063238 codefly_cli-0.0.8/codefly_cli/buf/validate/priv/__pycache__/private_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1304 2024-05-10 18:40:43.951308 codefly_cli-0.0.8/codefly_cli/buf/validate/priv/private.proto
--rw-r--r--   0        0        0     2332 2024-05-16 14:53:37.503853 codefly_cli-0.0.8/codefly_cli/buf/validate/priv/private_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.504685 codefly_cli-0.0.8/codefly_cli/buf/validate/priv/private_pb2_grpc.py
--rw-r--r--   0        0        0   166999 2024-05-10 18:40:43.974825 codefly_cli-0.0.8/codefly_cli/buf/validate/validate.proto
--rw-r--r--   0        0        0   144402 2024-05-16 14:53:37.506101 codefly_cli-0.0.8/codefly_cli/buf/validate/validate_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.504729 codefly_cli-0.0.8/codefly_cli/buf/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.8/codefly_cli/cli/__init__.py
--rw-r--r--   0        0        0      193 2024-05-13 13:43:44.884477 codefly_cli-0.0.8/codefly_cli/cli/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.8/codefly_cli/cli/v0/__init__.py
--rw-r--r--   0        0        0      196 2024-05-13 13:43:44.885610 codefly_cli-0.0.8/codefly_cli/cli/v0/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7582 2024-05-18 18:07:17.081796 codefly_cli-0.0.8/codefly_cli/cli/v0/__pycache__/cli_pb2.cpython-310.pyc
--rw-r--r--   0        0        0    10048 2024-05-18 18:07:16.992597 codefly_cli-0.0.8/codefly_cli/cli/v0/__pycache__/cli_pb2_grpc.cpython-310.pyc
--rw-r--r--   0        0        0    11729 2024-05-16 14:53:37.505430 codefly_cli-0.0.8/codefly_cli/cli/v0/cli_pb2.py
--rw-r--r--   0        0        0    28562 2024-05-16 14:53:37.504644 codefly_cli-0.0.8/codefly_cli/cli/v0/cli_pb2_grpc.py
--rw-r--r--   0        0        0     4280 2024-05-18 18:45:18.546664 codefly_cli-0.0.8/codefly_cli/codefly.py
--rw-r--r--   0        0        0     1517 2024-05-18 18:07:17.118704 codefly_cli-0.0.8/codefly_cli/google/api/__pycache__/annotations_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1912 2024-05-18 18:07:17.120443 codefly_cli-0.0.8/codefly_cli/google/api/__pycache__/http_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1792 2024-05-16 14:53:37.504861 codefly_cli-0.0.8/codefly_cli/google/api/annotations_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.504934 codefly_cli-0.0.8/codefly_cli/google/api/annotations_pb2_grpc.py
--rw-r--r--   0        0        0     2690 2024-05-16 14:53:37.504907 codefly_cli-0.0.8/codefly_cli/google/api/http_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.505129 codefly_cli-0.0.8/codefly_cli/google/api/http_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.8/codefly_cli/observability/__init__.py
--rw-r--r--   0        0        0      203 2024-05-13 13:47:20.666896 codefly_cli-0.0.8/codefly_cli/observability/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.8/codefly_cli/observability/v0/__init__.py
--rw-r--r--   0        0        0      206 2024-05-13 13:47:20.667998 codefly_cli-0.0.8/codefly_cli/observability/v0/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1828 2024-05-18 18:07:17.111714 codefly_cli-0.0.8/codefly_cli/observability/v0/__pycache__/dependencies_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     1550 2024-05-18 18:07:17.109926 codefly_cli-0.0.8/codefly_cli/observability/v0/__pycache__/inventory_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2265 2024-05-18 18:07:17.113715 codefly_cli-0.0.8/codefly_cli/observability/v0/__pycache__/logs_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2214 2024-05-18 18:07:17.115529 codefly_cli-0.0.8/codefly_cli/observability/v0/__pycache__/sessions_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     2474 2024-05-16 14:53:37.505558 codefly_cli-0.0.8/codefly_cli/observability/v0/dependencies_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506072 codefly_cli-0.0.8/codefly_cli/observability/v0/dependencies_pb2_grpc.py
--rw-r--r--   0        0        0     1837 2024-05-16 14:53:37.505766 codefly_cli-0.0.8/codefly_cli/observability/v0/inventory_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.505954 codefly_cli-0.0.8/codefly_cli/observability/v0/inventory_pb2_grpc.py
--rw-r--r--   0        0        0     2961 2024-05-16 14:53:37.506417 codefly_cli-0.0.8/codefly_cli/observability/v0/logs_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506415 codefly_cli-0.0.8/codefly_cli/observability/v0/logs_pb2_grpc.py
--rw-r--r--   0        0        0     2098 2024-05-16 14:53:37.506262 codefly_cli-0.0.8/codefly_cli/observability/v0/metrics_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506455 codefly_cli-0.0.8/codefly_cli/observability/v0/metrics_pb2_grpc.py
--rw-r--r--   0        0        0     2985 2024-05-16 14:53:37.506432 codefly_cli-0.0.8/codefly_cli/observability/v0/sessions_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506726 codefly_cli-0.0.8/codefly_cli/observability/v0/sessions_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.8/codefly_cli/services/__init__.py
--rw-r--r--   0        0        0      198 2024-05-13 13:47:20.650463 codefly_cli-0.0.8/codefly_cli/services/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.8/codefly_cli/services/agent/__init__.py
--rw-r--r--   0        0        0      204 2024-05-13 13:47:20.651647 codefly_cli-0.0.8/codefly_cli/services/agent/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.8/codefly_cli/services/agent/v0/__init__.py
--rw-r--r--   0        0        0      207 2024-05-13 13:47:20.652542 codefly_cli-0.0.8/codefly_cli/services/agent/v0/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3328 2024-05-18 18:07:17.092257 codefly_cli-0.0.8/codefly_cli/services/agent/v0/__pycache__/agent_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     4050 2024-05-18 18:07:17.105805 codefly_cli-0.0.8/codefly_cli/services/agent/v0/__pycache__/communicate_pb2.cpython-310.pyc
--rw-r--r--   0        0        0     5107 2024-05-16 14:53:37.507542 codefly_cli-0.0.8/codefly_cli/services/agent/v0/agent_pb2.py
--rw-r--r--   0        0        0     2895 2024-05-16 14:53:37.507520 codefly_cli-0.0.8/codefly_cli/services/agent/v0/agent_pb2_grpc.py
--rw-r--r--   0        0        0     6560 2024-05-16 14:53:37.507558 codefly_cli-0.0.8/codefly_cli/services/agent/v0/communicate_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.507148 codefly_cli-0.0.8/codefly_cli/services/agent/v0/communicate_pb2_grpc.py
--rw-r--r--   0        0        0     2426 2024-05-16 14:53:37.507482 codefly_cli-0.0.8/codefly_cli/services/agent/v0/cyclonedx_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.507429 codefly_cli-0.0.8/codefly_cli/services/agent/v0/cyclonedx_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.8/codefly_cli/services/builder/__init__.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.8/codefly_cli/services/builder/v0/__init__.py
--rw-r--r--   0        0        0    11603 2024-05-16 14:53:37.507453 codefly_cli-0.0.8/codefly_cli/services/builder/v0/builder_pb2.py
--rw-r--r--   0        0        0    15720 2024-05-16 14:53:37.508035 codefly_cli-0.0.8/codefly_cli/services/builder/v0/builder_pb2_grpc.py
--rw-r--r--   0        0        0     3239 2024-05-16 14:53:37.508589 codefly_cli-0.0.8/codefly_cli/services/builder/v0/deployment_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.508879 codefly_cli-0.0.8/codefly_cli/services/builder/v0/deployment_pb2_grpc.py
--rw-r--r--   0        0        0     1959 2024-05-16 14:53:37.508593 codefly_cli-0.0.8/codefly_cli/services/builder/v0/docker_pb2.py
--rw-r--r--   0        0        0      159 2024-05-16 14:53:37.508837 codefly_cli-0.0.8/codefly_cli/services/builder/v0/docker_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.8/codefly_cli/services/runtime/__init__.py
--rw-r--r--   0        0        0      206 2024-05-13 13:47:20.655031 codefly_cli-0.0.8/codefly_cli/services/runtime/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.8/codefly_cli/services/runtime/v0/__init__.py
--rw-r--r--   0        0        0      209 2024-05-13 13:47:20.655871 codefly_cli-0.0.8/codefly_cli/services/runtime/v0/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     7464 2024-05-18 18:07:17.096644 codefly_cli-0.0.8/codefly_cli/services/runtime/v0/__pycache__/runtime_pb2.cpython-310.pyc
--rw-r--r--   0        0        0    11252 2024-05-16 14:53:37.509254 codefly_cli-0.0.8/codefly_cli/services/runtime/v0/runtime_pb2.py
--rw-r--r--   0        0        0    15818 2024-05-16 14:53:37.509221 codefly_cli-0.0.8/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py
--rw-r--r--   0        0        0      713 2024-05-13 14:13:15.469467 codefly_cli-0.0.8/codefly_cli/tests/__pycache__/test_cli.cpython-310-pytest-8.2.0.pyc
--rw-r--r--   0        0        0      171 2024-05-13 14:10:06.354079 codefly_cli-0.0.8/codefly_cli/tests/test_cli.py
--rw-r--r--   0        0        0      448 2024-05-18 18:45:34.083362 codefly_cli-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 codefly_cli-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.9/codefly_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 14:08:31.584555 codefly_cli-0.0.9/codefly_cli/actions/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.9/codefly_cli/actions/v0/__init__.py
+-rw-r--r--   0        0        0     2004 2024-05-16 14:53:37.499836 codefly_cli-0.0.9/codefly_cli/actions/v0/module_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499681 codefly_cli-0.0.9/codefly_cli/actions/v0/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2009 2024-05-16 14:53:37.499220 codefly_cli-0.0.9/codefly_cli/actions/v0/organization_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499510 codefly_cli-0.0.9/codefly_cli/actions/v0/organization_pb2_grpc.py
+-rw-r--r--   0        0        0     3743 2024-05-16 14:53:37.499953 codefly_cli-0.0.9/codefly_cli/actions/v0/service_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499899 codefly_cli-0.0.9/codefly_cli/actions/v0/service_pb2_grpc.py
+-rw-r--r--   0        0        0     2588 2024-05-16 14:53:37.499937 codefly_cli-0.0.9/codefly_cli/actions/v0/workspace_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499877 codefly_cli-0.0.9/codefly_cli/actions/v0/workspace_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-05-13 14:08:31.584555 codefly_cli-0.0.9/codefly_cli/base/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-13 14:09:42.444829 codefly_cli-0.0.9/codefly_cli/base/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.9/codefly_cli/base/v0/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-13 13:43:44.892103 codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1676 2024-05-18 18:07:17.078576 codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/agent_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1855 2024-05-18 18:07:17.085209 codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/configuration_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     3371 2024-05-18 18:07:17.076349 codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/endpoint_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1615 2024-05-18 18:07:17.101736 codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/environment_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1791 2024-05-18 18:07:17.072066 codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/module_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1950 2024-05-18 18:07:17.103610 codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/network_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1704 2024-05-18 18:07:17.087333 codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/scope_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2613 2024-05-18 18:07:17.074126 codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/service_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1701 2024-05-18 18:07:17.098860 codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/spec_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2168 2024-05-18 18:07:16.996487 codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/workspace_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2399 2024-05-16 14:53:37.499708 codefly_cli-0.0.9/codefly_cli/base/v0/agent_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499646 codefly_cli-0.0.9/codefly_cli/base/v0/agent_pb2_grpc.py
+-rw-r--r--   0        0        0     2500 2024-05-16 14:53:37.499461 codefly_cli-0.0.9/codefly_cli/base/v0/configuration_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.499745 codefly_cli-0.0.9/codefly_cli/base/v0/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     5828 2024-05-16 14:53:37.500444 codefly_cli-0.0.9/codefly_cli/base/v0/endpoint_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.500443 codefly_cli-0.0.9/codefly_cli/base/v0/endpoint_pb2_grpc.py
+-rw-r--r--   0        0        0     2169 2024-05-16 14:53:37.500330 codefly_cli-0.0.9/codefly_cli/base/v0/environment_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.500340 codefly_cli-0.0.9/codefly_cli/base/v0/environment_pb2_grpc.py
+-rw-r--r--   0        0        0     2402 2024-05-16 14:53:37.500972 codefly_cli-0.0.9/codefly_cli/base/v0/module_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501854 codefly_cli-0.0.9/codefly_cli/base/v0/module_pb2_grpc.py
+-rw-r--r--   0        0        0     2768 2024-05-16 14:53:37.501436 codefly_cli-0.0.9/codefly_cli/base/v0/network_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501580 codefly_cli-0.0.9/codefly_cli/base/v0/network_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2024-05-16 14:53:37.501802 codefly_cli-0.0.9/codefly_cli/base/v0/organization_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501756 codefly_cli-0.0.9/codefly_cli/base/v0/organization_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2024-05-16 14:53:37.501624 codefly_cli-0.0.9/codefly_cli/base/v0/scope_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.501786 codefly_cli-0.0.9/codefly_cli/base/v0/scope_pb2_grpc.py
+-rw-r--r--   0        0        0     4669 2024-05-16 14:53:37.501891 codefly_cli-0.0.9/codefly_cli/base/v0/service_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.502450 codefly_cli-0.0.9/codefly_cli/base/v0/service_pb2_grpc.py
+-rw-r--r--   0        0        0     2414 2024-05-16 14:53:37.501961 codefly_cli-0.0.9/codefly_cli/base/v0/spec_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.502506 codefly_cli-0.0.9/codefly_cli/base/v0/spec_pb2_grpc.py
+-rw-r--r--   0        0        0     3318 2024-05-16 14:53:37.502732 codefly_cli-0.0.9/codefly_cli/base/v0/workspace_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.503340 codefly_cli-0.0.9/codefly_cli/base/v0/workspace_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.9/codefly_cli/buf/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-13 13:47:20.622712 codefly_cli-0.0.9/codefly_cli/buf/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1849 2024-05-10 18:40:43.954080 codefly_cli-0.0.9/codefly_cli/buf/validate/BUILD.bazel
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.9/codefly_cli/buf/validate/__init__.py
+-rw-r--r--   0        0        0      202 2024-05-13 13:47:20.623558 codefly_cli-0.0.9/codefly_cli/buf/validate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1735 2024-05-18 18:07:17.059629 codefly_cli-0.0.9/codefly_cli/buf/validate/__pycache__/expression_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0   105220 2024-05-18 18:07:17.056893 codefly_cli-0.0.9/codefly_cli/buf/validate/__pycache__/validate_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     4027 2024-05-10 18:40:43.958003 codefly_cli-0.0.9/codefly_cli/buf/validate/expression.proto
+-rw-r--r--   0        0        0     2292 2024-05-16 14:53:37.503962 codefly_cli-0.0.9/codefly_cli/buf/validate/expression_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.503883 codefly_cli-0.0.9/codefly_cli/buf/validate/expression_pb2_grpc.py
+-rw-r--r--   0        0        0     1064 2024-05-10 18:40:43.969884 codefly_cli-0.0.9/codefly_cli/buf/validate/priv/BUILD.bazel
+-rw-r--r--   0        0        0        0 2024-05-10 18:40:43.949057 codefly_cli-0.0.9/codefly_cli/buf/validate/priv/__init__.py
+-rw-r--r--   0        0        0      207 2024-05-11 14:39:48.143074 codefly_cli-0.0.9/codefly_cli/buf/validate/priv/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1833 2024-05-18 18:07:17.063238 codefly_cli-0.0.9/codefly_cli/buf/validate/priv/__pycache__/private_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1304 2024-05-10 18:40:43.951308 codefly_cli-0.0.9/codefly_cli/buf/validate/priv/private.proto
+-rw-r--r--   0        0        0     2332 2024-05-16 14:53:37.503853 codefly_cli-0.0.9/codefly_cli/buf/validate/priv/private_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.504685 codefly_cli-0.0.9/codefly_cli/buf/validate/priv/private_pb2_grpc.py
+-rw-r--r--   0        0        0   166999 2024-05-10 18:40:43.974825 codefly_cli-0.0.9/codefly_cli/buf/validate/validate.proto
+-rw-r--r--   0        0        0   144402 2024-05-16 14:53:37.506101 codefly_cli-0.0.9/codefly_cli/buf/validate/validate_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.504729 codefly_cli-0.0.9/codefly_cli/buf/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.9/codefly_cli/cli/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-13 13:43:44.884477 codefly_cli-0.0.9/codefly_cli/cli/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.9/codefly_cli/cli/v0/__init__.py
+-rw-r--r--   0        0        0      196 2024-05-13 13:43:44.885610 codefly_cli-0.0.9/codefly_cli/cli/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7582 2024-05-18 18:07:17.081796 codefly_cli-0.0.9/codefly_cli/cli/v0/__pycache__/cli_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0    10048 2024-05-18 18:07:16.992597 codefly_cli-0.0.9/codefly_cli/cli/v0/__pycache__/cli_pb2_grpc.cpython-310.pyc
+-rw-r--r--   0        0        0    11729 2024-05-16 14:53:37.505430 codefly_cli-0.0.9/codefly_cli/cli/v0/cli_pb2.py
+-rw-r--r--   0        0        0    28562 2024-05-16 14:53:37.504644 codefly_cli-0.0.9/codefly_cli/cli/v0/cli_pb2_grpc.py
+-rw-r--r--   0        0        0     4613 2024-05-20 14:13:29.173741 codefly_cli-0.0.9/codefly_cli/codefly.py
+-rw-r--r--   0        0        0     1517 2024-05-18 18:07:17.118704 codefly_cli-0.0.9/codefly_cli/google/api/__pycache__/annotations_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1912 2024-05-18 18:07:17.120443 codefly_cli-0.0.9/codefly_cli/google/api/__pycache__/http_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1792 2024-05-16 14:53:37.504861 codefly_cli-0.0.9/codefly_cli/google/api/annotations_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.504934 codefly_cli-0.0.9/codefly_cli/google/api/annotations_pb2_grpc.py
+-rw-r--r--   0        0        0     2690 2024-05-16 14:53:37.504907 codefly_cli-0.0.9/codefly_cli/google/api/http_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.505129 codefly_cli-0.0.9/codefly_cli/google/api/http_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.9/codefly_cli/observability/__init__.py
+-rw-r--r--   0        0        0      203 2024-05-13 13:47:20.666896 codefly_cli-0.0.9/codefly_cli/observability/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.9/codefly_cli/observability/v0/__init__.py
+-rw-r--r--   0        0        0      206 2024-05-13 13:47:20.667998 codefly_cli-0.0.9/codefly_cli/observability/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1828 2024-05-18 18:07:17.111714 codefly_cli-0.0.9/codefly_cli/observability/v0/__pycache__/dependencies_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     1550 2024-05-18 18:07:17.109926 codefly_cli-0.0.9/codefly_cli/observability/v0/__pycache__/inventory_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2265 2024-05-18 18:07:17.113715 codefly_cli-0.0.9/codefly_cli/observability/v0/__pycache__/logs_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2214 2024-05-18 18:07:17.115529 codefly_cli-0.0.9/codefly_cli/observability/v0/__pycache__/sessions_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     2474 2024-05-16 14:53:37.505558 codefly_cli-0.0.9/codefly_cli/observability/v0/dependencies_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506072 codefly_cli-0.0.9/codefly_cli/observability/v0/dependencies_pb2_grpc.py
+-rw-r--r--   0        0        0     1837 2024-05-16 14:53:37.505766 codefly_cli-0.0.9/codefly_cli/observability/v0/inventory_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.505954 codefly_cli-0.0.9/codefly_cli/observability/v0/inventory_pb2_grpc.py
+-rw-r--r--   0        0        0     2961 2024-05-16 14:53:37.506417 codefly_cli-0.0.9/codefly_cli/observability/v0/logs_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506415 codefly_cli-0.0.9/codefly_cli/observability/v0/logs_pb2_grpc.py
+-rw-r--r--   0        0        0     2098 2024-05-16 14:53:37.506262 codefly_cli-0.0.9/codefly_cli/observability/v0/metrics_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506455 codefly_cli-0.0.9/codefly_cli/observability/v0/metrics_pb2_grpc.py
+-rw-r--r--   0        0        0     2985 2024-05-16 14:53:37.506432 codefly_cli-0.0.9/codefly_cli/observability/v0/sessions_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.506726 codefly_cli-0.0.9/codefly_cli/observability/v0/sessions_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.9/codefly_cli/services/__init__.py
+-rw-r--r--   0        0        0      198 2024-05-13 13:47:20.650463 codefly_cli-0.0.9/codefly_cli/services/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.9/codefly_cli/services/agent/__init__.py
+-rw-r--r--   0        0        0      204 2024-05-13 13:47:20.651647 codefly_cli-0.0.9/codefly_cli/services/agent/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.9/codefly_cli/services/agent/v0/__init__.py
+-rw-r--r--   0        0        0      207 2024-05-13 13:47:20.652542 codefly_cli-0.0.9/codefly_cli/services/agent/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3328 2024-05-18 18:07:17.092257 codefly_cli-0.0.9/codefly_cli/services/agent/v0/__pycache__/agent_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     4050 2024-05-18 18:07:17.105805 codefly_cli-0.0.9/codefly_cli/services/agent/v0/__pycache__/communicate_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0     5107 2024-05-16 14:53:37.507542 codefly_cli-0.0.9/codefly_cli/services/agent/v0/agent_pb2.py
+-rw-r--r--   0        0        0     2895 2024-05-16 14:53:37.507520 codefly_cli-0.0.9/codefly_cli/services/agent/v0/agent_pb2_grpc.py
+-rw-r--r--   0        0        0     6560 2024-05-16 14:53:37.507558 codefly_cli-0.0.9/codefly_cli/services/agent/v0/communicate_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.507148 codefly_cli-0.0.9/codefly_cli/services/agent/v0/communicate_pb2_grpc.py
+-rw-r--r--   0        0        0     2426 2024-05-16 14:53:37.507482 codefly_cli-0.0.9/codefly_cli/services/agent/v0/cyclonedx_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.507429 codefly_cli-0.0.9/codefly_cli/services/agent/v0/cyclonedx_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.9/codefly_cli/services/builder/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.9/codefly_cli/services/builder/v0/__init__.py
+-rw-r--r--   0        0        0    11603 2024-05-16 14:53:37.507453 codefly_cli-0.0.9/codefly_cli/services/builder/v0/builder_pb2.py
+-rw-r--r--   0        0        0    15720 2024-05-16 14:53:37.508035 codefly_cli-0.0.9/codefly_cli/services/builder/v0/builder_pb2_grpc.py
+-rw-r--r--   0        0        0     3239 2024-05-16 14:53:37.508589 codefly_cli-0.0.9/codefly_cli/services/builder/v0/deployment_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.508879 codefly_cli-0.0.9/codefly_cli/services/builder/v0/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0     1959 2024-05-16 14:53:37.508593 codefly_cli-0.0.9/codefly_cli/services/builder/v0/docker_pb2.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:53:37.508837 codefly_cli-0.0.9/codefly_cli/services/builder/v0/docker_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.9/codefly_cli/services/runtime/__init__.py
+-rw-r--r--   0        0        0      206 2024-05-13 13:47:20.655031 codefly_cli-0.0.9/codefly_cli/services/runtime/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2024-04-19 14:01:44.838788 codefly_cli-0.0.9/codefly_cli/services/runtime/v0/__init__.py
+-rw-r--r--   0        0        0      209 2024-05-13 13:47:20.655871 codefly_cli-0.0.9/codefly_cli/services/runtime/v0/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     7464 2024-05-18 18:07:17.096644 codefly_cli-0.0.9/codefly_cli/services/runtime/v0/__pycache__/runtime_pb2.cpython-310.pyc
+-rw-r--r--   0        0        0    11252 2024-05-16 14:53:37.509254 codefly_cli-0.0.9/codefly_cli/services/runtime/v0/runtime_pb2.py
+-rw-r--r--   0        0        0    15818 2024-05-16 14:53:37.509221 codefly_cli-0.0.9/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py
+-rw-r--r--   0        0        0      713 2024-05-13 14:13:15.469467 codefly_cli-0.0.9/codefly_cli/tests/__pycache__/test_cli.cpython-310-pytest-8.2.0.pyc
+-rw-r--r--   0        0        0      171 2024-05-13 14:10:06.354079 codefly_cli-0.0.9/codefly_cli/tests/test_cli.py
+-rw-r--r--   0        0        0      448 2024-05-20 14:14:44.045739 codefly_cli-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      651 1970-01-01 00:00:00.000000 codefly_cli-0.0.9/PKG-INFO
```

### Comparing `codefly_cli-0.0.8/codefly_cli/actions/v0/module_pb2.py` & `codefly_cli-0.0.9/codefly_cli/actions/v0/module_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/actions/v0/organization_pb2.py` & `codefly_cli-0.0.9/codefly_cli/actions/v0/organization_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/actions/v0/service_pb2.py` & `codefly_cli-0.0.9/codefly_cli/actions/v0/service_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/actions/v0/workspace_pb2.py` & `codefly_cli-0.0.9/codefly_cli/actions/v0/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/agent_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/agent_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/configuration_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/configuration_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/endpoint_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/endpoint_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/environment_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/environment_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/module_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/module_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/network_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/network_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/scope_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/scope_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/service_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/service_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/spec_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/spec_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/__pycache__/workspace_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/base/v0/__pycache__/workspace_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/agent_pb2.py` & `codefly_cli-0.0.9/codefly_cli/base/v0/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/configuration_pb2.py` & `codefly_cli-0.0.9/codefly_cli/base/v0/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/endpoint_pb2.py` & `codefly_cli-0.0.9/codefly_cli/base/v0/endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/environment_pb2.py` & `codefly_cli-0.0.9/codefly_cli/base/v0/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/module_pb2.py` & `codefly_cli-0.0.9/codefly_cli/base/v0/module_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/network_pb2.py` & `codefly_cli-0.0.9/codefly_cli/base/v0/network_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/organization_pb2.py` & `codefly_cli-0.0.9/codefly_cli/base/v0/organization_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/scope_pb2.py` & `codefly_cli-0.0.9/codefly_cli/base/v0/scope_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/service_pb2.py` & `codefly_cli-0.0.9/codefly_cli/base/v0/service_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/spec_pb2.py` & `codefly_cli-0.0.9/codefly_cli/base/v0/spec_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/base/v0/workspace_pb2.py` & `codefly_cli-0.0.9/codefly_cli/base/v0/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/buf/validate/BUILD.bazel` & `codefly_cli-0.0.9/codefly_cli/buf/validate/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/buf/validate/__pycache__/expression_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/buf/validate/__pycache__/expression_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/buf/validate/__pycache__/validate_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/buf/validate/__pycache__/validate_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/buf/validate/expression.proto` & `codefly_cli-0.0.9/codefly_cli/buf/validate/expression.proto`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/buf/validate/expression_pb2.py` & `codefly_cli-0.0.9/codefly_cli/buf/validate/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/buf/validate/priv/BUILD.bazel` & `codefly_cli-0.0.9/codefly_cli/buf/validate/priv/BUILD.bazel`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/buf/validate/priv/__pycache__/private_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/buf/validate/priv/__pycache__/private_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/buf/validate/priv/private.proto` & `codefly_cli-0.0.9/codefly_cli/buf/validate/priv/private.proto`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/buf/validate/priv/private_pb2.py` & `codefly_cli-0.0.9/codefly_cli/buf/validate/priv/private_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/buf/validate/validate.proto` & `codefly_cli-0.0.9/codefly_cli/buf/validate/validate.proto`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/buf/validate/validate_pb2.py` & `codefly_cli-0.0.9/codefly_cli/buf/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/cli/v0/__pycache__/cli_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/cli/v0/__pycache__/cli_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/cli/v0/__pycache__/cli_pb2_grpc.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/cli/v0/__pycache__/cli_pb2_grpc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/cli/v0/cli_pb2.py` & `codefly_cli-0.0.9/codefly_cli/cli/v0/cli_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/cli/v0/cli_pb2_grpc.py` & `codefly_cli-0.0.9/codefly_cli/cli/v0/cli_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/codefly.py` & `codefly_cli-0.0.9/codefly_cli/codefly.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+import os, sys
+
+# Add the codefly_cli path
+sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '../codefly_cli')))
+
+import codefly_sdk.codefly as codefly
+
 import subprocess
 import time
 import grpc
 from typing import Optional, List
 
 from codefly_sdk.codefly import init
 
@@ -23,19 +30,47 @@
 def with_dependencies():
     launcher = Launcher(show_cli_output=True)
     launcher.start()
     codefly.init("..")
     yield
     launcher.close()
 
+
+def configuration_key(conf: configuration.Configuration, info: configuration.ConfigurationInformation, value: configuration.ConfigurationValue):
+    secret_prefix = ""
+    if value.secret:
+        secret_prefix = "SECRET_"
+    if conf.origin == "workspace":
+        k = f"CODEFLY__WORKSPACE_{secret_prefix}CONFIGURATION"
+    else:
+        k = f"CODEFLY__SERVICE_{secret_prefix}CONFIGURATION__{unique_to_env_key(conf.origin)}"
+    return f"{k}__{info.name}__{value.key}".upper()
+
+
+def setup_environment_with_configuration(conf: configuration.Configuration):
+    for info in conf.configurations:
+        for val in info.configuration_values:
+            key = configuration_key(conf, info, val)
+            os.environ[key] = val.value
+
+_with_cli_logs = False
+
+def with_cli_logs():
+    global _with_cli_logs
+    _with_cli_logs = True
+
+
 class Launcher:
-    def __init__(self, root: str = "..", scope: str = "", show_cli_output: bool = False, keep_alive: bool = False):
+    def __init__(self, root: str = "..", scope: str = "", keep_alive: bool = False):
         self.cmd = None
         self.cli = None
-        self.show_cli_output = show_cli_output
+
+        global _with_cli_logs
+        self.show_cli_output = _with_cli_logs
+
         self.dir = find_service_dir(os.path.abspath(root))
         print(f"running in {self.dir}")
         self.scope = scope
         self.keep_alive = keep_alive
         self.module = codefly.get_module()
         self.service = codefly.get_service()
         self.unique = codefly.get_unique()
@@ -48,15 +83,15 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self.keep_alive:
             return
         self.destroy()
 
     def start(self):
-        cmd = ["codefly", "run", "service", "-d",  "--exclude-root", "--cli-server"]
+        cmd = ["codefly", "run", "service",  "--exclude-root", "--cli-server"]
         if self.scope:
             cmd.extend(["--scope", self.scope])
         options = {"stdout": subprocess.PIPE}
         if self.show_cli_output:
             options = {}
         self.cmd = subprocess.Popen(cmd, cwd=self.dir, **options)
         port = 10000
@@ -88,37 +123,20 @@
                 if wait <= 0:
                     raise Exception("timeout waiting for flow to be ready") from e
                 time.sleep(0.5)
 
     def setup_environment(self):
         request = cli.GetConfigurationRequest(module=self.module, service=self.service)
         resp = self.cli.GetDependenciesConfigurations(request)
+        print("DEPPPP", resp.configurations)
+        print("RUNTIME", self.runtime_context)
         dependencies_configurations = filter_configurations(resp.configurations, self.runtime_context)
+        print("DEP", dependencies_configurations)
         for conf in dependencies_configurations:
-            self.setup_environment_with_configuration(conf)
-
-
-    def configuration_key(self, conf: configuration.Configuration, info: configuration.ConfigurationInformation, value: configuration.ConfigurationValue):
-        secret_prefix = ""
-        if value.secret:
-            secret_prefix = "SECRET_"
-        if conf.origin == "workspace":
-            k = f"CODEFLY__WORKSPACE_{secret_prefix}CONFIGURATION"
-        else:
-            k = f"CODEFLY__SERVICE_{secret_prefix}CONFIGURATION__{unique_to_env_key(conf.origin)}"
-        return f"{k}__{info.name}__{value.key}".upper()
-
-    def setup_environment_with_configuration(self, conf: configuration.Configuration):
-        for info in conf.configurations:
-            for val in info.configuration_values:
-                key = self.configuration_key(conf, info, val)
-                os.environ[key] = val.value
-
-
-
+            setup_environment_with_configuration(conf)
 
     def close(self):
         self.cli.StopFlow(Empty())
         if self.cmd is not None:
             self.cmd.terminate()
             self.cmd.wait()
```

### Comparing `codefly_cli-0.0.8/codefly_cli/google/api/__pycache__/annotations_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/google/api/__pycache__/annotations_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/google/api/__pycache__/http_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/google/api/__pycache__/http_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/google/api/annotations_pb2.py` & `codefly_cli-0.0.9/codefly_cli/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/google/api/http_pb2.py` & `codefly_cli-0.0.9/codefly_cli/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/observability/v0/__pycache__/dependencies_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/observability/v0/__pycache__/dependencies_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/observability/v0/__pycache__/inventory_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/observability/v0/__pycache__/inventory_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/observability/v0/__pycache__/logs_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/observability/v0/__pycache__/logs_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/observability/v0/__pycache__/sessions_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/observability/v0/__pycache__/sessions_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/observability/v0/dependencies_pb2.py` & `codefly_cli-0.0.9/codefly_cli/observability/v0/dependencies_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/observability/v0/inventory_pb2.py` & `codefly_cli-0.0.9/codefly_cli/observability/v0/inventory_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/observability/v0/logs_pb2.py` & `codefly_cli-0.0.9/codefly_cli/observability/v0/logs_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/observability/v0/metrics_pb2.py` & `codefly_cli-0.0.9/codefly_cli/observability/v0/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/observability/v0/sessions_pb2.py` & `codefly_cli-0.0.9/codefly_cli/observability/v0/sessions_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/services/agent/v0/__pycache__/agent_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/services/agent/v0/__pycache__/agent_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/services/agent/v0/__pycache__/communicate_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/services/agent/v0/__pycache__/communicate_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/services/agent/v0/agent_pb2.py` & `codefly_cli-0.0.9/codefly_cli/services/agent/v0/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/services/agent/v0/agent_pb2_grpc.py` & `codefly_cli-0.0.9/codefly_cli/services/agent/v0/agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/services/agent/v0/communicate_pb2.py` & `codefly_cli-0.0.9/codefly_cli/services/agent/v0/communicate_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/services/agent/v0/cyclonedx_pb2.py` & `codefly_cli-0.0.9/codefly_cli/services/agent/v0/cyclonedx_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/services/builder/v0/builder_pb2.py` & `codefly_cli-0.0.9/codefly_cli/services/builder/v0/builder_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/services/builder/v0/builder_pb2_grpc.py` & `codefly_cli-0.0.9/codefly_cli/services/builder/v0/builder_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/services/builder/v0/deployment_pb2.py` & `codefly_cli-0.0.9/codefly_cli/services/builder/v0/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/services/builder/v0/docker_pb2.py` & `codefly_cli-0.0.9/codefly_cli/services/builder/v0/docker_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/services/runtime/v0/__pycache__/runtime_pb2.cpython-310.pyc` & `codefly_cli-0.0.9/codefly_cli/services/runtime/v0/__pycache__/runtime_pb2.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/services/runtime/v0/runtime_pb2.py` & `codefly_cli-0.0.9/codefly_cli/services/runtime/v0/runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py` & `codefly_cli-0.0.9/codefly_cli/services/runtime/v0/runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/codefly_cli/tests/__pycache__/test_cli.cpython-310-pytest-8.2.0.pyc` & `codefly_cli-0.0.9/codefly_cli/tests/__pycache__/test_cli.cpython-310-pytest-8.2.0.pyc`

 * *Files identical despite different names*

### Comparing `codefly_cli-0.0.8/PKG-INFO` & `codefly_cli-0.0.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codefly-cli
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: Antoine Toussaint
 Author-email: antoine.toussaint@codefly.ai
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

