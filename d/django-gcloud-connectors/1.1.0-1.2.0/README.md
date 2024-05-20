# Comparing `tmp/django-gcloud-connectors-1.1.0.tar.gz` & `tmp/django-gcloud-connectors-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-gcloud-connectors-1.1.0.tar", last modified: Tue Mar  5 15:11:08 2024, max compression
+gzip compressed data, was "django-gcloud-connectors-1.2.0.tar", last modified: Mon May 20 14:08:04 2024, max compression
```

## Comparing `django-gcloud-connectors-1.1.0.tar` & `django-gcloud-connectors-1.2.0.tar`

### file list

```diff
@@ -1,120 +1,137 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1526 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      184 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1683 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      983 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/django_gcloud_connectors.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1683 2024-03-05 15:11:07.000000 django-gcloud-connectors-1.1.0/django_gcloud_connectors.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3257 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/django_gcloud_connectors.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-05 15:11:07.000000 django-gcloud-connectors-1.1.0/django_gcloud_connectors.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      133 2024-03-05 15:11:07.000000 django-gcloud-connectors-1.1.0/django_gcloud_connectors.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-03-05 15:11:07.000000 django-gcloud-connectors-1.1.0/django_gcloud_connectors.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/gcloudc/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/gcloudc/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/gcloudc/commands/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/commands/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/gcloudc/commands/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)     6923 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/commands/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/commands/management/commands/runserver.py
--rw-rw-rw-   0 root         (0) root         (0)      152 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/commands/management/commands/shell.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/commands/management/commands/test.py
--rw-rw-rw-   0 root         (0) root         (0)     3705 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/context_decorator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/gcloudc/core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1469 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/core/validators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/gcloudc/db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/
--rw-rw-rw-   0 root         (0) root         (0)      458 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24686 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/base.py
--rw-rw-rw-   0 root         (0) root         (0)     5893 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/caching.py
--rw-rw-rw-   0 root         (0) root         (0)    40639 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/commands.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/compiler.py
--rw-rw-rw-   0 root         (0) root         (0)     3062 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/constraints.py
--rw-rw-rw-   0 root         (0) root         (0)    12257 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/context.py
--rw-rw-rw-   0 root         (0) root         (0)      556 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/dbapi.py
--rw-rw-rw-   0 root         (0) root         (0)    13219 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/dnf.py
--rw-rw-rw-   0 root         (0) root         (0)     1818 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/expressions.py
--rw-rw-rw-   0 root         (0) root         (0)     4827 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/formatting.py
--rw-rw-rw-   0 root         (0) root         (0)    33337 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/indexing.py
--rw-rw-rw-   0 root         (0) root         (0)    18101 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/meta_queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/parsers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22069 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/parsers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1376 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/parsers/version_18.py
--rw-rw-rw-   0 root         (0) root         (0)     5637 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/parsers/version_19.py
--rw-rw-rw-   0 root         (0) root         (0)    24732 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/query.py
--rw-rw-rw-   0 root         (0) root         (0)     1650 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/query_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5499 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    17195 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/transaction.py
--rw-rw-rw-   0 root         (0) root         (0)     3728 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/unique_mixins.py
--rw-rw-rw-   0 root         (0) root         (0)     7310 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/unique_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    17616 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      404 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/gcloudc/db/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/gcloudc/db/models/fields/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/models/fields/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   290599 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/models/fields/allkeys-5.2.0.zip
--rw-rw-rw-   0 root         (0) root         (0)     1843 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/models/fields/charfields.py
--rw-rw-rw-   0 root         (0) root         (0)     5603 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/models/fields/computed.py
--rw-rw-rw-   0 root         (0) root         (0)    15112 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/models/fields/iterable.py
--rw-rw-rw-   0 root         (0) root         (0)     7711 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/models/fields/json.py
--rw-rw-rw-   0 root         (0) root         (0)    30847 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/models/fields/related.py
--rw-rw-rw-   0 root         (0) root         (0)     2623 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/db/transaction.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/gcloudc/forms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/forms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10445 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/forms/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/
--rw-rw-rw-   0 root         (0) root         (0)      693 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      909 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/concurrent_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    11918 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/models.py
--rw-rw-rw-   0 root         (0) root         (0)      802 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/router.py
--rw-rw-rw-   0 root         (0) root         (0)     2736 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_async_multi_query.py
--rw-rw-rw-   0 root         (0) root         (0)    32587 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_atomic.py
--rw-rw-rw-   0 root         (0) root         (0)     1076 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_caching.py
--rw-rw-rw-   0 root         (0) root         (0)      925 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_cloud_datastore_runner.py
--rw-rw-rw-   0 root         (0) root         (0)      330 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_collation_field.py
--rw-rw-rw-   0 root         (0) root         (0)     1266 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_computed_field.py
--rw-rw-rw-   0 root         (0) root         (0)    85794 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_connector.py
--rw-rw-rw-   0 root         (0) root         (0)    18571 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_db_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     1171 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_delete.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_django_interactions.py
--rw-rw-rw-   0 root         (0) root         (0)     2203 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_excluding_pks.py
--rw-rw-rw-   0 root         (0) root         (0)    16541 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_iterable_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     3947 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_json_field.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_operations.py
--rw-rw-rw-   0 root         (0) root         (0)     3466 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_query_by_keys.py
--rw-rw-rw-   0 root         (0) root         (0)    19748 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_query_transform.py
--rw-rw-rw-   0 root         (0) root         (0)    25599 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_related_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     5653 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_transaction_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)    16568 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/tests/test_unique_constraints.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/gcloudc/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1463 2024-03-05 15:10:58.000000 django-gcloud-connectors-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/test/
--rw-r--r--   0 root         (0) root         (0)     6088 2024-03-05 15:06:15.000000 django-gcloud-connectors-1.1.0/test/404.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/test/caching/
--rw-r--r--   0 root         (0) root         (0)     9538 2024-03-05 15:06:15.000000 django-gcloud-connectors-1.1.0/test/caching/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/test/commercial_support/
--rw-r--r--   0 root         (0) root         (0)     6886 2024-03-05 15:06:15.000000 django-gcloud-connectors-1.1.0/test/commercial_support/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/test/concepts_limitations/
--rw-r--r--   0 root         (0) root         (0)    14358 2024-03-05 15:06:15.000000 django-gcloud-connectors-1.1.0/test/concepts_limitations/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/test/contributing/
--rw-r--r--   0 root         (0) root         (0)    14947 2024-03-05 15:06:15.000000 django-gcloud-connectors-1.1.0/test/contributing/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/test/field_indexes/
--rw-r--r--   0 root         (0) root         (0)    10610 2024-03-05 15:06:15.000000 django-gcloud-connectors-1.1.0/test/field_indexes/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/test/fields/
--rw-r--r--   0 root         (0) root         (0)    15796 2024-03-05 15:06:15.000000 django-gcloud-connectors-1.1.0/test/fields/index.html
--rw-r--r--   0 root         (0) root         (0)     7583 2024-03-05 15:06:15.000000 django-gcloud-connectors-1.1.0/test/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/test/installation/
--rw-r--r--   0 root         (0) root         (0)     7999 2024-03-05 15:06:15.000000 django-gcloud-connectors-1.1.0/test/installation/index.html
--rw-r--r--   0 root         (0) root         (0)     5697 2024-03-05 15:06:15.000000 django-gcloud-connectors-1.1.0/test/search.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/test/transactions/
--rw-r--r--   0 root         (0) root         (0)    13302 2024-03-05 15:06:15.000000 django-gcloud-connectors-1.1.0/test/transactions/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 15:11:08.000000 django-gcloud-connectors-1.1.0/test/work_with_potato/
--rw-r--r--   0 root         (0) root         (0)     6558 2024-03-05 15:06:15.000000 django-gcloud-connectors-1.1.0/test/work_with_potato/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.636808 django-gcloud-connectors-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      184 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1722 2024-05-20 14:08:04.635808 django-gcloud-connectors-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1045 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.616808 django-gcloud-connectors-1.2.0/django_gcloud_connectors.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1722 2024-05-20 14:08:04.000000 django-gcloud-connectors-1.2.0/django_gcloud_connectors.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3631 2024-05-20 14:08:04.000000 django-gcloud-connectors-1.2.0/django_gcloud_connectors.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 14:08:04.000000 django-gcloud-connectors-1.2.0/django_gcloud_connectors.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      164 2024-05-20 14:08:04.000000 django-gcloud-connectors-1.2.0/django_gcloud_connectors.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-20 14:08:04.000000 django-gcloud-connectors-1.2.0/django_gcloud_connectors.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.616808 django-gcloud-connectors-1.2.0/gcloudc/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.616808 django-gcloud-connectors-1.2.0/gcloudc/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.617808 django-gcloud-connectors-1.2.0/gcloudc/commands/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/commands/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.617808 django-gcloud-connectors-1.2.0/gcloudc/commands/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)    10939 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/commands/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      142 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/commands/management/commands/runserver.py
+-rw-rw-rw-   0 root         (0) root         (0)      138 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/commands/management/commands/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)      487 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/commands/management/commands/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3705 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/context_decorator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.618808 django-gcloud-connectors-1.2.0/gcloudc/core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1469 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/core/validators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.618808 django-gcloud-connectors-1.2.0/gcloudc/db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.618808 django-gcloud-connectors-1.2.0/gcloudc/db/backends/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.620808 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.621808 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/base/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    27827 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/base/connection.py
+-rw-rw-rw-   0 root         (0) root         (0)      792 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/base/dbapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     6679 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/base/entity.py
+-rw-rw-rw-   0 root         (0) root         (0)    15536 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/base/query.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/base/traits.py
+-rw-rw-rw-   0 root         (0) root         (0)    23833 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/commands.py
+-rw-rw-rw-   0 root         (0) root         (0)     9485 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/constraints.py
+-rw-rw-rw-   0 root         (0) root         (0)     5266 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/formatting.py
+-rw-rw-rw-   0 root         (0) root         (0)    15934 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    34535 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/indexing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3759 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.622808 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    44811 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/parsers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14130 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/parsers/builder.py
+-rw-rw-rw-   0 root         (0) root         (0)    13488 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/parsers/dnf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1870 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/parsers/expressions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.623808 django-gcloud-connectors-1.2.0/gcloudc/db/backends/datastore/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/datastore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15007 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/datastore/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3313 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/datastore/compiler.py
+-rw-rw-rw-   0 root         (0) root         (0)     5501 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/datastore/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.623808 django-gcloud-connectors-1.2.0/gcloudc/db/backends/firestore/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/firestore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    28239 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/firestore/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3313 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/firestore/compiler.py
+-rw-rw-rw-   0 root         (0) root         (0)     5501 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/backends/firestore/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.624808 django-gcloud-connectors-1.2.0/gcloudc/db/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.626808 django-gcloud-connectors-1.2.0/gcloudc/db/models/fields/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/models/fields/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1759 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/models/fields/_compatibility.py
+-rw-rw-rw-   0 root         (0) root         (0)   290599 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/models/fields/allkeys-5.2.0.zip
+-rw-rw-rw-   0 root         (0) root         (0)     1721 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/models/fields/boolean.py
+-rw-rw-rw-   0 root         (0) root         (0)     1843 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/models/fields/charfields.py
+-rw-rw-rw-   0 root         (0) root         (0)     5603 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/models/fields/computed.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.626808 django-gcloud-connectors-1.2.0/gcloudc/db/models/fields/firestore/
+-rw-rw-rw-   0 root         (0) root         (0)     5261 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/models/fields/firestore/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15542 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/models/fields/iterable.py
+-rw-rw-rw-   0 root         (0) root         (0)     7718 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/models/fields/json.py
+-rw-rw-rw-   0 root         (0) root         (0)    30958 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/db/models/fields/related.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.626808 django-gcloud-connectors-1.2.0/gcloudc/forms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/forms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11911 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/forms/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.632808 django-gcloud-connectors-1.2.0/gcloudc/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1303 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      828 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/concurrent_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    11941 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      802 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/router.py
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_async_multi_query.py
+-rw-rw-rw-   0 root         (0) root         (0)    22347 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_atomic.py
+-rw-rw-rw-   0 root         (0) root         (0)      555 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_autocharfield.py
+-rw-rw-rw-   0 root         (0) root         (0)      858 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_caching.py
+-rw-rw-rw-   0 root         (0) root         (0)      925 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_cloud_datastore_runner.py
+-rw-rw-rw-   0 root         (0) root         (0)      330 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_collation_field.py
+-rw-rw-rw-   0 root         (0) root         (0)     1266 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_computed_field.py
+-rw-rw-rw-   0 root         (0) root         (0)    85237 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_connector.py
+-rw-rw-rw-   0 root         (0) root         (0)    21182 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_db_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_django_interactions.py
+-rw-rw-rw-   0 root         (0) root         (0)      878 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_exclude.py
+-rw-rw-rw-   0 root         (0) root         (0)     2971 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_excluding_pks.py
+-rw-rw-rw-   0 root         (0) root         (0)    23193 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_iterable_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     3983 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_json_field.py
+-rw-rw-rw-   0 root         (0) root         (0)     5688 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_mapfield.py
+-rw-rw-rw-   0 root         (0) root         (0)     1206 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_obscure_queries.py
+-rw-rw-rw-   0 root         (0) root         (0)      452 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_offset_limit.py
+-rw-rw-rw-   0 root         (0) root         (0)     1199 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)     6335 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_query_by_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)    23007 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_query_transform.py
+-rw-rw-rw-   0 root         (0) root         (0)    25532 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_related_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_subqueries.py
+-rw-rw-rw-   0 root         (0) root         (0)     4670 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_transaction_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)    19221 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/tests/test_unique_constraints.py
+-rw-rw-rw-   0 root         (0) root         (0)      934 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/gcloudc/utils.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 14:08:04.636808 django-gcloud-connectors-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2024-05-20 14:07:55.000000 django-gcloud-connectors-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.633808 django-gcloud-connectors-1.2.0/test/
+-rw-r--r--   0 root         (0) root         (0)     6289 2024-05-20 14:02:54.000000 django-gcloud-connectors-1.2.0/test/404.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.633808 django-gcloud-connectors-1.2.0/test/caching/
+-rw-r--r--   0 root         (0) root         (0)     7687 2024-05-20 14:02:54.000000 django-gcloud-connectors-1.2.0/test/caching/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.633808 django-gcloud-connectors-1.2.0/test/commercial_support/
+-rw-r--r--   0 root         (0) root         (0)     7050 2024-05-20 14:02:54.000000 django-gcloud-connectors-1.2.0/test/commercial_support/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.634808 django-gcloud-connectors-1.2.0/test/concepts_limitations/
+-rw-r--r--   0 root         (0) root         (0)    12045 2024-05-20 14:02:54.000000 django-gcloud-connectors-1.2.0/test/concepts_limitations/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.634808 django-gcloud-connectors-1.2.0/test/contributing/
+-rw-r--r--   0 root         (0) root         (0)    16349 2024-05-20 14:02:54.000000 django-gcloud-connectors-1.2.0/test/contributing/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.634808 django-gcloud-connectors-1.2.0/test/field_indexes/
+-rw-r--r--   0 root         (0) root         (0)    11186 2024-05-20 14:02:54.000000 django-gcloud-connectors-1.2.0/test/field_indexes/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.634808 django-gcloud-connectors-1.2.0/test/fields/
+-rw-r--r--   0 root         (0) root         (0)    16696 2024-05-20 14:02:54.000000 django-gcloud-connectors-1.2.0/test/fields/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.634808 django-gcloud-connectors-1.2.0/test/firestore/
+-rw-r--r--   0 root         (0) root         (0)    10998 2024-05-20 14:02:54.000000 django-gcloud-connectors-1.2.0/test/firestore/index.html
+-rw-r--r--   0 root         (0) root         (0)     7942 2024-05-20 14:02:54.000000 django-gcloud-connectors-1.2.0/test/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.635808 django-gcloud-connectors-1.2.0/test/installation/
+-rw-r--r--   0 root         (0) root         (0)     8221 2024-05-20 14:02:54.000000 django-gcloud-connectors-1.2.0/test/installation/index.html
+-rw-r--r--   0 root         (0) root         (0)     5861 2024-05-20 14:02:54.000000 django-gcloud-connectors-1.2.0/test/search.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.635808 django-gcloud-connectors-1.2.0/test/special_indexes/
+-rw-r--r--   0 root         (0) root         (0)     7512 2024-05-20 14:02:54.000000 django-gcloud-connectors-1.2.0/test/special_indexes/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.635808 django-gcloud-connectors-1.2.0/test/transactions/
+-rw-r--r--   0 root         (0) root         (0)     7246 2024-05-20 14:02:54.000000 django-gcloud-connectors-1.2.0/test/transactions/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 14:08:04.635808 django-gcloud-connectors-1.2.0/test/work_with_potato/
+-rw-r--r--   0 root         (0) root         (0)     6722 2024-05-20 14:02:54.000000 django-gcloud-connectors-1.2.0/test/work_with_potato/index.html
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-gcloud-connectors-1.1.0/LICENSE` & `django-gcloud-connectors-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-1.1.0/README.md` & `django-gcloud-connectors-1.2.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Django GCloud Connectors (gcloudc)
 
-**Note: This project is now living in [GitLab](https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors)**
+Django Google Cloud Connectors provides database backends for two non-relational database services that run on Google Cloud:
 
-The aim of this project is to create Django database connector / backend for Google Cloud.
+ - Google Cloud Datastore
+ - Google Cloud Firestore
 
-It currently provides support for Cloud Firestore in Datastore mode.
-Note: the `OPTIMISTIC_WITH_ENTITY_GROUPS` legacy concurrency mode is not supported.
+This django-gcloud-connectors project allows you to seamlessly use the Django ORM with these databases; allowing you to leverage
+the full power of Django on a massively scalable No-SQL database.
 
-[Documentation](https://potato-oss.gitlab.io/google-cloud/django-gcloud-connectors/)
+For more information on the project, please see the [documentation](https://potato-oss.gitlab.io/google-cloud/django-gcloud-connectors/)
 
 If you are interested in submitting a patch, please refer to the [Contributing](https://potato-oss.gitlab.io/google-cloud/django-gcloud-connectors/contributing) page.
 
 ---
 
 ## Looking for Commercial Support?
```

### Comparing `django-gcloud-connectors-1.1.0/django_gcloud_connectors.egg-info/SOURCES.txt` & `django-gcloud-connectors-1.2.0/django_gcloud_connectors.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -15,79 +15,90 @@
 gcloudc/commands/management/commands/__init__.py
 gcloudc/commands/management/commands/runserver.py
 gcloudc/commands/management/commands/shell.py
 gcloudc/commands/management/commands/test.py
 gcloudc/core/__init__.py
 gcloudc/core/validators.py
 gcloudc/db/__init__.py
-gcloudc/db/decorators.py
-gcloudc/db/transaction.py
 gcloudc/db/backends/__init__.py
+gcloudc/db/backends/common/__init__.py
+gcloudc/db/backends/common/commands.py
+gcloudc/db/backends/common/constraints.py
+gcloudc/db/backends/common/formatting.py
+gcloudc/db/backends/common/helpers.py
+gcloudc/db/backends/common/indexing.py
+gcloudc/db/backends/common/mixins.py
+gcloudc/db/backends/common/base/__init__.py
+gcloudc/db/backends/common/base/connection.py
+gcloudc/db/backends/common/base/dbapi.py
+gcloudc/db/backends/common/base/entity.py
+gcloudc/db/backends/common/base/query.py
+gcloudc/db/backends/common/base/traits.py
+gcloudc/db/backends/common/parsers/__init__.py
+gcloudc/db/backends/common/parsers/base.py
+gcloudc/db/backends/common/parsers/builder.py
+gcloudc/db/backends/common/parsers/dnf.py
+gcloudc/db/backends/common/parsers/expressions.py
 gcloudc/db/backends/datastore/__init__.py
 gcloudc/db/backends/datastore/base.py
-gcloudc/db/backends/datastore/caching.py
-gcloudc/db/backends/datastore/commands.py
 gcloudc/db/backends/datastore/compiler.py
-gcloudc/db/backends/datastore/constraints.py
-gcloudc/db/backends/datastore/context.py
-gcloudc/db/backends/datastore/dbapi.py
-gcloudc/db/backends/datastore/dnf.py
-gcloudc/db/backends/datastore/expressions.py
-gcloudc/db/backends/datastore/formatting.py
-gcloudc/db/backends/datastore/indexing.py
-gcloudc/db/backends/datastore/meta_queries.py
-gcloudc/db/backends/datastore/query.py
-gcloudc/db/backends/datastore/query_utils.py
 gcloudc/db/backends/datastore/schema.py
-gcloudc/db/backends/datastore/transaction.py
-gcloudc/db/backends/datastore/unique_mixins.py
-gcloudc/db/backends/datastore/unique_utils.py
-gcloudc/db/backends/datastore/utils.py
-gcloudc/db/backends/datastore/parsers/__init__.py
-gcloudc/db/backends/datastore/parsers/base.py
-gcloudc/db/backends/datastore/parsers/version_18.py
-gcloudc/db/backends/datastore/parsers/version_19.py
+gcloudc/db/backends/firestore/__init__.py
+gcloudc/db/backends/firestore/base.py
+gcloudc/db/backends/firestore/compiler.py
+gcloudc/db/backends/firestore/schema.py
 gcloudc/db/models/__init__.py
 gcloudc/db/models/fields/__init__.py
+gcloudc/db/models/fields/_compatibility.py
 gcloudc/db/models/fields/allkeys-5.2.0.zip
+gcloudc/db/models/fields/boolean.py
 gcloudc/db/models/fields/charfields.py
 gcloudc/db/models/fields/computed.py
 gcloudc/db/models/fields/iterable.py
 gcloudc/db/models/fields/json.py
 gcloudc/db/models/fields/related.py
+gcloudc/db/models/fields/firestore/__init__.py
 gcloudc/forms/__init__.py
 gcloudc/forms/fields.py
 gcloudc/tests/__init__.py
 gcloudc/tests/concurrent_utils.py
 gcloudc/tests/models.py
 gcloudc/tests/router.py
 gcloudc/tests/test_async_multi_query.py
 gcloudc/tests/test_atomic.py
+gcloudc/tests/test_autocharfield.py
 gcloudc/tests/test_caching.py
 gcloudc/tests/test_cloud_datastore_runner.py
 gcloudc/tests/test_collation_field.py
 gcloudc/tests/test_computed_field.py
 gcloudc/tests/test_connector.py
 gcloudc/tests/test_db_fields.py
 gcloudc/tests/test_delete.py
 gcloudc/tests/test_django_interactions.py
+gcloudc/tests/test_exclude.py
 gcloudc/tests/test_excluding_pks.py
 gcloudc/tests/test_iterable_fields.py
 gcloudc/tests/test_json_field.py
+gcloudc/tests/test_mapfield.py
+gcloudc/tests/test_obscure_queries.py
+gcloudc/tests/test_offset_limit.py
 gcloudc/tests/test_operations.py
 gcloudc/tests/test_query_by_keys.py
 gcloudc/tests/test_query_transform.py
 gcloudc/tests/test_related_fields.py
+gcloudc/tests/test_subqueries.py
 gcloudc/tests/test_transaction_hooks.py
 gcloudc/tests/test_unique_constraints.py
 test/404.html
 test/index.html
 test/search.html
 test/caching/index.html
 test/commercial_support/index.html
 test/concepts_limitations/index.html
 test/contributing/index.html
 test/field_indexes/index.html
 test/fields/index.html
+test/firestore/index.html
 test/installation/index.html
+test/special_indexes/index.html
 test/transactions/index.html
 test/work_with_potato/index.html
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/context_decorator.py` & `django-gcloud-connectors-1.2.0/gcloudc/context_decorator.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/core/validators.py` & `django-gcloud-connectors-1.2.0/gcloudc/core/validators.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/base.py` & `django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/base/connection.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,101 +1,316 @@
-import datetime
 import decimal
-import logging
-import os
+import datetime
 import uuid
-import warnings
-
-import requests
-
 from django.conf import settings
+from django.db import IntegrityError
 from django.core.exceptions import ImproperlyConfigured
-from django.db.backends.base.base import BaseDatabaseWrapper
-from django.db.backends.base.client import BaseDatabaseClient
-from django.db.backends.base.creation import BaseDatabaseCreation
-from django.db.backends.base.features import BaseDatabaseFeatures
-from django.db.backends.base.introspection import (
-    BaseDatabaseIntrospection,
-    TableInfo,
-)
 from django.db.backends.base.operations import BaseDatabaseOperations
-from django.db.backends.base.schema import BaseDatabaseSchemaEditor
-from django.db.backends.base.validation import BaseDatabaseValidation
 from django.utils import (
     timezone,
 )
 from django.utils.encoding import smart_str
-from google.cloud import (
-    datastore,
-    environment_vars,
+from google.api_core.datetime_helpers import DatetimeWithNanoseconds
+from typing import Optional, List, Tuple
+from .entity import Entity, Key
+from gcloudc.db.backends.common.indexing import load_special_indexes
+from gcloudc.db.backends.common.helpers import (
+    decimal_to_string,
+    ensure_datetime,
+    make_utc_compatible
+)
+from gcloudc.db.backends.common.constraints import (
+    check_unique_markers_in_memory,
+    has_unique_constraints,
+    perform_unique_checks,
 )
 
-from . import dbapi as Database
-from .commands import (
+from gcloudc.db.backends.common.commands import (
     DeleteCommand,
     FlushCommand,
     InsertCommand,
     SelectCommand,
     UpdateCommand,
     coerce_unicode,
 )
-from .indexing import load_special_indexes
-from .utils import (
-    decimal_to_string,
-    ensure_datetime,
-    get_datastore_key,
-    make_utc_compatible,
-)
 
-logger = logging.getLogger(__name__)
 
+class StagedWriteKind:
+    INSERT = 0
+    UPDATE = 1
+    DELETE = 2
 
-class Connection(object):
-    """ Dummy connection class """
+
+class Connection:
+    """ Base connection object for Datastore/Firestore implementations to subclass.
+        This holds the Datastore/Firestore client. All roads and RPC calls lead back to this object.
+    """
 
     def __init__(self, wrapper, params):
+        self.wrapper = wrapper
         self.creation = wrapper.creation
         self.ops = wrapper.ops
         self.queries = []
         self.settings_dict = params
         self.namespace = wrapper.namespace
+        self.database = wrapper.database
 
-        self.gclient = datastore.Client(
-            namespace=wrapper.namespace,
-            project=params["PROJECT"],
-            # avoid a bug in the google client - it tries to authenticate even when the emulator is enabled
-            # see https://github.com/googleapis/google-cloud-python/issues/5738
-            _http=requests.Session if os.environ.get(environment_vars.GCD_HOST) else None,
+        self._client = self._create_client(
+            params['PROJECT'],
+            database=self.database,
+            namespace=self.namespace,
         )
 
-    def acquire_constraint_markers(self, markers):
-        pass
+        self._autocommit = True
+        self._txn = None
+        self._seen_keys = set()
+        self._cache = {}
+
+        # On non-rel platforms often inside a transaction,
+        # you can't perform any read after performing any write. So... if we're inside
+        # transaction we "stage" the write and pretend it succeeded, and then do the actual
+        # write on transaction commit. We stage these documents by reference so that we
+        # only apply the final write for each key
+        self._staged_writes = {}
+
+    def _stage_write(self, entity_or_key, kind):
+        if kind == StagedWriteKind.DELETE:
+            assert (isinstance(entity_or_key, Key))
+            self._staged_writes[entity_or_key] = (kind, None)
+        else:
+            if kind == StagedWriteKind.UPDATE:
+                # There is a potential edge case where in the same transaction
+                # you do the following:
+                # 1. Create a entity
+                # 2. Update the entity
+                # Here, if we receive an update for an existing staged INSERT
+                # we replace the contents of the INSERT and don't stage an update
+                # so at the end of the transaction it looks like there was just
+                # one INSERT with the final data
+                if (
+                    entity_or_key.key() in self._staged_writes
+                    and self._staged_writes[entity_or_key.key()][0] == StagedWriteKind.INSERT
+                ):
+                    self._staged_writes[entity_or_key.key()][1] = entity_or_key
+                else:
+                    self._staged_writes[entity_or_key.key()] = (kind, entity_or_key)
+            else:
+                self._staged_writes[entity_or_key.key()] = (kind, entity_or_key)
 
-    def release_constraint_markers(self, markers):
-        pass
+    def _apply_staged_writes(self):
+        if not self._staged_writes:
+            return
+
+        assert (self._txn is not None)
+
+        for key, (kind, entity) in self._staged_writes.items():
+            if kind == StagedWriteKind.UPDATE:
+                self._put(key, entity, update=True)
+            elif kind == StagedWriteKind.DELETE:
+                self._delete(key)
+            else:
+                self._put(key, entity, update=False)
+
+        self._staged_writes.clear()
+
+    def _cache_entity(self, entity):
+        if self._txn is not None:
+            self._cache[entity.key()] = entity
+
+    def _find_entity_in_cache(self, field_values: List[Tuple[str, str]]) -> Optional[Entity]:
+        for entity in self._cache.values():
+            if all([entity._properties.get(k) == v for k, v in field_values]):
+                return entity
+
+    def _entity_from_cache(self, key) -> Optional[Entity]:
+        if self._txn is not None:
+            return self._cache.get(key)
+
+    def _create_client(self, project, namespace=None):
+        raise NotImplementedError()
+
+    def _close_client(self):
+        raise NotImplementedError()
+
+    def _begin(self):
+        raise NotImplementedError()
+
+    def _rollback(self):
+        raise NotImplementedError()
+
+    def _commit(self):
+        raise NotImplementedError()
+
+    def _put(self, key, entity, update: bool) -> Optional[Entity]:
+        raise NotImplementedError()
+
+    def _get(self, key_or_keys) -> List[Entity]:
+        """
+            Should return a list of one or more entities
+            from the provided keys
+        """
+        raise NotImplementedError()
+
+    def _delete(self, key: Key):
+        raise NotImplementedError()
+
+    def _exists(self, key):
+        raise NotImplementedError()
+
+    def new_key(self, table, id_or_name, parent=None, namespace=None) -> Key:
+        raise NotImplementedError()
+
+    def begin(self):
+        self._seen_keys = set()
+        self._cache = {}
+        self._staged_writes.clear()
+        return self._begin()
 
     def rollback(self):
-        pass
+        try:
+            if self._txn is not None:
+                return self._rollback()
+        finally:
+            self._txn = None
+            self._cache = {}
+            self._seen_keys = set()
+            self._staged_writes.clear()
 
     def commit(self):
-        pass
+        puts, deletes = [], []
+        for key, (kind, entity) in self._staged_writes.items():
+            if kind == StagedWriteKind.INSERT:
+                puts.append(entity)
+            elif kind == StagedWriteKind.UPDATE:
+                puts.append(entity)
+            else:
+                assert (kind == StagedWriteKind.DELETE)
+                deletes.append(entity)
+
+        self.wrapper.pre_commit(puts, deletes)
+        self._apply_staged_writes()
+        try:
+            self._commit()
+        finally:
+            self._txn = None
+            self._cache = {}
+            self._seen_keys = set()
+            self._staged_writes.clear()
+
+    def savepoint(self, sid):
+        raise NotImplementedError()
+
+    def savepoint_commit(self, sid):
+        raise NotImplementedError()
+
+    def savepoint_rollback(self, sid):
+        raise NotImplementedError()
+
+    def exists(self, key) -> bool:
+        return self._exists(key)
+
+    def put(self, entity, allow_existing=True):
+        key = entity.key()
+        new = not self.exists(key)
+
+        if not new and not allow_existing:
+            raise IntegrityError("Tried to INSERT with existing key")
+
+        if self._txn is not None:
+            self._stage_write(entity, StagedWriteKind.INSERT if new else StagedWriteKind.UPDATE)
+            self._cache_entity(entity)
+        else:
+            if new:
+                updated_entity = self._put(key, entity, update=False)
+            else:
+                updated_entity = self._put(key, entity, update=True)
+
+            if not updated_entity:
+                return
+
+            key = updated_entity.key()
+
+        self._seen_keys.add(key)
+
+    def get(self, key_or_keys):
+        is_list = hasattr(key_or_keys, "__iter__") and not isinstance(key_or_keys, str)
+        if not is_list:
+            keys = [key_or_keys]
+        else:
+            keys = key_or_keys
+
+        # Get what we can from the cache - this will be empty
+        # if we're not in a transaction
+        cached = [self._entity_from_cache(key) for key in keys]
+
+        # Make a list of all the keys that weren't cached
+        to_fetch = []
+        for key, ent in zip(keys, cached):
+            if not ent:
+                to_fetch.append(key)
+
+        # Fetch the ones we need
+        fetched = self._get(to_fetch)
+        fetched = {x.key(): x for x in fetched if x}
+
+        # Build results in the original order the keys
+        # were provided
+        results = []
+        for key, ent in zip(keys, cached):
+            result = ent or fetched.get(key)
+            if result:
+                results.append(result)
+                self._seen_keys.add(key)
+
+        if is_list:
+            return results
+        else:
+            return results[0] if results else None
+
+    def delete(self, key: Key):
+        if self._txn is not None:
+            self._stage_write(key, StagedWriteKind.DELETE)
+
+            # FIXME: Mark the entity as deleted in the cache.
+            # This is different to removing from the cache because
+            # we want subsequent gets to fail, not hit the database.
+        else:
+            return self._delete(key)
+
+    def _flush(self, tables, namespace=None):
+        raise NotImplementedError()
+
+    def flush(self, tables, namespace=None):
+        return self._flush(tables, namespace)
 
     def close(self):
-        pass
+        self._close_client()
+
+    @property
+    def autocommit(self):
+        return self._autocommit
+
+    @autocommit.setter
+    def autocommit(self, value):
+        if value and not self._autocommit:
+            self.rollback()
+        elif not value and self._autocommit:
+            self.begin()
+        self._autocommit = value
 
 
 class Cursor(object):
     """ Dummy cursor class """
 
     def __init__(self, connection):
         self.connection = connection
         self.start_cursor = None
         self.returned_ids = []
         self.rowcount = -1
-        self.last_select_command = None
+        self.last_select_command: Optional[SelectCommand] = None
         self.last_delete_command = None
 
     def execute(self, sql, *params):
         if isinstance(sql, SelectCommand):
             # Also catches subclasses of SelectCommand (e.g Update)
             self.last_select_command = sql
             self.rowcount = self.last_select_command.execute() or -1
@@ -105,15 +320,15 @@
             self.rowcount = sql.execute()
         elif isinstance(sql, DeleteCommand):
             self.rowcount = sql.execute()
         elif isinstance(sql, InsertCommand):
             self.connection.queries.append(sql)
             self.returned_ids = sql.execute()
         else:
-            raise Database.CouldBeSupportedError(
+            raise ValueError(
                 "Can't execute traditional SQL: '%s' (although perhaps we could make GQL work)" % sql
             )
 
     def next(self):
         row = self.fetchone()
         if row is None:
             raise StopIteration
@@ -122,26 +337,23 @@
     def fetchone(self, delete_flag=False):
         try:
             result = next(self.last_select_command.results)
 
             if isinstance(result, int):
                 return (result,)
 
-            query = self.last_select_command.query
-
             row = []
 
-            # Prepend extra select values to the resulting row
-            for col, select in query.extra_selects:
-                row.append(result.get(col))
+            for col in self.last_select_command.init_list:
+                if col == self.last_select_command.model._meta.pk.column:
+                    row.append(result.key().id_or_name)
+                else:
+                    row.append(result.get(col))
 
-            for col in self.last_select_command.query.init_list:
-                row.append(result.get(col))
-
-            self.returned_ids.append(result.key.id_or_name)
+            self.returned_ids.append(result.key().id_or_name)
             return row
         except StopIteration:
             return None
 
     def fetchmany(self, size, delete_flag=False):
         if not self.last_select_command.results:
             return []
@@ -165,20 +377,221 @@
     def __iter__(self):
         return self
 
     def close(self):
         pass
 
 
-MAXINT = 9223372036854775808
+class Wrapper:
+    """
+        A base class for all connections in gcloudc. This defines some additional
+        operation methods we expect each backend to implement.
+    """
+
+    TRANSACTION_ENTITY_LIMIT = 500
+
+    array_not_empty_operator_and_value = (">", None)
+    array_empty_operator_and_value = ("=", None)
+    supports_empty_array = False
+    supports_only_null_equality = False
+
+    # If this is True, we can get away with storing much less
+    # data when doing contains/icontains queries.
+    supports_range_queries_on_array = False
+
+    def __init__(self, *args, **kwargs):
+        self.connection = None
+        super().__init__(*args, **kwargs)
+
+    def _set_autocommit(self, autocommit):
+        if not self.connection:
+            raise ValueError("No valid connection")
+
+        self.connection.autocommit = autocommit
+
+    def is_usable(self):
+        return True
+
+    def get_connection_params(self):
+        if not self.settings_dict.get("INDEXES_FILE"):
+            raise ImproperlyConfigured("You must specify an INDEXES_FILE in the DATABASES setting")
+
+        return self.settings_dict.copy()
+
+    def _create_connection(self, params):
+        raise NotImplementedError()
+
+    def get_new_connection(self, params):
+        conn = self._create_connection(params)
+        load_special_indexes(conn)  # make sure special indexes are loaded
+        return conn
+
+    def init_connection_state(self):
+        pass
+
+    def create_cursor(self, name=None):
+        self.name = name
+        self.ensure_connection()
+        return Cursor(self.connection)
+
+    def get_query_class(self):
+        raise NotImplementedError()
+
+    def is_id_valid(self, value) -> bool:
+        if isinstance(value, int) and value > 0:
+            return True
+        elif isinstance(value, str) and value and not value.startswith("__"):
+            return True
+
+        return False
+
+    def transform_django_query(self, query, force_keys_only):
+        """
+            This is where the magic happens! We take a Django Query object, manipulate it
+            so that it's suitable for a non-relational backend and then return an ORQuery
+            that can be executed.
+        """
+
+        from gcloudc.db.backends.common.parsers import base
+        parser = base.BaseParser(query, self)
+        return parser.get_transformed_query(
+            self,
+            force_keys_only=force_keys_only
+        )
+
+    def namespace(self):
+        """
+            Returns the namespace of this connection if any. This is normally
+            specified in DATABASES, but not all backends support it. If it's unsupported
+            then return None.
+        """
+        raise NotImplementedError()
+
+    def database(self):
+        """
+            Returns the database of this connection if any. This is normally
+            specified in DATABASES, but not all backends support it. If it's unsupported
+            then return None.
+        """
+        raise NotImplementedError()
+
+    def generate_id(self, type):
+        raise NotImplementedError()
+
+    def reserve_id(self, table, id_or_name, namespace):
+        raise NotImplementedError()
+
+    def key_property_name(self):
+        """
+            Return the name of the "Key" field, e.g. __key__ or __name__
+        """
+        raise NotImplementedError()
+
+    def polymodel_property_name(self):
+        """
+            Ideally this would be the same on all backends, but
+            Datastore used the (problematic) "class", so for backwards
+            compatibility we need to be able to switch based
+            on the backend
+        """
+
+        raise NotImplementedError()
+
+    def to_native_key(self, key):
+        """
+            When given a Key object, this should return the native
+            type.
+        """
+        raise NotImplementedError()
+
+    def from_native_key(self, key) -> Key:
+        """
+            Returns an equivalent Key object to the native key passed
+            in.
+        """
+        raise NotImplementedError()
+
+    def to_native_entity(self, entity: Entity):
+        """
+            When given an Entity object, this should return the same
+            thing as a native type.
+        """
+        raise NotImplementedError()
+
+    def from_native_entity(self, entity_or_key) -> Entity:
+        """
+            Takes a native entity returned from a query, and turns it into an
+            Entity object. If the argument is a key this should be an "empty" entity
+            with just the key set.
+        """
+        raise NotImplementedError()
+
+    def pre_entity_insert(self, model, entity, constraints):
+        must_handle_unique = has_unique_constraints(model)
 
+        if must_handle_unique:
+            perform_unique_checks(
+                self,
+                model,
+                entity,
+                test_fn=lambda stored: stored and len(stored) > 0
+            )
+
+    def post_entity_insert(self, model, entity, constraints):
+        pass
+
+    def pre_entity_update(self, model, entity, constraints):
+        must_handle_unique = has_unique_constraints(model)
+
+        def check(stored):
+            return stored and stored[0] and stored[0].key() != entity.key()
+
+        if must_handle_unique:
+            perform_unique_checks(
+                self,
+                model,
+                entity,
+                test_fn=check
+            )
+
+    def post_entity_update(self, model, entity, constraints):
+        pass
+
+    def pre_entity_delete(self, model, entity, constraints):
+        pass
+
+    def post_entity_delete(self, model, entity, constraints):
+        pass
+
+    def pre_commit(self, puts, deletes):
+        check_unique_markers_in_memory(self, puts)
+
+    def _savepoint(self, sid):
+        self.connection.savepoint(sid)
+
+    def _savepoint_rollback(self, sid):
+        self.connection.savepoint_rollback(sid)
+
+    def _savepoint_commit(self, sid):
+        self.connection.savepoint_commit(sid)
+
+    def get_transaction_entity_limit(self) -> Optional[int]:
+        """
+            Returns the number of entities that can be read/written
+            within a transaction. Return None if there is no limit
+        """
+
+        return 500
+
+
+MAXINT = 9223372036854775808
 _BULK_BATCH_SIZE_SETTING = "BULK_BATCH_SIZE"
 
 
-class DatabaseOperations(BaseDatabaseOperations):
+class NoSQLDatabaseOperations(BaseDatabaseOperations):
     compiler_module = "gcloudc.db.backends.datastore.compiler"
 
     # Datastore will store all integers as 64bit long values
     integer_field_ranges = {
         "SmallIntegerField": (-MAXINT, MAXINT - 1),
         "IntegerField": (-MAXINT, MAXINT - 1),
         "BigIntegerField": (-MAXINT, MAXINT - 1),
@@ -289,73 +702,19 @@
         ]
 
         return [
             FlushCommand(table, self.connection)
             for table in tables + additional_djangaeidx_tables
         ]
 
-    def prep_lookup_key(self, model, value, field):
-        if isinstance(value, str):
-            value = value[:500]
-            left = value[500:]
-            if left:
-                warnings.warn(
-                    "Truncating primary key that is over 500 characters. " "THIS IS AN ERROR IN YOUR PROGRAM.",
-                    RuntimeWarning,
-                )
-
-            # This is a bit of a hack. Basically when you query an integer PK with a
-            # string containing an int. SQL seems to return the row regardless of type, and as far as
-            # I can tell, Django at no point tries to cast the value to an integer. So, in the
-            # case where the internal type is an AutoField, we try to cast the string value
-            # I would love a more generic solution... patches welcome!
-            # It would be nice to see the SQL output of the lookup_int_as_str test is on SQL, if
-            # the string is converted to an int, I'd love to know where!
-            if field.get_internal_type() == "AutoField":
-                try:
-                    value = int(value)
-                except (TypeError, ValueError):
-                    pass
-
-            value = get_datastore_key(model, value)
-        else:
-            value = get_datastore_key(model, value)
-
-        return value
-
-    def prep_lookup_date(self, model, value, field):
-        if isinstance(value, datetime.datetime):
-            return value
-
-        return self.adapt_datefield_value(value)
-
-    def prep_lookup_time(self, model, value, field):
-        if isinstance(value, datetime.datetime):
-            return value
-
-        return self.adapt_timefield_value(value)
-
-    def prep_lookup_value(self, model, value, field, column=None):
-        if field.primary_key and (not column or column == model._meta.pk.column):
-            return self.prep_lookup_key(model, value, field)
-
-        db_type = field.db_type(self.connection)
-
-        if db_type == "date":
-            return self.prep_lookup_date(model, value, field)
-        elif db_type == "time":
-            return self.prep_lookup_time(model, value, field)
-        elif db_type in ("list", "set"):
-            if hasattr(value, "__len__") and not value:
-                value = None  # Convert empty lists to None
-            elif hasattr(value, "__iter__"):
-                # Convert sets to lists
-                value = list(value)
-
-        return value
+    def execute_sql_flush(self, sql_list):
+        """Execute a list of SQL statements to flush the database."""
+        with self.connection.cursor() as cursor:
+            for sql in sql_list:
+                cursor.execute(sql)
 
     def value_for_db(self, value, field):
         if value is None:
             return None
 
         db_type = field.db_type(self.connection)
 
@@ -377,15 +736,18 @@
             # be binary
             if isinstance(value, str):
                 value = value.encode("ascii")
         elif db_type == "decimal":
             value = self.adapt_decimalfield_value(value, field.max_digits, field.decimal_places)
         elif db_type in ("list", "set"):
             if hasattr(value, "__len__") and not value:
-                value = None  # Convert empty lists to None
+                if not self.connection.supports_empty_array:
+                    value = None  # Convert empty lists to None
+                else:
+                    value = []
             elif hasattr(value, "__iter__"):
                 # Convert sets to lists
                 value = list(value)
 
         return value
 
     def last_insert_id(self, cursor, db_table, column):
@@ -427,299 +789,49 @@
         return value
 
     def value_to_db_decimal(self, value, max_digits, decimal_places):  # Django 1.8 compatibility
         return self.adapt_decimalfield_value(value, max_digits, decimal_places)
 
     # Unlike value_to_db, these are not overridden or standard Django, it's just nice to have symmetry
     def value_from_db_datetime(self, value):
+
+        # Convert to a regular datetime.datetime
+        if isinstance(value, DatetimeWithNanoseconds):
+            if not settings.USE_TZ:
+                # we always receive a timezone.utc set, even when there is no timezone enabled
+                value = value.utcfromtimestamp(value.timestamp())
+            else:
+                value = datetime.datetime.fromtimestamp(value.timestamp(), tz=value.tzinfo)
+
         if isinstance(value, int):
             # App Engine Query's don't return datetime fields (unlike Get) I HAVE NO IDEA WHY
             value = ensure_datetime(value)
-
         if value is not None and settings.USE_TZ and timezone.is_naive(value):
-            value = value.replace(tzinfo=timezone.utc)
+            value = value.replace(tzinfo=datetime.timezone.utc)
         return value
 
     def value_from_db_date(self, value):
         if isinstance(value, int):
             # App Engine Query's don't return datetime fields (unlike Get) I HAVE NO IDEA WHY
             value = ensure_datetime(value)
 
         if value:
             value = value.date()
         return value
 
     def value_from_db_time(self, value):
-        if isinstance(value, int):
-            # App Engine Query's don't return datetime fields (unlike Get) I HAVE NO IDEA WHY
-            value = ensure_datetime(value).time()
+        if isinstance(value, (DatetimeWithNanoseconds, int)):
+            # App Engine Queries don't return datetime fields (unlike Get) I HAVE NO IDEA WHY
+            value = ensure_datetime(value)
 
         if value is not None and settings.USE_TZ and timezone.is_naive(value):
             value = value.replace(tzinfo=timezone.utc)
 
         if value:
             value = value.time()
 
         return value
 
     def value_from_db_decimal(self, value):
         if value:
             value = decimal.Decimal(value)
         return value
-
-
-class DatabaseClient(BaseDatabaseClient):
-    pass
-
-
-class DatabaseCreation(BaseDatabaseCreation):
-    data_types = {
-        "AutoField": "key",
-        "RelatedAutoField": "key",
-        "ForeignKey": "key",
-        "OneToOneField": "key",
-        "ManyToManyField": "key",
-        "BigIntegerField": "long",
-        "BooleanField": "bool",
-        "CharField": "string",
-        "CommaSeparatedIntegerField": "string",
-        "DateField": "date",
-        "DateTimeField": "datetime",
-        "DecimalField": "decimal",
-        "DurationField": "long",
-        "EmailField": "string",
-        "FileField": "string",
-        "FilePathField": "string",
-        "FloatField": "float",
-        "ImageField": "string",
-        "IntegerField": "integer",
-        "IPAddressField": "string",
-        "NullBooleanField": "bool",
-        "PositiveIntegerField": "integer",
-        "PositiveSmallIntegerField": "integer",
-        "SlugField": "string",
-        "SmallIntegerField": "integer",
-        "TimeField": "time",
-        "URLField": "string",
-        "TextField": "text",
-        "BinaryField": "bytes",
-    }
-
-    def __init__(self, *args, **kwargs):
-        self.testbed = None
-        super(DatabaseCreation, self).__init__(*args, **kwargs)
-
-    def sql_create_model(self, model, *args, **kwargs):
-        return [], {}
-
-    def sql_for_pending_references(self, model, *args, **kwargs):
-        return []
-
-    def sql_indexes_for_model(self, model, *args, **kwargs):
-        return []
-
-    def _create_test_db(self, verbosity, autoclobber, *args):
-        pass
-
-    def _destroy_test_db(self, name, verbosity):
-        pass
-
-
-class DatabaseIntrospection(BaseDatabaseIntrospection):
-    def get_table_list(self, cursor):
-        query = cursor.connection.gclient.query(kind="__kind__")
-        query.keys_only()
-        kinds = [entity.key.id_or_name for entity in query.fetch()]
-        return [TableInfo(x, "t") for x in kinds]
-
-    def get_sequences(self, cursor, table_name, table_fields=()):
-        # __key__ is the only column that can auto-populate
-        return [{'table': table_name, 'column': '__key__'}]
-
-
-class DatabaseSchemaEditor(BaseDatabaseSchemaEditor):
-    def column_sql(self, model, field, include_default=False):
-        return "", {}
-
-    def create_model(self, model):
-        """ Don't do anything when creating tables """
-        pass
-
-    def alter_unique_together(self, *args, **kwargs):
-        pass
-
-    def alter_field(self, from_model, from_field, to_field):
-        pass
-
-    def remove_field(self, from_model, field):
-        pass
-
-    def add_field(self, model, field):
-        pass
-
-    def alter_index_together(self, model, old_index_together, new_index_together):
-        pass
-
-    def delete_model(self, model):
-        pass
-
-
-class DatabaseFeatures(BaseDatabaseFeatures):
-    empty_fetchmany_value = []
-    supports_transactions = False  # FIXME: Make this True!
-    can_return_id_from_insert = True
-    supports_select_related = False
-    autocommits_when_autocommit_is_off = True
-    uses_savepoints = False
-    allows_auto_pk_0 = False
-    has_native_duration_field = False
-
-
-class DatabaseWrapper(BaseDatabaseWrapper):
-
-    data_types = DatabaseCreation.data_types  # These moved in 1.8
-
-    operators = {
-        "exact": "= %s",
-        "iexact": "iexact %s",
-        "contains": "contains %s",
-        "icontains": "icontains %s",
-        "regex": "regex %s",
-        "iregex": "iregex %s",
-        "gt": "> %s",
-        "gte": ">= %s",
-        "lt": "< %s",
-        "lte": "<= %s",
-        "startswith": "startswith %s",
-        "endswith": "endswith %s",
-        "istartswith": "istartswith %s",
-        "iendswith": "iendswith %s",
-        "isnull": "isnull %s",
-    }
-
-    Database = Database
-
-    # These attributes are only used by Django >= 1.11
-    client_class = DatabaseClient
-    features_class = DatabaseFeatures
-    introspection_class = DatabaseIntrospection
-    features_class = DatabaseFeatures
-    ops_class = DatabaseOperations
-    creation_class = DatabaseCreation
-    validation_class = BaseDatabaseValidation
-
-    def __init__(self, *args, **kwargs):
-        super(DatabaseWrapper, self).__init__(*args, **kwargs)
-
-        if not hasattr(self, "client"):
-            # Django 1.11 creates these automatically, when we call super
-            # These are here for Django <= 1.10
-            self.features = DatabaseFeatures(self)
-            self.ops = DatabaseOperations(self)
-            self.client = DatabaseClient(self)
-            self.creation = DatabaseCreation(self)
-            self.introspection = DatabaseIntrospection(self)
-            self.validation = BaseDatabaseValidation(self)
-
-        self.gcloud_project = self.settings_dict["PROJECT"]
-        self.namespace = self.settings_dict.get("NAMESPACE") or None
-        self.autocommit = True
-
-    def is_usable(self):
-        return True
-
-    def get_connection_params(self):
-        if not self.settings_dict.get("INDEXES_FILE"):
-            raise ImproperlyConfigured("You must specify an INDEXES_FILE in the DATABASES setting")
-
-        return self.settings_dict.copy()
-
-    def get_new_connection(self, params):
-        conn = Connection(self, params)
-        load_special_indexes(conn)  # make sure special indexes are loaded
-        return conn
-
-    def init_connection_state(self):
-        pass
-
-    def _start_transaction_under_autocommit(self):
-        pass
-
-    def _set_autocommit(self, enabled):
-        self.autocommit = enabled
-
-    def create_cursor(self, name=None):
-        self.name = name
-        if not self.connection:
-            self.connection = self.get_new_connection(self.settings_dict)
-
-        return Cursor(self.connection)
-
-    def schema_editor(self, *args, **kwargs):
-        return DatabaseSchemaEditor(self, *args, **kwargs)
-
-    def validate_no_broken_transaction(self):
-        # Override this to do nothing, because it's not relevant to the Datastore
-        pass
-
-    def on_commit(self, func):
-        # FIXME: This override needs to go away when we implement in_atomic_block
-        # on the connection - which we can't do unless we move wholesale to Django's
-        # atomic decorator (see issue #10)
-
-        from django.db.transaction import TransactionManagementError
-        from gcloudc.db.transaction import in_atomic_block
-
-        if in_atomic_block(using=self.alias or "default"):
-            # Transaction in progress; save for execution on commit.
-            self.run_on_commit.append((set(self.savepoint_ids), func))
-        elif not self.get_autocommit():
-            raise TransactionManagementError('on_commit() cannot be used in manual transaction management')
-        else:
-            # No transaction in progress and in autocommit mode; execute
-            # immediately.
-            func()
-
-    def run_and_clear_commit_hooks(self):
-        # FIXME: This override needs to go away when we implement in_atomic_block
-        # on the connection - which we can't do unless we move wholesale to Django's
-        # atomic decorator (see issue #10)
-
-        from gcloudc.db.transaction import in_atomic_block
-
-        if in_atomic_block(using=self.alias or "default"):
-            # FIXME: This should throw an error, but we can't because
-            # Django's atomic blocks toggle autocommit in get_or_create
-            # We need to unify with Django's decorators (see issue #10)
-            return
-
-        current_run_on_commit = self.run_on_commit
-        self.run_on_commit = []
-        while current_run_on_commit:
-            sids, func = current_run_on_commit.pop(0)
-            func()
-
-    def close(self):
-        """Close the connection to the database."""
-
-        from gcloudc.db.transaction import in_atomic_block
-
-        # FIXME: This override needs to go away when we implement in_atomic_block
-        # on the connection - which we can't do unless we move wholesale to Django's
-        # atomic decorator (see issue #10)
-
-        self.validate_thread_sharing()
-        self.run_on_commit = []
-
-        # Don't call validate_no_atomic_block() to avoid making it difficult
-        # to get rid of a connection in an invalid state. The next connect()
-        # will reset the transaction state anyway.
-        if self.closed_in_transaction or self.connection is None:
-            return
-        try:
-            self._close()
-        finally:
-            if in_atomic_block(using=self.alias or "default"):
-                self.closed_in_transaction = True
-                self.needs_rollback = True
-            else:
-                self.connection = None
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/compiler.py` & `django-gcloud-connectors-1.2.0/gcloudc/db/backends/datastore/compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     OrderBy,
     Value,
 )
 from django.db.models.sql import compiler
 from django.db.models.sql.query import get_order_dir
 
 # GCLOUDC
-from .commands import (
+from gcloudc.db.backends.common.commands import (
     DeleteCommand,
     InsertCommand,
     SelectCommand,
     UpdateCommand,
 )
 
 
@@ -35,28 +35,28 @@
     def as_sql(self, with_limits=True, with_col_aliases=False, subquery=False):
         self.pre_sql_setup()
         self.refcounts_before = self.query.alias_refcount.copy()
 
         select = SelectCommand(self.connection, self.query)
         return (select, tuple())
 
-    def get_select(self):
+    def get_select(self, **kwargs):
         self.query.select_related = False  # Make sure select_related is disabled for all queries
-        return super(SQLCompiler, self).get_select()
+        return super(SQLCompiler, self).get_select(**kwargs)
 
 
 class SQLInsertCompiler(SQLCompiler, compiler.SQLInsertCompiler):
     def __init__(self, *args, **kwargs):
         self.return_id = None
         super(SQLInsertCompiler, self).__init__(*args, **kwargs)
 
     def as_sql(self, with_limits=True, with_col_aliases=False, subquery=False):
         self.pre_sql_setup()
 
-        from gcloudc.db.backends.datastore.utils import get_concrete_fields
+        from gcloudc.db.backends.common.helpers import get_concrete_fields
 
         # Always pass down all the fields on an insert
         return [
             (
                 InsertCommand(
                     self.connection,
                     self.query.model,
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/dnf.py` & `django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/parsers/dnf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 """ Disjunctive Normal Form (DNF). https://en.wikipedia.org/wiki/Disjunctive_normal_form
     This module rearranges the WHERE trees of queries to make them executable on the Datastore.
     This is essentially moving the OR operators to the top of the WHERE tree to allow them to be
     performed as separate queries, because the Datastore can't perform OR operations within a query
 """
 
 import copy
-from functools import cmp_to_key
 from itertools import product
 
 from django.conf import settings
-from django.db import NotSupportedError
+from django.db import NotSupportedError, connections
 from django.core.exceptions import EmptyResultSet
-from google.cloud.datastore.key import Key
-
-from .query import WhereNode
-from .query_utils import compare_keys
+from gcloudc.db.backends.common.parsers.builder import WhereNode
 
 # Maximum number of subqueries in a multiquery
 DEFAULT_MAX_ALLOWABLE_QUERIES = 100
 
 
 def preprocess_node(node, negated):
 
@@ -35,28 +31,32 @@
                     child.value = None
                 else:
                     child.operator = ">"
                     child.value = None
 
             elif node.negated and child.operator == "=":
                 # Excluded equalities become inequalities
-
+                supports_only_null_equality = connections[node.using].supports_only_null_equality
                 lhs, rhs = WhereNode(node.using), WhereNode(node.using)
                 lhs.column = rhs.column = child.column
                 lhs.value = rhs.value = child.value
                 lhs.is_iterable_field = rhs.is_iterable_field = child.is_iterable_field
                 lhs.operator = "<"
                 rhs.operator = ">"
 
-                child.operator = child.value = child.column = None
                 child.connector = "OR"
                 child.children = [lhs, rhs]
-
-                assert not child.is_leaf
-
+                if supports_only_null_equality and child.value is not None:
+                    # We're not excluding None, so we should explicitly look for it
+                    extra = WhereNode(node.using)
+                    extra.column = lhs.column
+                    extra.value = None
+                    extra.operator = "="
+                    child.children.append(extra)
+                child.operator = child.value = child.column = None
             elif child.operator == "IN":
                 # Explode IN filters into a series of 'OR statements to make life
                 # easier later
                 new_children = []
 
                 for value in child.value:
                     if node.negated:
@@ -209,15 +209,15 @@
     for and_branch in query.where.children:
         if and_branch.is_leaf:
             children = [and_branch]
         else:
             children = and_branch.children
 
         for node in children:
-            if node.column == "__key__" and node.operator in ("=", "IN"):
+            if node.column == query.connection.key_property_name() and node.operator in ("=", "IN"):
                 break
         else:
             all_pks = False
             break
 
     MAX_ALLOWABLE_QUERIES = getattr(settings, "DJANGAE_MAX_QUERY_BRANCHES", DEFAULT_MAX_ALLOWABLE_QUERIES)
 
@@ -263,15 +263,15 @@
         for and_branch in node.children[:]:
             # If we have a Root OR with leaf elements, we don't need to worry
             if and_branch.is_leaf:
                 break
 
             pk_equality_found = None
             for child in and_branch.children:
-                if child.column == "__key__" and child.operator == "=":
+                if child.column == query.connection.key_property_name() and child.operator == "=":
                     if pk_equality_found and pk_equality_found != child.value:
                         # Remove this AND branch as it's impossible to return anything
                         if and_branch in node.children:
                             node.children.remove(and_branch)
                     else:
                         pk_equality_found = child.value
             if not node.children:
@@ -295,17 +295,14 @@
             altered = False
             for node in and_branch.children:
                 key = (node.column, node.operator)
                 if key in seen:
                     altered = True
 
                     cmp_kwargs = {}
-                    if isinstance(seen[key].value, Key) or isinstance(node.value, Key):
-                        cmp_kwargs["key"] = cmp_to_key(compare_keys)
-
                     if node.operator in ('<', '<='):
                         seen[key].value = min(seen[key].value, node.value, **cmp_kwargs)
                     elif node.operator in ('>', '>='):
                         seen[key].value = max(seen[key].value, node.value, **cmp_kwargs)
                     elif node.operator == "=":
                         if isinstance(node.value, (list, tuple, set)):
                             # Iterable fields can filter on more than one value using
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/expressions.py` & `django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/parsers/expressions.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 from django.db.models.aggregates import Aggregate
 from django.db.models.expressions import (
     Expression,
     Col,
     F,
 )
 
-from gcloudc.db.backends.datastore.utils import get_prepared_db_value
+from gcloudc.db.backends.common.helpers import get_prepared_db_value
+
 
 CONNECTORS = {
-    F.ADD: lambda l, r: l + r,
-    F.SUB: lambda l, r: l - r,
-    F.MUL: lambda l, r: l * r,
-    F.DIV: lambda l, r: l / r,
+    F.ADD: lambda l, r: l + r,  # noqa:E741
+    F.SUB: lambda l, r: l - r,  # noqa:E741
+    F.MUL: lambda l, r: l * r,  # noqa:E741
+    F.DIV: lambda l, r: l / r,  # noqa:E741
 }
 
 
 def evaluate_expression(expression, instance, connection):
     """ A limited evaluator for Django's F expressions. This are evaluated within
         the get/put transaction in _update_entity so these will happen atomically
     """
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/formatting.py` & `django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/formatting.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import unicode_literals
 
-import json
 
 SELECT_PATTERN = """
 SELECT (%(columns)s) FROM %(table)s
 WHERE %(where)s
 ORDER BY %(order)s
 OFFSET %(offset)s
 LIMIT %(limit)s
@@ -54,34 +53,49 @@
         "columns": ", ".join(columns),
         "values": _generate_values_expression(command.objs, columns),
     }
 
     return (INSERT_PATTERN % params).replace("\n", " ").strip()
 
 
-def _generate_where_expression(representation):
+def _generate_where_expression(command):
     where = []
-    for branch in representation["where"]:
-        branch = "(" + " AND ".join(["%s%s" % (k, _quote_string(v)) for k, v in branch.items()]) + ")"
-        where.append(branch)
+    for branch in command.query.queries:
+        filters = []
+        for key, values in branch.filters.items():
+            (column, operator) = key
+            if len(values) == 1:
+                filters.append(f"{column}{operator}{_quote_string(values[0])}")
+            else:
+                assert operator == '='
+                quoted = map(_quote_string, values)
+                filters.append(f"{column} IN ({', '.join(quoted)})")
+
+        branch_sql = (
+            "("
+            + " AND ".join(filters)
+            + ")"
+        )
+
+        where.append(branch_sql)
 
     return " OR ".join(where)
 
 
 def _quote_string(value):
     needs_quoting = isinstance(value, str)
     # in ANSI SQL as well as GQL, string literals are wrapped in single quotes
     return "'{}'".format(value) if needs_quoting else str(value)
 
 
-def _generate_select_sql(command, representation):
-    has_offset = representation["low_mark"] > 0
-    has_limit = representation["high_mark"] is not None
-    has_ordering = bool(representation["order_by"])
-    has_where = bool(representation["where"])
+def _generate_select_sql(command):
+    has_offset = (command.original_query.low_mark or 0) > 0
+    has_limit = command.original_query.high_mark is not None
+    has_ordering = bool(command.query.ordering)
+    has_where = bool(len(command.query.queries) > 0)
 
     lines = SELECT_PATTERN.split("\n")
 
     # Remove limit and offset and where if we don't need them
     if not has_limit:
         del lines[4]
 
@@ -94,83 +108,86 @@
     if not has_where:
         del lines[1]
 
     sql = "\n".join(lines)
 
     columns = (
         "*"
-        if not representation["columns"]
-        else ", ".join(sorted(representation["columns"]))  # Just to make the output predictable
+        if not command.query.only_return_fields and not command.query.only_return_keys
+        else ", ".join(sorted(command.query.only_return_fields or command.query.wrapper.key_property_name()))  # noqa Just to make the output predictable
     )
 
     ordering = [
-        ("%s %s" % (x.lstrip("-"), "DESC" if x.startswith("-") else "")).strip() for x in representation["order_by"]
+        ("%s %s" % (x.lstrip("-"), "DESC" if x.startswith("-") else "")).strip() for x in command.query.ordering
     ]
 
     replacements = {
-        "table": representation["table"],
+        "table": command.query.queries[0].path[0],
         "columns": columns,
-        "offset": representation["low_mark"],
-        "limit": (representation["high_mark"] or 0) - (representation["low_mark"] or 0),
-        "where": _generate_where_expression(representation),
+        "offset": command.original_query.low_mark,
+        "limit": (command.original_query.high_mark or 0) - (command.original_query.low_mark or 0),
+        "where": _generate_where_expression(command),
         "order": ", ".join(ordering),
     }
 
     return (sql % replacements).replace("\n", " ").strip()
 
 
-def _generate_delete_sql(command, representation):
-    has_where = bool(representation["where"])
+def _generate_delete_sql(command):
+    has_where = bool(len(command.query.queries) > 0)
+
+    replacements = {
+        "table": command.query.queries[0].path[0],
+        "where": _generate_where_expression(command),
+    }
 
     lines = DELETE_PATTERN.split("\n")
     if not has_where:
         del lines[1]
 
     sql = "\n".join(lines)
 
     return (
-        (sql % {"table": representation["table"], "where": _generate_where_expression(representation)})
+        (sql % replacements)
         .replace("\n", " ")
         .strip()
     )
 
 
-def _generate_update_sql(command, representation):
-    has_where = bool(representation["where"])
+def _generate_update_sql(command):
+    has_where = bool(len(command.query.queries) > 0)
 
     lines = UPDATE_PATTERN.split("\n")
     if not has_where:
         del lines[2]
 
     sql = "\n".join(lines)
     columns = sorted([x[0].column for x in command.values])
 
     values = {x[0].column: str(x[2]) for x in command.values}
 
     params = {
-        "table": representation["table"],
+        "table": command.query.queries[0].path[0],
         "columns": ", ".join(columns),
         "values": "(" + ", ".join([values[x] for x in columns]) + ")",
-        "where": _generate_where_expression(representation),
+        "where": _generate_where_expression(command),
     }
 
     return (sql % params).replace("\n", " ").strip()
 
 
 def generate_sql_representation(command):
     from .commands import SelectCommand, DeleteCommand, UpdateCommand, InsertCommand
 
     if isinstance(command, InsertCommand):
         # Inserts don't have a .query so we have to deal with them
         # separately
         return _generate_insert_sql(command)
 
-    representation = json.loads(command.query.serialize())
-
     if isinstance(command, SelectCommand):
-        return _generate_select_sql(command, representation)
+        return _generate_select_sql(command)
     elif isinstance(command, DeleteCommand):
-        return _generate_delete_sql(command, representation)
+        return _generate_delete_sql(command)
     elif isinstance(command, UpdateCommand):
-        return _generate_update_sql(command, representation)
+        return _generate_update_sql(command)
 
     raise NotImplementedError("Unrecognized query type")
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/indexing.py` & `django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/indexing.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,18 @@
 
 import django
 import yaml
 from django.apps import apps
 from django.conf import settings
 from django.core.exceptions import ValidationError
 from django.db import models
-from google.cloud.datastore.entity import Entity
 
 from gcloudc.core.validators import MaxBytesValidator
-
-from . import transaction
-from .utils import get_top_concrete_parent
+from gcloudc.db.backends.common.helpers import get_top_concrete_parent
+from gcloudc.db.backends.common.base.entity import Entity
 
 logger = logging.getLogger(__name__)
 _project_special_indexes = {}
 _app_special_indexes = {}
 _last_loaded_times = {}
 _indexes_loaded = False
 
@@ -268,15 +266,15 @@
 
     def prep_value_for_database(self, value, index, **kwargs):
         raise NotImplementedError()
 
     def prep_value_for_query(self, value, **kwargs):
         raise NotImplementedError()
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, **kwargs):
         raise NotImplementedError()
 
     def prep_query_operator(self, op):
         if "__" in op:
             return op.split("__")[-1]
         else:
             return "exact"  # By default do an exact operation
@@ -380,15 +378,15 @@
             value = str(value)
         return value.lower()
 
     def prep_value_for_query(self, value, **kwargs):
         value = self.unescape(value)
         return value.lower()
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, **kwargs):
         return "_idx_iexact_{0}".format(field_column)
 
 
 class HourIndexer(TimeIndexerMixin, Indexer):
     OPERATOR = "hour"
 
     def validate_can_be_indexed(self, value, negated):
@@ -403,15 +401,15 @@
         if isinstance(value, int):
             return value
 
         if isinstance(value, str):
             value = datetime.datetime.strptime(value, "%Y-%m-%d %H:%M:%S")
         return value.hour
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, **kwargs):
         return "_idx_hour_{0}".format(field_column)
 
 
 class MinuteIndexer(TimeIndexerMixin, Indexer):
     OPERATOR = "minute"
 
     def validate_can_be_indexed(self, value, negated):
@@ -426,15 +424,15 @@
         if isinstance(value, int):
             return value
 
         if isinstance(value, str):
             value = datetime.datetime.strptime(value, "%Y-%m-%d %H:%M:%S")
         return value.minute
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, **kwargs):
         return "_idx_minute_{0}".format(field_column)
 
 
 class SecondIndexer(TimeIndexerMixin, Indexer):
     OPERATOR = "second"
 
     def validate_can_be_indexed(self, value, negated):
@@ -449,15 +447,15 @@
         if isinstance(value, int):
             return value
 
         if isinstance(value, str):
             value = datetime.datetime.strptime(value, "%Y-%m-%d %H:%M:%S")
         return value.second
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, **kwargs):
         return "_idx_second_{0}".format(field_column)
 
 
 class DayIndexer(DateIndexerMixin, Indexer):
     OPERATOR = "day"
 
     def validate_can_be_indexed(self, value, negated):
@@ -472,15 +470,15 @@
         if isinstance(value, int):
             return value
 
         if isinstance(value, str):
             value = datetime.datetime.strptime(value, "%Y-%m-%d %H:%M:%S")
         return value.day
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, **kwargs):
         return "_idx_day_{0}".format(field_column)
 
 
 class YearIndexer(DateIndexerMixin, Indexer):
     OPERATOR = "year"
 
     def validate_can_be_indexed(self, value, negated):
@@ -496,15 +494,15 @@
             return value
 
         if isinstance(value, str):
             value = datetime.datetime.strptime(value, "%Y-%m-%d %H:%M:%S")
 
         return value.year
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, **kwargs):
         return "_idx_year_{0}".format(field_column)
 
 
 class MonthIndexer(DateIndexerMixin, Indexer):
     OPERATOR = "month"
 
     def validate_can_be_indexed(self, value, negated):
@@ -520,15 +518,15 @@
             return value
 
         if isinstance(value, str):
             value = datetime.datetime.strptime(value, "%Y-%m-%d %H:%M:%S")
 
         return value.month
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, **kwargs):
         return "_idx_month_{0}".format(field_column)
 
 
 class WeekDayIndexer(DateIndexerMixin, Indexer):
     OPERATOR = "week_day"
 
     def validate_can_be_indexed(self, value, negated):
@@ -543,15 +541,15 @@
                 return zero_based_weekday + 2
 
         return None
 
     def prep_value_for_query(self, value, **kwargs):
         return value
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, **kwargs):
         return "_idx_week_day_{0}".format(field_column)
 
 
 class ContainsIndexer(StringIndexerMixin, Indexer):
     PREP_VALUE_RETURNS_ENTITIES = True
     OPERATOR = u"contains"
     INDEXED_COLUMN_NAME = OPERATOR
@@ -570,57 +568,76 @@
     def cleanup(cls, client, datastore_key):
 
         # Kindless query, we don't know the kinds because we don't know all the fields
         # that use contains. But, we do know that all the things we need to delete are:
         # a.) A descendent
         # b.) Have a key name of whatever OPERATOR is
 
-        qry = client.query(namespace=datastore_key.namespace, ancestor=datastore_key)
-        qry.keys_only()
+        qry = client.wrapper.get_query_class()(
+            connection=client.wrapper,
+            namespace=datastore_key.namespace,
+            table_or_path=list(datastore_key.path) + [datastore_key.id_or_name],
+            only_return_keys=True
+        )
 
         # Delete all the entities matching the ancestor query
-        client.delete([x.key for x in qry.fetch() if x.key.id_or_name == cls.OPERATOR])
+        keys = [
+            x.key()
+            for x in qry.fetch(offset=0, limit=None)
+            if x.key().id_or_name == cls.OPERATOR
+        ]
+        for key in keys:
+            client.delete(key)
 
     def _generate_kind_name(self, model, column):
         return "_djangae_idx_{}_{}".format(get_top_concrete_parent(model)._meta.db_table, column)
 
-    def _generate_permutations(self, value):
-        return [value[i:] for i in range(len(value))]
+    def _generate_permutations(self, value, connection):
+        if connection.supports_range_queries_on_array:
+            return [value[i:] for i in range(len(value))]
+        else:
+            results = set()
+            for i in range(len(value) + 1):
+                for j in range(i, len(value) + 1):
+                    new_v = value[i:j]
+                    if new_v:
+                        results.add(new_v)
+            return sorted(list(results))
 
     def prep_value_for_database(self, value, index, model, column, connection):
         if value is None:
             raise IgnoreForIndexing([])
 
         # If this a date or a datetime, or something that supports isoformat, then use that
         if hasattr(value, "isoformat"):
             value = value.isoformat()
 
         if _is_iterable(value):
-            value = list(chain(*[self._generate_permutations(v) for v in value]))
+            value = list(chain(*[self._generate_permutations(v, connection) for v in value]))
         else:
-            value = self._generate_permutations(value)
+            value = self._generate_permutations(value, connection)
 
         if not value:
             raise IgnoreForIndexing([])
 
         value = list(set(value))  # De-duplicate
 
-        key = transaction._rpc(using=connection.alias).key(
+        key = connection.connection.new_key(
             self._generate_kind_name(model, column), self.OPERATOR
         )
         entity = Entity(key)
         entity[self.INDEXED_COLUMN_NAME] = value
         return [entity]
 
     def prep_query_operator(self, operator):
         return "IN"
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, connection):
         # prep_value_for_query returns a list PKs, so we return __key__ as the column
-        return "__key__"
+        return connection.key_property_name()
 
     def prep_value_for_query(self, value, model, column, connection):
         """
             Return a list of IDs of the associated contains models, these should
             match up with the IDs from the parent entities
         """
 
@@ -633,35 +650,44 @@
         if STRIP_PERCENTS:
             # SQL does __contains by doing LIKE %value%
             if value.startswith("%") and value.endswith("%"):
                 value = value[1:-1]
 
         namespace = connection.namespace
 
-        qry = transaction._rpc(using=connection.alias).query(
-            kind=self._generate_kind_name(model, column), namespace=namespace
+        qry = connection.get_query_class()(
+            table_or_path=[self._generate_kind_name(model, column)],
+            is_nested_collection=True,
+            namespace=namespace,
+            connection=connection,
+            only_return_keys=True
         )
-        qry.keys_only()
-
-        qry.add_filter(self.INDEXED_COLUMN_NAME, ">=", value)
-        qry.add_filter(self.INDEXED_COLUMN_NAME, "<=", value + u"\ufffd")
 
+        if connection.supports_range_queries_on_array:
+            qry.add_filter(self.INDEXED_COLUMN_NAME, ">=", value)
+            qry.add_filter(self.INDEXED_COLUMN_NAME, "<=", value + u"\ufffd")
+        else:
+            qry.add_filter(self.INDEXED_COLUMN_NAME, "array_contains", value)
         # We can't filter on the 'name' as part of the query, because the name is the key and these
         # are child entities of the ancestor entities which they are indexing, and as we don't know
         # the keys of the ancestor entities we can't create the complete keys, hence the comparison
         # of `x.name() == self.OPERATOR` happens here in python
-        resulting_keys = set([x.key.parent for x in qry.fetch() if x.key.name == self.OPERATOR])
+        resulting_keys = set([
+            x.key().ancestor()
+            for x in qry.fetch(offset=0, limit=None)
+            if x.key().id_or_name == self.OPERATOR
+        ])
         return resulting_keys
 
 
 class IContainsIndexer(ContainsIndexer):
     OPERATOR = "icontains"
 
-    def _generate_permutations(self, value):
-        return super(IContainsIndexer, self)._generate_permutations(value.lower())
+    def _generate_permutations(self, value, connection):
+        return super(IContainsIndexer, self)._generate_permutations(value.lower(), connection)
 
     def prep_value_for_query(self, value, model, column, connection):
         return super(IContainsIndexer, self).prep_value_for_query(value.lower(), model, column, connection)
 
 
 class LegacyContainsIndexer(StringIndexerMixin, Indexer):
     OPERATOR = "contains"
@@ -722,15 +748,15 @@
         if STRIP_PERCENTS:
             # SQL does __contains by doing LIKE %value%
             if value.startswith("%") and value.endswith("%"):
                 value = value[1:-1]
 
         return value
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, **kwargs):
         # This we use when we actually query to return the right field for a given
         # value length
         length = len(value)
 
         column_number = 0
         for x in CHARACTERS_PER_COLUMN:
             if length > x:
@@ -747,15 +773,15 @@
     def prep_value_for_database(self, value, index, **kwargs):
         if value is None:
             raise IgnoreForIndexing("")
         value = _make_lower(value)
         result = super(LegacyIContainsIndexer, self).prep_value_for_database(value, index)
         return result if result else None
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, **kwargs):
         column_name = super(LegacyIContainsIndexer, self).indexed_column_name(field_column, value, index)
         return column_name.replace("_idx_contains_", "_idx_icontains_")
 
     def prep_value_for_query(self, value, **kwargs):
         return super(LegacyIContainsIndexer, self).prep_value_for_query(value).lower()
 
 
@@ -800,15 +826,15 @@
     def prep_value_for_query(self, value, **kwargs):
         value = self.unescape(value)
         if STRIP_PERCENTS:
             if value.startswith("%"):
                 value = value[1:]
         return value
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, **kwargs):
         return "_idx_endswith_{0}".format(field_column)
 
     def prep_query_operator(self, op):
         return "exact"
 
 
 class IEndsWithIndexer(EndsWithIndexer):
@@ -822,15 +848,15 @@
         if value:
             value = _make_lower(value)
         return super(IEndsWithIndexer, self).prep_value_for_database(value, index)
 
     def prep_value_for_query(self, value, **kwargs):
         return super(IEndsWithIndexer, self).prep_value_for_query(value.lower())
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, **kwargs):
         return "_idx_iendswith_{0}".format(field_column)
 
 
 class StartsWithIndexer(StringIndexerMixin, Indexer):
     """
         Although we can do a startswith natively, doing it this way allows us to
         use more queries (E.g. we save an exclude)
@@ -871,15 +897,15 @@
     def prep_value_for_query(self, value, **kwargs):
         value = self.unescape(value)
         if STRIP_PERCENTS:
             if value.endswith("%"):
                 value = value[:-1]
         return value
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, **kwargs):
         return "_idx_startswith_{0}".format(field_column)
 
     def prep_query_operator(self, op):
         return "exact"
 
 
 class IStartsWithIndexer(StartsWithIndexer):
@@ -893,15 +919,15 @@
         if value:
             value = _make_lower(value)
         return super(IStartsWithIndexer, self).prep_value_for_database(value, index)
 
     def prep_value_for_query(self, value, **kwargs):
         return super(IStartsWithIndexer, self).prep_value_for_query(value.lower())
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, **kwargs):
         return "_idx_istartswith_{0}".format(field_column)
 
 
 def _to_hex(value):
     value = codecs.encode(
         value.encode("utf8"), "hex"
     ).decode("utf8")
@@ -952,15 +978,15 @@
 
     def prep_value_for_database(self, value, index, **kwargs):
         return self.check_if_match(value, index)
 
     def prep_value_for_query(self, value, **kwargs):
         return True
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, **kwargs):
         return "_idx_regex_{0}_{1}".format(field_column, _to_hex(self.get_pattern(index)))
 
     def prep_query_operator(self, op):
         return "exact"
 
 
 class IRegexIndexer(RegexIndexer):
@@ -968,15 +994,15 @@
 
     def prepare_index_type(self, index_type, value):
         return "{}__{}".format(index_type, _to_hex(value))
 
     def prep_value_for_database(self, value, index, **kwargs):
         return self.check_if_match(value, index, flags=re.IGNORECASE)
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, **kwargs):
         return "_idx_iregex_{0}_{1}".format(field_column, _to_hex(self.get_pattern(index)))
 
 
 _REGISTERED_INDEXERS = []
 
 
 def register_indexer(indexer_class):
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/meta_queries.py` & `django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/base/query.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,484 +1,455 @@
-import copy
-import threading
-from functools import cmp_to_key, partial
-from itertools import groupby
-
-from django.conf import settings
-from google.cloud.datastore.key import Key
-
-from . import POLYMODEL_CLASS_ATTRIBUTE, caching
-from .query_utils import compare_keys, get_filter, is_keys_only
-from .utils import django_ordering_comparison, entity_matches_query
-
-
-class AsyncMultiQuery(object):
-    """
-        Runs multiple queries simultaneously and merges the result sets based on the
-        shared ordering.
-    """
-
-    # Testing seems to show that more threads == better, but I'm concerned if we
-    # raise this too high we'll start hitting bottlenecks elsewhere. Serious performance
-    # testing needs to happen. Theoretically I think we could make THREAD_COUNT == len(queries)
-    # but I'd rather prove that doesn't cause problems before I do it!
-    THREAD_COUNT = 8
-
-    def __init__(self, queries, orderings):
-        self._queries = [copy.copy(x) for x in queries]
-        self._orderings = orderings
-        self._min_max_cache = {}
-
-        # When set, this is called on the query before .Run() is called
-        # Which allows you to manipulate the options. Recommend this is set/unset
-        # in a try/finally
-        self._query_decorator = None
-        self._keys_only = False
-
-    def keys_only(self):
-        self._keys_only = True
-        for query in self._queries:
-            query.keys_only()
+from typing import List, Set, Union
 
-    def _spawn_thread(self, i, query, result_queues, **query_run_args):
-        """
-            Spawns a thread to return a queries resultset
+from .entity import Key, Entity
+from .connection import Wrapper
+from gcloudc.db.backends.common.helpers import entity_matches_query
+from django.db import ProgrammingError
+from functools import cmp_to_key
+
+#  This is a list of the possible operators accepted by the query class when adding
+#  filters. It may seem that there should be more of these (e.g. IN, contains-any etc.)
+#  However:
+#    - Even on Firestore, OR queries are performed on disjunctive normal form representations
+#      of the query, that's exactly what we're doing anyway so using the Firestore version
+#      probably doesn't buy us much, at the cost of increased complexity
+#    - contains-any is just the same thing, it goes through the list of values running an OR
+#      query
+#    - contains is just an equality on a list property, it's a little counter intuitive but that's
+#      what it is
+#    - is null is just `= None`
+
+
+class Operator:
+    EQ = "="
+    LT = "<"
+    LTE = "<="
+    GT = ">"
+    GTE = ">="
+
+
+class Query:
+    def __init__(
+        self, wrapper: Wrapper, table_or_path,
+        only_return_keys=False,
+        only_return_fields=None,
+        namespace=None,
+        is_nested_collection=False,  # Whether this query is for a nested collection or not
+    ):
+        wrapper.ensure_connection()
 
-            *Note* by evaluating the entire query results in the thread we ruin the datastore
-            query batching in the situation that you:
+        self.connection = wrapper.connection
+        self.wrapper = wrapper
+        self.namespace = namespace
+        self.only_return_keys = only_return_keys
+        self.only_return_fields = only_return_fields or []
+        self.path = (
+            table_or_path
+            if isinstance(table_or_path, (list, tuple))
+            else [table_or_path]
+        )
+
+        # A dict of (col, op): [values] of filters
+        # that have been added to this query
+        self._filters = {}
+
+        # A list of orderings that have been added to this query
+        self._orderings = []
+
+    @property
+    def filters(self):
+        return self._filters
+
+    def distinct_on(self, fields):
+        raise NotImplementedError()
+
+    def has_filter(self, property, operator) -> bool:
+        return (property, operator) in self._filters
+
+    def get_filter(self, property, operator):
+        return self._filters.get((property, operator))
+
+    def _add_filter(self, property, operator, value):
+        raise NotImplementedError()
+
+    def add_filter(self, property, operator, value):
+        self._add_filter(property, operator, value)
+        self._filters.setdefault((property, operator), []).append(value)
+
+    def fetch(self, offset, limit):
+        raise NotImplementedError()
+
+    def count(self, limit):
+        raise NotImplementedError()
+
+    def order_by(self, orderings):
+        self._order_by(orderings)
+        self._orderings.extend(orderings)
+
+    def _order_by(self, orderings):
+        raise NotImplementedError()
+
+    def __repr__(self):
+        return f"<Query {self.filters!r}>"
+
+
+class ORQuery:
+
+    def __init__(
+            self, wrapper, table_or_path, unique_combinations,
+            only_return_keys=False, only_return_fields=None,
+            namespace=None, select=None, distinct_fields=None,
+            annotations=None
+        ):  # noqa
+
+        self.wrapper = wrapper
+        self.queries = []
+
+        # self.select is the list of properties that an entity should have when
+        # it is returned. This is used externally to know what must be returned to Django
+        # when the results are processed. It's not always the same as only_return_fields
+        # and is set by the query parsing process
+        self.select = select
+
+        self.unique_combinations = unique_combinations
+        self.only_return_keys = only_return_keys
+        self.only_return_fields = only_return_fields or []
+        self.distinct_fields = distinct_fields
+        self.path = (
+            table_or_path
+            if isinstance(table_or_path, (list, tuple))
+            else [table_or_path]
+        )
+        self.ordering = []
+        self.namespace = namespace
+        self._excluded_keys: Set[Key] = set()
 
-             a. Have limited the query
-             b. Have a large number of results in one or more branches of the OR
+        # Annotations are in the form of (column, transform func, arguments)
+        # and are used to add additional data to entities being returned from
+        # queries
+        self.annotations = annotations or []
+
+    def set_excluded_keys(self, keys: Set[Key]):
+        self._excluded_keys = keys
+
+    def push_query(self, connection) -> Query:
+        query_class = connection.get_query_class()
+        query = query_class(
+            connection,
+            self.path,
+            only_return_keys=self.only_return_keys,
+            only_return_fields=self.only_return_fields,
+            namespace=self.namespace
+        )
+        self.queries.append(query)
+        return query
 
-            Basically, if you do this:
+    def query_count(self) -> int:
+        return len(self.queries)
 
-            MyModel.objects.filter(field1__in=("A", "B"))[:1000]
+    def query_at(self, i) -> Query:
+        return self.queries[i]
 
-            and you have 1000 results with "A" and 1000 results with "B" all
-            2000 results will be fetched even though you asked for 1000. However, this is
-            not the most likely situation for a MultiQuery when normally few results will be returned
-            by each branch. Threading seems to help in the common case but we can revisit
-            when we have more data. If threading isn't worth the cost we can revert to just using
-            async queries like Google's multiquery does.
-        """
+    def order_by(self, ordering):
+        self.ordering = ordering
 
-        keys_only = self._keys_only
+    def _apply_ordering(self):
+        for query in self.queries:
+            query.order_by(self.ordering)
+
+    def _apply_distinct(self):
+        if self.distinct_fields is None:
+            return
 
-        class Thread(threading.Thread):
-            def __init__(self, query, *args, **kwargs):
-                self.query = query
-                self.results_fetched = False
-                super(Thread, self).__init__(*args, **kwargs)
-
-            def run(self):
-                # Evaluate the result set in the thread, but return an iterator
-                # so we can change this if necessary without breaking assumptions elsewhere
-                result_queues[i] = (x.key if keys_only else x for x in self.query.fetch(**query_run_args))
-                self.results_fetched = True
-
-        if self._query_decorator:
-            query = self._query_decorator(query)
-
-        thread = Thread(query)
-        thread.start()
-        return thread
+        for query in self.queries:
+            query.distinct_on(self.distinct_fields)
 
-    def _fetch_results(self, limit=None):
+    def _can_use_get(self) -> bool:
         """
-            Returns a list of generators (one for each query in the multi query)
-            which generate entity results (or keys if it's keys_only)
-
-            Uses multiple threads to submit RPC calls
+            Returns true if every subquery does an equality filter on a key
         """
 
-        threads = []
+        for query in self.queries:
+            if not query.has_filter(self.wrapper.key_property_name(), Operator.EQ):
+                return False
+        else:
+            return True
 
-        # We need to grab a set of results per query
-        result_queues = [None] * len(self._queries)
+    def _unique_combo_for_query(self, query):
+        """
+            If this query has filters on a unique combination
+            this returns that combination of fields, otherwise
+            returns None
+        """
 
-        # Go through the queries, trigger new threads as they become available
-        for i, query in enumerate(self._queries):
-            # Iterate while we have a full thread list
-            while len(threads) >= self.THREAD_COUNT:
-                try:
-                    complete = next(x for x in threads if x.results_fetched)
-                except StopIteration:
-                    # No threads available, continue waiting
+        for combo in self.unique_combinations:
+            found = 0
+            for field in combo:
+                if query.has_filter(field, "="):
+                    found += 1
                     continue
 
-                # Remove the complete thread
-                complete.join()
-                threads.remove(complete)
-
-            # Spawn a new thread
-            threads.append(self._spawn_thread(i, query, result_queues, limit=limit))
-
-        [x.join() for x in threads]  # Wait until all the threads are done
-
-        return result_queues
-
-    def _compare_entities(self, lhs, rhs):
-        def cmp(a, b):
-            # Treat None as less than everything for the purpose
-            # of ordering
-            if a is None and b is None:
-                return 0
-            elif a is None:
-                return -1
-            elif b is None:
-                return 1
+            if found == len(combo):
+                return combo
 
-            return (a > b) - (a < b)
+        return None
 
-        if isinstance(lhs, Key) and isinstance(rhs, Key):
-            return compare_keys(lhs, rhs)
+    def _extract_keys(self) -> List[Key]:
+        assert (self._can_use_get())
+        result = []
+        for query in self.queries:
+            value = query.get_filter(self.wrapper.key_property_name(), Operator.EQ)
+            if len(value) > 1:
+                # If we have a key equality on more than one value
+                # it won't return anything, so do nothing
+                continue
 
-        def get_extreme_if_list_property(entity_key, column, value, descending):
-            if not isinstance(value, list):
-                return value
+            result.append(value[0])
 
-            if (entity_key, column) in self._min_max_cache:
-                return self._min_max_cache[(entity_key, column)]
+        return result
 
-            if descending:
-                value = min(value)
-            else:
-                value = max(value)
-            self._min_max_cache[(entity_key, column)] = value
+    def _check_queries_dont_match_cached_entities(self):
+        """
+            If we have an item in the transaction cache, and you make a query
+            for something that could match that cache we raise an exception to protect
+            you from accessing stale results. Items only go into the cache when you put
+            them, so if you subsequently run a query that would match a previously put
+            item you won't get it back.
+        """
 
-        if not lhs:
-            return cmp(lhs, rhs)
+        for query in self.queries:
+            query.wrapper.ensure_connection()
+            for v in query.wrapper.connection._cache.values():
+                if entity_matches_query(v, query):
+                    raise ProgrammingError(
+                        f"Performed query on collection {query.path} in a transaction "
+                        "that would match a document which has already been put"
+                    )
 
-        for column in self._orderings:
-            descending = column.startswith("-")
-            column = column.lstrip("-")
+    def _apply_annotations(self, entity):
+        for col, func, args in self.annotations:
+            entity[col] = func(entity, *args)
 
-            lhs_value = lhs.key if column == "__key__" else lhs[column]
-            rhs_value = rhs.key if column == "__key__" else rhs[column]
+    def fetch(self, offset, limit):
 
-            lhs_value = get_extreme_if_list_property(lhs.key, column, lhs_value, descending)
-            rhs_value = get_extreme_if_list_property(lhs.key, column, rhs_value, descending)
+        def cmp(a, b) -> int:
+            if a.less_than(b, self.ordering, self.wrapper.key_property_name()):
+                return -1
+            elif b.less_than(a, self.ordering, self.wrapper.key_property_name()):
+                return 1
+            return 0
 
-            if isinstance(lhs_value, Key) and isinstance(rhs_value, Key):
-                result = compare_keys(lhs_value, rhs_value)
-            else:
-                result = cmp(lhs_value, rhs_value)
+        # FIXME: deduplicate distinct entities
 
-            if descending:
-                result = -result
-            if result:
-                return result
+        # FIXME: Make async
+        self._apply_ordering()
+        self._apply_distinct()
+
+        original_limit = limit
+
+        # If we are excluding keys from the resultset, then
+        # we need to fetch more results than requested
+        if self._excluded_keys and limit is not None:
+            limit += len(self._excluded_keys)
+
+        resultsets = []
+        if len(self.queries) == 1:
+            # Simple case, single query branch (no OR) so we can leverage
+            # the database directly for most things
+
+            qry = self.queries[0]
+
+            # Optimisation, if we're filtering on a single key
+            # and that key is in the cache, then fallback to
+            # that. If the key isn't in the cache it's still more
+            # optimal to do a query than a get()
+            cache_hit = False
+            combo = self._unique_combo_for_query(qry)
+
+            if self._can_use_get():
+                keys = self._extract_keys()
+                if keys and keys[0] in qry.connection._cache:
+                    # Set the resultsets and fall through
+                    cache_hit = True
+                    resultsets = [
+                        [qry.connection.get(keys[0])]
+                    ]
+
+                    resultsets[0].sort(key=cmp_to_key(cmp))
+            elif combo:
+                # Unique combination optimisation. If we query on a unique
+                # combination, and that exists in the cache, then don't do
+                # a query
+                values = [(k, qry.get_filter(k, "=")[0]) for k in combo]
+                entity = qry.connection._find_entity_in_cache(values)
+                if entity:
+                    cache_hit = True
+                    resultsets = [[entity]]
+
+            if not cache_hit:
+                self._check_queries_dont_match_cached_entities()
+
+                returned_count = 0
+                for entity in qry.fetch(offset=offset, limit=limit):
+                    if limit is not None and returned_count == original_limit:
+                        return
 
-        return compare_keys(lhs.key, rhs.key)
+                    key = entity.key()
+                    if key in self._excluded_keys:
+                        continue
 
-    def fetch(self, offset=None, limit=None):
-        """
-            Returns an iterator through the result set.
+                    self._apply_annotations(entity)
+                    returned_count += 1
+                    yield entity
+        elif self._can_use_get():
+            # Optimisation, if we can do a get() query with the available
+            # keys then do that because multiple key filters will mean many
+            # queries, when we can just do one and then filter in memory
+            keys = self._extract_keys()
+            wrapper = self.queries[0].wrapper
+            conn = wrapper.connection
+            resultsets = conn.get([x for x in keys if x])
+            resultsets = [
+                [x] for x in resultsets
+                if any([entity_matches_query(x, qry) for qry in self.queries])
+            ]
+        else:
+            # FIXME: Should we handle looking up unique entities in the cache
+            # in multi-query situations? We currently only do this in the single-query
+            # version
+            self._check_queries_dont_match_cached_entities()
+            if limit is not None:
+                offset = offset or 0
+                limit = offset + limit
 
-            This calls _fetch_results which returns a list of iterators,
-            where each is the result of a single query. This function does a
-            zig-zag merge of the entities. It starts by creating a list of the next
-            entry in each resultset, then iteratively picks the next entity and then
-            fills the slot from the counterpart result set until all the slots are None.
-        """
-        self._min_max_cache = {}
+            for qry in self.queries:
+                resultsets.append([x for x in qry.fetch(offset=0, limit=limit)])
 
-        # We have to assume that one branch might return all the results and as
-        # offsetting is done by skipping results we need to get offset + limit results
-        # from each branch
-        results = self._fetch_results(limit=(offset or 0) + limit if limit is not None else None)
+            for resultset in resultsets:
+                resultset.sort(key=cmp_to_key(cmp))
 
         # Go through each outstanding result queue and store
         # the next entry of each (None if the result queue is done)
-        next_entries = [None] * len(results)
-        for i, queue in enumerate(results):
-            try:
-                next_entries[i] = next(results[i])
-            except StopIteration:
-                next_entries[i] = None
+        next_entries = [None] * len(resultsets)
+
+        def shift_queue(idx):
+            while resultsets[idx]:
+                try:
+                    next_entries[idx] = resultsets[idx].pop(0)
+                except IndexError:
+                    next_entries[idx] = None
+                else:
+                    key = next_entries[idx].key()
+                    if key in self._excluded_keys:
+                        continue
+                    else:
+                        break
+            else:
+                next_entries[idx] = None
+
+        for i in range(len(resultsets)):
+            shift_queue(i)
 
         returned_count = 0
         yielded_count = 0
 
         seen_keys = set()  # For de-duping results
-        while any(next_entries):
+        while any([x for x in next_entries if x is not None]):
 
             def get_next():
                 idx, lowest = None, None
 
                 for i, entry in enumerate(next_entries):
                     if entry is None:
                         continue
 
-                    if lowest is None or self._compare_entities(entry, lowest) < 0:
+                    if lowest is None or self._less_than(entry, lowest, self.ordering):
                         idx, lowest = i, entry
 
                 # Move the queue along if we found the entry there
-                if lowest is not None:
-                    try:
-                        next_entries[idx] = next(results[idx])
-                    except StopIteration:
-                        next_entries[idx] = None
+                if lowest is not None and idx is not None:
+                    shift_queue(idx)
 
                 return lowest
 
             # Find the next entry from the available queues
             next_entity = get_next()
 
             # No more entries if this is the case
             if next_entity is None:
                 break
 
-            next_key = next_entity if isinstance(next_entity, Key) else next_entity.key
+            next_key = next_entity.key()
 
             # Make sure we haven't seen this result before before yielding
             if next_key not in seen_keys:
                 returned_count += 1
                 seen_keys.add(next_key)
 
                 if offset and returned_count <= offset:
                     # We haven't hit the offset yet, so just
                     # keep fetching entities
                     continue
 
+                self._apply_annotations(next_entity)
+
                 yielded_count += 1
                 yield next_entity
 
-                if limit and yielded_count == limit:
+                if limit and yielded_count == original_limit:
                     break
 
+    def count(self, limit=None):
+        # FIXME: deduplicate distinct entities
+        original_limit = limit
+
+        results = []
+        if self._excluded_keys:
+            if limit is not None:
+                limit += len(self._excluded_keys)
+
+            # We have to skip these manually
+            for query in self.queries:
+                query.only_return_keys = True
+                count = 0
+                for result in query.fetch(offset=None, limit=limit):
+                    if result.key() in self._excluded_keys:
+                        continue
+                    else:
+                        count += 1
+                results.append(count)
+        else:
+            for query in self.queries:
+                results.append(query.count(limit=limit))
 
-def _convert_entity_based_on_query_options(entity, keys_only, projection):
-    if keys_only:
-        return entity.key
-
-    if projection:
-        keys = list(entity.keys())
-        for k in keys:
-            if k not in list(projection) + [POLYMODEL_CLASS_ATTRIBUTE]:
-                del entity[k]
-
-    return entity
-
-
-# The max number of entities in a resultset that will be cached
-# if a query returns more than this number then only the first ones
-# will be cached
-DEFAULT_MAX_ENTITY_COUNT = 8
-
-
-class QueryByKeys(object):
-    """ Does the most efficient fetching possible for when we have the keys of the entities we want. """
-
-    def __init__(self, connection, model, queries, ordering, namespace):
-        # Imported here for potential circular import and isolation reasons
-        from .dnf import DEFAULT_MAX_ALLOWABLE_QUERIES
-
-        # `queries` should be filtered by __key__ with keys that have the namespace applied to them.
-        # `namespace` is passed for explicit niceness (mostly so that we don't have to assume that
-        # all the keys belong to the same namespace, even though they will).
-        def _get_key(query):
-            result = get_filter(query, ("__key__", "="))
+        result = sum(results)
+        if original_limit is not None:
+            return min(result, original_limit)
+        else:
             return result
 
-        def compare_queries(lhs, rhs):
-            return compare_keys(_get_key(lhs), _get_key(rhs))
-
-        self.connection = connection
-        self.model = model
-        self.namespace = namespace
-
-        # groupby requires that the iterable is sorted by the given key before grouping
-        self.queries = sorted(queries, key=cmp_to_key(compare_queries))
-        self.query_count = len(self.queries)
-        self.queries_by_key = {a: list(b) for a, b in groupby(self.queries, _get_key)}
-
-        self.max_allowable_queries = getattr(settings, "DJANGAE_MAX_QUERY_BRANCHES", DEFAULT_MAX_ALLOWABLE_QUERIES)
-        self.can_multi_query = self.query_count < self.max_allowable_queries
-
-        self.ordering = ordering
-        self.kind = queries[0].kind
-        self._keys_only_override = False
-
-    def keys_only(self):
-        self._keys_only_override = True
-
-    def fetch(self, limit=None, offset=None):
+    def _less_than(self, lhs: Union[Entity, Key], rhs: Union[Entity, Key], ordering: List[str]) -> bool:
         """
-            Here are the options:
-
-            1. Single key, hit memcache
-            2. Multikey projection, async MultiQueries with ancestors chained
-            3. Full select, datastore get
+            Returns True if lhs < rhs depending on the ordering.
         """
-        from gcloudc.db.backends.datastore import transaction
-        from gcloudc.db.backends.datastore.caching import MAX_CACHE_COUNT
-
-        base_query = self.queries[0]
-        key_count = len(self.queries_by_key)
-
-        is_projection = False
-
-        cache_results = True
-        results = None
-
-        if key_count == 1:
-            # FIXME: Potentially could use get_multi in memcache and the make a query
-            # for whatever remains
-            key = next(iter(self.queries_by_key))
-            assert (isinstance(key, Key))
-
-            result = caching.get_from_cache_by_key(key)
-            if result is not None:
-                results = [result]
-                cache_results = False  # Don't update cache, we just got it from there
-
-        client = transaction._rpc(self.connection)
-
-        if results is None:
-            if base_query.projection and self.can_multi_query:
-                is_projection = True
-
-                # If we can multi-query in a single query, we do so using a number of
-                # ancestor queries (to stay consistent) otherwise, we just do a
-                # datastore Get, but this will return extra data over the RPC
-                to_fetch = (offset or 0) + limit if limit else None
-
-                # strip the optional "-" prefix from order (indicating descending order)
-                additional_cols = set([
-                    x if x[0] != "-" else x[1:]
-                    for x in self.ordering
-                    if x not in base_query.projection
-                ])
-
-                multi_query = []
-                orderings = base_query.order
-                for key, queries in self.queries_by_key.items():
-                    for query in queries:
-                        if additional_cols:
-                            # We need to include additional orderings in the projection so that we can
-                            # sort them in memory. Annoyingly that means reinstantiating the queries
-                            query = client.query(
-                                kind=query.kind,
-                                filters=query.filters,
-                                projection=list(base_query.projection) + list(additional_cols),
-                                namespace=self.namespace,
-                            )
-
-                        query.ancestor = key  # Make this an ancestor query
-                        multi_query.append(query)
-
-                if len(multi_query) == 1:
-                    results = multi_query[0].fetch(limit=to_fetch)
-                else:
-                    results = AsyncMultiQuery(multi_query, orderings).fetch(limit=to_fetch)
-            else:
-                # Can pass 1000 keys to a datastore.Get, so if there are more we need to do them
-                # in multiple gets
-                MAX_ALLOWED_GET = 1000
-
-                all_keys = list(self.queries_by_key.keys())
-                next_keys, remaining_keys = all_keys[:MAX_ALLOWED_GET], all_keys[MAX_ALLOWED_GET:]
-
-                results = []
-                while next_keys:
-                    results.extend(client.get(next_keys))
-                    next_keys, remaining_keys = remaining_keys[:MAX_ALLOWED_GET], remaining_keys[MAX_ALLOWED_GET:]
-
-        def iter_results(results):
-            returned = 0
-
-            # This is safe, because Django is fetching all results any way :(
-            sorted_results = sorted(results, key=cmp_to_key(partial(django_ordering_comparison, self.ordering)))
-            sorted_results = [result for result in sorted_results if result is not None]
-
-            if cache_results and sorted_results and not base_query.projection:
-                caching.add_entities_to_cache(
-                    self.model,
-                    sorted_results[:MAX_CACHE_COUNT],
-                    caching.CachingSituation.DATASTORE_GET,
-                    self.namespace,
-                    connection_alias=self.connection
-                )
-
-            for result in sorted_results:
-                if is_projection:
-                    matches_query = True
-                else:
-                    matches_query = any(entity_matches_query(result, qry) for qry in self.queries_by_key[result.key])
-
-                if not matches_query:
-                    continue
-
-                if offset and returned < offset:
-                    # Skip entities based on offset
-                    returned += 1
-                    continue
-                else:
-                    yield _convert_entity_based_on_query_options(
-                        result, self._keys_only_override or is_keys_only(base_query), base_query.projection
-                    )
-
-                    returned += 1
-
-                    # If there is a limit, we might be done!
-                    if limit is not None and returned == (offset or 0) + limit:
-                        break
-
-        return iter_results(results)
-
-
-class NoOpQuery(object):
-    def fetch(self, limit, offset):
-        return []
-
-
-class UniqueQuery(object):
-    """
-        This mimics a normal query but hits the cache if possible. It must
-        be passed the set of unique fields that form a unique constraint
-    """
 
-    def __init__(self, connection, unique_identifier, gae_query, model, namespace):
-        self._identifier = unique_identifier
-        self._gae_query = gae_query
-        self._model = model
-        self._namespace = namespace
-        self._connection = connection
-        self._keys_only = False
-
-        self.kind = gae_query.kind
-
-    def keys_only(self):
-        self._gae_query.keys_only()
-        self._keys_only = True
-
-    def fetch(self, limit, offset):
-        do_cache = True
-        ret = caching.get_from_cache(self._identifier, self._namespace)
-
-        if ret is not None:
-            if not entity_matches_query(ret, self._gae_query):
-                ret = None
-            else:
-                ret = [ret]
-
-        if ret is None:
-            ret = list(self._gae_query.fetch(limit=limit, offset=offset))
-        else:
-            # We don't want to cache a result already coming from the cache...
-            do_cache = False
-
-        if self._keys_only or self._gae_query.projection:
-            # ...nor if it's coming from a keys_only/projection query
-            do_cache = False
-
-        if len(ret) == 1 and do_cache:
-            caching.add_entities_to_cache(
-                self._model,
-                [ret[0]],
-                caching.CachingSituation.DATASTORE_GET,
-                self._namespace,
-                connection_alias=self._connection
-            )
-
-        return iter(ret)
+        if isinstance(lhs, Key) and isinstance(rhs, Key):
+            return lhs < rhs
+        elif isinstance(lhs, Key) != isinstance(rhs, Key):
+            raise ValueError("Tried to compare Entity with Key")
+
+        # Handle None cases (None is always less)
+        if lhs is None and rhs is None:
+            return False
+        elif lhs is None:
+            return True
+        elif rhs is None:
+            return False
+
+        return lhs.less_than(
+            rhs, ordering,
+            self.queries[0].wrapper.key_property_name()
+        )
+
+    def __repr__(self):
+        queries_repr = "\n".join([f'\t{x!r}' for x in self.queries])
+        return f"<ORQuery \n{queries_repr}\n>"
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/query.py` & `django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/commands.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,683 +1,678 @@
-import datetime
-import json
+import copy
 import logging
-import re
-from itertools import chain
+from datetime import datetime
 
 from django.db import (
-    NotSupportedError,
-    connections,
+    DatabaseError,
+    IntegrityError,
+    OperationalError,
+)
+from django.db.models.expressions import Star
+from django.utils.encoding import (
+    force_str,
 )
-from django.db.models import AutoField
-from django.core.exceptions import EmptyResultSet
 
-from . import POLYMODEL_CLASS_ATTRIBUTE
-from .indexing import (
-    add_special_index,
-    get_indexer,
+from gcloudc.db.backends.common.base.entity import Entity
+from gcloudc.db.backends.common import helpers
+from django.db.transaction import atomic
+from gcloudc.db.backends.common.base.dbapi import NotSupportedError
+
+from .formatting import generate_sql_representation
+from gcloudc.db.backends.common.constraints import (
+    _unique_combinations,
+    CONSTRAINT_VIOLATION_MSG,
 )
-from .utils import (
+
+from gcloudc.db.backends.common.helpers import (
+    MockInstance,
+    django_instance_to_entities,
     ensure_datetime,
-    get_field_from_column,
-    get_top_concrete_parent,
+    get_document_key,
     has_concrete_parents,
+    get_model_from_db_table
 )
 
+# We can retry transactions only if the command is not
+# being executed within an existing transaction. This controls
+# how many times we try in that case.
+_TRANSACTION_TRIES = 5
+
 logger = logging.getLogger(__name__)
 
+OPERATORS_MAP = {
+    "exact": "=",
+    "gt": ">",
+    "gte": ">=",
+    "lt": "<",
+    "lte": "<=",
+    # The following operators are supported with special code below.
+    "isnull": None,
+    "in": None,
+    "range": None,
+}
 
-VALID_QUERY_KINDS = ("SELECT", "UPDATE", "INSERT", "DELETE", "COUNT", "AVERAGE")
+EXTRA_SELECT_FUNCTIONS = {
+    "+": lambda x, y: x + y,
+    "-": lambda x, y: x - y,
+    "/": lambda x, y: x / y,
+    "*": lambda x, y: x * y,
+    "<": lambda x, y: x < y,
+    ">": lambda x, y: x > y,
+    "=": lambda x, y: x == y,
+}
 
-VALID_ANNOTATIONS = {"MIN": min, "MAX": max, "SUM": sum, "COUNT": len, "AVG": lambda x: (sum(x) / len(x))}
+REVERSE_OP_MAP = {"=": "exact", ">": "gt", ">=": "gte", "<": "lt", "<=": "lte"}
 
-VALID_CONNECTORS = ("AND", "OR")
+INEQUALITY_OPERATORS = frozenset([">", "<", "<=", ">="])
 
 
-VALID_OPERATORS = ("=", "<", ">", "<=", ">=", "IN")
+def field_conv_year_only(value):
+    value = ensure_datetime(value)
+    return datetime(value.year, 1, 1, 0, 0)
 
 
-def convert_operator(operator):
-    if operator == "exact":
-        return "="
-    elif operator == "gt":
-        return ">"
-    elif operator == "lt":
-        return "<"
-    elif operator == "gte":
-        return ">="
-    elif operator == "lte":
-        return "<="
-
-    return operator.upper()
-
-
-class WhereNode(object):
-    def __init__(self, using):
-        self.using = using
-
-        self.column = None
-        self.operator = None
-        self.value = None
-        self.output_field = None
-        self.will_never_return_results = False
-        self.lookup_name = None
-        self.is_iterable_field = False
-
-        self.children = []
-        self.connector = "AND"
-        self.negated = False
-
-    @property
-    def is_leaf(self):
-        return bool(self.column and self.operator)
-
-    def set_connector(self, connector):
-        self.connector = connector
-
-    def append_child(self, node):
-        self.children.append(node)
-
-    def set_leaf(self, column, operator, value, is_pk_field, negated, lookup_name, namespace, target_field=None):
-
-        # We need access to the Datastore client to access the Key factory
-        wrapper = connections[self.using]
-        wrapper.ensure_connection()
-        gclient = wrapper.connection.gclient
-
-        assert column
-        assert operator
-        assert isinstance(is_pk_field, bool)
-        assert isinstance(negated, bool)
-
-        if operator == "iexact" and isinstance(target_field, AutoField):
-            # When new instance is created, automatic primary key 'id'
-            # does not generate '_idx_iexact_id'.
-            # As the primary key 'id' (AutoField) is integer and is always case insensitive,
-            # we can deal with 'id_iexact=' query by using 'exact' rather than 'iexact'.
-            operator = "exact"
-            value = int(value)
-
-        if is_pk_field:
-            # If this is a primary key, we need to make sure that the value
-            # we pass to the query is a datastore Key. We have to deal with IN queries here
-            # because they aren't flattened until the DNF stage
-            model = get_top_concrete_parent(target_field.model)
-            table = model._meta.db_table
+def field_conv_month_only(value):
+    value = ensure_datetime(value)
+    return datetime(value.year, value.month, 1, 0, 0)
 
-            if isinstance(value, (list, tuple)):
-                value = [gclient.key(table, x, namespace=namespace) for x in value if x]
-            else:
-                # Django 1.11 has operators as symbols, earlier versions use "exact" etc.
-                if (operator == "isnull" and value is True) or (
-                    operator in ("exact", "lt", "lte", "<", "<=", "=") and not value
-                ):
-                    # id=None will never return anything and
-                    # Empty strings and 0 are forbidden as keys
-                    self.will_never_return_results = True
-                elif operator in ("gt", "gte", ">", ">=") and not value:
-                    # If the value is 0 or "", then we need to manipulate the value and operator here to
-                    # get the right result (given that both are invalid keys) so for both we return
-                    # >= 1 or >= "\0" for strings
-                    if isinstance(value, int):
-                        value = 1
-                    else:
-                        value = "\0"
 
-                    value = gclient.key(table, value, namespace=namespace)
-                    operator = "gte"
-                else:
-                    value = gclient.key(table, value, namespace=namespace)
-            column = "__key__"
+def field_conv_day_only(value):
+    value = ensure_datetime(value)
+    return datetime(value.year, value.month, value.day, 0, 0)
 
-        # Do any special index conversions necessary to perform this lookup
-        special_indexer = get_indexer(target_field, operator)
 
-        if special_indexer:
-            if is_pk_field:
-                column = model._meta.pk.column
-                value = str(value.id_or_name)
-
-            add_special_index(connections[self.using], target_field.model, column, special_indexer, operator, value)
-            index_type = special_indexer.prepare_index_type(operator, value)
-            value = special_indexer.prep_value_for_query(
-                value, model=target_field.model, column=column, connection=connections[self.using]
-            )
-            column = special_indexer.indexed_column_name(column, value, index_type)
-            operator = special_indexer.prep_query_operator(operator)
+def coerce_unicode(value):
+    if isinstance(value, bytes):
+        try:
+            value = value.decode("utf-8")
+        except UnicodeDecodeError:
+            # This must be a Django databaseerror, because the exception happens too
+            # early before Django's exception wrapping can take effect (e.g. it happens on SQL
+            # construction, not on execution.
+            raise DatabaseError("Bytestring is not encoded in utf-8")
 
-        self.column = column
-        self.operator = convert_operator(operator)
-        self.value = value
-        self.lookup_name = lookup_name
-        self.is_iterable_field = target_field.db_type(wrapper) in ['list', 'set']
-
-    def __iter__(self):
-        for child in chain(*map(iter, self.children)):
-            yield child
-        yield self
+    # The SDK raises BadValueError for unicode sub-classes like SafeText.
+    return str(value)
 
-    def __repr__(self):
-        if self.is_leaf:
-            return "[%s%s%s]" % (self.column, self.operator, self.value)
-        else:
-            return "(%s:%s%s)" % (
-                self.connector,
-                "!" if self.negated else "",
-                ",".join([repr(x) for x in self.children]),
-            )
 
-    def __eq__(self, rhs):
-        if self.is_leaf != rhs.is_leaf:
-            return False
+def log_once(logging_call, text, args):
+    """
+        Only logs one instance of the combination of text and arguments to the passed
+        logging function
+    """
+    identifier = "%s:%s" % (text, args)
+    if identifier in log_once.logged:
+        return
+    logging_call(text % args)
+    log_once.logged.add(identifier)
 
-        if self.is_leaf:
-            return self.column == rhs.column and self.value == rhs.value and self.operator == rhs.operator
-        else:
-            return self.connector == rhs.connector and self.children == rhs.children
 
-    def __hash__(self):
-        if self.is_leaf:
-            value = frozenset(self.value) if isinstance(self.value, (set, list, tuple)) else self.value
-            return hash((self.column, value, self.operator))
-        else:
-            return hash((self.connector,) + tuple([hash(x) for x in self.children]))
+log_once.logged = set()
 
 
-class Query(object):
-    def __init__(self, model, kind):
-        assert kind in VALID_QUERY_KINDS
+def convert_django_ordering_to_gae(ordering):
+    return ordering
 
-        self.model = model
-        self.concrete_model = get_top_concrete_parent(model)
-        self.kind = kind
 
-        self.projection_possible = True
-        self.tables = []
+def limit_results_generator(results, limit):
+    for result in results:
+        yield result
+        limit -= 1
+        if not limit:
+            raise StopIteration
+
+
+class SelectCommand(object):
+    def __init__(self, wrapper, query, keys_only=False):
+        from gcloudc.db.backends.common.base.connection import Wrapper
+
+        assert (isinstance(wrapper, Wrapper))
+
+        self.wrapper = wrapper
+        self.connection = wrapper.connection
+        self.namespace = wrapper.namespace
+        self.results = iter([])
+        self.model = query.model
+        self.query = wrapper.transform_django_query(
+            query, keys_only
+        )
+
+        self.original_query = query
+        self.init_list = [x[0] for x in self.query.annotations] + list(self.query.select or [])
+
+    def _determine_query_kind(self):
+        """ Basically returns SELECT or COUNT """
+        query = self.original_query
+
+        if query.annotations:
+            if "__count" in query.annotations:
+                field = query.annotations["__count"].source_expressions[0]
+                if isinstance(field, Star) or field.value == "*":
+                    return "COUNT"
+
+        return "SELECT"
+
+    def __eq__(self, other):
+        return isinstance(other, self.__class__) and self.query == other.query
+
+    def __ne__(self, other):
+        return not self.__eq__(other)
 
-        self.columns = None  # None means all fields
-        self.init_list = []
+    def execute(self):
+        high_mark = self.original_query.high_mark
+        low_mark = self.original_query.low_mark
+        limit = None if high_mark is None else (high_mark - (low_mark or 0))
+        offset = low_mark or 0
 
-        self.distinct = False
-        self.order_by = []
-        self.row_data = []  # For insert/updates
-        self._where = None
-        self.low_mark = self.high_mark = None
+        query_type = self._determine_query_kind()
 
-        self.annotations = []
-        self.per_entity_annotations = []
-        self.extra_selects = []
-        self.polymodel_filter_added = False
+        if query_type == "COUNT":
+            self.results = iter([self.query.count(limit=limit)])
+            return 1
+        elif query_type == "AVERAGE":
+            raise ValueError("AVERAGE not yet supported")
 
-        # A list of PKs that should be excluded from the resultset
-        self.excluded_pks = set()
+        assert (query_type == "SELECT")
 
-    @property
-    def is_normalized(self):
+        results_returned = 0
+        results = []
+
+        for entity in self.query.fetch(limit=limit, offset=offset):
+            if entity:
+                results.append(entity)
+                results_returned += 1
+
+        self.results = iter(results)
+        return results_returned
+
+    def __repr__(self):
+        return force_str(generate_sql_representation(self))
+
+    def __mod__(self, params):
+        return repr(self)
+
+    def lower(self):
         """
-            Returns True if this query has a normalized where tree
+            This exists solely for django-debug-toolbar compatibility.
         """
-        if not self.where:
-            return True
+        return str(self).lower()
 
-        # Only a leaf node, return True
-        if not self.where.is_leaf:
-            return True
 
-        # If we have children, and they are all leaf nodes then this is a normalized
-        # query
-        return self.where.connector == "OR" and self.where.children and all(x.is_leaf for x in self.where.children)
-
-    def add_extra_select(self, column, lookup):
-        if lookup.lower().startswith("select "):
-            raise ValueError("SQL statements aren't supported with extra(select=)")
-
-        # Boolean expression test
-        bool_expr = r"(?P<lhs>[a-zA-Z0-9_]+)\s?(?P<op>[=|>|<]{1,2})\s?(?P<rhs>[\w+|']+)"
-
-        # Operator expression test
-        op_expr = r"(?P<lhs>[a-zA-Z0-9_]+)\s?(?P<op>[+|-|/|*])\s?(?P<rhs>[\w+|']+)"
-
-        OP_LOOKUP = {
-            "=": lambda x, y: x == y,
-            "is": lambda x, y: x == y,
-            "<": lambda x, y: x < y,
-            ">": lambda x, y: x > y,
-            ">=": lambda x, y: x >= y,
-            "<=": lambda x, y: x <= y,
-            "+": lambda x, y: x + y,
-            "-": lambda x, y: x - y,
-            "/": lambda x, y: x / y,
-            "*": lambda x, y: x * y,
-        }
-
-        for regex in (bool_expr, op_expr):
-            match = re.match(regex, lookup)
-            if match:
-                lhs = match.group("lhs")
-                rhs = match.group("rhs")
-                op = match.group("op").lower()
-                if op in OP_LOOKUP:
-                    self.extra_selects.append((column, (OP_LOOKUP[op], (lhs, rhs))))
-                else:
-                    raise ValueError("Unsupported operator")
+class FlushCommand(object):
+    """
+        sql_flush returns the SQL statements to flush the database,
+        which are then executed by cursor.execute()
+
+        We instead return a list of FlushCommands which are called by
+        our cursor.execute
+    """
+
+    def __init__(self, table, connection):
+        self.connection = connection
+        self.table = table
+        self.namespace = connection.namespace
+
+    def execute(self):
+        self.connection.ensure_connection()
+        self.connection.connection.flush([self.table], namespace=self.namespace)
+
+
+def perform_unique_checks(namespace, model, rpc, primary, test_fn):
+    def _test_combination(combination):
+        # We can't `break` two levels at once, hence the nested function
+        query = rpc.query(kind=primary.kind, namespace=namespace)
+
+        for field in combination:
+            col_name = model._meta.get_field(field).column
+            value = primary.get(col_name)
+            if isinstance(value, list):
+                if not value:
+                    # For lists, empty values are treated as effectively NULL
+                    return
+                for item in value:
+                    query.add_filter(col_name, '=', item)
+            elif value is None:
                 return
+            else:
+                query.add_filter(col_name, '=', value)
 
-        # Assume literal
-        self.extra_selects.append((column, (lambda x: x, [lookup])))
+        # only perform the query if there are filters on it
+        if len(query.filters):
+            res = list(query.fetch(1))
+            if test_fn(res):
+                raise IntegrityError(
+                    CONSTRAINT_VIOLATION_MSG.format(model._meta.db_table, ", ".join(combination))
+                )
 
-    def add_source_table(self, table):
-        if table in self.tables:
-            return
-
-        self.tables.append(table)
-
-    def set_distinct(self, distinct_fields):
-        self.distinct = True
-        if distinct_fields:
-            for field in distinct_fields:
-                self.add_projected_column(field)
-        elif not self.columns:
-            for field in self.model._meta.fields:
-                self.add_projected_column(field.column)
-
-    def add_order_by(self, column):
-        self.order_by.append(column)
-
-    def add_annotation(self, column, annotation):
-        # The Trunc annotation class doesn't exist in Django 1.8, hence we compare by
-        # strings, rather than importing the class to compare it
-        name = annotation.__class__.__name__
-        if name == "Count":
-            return  # Handled elsewhere
-
-        if name == "Value":
-            # This may break if we, in the future, decide we want to support Values in
-            # F expression. AFAICT, Value is only used (outside of F expressions) as a
-            # trick when performing "exists" queries, so it should be safe to ignore.
-            return
-
-        if name not in ("Trunc", "Col", "Date", "DateTime"):
-            raise NotSupportedError("Unsupported annotation %s" % name)
-
-        def process_date(value, lookup_type):
-            value = ensure_datetime(value)
-            ret = datetime.datetime.utcfromtimestamp(0)
-
-            POSSIBLE_LOOKUPS = ("year", "month", "day", "hour", "minute", "second")
-
-            ret = ret.replace(
-                value.year,
-                value.month if lookup_type in POSSIBLE_LOOKUPS[1:] else ret.month,
-                value.day if lookup_type in POSSIBLE_LOOKUPS[2:] else ret.day,
-                value.hour if lookup_type in POSSIBLE_LOOKUPS[3:] else ret.hour,
-                value.minute if lookup_type in POSSIBLE_LOOKUPS[4:] else ret.minute,
-                value.second if lookup_type in POSSIBLE_LOOKUPS[5:] else ret.second,
-            )
+    combinations = _unique_combinations(model, ignore_pk=True)
+    for combination in combinations:
+        _test_combination(combination)
 
-            return ret
 
-        # Abuse the extra_select functionality
-        if name == "Col":
-            self.extra_selects.append((column, (lambda x: x, [column])))
-        elif name in ("Trunc", "Date", "DateTime"):
-            # Trunc stores the source column and the lookup type differently to Date
-            # which is why we have the getattr craziness here
-            lookup_column = (
-                annotation.lhs.output_field.column if name == "Trunc" else getattr(annotation, "lookup", column)
-            )
+class BulkInsertError(IntegrityError, NotSupportedError):
+    pass
 
-            lookup_type = getattr(annotation, "lookup_type", getattr(annotation, "kind", None))
-            assert lookup_type
 
-            self.extra_selects.append((column, (lambda x: process_date(x, lookup_type), [lookup_column])))
-            # Override the projection so that we only get this column
-            self.columns = set([lookup_column])
-
-    def add_projected_column(self, column):
-        self.init_list.append(column)
-
-        if not self.projection_possible:
-            # If we previously tried to add a column that couldn't be
-            # projected, we don't try and add any more
-            return
-
-        field = get_field_from_column(self.model, column)
-
-        if field is None:
-            raise NotSupportedError(
-                "{} is not a valid column for the queried model. Did you try to join?".format(column)
-            )
+class BulkDeleteError(IntegrityError, NotSupportedError):
+    pass
 
-        if field.db_type(self.connection) in ("bytes", "text", "list", "set"):
-            logger.warn("Disabling projection query as %s is an unprojectable type", column)
-            self.columns = None
-            self.projection_possible = False
-            return
 
-        if not self.columns:
-            self.columns = set([column])
-        else:
-            self.columns.add(column)
+class InsertCommand(object):
+    def __init__(self, connection, model, objs, fields, raw):
+        self.has_pk = any(x.primary_key for x in fields)
+        self.model = model
+        self.objs = objs
+        self.connection = connection
+        self.namespace = connection.namespace
+        self.raw = raw
+        self.fields = fields
+
+        self.entities = []
+        self.included_keys = []
+
+        for obj in self.objs:
+            if self.has_pk:
+                # We must convert the PK value here, even though this normally happens in
+                # django_instance_to_entities otherwise
+                # custom PK fields don't work properly
+                value = self.model._meta.pk.get_db_prep_save(self.model._meta.pk.pre_save(obj, True), self.connection)
+                self.included_keys.append(get_document_key(self.connection, self.model, value) if value else None)
 
-    def add_row(self, data):
-        assert self.columns
-        assert len(data) == len(self.columns)
-
-        self.row_data.append(data)
-
-    def prepare(self):
-        if not self.init_list:
-            self.init_list = [x.column for x in self.model._meta.fields]
-
-        self._remove_impossible_branches()
-        self._remove_erroneous_isnull()
-        self._remove_negated_empty_in()
-        self._add_inheritence_filter()
-        self._populate_excluded_pks()
-        self._disable_projection_if_fields_used_in_equality_filter()
-        self._check_only_single_inequality_filter()
-
-    @property
-    def where(self):
-        return self._where
-
-    @where.setter
-    def where(self, where):
-        assert where is None or isinstance(where, WhereNode)
-
-        self._where = where
-
-    def _populate_excluded_pks(self):
-        if not self._where:
-            return
-
-        self.excluded_pks = set()
-
-        def walk(node, negated):
-            if node.connector == "OR":
-                # We can only process AND nodes, if we hit an OR we can't
-                # use the excluded PK optimization
-                return
+                if value == 0:
+                    raise IntegrityError("The datastore doesn't support 0 as a key value")
 
-            if node.negated:
-                negated = not negated
+                if not self.model._meta.pk.blank and self.included_keys[-1] is None:
+                    raise IntegrityError("You must specify a primary key value for {} instances".format(self.model))
+            else:
+                # We zip() self.entities and self.included_keys in execute(), so they should be the same length
+                self.included_keys.append(None)
 
-            for child in node.children[:]:
-                # As more than one inequality filter is not allowed on the datastore
-                # this leaf + count check is probably pointless, but at least if you
-                # do try to exclude two things it will blow up in the right place and not
-                # return incorrect results
-                if child.is_leaf and len(node.children) == 1:
-                    if negated and child.operator == "=" and child.column == "__key__":
-                        self.excluded_pks.add(child.value)
-                        node.children.remove(child)
-                    elif negated and child.operator == "IN" and child.column == "__key__":
-                        [self.excluded_pks.add(x) for x in child.value]
-                        node.children.remove(child)
-                else:
-                    walk(child, negated)
+            # We don't use the values returned, but this does make sure we're
+            # doing the same validation as Django. See issue #493 for an
+            # example of how not doing this can mess things up
+            for field in fields:
+                field.get_db_prep_save(
+                    getattr(obj, field.attname) if raw else field.pre_save(obj, True), connection=connection
+                )
+
+            primary, descendents = django_instance_to_entities(self.connection, self.fields, self.raw, obj)
 
-            node.children = [x for x in node.children if x.children or x.column]
+            # Append the entity, and any descendents to the list to insert
+            self.entities.append((primary, descendents))
 
-        walk(self._where, False)
+    def execute(self):
+        """
+        Returns the keys of all entities succesfully put into the database.
+
+        Under the hood this handles a few implementation specific details,
+        such as checking that any unique constraints defined on the entity
+        model are respected.
+        """
+        check_existence = self.has_pk and not has_concrete_parents(self.model)
 
-        if not self._where.children:
-            self._where = None
+        def perform_insert(entities):
+            results = []
+            for primary, descendents in entities:
+                if primary.key().is_partial():
+                    db_type = self.model._meta.pk.db_type(self.connection)
+                    primary.key().complete_key(
+                        self.connection.generate_id(
+                            int if db_type in ('key', 'int', 'long') else str
+                        )
+                    )
 
-    def _remove_negated_empty_in(self):
-        """
-            An empty exclude(id__in=[]) is pointless, but can cause trouble
-            during denormalization. We remove such nodes here.
-        """
-        if not self._where:
-            return
-
-        def walk(node, negated):
-            if node.negated:
-                negated = node.negated
-
-            for child in node.children[:]:
-                if negated and child.operator == "IN" and not child.value:
-                    node.children.remove(child)
-
-                walk(child, negated)
-
-            node.children = [x for x in node.children if x.children or x.column]
-
-        had_where = bool(self._where.children)
-        walk(self._where, False)
-
-        # Reset the where if that was the only filter
-        if had_where and not bool(self._where.children):
-            self._where = None
-
-    def _remove_erroneous_isnull(self):
-        # This is a little crazy, but bear with me...
-        # If you run a query like this:  filter(thing=1).exclude(field1="test") where field1 is
-        # null-able you'll end up with a negated branch in the where tree which is:
-
-        #           AND (negated)
-        #          /            \
-        #   field1="test"   field1__isnull=False
-
-        # This is because on SQL, field1 != "test" won't give back rows where field1 is null, so
-        # django has to include the negated isnull=False as well in order to get back the null rows
-        # as well.  On App Engine though None is just a value, not the lack of a value, so it's
-        # enough to just have the first branch in the negated node and in fact, if you try to use
-        # the above tree, it will result in looking for:
-        #  field1 < "test" and field1 > "test" and field1__isnull=True
-        # which returns the wrong result (it'll return when field1 == None only)
-
-        def walk(node, negated):
-            if node.negated:
-                negated = not negated
-
-            if not node.is_leaf:
-                equality_fields = set()
-                negated_isnull_fields = set()
-                isnull_lookup = {}
-
-                for child in node.children[:]:
-                    if negated:
-                        if child.lookup_name != "isnull":
-                            equality_fields.add(child.column)
-                            if child.column in negated_isnull_fields:
-                                node.children.remove(isnull_lookup[child.column])
-                        else:
-                            negated_isnull_fields.add(child.column)
-                            if child.column in equality_fields:
-                                node.children.remove(child)
-                            else:
-                                isnull_lookup[child.column] = child
-
-                    walk(child, negated)
-
-        if self.where:
-            walk(self._where, False)
-
-    def _remove_impossible_branches(self):
-        """
-            If we mark a child node as never returning results we either need to
-            remove those nodes, or remove the branches of the tree they are on depending
-            on the connector of the parent node.
-        """
-        if not self._where:
-            return
-
-        def walk(node, negated):
-            if node.negated:
-                negated = not negated
-
-            for child in node.children[:]:
-                walk(child, negated)
-
-                if child.will_never_return_results:
-                    if node.connector == "AND":
-                        if child.negated:
-                            node.children.remove(child)
-                        else:
-                            node.will_never_return_results = True
-                    else:
-                        # OR
-                        if not child.negated:
-                            node.children.remove(child)
-                            if not node.children:
-                                node.will_never_return_results = True
-                        else:
-                            node.children[:] = []
-
-        walk(self._where, False)
-
-        if self._where.will_never_return_results:
-            # We removed all the children of the root where node, so no results
-            raise EmptyResultSet()
-
-    def _check_only_single_inequality_filter(self):
-        inequality_fields = set()
-
-        def walk(node, negated):
-            if node.negated:
-                negated = not negated
-
-            for child in node.children[:]:
-                if (negated and child.operator == "=") or child.operator in (">", "<", ">=", "<="):
-                    inequality_fields.add(child.column)
-                walk(child, negated)
-
-            if len(inequality_fields) > 1:
-                raise NotSupportedError(
-                    "You can only have one inequality filter per query on the rpc. "
-                    "Filters were: %s" % " ".join(inequality_fields)
+                self.connection.pre_entity_insert(
+                    self.model, primary, {}
                 )
 
-        if self.where:
-            walk(self._where, False)
+                self.connection.connection.put(primary)
 
-    def _disable_projection_if_fields_used_in_equality_filter(self):
-        if not self._where or not self.columns:
-            return
+                self.connection.post_entity_insert(
+                    self.model, primary, {}
+                )
 
-        equality_columns = set()
+                new_key = primary.key()
 
-        def walk(node):
-            if not node.is_leaf:
-                for child in node.children:
-                    walk(child)
-            elif node.operator == "=" or node.operator == "IN":
-                equality_columns.add(node.column)
+                for descendent in descendents or []:
+                    ancestor_key = self.connection.connection.new_key(
+                        descendent.key().path[0],
+                        descendent.key().id_or_name,
+                        parent=new_key,
+                    )
+                    descendent.set_key(ancestor_key)
+                    self.connection.connection.put(descendent)
+
+                results.append(new_key)
+            return results
+
+        @atomic(using=self.connection.alias)
+        def insert_chunk(keys, entities):
+            for key in keys:
+                # sanity check the key isn't already taken
+                if check_existence and key is not None:
+                    if self.connection.connection.exists(key):
+                        raise IntegrityError("Tried to INSERT with existing key")
+
+                    if key.id_or_name is not None:
+                        # quick validation of the ID value
+                        if not self.connection.is_id_valid(key.id_or_name):
+                            raise NotSupportedError(
+                                "Key value ({}) is not valid.".format(key.id_or_name)
+                            )
+
+                        # Reserve any explicit id
+                        # FIXME: This only uses part of the path and won't work
+                        # for nested collisions
+                        assert (len(key.path) == 1)
+                        self.connection.reserve_id(
+                            key.path[0], key.id_or_name, self.namespace
+                        )
+
+            results = perform_insert(entities)
+            return results
+
+        tries = 1 if self.connection.in_atomic_block else _TRANSACTION_TRIES
+        for i in range(tries):
+            try:
+                return insert_chunk(self.included_keys, self.entities)
+            except OperationalError:
+                if i == tries - 1:
+                    raise
+                continue
 
-        walk(self._where)
+    def lower(self):
+        """
+            This exists solely for django-debug-toolbar compatibility.
+        """
+        return str(self).lower()
 
-        if equality_columns and equality_columns.intersection(self.columns):
-            self.columns = None
-            self.projection_possible = False
+    def __str__(self):
+        return generate_sql_representation(self)
 
-    def _add_inheritence_filter(self):
-        """
-            We support inheritence with polymodels. Whenever we set
-            the 'where' on this query, we manipulate the tree so that
-            the lookups are ANDed with a filter on 'class = db_table'
-            and on inserts, we add the 'class' column if the model is part
-            of an inheritance tree.
 
-            We only do any of this if the model has concrete parents and isn't
-            a proxy model
+class DeleteCommand(object):
+    """
+    Delete an entity / multiple entities.
+
+    Limits imposed by the Firestore in Datastore mode (such as 500 write operations
+    per batch) and the backend internal implementation details are handled under the hood.
+    """
+
+    def __init__(self, connection, query):
+        self.connection = connection
+        self.model = query.model
+        self.namespace = connection.namespace
+
+        self.select = SelectCommand(connection, query, keys_only=True)
+        self.query = self.select.query  # we only need this for the generate_sql_formatter caller...
+
+        if query.model:
+            table = helpers.get_top_concrete_parent(query.model)._meta.db_table
+        else:
+            table = query.tables[0]
+            assert (table)
+
+        self.table_to_delete = table  # used in wipe_polymodel_from_entity
+
+    def execute(self):
         """
-        if has_concrete_parents(self.model) and not self.model._meta.proxy:
-            if self.polymodel_filter_added:
-                return
+            Ideally we'd just be able to tell appengine to delete all the entities
+            which match the query, that would be nice wouldn't it?
+
+            Except we can't. Firstly delete() only accepts keys so we first have to
+            execute a keys_only query to find the entities that match the query, then send
+            those keys to delete().
+
+            And then there are polymodels (model inheritence) which means we might not even be
+            deleting the entity after all, only deleting some of the fields from it.
 
-            new_filter = WhereNode(self.connection.alias)
-            new_filter.column = POLYMODEL_CLASS_ATTRIBUTE
-            new_filter.operator = "="
-            new_filter.value = self.model._meta.db_table
-
-            # We add this bare AND just to stay consistent with what Django does
-            new_and = WhereNode(self.connection.alias)
-            new_and.connector = "AND"
-            new_and.children = [new_filter]
-
-            new_root = WhereNode(self.connection.alias)
-            new_root.connector = "AND"
-            new_root.children = [new_and]
-            if self._where:
-                # Add the original where if there was one
-                new_root.children.append(self._where)
-            self._where = new_root
-
-            self.polymodel_filter_added = True
-
-    def serialize(self):
-        """
-            The idea behind this function is to provide a way to serialize this
-            query to a string which can be compared to another query. Pickle won't
-            work as some of the values etc. might not be picklable.
-
-            FIXME: This function is incomplete! Not all necessary members are serialized
-        """
-        if not self.is_normalized:
-            raise ValueError("You cannot serialize queries unless they are normalized")
-
-        result = {}
-        result["kind"] = self.kind
-        result["table"] = self.model._meta.db_table
-        result["concrete_table"] = self.concrete_model._meta.db_table
-        result["columns"] = list(self.columns or [])  # set() is not JSONifiable
-        result["projection_possible"] = self.projection_possible
-        result["init_list"] = self.init_list
-        result["distinct"] = self.distinct
-        result["order_by"] = self.order_by
-        result["low_mark"] = self.low_mark
-        result["high_mark"] = self.high_mark
-        result["excluded_pks"] = list(map(str, self.excluded_pks))
-
-        where = []
-
-        if self.where:
-            assert self.where.connector == "OR"
-            for node in self.where.children:
-                assert node.connector == "AND"
+            What we do then is do a keys_only query, then iterate the entities in batches of
+            500, each entity in the batch has its polymodel fields wiped out
+            (if necessary) and then we do either a put() or delete() all inside a transaction.
 
-                query = {}
+            Oh, and we wipe out memcache in an independent transaction.
+
+            Things to improve:
+
+            - Check the entity matches the query still (there's a fixme there)
+        """
+        from gcloudc.db.backends.common.indexing import indexers_for_model
+
+        @atomic(using=self.connection.alias)
+        def delete_batch(key_slice):
+            """
+                Batch fetch entities, wiping out any polymodel fields if
+                necessary, before deleting the entities by key.
+
+                Any memcache references are also removed.
+            """
+            entities_to_delete = []
+            entities_to_update = []
+            updated_keys = []
+
+            # get() expects Key objects, not just dicts with id keys
+            keys_in_slice = [
+                self.connection.connection.new_key(
+                    self.model._meta.db_table,
+                    key_id,
+                    namespace=self.connection.namespace
+                )
+                for key_id in key_slice
+            ]
+            entities = self.connection.connection.get(keys_in_slice)
+            for entity in entities:
+
+                # make sure the entity still exists
+                if entity is None:
+                    continue
 
-                if node.children:
-                    for lookup in node.children:
+                # handle polymodels
+                _wipe_polymodel_from_entity(entity, self.table_to_delete)
 
-                        query["".join([lookup.column, lookup.operator])] = _serialize_sql_value(lookup.value)
+                if not entity.get("class"):
+                    entities_to_delete.append(entity)
                 else:
-                    query["".join([node.column, node.operator])] = _serialize_sql_value(node.value)
+                    entities_to_update.append(entity)
+                updated_keys.append(entity)
 
-                where.append(query)
+            # we don't need an explicit batch here, as we are inside a transaction
+            # which already applies this behaviour of non blocking RPCs until
+            # the transaction is commited
 
-        result["where"] = where
+            client = self.connection.connection
 
-        return json.dumps(result)
+            for entity in entities:
+                self.connection.pre_entity_delete(self.model, entity, {})
 
+            for entity in entities_to_delete:
+                client.delete(entity.key())
 
-INVALID_ORDERING_FIELD_MESSAGE = (
-    "Ordering on TextField or BinaryField is not supported on the rpc. "
-    "You might consider using a ComputedCharField which stores the first "
-    "_MAX_STRING_LENGTH (from google.appengine.api.datastore_types) bytes of the "
-    "field and instead order on that."
-)
+            for entity in entities_to_update:
+                client.put(entity)
+
+            for entity in entities:
+                self.connection.post_entity_delete(self.model, entity, {})
+
+            # Clean up any special indexes that need to be removed
+            for indexer in indexers_for_model(self.model):
+                for entity in entities_to_delete:
+                    indexer.cleanup(client, entity.key())
 
+            return len(updated_keys)
 
-def _serialize_sql_value(value):
-    if isinstance(value, int):
-        return value
-    else:
-        return str("NULL" if value is None else value)
+        # grab the result of the keys only query (see __init__)
+        self.select.execute()
+        key_ids = [x.key().id_or_name for x in self.select.results]
 
+        # for now we can only process 500 entities
+        # otherwise we need to handle rollback of independent transactions
+        # and race conditions between items being deleted and restored...
+        max_batch_size = self.connection.TRANSACTION_ENTITY_LIMIT
 
-def _get_parser(query, connection=None):
-    from gcloudc.db.backends.datastore.parsers import base
+        if len(key_ids) > max_batch_size:
+            raise BulkDeleteError(
+                "Bulk deletes for {} can only delete {} instances per batch".format(self.model, max_batch_size)
+            )
 
-    return base.BaseParser(query, connection)
+        tries = 1 if self.connection.in_atomic_block else _TRANSACTION_TRIES
+        for i in range(tries):
+            try:
+                return delete_batch(key_ids)
+            except OperationalError:
+                if i == tries - 1:
+                    raise
+                continue
 
+    def lower(self):
+        """
+            This exists solely for django-debug-toolbar compatibility.
+        """
+        return str(self).lower()
 
-def transform_query(connection, query):
-    return _get_parser(query, connection).get_transformed_query()
+    def __str__(self):
+        return generate_sql_representation(self)
+
+
+def _wipe_polymodel_from_entity(entity, db_table):
+    """
+        Wipes out the fields associated with the specified polymodel table.
+    """
+    polymodel_value = entity.get("class", [])
+    if polymodel_value and db_table in polymodel_value:
+        # Remove any local fields from this model from the entity
+        model = get_model_from_db_table(db_table)
+        for field in model._meta.local_fields:
+            col = field.column
+            if col in entity:
+                del entity[col]
+
+        # Then remove this model from the polymodel heirarchy
+        polymodel_value.remove(db_table)
+        if polymodel_value:
+            entity["class"] = polymodel_value
+
+
+class UpdateCommand(object):
+    def __init__(self, connection, query):
+        self.model = query.model
+        self.select = SelectCommand(connection, query, keys_only=False)
+        self.query = self.select.query
+        self.values = query.values
+        self.connection = connection
+        self.namespace = connection.namespace
+        self.results = []
+
+    def __str__(self):
+        return generate_sql_representation(self)
+
+    def lower(self):
+        """
+            This exists solely for django-debug-toolbar compatibility.
+        """
+        return str(self).lower()
+
+    def _update_entity(self, result):
+        def update_txt():
+            if result is None:
+                # Return false to indicate update failure
+                return False
+
+            original = copy.deepcopy(result)
+
+            instance_kwargs = {field.attname: value for field, param, value in self.values}
+
+            # Note: If you replace MockInstance with self.model, you'll find that some delete
+            # tests fail in the test app. This is because any unspecified fields would then call
+            # get_default (even though we aren't going to use them) which may run a query which
+            # fails inside this transaction. Given as we are just using MockInstance so that we can
+            # call django_instance_to_entities it on it with the subset of fields we pass in,
+            # what we have is fine.
+            meta = self.model._meta
+            instance = MockInstance(_original=MockInstance(_meta=meta, **result), _meta=meta, **instance_kwargs)
+
+            # Convert the instance to an entity
+            primary, descendents = django_instance_to_entities(
+                self.connection,
+                [x[0] for x in self.values],  # Pass in the fields that were updated
+                True,
+                instance,
+                model=self.model,
+            )
+            # Update the entity we read above with the new values
+            result.update(primary)
+
+            # Remove fields which have been marked to be unindexed
+            for col in getattr(primary, "_properties_to_remove", []):
+                if col in result:
+                    del result[col]
+
+            # Make sure that any polymodel classes which were in the original entity are kept,
+            # as django_instance_to_entities may have wiped them as well as added them.
+            polymodel_classes = list(
+                set(
+                    original.get(self.connection.polymodel_property_name(), []) +
+                    result.get(self.connection.polymodel_property_name(), [])
+                )
+            )
+            if polymodel_classes:
+                result[self.connection.polymodel_property_name()] = polymodel_classes
+
+            def perform_insert():
+                """
+                    Inserts result, and any descendents with their ancestor
+                    value set
+                """
+
+                self.connection.pre_entity_update(self.model, result, {})
+                self.connection.connection.put(result)
+                self.connection.post_entity_update(self.model, result, {})
+
+                inserted_key = result.key()
+                self.results.append((result, None))
+
+                if descendents:
+                    for descendent in descendents:
+                        final_descendent = Entity(
+                            self.connection.connection.new_key(
+                                descendent.key().path[0],
+                                descendent.key().id_or_name,
+                                parent=inserted_key,
+                                namespace=inserted_key.namespace
+                            )
+                        )
+                        final_descendent.update(descendent)
+                        self.connection.connection.put(final_descendent)
+
+            # this will be async as we're inside a transaction block
+            perform_insert()
+
+            # Return true to indicate update success
+            return True
 
+        return update_txt()
 
-def extract_ordering(query):
-    return _get_parser(query).get_extracted_ordering()
+    def execute(self):
+        @atomic(using=self.connection.alias)
+        def perform_update():
+            self.select.execute()
+            results = list(self.select.results)
+
+            i = 0
+            for result in results:
+                if self._update_entity(result):
+                    i += 1
+
+            return i
+
+        # TODO: potential optimisation - consider running transactions
+        # around single entity update rather than the whole batch.
+        # This could potentially open a can of worms but would have the
+        # benefit of locking fewer rows.
+        tries = 1 if self.connection.in_atomic_block else _TRANSACTION_TRIES
+        for i in range(tries):
+            try:
+                return perform_update()
+            except OperationalError:
+                if i == tries - 1:
+                    raise
+                continue
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/schema.py` & `django-gcloud-connectors-1.2.0/gcloudc/db/backends/datastore/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # STANDARD LIBRARY
 import logging
 
 # 3RD PARTY
 from django.db.backends.base.schema import BaseDatabaseSchemaEditor
 
 # DJANGAE
-from gcloudc.db.backends.datastore.dbapi import CouldBeSupportedError
+from gcloudc.db.backends.common.base.dbapi import CouldBeSupportedError
 
 logger = logging.getLogger("djangae")
 
 
 class DatabaseSchemaEditor(BaseDatabaseSchemaEditor):
     """
     Work in progress!
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/unique_mixins.py` & `django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/mixins.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.core.exceptions import NON_FIELD_ERRORS
 
-from .dbapi import NotSupportedError
+from gcloudc.db.backends.common.base.dbapi import NotSupportedError
 
 
 MAX_ALLOWABLE_QUERIES = 30
 
 
 class UniquenessMixin(object):
     """
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/unique_utils.py` & `django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/constraints.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,37 @@
+"""
+The Datastore does not provide database level constraints around uniqueness
+(unlike relational a SQL database, where you can ensure uniqueness for a certain
+column, or a combination of columns).
+
+To mimic the ability to define these constraints using the Django API,
+we have implemented an approach where, thanks to Cloud Firestore strong
+consistency we check unique constraints transactionally before any write
+
+This allows us to efficiently check for existing constraints before doing a put().
+"""
+
 from hashlib import md5
 
+from django.db import NotSupportedError
+from django.db.utils import IntegrityError
+from .helpers import get_top_concrete_parent, get_bottom_concrete_model
 
-def _has_enabled_constraints(model_or_instance):
-    """
-    Since we're no longer doing any extra write to enforce uniqueness there's
-    not much point in not enforcing it, so we always keep it enabled
-    """
-    return True
 
+UNIQUE_MARKER_KIND = "uniquemarker"
+CONSTRAINT_VIOLATION_MSG = "Unique constraint violation for kind {} on fields: {}"
 
-def _has_unique_constraints(model_or_instance):
+
+def _format_value_for_identifier(value):
+    # AppEngine max key length is 500 chars, so if the value is a string we hexdigest it to reduce the length
+    # otherwise we str() it as it's probably an int or bool or something.
+    return md5(value.encode("utf-8")).hexdigest() if isinstance(value, str) else str(value)
+
+
+def has_unique_constraints(model_or_instance):
     """
     Returns a boolean to indicate if the given model has any type of unique
     constraint defined (e.g. unique on a single field, or meta.unique_together).
 
     To support concrete model inheritance we state that uniqueness checks
     should only be performed on the class that the defines the unique constraint.
 
@@ -30,54 +48,82 @@
         field.unique and field.model == model_class
         for field in meta_options.fields
     )
 
     return any([unique_fields, unique_together])
 
 
-def query_is_unique(model, query):
-    """
-        If the query is entirely on unique constraints then return the unique identifier for
-        that unique combination. Otherwise return False
+def check_unique_markers_in_memory(wrapper, entities):
     """
+    Compare the entities using their in memory properties, to see if any
+    unique constraints are violated.
 
-    from . import meta_queries  # Circular import workaround
+    This would always need to be used in conjunction with RPC checks against
+    persisted markers to ensure data integrity.
+    """
 
-    if isinstance(query, meta_queries.AsyncMultiQuery):
-        # By definition, a multiquery is not unique
-        return False
+    polymodel_field = wrapper.polymodel_property_name()
 
-    combinations = _unique_combinations(model)
+    all_unique_marker_key_values = set([])
+    for entity in entities:
+        tables = [entity.key().path[-1]] + entity.get(polymodel_field, [])
+        model = get_bottom_concrete_model(tables)
+        if not model:
+            # Not all entities have a model
+            continue
 
-    query_by_keys = {"{} {}".format(x[0], x[1]): x[2] for x in query.filters}
-    for combination in combinations:
-        unique_match = True
-        field_names = []
-        for field in combination:
-            if field == model._meta.pk.column:
-                field = "__key__"
+        unique_marker_key_values = unique_identifiers_from_entity(model, entity, ignore_pk=True)
+        for named_key in unique_marker_key_values:
+            if named_key not in all_unique_marker_key_values:
+                all_unique_marker_key_values.add(named_key)
             else:
-                field = model._meta.get_field(field).column
-            field_names.append(field)
+                table_name = named_key.split("|")[0]
+                unique_fields = named_key.split("|")[1:]
+                raise IntegrityError(CONSTRAINT_VIOLATION_MSG.format(table_name, unique_fields))
 
-            # We don't match this combination if the field didn't exist in the queried fields
-            # or if it was, but the value was None (you can have multiple NULL values, they aren't unique)
-            matching_filters = list(filter(lambda x: x[0] == field and x[1] == '=', query.filters))
-            if len(matching_filters) != 1 or matching_filters[0][2] is None:
-                unique_match = False
-                break
 
-        if unique_match:
-            return "|".join(
-                [model._meta.db_table]
-                + ["{}:{}".format(x, _format_value_for_identifier(
-                    query_by_keys["{} =".format(x)])) for x in field_names]
-            )
+def _unique_combinations(model, ignore_pk=False):
+    """
+    Returns an iterable of iterables to represent all the unique constraints
+    defined on the model. For example given the following model definition:
+
+        class ExampleModel(models.Model):
+            username = models.CharField(unique=True)
+            email = models.EmailField(primary_key=True)
+            first_name = models.CharField()
+            second_name = models.CharField()
+
+        class Meta:
+            unique_together = ('first_name', 'second_name')
+
+    This method would return
+
+    [
+        ['username'], # from field level unique=True
+        ['email'], # implicit unique constraint from primary_key=True
+        ['first_name', 'second_name'] # from model meta unique_together
+    ]
+
+    Fields with unique constraint defined in a concrete parent model are ingored
+    since they're checked when that model is saved
+    """
+    # first grab all the unique together constraints
+    unique_constraints = [list(together_constraint) for together_constraint in model._meta.unique_together]
+
+    # then the column level constraints - special casing PK if required
+    for field in model._meta.fields:
+        if field.primary_key and ignore_pk:
+            continue
+
+        if field.unique and field.model == model:
+            unique_constraints.append([field.name])
 
-    return False
+    # the caller should sort each inner iterable really - but we do this here
+    # for now - motive being that interpolated keys from these values are consistent
+    return [sorted(constraint) for constraint in unique_constraints]
 
 
 def unique_identifiers_from_entity(model, entity, ignore_pk=True, ignore_null_values=True):
     """
     This method returns a list of all unique marker key identifier values for
     the given entity by combining the field and entity values. For example:
 
@@ -88,15 +134,18 @@
         djange_<model_db_table>|<field_name>:<entity_value>|<field_name>:<entity_value>
         ...
     ]
 
     These are then used before we put() anything into the database, to check
     that there are no existing markers satisfying those unique constraints.
     """
-    from .utils import get_top_concrete_parent
+
+    assert (entity is not None)
+
+    field_data = entity._data if hasattr(entity, "_data") else entity
 
     # get all combintatons of unique combinations defined on the model class
     unique_combinations = _unique_combinations(model, ignore_pk)
 
     meta = model._meta
 
     identifiers = []
@@ -105,17 +154,17 @@
 
         include_combination = True
 
         for field_name in combination:
             field = meta.get_field(field_name)
 
             if field.primary_key:
-                value = entity.key.id_or_name
+                value = entity.key().id_or_name
             else:
-                value = entity.get(field.column)  # Get the value from the entity
+                value = field_data.get(field.column)  # Get the value from the entity
 
             # If ignore_null_values is True, then we don't include combinations where the value is None
             # or if the field is a multivalue field where None means no value (you can't store None in a list)
             if (value is None and ignore_null_values) or (not value and isinstance(value, (list, set))):
                 include_combination = False
                 break
 
@@ -138,52 +187,56 @@
                 constraint_suffix = "|".join(identifier_pairs)
                 constraint_value = "{prefix}|{suffix}".format(prefix=constraint_prefix, suffix=constraint_suffix)
                 identifiers.append(constraint_value)
 
     return identifiers
 
 
-def _unique_combinations(model, ignore_pk=False):
+def perform_unique_checks(connection, model, primary, test_fn):
     """
-    Returns an iterable of iterables to represent all the unique constraints
-    defined on the model. For example given the following model definition:
-
-        class ExampleModel(models.Model):
-            username = models.CharField(unique=True)
-            email = models.EmailField(primary_key=True)
-            first_name = models.CharField()
-            second_name = models.CharField()
-
-        class Meta:
-            unique_together = ('first_name', 'second_name')
-
-    This method would return
-
-    [
-        ['username'], # from field level unique=True
-        ['email'], # implicit unique constraint from primary_key=True
-        ['first_name', 'second_name'] # from model meta unique_together
-    ]
-
-    Fields with unique constraint defined in a concrete parent model are ingored
-    since they're checked when that model is saved
+        fetch_fn: Given a combination (and the default_fetch_fn), returns the result that's passed to test_fn
+        test_fn: Takes a query result and returns true if it will cause a constraint issue
     """
-    # first grab all the unique together constraints
-    unique_constraints = [list(together_constraint) for together_constraint in model._meta.unique_together]
+    def fetch(combination, **kwargs):
+        query = connection.get_query_class()(
+            connection,
+            [primary.key().path[-1]],
+            namespace=connection.namespace,
+        )
 
-    # then the column level constraints - special casing PK if required
-    for field in model._meta.fields:
-        if field.primary_key and ignore_pk:
-            continue
-
-        if field.unique and field.model == model:
-            unique_constraints.append([field.name])
-
-    # the caller should sort each inner iterable really - but we do this here
-    # for now - motive being that interpolated keys from these values are consistent
-    return [sorted(constraint) for constraint in unique_constraints]
+        filtered = False
+        for field in combination:
+            field = model._meta.get_field(field)
+            col_name = field.column
+            value = primary.get(col_name)
+            if value is None:
+                return
+            if field.db_type(connection) in ('list', 'set'):
+                if len(value) == 0:
+                    return
+                if isinstance(value, (list, set, tuple)) and value:
+                    query.add_filter(col_name, 'array_contains_all', value)
+                else:
+                    query.add_filter(col_name, 'array_contains', value)
+                filtered = True
+            elif value is None:
+                return
+            else:
+                query.add_filter(col_name, '=', value)
+                filtered = True
 
+        # only perform the query if there are filters on it
+        if filtered:
+            try:
+                return list(query.fetch(offset=0, limit=1))
+            except NotSupportedError:
+                # This query with `limit=1` isn't supported in Firestore,
+                # retry removing the limit.
+                return list(query.fetch(offset=0, limit=None))
 
-def _format_value_for_identifier(value):
-    # AppEngine max key length is 500 chars, so if the value is a string we hexdigest it to reduce the length
-    # otherwise we str() it as it's probably an int or bool or something.
-    return md5(value.encode("utf-8")).hexdigest() if isinstance(value, str) else str(value)
+    combinations = _unique_combinations(model, ignore_pk=True)
+    for combination in combinations:
+        res = fetch(combination)
+        if res and test_fn(res):
+            raise IntegrityError(
+                CONSTRAINT_VIOLATION_MSG.format(model._meta.db_table, ", ".join(combination))
+            )
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/db/backends/datastore/utils.py` & `django-gcloud-connectors-1.2.0/gcloudc/db/backends/common/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from datetime import datetime
 from decimal import Decimal
-from itertools import chain
+from functools import lru_cache
+from logging import Logger
 from typing import (
     Set,
     Tuple,
 )
 
 from django.apps import apps
 from django.conf import settings
 from django.db import IntegrityError
 from django.db.backends.utils import format_number
 from django.utils import timezone
-from google.cloud.datastore.entity import Entity
-from google.cloud.datastore.key import Key
+from gcloudc.db.backends.common.base.entity import Entity
 
 from gcloudc.utils import memoized
 
 try:
     from django.db.models.expressions import BaseExpression
 except ImportError:
     from django.db.models.expressions import ExpressionNode as BaseExpression
@@ -91,15 +91,15 @@
     return get_top_concrete_parent(model)._meta.db_table
 
 
 def get_prepared_db_value(connection, instance, field, raw=False):
     value = getattr(instance, field.attname) if raw else field.pre_save(instance, instance._state.adding)
 
     if isinstance(value, BaseExpression):
-        from gcloudc.db.backends.datastore.expressions import (
+        from gcloudc.db.backends.common.parsers.expressions import (
             evaluate_expression,
         )
 
         # We can't actually support F expressions on the datastore, but we can simulate
         # them, evaluating the expression in place.
         # TODO: For saves and updates we should raise a Warning. When evaluated in a filter
         # we should raise an Error
@@ -123,14 +123,34 @@
 
 
 @memoized
 def get_top_concrete_parent(model):
     return get_concrete_parents(model)[-1]
 
 
+def get_bottom_concrete_model(tables):
+    """
+        Given a list of db_tables from a heirarchy of concrete models
+        this works out which one is the "bottom" model
+    """
+
+    lowest = None
+    highest_parent_count = 0
+
+    for table in tables:
+        model = get_model_from_db_table(table)
+        if model:
+            parents = get_concrete_parents(model)
+            if len(parents) >= highest_parent_count:
+                lowest = model
+                highest_parent_count = len(parents)
+
+    return lowest
+
+
 def get_concrete_fields(model, ignore_leaf=False):
     """
         Returns all the concrete fields for the model, including those
         from parent models
     """
     concrete_classes = get_concrete_parents(model, ignore_leaf)
     fields = []
@@ -212,16 +232,15 @@
             entity, [entity, entity, ...]
 
        Where the first result in the tuple is the primary entity, and the
        remaining entities are optionally descendents of the primary entity. This
        is useful for special indexes (e.g. contains)
     """
 
-    from gcloudc.db.backends.datastore import POLYMODEL_CLASS_ATTRIBUTE
-    from gcloudc.db.backends.datastore.indexing import (
+    from gcloudc.db.backends.common.indexing import (
         IgnoreForIndexing,
         get_indexer,
         special_indexes_for_column,
     )
 
     model = model or type(instance)
     inheritance_root = get_top_concrete_parent(model)
@@ -279,15 +298,15 @@
 
             # If the indexer returns additional entities (instead of indexing a special column)
             # then just store those entities
             if indexer.PREP_VALUE_RETURNS_ENTITIES:
                 descendents.extend(values)
             else:
                 for i, v in enumerate(values):
-                    column = indexer.indexed_column_name(field.column, v, index)
+                    column = indexer.indexed_column_name(field.column, v, index, connection=connection)
 
                     if unindex:
                         fields_to_unindex.add(column)
                         continue
 
                     # If the column already exists in the values, then we convert it to a
                     # list and append the new value
@@ -296,41 +315,40 @@
                             field_values[column] = [field_values[column], v]
                         else:
                             field_values[column].append(v)
                     else:
                         # Otherwise we just set the column to the value
                         field_values[column] = v
 
-    args = [db_table]
-    if primary_key is not None:
-        args.append(primary_key)
+    key = connection.connection.new_key(
+        db_table, primary_key,
+        namespace=connection.namespace
+    )
 
-    key = Key(*args, namespace=connection.namespace, project=connection.gcloud_project)
+    assert (key)
 
     exclude_from_indexes = model_fields_to_exclude_from_indexes(connection, model)
 
-    entity = Entity(key, exclude_from_indexes)
-    entity.update(field_values)
+    entity = Entity(key, field_values, exclude_from_indexes=exclude_from_indexes)
 
-    if fields_to_unindex:
-        entity._properties_to_remove = fields_to_unindex
+    for field in fields_to_unindex or []:
+        entity.add_property_to_unindex(field)
 
     classes = get_concrete_db_tables(model)
     if len(classes) > 1:
-        entity[POLYMODEL_CLASS_ATTRIBUTE] = list(set(classes))
+        entity[connection.polymodel_property_name()] = list(set(classes))
 
     return entity, descendents
 
 
-def get_datastore_key(connection, model, pk):
+def get_document_key(connection, model, pk):
     """ Return a datastore.Key for the given model and primary key.
     """
-    factory = connection.connection.gclient.key
     kind = get_top_concrete_parent(model)._meta.db_table
-    return factory(kind, pk, namespace=connection.namespace)
+    return connection.connection.new_key(kind, pk, namespace=connection.namespace)
 
 
 class MockInstance(object):
     """
         This creates a mock instance for use when passing a datastore entity
         into get_prepared_db_value. This is used when performing updates to prevent a complete
         conversion to a Django instance before writing back the entity
@@ -352,151 +370,91 @@
 
     def __getattr__(self, attr):
         if attr in self.fields:
             return self.fields[attr]
         raise AttributeError(attr)
 
 
-def key_exists(connection, key):
-    from . import transaction
-    qry = transaction._rpc(connection).query(namespace=key.namespace, ancestor=key)
-    qry.keys_only()
-    qry.add_filter("__key__", "=", key)
-    return count_query(qry) > 0
-
-
 # Null-friendly comparison functions
 
 
 def lt(x, y):
     if x is None and y is None:
         return False
     if x is None and y is not None:
         return True
     elif x is not None and y is None:
         return False
-    elif isinstance(x, Key) and isinstance(y, Key):
-        lhs = tuple([x.namespace] + list(x.flat_path))
-        rhs = tuple([y.namespace] + list(y.flat_path))
-        return lhs < rhs
     else:
         return x < y
 
 
 def gt(x, y):
     if x is None and y is None:
         return False
     if x is None and y is not None:
         return False
     elif x is not None and y is None:
         return True
-    elif isinstance(x, Key) and isinstance(y, Key):
-        lhs = tuple([x.namespace] + list(x.flat_path))
-        rhs = tuple([y.namespace] + list(y.flat_path))
-        return lhs > rhs
     else:
         return x > y
 
 
 def gte(x, y):
     return not lt(x, y)
 
 
 def lte(x, y):
     return not gt(x, y)
 
 
-def django_ordering_comparison(ordering, lhs, rhs):
-    if not ordering:
-        return -1  # Really doesn't matter
-
-    ASCENDING = 1
-    DESCENDING = 2
-
-    for order in ordering:
-        direction = DESCENDING if order.startswith("-") else ASCENDING
-        order = order.lstrip("-")
-
-        if lhs is not None:
-            lhs_value = lhs.key if order == "__key__" else lhs.get(order)
-        else:
-            lhs_value = None
-
-        if rhs is not None:
-            rhs_value = rhs.key if order == "__key__" else rhs.get(order)
-        else:
-            rhs_value = None
-
-        if direction == ASCENDING and lhs_value != rhs_value:
-            return -1 if lt(lhs_value, rhs_value) else 1
-        elif direction == DESCENDING and lhs_value != rhs_value:
-            return 1 if lt(lhs_value, rhs_value) else -1
-
-    return 0
-
-
 def entity_matches_query(entity, query):
     """
         Return True if the entity would potentially be returned by the datastore
         query
     """
-    from . import meta_queries
-
-    OPERATORS = {"=": lambda x, y: x == y, "<": lt, ">": gt, "<=": lte, ">=": gte}
-
-    queries = [query]
-    if isinstance(query, meta_queries.AsyncMultiQuery):
-        raise NotImplementedError(
-            "We just need to separate the multiquery " "into 'queries' then everything should work"
-        )
-
-    for query in queries:
-        comparisons = chain([("__kind__", "=", None)], [(x[0], x[1], x[2]) for x in query.filters])
 
-        for ent_attr, op, query_value in comparisons:
-            if ent_attr == "__key__":
-                continue
-
-            compare = OPERATORS[op]  # We want this to throw if there's some op we don't know about
-
-            if ent_attr == "__kind__":
-                ent_value = entity.kind
-                query_value = query.kind
-            else:
-                ent_value = entity.get(ent_attr)
+    OPERATORS = {
+        "=": lambda x, y: x == y,
+        "<": lt,
+        ">": gt,
+        "<=": lte,
+        ">=": gte,
+        "array_contains": lambda e, q: e and q in e,
+        "array_contains_all": lambda e, q: e and set(e).intersection(set(q)) == set(q)
+    }
 
-            if not isinstance(query_value, (list, tuple)):
-                query_values = [query_value]
-            else:
-                # The query value can be a list of ANDed values
-                query_values = query_value
+    if list(entity.key().path) != list(query.path):
+        # If the entity key doesn't match the query key then it can't match.
+        return False
 
-            if not isinstance(ent_value, (list, tuple)):
-                ent_value = [ent_value]
+    for (prop, op), query_values in query._filters.items():
+        if prop == query.wrapper.key_property_name():
+            ent_value = entity.key()
+        else:
+            ent_value = entity.get(prop)
 
-            matches = False
-            for value in query_values:  # [22, 23]
-                # If any of the values don't match then this query doesn't match
-                if op == '=' and isinstance(value, (list, tuple)):
-                    if any(attr not in ent_attr for attr in value):
-                        matches = False
-                        break
-                elif not any(compare(attr, value) for attr in ent_value):
-                    matches = False
-                    break
-            else:
-                # One of the ent_attrs matches the query_attrs
-                matches = True
+        compare = OPERATORS[op]  # We want this to throw if there's some op we don't know about
 
-            if not matches:
-                # One of the AND values didn't match
+        matches = False
+        for value in query_values:  # [22, 23]
+            # If any of the values don't match then this query doesn't match
+            if not compare(ent_value, value):
+                matches = False
                 break
         else:
-            # If we got through the loop without breaking, then the entity matches
-            return True
+            # One of the ent_attrs matches the query_attrs
+            matches = True
+
+        if not matches:
+            # One of the AND values didn't match
+            break
+    else:
+        # If we got through the loop without breaking, then the entity matches
+        return True
 
     return False
 
 
 def ensure_datetime(value):
     """
         Painfully, sometimes the Datastore returns dates as datetime objects, and sometimes
@@ -529,7 +487,12 @@
         # If we have more results then use cursor offsetting and repeat
         iterator = query.fetch(limit=0, offset=MAX_INT, start_cursor=iterator.next_page_token)
         [x for x in iterator]  # Force evaluation of the iterator
 
         count += iterator._skipped_results
 
     return count
+
+
+@lru_cache(None)
+def log_once(logger: Logger, msg: str, method='info'):
+    getattr(logger, method)(msg)
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/db/models/fields/allkeys-5.2.0.zip` & `django-gcloud-connectors-1.2.0/gcloudc/db/models/fields/allkeys-5.2.0.zip`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/db/models/fields/charfields.py` & `django-gcloud-connectors-1.2.0/gcloudc/db/models/fields/charfields.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/db/models/fields/computed.py` & `django-gcloud-connectors-1.2.0/gcloudc/db/models/fields/computed.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/db/models/fields/iterable.py` & `django-gcloud-connectors-1.2.0/gcloudc/db/models/fields/iterable.py`

 * *Files 11% similar despite different names*

```diff
@@ -52,15 +52,27 @@
         return [self.lhs.output_field.get_prep_value(v) for v in self.rhs]
 
 
 class IsEmptyLookup(Lookup):
     lookup_name = "isempty"
 
     def get_rhs_op(self, connection, rhs):
-        return "isnull %s" % rhs
+        if connection.supports_empty_array:
+            if rhs:
+                return "= %s"
+            else:
+                return "!= %s"
+        else:
+            return "isnull %s" % rhs
+
+    def get_db_prep_lookup(self, value, connection):
+        if connection.supports_empty_array:
+            return ('%s', [[]])
+        else:
+            return super().get_db_prep_lookup(value, connection)
 
     def get_prep_lookup(self):
         if self.rhs not in (True, False):
             raise ValueError("__isempty takes a boolean as a value")
 
         return self.rhs
 
@@ -251,17 +263,18 @@
 
     def get_db_prep_value(self, value, connection, prepared=False):
         if not prepared:
             value = self.get_prep_value(value)
             if value is None:
                 return None
 
-        # If the value is an empty iterable, store None
-        if value == self._iterable_type([]):
-            return None
+        if not connection.supports_empty_array:
+            # If the value is an empty iterable, store None
+            if value == self._iterable_type([]):
+                return None
 
         return self._map(self.item_field_type.get_db_prep_save, value, connection=connection)
 
     def get_db_prep_lookup(self, lookup_type, value, connection, prepared=False):
         """
         Passes the value through get_db_prep_lookup of item_field.
         """
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/db/models/fields/json.py` & `django-gcloud-connectors-1.2.0/gcloudc/db/models/fields/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import json
 from collections import OrderedDict
 
 from django.db import models
 from django.core.serializers.json import DjangoJSONEncoder
 
-from gcloudc.db.backends.datastore.indexing import Indexer, register_indexer, IgnoreForIndexing
+from gcloudc.db.backends.common.indexing import Indexer, register_indexer, IgnoreForIndexing
 from gcloudc.forms.fields import JSONFormField, JSONWidget
 
 __all__ = ("JSONField",)
 
 
 def dumps(value):
     return DjangoJSONEncoder().encode(value)
@@ -252,13 +252,13 @@
                 raise IgnoreForIndexing("")
 
         if is_isnull:
             return value is None
 
         return value
 
-    def indexed_column_name(self, field_column, value, index):
+    def indexed_column_name(self, field_column, value, index, **kwargs):
         return "_idx_json_path_{}_{}".format(field_column, index.split("__", 1)[-1])
 
 
 # Especially for JSON fields
 register_indexer(JSONKeyLookupIndexer)
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/db/models/fields/related.py` & `django-gcloud-connectors-1.2.0/gcloudc/db/models/fields/related.py`

 * *Files 2% similar despite different names*

```diff
@@ -515,22 +515,22 @@
 
     def contribute_to_related_class(self, cls, related):
         # Internal M2Ms (i.e., those with a related name ending with '+')
         # and swapped models don't get a related descriptor.
         if not self.remote_field.is_hidden() and not related.model._meta.swapped:
             setattr(cls, related.get_accessor_name(), RelatedIteratorObjectsDescriptor(related))
 
-    def get_db_prep_save(self, *args, **kwargs):
-        ret = super(RelatedIteratorField, self).get_db_prep_save(*args, **kwargs)
+    def get_db_prep_save(self, value, connection, *args, **kwargs):
+        ret = super(RelatedIteratorField, self).get_db_prep_save(value, connection, *args, **kwargs)
 
-        if not ret:
-            return None
-
-        if isinstance(ret, set):
-            ret = list(ret)
+        if not ret and isinstance(ret, (list, set, tuple)):
+            if connection.supports_empty_array:
+                return []
+            else:
+                return None
 
         ret = [self.remote_field.model._meta.pk.clean(x, self.remote_field.model) for x in ret]
 
         return ret
 
     def get_db_prep_lookup(self, *args, **kwargs):
         ret = super(RelatedIteratorField, self).get_db_prep_lookup(*args, **kwargs)
@@ -786,15 +786,15 @@
     def __get__(self, instance):
         if instance is None:
             return self
 
         value = getattr(instance, self.attname)
 
         from gcloudc.forms.fields import decode_pk
-        from gcloudc.db.backends.datastore.utils import get_model_from_db_table
+        from gcloudc.db.backends.common.helpers import get_model_from_db_table
 
         if value is None:
             return None
 
         model_ref, pk = decode_pk(value)
         try:
             return get_model_from_db_table(model_ref).objects.get(pk=pk)
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/tests/concurrent_utils.py` & `django-gcloud-connectors-1.2.0/gcloudc/tests/concurrent_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 def increment_integer_model(integer_pk, using='default', init_django=False):
     if init_django:
         import django
         from gcloudc.tests.router import Router
         django.setup()
         Router.activate_connection(connection_alias=using)
 
-    from django.db import connection
+    from django.db import connections, transaction, IntegrityError
     from .models import (
         IntegerModel,
     )
-    from gcloudc.db import transaction
-    from gcloudc.db.backends.datastore.transaction import TransactionFailedError
 
-    connection.connect()  # Make sure we have a connection
+    connection = connections['default']
+    connection.ensure_connection()
+
     try:
         with transaction.atomic(using=using):
             the_integer = IntegerModel.objects.get(pk=integer_pk)
             the_integer.integer_field = the_integer.integer_field + 1
             the_integer.save()
-    except TransactionFailedError:
+    except IntegrityError:
         raise Exception("TransactionFailedError")
     except Exception as e:
         raise Exception(f"{e.__class__}: {e.args}")
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/tests/models.py` & `django-gcloud-connectors-1.2.0/gcloudc/tests/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,14 +150,15 @@
 
 class RelatedCharFieldModel(models.Model):
     char_field = CharField(max_length=500)
 
 
 class StringPkModel(models.Model):
     name = models.CharField(max_length=500, primary_key=True)
+    other = models.CharField(max_length=500, blank=True)
 
 
 class IterableRelatedWithNonIntPkModel(models.Model):
     related_set = RelatedListField(StringPkModel, related_name="+")
     related_list = RelatedListField(StringPkModel, related_name="+")
 
 
@@ -337,16 +338,16 @@
 
 
 class MultiTableChildTwo(MultiTableParent):
     child_two_field = models.CharField(max_length=32)
 
 
 class DateTimeModel(models.Model):
-    datetime_field = models.DateTimeField(auto_now_add=True)
-    date_field = models.DateField(auto_now_add=True)
+    datetime_field = models.DateTimeField()
+    date_field = models.DateField()
 
 
 class NonIndexedModel(models.Model):
     content = models.TextField()
     binary = models.BinaryField()
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/tests/router.py` & `django-gcloud-connectors-1.2.0/gcloudc/tests/router.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/tests/test_async_multi_query.py` & `django-gcloud-connectors-1.2.0/gcloudc/tests/test_async_multi_query.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import sleuth
 from django.db import NotSupportedError
 from django.db.models import Q
 from django.test import override_settings
 
-from . import TestCase
+from . import TestCase, firestore_only, datastore_only
 from .models import (
     MultiQueryModel,
     NullableFieldModel,
 )
 
 
 class AsyncMultiQueryTest(TestCase):
@@ -19,16 +19,18 @@
         for i in range(100):
             MultiQueryModel.objects.create(field1=i)
 
         self.assertEqual(len(MultiQueryModel.objects.filter(field1__in=list(range(100)))), 100)
 
         self.assertEqual(MultiQueryModel.objects.filter(field1__in=list(range(100))).count(), 100)
 
+        qs = MultiQueryModel.objects.filter(field1__in=list(range(100))).values_list("field1", flat=True)
+
         self.assertItemsEqual(
-            MultiQueryModel.objects.filter(field1__in=list(range(100))).values_list("field1", flat=True),
+            qs,
             list(range(100)),
         )
 
         self.assertItemsEqual(
             MultiQueryModel.objects.filter(field1__in=list(range(100)))
             .order_by("-field1")
             .values_list("field1", flat=True),
@@ -45,15 +47,16 @@
     def test_pk_in_with_slicing(self):
         i1 = MultiQueryModel.objects.create()
 
         self.assertFalse(MultiQueryModel.objects.filter(pk__in=[i1.pk])[9999:])
 
         self.assertFalse(MultiQueryModel.objects.filter(pk__in=[i1.pk])[9999:10000])
 
-    def test_limit_correctly_applied_per_branch(self):
+    @datastore_only
+    def test_limit_correctly_applied_per_branch_ds(self):
         MultiQueryModel.objects.create(field2="test")
         MultiQueryModel.objects.create(field2="test2")
 
         with sleuth.watch("google.cloud.datastore.query.Query.fetch") as run_calls:
 
             list(MultiQueryModel.objects.filter(field2__in=["test", "test2"])[:1])
 
@@ -63,16 +66,45 @@
         with sleuth.watch("google.cloud.datastore.query.Query.fetch") as run_calls:
 
             list(MultiQueryModel.objects.filter(field2__in=["test", "test2"])[1:2])
 
             self.assertEqual(2, run_calls.calls[0].kwargs["limit"])
             self.assertEqual(2, run_calls.calls[1].kwargs["limit"])
 
+    @firestore_only
+    def test_limit_correctly_applied_per_branch_fs(self):
+        MultiQueryModel.objects.create(field2="test")
+        MultiQueryModel.objects.create(field2="test2")
+
+        with sleuth.watch("google.cloud.firestore_v1.query.Query.limit") as run_calls:
+
+            list(MultiQueryModel.objects.filter(field2__in=["test", "test2"])[:1])
+
+            self.assertEqual(1, run_calls.calls[0].args[1])
+            self.assertEqual(1, run_calls.calls[1].args[1])
+
+        with sleuth.watch("google.cloud.firestore_v1.query.Query.limit") as run_calls:
+
+            list(MultiQueryModel.objects.filter(field2__in=["test", "test2"])[1:2])
+
+            self.assertEqual(2, run_calls.calls[0].args[1])
+            self.assertEqual(2, run_calls.calls[1].args[1])
+
     def test_ordered_by_nullable_field(self):
         NullableFieldModel.objects.create(pk=1)
         NullableFieldModel.objects.create(pk=5, nullable=2)
 
         results = NullableFieldModel.objects.filter(
             Q(nullable=1) | Q(nullable=2) | Q(nullable__isnull=True)
         ).order_by("nullable").values_list("pk", flat=True)
 
         self.assertCountEqual(results, [1, 5])
+
+    @firestore_only
+    def test_correct_number_of_queries(self):
+        ids = [str(x) for x in range(50)]
+
+        qs = MultiQueryModel.objects.filter(field2__in=ids).filter(field2__in=ids)
+
+        with sleuth.watch("gcloudc.db.backends.firestore.base.Query.fetch") as fetch_calls:
+            list(qs)
+            self.assertEqual(fetch_calls.call_count, 50)
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/tests/test_caching.py` & `django-gcloud-connectors-1.2.0/gcloudc/tests/test_caching.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,19 @@
-from gcloudc.db.backends.datastore.caching import get_context
-
 from . import TestCase
 from .models import KeysOnlyModel
 
 
 class RegressionsTestCase(TestCase):
     databases = "__all__"
 
     def test_keysonly_query_with_projection_returns_results_every_time(self):
         """Regression test for https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/-/issues/56"""
 
         instance = KeysOnlyModel.objects.create(name="Alice", flag=False)
 
-        # Clear the process cache as the create call adds `instance` to the
-        # process cache
-        get_context().reset(keep_disabled_flags=True)
-
         # Run two queries that result in a keys only query that use a projection
         first_queryset = KeysOnlyModel.objects.filter(
             pk__in=[instance.pk], flag=False
         ).values_list("id", flat=True)
         second_queryset = first_queryset.all()  # Clones the queryset above
 
         # Both should yield the same results
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/tests/test_cloud_datastore_runner.py` & `django-gcloud-connectors-1.2.0/gcloudc/tests/test_cloud_datastore_runner.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/tests/test_computed_field.py` & `django-gcloud-connectors-1.2.0/gcloudc/tests/test_computed_field.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/tests/test_connector.py` & `django-gcloud-connectors-1.2.0/gcloudc/tests/test_connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,58 +22,50 @@
     ValidationError,
 )
 from django.db import (
     DatabaseError,
     DataError,
     IntegrityError,
     NotSupportedError,
+    transaction,
 )
-from django.db import connection
 from django.db import connection as default_connection
 from django.db import models
 from django.db.models.query import Q
 from django.forms import ModelForm
 from django.forms.models import modelformset_factory
 from django.test import RequestFactory
 from django.test.utils import override_settings
 from django.urls import path
 from django.utils.safestring import SafeText
 
 from django.utils.timezone import make_aware
-from google.cloud.datastore import key
-from google.cloud.datastore.entity import Entity
+from gcloudc.db.backends.common.base.entity import Entity, Key
 
-from gcloudc.db.backends.datastore import (
-    caching,
-    indexing,
-    transaction,
-)
+from gcloudc.db.backends.common import indexing
+from gcloudc.db.backends.common.parsers.expressions import Scatter
 
-from gcloudc.db.backends.datastore.expressions import Scatter
-
-from gcloudc.db.backends.datastore.commands import FlushCommand
-from gcloudc.db.backends.datastore.indexing import (
+from gcloudc.db.backends.common.commands import FlushCommand
+from gcloudc.db.backends.common.indexing import (
     IExactIndexer,
     add_special_index,
     get_indexer,
 )
-from gcloudc.db.backends.datastore.unique_mixins import UniquenessMixin
-from gcloudc.db.backends.datastore.unique_utils import (
+from gcloudc.db.backends.common.mixins import UniquenessMixin
+from gcloudc.db.backends.common.constraints import (
     _unique_combinations,
-    query_is_unique,
     unique_identifiers_from_entity,
 )
-from gcloudc.db.backends.datastore.utils import (
+from gcloudc.db.backends.common.helpers import (
     decimal_to_string,
     entity_matches_query,
     normalise_field_value,
 )
-from gcloudc.db.decorators import disable_cache
 
-from . import TestCase
+from . import TestCase, firestore_only, datastore_only
 from .models import (
     Animal,
     DateTimeModel,
     DurationModel,
     Enclosure,
     IntegerModel,
     ManyFields,
@@ -128,45 +120,115 @@
         results = IntegerModel.objects.filter(pk__lt=0)
         self.assertEqual(0, len(results))
 
         results = IntegerModel.objects.filter(pk__lte=0)
         self.assertEqual(0, len(results))
 
     def test_entity_matches_query(self):
-        rpc = transaction._rpc(default_connection.alias)
-
-        entity = Entity(rpc.key("test_model"))
+        k = default_connection.connection.new_key(
+            "test_model", 1, namespace=default_connection.namespace
+        )
+        entity = Entity(k)
         entity["name"] = "Charlie"
         entity["age"] = 22
 
-        query = rpc.query(kind="test_model")
+        query = default_connection.get_query_class()(
+            table_or_path=["test_model"], namespace=default_connection.namespace,
+            connection=default_connection
+        )
         query.add_filter("name", "=", "Charlie")
         self.assertTrue(entity_matches_query(entity, query))
 
-        query = rpc.query(kind="test_model")
+        query = default_connection.get_query_class()(
+            table_or_path=["test_model"], namespace=default_connection.namespace,
+            connection=default_connection
+        )
         query.add_filter("age", ">=", 5)
         self.assertTrue(entity_matches_query(entity, query))
 
-        query = rpc.query(kind="test_model")
+        query = default_connection.get_query_class()(
+            table_or_path=["test_model"], namespace=default_connection.namespace,
+            connection=default_connection
+        )
         query.add_filter("age", "<", 22)
         self.assertFalse(entity_matches_query(entity, query))
 
-        query = rpc.query(kind="test_model")
+        query = default_connection.get_query_class()(
+            table_or_path=["test_model"], namespace=default_connection.namespace,
+            connection=default_connection
+        )
         query.add_filter("age", "<=", 22)
         self.assertTrue(entity_matches_query(entity, query))
 
-        query = rpc.query(kind="test_model")
+        query = default_connection.get_query_class()(
+            table_or_path=["test_model"], namespace=default_connection.namespace,
+            connection=default_connection
+        )
         query.add_filter("name", "=", "Fred")
         self.assertFalse(entity_matches_query(entity, query))
 
+        query = default_connection.get_query_class()(
+            table_or_path=["test_model"], namespace=default_connection.namespace,
+            connection=default_connection
+        )
+        query.add_filter("name", "array_contains", "Fred")
         # If the entity has a list field, then if any of them match the
         # query then it's a match
         entity["name"] = ["Bob", "Fred", "Dave"]
         self.assertTrue(entity_matches_query(entity, query))  # ListField test
 
+        entity["name"] = None
+        query.add_filter("name", "array_contains", "Fred")
+        self.assertFalse(entity_matches_query(entity, query))  # ListField test
+
+    def test_entity_matches_query_same_field_different_collection(self):
+        """
+            Test that the entity_matches_query does not match entities from
+            a different collection.
+        """
+        k = default_connection.connection.new_key(
+            "test_model", 1, namespace=default_connection.namespace
+        )
+        entity = Entity(k)
+        entity["name"] = "Charlie"
+        entity["age"] = 22
+
+        query = default_connection.get_query_class()(
+            table_or_path=["another_model"], namespace=default_connection.namespace,
+            connection=default_connection
+        )
+        query.add_filter("name", "=", "Charlie")
+        self.assertFalse(entity_matches_query(entity, query))
+
+    def test_entity_matches_query_array_contains_all(self):
+        """
+            Test that the entity_matches_query works with array_contains_all operator.
+        """
+        k = default_connection.connection.new_key(
+            "test_model", 1, namespace=default_connection.namespace
+        )
+        entity = Entity(k)
+        entity["names"] = ["Charlie", "Fred", "Dave"]
+
+        query = default_connection.get_query_class()(
+            table_or_path=["test_model"], namespace=default_connection.namespace,
+            connection=default_connection
+        )
+
+        query.add_filter("names", "array_contains_all", ["Charlie", "Fred"])
+        self.assertTrue(entity_matches_query(entity, query))
+
+        query.add_filter("names", "array_contains_all", ["Charlie", "Another"])
+        self.assertFalse(entity_matches_query(entity, query))
+
+        entity["names"] = None
+
+        query.add_filter("names", "array_contains_all", ["Charlie", "Fred"])
+        self.assertFalse(entity_matches_query(entity, query))
+
     def test_exclude_pks_with_slice(self):
         for i in range(10):
             TestFruit.objects.create(name=str(i), color=str(i))
 
         to_exclude = [str(x) for x in list(range(5)) + list(range(15, 20))]
 
         to_return = TestFruit.objects.exclude(pk__in=set(to_exclude)).values_list("pk", flat=True)[:2]
@@ -184,56 +246,41 @@
 
         self.assertEqual(1, TestFruit.objects.filter(pk__in=["Apple", "Orange"]).exclude(pk__in=["Apple"]).count())
 
     def test_defaults(self):
         fruit = TestFruit.objects.create(name="Apple", color="Red")
         self.assertEqual("Unknown", fruit.origin)
 
-        rpc = transaction._rpc(default_connection.alias)
+        rpc = default_connection.connection
+
+        instance = rpc.get(
+            default_connection.connection.new_key(
+                TestFruit._meta.db_table, fruit.pk, namespace=default_connection.namespace
+            )
+        )
 
-        instance = rpc.get(rpc.key(TestFruit._meta.db_table, fruit.pk))
         del instance["origin"]
         rpc.put(instance)
 
         fruit = TestFruit.objects.get()
         self.assertIsNone(fruit.origin)
         fruit.save()
 
         fruit = TestFruit.objects.get()
         self.assertEqual("Unknown", fruit.origin)
 
-    @disable_cache()
     def test_get_by_keys(self):
         colors = ["Red", "Green", "Blue", "Yellow", "Orange"]
         fruits = [TestFruit.objects.create(name=str(x), color=random.choice(colors)) for x in range(32)]
-        rpc = transaction._rpc(default_connection.alias)
-
-        # Check that projections work with key lookups
-        with sleuth.watch("gcloudc.db.backends.datastore.transaction.Transaction.query") as query:
-            TestFruit.objects.only("color").get(pk="0").color
-            self.assertEqual(query.calls[0].kwargs["projection"], ["color"])
-
-            # Make sure the query is an ancestor of the key
-            self.assertEqual(
-                query.call_returns[0].ancestor,
-                rpc.key(
-                    TestFruit._meta.db_table, "0"
-                )
-            )
 
-        # Now check projections work with fewer than 100 things
-        with sleuth.watch('gcloudc.db.backends.datastore.meta_queries.AsyncMultiQuery.__init__') as query_init:
-            with sleuth.watch("gcloudc.db.backends.datastore.transaction.Transaction.query") as query:
-                keys = [str(x) for x in range(32)]
-                results = list(TestFruit.objects.only("color").filter(pk__in=keys).order_by("name"))  # One multiquery
-                self.assertEqual(query_init.call_count, 1)
-                self.assertEqual(len([x.ancestor for x in query.call_returns if x.ancestor]), 32)  # 32 Ancestor calls
+        keys = [str(x) for x in range(32)]
+        results = list(TestFruit.objects.only("color").filter(pk__in=keys).order_by("name"))  # One multiquery
 
-                # Confirm the ordering is correct
-                self.assertEqual(sorted(keys), [x.pk for x in results])
+        # Confirm the ordering is correct
+        self.assertEqual(sorted(keys), [x.pk for x in results])
 
         results = list(TestFruit.objects.only("color").filter(pk__in=keys).order_by("name")[5:10])
         self.assertEqual(len(results), 5)
         self.assertEqual([x.pk for x in results], sorted(keys)[5:10])
 
         # Make sure we can do a normal (non-projection) get by keys
         self.assertItemsEqual(TestFruit.objects.filter(pk__in=keys), fruits)
@@ -265,18 +312,17 @@
             return _wrapped
 
         from django.db.models import query
         wrapped_get = wrap_get(query.QuerySet.get)
 
         UniqueModel.objects.create(unique_field="Test")
 
-        with disable_cache():
-            with sleuth.switch("django.db.models.query.QuerySet.get", wrapped_get):
-                instance, created = UniqueModel.objects.get_or_create(unique_field="Test")
-                self.assertFalse(created)
+        with sleuth.switch("django.db.models.query.QuerySet.get", wrapped_get):
+            instance, created = UniqueModel.objects.get_or_create(unique_field="Test")
+            self.assertFalse(created)
 
     def test_setting_non_null_null_throws_integrity_error(self):
         with self.assertRaises(IntegrityError):
             IntegerModel.objects.create(integer_field=None)
 
         with self.assertRaises(IntegrityError):
             instance = IntegerModel()
@@ -304,50 +350,18 @@
         self.assertEqual(u'-0002312487812767', decimal_to_string(decimal.Decimal(-2312487812767)))
         self.assertEqual(u'002312487812', decimal_to_string(decimal.Decimal(2312487812), 12))
         self.assertEqual(u'002387812.320', decimal_to_string(decimal.Decimal(2387812.32), 12, 3))
         self.assertEqual(u'-002387812.513', decimal_to_string(decimal.Decimal(-2387812.513212), 12, 3))
         self.assertEqual(u'0237812.000', decimal_to_string(decimal.Decimal(237812), 10, 3))
         self.assertEqual(u'-0237812.210', decimal_to_string(decimal.Decimal(-237812.21), 10, 3))
 
-    def test_gae_conversion(self):
-        # A PK IN query should result in a single get by key
-
-        with sleuth.watch("gcloudc.db.backends.datastore.transaction.Transaction.get") as get_mock:
-            list(TestUser.objects.filter(pk__in=[1, 2, 3]))  # Force the query to run
-            self.assertEqual(1, get_mock.call_count)
-
-        with sleuth.watch("gcloudc.db.backends.datastore.transaction.Transaction.query") as query_mock:
-            list(TestUser.objects.filter(username="test"))
-            self.assertEqual(1, query_mock.call_count)
-
-        with sleuth.watch("gcloudc.db.backends.datastore.meta_queries.AsyncMultiQuery.fetch") as query_mock:
-            list(TestUser.objects.filter(username__in=["test", "cheese"]))
-            self.assertEqual(1, query_mock.call_count)
-
-        with sleuth.watch("gcloudc.db.backends.datastore.transaction.Transaction.get") as get_mock:
-            list(TestUser.objects.filter(pk=1))
-            self.assertEqual(1, get_mock.call_count)
-
-        with sleuth.watch("gcloudc.db.backends.datastore.meta_queries.AsyncMultiQuery.fetch") as query_mock:
-            list(TestUser.objects.exclude(username__startswith="test"))
-            self.assertEqual(1, query_mock.call_count)
-
-        with sleuth.watch("gcloudc.db.backends.datastore.transaction.Transaction.get") as get_mock:
-            list(
-                TestUser.objects.filter(pk__in=[1, 2, 3, 4, 5, 6, 7, 8]).
-                filter(username__in=["test", "test2", "test3"]).
-                filter(email__in=["test@example.com", "test2@example.com"])
-            )
-
-            self.assertEqual(1, get_mock.call_count)
-
     def test_gae_query_display(self):
         # Shouldn't raise any exceptions:
-        representation = str(TestUser.objects.filter(username='test').query)
-        self.assertTrue('test' in representation)
+        representation = str(TestUser.objects.filter(username='test-value').query)
+        self.assertTrue('test-value' in representation)
         self.assertTrue('username' in representation)
 
     def test_range_behaviour(self):
         IntegerModel.objects.create(integer_field=5)
         IntegerModel.objects.create(integer_field=10)
         IntegerModel.objects.create(integer_field=15)
 
@@ -392,16 +406,14 @@
         null_date.save()
 
         null_date = NullDate.objects.get()
         self.assertIsNone(null_date.date)
         self.assertIsNone(null_date.time)
         self.assertIsNone(null_date.datetime)
 
-    # Needs cache disabled, since the cached value still has the pre-transformed values
-    @disable_cache()
     def test_convert_str_subclasses_to_str(self):
         # The App Engine SDK raises BadValueError if you try saving a SafeText
         # string to a CharField. Djangae explicitly converts it to str.
         grue = SafeText(u'grue')
 
         self.assertIsInstance(grue, str)
         self.assertNotEqual(type(grue), str)
@@ -436,14 +448,19 @@
                 origin="England"
             ).exclude(name="Pear").order_by("origin"))
         )
 
         # And apparently having both a __gt and a __lt filter on the same field is also fine
         self.assertItemsEqual([banana], list(TestFruit.objects.order_by().filter(name__lt="Pear", name__gt="Apple")))
 
+    # FIXME: This is only skipped on Firestore because it orders by ID descending
+    # and Firestore can't do that (:shrug:). If Firestore gains that ability, or
+    # we find a workaround then we can enable this. Alternatively we can update
+    # the test to not do a descending query.
+    @datastore_only
     def test_excluding_pks_is_emulated(self):
         apple = TestFruit.objects.create(name="Apple", color="Green", is_mouldy=True, origin="England")
         banana = TestFruit.objects.create(name="Banana", color="Yellow", is_mouldy=True, origin="Dominican Republic")
         cherry = TestFruit.objects.create(name="Cherry", color="Red", is_mouldy=True, origin="Germany")
         pear = TestFruit.objects.create(name="Pear", color="Green", origin="England")
 
         self.assertEqual(
@@ -564,94 +581,135 @@
 
         with concurrent.futures.ThreadPoolExecutor(max_workers=len(properties_to_set)) as executor:
             for property, value in properties_to_set.items():
                 thread_property_map[property] = executor.submit(
                     set_test_many_fields_model_field, original_fruit, property, value)
         concurrent.futures.wait(thread_property_map.values())
 
-        with disable_cache():
-            original_fruit.refresh_from_db()
+        original_fruit.refresh_from_db()
 
         futures_exceptions = [future.exception() for future in thread_property_map.values()]
         number_successful_writes = len(list(itertools.filterfalse(None, futures_exceptions)))
         self.assertGreater(number_successful_writes, 0, 'It should save at least once')
 
         for property, future in thread_property_map.items():
             exception = future.exception()
             if exception:
-                self.assertIsInstance(exception, transaction.TransactionFailedError)
+                self.assertIsInstance(exception, DatabaseError)
             else:
                 self.assertEqual(getattr(original_fruit, property), properties_to_set.get(property))
 
+    def test_is_null_filtering(self):
+        o1 = ModelWithNullableCharField.objects.create(some_id=1, field1="test")
+        o2 = ModelWithNullableCharField.objects.create(some_id=1)
+        o3 = ModelWithNullableCharField.objects.create(some_id=1)
+
+        self.assertEqual(
+            {o2, o3},
+            set(ModelWithNullableCharField.objects.filter(field1__isnull=True))
+        )
+
+        self.assertEqual(
+            {o1},
+            set(ModelWithNullableCharField.objects.filter(field1__isnull=False))
+        )
+
+    @datastore_only
     def test_ordering_by_scatter_property(self):
         try:
             list(TestFruit.objects.order_by(Scatter()))
         except:  # noqa
             raise
             logging.exception("Error sorting on __scatter__")
             self.fail("Unable to sort on __scatter__ property like we should")
 
+    def test_text_fields_arent_indexed(self):
+        # String that is too long for Datastore or Firestore indexing
+        long_string = "".join([random.choice(letters) for x in range(1600)])
+        self.assertTrue(len(long_string) > 1500)
+        fruit = TestFruit.objects.create(pk="test", text_field=long_string)
+        fruit.refresh_from_db()
+        fruit.save()
+
+    def test_bytes_fields_arent_indexed(self):
+        # String that is too long for Datastore or Firestore indexing
+        long_string = "".join([random.choice(letters) for x in range(1600)])
+        long_string = long_string.encode("ascii")
+        fruit = TestFruit.objects.create(pk="test", binary_field=long_string)
+        fruit.refresh_from_db()
+        fruit.save()
+
     def test_ordering_on_non_indexed_fields_not_supported(self):
         self.assertRaises(NotSupportedError, list, TestFruit.objects.order_by("text_field"))
         self.assertRaises(NotSupportedError, list, TestFruit.objects.order_by("binary_field"))
 
     def test_ordering_on_sparse_field(self):
         """
         Case when sorting on field that is not present in all of
         Datastore entities. That can easily happen when you added
         new field to model and did not populated all existing entities
         """
-        rpc = transaction._rpc(default_connection.alias)
+        rpc = default_connection.connection
 
         # Clean state
         self.assertEqual(TestFruit.objects.count(), 0)
 
         # Put constistent instances to Datastore
         TestFruit.objects.create(name='a', color='a')
         TestFruit.objects.create(name='b', color='b')
 
         # Put inconsistent instances to Datastore
         # Color fields is missing (not even None)
         # we need more than 1 so we explore all sorting branches
         values = {'name': 'c'}
-        entity = Entity(rpc.key(TestFruit._meta.db_table, 'c'))
-        entity.update(values)
+        entity = Entity(Key(TestFruit._meta.db_table, 'c', namespace=default_connection.namespace))
+        entity._properties.update(values)
         rpc.put(entity)
 
         values = {'name': 'd'}
-        entity = Entity(rpc.key(TestFruit._meta.db_table, 'd'))
-        entity.update(values)
+        entity = Entity(Key(TestFruit._meta.db_table, 'd', namespace=default_connection.namespace))
+        entity._properties.update(values)
         rpc.put(entity)
 
         # Ok, we can get all 4 instances
         self.assertEqual(TestFruit.objects.count(), 4)
 
-        # Sorted list. No exception should be raised
-        # (esp KeyError from django_ordering_comparison)
-        with sleuth.watch('gcloudc.db.backends.datastore.meta_queries.django_ordering_comparison') as compare:
-            all_names = ['a', 'b', 'c', 'd']
-            fruits = list(
-                TestFruit.objects.filter(name__in=all_names).order_by('color', 'name')
-            )
-            # Make sure troubled code got triggered
-            # ie. with all() it doesn't
-            self.assertTrue(compare.called)
+        all_names = ['a', 'b', 'c', 'd']
+        fruits = list(
+            TestFruit.objects.filter(name__in=all_names).order_by('color', 'name')
+        )
+        values = [(x.color or "", x.name) for x in fruits]
+        self.assertEqual(sorted(values), values)
 
         # Test the ordering of the results.  The ones with a color of None should come back first,
         # and of the ones with color=None, they should be ordered by name
         # Missing one (None) as first
         expected_fruits = [
             ('c', None), ('d', None), ('a', 'a'), ('b', 'b'),
         ]
 
         self.assertEqual(
             [(fruit.name, fruit.color) for fruit in fruits],
             expected_fruits,
         )
 
+    def test_double_order_on_same_key(self):
+
+        a = TestFruit.objects.create(name='a', color='a')
+        b = TestFruit.objects.create(name='b', color='b')
+
+        self.assertEqual(list(TestFruit.objects.order_by('color', 'color')), [a, b])
+
+    def test_order_on_field_after_key(self):
+
+        a = TestFruit.objects.create(name='a', color='a')
+        b = TestFruit.objects.create(name='b', color='b')
+
+        self.assertEqual(list(TestFruit.objects.order_by('name', 'color')), [a, b])
+
     def test_duration_field_stored_as_float(self):
         """ See issue #512.  We have a bug report that the DurationField comes back as None when
             the value is set to a particular value which is roughly 3 days. This is caused by it
             being stored as a float instead of an int in the DB.
         """
         td2 = datetime.timedelta(days=2)
         # If the duration value is stored as a float instead of an int then this particular duration
@@ -673,18 +731,18 @@
         durations_as_2 = DurationModel.objects.get(pk=durations_as_2.pk)
         durations_as_3 = DurationModel.objects.get(pk=durations_as_3.pk)
         self.assertEqual(durations_as_2.duration_field, td2)
         self.assertEqual(durations_as_2.duration_field_nullable, td2)
         self.assertEqual(durations_as_3.duration_field, td3)
         self.assertEqual(durations_as_3.duration_field_nullable, td3)
         # And just for good measure, check the raw value in the datastore
-        rpc = transaction._rpc(default_connection.alias)
-
-        key = rpc.key(DurationModel._meta.db_table, durations_as_3.pk)
-        entity = rpc.get(key)
+        key = default_connection.connection.new_key(
+            DurationModel._meta.db_table, durations_as_3.pk, namespace=default_connection.namespace
+        )
+        entity = default_connection.connection.get(key)
         self.assertTrue(isinstance(entity['duration_field'], int))
 
     def test_datetime_and_time_fields_precision_for_projection_queries(self):
         """
         The returned datetime and time values should include microseconds.
         See issue #707.
         """
@@ -731,39 +789,35 @@
         t1 = TestUser.objects.create(username='foo', field2='bar')
         condition = Q() | Q(username='foo')
         self.assertEqual(t1, TestUser.objects.filter(condition).first())
 
         condition = Q()
         self.assertEqual(t1, TestUser.objects.filter(condition).first())
 
-    def test_only_defer_does_project(self):
-        with sleuth.watch("gcloudc.db.backends.datastore.transaction.Transaction.query") as query:
-            with sleuth.watch("google.cloud.datastore.query.Query.keys_only") as keys_only:
-                list(TestUser.objects.only("pk").all())
-                self.assertFalse(query.calls[0].kwargs["projection"])
-                self.assertEqual(1, keys_only.call_count)
-
-        with sleuth.watch("gcloudc.db.backends.datastore.transaction.Transaction.query") as query:
-            with sleuth.watch("google.cloud.datastore.query.Query.keys_only") as keys_only:
-                list(TestUser.objects.values("pk"))
-                self.assertFalse(query.calls[0].kwargs["projection"])
-                self.assertEqual(1, keys_only.call_count)
-
-        with sleuth.watch("gcloudc.db.backends.datastore.transaction.Transaction.query") as query:
-            with sleuth.watch("google.cloud.datastore.query.Query.keys_only") as keys_only:
-                list(TestUser.objects.only("username").all())
-                self.assertEqual(0, keys_only.call_count)
-                self.assertItemsEqual(query.calls[0].kwargs["projection"], ["username"])
-
-        with sleuth.watch("gcloudc.db.backends.datastore.transaction.Transaction.query") as query:
-            with sleuth.watch("google.cloud.datastore.query.Query.keys_only") as keys_only:
-                list(TestUser.objects.defer("username").all())
-                self.assertEqual(0, keys_only.call_count)
-                self.assertTrue(query.calls[0].kwargs["projection"])
-                self.assertFalse("username" in query.calls[0].kwargs["projection"])
+    def test_only_defer_does_projection(self):
+        with sleuth.watch("gcloudc.db.backends.common.base.query.Query.__init__") as query:
+            list(TestUser.objects.only("username").all())
+            self.assertFalse(query.calls[0].kwargs.get("only_return_keys"))
+            self.assertItemsEqual(query.calls[0].kwargs.get("only_return_fields", []), ["username"])
+
+        with sleuth.watch("gcloudc.db.backends.common.base.query.Query.__init__") as query:
+            list(TestUser.objects.only("pk").all())
+            self.assertFalse(query.calls[0].kwargs.get("only_return_fields"))
+            self.assertTrue(query.calls[0].kwargs.get("only_return_keys"))
+
+        with sleuth.watch("gcloudc.db.backends.common.base.query.Query.__init__") as query:
+            list(TestUser.objects.values("pk"))
+            self.assertFalse(query.calls[0].kwargs.get("only_return_fields"))
+            self.assertTrue(query.calls[0].kwargs.get("only_return_keys"))
+
+        with sleuth.watch("gcloudc.db.backends.common.base.query.Query.__init__") as query:
+            list(TestUser.objects.defer("username").all())
+            self.assertFalse(query.calls[0].kwargs.get("only_return_keys"))
+            self.assertTrue(query.calls[0].kwargs["only_return_fields"])
+            self.assertFalse("username" in query.calls[0].kwargs["only_return_fields"])
 
     def test_chaining_none_filter(self):
         t1 = TestUser.objects.create()
         self.assertFalse(TestUser.objects.none().filter(pk=t1.pk))
 
     def test_values_list_returns_str_strings(self):
         TestUser.objects.create(username=u"Łukasz")
@@ -809,67 +863,14 @@
 
     def test_cache_timeout(self):
         cache.set('test?', 'yes!', 1)
         import time
         time.sleep(1)
         self.assertEqual(cache.get('test?'), None)
 
-    @override_settings(ROOT_URLCONF="gcloudc.tests.test_connector")
-    def test_cache_cleared_on_request(self):
-        user = TestUser.objects.create(username="test")
-
-        user_key = key.Key(
-            TestUser._meta.db_table,
-            user.pk,
-            namespace=connection.settings_dict["NAMESPACE"],
-            project=connection.settings_dict["PROJECT"]
-        )
-
-        from_cache = caching.get_from_cache_by_key(
-            user_key
-        )
-
-        self.assertIsNotNone(from_cache)
-        self.client.get("/")
-
-        from_cache = caching.get_from_cache_by_key(
-            user_key
-        )
-
-        self.assertIsNone(from_cache)
-
-    def test_disable_cache_decorator(self):
-        user = TestUser.objects.create(username="randy", first_name="Randy")
-
-        with transaction.atomic():
-            with sleuth.watch('gcloudc.db.backends.datastore.context.CacheDict.get') as cachedict_get:
-                user.first_name = "Łukasz"
-                user.save()
-
-                from_cache = TestUser.objects.get(username="randy")
-
-                # Ok, cache works
-                self.assertEqual(from_cache.first_name, "Łukasz")
-                # This is not 1, because of unique constraints
-                self.assertEqual(cachedict_get.call_count, 3)
-
-                with disable_cache():
-                    non_cached = TestUser.objects.get(username="randy")
-                    # Result is not fetched from the cache
-                    self.assertEqual(non_cached.first_name, "Randy")
-                    # Same call count as before
-                    self.assertEqual(cachedict_get.call_count, 3)
-
-                from_cache = TestUser.objects.get(username="randy")
-
-                # Previous GET didn't override the cache
-                self.assertEqual(from_cache.first_name, "Łukasz")
-                # One extra call to cache.get
-                self.assertEqual(cachedict_get.call_count, 4)
-
 
 def compare_markers(list1, list2):
     return (
         sorted([(x.key(), x.instance) for x in list1]) == sorted([(x.key(), x.instance) for x in list2])
     )
 
 
@@ -948,41 +949,22 @@
         ModelWithUniques.objects.create(name="One")
 
         instance = ModelWithUniques.objects.create(name="Two")
         with self.assertRaises(IntegrityError):
             instance.name = "One"
             instance.save()
 
-    def test_delete_works_regardless_of_markers(self):
-        stale_instance = ModelWithUniques.objects.create(name="One")
-
-        rpc = transaction._rpc(default_connection.alias)
-        # Delete the entity without updating the markers
-        key = rpc.key(ModelWithUniques._meta.db_table, stale_instance.pk)
-        rpc.delete(key)
-
-        ModelWithUniques.objects.create(name="One")
-
     def test_unique_combinations_are_returned_correctly(self):
         combos_one = _unique_combinations(ModelWithUniquesOnForeignKey, ignore_pk=True)
         combos_two = _unique_combinations(ModelWithUniquesOnForeignKey, ignore_pk=False)
-        rpc = transaction._rpc(default_connection.alias)
 
         self.assertEqual([['name', 'related_name'], ['name'], ['related_name']], combos_one)
         self.assertEqual([['name', 'related_name'], ['id'], ['name'], ['related_name']], combos_two)
 
-        class Entity(dict):
-            def __init__(self, model, id):
-                self._key = rpc.key(model, id)
-
-            @property
-            def key(self):
-                return self._key
-
-        e1 = Entity(ModelWithUniquesOnForeignKey._meta.db_table, 1)
+        e1 = Entity(Key(ModelWithUniquesOnForeignKey._meta.db_table, 1))
         e1["name"] = "One"
         e1["related_name_id"] = 1
 
         ids_one = unique_identifiers_from_entity(ModelWithUniquesOnForeignKey, e1, ignore_pk=False)
 
         self.assertItemsEqual([
             u'tests_modelwithuniquesonforeignkey|id:1',
@@ -1180,36 +1162,69 @@
     def test_datetime_contains(self):
         """
             Django allows for __contains on datetime field, so that you can search for a specific
             date. This is probably just because SQL allows querying it on a string, and contains just
             turns into a like query. This test just makes sure we behave the same
         """
 
-        instance = DateTimeModel.objects.create()  # Create a DateTimeModel, it has auto_now stuff
+        from django.utils import timezone
+        fake_future_datetime = datetime.datetime(2100, 2, 10, 11, 59, 59, tzinfo=timezone.utc)
+        fake_future_date = datetime.date(2100, 2, 10)
+        today_datetime = datetime.datetime.now()
+        today_date = datetime.date.today()
+
+        DateTimeModel.objects.create(datetime_field=fake_future_datetime, date_field=fake_future_date)
+
+        instance_today_1 = DateTimeModel.objects.create(
+            datetime_field=today_datetime,
+            date_field=today_date
+        )
 
         by_datetime = list(DateTimeModel.objects.filter(
-                datetime_field__contains=instance.datetime_field.date()
+            datetime_field__contains=today_date
         ))
 
         # Make sure that if we query a datetime on a date it is properly returned
         self.assertItemsEqual(
-            [instance],
+            [instance_today_1],
             by_datetime
         )
 
-        by_year = list(DateTimeModel.objects.filter(date_field__contains=instance.date_field.year))
-        self.assertItemsEqual([instance], by_year)
+        by_year = list(DateTimeModel.objects.filter(date_field__contains=today_date.year))
+        self.assertItemsEqual([instance_today_1], by_year)
+
+        # Try with 2 mathing entities
+        instance_today_2 = DateTimeModel.objects.create(
+            datetime_field=today_datetime,
+            date_field=today_date
+        )
+
+        by_datetime = list(DateTimeModel.objects.filter(
+            datetime_field__contains=today_date
+        ))
+
+        # Make sure that if we query a datetime on a date it is properly returned
+        self.assertItemsEqual(
+            [instance_today_1, instance_today_2],
+            by_datetime
+        )
+
+        by_year = list(DateTimeModel.objects.filter(date_field__contains=today_date.year))
+        self.assertItemsEqual([instance_today_1, instance_today_2], by_year)
 
     # See https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/issues/2
     def test_datetime_compare(self):
         from django.utils import timezone
         fake_future = datetime.datetime(2100, 2, 10, 11, 59, 59, tzinfo=timezone.utc)
         fake_now = timezone.datetime(2020, 2, 10, 11, 59, 59)
 
-        instance = DateTimeModel.objects.create(datetime_field=fake_future)
+        instance = DateTimeModel.objects.create(
+            datetime_field=fake_future,
+            date_field=datetime.date.today(),
+        )
 
         fetched = DateTimeModel.objects.get(datetime_field__gt=fake_now, pk=instance.pk)
 
         self.assertEqual(fetched, instance)
 
     def test_combinations_of_special_indexes(self):
         qs = TestUser.objects.filter(username__iexact='Hello') | TestUser.objects.filter(username__contains='ood')
@@ -1245,14 +1260,19 @@
         self.assertEqual(child2, MultiTableChildTwo.objects.get(pk=child2.pk))
         self.assertTrue(MultiTableParent.objects.filter(pk=child2.pk).exists())
 
     def test_anding_pks(self):
         results = TestUser.objects.filter(id__exact=self.u1.pk).filter(id__exact=self.u2.pk)
         self.assertEqual(list(results), [])
 
+    def test_filter_by_key_then_projection(self):
+        results = list(TestFruit.objects.filter(name="apple").values_list("pk", "color"))
+        self.assertEqual(len(results), 1)
+        self.assertEqual(results[0], ("apple", "red"))
+
     def test_unusual_queries(self):
 
         results = list(TestFruit.objects.filter(name__in=["apple", "orange"]))
         self.assertEqual(1, len(results))
         self.assertItemsEqual(["apple"], [x.name for x in results])
 
         results = TestFruit.objects.filter(name__in=["apple", "banana"])
@@ -1344,14 +1364,28 @@
         results = list(TestFruit.objects.filter(name='', color='red').order_by("name"))
         self.assertItemsEqual([], results)
 
         # IN query
         results = list(TestFruit.objects.filter(name__in=['', 'apple']))
         self.assertItemsEqual([self.apple], results)
 
+    def test_sorting_by_filtered_field(self):
+        user = TestUser.objects.create(
+            username="F",
+            email="test4@example.com",
+            last_login=(datetime.datetime.now() - datetime.timedelta(days=1)).date(),
+            id=6, first_name="F", second_name="F"
+        )
+
+        yesterday = (datetime.datetime.now() - datetime.timedelta(days=1)).date()
+
+        # Filtering
+        results = list(TestUser.objects.filter(last_login=yesterday).order_by("-last_login"))
+        self.assertItemsEqual([user], results)
+
     def test_or_queryset(self):
         """
             This constructs an OR query, this is currently broken in the parse_where_and_check_projection
             function. WE MUST FIX THIS!
         """
         q1 = TestUser.objects.filter(username="A")
         q2 = TestUser.objects.filter(username="B")
@@ -1447,20 +1481,28 @@
     def test_invalid_id_value_on_insert(self):
         user = TestUser.objects.get(username="A")
         # pass in a User object as if it's an int
         permission = Permission(user_id=user, perm="test_perm")
         with self.assertRaises(TypeError):
             permission.save(force_insert=True)
 
-    def test_values_list_on_pk_does_keys_only_query(self):
+    @datastore_only
+    def test_values_list_on_pk_does_keys_only_query_ds(self):
         with sleuth.watch("google.cloud.datastore.query.Query.keys_only") as keys_only:
             list(TestUser.objects.all().values_list('pk', flat=True))
             self.assertTrue(keys_only.called)
             self.assertEqual(5, len(TestUser.objects.all().values_list('pk')))
 
+    @firestore_only
+    def test_values_list_on_pk_does_keys_only_query_fs(self):
+        with sleuth.watch("google.cloud.firestore.Query.select") as keys_only:
+            list(TestUser.objects.all().values_list('pk', flat=True))
+            self.assertTrue(keys_only.called)
+            self.assertEqual(5, len(TestUser.objects.all().values_list('pk')))
+
     def test_iexact(self):
         user = TestUser.objects.get(username__iexact="a")
         self.assertEqual("A", user.username)
 
         add_special_index(default_connection, IntegerModel, "integer_field", IExactIndexer(), "iexact")
         IntegerModel.objects.create(integer_field=1000)
         integer_model = IntegerModel.objects.get(integer_field__iexact=str(1000))
@@ -1623,14 +1665,52 @@
         TestFruit.objects.create(name="Apple", origin="New Zealand", color="Green")
         TestFruit.objects.create(name="Grape", origin="New Zealand", color="Red")
         nz_colours = TestFruit.objects.filter(
             origin="New Zealand"
         ).distinct("color").values_list("color", flat=True)
         self.assertEqual(sorted(nz_colours), ["Green", "Red"])
 
+    def test_values_list_on_distinct_with_limit(self):
+        TestFruit.objects.create(name="Kiwi", origin="New Zealand", color="Green")
+        TestFruit.objects.create(name="Apple", origin="New Zealand", color="Green")
+        TestFruit.objects.create(name="Grape", origin="New Zealand", color="Red")
+
+        nz_colours = TestFruit.objects.filter(
+            origin="New Zealand"
+        ).distinct("color").order_by('color').values_list("color", flat=True)[:1]
+
+        self.assertEqual(sorted(nz_colours), ["Green"])
+
+    def test_values_list_on_distinct_offset(self):
+        TestFruit.objects.create(name="Kiwi", origin="New Zealand", color="Green")
+        TestFruit.objects.create(name="Apple", origin="New Zealand", color="Green")
+        TestFruit.objects.create(name="Grape", origin="New Zealand", color="Red")
+
+        nz_colours = TestFruit.objects.filter(
+            origin="New Zealand"
+        ).distinct("color").order_by('color').values_list("color", flat=True)[1:]
+
+        self.assertEqual(sorted(nz_colours), ["Red"])
+
+    def test_values_list_on_distinct_limit_and_offset(self):
+        TestFruit.objects.create(name="Kiwi", origin="New Zealand", color="Green")
+        TestFruit.objects.create(name="Apple", origin="New Zealand", color="Green")
+        TestFruit.objects.create(name="Orange", origin="New Zealand", color="Orange")
+        TestFruit.objects.create(name="Orange2", origin="New Zealand", color="Orange")
+        TestFruit.objects.create(name="Grape", origin="New Zealand", color="Red")
+        TestFruit.objects.create(name="Apple2", origin="New Zealand", color="Red")
+        TestFruit.objects.create(name="Banana", origin="New Zealand", color="Yellow")
+        TestFruit.objects.create(name="Mango", origin="New Zealand", color="Yellow")
+
+        nz_colours = TestFruit.objects.filter(
+            origin="New Zealand"
+        ).distinct("color").order_by('color').values_list("color", flat=True)[1:3]
+
+        self.assertEqual(sorted(nz_colours), ["Orange", "Red"])
+
     def test_empty_key_lookups_work_correctly(self):
         t1 = TestFruit.objects.create(name="Kiwi", origin="New Zealand", color="Green")
         TestFruit.objects.create(name="Apple", origin="New Zealand", color="Green")
 
         self.assertEqual(
             t1,
             TestFruit.objects.exclude(name="Apple").exclude(name="").get(name="Kiwi")
@@ -1811,14 +1891,15 @@
         )
 
         self.assertEqual(
             0,
             len(SliceModel.objects.filter(field1__in=["test", "test2"])[2:])
         )
 
+    @datastore_only
     def test_slice_params_are_passed_to_query(self):
         for i in range(15):
             SliceModel.objects.create(field1=str(i))
 
         with sleuth.watch('google.cloud.datastore.query.Query.fetch') as Run:
             qs = SliceModel.objects.order_by("field1")[:5]
 
@@ -1862,27 +1943,16 @@
         except TestFruit.DoesNotExist:
             self.fail("Unable to retrieve fruit from the default namespace")
 
         self.assertEqual(1, TestFruit.objects.filter(name="Orange", color="Orange").count())
         self.assertEqual(0, TestFruit.objects.using("non_default_connection")
                          .filter(name="Orange", color="Orange").count())
 
-    def test_no_database_namespace_defaults_to_empty(self):
-        """
-            Test that creating an object without a namespace makes one that is
-            retrievable with just a kind and ID
-        """
-
-        TestFruit.objects.using("nonamespace").create(name="Apple", color="Red")
-        rpc = transaction._rpc("nonamespace")
-
-        key = rpc.key(TestFruit._meta.db_table, "Apple")
-        self.assertTrue(rpc.get(key))
-
     @skipIf("nonamespace" not in settings.DATABASES, "This test is designed for the Djangae testapp settings")
+    @datastore_only
     def test_move_objects_between_namespaces(self):
         objs = [
             TestFruit.objects.create(name="Banana", color="Black"),
             TestFruit.objects.create(name="Tomato", color="Red"),
         ]
         # First, check that these objects do not exist in the other namespace.
         # We check this in several ways to check that the namespace functionality works in the
@@ -1974,101 +2044,23 @@
         ).order_by("username")[1:2]
 
         self.assertEqual(len(qs), 1)
         self.assertItemsEqual([u2], qs)
 
 
 class UniqueQueryTest(TestCase):
-    def test_query_is_unique(self):
-        rpc = transaction._rpc(default_connection.alias)
-        query = rpc.query(kind="test_testuser")
-
-        # Query with no filter is not unique
-        self.assertFalse(query_is_unique(TestUser, query))
-
-        # Query with filter value set to None is not unique
-        query.add_filter('username', '=', None)
-        self.assertFalse(query_is_unique(TestUser, query))
-
-        # Query on unique field is unique
-        query = rpc.query(kind="test_testuser")
-        query.add_filter('username', '=', "randy")
-        self.assertTrue(query_is_unique(TestUser, query))
-
-        # Query on unique_together fields is unique
-        query = rpc.query(kind="test_testuser")
-        query.add_filter('first_name', '=', "Randy")
-        query.add_filter('second_name', '=', "Munroe")
-        self.assertTrue(query_is_unique(TestUser, query))
-
-        # Query on one unique_together field only is not unique
-        query = rpc.query(kind="test_testuser")
-        query.add_filter('second_name', '=', "Munroe")
-        self.assertFalse(query_is_unique(TestUser, query))
-
-        # Query on unique list field is unique only if filtering on one
-        # value only, as multiple values are interpreted as "one of"
-        query = rpc.query(kind="test_testuniquemodel")
-        query.add_filter('unique_list_field', '=', 'a')
-        query.add_filter('unique_list_field', '=', 'b')
-        self.assertFalse(query_is_unique(UniqueModel, query))
-
-        query = rpc.query(kind="test_testuniquemodel")
-        query.add_filter('unique_list_field', '=', 'b')
-        self.assertTrue(query_is_unique(UniqueModel, query))
-
-        # Query on pk field is unique
-        query = rpc.query(kind="test_testfruit")
-        # name is pk
-        query.add_filter('__key__', '=', rpc.key('test__testfruit', 'banana'))
-        self.assertTrue(query_is_unique(TestFruit, query))
-
     def test_entity_in_cache(self):
-        TestUser.objects.create(username="randy")
+        with transaction.atomic():
+            TestUser.objects.create(id=1, username="randy")
 
-        with sleuth.watch("google.cloud.datastore.query.Query.fetch") as fetch:
-            list(TestUser.objects.filter(username="randy"))
-            self.assertEqual(fetch.call_count, 0)
-
-    def test_entity_not_in_cache(self):
-        TestUser.objects.create(username="randy")
-
-        with sleuth.watch("google.cloud.datastore.query.Query.fetch") as fetch:
-            with sleuth.fake(
-                "gcloudc.db.backends.datastore.meta_queries.caching.get_from_cache",
-                return_value=None
-            ) as get_from_cache:
-                with sleuth.watch(
-                    "gcloudc.db.backends.datastore.meta_queries.caching.add_entities_to_cache"
-                ) as add_to_cache:
-                    list(TestUser.objects.filter(username="randy"))
-                    self.assertEqual(add_to_cache.call_count, 1)
-                    self.assertEqual(fetch.call_count, 1)
-                    self.assertEqual(get_from_cache.call_count, 1)
-
-    def test_keys_only_query_doesnt_cache(self):
-        TestUser.objects.create(username="randy")
-
-        with sleuth.watch("gcloudc.db.backends.datastore.meta_queries.caching.add_entities_to_cache") as add_to_cache:
-            list(TestUser.objects.filter(username="randy").only("pk"))
-            self.assertEqual(add_to_cache.call_count, 0)
-
-    def test_projection_query_doesnt_cache(self):
-        TestUser.objects.create(username="randy")
-
-        with sleuth.watch("gcloudc.db.backends.datastore.meta_queries.caching.add_entities_to_cache") as add_to_cache:
-            list(TestUser.objects.filter(username="randy").only("first_name"))
-            self.assertEqual(add_to_cache.call_count, 0)
+            with sleuth.watch("google.cloud.datastore.query.Query.fetch") as fetch:
+                list(TestUser.objects.filter(pk=1))
+                self.assertEqual(fetch.call_count, 0)
 
 
 class FieldConversionTests(TestCase):
     def test_uuid_field_handled(self):
         instance = UUIDTestModel.objects.create()
         self.assertTrue(isinstance(instance.uuid, uuid.UUID))
 
         instance.refresh_from_db()
         self.assertTrue(isinstance(instance.uuid, uuid.UUID))
-
-
-class TransactionFailedErrorTests(TestCase):
-    def test_transaction_failed_subclassing_generic_db_exception(self):
-        self.assertTrue(issubclass(transaction.TransactionFailedError, DatabaseError))
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/tests/test_db_fields.py` & `django-gcloud-connectors-1.2.0/gcloudc/tests/test_db_fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import pickle
 from datetime import timedelta
+import sleuth
 
 import django
 from django import forms
 from django.core.exceptions import ValidationError
 from django.db import (
     DatabaseError,
     connection,
     models,
 )
 from django.test import override_settings
 
-from gcloudc.db.decorators import disable_cache
+from gcloudc.db.backends.common.base.entity import Entity
+
+from gcloudc.db.models.fields.boolean import TrueOrNoneField
 from gcloudc.db.models.fields.charfields import (
     CharField,
     CharOrNoneField,
 )
 from gcloudc.db.models.fields.computed import (
     ComputedBooleanField,
     ComputedCharField,
@@ -30,15 +33,15 @@
 from gcloudc.db.models.fields.json import JSONField
 from gcloudc.db.models.fields.related import (
     GenericRelationField,
     RelatedListField,
     RelatedSetField,
 )
 
-from . import TestCase
+from . import TestCase, firestore_only, datastore_only
 from .models import (
     BasicTestModel,
     BinaryFieldModel,
     EmptyIndexesModel,
     IndexAllFieldsModel,
     IndexPrimaryKeyModel,
     IndexSelectedFieldsModel,
@@ -318,126 +321,151 @@
 
 
 class ModelWithNonNullableFieldAndDefaultValue(models.Model):
     some_field = models.IntegerField(null=False, default=1086)
 
 
 class NonIndexedModelFieldsTests(TestCase):
+
+    @datastore_only
     def test_long_textfield(self):
         """
         Assert long text fields are implicitly excluded from the datastore index.
+
+        This is datastore_only because Firestore indexes all fields.
+
+        There are "single-field index exemptions" but it's not clear how to use those.
+        Possible FIXME?
         """
         long_text = "A" * 1501
         instance = NonIndexedModel()
         instance.content = long_text
         instance.save()
 
         # grab the entity from the datastore directly
-        client = connection.connection.gclient
-        key = client.key(instance._meta.db_table, instance.pk, namespace=connection.namespace)
-        entity = client.get(key)
-
-        self.assertIn('content', entity.exclude_from_indexes)
+        key = connection.connection.new_key(instance._meta.db_table, instance.pk, namespace=connection.namespace)
+        entity = connection.connection.get(key)
+        self.assertIn('content', entity._properties_to_exclude_from_index)
 
+    @datastore_only
     def test_big_binaryfield(self):
         """
         Assert binary fields are implicitly excluded from the datastore index.
         """
         long_binary = ("A" * 1501).encode('utf-8')
         instance = NonIndexedModel()
         instance.binary = long_binary
         instance.save()
 
         # grab the entity from the datastore directly
-        client = connection.connection.gclient
+        client = connection.connection._client
         key = client.key(instance._meta.db_table, instance.pk, namespace=connection.namespace)
         entity = client.get(key)
 
         self.assertIn('binary', entity.exclude_from_indexes)
 
+    @firestore_only
+    def test_it_warns_it_is_not_supported_on_firestore(self):
+        """
+        Assert that we raise a warning when trying to exclude fields from the index
+        in firestore.
+        """
+        with sleuth.watch("gcloudc.db.backends.firestore.base.logger.warn") as mock_warn:
+            instance = NonIndexedModel()
+            instance.save()
+            self.assertTrue(mock_warn.called)
+            self.assertIn("Firestore doesn't support excluding fields from indexing", mock_warn.calls[0].args[0])
+
 
 class IndexFieldsModelTests(TestCase):
     """
     Tests to assert behaviour when configuring database indexes.
     """
 
+    @datastore_only
     def test_index_selected_fields(self):
         instance = IndexSelectedFieldsModel()
         instance.save()
 
         # grab the entity from the datastore directly
-        client = connection.connection.gclient
+        client = connection.connection._client
         key = client.key(instance._meta.db_table, instance.pk, namespace=connection.namespace)
         entity = client.get(key)
 
         self.assertNotIn('field1', entity.exclude_from_indexes)
         self.assertIn('field2', entity.exclude_from_indexes)
         # `field3` is a text field and so should not be indexed
         self.assertIn('field3', entity.exclude_from_indexes)
 
+    @datastore_only
     def test_index_all_fields_including_text_or_binary_field(self):
         instance = IndexAllFieldsModel()
         instance.save()
 
         # grab the entity from the datastore directly
-        client = connection.connection.gclient
+        client = connection.connection._client
         key = client.key(instance._meta.db_table, instance.pk, namespace=connection.namespace)
         entity = client.get(key)
 
         self.assertNotIn('field1', entity.exclude_from_indexes)
         self.assertNotIn('field2', entity.exclude_from_indexes)
         # Even though we selected `field3` and `field4` to be indexed in
         # the meta, the fields should not be indexed as they are text & binary fields
         self.assertIn('field3', entity.exclude_from_indexes)
         self.assertIn('field4', entity.exclude_from_indexes)
 
+    @datastore_only
     def test_primary_key_field_not_indexed(self):
         instance = IndexPrimaryKeyModel(field1="foo")
         instance.save()
 
         # grab the entity from the datastore directly
-        client = connection.connection.gclient
+        client = connection.connection._client
         key = client.key(instance._meta.db_table, instance.pk, namespace=connection.namespace)
         entity = client.get(key)
 
         # Even though we only selected `field2` to be indexed in
         # the meta, `field1` should still be indexed as it is a primary key
         self.assertNotIn('field1', entity.exclude_from_indexes)
         self.assertNotIn('field2', entity.exclude_from_indexes)
 
+    @datastore_only
     def test_all_fields_indexed_by_default_if_no_indexes_in_meta(self):
         instance = BasicTestModel(field1="foo", field2=1)
         instance.save()
 
         # grab the entity from the datastore directly
-        client = connection.connection.gclient
+        client = connection.connection._client
         key = client.key(instance._meta.db_table, instance.pk, namespace=connection.namespace)
         entity = client.get(key)
 
         self.assertNotIn('field1', entity.exclude_from_indexes)
         self.assertNotIn('field2', entity.exclude_from_indexes)
 
+    @datastore_only
     def test_single_property_query(self):
         IndexSelectedFieldsModel.objects.create(field1=1, field2="foo")
         # where `field1` is indexed
         self.assertTrue(IndexSelectedFieldsModel.objects.filter(field1=1).exists())
 
         # where `field2` is not indexed and so should raise an exception
         self.assertRaises(DatabaseError, list, IndexSelectedFieldsModel.objects.filter(field2="foo"))
 
+    @datastore_only
     def test_composite_index_query(self):
         IndexAllFieldsModel.objects.create(field1=1, field2="foo")
         # where `field1` and `field2` are indexed
         self.assertTrue(IndexAllFieldsModel.objects.filter(field1=1, field2="foo").exists())
 
         IndexSelectedFieldsModel.objects.create(field1=1, field2="foo")
         # where `field2` is not indexed and so should raise an exception
         # as a property cannot be excluded from composite indexes
         self.assertRaises(DatabaseError, list, IndexSelectedFieldsModel.objects.filter(field1=1, field2="foo"))
 
+    @datastore_only
     def test_projection_query(self):
         IndexSelectedFieldsModel.objects.create(
             field1=1, field2="foo", field3="hello world"
         )
         # where `field1` is indexed
         self.assertEqual(
             IndexSelectedFieldsModel.objects.values_list("field1", flat=True)[0], 1
@@ -445,67 +473,89 @@
         # where `field2` is not indexed and so should raise an exception
         self.assertRaises(
             DatabaseError,
             list,
             IndexSelectedFieldsModel.objects.values_list("field1", "field2"),
         )
 
+    @datastore_only
     def test_empty_indexes(self):
         instance = EmptyIndexesModel.objects.create(field1=1, field2="foo")
 
         # grab the entity from the datastore directly
-        client = connection.connection.gclient
+        client = connection.connection._client
         key = client.key(instance._meta.db_table, instance.pk, namespace=connection.namespace)
         entity = client.get(key)
 
         # despite passing an empty list to indexes we have a limitation where
         # that doesn't really work as you might expect due to the internals
         # of django we can't get around - so we fall back to indexing all fields
         self.assertNotIn('field1', entity.exclude_from_indexes)
         self.assertNotIn('field2', entity.exclude_from_indexes)
 
 
 # ModelWithNonNullableFieldAndDefaultValueTests verifies that we maintain same
 # behavior as Django with respect to a model field that is non-nullable with default value.
 class ModelWithNonNullableFieldAndDefaultValueTests(TestCase):
+    def _create_instance(self):
+        instance = ModelWithNonNullableFieldAndDefaultValue.objects.create(some_field=1)
+        client = connection.connection
 
-    # Note: needs to disable cache, otherwise refresh_from_db would hit the cache
-    # and not see changes made with the low-level sdk
-    @disable_cache()
-    def _create_instance_with_null_field_value(self):
+        instance_default_values = {x.attname: x.default for x in ModelWithNonNullableFieldAndDefaultValue._meta.fields
+                                   if x.default != django.db.models.fields.NOT_PROVIDED}
 
-        instance = ModelWithNonNullableFieldAndDefaultValue.objects.create(some_field=1)
-        client = connection.connection.gclient
-        entity = client.get(
-            client.key(
-                ModelWithNonNullableFieldAndDefaultValue._meta.db_table,
-                instance.pk,
-                namespace=connection.settings_dict.get("NAMESPACE", ""),
-            )
+        k = connection.connection.new_key(
+            ModelWithNonNullableFieldAndDefaultValue._meta.db_table,
+            instance.pk,
+            namespace=connection.namespace
         )
-        del entity["some_field"]
+
+        del instance_default_values["some_field"]
+
+        entity = Entity(k, properties=instance_default_values)
+
         client.put(entity)
 
         instance.refresh_from_db()
-
         return instance
 
     def test_none_in_db_reads_as_none_in_model(self):
-        instance = self._create_instance_with_null_field_value()
+        instance = self._create_instance()
         self.assertIsNone(instance.some_field)
 
     def test_none_in_model_saved_as_default(self):
-
-        instance = self._create_instance_with_null_field_value()
-
+        instance = self._create_instance()
+        instance.refresh_from_db()
         instance.save()
         instance.refresh_from_db()
 
         self.assertEqual(instance.some_field, 1086)
 
+    @datastore_only
+    def test_key_is_deleted_from_entity(self):
+        instance = ModelWithNonNullableFieldAndDefaultValue.objects.create(some_field=1)
+        client = connection.connection
+
+        instance_default_values = {x.attname: x.default for x in ModelWithNonNullableFieldAndDefaultValue._meta.fields
+                                   if x.default != django.db.models.fields.NOT_PROVIDED}
+
+        k = connection.connection.new_key(
+            ModelWithNonNullableFieldAndDefaultValue._meta.db_table,
+            instance.pk,
+            namespace=connection.namespace
+        )
+
+        del instance_default_values["some_field"]
+
+        entity = Entity(k, properties=instance_default_values)
+
+        client.put(entity)
+
+        instance.refresh_from_db()
+
 
 class NullableFieldModelTests(TestCase):
 
     def test_query_in_list_of_null_not_supported_in_django_32(self):
         """Before Django 3.2, this unit test's query used to return [1],
         but since the following change is no longer supported:
         https://code.djangoproject.com/ticket/31667"""
@@ -530,7 +580,30 @@
     def test_query_in_list_of_null_and_non_null(self):
         NullableFieldModel.objects.create(pk=1)
         NullableFieldModel.objects.create(pk=5, nullable=2)
         NullableFieldModel.objects.create(pk=6, nullable=3)
 
         results = NullableFieldModel.objects.filter(nullable__in=[None, 3])
         self.assertEqual({r.pk for r in results}, {1, 6})
+
+
+class TrueOrNoneModel(models.Model):
+    name = models.CharField(max_length=100)
+    true_or_null = TrueOrNoneField()
+
+    class Meta:
+        unique_together = [("name", "true_or_null")]
+
+
+class TrueOrNoneFieldTestCase(TestCase):
+    """ Tests for using the TrueOrNoneField. """
+
+    def test_converts_false_to_none(self):
+        obj = TrueOrNoneModel.objects.create(name="Gordon", true_or_null=False)
+        obj.refresh_from_db()
+        self.assertIsNone(obj.true_or_null)
+
+    def test_unique_together(self):
+        """ Any objects where true_or_null is None should be ignored by the unique_together check.
+        """
+        TrueOrNoneModel.objects.create(name="Gordon", true_or_null=True)
+        TrueOrNoneModel.objects.create(name="Gordon", true_or_null=None)
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/tests/test_delete.py` & `django-gcloud-connectors-1.2.0/gcloudc/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/tests/test_django_interactions.py` & `django-gcloud-connectors-1.2.0/gcloudc/tests/test_django_interactions.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/tests/test_excluding_pks.py` & `django-gcloud-connectors-1.2.0/gcloudc/tests/test_excluding_pks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,23 @@
-from django.db import models
+import uuid
+
+from django.db import models, transaction
 
 from . import TestCase
 
 
 class ExcludedPKModel(models.Model):
     name = models.CharField(max_length=30, primary_key=True)
     color = models.CharField(max_length=30)
 
 
+class UUIDPKModel(models.Model):
+    id = models.UUIDField(default=uuid.uuid4, primary_key=True)
+
+
 class ExcludingPKTests(TestCase):
     def test_exclude_pks_with_slice(self):
         for i in range(10):
             ExcludedPKModel.objects.create(name=str(i), color=str(i))
 
         to_exclude = [str(x) for x in list(range(5)) + list(range(15, 20))]
 
@@ -55,7 +61,20 @@
 
         self.assertEqual(
             ['Orange'],
             [e.pk for e in ExcludedPKModel.objects.filter(
                 color__in=["Red", "Orange"]
             ).exclude(pk__in=["Apple"])]
         )
+
+    def test_exclude_by_pk_inside_transaction(self):
+        ExcludedPKModel.objects.create(name="Apple", color="Red")
+        uuid1 = UUIDPKModel.objects.create()
+
+        with transaction.atomic():
+            obj = ExcludedPKModel.objects.get(pk="Apple")
+            self.assertEqual(ExcludedPKModel.objects.exclude(pk=obj.pk).count(), 0)
+            self.assertEqual(len(ExcludedPKModel.objects.exclude(pk=obj.pk)), 0)
+
+            uuid1 = UUIDPKModel.objects.get(pk=uuid1.pk)
+            self.assertEqual(UUIDPKModel.objects.exclude(pk=uuid1.pk).count(), 0)
+            self.assertEqual(len(UUIDPKModel.objects.exclude(pk=uuid1.pk)), 0)
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/tests/test_iterable_fields.py` & `django-gcloud-connectors-1.2.0/gcloudc/tests/test_iterable_fields.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import sleuth
 
 from django import forms
 from django.core import serializers
 from django.core.exceptions import (
     ImproperlyConfigured,
     ValidationError,
 )
@@ -16,16 +17,17 @@
     ListField,
     SetField,
 )
 from gcloudc.db.models.fields.related import (
     RelatedListField,
     RelatedSetField,
 )
+from gcloudc.forms.fields import CommaSeparatedListWidget, ListFormField
 
-from . import TestCase
+from . import TestCase, datastore_only, firestore_only
 
 
 class IterableIterableRelatedModel(models.Model):
     name = models.CharField(max_length=500)
 
     def __str__(self):
         return "%s:%s" % (self.pk, self.name)
@@ -49,14 +51,15 @@
 class IterableFieldModel(models.Model):
     set_field = SetField(models.CharField(max_length=1))
     list_field = ListField(models.CharField(max_length=1))
     set_field_int = SetField(models.BigIntegerField(max_length=1))
     list_field_int = ListField(models.BigIntegerField(max_length=1))
     set_field_dt = SetField(models.DateTimeField())
     list_field_dt = ListField(models.DateTimeField())
+    index = models.IntegerField(null=True)
 
     class Meta:
         app_label = "gcloudc"
 
 
 class IterableFieldTests(TestCase):
     def test_filtering_on_iterable_fields(self):
@@ -139,19 +142,19 @@
         qry = IterableFieldModel.objects.filter(set_field__overlap=set(["A", "B"]))
         self.assertEqual(sorted(x.pk for x in qry), sorted([list1.pk, list2.pk]))
         qry = IterableFieldModel.objects.filter(set_field__overlap=["H"])
         self.assertEqual(sorted(x.pk for x in qry), [list2.pk])
 
         # Filtering using two __overlap filters, applied one after the other
         qry = IterableFieldModel.objects.filter(
-                **{"list_field__overlap": ["A"]}
+                **{"list_field__overlap": ["D", "H"]}
             ).filter(
-                **{"list_field__overlap": ["J"]}
+                **{"list_field__overlap": ["A"]}
             )
-        self.assertEqual(list(qry), [list2])
+        self.assertItemsEqual(list(qry), [list1, list2])
 
         # Filtering with combination of __contains and __overlap filters, in either order.
         qry = IterableFieldModel.objects.filter(
                 **{"list_field__contains": ["A", "D"]}
             ).filter(
                 **{"list_field__overlap": ["B", "J"]}
             )
@@ -204,14 +207,117 @@
             IterableFieldModel.objects
             .filter(list_field__contains='A')
             .filter(list_field__contains='B')
             .filter(pk__in=[A.pk, AB.pk])
         )
         self.assertEqual(set(qry), {AB})
 
+    @datastore_only
+    def test_filtering_multiple_contains_iterable(self):
+        """
+        This is a copy of test_filtering_multiple_contains_iterable_fs, but checks we raise a warning
+        when appropriate on firestore.
+        """
+        A = IterableFieldModel.objects.create(list_field=["A"], set_field=set(["A"]), index=1)
+        AB = IterableFieldModel.objects.create(list_field=["A"], set_field=set(["B"]), index=2)
+        ABAB = IterableFieldModel.objects.create(list_field=["A", "B"], set_field=set(["A", "B"]), index=3)
+        ABCABC = IterableFieldModel.objects.create(list_field=["A", "B", "C"], set_field=set(["A", "B", "C"]), index=4)
+
+        qry = (
+            IterableFieldModel.objects
+            .filter(list_field__contains=['A'])
+        )
+
+        self.assertEqual(set(qry), {A, AB, ABAB, ABCABC})
+
+        qry = (
+            IterableFieldModel.objects
+            .filter(list_field__contains=['A'])
+            .order_by('index')
+            [1:3]
+        )
+
+        self.assertEqual(set(qry), {AB, ABAB})
+
+        qry = (
+            IterableFieldModel.objects
+            .filter(list_field__contains=['A'])
+            .filter(set_field__contains=['B'])
+        )
+
+        self.assertEqual(set(qry), {AB, ABAB, ABCABC})
+
+        qry = (
+            IterableFieldModel.objects
+            .filter(list_field__contains=['A'])
+            .filter(set_field__contains=['B'])
+            .order_by('index')
+            [1:3]
+        )
+
+        self.assertEqual(set(qry), {ABAB, ABCABC})
+
+    @firestore_only
+    def test_filtering_multiple_contains_iterable_fs(self):
+        """
+        This is a copy of test_filtering_multiple_contains_iterable_fs, but checks we raise a warning
+        when appropriate on firestore.
+        """
+        A = IterableFieldModel.objects.create(list_field=["A"], set_field=set(["A"]), index=1)
+        AB = IterableFieldModel.objects.create(list_field=["A"], set_field=set(["B"]), index=2)
+        ABAB = IterableFieldModel.objects.create(list_field=["A", "B"], set_field=set(["A", "B"]), index=3)
+        ABCABC = IterableFieldModel.objects.create(list_field=["A", "B", "C"], set_field=set(["A", "B", "C"]), index=4)
+
+        with sleuth.watch("gcloudc.db.backends.firestore.base.logger.warn") as mock_warn:
+            # No need for in memory pagination if we have a single array filter.
+            qry = (
+                IterableFieldModel.objects
+                .filter(list_field__contains=['A'])
+            )
+
+            self.assertEqual(set(qry), {A, AB, ABAB, ABCABC})
+            self.assertFalse(mock_warn.called)
+
+        with sleuth.watch("gcloudc.db.backends.firestore.base.logger.warn") as mock_warn:
+            # No need for in memory pagination if we have a single array filter (eben if we have an offset
+            # and limit.
+            qry = (
+                IterableFieldModel.objects
+                .filter(list_field__contains=['A'])
+                .order_by('index')
+                [1:3]
+            )
+
+            self.assertEqual(set(qry), {AB, ABAB})
+            self.assertFalse(mock_warn.called)
+
+        with sleuth.watch("gcloudc.db.backends.firestore.base.logger.warn") as mock_warn:
+            # We need in memory pagination if we have multiple array filters.
+            qry = (
+                IterableFieldModel.objects
+                .filter(list_field__contains=['A'])
+                .filter(set_field__contains=['B'])
+            )
+
+            self.assertEqual(set(qry), {AB, ABAB, ABCABC})
+            self.assertIn("This should be avoided", mock_warn.calls[0].args[0])
+
+        with sleuth.watch("gcloudc.db.backends.firestore.base.logger.warn") as mock_warn:
+            # In memory pagination works with offset and filter
+            qry = (
+                IterableFieldModel.objects
+                .filter(list_field__contains=['A'])
+                .filter(set_field__contains=['B'])
+                .order_by('index')
+                [1:3]
+            )
+
+            self.assertEqual(set(qry), {ABAB, ABCABC})
+            self.assertIn("This should be avoided", mock_warn.calls[0].args[0])
+
     def test_list_field(self):
         instance = IterableFieldModel.objects.create()
         self.assertEqual([], instance.list_field)
         instance.list_field.append("One")
         self.assertEqual(["One"], instance.list_field)
         instance.save()
 
@@ -221,28 +327,46 @@
         self.assertEqual(["One"], instance.list_field)
 
         results = IterableFieldModel.objects.filter(list_field__contains=["One"])
         self.assertEqual([instance], list(results))
 
         self.assertEqual([1, 2], ListField(models.IntegerField).to_python("[1, 2]"))
 
+    def test_list_field_multiple_contains_iterable(self):
+        instance = IterableFieldModel.objects.create()
+        self.assertEqual([], instance.list_field)
+        instance.list_field.append("One")
+        self.assertEqual(["One"], instance.list_field)
+        instance.save()
+
+        self.assertEqual(["One"], instance.list_field)
+
+        instance = IterableFieldModel.objects.get(pk=instance.pk)
+        self.assertEqual(["One"], instance.list_field)
+
+        results = IterableFieldModel.objects.filter(list_field__contains=["One"])
+        self.assertEqual([instance], list(results))
+
+        self.assertEqual([1, 2], ListField(models.IntegerField).to_python("[1, 2]"))
+
     def test_set_field(self):
         instance = IterableFieldModel.objects.create()
         self.assertEqual(set(), instance.set_field)
         instance.set_field.add("One")
         self.assertEqual(set(["One"]), instance.set_field)
         instance.save()
 
         self.assertEqual(set(["One"]), instance.set_field)
 
         instance = IterableFieldModel.objects.get(pk=instance.pk)
         self.assertEqual(set(["One"]), instance.set_field)
 
         self.assertEqual({1, 2}, SetField(models.IntegerField).to_python("[1, 2]"))
 
+    @datastore_only
     def test_empty_list_queryable_with_is_null(self):
         instance = IterableFieldModel.objects.create()
 
         self.assertTrue(IterableFieldModel.objects.filter(set_field__isempty=True).exists())
 
         instance.set_field.add(1)
         instance.save()
@@ -286,24 +410,61 @@
         self.assertEqual("['bar']", instance._meta.get_field("list_field").value_to_string(instance))
         self.assertEqual("[123]", instance._meta.get_field("set_field_int").value_to_string(instance))
         self.assertEqual("[456]", instance._meta.get_field("list_field_int").value_to_string(instance))
         self.assertEqual("['2017-01-01T12:00:00']", instance._meta.get_field("set_field_dt").value_to_string(instance))
         self.assertEqual("['2017-01-01T12:00:00']", instance._meta.get_field("list_field_dt").value_to_string(instance))
 
     def test_saving_forms(self):
-        class TestForm(forms.ModelForm):
+        class TextareaForm(forms.ModelForm):
             class Meta:
                 model = IterableFieldModel
                 fields = ("set_field", "list_field")
 
-        post_data = {"set_field": ["1", "2"], "list_field": ["1", "2"]}
+        class TextInputForm(forms.ModelForm):
+            set_field = ListFormField(widget=CommaSeparatedListWidget())
+            list_field = ListFormField(widget=CommaSeparatedListWidget())
 
-        form = TestForm(post_data)
-        self.assertTrue(form.is_valid())
-        self.assertTrue(form.save())
+            class Meta:
+                model = IterableFieldModel
+                fields = ("set_field", "list_field")
+
+        for form_class, post_data, expected_values in [
+            (
+                TextareaForm,
+                # Passing the data in its pre-formatted state
+                {"set_field": ["1", "2"], "list_field": ["1", "2"]},
+                {"set_field": {"1", "2"}, "list_field": ["1", "2"]}
+            ),
+            (
+                TextareaForm,
+                # Passing the data as it would be submitted from the form using the widget
+                {"set_field": "A\nB", "list_field": "a\nb"},
+                {"set_field": {"A", "B"}, "list_field": ["a", "b"]}
+            ),
+            (
+                TextInputForm,
+                # Passing the data in its pre-formatted state
+                {"set_field": ["1", "2"], "list_field": ["1", "2"]},
+                {"set_field": {"1", "2"}, "list_field": ["1", "2"]}
+            ),
+            (
+                TextInputForm,
+                # Passing the data as it would be submitted from the form using the widget
+                {"set_field": "A,B", "list_field": "a,b"},
+                {"set_field": {"A", "B"}, "list_field": ["a", "b"]}
+            ),
+        ]:
+            form = form_class(post_data)
+            self.assertTrue(
+                form.is_valid(),
+                f"{form_class.__name__} failed for values {post_data}. {form.errors!r}"
+            )
+            obj = form.save()
+            for field_name, expected in expected_values.items():
+                self.assertEqual(getattr(obj, field_name), expected)
 
     def test_cannot_have_min_length_and_blank(self):
         """ Having min_length=X, blank=True doesn't make any sense, especially when you consider
             that django will skip the min_length check when the value (list/set)is empty.
         """
         self.assertRaises(ImproperlyConfigured, ListField, CharField(max_length=100), min_length=1, blank=True)
         self.assertRaises(ImproperlyConfigured, SetField, CharField(max_length=100), min_length=1, blank=True)
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/tests/test_json_field.py` & `django-gcloud-connectors-1.2.0/gcloudc/tests/test_json_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,39 +3,40 @@
 from django.db import (
     connection,
     models,
 )
 from gcloudc.db.models.fields.json import JSONField
 from google.cloud.datastore.entity import Entity
 
-from . import TestCase
+from . import TestCase, datastore_only
 
 
 class JSONFieldModel(models.Model):
     json_field = JSONField(use_ordered_dict=True, blank=True)
 
 
 class JSONFieldWithDefaultModel(models.Model):
     json_field = JSONField(use_ordered_dict=True)
 
 
 class JSONFieldModelTests(TestCase):
+    @datastore_only
     def test_invalid_data_in_datastore_doesnt_throw_an_error(self):
         """
             If invalid data is found while reading the entity data, then
             we should silently ignore the error and just return the data as-is
             rather than converting to list/dict.
             The reason is that if we blow up on load, then there's no way to load the
             entity (in Django) to repair the data. This is also consistent with the behaviour
             of Django when (for example) you load a NULL from the database into a field that is
             non-nullable. The field value will still be None when read.
         """
         bool(JSONFieldModel.objects.exists())  # Force a connection (Django might not have made one yet)
 
-        client = connection.connection.gclient
+        client = connection.connection._client
         entity = Entity(
             client.key(JSONFieldModel._meta.db_table, 1, namespace=connection.settings_dict["NAMESPACE"])
         )
         entity["json_field"] = "bananas"
         client.put(entity)
 
         instance = JSONFieldModel.objects.get(pk=1)
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/tests/test_operations.py` & `django-gcloud-connectors-1.2.0/gcloudc/tests/test_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class OperationsTests(TestCase):
 
     def test_bulk_batch_size_override(self):
 
         with sleuth.watch(
-            "gcloudc.db.backends.datastore.commands.InsertCommand.__init__"
+            "gcloudc.db.backends.common.commands.InsertCommand.__init__"
         ) as bbs:
 
             try:
                 original = settings.DATABASES["default"].get("OPTIONS", {})
                 settings.DATABASES["default"]["OPTIONS"] = {
                     'BULK_BATCH_SIZE': 25
                 }
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/tests/test_related_fields.py` & `django-gcloud-connectors-1.2.0/gcloudc/tests/test_related_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,19 +207,17 @@
         result = list(thing.related_list.values_list("pk", "name"))
         self.assertEqual(result, [(a.pk, "A"), (b.pk, "B")])
 
     def test_indexing_doesnt_over_fetch(self):
         a, b = ISOther.objects.create(), ISOther.objects.create()
         thing = ISModel.objects.create(related_list_ids=[a.pk, b.pk])
 
-        with sleuth.watch("gcloudc.db.backends.datastore.meta_queries.QueryByKeys.__init__") as get:
+        with sleuth.watch("gcloudc.db.backends.common.base.query.ORQuery.push_query") as get:
             thing.related_list.all()[0]
-
             self.assertEqual(1, get.call_count)
-            self.assertEqual(1, len(get.calls[0].args[3]))
 
     def test_can_update_related_field_from_form(self):
         related = ISOther.objects.create()
         thing = ISModel.objects.create(related_list=[related])
         before_list = thing.related_list
         thing.related_list.field.save_form_data(thing, [])
         self.assertNotEqual(before_list.all(), thing.related_list.all())
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/tests/test_transaction_hooks.py` & `django-gcloud-connectors-1.2.0/gcloudc/tests/test_transaction_hooks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from django.db import connection
-from gcloudc.db import transaction
+from django.db import transaction
 from django.test import TransactionTestCase, skipUnlessDBFeature
 
 from .models import Thing
 
 
 class ForcedError(Exception):
     pass
@@ -33,40 +33,14 @@
     def assertDone(self, nums):
         self.assertNotified(nums)
         self.assertEqual(sorted(t.num for t in Thing.objects.all()), sorted(nums))
 
     def assertNotified(self, nums):
         self.assertEqual(self.notified, nums)
 
-    def test_independent_transactions(self):
-        with transaction.atomic():
-            self.do(1)
-
-            with transaction.atomic(independent=True):
-                self.do(2)
-
-            self.assertDone([2])
-
-        self.assertDone([2, 1])
-
-    def test_independent_transaction_rollback(self):
-        with transaction.atomic():
-            self.do(1)
-
-            try:
-                with transaction.atomic(independent=True):
-                    self.do(2)
-                    raise ForcedError()
-            except ForcedError:
-                pass
-
-            self.assertDone([])
-
-        self.assertDone([1])
-
     def test_executes_immediately_if_no_transaction(self):
         self.do(1)
         self.assertDone([1])
 
     def test_delays_execution_until_after_transaction_commit(self):
         with transaction.atomic():
             self.do(1)
@@ -99,27 +73,14 @@
                     self.do(1)
                 raise ForcedError()
         except ForcedError:
             pass
 
         self.assertDone([])
 
-    def test_inner_savepoint_rolled_back_with_outer(self):
-        with transaction.atomic():
-            try:
-                with transaction.atomic(independent=True):
-                    with transaction.atomic():
-                        self.do(1)
-                    raise ForcedError()
-            except ForcedError:
-                pass
-            self.do(2)
-
-        self.assertDone([2])
-
     def test_runs_hooks_in_order_registered(self):
         with transaction.atomic():
             self.do(1)
             with transaction.atomic():
                 self.do(2)
             self.do(3)
 
@@ -168,14 +129,16 @@
 
         with transaction.atomic():
             self.do(1)
 
         self.assertDone([1])
 
     def test_db_query_in_hook(self):
+        self.assertFalse(Thing.objects.all())
+
         with transaction.atomic():
             Thing.objects.create(num=1)
             transaction.on_commit(
                 lambda: [self.notify(t.num) for t in Thing.objects.all()]
             )
 
         self.assertDone([1])
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/tests/test_unique_constraints.py` & `django-gcloud-connectors-1.2.0/gcloudc/tests/test_unique_constraints.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import concurrent.futures
 from unittest import skip
 
 import sleuth
 from django.db import connection
 from django.db.models import Model
 from django.db.utils import IntegrityError
-from gcloudc.db import transaction
+from django.db import transaction
 
-from gcloudc.db.backends.datastore.transaction import TransactionFailedError
 from gcloudc.db.models.fields.charfields import CharField
+from gcloudc.db.backends.common.base.dbapi import TransactionFailedError
+
 
 from . import TestCase
 from .models import (
     NullableUniqueTogether,
     TestUser,
     TestUserTwo,
 )
@@ -111,16 +112,16 @@
     def test_error_on_update_does_not_change_entity(self):
         """
         Assert that when there is an error / exception raised as part of the
         update command, the entity is rolled back to its originial state.
         """
         user = TestUserTwo.objects.create(username="AshtonGateEight")
 
-        with sleuth.detonate("gcloudc.db.backends.datastore.transaction.Transaction.put", TransactionFailedError):
-            with self.assertRaises(TransactionFailedError):
+        with sleuth.detonate("gcloudc.db.backends.common.base.connection.Connection.put", TransactionFailedError):
+            with self.assertRaises(IntegrityError):
                 user.username = "Red Army"
                 user.save()
 
         user.refresh_from_db()
         self.assertEqual(user.username, "AshtonGateEight")
 
     def test_bulk_update(self):
@@ -191,42 +192,93 @@
 
         user_one.refresh_from_db()
         user_two.refresh_from_db()
 
         self.assertEqual(user_one.first_name, "steve")
         self.assertEqual(user_two.first_name, "joe")
 
+    @skip("This test fails sporadically - hopefully it's an emulator issue that will be fixed in an update")  # noqa
     def test_multithread_unique(self):
         """
         Ensure that with multiple insert in parallell, only one is accepted
         """
-        # Keeping this number large, to increase the chance it will actually fail if there is
-        # contention (otherwise it'd be the same as the "serial" example)
+        # Keeping this number large, to increase the chance it will actually fail if
+        # there is contention (otherwise it'd be the same as the "serial" example)
         concurrent_writes = 10
 
         def create_user():
             TestUserTwo.objects.create(username="contentious")
 
         futures = []
 
-        with concurrent.futures.ThreadPoolExecutor(max_workers=concurrent_writes) as executor:
+        with concurrent.futures.ThreadPoolExecutor(
+            max_workers=concurrent_writes
+        ) as executor:
             for _ in range(concurrent_writes):
                 futures.append(executor.submit(create_user))
 
         concurrent.futures.wait(futures)
 
         futures_exceptions = [
-            future.exception()
-            for future in futures
-            if future.exception() is not None
+            future.exception() for future in futures if future.exception() is not None
         ]
 
         self.assertEqual(len(futures_exceptions), concurrent_writes - 1)
         self.assertEqual(TestUserTwo.objects.count(), 1)
 
+    @skip("This test is not really testing gcloudc, but the datastore emulator.")
+    def test_multithread_unique_with_sdk(self):
+        from google.cloud import datastore
+        import requests
+        import os
+
+        def get_new_client():
+            return datastore.Client(
+                project=os.environ.get("GCLOUDC_PROJECT_ID", "test"),
+                namespace=None,
+                _http=requests.Session,
+            )
+
+        def read_then_write():
+            client = get_new_client()
+            kind = "WithFakeUniqueModel"
+            query = client.query(kind=kind)
+            with client.transaction():
+                res = query.add_filter("username", "=", "barbero").fetch()
+                if len(list(res)) > 0:
+                    raise IntegrityError("Nopes")
+
+                key = client.key(kind)
+                new_item = datastore.Entity(key)
+                new_item["username"] = "barbero"
+                client.put(new_item)
+
+        concurrent_writes = 500
+
+        futures = []
+        print(
+            os.environ.get("GCLOUDC_PROJECT_ID", "test"),
+        )
+        with concurrent.futures.ThreadPoolExecutor(
+            max_workers=concurrent_writes
+        ) as executor:
+            for _ in range(concurrent_writes):
+                futures.append(executor.submit(read_then_write))
+
+        concurrent.futures.wait(futures)
+
+        futures_exceptions = [
+            future.exception() for future in futures if future.exception() is not None
+        ]
+
+        if len(futures_exceptions) != concurrent_writes - 1:
+            print(futures_exceptions[0])
+
+        self.assertEqual(len(futures_exceptions), concurrent_writes - 1)
+
     # see https://github.com/googleapis/google-cloud-python/issues/9921
     @skip("This test should (probably) not fail once the emulator bug is fixed")
     def test_500_limit(self):
         # TODO: datastore emulator seems to fail at the old 25 limit, update
         # this test once emulator issue is addressed
         for i in range(25):
             username = "stevep_{}".format(i)
@@ -259,28 +311,28 @@
         Assert that there is currently a practical limitation when deleting multi
         entities, based on a combination of the unique markers per model
         and transaction limit of touching 500 entities.
         """
         TestUserTwo.objects.create(username="Mickey Bell")
         TestUserTwo.objects.create(username="Tony Thorpe")
 
-        with sleuth.switch("gcloudc.db.backends.datastore.transaction.TRANSACTION_ENTITY_LIMIT", 1):
+        with sleuth.fake("gcloudc.db.backends.common.base.connection.Wrapper.TRANSACTION_ENTITY_LIMIT", 1):
             with self.assertRaises(Exception):
                 TestUserTwo.objects.all().delete()
 
     def test_delete_entity_fails(self):
         """
         Assert that if the entity delete operation fails, the user is not deleted.
         """
         user = TestUserTwo.objects.create(username="Mickey Bell")
 
         with sleuth.detonate(
-            "gcloudc.db.backends.datastore.commands.remove_entities_from_cache_by_key", TransactionFailedError
+            "gcloudc.db.backends.common.base.connection.Connection.delete", TransactionFailedError
         ):
-            with self.assertRaises(TransactionFailedError):
+            with self.assertRaises(IntegrityError):
                 user.delete()
 
         # the entity in question should not have been deleted, as error in the
         # transactions atomic block should revert all changes
         user.refresh_from_db()
 
     def test_polymodels_with_base_unique(self):
@@ -433,7 +485,27 @@
         Test creating an object, updating a non-unique field and re-saving it within a transaction
         does not raise a unique constraing error.
         """
         with transaction.atomic():
             user = TestUser.objects.create(username="tommyd", first_name="Tommy", second_name="Shelby")
             user.field2 = 'updated'
             user.save()
+
+
+class MultiDBUniqueConstraintsTestCase(TestCase):
+
+    databases = ["default", "non_default_connection"]
+
+    def test_constraints_are_separate_per_db(self):
+        """ A unique constraint should not be incorrectly enforced across objects in different DBs.
+        """
+        field_values = {"first_name": "Hailey", "second_name": "Williams"}
+        user1 = TestUser(**field_values)
+        user2 = TestUser(**field_values)
+        user1.save(using="default")
+        user2.save(using="non_default_connection")
+        # Should be able to save the same objects (with their PKs now set) twice
+        user1.save(using="default")
+        user2.save(using="non_default_connection")
+        # Test that our field values do actually violate the unique constraint
+        user3 = TestUser(**field_values)
+        self.assertRaises(IntegrityError, user3.save, using="default")
```

### Comparing `django-gcloud-connectors-1.1.0/gcloudc/utils.py` & `django-gcloud-connectors-1.2.0/gcloudc/utils.py`

 * *Files identical despite different names*

### Comparing `django-gcloud-connectors-1.1.0/setup.py` & `django-gcloud-connectors-1.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import os
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 NAME = 'django-gcloud-connectors'
 
-DESCRIPTION = 'A Django library for connecting to Google Cloud Datastore from Python 3 runtimes.'
+DESCRIPTION = 'A Django library for connecting to Google Cloud Datastore and Firestore from Python 3 runtimes.'
 URL = 'https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors'
 LONG_DESCRIPTION = open(os.path.join(os.path.dirname(__file__), 'README.md')).read()
 
 AUTHOR = "Potato London Ltd."
 AUTHOR_EMAIL = "mail@p.ota.to"
 
 if os.environ.get('CI_COMMIT_TAG'):
     VERSION = os.environ['CI_COMMIT_TAG']
 else:
-    VERSION = '1.0.1a'
+    VERSION = '1.2.0'
 
 setup(
     name=NAME,
     version=VERSION,
     packages=find_packages(),
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
@@ -32,17 +32,18 @@
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
     ],
     install_requires=[
-        'django>=3.2,<4.2',
+        'django>=3.2,<5.0',
         'pyyaml>=6.0.1,<6.1',
-        'google-cloud-datastore>=1.15.3',
+        'google-cloud-datastore>=2.19.0',
+        'google-cloud-firestore>=2.15.0',
         'pyuca==1.2',
     ],
     include_package_data=True,
     extras_require={
         'test': [
             "unittest-xml-reporting==3.2.0",
             "sleuth-mock==0.1"
```

### Comparing `django-gcloud-connectors-1.1.0/test/404.html` & `django-gcloud-connectors-1.2.0/test/404.html`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,18 @@
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="/google-cloud/django-gcloud-connectors/caching/">Caching</a>
                 </li>
               </ul>
               <ul>
+                <li class="toctree-l1"><a class="reference internal" href="/google-cloud/django-gcloud-connectors/firestore/">Firestore</a>
+                </li>
+              </ul>
+              <ul>
                 <li class="toctree-l1"><a class="reference internal" href="/google-cloud/django-gcloud-connectors/contributing/">Contributing & Testing</a>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="/google-cloud/django-gcloud-connectors/commercial_support/">Commercial Support</a>
                 </li>
               </ul>
```

#### html2text {}

```diff
@@ -3,14 +3,15 @@
     * _H_o_m_e
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _C_o_n_c_e_p_t_s_ _&_ _l_i_m_i_t_a_t_i_o_n_s
     * _F_i_e_l_d_s
     * _F_i_e_l_d_ _I_n_d_e_x_e_s
     * _T_r_a_n_s_a_c_t_i_o_n_s
     * _C_a_c_h_i_n_g
+    * _F_i_r_e_s_t_o_r_e
     * _C_o_n_t_r_i_b_u_t_i_n_g_ _&_ _T_e_s_t_i_n_g
     * _C_o_m_m_e_r_c_i_a_l_ _S_u_p_p_o_r_t
     * _W_o_r_k_ _w_i_t_h_ _u_s_!
 _D_j_a_n_g_o_ _G_c_l_o_u_d_ _C_o_n_n_e_c_t_o_r_s_ _D_o_c_u_m_e_n_t_a_t_i_o_n
 ===============================================================================
 ************ 440044 ************
 PPaaggee nnoott ffoouunndd
```

### Comparing `django-gcloud-connectors-1.1.0/test/caching/index.html` & `django-gcloud-connectors-1.2.0/test/installation/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
     <meta charset="utf-8" />
     <meta http-equiv="X-UA-Compatible" content="IE=edge" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><link rel="canonical" href="https://potato-oss.gitlab.io/google-cloud/django-gcloud-connectors/caching/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><link rel="canonical" href="https://potato-oss.gitlab.io/google-cloud/django-gcloud-connectors/installation/" />
       <link rel="shortcut icon" href="../img/favicon.ico" />
-    <title>Caching - Django Gcloud Connectors Documentation</title>
+    <title>Installation - Django Gcloud Connectors Documentation</title>
     <link rel="stylesheet" href="../css/theme.css" />
     <link rel="stylesheet" href="../css/theme_extra.css" />
         <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/styles/github.min.css" />
     
       <script>
         // Current page data
-        var mkdocs_page_name = "Caching";
-        var mkdocs_page_input_path = "caching.md";
-        var mkdocs_page_url = "/google-cloud/django-gcloud-connectors/caching/";
+        var mkdocs_page_name = "Installation";
+        var mkdocs_page_input_path = "installation.md";
+        var mkdocs_page_url = "/google-cloud/django-gcloud-connectors/installation/";
       </script>
     
     <!--[if lt IE 9]>
       <script src="../js/html5shiv.min.js"></script>
     <![endif]-->
       <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/highlight.min.js"></script>
       <script>hljs.highlightAll();</script> 
@@ -39,16 +39,20 @@
       </div>
 
       <div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="..">Home</a>
                 </li>
               </ul>
-              <ul>
-                <li class="toctree-l1"><a class="reference internal" href="../installation/">Installation</a>
+              <ul class="current">
+                <li class="toctree-l1 current"><a class="reference internal current" href="#">Installation</a>
+    <ul class="current">
+    <li class="toctree-l2"><a class="reference internal" href="#automatic-cloud-datastore-emulator-startup">Automatic Cloud Datastore Emulator startup</a>
+    </li>
+    </ul>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../concepts_limitations/">Concepts & limitations</a>
                 </li>
               </ul>
               <ul>
@@ -59,24 +63,20 @@
                 <li class="toctree-l1"><a class="reference internal" href="../field_indexes/">Field Indexes</a>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../transactions/">Transactions</a>
                 </li>
               </ul>
-              <ul class="current">
-                <li class="toctree-l1 current"><a class="reference internal current" href="./">Caching</a>
-    <ul class="current">
-    <li class="toctree-l2"><a class="reference internal" href="#refreshing-models">Refreshing Models</a>
-    </li>
-    <li class="toctree-l2"><a class="reference internal" href="#inside-transactions">Inside transactions</a>
-    </li>
-    <li class="toctree-l2"><a class="reference internal" href="#non-unique-queries">Non-unique queries</a>
-    </li>
-    </ul>
+              <ul>
+                <li class="toctree-l1"><a class="reference internal" href="../caching/">Caching</a>
+                </li>
+              </ul>
+              <ul>
+                <li class="toctree-l1"><a class="reference internal" href="../firestore/">Firestore</a>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../contributing/">Contributing & Testing</a>
                 </li>
               </ul>
               <ul>
@@ -97,84 +97,52 @@
           <a href="..">Django Gcloud Connectors Documentation</a>
         
       </nav>
       <div class="wy-nav-content">
         <div class="rst-content"><div role="navigation" aria-label="breadcrumbs navigation">
   <ul class="wy-breadcrumbs">
     <li><a href=".." class="icon icon-home" aria-label="Docs"></a></li>
-      <li class="breadcrumb-item active">Caching</li>
+      <li class="breadcrumb-item active">Installation</li>
     <li class="wy-breadcrumbs-aside">
-          <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/caching.md" class="icon icon-gitlab"> Edit on GitLab</a>
+          <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/installation.md" class="icon icon-gitlab"> Edit on GitLab</a>
     </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
             <div class="section" itemprop="articleBody">
               
-                <h1 id="caching">Caching</h1>
-<p>All models handled via the connector are, by default, cached in memory by:</p>
+                <h1 id="installation">Installation</h1>
+<p>The most common way to install <code>gcloudc</code> is to use it as part of <a href="https://potato-oss.gitlab.io/djangae/djangae/">Djangae</a>.</p>
+<p>You can also install it on its own with <code>pip install django-gcloud-connectors</code>.</p>
+<p>However you install it, you will need to set your <code>DATABASES</code> configuration in your Django settings module to look something like this:</p>
+<pre><code class="language-python">from djangae
+DATABASES = {
+    &quot;default&quot;: {
+        'ENGINE': 'gcloudc.db.backends.datastore',
+        'PROJECT': 'YOUR_GCP_PROJECT_NAME',  # You can use djangae.environment.project_id() here
+        'INDEXES_FILE': 'PATH_TO_A_FILE_FOR_SPECICAL_INDEXES',
+    }
+}
+</code></pre>
+<p>The possible engines you can choose are:</p>
 <ul>
-<li>Primary key</li>
-<li>Unique fields</li>
+<li><code>gcloudc.db.backends.firestore</code></li>
+<li><code>gcloudc.db.backends.datastore</code></li>
 </ul>
-<h2 id="refreshing-models">Refreshing Models</h2>
-<p>While in most scenario caching is good and you'll benefit from it, it does slightly
-change the semantics of <code>refresh_from_db</code>: this will effectively refresh from cache,
-not from the database.</p>
-<p>If you're using <code>refresh_from_db</code> simply to discard the unsaved changes you've made to
-a model and "reset" to the original state, that's ok.</p>
-<p>If instead, you need to absolutely make sure to get the latest value from the database
-then you can temporarily disable the cache with the <code>gcloudc.context_decorators.disable_cache</code>
-context manager:</p>
-<pre><code class="language-python">from gcloudc.context_decorators import disable_cache
-
-
-with disable_cache():
-    instance.refresh_from_db()
-</code></pre>
-<p>You can also disable the cache globally by setting <code>GCLOUDC_CACHE_ENABLED</code> to <code>False</code>.</p>
-<p><strong>Warning:</strong> if you disable the cache, you may have weird behaviour inside transactions.
-Read on!</p>
-<h2 id="inside-transactions">Inside transactions</h2>
-<p>The connectors cache is particularly useful inside transactions.
-In datastore transactions, any write done inside of it will note be "seen" until
-the transaction is committed, which would lead to scenario like this</p>
-<pre><code class="language-python">with transaction.atomic():
-    obj = Model.object.create(...)
-    ...
-    Model.object.get(pk=obj.pk) # &lt;-- raises Model.DoesNotExists
-</code></pre>
-<p>This is generally not what you want, but you'll only have to worry about it
-if you disable the cache.</p>
-<h2 id="non-unique-queries">Non-unique queries</h2>
-<p>Only "unique[^*]" queries are performed on the cache. Non-unique queries will
-still be performed on the underlying datastore instance.</p>
-<p>If, inside a transaction, you're performing a query on a kind that has been
-modified in that same transaction, the query won't see those changes.</p>
-<p>For example</p>
-<pre><code class="language-python">
-number = IntegerModel(value=1)
-number.save()
-
-with transaction.atomic():
-    number.value = 100
-    bigger_than_10 = IntegerModel.objects.filter(value__gt=10).count()
-    # bigger_than_10 == 0 here, the query didn't pick up the change outside the transaction
-</code></pre>
-<p>[^*]: By unique here we mean a query that will return either 1 or no result as a consequence
-of a unique constraint: this includes queries by primary key, query with an equality filter
-or a <code>unique=True</code> field or queries with equality filters on all fields for a <code>unique_together</code>
-constraint</p>
+<p>INDEXES_FILE is an absolute path to a yaml file that will be automatically generated. See [special_indexes.md] for more information.</p>
+<h2 id="automatic-cloud-datastore-emulator-startup">Automatic Cloud Datastore Emulator startup</h2>
+<p>gcloudc provides overrides for the <code>runserver</code> and <code>test</code> commands which
+start and stop a Cloud Datastore Emulator instance. To enable this functionality add <code>gcloudc.commands</code> <em>at the beginning</em> of your <code>INSTALLED_APPS</code> setting.</p>
               
             </div>
           </div><footer>
     <div class="rst-footer-buttons" role="navigation" aria-label="Footer Navigation">
-        <a href="../transactions/" class="btn btn-neutral float-left" title="Transactions"><span class="icon icon-circle-arrow-left"></span> Previous</a>
-        <a href="../contributing/" class="btn btn-neutral float-right" title="Contributing & Testing">Next <span class="icon icon-circle-arrow-right"></span></a>
+        <a href=".." class="btn btn-neutral float-left" title="Home"><span class="icon icon-circle-arrow-left"></span> Previous</a>
+        <a href="../concepts_limitations/" class="btn btn-neutral float-right" title="Concepts & limitations">Next <span class="icon icon-circle-arrow-right"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <!-- Copyright etc -->
   </div>
@@ -193,18 +161,18 @@
   <span class="rst-current-version" data-toggle="rst-current-version">
     
         <span>
           <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/" class="icon icon-gitlab" style="color: #fcfcfc"> GitLab</a>
         </span>
     
     
-      <span><a href="../transactions/" style="color: #fcfcfc">&laquo; Previous</a></span>
+      <span><a href=".." style="color: #fcfcfc">&laquo; Previous</a></span>
     
     
-      <span><a href="../contributing/" style="color: #fcfcfc">Next &raquo;</a></span>
+      <span><a href="../concepts_limitations/" style="color: #fcfcfc">Next &raquo;</a></span>
     
   </span>
 </div>
     <script src="../js/jquery-3.6.0.min.js"></script>
     <script>var base_url = "..";</script>
     <script src="../js/theme_extra.js"></script>
     <script src="../js/theme.js"></script>
```

#### html2text {}

```diff
@@ -1,74 +1,45 @@
 _D_j_a_n_g_o_ _G_c_l_o_u_d_ _C_o_n_n_e_c_t_o_r_s_ _D_o_c_u_m_e_n_t_a_t_i_o_n
 [q                   ]
     * _H_o_m_e
     * _I_n_s_t_a_l_l_a_t_i_o_n
+          o _A_u_t_o_m_a_t_i_c_ _C_l_o_u_d_ _D_a_t_a_s_t_o_r_e_ _E_m_u_l_a_t_o_r_ _s_t_a_r_t_u_p
     * _C_o_n_c_e_p_t_s_ _&_ _l_i_m_i_t_a_t_i_o_n_s
     * _F_i_e_l_d_s
     * _F_i_e_l_d_ _I_n_d_e_x_e_s
     * _T_r_a_n_s_a_c_t_i_o_n_s
     * _C_a_c_h_i_n_g
-          o _R_e_f_r_e_s_h_i_n_g_ _M_o_d_e_l_s
-          o _I_n_s_i_d_e_ _t_r_a_n_s_a_c_t_i_o_n_s
-          o _N_o_n_-_u_n_i_q_u_e_ _q_u_e_r_i_e_s
+    * _F_i_r_e_s_t_o_r_e
     * _C_o_n_t_r_i_b_u_t_i_n_g_ _&_ _T_e_s_t_i_n_g
     * _C_o_m_m_e_r_c_i_a_l_ _S_u_p_p_o_r_t
     * _W_o_r_k_ _w_i_t_h_ _u_s_!
 _D_j_a_n_g_o_ _G_c_l_o_u_d_ _C_o_n_n_e_c_t_o_r_s_ _D_o_c_u_m_e_n_t_a_t_i_o_n
-    * Caching
+    * Installation
     * _E_d_i_t_ _o_n_ _G_i_t_L_a_b
 ===============================================================================
-************ CCaacchhiinngg ************
-All models handled via the connector are, by default, cached in memory by:
-    * Primary key
-    * Unique fields
-********** RReeffrreesshhiinngg MMooddeellss **********
-While in most scenario caching is good and you'll benefit from it, it does
-slightly change the semantics of refresh_from_db: this will effectively refresh
-from cache, not from the database.
-If you're using refresh_from_db simply to discard the unsaved changes you've
-made to a model and "reset" to the original state, that's ok.
-If instead, you need to absolutely make sure to get the latest value from the
-database then you can temporarily disable the cache with the
-gcloudc.context_decorators.disable_cache context manager:
-from gcloudc.context_decorators import disable_cache
-
-
-with disable_cache():
-    instance.refresh_from_db()
-You can also disable the cache globally by setting GCLOUDC_CACHE_ENABLED to
-False.
-WWaarrnniinngg:: if you disable the cache, you may have weird behaviour inside
-transactions. Read on!
-********** IInnssiiddee ttrraannssaaccttiioonnss **********
-The connectors cache is particularly useful inside transactions. In datastore
-transactions, any write done inside of it will note be "seen" until the
-transaction is committed, which would lead to scenario like this
-with transaction.atomic():
-    obj = Model.object.create(...)
-    ...
-    Model.object.get(pk=obj.pk) # <-- raises Model.DoesNotExists
-This is generally not what you want, but you'll only have to worry about it if
-you disable the cache.
-********** NNoonn--uunniiqquuee qquueerriieess **********
-Only "unique[^*]" queries are performed on the cache. Non-unique queries will
-still be performed on the underlying datastore instance.
-If, inside a transaction, you're performing a query on a kind that has been
-modified in that same transaction, the query won't see those changes.
-For example
-
-number = IntegerModel(value=1)
-number.save()
-
-with transaction.atomic():
-    number.value = 100
-    bigger_than_10 = IntegerModel.objects.filter(value__gt=10).count()
-    # bigger_than_10 == 0 here, the query didn't pick up the change outside the
-transaction
-[^*]: By unique here we mean a query that will return either 1 or no result as
-a consequence of a unique constraint: this includes queries by primary key,
-query with an equality filter or a unique=True field or queries with equality
-filters on all fields for a unique_together constraint
+************ IInnssttaallllaattiioonn ************
+The most common way to install gcloudc is to use it as part of _D_j_a_n_g_a_e.
+You can also install it on its own with pip install django-gcloud-connectors.
+However you install it, you will need to set your DATABASES configuration in
+your Django settings module to look something like this:
+from djangae
+DATABASES = {
+    "default": {
+        'ENGINE': 'gcloudc.db.backends.datastore',
+        'PROJECT': 'YOUR_GCP_PROJECT_NAME',  # You can use
+djangae.environment.project_id() here
+        'INDEXES_FILE': 'PATH_TO_A_FILE_FOR_SPECICAL_INDEXES',
+    }
+}
+The possible engines you can choose are:
+    * gcloudc.db.backends.firestore
+    * gcloudc.db.backends.datastore
+INDEXES_FILE is an absolute path to a yaml file that will be automatically
+generated. See [special_indexes.md] for more information.
+********** AAuuttoommaattiicc CClloouudd DDaattaassttoorree EEmmuullaattoorr ssttaarrttuupp **********
+gcloudc provides overrides for the runserver and test commands which start and
+stop a Cloud Datastore Emulator instance. To enable this functionality add
+gcloudc.commands aatt tthhee bbeeggiinnnniinngg of your INSTALLED_APPS setting.
 _P_r_e_v_i_o_u_s _N_e_x_t
 ===============================================================================
 Built with _M_k_D_o_c_s using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
 _G_i_t_L_a_b _«_ _P_r_e_v_i_o_u_s _N_e_x_t_ _»
```

### Comparing `django-gcloud-connectors-1.1.0/test/commercial_support/index.html` & `django-gcloud-connectors-1.2.0/test/commercial_support/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -64,19 +64,23 @@
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../caching/">Caching</a>
                 </li>
               </ul>
               <ul>
+                <li class="toctree-l1"><a class="reference internal" href="../firestore/">Firestore</a>
+                </li>
+              </ul>
+              <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../contributing/">Contributing & Testing</a>
                 </li>
               </ul>
               <ul class="current">
-                <li class="toctree-l1 current"><a class="reference internal current" href="./">Commercial Support</a>
+                <li class="toctree-l1 current"><a class="reference internal current" href="#">Commercial Support</a>
     <ul class="current">
     </ul>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../work_with_potato/">Work with us!</a>
                 </li>
```

#### html2text {}

```diff
@@ -3,14 +3,15 @@
     * _H_o_m_e
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _C_o_n_c_e_p_t_s_ _&_ _l_i_m_i_t_a_t_i_o_n_s
     * _F_i_e_l_d_s
     * _F_i_e_l_d_ _I_n_d_e_x_e_s
     * _T_r_a_n_s_a_c_t_i_o_n_s
     * _C_a_c_h_i_n_g
+    * _F_i_r_e_s_t_o_r_e
     * _C_o_n_t_r_i_b_u_t_i_n_g_ _&_ _T_e_s_t_i_n_g
     * _C_o_m_m_e_r_c_i_a_l_ _S_u_p_p_o_r_t
     * _W_o_r_k_ _w_i_t_h_ _u_s_!
 _D_j_a_n_g_o_ _G_c_l_o_u_d_ _C_o_n_n_e_c_t_o_r_s_ _D_o_c_u_m_e_n_t_a_t_i_o_n
     * Commercial Support
     * _E_d_i_t_ _o_n_ _G_i_t_L_a_b
 ===============================================================================
```

### Comparing `django-gcloud-connectors-1.1.0/test/concepts_limitations/index.html` & `django-gcloud-connectors-1.2.0/test/concepts_limitations/index.html`

 * *Files 17% similar despite different names*

```diff
@@ -44,36 +44,16 @@
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../installation/">Installation</a>
                 </li>
               </ul>
               <ul class="current">
-                <li class="toctree-l1 current"><a class="reference internal current" href="./">Concepts & limitations</a>
+                <li class="toctree-l1 current"><a class="reference internal current" href="#">Concepts & limitations</a>
     <ul class="current">
-    <li class="toctree-l2"><a class="reference internal" href="#foreign-keys">Foreign Keys</a>
-    </li>
-    <li class="toctree-l2"><a class="reference internal" href="#many-to-many-relationships">Many-to-many relationships</a>
-    </li>
-    <li class="toctree-l2"><a class="reference internal" href="#migrations">Migrations</a>
-        <ul>
-    <li class="toctree-l3"><a class="reference internal" href="#deleting-fields">Deleting fields</a>
-    </li>
-    <li class="toctree-l3"><a class="reference internal" href="#making-new-fields-queryable">Making new fields queryable</a>
-    </li>
-        </ul>
-    </li>
-    <li class="toctree-l2"><a class="reference internal" href="#complex-queries">Complex queries</a>
-        <ul>
-    <li class="toctree-l3"><a class="reference internal" href="#inequalities">Inequalities</a>
-    </li>
-    <li class="toctree-l3"><a class="reference internal" href="#special-indexes">Special indexes</a>
-    </li>
-        </ul>
-    </li>
     </ul>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../fields/">Fields</a>
                 </li>
               </ul>
@@ -86,14 +66,18 @@
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../caching/">Caching</a>
                 </li>
               </ul>
               <ul>
+                <li class="toctree-l1"><a class="reference internal" href="../firestore/">Firestore</a>
+                </li>
+              </ul>
+              <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../contributing/">Contributing & Testing</a>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../commercial_support/">Commercial Support</a>
                 </li>
               </ul>
@@ -122,28 +106,27 @@
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
             <div class="section" itemprop="articleBody">
               
                 <h1 id="concepts-limitations">Concepts &amp; Limitations</h1>
+<h1 id="cloud-datastore">Cloud Datastore</h1>
 <p>It is <em>strongly recommended</em> that you read the Cloud Datastore API documentation before using this ORM backend. Understanding of the Datastore
 vs SQL will help avoid unexpected surprises!</p>
 <p>The Google Cloud Datastore is <em>not</em> your traditional SQL database, and for that reason the Datastore backend doesn't support
 all of the functionality of the Django ORM (although it supports the majority). Also, some things don't always work the way
 you'd expect. As the Datastore is a No-SQL database, anything relying on cross-table queries or aggregates is basically unsupported.</p>
 <p>Here are some of the limitations and differences:</p>
 <ul>
-<li>We ship specialised atomic() decorators, including support for "independent" transactions. See <a href="../transactions/">Transactions</a>.</li>
 <li>There is no support for savepoints, nested atomic() blocks are effectively a no-op</li>
-<li>Django's atomic() decorators WILL NOT WORK</li>
 <li>No support for select_related(), although prefetch_related() works</li>
 <li>No support for cross-table ordering</li>
 <li>Only up-to 500 entities can be read or written inside an atomic() block</li>
-<li>No support for aggregate queries</li>
+<li>No support for aggregate queries (yet)</li>
 <li>Queries can only contain a single inequality operation (gt, lt, lte, gte, isnull=False), and the resultset must be ordered by the field you're testing for inequality</li>
 </ul>
 <p>The advantage of course is that you can build your Django application for near-infinite scalability of data, and increased uptime.</p>
 <p>Further differences are discussed below.</p>
 <h2 id="foreign-keys">Foreign Keys</h2>
 <p>The Cloud Datastore doesn't have the concept of a foreign key <em>constraint</em>,
 so relations are not enforced at the database level in the same way that they would be on a classic SQL database,
@@ -189,43 +172,14 @@
 <p>The Cloud Datastore can only perform queries using an index. In other words, it won't do a table scan.
 As such, it can generally only perform queries which can be done by working its way through a single, ordered index.
 Therefore some types of queries are not possible, or can only be performed with additional trickery.</p>
 <h3 id="inequalities">Inequalities</h3>
 <p>Queries which contain multiple inequality filters, e.g. <code>.filter(field_a__gte=x, field_b__gte=y)</code> are not possible.
 Inequalities are any of <code>__gt</code>, <code>__lt</code>, <code>__lte</code>, <code>__gte</code>, <code>__isnull=False</code>.</p>
 <p>Additionally, if your query contains an inequality then it must be ordered by the field you're testing for inequality.</p>
-<h3 id="special-indexes">Special indexes</h3>
-<p>Queries which use the following filters cannot be performed directly on the Cloud Datastore:</p>
-<ul>
-<li><code>__iexact</code></li>
-<li><code>__contains</code></li>
-<li><code>__icontains</code></li>
-<li><code>__startswith</code></li>
-<li><code>__endswith</code></li>
-<li><code>__regex</code></li>
-<li><code>__iregex</code></li>
-<li><code>__date</code></li>
-<li><code>__iso_year</code></li>
-<li><code>__iso_week_day</code></li>
-<li><code>__quarter</code></li>
-<li><code>__year</code></li>
-<li><code>__month</code></li>
-<li><code>__day</code></li>
-<li><code>__week</code></li>
-<li><code>__week_day</code></li>
-<li><code>__hour</code></li>
-<li><code>__minute</code></li>
-<li><code>__second</code></li>
-<li><code>__time</code></li>
-</ul>
-<p>as they require inexact matching of field values (or parts of field values).
-But gcloudc <em>does</em> support many of them via its built-in "special indexes" system,
-which indexes the relevant parts/permutations of the field values to allow them to be queried directly via an index.</p>
-<p>To configure this you need to set the <code>"INDEXES_FILE"</code> in the <code>DATABASES</code> setting. See <a href="../installation/">Installation</a>.</p>
-<p>For queries of these types, you may also wish to explore the <a href="../fields/#computed-fields">computed fields</a>.</p>
               
             </div>
           </div><footer>
     <div class="rst-footer-buttons" role="navigation" aria-label="Footer Navigation">
         <a href="../installation/" class="btn btn-neutral float-left" title="Installation"><span class="icon icon-circle-arrow-left"></span> Previous</a>
         <a href="../fields/" class="btn btn-neutral float-right" title="Fields">Next <span class="icon icon-circle-arrow-right"></span></a>
     </div>
```

#### html2text {}

```diff
@@ -1,50 +1,41 @@
 _D_j_a_n_g_o_ _G_c_l_o_u_d_ _C_o_n_n_e_c_t_o_r_s_ _D_o_c_u_m_e_n_t_a_t_i_o_n
 [q                   ]
     * _H_o_m_e
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _C_o_n_c_e_p_t_s_ _&_ _l_i_m_i_t_a_t_i_o_n_s
-          o _F_o_r_e_i_g_n_ _K_e_y_s
-          o _M_a_n_y_-_t_o_-_m_a_n_y_ _r_e_l_a_t_i_o_n_s_h_i_p_s
-          o _M_i_g_r_a_t_i_o_n_s
-                # _D_e_l_e_t_i_n_g_ _f_i_e_l_d_s
-                # _M_a_k_i_n_g_ _n_e_w_ _f_i_e_l_d_s_ _q_u_e_r_y_a_b_l_e
-          o _C_o_m_p_l_e_x_ _q_u_e_r_i_e_s
-                # _I_n_e_q_u_a_l_i_t_i_e_s
-                # _S_p_e_c_i_a_l_ _i_n_d_e_x_e_s
     * _F_i_e_l_d_s
     * _F_i_e_l_d_ _I_n_d_e_x_e_s
     * _T_r_a_n_s_a_c_t_i_o_n_s
     * _C_a_c_h_i_n_g
+    * _F_i_r_e_s_t_o_r_e
     * _C_o_n_t_r_i_b_u_t_i_n_g_ _&_ _T_e_s_t_i_n_g
     * _C_o_m_m_e_r_c_i_a_l_ _S_u_p_p_o_r_t
     * _W_o_r_k_ _w_i_t_h_ _u_s_!
 _D_j_a_n_g_o_ _G_c_l_o_u_d_ _C_o_n_n_e_c_t_o_r_s_ _D_o_c_u_m_e_n_t_a_t_i_o_n
     * Concepts & limitations
     * _E_d_i_t_ _o_n_ _G_i_t_L_a_b
 ===============================================================================
 ************ CCoonncceeppttss && LLiimmiittaattiioonnss ************
+************ CClloouudd DDaattaassttoorree ************
 It is ssttrroonnggllyy rreeccoommmmeennddeedd that you read the Cloud Datastore API documentation
 before using this ORM backend. Understanding of the Datastore vs SQL will help
 avoid unexpected surprises!
 The Google Cloud Datastore is nnoott your traditional SQL database, and for that
 reason the Datastore backend doesn't support all of the functionality of the
 Django ORM (although it supports the majority). Also, some things don't always
 work the way you'd expect. As the Datastore is a No-SQL database, anything
 relying on cross-table queries or aggregates is basically unsupported.
 Here are some of the limitations and differences:
-    * We ship specialised atomic() decorators, including support for
-      "independent" transactions. See _T_r_a_n_s_a_c_t_i_o_n_s.
     * There is no support for savepoints, nested atomic() blocks are
       effectively a no-op
-    * Django's atomic() decorators WILL NOT WORK
     * No support for select_related(), although prefetch_related() works
     * No support for cross-table ordering
     * Only up-to 500 entities can be read or written inside an atomic() block
-    * No support for aggregate queries
+    * No support for aggregate queries (yet)
     * Queries can only contain a single inequality operation (gt, lt, lte, gte,
       isnull=False), and the resultset must be ordered by the field you're
       testing for inequality
 The advantage of course is that you can build your Django application for near-
 infinite scalability of data, and increased uptime.
 Further differences are discussed below.
 ********** FFoorreeiiggnn KKeeyyss **********
@@ -106,41 +97,11 @@
 trickery.
 ******** IInneeqquuaalliittiieess ********
 Queries which contain multiple inequality filters, e.g. .filter(field_a__gte=x,
 field_b__gte=y) are not possible. Inequalities are any of __gt, __lt, __lte,
 __gte, __isnull=False.
 Additionally, if your query contains an inequality then it must be ordered by
 the field you're testing for inequality.
-******** SSppeecciiaall iinnddeexxeess ********
-Queries which use the following filters cannot be performed directly on the
-Cloud Datastore:
-    * __iexact
-    * __contains
-    * __icontains
-    * __startswith
-    * __endswith
-    * __regex
-    * __iregex
-    * __date
-    * __iso_year
-    * __iso_week_day
-    * __quarter
-    * __year
-    * __month
-    * __day
-    * __week
-    * __week_day
-    * __hour
-    * __minute
-    * __second
-    * __time
-as they require inexact matching of field values (or parts of field values).
-But gcloudc ddooeess support many of them via its built-in "special indexes"
-system, which indexes the relevant parts/permutations of the field values to
-allow them to be queried directly via an index.
-To configure this you need to set the "INDEXES_FILE" in the DATABASES setting.
-See _I_n_s_t_a_l_l_a_t_i_o_n.
-For queries of these types, you may also wish to explore the _c_o_m_p_u_t_e_d_ _f_i_e_l_d_s.
 _P_r_e_v_i_o_u_s _N_e_x_t
 ===============================================================================
 Built with _M_k_D_o_c_s using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
 _G_i_t_L_a_b _«_ _P_r_e_v_i_o_u_s _N_e_x_t_ _»
```

### Comparing `django-gcloud-connectors-1.1.0/test/contributing/index.html` & `django-gcloud-connectors-1.2.0/test/contributing/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -63,16 +63,20 @@
                 <li class="toctree-l1"><a class="reference internal" href="../transactions/">Transactions</a>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../caching/">Caching</a>
                 </li>
               </ul>
+              <ul>
+                <li class="toctree-l1"><a class="reference internal" href="../firestore/">Firestore</a>
+                </li>
+              </ul>
               <ul class="current">
-                <li class="toctree-l1 current"><a class="reference internal current" href="./">Contributing & Testing</a>
+                <li class="toctree-l1 current"><a class="reference internal current" href="#">Contributing & Testing</a>
     <ul class="current">
     <li class="toctree-l2"><a class="reference internal" href="#get-started-with-development">Get started with development</a>
     </li>
     <li class="toctree-l2"><a class="reference internal" href="#pick-an-issue-send-a-merge-request">Pick an issue &amp; send a merge request</a>
     </li>
     <li class="toctree-l2"><a class="reference internal" href="#code-style">Code style</a>
     </li>
@@ -82,14 +86,16 @@
     </li>
     <li class="toctree-l2"><a class="reference internal" href="#setting-up">Setting up</a>
     </li>
     <li class="toctree-l2"><a class="reference internal" href="#running-tests">Running tests</a>
         <ul>
     <li class="toctree-l3"><a class="reference internal" href="#running-tests-with-tox">Running tests with tox</a>
     </li>
+    <li class="toctree-l3"><a class="reference internal" href="#quick-tests-run-during-development">Quick tests run during development</a>
+    </li>
     <li class="toctree-l3"><a class="reference internal" href="#running-tests-with-real-datastore">Running tests with real Datastore</a>
     </li>
         </ul>
     </li>
     <li class="toctree-l2"><a class="reference internal" href="#indexes-management">Indexes management</a>
         <ul>
     <li class="toctree-l3"><a class="reference internal" href="#updating-during-development">Updating during development</a>
@@ -164,52 +170,63 @@
 <p>On setting up the first time, you'll need to:</p>
 <ul>
 <li>Install the gcloud datastore emulator: <code>gcloud components install cloud-datastore-emulator</code><ul>
 <li>If you don't have <code>gcloud</code> (the Google Cloud SDK) installed, installation instructions can be found <a href="https://cloud.google.com/sdk/install">here</a></li>
 <li>Note that the Datastore emulator <a href="https://cloud.google.com/datastore/docs/tools/datastore-emulator">requires the Java JRE</a>.</li>
 </ul>
 </li>
+<li>And/or if you want to use the Firestore connector, install the Firestore emulator: <code>gcloud components install cloud-firestore-emulator</code></li>
 </ul>
 <h2 id="running-tests">Running tests</h2>
 <p>To run the tests, you'll need to:</p>
 <ul>
 <li>Create a Python 3 virtual environment: <code>python3 -m venv .venv &amp;&amp; source ./.venv/bin/activate</code></li>
 <li>Install the dependencies: <code>pip install -e ".[test]"</code></li>
 <li>Create test output directory: <code>mkdir .reports</code></li>
 </ul>
-<p>Then you can run the tests:</p>
+<p>Then, to run the tests for the Datastore connector:</p>
 <pre><code>$ django-admin test --settings=test_settings
 </code></pre>
+<p>Or to run the tests for the Firestore connector:</p>
+<pre><code>$ django-admin test --settings=test_settings_firestore
+</code></pre>
 <h3 id="running-tests-with-tox">Running tests with tox</h3>
 <p>You can also run the test suite using <code>tox</code>, a generic virtual environment management and test command line tool.</p>
 <p>Using <code>tox</code> will test against multiple versions of django, making it more comprehensive than <code>django-admin test</code> which will test against a single django version. Because of this <code>tox</code> is slower to run the test suite than <code>django-admin test</code>.</p>
 <p>To use <code>tox</code>:</p>
 <ul>
 <li>Create a Python 3 virtual environment: <code>python3 -m venv .venv &amp;&amp; source ./.venv/bin/activate</code></li>
 <li>Install the prerequisites: <code>pip3 install tox</code></li>
 <li>Create test output directory: <code>mkdir .reports</code></li>
 </ul>
 <p>Then you can run:</p>
 <pre><code>$ tox
 </code></pre>
 <p>Under the hood running <code>tox</code> will install all of the dependencies inside a virtual environment then run <code>./manage.py test</code>.</p>
 <p>To pass down arguments to this command simply separate them with a double hyphen. e.g.</p>
-<pre><code>$ tox -e py37 -- --failfast
+<pre><code>$ tox -e py311 -- --failfast
 </code></pre>
+<h3 id="quick-tests-run-during-development">Quick tests run during development</h3>
+<p>It might be useful during develpment and for rapid test iterations to run tests against a single python version instead of running tests for all enviroments using the <code>tox</code> command. Here's the required steps:
+* Create a Python 3 virtualenv: <code>python3 -m venv .venv &amp;&amp; source ./.venv/bin/activate</code>
+* Install the prerequisites: <code>pip3 install tox</code>
+* run <code>pip install -e ".[test]"</code>
+* run <code>django-admin test --settings=test_settings_firestore</code> to run tests with firestore configurations
+* run <code>django-admin test --settings=test_settings</code> to run tests with datastore configurations</p>
 <h3 id="running-tests-with-real-datastore">Running tests with real Datastore</h3>
 <p>It is sometimes useful to be able to run tests against a real version of the Datastore instead of the emulator.</p>
 <p>You need to create your own GCP project and then set the <code>GCLOUDC_PROJECT_ID</code> environment variable.
 Two GCP Projects have been set for Pototo employees:
 - <code>gclouc-test-optimistic</code> for datastore running in OPTIMISTIC concurrency mode.
 - <code>gclouc-test-pessimistic</code> for datastore running in PESSIMISTIC concurrency mode.</p>
 <p>Make sure you have the have configured the application default credentials by running:</p>
 <pre><code>gcloud auth application-default login
 </code></pre>
 <p>You can then run tox passing the <code>--use-remote-datastore</code> option like this:</p>
-<pre><code>$ tox -e py39-22 -- --use-remote-datastore
+<pre><code>$ tox -e py311-42 -- --use-remote-datastore --settings=test_settings
 </code></pre>
 <h2 id="indexes-management">Indexes management</h2>
 <h3 id="updating-during-development">Updating during development</h3>
 <p>When running the test locally, we use the Google Cloud datastore emulator as database.
 When a query that requires a composite index is run, the emulator detects it and if not present already, it adds it to the <code>.index.yaml</code> file, below the <code># AUTOGENERATED</code> row.</p>
 <p>You'll notice this, because the file will appear to have changes in git.
 Unfortunately, all the automatically-added lines are discarded every time the emulator starts. If you notice new indexes have been added, move them above the <code># AUTOGENERATED</code> line and save the file. This will ensure they won't be deleted automatically.</p>
@@ -228,15 +245,15 @@
 </code></pre>
 <p>This will trigger a pipeline that will publish the package in test.pypi.org.
 If that is successful, you can then manually trigger the job <code>publish to prod pypi</code> on the same pipeline to deploy to the official pypi registry.</p>
               
             </div>
           </div><footer>
     <div class="rst-footer-buttons" role="navigation" aria-label="Footer Navigation">
-        <a href="../caching/" class="btn btn-neutral float-left" title="Caching"><span class="icon icon-circle-arrow-left"></span> Previous</a>
+        <a href="../firestore/" class="btn btn-neutral float-left" title="Firestore"><span class="icon icon-circle-arrow-left"></span> Previous</a>
         <a href="../commercial_support/" class="btn btn-neutral float-right" title="Commercial Support">Next <span class="icon icon-circle-arrow-right"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <!-- Copyright etc -->
@@ -256,15 +273,15 @@
   <span class="rst-current-version" data-toggle="rst-current-version">
     
         <span>
           <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/" class="icon icon-gitlab" style="color: #fcfcfc"> GitLab</a>
         </span>
     
     
-      <span><a href="../caching/" style="color: #fcfcfc">&laquo; Previous</a></span>
+      <span><a href="../firestore/" style="color: #fcfcfc">&laquo; Previous</a></span>
     
     
       <span><a href="../commercial_support/" style="color: #fcfcfc">Next &raquo;</a></span>
     
   </span>
 </div>
     <script src="../js/jquery-3.6.0.min.js"></script>
```

#### html2text {}

```diff
@@ -3,23 +3,25 @@
     * _H_o_m_e
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _C_o_n_c_e_p_t_s_ _&_ _l_i_m_i_t_a_t_i_o_n_s
     * _F_i_e_l_d_s
     * _F_i_e_l_d_ _I_n_d_e_x_e_s
     * _T_r_a_n_s_a_c_t_i_o_n_s
     * _C_a_c_h_i_n_g
+    * _F_i_r_e_s_t_o_r_e
     * _C_o_n_t_r_i_b_u_t_i_n_g_ _&_ _T_e_s_t_i_n_g
           o _G_e_t_ _s_t_a_r_t_e_d_ _w_i_t_h_ _d_e_v_e_l_o_p_m_e_n_t
           o _P_i_c_k_ _a_n_ _i_s_s_u_e_ _&_ _s_e_n_d_ _a_ _m_e_r_g_e_ _r_e_q_u_e_s_t
           o _C_o_d_e_ _s_t_y_l_e
           o _N_e_e_d_ _h_e_l_p_?
           o _M_e_r_g_e_ _r_e_q_u_e_s_t_ _r_e_q_u_i_r_e_m_e_n_t_s
           o _S_e_t_t_i_n_g_ _u_p
           o _R_u_n_n_i_n_g_ _t_e_s_t_s
                 # _R_u_n_n_i_n_g_ _t_e_s_t_s_ _w_i_t_h_ _t_o_x
+                # _Q_u_i_c_k_ _t_e_s_t_s_ _r_u_n_ _d_u_r_i_n_g_ _d_e_v_e_l_o_p_m_e_n_t
                 # _R_u_n_n_i_n_g_ _t_e_s_t_s_ _w_i_t_h_ _r_e_a_l_ _D_a_t_a_s_t_o_r_e
           o _I_n_d_e_x_e_s_ _m_a_n_a_g_e_m_e_n_t
                 # _U_p_d_a_t_i_n_g_ _d_u_r_i_n_g_ _d_e_v_e_l_o_p_m_e_n_t
                 # _D_e_p_l_o_y_i_n_g_ _i_n_d_e_x_e_s
           o _R_e_l_e_a_s_e_ _p_r_o_c_e_s_s
     * _C_o_m_m_e_r_c_i_a_l_ _S_u_p_p_o_r_t
     * _W_o_r_k_ _w_i_t_h_ _u_s_!
@@ -54,22 +56,26 @@
 ********** SSeettttiinngg uupp **********
 On setting up the first time, you'll need to:
     * Install the gcloud datastore emulator: gcloud components install cloud-
       datastore-emulator
           o If you don't have gcloud (the Google Cloud SDK) installed,
             installation instructions can be found _h_e_r_e
           o Note that the Datastore emulator _r_e_q_u_i_r_e_s_ _t_h_e_ _J_a_v_a_ _J_R_E.
+    * And/or if you want to use the Firestore connector, install the Firestore
+      emulator: gcloud components install cloud-firestore-emulator
 ********** RRuunnnniinngg tteessttss **********
 To run the tests, you'll need to:
     * Create a Python 3 virtual environment: python3 -m venv .venv && source
       ./.venv/bin/activate
     * Install the dependencies: pip install -e ".[test]"
     * Create test output directory: mkdir .reports
-Then you can run the tests:
+Then, to run the tests for the Datastore connector:
 $ django-admin test --settings=test_settings
+Or to run the tests for the Firestore connector:
+$ django-admin test --settings=test_settings_firestore
 ******** RRuunnnniinngg tteessttss wwiitthh ttooxx ********
 You can also run the test suite using tox, a generic virtual environment
 management and test command line tool.
 Using tox will test against multiple versions of django, making it more
 comprehensive than django-admin test which will test against a single django
 version. Because of this tox is slower to run the test suite than django-admin
 test.
@@ -80,27 +86,36 @@
     * Create test output directory: mkdir .reports
 Then you can run:
 $ tox
 Under the hood running tox will install all of the dependencies inside a
 virtual environment then run ./manage.py test.
 To pass down arguments to this command simply separate them with a double
 hyphen. e.g.
-$ tox -e py37 -- --failfast
+$ tox -e py311 -- --failfast
+******** QQuuiicckk tteessttss rruunn dduurriinngg ddeevveellooppmmeenntt ********
+It might be useful during develpment and for rapid test iterations to run tests
+against a single python version instead of running tests for all enviroments
+using the tox command. Here's the required steps: * Create a Python 3
+virtualenv: python3 -m venv .venv && source ./.venv/bin/activate * Install the
+prerequisites: pip3 install tox * run pip install -e ".[test]" * run django-
+admin test --settings=test_settings_firestore to run tests with firestore
+configurations * run django-admin test --settings=test_settings to run tests
+with datastore configurations
 ******** RRuunnnniinngg tteessttss wwiitthh rreeaall DDaattaassttoorree ********
 It is sometimes useful to be able to run tests against a real version of the
 Datastore instead of the emulator.
 You need to create your own GCP project and then set the GCLOUDC_PROJECT_ID
 environment variable. Two GCP Projects have been set for Pototo employees: -
 gclouc-test-optimistic for datastore running in OPTIMISTIC concurrency mode. -
 gclouc-test-pessimistic for datastore running in PESSIMISTIC concurrency mode.
 Make sure you have the have configured the application default credentials by
 running:
 gcloud auth application-default login
 You can then run tox passing the --use-remote-datastore option like this:
-$ tox -e py39-22 -- --use-remote-datastore
+$ tox -e py311-42 -- --use-remote-datastore --settings=test_settings
 ********** IInnddeexxeess mmaannaaggeemmeenntt **********
 ******** UUppddaattiinngg dduurriinngg ddeevveellooppmmeenntt ********
 When running the test locally, we use the Google Cloud datastore emulator as
 database. When a query that requires a composite index is run, the emulator
 detects it and if not present already, it adds it to the .index.yaml file,
 below the # AUTOGENERATED row.
 You'll notice this, because the file will appear to have changes in git.
```

### Comparing `django-gcloud-connectors-1.1.0/test/field_indexes/index.html` & `django-gcloud-connectors-1.2.0/test/field_indexes/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -52,15 +52,15 @@
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../fields/">Fields</a>
                 </li>
               </ul>
               <ul class="current">
-                <li class="toctree-l1 current"><a class="reference internal current" href="./">Field Indexes</a>
+                <li class="toctree-l1 current"><a class="reference internal current" href="#">Field Indexes</a>
     <ul class="current">
     <li class="toctree-l2"><a class="reference internal" href="#default">Default</a>
     </li>
     <li class="toctree-l2"><a class="reference internal" href="#meta-indexes">Meta Indexes</a>
     </li>
     <li class="toctree-l2"><a class="reference internal" href="#runtime-warnings">Runtime Warnings</a>
     </li>
@@ -74,14 +74,18 @@
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../caching/">Caching</a>
                 </li>
               </ul>
               <ul>
+                <li class="toctree-l1"><a class="reference internal" href="../firestore/">Firestore</a>
+                </li>
+              </ul>
+              <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../contributing/">Contributing & Testing</a>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../commercial_support/">Commercial Support</a>
                 </li>
               </ul>
@@ -141,14 +145,15 @@
 </code></pre>
 <p>In the above example <code>field1</code> and <code>field2</code> will be indexed. <code>field3</code> will be excluded because it is NOT referenced in <code>Meta.indexes</code>.</p>
 <p>This configurability is useful because <a href="https://cloud.google.com/datastore/docs/concepts/indexes#unindexed_properties">excluding fields can provide cost and performance improvements</a>.</p>
 <h2 id="runtime-warnings">Runtime Warnings</h2>
 <p>To help identify queries which are executed through the ORM which depend on an index which is missing, we raise a <code>DatabaseError</code> at runtime.</p>
 <h2 id="limitations">Limitations</h2>
 <ul>
+<li>We only support this on the Datastore backend. For Firestore single field exceptions can be added from the console, see the <a href="https://cloud.google.com/firestore/docs/query-data/indexing#:~:text=Single%2Dfield%20index%20exemptions%20allow,go%20to%20the%20Databases%20page.&amp;text=Select%20the%20required%20database%20from%20the%20list%20of%20databases.,-In%20the%20navigation">documentation</a></li>
 <li>We only support single property indexes on the model, i.e. composite indexes are not supported yet (you need an <code>index.yaml</code> or similar for these).</li>
 <li><code>db_index</code> is not supported at field level (the django docs have a future deprecation warning). You must use <code>Meta.indexes</code>.</li>
 <li><code>TextField</code> and <code>BinaryField</code> will not be indexed, even if defined in the Meta. This is because these fields exceed the maximum size limits for their respective indexed properties.</li>
 <li>Queries requiring composite indexes need all properties to be indexed - see the unindexed properties section in <a href="https://cloud.google.com/datastore/docs/concepts/indexes#unindexed_properties">the docs</a>, i.e. "if a property appears in a composite index, then excluding the property will disable it in the composite index."</li>
 <li>Projection queries require that the specified fields are indexed - see the projection queries section in <a href="https://cloud.google.com/datastore/docs/concepts/queries#projection_queries">the docs</a>, i.e. "Projection queries require the specified properties to be indexed."</li>
 <li>If you add fields to the meta indexes, these indexes won’t be applied to existing entities in the datastore but will require a migration.</li>
 <li>Setting the indexes in the meta to an empty list (i.e. <code>indexes = []</code>) will not exclude all fields from being indexed; instead, all fields will remain indexed. If you wish to exclude all fields that can be indexed, you can pass the primary key field to the meta, i.e. <code>indexes = [models.Index(fields=["id"])]</code> in the above example, as the primary key field will always be indexed, whether defined in the meta or not.</li>
```

#### html2text {}

```diff
@@ -7,14 +7,15 @@
     * _F_i_e_l_d_ _I_n_d_e_x_e_s
           o _D_e_f_a_u_l_t
           o _M_e_t_a_ _I_n_d_e_x_e_s
           o _R_u_n_t_i_m_e_ _W_a_r_n_i_n_g_s
           o _L_i_m_i_t_a_t_i_o_n_s
     * _T_r_a_n_s_a_c_t_i_o_n_s
     * _C_a_c_h_i_n_g
+    * _F_i_r_e_s_t_o_r_e
     * _C_o_n_t_r_i_b_u_t_i_n_g_ _&_ _T_e_s_t_i_n_g
     * _C_o_m_m_e_r_c_i_a_l_ _S_u_p_p_o_r_t
     * _W_o_r_k_ _w_i_t_h_ _u_s_!
 _D_j_a_n_g_o_ _G_c_l_o_u_d_ _C_o_n_n_e_c_t_o_r_s_ _D_o_c_u_m_e_n_t_a_t_i_o_n
     * Field Indexes
     * _E_d_i_t_ _o_n_ _G_i_t_L_a_b
 ===============================================================================
@@ -50,14 +51,16 @@
 because it is NOT referenced in Meta.indexes.
 This configurability is useful because _e_x_c_l_u_d_i_n_g_ _f_i_e_l_d_s_ _c_a_n_ _p_r_o_v_i_d_e_ _c_o_s_t_ _a_n_d
 _p_e_r_f_o_r_m_a_n_c_e_ _i_m_p_r_o_v_e_m_e_n_t_s.
 ********** RRuunnttiimmee WWaarrnniinnggss **********
 To help identify queries which are executed through the ORM which depend on an
 index which is missing, we raise a DatabaseError at runtime.
 ********** LLiimmiittaattiioonnss **********
+    * We only support this on the Datastore backend. For Firestore single field
+      exceptions can be added from the console, see the _d_o_c_u_m_e_n_t_a_t_i_o_n
     * We only support single property indexes on the model, i.e. composite
       indexes are not supported yet (you need an index.yaml or similar for
       these).
     * db_index is not supported at field level (the django docs have a future
       deprecation warning). You must use Meta.indexes.
     * TextField and BinaryField will not be indexed, even if defined in the
       Meta. This is because these fields exceed the maximum size limits for
```

### Comparing `django-gcloud-connectors-1.1.0/test/fields/index.html` & `django-gcloud-connectors-1.2.0/test/fields/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -48,22 +48,24 @@
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../concepts_limitations/">Concepts & limitations</a>
                 </li>
               </ul>
               <ul class="current">
-                <li class="toctree-l1 current"><a class="reference internal current" href="./">Fields</a>
+                <li class="toctree-l1 current"><a class="reference internal current" href="#">Fields</a>
     <ul class="current">
     <li class="toctree-l2"><a class="reference internal" href="#listfield">ListField</a>
     </li>
     <li class="toctree-l2"><a class="reference internal" href="#setfield">SetField</a>
     </li>
     <li class="toctree-l2"><a class="reference internal" href="#charornonefield">CharOrNoneField</a>
     </li>
+    <li class="toctree-l2"><a class="reference internal" href="#trueornonefield">TrueOrNoneField</a>
+    </li>
     <li class="toctree-l2"><a class="reference internal" href="#charfield">CharField</a>
     </li>
     <li class="toctree-l2"><a class="reference internal" href="#relatedlistfield">RelatedListField</a>
     </li>
     <li class="toctree-l2"><a class="reference internal" href="#relatedsetfield">RelatedSetField</a>
     </li>
     <li class="toctree-l2"><a class="reference internal" href="#computed-fields">Computed fields</a>
@@ -82,14 +84,18 @@
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../caching/">Caching</a>
                 </li>
               </ul>
               <ul>
+                <li class="toctree-l1"><a class="reference internal" href="../firestore/">Firestore</a>
+                </li>
+              </ul>
+              <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../contributing/">Contributing & Testing</a>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../commercial_support/">Commercial Support</a>
                 </li>
               </ul>
@@ -142,14 +148,21 @@
 This is useful if you want values to be unique but also want to allow empty values.</p>
 <p>It is generally not good practice to put <code>null=True</code> on a Django <code>CharField</code>,
 and even if you do, when you edit such a field through a Django form,
 an empty value will be stored as an empty string rather than <code>None</code>.</p>
 <p>This field will instead store empty values as <code>None</code>, which then allows enforcement of uniqueness
 for non-empty values (because multiple empty string values will violate a unique constraint,
 whereas multiple <code>None</code> values will not).</p>
+<h2 id="trueornonefield">TrueOrNoneField</h2>
+<p>A field that stores either <code>True</code> or <code>None</code>.
+This is useful for when you want to enforce that only one object can have this field set to <code>True</code>.
+Any objects on which the field value is <code>None</code> will be ignored by unique constraints, thereby allowing
+you to set <code>unique=True</code> on the field to enforce that only one object can have the field set to <code>True</code>.</p>
+<p>Similarly, you can use the field in a <code>unique_together</code> constraint, and any <code>None</code> values will be
+ignored by the constraint.</p>
 <h2 id="charfield">CharField</h2>
 <p>On the Cloud Datastore, every <code>str</code> property has the same maximum length of 1500 <em>bytes</em> (not characters),
 so the required <code>max_length</code> argument of Django's <code>CharField</code> is both ignored and unreliable.</p>
 <p>gcloudc's <code>CharField</code> sets a default <code>max_length</code> of 1500 and enforces it in bytes, the same way as the Datastore does.</p>
 <p>This means you can omit the <code>max_length</code> argument from the field,
 and can rely on the field to correctly validate the values to the requirements of the database.</p>
 <h2 id="relatedlistfield">RelatedListField</h2>
```

#### html2text {}

```diff
@@ -3,22 +3,24 @@
     * _H_o_m_e
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _C_o_n_c_e_p_t_s_ _&_ _l_i_m_i_t_a_t_i_o_n_s
     * _F_i_e_l_d_s
           o _L_i_s_t_F_i_e_l_d
           o _S_e_t_F_i_e_l_d
           o _C_h_a_r_O_r_N_o_n_e_F_i_e_l_d
+          o _T_r_u_e_O_r_N_o_n_e_F_i_e_l_d
           o _C_h_a_r_F_i_e_l_d
           o _R_e_l_a_t_e_d_L_i_s_t_F_i_e_l_d
           o _R_e_l_a_t_e_d_S_e_t_F_i_e_l_d
           o _C_o_m_p_u_t_e_d_ _f_i_e_l_d_s
           o _Q_u_e_r_y_i_n_g_ _o_n_ _i_t_e_r_a_b_l_e_ _f_i_e_l_d_s
     * _F_i_e_l_d_ _I_n_d_e_x_e_s
     * _T_r_a_n_s_a_c_t_i_o_n_s
     * _C_a_c_h_i_n_g
+    * _F_i_r_e_s_t_o_r_e
     * _C_o_n_t_r_i_b_u_t_i_n_g_ _&_ _T_e_s_t_i_n_g
     * _C_o_m_m_e_r_c_i_a_l_ _S_u_p_p_o_r_t
     * _W_o_r_k_ _w_i_t_h_ _u_s_!
 _D_j_a_n_g_o_ _G_c_l_o_u_d_ _C_o_n_n_e_c_t_o_r_s_ _D_o_c_u_m_e_n_t_a_t_i_o_n
     * Fields
     * _E_d_i_t_ _o_n_ _G_i_t_L_a_b
 ===============================================================================
@@ -49,14 +51,22 @@
 It is generally not good practice to put null=True on a Django CharField, and
 even if you do, when you edit such a field through a Django form, an empty
 value will be stored as an empty string rather than None.
 This field will instead store empty values as None, which then allows
 enforcement of uniqueness for non-empty values (because multiple empty string
 values will violate a unique constraint, whereas multiple None values will
 not).
+********** TTrruueeOOrrNNoonneeFFiieelldd **********
+A field that stores either True or None. This is useful for when you want to
+enforce that only one object can have this field set to True. Any objects on
+which the field value is None will be ignored by unique constraints, thereby
+allowing you to set unique=True on the field to enforce that only one object
+can have the field set to True.
+Similarly, you can use the field in a unique_together constraint, and any None
+values will be ignored by the constraint.
 ********** CChhaarrFFiieelldd **********
 On the Cloud Datastore, every str property has the same maximum length of 1500
 bbyytteess (not characters), so the required max_length argument of Django's
 CharField is both ignored and unreliable.
 gcloudc's CharField sets a default max_length of 1500 and enforces it in bytes,
 the same way as the Datastore does.
 This means you can omit the max_length argument from the field, and can rely on
```

### Comparing `django-gcloud-connectors-1.1.0/test/index.html` & `django-gcloud-connectors-1.2.0/test/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -36,16 +36,18 @@
       <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" title="Type search term here" />
   </form>
 </div>
       </div>
 
       <div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul class="current">
-                <li class="toctree-l1 current"><a class="reference internal current" href=".">Home</a>
+                <li class="toctree-l1 current"><a class="reference internal current" href="#">Home</a>
     <ul class="current">
+    <li class="toctree-l2"><a class="reference internal" href="#notes">Notes</a>
+    </li>
     </ul>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="installation/">Installation</a>
                 </li>
               </ul>
@@ -66,14 +68,18 @@
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="caching/">Caching</a>
                 </li>
               </ul>
               <ul>
+                <li class="toctree-l1"><a class="reference internal" href="firestore/">Firestore</a>
+                </li>
+              </ul>
+              <ul>
                 <li class="toctree-l1"><a class="reference internal" href="contributing/">Contributing & Testing</a>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="commercial_support/">Commercial Support</a>
                 </li>
               </ul>
@@ -101,18 +107,23 @@
     </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
             <div class="section" itemprop="articleBody">
               
-                <h1 id="django-gcloud-connectors-gcloudc">Django Gcloud Connectors (gcloudc)</h1>
-<p>The aim of this project is to create Django database connector / backend for Google Cloud.</p>
-<p>Currently it contains a connector for the Google Cloud Firestore in Datastore mode,
-but in the future it may also include a Firestore connector, or even a MemoryStore one.</p>
+                <h1 id="django-gcloud-connectors-gcloudc">Django GCloud Connectors (gcloudc)</h1>
+<p>This project provides a Django database connector / backend for the non-relational databases provided by Google Cloud Platform.</p>
+<p>Currently it contains connectors for:</p>
+<ul>
+<li>Firestore in Datastore mode</li>
+<li>Firestore in native mode</li>
+</ul>
+<p>It could in theory be expanded to create connectors for other non-relational databases.</p>
+<h3 id="notes">Notes</h3>
 <p>Note: from version <code>1.0.0</code> we dropped support the <code>OPTIMISTIC_WITH_ENTITY_GROUPS</code> legacy concurrency mode and legacy Datastore.
 Use <code>0.4.0</code> if you need to support legacy behaviour (please be aware transactions and uniqueness constraints are buggy in  versions &lt; <code>1.0.0</code>, for more information please refer to the <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/-/blob/master/CHANGELOG.md">changelog</a>).</p>
 <p>This is the continuation of the Datastore connector from the <a href="https://github.com/potatolondon/djangae">Djangae project</a>
 but converted to use the <a href="https://googleapis.github.io/google-cloud-python/latest/datastore/">Cloud Datastore API</a> on Python 3.
 It is deliberately split out into its own library so that if you want to you can use Django's ORM with the Cloud Datastore on any platform.
 For example, you could run Django on AWS and still use this library to connect the ORM to your Google Cloud Datastore.</p>
               
@@ -162,10 +173,10 @@
         });
     </script>
 
 </body>
 </html>
 
 <!--
-MkDocs version : 1.5.3
-Build Date UTC : 2024-03-05 15:06:15.853466+00:00
+MkDocs version : 1.6.0
+Build Date UTC : 2024-05-20 14:02:54.095913+00:00
 -->
```

#### html2text {}

```diff
@@ -1,29 +1,34 @@
 _D_j_a_n_g_o_ _G_c_l_o_u_d_ _C_o_n_n_e_c_t_o_r_s_ _D_o_c_u_m_e_n_t_a_t_i_o_n
 [q                   ]
     * _H_o_m_e
+          o _N_o_t_e_s
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _C_o_n_c_e_p_t_s_ _&_ _l_i_m_i_t_a_t_i_o_n_s
     * _F_i_e_l_d_s
     * _F_i_e_l_d_ _I_n_d_e_x_e_s
     * _T_r_a_n_s_a_c_t_i_o_n_s
     * _C_a_c_h_i_n_g
+    * _F_i_r_e_s_t_o_r_e
     * _C_o_n_t_r_i_b_u_t_i_n_g_ _&_ _T_e_s_t_i_n_g
     * _C_o_m_m_e_r_c_i_a_l_ _S_u_p_p_o_r_t
     * _W_o_r_k_ _w_i_t_h_ _u_s_!
 _D_j_a_n_g_o_ _G_c_l_o_u_d_ _C_o_n_n_e_c_t_o_r_s_ _D_o_c_u_m_e_n_t_a_t_i_o_n
     * Home
     * _E_d_i_t_ _o_n_ _G_i_t_L_a_b
 ===============================================================================
-************ DDjjaannggoo GGcclloouudd CCoonnnneeccttoorrss ((ggcclloouuddcc)) ************
-The aim of this project is to create Django database connector / backend for
-Google Cloud.
-Currently it contains a connector for the Google Cloud Firestore in Datastore
-mode, but in the future it may also include a Firestore connector, or even a
-MemoryStore one.
+************ DDjjaannggoo GGCClloouudd CCoonnnneeccttoorrss ((ggcclloouuddcc)) ************
+This project provides a Django database connector / backend for the non-
+relational databases provided by Google Cloud Platform.
+Currently it contains connectors for:
+    * Firestore in Datastore mode
+    * Firestore in native mode
+It could in theory be expanded to create connectors for other non-relational
+databases.
+******** NNootteess ********
 Note: from version 1.0.0 we dropped support the OPTIMISTIC_WITH_ENTITY_GROUPS
 legacy concurrency mode and legacy Datastore. Use 0.4.0 if you need to support
 legacy behaviour (please be aware transactions and uniqueness constraints are
 buggy in versions < 1.0.0, for more information please refer to the _c_h_a_n_g_e_l_o_g).
 This is the continuation of the Datastore connector from the _D_j_a_n_g_a_e_ _p_r_o_j_e_c_t
 but converted to use the _C_l_o_u_d_ _D_a_t_a_s_t_o_r_e_ _A_P_I on Python 3. It is deliberately
 split out into its own library so that if you want to you can use Django's ORM
```

### Comparing `django-gcloud-connectors-1.1.0/test/installation/index.html` & `django-gcloud-connectors-1.2.0/test/transactions/index.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
     <meta charset="utf-8" />
     <meta http-equiv="X-UA-Compatible" content="IE=edge" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><link rel="canonical" href="https://potato-oss.gitlab.io/google-cloud/django-gcloud-connectors/installation/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><link rel="canonical" href="https://potato-oss.gitlab.io/google-cloud/django-gcloud-connectors/transactions/" />
       <link rel="shortcut icon" href="../img/favicon.ico" />
-    <title>Installation - Django Gcloud Connectors Documentation</title>
+    <title>Transactions - Django Gcloud Connectors Documentation</title>
     <link rel="stylesheet" href="../css/theme.css" />
     <link rel="stylesheet" href="../css/theme_extra.css" />
         <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/styles/github.min.css" />
     
       <script>
         // Current page data
-        var mkdocs_page_name = "Installation";
-        var mkdocs_page_input_path = "installation.md";
-        var mkdocs_page_url = "/google-cloud/django-gcloud-connectors/installation/";
+        var mkdocs_page_name = "Transactions";
+        var mkdocs_page_input_path = "transactions.md";
+        var mkdocs_page_url = "/google-cloud/django-gcloud-connectors/transactions/";
       </script>
     
     <!--[if lt IE 9]>
       <script src="../js/html5shiv.min.js"></script>
     <![endif]-->
       <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/highlight.min.js"></script>
       <script>hljs.highlightAll();</script> 
@@ -39,43 +39,45 @@
       </div>
 
       <div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="..">Home</a>
                 </li>
               </ul>
-              <ul class="current">
-                <li class="toctree-l1 current"><a class="reference internal current" href="./">Installation</a>
-    <ul class="current">
-    <li class="toctree-l2"><a class="reference internal" href="#automatic-cloud-datastore-emulator-startup">Automatic Cloud Datastore Emulator startup</a>
-    </li>
-    </ul>
+              <ul>
+                <li class="toctree-l1"><a class="reference internal" href="../installation/">Installation</a>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../concepts_limitations/">Concepts & limitations</a>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../fields/">Fields</a>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../field_indexes/">Field Indexes</a>
                 </li>
               </ul>
-              <ul>
-                <li class="toctree-l1"><a class="reference internal" href="../transactions/">Transactions</a>
+              <ul class="current">
+                <li class="toctree-l1 current"><a class="reference internal current" href="#">Transactions</a>
+    <ul class="current">
+    </ul>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../caching/">Caching</a>
                 </li>
               </ul>
               <ul>
+                <li class="toctree-l1"><a class="reference internal" href="../firestore/">Firestore</a>
+                </li>
+              </ul>
+              <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../contributing/">Contributing & Testing</a>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../commercial_support/">Commercial Support</a>
                 </li>
               </ul>
@@ -93,48 +95,39 @@
           <a href="..">Django Gcloud Connectors Documentation</a>
         
       </nav>
       <div class="wy-nav-content">
         <div class="rst-content"><div role="navigation" aria-label="breadcrumbs navigation">
   <ul class="wy-breadcrumbs">
     <li><a href=".." class="icon icon-home" aria-label="Docs"></a></li>
-      <li class="breadcrumb-item active">Installation</li>
+      <li class="breadcrumb-item active">Transactions</li>
     <li class="wy-breadcrumbs-aside">
-          <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/installation.md" class="icon icon-gitlab"> Edit on GitLab</a>
+          <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/transactions.md" class="icon icon-gitlab"> Edit on GitLab</a>
     </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
             <div class="section" itemprop="articleBody">
               
-                <h1 id="installation">Installation</h1>
-<p>The most common way to install <code>gcloudc</code> is to use it as part of <a href="https://potato-oss.gitlab.io/djangae/djangae/">Djangae</a>.</p>
-<p>You can also install it on its own with <code>pip install django-gcloud-connectors</code>.</p>
-<p>However you install it, you will need to set your <code>DATABASES</code> configuration in your Django settings module to look something like this:</p>
-<pre><code class="language-python">from djangae
-DATABASES = {
-    &quot;default&quot;: {
-        'ENGINE': 'gcloudc.db.backends.datastore',
-        'PROJECT': 'YOUR_GCP_PROJECT_NAME',  # You can use djangae.environment.project_id() here
-        'INDEXES_FILE': 'PATH_TO_A_FILE_FOR_SPECICAL_INDEXES',
-    }
-}
-</code></pre>
-<p>Note that the <code>INDEXES_FILE</code> here is <em>not</em> the <code>index.yaml</code> file, but a separate file for gcloudc to store its "special indexes" in.
-See <a href="../concepts_limitations/#special-indexes">Special Indexes</a>.</p>
-<h2 id="automatic-cloud-datastore-emulator-startup">Automatic Cloud Datastore Emulator startup</h2>
-<p>gcloudc provides overrides for the <code>runserver</code> and <code>test</code> commands which
-start and stop a Cloud Datastore Emulator instance. To enable this functionality add <code>gcloudc.commands</code> <em>at the beginning</em> of your <code>INSTALLED_APPS</code> setting.</p>
+                <h1 id="transactions">Transactions</h1>
+<p>Transactions on the Cloud Datastore behave differently to those of a SQL database.
+It's worth reading the <a href="https://cloud.google.com/datastore/docs/concepts/transactions">Cloud Datastore transactions documentation</a>
+to familiarise yourself with their behaviour.
+Crucially:</p>
+<blockquote>
+<p>"queries and lookups inside a Datastore mode transaction do <em>not</em> see the results of previous writes inside that transaction".</p>
+</blockquote>
+<p>This is partially mitigated by our caching system. For more info on how querying and caching work see the <a href="../caching">caching</a> docs.</p>
               
             </div>
           </div><footer>
     <div class="rst-footer-buttons" role="navigation" aria-label="Footer Navigation">
-        <a href=".." class="btn btn-neutral float-left" title="Home"><span class="icon icon-circle-arrow-left"></span> Previous</a>
-        <a href="../concepts_limitations/" class="btn btn-neutral float-right" title="Concepts & limitations">Next <span class="icon icon-circle-arrow-right"></span></a>
+        <a href="../field_indexes/" class="btn btn-neutral float-left" title="Field Indexes"><span class="icon icon-circle-arrow-left"></span> Previous</a>
+        <a href="../caching/" class="btn btn-neutral float-right" title="Caching">Next <span class="icon icon-circle-arrow-right"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <!-- Copyright etc -->
   </div>
@@ -153,18 +146,18 @@
   <span class="rst-current-version" data-toggle="rst-current-version">
     
         <span>
           <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/" class="icon icon-gitlab" style="color: #fcfcfc"> GitLab</a>
         </span>
     
     
-      <span><a href=".." style="color: #fcfcfc">&laquo; Previous</a></span>
+      <span><a href="../field_indexes/" style="color: #fcfcfc">&laquo; Previous</a></span>
     
     
-      <span><a href="../concepts_limitations/" style="color: #fcfcfc">Next &raquo;</a></span>
+      <span><a href="../caching/" style="color: #fcfcfc">Next &raquo;</a></span>
     
   </span>
 </div>
     <script src="../js/jquery-3.6.0.min.js"></script>
     <script>var base_url = "..";</script>
     <script src="../js/theme_extra.js"></script>
     <script src="../js/theme.js"></script>
```

#### html2text {}

```diff
@@ -1,41 +1,29 @@
 _D_j_a_n_g_o_ _G_c_l_o_u_d_ _C_o_n_n_e_c_t_o_r_s_ _D_o_c_u_m_e_n_t_a_t_i_o_n
 [q                   ]
     * _H_o_m_e
     * _I_n_s_t_a_l_l_a_t_i_o_n
-          o _A_u_t_o_m_a_t_i_c_ _C_l_o_u_d_ _D_a_t_a_s_t_o_r_e_ _E_m_u_l_a_t_o_r_ _s_t_a_r_t_u_p
     * _C_o_n_c_e_p_t_s_ _&_ _l_i_m_i_t_a_t_i_o_n_s
     * _F_i_e_l_d_s
     * _F_i_e_l_d_ _I_n_d_e_x_e_s
     * _T_r_a_n_s_a_c_t_i_o_n_s
     * _C_a_c_h_i_n_g
+    * _F_i_r_e_s_t_o_r_e
     * _C_o_n_t_r_i_b_u_t_i_n_g_ _&_ _T_e_s_t_i_n_g
     * _C_o_m_m_e_r_c_i_a_l_ _S_u_p_p_o_r_t
     * _W_o_r_k_ _w_i_t_h_ _u_s_!
 _D_j_a_n_g_o_ _G_c_l_o_u_d_ _C_o_n_n_e_c_t_o_r_s_ _D_o_c_u_m_e_n_t_a_t_i_o_n
-    * Installation
+    * Transactions
     * _E_d_i_t_ _o_n_ _G_i_t_L_a_b
 ===============================================================================
-************ IInnssttaallllaattiioonn ************
-The most common way to install gcloudc is to use it as part of _D_j_a_n_g_a_e.
-You can also install it on its own with pip install django-gcloud-connectors.
-However you install it, you will need to set your DATABASES configuration in
-your Django settings module to look something like this:
-from djangae
-DATABASES = {
-    "default": {
-        'ENGINE': 'gcloudc.db.backends.datastore',
-        'PROJECT': 'YOUR_GCP_PROJECT_NAME',  # You can use
-djangae.environment.project_id() here
-        'INDEXES_FILE': 'PATH_TO_A_FILE_FOR_SPECICAL_INDEXES',
-    }
-}
-Note that the INDEXES_FILE here is nnoott the index.yaml file, but a separate file
-for gcloudc to store its "special indexes" in. See _S_p_e_c_i_a_l_ _I_n_d_e_x_e_s.
-********** AAuuttoommaattiicc CClloouudd DDaattaassttoorree EEmmuullaattoorr ssttaarrttuupp **********
-gcloudc provides overrides for the runserver and test commands which start and
-stop a Cloud Datastore Emulator instance. To enable this functionality add
-gcloudc.commands aatt tthhee bbeeggiinnnniinngg of your INSTALLED_APPS setting.
+************ TTrraannssaaccttiioonnss ************
+Transactions on the Cloud Datastore behave differently to those of a SQL
+database. It's worth reading the _C_l_o_u_d_ _D_a_t_a_s_t_o_r_e_ _t_r_a_n_s_a_c_t_i_o_n_s_ _d_o_c_u_m_e_n_t_a_t_i_o_n to
+familiarise yourself with their behaviour. Crucially:
+     "queries and lookups inside a Datastore mode transaction do nnoott see
+     the results of previous writes inside that transaction".
+This is partially mitigated by our caching system. For more info on how
+querying and caching work see the _c_a_c_h_i_n_g docs.
 _P_r_e_v_i_o_u_s _N_e_x_t
 ===============================================================================
 Built with _M_k_D_o_c_s using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
 _G_i_t_L_a_b _«_ _P_r_e_v_i_o_u_s _N_e_x_t_ _»
```

### Comparing `django-gcloud-connectors-1.1.0/test/search.html` & `django-gcloud-connectors-1.2.0/test/search.html`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,18 @@
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="./caching/">Caching</a>
                 </li>
               </ul>
               <ul>
+                <li class="toctree-l1"><a class="reference internal" href="./firestore/">Firestore</a>
+                </li>
+              </ul>
+              <ul>
                 <li class="toctree-l1"><a class="reference internal" href="./contributing/">Contributing & Testing</a>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="./commercial_support/">Commercial Support</a>
                 </li>
               </ul>
```

#### html2text {}

```diff
@@ -3,14 +3,15 @@
     * _H_o_m_e
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _C_o_n_c_e_p_t_s_ _&_ _l_i_m_i_t_a_t_i_o_n_s
     * _F_i_e_l_d_s
     * _F_i_e_l_d_ _I_n_d_e_x_e_s
     * _T_r_a_n_s_a_c_t_i_o_n_s
     * _C_a_c_h_i_n_g
+    * _F_i_r_e_s_t_o_r_e
     * _C_o_n_t_r_i_b_u_t_i_n_g_ _&_ _T_e_s_t_i_n_g
     * _C_o_m_m_e_r_c_i_a_l_ _S_u_p_p_o_r_t
     * _W_o_r_k_ _w_i_t_h_ _u_s_!
 _D_j_a_n_g_o_ _G_c_l_o_u_d_ _C_o_n_n_e_c_t_o_r_s_ _D_o_c_u_m_e_n_t_a_t_i_o_n
 ===============================================================================
 ************ SSeeaarrcchh RReessuullttss ************
 [q                   ]
```

### Comparing `django-gcloud-connectors-1.1.0/test/transactions/index.html` & `django-gcloud-connectors-1.2.0/test/firestore/index.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
     <meta charset="utf-8" />
     <meta http-equiv="X-UA-Compatible" content="IE=edge" />
-    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><link rel="canonical" href="https://potato-oss.gitlab.io/google-cloud/django-gcloud-connectors/transactions/" />
+    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><link rel="canonical" href="https://potato-oss.gitlab.io/google-cloud/django-gcloud-connectors/firestore/" />
       <link rel="shortcut icon" href="../img/favicon.ico" />
-    <title>Transactions - Django Gcloud Connectors Documentation</title>
+    <title>Firestore - Django Gcloud Connectors Documentation</title>
     <link rel="stylesheet" href="../css/theme.css" />
     <link rel="stylesheet" href="../css/theme_extra.css" />
         <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/styles/github.min.css" />
     
       <script>
         // Current page data
-        var mkdocs_page_name = "Transactions";
-        var mkdocs_page_input_path = "transactions.md";
-        var mkdocs_page_url = "/google-cloud/django-gcloud-connectors/transactions/";
+        var mkdocs_page_name = "Firestore";
+        var mkdocs_page_input_path = "firestore.md";
+        var mkdocs_page_url = "/google-cloud/django-gcloud-connectors/firestore/";
       </script>
     
     <!--[if lt IE 9]>
       <script src="../js/html5shiv.min.js"></script>
     <![endif]-->
       <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.8.0/highlight.min.js"></script>
       <script>hljs.highlightAll();</script> 
@@ -55,43 +55,35 @@
                 <li class="toctree-l1"><a class="reference internal" href="../fields/">Fields</a>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../field_indexes/">Field Indexes</a>
                 </li>
               </ul>
+              <ul>
+                <li class="toctree-l1"><a class="reference internal" href="../transactions/">Transactions</a>
+                </li>
+              </ul>
+              <ul>
+                <li class="toctree-l1"><a class="reference internal" href="../caching/">Caching</a>
+                </li>
+              </ul>
               <ul class="current">
-                <li class="toctree-l1 current"><a class="reference internal current" href="./">Transactions</a>
+                <li class="toctree-l1 current"><a class="reference internal current" href="#">Firestore</a>
     <ul class="current">
-    <li class="toctree-l2"><a class="reference internal" href="#atomic">atomic</a>
+    <li class="toctree-l2"><a class="reference internal" href="#primary-keys-are-stored-as-strings">Primary keys are stored as strings</a>
     </li>
-    <li class="toctree-l2"><a class="reference internal" href="#non_atomic">non_atomic</a>
+    <li class="toctree-l2"><a class="reference internal" href="#you-cant-sort-by-pk-descending">You can't sort by PK descending</a>
     </li>
-    <li class="toctree-l2"><a class="reference internal" href="#in_atomic_block">in_atomic_block</a>
-    </li>
-    <li class="toctree-l2"><a class="reference internal" href="#on_commit">on_commit</a>
-    </li>
-    <li class="toctree-l2"><a class="reference internal" href="#transaction-objects">Transaction objects</a>
-        <ul>
-    <li class="toctree-l3"><a class="reference internal" href="#refresh_if_unread">refresh_if_unread</a>
-    </li>
-    <li class="toctree-l3"><a class="reference internal" href="#has_already_been_read">has_already_been_read</a>
-    </li>
-        </ul>
-    </li>
-    <li class="toctree-l2"><a class="reference internal" href="#example-usage">Example usage</a>
+    <li class="toctree-l2"><a class="reference internal" href="#indexes-are-not-generated-by-the-local-emulator">Indexes are not generated by the local emulator</a>
     </li>
     </ul>
                 </li>
               </ul>
               <ul>
-                <li class="toctree-l1"><a class="reference internal" href="../caching/">Caching</a>
-                </li>
-              </ul>
-              <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../contributing/">Contributing & Testing</a>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../commercial_support/">Commercial Support</a>
                 </li>
               </ul>
@@ -109,122 +101,92 @@
           <a href="..">Django Gcloud Connectors Documentation</a>
         
       </nav>
       <div class="wy-nav-content">
         <div class="rst-content"><div role="navigation" aria-label="breadcrumbs navigation">
   <ul class="wy-breadcrumbs">
     <li><a href=".." class="icon icon-home" aria-label="Docs"></a></li>
-      <li class="breadcrumb-item active">Transactions</li>
+      <li class="breadcrumb-item active">Firestore</li>
     <li class="wy-breadcrumbs-aside">
-          <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/transactions.md" class="icon icon-gitlab"> Edit on GitLab</a>
+          <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/edit/master/docs/firestore.md" class="icon icon-gitlab"> Edit on GitLab</a>
     </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
             <div class="section" itemprop="articleBody">
               
-                <h1 id="transactions">Transactions</h1>
-<p>Transactions on the Cloud Datastore behave differently to those of a SQL database.
-It's worth reading the <a href="https://cloud.google.com/datastore/docs/concepts/transactions">Cloud Datastore transactions documentation</a>
-to familiarise yourself with their behaviour.
-Crucially:</p>
-<blockquote>
-<p>"queries and lookups inside a Datastore mode transaction do <em>not</em> see the results of previous writes inside that transaction".</p>
-</blockquote>
-<p>This is partially mitigated by our caching system. For more info on how querying and caching work
-when using <code>gcloudc.db.transaction</code> see the <a href="../caching#inside-transactions">caching</a> docs.</p>
-<p><em>Django's</em> <code>atomic</code> <em>decorator/context manager will have no effect on the Datastore.</em></p>
-<p>However, <code>gcloudc.db.transaction</code> provides a separate set of decorators/context managers for managing transactions.</p>
-<h2 id="atomic"><code>atomic</code></h2>
-<pre><code class="language-python">atomic(
-    independent=False,
-    mandatory=False,
-    using=&quot;default&quot;,
-    read_only=False,
-    enable_cache=True,
-) -&gt; Transaction
-</code></pre>
-<p>This can be used either as a decorator or a context manager to execute a block of code within a Datastore transaction.</p>
-<p>If used as a context manager, it will return the <code>Transaction</code> object.
-If used as a function decorator, you will need to call <code>current_transaction()</code> to get the <code>Transaction</code> object.</p>
-<p>See <a href="#transaction-objects">Transaction object</a>.</p>
-<p>The kwargs are:</p>
-<ul>
-<li><code>independent</code>: forces the start of a new, independent transaction, even if you are currently already in a transaction.</li>
-<li><code>mandatory</code>: forces a check to ensure that you are already within an outer transaction. Raises <code>TransactionFailedError</code> if not.</li>
-<li><code>using</code>: the database connection name to use (works the same as Django's <code>using</code> parameter for database operations).</li>
-<li><code>read_only</code>: for creating a read-only transaction. This functionality is not yet implemented.</li>
-<li><code>enable_cache</code>: enables gcloudc's caching of queries which can only return a singular, unique result.</li>
-</ul>
-<p>For more info on caching and transactions see the <a href="../caching#inside-transactions">caching</a> docs</p>
-<h2 id="non_atomic"><code>non_atomic</code></h2>
-<pre><code class="language-python">non_atomic(using=&quot;default&quot;)
-</code></pre>
-<p>This can be used either as a decorator or a context manager to break out and execute a block of code outside of the current transaction.</p>
-<h2 id="in_atomic_block"><code>in_atomic_block</code></h2>
-<pre><code class="language-python">in_atomic_block(using=&quot;default&quot;) -&gt; bool
-</code></pre>
-<p>This function tells you whether or not you are currently inside an atomic transaction.</p>
-<h2 id="on_commit"><code>on_commit</code></h2>
-<pre><code class="language-python">on_commit(func, using=None)
-</code></pre>
-<p>The same as Django's <code>on_commit</code>, this registers a function to be called when the current transaction is committed.
-If the current transaction is rolled back, <code>func</code> will not be called.</p>
-<h2 id="transaction-objects">Transaction objects</h2>
-<p>When using <code>atomic</code> as a context manager, or using <code>current_transaction()</code>, you will get a <code>Transaction</code> object.
-This can and should be used to perform operations within the transaction.</p>
-<p>A <code>Transaction</code> object has the following methods:</p>
-<h3 id="refresh_if_unread"><code>refresh_if_unread</code></h3>
-<pre><code class="language-python">refresh_if_unread(instance) -&gt; None
-</code></pre>
-<p>This method should be used to refresh instances of Django models from the database.</p>
-<p>Remember that "queries and lookups inside a Datastore mode transaction do <em>not</em> see the results of previous writes inside that transaction",
-therefore, if you query for an object inside a transaction, then modify it, save it and fetch it from the DB again,
-the object that you get back will be the original (unmodified) version, as it existed before the transaction started.
-So if you then modify and save the object again, you'll overwrite the changes which you made earlier in the transaction.
-Therefore, to avoid this problem, this method will only re-fetch the given object from the database if it has not yet been fetched within the current transaction.</p>
-<p>Note: the current implementation of caching should not require this method.
-We're investigating if it's still necessary or not. If not it might get deprecated soon.</p>
-<h3 id="has_already_been_read"><code>has_already_been_read</code></h3>
-<pre><code class="language-python">has_already_been_read(instance) -&gt; bool
-</code></pre>
-<p>This method tells you whether or not the given Django model instance has been read from the database within the current transaction.</p>
-<h2 id="example-usage">Example usage</h2>
-<pre><code class="language-python">from gclouc.db.transaction import atomic, current_transaction, on_commit
-
-# Using atomic() as a context manager
-counter = MyCounter.objects.get(pk=1)
-with atomic() as transaction:
-    on_commit(log_counter_increment)  # Will only happen if the transaction is successful
-    transaction.refresh_if_unread(counter)
-    counter.count = counter.count + 1
-    counter.save()
-
-# Using atomic() as a decorator
-@atomic()
-def increment_counter(counter):
-    transaction = current_transaction()
-    on_commit(log_counter_increment)  # Will only happen if the transaction is successful
-    transaction.refresh_if_unread(obj)
-    counter.count = counter.count + 1
-    counter.save()
-
-counter = MyCounter.objects.get(pk=1)
-increment_counter(counter)
-
-def log_counter_increment():
-    logging.info(&quot;Incremented counter!&quot;)
-</code></pre>
+                <h1 id="firestore">Firestore</h1>
+<p>Generally Firestore in Datastore mode seems to provide a better "normal" database experience than Firestore in native mode,
+so it is assumed that most users of <code>gcloudc</code> will use the Datastore connector.
+However, Firestore's native mode has the benefits of its realtime functionality, which may be a significant advantage for some use cases.</p>
+<p>If you're using Firestore in native mode, beware of the following limitations.</p>
+<h2 id="primary-keys-are-stored-as-strings">Primary keys are stored as strings</h2>
+<p>Firestore always stores the primary key field as a string,
+so if you don't override the primary key field on your models then you will get Django's default <code>AutoField</code>,
+which may cause surprises.</p>
+<p>The <code>AutoField</code> tries to store an integer.
+In order to make sorting work correctly, <code>gcloudc</code> will pad the integer with zeros so that all values are the same length.
+This means that <code>str(obj.pk)</code>, as might be used in a URL path,
+will not necessarily give you the correct value to query for the object directly in the Firestore web console at
+<a href="https://console.cloud.google.com">console.cloud.google.com</a>.</p>
+<p>To avoid this problem, one solution is to use the supplied <code>AutoCharField</code>. E.g.:</p>
+<pre><code class="language-python">from gcloudc.db.models.fields.firestore import AutoCharField
+
+class MyModel(models.Model):
+
+    id = AutoCharField(primary_key=True)
+</code></pre>
+<p>This generates ID values in the same format that Firestore generates automatically.</p>
+<p>Alternatively you can use Django's <code>UUIDField</code> for your primary keys.</p>
+<h2 id="you-cant-sort-by-pk-descending">You can't sort by PK descending</h2>
+<p>Currently, sorting a query by primary key descending is not allowed.
+To get around this you need to duplicate the primary key onto a separate field and then order by that field.
+For example:</p>
+<pre><code class="language-python">from gcloudc.db.backends.firestore.transaction import Transaction
+
+class DenormalizedPK(models.Model):
+    uid = models.CharField(max_length=64, editable=False)
+
+    class Meta:
+        abstract = True
+
+    def save(self, *args, **kwargs):
+        if not self.pk:
+            # H! This generates a Firestore ID so that we can denormalize before save.
+            self.pk = Transaction(connection, None)._generate_id(str)
+
+        self.uid = self.pk
+        return super().save(*args, **kwargs)
+</code></pre>
+<h2 id="indexes-are-not-generated-by-the-local-emulator">Indexes are not generated by the local emulator</h2>
+<p>Unlike with the Datastore emulator, the local Firestore emulator does not generate index definitions for you.
+However, it does provide a URL on localhost from which the indexes which would be required for
+queries which have been performed during the current run of the emulator.
+These indexes are provided in a different format to the one required in the <code>firestore.indexes.json</code>
+file in which you must provide your index definitions for deployment.</p>
+<p>To extract these indexes from the emulator and merge them into your <code>firestore.indexes.json</code> file in
+the correct format, <code>gcloudc</code> provides a utility <code>gcloudc.utils.firestore_indexes.update_firestore_indexes</code>.</p>
+<pre><code class="language-python">update_firestore_indexes(
+    emulator_project,
+    emulator_config=&quot;firebase.json&quot;,
+    indexes_file=&quot;firestore.indexes.json&quot;
+)
+</code></pre>
+<p>You might want to call this in <code>manage.py</code> before shutdown, perhaps only for certain commands,
+or perhaps call it in specific tests. It's up to you.</p>
+<p>Note that the <code>emulator_project</code> argument appears to need to be the name of the project that the
+emulator was started with, even if you're using the emulator in multi-project mode.
+Presumably this may change in the future.</p>
               
             </div>
           </div><footer>
     <div class="rst-footer-buttons" role="navigation" aria-label="Footer Navigation">
-        <a href="../field_indexes/" class="btn btn-neutral float-left" title="Field Indexes"><span class="icon icon-circle-arrow-left"></span> Previous</a>
-        <a href="../caching/" class="btn btn-neutral float-right" title="Caching">Next <span class="icon icon-circle-arrow-right"></span></a>
+        <a href="../caching/" class="btn btn-neutral float-left" title="Caching"><span class="icon icon-circle-arrow-left"></span> Previous</a>
+        <a href="../contributing/" class="btn btn-neutral float-right" title="Contributing & Testing">Next <span class="icon icon-circle-arrow-right"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <!-- Copyright etc -->
   </div>
@@ -243,18 +205,18 @@
   <span class="rst-current-version" data-toggle="rst-current-version">
     
         <span>
           <a href="https://gitlab.com/potato-oss/google-cloud/django-gcloud-connectors/" class="icon icon-gitlab" style="color: #fcfcfc"> GitLab</a>
         </span>
     
     
-      <span><a href="../field_indexes/" style="color: #fcfcfc">&laquo; Previous</a></span>
+      <span><a href="../caching/" style="color: #fcfcfc">&laquo; Previous</a></span>
     
     
-      <span><a href="../caching/" style="color: #fcfcfc">Next &raquo;</a></span>
+      <span><a href="../contributing/" style="color: #fcfcfc">Next &raquo;</a></span>
     
   </span>
 </div>
     <script src="../js/jquery-3.6.0.min.js"></script>
     <script>var base_url = "..";</script>
     <script src="../js/theme_extra.js"></script>
     <script src="../js/theme.js"></script>
```

#### html2text {}

```diff
@@ -2,130 +2,88 @@
 [q                   ]
     * _H_o_m_e
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _C_o_n_c_e_p_t_s_ _&_ _l_i_m_i_t_a_t_i_o_n_s
     * _F_i_e_l_d_s
     * _F_i_e_l_d_ _I_n_d_e_x_e_s
     * _T_r_a_n_s_a_c_t_i_o_n_s
-          o _a_t_o_m_i_c
-          o _n_o_n___a_t_o_m_i_c
-          o _i_n___a_t_o_m_i_c___b_l_o_c_k
-          o _o_n___c_o_m_m_i_t
-          o _T_r_a_n_s_a_c_t_i_o_n_ _o_b_j_e_c_t_s
-                # _r_e_f_r_e_s_h___i_f___u_n_r_e_a_d
-                # _h_a_s___a_l_r_e_a_d_y___b_e_e_n___r_e_a_d
-          o _E_x_a_m_p_l_e_ _u_s_a_g_e
     * _C_a_c_h_i_n_g
+    * _F_i_r_e_s_t_o_r_e
+          o _P_r_i_m_a_r_y_ _k_e_y_s_ _a_r_e_ _s_t_o_r_e_d_ _a_s_ _s_t_r_i_n_g_s
+          o _Y_o_u_ _c_a_n_'_t_ _s_o_r_t_ _b_y_ _P_K_ _d_e_s_c_e_n_d_i_n_g
+          o _I_n_d_e_x_e_s_ _a_r_e_ _n_o_t_ _g_e_n_e_r_a_t_e_d_ _b_y_ _t_h_e_ _l_o_c_a_l_ _e_m_u_l_a_t_o_r
     * _C_o_n_t_r_i_b_u_t_i_n_g_ _&_ _T_e_s_t_i_n_g
     * _C_o_m_m_e_r_c_i_a_l_ _S_u_p_p_o_r_t
     * _W_o_r_k_ _w_i_t_h_ _u_s_!
 _D_j_a_n_g_o_ _G_c_l_o_u_d_ _C_o_n_n_e_c_t_o_r_s_ _D_o_c_u_m_e_n_t_a_t_i_o_n
-    * Transactions
+    * Firestore
     * _E_d_i_t_ _o_n_ _G_i_t_L_a_b
 ===============================================================================
-************ TTrraannssaaccttiioonnss ************
-Transactions on the Cloud Datastore behave differently to those of a SQL
-database. It's worth reading the _C_l_o_u_d_ _D_a_t_a_s_t_o_r_e_ _t_r_a_n_s_a_c_t_i_o_n_s_ _d_o_c_u_m_e_n_t_a_t_i_o_n to
-familiarise yourself with their behaviour. Crucially:
-     "queries and lookups inside a Datastore mode transaction do nnoott see
-     the results of previous writes inside that transaction".
-This is partially mitigated by our caching system. For more info on how
-querying and caching work when using gcloudc.db.transaction see the _c_a_c_h_i_n_g
-docs.
-DDjjaannggoo''ss atomic ddeeccoorraattoorr//ccoonntteexxtt mmaannaaggeerr wwiillll hhaavvee nnoo eeffffeecctt oonn tthhee DDaattaassttoorree..
-However, gcloudc.db.transaction provides a separate set of decorators/context
-managers for managing transactions.
-********** aattoommiicc **********
-atomic(
-    independent=False,
-    mandatory=False,
-    using="default",
-    read_only=False,
-    enable_cache=True,
-) -> Transaction
-This can be used either as a decorator or a context manager to execute a block
-of code within a Datastore transaction.
-If used as a context manager, it will return the Transaction object. If used as
-a function decorator, you will need to call current_transaction() to get the
-Transaction object.
-See _T_r_a_n_s_a_c_t_i_o_n_ _o_b_j_e_c_t.
-The kwargs are:
-    * independent: forces the start of a new, independent transaction, even if
-      you are currently already in a transaction.
-    * mandatory: forces a check to ensure that you are already within an outer
-      transaction. Raises TransactionFailedError if not.
-    * using: the database connection name to use (works the same as Django's
-      using parameter for database operations).
-    * read_only: for creating a read-only transaction. This functionality is
-      not yet implemented.
-    * enable_cache: enables gcloudc's caching of queries which can only return
-      a singular, unique result.
-For more info on caching and transactions see the _c_a_c_h_i_n_g docs
-********** nnoonn__aattoommiicc **********
-non_atomic(using="default")
-This can be used either as a decorator or a context manager to break out and
-execute a block of code outside of the current transaction.
-********** iinn__aattoommiicc__bblloocckk **********
-in_atomic_block(using="default") -> bool
-This function tells you whether or not you are currently inside an atomic
-transaction.
-********** oonn__ccoommmmiitt **********
-on_commit(func, using=None)
-The same as Django's on_commit, this registers a function to be called when the
-current transaction is committed. If the current transaction is rolled back,
-func will not be called.
-********** TTrraannssaaccttiioonn oobbjjeeccttss **********
-When using atomic as a context manager, or using current_transaction(), you
-will get a Transaction object. This can and should be used to perform
-operations within the transaction.
-A Transaction object has the following methods:
-******** rreeffrreesshh__iiff__uunnrreeaadd ********
-refresh_if_unread(instance) -> None
-This method should be used to refresh instances of Django models from the
-database.
-Remember that "queries and lookups inside a Datastore mode transaction do nnoott
-see the results of previous writes inside that transaction", therefore, if you
-query for an object inside a transaction, then modify it, save it and fetch it
-from the DB again, the object that you get back will be the original
-(unmodified) version, as it existed before the transaction started. So if you
-then modify and save the object again, you'll overwrite the changes which you
-made earlier in the transaction. Therefore, to avoid this problem, this method
-will only re-fetch the given object from the database if it has not yet been
-fetched within the current transaction.
-Note: the current implementation of caching should not require this method.
-We're investigating if it's still necessary or not. If not it might get
-deprecated soon.
-******** hhaass__aallrreeaaddyy__bbeeeenn__rreeaadd ********
-has_already_been_read(instance) -> bool
-This method tells you whether or not the given Django model instance has been
-read from the database within the current transaction.
-********** EExxaammppllee uussaaggee **********
-from gclouc.db.transaction import atomic, current_transaction, on_commit
-
-# Using atomic() as a context manager
-counter = MyCounter.objects.get(pk=1)
-with atomic() as transaction:
-    on_commit(log_counter_increment)  # Will only happen if the transaction is
-successful
-    transaction.refresh_if_unread(counter)
-    counter.count = counter.count + 1
-    counter.save()
-
-# Using atomic() as a decorator
-@atomic()
-def increment_counter(counter):
-    transaction = current_transaction()
-    on_commit(log_counter_increment)  # Will only happen if the transaction is
-successful
-    transaction.refresh_if_unread(obj)
-    counter.count = counter.count + 1
-    counter.save()
+************ FFiirreessttoorree ************
+Generally Firestore in Datastore mode seems to provide a better "normal"
+database experience than Firestore in native mode, so it is assumed that most
+users of gcloudc will use the Datastore connector. However, Firestore's native
+mode has the benefits of its realtime functionality, which may be a significant
+advantage for some use cases.
+If you're using Firestore in native mode, beware of the following limitations.
+********** PPrriimmaarryy kkeeyyss aarree ssttoorreedd aass ssttrriinnggss **********
+Firestore always stores the primary key field as a string, so if you don't
+override the primary key field on your models then you will get Django's
+default AutoField, which may cause surprises.
+The AutoField tries to store an integer. In order to make sorting work
+correctly, gcloudc will pad the integer with zeros so that all values are the
+same length. This means that str(obj.pk), as might be used in a URL path, will
+not necessarily give you the correct value to query for the object directly in
+the Firestore web console at _c_o_n_s_o_l_e_._c_l_o_u_d_._g_o_o_g_l_e_._c_o_m.
+To avoid this problem, one solution is to use the supplied AutoCharField. E.g.:
+from gcloudc.db.models.fields.firestore import AutoCharField
 
-counter = MyCounter.objects.get(pk=1)
-increment_counter(counter)
+class MyModel(models.Model):
 
-def log_counter_increment():
-    logging.info("Incremented counter!")
+    id = AutoCharField(primary_key=True)
+This generates ID values in the same format that Firestore generates
+automatically.
+Alternatively you can use Django's UUIDField for your primary keys.
+********** YYoouu ccaann''tt ssoorrtt bbyy PPKK ddeesscceennddiinngg **********
+Currently, sorting a query by primary key descending is not allowed. To get
+around this you need to duplicate the primary key onto a separate field and
+then order by that field. For example:
+from gcloudc.db.backends.firestore.transaction import Transaction
+
+class DenormalizedPK(models.Model):
+    uid = models.CharField(max_length=64, editable=False)
+
+    class Meta:
+        abstract = True
+
+    def save(self, *args, **kwargs):
+        if not self.pk:
+            # H! This generates a Firestore ID so that we can denormalize
+before save.
+            self.pk = Transaction(connection, None)._generate_id(str)
+
+        self.uid = self.pk
+        return super().save(*args, **kwargs)
+********** IInnddeexxeess aarree nnoott ggeenneerraatteedd bbyy tthhee llooccaall eemmuullaattoorr **********
+Unlike with the Datastore emulator, the local Firestore emulator does not
+generate index definitions for you. However, it does provide a URL on localhost
+from which the indexes which would be required for queries which have been
+performed during the current run of the emulator. These indexes are provided in
+a different format to the one required in the firestore.indexes.json file in
+which you must provide your index definitions for deployment.
+To extract these indexes from the emulator and merge them into your
+firestore.indexes.json file in the correct format, gcloudc provides a utility
+gcloudc.utils.firestore_indexes.update_firestore_indexes.
+update_firestore_indexes(
+    emulator_project,
+    emulator_config="firebase.json",
+    indexes_file="firestore.indexes.json"
+)
+You might want to call this in manage.py before shutdown, perhaps only for
+certain commands, or perhaps call it in specific tests. It's up to you.
+Note that the emulator_project argument appears to need to be the name of the
+project that the emulator was started with, even if you're using the emulator
+in multi-project mode. Presumably this may change in the future.
 _P_r_e_v_i_o_u_s _N_e_x_t
 ===============================================================================
 Built with _M_k_D_o_c_s using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
 _G_i_t_L_a_b _«_ _P_r_e_v_i_o_u_s _N_e_x_t_ _»
```

### Comparing `django-gcloud-connectors-1.1.0/test/work_with_potato/index.html` & `django-gcloud-connectors-1.2.0/test/work_with_potato/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -64,23 +64,27 @@
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../caching/">Caching</a>
                 </li>
               </ul>
               <ul>
+                <li class="toctree-l1"><a class="reference internal" href="../firestore/">Firestore</a>
+                </li>
+              </ul>
+              <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../contributing/">Contributing & Testing</a>
                 </li>
               </ul>
               <ul>
                 <li class="toctree-l1"><a class="reference internal" href="../commercial_support/">Commercial Support</a>
                 </li>
               </ul>
               <ul class="current">
-                <li class="toctree-l1 current"><a class="reference internal current" href="./">Work with us!</a>
+                <li class="toctree-l1 current"><a class="reference internal current" href="#">Work with us!</a>
     <ul class="current">
     </ul>
                 </li>
               </ul>
       </div>
     </div>
     </nav>
```

#### html2text {}

```diff
@@ -3,14 +3,15 @@
     * _H_o_m_e
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _C_o_n_c_e_p_t_s_ _&_ _l_i_m_i_t_a_t_i_o_n_s
     * _F_i_e_l_d_s
     * _F_i_e_l_d_ _I_n_d_e_x_e_s
     * _T_r_a_n_s_a_c_t_i_o_n_s
     * _C_a_c_h_i_n_g
+    * _F_i_r_e_s_t_o_r_e
     * _C_o_n_t_r_i_b_u_t_i_n_g_ _&_ _T_e_s_t_i_n_g
     * _C_o_m_m_e_r_c_i_a_l_ _S_u_p_p_o_r_t
     * _W_o_r_k_ _w_i_t_h_ _u_s_!
 _D_j_a_n_g_o_ _G_c_l_o_u_d_ _C_o_n_n_e_c_t_o_r_s_ _D_o_c_u_m_e_n_t_a_t_i_o_n
     * Work with us!
     * _E_d_i_t_ _o_n_ _G_i_t_L_a_b
 ===============================================================================
```

