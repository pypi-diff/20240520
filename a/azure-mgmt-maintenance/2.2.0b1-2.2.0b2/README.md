# Comparing `tmp/azure-mgmt-maintenance-2.2.0b1.tar.gz` & `tmp/azure-mgmt-maintenance-2.2.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-mgmt-maintenance-2.2.0b1.tar", last modified: Mon Oct 23 05:53:54 2023, max compression
+gzip compressed data, was "azure-mgmt-maintenance-2.2.0b2.tar", last modified: Mon May 20 06:12:09 2024, max compression
```

## Comparing `azure-mgmt-maintenance-2.2.0b1.tar` & `azure-mgmt-maintenance-2.2.0b2.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-23 05:53:54.854308 azure-mgmt-maintenance-2.2.0b1/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4507 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      217 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/MANIFEST.in
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     7616 2023-10-23 05:53:54.854308 azure-mgmt-maintenance-2.2.0b1/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2031 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      630 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/_meta.json
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-23 05:53:54.850309 azure-mgmt-maintenance-2.2.0b1/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-23 05:53:54.850309 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-23 05:53:54.850309 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      921 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3637 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8413 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/_maintenance_management_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    79289 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/_serialization.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/_vendor.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      488 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-23 05:53:54.850309 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      868 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3685 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/_configuration.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8589 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/_maintenance_management_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-23 05:53:54.854308 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2219 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6273 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_apply_update_for_resource_group_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27851 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_apply_updates_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    21428 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_configuration_assignments_for_resource_group_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19956 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_configuration_assignments_for_subscriptions_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    44466 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_configuration_assignments_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6146 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_configuration_assignments_within_subscription_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6425 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_maintenance_configurations_for_resource_group_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24528 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_maintenance_configurations_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5835 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8779 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_public_maintenance_configurations_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11717 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_updates_operations.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-23 05:53:54.854308 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/models/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2728 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/models/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3895 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/models/_maintenance_management_client_enums.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    42895 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/models/_models_py3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/models/_patch.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-23 05:53:54.854308 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2219 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7413 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_apply_update_for_resource_group_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    37719 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_apply_updates_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27472 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_configuration_assignments_for_resource_group_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25320 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_configuration_assignments_for_subscriptions_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    59783 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_configuration_assignments_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7108 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_configuration_assignments_within_subscription_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7555 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_maintenance_configurations_for_resource_group_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    31053 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_maintenance_configurations_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6546 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_patch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10849 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_public_maintenance_configurations_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15086 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_updates_operations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/py.typed
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2023-10-23 05:53:54.854308 azure-mgmt-maintenance-2.2.0b1/azure_mgmt_maintenance.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)     7616 2023-10-23 05:53:54.000000 azure-mgmt-maintenance-2.2.0b1/azure_mgmt_maintenance.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3018 2023-10-23 05:53:54.000000 azure-mgmt-maintenance-2.2.0b1/azure_mgmt_maintenance.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-10-23 05:53:54.000000 azure-mgmt-maintenance-2.2.0b1/azure_mgmt_maintenance.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2023-10-23 05:53:54.000000 azure-mgmt-maintenance-2.2.0b1/azure_mgmt_maintenance.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      124 2023-10-23 05:53:54.000000 azure-mgmt-maintenance-2.2.0b1/azure_mgmt_maintenance.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2023-10-23 05:53:54.000000 azure-mgmt-maintenance-2.2.0b1/azure_mgmt_maintenance.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2023-10-23 05:53:54.854308 azure-mgmt-maintenance-2.2.0b1/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2848 2023-10-23 05:53:09.000000 azure-mgmt-maintenance-2.2.0b1/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-20 06:12:09.886849 azure-mgmt-maintenance-2.2.0b2/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4604 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1074 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      217 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7533 2024-05-20 06:12:09.886849 azure-mgmt-maintenance-2.2.0b2/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2031 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      632 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/_meta.json
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-20 06:12:09.878849 azure-mgmt-maintenance-2.2.0b2/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-20 06:12:09.878849 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       65 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-20 06:12:09.878849 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      921 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3482 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9678 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/_maintenance_management_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    78873 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/_serialization.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      778 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/_vendor.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      488 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-20 06:12:09.878849 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      868 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3530 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/_configuration.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9882 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/_maintenance_management_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-20 06:12:09.882849 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2317 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5992 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_apply_update_for_resource_group_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25316 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_apply_updates_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19541 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_configuration_assignments_for_resource_group_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    18209 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_configuration_assignments_for_subscriptions_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    40580 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_configuration_assignments_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5935 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_configuration_assignments_within_subscription_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6164 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_maintenance_configurations_for_resource_group_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22381 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_maintenance_configurations_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5636 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8281 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_public_maintenance_configurations_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5094 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_scheduled_event_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10979 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_updates_operations.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-20 06:12:09.882849 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/models/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2820 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/models/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3886 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/models/_maintenance_management_client_enums.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    43400 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/models/_models_py3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/models/_patch.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-20 06:12:09.886849 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2317 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7132 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_apply_update_for_resource_group_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35184 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_apply_updates_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25585 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_configuration_assignments_for_resource_group_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    23573 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_configuration_assignments_for_subscriptions_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    55897 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_configuration_assignments_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6897 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_configuration_assignments_within_subscription_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7294 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_maintenance_configurations_for_resource_group_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    28906 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_maintenance_configurations_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6347 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      674 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_patch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10351 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_public_maintenance_configurations_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6780 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_scheduled_event_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14348 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_updates_operations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       26 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/py.typed
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-20 06:12:09.886849 azure-mgmt-maintenance-2.2.0b2/azure_mgmt_maintenance.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7533 2024-05-20 06:12:09.000000 azure-mgmt-maintenance-2.2.0b2/azure_mgmt_maintenance.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3152 2024-05-20 06:12:09.000000 azure-mgmt-maintenance-2.2.0b2/azure_mgmt_maintenance.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-20 06:12:09.000000 azure-mgmt-maintenance-2.2.0b2/azure_mgmt_maintenance.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-20 06:12:09.000000 azure-mgmt-maintenance-2.2.0b2/azure_mgmt_maintenance.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       56 2024-05-20 06:12:09.000000 azure-mgmt-maintenance-2.2.0b2/azure_mgmt_maintenance.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-05-20 06:12:09.000000 azure-mgmt-maintenance-2.2.0b2/azure_mgmt_maintenance.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-05-20 06:12:09.886849 azure-mgmt-maintenance-2.2.0b2/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2775 2024-05-20 06:10:44.000000 azure-mgmt-maintenance-2.2.0b2/setup.py
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/CHANGELOG.md` & `azure-mgmt-maintenance-2.2.0b2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Release History
 
+## 2.2.0b2 (2024-05-20)
+
+### Features Added
+
+  - Added operation group ScheduledEventOperations
+
 ## 2.2.0b1 (2023-10-22)
 
 ### Features Added
 
   - Added operation ApplyUpdatesOperations.create_or_update_or_cancel
 
 ## 2.1.0 (2023-08-18)
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/LICENSE` & `azure-mgmt-maintenance-2.2.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-mgmt-maintenance-2.2.0b1/PKG-INFO` & `azure-mgmt-maintenance-2.2.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-maintenance
-Version: 2.2.0b1
+Version: 2.2.0b2
 Summary: Microsoft Azure Maintenance Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: isodate<1.0.0,>=0.6.1
-Requires-Dist: azure-common~=1.1
-Requires-Dist: azure-mgmt-core<2.0.0,>=1.3.2
-Requires-Dist: typing-extensions>=4.3.0; python_version < "3.8.0"
 
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Maintenance Management Client Library.
-This package has been tested with Python 3.7+.
+This package has been tested with Python 3.8+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
 ## Getting started
 
 ### Prerequisites
 
-- Python 3.7+ is required to use this package.
+- Python 3.8+ is required to use this package.
 - [Azure subscription](https://azure.microsoft.com/free/)
 
 ### Install the package
 
 ```bash
 pip install azure-mgmt-maintenance
 pip install azure-identity
@@ -86,14 +82,20 @@
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 # Release History
 
+## 2.2.0b2 (2024-05-20)
+
+### Features Added
+
+  - Added operation group ScheduledEventOperations
+
 ## 2.2.0b1 (2023-10-22)
 
 ### Features Added
 
   - Added operation ApplyUpdatesOperations.create_or_update_or_cancel
 
 ## 2.1.0 (2023-08-18)
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/README.md` & `azure-mgmt-maintenance-2.2.0b2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Maintenance Management Client Library.
-This package has been tested with Python 3.7+.
+This package has been tested with Python 3.8+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
 ## Getting started
 
 ### Prerequisites
 
-- Python 3.7+ is required to use this package.
+- Python 3.8+ is required to use this package.
 - [Azure subscription](https://azure.microsoft.com/free/)
 
 ### Install the package
 
 ```bash
 pip install azure-mgmt-maintenance
 pip install azure-identity
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/_meta.json` & `azure-mgmt-maintenance-2.2.0b2/_meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'autorest_command'": "'autorest specification/maintenance/resource-manager/readme.md "*

 * *                       '--generate-sample=True --include-x-ms-examples-original-file=True --python '*

 * *                       '--python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk '*

 * *                       '--use=@autorest/python@6.13.7 --use=@autorest/modelerfour@4.27.0 '*

 * *                       "--version=3.9.7 --version-tolerant=False'",*

 * * "'commit'": "'f8b7c60c9839bc32fa19eb3d1d13069b70ba345d'",*

 * * "'use'": "['@ […]*

```diff
@@ -1,11 +1,11 @@
 {
     "autorest": "3.9.7",
-    "autorest_command": "autorest specification/maintenance/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.7.1 --use=@autorest/modelerfour@4.26.2 --version=3.9.7 --version-tolerant=False",
-    "commit": "e6d90862a97c4f04f0c26a8869602bbfd8b10280",
+    "autorest_command": "autorest specification/maintenance/resource-manager/readme.md --generate-sample=True --include-x-ms-examples-original-file=True --python --python-sdks-folder=/home/vsts/work/1/azure-sdk-for-python/sdk --use=@autorest/python@6.13.7 --use=@autorest/modelerfour@4.27.0 --version=3.9.7 --version-tolerant=False",
+    "commit": "f8b7c60c9839bc32fa19eb3d1d13069b70ba345d",
     "readme": "specification/maintenance/resource-manager/readme.md",
     "repository_url": "https://github.com/Azure/azure-rest-api-specs",
     "use": [
-        "@autorest/python@6.7.1",
-        "@autorest/modelerfour@4.26.2"
+        "@autorest/python@6.13.7",
+        "@autorest/modelerfour@4.27.0"
     ]
 }
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/__init__.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/_configuration.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/_configuration.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,64 +4,62 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
-from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMChallengeAuthenticationPolicy, ARMHttpLoggingPolicy
 
 from ._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
-class MaintenanceManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+class MaintenanceManagementClientConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
     """Configuration for MaintenanceManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: Subscription credentials that uniquely identify a Microsoft Azure
-     subscription. The subscription ID forms part of the URI for every service call. Required.
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-09-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-10-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "TokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(MaintenanceManagementClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2023-09-01-preview")
+        api_version: str = kwargs.pop("api_version", "2023-10-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-maintenance/{}".format(VERSION))
+        self.polling_interval = kwargs.get("polling_interval", 30)
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
         self.redirect_policy = kwargs.get("redirect_policy") or policies.RedirectPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.RetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
             self.authentication_policy = ARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/_maintenance_management_client.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/_maintenance_management_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, TYPE_CHECKING
 
+from azure.core.pipeline import policies
 from azure.core.rest import HttpRequest, HttpResponse
 from azure.mgmt.core import ARMPipelineClient
+from azure.mgmt.core.policies import ARMAutoResourceProviderRegistrationPolicy
 
 from . import models as _models
 from ._configuration import MaintenanceManagementClientConfiguration
 from ._serialization import Deserializer, Serializer
 from .operations import (
     ApplyUpdateForResourceGroupOperations,
     ApplyUpdatesOperations,
@@ -22,25 +24,28 @@
     ConfigurationAssignmentsForSubscriptionsOperations,
     ConfigurationAssignmentsOperations,
     ConfigurationAssignmentsWithinSubscriptionOperations,
     MaintenanceConfigurationsForResourceGroupOperations,
     MaintenanceConfigurationsOperations,
     Operations,
     PublicMaintenanceConfigurationsOperations,
+    ScheduledEventOperations,
     UpdatesOperations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials import TokenCredential
 
 
 class MaintenanceManagementClient:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
     """Azure Maintenance Management Client.
 
+    :ivar scheduled_event: ScheduledEventOperations operations
+    :vartype scheduled_event: azure.mgmt.maintenance.operations.ScheduledEventOperations
     :ivar public_maintenance_configurations: PublicMaintenanceConfigurationsOperations operations
     :vartype public_maintenance_configurations:
      azure.mgmt.maintenance.operations.PublicMaintenanceConfigurationsOperations
     :ivar apply_updates: ApplyUpdatesOperations operations
     :vartype apply_updates: azure.mgmt.maintenance.operations.ApplyUpdatesOperations
     :ivar configuration_assignments: ConfigurationAssignmentsOperations operations
     :vartype configuration_assignments:
@@ -69,40 +74,58 @@
      azure.mgmt.maintenance.operations.ConfigurationAssignmentsForResourceGroupOperations
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.maintenance.operations.Operations
     :ivar updates: UpdatesOperations operations
     :vartype updates: azure.mgmt.maintenance.operations.UpdatesOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials.TokenCredential
-    :param subscription_id: Subscription credentials that uniquely identify a Microsoft Azure
-     subscription. The subscription ID forms part of the URI for every service call. Required.
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2023-09-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-10-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(
         self,
         credential: "TokenCredential",
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = MaintenanceManagementClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        _policies = kwargs.pop("policies", None)
+        if _policies is None:
+            _policies = [
+                policies.RequestIdPolicy(**kwargs),
+                self._config.headers_policy,
+                self._config.user_agent_policy,
+                self._config.proxy_policy,
+                policies.ContentDecodePolicy(**kwargs),
+                ARMAutoResourceProviderRegistrationPolicy(),
+                self._config.redirect_policy,
+                self._config.retry_policy,
+                self._config.authentication_policy,
+                self._config.custom_hook_policy,
+                self._config.logging_policy,
+                policies.DistributedTracingPolicy(**kwargs),
+                policies.SensitiveHeaderCleanupPolicy(**kwargs) if self._config.redirect_policy else None,
+                self._config.http_logging_policy,
+            ]
+        self._client: ARMPipelineClient = ARMPipelineClient(base_url=base_url, policies=_policies, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
+        self.scheduled_event = ScheduledEventOperations(self._client, self._config, self._serialize, self._deserialize)
         self.public_maintenance_configurations = PublicMaintenanceConfigurationsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.apply_updates = ApplyUpdatesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.configuration_assignments = ConfigurationAssignmentsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
@@ -123,15 +146,15 @@
         )
         self.configuration_assignments_for_resource_group = ConfigurationAssignmentsForResourceGroupOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.updates = UpdatesOperations(self._client, self._config, self._serialize, self._deserialize)
 
-    def _send_request(self, request: HttpRequest, **kwargs: Any) -> HttpResponse:
+    def _send_request(self, request: HttpRequest, *, stream: bool = False, **kwargs: Any) -> HttpResponse:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
         >>> response = client._send_request(request)
         <HttpResponse: 200 OK>
@@ -143,15 +166,15 @@
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
         :rtype: ~azure.core.rest.HttpResponse
         """
 
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
-        return self._client.send_request(request_copy, **kwargs)
+        return self._client.send_request(request_copy, stream=stream, **kwargs)  # type: ignore
 
     def close(self) -> None:
         self._client.close()
 
     def __enter__(self) -> "MaintenanceManagementClient":
         self._client.__enter__()
         return self
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/_patch.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/_serialization.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/_serialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,16 @@
     from urllib import quote  # type: ignore
 except ImportError:
     from urllib.parse import quote
 import xml.etree.ElementTree as ET
 
 import isodate  # type: ignore
 
-from azure.core.exceptions import DeserializationError, SerializationError, raise_with_traceback
-from azure.core.serialization import NULL as AzureCoreNull
+from azure.core.exceptions import DeserializationError, SerializationError
+from azure.core.serialization import NULL as CoreNull
 
 _BOM = codecs.BOM_UTF8.decode(encoding="utf-8")
 
 ModelType = TypeVar("ModelType", bound="Model")
 JSON = MutableMapping[str, Any]
 
 
@@ -120,15 +120,15 @@
                     if isinstance(data, unicode):  # type: ignore
                         # If I'm Python 2.7 and unicode XML will scream if I try a "fromstring" on unicode string
                         data_as_str = data_as_str.encode(encoding="utf-8")  # type: ignore
                 except NameError:
                     pass
 
                 return ET.fromstring(data_as_str)  # nosec
-            except ET.ParseError:
+            except ET.ParseError as err:
                 # It might be because the server has an issue, and returned JSON with
                 # content-type XML....
                 # So let's try a JSON load, and if it's still broken
                 # let's flow the initial exception
                 def _json_attemp(data):
                     try:
                         return True, json.loads(data)
@@ -139,15 +139,15 @@
                 if success:
                     return json_result
                 # If i'm here, it's not JSON, it's not XML, let's scream
                 # and raise the last context in this block (the XML exception)
                 # The function hack is because Py2.7 messes up with exception
                 # context otherwise.
                 _LOGGER.critical("Wasn't XML not JSON, failing")
-                raise_with_traceback(DeserializationError, "XML is invalid")
+                raise DeserializationError("XML is invalid") from err
         raise DeserializationError("Cannot deserialize content-type: {}".format(content_type))
 
     @classmethod
     def deserialize_from_http_generics(cls, body_bytes: Optional[Union[AnyStr, IO]], headers: Mapping) -> Any:
         """Deserialize from HTTP response.
 
         Use bytes and headers to NOT use any requests/aiohttp or whatever
@@ -166,21 +166,14 @@
             content_type = "application/json"
 
         if body_bytes:
             return cls.deserialize_from_text(body_bytes, content_type)
         return None
 
 
-try:
-    basestring  # type: ignore
-    unicode_str = unicode  # type: ignore
-except NameError:
-    basestring = str
-    unicode_str = str
-
 _LOGGER = logging.getLogger(__name__)
 
 try:
     _long_type = long  # type: ignore
 except NameError:
     _long_type = int
 
@@ -291,15 +284,15 @@
     """
 
     _subtype_map: Dict[str, Dict[str, Any]] = {}
     _attribute_map: Dict[str, Dict[str, Any]] = {}
     _validation: Dict[str, Dict[str, Any]] = {}
 
     def __init__(self, **kwargs: Any) -> None:
-        self.additional_properties: Dict[str, Any] = {}
+        self.additional_properties: Optional[Dict[str, Any]] = {}
         for k in kwargs:
             if k not in self._attribute_map:
                 _LOGGER.warning("%s is not a known attribute of class %s and will be ignored", k, self.__class__)
             elif k in self._validation and self._validation[k].get("readonly", False):
                 _LOGGER.warning("Readonly attribute %s will be ignored in class %s", k, self.__class__)
             else:
                 setattr(self, k, kwargs[k])
@@ -336,26 +329,26 @@
             xml_map = cls._xml_map  # type: ignore
         except AttributeError:
             xml_map = {}
 
         return _create_xml_node(xml_map.get("name", cls.__name__), xml_map.get("prefix", None), xml_map.get("ns", None))
 
     def serialize(self, keep_readonly: bool = False, **kwargs: Any) -> JSON:
-        """Return the JSON that would be sent to azure from this model.
+        """Return the JSON that would be sent to server from this model.
 
         This is an alias to `as_dict(full_restapi_key_transformer, keep_readonly=False)`.
 
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param bool keep_readonly: If you want to serialize the readonly attributes
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
-        return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)
+        return serializer._serialize(self, keep_readonly=keep_readonly, **kwargs)  # type: ignore
 
     def as_dict(
         self,
         keep_readonly: bool = True,
         key_transformer: Callable[[str, Dict[str, Any], Any], Any] = attribute_transformer,
         **kwargs: Any
     ) -> JSON:
@@ -386,15 +379,15 @@
         If you want XML serialization, you can pass the kwargs is_xml=True.
 
         :param function key_transformer: A key transformer function.
         :returns: A dict JSON compatible object
         :rtype: dict
         """
         serializer = Serializer(self._infer_class_models())
-        return serializer._serialize(self, key_transformer=key_transformer, keep_readonly=keep_readonly, **kwargs)
+        return serializer._serialize(self, key_transformer=key_transformer, keep_readonly=keep_readonly, **kwargs)  # type: ignore
 
     @classmethod
     def _infer_class_models(cls):
         try:
             str_models = cls.__module__.rsplit(".", 1)[0]
             models = sys.modules[str_models]
             client_models = {k: v for k, v in models.__dict__.items() if isinstance(v, type)}
@@ -411,15 +404,15 @@
 
         :param str data: A str using RestAPI structure. JSON by default.
         :param str content_type: JSON by default, set application/xml if XML.
         :returns: An instance of this model
         :raises: DeserializationError if something went wrong
         """
         deserializer = Deserializer(cls._infer_class_models())
-        return deserializer(cls.__name__, data, content_type=content_type)
+        return deserializer(cls.__name__, data, content_type=content_type)  # type: ignore
 
     @classmethod
     def from_dict(
         cls: Type[ModelType],
         data: Any,
         key_extractors: Optional[Callable[[str, Dict[str, Any], Any], Any]] = None,
         content_type: Optional[str] = None,
@@ -441,15 +434,15 @@
                 attribute_key_case_insensitive_extractor,
                 rest_key_case_insensitive_extractor,
                 last_rest_key_case_insensitive_extractor,
             ]
             if key_extractors is None
             else key_extractors
         )
-        return deserializer(cls.__name__, data, content_type=content_type)
+        return deserializer(cls.__name__, data, content_type=content_type)  # type: ignore
 
     @classmethod
     def _flatten_subtype(cls, key, objects):
         if "_subtype_map" not in cls.__dict__:
             return {}
         result = dict(cls._subtype_map[key])
         for valuetype in cls._subtype_map[key].values():
@@ -541,15 +534,15 @@
         "min_items": lambda x, y: len(x) < y,
         "max_items": lambda x, y: len(x) > y,
         "pattern": lambda x, y: not re.match(y, x, re.UNICODE),
         "unique": lambda x, y: len(x) != len(set(x)),
         "multiple": lambda x, y: x % y != 0,
     }
 
-    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
+    def __init__(self, classes: Optional[Mapping[str, type]] = None):
         self.serialize_type = {
             "iso-8601": Serializer.serialize_iso,
             "rfc-1123": Serializer.serialize_rfc,
             "unix-time": Serializer.serialize_unix,
             "duration": Serializer.serialize_duration,
             "date": Serializer.serialize_date,
             "time": Serializer.serialize_time,
@@ -557,15 +550,15 @@
             "long": Serializer.serialize_long,
             "bytearray": Serializer.serialize_bytearray,
             "base64": Serializer.serialize_base64,
             "object": self.serialize_object,
             "[]": self.serialize_iter,
             "{}": self.serialize_dict,
         }
-        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
+        self.dependencies: Dict[str, type] = dict(classes) if classes else {}
         self.key_transformer = full_restapi_key_transformer
         self.client_side_validation = True
 
     def _serialize(self, target_obj, data_type=None, **kwargs):
         """Serialize data into a string according to type.
 
         :param target_obj: The data to be serialized.
@@ -645,15 +638,15 @@
                                     new_attr.tag = "}".join([splitted_tag[0], xml_name])
                                 else:
                                     new_attr.tag = xml_name
                             serialized.append(new_attr)  # type: ignore
                         else:  # That's a basic type
                             # Integrate namespace if necessary
                             local_node = _create_xml_node(xml_name, xml_prefix, xml_ns)
-                            local_node.text = unicode_str(new_attr)
+                            local_node.text = str(new_attr)
                             serialized.append(local_node)  # type: ignore
                     else:  # JSON
                         for k in reversed(keys):  # type: ignore
                             new_attr = {k: new_attr}
 
                         _new_attr = new_attr
                         _serialized = serialized
@@ -664,15 +657,15 @@
                             _serialized = _serialized[k]
                 except ValueError as err:
                     if isinstance(err, SerializationError):
                         raise
 
         except (AttributeError, KeyError, TypeError) as err:
             msg = "Attribute {} in object {} cannot be serialized.\n{}".format(attr_name, class_name, str(target_obj))
-            raise_with_traceback(SerializationError, msg, err)
+            raise SerializationError(msg) from err
         else:
             return serialized
 
     def body(self, data, data_type, **kwargs):
         """Serialize data intended for a request body.
 
         :param data: The data to be serialized.
@@ -706,15 +699,15 @@
                     deserializer.key_extractors = [
                         rest_key_case_insensitive_extractor,
                         attribute_key_case_insensitive_extractor,
                         last_rest_key_case_insensitive_extractor,
                     ]
                 data = deserializer._deserialize(data_type, data)
             except DeserializationError as err:
-                raise_with_traceback(SerializationError, "Unable to build a model: " + str(err), err)
+                raise SerializationError("Unable to build a model: " + str(err)) from err
 
         return self._serialize(data, data_type, **kwargs)
 
     def url(self, name, data, data_type, **kwargs):
         """Serialize data intended for a URL path.
 
         :param data: The data to be serialized.
@@ -726,38 +719,39 @@
         try:
             output = self.serialize_data(data, data_type, **kwargs)
             if data_type == "bool":
                 output = json.dumps(output)
 
             if kwargs.get("skip_quote") is True:
                 output = str(output)
+                output = output.replace("{", quote("{")).replace("}", quote("}"))
             else:
                 output = quote(str(output), safe="")
         except SerializationError:
             raise TypeError("{} must be type {}.".format(name, data_type))
         else:
             return output
 
     def query(self, name, data, data_type, **kwargs):
         """Serialize data intended for a URL query.
 
         :param data: The data to be serialized.
         :param str data_type: The type to be serialized from.
         :keyword bool skip_quote: Whether to skip quote the serialized result.
         Defaults to False.
-        :rtype: str
+        :rtype: str, list
         :raises: TypeError if serialization fails.
         :raises: ValueError if data is None
         """
         try:
             # Treat the list aside, since we don't want to encode the div separator
             if data_type.startswith("["):
                 internal_data_type = data_type[1:-1]
                 do_quote = not kwargs.get("skip_quote", False)
-                return str(self.serialize_iter(data, internal_data_type, do_quote=do_quote, **kwargs))
+                return self.serialize_iter(data, internal_data_type, do_quote=do_quote, **kwargs)
 
             # Not a list, regular serialization
             output = self.serialize_data(data, data_type, **kwargs)
             if data_type == "bool":
                 output = json.dumps(output)
             if kwargs.get("skip_quote") is True:
                 output = str(output)
@@ -800,15 +794,15 @@
         :raises: ValueError if data is None
         :raises: SerializationError if serialization fails.
         """
         if data is None:
             raise ValueError("No value for given attribute")
 
         try:
-            if data is AzureCoreNull:
+            if data is CoreNull:
                 return None
             if data_type in self.basic_types.values():
                 return self.serialize_basic(data, data_type, **kwargs)
 
             elif data_type in self.serialize_type:
                 return self.serialize_type[data_type](data, **kwargs)
 
@@ -820,15 +814,15 @@
 
             iter_type = data_type[0] + data_type[-1]
             if iter_type in self.serialize_type:
                 return self.serialize_type[iter_type](data, data_type[1:-1], **kwargs)
 
         except (ValueError, TypeError) as err:
             msg = "Unable to serialize value: {!r} as type: {!r}."
-            raise_with_traceback(SerializationError, msg.format(data, data_type), err)
+            raise SerializationError(msg.format(data, data_type)) from err
         else:
             return self._serialize(data, **kwargs)
 
     @classmethod
     def _get_custom_serializers(cls, data_type, **kwargs):
         custom_serializer = kwargs.get("basic_types_serializers", {}).get(data_type)
         if custom_serializer:
@@ -989,15 +983,15 @@
         if isinstance(attr, ET.Element):
             return attr
         obj_type = type(attr)
         if obj_type in self.basic_types:
             return self.serialize_basic(attr, self.basic_types[obj_type], **kwargs)
         if obj_type is _long_type:
             return self.serialize_long(attr)
-        if obj_type is unicode_str:
+        if obj_type is str:
             return self.serialize_unicode(attr)
         if obj_type is datetime.datetime:
             return self.serialize_iso(attr)
         if obj_type is datetime.date:
             return self.serialize_date(attr)
         if obj_type is datetime.time:
             return self.serialize_time(attr)
@@ -1166,18 +1160,18 @@
                 microseconds = "." + microseconds
             date = "{:04}-{:02}-{:02}T{:02}:{:02}:{:02}".format(
                 utc.tm_year, utc.tm_mon, utc.tm_mday, utc.tm_hour, utc.tm_min, utc.tm_sec
             )
             return date + microseconds + "Z"
         except (ValueError, OverflowError) as err:
             msg = "Unable to serialize datetime object."
-            raise_with_traceback(SerializationError, msg, err)
+            raise SerializationError(msg) from err
         except AttributeError as err:
             msg = "ISO-8601 object must be valid Datetime object."
-            raise_with_traceback(TypeError, msg, err)
+            raise TypeError(msg) from err
 
     @staticmethod
     def serialize_unix(attr, **kwargs):
         """Serialize Datetime object into IntTime format.
         This is represented as seconds.
 
         :param Datetime attr: Object to be serialized.
@@ -1205,15 +1199,14 @@
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = working_data.get(working_key, data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
             # that all properties under are None as well
-            # https://github.com/Azure/msrest-for-python/issues/197
             return None
         key = ".".join(dict_keys[1:])
 
     return working_data.get(key)
 
 
 def rest_key_case_insensitive_extractor(attr, attr_desc, data):
@@ -1226,15 +1219,14 @@
             key = _decode_attribute_map_key(dict_keys[0])
             break
         working_key = _decode_attribute_map_key(dict_keys[0])
         working_data = attribute_key_case_insensitive_extractor(working_key, None, working_data)
         if working_data is None:
             # If at any point while following flatten JSON path see None, it means
             # that all properties under are None as well
-            # https://github.com/Azure/msrest-for-python/issues/197
             return None
         key = ".".join(dict_keys[1:])
 
     if working_data:
         return attribute_key_case_insensitive_extractor(key, None, working_data)
 
 
@@ -1367,15 +1359,15 @@
     :ivar list key_extractors: Ordered list of extractors to be used by this deserializer.
     """
 
     basic_types = {str: "str", int: "int", bool: "bool", float: "float"}
 
     valid_date = re.compile(r"\d{4}[-]\d{2}[-]\d{2}T\d{2}:\d{2}:\d{2}" r"\.?\d*Z?[-+]?[\d{2}]?:?[\d{2}]?")
 
-    def __init__(self, classes: Optional[Mapping[str, Type[ModelType]]] = None):
+    def __init__(self, classes: Optional[Mapping[str, type]] = None):
         self.deserialize_type = {
             "iso-8601": Deserializer.deserialize_iso,
             "rfc-1123": Deserializer.deserialize_rfc,
             "unix-time": Deserializer.deserialize_unix,
             "duration": Deserializer.deserialize_duration,
             "date": Deserializer.deserialize_date,
             "time": Deserializer.deserialize_time,
@@ -1387,15 +1379,15 @@
             "[]": self.deserialize_iter,
             "{}": self.deserialize_dict,
         }
         self.deserialize_expected_types = {
             "duration": (isodate.Duration, datetime.timedelta),
             "iso-8601": (datetime.datetime),
         }
-        self.dependencies: Dict[str, Type[ModelType]] = dict(classes) if classes else {}
+        self.dependencies: Dict[str, type] = dict(classes) if classes else {}
         self.key_extractors = [rest_key_extractor, xml_key_extractor]
         # Additional properties only works if the "rest_key_extractor" is used to
         # extract the keys. Making it to work whatever the key extractor is too much
         # complicated, with no real scenario for now.
         # So adding a flag to disable additional properties detection. This flag should be
         # used if your expect the deserialization to NOT come from a JSON REST syntax.
         # Otherwise, result are unexpected
@@ -1440,15 +1432,15 @@
                     setattr(data, attr, self._deserialize(local_type, value))
                 return data
             except AttributeError:
                 return
 
         response, class_name = self._classify_target(target_obj, data)
 
-        if isinstance(response, basestring):
+        if isinstance(response, str):
             return self.deserialize_data(data, response)
         elif isinstance(response, type) and issubclass(response, Enum):
             return self.deserialize_enum(data, response)
 
         if data is None:
             return data
         try:
@@ -1477,15 +1469,15 @@
                             continue
                         raw_value = found_value
 
                 value = self.deserialize_data(raw_value, attr_desc["type"])
                 d_attrs[attr] = value
         except (AttributeError, TypeError, KeyError) as err:
             msg = "Unable to deserialize to object: " + class_name  # type: ignore
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             additional_properties = self._build_additional_properties(attributes, data)
             return self._instantiate_model(response, d_attrs, additional_properties)
 
     def _build_additional_properties(self, attribute_map, data):
         if not self.additional_properties_detection:
             return None
@@ -1511,22 +1503,22 @@
 
         :param str target: The target object type to deserialize to.
         :param str/dict data: The response data to deserialize.
         """
         if target is None:
             return None, None
 
-        if isinstance(target, basestring):
+        if isinstance(target, str):
             try:
                 target = self.dependencies[target]
             except KeyError:
                 return target, target
 
         try:
-            target = target._classify(data, self.dependencies)
+            target = target._classify(data, self.dependencies)  # type: ignore
         except AttributeError:
             pass  # Target is not a Model, no classify
         return target, target.__class__.__name__  # type: ignore
 
     def failsafe_deserialize(self, target_obj, data, content_type=None):
         """Ignores any errors encountered in deserialization,
         and falls back to not deserializing the object. Recommended
@@ -1574,15 +1566,15 @@
         if hasattr(raw_data, "body"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text(), raw_data.headers)
 
         # Assume this enough to recognize requests.Response without importing it.
         if hasattr(raw_data, "_content_consumed"):
             return RawDeserializer.deserialize_from_http_generics(raw_data.text, raw_data.headers)
 
-        if isinstance(raw_data, (basestring, bytes)) or hasattr(raw_data, "read"):
+        if isinstance(raw_data, (str, bytes)) or hasattr(raw_data, "read"):
             return RawDeserializer.deserialize_from_text(raw_data, content_type)  # type: ignore
         return raw_data
 
     def _instantiate_model(self, response, attrs, additional_properties=None):
         """Instantiate a response model passing in deserialized args.
 
         :param response: The response model class.
@@ -1648,15 +1640,15 @@
                 if isinstance(data, ET.Element):
                     data = data.text
                 return self.deserialize_enum(data, obj_type)
 
         except (ValueError, TypeError, AttributeError) as err:
             msg = "Unable to deserialize response data."
             msg += " Data: {}, {}".format(data, data_type)
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return self._deserialize(obj_type, data)
 
     def deserialize_iter(self, attr, iter_type):
         """Deserialize an iterable.
 
         :param list attr: Iterable to be deserialized.
@@ -1696,15 +1688,15 @@
         :raises: TypeError if non-builtin datatype encountered.
         """
         if attr is None:
             return None
         if isinstance(attr, ET.Element):
             # Do no recurse on XML, just return the tree as-is
             return attr
-        if isinstance(attr, basestring):
+        if isinstance(attr, str):
             return self.deserialize_basic(attr, "str")
         obj_type = type(attr)
         if obj_type in self.basic_types:
             return self.deserialize_basic(attr, self.basic_types[obj_type])
         if obj_type is _long_type:
             return self.deserialize_long(attr)
 
@@ -1753,15 +1745,15 @@
                     # None or '', node <a/> with a strong type is None.
                     # Don't try to model "empty bool" or "empty int"
                     return None
 
         if data_type == "bool":
             if attr in [True, False, 1, 0]:
                 return bool(attr)
-            elif isinstance(attr, basestring):
+            elif isinstance(attr, str):
                 if attr.lower() in ["true", "1"]:
                     return True
                 elif attr.lower() in ["false", "0"]:
                     return False
             raise TypeError("Invalid boolean value: {}".format(attr))
 
         if data_type == "str":
@@ -1804,15 +1796,14 @@
         """
         if isinstance(data, enum_obj) or data is None:
             return data
         if isinstance(data, Enum):
             data = data.value
         if isinstance(data, int):
             # Workaround. We might consider remove it in the future.
-            # https://github.com/Azure/azure-rest-api-specs/issues/141
             try:
                 return list(enum_obj.__members__.values())[data]
             except IndexError:
                 error = "{!r} is not a valid index for enum {!r}"
                 raise DeserializationError(error.format(data, enum_obj))
         try:
             return enum_obj(str(data))
@@ -1858,18 +1849,18 @@
         :param str attr: response string to be deserialized.
         :rtype: Decimal
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
-            return decimal.Decimal(attr)  # type: ignore
+            return decimal.Decimal(str(attr))  # type: ignore
         except decimal.DecimalException as err:
             msg = "Invalid decimal {}".format(attr)
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
 
     @staticmethod
     def deserialize_long(attr):
         """Deserialize string into long (Py2) or int (Py3).
 
         :param str attr: response string to be deserialized.
         :rtype: long or int
@@ -1889,15 +1880,15 @@
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         try:
             duration = isodate.parse_duration(attr)
         except (ValueError, OverflowError, AttributeError) as err:
             msg = "Cannot deserialize duration object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return duration
 
     @staticmethod
     def deserialize_date(attr):
         """Deserialize ISO-8601 formatted string into Date object.
 
@@ -1906,15 +1897,15 @@
         :raises: DeserializationError if string format invalid.
         """
         if isinstance(attr, ET.Element):
             attr = attr.text
         if re.search(r"[^\W\d_]", attr, re.I + re.U):  # type: ignore
             raise DeserializationError("Date must have only digits and -. Received: %s" % attr)
         # This must NOT use defaultmonth/defaultday. Using None ensure this raises an exception.
-        return isodate.parse_date(attr, defaultmonth=None, defaultday=None)
+        return isodate.parse_date(attr, defaultmonth=0, defaultday=0)
 
     @staticmethod
     def deserialize_time(attr):
         """Deserialize ISO-8601 formatted string into time object.
 
         :param str attr: response string to be deserialized.
         :rtype: datetime.time
@@ -1941,15 +1932,15 @@
             date_obj = datetime.datetime(
                 *parsed_date[:6], tzinfo=_FixedOffset(datetime.timedelta(minutes=(parsed_date[9] or 0) / 60))
             )
             if not date_obj.tzinfo:
                 date_obj = date_obj.astimezone(tz=TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to rfc datetime object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return date_obj
 
     @staticmethod
     def deserialize_iso(attr):
         """Deserialize ISO-8601 formatted string into Datetime object.
 
@@ -1978,15 +1969,15 @@
 
             date_obj = isodate.parse_datetime(attr)
             test_utc = date_obj.utctimetuple()
             if test_utc.tm_year > 9999 or test_utc.tm_year < 1:
                 raise OverflowError("Hit max or min date")
         except (ValueError, OverflowError, AttributeError) as err:
             msg = "Cannot deserialize datetime object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return date_obj
 
     @staticmethod
     def deserialize_unix(attr):
         """Serialize Datetime object into IntTime format.
         This is represented as seconds.
@@ -1994,13 +1985,14 @@
         :param int attr: Object to be serialized.
         :rtype: Datetime
         :raises: DeserializationError if format invalid
         """
         if isinstance(attr, ET.Element):
             attr = int(attr.text)  # type: ignore
         try:
+            attr = int(attr)
             date_obj = datetime.datetime.fromtimestamp(attr, TZ_UTC)
         except ValueError as err:
             msg = "Cannot deserialize to unix datetime object."
-            raise_with_traceback(DeserializationError, msg, err)
+            raise DeserializationError(msg) from err
         else:
             return date_obj
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/_vendor.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/_vendor.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/__init__.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/_configuration.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/_configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,64 +4,62 @@
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any, TYPE_CHECKING
 
-from azure.core.configuration import Configuration
 from azure.core.pipeline import policies
 from azure.mgmt.core.policies import ARMHttpLoggingPolicy, AsyncARMChallengeAuthenticationPolicy
 
 from .._version import VERSION
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
-class MaintenanceManagementClientConfiguration(Configuration):  # pylint: disable=too-many-instance-attributes
+class MaintenanceManagementClientConfiguration:  # pylint: disable=too-many-instance-attributes,name-too-long
     """Configuration for MaintenanceManagementClient.
 
     Note that all parameters used to create this instance are saved as instance
     attributes.
 
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: Subscription credentials that uniquely identify a Microsoft Azure
-     subscription. The subscription ID forms part of the URI for every service call. Required.
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
-    :keyword api_version: Api Version. Default value is "2023-09-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-10-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(self, credential: "AsyncTokenCredential", subscription_id: str, **kwargs: Any) -> None:
-        super(MaintenanceManagementClientConfiguration, self).__init__(**kwargs)
-        api_version: str = kwargs.pop("api_version", "2023-09-01-preview")
+        api_version: str = kwargs.pop("api_version", "2023-10-01-preview")
 
         if credential is None:
             raise ValueError("Parameter 'credential' must not be None.")
         if subscription_id is None:
             raise ValueError("Parameter 'subscription_id' must not be None.")
 
         self.credential = credential
         self.subscription_id = subscription_id
         self.api_version = api_version
         self.credential_scopes = kwargs.pop("credential_scopes", ["https://management.azure.com/.default"])
         kwargs.setdefault("sdk_moniker", "mgmt-maintenance/{}".format(VERSION))
+        self.polling_interval = kwargs.get("polling_interval", 30)
         self._configure(**kwargs)
 
     def _configure(self, **kwargs: Any) -> None:
         self.user_agent_policy = kwargs.get("user_agent_policy") or policies.UserAgentPolicy(**kwargs)
         self.headers_policy = kwargs.get("headers_policy") or policies.HeadersPolicy(**kwargs)
         self.proxy_policy = kwargs.get("proxy_policy") or policies.ProxyPolicy(**kwargs)
         self.logging_policy = kwargs.get("logging_policy") or policies.NetworkTraceLoggingPolicy(**kwargs)
         self.http_logging_policy = kwargs.get("http_logging_policy") or ARMHttpLoggingPolicy(**kwargs)
-        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.custom_hook_policy = kwargs.get("custom_hook_policy") or policies.CustomHookPolicy(**kwargs)
         self.redirect_policy = kwargs.get("redirect_policy") or policies.AsyncRedirectPolicy(**kwargs)
+        self.retry_policy = kwargs.get("retry_policy") or policies.AsyncRetryPolicy(**kwargs)
         self.authentication_policy = kwargs.get("authentication_policy")
         if self.credential and not self.authentication_policy:
             self.authentication_policy = AsyncARMChallengeAuthenticationPolicy(
                 self.credential, *self.credential_scopes, **kwargs
             )
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/_maintenance_management_client.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/_maintenance_management_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, Awaitable, TYPE_CHECKING
 
+from azure.core.pipeline import policies
 from azure.core.rest import AsyncHttpResponse, HttpRequest
 from azure.mgmt.core import AsyncARMPipelineClient
+from azure.mgmt.core.policies import AsyncARMAutoResourceProviderRegistrationPolicy
 
 from .. import models as _models
 from .._serialization import Deserializer, Serializer
 from ._configuration import MaintenanceManagementClientConfiguration
 from .operations import (
     ApplyUpdateForResourceGroupOperations,
     ApplyUpdatesOperations,
@@ -22,25 +24,28 @@
     ConfigurationAssignmentsForSubscriptionsOperations,
     ConfigurationAssignmentsOperations,
     ConfigurationAssignmentsWithinSubscriptionOperations,
     MaintenanceConfigurationsForResourceGroupOperations,
     MaintenanceConfigurationsOperations,
     Operations,
     PublicMaintenanceConfigurationsOperations,
+    ScheduledEventOperations,
     UpdatesOperations,
 )
 
 if TYPE_CHECKING:
     # pylint: disable=unused-import,ungrouped-imports
     from azure.core.credentials_async import AsyncTokenCredential
 
 
 class MaintenanceManagementClient:  # pylint: disable=client-accepts-api-version-keyword,too-many-instance-attributes
     """Azure Maintenance Management Client.
 
+    :ivar scheduled_event: ScheduledEventOperations operations
+    :vartype scheduled_event: azure.mgmt.maintenance.aio.operations.ScheduledEventOperations
     :ivar public_maintenance_configurations: PublicMaintenanceConfigurationsOperations operations
     :vartype public_maintenance_configurations:
      azure.mgmt.maintenance.aio.operations.PublicMaintenanceConfigurationsOperations
     :ivar apply_updates: ApplyUpdatesOperations operations
     :vartype apply_updates: azure.mgmt.maintenance.aio.operations.ApplyUpdatesOperations
     :ivar configuration_assignments: ConfigurationAssignmentsOperations operations
     :vartype configuration_assignments:
@@ -69,40 +74,58 @@
      azure.mgmt.maintenance.aio.operations.ConfigurationAssignmentsForResourceGroupOperations
     :ivar operations: Operations operations
     :vartype operations: azure.mgmt.maintenance.aio.operations.Operations
     :ivar updates: UpdatesOperations operations
     :vartype updates: azure.mgmt.maintenance.aio.operations.UpdatesOperations
     :param credential: Credential needed for the client to connect to Azure. Required.
     :type credential: ~azure.core.credentials_async.AsyncTokenCredential
-    :param subscription_id: Subscription credentials that uniquely identify a Microsoft Azure
-     subscription. The subscription ID forms part of the URI for every service call. Required.
+    :param subscription_id: The ID of the target subscription. The value must be an UUID. Required.
     :type subscription_id: str
     :param base_url: Service URL. Default value is "https://management.azure.com".
     :type base_url: str
-    :keyword api_version: Api Version. Default value is "2023-09-01-preview". Note that overriding
+    :keyword api_version: Api Version. Default value is "2023-10-01-preview". Note that overriding
      this default value may result in unsupported behavior.
     :paramtype api_version: str
     """
 
     def __init__(
         self,
         credential: "AsyncTokenCredential",
         subscription_id: str,
         base_url: str = "https://management.azure.com",
         **kwargs: Any
     ) -> None:
         self._config = MaintenanceManagementClientConfiguration(
             credential=credential, subscription_id=subscription_id, **kwargs
         )
-        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, config=self._config, **kwargs)
+        _policies = kwargs.pop("policies", None)
+        if _policies is None:
+            _policies = [
+                policies.RequestIdPolicy(**kwargs),
+                self._config.headers_policy,
+                self._config.user_agent_policy,
+                self._config.proxy_policy,
+                policies.ContentDecodePolicy(**kwargs),
+                AsyncARMAutoResourceProviderRegistrationPolicy(),
+                self._config.redirect_policy,
+                self._config.retry_policy,
+                self._config.authentication_policy,
+                self._config.custom_hook_policy,
+                self._config.logging_policy,
+                policies.DistributedTracingPolicy(**kwargs),
+                policies.SensitiveHeaderCleanupPolicy(**kwargs) if self._config.redirect_policy else None,
+                self._config.http_logging_policy,
+            ]
+        self._client: AsyncARMPipelineClient = AsyncARMPipelineClient(base_url=base_url, policies=_policies, **kwargs)
 
         client_models = {k: v for k, v in _models.__dict__.items() if isinstance(v, type)}
         self._serialize = Serializer(client_models)
         self._deserialize = Deserializer(client_models)
         self._serialize.client_side_validation = False
+        self.scheduled_event = ScheduledEventOperations(self._client, self._config, self._serialize, self._deserialize)
         self.public_maintenance_configurations = PublicMaintenanceConfigurationsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.apply_updates = ApplyUpdatesOperations(self._client, self._config, self._serialize, self._deserialize)
         self.configuration_assignments = ConfigurationAssignmentsOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
@@ -123,15 +146,17 @@
         )
         self.configuration_assignments_for_resource_group = ConfigurationAssignmentsForResourceGroupOperations(
             self._client, self._config, self._serialize, self._deserialize
         )
         self.operations = Operations(self._client, self._config, self._serialize, self._deserialize)
         self.updates = UpdatesOperations(self._client, self._config, self._serialize, self._deserialize)
 
-    def _send_request(self, request: HttpRequest, **kwargs: Any) -> Awaitable[AsyncHttpResponse]:
+    def _send_request(
+        self, request: HttpRequest, *, stream: bool = False, **kwargs: Any
+    ) -> Awaitable[AsyncHttpResponse]:
         """Runs the network request through the client's chained policies.
 
         >>> from azure.core.rest import HttpRequest
         >>> request = HttpRequest("GET", "https://www.example.org/")
         <HttpRequest [GET], url: 'https://www.example.org/'>
         >>> response = await client._send_request(request)
         <AsyncHttpResponse: 200 OK>
@@ -143,15 +168,15 @@
         :keyword bool stream: Whether the response payload will be streamed. Defaults to False.
         :return: The response of your network call. Does not do error handling on your response.
         :rtype: ~azure.core.rest.AsyncHttpResponse
         """
 
         request_copy = deepcopy(request)
         request_copy.url = self._client.format_url(request_copy.url)
-        return self._client.send_request(request_copy, **kwargs)
+        return self._client.send_request(request_copy, stream=stream, **kwargs)  # type: ignore
 
     async def close(self) -> None:
         await self._client.close()
 
     async def __aenter__(self) -> "MaintenanceManagementClient":
         await self._client.__aenter__()
         return self
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/_patch.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/__init__.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+from ._scheduled_event_operations import ScheduledEventOperations
 from ._public_maintenance_configurations_operations import PublicMaintenanceConfigurationsOperations
 from ._apply_updates_operations import ApplyUpdatesOperations
 from ._configuration_assignments_operations import ConfigurationAssignmentsOperations
 from ._maintenance_configurations_operations import MaintenanceConfigurationsOperations
 from ._maintenance_configurations_for_resource_group_operations import (
     MaintenanceConfigurationsForResourceGroupOperations,
 )
@@ -23,14 +24,15 @@
 from ._updates_operations import UpdatesOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
+    "ScheduledEventOperations",
     "PublicMaintenanceConfigurationsOperations",
     "ApplyUpdatesOperations",
     "ConfigurationAssignmentsOperations",
     "MaintenanceConfigurationsOperations",
     "MaintenanceConfigurationsForResourceGroupOperations",
     "ApplyUpdateForResourceGroupOperations",
     "ConfigurationAssignmentsWithinSubscriptionOperations",
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_apply_update_for_resource_group_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_apply_update_for_resource_group_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -56,15 +56,14 @@
     def list(self, resource_group_name: str, **kwargs: Any) -> AsyncIterable["_models.ApplyUpdate"]:
         """Get Configuration records within a subscription and resource group.
 
         Get Configuration records within a subscription and resource group.
 
         :param resource_group_name: Resource Group Name. Required.
         :type resource_group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ApplyUpdate or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.maintenance.models.ApplyUpdate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -78,64 +77,59 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     resource_group_name=resource_group_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ListApplyUpdate", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Maintenance/applyUpdates"
-    }
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_apply_updates_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_apply_updates_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -87,15 +87,14 @@
         :type resource_parent_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param apply_update_name: applyUpdate Id. Required.
         :type apply_update_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ApplyUpdate or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ApplyUpdate
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -106,53 +105,48 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ApplyUpdate] = kwargs.pop("cls", None)
 
-        request = build_get_parent_request(
+        _request = build_get_parent_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_parent_type=resource_parent_type,
             resource_parent_name=resource_parent_name,
             resource_type=resource_type,
             resource_name=resource_name,
             apply_update_name=apply_update_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get_parent.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ApplyUpdate", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get_parent.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/applyUpdates/{applyUpdateName}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace_async
     async def get(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_type: str,
@@ -170,15 +164,14 @@
         :type provider_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param apply_update_name: applyUpdate Id. Required.
         :type apply_update_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ApplyUpdate or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ApplyUpdate
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -189,51 +182,46 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ApplyUpdate] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_type=resource_type,
             resource_name=resource_name,
             apply_update_name=apply_update_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ApplyUpdate", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/applyUpdates/{applyUpdateName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     async def create_or_update_or_cancel(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_type: str,
@@ -259,29 +247,28 @@
         :param apply_update_name: ApplyUpdate name. Required.
         :type apply_update_name: str
         :param apply_update: The ApplyUpdate. Required.
         :type apply_update: ~azure.mgmt.maintenance.models.ApplyUpdate
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ApplyUpdate or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ApplyUpdate
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def create_or_update_or_cancel(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_type: str,
         resource_name: str,
         apply_update_name: str,
-        apply_update: IO,
+        apply_update: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ApplyUpdate:
         """Apply Updates to resource.
 
         Apply maintenance updates to resource.
@@ -293,33 +280,32 @@
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param apply_update_name: ApplyUpdate name. Required.
         :type apply_update_name: str
         :param apply_update: The ApplyUpdate. Required.
-        :type apply_update: IO
+        :type apply_update: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ApplyUpdate or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ApplyUpdate
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def create_or_update_or_cancel(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_type: str,
         resource_name: str,
         apply_update_name: str,
-        apply_update: Union[_models.ApplyUpdate, IO],
+        apply_update: Union[_models.ApplyUpdate, IO[bytes]],
         **kwargs: Any
     ) -> _models.ApplyUpdate:
         """Apply Updates to resource.
 
         Apply maintenance updates to resource.
 
         :param resource_group_name: Resource group name. Required.
@@ -328,20 +314,17 @@
         :type provider_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param apply_update_name: ApplyUpdate name. Required.
         :type apply_update_name: str
-        :param apply_update: The ApplyUpdate. Is either a ApplyUpdate type or a IO type. Required.
-        :type apply_update: ~azure.mgmt.maintenance.models.ApplyUpdate or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+        :param apply_update: The ApplyUpdate. Is either a ApplyUpdate type or a IO[bytes] type.
+         Required.
+        :type apply_update: ~azure.mgmt.maintenance.models.ApplyUpdate or IO[bytes]
         :return: ApplyUpdate or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ApplyUpdate
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -361,35 +344,34 @@
         _json = None
         _content = None
         if isinstance(apply_update, (IOBase, bytes)):
             _content = apply_update
         else:
             _json = self._serialize.body(apply_update, "ApplyUpdate")
 
-        request = build_create_or_update_or_cancel_request(
+        _request = build_create_or_update_or_cancel_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_type=resource_type,
             resource_name=resource_name,
             apply_update_name=apply_update_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create_or_update_or_cancel.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
@@ -402,18 +384,14 @@
             deserialized = self._deserialize("ApplyUpdate", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create_or_update_or_cancel.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/applyUpdates/{applyUpdateName}"
-    }
-
     @distributed_trace_async
     async def create_or_update_parent(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_parent_type: str,
         resource_parent_name: str,
@@ -433,15 +411,14 @@
         :type resource_parent_type: str
         :param resource_parent_name: Resource parent identifier. Required.
         :type resource_parent_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ApplyUpdate or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ApplyUpdate
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -452,33 +429,32 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ApplyUpdate] = kwargs.pop("cls", None)
 
-        request = build_create_or_update_parent_request(
+        _request = build_create_or_update_parent_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_parent_type=resource_parent_type,
             resource_parent_name=resource_parent_name,
             resource_type=resource_type,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.create_or_update_parent.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
@@ -491,18 +467,14 @@
             deserialized = self._deserialize("ApplyUpdate", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create_or_update_parent.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/applyUpdates/default"
-    }
-
     @distributed_trace_async
     async def create_or_update(
         self, resource_group_name: str, provider_name: str, resource_type: str, resource_name: str, **kwargs: Any
     ) -> _models.ApplyUpdate:
         """Apply Updates to resource.
 
         Apply maintenance updates to resource.
@@ -511,15 +483,14 @@
         :type resource_group_name: str
         :param provider_name: Resource provider name. Required.
         :type provider_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ApplyUpdate or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ApplyUpdate
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -530,31 +501,30 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ApplyUpdate] = kwargs.pop("cls", None)
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_type=resource_type,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
@@ -567,25 +537,20 @@
             deserialized = self._deserialize("ApplyUpdate", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/applyUpdates/default"
-    }
-
     @distributed_trace
     def list(self, **kwargs: Any) -> AsyncIterable["_models.ApplyUpdate"]:
         """Get Configuration records within a subscription.
 
         Get Configuration records within a subscription.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ApplyUpdate or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.maintenance.models.ApplyUpdate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -599,61 +564,58 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ListApplyUpdate", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/applyUpdates"}
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_configuration_assignments_for_resource_group_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_configuration_assignments_for_resource_group_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -33,15 +33,15 @@
     build_update_request,
 )
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class ConfigurationAssignmentsForResourceGroupOperations:
+class ConfigurationAssignmentsForResourceGroupOperations:  # pylint: disable=name-too-long
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.maintenance.aio.MaintenanceManagementClient`'s
         :attr:`configuration_assignments_for_resource_group` attribute.
@@ -64,15 +64,14 @@
 
         Get configuration assignment for resource..
 
         :param resource_group_name: Resource group name. Required.
         :type resource_group_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -83,48 +82,43 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConfigurationAssignment] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     async def create_or_update(
         self,
         resource_group_name: str,
         configuration_assignment_name: str,
         configuration_assignment: _models.ConfigurationAssignment,
@@ -141,72 +135,67 @@
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
         :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def create_or_update(
         self,
         resource_group_name: str,
         configuration_assignment_name: str,
-        configuration_assignment: IO,
+        configuration_assignment: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param resource_group_name: Resource group name. Required.
         :type resource_group_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
-        :type configuration_assignment: IO
+        :type configuration_assignment: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def create_or_update(
         self,
         resource_group_name: str,
         configuration_assignment_name: str,
-        configuration_assignment: Union[_models.ConfigurationAssignment, IO],
+        configuration_assignment: Union[_models.ConfigurationAssignment, IO[bytes]],
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param resource_group_name: Resource group name. Required.
         :type resource_group_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Is either a
-         ConfigurationAssignment type or a IO type. Required.
-        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ConfigurationAssignment type or a IO[bytes] type. Required.
+        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or
+         IO[bytes]
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -226,32 +215,31 @@
         _json = None
         _content = None
         if isinstance(configuration_assignment, (IOBase, bytes)):
             _content = configuration_assignment
         else:
             _json = self._serialize.body(configuration_assignment, "ConfigurationAssignment")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
@@ -264,18 +252,14 @@
             deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
-
     @overload
     async def update(
         self,
         resource_group_name: str,
         configuration_assignment_name: str,
         configuration_assignment: _models.ConfigurationAssignment,
         *,
@@ -291,72 +275,67 @@
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
         :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def update(
         self,
         resource_group_name: str,
         configuration_assignment_name: str,
-        configuration_assignment: IO,
+        configuration_assignment: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param resource_group_name: Resource group name. Required.
         :type resource_group_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
-        :type configuration_assignment: IO
+        :type configuration_assignment: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def update(
         self,
         resource_group_name: str,
         configuration_assignment_name: str,
-        configuration_assignment: Union[_models.ConfigurationAssignment, IO],
+        configuration_assignment: Union[_models.ConfigurationAssignment, IO[bytes]],
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param resource_group_name: Resource group name. Required.
         :type resource_group_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Is either a
-         ConfigurationAssignment type or a IO type. Required.
-        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ConfigurationAssignment type or a IO[bytes] type. Required.
+        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or
+         IO[bytes]
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -376,65 +355,59 @@
         _json = None
         _content = None
         if isinstance(configuration_assignment, (IOBase, bytes)):
             _content = configuration_assignment
         else:
             _json = self._serialize.body(configuration_assignment, "ConfigurationAssignment")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace_async
     async def delete(
         self, resource_group_name: str, configuration_assignment_name: str, **kwargs: Any
     ) -> Optional[_models.ConfigurationAssignment]:
         """Unregister configuration for resource.
 
         Unregister configuration for resource.
 
         :param resource_group_name: Resource group name. Required.
         :type resource_group_name: str
         :param configuration_assignment_name: Unique configuration assignment name. Required.
         :type configuration_assignment_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or None or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment or None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -445,43 +418,38 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.ConfigurationAssignment]] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
         if response.status_code == 200:
             deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_configuration_assignments_for_subscriptions_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_configuration_assignments_for_subscriptions_operations.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -33,15 +33,15 @@
     build_update_request,
 )
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class ConfigurationAssignmentsForSubscriptionsOperations:
+class ConfigurationAssignmentsForSubscriptionsOperations:  # pylint: disable=name-too-long
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.maintenance.aio.MaintenanceManagementClient`'s
         :attr:`configuration_assignments_for_subscriptions` attribute.
@@ -60,15 +60,14 @@
     async def get(self, configuration_assignment_name: str, **kwargs: Any) -> _models.ConfigurationAssignment:
         """Get configuration assignment.
 
         Get configuration assignment for resource..
 
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -79,47 +78,42 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConfigurationAssignment] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     async def create_or_update(
         self,
         configuration_assignment_name: str,
         configuration_assignment: _models.ConfigurationAssignment,
         *,
@@ -133,66 +127,61 @@
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
         :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def create_or_update(
         self,
         configuration_assignment_name: str,
-        configuration_assignment: IO,
+        configuration_assignment: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
-        :type configuration_assignment: IO
+        :type configuration_assignment: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def create_or_update(
         self,
         configuration_assignment_name: str,
-        configuration_assignment: Union[_models.ConfigurationAssignment, IO],
+        configuration_assignment: Union[_models.ConfigurationAssignment, IO[bytes]],
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Is either a
-         ConfigurationAssignment type or a IO type. Required.
-        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ConfigurationAssignment type or a IO[bytes] type. Required.
+        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or
+         IO[bytes]
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -212,31 +201,30 @@
         _json = None
         _content = None
         if isinstance(configuration_assignment, (IOBase, bytes)):
             _content = configuration_assignment
         else:
             _json = self._serialize.body(configuration_assignment, "ConfigurationAssignment")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
@@ -249,18 +237,14 @@
             deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
-
     @overload
     async def update(
         self,
         configuration_assignment_name: str,
         configuration_assignment: _models.ConfigurationAssignment,
         *,
         content_type: str = "application/json",
@@ -273,66 +257,61 @@
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
         :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def update(
         self,
         configuration_assignment_name: str,
-        configuration_assignment: IO,
+        configuration_assignment: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
-        :type configuration_assignment: IO
+        :type configuration_assignment: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def update(
         self,
         configuration_assignment_name: str,
-        configuration_assignment: Union[_models.ConfigurationAssignment, IO],
+        configuration_assignment: Union[_models.ConfigurationAssignment, IO[bytes]],
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Is either a
-         ConfigurationAssignment type or a IO type. Required.
-        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ConfigurationAssignment type or a IO[bytes] type. Required.
+        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or
+         IO[bytes]
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -352,62 +331,56 @@
         _json = None
         _content = None
         if isinstance(configuration_assignment, (IOBase, bytes)):
             _content = configuration_assignment
         else:
             _json = self._serialize.body(configuration_assignment, "ConfigurationAssignment")
 
-        request = build_update_request(
+        _request = build_update_request(
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace_async
     async def delete(
         self, configuration_assignment_name: str, **kwargs: Any
     ) -> Optional[_models.ConfigurationAssignment]:
         """Unregister configuration for resource.
 
         Unregister configuration for resource.
 
         :param configuration_assignment_name: Unique configuration assignment name. Required.
         :type configuration_assignment_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or None or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment or None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -418,42 +391,37 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.ConfigurationAssignment]] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
         if response.status_code == 200:
             deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_configuration_assignments_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_configuration_assignments_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -89,15 +89,14 @@
         :type resource_parent_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -108,53 +107,48 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConfigurationAssignment] = kwargs.pop("cls", None)
 
-        request = build_get_parent_request(
+        _request = build_get_parent_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_parent_type=resource_parent_type,
             resource_parent_name=resource_parent_name,
             resource_type=resource_type,
             resource_name=resource_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get_parent.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get_parent.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     async def create_or_update_parent(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_parent_type: str,
@@ -186,15 +180,14 @@
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
         :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def create_or_update_parent(
@@ -202,15 +195,15 @@
         resource_group_name: str,
         provider_name: str,
         resource_parent_type: str,
         resource_parent_name: str,
         resource_type: str,
         resource_name: str,
         configuration_assignment_name: str,
-        configuration_assignment: IO,
+        configuration_assignment: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
@@ -226,19 +219,18 @@
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
-        :type configuration_assignment: IO
+        :type configuration_assignment: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def create_or_update_parent(
@@ -246,15 +238,15 @@
         resource_group_name: str,
         provider_name: str,
         resource_parent_type: str,
         resource_parent_name: str,
         resource_type: str,
         resource_name: str,
         configuration_assignment_name: str,
-        configuration_assignment: Union[_models.ConfigurationAssignment, IO],
+        configuration_assignment: Union[_models.ConfigurationAssignment, IO[bytes]],
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param resource_group_name: Resource group name. Required.
@@ -268,20 +260,17 @@
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Is either a
-         ConfigurationAssignment type or a IO type. Required.
-        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ConfigurationAssignment type or a IO[bytes] type. Required.
+        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or
+         IO[bytes]
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -301,37 +290,36 @@
         _json = None
         _content = None
         if isinstance(configuration_assignment, (IOBase, bytes)):
             _content = configuration_assignment
         else:
             _json = self._serialize.body(configuration_assignment, "ConfigurationAssignment")
 
-        request = build_create_or_update_parent_request(
+        _request = build_create_or_update_parent_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_parent_type=resource_parent_type,
             resource_parent_name=resource_parent_name,
             resource_type=resource_type,
             resource_name=resource_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create_or_update_parent.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
@@ -344,18 +332,14 @@
             deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create_or_update_parent.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
-
     @distributed_trace_async
     async def delete_parent(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_parent_type: str,
         resource_parent_name: str,
@@ -378,15 +362,14 @@
         :type resource_parent_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param configuration_assignment_name: Unique configuration assignment name. Required.
         :type configuration_assignment_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or None or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment or None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -397,55 +380,50 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.ConfigurationAssignment]] = kwargs.pop("cls", None)
 
-        request = build_delete_parent_request(
+        _request = build_delete_parent_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_parent_type=resource_parent_type,
             resource_parent_name=resource_parent_name,
             resource_type=resource_type,
             resource_name=resource_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.delete_parent.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
         if response.status_code == 200:
             deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    delete_parent.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace_async
     async def get(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_type: str,
@@ -463,15 +441,14 @@
         :type provider_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -482,51 +459,46 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConfigurationAssignment] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_type=resource_type,
             resource_name=resource_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     async def create_or_update(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_type: str,
@@ -552,29 +524,28 @@
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
         :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def create_or_update(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_type: str,
         resource_name: str,
         configuration_assignment_name: str,
-        configuration_assignment: IO,
+        configuration_assignment: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
@@ -586,33 +557,32 @@
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
-        :type configuration_assignment: IO
+        :type configuration_assignment: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def create_or_update(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_type: str,
         resource_name: str,
         configuration_assignment_name: str,
-        configuration_assignment: Union[_models.ConfigurationAssignment, IO],
+        configuration_assignment: Union[_models.ConfigurationAssignment, IO[bytes]],
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param resource_group_name: Resource group name. Required.
@@ -622,20 +592,17 @@
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Is either a
-         ConfigurationAssignment type or a IO type. Required.
-        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ConfigurationAssignment type or a IO[bytes] type. Required.
+        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or
+         IO[bytes]
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -655,35 +622,34 @@
         _json = None
         _content = None
         if isinstance(configuration_assignment, (IOBase, bytes)):
             _content = configuration_assignment
         else:
             _json = self._serialize.body(configuration_assignment, "ConfigurationAssignment")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_type=resource_type,
             resource_name=resource_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
@@ -696,18 +662,14 @@
             deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
-
     @distributed_trace_async
     async def delete(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_type: str,
         resource_name: str,
@@ -724,15 +686,14 @@
         :type provider_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param configuration_assignment_name: Unique configuration assignment name. Required.
         :type configuration_assignment_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or None or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment or None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -743,53 +704,48 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.ConfigurationAssignment]] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_type=resource_type,
             resource_name=resource_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
         if response.status_code == 200:
             deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace
     def list_parent(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_parent_type: str,
@@ -810,15 +766,14 @@
         :type resource_parent_type: str
         :param resource_parent_name: Resource parent identifier. Required.
         :type resource_parent_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ConfigurationAssignment or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.maintenance.models.ConfigurationAssignment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -834,77 +789,72 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_parent_request(
+                _request = build_list_parent_request(
                     resource_group_name=resource_group_name,
                     provider_name=provider_name,
                     resource_parent_type=resource_parent_type,
                     resource_parent_name=resource_parent_name,
                     resource_type=resource_type,
                     resource_name=resource_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_parent.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ListConfigurationAssignmentsResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_parent.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments"
-    }
-
     @distributed_trace
     def list(
         self, resource_group_name: str, provider_name: str, resource_type: str, resource_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.ConfigurationAssignment"]:
         """List configurationAssignments for resource.
 
         List configurationAssignments for resource.
@@ -913,15 +863,14 @@
         :type resource_group_name: str
         :param provider_name: Resource provider name. Required.
         :type provider_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ConfigurationAssignment or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.maintenance.models.ConfigurationAssignment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -937,67 +886,62 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     resource_group_name=resource_group_name,
                     provider_name=provider_name,
                     resource_type=resource_type,
                     resource_name=resource_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ListConfigurationAssignmentsResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments"
-    }
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_configuration_assignments_within_subscription_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_maintenance_configurations_for_resource_group_operations.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -23,116 +23,115 @@
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
 from ... import models as _models
 from ..._vendor import _convert_request
-from ...operations._configuration_assignments_within_subscription_operations import build_list_request
+from ...operations._maintenance_configurations_for_resource_group_operations import build_list_request
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class ConfigurationAssignmentsWithinSubscriptionOperations:
+class MaintenanceConfigurationsForResourceGroupOperations:  # pylint: disable=name-too-long
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.maintenance.aio.MaintenanceManagementClient`'s
-        :attr:`configuration_assignments_within_subscription` attribute.
+        :attr:`maintenance_configurations_for_resource_group` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, **kwargs: Any) -> AsyncIterable["_models.ConfigurationAssignment"]:
-        """Get configuration assignment within a subscription.
+    def list(self, resource_group_name: str, **kwargs: Any) -> AsyncIterable["_models.MaintenanceConfiguration"]:
+        """Get Configuration records within a subscription and resource group.
 
-        Get configuration assignment within a subscription.
+        Get Configuration records within a subscription and resource group.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either ConfigurationAssignment or the result of
+        :param resource_group_name: Resource Group Name. Required.
+        :type resource_group_name: str
+        :return: An iterator like instance of either MaintenanceConfiguration or the result of
          cls(response)
         :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.maintenance.models.ConfigurationAssignment]
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.maintenance.models.MaintenanceConfiguration]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.ListConfigurationAssignmentsResult] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ListMaintenanceConfigurationsResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
+                    resource_group_name=resource_group_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
-            deserialized = self._deserialize("ListConfigurationAssignmentsResult", pipeline_response)
+            deserialized = self._deserialize("ListMaintenanceConfigurationsResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/configurationAssignments"}
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_maintenance_configurations_for_resource_group_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_maintenance_configurations_for_resource_group_operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,103 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
+from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
 import urllib.parse
 
-from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
+from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import AsyncHttpResponse
+from azure.core.pipeline.transport import HttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from ... import models as _models
-from ..._vendor import _convert_request
-from ...operations._maintenance_configurations_for_resource_group_operations import build_list_request
+from .. import models as _models
+from .._serialization import Serializer
+from .._vendor import _convert_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
+_SERIALIZER = Serializer()
+_SERIALIZER.client_side_validation = False
 
-class MaintenanceConfigurationsForResourceGroupOperations:
+
+def build_list_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
+    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
+
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
+    accept = _headers.pop("Accept", "application/json")
+
+    # Construct URL
+    _url = kwargs.pop(
+        "template_url",
+        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Maintenance/maintenanceConfigurations",
+    )  # pylint: disable=line-too-long
+    path_format_arguments = {
+        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
+        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
+    }
+
+    _url: str = _url.format(**path_format_arguments)  # type: ignore
+
+    # Construct parameters
+    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
+
+    # Construct headers
+    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
+
+    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
+
+
+class MaintenanceConfigurationsForResourceGroupOperations:  # pylint: disable=name-too-long
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.maintenance.aio.MaintenanceManagementClient`'s
+        :class:`~azure.mgmt.maintenance.MaintenanceManagementClient`'s
         :attr:`maintenance_configurations_for_resource_group` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs) -> None:
+    def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, resource_group_name: str, **kwargs: Any) -> AsyncIterable["_models.MaintenanceConfiguration"]:
+    def list(self, resource_group_name: str, **kwargs: Any) -> Iterable["_models.MaintenanceConfiguration"]:
         """Get Configuration records within a subscription and resource group.
 
         Get Configuration records within a subscription and resource group.
 
         :param resource_group_name: Resource Group Name. Required.
         :type resource_group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either MaintenanceConfiguration or the result of
          cls(response)
-        :rtype:
-         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.maintenance.models.MaintenanceConfiguration]
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.maintenance.models.MaintenanceConfiguration]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ListMaintenanceConfigurationsResult] = kwargs.pop("cls", None)
@@ -80,64 +109,59 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     resource_group_name=resource_group_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
-        async def extract_data(pipeline_response):
+        def extract_data(pipeline_response):
             deserialized = self._deserialize("ListMaintenanceConfigurationsResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
-            return None, AsyncList(list_of_elem)
+            return None, iter(list_of_elem)
 
-        async def get_next(next_link=None):
-            request = prepare_request(next_link)
+        def get_next(next_link=None):
+            _request = prepare_request(next_link)
 
             _stream = False
-            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Maintenance/maintenanceConfigurations"
-    }
+        return ItemPaged(get_next, extract_data)
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_maintenance_configurations_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_maintenance_configurations_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -68,15 +68,14 @@
 
         Get Configuration record.
 
         :param resource_group_name: Resource Group Name. Required.
         :type resource_group_name: str
         :param resource_name: Maintenance Configuration Name. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: MaintenanceConfiguration or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -87,48 +86,43 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MaintenanceConfiguration] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("MaintenanceConfiguration", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/maintenanceConfigurations/{resourceName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     async def create_or_update(
         self,
         resource_group_name: str,
         resource_name: str,
         configuration: _models.MaintenanceConfiguration,
@@ -145,72 +139,66 @@
         :param resource_name: Maintenance Configuration Name. Required.
         :type resource_name: str
         :param configuration: The configuration. Required.
         :type configuration: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: MaintenanceConfiguration or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def create_or_update(
         self,
         resource_group_name: str,
         resource_name: str,
-        configuration: IO,
+        configuration: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.MaintenanceConfiguration:
         """Create or Update configuration record.
 
         Create or Update configuration record.
 
         :param resource_group_name: Resource Group Name. Required.
         :type resource_group_name: str
         :param resource_name: Maintenance Configuration Name. Required.
         :type resource_name: str
         :param configuration: The configuration. Required.
-        :type configuration: IO
+        :type configuration: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: MaintenanceConfiguration or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def create_or_update(
         self,
         resource_group_name: str,
         resource_name: str,
-        configuration: Union[_models.MaintenanceConfiguration, IO],
+        configuration: Union[_models.MaintenanceConfiguration, IO[bytes]],
         **kwargs: Any
     ) -> _models.MaintenanceConfiguration:
         """Create or Update configuration record.
 
         Create or Update configuration record.
 
         :param resource_group_name: Resource Group Name. Required.
         :type resource_group_name: str
         :param resource_name: Maintenance Configuration Name. Required.
         :type resource_name: str
-        :param configuration: The configuration. Is either a MaintenanceConfiguration type or a IO
-         type. Required.
-        :type configuration: ~azure.mgmt.maintenance.models.MaintenanceConfiguration or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+        :param configuration: The configuration. Is either a MaintenanceConfiguration type or a
+         IO[bytes] type. Required.
+        :type configuration: ~azure.mgmt.maintenance.models.MaintenanceConfiguration or IO[bytes]
         :return: MaintenanceConfiguration or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -230,32 +218,31 @@
         _json = None
         _content = None
         if isinstance(configuration, (IOBase, bytes)):
             _content = configuration
         else:
             _json = self._serialize.body(configuration, "MaintenanceConfiguration")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
@@ -268,31 +255,26 @@
             deserialized = self._deserialize("MaintenanceConfiguration", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/maintenanceConfigurations/{resourceName}"
-    }
-
     @distributed_trace_async
     async def delete(
         self, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> Optional[_models.MaintenanceConfiguration]:
         """Delete Configuration record.
 
         Delete Configuration record.
 
         :param resource_group_name: Resource Group Name. Required.
         :type resource_group_name: str
         :param resource_name: Maintenance Configuration Name. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: MaintenanceConfiguration or None or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.MaintenanceConfiguration or None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -303,50 +285,45 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.MaintenanceConfiguration]] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
         if response.status_code == 200:
             deserialized = self._deserialize("MaintenanceConfiguration", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/maintenanceConfigurations/{resourceName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     async def update(
         self,
         resource_group_name: str,
         resource_name: str,
         configuration: _models.MaintenanceConfiguration,
@@ -363,72 +340,66 @@
         :param resource_name: Maintenance Configuration Name. Required.
         :type resource_name: str
         :param configuration: The configuration. Required.
         :type configuration: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: MaintenanceConfiguration or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     async def update(
         self,
         resource_group_name: str,
         resource_name: str,
-        configuration: IO,
+        configuration: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.MaintenanceConfiguration:
         """Patch configuration record.
 
         Patch configuration record.
 
         :param resource_group_name: Resource Group Name. Required.
         :type resource_group_name: str
         :param resource_name: Maintenance Configuration Name. Required.
         :type resource_name: str
         :param configuration: The configuration. Required.
-        :type configuration: IO
+        :type configuration: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: MaintenanceConfiguration or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace_async
     async def update(
         self,
         resource_group_name: str,
         resource_name: str,
-        configuration: Union[_models.MaintenanceConfiguration, IO],
+        configuration: Union[_models.MaintenanceConfiguration, IO[bytes]],
         **kwargs: Any
     ) -> _models.MaintenanceConfiguration:
         """Patch configuration record.
 
         Patch configuration record.
 
         :param resource_group_name: Resource Group Name. Required.
         :type resource_group_name: str
         :param resource_name: Maintenance Configuration Name. Required.
         :type resource_name: str
-        :param configuration: The configuration. Is either a MaintenanceConfiguration type or a IO
-         type. Required.
-        :type configuration: ~azure.mgmt.maintenance.models.MaintenanceConfiguration or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+        :param configuration: The configuration. Is either a MaintenanceConfiguration type or a
+         IO[bytes] type. Required.
+        :type configuration: ~azure.mgmt.maintenance.models.MaintenanceConfiguration or IO[bytes]
         :return: MaintenanceConfiguration or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -448,59 +419,53 @@
         _json = None
         _content = None
         if isinstance(configuration, (IOBase, bytes)):
             _content = configuration
         else:
             _json = self._serialize.body(configuration, "MaintenanceConfiguration")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("MaintenanceConfiguration", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/maintenanceConfigurations/{resourceName}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace
     def list(self, **kwargs: Any) -> AsyncIterable["_models.MaintenanceConfiguration"]:
         """Get Configuration records within a subscription.
 
         Get Configuration records within a subscription.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either MaintenanceConfiguration or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.maintenance.models.MaintenanceConfiguration]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -516,61 +481,58 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ListMaintenanceConfigurationsResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/maintenanceConfigurations"}
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -54,15 +54,14 @@
 
     @distributed_trace
     def list(self, **kwargs: Any) -> AsyncIterable["_models.Operation"]:
         """List available operations.
 
         List the available operations supported by the Microsoft.Maintenance resource provider.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Operation or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.maintenance.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -76,60 +75,57 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("OperationsListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/providers/Microsoft.Maintenance/operations"}
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_patch.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_public_maintenance_configurations_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_public_maintenance_configurations_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -30,15 +30,15 @@
 from ..._vendor import _convert_request
 from ...operations._public_maintenance_configurations_operations import build_get_request, build_list_request
 
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
 
-class PublicMaintenanceConfigurationsOperations:
+class PublicMaintenanceConfigurationsOperations:  # pylint: disable=name-too-long
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.maintenance.aio.MaintenanceManagementClient`'s
         :attr:`public_maintenance_configurations` attribute.
@@ -55,15 +55,14 @@
 
     @distributed_trace
     def list(self, **kwargs: Any) -> AsyncIterable["_models.MaintenanceConfiguration"]:
         """Get Public Maintenance Configuration records.
 
         Get Public Maintenance Configuration records.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either MaintenanceConfiguration or the result of
          cls(response)
         :rtype:
          ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.maintenance.models.MaintenanceConfiguration]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
@@ -79,80 +78,74 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ListMaintenanceConfigurationsResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/publicMaintenanceConfigurations"
-    }
-
     @distributed_trace_async
     async def get(self, resource_name: str, **kwargs: Any) -> _models.MaintenanceConfiguration:
         """Get Public Maintenance Configuration record.
 
         Get Public Maintenance Configuration record.
 
         :param resource_name: Maintenance Configuration Name. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: MaintenanceConfiguration or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -163,40 +156,35 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MaintenanceConfiguration] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("MaintenanceConfiguration", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/publicMaintenanceConfigurations/{resourceName}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/aio/operations/_updates_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_updates_operations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -75,15 +75,14 @@
         :type resource_parent_type: str
         :param resource_parent_name: Resource parent identifier. Required.
         :type resource_parent_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Update or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.maintenance.models.Update]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -97,77 +96,72 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_parent_request(
+                _request = build_list_parent_request(
                     resource_group_name=resource_group_name,
                     provider_name=provider_name,
                     resource_parent_type=resource_parent_type,
                     resource_parent_name=resource_parent_name,
                     resource_type=resource_type,
                     resource_name=resource_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_parent.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ListUpdatesResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
 
-    list_parent.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/updates"
-    }
-
     @distributed_trace
     def list(
         self, resource_group_name: str, provider_name: str, resource_type: str, resource_name: str, **kwargs: Any
     ) -> AsyncIterable["_models.Update"]:
         """Get Updates to resource.
 
         Get updates to resources.
@@ -176,15 +170,14 @@
         :type resource_group_name: str
         :param provider_name: Resource provider name. Required.
         :type provider_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Update or the result of cls(response)
         :rtype: ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.maintenance.models.Update]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -198,67 +191,62 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     resource_group_name=resource_group_name,
                     provider_name=provider_name,
                     resource_type=resource_type,
                     resource_name=resource_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         async def extract_data(pipeline_response):
             deserialized = self._deserialize("ListUpdatesResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, AsyncList(list_of_elem)
 
         async def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return AsyncItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/updates"
-    }
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/models/__init__.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from ._models_py3 import ListUpdatesResult
 from ._models_py3 import MaintenanceConfiguration
 from ._models_py3 import MaintenanceError
 from ._models_py3 import Operation
 from ._models_py3 import OperationInfo
 from ._models_py3 import OperationsListResult
 from ._models_py3 import Resource
+from ._models_py3 import ScheduledEventApproveResponse
 from ._models_py3 import SystemData
 from ._models_py3 import TagSettingsProperties
 from ._models_py3 import Update
 
 from ._maintenance_management_client_enums import CreatedByType
 from ._maintenance_management_client_enums import ImpactType
 from ._maintenance_management_client_enums import MaintenanceScope
@@ -52,14 +53,15 @@
     "ListUpdatesResult",
     "MaintenanceConfiguration",
     "MaintenanceError",
     "Operation",
     "OperationInfo",
     "OperationsListResult",
     "Resource",
+    "ScheduledEventApproveResponse",
     "SystemData",
     "TagSettingsProperties",
     "Update",
     "CreatedByType",
     "ImpactType",
     "MaintenanceScope",
     "RebootOptions",
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/models/_maintenance_management_client_enums.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/models/_maintenance_management_client_enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 
 class MaintenanceScope(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Gets or sets maintenanceScope of the configuration."""
 
     HOST = "Host"
     """This maintenance scope controls installation of azure platform updates i.e. services on
-    #: physical nodes hosting customer VMs."""
+    physical nodes hosting customer VMs."""
     RESOURCE = "Resource"
     """This maintenance scope controls the default update maintenance of the Azure Resource"""
     OS_IMAGE = "OSImage"
     """This maintenance scope controls os image installation on VM/VMSS"""
     EXTENSION = "Extension"
     """This maintenance scope controls extension installation on VM/VMSS"""
     IN_GUEST_PATCH = "InGuestPatch"
@@ -82,18 +82,18 @@
     """Updates installation failed but are ready to retry again."""
     RETRY_LATER = "RetryLater"
     """Updates installation failed and should be retried later."""
     NO_UPDATES_PENDING = "NoUpdatesPending"
     """No updates are pending."""
     CANCEL = "Cancel"
     """Cancel the schedule and stop creating PMR for resources part of it. Applicable to Maintenance
-    #: Configuration resource type only."""
+    Configuration resource type only."""
     CANCELLED = "Cancelled"
     """Send the Cancelled response to the user if request came to cancel the schedule. Applicable to
-    #: Maintenance Configuration resource type only."""
+    Maintenance Configuration resource type only."""
 
 
 class Visibility(str, Enum, metaclass=CaseInsensitiveEnumMeta):
     """Gets or sets the visibility of the configuration. The default value is 'Custom'."""
 
     CUSTOM = "Custom"
     """Only visible to users with permissions."""
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/models/_models_py3.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/models/_models_py3.py`

 * *Files 2% similar despite different names*

```diff
@@ -792,14 +792,34 @@
         :keyword value: A collection of operations.
         :paramtype value: list[~azure.mgmt.maintenance.models.Operation]
         """
         super().__init__(**kwargs)
         self.value = value
 
 
+class ScheduledEventApproveResponse(_serialization.Model):
+    """Response of scheduled event acknowledge.
+
+    :ivar value: Successfully Approved.
+    :vartype value: str
+    """
+
+    _attribute_map = {
+        "value": {"key": "value", "type": "str"},
+    }
+
+    def __init__(self, *, value: Optional[str] = None, **kwargs: Any) -> None:
+        """
+        :keyword value: Successfully Approved.
+        :paramtype value: str
+        """
+        super().__init__(**kwargs)
+        self.value = value
+
+
 class SystemData(_serialization.Model):
     """Metadata pertaining to creation and last modification of the resource.
 
     :ivar created_by: The identity that created the resource.
     :vartype created_by: str
     :ivar created_by_type: The type of identity that created the resource. Known values are:
      "User", "Application", "ManagedIdentity", and "Key".
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/models/_patch.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/models/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/__init__.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
+from ._scheduled_event_operations import ScheduledEventOperations
 from ._public_maintenance_configurations_operations import PublicMaintenanceConfigurationsOperations
 from ._apply_updates_operations import ApplyUpdatesOperations
 from ._configuration_assignments_operations import ConfigurationAssignmentsOperations
 from ._maintenance_configurations_operations import MaintenanceConfigurationsOperations
 from ._maintenance_configurations_for_resource_group_operations import (
     MaintenanceConfigurationsForResourceGroupOperations,
 )
@@ -23,14 +24,15 @@
 from ._updates_operations import UpdatesOperations
 
 from ._patch import __all__ as _patch_all
 from ._patch import *  # pylint: disable=unused-wildcard-import
 from ._patch import patch_sdk as _patch_sdk
 
 __all__ = [
+    "ScheduledEventOperations",
     "PublicMaintenanceConfigurationsOperations",
     "ApplyUpdatesOperations",
     "ConfigurationAssignmentsOperations",
     "MaintenanceConfigurationsOperations",
     "MaintenanceConfigurationsForResourceGroupOperations",
     "ApplyUpdateForResourceGroupOperations",
     "ConfigurationAssignmentsWithinSubscriptionOperations",
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_apply_update_for_resource_group_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_apply_update_for_resource_group_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -36,15 +36,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Maintenance/applyUpdates",
     )  # pylint: disable=line-too-long
@@ -87,15 +87,14 @@
     def list(self, resource_group_name: str, **kwargs: Any) -> Iterable["_models.ApplyUpdate"]:
         """Get Configuration records within a subscription and resource group.
 
         Get Configuration records within a subscription and resource group.
 
         :param resource_group_name: Resource Group Name. Required.
         :type resource_group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ApplyUpdate or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.maintenance.models.ApplyUpdate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -109,64 +108,59 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     resource_group_name=resource_group_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ListApplyUpdate", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Maintenance/applyUpdates"
-    }
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_apply_updates_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_apply_updates_operations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -47,15 +47,15 @@
     apply_update_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/applyUpdates/{applyUpdateName}",
     )  # pylint: disable=line-too-long
@@ -89,15 +89,15 @@
     apply_update_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/applyUpdates/{applyUpdateName}",
     )  # pylint: disable=line-too-long
@@ -129,15 +129,15 @@
     apply_update_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/applyUpdates/{applyUpdateName}",
@@ -173,15 +173,15 @@
     resource_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/applyUpdates/default",
     )  # pylint: disable=line-too-long
@@ -213,15 +213,15 @@
     resource_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/applyUpdates/default",
     )  # pylint: disable=line-too-long
@@ -244,15 +244,15 @@
     return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop("template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/applyUpdates")
     path_format_arguments = {
         "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
     }
@@ -313,15 +313,14 @@
         :type resource_parent_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param apply_update_name: applyUpdate Id. Required.
         :type apply_update_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ApplyUpdate or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ApplyUpdate
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -332,53 +331,48 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ApplyUpdate] = kwargs.pop("cls", None)
 
-        request = build_get_parent_request(
+        _request = build_get_parent_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_parent_type=resource_parent_type,
             resource_parent_name=resource_parent_name,
             resource_type=resource_type,
             resource_name=resource_name,
             apply_update_name=apply_update_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get_parent.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ApplyUpdate", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get_parent.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/applyUpdates/{applyUpdateName}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace
     def get(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_type: str,
@@ -396,15 +390,14 @@
         :type provider_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param apply_update_name: applyUpdate Id. Required.
         :type apply_update_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ApplyUpdate or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ApplyUpdate
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -415,51 +408,46 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ApplyUpdate] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_type=resource_type,
             resource_name=resource_name,
             apply_update_name=apply_update_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ApplyUpdate", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/applyUpdates/{applyUpdateName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     def create_or_update_or_cancel(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_type: str,
@@ -485,29 +473,28 @@
         :param apply_update_name: ApplyUpdate name. Required.
         :type apply_update_name: str
         :param apply_update: The ApplyUpdate. Required.
         :type apply_update: ~azure.mgmt.maintenance.models.ApplyUpdate
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ApplyUpdate or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ApplyUpdate
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def create_or_update_or_cancel(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_type: str,
         resource_name: str,
         apply_update_name: str,
-        apply_update: IO,
+        apply_update: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ApplyUpdate:
         """Apply Updates to resource.
 
         Apply maintenance updates to resource.
@@ -519,33 +506,32 @@
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param apply_update_name: ApplyUpdate name. Required.
         :type apply_update_name: str
         :param apply_update: The ApplyUpdate. Required.
-        :type apply_update: IO
+        :type apply_update: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ApplyUpdate or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ApplyUpdate
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def create_or_update_or_cancel(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_type: str,
         resource_name: str,
         apply_update_name: str,
-        apply_update: Union[_models.ApplyUpdate, IO],
+        apply_update: Union[_models.ApplyUpdate, IO[bytes]],
         **kwargs: Any
     ) -> _models.ApplyUpdate:
         """Apply Updates to resource.
 
         Apply maintenance updates to resource.
 
         :param resource_group_name: Resource group name. Required.
@@ -554,20 +540,17 @@
         :type provider_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param apply_update_name: ApplyUpdate name. Required.
         :type apply_update_name: str
-        :param apply_update: The ApplyUpdate. Is either a ApplyUpdate type or a IO type. Required.
-        :type apply_update: ~azure.mgmt.maintenance.models.ApplyUpdate or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+        :param apply_update: The ApplyUpdate. Is either a ApplyUpdate type or a IO[bytes] type.
+         Required.
+        :type apply_update: ~azure.mgmt.maintenance.models.ApplyUpdate or IO[bytes]
         :return: ApplyUpdate or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ApplyUpdate
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -587,35 +570,34 @@
         _json = None
         _content = None
         if isinstance(apply_update, (IOBase, bytes)):
             _content = apply_update
         else:
             _json = self._serialize.body(apply_update, "ApplyUpdate")
 
-        request = build_create_or_update_or_cancel_request(
+        _request = build_create_or_update_or_cancel_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_type=resource_type,
             resource_name=resource_name,
             apply_update_name=apply_update_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create_or_update_or_cancel.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
@@ -628,18 +610,14 @@
             deserialized = self._deserialize("ApplyUpdate", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create_or_update_or_cancel.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/applyUpdates/{applyUpdateName}"
-    }
-
     @distributed_trace
     def create_or_update_parent(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_parent_type: str,
         resource_parent_name: str,
@@ -659,15 +637,14 @@
         :type resource_parent_type: str
         :param resource_parent_name: Resource parent identifier. Required.
         :type resource_parent_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ApplyUpdate or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ApplyUpdate
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -678,33 +655,32 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ApplyUpdate] = kwargs.pop("cls", None)
 
-        request = build_create_or_update_parent_request(
+        _request = build_create_or_update_parent_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_parent_type=resource_parent_type,
             resource_parent_name=resource_parent_name,
             resource_type=resource_type,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.create_or_update_parent.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
@@ -717,18 +693,14 @@
             deserialized = self._deserialize("ApplyUpdate", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create_or_update_parent.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/applyUpdates/default"
-    }
-
     @distributed_trace
     def create_or_update(
         self, resource_group_name: str, provider_name: str, resource_type: str, resource_name: str, **kwargs: Any
     ) -> _models.ApplyUpdate:
         """Apply Updates to resource.
 
         Apply maintenance updates to resource.
@@ -737,15 +709,14 @@
         :type resource_group_name: str
         :param provider_name: Resource provider name. Required.
         :type provider_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ApplyUpdate or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ApplyUpdate
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -756,31 +727,30 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ApplyUpdate] = kwargs.pop("cls", None)
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_type=resource_type,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
@@ -793,25 +763,20 @@
             deserialized = self._deserialize("ApplyUpdate", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/applyUpdates/default"
-    }
-
     @distributed_trace
     def list(self, **kwargs: Any) -> Iterable["_models.ApplyUpdate"]:
         """Get Configuration records within a subscription.
 
         Get Configuration records within a subscription.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ApplyUpdate or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.maintenance.models.ApplyUpdate]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -825,61 +790,58 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ListApplyUpdate", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/applyUpdates"}
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_configuration_assignments_for_resource_group_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_configuration_assignments_for_resource_group_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -37,15 +37,15 @@
 
 def build_get_request(
     resource_group_name: str, configuration_assignment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}",
     )  # pylint: disable=line-too-long
@@ -70,15 +70,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, configuration_assignment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}",
@@ -106,15 +106,15 @@
 
 def build_update_request(
     resource_group_name: str, configuration_assignment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}",
@@ -142,15 +142,15 @@
 
 def build_delete_request(
     resource_group_name: str, configuration_assignment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}",
     )  # pylint: disable=line-too-long
@@ -169,15 +169,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class ConfigurationAssignmentsForResourceGroupOperations:
+class ConfigurationAssignmentsForResourceGroupOperations:  # pylint: disable=name-too-long
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.maintenance.MaintenanceManagementClient`'s
         :attr:`configuration_assignments_for_resource_group` attribute.
@@ -200,15 +200,14 @@
 
         Get configuration assignment for resource..
 
         :param resource_group_name: Resource group name. Required.
         :type resource_group_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -219,48 +218,43 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConfigurationAssignment] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     def create_or_update(
         self,
         resource_group_name: str,
         configuration_assignment_name: str,
         configuration_assignment: _models.ConfigurationAssignment,
@@ -277,72 +271,67 @@
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
         :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def create_or_update(
         self,
         resource_group_name: str,
         configuration_assignment_name: str,
-        configuration_assignment: IO,
+        configuration_assignment: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param resource_group_name: Resource group name. Required.
         :type resource_group_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
-        :type configuration_assignment: IO
+        :type configuration_assignment: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def create_or_update(
         self,
         resource_group_name: str,
         configuration_assignment_name: str,
-        configuration_assignment: Union[_models.ConfigurationAssignment, IO],
+        configuration_assignment: Union[_models.ConfigurationAssignment, IO[bytes]],
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param resource_group_name: Resource group name. Required.
         :type resource_group_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Is either a
-         ConfigurationAssignment type or a IO type. Required.
-        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ConfigurationAssignment type or a IO[bytes] type. Required.
+        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or
+         IO[bytes]
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -362,32 +351,31 @@
         _json = None
         _content = None
         if isinstance(configuration_assignment, (IOBase, bytes)):
             _content = configuration_assignment
         else:
             _json = self._serialize.body(configuration_assignment, "ConfigurationAssignment")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
@@ -400,18 +388,14 @@
             deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
-
     @overload
     def update(
         self,
         resource_group_name: str,
         configuration_assignment_name: str,
         configuration_assignment: _models.ConfigurationAssignment,
         *,
@@ -427,72 +411,67 @@
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
         :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def update(
         self,
         resource_group_name: str,
         configuration_assignment_name: str,
-        configuration_assignment: IO,
+        configuration_assignment: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param resource_group_name: Resource group name. Required.
         :type resource_group_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
-        :type configuration_assignment: IO
+        :type configuration_assignment: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def update(
         self,
         resource_group_name: str,
         configuration_assignment_name: str,
-        configuration_assignment: Union[_models.ConfigurationAssignment, IO],
+        configuration_assignment: Union[_models.ConfigurationAssignment, IO[bytes]],
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param resource_group_name: Resource group name. Required.
         :type resource_group_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Is either a
-         ConfigurationAssignment type or a IO type. Required.
-        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ConfigurationAssignment type or a IO[bytes] type. Required.
+        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or
+         IO[bytes]
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -512,65 +491,59 @@
         _json = None
         _content = None
         if isinstance(configuration_assignment, (IOBase, bytes)):
             _content = configuration_assignment
         else:
             _json = self._serialize.body(configuration_assignment, "ConfigurationAssignment")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace
     def delete(
         self, resource_group_name: str, configuration_assignment_name: str, **kwargs: Any
     ) -> Optional[_models.ConfigurationAssignment]:
         """Unregister configuration for resource.
 
         Unregister configuration for resource.
 
         :param resource_group_name: Resource group name. Required.
         :type resource_group_name: str
         :param configuration_assignment_name: Unique configuration assignment name. Required.
         :type configuration_assignment_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or None or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment or None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -581,43 +554,38 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.ConfigurationAssignment]] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
         if response.status_code == 200:
             deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_configuration_assignments_for_subscriptions_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_configuration_assignments_for_subscriptions_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -35,15 +35,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_request(configuration_assignment_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}",
     )  # pylint: disable=line-too-long
@@ -67,15 +67,15 @@
 
 def build_create_or_update_request(
     configuration_assignment_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}",
@@ -100,15 +100,15 @@
     return HttpRequest(method="PUT", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_update_request(configuration_assignment_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}",
@@ -133,15 +133,15 @@
     return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_delete_request(configuration_assignment_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}",
     )  # pylint: disable=line-too-long
@@ -159,15 +159,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="DELETE", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class ConfigurationAssignmentsForSubscriptionsOperations:
+class ConfigurationAssignmentsForSubscriptionsOperations:  # pylint: disable=name-too-long
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.maintenance.MaintenanceManagementClient`'s
         :attr:`configuration_assignments_for_subscriptions` attribute.
@@ -186,15 +186,14 @@
     def get(self, configuration_assignment_name: str, **kwargs: Any) -> _models.ConfigurationAssignment:
         """Get configuration assignment.
 
         Get configuration assignment for resource..
 
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -205,47 +204,42 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConfigurationAssignment] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     def create_or_update(
         self,
         configuration_assignment_name: str,
         configuration_assignment: _models.ConfigurationAssignment,
         *,
@@ -259,66 +253,61 @@
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
         :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def create_or_update(
         self,
         configuration_assignment_name: str,
-        configuration_assignment: IO,
+        configuration_assignment: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
-        :type configuration_assignment: IO
+        :type configuration_assignment: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def create_or_update(
         self,
         configuration_assignment_name: str,
-        configuration_assignment: Union[_models.ConfigurationAssignment, IO],
+        configuration_assignment: Union[_models.ConfigurationAssignment, IO[bytes]],
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Is either a
-         ConfigurationAssignment type or a IO type. Required.
-        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ConfigurationAssignment type or a IO[bytes] type. Required.
+        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or
+         IO[bytes]
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -338,31 +327,30 @@
         _json = None
         _content = None
         if isinstance(configuration_assignment, (IOBase, bytes)):
             _content = configuration_assignment
         else:
             _json = self._serialize.body(configuration_assignment, "ConfigurationAssignment")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
@@ -375,18 +363,14 @@
             deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
-
     @overload
     def update(
         self,
         configuration_assignment_name: str,
         configuration_assignment: _models.ConfigurationAssignment,
         *,
         content_type: str = "application/json",
@@ -399,66 +383,61 @@
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
         :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def update(
         self,
         configuration_assignment_name: str,
-        configuration_assignment: IO,
+        configuration_assignment: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
-        :type configuration_assignment: IO
+        :type configuration_assignment: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def update(
         self,
         configuration_assignment_name: str,
-        configuration_assignment: Union[_models.ConfigurationAssignment, IO],
+        configuration_assignment: Union[_models.ConfigurationAssignment, IO[bytes]],
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Is either a
-         ConfigurationAssignment type or a IO type. Required.
-        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ConfigurationAssignment type or a IO[bytes] type. Required.
+        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or
+         IO[bytes]
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -478,60 +457,54 @@
         _json = None
         _content = None
         if isinstance(configuration_assignment, (IOBase, bytes)):
             _content = configuration_assignment
         else:
             _json = self._serialize.body(configuration_assignment, "ConfigurationAssignment")
 
-        request = build_update_request(
+        _request = build_update_request(
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace
     def delete(self, configuration_assignment_name: str, **kwargs: Any) -> Optional[_models.ConfigurationAssignment]:
         """Unregister configuration for resource.
 
         Unregister configuration for resource.
 
         :param configuration_assignment_name: Unique configuration assignment name. Required.
         :type configuration_assignment_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or None or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment or None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -542,42 +515,37 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.ConfigurationAssignment]] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
         if response.status_code == 200:
             deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_configuration_assignments_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_configuration_assignments_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -47,15 +47,15 @@
     configuration_assignment_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}",
     )  # pylint: disable=line-too-long
@@ -93,15 +93,15 @@
     configuration_assignment_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}",
@@ -142,15 +142,15 @@
     configuration_assignment_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}",
     )  # pylint: disable=line-too-long
@@ -186,15 +186,15 @@
     configuration_assignment_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}",
     )  # pylint: disable=line-too-long
@@ -228,15 +228,15 @@
     configuration_assignment_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}",
@@ -273,15 +273,15 @@
     configuration_assignment_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}",
     )  # pylint: disable=line-too-long
@@ -316,15 +316,15 @@
     resource_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments",
     )  # pylint: disable=line-too-long
@@ -356,15 +356,15 @@
     resource_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments",
     )  # pylint: disable=line-too-long
@@ -432,15 +432,14 @@
         :type resource_parent_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -451,53 +450,48 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConfigurationAssignment] = kwargs.pop("cls", None)
 
-        request = build_get_parent_request(
+        _request = build_get_parent_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_parent_type=resource_parent_type,
             resource_parent_name=resource_parent_name,
             resource_type=resource_type,
             resource_name=resource_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get_parent.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get_parent.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     def create_or_update_parent(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_parent_type: str,
@@ -529,15 +523,14 @@
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
         :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def create_or_update_parent(
@@ -545,15 +538,15 @@
         resource_group_name: str,
         provider_name: str,
         resource_parent_type: str,
         resource_parent_name: str,
         resource_type: str,
         resource_name: str,
         configuration_assignment_name: str,
-        configuration_assignment: IO,
+        configuration_assignment: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
@@ -569,19 +562,18 @@
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
-        :type configuration_assignment: IO
+        :type configuration_assignment: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def create_or_update_parent(
@@ -589,15 +581,15 @@
         resource_group_name: str,
         provider_name: str,
         resource_parent_type: str,
         resource_parent_name: str,
         resource_type: str,
         resource_name: str,
         configuration_assignment_name: str,
-        configuration_assignment: Union[_models.ConfigurationAssignment, IO],
+        configuration_assignment: Union[_models.ConfigurationAssignment, IO[bytes]],
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param resource_group_name: Resource group name. Required.
@@ -611,20 +603,17 @@
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Is either a
-         ConfigurationAssignment type or a IO type. Required.
-        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ConfigurationAssignment type or a IO[bytes] type. Required.
+        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or
+         IO[bytes]
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -644,37 +633,36 @@
         _json = None
         _content = None
         if isinstance(configuration_assignment, (IOBase, bytes)):
             _content = configuration_assignment
         else:
             _json = self._serialize.body(configuration_assignment, "ConfigurationAssignment")
 
-        request = build_create_or_update_parent_request(
+        _request = build_create_or_update_parent_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_parent_type=resource_parent_type,
             resource_parent_name=resource_parent_name,
             resource_type=resource_type,
             resource_name=resource_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create_or_update_parent.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
@@ -687,18 +675,14 @@
             deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create_or_update_parent.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
-
     @distributed_trace
     def delete_parent(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_parent_type: str,
         resource_parent_name: str,
@@ -721,15 +705,14 @@
         :type resource_parent_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param configuration_assignment_name: Unique configuration assignment name. Required.
         :type configuration_assignment_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or None or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment or None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -740,55 +723,50 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.ConfigurationAssignment]] = kwargs.pop("cls", None)
 
-        request = build_delete_parent_request(
+        _request = build_delete_parent_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_parent_type=resource_parent_type,
             resource_parent_name=resource_parent_name,
             resource_type=resource_type,
             resource_name=resource_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.delete_parent.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
         if response.status_code == 200:
             deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    delete_parent.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace
     def get(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_type: str,
@@ -806,15 +784,14 @@
         :type provider_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -825,51 +802,46 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.ConfigurationAssignment] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_type=resource_type,
             resource_name=resource_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     def create_or_update(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_type: str,
@@ -895,29 +867,28 @@
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
         :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def create_or_update(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_type: str,
         resource_name: str,
         configuration_assignment_name: str,
-        configuration_assignment: IO,
+        configuration_assignment: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
@@ -929,33 +900,32 @@
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Required.
-        :type configuration_assignment: IO
+        :type configuration_assignment: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def create_or_update(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_type: str,
         resource_name: str,
         configuration_assignment_name: str,
-        configuration_assignment: Union[_models.ConfigurationAssignment, IO],
+        configuration_assignment: Union[_models.ConfigurationAssignment, IO[bytes]],
         **kwargs: Any
     ) -> _models.ConfigurationAssignment:
         """Create configuration assignment.
 
         Register configuration for resource.
 
         :param resource_group_name: Resource group name. Required.
@@ -965,20 +935,17 @@
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param configuration_assignment_name: Configuration assignment name. Required.
         :type configuration_assignment_name: str
         :param configuration_assignment: The configurationAssignment. Is either a
-         ConfigurationAssignment type or a IO type. Required.
-        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+         ConfigurationAssignment type or a IO[bytes] type. Required.
+        :type configuration_assignment: ~azure.mgmt.maintenance.models.ConfigurationAssignment or
+         IO[bytes]
         :return: ConfigurationAssignment or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -998,35 +965,34 @@
         _json = None
         _content = None
         if isinstance(configuration_assignment, (IOBase, bytes)):
             _content = configuration_assignment
         else:
             _json = self._serialize.body(configuration_assignment, "ConfigurationAssignment")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_type=resource_type,
             resource_name=resource_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
@@ -1039,18 +1005,14 @@
             deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
-
     @distributed_trace
     def delete(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_type: str,
         resource_name: str,
@@ -1067,15 +1029,14 @@
         :type provider_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
         :param configuration_assignment_name: Unique configuration assignment name. Required.
         :type configuration_assignment_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: ConfigurationAssignment or None or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.ConfigurationAssignment or None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -1086,53 +1047,48 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.ConfigurationAssignment]] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             provider_name=provider_name,
             resource_type=resource_type,
             resource_name=resource_name,
             configuration_assignment_name=configuration_assignment_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
         if response.status_code == 200:
             deserialized = self._deserialize("ConfigurationAssignment", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments/{configurationAssignmentName}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace
     def list_parent(
         self,
         resource_group_name: str,
         provider_name: str,
         resource_parent_type: str,
@@ -1153,15 +1109,14 @@
         :type resource_parent_type: str
         :param resource_parent_name: Resource parent identifier. Required.
         :type resource_parent_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ConfigurationAssignment or the result of
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.maintenance.models.ConfigurationAssignment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -1176,77 +1131,72 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_parent_request(
+                _request = build_list_parent_request(
                     resource_group_name=resource_group_name,
                     provider_name=provider_name,
                     resource_parent_type=resource_parent_type,
                     resource_parent_name=resource_parent_name,
                     resource_type=resource_type,
                     resource_name=resource_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_parent.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ListConfigurationAssignmentsResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_parent.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments"
-    }
-
     @distributed_trace
     def list(
         self, resource_group_name: str, provider_name: str, resource_type: str, resource_name: str, **kwargs: Any
     ) -> Iterable["_models.ConfigurationAssignment"]:
         """List configurationAssignments for resource.
 
         List configurationAssignments for resource.
@@ -1255,15 +1205,14 @@
         :type resource_group_name: str
         :param provider_name: Resource provider name. Required.
         :type provider_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ConfigurationAssignment or the result of
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.maintenance.models.ConfigurationAssignment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -1278,67 +1227,62 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     resource_group_name=resource_group_name,
                     provider_name=provider_name,
                     resource_type=resource_type,
                     resource_name=resource_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ListConfigurationAssignmentsResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/configurationAssignments"
-    }
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_configuration_assignments_within_subscription_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_configuration_assignments_within_subscription_operations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -36,15 +36,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/configurationAssignments"
     )  # pylint: disable=line-too-long
     path_format_arguments = {
@@ -58,15 +58,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class ConfigurationAssignmentsWithinSubscriptionOperations:
+class ConfigurationAssignmentsWithinSubscriptionOperations:  # pylint: disable=name-too-long
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.maintenance.MaintenanceManagementClient`'s
         :attr:`configuration_assignments_within_subscription` attribute.
@@ -83,15 +83,14 @@
 
     @distributed_trace
     def list(self, **kwargs: Any) -> Iterable["_models.ConfigurationAssignment"]:
         """Get configuration assignment within a subscription.
 
         Get configuration assignment within a subscription.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either ConfigurationAssignment or the result of
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.maintenance.models.ConfigurationAssignment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -106,61 +105,58 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ListConfigurationAssignmentsResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/configurationAssignments"}
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_maintenance_configurations_for_resource_group_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_operations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -32,142 +32,122 @@
 T = TypeVar("T")
 ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
 
 _SERIALIZER = Serializer()
 _SERIALIZER.client_side_validation = False
 
 
-def build_list_request(resource_group_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
+def build_list_request(**kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
-    _url = kwargs.pop(
-        "template_url",
-        "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Maintenance/maintenanceConfigurations",
-    )  # pylint: disable=line-too-long
-    path_format_arguments = {
-        "subscriptionId": _SERIALIZER.url("subscription_id", subscription_id, "str"),
-        "resourceGroupName": _SERIALIZER.url("resource_group_name", resource_group_name, "str"),
-    }
-
-    _url: str = _url.format(**path_format_arguments)  # type: ignore
+    _url = kwargs.pop("template_url", "/providers/Microsoft.Maintenance/operations")
 
     # Construct parameters
     _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class MaintenanceConfigurationsForResourceGroupOperations:
+class Operations:
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.maintenance.MaintenanceManagementClient`'s
-        :attr:`maintenance_configurations_for_resource_group` attribute.
+        :attr:`operations` attribute.
     """
 
     models = _models
 
     def __init__(self, *args, **kwargs):
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, resource_group_name: str, **kwargs: Any) -> Iterable["_models.MaintenanceConfiguration"]:
-        """Get Configuration records within a subscription and resource group.
+    def list(self, **kwargs: Any) -> Iterable["_models.Operation"]:
+        """List available operations.
 
-        Get Configuration records within a subscription and resource group.
+        List the available operations supported by the Microsoft.Maintenance resource provider.
 
-        :param resource_group_name: Resource Group Name. Required.
-        :type resource_group_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either MaintenanceConfiguration or the result of
-         cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.maintenance.models.MaintenanceConfiguration]
+        :return: An iterator like instance of either Operation or the result of cls(response)
+        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.maintenance.models.Operation]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.ListMaintenanceConfigurationsResult] = kwargs.pop("cls", None)
+        cls: ClsType[_models.OperationsListResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
-                    resource_group_name=resource_group_name,
-                    subscription_id=self._config.subscription_id,
+                _request = build_list_request(
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
-            deserialized = self._deserialize("ListMaintenanceConfigurationsResult", pipeline_response)
+            deserialized = self._deserialize("OperationsListResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Maintenance/maintenanceConfigurations"
-    }
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_maintenance_configurations_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_maintenance_configurations_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -37,15 +37,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_get_request(resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/maintenanceConfigurations/{resourceName}",
     )  # pylint: disable=line-too-long
@@ -68,15 +68,15 @@
 
 def build_create_or_update_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/maintenanceConfigurations/{resourceName}",
@@ -102,15 +102,15 @@
 
 def build_delete_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/maintenanceConfigurations/{resourceName}",
     )  # pylint: disable=line-too-long
@@ -133,15 +133,15 @@
 
 def build_update_request(
     resource_group_name: str, resource_name: str, subscription_id: str, **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     content_type: Optional[str] = kwargs.pop("content_type", _headers.pop("Content-Type", None))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/maintenanceConfigurations/{resourceName}",
@@ -165,15 +165,15 @@
     return HttpRequest(method="PATCH", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_list_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url", "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/maintenanceConfigurations"
     )  # pylint: disable=line-too-long
     path_format_arguments = {
@@ -216,15 +216,14 @@
 
         Get Configuration record.
 
         :param resource_group_name: Resource Group Name. Required.
         :type resource_group_name: str
         :param resource_name: Maintenance Configuration Name. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: MaintenanceConfiguration or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -235,48 +234,43 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MaintenanceConfiguration] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("MaintenanceConfiguration", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/maintenanceConfigurations/{resourceName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     def create_or_update(
         self,
         resource_group_name: str,
         resource_name: str,
         configuration: _models.MaintenanceConfiguration,
@@ -293,72 +287,66 @@
         :param resource_name: Maintenance Configuration Name. Required.
         :type resource_name: str
         :param configuration: The configuration. Required.
         :type configuration: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: MaintenanceConfiguration or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def create_or_update(
         self,
         resource_group_name: str,
         resource_name: str,
-        configuration: IO,
+        configuration: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.MaintenanceConfiguration:
         """Create or Update configuration record.
 
         Create or Update configuration record.
 
         :param resource_group_name: Resource Group Name. Required.
         :type resource_group_name: str
         :param resource_name: Maintenance Configuration Name. Required.
         :type resource_name: str
         :param configuration: The configuration. Required.
-        :type configuration: IO
+        :type configuration: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: MaintenanceConfiguration or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def create_or_update(
         self,
         resource_group_name: str,
         resource_name: str,
-        configuration: Union[_models.MaintenanceConfiguration, IO],
+        configuration: Union[_models.MaintenanceConfiguration, IO[bytes]],
         **kwargs: Any
     ) -> _models.MaintenanceConfiguration:
         """Create or Update configuration record.
 
         Create or Update configuration record.
 
         :param resource_group_name: Resource Group Name. Required.
         :type resource_group_name: str
         :param resource_name: Maintenance Configuration Name. Required.
         :type resource_name: str
-        :param configuration: The configuration. Is either a MaintenanceConfiguration type or a IO
-         type. Required.
-        :type configuration: ~azure.mgmt.maintenance.models.MaintenanceConfiguration or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+        :param configuration: The configuration. Is either a MaintenanceConfiguration type or a
+         IO[bytes] type. Required.
+        :type configuration: ~azure.mgmt.maintenance.models.MaintenanceConfiguration or IO[bytes]
         :return: MaintenanceConfiguration or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -378,32 +366,31 @@
         _json = None
         _content = None
         if isinstance(configuration, (IOBase, bytes)):
             _content = configuration
         else:
             _json = self._serialize.body(configuration, "MaintenanceConfiguration")
 
-        request = build_create_or_update_request(
+        _request = build_create_or_update_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.create_or_update.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 201]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
@@ -416,31 +403,26 @@
             deserialized = self._deserialize("MaintenanceConfiguration", pipeline_response)
 
         if cls:
             return cls(pipeline_response, deserialized, {})  # type: ignore
 
         return deserialized  # type: ignore
 
-    create_or_update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/maintenanceConfigurations/{resourceName}"
-    }
-
     @distributed_trace
     def delete(
         self, resource_group_name: str, resource_name: str, **kwargs: Any
     ) -> Optional[_models.MaintenanceConfiguration]:
         """Delete Configuration record.
 
         Delete Configuration record.
 
         :param resource_group_name: Resource Group Name. Required.
         :type resource_group_name: str
         :param resource_name: Maintenance Configuration Name. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: MaintenanceConfiguration or None or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.MaintenanceConfiguration or None
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -451,50 +433,45 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[Optional[_models.MaintenanceConfiguration]] = kwargs.pop("cls", None)
 
-        request = build_delete_request(
+        _request = build_delete_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.delete.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200, 204]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = None
         if response.status_code == 200:
             deserialized = self._deserialize("MaintenanceConfiguration", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    delete.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/maintenanceConfigurations/{resourceName}"
-    }
+        return deserialized  # type: ignore
 
     @overload
     def update(
         self,
         resource_group_name: str,
         resource_name: str,
         configuration: _models.MaintenanceConfiguration,
@@ -511,72 +488,66 @@
         :param resource_name: Maintenance Configuration Name. Required.
         :type resource_name: str
         :param configuration: The configuration. Required.
         :type configuration: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :keyword content_type: Body Parameter content-type. Content type parameter for JSON body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: MaintenanceConfiguration or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @overload
     def update(
         self,
         resource_group_name: str,
         resource_name: str,
-        configuration: IO,
+        configuration: IO[bytes],
         *,
         content_type: str = "application/json",
         **kwargs: Any
     ) -> _models.MaintenanceConfiguration:
         """Patch configuration record.
 
         Patch configuration record.
 
         :param resource_group_name: Resource Group Name. Required.
         :type resource_group_name: str
         :param resource_name: Maintenance Configuration Name. Required.
         :type resource_name: str
         :param configuration: The configuration. Required.
-        :type configuration: IO
+        :type configuration: IO[bytes]
         :keyword content_type: Body Parameter content-type. Content type parameter for binary body.
          Default value is "application/json".
         :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: MaintenanceConfiguration or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :raises ~azure.core.exceptions.HttpResponseError:
         """
 
     @distributed_trace
     def update(
         self,
         resource_group_name: str,
         resource_name: str,
-        configuration: Union[_models.MaintenanceConfiguration, IO],
+        configuration: Union[_models.MaintenanceConfiguration, IO[bytes]],
         **kwargs: Any
     ) -> _models.MaintenanceConfiguration:
         """Patch configuration record.
 
         Patch configuration record.
 
         :param resource_group_name: Resource Group Name. Required.
         :type resource_group_name: str
         :param resource_name: Maintenance Configuration Name. Required.
         :type resource_name: str
-        :param configuration: The configuration. Is either a MaintenanceConfiguration type or a IO
-         type. Required.
-        :type configuration: ~azure.mgmt.maintenance.models.MaintenanceConfiguration or IO
-        :keyword content_type: Body Parameter content-type. Known values are: 'application/json'.
-         Default value is None.
-        :paramtype content_type: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
+        :param configuration: The configuration. Is either a MaintenanceConfiguration type or a
+         IO[bytes] type. Required.
+        :type configuration: ~azure.mgmt.maintenance.models.MaintenanceConfiguration or IO[bytes]
         :return: MaintenanceConfiguration or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -596,59 +567,53 @@
         _json = None
         _content = None
         if isinstance(configuration, (IOBase, bytes)):
             _content = configuration
         else:
             _json = self._serialize.body(configuration, "MaintenanceConfiguration")
 
-        request = build_update_request(
+        _request = build_update_request(
             resource_group_name=resource_group_name,
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
             content_type=content_type,
             json=_json,
             content=_content,
-            template_url=self.update.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("MaintenanceConfiguration", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
-
-        return deserialized
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-    update.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/Microsoft.Maintenance/maintenanceConfigurations/{resourceName}"
-    }
+        return deserialized  # type: ignore
 
     @distributed_trace
     def list(self, **kwargs: Any) -> Iterable["_models.MaintenanceConfiguration"]:
         """Get Configuration records within a subscription.
 
         Get Configuration records within a subscription.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either MaintenanceConfiguration or the result of
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.maintenance.models.MaintenanceConfiguration]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -663,61 +628,58 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ListMaintenanceConfigurationsResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/maintenanceConfigurations"}
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/aio/operations/_configuration_assignments_within_subscription_operations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,157 +1,134 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
-from typing import Any, Callable, Dict, Iterable, Optional, TypeVar
+from typing import Any, AsyncIterable, Callable, Dict, Optional, TypeVar
 import urllib.parse
 
+from azure.core.async_paging import AsyncItemPaged, AsyncList
 from azure.core.exceptions import (
     ClientAuthenticationError,
     HttpResponseError,
     ResourceExistsError,
     ResourceNotFoundError,
     ResourceNotModifiedError,
     map_error,
 )
-from azure.core.paging import ItemPaged
 from azure.core.pipeline import PipelineResponse
-from azure.core.pipeline.transport import HttpResponse
+from azure.core.pipeline.transport import AsyncHttpResponse
 from azure.core.rest import HttpRequest
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.utils import case_insensitive_dict
 from azure.mgmt.core.exceptions import ARMErrorFormat
 
-from .. import models as _models
-from .._serialization import Serializer
-from .._vendor import _convert_request
+from ... import models as _models
+from ..._vendor import _convert_request
+from ...operations._configuration_assignments_within_subscription_operations import build_list_request
 
 T = TypeVar("T")
-ClsType = Optional[Callable[[PipelineResponse[HttpRequest, HttpResponse], T, Dict[str, Any]], Any]]
+ClsType = Optional[Callable[[PipelineResponse[HttpRequest, AsyncHttpResponse], T, Dict[str, Any]], Any]]
 
-_SERIALIZER = Serializer()
-_SERIALIZER.client_side_validation = False
 
-
-def build_list_request(**kwargs: Any) -> HttpRequest:
-    _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
-    _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
-
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
-    accept = _headers.pop("Accept", "application/json")
-
-    # Construct URL
-    _url = kwargs.pop("template_url", "/providers/Microsoft.Maintenance/operations")
-
-    # Construct parameters
-    _params["api-version"] = _SERIALIZER.query("api_version", api_version, "str")
-
-    # Construct headers
-    _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
-
-    return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
-
-
-class Operations:
+class ConfigurationAssignmentsWithinSubscriptionOperations:  # pylint: disable=name-too-long
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
-        :class:`~azure.mgmt.maintenance.MaintenanceManagementClient`'s
-        :attr:`operations` attribute.
+        :class:`~azure.mgmt.maintenance.aio.MaintenanceManagementClient`'s
+        :attr:`configuration_assignments_within_subscription` attribute.
     """
 
     models = _models
 
-    def __init__(self, *args, **kwargs):
+    def __init__(self, *args, **kwargs) -> None:
         input_args = list(args)
         self._client = input_args.pop(0) if input_args else kwargs.pop("client")
         self._config = input_args.pop(0) if input_args else kwargs.pop("config")
         self._serialize = input_args.pop(0) if input_args else kwargs.pop("serializer")
         self._deserialize = input_args.pop(0) if input_args else kwargs.pop("deserializer")
 
     @distributed_trace
-    def list(self, **kwargs: Any) -> Iterable["_models.Operation"]:
-        """List available operations.
+    def list(self, **kwargs: Any) -> AsyncIterable["_models.ConfigurationAssignment"]:
+        """Get configuration assignment within a subscription.
 
-        List the available operations supported by the Microsoft.Maintenance resource provider.
+        Get configuration assignment within a subscription.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
-        :return: An iterator like instance of either Operation or the result of cls(response)
-        :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.maintenance.models.Operation]
+        :return: An iterator like instance of either ConfigurationAssignment or the result of
+         cls(response)
+        :rtype:
+         ~azure.core.async_paging.AsyncItemPaged[~azure.mgmt.maintenance.models.ConfigurationAssignment]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
-        cls: ClsType[_models.OperationsListResult] = kwargs.pop("cls", None)
+        cls: ClsType[_models.ListConfigurationAssignmentsResult] = kwargs.pop("cls", None)
 
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
             409: ResourceExistsError,
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
+                    subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
-        def extract_data(pipeline_response):
-            deserialized = self._deserialize("OperationsListResult", pipeline_response)
+        async def extract_data(pipeline_response):
+            deserialized = self._deserialize("ListConfigurationAssignmentsResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
-            return None, iter(list_of_elem)
+            return None, AsyncList(list_of_elem)
 
-        def get_next(next_link=None):
-            request = prepare_request(next_link)
+        async def get_next(next_link=None):
+            _request = prepare_request(next_link)
 
             _stream = False
-            pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+            pipeline_response: PipelineResponse = await self._client._pipeline.run(  # pylint: disable=protected-access
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
-        return ItemPaged(get_next, extract_data)
-
-    list.metadata = {"url": "/providers/Microsoft.Maintenance/operations"}
+        return AsyncItemPaged(get_next, extract_data)
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_patch.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_public_maintenance_configurations_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_public_maintenance_configurations_operations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -36,15 +36,15 @@
 _SERIALIZER.client_side_validation = False
 
 
 def build_list_request(subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/publicMaintenanceConfigurations",
     )  # pylint: disable=line-too-long
@@ -63,15 +63,15 @@
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
 def build_get_request(resource_name: str, subscription_id: str, **kwargs: Any) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/publicMaintenanceConfigurations/{resourceName}",
     )  # pylint: disable=line-too-long
@@ -87,15 +87,15 @@
 
     # Construct headers
     _headers["Accept"] = _SERIALIZER.header("accept", accept, "str")
 
     return HttpRequest(method="GET", url=_url, params=_params, headers=_headers, **kwargs)
 
 
-class PublicMaintenanceConfigurationsOperations:
+class PublicMaintenanceConfigurationsOperations:  # pylint: disable=name-too-long
     """
     .. warning::
         **DO NOT** instantiate this class directly.
 
         Instead, you should access the following operations through
         :class:`~azure.mgmt.maintenance.MaintenanceManagementClient`'s
         :attr:`public_maintenance_configurations` attribute.
@@ -112,15 +112,14 @@
 
     @distributed_trace
     def list(self, **kwargs: Any) -> Iterable["_models.MaintenanceConfiguration"]:
         """Get Public Maintenance Configuration records.
 
         Get Public Maintenance Configuration records.
 
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either MaintenanceConfiguration or the result of
          cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.maintenance.models.MaintenanceConfiguration]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
@@ -135,80 +134,74 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ListMaintenanceConfigurationsResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/publicMaintenanceConfigurations"
-    }
-
     @distributed_trace
     def get(self, resource_name: str, **kwargs: Any) -> _models.MaintenanceConfiguration:
         """Get Public Maintenance Configuration record.
 
         Get Public Maintenance Configuration record.
 
         :param resource_name: Maintenance Configuration Name. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: MaintenanceConfiguration or the result of cls(response)
         :rtype: ~azure.mgmt.maintenance.models.MaintenanceConfiguration
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         error_map = {
             401: ClientAuthenticationError,
             404: ResourceNotFoundError,
@@ -219,40 +212,35 @@
 
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
         api_version: str = kwargs.pop("api_version", _params.pop("api-version", self._config.api_version))
         cls: ClsType[_models.MaintenanceConfiguration] = kwargs.pop("cls", None)
 
-        request = build_get_request(
+        _request = build_get_request(
             resource_name=resource_name,
             subscription_id=self._config.subscription_id,
             api_version=api_version,
-            template_url=self.get.metadata["url"],
             headers=_headers,
             params=_params,
         )
-        request = _convert_request(request)
-        request.url = self._client.format_url(request.url)
+        _request = _convert_request(_request)
+        _request.url = self._client.format_url(_request.url)
 
         _stream = False
         pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-            request, stream=_stream, **kwargs
+            _request, stream=_stream, **kwargs
         )
 
         response = pipeline_response.http_response
 
         if response.status_code not in [200]:
             map_error(status_code=response.status_code, response=response, error_map=error_map)
             error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
             raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
         deserialized = self._deserialize("MaintenanceConfiguration", pipeline_response)
 
         if cls:
-            return cls(pipeline_response, deserialized, {})
+            return cls(pipeline_response, deserialized, {})  # type: ignore
 
-        return deserialized
-
-    get.metadata = {
-        "url": "/subscriptions/{subscriptionId}/providers/Microsoft.Maintenance/publicMaintenanceConfigurations/{resourceName}"
-    }
+        return deserialized  # type: ignore
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure/mgmt/maintenance/operations/_updates_operations.py` & `azure-mgmt-maintenance-2.2.0b2/azure/mgmt/maintenance/operations/_updates_operations.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# pylint: disable=too-many-lines
+# pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See License.txt in the project root for license information.
 # Code generated by Microsoft (R) AutoRest Code Generator.
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
@@ -45,15 +45,15 @@
     resource_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/updates",
     )  # pylint: disable=line-too-long
@@ -85,15 +85,15 @@
     resource_name: str,
     subscription_id: str,
     **kwargs: Any
 ) -> HttpRequest:
     _headers = case_insensitive_dict(kwargs.pop("headers", {}) or {})
     _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
-    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-09-01-preview"))
+    api_version: str = kwargs.pop("api_version", _params.pop("api-version", "2023-10-01-preview"))
     accept = _headers.pop("Accept", "application/json")
 
     # Construct URL
     _url = kwargs.pop(
         "template_url",
         "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/updates",
     )  # pylint: disable=line-too-long
@@ -158,15 +158,14 @@
         :type resource_parent_type: str
         :param resource_parent_name: Resource parent identifier. Required.
         :type resource_parent_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Update or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.maintenance.models.Update]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -180,77 +179,72 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_parent_request(
+                _request = build_list_parent_request(
                     resource_group_name=resource_group_name,
                     provider_name=provider_name,
                     resource_parent_type=resource_parent_type,
                     resource_parent_name=resource_parent_name,
                     resource_type=resource_type,
                     resource_name=resource_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list_parent.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ListUpdatesResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
 
-    list_parent.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceParentType}/{resourceParentName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/updates"
-    }
-
     @distributed_trace
     def list(
         self, resource_group_name: str, provider_name: str, resource_type: str, resource_name: str, **kwargs: Any
     ) -> Iterable["_models.Update"]:
         """Get Updates to resource.
 
         Get updates to resources.
@@ -259,15 +253,14 @@
         :type resource_group_name: str
         :param provider_name: Resource provider name. Required.
         :type provider_name: str
         :param resource_type: Resource type. Required.
         :type resource_type: str
         :param resource_name: Resource identifier. Required.
         :type resource_name: str
-        :keyword callable cls: A custom type or function that will be passed the direct response
         :return: An iterator like instance of either Update or the result of cls(response)
         :rtype: ~azure.core.paging.ItemPaged[~azure.mgmt.maintenance.models.Update]
         :raises ~azure.core.exceptions.HttpResponseError:
         """
         _headers = kwargs.pop("headers", {}) or {}
         _params = case_insensitive_dict(kwargs.pop("params", {}) or {})
 
@@ -281,67 +274,62 @@
             304: ResourceNotModifiedError,
         }
         error_map.update(kwargs.pop("error_map", {}) or {})
 
         def prepare_request(next_link=None):
             if not next_link:
 
-                request = build_list_request(
+                _request = build_list_request(
                     resource_group_name=resource_group_name,
                     provider_name=provider_name,
                     resource_type=resource_type,
                     resource_name=resource_name,
                     subscription_id=self._config.subscription_id,
                     api_version=api_version,
-                    template_url=self.list.metadata["url"],
                     headers=_headers,
                     params=_params,
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
 
             else:
                 # make call to next link with the client's api-version
                 _parsed_next_link = urllib.parse.urlparse(next_link)
                 _next_request_params = case_insensitive_dict(
                     {
                         key: [urllib.parse.quote(v) for v in value]
                         for key, value in urllib.parse.parse_qs(_parsed_next_link.query).items()
                     }
                 )
                 _next_request_params["api-version"] = self._config.api_version
-                request = HttpRequest(
+                _request = HttpRequest(
                     "GET", urllib.parse.urljoin(next_link, _parsed_next_link.path), params=_next_request_params
                 )
-                request = _convert_request(request)
-                request.url = self._client.format_url(request.url)
-                request.method = "GET"
-            return request
+                _request = _convert_request(_request)
+                _request.url = self._client.format_url(_request.url)
+                _request.method = "GET"
+            return _request
 
         def extract_data(pipeline_response):
             deserialized = self._deserialize("ListUpdatesResult", pipeline_response)
             list_of_elem = deserialized.value
             if cls:
                 list_of_elem = cls(list_of_elem)  # type: ignore
             return None, iter(list_of_elem)
 
         def get_next(next_link=None):
-            request = prepare_request(next_link)
+            _request = prepare_request(next_link)
 
             _stream = False
             pipeline_response: PipelineResponse = self._client._pipeline.run(  # pylint: disable=protected-access
-                request, stream=_stream, **kwargs
+                _request, stream=_stream, **kwargs
             )
             response = pipeline_response.http_response
 
             if response.status_code not in [200]:
                 map_error(status_code=response.status_code, response=response, error_map=error_map)
                 error = self._deserialize.failsafe_deserialize(_models.MaintenanceError, pipeline_response)
                 raise HttpResponseError(response=response, model=error, error_format=ARMErrorFormat)
 
             return pipeline_response
 
         return ItemPaged(get_next, extract_data)
-
-    list.metadata = {
-        "url": "/subscriptions/{subscriptionId}/resourcegroups/{resourceGroupName}/providers/{providerName}/{resourceType}/{resourceName}/providers/Microsoft.Maintenance/updates"
-    }
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure_mgmt_maintenance.egg-info/PKG-INFO` & `azure-mgmt-maintenance-2.2.0b2/azure_mgmt_maintenance.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 Metadata-Version: 2.1
 Name: azure-mgmt-maintenance
-Version: 2.2.0b1
+Version: 2.2.0b2
 Summary: Microsoft Azure Maintenance Management Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: azpysdkhelp@microsoft.com
 License: MIT License
 Keywords: azure,azure sdk
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: isodate<1.0.0,>=0.6.1
-Requires-Dist: azure-common~=1.1
-Requires-Dist: azure-mgmt-core<2.0.0,>=1.3.2
-Requires-Dist: typing-extensions>=4.3.0; python_version < "3.8.0"
 
 # Microsoft Azure SDK for Python
 
 This is the Microsoft Azure Maintenance Management Client Library.
-This package has been tested with Python 3.7+.
+This package has been tested with Python 3.8+.
 For a more complete view of Azure libraries, see the [azure sdk python release](https://aka.ms/azsdk/python/all).
 
 ## _Disclaimer_
 
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
 ## Getting started
 
 ### Prerequisites
 
-- Python 3.7+ is required to use this package.
+- Python 3.8+ is required to use this package.
 - [Azure subscription](https://azure.microsoft.com/free/)
 
 ### Install the package
 
 ```bash
 pip install azure-mgmt-maintenance
 pip install azure-identity
@@ -86,14 +82,20 @@
 If you encounter any bugs or have suggestions, please file an issue in the
 [Issues](https://github.com/Azure/azure-sdk-for-python/issues)
 section of the project. 
 
 
 # Release History
 
+## 2.2.0b2 (2024-05-20)
+
+### Features Added
+
+  - Added operation group ScheduledEventOperations
+
 ## 2.2.0b1 (2023-10-22)
 
 ### Features Added
 
   - Added operation ApplyUpdatesOperations.create_or_update_or_cancel
 
 ## 2.1.0 (2023-08-18)
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/azure_mgmt_maintenance.egg-info/SOURCES.txt` & `azure-mgmt-maintenance-2.2.0b2/azure_mgmt_maintenance.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 azure/mgmt/maintenance/aio/operations/_configuration_assignments_operations.py
 azure/mgmt/maintenance/aio/operations/_configuration_assignments_within_subscription_operations.py
 azure/mgmt/maintenance/aio/operations/_maintenance_configurations_for_resource_group_operations.py
 azure/mgmt/maintenance/aio/operations/_maintenance_configurations_operations.py
 azure/mgmt/maintenance/aio/operations/_operations.py
 azure/mgmt/maintenance/aio/operations/_patch.py
 azure/mgmt/maintenance/aio/operations/_public_maintenance_configurations_operations.py
+azure/mgmt/maintenance/aio/operations/_scheduled_event_operations.py
 azure/mgmt/maintenance/aio/operations/_updates_operations.py
 azure/mgmt/maintenance/models/__init__.py
 azure/mgmt/maintenance/models/_maintenance_management_client_enums.py
 azure/mgmt/maintenance/models/_models_py3.py
 azure/mgmt/maintenance/models/_patch.py
 azure/mgmt/maintenance/operations/__init__.py
 azure/mgmt/maintenance/operations/_apply_update_for_resource_group_operations.py
@@ -43,14 +44,15 @@
 azure/mgmt/maintenance/operations/_configuration_assignments_operations.py
 azure/mgmt/maintenance/operations/_configuration_assignments_within_subscription_operations.py
 azure/mgmt/maintenance/operations/_maintenance_configurations_for_resource_group_operations.py
 azure/mgmt/maintenance/operations/_maintenance_configurations_operations.py
 azure/mgmt/maintenance/operations/_operations.py
 azure/mgmt/maintenance/operations/_patch.py
 azure/mgmt/maintenance/operations/_public_maintenance_configurations_operations.py
+azure/mgmt/maintenance/operations/_scheduled_event_operations.py
 azure/mgmt/maintenance/operations/_updates_operations.py
 azure_mgmt_maintenance.egg-info/PKG-INFO
 azure_mgmt_maintenance.egg-info/SOURCES.txt
 azure_mgmt_maintenance.egg-info/dependency_links.txt
 azure_mgmt_maintenance.egg-info/not-zip-safe
 azure_mgmt_maintenance.egg-info/requires.txt
 azure_mgmt_maintenance.egg-info/top_level.txt
```

### Comparing `azure-mgmt-maintenance-2.2.0b1/setup.py` & `azure-mgmt-maintenance-2.2.0b2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -49,19 +49,19 @@
     url="https://github.com/Azure/azure-sdk-for-python",
     keywords="azure, azure sdk",  # update with search keywords relevant to the azure service / product
     classifiers=[
         "Development Status :: 4 - Beta",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
     ],
     zip_safe=False,
     packages=find_packages(
         exclude=[
             "tests",
             # Exclude packages that will be covered by PEP420 or nspkg
@@ -70,14 +70,13 @@
         ]
     ),
     include_package_data=True,
     package_data={
         "pytyped": ["py.typed"],
     },
     install_requires=[
-        "isodate<1.0.0,>=0.6.1",
-        "azure-common~=1.1",
-        "azure-mgmt-core>=1.3.2,<2.0.0",
-        "typing-extensions>=4.3.0; python_version<'3.8.0'",
+        "isodate>=0.6.1",
+        "azure-common>=1.1",
+        "azure-mgmt-core>=1.3.2",
     ],
-    python_requires=">=3.7",
+    python_requires=">=3.8",
 )
```

