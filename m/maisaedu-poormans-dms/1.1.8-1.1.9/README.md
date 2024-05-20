# Comparing `tmp/maisaedu-poormans-dms-1.1.8.tar.gz` & `tmp/maisaedu-poormans-dms-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maisaedu-poormans-dms-1.1.8.tar", last modified: Thu Aug 17 14:28:27 2023, max compression
+gzip compressed data, was "maisaedu-poormans-dms-1.1.9.tar", last modified: Tue Aug 29 14:08:16 2023, max compression
```

## Comparing `maisaedu-poormans-dms-1.1.8.tar` & `maisaedu-poormans-dms-1.1.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:27.700406 maisaedu-poormans-dms-1.1.8/
--rw-r--r--   0 vsts      (1001) docker     (123)     1076 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-08-17 14:28:27.700406 maisaedu-poormans-dms-1.1.8/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:27.696406 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/
--rw-r--r--   0 vsts      (1001) docker     (123)    16086 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:27.700406 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:27.700406 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/Contracts/
--rw-r--r--   0 vsts      (1001) docker     (123)      530 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorInterface.py
--rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorRowInterface.py
--rw-r--r--   0 vsts      (1001) docker     (123)      509 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorRowReaderInterface.py
--rw-r--r--   0 vsts      (1001) docker     (123)      337 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorRowWriterInterface.py
--rw-r--r--   0 vsts      (1001) docker     (123)      189 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorTableInterface.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/Contracts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2142 2023-08-17 14:28:07.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/Migrator.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:27.700406 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/MigratorRow/
--rw-r--r--   0 vsts      (1001) docker     (123)     4788 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/MigratorRow/MigratorRow.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3495 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/MigratorRow/Reader.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5047 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/MigratorRow/Writer.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/MigratorRow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5178 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/MigratorTable.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:27.700406 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/
--rw-r--r--   0 vsts      (1001) docker     (123)     1881 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Connector.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:27.700406 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Contracts/
--rw-r--r--   0 vsts      (1001) docker     (123)      256 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Contracts/WriterInterface.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Contracts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3902 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/MigratorRedshift.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:27.700406 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Models/
--rw-r--r--   0 vsts      (1001) docker     (123)      605 2023-08-17 14:28:07.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Models/ExtractionOperation.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1460 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Models/Struct.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Models/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6053 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Reader.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:27.700406 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Services/
--rw-r--r--   0 vsts      (1001) docker     (123)     3831 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Services/AdapterSourceTarget.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2821 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Services/ExtractionOperation.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2721 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Services/Struct.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Services/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1266 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Types.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:27.700406 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Writer/
--rw-r--r--   0 vsts      (1001) docker     (123)     3197 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Writer/GenericWriter.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5060 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Writer/WriterCDC.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1431 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Writer/WriterNonCDC.py
--rw-r--r--   0 vsts      (1001) docker     (123)      339 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Writer/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14790 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/sql_server_migration.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-08-17 14:28:27.696406 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      288 2023-08-17 14:28:27.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     2301 2023-08-17 14:28:27.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-08-17 14:28:27.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)      107 2023-08-17 14:28:27.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       22 2023-08-17 14:28:27.000000 maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-08-17 14:28:27.700406 maisaedu-poormans-dms-1.1.8/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)      643 2023-08-17 14:28:06.000000 maisaedu-poormans-dms-1.1.8/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:16.967563 maisaedu-poormans-dms-1.1.9/
+-rw-r--r--   0 vsts      (1001) docker     (999)     1076 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (999)      288 2023-08-29 14:08:16.967563 maisaedu-poormans-dms-1.1.9/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:16.959562 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/
+-rw-r--r--   0 vsts      (1001) docker     (999)    16086 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:16.963562 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:16.963562 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/Contracts/
+-rw-r--r--   0 vsts      (1001) docker     (999)      530 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (999)      415 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorRowInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (999)      509 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorRowReaderInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (999)      337 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorRowWriterInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (999)      189 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorTableInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (999)        0 2023-08-29 14:07:58.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/Contracts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     2142 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/Migrator.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:16.963562 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/
+-rw-r--r--   0 vsts      (1001) docker     (999)     4788 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/MigratorRow.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     3495 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/Reader.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     5047 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/Writer.py
+-rw-r--r--   0 vsts      (1001) docker     (999)        0 2023-08-29 14:07:58.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     5178 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/MigratorTable.py
+-rw-r--r--   0 vsts      (1001) docker     (999)        0 2023-08-29 14:07:58.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:16.967563 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/
+-rw-r--r--   0 vsts      (1001) docker     (999)     1881 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Connector.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:16.967563 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Contracts/
+-rw-r--r--   0 vsts      (1001) docker     (999)      256 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Contracts/WriterInterface.py
+-rw-r--r--   0 vsts      (1001) docker     (999)        0 2023-08-29 14:07:58.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Contracts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     3902 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/MigratorRedshift.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:16.967563 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Models/
+-rw-r--r--   0 vsts      (1001) docker     (999)      605 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Models/ExtractionOperation.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     1460 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Models/Struct.py
+-rw-r--r--   0 vsts      (1001) docker     (999)        0 2023-08-29 14:07:58.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Models/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     6053 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Reader.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:16.967563 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Services/
+-rw-r--r--   0 vsts      (1001) docker     (999)     3831 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Services/AdapterSourceTarget.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     2821 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Services/ExtractionOperation.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     2721 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Services/Struct.py
+-rw-r--r--   0 vsts      (1001) docker     (999)        0 2023-08-29 14:07:58.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Services/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     1266 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Types.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:16.967563 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Writer/
+-rw-r--r--   0 vsts      (1001) docker     (999)     3197 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Writer/GenericWriter.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     5060 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Writer/WriterCDC.py
+-rw-r--r--   0 vsts      (1001) docker     (999)     1431 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Writer/WriterNonCDC.py
+-rw-r--r--   0 vsts      (1001) docker     (999)      339 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Writer/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (999)        0 2023-08-29 14:07:58.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (999)    14790 2023-08-29 14:07:58.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/sql_server_migration.py
+drwxr-xr-x   0 vsts      (1001) docker     (999)        0 2023-08-29 14:08:16.963562 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (999)      288 2023-08-29 14:08:16.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (999)     2301 2023-08-29 14:08:16.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (999)        1 2023-08-29 14:08:16.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (999)      107 2023-08-29 14:08:16.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (999)       22 2023-08-29 14:08:16.000000 maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (999)       38 2023-08-29 14:08:16.967563 maisaedu-poormans-dms-1.1.9/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (999)      643 2023-08-29 14:07:59.000000 maisaedu-poormans-dms-1.1.9/setup.py
```

### Comparing `maisaedu-poormans-dms-1.1.8/LICENSE` & `maisaedu-poormans-dms-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/__init__.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/__init__.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorInterface.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/Contracts/MigratorInterface.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/Migrator.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/Migrator.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/MigratorRow/MigratorRow.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/MigratorRow.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/MigratorRow/Reader.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/Reader.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/MigratorRow/Writer.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/MigratorRow/Writer.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/postgres_migration/MigratorTable.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/postgres_migration/MigratorTable.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Connector.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Connector.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/MigratorRedshift.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/MigratorRedshift.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Models/ExtractionOperation.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Models/ExtractionOperation.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Models/Struct.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Models/Struct.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Reader.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Reader.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Services/AdapterSourceTarget.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Services/AdapterSourceTarget.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Services/ExtractionOperation.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Services/ExtractionOperation.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Services/Struct.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Services/Struct.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Types.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Types.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Writer/GenericWriter.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Writer/GenericWriter.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Writer/WriterCDC.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Writer/WriterCDC.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/redshift_migration/Writer/WriterNonCDC.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/redshift_migration/Writer/WriterNonCDC.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms/sql_server_migration.py` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms/sql_server_migration.py`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/maisaedu_poormans_dms.egg-info/SOURCES.txt` & `maisaedu-poormans-dms-1.1.9/maisaedu_poormans_dms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maisaedu-poormans-dms-1.1.8/setup.py` & `maisaedu-poormans-dms-1.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="maisaedu-poormans-dms",
-    version="1.1.8",
+    version="1.1.9",
     description="A library for making database migration tasks, for +A Education",
     license="MIT License",
     author="A+ Educação",
     author_email="dataeng@maisaedu.com.br",
     packages=find_packages(),
     scripts=[],
     install_requires=[
```

