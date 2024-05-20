# Comparing `tmp/weaviate_client-4.6.3.tar.gz` & `tmp/weaviate_client-4.7.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weaviate_client-4.6.3.tar", last modified: Mon May 20 17:27:58 2024, max compression
+gzip compressed data, was "weaviate_client-4.7.0a0.tar", last modified: Fri May 17 21:34:32 2024, max compression
```

## Comparing `weaviate_client-4.6.3.tar` & `weaviate_client-4.7.0a0.tar`

### file list

```diff
@@ -1,425 +1,425 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.358898 weaviate_client-4.6.3/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.302897 weaviate_client-4.6.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.302897 weaviate_client-4.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/.github/workflows/main.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    19131 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-20 17:27:58.358898 weaviate_client-4.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.302897 weaviate_client-4.6.3/ci/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/ci/compose.sh
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/ci/docker-compose-async.yml
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/ci/docker-compose-azure.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/ci/docker-compose-cluster.yml
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/ci/docker-compose-generative.yml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/ci/docker-compose-okta-cc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/ci/docker-compose-okta-users.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/ci/docker-compose-proxy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/ci/docker-compose-rerank.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/ci/docker-compose-wcs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/ci/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.302897 weaviate_client-4.6.3/ci/proxy/
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/ci/proxy/envoy.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      922 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/ci/start_weaviate.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/ci/stop_weaviate.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.310897 weaviate_client-4.6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    57456 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.auth.rst
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.backup.rst
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.batch.rst
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.classification.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.client.rst
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.cluster.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.collections.aggregations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.collections.batch.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.collections.classes.rst
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.collections.grpc.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.collections.queries.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.collections.rst
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.connect.rst
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.contextionary.rst
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.data.references.rst
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.data.replication.rst
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.gql.rst
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.proto.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.proto.v1.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.rst
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.schema.properties.rst
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.schema.rst
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/docs/weaviate.util.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.314897 weaviate_client-4.6.3/integration/
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/1234.3gp
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)   172641 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/hobbits.mp4
--rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    19365 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_batch_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)    17338 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    78596 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    31180 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_collection_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_collection_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_collection_batch_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    35482 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_collection_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    27875 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_collection_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_collection_geo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_collection_get.py
--rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_collection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_collection_multi_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    18946 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_collection_nested.py
--rw-r--r--   0 runner    (1001) docker     (127)    25135 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_collection_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    41744 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_collection_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_collection_rerank.py
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_gql_raw_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    21986 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_named_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/test_tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration/weaviate-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.314897 weaviate_client-4.6.3/integration_embedded/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration_embedded/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration_embedded/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.314897 weaviate_client-4.6.3/integration_v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration_v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration_v3/people_schema.json
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration_v3/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration_v3/test_backup.py
--rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration_v3/test_backup_v4.py
--rw-r--r--   0 runner    (1001) docker     (127)    20525 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration_v3/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration_v3/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration_v3/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    31522 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration_v3/test_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration_v3/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration_v3/test_grcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration_v3/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration_v3/test_stress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/integration_v3/test_timeout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.318897 weaviate_client-4.6.3/mock_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/mock_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/mock_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/mock_tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/mock_tests/test_automatic_retries.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/mock_tests/test_batching_manual.py
--rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/mock_tests/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/mock_tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/mock_tests/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/mock_tests/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/mock_tests/test_resend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/mock_tests/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.318897 weaviate_client-4.6.3/profiling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/profiling/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/profiling/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/profiling/test_import_and_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/profiling/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/profiling/test_refs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/profiling/test_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/publishing.md
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/run-mypy.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-20 17:27:58.358898 weaviate_client-4.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.318897 weaviate_client-4.6.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.318897 weaviate_client-4.6.3/test/batch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/batch/test_requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.322897 weaviate_client-4.6.3/test/classification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19246 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/classification/test_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.322897 weaviate_client-4.6.3/test/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/cluster/test_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.322897 weaviate_client-4.6.3/test/collection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/collection/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/collection/test_aggregates.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/collection/test_byteops.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/collection/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/collection/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/collection/test_collection_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    37924 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/collection/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/collection/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/collection/test_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.322897 weaviate_client-4.6.3/test/connection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/connection/test_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.322897 weaviate_client-4.6.3/test/contextionary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/contextionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/contextionary/test_text2vec_contextionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.322897 weaviate_client-4.6.3/test/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.322897 weaviate_client-4.6.3/test/data/references/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/data/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/data/references/test_crud_references.py
--rw-r--r--   0 runner    (1001) docker     (127)    31268 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/data/test_crud_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.322897 weaviate_client-4.6.3/test/gql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/gql/test_aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)    46096 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/gql/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    33189 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/gql/test_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/gql/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.326897 weaviate_client-4.6.3/test/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.326897 weaviate_client-4.6.3/test/schema/properties/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/schema/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/schema/properties/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/schema/schema_company.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/schema/tenants.json
--rw-r--r--   0 runner    (1001) docker     (127)    25534 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/schema/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/test_embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/test_server_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    57211 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/test/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.326897 weaviate_client-4.6.3/weaviate/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.326897 weaviate_client-4.6.3/weaviate/backup/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/backup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26299 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/backup/backup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.326897 weaviate_client-4.6.3/weaviate/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74441 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/batch/crud_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/batch/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.330897 weaviate_client-4.6.3/weaviate/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/classes/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/classes/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/classes/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/classes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/classes/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/classes/generics.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/classes/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/classes/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/classes/tenants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.330897 weaviate_client-4.6.3/weaviate/classification/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/classification/classification.py
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/classification/config_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    22104 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.330897 weaviate_client-4.6.3/weaviate/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/cluster/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.334897 weaviate_client-4.6.3/weaviate/collections/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/aggregate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.334897 weaviate_client-4.6.3/weaviate/collections/aggregations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/aggregations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/aggregations/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/aggregations/hybrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/aggregations/near_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/aggregations/near_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/aggregations/near_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/aggregations/near_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/aggregations/over_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/backups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.334897 weaviate_client-4.6.3/weaviate/collections/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27776 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/batch/batch_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/batch/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/batch/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/batch/grpc_batch_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/batch/grpc_batch_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/batch/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.338897 weaviate_client-4.6.3/weaviate/collections/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15550 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/classes/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/classes/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/classes/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    70855 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/classes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/classes/config_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13396 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/classes/config_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    41098 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/classes/config_named_vectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3836 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/classes/config_vector_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    40850 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/classes/config_vectorizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/classes/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    21511 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/classes/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/classes/grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    19528 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/classes/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/classes/orm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/classes/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/classes/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    15295 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    26760 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.338897 weaviate_client-4.6.3/weaviate/collections/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28488 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/grpc/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/grpc/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/grpc/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/iterator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.338897 weaviate_client-4.6.3/weaviate/collections/queries/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24324 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.338897 weaviate_client-4.6.3/weaviate/collections/queries/bm25/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/bm25/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/bm25/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/bm25/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/bm25/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/bm25/query.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/byteops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.338897 weaviate_client-4.6.3/weaviate/collections/queries/fetch_object_by_id/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/fetch_object_by_id/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/fetch_object_by_id/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/fetch_object_by_id/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.342897 weaviate_client-4.6.3/weaviate/collections/queries/fetch_objects/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/fetch_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/fetch_objects/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/fetch_objects/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/fetch_objects/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/fetch_objects/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.342897 weaviate_client-4.6.3/weaviate/collections/queries/hybrid/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/hybrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/hybrid/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12154 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/hybrid/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6337 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/hybrid/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/hybrid/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.342897 weaviate_client-4.6.3/weaviate/collections/queries/near_image/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_image/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_image/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_image/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9473 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_image/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.342897 weaviate_client-4.6.3/weaviate/collections/queries/near_media/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_media/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_media/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5747 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_media/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9877 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_media/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.342897 weaviate_client-4.6.3/weaviate/collections/queries/near_object/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_object/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10965 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_object/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_object/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_object/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.346897 weaviate_client-4.6.3/weaviate/collections/queries/near_text/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_text/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_text/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_text/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    10236 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_text/query.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.346897 weaviate_client-4.6.3/weaviate/collections/queries/near_vector/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_vector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5750 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_vector/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11043 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_vector/generate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_vector/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     9197 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/queries/near_vector/query.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/collections/tenants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.346897 weaviate_client-4.6.3/weaviate/connect/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/connect/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/connect/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/connect/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/connect/integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)    24991 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/connect/v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    28105 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/connect/v4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.346897 weaviate_client-4.6.3/weaviate/contextionary/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/contextionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/contextionary/crud_contextionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.346897 weaviate_client-4.6.3/weaviate/data/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38789 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/data/crud_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.346897 weaviate_client-4.6.3/weaviate/data/references/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/data/references/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27102 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/data/references/crud_references.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.346897 weaviate_client-4.6.3/weaviate/data/replication/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/data/replication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/data/replication/replication.py
--rw-r--r--   0 runner    (1001) docker     (127)    12458 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/error_msgs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.350897 weaviate_client-4.6.3/weaviate/gql/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42084 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/gql/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)    36163 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/gql/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)    75456 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/gql/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/gql/multi_get.py
--rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/gql/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/integrations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.350897 weaviate_client-4.6.3/weaviate/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/outputs/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/outputs/backup.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/outputs/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/outputs/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/outputs/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/outputs/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/outputs/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/outputs/tenants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.350897 weaviate_client-4.6.3/weaviate/proto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.354897 weaviate_client-4.6.3/weaviate/proto/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/base_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/base_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/batch_delete_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/batch_delete_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/batch_delete_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/batch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/batch_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/batch_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/properties_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/properties_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/properties_pb2_grpc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      391 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/regen.sh
--rw-r--r--   0 runner    (1001) docker     (127)    18051 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/search_get_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    29649 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/search_get_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/search_get_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/tenants_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/tenants_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/tenants_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/weaviate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/weaviate_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/proto/v1/weaviate_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.354897 weaviate_client-4.6.3/weaviate/schema/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34232 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/schema/crud_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.354897 weaviate_client-4.6.3/weaviate/schema/properties/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/schema/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/schema/properties/crud_properties.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28584 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/validator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11696 2024-05-20 17:27:27.000000 weaviate_client-4.6.3/weaviate/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 17:27:58.354897 weaviate_client-4.6.3/weaviate_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-20 17:27:58.000000 weaviate_client-4.6.3/weaviate_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-20 17:27:58.000000 weaviate_client-4.6.3/weaviate_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 17:27:58.000000 weaviate_client-4.6.3/weaviate_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 17:27:57.000000 weaviate_client-4.6.3/weaviate_client.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-20 17:27:58.000000 weaviate_client-4.6.3/weaviate_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 17:27:58.000000 weaviate_client-4.6.3/weaviate_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.847189 weaviate_client-4.7.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.787190 weaviate_client-4.7.0a0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.787190 weaviate_client-4.7.0a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)    12730 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/.github/workflows/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19131 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-17 21:34:32.847189 weaviate_client-4.7.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.791190 weaviate_client-4.7.0a0/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/ci/compose.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/ci/docker-compose-async.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/ci/docker-compose-azure.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/ci/docker-compose-cluster.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/ci/docker-compose-generative.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/ci/docker-compose-okta-cc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/ci/docker-compose-okta-users.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/ci/docker-compose-proxy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/ci/docker-compose-rerank.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/ci/docker-compose-wcs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/ci/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.791190 weaviate_client-4.7.0a0/ci/proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/ci/proxy/envoy.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      922 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/ci/start_weaviate.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      137 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/ci/stop_weaviate.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.795189 weaviate_client-4.7.0a0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    57214 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.auth.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.backup.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.batch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.classification.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.cluster.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.collections.aggregations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.collections.batch.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.collections.classes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.collections.grpc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.collections.queries.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.collections.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.connect.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.contextionary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.data.references.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.data.replication.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.gql.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.proto.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.proto.v1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.schema.properties.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.schema.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/docs/weaviate.util.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.799189 weaviate_client-4.7.0a0/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/1234.3gp
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7615 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)   172641 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/hobbits.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19365 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_batch_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17338 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78596 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31180 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_collection_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_collection_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_collection_batch_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34388 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_collection_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27875 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_collection_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_collection_geo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_collection_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_collection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_collection_multi_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18946 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_collection_nested.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25135 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_collection_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41744 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_collection_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_collection_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_gql_raw_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21762 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_named_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12623 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/test_tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6469 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration/weaviate-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.799189 weaviate_client-4.7.0a0/integration_embedded/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration_embedded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration_embedded/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.803190 weaviate_client-4.7.0a0/integration_v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration_v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration_v3/people_schema.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration_v3/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12340 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration_v3/test_backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15214 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration_v3/test_backup_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20525 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration_v3/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration_v3/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration_v3/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31522 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration_v3/test_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration_v3/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4740 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration_v3/test_grcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration_v3/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration_v3/test_stress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/integration_v3/test_timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.803190 weaviate_client-4.7.0a0/mock_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/mock_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/mock_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/mock_tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/mock_tests/test_automatic_retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/mock_tests/test_batching_manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12296 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/mock_tests/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/mock_tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/mock_tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/mock_tests/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/mock_tests/test_resend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/mock_tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.807190 weaviate_client-4.7.0a0/profiling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/profiling/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19458 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/profiling/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/profiling/test_import_and_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8349 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/profiling/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9294 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/profiling/test_refs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/profiling/test_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/publishing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      245 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/run-mypy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-17 21:34:32.847189 weaviate_client-4.7.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.807190 weaviate_client-4.7.0a0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.807190 weaviate_client-4.7.0a0/test/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12638 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/batch/test_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.807190 weaviate_client-4.7.0a0/test/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19246 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/classification/test_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.807190 weaviate_client-4.7.0a0/test/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/cluster/test_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.811190 weaviate_client-4.7.0a0/test/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/collection/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/collection/test_aggregates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/collection/test_byteops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/collection/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/collection/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/collection/test_collection_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37924 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/collection/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/collection/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/collection/test_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.811190 weaviate_client-4.7.0a0/test/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/connection/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.811190 weaviate_client-4.7.0a0/test/contextionary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/contextionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/contextionary/test_text2vec_contextionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.811190 weaviate_client-4.7.0a0/test/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.811190 weaviate_client-4.7.0a0/test/data/references/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/data/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12887 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/data/references/test_crud_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31268 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/data/test_crud_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.811190 weaviate_client-4.7.0a0/test/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/gql/test_aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46096 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/gql/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33189 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/gql/test_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/gql/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.811190 weaviate_client-4.7.0a0/test/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.811190 weaviate_client-4.7.0a0/test/schema/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/schema/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/schema/properties/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/schema/schema_company.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/schema/tenants.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25534 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/schema/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13342 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/test_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/test_server_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57211 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/test/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.815189 weaviate_client-4.7.0a0/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.815189 weaviate_client-4.7.0a0/weaviate/backup/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/backup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26299 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/backup/backup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.815189 weaviate_client-4.7.0a0/weaviate/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74441 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/batch/crud_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10961 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/batch/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.819189 weaviate_client-4.7.0a0/weaviate/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/classes/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/classes/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/classes/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/classes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/classes/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/classes/generics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/classes/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/classes/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/classes/tenants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.819189 weaviate_client-4.7.0a0/weaviate/classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4265 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/classification/classification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/classification/config_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22104 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.819189 weaviate_client-4.7.0a0/weaviate/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/cluster/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.819189 weaviate_client-4.7.0a0/weaviate/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/aggregate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.823189 weaviate_client-4.7.0a0/weaviate/collections/aggregations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/aggregations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/aggregations/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/aggregations/hybrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/aggregations/near_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4115 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/aggregations/near_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/aggregations/near_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/aggregations/near_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/aggregations/over_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/backups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.823189 weaviate_client-4.7.0a0/weaviate/collections/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27776 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/batch/batch_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8636 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/batch/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/batch/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/batch/grpc_batch_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/batch/grpc_batch_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/batch/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.827189 weaviate_client-4.7.0a0/weaviate/collections/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15550 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/classes/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/classes/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/classes/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70969 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/classes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/classes/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13424 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/classes/config_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41098 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/classes/config_named_vectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/classes/config_vector_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40850 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/classes/config_vectorizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/classes/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21511 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/classes/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11942 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/classes/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19528 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/classes/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/classes/orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/classes/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/classes/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13400 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15295 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12632 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27210 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.827189 weaviate_client-4.7.0a0/weaviate/collections/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28934 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/grpc/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/grpc/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/grpc/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/iterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11785 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.827189 weaviate_client-4.7.0a0/weaviate/collections/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24324 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.827189 weaviate_client-4.7.0a0/weaviate/collections/queries/bm25/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/bm25/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6031 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/bm25/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10501 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/bm25/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/bm25/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8655 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/bm25/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/byteops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.831189 weaviate_client-4.7.0a0/weaviate/collections/queries/fetch_object_by_id/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/fetch_object_by_id/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/fetch_object_by_id/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/fetch_object_by_id/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.831189 weaviate_client-4.7.0a0/weaviate/collections/queries/fetch_objects/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/fetch_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/fetch_objects/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/fetch_objects/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/fetch_objects/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/fetch_objects/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.831189 weaviate_client-4.7.0a0/weaviate/collections/queries/hybrid/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/hybrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/hybrid/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12377 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/hybrid/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6362 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/hybrid/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10529 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/hybrid/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.831189 weaviate_client-4.7.0a0/weaviate/collections/queries/near_image/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_image/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11541 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_image/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5659 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_image/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9695 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_image/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.831189 weaviate_client-4.7.0a0/weaviate/collections/queries/near_media/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_media/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11945 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_media/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_media/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_media/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.835189 weaviate_client-4.7.0a0/weaviate/collections/queries/near_object/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_object/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_object/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_object/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9335 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_object/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.835189 weaviate_client-4.7.0a0/weaviate/collections/queries/near_text/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_text/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12300 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_text/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5637 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_text/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10452 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_text/query.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.835189 weaviate_client-4.7.0a0/weaviate/collections/queries/near_vector/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_vector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_vector/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_vector/generate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_vector/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9413 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/queries/near_vector/query.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12067 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/collections/tenants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.835189 weaviate_client-4.7.0a0/weaviate/connect/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/connect/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/connect/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18036 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/connect/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5742 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/connect/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24991 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/connect/v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28105 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/connect/v4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.839189 weaviate_client-4.7.0a0/weaviate/contextionary/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/contextionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/contextionary/crud_contextionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.839189 weaviate_client-4.7.0a0/weaviate/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38789 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/data/crud_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.839189 weaviate_client-4.7.0a0/weaviate/data/references/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/data/references/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27102 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/data/references/crud_references.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.839189 weaviate_client-4.7.0a0/weaviate/data/replication/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/data/replication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/data/replication/replication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12458 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/embedded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/error_msgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10659 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.839189 weaviate_client-4.7.0a0/weaviate/gql/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42084 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/gql/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36163 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/gql/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75456 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/gql/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/gql/multi_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4906 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/gql/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/integrations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.839189 weaviate_client-4.7.0a0/weaviate/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/outputs/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/outputs/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/outputs/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/outputs/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/outputs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/outputs/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/outputs/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/outputs/tenants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.843189 weaviate_client-4.7.0a0/weaviate/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.847189 weaviate_client-4.7.0a0/weaviate/proto/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8385 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/base_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13054 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/base_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/batch_delete_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/batch_delete_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/batch_delete_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/batch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/batch_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/batch_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/properties_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/properties_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/properties_pb2_grpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      391 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/regen.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    18051 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/search_get_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29649 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/search_get_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/search_get_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/tenants_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/tenants_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/tenants_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/weaviate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/weaviate_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7590 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/proto/v1/weaviate_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.847189 weaviate_client-4.7.0a0/weaviate/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34232 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/schema/crud_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.847189 weaviate_client-4.7.0a0/weaviate/schema/properties/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/schema/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/schema/properties/crud_properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28584 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11696 2024-05-17 21:34:10.000000 weaviate_client-4.7.0a0/weaviate/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 21:34:32.847189 weaviate_client-4.7.0a0/weaviate_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-17 21:34:32.000000 weaviate_client-4.7.0a0/weaviate_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11952 2024-05-17 21:34:32.000000 weaviate_client-4.7.0a0/weaviate_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:34:32.000000 weaviate_client-4.7.0a0/weaviate_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 21:34:32.000000 weaviate_client-4.7.0a0/weaviate_client.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-17 21:34:32.000000 weaviate_client-4.7.0a0/weaviate_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 21:34:32.000000 weaviate_client-4.7.0a0/weaviate_client.egg-info/top_level.txt
```

### Comparing `weaviate_client-4.6.3/.flake8` & `weaviate_client-4.7.0a0/.flake8`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/.github/workflows/main.yaml` & `weaviate_client-4.7.0a0/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/.pre-commit-config.yaml` & `weaviate_client-4.7.0a0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/.pylintrc` & `weaviate_client-4.7.0a0/.pylintrc`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/CONTRIBUTING.md` & `weaviate_client-4.7.0a0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/LICENSE` & `weaviate_client-4.7.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/PKG-INFO` & `weaviate_client-4.7.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weaviate-client
-Version: 4.6.3
+Version: 4.7.0a0
 Summary: A python native Weaviate client
 Home-page: https://github.com/weaviate/weaviate-python-client
 Author: Weaviate
 Author-email: hello@weaviate.io,
 License: BSD 3-clause
 Project-URL: Documentation, https://weaviate-python-client.readthedocs.io
 Project-URL: Source, https://github.com/weaviate/weaviate-python-client
```

### Comparing `weaviate_client-4.6.3/README.rst` & `weaviate_client-4.7.0a0/README.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/ci/docker-compose-async.yml` & `weaviate_client-4.7.0a0/ci/docker-compose-async.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/ci/docker-compose-azure.yml` & `weaviate_client-4.7.0a0/ci/docker-compose-azure.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/ci/docker-compose-cluster.yml` & `weaviate_client-4.7.0a0/ci/docker-compose-cluster.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/ci/docker-compose-generative.yml` & `weaviate_client-4.7.0a0/ci/docker-compose-generative.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/ci/docker-compose-okta-cc.yml` & `weaviate_client-4.7.0a0/ci/docker-compose-okta-cc.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/ci/docker-compose-okta-users.yml` & `weaviate_client-4.7.0a0/ci/docker-compose-okta-users.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/ci/docker-compose-proxy.yml` & `weaviate_client-4.7.0a0/ci/docker-compose-proxy.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/ci/docker-compose-rerank.yml` & `weaviate_client-4.7.0a0/ci/docker-compose-rerank.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/ci/docker-compose-wcs.yml` & `weaviate_client-4.7.0a0/ci/docker-compose-wcs.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/ci/docker-compose.yml` & `weaviate_client-4.7.0a0/ci/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/ci/proxy/envoy.yaml` & `weaviate_client-4.7.0a0/ci/proxy/envoy.yaml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/ci/start_weaviate.sh` & `weaviate_client-4.7.0a0/ci/start_weaviate.sh`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/docs/Makefile` & `weaviate_client-4.7.0a0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/docs/README.rst` & `weaviate_client-4.7.0a0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/docs/changelog.rst` & `weaviate_client-4.7.0a0/docs/changelog.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 Changelog
 =========
-Version 4.6.3
---------------
-This patch version includes:
-    - Removal of top-level validation of ``vector`` in ``data.insert``, ``data.replace``, and ``data.update``. This validation occurs within the ``_get_vector_v4`` method now instead.
 
 Version 4.6.2
 --------------
 This patch version includes:
   - Respect default vectorizer
   - Wait for Weaviate 1.25 to be ready before starting the embedded client
   - Add missing models for voyageai
```

### Comparing `weaviate_client-4.6.3/docs/conf.py` & `weaviate_client-4.7.0a0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/docs/index.rst` & `weaviate_client-4.7.0a0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/docs/make.bat` & `weaviate_client-4.7.0a0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/docs/weaviate.classification.rst` & `weaviate_client-4.7.0a0/docs/weaviate.classification.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/docs/weaviate.collections.aggregations.rst` & `weaviate_client-4.7.0a0/docs/weaviate.collections.aggregations.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/docs/weaviate.collections.batch.rst` & `weaviate_client-4.7.0a0/docs/weaviate.collections.batch.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/docs/weaviate.collections.classes.rst` & `weaviate_client-4.7.0a0/docs/weaviate.collections.classes.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/docs/weaviate.collections.grpc.rst` & `weaviate_client-4.7.0a0/docs/weaviate.collections.grpc.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/docs/weaviate.collections.queries.rst` & `weaviate_client-4.7.0a0/docs/weaviate.collections.queries.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/docs/weaviate.collections.rst` & `weaviate_client-4.7.0a0/docs/weaviate.collections.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/docs/weaviate.connect.rst` & `weaviate_client-4.7.0a0/docs/weaviate.connect.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/docs/weaviate.gql.rst` & `weaviate_client-4.7.0a0/docs/weaviate.gql.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/docs/weaviate.proto.v1.rst` & `weaviate_client-4.7.0a0/docs/weaviate.proto.v1.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/docs/weaviate.rst` & `weaviate_client-4.7.0a0/docs/weaviate.rst`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/1234.3gp` & `weaviate_client-4.7.0a0/integration/1234.3gp`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/conftest.py` & `weaviate_client-4.7.0a0/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/constants.py` & `weaviate_client-4.7.0a0/integration/constants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/hobbits.mp4` & `weaviate_client-4.7.0a0/integration/hobbits.mp4`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_auth.py` & `weaviate_client-4.7.0a0/integration/test_auth.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_batch_v4.py` & `weaviate_client-4.7.0a0/integration/test_batch_v4.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_client.py` & `weaviate_client-4.7.0a0/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_collection.py` & `weaviate_client-4.7.0a0/integration/test_collection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_collection_aggregate.py` & `weaviate_client-4.7.0a0/integration/test_collection_aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_collection_batch.py` & `weaviate_client-4.7.0a0/integration/test_collection_batch.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_collection_batch_delete.py` & `weaviate_client-4.7.0a0/integration/test_collection_batch_delete.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_collection_config.py` & `weaviate_client-4.7.0a0/integration/test_collection_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -447,15 +447,14 @@
     )
     if collection._connection._weaviate_version.is_lower_than(1, 24, 0):
         pytest.skip("BQ+HNSW is not supported in Weaviate versions lower than 1.24.0")
 
     config = collection.config.get()
     assert config.vector_index_type == VectorIndexType.HNSW
     assert config.vector_index_config is not None
-    assert isinstance(config.vector_index_config, _VectorIndexConfigHNSW)
     assert isinstance(config.vector_index_config.quantizer, _BQConfig)
 
 
 def test_update_flat(collection_factory: CollectionFactory) -> None:
     collection = collection_factory(
         vector_index_config=Configure.VectorIndex.flat(
             vector_cache_max_objects=5,
@@ -757,63 +756,44 @@
         pytest.skip("Dynamic index is not supported in Weaviate versions lower than 1.25.0")
 
     collection = collection_factory(
         vector_index_config=Configure.VectorIndex.dynamic(
             distance_metric=VectorDistances.COSINE,
             threshold=1000,
             hnsw=Configure.VectorIndex.hnsw(
-                cleanup_interval_seconds=123,
-                flat_search_cutoff=1234,
-                vector_cache_max_objects=789,
-                quantizer=Configure.VectorIndex.Quantizer.pq(centroids=128),
-            ),
-            flat=Configure.VectorIndex.flat(
-                vector_cache_max_objects=7643,
-                quantizer=Configure.VectorIndex.Quantizer.bq(rescore_limit=10),
+                cleanup_interval_seconds=123, flat_search_cutoff=1234, vector_cache_max_objects=789
             ),
+            flat=Configure.VectorIndex.flat(vector_cache_max_objects=7643),
         ),
         ports=(8090, 50061),
     )
 
     config = collection.config.get()
     assert isinstance(config.vector_index_config, _VectorIndexConfigDynamic)
     assert config.vector_index_config.distance_metric == VectorDistances.COSINE
     assert config.vector_index_config.threshold == 1000
     assert isinstance(config.vector_index_config.hnsw, _VectorIndexConfigHNSW)
     assert config.vector_index_config.hnsw.cleanup_interval_seconds == 123
     assert config.vector_index_config.hnsw.flat_search_cutoff == 1234
     assert config.vector_index_config.hnsw.vector_cache_max_objects == 789
-    assert isinstance(config.vector_index_config.hnsw.quantizer, _PQConfig)
-    assert config.vector_index_config.hnsw.quantizer.centroids == 128
     assert isinstance(config.vector_index_config.flat, _VectorIndexConfigFlat)
     assert config.vector_index_config.flat.vector_cache_max_objects == 7643
-    assert isinstance(config.vector_index_config.flat.quantizer, _BQConfig)
-    assert config.vector_index_config.flat.quantizer.rescore_limit == 10
 
     collection.config.update(
         vectorizer_config=Reconfigure.VectorIndex.dynamic(
             threshold=2000,
             hnsw=Reconfigure.VectorIndex.hnsw(
-                flat_search_cutoff=4567,
-                vector_cache_max_objects=678,
-                quantizer=Reconfigure.VectorIndex.Quantizer.pq(centroids=128),
-            ),
-            flat=Reconfigure.VectorIndex.flat(
-                vector_cache_max_objects=9876,
-                quantizer=Reconfigure.VectorIndex.Quantizer.bq(rescore_limit=11),
+                flat_search_cutoff=4567, vector_cache_max_objects=678
             ),
+            flat=Reconfigure.VectorIndex.flat(vector_cache_max_objects=9876),
         ),
     )
     config = collection.config.get()
     assert isinstance(config.vector_index_config, _VectorIndexConfigDynamic)
     assert config.vector_index_config.distance_metric == VectorDistances.COSINE
     assert config.vector_index_config.threshold == 2000
     assert isinstance(config.vector_index_config.hnsw, _VectorIndexConfigHNSW)
     assert config.vector_index_config.hnsw.cleanup_interval_seconds == 123
     assert config.vector_index_config.hnsw.flat_search_cutoff == 4567
     assert config.vector_index_config.hnsw.vector_cache_max_objects == 678
-    assert isinstance(config.vector_index_config.hnsw.quantizer, _PQConfig)
-    assert config.vector_index_config.hnsw.quantizer.centroids == 128
     assert isinstance(config.vector_index_config.flat, _VectorIndexConfigFlat)
     assert config.vector_index_config.flat.vector_cache_max_objects == 9876
-    assert isinstance(config.vector_index_config.flat.quantizer, _BQConfig)
-    assert config.vector_index_config.flat.quantizer.rescore_limit == 11
```

### Comparing `weaviate_client-4.6.3/integration/test_collection_filter.py` & `weaviate_client-4.7.0a0/integration/test_collection_filter.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_collection_geo.py` & `weaviate_client-4.7.0a0/integration/test_collection_geo.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_collection_get.py` & `weaviate_client-4.7.0a0/integration/test_collection_get.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_collection_model.py` & `weaviate_client-4.7.0a0/integration/test_collection_model.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_collection_multi_node.py` & `weaviate_client-4.7.0a0/integration/test_collection_multi_node.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_collection_nested.py` & `weaviate_client-4.7.0a0/integration/test_collection_nested.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_collection_openai.py` & `weaviate_client-4.7.0a0/integration/test_collection_openai.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_collection_references.py` & `weaviate_client-4.7.0a0/integration/test_collection_references.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_collection_rerank.py` & `weaviate_client-4.7.0a0/integration/test_collection_rerank.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_gql_raw_v4.py` & `weaviate_client-4.7.0a0/integration/test_gql_raw_v4.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_iterator.py` & `weaviate_client-4.7.0a0/integration/test_iterator.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/test_named_vectors.py` & `weaviate_client-4.7.0a0/integration/test_named_vectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import pytest
 import weaviate.classes as wvc
 
 from weaviate.collections.classes.data import DataObject
 
 from weaviate.collections.classes.config import (
     PQConfig,
-    _VectorIndexConfigHNSW,
     _VectorIndexConfigFlat,
     Vectorizers,
 )
 
 from weaviate.collections.classes.aggregate import AggregateInteger
 
 from weaviate.exceptions import WeaviateInvalidInputError
@@ -471,15 +470,14 @@
             ),
         ],
     )
     config = collection.config.get()
     assert config.vector_config is not None
     assert config.vector_config["first"].vector_index_config is not None
     assert config.vector_config["second"].vector_index_config is not None
-    assert isinstance(config.vector_config["second"].vector_index_config, _VectorIndexConfigHNSW)
     assert config.vector_config["second"].vector_index_config.quantizer is None
 
     collection.config.update(
         vectorizer_config=[
             wvc.config.Reconfigure.NamedVectors.update(
                 name="second",
                 vector_index_config=wvc.config.Reconfigure.VectorIndex.hnsw(
@@ -488,15 +486,14 @@
             )
         ]
     )
     config = collection.config.get()
     assert config.vector_config is not None
     assert config.vector_config["first"].vector_index_config is not None
     assert config.vector_config["second"].vector_index_config is not None
-    assert isinstance(config.vector_config["second"].vector_index_config, _VectorIndexConfigHNSW)
     assert isinstance(config.vector_config["second"].vector_index_config.quantizer, PQConfig)
     assert config.vector_config["second"].vector_index_config.quantizer.centroids == 256
 
 
 # def test_update_to_change_quantizer_from_pq_to_bq_on_specific_named_vector(
 #     collection_factory: CollectionFactory,
 # ) -> None:
```

### Comparing `weaviate_client-4.6.3/integration/test_tenants.py` & `weaviate_client-4.7.0a0/integration/test_tenants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration/weaviate-logo.png` & `weaviate_client-4.7.0a0/integration/weaviate-logo.png`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration_embedded/test_client.py` & `weaviate_client-4.7.0a0/integration_embedded/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration_v3/people_schema.json` & `weaviate_client-4.7.0a0/integration_v3/people_schema.json`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration_v3/test_authentication.py` & `weaviate_client-4.7.0a0/integration_v3/test_authentication.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration_v3/test_backup.py` & `weaviate_client-4.7.0a0/integration_v3/test_backup.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration_v3/test_backup_v4.py` & `weaviate_client-4.7.0a0/integration_v3/test_backup_v4.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration_v3/test_batch.py` & `weaviate_client-4.7.0a0/integration_v3/test_batch.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration_v3/test_classification.py` & `weaviate_client-4.7.0a0/integration_v3/test_classification.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration_v3/test_cluster.py` & `weaviate_client-4.7.0a0/integration_v3/test_cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration_v3/test_crud.py` & `weaviate_client-4.7.0a0/integration_v3/test_crud.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration_v3/test_graphql.py` & `weaviate_client-4.7.0a0/integration_v3/test_graphql.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration_v3/test_grcp.py` & `weaviate_client-4.7.0a0/integration_v3/test_grcp.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration_v3/test_schema.py` & `weaviate_client-4.7.0a0/integration_v3/test_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration_v3/test_stress.py` & `weaviate_client-4.7.0a0/integration_v3/test_stress.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/integration_v3/test_timeout.py` & `weaviate_client-4.7.0a0/integration_v3/test_timeout.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/mock_tests/conftest.py` & `weaviate_client-4.7.0a0/mock_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/mock_tests/test_auth.py` & `weaviate_client-4.7.0a0/mock_tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/mock_tests/test_automatic_retries.py` & `weaviate_client-4.7.0a0/mock_tests/test_automatic_retries.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/mock_tests/test_batching_manual.py` & `weaviate_client-4.7.0a0/mock_tests/test_batching_manual.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/mock_tests/test_collection.py` & `weaviate_client-4.7.0a0/mock_tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/mock_tests/test_connection.py` & `weaviate_client-4.7.0a0/mock_tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/mock_tests/test_exception.py` & `weaviate_client-4.7.0a0/mock_tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/mock_tests/test_graphql.py` & `weaviate_client-4.7.0a0/mock_tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/mock_tests/test_resend.py` & `weaviate_client-4.7.0a0/mock_tests/test_resend.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/mock_tests/test_schema.py` & `weaviate_client-4.7.0a0/mock_tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/profiling/conftest.py` & `weaviate_client-4.7.0a0/profiling/conftest.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/profiling/constants.py` & `weaviate_client-4.7.0a0/profiling/constants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/profiling/test_import_and_query.py` & `weaviate_client-4.7.0a0/profiling/test_import_and_query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/profiling/test_profiling.py` & `weaviate_client-4.7.0a0/profiling/test_profiling.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/profiling/test_refs.py` & `weaviate_client-4.7.0a0/profiling/test_refs.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/profiling/test_sphere.py` & `weaviate_client-4.7.0a0/profiling/test_sphere.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/publishing.md` & `weaviate_client-4.7.0a0/publishing.md`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/pyproject.toml` & `weaviate_client-4.7.0a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/requirements-devel.txt` & `weaviate_client-4.7.0a0/requirements-devel.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 setuptools_scm
 Sphinx>=7.0.0
 sphinx-rtd-theme==2.0.0
 autodoc-pydantic==2.2.0
 
 grpcio-tools
 
-pytest==8.2.1
+pytest==8.2.0
 pytest-cov==5.0.0
 pytest-benchmark==4.0.0
 pytest-profiling==1.7.0
 coverage==7.5.1
 pytest-xdist==3.6.1
 werkzeug>=2.3.7
 pytest-httpserver>=1.0.8
```

### Comparing `weaviate_client-4.6.3/setup.cfg` & `weaviate_client-4.7.0a0/setup.cfg`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/README.md` & `weaviate_client-4.7.0a0/test/README.md`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/batch/test_requests.py` & `weaviate_client-4.7.0a0/test/batch/test_requests.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/classification/test_classification.py` & `weaviate_client-4.7.0a0/test/classification/test_classification.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/cluster/test_cluster.py` & `weaviate_client-4.7.0a0/test/cluster/test_cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/collection/test_aggregates.py` & `weaviate_client-4.7.0a0/test/collection/test_aggregates.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/collection/test_byteops.py` & `weaviate_client-4.7.0a0/test/collection/test_byteops.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/collection/test_classes.py` & `weaviate_client-4.7.0a0/test/collection/test_classes.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/collection/test_client.py` & `weaviate_client-4.7.0a0/test/collection/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/collection/test_collection_model.py` & `weaviate_client-4.7.0a0/test/collection/test_collection_model.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/collection/test_config.py` & `weaviate_client-4.7.0a0/test/collection/test_config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/collection/test_filter.py` & `weaviate_client-4.7.0a0/test/collection/test_filter.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/collection/test_queries.py` & `weaviate_client-4.7.0a0/test/collection/test_queries.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/connection/test_connection.py` & `weaviate_client-4.7.0a0/test/connection/test_connection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/contextionary/test_text2vec_contextionary.py` & `weaviate_client-4.7.0a0/test/contextionary/test_text2vec_contextionary.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/data/references/test_crud_references.py` & `weaviate_client-4.7.0a0/test/data/references/test_crud_references.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/data/test_crud_data.py` & `weaviate_client-4.7.0a0/test/data/test_crud_data.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/gql/test_aggregate.py` & `weaviate_client-4.7.0a0/test/gql/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/gql/test_filter.py` & `weaviate_client-4.7.0a0/test/gql/test_filter.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/gql/test_get.py` & `weaviate_client-4.7.0a0/test/gql/test_get.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/gql/test_query.py` & `weaviate_client-4.7.0a0/test/gql/test_query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/schema/properties/test_properties.py` & `weaviate_client-4.7.0a0/test/schema/properties/test_properties.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/schema/schema_company.json` & `weaviate_client-4.7.0a0/test/schema/schema_company.json`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/schema/test_schema.py` & `weaviate_client-4.7.0a0/test/schema/test_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/test_auth.py` & `weaviate_client-4.7.0a0/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/test_client.py` & `weaviate_client-4.7.0a0/test/test_client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/test_embedded.py` & `weaviate_client-4.7.0a0/test/test_embedded.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/test_exceptions.py` & `weaviate_client-4.7.0a0/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/test_server_version.py` & `weaviate_client-4.7.0a0/test/test_server_version.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/test_util.py` & `weaviate_client-4.7.0a0/test/test_util.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/test/util.py` & `weaviate_client-4.7.0a0/test/util.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/__init__.py` & `weaviate_client-4.7.0a0/weaviate/__init__.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/auth.py` & `weaviate_client-4.7.0a0/weaviate/auth.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/backup/backup.py` & `weaviate_client-4.7.0a0/weaviate/backup/backup.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/batch/crud_batch.py` & `weaviate_client-4.7.0a0/weaviate/batch/crud_batch.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/batch/requests.py` & `weaviate_client-4.7.0a0/weaviate/batch/requests.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/classes/config.py` & `weaviate_client-4.7.0a0/weaviate/classes/config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/classes/query.py` & `weaviate_client-4.7.0a0/weaviate/classes/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/classification/classification.py` & `weaviate_client-4.7.0a0/weaviate/classification/classification.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/classification/config_builder.py` & `weaviate_client-4.7.0a0/weaviate/classification/config_builder.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/client.py` & `weaviate_client-4.7.0a0/weaviate/client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/cluster/cluster.py` & `weaviate_client-4.7.0a0/weaviate/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/cluster/types.py` & `weaviate_client-4.7.0a0/weaviate/cluster/types.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/aggregations/base.py` & `weaviate_client-4.7.0a0/weaviate/collections/aggregations/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/aggregations/hybrid.py` & `weaviate_client-4.7.0a0/weaviate/collections/aggregations/hybrid.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/aggregations/near_image.py` & `weaviate_client-4.7.0a0/weaviate/collections/aggregations/near_image.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/aggregations/near_object.py` & `weaviate_client-4.7.0a0/weaviate/collections/aggregations/near_object.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/aggregations/near_text.py` & `weaviate_client-4.7.0a0/weaviate/collections/aggregations/near_text.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/aggregations/near_vector.py` & `weaviate_client-4.7.0a0/weaviate/collections/aggregations/near_vector.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/aggregations/over_all.py` & `weaviate_client-4.7.0a0/weaviate/collections/aggregations/over_all.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/backups.py` & `weaviate_client-4.7.0a0/weaviate/collections/backups.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/base.py` & `weaviate_client-4.7.0a0/weaviate/collections/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/batch/base.py` & `weaviate_client-4.7.0a0/weaviate/collections/batch/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/batch/batch_wrapper.py` & `weaviate_client-4.7.0a0/weaviate/collections/batch/batch_wrapper.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/batch/client.py` & `weaviate_client-4.7.0a0/weaviate/collections/batch/client.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/batch/collection.py` & `weaviate_client-4.7.0a0/weaviate/collections/batch/collection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/batch/grpc_batch_delete.py` & `weaviate_client-4.7.0a0/weaviate/collections/batch/grpc_batch_delete.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/batch/grpc_batch_objects.py` & `weaviate_client-4.7.0a0/weaviate/collections/batch/grpc_batch_objects.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/batch/rest.py` & `weaviate_client-4.7.0a0/weaviate/collections/batch/rest.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/classes/aggregate.py` & `weaviate_client-4.7.0a0/weaviate/collections/classes/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/classes/batch.py` & `weaviate_client-4.7.0a0/weaviate/collections/classes/batch.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/classes/cluster.py` & `weaviate_client-4.7.0a0/weaviate/collections/classes/cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/classes/config.py` & `weaviate_client-4.7.0a0/weaviate/collections/classes/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1150,15 +1150,15 @@
         return VectorIndexType.FLAT.value
 
 
 VectorIndexConfigFlat = _VectorIndexConfigFlat
 
 
 @dataclass
-class _VectorIndexConfigDynamic(_ConfigBase):
+class _VectorIndexConfigDynamic(_VectorIndexConfig):
     distance_metric: VectorDistances
     hnsw: Optional[VectorIndexConfigHNSW]
     flat: Optional[VectorIndexConfigFlat]
     threshold: Optional[int]
 
     @staticmethod
     def vector_index_type() -> str:
@@ -1676,24 +1676,29 @@
 
     @staticmethod
     def dynamic(
         distance_metric: Optional[VectorDistances] = None,
         threshold: Optional[int] = None,
         hnsw: Optional[_VectorIndexConfigHNSWCreate] = None,
         flat: Optional[_VectorIndexConfigFlatCreate] = None,
+        quantizer: Optional[_BQConfigCreate] = None,
     ) -> _VectorIndexConfigDynamicCreate:
         """Create a `_VectorIndexConfigDynamicCreate` object to be used when defining the DYNAMIC vector index configuration of Weaviate.
 
         Use this method when defining the `vector_index_config` argument in `collections.create()`.
 
         Arguments:
             See [the docs](https://weaviate.io/developers/weaviate/configuration/indexes#how-to-configure-hnsw) for a more detailed view!
         """  # noqa: D417 (missing argument descriptions in the docstring)
         return _VectorIndexConfigDynamicCreate(
-            distance=distance_metric, threshold=threshold, hnsw=hnsw, flat=flat, quantizer=None
+            distance=distance_metric,
+            threshold=threshold,
+            hnsw=hnsw,
+            flat=flat,
+            quantizer=quantizer,
         )
 
 
 class Configure:
     """Use this factory class to generate the correct object for use when using the `collections.create()` method. E.g., `.multi_tenancy()` will return a `MultiTenancyConfigCreate` object to be used in the `multi_tenancy_config` argument.
 
     Each class method provides options specific to the named configuration type in the function's name. Under-the-hood data validation steps
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/classes/config_base.py` & `weaviate_client-4.7.0a0/weaviate/collections/classes/config_base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/classes/config_methods.py` & `weaviate_client-4.7.0a0/weaviate/collections/classes/config_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,14 +159,15 @@
         return __get_hnsw_config(schema["vectorIndexConfig"])
     elif schema["vectorIndexType"] == "flat":
         return __get_flat_config(schema["vectorIndexConfig"])
     elif schema["vectorIndexType"] == "dynamic":
         return _VectorIndexConfigDynamic(
             distance_metric=VectorDistances(schema["vectorIndexConfig"]["distance"]),
             threshold=schema["vectorIndexConfig"].get("threshold"),
+            quantizer=None,
             hnsw=__get_hnsw_config(schema["vectorIndexConfig"]["hnsw"]),
             flat=__get_flat_config(schema["vectorIndexConfig"]["flat"]),
         )
     else:
         return None
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/classes/config_named_vectors.py` & `weaviate_client-4.7.0a0/weaviate/collections/classes/config_named_vectors.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/classes/config_vector_index.py` & `weaviate_client-4.7.0a0/weaviate/collections/classes/config_vector_index.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,25 +112,14 @@
     hnsw: Optional[_VectorIndexConfigHNSWCreate]
     flat: Optional[_VectorIndexConfigFlatCreate]
 
     @staticmethod
     def vector_index_type() -> VectorIndexType:
         return VectorIndexType.DYNAMIC
 
-    def _to_dict(self) -> dict:
-        ret_dict = super()._to_dict()
-        if self.hnsw is not None:
-            ret_dict["hnsw"] = self.hnsw._to_dict()
-        if self.flat is not None:
-            ret_dict["flat"] = self.flat._to_dict()
-        if self.threshold is not None:
-            ret_dict["threshold"] = self.threshold
-
-        return ret_dict
-
 
 class _VectorIndexConfigDynamicUpdate(_VectorIndexConfigUpdate):
     threshold: Optional[int]
     hnsw: Optional[_VectorIndexConfigHNSWUpdate]
     flat: Optional[_VectorIndexConfigFlatUpdate]
 
     @staticmethod
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/classes/config_vectorizers.py` & `weaviate_client-4.7.0a0/weaviate/collections/classes/config_vectorizers.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/classes/data.py` & `weaviate_client-4.7.0a0/weaviate/collections/classes/data.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/classes/filters.py` & `weaviate_client-4.7.0a0/weaviate/collections/classes/filters.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/classes/grpc.py` & `weaviate_client-4.7.0a0/weaviate/collections/classes/grpc.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/classes/internal.py` & `weaviate_client-4.7.0a0/weaviate/collections/classes/internal.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/classes/orm.py` & `weaviate_client-4.7.0a0/weaviate/collections/classes/orm.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/classes/tenants.py` & `weaviate_client-4.7.0a0/weaviate/collections/classes/tenants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/classes/types.py` & `weaviate_client-4.7.0a0/weaviate/collections/classes/types.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/cluster.py` & `weaviate_client-4.7.0a0/weaviate/collections/cluster.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/collection.py` & `weaviate_client-4.7.0a0/weaviate/collections/collection.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/collections.py` & `weaviate_client-4.7.0a0/weaviate/collections/collections.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/config.py` & `weaviate_client-4.7.0a0/weaviate/collections/config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/data.py` & `weaviate_client-4.7.0a0/weaviate/collections/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,14 +369,17 @@
             _validate_input(
                 [
                     _ValidateArgument(expected=[UUID, None], name="uuid", value=uuid),
                     _ValidateArgument(expected=[Mapping], name="properties", value=properties),
                     _ValidateArgument(
                         expected=[Mapping, None], name="references", value=references
                     ),
+                    _ValidateArgument(
+                        expected=[Sequence, None, Mapping], name="vector", value=vector
+                    ),
                 ],
             )
         props = self._serialize_props(properties) if properties is not None else {}
         refs = self._serialize_refs(references) if references is not None else {}
         weaviate_obj: Dict[str, Any] = {
             "class": self.name,
             "properties": {**props, **refs},
@@ -471,14 +474,17 @@
             _validate_input(
                 [
                     _ValidateArgument(expected=[UUID], name="uuid", value=uuid),
                     _ValidateArgument(expected=[Mapping], name="properties", value=properties),
                     _ValidateArgument(
                         expected=[Mapping, None], name="references", value=references
                     ),
+                    _ValidateArgument(
+                        expected=[Sequence, None, Mapping], name="vector", value=vector
+                    ),
                 ]
             )
         props = self._serialize_props(properties) if properties is not None else {}
         refs = self._serialize_refs(references) if references is not None else {}
         weaviate_obj: Dict[str, Any] = {
             "class": self.name,
             "properties": {**props, **refs},
@@ -520,14 +526,17 @@
                     _ValidateArgument(expected=[UUID], name="uuid", value=uuid),
                     _ValidateArgument(
                         expected=[Mapping, None], name="properties", value=properties
                     ),
                     _ValidateArgument(
                         expected=[Mapping, None], name="references", value=references
                     ),
+                    _ValidateArgument(
+                        expected=[Sequence, None, Mapping], name="vector", value=vector
+                    ),
                 ],
             )
         props = self._serialize_props(properties) if properties is not None else {}
         refs = self._serialize_refs(references) if references is not None else {}
         weaviate_obj: Dict[str, Any] = {"class": self.name, "properties": {**props, **refs}}
         if vector is not None:
             weaviate_obj = self.__parse_vector(weaviate_obj, vector)
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/filters.py` & `weaviate_client-4.7.0a0/weaviate/collections/filters.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/grpc/query.py` & `weaviate_client-4.7.0a0/weaviate/collections/grpc/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-from dataclasses import dataclass
 import struct
+import uuid as uuid_lib
+from dataclasses import dataclass
 from typing import Any, Dict, List, Literal, Optional, Sequence, Set, TypeVar, Union, cast, Tuple
 
-from typing_extensions import TypeAlias
-
 import grpc  # type: ignore
-import uuid as uuid_lib
+from typing_extensions import TypeAlias
 
 from weaviate.collections.classes.config import ConsistencyLevel
-
 from weaviate.collections.classes.filters import _Filters
 from weaviate.collections.classes.grpc import (
     HybridFusion,
     _QueryReferenceMultiTarget,
     _MetadataQuery,
     _HybridNearText,
     _HybridNearVector,
@@ -25,27 +23,22 @@
     REFERENCE,
     REFERENCES,
     _Sorting,
     Rerank,
 )
 from weaviate.collections.classes.internal import _Generative, _GroupBy
 from weaviate.collections.filters import _FilterToGRPC
-
 from weaviate.collections.grpc.shared import _BaseGRPC
-
 from weaviate.connect import ConnectionV4
 from weaviate.exceptions import WeaviateQueryError, WeaviateUnsupportedFeatureError
+from weaviate.proto.v1 import search_get_pb2
 from weaviate.types import NUMBER, UUID
 from weaviate.util import _get_vector_v4
-
-from weaviate.proto.v1 import search_get_pb2
-
 from weaviate.validator import _ValidateArgument, _validate_input
 
-
 # Can be found in the google.protobuf.internal.well_known_types.pyi stub file but is defined explicitly here for clarity.
 _PyValue: TypeAlias = Union[
     Dict[str, "_PyValue"],
     List["_PyValue"],
     str,
     float,
     bool,
@@ -153,15 +146,15 @@
         filters: Optional[_Filters] = None,
         group_by: Optional[_GroupBy] = None,
         return_metadata: Optional[_MetadataQuery] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Optional[REFERENCES] = None,
         generative: Optional[_Generative] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
     ) -> search_get_pb2.SearchReply:
         if self._connection._weaviate_version.is_lower_than(1, 25, 0) and (
             isinstance(vector, _HybridNearText) or isinstance(vector, _HybridNearVector)
         ):
             raise WeaviateUnsupportedFeatureError(
                 "Hybrid search with NearText or NearVector",
                 str(self._connection._weaviate_version),
@@ -173,36 +166,39 @@
                     _ValidateArgument([None, str], "query", query),
                     _ValidateArgument([float, int, None], "alpha", alpha),
                     _ValidateArgument(
                         [list, _HybridNearText, _HybridNearVector, None], "vector", vector
                     ),
                     _ValidateArgument([List, None], "properties", properties),
                     _ValidateArgument([HybridFusion, None], "fusion_type", fusion_type),
-                    _ValidateArgument([str, None], "target_vector", target_vector),
+                    _ValidateArgument([str, List, None], "target_vector", target_vector),
                 ]
             )
 
         # Set hybrid search to only query the other search-type if one of the two is not set
         if query is None:
             alpha = 1
 
+        if target_vector is not None and isinstance(target_vector, str):
+            target_vector = [target_vector]
+
         hybrid_search = (
             search_get_pb2.Hybrid(
                 properties=properties,
                 query=query,
                 alpha=float(alpha) if alpha is not None else None,
                 fusion_type=(
                     cast(
                         search_get_pb2.Hybrid.FusionType,
                         search_get_pb2.Hybrid.FusionType.Value(fusion_type.value),
                     )
                     if fusion_type is not None
                     else None
                 ),
-                target_vectors=[target_vector] if target_vector is not None else None,
+                target_vectors=target_vector,
                 vector_bytes=(
                     struct.pack("{}f".format(len(vector)), *vector)
                     if vector is not None and isinstance(vector, list)
                     else None
                 ),
                 near_text=(
                     search_get_pb2.NearTextSearch(
@@ -297,30 +293,33 @@
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         autocut: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[_GroupBy] = None,
         generative: Optional[_Generative] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[List[str], str]] = None,
         return_metadata: Optional[_MetadataQuery] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Optional[REFERENCES] = None,
     ) -> search_get_pb2.SearchReply:
         if self._validate_arguments:
             _validate_input(
                 [
                     _ValidateArgument([List], "near_vector", near_vector),
-                    _ValidateArgument([str, None], "target_vector", target_vector),
+                    _ValidateArgument([str, List, None], "target_vector", target_vector),
                 ]
             )
 
         near_vector = _get_vector_v4(near_vector)
         certainty, distance = self.__parse_near_options(certainty, distance)
 
+        if target_vector is not None and isinstance(target_vector, str):
+            target_vector = [target_vector]
+
         request = self.__create_request(
             limit=limit,
             offset=offset,
             filters=filters,
             metadata=return_metadata,
             return_properties=return_properties,
             return_references=return_references,
@@ -328,15 +327,15 @@
             rerank=rerank,
             autocut=autocut,
             group_by=group_by,
             near_vector=search_get_pb2.NearVector(
                 certainty=certainty,
                 distance=distance,
                 vector_bytes=struct.pack("{}f".format(len(near_vector)), *near_vector),
-                target_vectors=[target_vector] if target_vector is not None else None,
+                target_vectors=target_vector,
             ),
         )
 
         return self.__call(request)
 
     def near_object(
         self,
@@ -346,29 +345,32 @@
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         autocut: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[_GroupBy] = None,
         generative: Optional[_Generative] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         return_metadata: Optional[_MetadataQuery] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Optional[REFERENCES] = None,
     ) -> search_get_pb2.SearchReply:
         if self._validate_arguments:
             _validate_input(
                 [
                     _ValidateArgument([str, uuid_lib.UUID], "near_object", near_object),
-                    _ValidateArgument([str, None], "target_vector", target_vector),
+                    _ValidateArgument([str, List, None], "target_vector", target_vector),
                 ]
             )
 
         certainty, distance = self.__parse_near_options(certainty, distance)
 
+        if target_vector is not None and isinstance(target_vector, str):
+            target_vector = [target_vector]
+
         base_request = self.__create_request(
             limit=limit,
             offset=offset,
             filters=filters,
             metadata=return_metadata,
             return_properties=return_properties,
             return_references=return_references,
@@ -376,15 +378,15 @@
             rerank=rerank,
             autocut=autocut,
             group_by=group_by,
             near_object=search_get_pb2.NearObject(
                 id=str(near_object),
                 certainty=certainty,
                 distance=distance,
-                target_vectors=[target_vector] if target_vector is not None else None,
+                target_vectors=target_vector,
             ),
         )
 
         return self.__call(base_request)
 
     def near_text(
         self,
@@ -396,38 +398,41 @@
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         autocut: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[_GroupBy] = None,
         generative: Optional[_Generative] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         return_metadata: Optional[_MetadataQuery] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Optional[REFERENCES] = None,
     ) -> search_get_pb2.SearchReply:
         if self._validate_arguments:
             _validate_input(
                 [
                     _ValidateArgument([List, str], "near_text", near_text),
                     _ValidateArgument([Move, None], "move_away", move_away),
                     _ValidateArgument([Move, None], "move_to", move_to),
-                    _ValidateArgument([str, None], "target_vector", target_vector),
+                    _ValidateArgument([str, List, None], "target_vector", target_vector),
                 ]
             )
 
         if isinstance(near_text, str):
             near_text = [near_text]
         certainty, distance = self.__parse_near_options(certainty, distance)
 
+        if target_vector is not None and isinstance(target_vector, str):
+            target_vector = [target_vector]
+
         near_text_req = search_get_pb2.NearTextSearch(
             query=near_text,
             certainty=certainty,
             distance=distance,
-            target_vectors=[target_vector] if target_vector is not None else None,
+            target_vectors=target_vector,
             move_away=self.__parse_move(move_away),
             move_to=self.__parse_move(move_to),
         )
 
         request = self.__create_request(
             limit=limit,
             offset=offset,
@@ -453,15 +458,15 @@
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         autocut: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[_GroupBy] = None,
         generative: Optional[_Generative] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         return_metadata: Optional[_MetadataQuery] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Optional[REFERENCES] = None,
     ) -> search_get_pb2.SearchReply:
         if self._validate_arguments:
             _validate_input(
                 [
@@ -469,39 +474,40 @@
                     _ValidateArgument([str, None], "target_vector", target_vector),
                 ]
             )
 
         certainty, distance = self.__parse_near_options(certainty, distance)
 
         kwargs: Dict[str, Any] = {}
-        target_vectors = [target_vector] if target_vector is not None else None
+        if target_vector is not None and isinstance(target_vector, str):
+            target_vector = [target_vector]
 
         if type_ == "audio":
             kwargs["near_audio"] = search_get_pb2.NearAudioSearch(
-                audio=media, distance=distance, certainty=certainty, target_vectors=target_vectors
+                audio=media, distance=distance, certainty=certainty, target_vectors=target_vector
             )
         elif type_ == "depth":
             kwargs["near_depth"] = search_get_pb2.NearDepthSearch(
-                depth=media, distance=distance, certainty=certainty, target_vectors=target_vectors
+                depth=media, distance=distance, certainty=certainty, target_vectors=target_vector
             )
         elif type_ == "image":
             kwargs["near_image"] = search_get_pb2.NearImageSearch(
-                image=media, distance=distance, certainty=certainty, target_vectors=target_vectors
+                image=media, distance=distance, certainty=certainty, target_vectors=target_vector
             )
         elif type_ == "imu":
             kwargs["near_imu"] = search_get_pb2.NearIMUSearch(
-                imu=media, distance=distance, certainty=certainty, target_vectors=target_vectors
+                imu=media, distance=distance, certainty=certainty, target_vectors=target_vector
             )
         elif type_ == "thermal":
             kwargs["near_thermal"] = search_get_pb2.NearThermalSearch(
-                thermal=media, distance=distance, certainty=certainty, target_vectors=target_vectors
+                thermal=media, distance=distance, certainty=certainty, target_vectors=target_vector
             )
         elif type_ == "video":
             kwargs["near_video"] = search_get_pb2.NearVideoSearch(
-                video=media, distance=distance, certainty=certainty, target_vectors=target_vectors
+                video=media, distance=distance, certainty=certainty, target_vectors=target_vector
             )
         else:
             raise ValueError(
                 f"type_ must be one of ['audio', 'depth', 'image', 'imu', 'thermal', 'video'], but got {type_}"
             )
         request = self.__create_request(
             limit=limit,
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/grpc/shared.py` & `weaviate_client-4.7.0a0/weaviate/collections/grpc/shared.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/grpc/tenants.py` & `weaviate_client-4.7.0a0/weaviate/collections/grpc/tenants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/iterator.py` & `weaviate_client-4.7.0a0/weaviate/collections/iterator.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/orm.py` & `weaviate_client-4.7.0a0/weaviate/collections/orm.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/base.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/bm25/generate.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/bm25/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/bm25/generate.pyi` & `weaviate_client-4.7.0a0/weaviate/collections/queries/bm25/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/bm25/query.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/bm25/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/bm25/query.pyi` & `weaviate_client-4.7.0a0/weaviate/collections/queries/bm25/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/byteops.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/byteops.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/fetch_object_by_id/query.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/fetch_object_by_id/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/fetch_object_by_id/query.pyi` & `weaviate_client-4.7.0a0/weaviate/collections/queries/fetch_object_by_id/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/fetch_objects/generate.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/fetch_objects/generate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/fetch_objects/generate.pyi` & `weaviate_client-4.7.0a0/weaviate/collections/queries/fetch_objects/generate.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/fetch_objects/query.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/fetch_objects/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/fetch_objects/query.pyi` & `weaviate_client-4.7.0a0/weaviate/collections/queries/fetch_objects/query.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/hybrid/generate.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/hybrid/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generic, List, Optional
+from typing import Generic, List, Optional, Union
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
 from weaviate.collections.classes.grpc import (
     METADATA,
     GroupBy,
@@ -38,15 +38,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
     ) -> GenerativeSearchReturnType[Properties, References, TProperties, TReferences]:
         """Perform retrieval-augmented generation (RaG) on the results of an object search in this collection using the hybrid algorithm blending keyword-based BM25 and vector-based similarity.
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/hybrid/generate.pyi` & `weaviate_client-4.7.0a0/weaviate/collections/queries/hybrid/generate.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generic, List, Literal, Optional, Type, overload
+from typing import Generic, List, Literal, Optional, Type, Union, overload
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
 from weaviate.collections.classes.grpc import (
     METADATA,
     PROPERTIES,
@@ -36,15 +36,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GenerativeReturn[Properties, References]: ...
     @overload
     def hybrid(
@@ -60,15 +60,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> GenerativeReturn[Properties, CrossReferences]: ...
     @overload
     def hybrid(
@@ -84,15 +84,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GenerativeReturn[Properties, TReferences]: ...
     @overload
     def hybrid(
@@ -108,15 +108,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GenerativeReturn[TProperties, References]: ...
     @overload
     def hybrid(
@@ -132,15 +132,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GenerativeReturn[TProperties, CrossReferences]: ...
     @overload
     def hybrid(
@@ -156,15 +156,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> GenerativeReturn[TProperties, TReferences]: ...
 
     ##### GROUP BY #####
@@ -183,15 +183,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GenerativeGroupByReturn[Properties, References]: ...
     @overload
     def hybrid(
@@ -207,15 +207,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> GenerativeGroupByReturn[Properties, CrossReferences]: ...
     @overload
     def hybrid(
@@ -231,15 +231,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GenerativeGroupByReturn[Properties, TReferences]: ...
     @overload
     def hybrid(
@@ -255,15 +255,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GenerativeGroupByReturn[TProperties, References]: ...
     @overload
     def hybrid(
@@ -279,15 +279,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GenerativeGroupByReturn[TProperties, CrossReferences]: ...
     @overload
     def hybrid(
@@ -303,13 +303,13 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> GenerativeGroupByReturn[TProperties, TReferences]: ...
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/hybrid/query.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/hybrid/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generic, List, Optional
+from typing import Generic, List, Optional, Union
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
 
 from weaviate.collections.classes.grpc import (
     METADATA,
@@ -35,15 +35,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
     ) -> QuerySearchReturnType[Properties, References, TProperties, TReferences]:
         """Search for objects in this collection using the hybrid algorithm blending keyword-based BM25 and vector-based similarity.
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/hybrid/query.pyi` & `weaviate_client-4.7.0a0/weaviate/collections/queries/hybrid/query.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generic, List, Literal, Optional, Type, overload
+from typing import Generic, List, Literal, Optional, Type, Union, overload
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
 from weaviate.collections.classes.grpc import (
     METADATA,
     PROPERTIES,
@@ -33,15 +33,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> QueryReturn[Properties, References]: ...
     @overload
     def hybrid(
@@ -54,15 +54,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> QueryReturn[Properties, CrossReferences]: ...
     @overload
     def hybrid(
@@ -75,15 +75,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> QueryReturn[Properties, TReferences]: ...
     @overload
     def hybrid(
@@ -96,15 +96,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> QueryReturn[TProperties, References]: ...
     @overload
     def hybrid(
@@ -117,15 +117,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> QueryReturn[TProperties, CrossReferences]: ...
     @overload
     def hybrid(
@@ -138,15 +138,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> QueryReturn[TProperties, TReferences]: ...
 
     ##### GROUP BY #####
@@ -162,15 +162,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GroupByReturn[Properties, References]: ...
     @overload
     def hybrid(
@@ -183,15 +183,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> GroupByReturn[Properties, CrossReferences]: ...
     @overload
     def hybrid(
@@ -204,15 +204,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GroupByReturn[Properties, TReferences]: ...
     @overload
     def hybrid(
@@ -225,15 +225,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GroupByReturn[TProperties, References]: ...
     @overload
     def hybrid(
@@ -246,15 +246,15 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GroupByReturn[TProperties, CrossReferences]: ...
     @overload
     def hybrid(
@@ -267,13 +267,13 @@
         fusion_type: Optional[HybridFusion] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> GroupByReturn[TProperties, TReferences]: ...
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_image/generate.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_image/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
     ) -> GenerativeSearchReturnType[Properties, References, TProperties, TReferences]:
         """Perform retrieval-augmented generation (RaG) on the results of a by-image object search in this collection using an image-capable vectorization module and vector-based similarity search.
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_image/generate.pyi` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_image/generate.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GenerativeReturn[Properties, References]: ...
     @overload
     def near_image(
@@ -50,15 +50,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> GenerativeReturn[Properties, CrossReferences]: ...
     @overload
     def near_image(
@@ -72,15 +72,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GenerativeReturn[Properties, TReferences]: ...
     @overload
     def near_image(
@@ -94,15 +94,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GenerativeReturn[TProperties, References]: ...
     @overload
     def near_image(
@@ -116,15 +116,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GenerativeReturn[TProperties, CrossReferences]: ...
     @overload
     def near_image(
@@ -138,15 +138,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> GenerativeReturn[TProperties, TReferences]: ...
     ### GroupBy ###
     @overload
@@ -161,15 +161,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GenerativeGroupByReturn[Properties, References]: ...
     @overload
     def near_image(
@@ -183,15 +183,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> GenerativeGroupByReturn[Properties, CrossReferences]: ...
     @overload
     def near_image(
@@ -205,15 +205,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GenerativeGroupByReturn[Properties, TReferences]: ...
     @overload
     def near_image(
@@ -227,15 +227,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GenerativeGroupByReturn[TProperties, References]: ...
     @overload
     def near_image(
@@ -249,15 +249,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GenerativeGroupByReturn[TProperties, CrossReferences]: ...
     @overload
     def near_image(
@@ -271,13 +271,13 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> GenerativeGroupByReturn[TProperties, TReferences]: ...
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_image/query.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_image/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from io import BufferedReader
 from pathlib import Path
-from typing import Generic, Optional, Union
+from typing import Generic, List, Optional, Union
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
 from weaviate.collections.classes.grpc import METADATA, GroupBy, Rerank
 from weaviate.collections.classes.internal import (
     _GroupBy,
@@ -27,15 +27,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
     ) -> QuerySearchReturnType[Properties, References, TProperties, TReferences]:
         """Search for objects by image in this collection using an image-capable vectorization module and vector-based similarity search.
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_image/query.pyi` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_image/query.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from io import BufferedReader
 from pathlib import Path
-from typing import Generic, Literal, Optional, Type, Union, overload
+from typing import Generic, List, Literal, Optional, Type, Union, overload
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
 from weaviate.collections.classes.grpc import METADATA, PROPERTIES, REFERENCES, GroupBy, Rerank
 from weaviate.collections.classes.internal import (
     GroupByReturn,
@@ -25,15 +25,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> QueryReturn[Properties, References]: ...
     @overload
     def near_image(
@@ -44,15 +44,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> QueryReturn[Properties, CrossReferences]: ...
     @overload
     def near_image(
@@ -63,15 +63,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> QueryReturn[Properties, TReferences]: ...
     @overload
     def near_image(
@@ -82,15 +82,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> QueryReturn[TProperties, References]: ...
     @overload
     def near_image(
@@ -101,15 +101,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> QueryReturn[TProperties, CrossReferences]: ...
     @overload
     def near_image(
@@ -120,15 +120,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> QueryReturn[TProperties, TReferences]: ...
 
     ### GroupBy ###
@@ -142,15 +142,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GroupByReturn[Properties, References]: ...
     @overload
     def near_image(
@@ -161,15 +161,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> GroupByReturn[Properties, CrossReferences]: ...
     @overload
     def near_image(
@@ -180,15 +180,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GroupByReturn[Properties, TReferences]: ...
     @overload
     def near_image(
@@ -199,15 +199,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GroupByReturn[TProperties, References]: ...
     @overload
     def near_image(
@@ -218,15 +218,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GroupByReturn[TProperties, CrossReferences]: ...
     @overload
     def near_image(
@@ -237,13 +237,13 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> GroupByReturn[TProperties, TReferences]: ...
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_media/generate.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_media/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
     ) -> GenerativeSearchReturnType[Properties, References, TProperties, TReferences]:
         """Perform retrieval-augmented generation (RaG) on the results of a by-audio object search in this collection using an audio-capable vectorization module and vector-based similarity search.
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_media/generate.pyi` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_media/generate.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GenerativeReturn[Properties, References]: ...
     @overload
     def near_media(
@@ -59,15 +59,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> GenerativeReturn[Properties, CrossReferences]: ...
     @overload
     def near_media(
@@ -82,15 +82,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GenerativeReturn[Properties, TReferences]: ...
     @overload
     def near_media(
@@ -105,15 +105,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GenerativeReturn[TProperties, References]: ...
     @overload
     def near_media(
@@ -128,15 +128,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GenerativeReturn[TProperties, CrossReferences]: ...
     @overload
     def near_media(
@@ -151,15 +151,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> GenerativeReturn[TProperties, TReferences]: ...
     ### GroupBy ###
     @overload
@@ -175,15 +175,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GenerativeGroupByReturn[Properties, References]: ...
     @overload
     def near_media(
@@ -198,15 +198,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> GenerativeGroupByReturn[Properties, CrossReferences]: ...
     @overload
     def near_media(
@@ -221,15 +221,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GenerativeGroupByReturn[Properties, TReferences]: ...
     @overload
     def near_media(
@@ -244,15 +244,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GenerativeGroupByReturn[TProperties, References]: ...
     @overload
     def near_media(
@@ -267,15 +267,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GenerativeGroupByReturn[TProperties, CrossReferences]: ...
     @overload
     def near_media(
@@ -290,13 +290,13 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> GenerativeGroupByReturn[TProperties, TReferences]: ...
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_media/query.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_media/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from io import BufferedReader
 from pathlib import Path
-from typing import Generic, Optional, Union
+from typing import Generic, List, Optional, Union
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
 from weaviate.collections.classes.grpc import GroupBy, METADATA, NearMediaType, Rerank
 from weaviate.collections.classes.internal import (
     _GroupBy,
@@ -28,15 +28,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
     ) -> QuerySearchReturnType[Properties, References, TProperties, TReferences]:
         """Search for objects by audio in this collection using an audio-capable vectorization module and vector-based similarity search.
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_media/query.pyi` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_vector/query.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,268 +1,247 @@
-from io import BufferedReader
-from pathlib import Path
-from typing import Generic, Literal, Optional, Type, Union, overload
+from typing import Generic, List, Literal, Optional, Type, Union, overload
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
-from weaviate.collections.classes.grpc import (
-    GroupBy,
-    METADATA,
-    PROPERTIES,
-    REFERENCES,
-    NearMediaType,
-    Rerank,
-)
+from weaviate.collections.classes.grpc import METADATA, PROPERTIES, REFERENCES, GroupBy, Rerank
 from weaviate.collections.classes.internal import (
     GroupByReturn,
     QueryReturn,
     CrossReferences,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
 from weaviate.types import NUMBER, INCLUDE_VECTOR
 
-class _NearMediaQuery(Generic[Properties, References], _BaseQuery[Properties, References]):
+class _NearVectorQuery(Generic[Properties, References], _BaseQuery[Properties, References]):
     @overload
-    def near_media(
+    def near_vector(
         self,
-        media: Union[str, Path, BufferedReader],
-        media_type: NearMediaType,
+        near_vector: List[float],
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> QueryReturn[Properties, References]: ...
     @overload
-    def near_media(
+    def near_vector(
         self,
-        media: Union[str, Path, BufferedReader],
-        media_type: NearMediaType,
+        near_vector: List[float],
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> QueryReturn[Properties, CrossReferences]: ...
     @overload
-    def near_media(
+    def near_vector(
         self,
-        media: Union[str, Path, BufferedReader],
-        media_type: NearMediaType,
+        near_vector: List[float],
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> QueryReturn[Properties, TReferences]: ...
     @overload
-    def near_media(
+    def near_vector(
         self,
-        media: Union[str, Path, BufferedReader],
-        media_type: NearMediaType,
+        near_vector: List[float],
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> QueryReturn[TProperties, References]: ...
     @overload
-    def near_media(
+    def near_vector(
         self,
-        media: Union[str, Path, BufferedReader],
-        media_type: NearMediaType,
+        near_vector: List[float],
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> QueryReturn[TProperties, CrossReferences]: ...
     @overload
-    def near_media(
+    def near_vector(
         self,
-        media: Union[str, Path, BufferedReader],
-        media_type: NearMediaType,
+        near_vector: List[float],
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> QueryReturn[TProperties, TReferences]: ...
 
     ### GroupBy ###
 
     @overload
-    def near_media(
+    def near_vector(
         self,
-        media: Union[str, Path, BufferedReader],
-        media_type: NearMediaType,
+        near_vector: List[float],
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GroupByReturn[Properties, References]: ...
     @overload
-    def near_media(
+    def near_vector(
         self,
-        media: Union[str, Path, BufferedReader],
-        media_type: NearMediaType,
+        near_vector: List[float],
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> GroupByReturn[Properties, CrossReferences]: ...
     @overload
-    def near_media(
+    def near_vector(
         self,
-        media: Union[str, Path, BufferedReader],
-        media_type: NearMediaType,
+        near_vector: List[float],
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GroupByReturn[Properties, TReferences]: ...
     @overload
-    def near_media(
+    def near_vector(
         self,
-        media: Union[str, Path, BufferedReader],
-        media_type: NearMediaType,
+        near_vector: List[float],
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GroupByReturn[TProperties, References]: ...
     @overload
-    def near_media(
+    def near_vector(
         self,
-        media: Union[str, Path, BufferedReader],
-        media_type: NearMediaType,
+        near_vector: List[float],
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GroupByReturn[TProperties, CrossReferences]: ...
     @overload
-    def near_media(
+    def near_vector(
         self,
-        media: Union[str, Path, BufferedReader],
-        media_type: NearMediaType,
+        near_vector: List[float],
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> GroupByReturn[TProperties, TReferences]: ...
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_object/generate.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_object/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generic, List, Optional
+from typing import Generic, List, Optional, Union
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
 from weaviate.collections.classes.grpc import METADATA, GroupBy, Rerank
 from weaviate.collections.classes.internal import (
     _Generative,
@@ -29,15 +29,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
     ) -> GenerativeSearchReturnType[Properties, References, TProperties, TReferences]:
         """Perform retrieval-augmented generation (RaG) on the results of a by-object object search in this collection using a vector-based similarity search.
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_object/generate.pyi` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_object/generate.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GenerativeReturn[Properties, References]: ...
     @overload
     def near_object(
@@ -48,15 +48,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> GenerativeReturn[Properties, CrossReferences]: ...
     @overload
     def near_object(
@@ -70,15 +70,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GenerativeReturn[Properties, TReferences]: ...
     @overload
     def near_object(
@@ -92,15 +92,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GenerativeReturn[TProperties, References]: ...
     @overload
     def near_object(
@@ -114,15 +114,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GenerativeReturn[TProperties, CrossReferences]: ...
     @overload
     def near_object(
@@ -136,15 +136,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> GenerativeReturn[TProperties, TReferences]: ...
     ### GroupBy ###
     @overload
@@ -159,15 +159,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GenerativeGroupByReturn[Properties, References]: ...
     @overload
     def near_object(
@@ -181,15 +181,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> GenerativeGroupByReturn[Properties, CrossReferences]: ...
     @overload
     def near_object(
@@ -203,15 +203,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GenerativeGroupByReturn[Properties, TReferences]: ...
     @overload
     def near_object(
@@ -225,15 +225,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GenerativeGroupByReturn[TProperties, References]: ...
     @overload
     def near_object(
@@ -247,15 +247,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GenerativeGroupByReturn[TProperties, CrossReferences]: ...
     @overload
     def near_object(
@@ -269,13 +269,13 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> GenerativeGroupByReturn[TProperties, TReferences]: ...
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_object/query.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_object/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generic, Optional
+from typing import Generic, List, Optional, Union
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
 from weaviate.collections.classes.grpc import METADATA, GroupBy, Rerank
 from weaviate.collections.classes.internal import (
     _GroupBy,
@@ -25,15 +25,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
     ) -> QuerySearchReturnType[Properties, References, TProperties, TReferences]:
         """Search for objects in this collection by another object using a vector-based similarity search.
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_object/query.pyi` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_object/query.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generic, Literal, Optional, Type, Union, overload
+from typing import Generic, List, Literal, Optional, Type, Union, overload
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
 from weaviate.collections.classes.grpc import METADATA, PROPERTIES, REFERENCES, GroupBy, Rerank
 from weaviate.collections.classes.internal import (
     GroupByReturn,
@@ -23,15 +23,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> QueryReturn[Properties, References]: ...
     @overload
     def near_object(
@@ -42,15 +42,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> QueryReturn[Properties, CrossReferences]: ...
     @overload
     def near_object(
@@ -61,15 +61,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> QueryReturn[Properties, TReferences]: ...
     @overload
     def near_object(
@@ -80,15 +80,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> QueryReturn[TProperties, References]: ...
     @overload
     def near_object(
@@ -99,15 +99,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> QueryReturn[TProperties, CrossReferences]: ...
     @overload
     def near_object(
@@ -118,15 +118,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> QueryReturn[TProperties, TReferences]: ...
 
     ### GroupBy ###
@@ -140,15 +140,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GroupByReturn[Properties, References]: ...
     @overload
     def near_object(
@@ -159,15 +159,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> GroupByReturn[Properties, CrossReferences]: ...
     @overload
     def near_object(
@@ -178,15 +178,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GroupByReturn[Properties, TReferences]: ...
     @overload
     def near_object(
@@ -197,15 +197,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GroupByReturn[TProperties, References]: ...
     @overload
     def near_object(
@@ -216,15 +216,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GroupByReturn[TProperties, CrossReferences]: ...
     @overload
     def near_object(
@@ -235,13 +235,13 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> GroupByReturn[TProperties, TReferences]: ...
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_text/generate.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_text/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
     ) -> GenerativeSearchReturnType[Properties, References, TProperties, TReferences]:
         """Perform retrieval-augmented generation (RaG) on the results of a by-image object search in this collection using the image-capable vectorization module and vector-based similarity search.
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_text/generate.pyi` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_text/generate.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GenerativeReturn[Properties, References]: ...
     @overload
     def near_text(
@@ -59,15 +59,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> GenerativeReturn[Properties, CrossReferences]: ...
     @overload
     def near_text(
@@ -83,15 +83,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GenerativeReturn[Properties, TReferences]: ...
     @overload
     def near_text(
@@ -107,15 +107,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GenerativeReturn[TProperties, References]: ...
     @overload
     def near_text(
@@ -131,15 +131,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GenerativeReturn[TProperties, CrossReferences]: ...
     @overload
     def near_text(
@@ -155,15 +155,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> GenerativeReturn[TProperties, TReferences]: ...
     ### GroupBy ###
     @overload
@@ -180,15 +180,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GenerativeGroupByReturn[Properties, References]: ...
     @overload
     def near_text(
@@ -204,15 +204,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> GenerativeGroupByReturn[Properties, CrossReferences]: ...
     @overload
     def near_text(
@@ -228,15 +228,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GenerativeGroupByReturn[Properties, TReferences]: ...
     @overload
     def near_text(
@@ -252,15 +252,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GenerativeGroupByReturn[TProperties, References]: ...
     @overload
     def near_text(
@@ -276,15 +276,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GenerativeGroupByReturn[TProperties, CrossReferences]: ...
     @overload
     def near_text(
@@ -300,13 +300,13 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> GenerativeGroupByReturn[TProperties, TReferences]: ...
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_text/query.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_text/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
     ) -> QuerySearchReturnType[Properties, References, TProperties, TReferences]:
         """Search for objects in this collection by text using text-capable vectorization module and vector-based similarity search.
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_text/query.pyi` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_text/query.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> QueryReturn[Properties, References]: ...
     @overload
     def near_text(
@@ -53,15 +53,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> QueryReturn[Properties, CrossReferences]: ...
     @overload
     def near_text(
@@ -74,15 +74,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> QueryReturn[Properties, TReferences]: ...
     @overload
     def near_text(
@@ -95,15 +95,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> QueryReturn[TProperties, References]: ...
     @overload
     def near_text(
@@ -116,15 +116,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> QueryReturn[TProperties, CrossReferences]: ...
     @overload
     def near_text(
@@ -137,15 +137,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> QueryReturn[TProperties, TReferences]: ...
 
     ### GroupBy ###
@@ -161,15 +161,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GroupByReturn[Properties, References]: ...
     @overload
     def near_text(
@@ -182,15 +182,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> QueryReturn[Properties, CrossReferences]: ...
     @overload
     def near_text(
@@ -203,15 +203,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GroupByReturn[Properties, TReferences]: ...
     @overload
     def near_text(
@@ -224,15 +224,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GroupByReturn[TProperties, References]: ...
     @overload
     def near_text(
@@ -245,15 +245,15 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GroupByReturn[TProperties, CrossReferences]: ...
     @overload
     def near_text(
@@ -266,13 +266,13 @@
         move_away: Optional[Move] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> GroupByReturn[TProperties, TReferences]: ...
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_vector/generate.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_vector/generate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generic, List, Optional
+from typing import Generic, List, Optional, Union
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
 from weaviate.collections.classes.grpc import METADATA, GroupBy, Rerank
 from weaviate.collections.classes.internal import (
     _Generative,
@@ -29,15 +29,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
     ) -> GenerativeSearchReturnType[Properties, References, TProperties, TReferences]:
         """Perform retrieval-augmented generation (RaG) on the results of a by-vector object search in this collection using vector-based similarity search.
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_vector/generate.pyi` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_vector/generate.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GenerativeReturn[Properties, References]: ...
     @overload
     def near_vector(
@@ -48,15 +48,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> GenerativeReturn[Properties, CrossReferences]: ...
     @overload
     def near_vector(
@@ -70,15 +70,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GenerativeReturn[Properties, TReferences]: ...
     @overload
     def near_vector(
@@ -92,15 +92,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GenerativeReturn[TProperties, References]: ...
     @overload
     def near_vector(
@@ -114,15 +114,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GenerativeReturn[TProperties, CrossReferences]: ...
     @overload
     def near_vector(
@@ -136,15 +136,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> GenerativeReturn[TProperties, TReferences]: ...
     ### GroupBy ###
     @overload
@@ -159,15 +159,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GenerativeGroupByReturn[Properties, References]: ...
     @overload
     def near_vector(
@@ -181,15 +181,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> GenerativeGroupByReturn[Properties, CrossReferences]: ...
     @overload
     def near_vector(
@@ -203,15 +203,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GenerativeGroupByReturn[Properties, TReferences]: ...
     @overload
     def near_vector(
@@ -225,15 +225,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GenerativeGroupByReturn[TProperties, References]: ...
     @overload
     def near_vector(
@@ -247,15 +247,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GenerativeGroupByReturn[TProperties, CrossReferences]: ...
     @overload
     def near_vector(
@@ -269,13 +269,13 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> GenerativeGroupByReturn[TProperties, TReferences]: ...
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_vector/query.py` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_vector/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Generic, List, Optional
+from typing import Generic, List, Optional, Union
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
 from weaviate.collections.classes.grpc import METADATA, GroupBy, Rerank
 from weaviate.collections.classes.internal import (
     _GroupBy,
@@ -25,15 +25,15 @@
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Optional[GroupBy] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[List[str], str]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[ReturnProperties[TProperties]] = None,
         return_references: Optional[ReturnReferences[TReferences]] = None,
     ) -> QuerySearchReturnType[Properties, References, TProperties, TReferences]:
         """Search for objects by vector in this collection using and vector-based similarity search.
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/queries/near_vector/query.pyi` & `weaviate_client-4.7.0a0/weaviate/collections/queries/near_media/query.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,247 +1,268 @@
+from io import BufferedReader
+from pathlib import Path
 from typing import Generic, List, Literal, Optional, Type, Union, overload
 
 from weaviate.collections.classes.filters import (
     _Filters,
 )
-from weaviate.collections.classes.grpc import METADATA, PROPERTIES, REFERENCES, GroupBy, Rerank
+from weaviate.collections.classes.grpc import (
+    GroupBy,
+    METADATA,
+    PROPERTIES,
+    REFERENCES,
+    NearMediaType,
+    Rerank,
+)
 from weaviate.collections.classes.internal import (
     GroupByReturn,
     QueryReturn,
     CrossReferences,
 )
 from weaviate.collections.classes.types import Properties, TProperties, References, TReferences
 from weaviate.collections.queries.base import _BaseQuery
 from weaviate.types import NUMBER, INCLUDE_VECTOR
 
-class _NearVectorQuery(Generic[Properties, References], _BaseQuery[Properties, References]):
+class _NearMediaQuery(Generic[Properties, References], _BaseQuery[Properties, References]):
     @overload
-    def near_vector(
+    def near_media(
         self,
-        near_vector: List[float],
+        media: Union[str, Path, BufferedReader],
+        media_type: NearMediaType,
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> QueryReturn[Properties, References]: ...
     @overload
-    def near_vector(
+    def near_media(
         self,
-        near_vector: List[float],
+        media: Union[str, Path, BufferedReader],
+        media_type: NearMediaType,
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> QueryReturn[Properties, CrossReferences]: ...
     @overload
-    def near_vector(
+    def near_media(
         self,
-        near_vector: List[float],
+        media: Union[str, Path, BufferedReader],
+        media_type: NearMediaType,
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> QueryReturn[Properties, TReferences]: ...
     @overload
-    def near_vector(
+    def near_media(
         self,
-        near_vector: List[float],
+        media: Union[str, Path, BufferedReader],
+        media_type: NearMediaType,
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> QueryReturn[TProperties, References]: ...
     @overload
-    def near_vector(
+    def near_media(
         self,
-        near_vector: List[float],
+        media: Union[str, Path, BufferedReader],
+        media_type: NearMediaType,
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> QueryReturn[TProperties, CrossReferences]: ...
     @overload
-    def near_vector(
+    def near_media(
         self,
-        near_vector: List[float],
+        media: Union[str, Path, BufferedReader],
+        media_type: NearMediaType,
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: Literal[None] = None,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> QueryReturn[TProperties, TReferences]: ...
 
     ### GroupBy ###
 
     @overload
-    def near_vector(
+    def near_media(
         self,
-        near_vector: List[float],
+        media: Union[str, Path, BufferedReader],
+        media_type: NearMediaType,
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Literal[None] = None,
     ) -> GroupByReturn[Properties, References]: ...
     @overload
-    def near_vector(
+    def near_media(
         self,
-        near_vector: List[float],
+        media: Union[str, Path, BufferedReader],
+        media_type: NearMediaType,
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: REFERENCES,
     ) -> GroupByReturn[Properties, CrossReferences]: ...
     @overload
-    def near_vector(
+    def near_media(
         self,
-        near_vector: List[float],
+        media: Union[str, Path, BufferedReader],
+        media_type: NearMediaType,
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Optional[PROPERTIES] = None,
         return_references: Type[TReferences],
     ) -> GroupByReturn[Properties, TReferences]: ...
     @overload
-    def near_vector(
+    def near_media(
         self,
-        near_vector: List[float],
+        media: Union[str, Path, BufferedReader],
+        media_type: NearMediaType,
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Literal[None] = None,
     ) -> GroupByReturn[TProperties, References]: ...
     @overload
-    def near_vector(
+    def near_media(
         self,
-        near_vector: List[float],
+        media: Union[str, Path, BufferedReader],
+        media_type: NearMediaType,
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: REFERENCES,
     ) -> GroupByReturn[TProperties, CrossReferences]: ...
     @overload
-    def near_vector(
+    def near_media(
         self,
-        near_vector: List[float],
+        media: Union[str, Path, BufferedReader],
+        media_type: NearMediaType,
         *,
         certainty: Optional[NUMBER] = None,
         distance: Optional[NUMBER] = None,
         limit: Optional[int] = None,
         offset: Optional[int] = None,
         auto_limit: Optional[int] = None,
         filters: Optional[_Filters] = None,
         group_by: GroupBy,
         rerank: Optional[Rerank] = None,
-        target_vector: Optional[str] = None,
+        target_vector: Optional[Union[str, List[str]]] = None,
         include_vector: INCLUDE_VECTOR = False,
         return_metadata: Optional[METADATA] = None,
         return_properties: Type[TProperties],
         return_references: Type[TReferences],
     ) -> GroupByReturn[TProperties, TReferences]: ...
```

### Comparing `weaviate_client-4.6.3/weaviate/collections/query.py` & `weaviate_client-4.7.0a0/weaviate/collections/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/collections/tenants.py` & `weaviate_client-4.7.0a0/weaviate/collections/tenants.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/config.py` & `weaviate_client-4.7.0a0/weaviate/config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/connect/authentication.py` & `weaviate_client-4.7.0a0/weaviate/connect/authentication.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/connect/base.py` & `weaviate_client-4.7.0a0/weaviate/connect/base.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/connect/helpers.py` & `weaviate_client-4.7.0a0/weaviate/connect/helpers.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/connect/integrations.py` & `weaviate_client-4.7.0a0/weaviate/connect/integrations.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/connect/v3.py` & `weaviate_client-4.7.0a0/weaviate/connect/v3.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/connect/v4.py` & `weaviate_client-4.7.0a0/weaviate/connect/v4.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/contextionary/crud_contextionary.py` & `weaviate_client-4.7.0a0/weaviate/contextionary/crud_contextionary.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/data/crud_data.py` & `weaviate_client-4.7.0a0/weaviate/data/crud_data.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/data/references/crud_references.py` & `weaviate_client-4.7.0a0/weaviate/data/references/crud_references.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/embedded.py` & `weaviate_client-4.7.0a0/weaviate/embedded.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/error_msgs.py` & `weaviate_client-4.7.0a0/weaviate/error_msgs.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/exceptions.py` & `weaviate_client-4.7.0a0/weaviate/exceptions.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/gql/aggregate.py` & `weaviate_client-4.7.0a0/weaviate/gql/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/gql/filter.py` & `weaviate_client-4.7.0a0/weaviate/gql/filter.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/gql/get.py` & `weaviate_client-4.7.0a0/weaviate/gql/get.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/gql/multi_get.py` & `weaviate_client-4.7.0a0/weaviate/gql/multi_get.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/gql/query.py` & `weaviate_client-4.7.0a0/weaviate/gql/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/integrations.py` & `weaviate_client-4.7.0a0/weaviate/integrations.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/outputs/aggregate.py` & `weaviate_client-4.7.0a0/weaviate/outputs/aggregate.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/outputs/config.py` & `weaviate_client-4.7.0a0/weaviate/outputs/config.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/outputs/query.py` & `weaviate_client-4.7.0a0/weaviate/outputs/query.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/proto/v1/base_pb2.py` & `weaviate_client-4.7.0a0/weaviate/proto/v1/base_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/proto/v1/base_pb2.pyi` & `weaviate_client-4.7.0a0/weaviate/proto/v1/base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/proto/v1/batch_delete_pb2.py` & `weaviate_client-4.7.0a0/weaviate/proto/v1/batch_delete_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/proto/v1/batch_delete_pb2.pyi` & `weaviate_client-4.7.0a0/weaviate/proto/v1/batch_delete_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/proto/v1/batch_pb2.py` & `weaviate_client-4.7.0a0/weaviate/proto/v1/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/proto/v1/batch_pb2.pyi` & `weaviate_client-4.7.0a0/weaviate/proto/v1/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/proto/v1/properties_pb2.py` & `weaviate_client-4.7.0a0/weaviate/proto/v1/properties_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/proto/v1/properties_pb2.pyi` & `weaviate_client-4.7.0a0/weaviate/proto/v1/properties_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/proto/v1/search_get_pb2.py` & `weaviate_client-4.7.0a0/weaviate/proto/v1/search_get_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/proto/v1/search_get_pb2.pyi` & `weaviate_client-4.7.0a0/weaviate/proto/v1/search_get_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/proto/v1/tenants_pb2.py` & `weaviate_client-4.7.0a0/weaviate/proto/v1/tenants_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/proto/v1/tenants_pb2.pyi` & `weaviate_client-4.7.0a0/weaviate/proto/v1/tenants_pb2.pyi`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/proto/v1/weaviate_pb2.py` & `weaviate_client-4.7.0a0/weaviate/proto/v1/weaviate_pb2.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/proto/v1/weaviate_pb2_grpc.py` & `weaviate_client-4.7.0a0/weaviate/proto/v1/weaviate_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/schema/crud_schema.py` & `weaviate_client-4.7.0a0/weaviate/schema/crud_schema.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/schema/properties/crud_properties.py` & `weaviate_client-4.7.0a0/weaviate/schema/properties/crud_properties.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/types.py` & `weaviate_client-4.7.0a0/weaviate/types.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/util.py` & `weaviate_client-4.7.0a0/weaviate/util.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/validator.py` & `weaviate_client-4.7.0a0/weaviate/validator.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate/warnings.py` & `weaviate_client-4.7.0a0/weaviate/warnings.py`

 * *Files identical despite different names*

### Comparing `weaviate_client-4.6.3/weaviate_client.egg-info/PKG-INFO` & `weaviate_client-4.7.0a0/weaviate_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weaviate-client
-Version: 4.6.3
+Version: 4.7.0a0
 Summary: A python native Weaviate client
 Home-page: https://github.com/weaviate/weaviate-python-client
 Author: Weaviate
 Author-email: hello@weaviate.io,
 License: BSD 3-clause
 Project-URL: Documentation, https://weaviate-python-client.readthedocs.io
 Project-URL: Source, https://github.com/weaviate/weaviate-python-client
```

### Comparing `weaviate_client-4.6.3/weaviate_client.egg-info/SOURCES.txt` & `weaviate_client-4.7.0a0/weaviate_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

