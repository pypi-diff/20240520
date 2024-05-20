# Comparing `tmp/digitalhub_core-0.4.0b8.tar.gz` & `tmp/digitalhub_core-0.5.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_core-0.4.0b8.tar", last modified: Tue May 14 10:36:05 2024, max compression
+gzip compressed data, was "digitalhub_core-0.5.0b0.tar", last modified: Mon May 20 12:48:09 2024, max compression
```

## Comparing `digitalhub_core-0.4.0b8.tar` & `digitalhub_core-0.5.0b0.tar`

### file list

```diff
@@ -1,129 +1,122 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:05.005934 digitalhub_core-0.4.0b8/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub_core-0.4.0b8/LICENSE.txt
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    15054 2024-05-14 10:36:05.005934 digitalhub_core-0.4.0b8/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      499 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.957934 digitalhub_core-0.4.0b8/digitalhub_core/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1259 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.961934 digitalhub_core-0.4.0b8/digitalhub_core/client/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/client/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2352 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/client/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.961934 digitalhub_core-0.4.0b8/digitalhub_core/client/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-10-10 11:19:53.000000 digitalhub_core-0.4.0b8/digitalhub_core/client/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1166 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/client/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8892 2024-05-02 13:03:59.000000 digitalhub_core-0.4.0b8/digitalhub_core/client/objects/dhcore.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16292 2024-05-13 12:38:37.000000 digitalhub_core-0.4.0b8/digitalhub_core/client/objects/local.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.965934 digitalhub_core-0.4.0b8/digitalhub_core/context/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/context/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3098 2024-03-12 14:22:03.000000 digitalhub_core-0.4.0b8/digitalhub_core/context/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2926 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/context/context.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.965934 digitalhub_core-0.4.0b8/digitalhub_core/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.969934 digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1521 2024-02-05 10:28:22.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3172 2024-05-02 12:54:20.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2485 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1567 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.969934 digitalhub_core-0.4.0b8/digitalhub_core/entities/_builders/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-27 11:31:31.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_builders/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-05-06 11:10:34.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_builders/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1435 2024-05-06 11:10:34.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_builders/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1748 2024-05-06 11:10:34.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/_builders/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.973934 digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6641 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14010 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      339 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1876 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      322 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/status.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-05-06 11:13:11.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/entity_types.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.977934 digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6298 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16737 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1699 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-22 07:49:08.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.977934 digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8705 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    22032 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1467 2024-02-29 07:59:41.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:23.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/status.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      927 2024-05-06 11:13:11.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.981934 digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4897 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14326 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3532 2024-05-09 11:08:45.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2620 2024-05-13 12:22:42.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.985934 digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:39:09.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6160 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8742 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      221 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      746 2024-02-15 09:49:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-02-15 09:23:29.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.989934 digitalhub_core-0.4.0b8/digitalhub_core/entities/services/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:49:32.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/services/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6121 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/services/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     7385 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/services/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/services/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      368 2024-02-15 09:49:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/services/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:37.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/services/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.993934 digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5550 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    10643 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5151 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      431 2024-03-19 10:12:26.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      206 2023-11-17 12:02:01.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.993934 digitalhub_core-0.4.0b8/digitalhub_core/entities/workflows/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/workflows/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6358 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/workflows/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16023 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/workflows/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/workflows/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      295 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/workflows/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:47.000000 digitalhub_core-0.4.0b8/digitalhub_core/entities/workflows/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.993934 digitalhub_core-0.4.0b8/digitalhub_core/registry/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/registry/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1468 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/registry/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1866 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/registry/registry.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3714 2024-05-06 11:10:35.000000 digitalhub_core-0.4.0b8/digitalhub_core/registry/utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.997934 digitalhub_core-0.4.0b8/digitalhub_core/runtimes/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-05 11:37:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/runtimes/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3931 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/runtimes/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1005 2024-05-06 11:10:34.000000 digitalhub_core-0.4.0b8/digitalhub_core/runtimes/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.997934 digitalhub_core-0.4.0b8/digitalhub_core/stores/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/stores/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6767 2024-05-13 12:39:44.000000 digitalhub_core-0.4.0b8/digitalhub_core/stores/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:04.997934 digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4587 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4508 2024-03-12 13:41:08.000000 digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/local.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5039 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/remote.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8844 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/s3.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8927 2024-04-19 08:14:45.000000 digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/sql.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:05.001934 digitalhub_core-0.4.0b8/digitalhub_core/utils/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3646 2024-03-12 14:23:02.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/api.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2215 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/env_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      346 2023-12-11 08:31:30.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/exceptions.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1332 2024-04-08 14:07:02.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/file_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4237 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/generic_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3054 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/git_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-02-01 10:08:51.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/io_utils.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      460 2023-11-21 13:33:17.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/logger.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      805 2024-04-23 09:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core/utils/uri_utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 10:36:05.001934 digitalhub_core-0.4.0b8/digitalhub_core.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    15054 2024-05-14 10:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4165 2024-05-14 10:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-14 10:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      250 2024-05-14 10:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-14 10:36:04.000000 digitalhub_core-0.4.0b8/digitalhub_core.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1731 2024-05-13 12:41:00.000000 digitalhub_core-0.4.0b8/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-14 10:36:05.005934 digitalhub_core-0.4.0b8/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.206920 digitalhub_core-0.5.0b0/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub_core-0.5.0b0/LICENSE.txt
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    15054 2024-05-20 12:48:09.206920 digitalhub_core-0.5.0b0/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      499 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.190919 digitalhub_core-0.5.0b0/digitalhub_core/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1259 2024-05-20 09:51:08.000000 digitalhub_core-0.5.0b0/digitalhub_core/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.190919 digitalhub_core-0.5.0b0/digitalhub_core/client/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/client/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2352 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/client/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.190919 digitalhub_core-0.5.0b0/digitalhub_core/client/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-10-10 11:19:53.000000 digitalhub_core-0.5.0b0/digitalhub_core/client/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1166 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/client/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8892 2024-05-02 13:03:59.000000 digitalhub_core-0.5.0b0/digitalhub_core/client/objects/dhcore.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16292 2024-05-13 12:38:37.000000 digitalhub_core-0.5.0b0/digitalhub_core/client/objects/local.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.190919 digitalhub_core-0.5.0b0/digitalhub_core/context/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/context/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3098 2024-03-12 14:22:03.000000 digitalhub_core-0.5.0b0/digitalhub_core/context/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2926 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/context/context.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.194919 digitalhub_core-0.5.0b0/digitalhub_core/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.194919 digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1521 2024-02-05 10:28:22.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3172 2024-05-02 12:54:20.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2485 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1567 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.194919 digitalhub_core-0.5.0b0/digitalhub_core/entities/_builders/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-27 11:31:31.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_builders/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_builders/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1435 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_builders/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1748 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/_builders/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.194919 digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6641 2024-05-20 09:51:08.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14010 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      339 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1876 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      322 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/status.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      318 2024-05-06 11:13:11.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/entity_types.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.198919 digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6298 2024-05-20 09:51:08.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16737 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1699 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-22 07:49:08.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.198919 digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8705 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    22032 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      224 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1467 2024-02-29 07:59:41.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-02-15 09:23:23.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/status.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      927 2024-05-06 11:13:11.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.198919 digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4897 2024-05-20 09:51:08.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    14326 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3532 2024-05-09 11:08:45.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2620 2024-05-13 12:22:42.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.198919 digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-02-06 10:39:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6160 2024-05-20 09:51:08.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8742 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      221 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      746 2024-02-15 09:49:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      212 2024-02-15 09:23:29.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.202919 digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5550 2024-05-20 09:51:08.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    10643 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      215 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5151 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      431 2024-03-19 10:12:26.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      206 2023-11-17 12:02:01.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.202919 digitalhub_core-0.5.0b0/digitalhub_core/entities/workflows/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/workflows/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6358 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/workflows/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    16023 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/workflows/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      227 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/workflows/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      295 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/workflows/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      218 2024-02-15 09:23:47.000000 digitalhub_core-0.5.0b0/digitalhub_core/entities/workflows/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.202919 digitalhub_core-0.5.0b0/digitalhub_core/registry/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/registry/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1468 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/registry/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1866 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/registry/registry.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3714 2024-05-06 11:10:35.000000 digitalhub_core-0.5.0b0/digitalhub_core/registry/utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.202919 digitalhub_core-0.5.0b0/digitalhub_core/runtimes/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-09-05 11:37:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/runtimes/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3931 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/runtimes/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1005 2024-05-06 11:10:34.000000 digitalhub_core-0.5.0b0/digitalhub_core/runtimes/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.202919 digitalhub_core-0.5.0b0/digitalhub_core/stores/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/stores/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6767 2024-05-20 09:51:09.000000 digitalhub_core-0.5.0b0/digitalhub_core/stores/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.206920 digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4587 2024-04-19 08:14:45.000000 digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4508 2024-03-12 13:41:08.000000 digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/local.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     5039 2024-04-19 08:14:45.000000 digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/remote.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8844 2024-04-19 08:14:45.000000 digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/s3.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     8927 2024-04-19 08:14:45.000000 digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/sql.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.206920 digitalhub_core-0.5.0b0/digitalhub_core/utils/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2023-07-13 10:23:55.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3646 2024-03-12 14:23:02.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/api.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2215 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/env_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      346 2023-12-11 08:31:30.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/exceptions.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1332 2024-04-08 14:07:02.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/file_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     4237 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/generic_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3054 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/git_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1794 2024-02-01 10:08:51.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/io_utils.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      460 2023-11-21 13:33:17.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/logger.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      805 2024-04-23 09:36:04.000000 digitalhub_core-0.5.0b0/digitalhub_core/utils/uri_utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-20 12:48:09.206920 digitalhub_core-0.5.0b0/digitalhub_core.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    15054 2024-05-20 12:48:09.000000 digitalhub_core-0.5.0b0/digitalhub_core.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3901 2024-05-20 12:48:09.000000 digitalhub_core-0.5.0b0/digitalhub_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-20 12:48:09.000000 digitalhub_core-0.5.0b0/digitalhub_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      250 2024-05-20 12:48:09.000000 digitalhub_core-0.5.0b0/digitalhub_core.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-20 12:48:09.000000 digitalhub_core-0.5.0b0/digitalhub_core.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1731 2024-05-20 07:16:51.000000 digitalhub_core-0.5.0b0/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-20 12:48:09.206920 digitalhub_core-0.5.0b0/setup.cfg
```

### Comparing `digitalhub_core-0.4.0b8/LICENSE.txt` & `digitalhub_core-0.5.0b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/PKG-INFO` & `digitalhub_core-0.5.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-core
-Version: 0.4.0b8
+Version: 0.5.0b0
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/__init__.py` & `digitalhub_core-0.5.0b0/digitalhub_core/__init__.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/client/builder.py` & `digitalhub_core-0.5.0b0/digitalhub_core/client/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/client/objects/base.py` & `digitalhub_core-0.5.0b0/digitalhub_core/client/objects/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/client/objects/dhcore.py` & `digitalhub_core-0.5.0b0/digitalhub_core/client/objects/dhcore.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/client/objects/local.py` & `digitalhub_core-0.5.0b0/digitalhub_core/client/objects/local.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/context/builder.py` & `digitalhub_core-0.5.0b0/digitalhub_core/context/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/context/context.py` & `digitalhub_core-0.5.0b0/digitalhub_core/context/context.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/base.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/entity.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/metadata.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/spec.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/_base/status.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/_base/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/_builders/metadata.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/_builders/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/_builders/spec.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/_builders/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/_builders/status.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/_builders/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/crud.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/entity.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/artifacts/spec.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/artifacts/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/crud.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/entity.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/functions/spec.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/functions/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/crud.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/entity.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/projects/spec.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/registries.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/crud.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/entity.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/spec.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/runs/status.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/runs/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/crud.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/entity.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/secrets/spec.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/secrets/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/services/crud.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/workflows/crud.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,134 +1,132 @@
 """
-Service operations module.
+Workflow operations module.
 """
 from __future__ import annotations
 
 import typing
 
 from digitalhub_core.context.builder import check_context, get_context
 from digitalhub_core.entities.entity_types import EntityTypes
-from digitalhub_core.entities.services.entity import service_from_dict, service_from_parameters
+from digitalhub_core.entities.workflows.entity import workflow_from_dict, workflow_from_parameters
 from digitalhub_core.utils.api import api_ctx_delete, api_ctx_list, api_ctx_read, api_ctx_update
 from digitalhub_core.utils.io_utils import read_yaml
 
 if typing.TYPE_CHECKING:
-    from digitalhub_core.entities.services.entity import Service
+    from digitalhub_core.entities.workflows.entity import Workflow
 
 
-ENTITY_TYPE = EntityTypes.SERVICES.value
+ENTITY_TYPE = EntityTypes.WORKFLOWS.value
 
 
-def create_service(**kwargs) -> Service:
+def create_workflow(**kwargs) -> Workflow:
     """
-    Create a new Service instance with the specified parameters.
+    Create a new Workflow instance with the specified parameters.
 
     Parameters
     ----------
     **kwargs
         Keyword arguments.
 
     Returns
     -------
-    Service
-        An instance of the created service.
+    Workflow
+        An instance of the created workflow.
     """
-    return service_from_parameters(**kwargs)
+    return workflow_from_parameters(**kwargs)
 
 
-def create_service_from_dict(obj: dict) -> Service:
+def create_workflow_from_dict(obj: dict) -> Workflow:
     """
-    Create a new Service instance from a dictionary.
+    Create a new Workflow instance from a dictionary.
 
     Parameters
     ----------
     obj : dict
         Dictionary to create object from.
 
     Returns
     -------
-    Service
-        Service object.
+    Workflow
+        Workflow object.
     """
     check_context(obj.get("project"))
-    return service_from_dict(obj)
+    return workflow_from_dict(obj)
 
 
-def new_service(
+def new_workflow(
     project: str,
     name: str,
     kind: str,
     uuid: str | None = None,
     description: str | None = None,
-    source: str | None = None,
+    git_source: str | None = None,
     labels: list[str] | None = None,
     embedded: bool = True,
     **kwargs,
-) -> Service:
+) -> Workflow:
     """
-    Create a new Service instance with the specified parameters.
+    Create a new Workflow instance with the specified parameters.
 
     Parameters
     ----------
     project : str
-        A string representing the project associated with this service.
+        A string representing the project associated with this workflow.
     name : str
-        The name of the service.
-    kind : str
-        Kind of the object.
+        The name of the workflow.
     uuid : str
         ID of the object in form of UUID.
     description : str
-        A description of the service.
-    source : str
-        Remote git source for object.
+        A description of the workflow.
     labels : list[str]
         List of labels.
     embedded : bool
         Flag to determine if object must be embedded in project.
     **kwargs
         Spec keyword arguments.
 
     Returns
     -------
-    Service
-        An instance of the created service.
+    Workflow
+        An instance of the created workflow.
     """
-    obj = create_service(
+    obj = create_workflow(
         project=project,
         name=name,
         kind=kind,
         uuid=uuid,
         description=description,
-        source=source,
+        git_source=git_source,
         labels=labels,
         embedded=embedded,
         **kwargs,
     )
     obj.save()
     return obj
 
 
-def get_service(project: str, entity_name: str | None = None, entity_id: str | None = None, **kwargs) -> Service:
+def get_workflow(project: str, entity_name: str | None = None, entity_id: str | None = None, **kwargs) -> Workflow:
     """
-    Retrieves service details from backend.
+    Retrieves workflow details from backend.
 
     Parameters
     ----------
 
     project : str
         Project name.
-    name : str
-        The name of the service.
+    entity_name : str
+        Entity name.
+    entity_id : str
+        Entity ID.
     uuid : str
         ID of the object in form of UUID.
 
     Returns
     -------
-    Service
+    Workflow
         Object instance.
     """
     if (entity_id is None) and (entity_name is None):
         raise ValueError("Either entity_name or entity_id must be provided.")
 
     context = get_context(project)
 
@@ -139,36 +137,46 @@
 
         api = api_ctx_list(project, ENTITY_TYPE)
         kwargs["params"]["name"] = entity_name
         obj = context.list_objects(api, **kwargs)[0]
     else:
         api = api_ctx_read(project, ENTITY_TYPE, entity_id)
         obj = context.read_object(api, **kwargs)
-    return create_service_from_dict(obj)
+    return create_workflow_from_dict(obj)
 
 
-def import_service(file: str) -> Service:
+def import_workflow(file: str) -> Workflow:
     """
-    Import an Service object from a file using the specified file path.
+    Import an Workflow object from a file using the specified file path.
 
     Parameters
     ----------
     file : str
         Path to the file.
 
     Returns
     -------
-    Service
+    Workflow
         Object instance.
     """
     obj: dict = read_yaml(file)
-    return create_service_from_dict(obj)
+    if isinstance(obj, list):
+        wf_dict = obj[0]
+        task_dicts = obj[1:]
+    else:
+        wf_dict = obj
+        task_dicts = []
+
+    check_context(obj.get("project"))
+    workflow = create_workflow_from_dict(wf_dict)
+    workflow.import_tasks(task_dicts)
+    return workflow
 
 
-def delete_service(
+def delete_workflow(
     project: str,
     entity_name: str | None = None,
     entity_id: str | None = None,
     delete_all_versions: bool = False,
     cascade: bool = True,
     **kwargs,
 ) -> dict:
@@ -213,41 +221,41 @@
         obj = context.list_objects(api, **kwargs)[0]
         entity_id = obj["id"]
 
     api = api_ctx_delete(project, ENTITY_TYPE, entity_id)
     return context.delete_object(api, **kwargs)
 
 
-def update_service(entity: Service, **kwargs) -> dict:
+def update_workflow(entity: Workflow, **kwargs) -> dict:
     """
     Update object in backend.
 
     Parameters
     ----------
-    entity : Service
+    entity : Workflow
         The object to update.
 
     Returns
     -------
     dict
         Response from backend.
     """
     api = api_ctx_update(entity.project, ENTITY_TYPE, entity_id=entity.id)
     return get_context(entity.project).update_object(api, entity.to_dict(), **kwargs)
 
 
-def list_services(project: str, **kwargs) -> list[dict]:
+def list_workflows(project: str, **kwargs) -> list[dict]:
     """
     List all objects from backend.
 
     Parameters
     ----------
     project : str
         Project name.
 
     Returns
     -------
     list[dict]
-        List of services dict representations.
+        List of workflows dict representations.
     """
     api = api_ctx_list(project, ENTITY_TYPE)
     return get_context(project).list_objects(api, **kwargs)
```

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/services/entity.py` & `digitalhub_core-0.5.0b0/digitalhub_core/stores/builder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,278 +1,262 @@
 """
-Service module.
+Store builder module.
 """
 from __future__ import annotations
 
+import os
 import typing
-from pathlib import Path
 
-from digitalhub_core.context.builder import get_context
-from digitalhub_core.entities._base.entity import Entity
-from digitalhub_core.entities._builders.metadata import build_metadata
-from digitalhub_core.entities._builders.spec import build_spec
-from digitalhub_core.entities._builders.status import build_status
-from digitalhub_core.entities.entity_types import EntityTypes
-from digitalhub_core.utils.api import api_ctx_create, api_ctx_read, api_ctx_update
-from digitalhub_core.utils.generic_utils import build_uuid, get_timestamp
-from digitalhub_core.utils.io_utils import write_yaml
+from digitalhub_core.stores.objects.base import StoreParameters
+from digitalhub_core.stores.objects.local import LocalStore, LocalStoreConfig
+from digitalhub_core.stores.objects.remote import RemoteStore, RemoteStoreConfig
+from digitalhub_core.stores.objects.s3 import S3Store, S3StoreConfig
+from digitalhub_core.stores.objects.sql import SqlStore, SQLStoreConfig
+from digitalhub_core.utils.exceptions import StoreError
+from digitalhub_core.utils.uri_utils import map_uri_scheme
+from pydantic import ValidationError
 
 if typing.TYPE_CHECKING:
-    from digitalhub_core.context.context import Context
-    from digitalhub_core.entities.services.metadata import ServiceMetadata
-    from digitalhub_core.entities.services.spec import ServiceSpec
-    from digitalhub_core.entities.services.status import ServiceStatus
+    from digitalhub_core.stores.objects.base import Store
 
 
-class Service(Entity):
+REGISTRY_STORES = {
+    "local": LocalStore,
+    "s3": S3Store,
+    "remote": RemoteStore,
+    "sql": SqlStore,
+}
+
+
+class StoreBuilder:
     """
-    A class representing a service.
+    Store builder class.
     """
 
-    ENTITY_TYPE = EntityTypes.SERVICES.value
-
-    def __init__(
-        self,
-        project: str,
-        name: str,
-        uuid: str,
-        kind: str,
-        metadata: ServiceMetadata,
-        spec: ServiceSpec,
-        status: ServiceStatus,
-        user: str | None = None,
-    ) -> None:
+    def __init__(self) -> None:
         """
         Constructor.
+        """
+        self._instances: dict[str, Store] = {}
+        self._default: Store | None = None
+        self._def_scheme = "s3"
 
-        Parameters
-        ----------
-        project : str
-            Project name.
-        name : str
-            Name of the object.
-        uuid : str
-            Version of the object.
-        kind : str
-            Kind of the object.
-        metadata : ServiceMetadata
-            Metadata of the object.
-        spec : ServiceSpec
-            Specification of the object.
-        status : ServiceStatus
-            Status of the object.
-        user : str
-            Owner of the object.
-        """
-        super().__init__()
-        self.project = project
-        self.name = name
-        self.id = uuid
-        self.kind = kind
-        self.key = f"store://{project}/{self.ENTITY_TYPE}/{kind}/{name}:{uuid}"
-        self.metadata = metadata
-        self.spec = spec
-        self.status = status
-        self.user = user
-
-        # Add attributes to be used in the to_dict method
-        self._obj_attr.extend(["project", "name", "id", "key"])
-
-    #############################
-    #  Save / Refresh / Export
-    #############################
-
-    def save(self, update: bool = False) -> Service:
+    def build(self, store_cfg: StoreParameters) -> None:
         """
-        Save entity into backend.
+        Build a store instance and register it.
+        It overrides any existing instance.
 
         Parameters
         ----------
-        update : bool
-            Flag to indicate update.
+        store_cfg : StoreParameters
+            Store configuration.
 
         Returns
         -------
-        Service
-            Entity saved.
+        None
         """
-        obj = self.to_dict()
-
-        if not update:
-            api = api_ctx_create(self.project, self.ENTITY_TYPE)
-            new_obj = self._context().create_object(api, obj)
-            self._update_attributes(new_obj)
-            return self
-
-        self.metadata.updated = obj["metadata"]["updated"] = get_timestamp()
-        api = api_ctx_update(self.project, self.ENTITY_TYPE, self.id)
-        new_obj = self._context().update_object(api, obj)
-        self._update_attributes(new_obj)
-        return self
+        scheme = map_uri_scheme(store_cfg.type)
+        self._instances[scheme] = self.build_store(store_cfg)
 
-    def refresh(self) -> Service:
+    def get(self, uri: str) -> Store:
         """
-        Refresh object from backend.
+        Get a store instance by URI.
+
+        Parameters
+        ----------
+        uri : str
+            URI to parse.
 
         Returns
         -------
-        Service
-            Entity refreshed.
+        Store
+            The store instance.
         """
-        api = api_ctx_read(self.project, self.ENTITY_TYPE, self.id)
-        obj = self._context().read_object(api)
-        self._update_attributes(obj)
-        return self
+        scheme = map_uri_scheme(uri)
+        if scheme not in self._instances:
+            store_cfg = get_env_store_config(scheme)
+            self._instances[scheme] = self.build_store(store_cfg)
+        return self._instances[scheme]
 
-    def export(self, filename: str | None = None) -> None:
+    def default(self) -> Store:
         """
-        Export object as a YAML file.
-
-        Parameters
-        ----------
-        filename : str
-            Name of the export YAML file. If not specified, the default value is used.
+        Get the default store instance.
 
         Returns
         -------
-        None
-        """
-        obj = self.to_dict()
-        if filename is None:
-            filename = f"{self.kind}_{self.name}_{self.id}.yml"
-        pth = Path(self._context().project_dir) / filename
-        pth.parent.mkdir(parents=True, exist_ok=True)
-        write_yaml(pth, obj)
-
-    #############################
-    #  Context
-    #############################
+        Store
+            The default store instance.
+
+        Raises
+        ------
+        StoreError
+            If no default store is set.
+        """
+        if self._default is None:
+            store_cfg = get_env_store_config(self._def_scheme)
+            self._default = self.build_store(store_cfg)
+        return self._default
 
-    def _context(self) -> Context:
+    def build_store(self, cfg: StoreParameters) -> Store:
         """
-        Get context.
+        Build a store instance.
+
+        Parameters
+        ----------
+        cfg : StoreParameters
+            Store configuration.
 
         Returns
         -------
-        Context
-            Context.
-        """
-        return get_context(self.project)
+        Store
+            The store instance.
 
-    #############################
-    #  Static interface methods
-    #############################
+        Raises
+        ------
+        NotImplementedError
+            If the store type is not implemented.
+        """
+        try:
+            obj = REGISTRY_STORES[cfg.type](cfg.name, cfg.type, cfg.config)
+            if cfg.is_default and self._default is not None:
+                raise StoreError("Only one default store!")
+            return obj
+        except KeyError as exc:
+            raise NotImplementedError from exc
 
     @staticmethod
-    def _parse_dict(obj: dict, validate: bool = True) -> dict:
+    def _check_config(config: StoreParameters | dict) -> StoreParameters:
         """
-        Get dictionary and parse it to a valid entity dictionary.
+        Check the store configuration validity.
 
         Parameters
         ----------
-        obj : dict
-            Dictionary to parse.
+        config : StoreParameters | dict
+            The store configuration.
 
         Returns
         -------
-        dict
-            A dictionary containing the attributes of the entity instance.
-        """
-        project = obj.get("project")
-        name = obj.get("name")
-        kind = obj.get("kind")
-        uuid = build_uuid(obj.get("id"))
-        metadata = build_metadata(ServiceMetadata, **obj.get("metadata", {}))
-        spec = build_spec(kind, validate=validate, **obj.get("spec", {}))
-        status = build_status(kind, **obj.get("status", {}))
-        user = obj.get("user")
-        return {
-            "project": project,
-            "name": name,
-            "uuid": uuid,
-            "kind": kind,
-            "metadata": metadata,
-            "spec": spec,
-            "status": status,
-            "user": user,
-        }
-
-
-def service_from_parameters(
-    project: str,
-    name: str,
-    kind: str,
-    uuid: str | None = None,
-    description: str | None = None,
-    source: str | None = None,
-    labels: list[str] | None = None,
-    embedded: bool = True,
-    **kwargs,
-) -> Service:
+        StoreParameters
+            The store configuration.
+
+        Raises
+        ------
+        TypeError
+            If the config parameter is not a StoreParameters instance or a well-formed dictionary.
+        """
+        if not isinstance(config, StoreParameters):
+            try:
+                return StoreParameters(**config)
+            except TypeError as exc:
+                raise StoreError("Invalid store configuration type.") from exc
+            except ValidationError as exc:
+                raise StoreError("Malformed store configuration parameters.") from exc
+        return config
+
+
+def get_env_store_config(scheme: str) -> StoreParameters:
     """
-    Create a new Service instance with the specified parameters.
+    Get a store configuration from the environment.
 
     Parameters
     ----------
-    project : str
-        A string representing the project associated with this service.
-    name : str
-        The name of the service.
-    kind : str
-        Kind of the object.
-    uuid : str
-        ID of the object in form of UUID.
-    source : str
-        Remote git source for object.
-    labels : list[str]
-        List of labels.
-    description : str
-        A description of the service.
-    embedded : bool
-        Flag to determine if object must be embedded in project.
-    **kwargs
-        Spec keyword arguments.
+    scheme : str
+        URI scheme.
 
     Returns
     -------
-    Service
-        An instance of the created service.
+    StoreParameters
+        The store configuration based on the scheme.
+
+    Raises
+    ------
+    ValueError
+        If the scheme is not supported.
     """
-    uuid = build_uuid(uuid)
-    metadata = build_metadata(
-        ServiceMetadata,
-        project=project,
-        name=name,
-        version=uuid,
-        description=description,
-        source=source,
-        labels=labels,
-        embedded=embedded,
-    )
-    spec = build_spec(kind, **kwargs)
-    status = build_status(kind)
-    return Service(
-        project=project,
-        name=name,
-        uuid=uuid,
-        kind=kind,
-        metadata=metadata,
-        spec=spec,
-        status=status,
-    )
+    if scheme == "s3":
+        return StoreParameters(
+            name="s3",
+            type="s3",
+            config=S3StoreConfig(
+                endpoint_url=os.getenv("S3_ENDPOINT_URL"),  # type: ignore
+                aws_access_key_id=os.getenv("AWS_ACCESS_KEY_ID"),  # type: ignore
+                aws_secret_access_key=os.getenv("AWS_SECRET_ACCESS_KEY"),  # type: ignore
+                bucket_name=os.getenv("S3_BUCKET_NAME"),  # type: ignore
+            ),
+        )
+    if scheme == "sql":
+        return StoreParameters(
+            name="sql",
+            type="sql",
+            config=SQLStoreConfig(
+                host=os.getenv("POSTGRES_HOST"),  # type: ignore
+                port=os.getenv("POSTGRES_PORT"),  # type: ignore
+                user=os.getenv("POSTGRES_USER"),  # type: ignore
+                password=os.getenv("POSTGRES_PASSWORD"),  # type: ignore
+                database=os.getenv("POSTGRES_DATABASE"),  # type: ignore
+                pg_schema=os.getenv("POSTGRES_SCHEMA"),  # type: ignore
+            ),
+        )
+    if scheme == "remote":
+        return StoreParameters(
+            name="remote",
+            type="remote",
+            config=RemoteStoreConfig(),
+        )
+    if scheme == "local":
+        return StoreParameters(
+            name="local",
+            type="local",
+            config=LocalStoreConfig(
+                path="tempsdk",
+            ),
+        )
+    raise ValueError(f"Unsupported scheme {scheme}")
 
 
-def service_from_dict(obj: dict) -> Service:
+def set_store(store_cfg: StoreParameters) -> None:
     """
-    Create Service instance from a dictionary.
+    Set a new store instance with the given configuration.
 
     Parameters
     ----------
-    obj : dict
-        Dictionary to create object from.
+    store_cfg : StoreParameters
+        Store configuration.
+
+    Returns
+    -------
+    None
+    """
+    store_builder.build(store_cfg)
+
+
+def get_store(uri: str) -> Store:
+    """
+    Get store instance by uri.
+
+    Parameters
+    ---------
+    uri : str
+        URI to parse.
 
     Returns
     -------
-    Service
-        Service instance.
+    Store
+        Store instance.
+    """
+    return store_builder.get(uri)
+
+
+def get_default_store() -> Store:
     """
-    return Service.from_dict(obj, validate=False)
+    Get the default store instance. The default store is the one that
+    can persist artifacts and dataitems.
+
+    Returns
+    -------
+    Store
+        Default store instance.
+    """
+    return store_builder.default()
+
+
+store_builder = StoreBuilder()
```

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/crud.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/entity.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/tasks/models.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/tasks/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/entities/workflows/entity.py` & `digitalhub_core-0.5.0b0/digitalhub_core/entities/workflows/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/registry/models.py` & `digitalhub_core-0.5.0b0/digitalhub_core/registry/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/registry/registry.py` & `digitalhub_core-0.5.0b0/digitalhub_core/registry/registry.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/registry/utils.py` & `digitalhub_core-0.5.0b0/digitalhub_core/registry/utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/runtimes/base.py` & `digitalhub_core-0.5.0b0/digitalhub_core/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/runtimes/builder.py` & `digitalhub_core-0.5.0b0/digitalhub_core/runtimes/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/base.py` & `digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/local.py` & `digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/local.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/remote.py` & `digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/remote.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/s3.py` & `digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/s3.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/stores/objects/sql.py` & `digitalhub_core-0.5.0b0/digitalhub_core/stores/objects/sql.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/utils/api.py` & `digitalhub_core-0.5.0b0/digitalhub_core/utils/api.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/utils/env_utils.py` & `digitalhub_core-0.5.0b0/digitalhub_core/utils/env_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/utils/file_utils.py` & `digitalhub_core-0.5.0b0/digitalhub_core/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/utils/generic_utils.py` & `digitalhub_core-0.5.0b0/digitalhub_core/utils/generic_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/utils/git_utils.py` & `digitalhub_core-0.5.0b0/digitalhub_core/utils/git_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/utils/io_utils.py` & `digitalhub_core-0.5.0b0/digitalhub_core/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core/utils/uri_utils.py` & `digitalhub_core-0.5.0b0/digitalhub_core/utils/uri_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core.egg-info/PKG-INFO` & `digitalhub_core-0.5.0b0/digitalhub_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub-core
-Version: 0.4.0b8
+Version: 0.5.0b0
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub_core-0.4.0b8/digitalhub_core.egg-info/SOURCES.txt` & `digitalhub_core-0.5.0b0/digitalhub_core.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -55,20 +55,14 @@
 digitalhub_core/entities/runs/status.py
 digitalhub_core/entities/secrets/__init__.py
 digitalhub_core/entities/secrets/crud.py
 digitalhub_core/entities/secrets/entity.py
 digitalhub_core/entities/secrets/metadata.py
 digitalhub_core/entities/secrets/spec.py
 digitalhub_core/entities/secrets/status.py
-digitalhub_core/entities/services/__init__.py
-digitalhub_core/entities/services/crud.py
-digitalhub_core/entities/services/entity.py
-digitalhub_core/entities/services/metadata.py
-digitalhub_core/entities/services/spec.py
-digitalhub_core/entities/services/status.py
 digitalhub_core/entities/tasks/__init__.py
 digitalhub_core/entities/tasks/crud.py
 digitalhub_core/entities/tasks/entity.py
 digitalhub_core/entities/tasks/metadata.py
 digitalhub_core/entities/tasks/models.py
 digitalhub_core/entities/tasks/spec.py
 digitalhub_core/entities/tasks/status.py
```

### Comparing `digitalhub_core-0.4.0b8/pyproject.toml` & `digitalhub_core-0.5.0b0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-core"
-version = "0.4.0b8"
+version = "0.5.0b0"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -61,15 +61,15 @@
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
 
 [tool.bumpver]
-current_version = "0.4.0b8"
+current_version = "0.5.0b0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

