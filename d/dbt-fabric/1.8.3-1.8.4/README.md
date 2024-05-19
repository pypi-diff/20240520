# Comparing `tmp/dbt-fabric-1.8.3.tar.gz` & `tmp/dbt-fabric-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-fabric-1.8.3.tar", last modified: Thu Apr 25 00:47:46 2024, max compression
+gzip compressed data, was "dbt-fabric-1.8.4.tar", last modified: Sun May 19 23:23:21 2024, max compression
```

## Comparing `dbt-fabric-1.8.3.tar` & `dbt-fabric-1.8.4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.759906 dbt-fabric-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-25 00:47:46.759906 dbt-fabric-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.751906 dbt-fabric-1.8.3/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.751906 dbt-fabric-1.8.3/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.751906 dbt-fabric-1.8.3/dbt/adapters/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9641 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16541 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_connection_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_relation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.755906 dbt-fabric-1.8.3/dbt/adapters/fabric/relation_configs/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/relation_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/relation_configs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/adapters/fabric/relation_configs/policies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.751906 dbt-fabric-1.8.3/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.755906 dbt-fabric-1.8.3/dbt/include/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.751906 dbt-fabric-1.8.3/dbt/include/fabric/macros/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.755906 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/schema.sql
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/show.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.751906 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.751906 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.755906 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/incremental/incremental_strategies.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/incremental/merge.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.755906 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/table/clone.sql
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.755906 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.755906 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/seeds/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.755906 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.759906 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/tests/helpers.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.759906 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/get_tables_by_pattern.sql
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/dbt/include/fabric/macros/utils/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 00:47:46.759906 dbt-fabric-1.8.3/dbt_fabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-25 00:47:46.000000 dbt-fabric-1.8.3/dbt_fabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-04-25 00:47:46.000000 dbt-fabric-1.8.3/dbt_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 00:47:46.000000 dbt-fabric-1.8.3/dbt_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-25 00:47:46.000000 dbt-fabric-1.8.3/dbt_fabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-25 00:47:46.000000 dbt-fabric-1.8.3/dbt_fabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 00:47:46.759906 dbt-fabric-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-04-25 00:46:55.000000 dbt-fabric-1.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.025731 dbt-fabric-1.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-19 23:23:21.025731 dbt-fabric-1.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.013731 dbt-fabric-1.8.4/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.013731 dbt-fabric-1.8.4/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.017731 dbt-fabric-1.8.4/dbt/adapters/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/adapters/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/adapters/fabric/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9641 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/adapters/fabric/fabric_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/adapters/fabric/fabric_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/adapters/fabric/fabric_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16541 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/adapters/fabric/fabric_connection_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/adapters/fabric/fabric_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/adapters/fabric/fabric_relation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.017731 dbt-fabric-1.8.4/dbt/adapters/fabric/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/adapters/fabric/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/adapters/fabric/relation_configs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/adapters/fabric/relation_configs/policies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.013731 dbt-fabric-1.8.4/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.017731 dbt-fabric-1.8.4/dbt/include/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.017731 dbt-fabric-1.8.4/dbt/include/fabric/macros/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.017731 dbt-fabric-1.8.4/dbt/include/fabric/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/adapters/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/adapters/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/adapters/show.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.017731 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.013731 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.021731 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/incremental/incremental_strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/incremental/merge.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.021731 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/table/clone.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.021731 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.021731 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/seeds/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.021731 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.021731 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/tests/helpers.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.021731 dbt-fabric-1.8.4/dbt/include/fabric/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/utils/get_tables_by_pattern.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/dbt/include/fabric/macros/utils/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:23:21.025731 dbt-fabric-1.8.4/dbt_fabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-19 23:23:20.000000 dbt-fabric-1.8.4/dbt_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-19 23:23:20.000000 dbt-fabric-1.8.4/dbt_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 23:23:20.000000 dbt-fabric-1.8.4/dbt_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-19 23:23:20.000000 dbt-fabric-1.8.4/dbt_fabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 23:23:20.000000 dbt-fabric-1.8.4/dbt_fabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 23:23:21.025731 dbt-fabric-1.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3362 2024-05-19 23:22:39.000000 dbt-fabric-1.8.4/setup.py
```

### Comparing `dbt-fabric-1.8.3/LICENSE` & `dbt-fabric-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/PKG-INFO` & `dbt-fabric-1.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-fabric
-Version: 1.8.3
+Version: 1.8.4
 Summary: A Microsoft Fabric Synapse Data Warehouse adapter plugin for dbt
 Home-page: https://github.com/microsoft/dbt-fabric
 Author: Pradeep Srikakolapu
 License: MIT
 Project-URL: Setup & configuration, https://docs.getdbt.com/reference/warehouse-profiles/fabric-profile
 Project-URL: Documentation & usage, https://docs.getdbt.com/reference/resource-configs/fabric-configs
 Project-URL: Changelog, https://github.com/microsoft/dbt-fabric/blob/master/CHANGELOG.md
```

### Comparing `dbt-fabric-1.8.3/README.md` & `dbt-fabric-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/adapters/fabric/__init__.py` & `dbt-fabric-1.8.4/dbt/adapters/fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_adapter.py` & `dbt-fabric-1.8.4/dbt/adapters/fabric/fabric_adapter.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_column.py` & `dbt-fabric-1.8.4/dbt/adapters/fabric/fabric_column.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_connection_manager.py` & `dbt-fabric-1.8.4/dbt/adapters/fabric/fabric_connection_manager.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_credentials.py` & `dbt-fabric-1.8.4/dbt/adapters/fabric/fabric_credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/adapters/fabric/fabric_relation.py` & `dbt-fabric-1.8.4/dbt/adapters/fabric/fabric_relation.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/adapters/fabric/relation_configs/base.py` & `dbt-fabric-1.8.4/dbt/adapters/fabric/relation_configs/base.py`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/apply_grants.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/catalog.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/adapters/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/columns.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/indexes.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/metadata.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/relation.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/adapters/schema.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/incremental/incremental.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/incremental/merge.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/table/clone.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/table/clone.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/table/columns_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/table/table.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/models/view/view.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/models/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/seeds/helpers.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/snapshots/helpers.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/snapshots/snapshot.sql`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,18 @@
                                                to_relation=target_relation) %}
       {% set missing_columns = adapter.get_missing_columns(staging_table, target_relation)
                                    | rejectattr('name', 'equalto', 'dbt_change_type')
                                    | rejectattr('name', 'equalto', 'DBT_CHANGE_TYPE')
                                    | rejectattr('name', 'equalto', 'dbt_unique_key')
                                    | rejectattr('name', 'equalto', 'DBT_UNIQUE_KEY')
                                    | list %}
-      {% do create_columns(target_relation, missing_columns) %}
+      {% if missing_columns|length > 0 %}
+        {{log("Missing columns length is: "~ missing_columns|length)}}
+        {% do create_columns(target_relation, missing_columns) %}
+      {% endif %}
       {% set source_columns = adapter.get_columns_in_relation(staging_table)
                                    | rejectattr('name', 'equalto', 'dbt_change_type')
                                    | rejectattr('name', 'equalto', 'DBT_CHANGE_TYPE')
                                    | rejectattr('name', 'equalto', 'dbt_unique_key')
                                    | rejectattr('name', 'equalto', 'DBT_UNIQUE_KEY')
                                    | list %}
       {% set quoted_source_columns = [] %}
```

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/dbt/include/fabric/macros/materializations/tests/helpers.sql` & `dbt-fabric-1.8.4/dbt/include/fabric/macros/materializations/tests/helpers.sql`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% macro fabric__get_test_sql(main_sql, fail_calc, warn_if, error_if, limit) -%}
 
   {% if main_sql.strip().lower().startswith('with') %}
     {% set testview %}
-      {{ generate_schema_name('tests_schema') }}.testview_{{ range(1300, 19000) | random }}
+      {{ config.get('schema') }}.testview_{{ range(1300, 19000) | random }}
     {% endset %}
 
     {% set sql = main_sql.replace("'", "''")%}
 
     EXEC('create view {{testview}} as {{ sql }};')
     select
       {{ "top (" ~ limit ~ ')' if limit != none }}
```

### Comparing `dbt-fabric-1.8.3/dbt_fabric.egg-info/PKG-INFO` & `dbt-fabric-1.8.4/dbt_fabric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-fabric
-Version: 1.8.3
+Version: 1.8.4
 Summary: A Microsoft Fabric Synapse Data Warehouse adapter plugin for dbt
 Home-page: https://github.com/microsoft/dbt-fabric
 Author: Pradeep Srikakolapu
 License: MIT
 Project-URL: Setup & configuration, https://docs.getdbt.com/reference/warehouse-profiles/fabric-profile
 Project-URL: Documentation & usage, https://docs.getdbt.com/reference/resource-configs/fabric-configs
 Project-URL: Changelog, https://github.com/microsoft/dbt-fabric/blob/master/CHANGELOG.md
```

### Comparing `dbt-fabric-1.8.3/dbt_fabric.egg-info/SOURCES.txt` & `dbt-fabric-1.8.4/dbt_fabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-fabric-1.8.3/setup.py` & `dbt-fabric-1.8.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,17 @@
     author=", ".join(authors_list),
     url="https://github.com/microsoft/dbt-fabric",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "pyodbc>=4.0.35,<5.2.0",
         "azure-identity>=1.12.0",
-        "dbt-common>=0.1.0a1,<2.0",
-        "dbt-core>=1.8.0a1",
-        "dbt-adapters>=0.1.0a1,<2.0",
+        "dbt-common>=1.0.4,<2.0",
+        "dbt-core==1.8.0",
+        "dbt-adapters>=1.1.1,<2.0",
     ],
     cmdclass={
         "verify": VerifyVersionCommand,
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
```

