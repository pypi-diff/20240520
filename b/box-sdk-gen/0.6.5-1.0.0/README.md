# Comparing `tmp/box_sdk_gen-0.6.5.tar.gz` & `tmp/box_sdk_gen-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "box_sdk_gen-0.6.5.tar", last modified: Thu May  9 16:16:13 2024, max compression
+gzip compressed data, was "box_sdk_gen-1.0.0.tar", last modified: Mon May 20 13:42:11 2024, max compression
```

## Comparing `box_sdk_gen-0.6.5.tar` & `box_sdk_gen-1.0.0.tar`

### file list

```diff
@@ -1,112 +1,315 @@
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-09 16:16:13.633000 box_sdk_gen-0.6.5/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     9574 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/LICENSE
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8497 2024-05-09 16:16:13.632000 box_sdk_gen-0.6.5/PKG-INFO
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6560 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/README.md
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-09 16:16:13.610000 box_sdk_gen-0.6.5/box_sdk_gen/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      250 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/__init__.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-09 16:16:13.613000 box_sdk_gen-0.6.5/box_sdk_gen/box/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      251 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/box/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    10021 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/box/ccg_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5690 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/box/developer_token_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3833 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/box/errors.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    18147 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/box/jwt_auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    10483 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/box/oauth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2015 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/box/token_storage.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    16977 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/client.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-09 16:16:13.613000 box_sdk_gen-0.6.5/box_sdk_gen/internal/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       89 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/internal/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5352 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/internal/base_object.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7893 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/internal/utils.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-09 16:16:13.628000 box_sdk_gen-0.6.5/box_sdk_gen/managers/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3694 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7596 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/ai.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    18009 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/authorization.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5782 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/avatars.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    20524 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/chunked_uploads.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    26186 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/classifications.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8003 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/collaboration_allowlist_entries.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8119 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/collaboration_allowlist_exempt_targets.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6383 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/collections.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    13386 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/comments.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6476 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/device_pinners.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4370 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/downloads.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5864 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/email_aliases.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    15816 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/events.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    11377 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/file_classifications.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    14891 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/file_metadata.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    15292 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/file_requests.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5785 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/file_version_legal_holds.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6443 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/file_version_retentions.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    15125 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/file_versions.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6779 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/file_watermarks.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    26447 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/files.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    11915 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/folder_classifications.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7162 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/folder_locks.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    15868 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/folder_metadata.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7183 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/folder_watermarks.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    36868 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/folders.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    18131 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/groups.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    10362 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/integration_mappings.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6503 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/invites.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    12417 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/legal_hold_policies.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    17898 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/legal_hold_policy_assignments.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    11646 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/list_collaborations.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    16444 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/memberships.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    12347 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/metadata_cascade_policies.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    24198 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/metadata_templates.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3675 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/recent_items.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    19401 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/retention_policies.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    16875 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/retention_policy_assignments.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    25713 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/search.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4154 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/session_termination.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    21070 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/shared_links_files.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    21205 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/shared_links_folders.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    19813 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/shared_links_web_links.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     6561 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/shield_information_barrier_reports.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    10658 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/shield_information_barrier_segment_members.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    12372 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/shield_information_barrier_segment_restrictions.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    10513 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/shield_information_barrier_segments.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7863 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/shield_information_barriers.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    14228 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/sign_requests.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4203 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/sign_templates.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    15571 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/skills.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     4930 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/storage_policies.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    12643 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/storage_policy_assignments.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    10563 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/task_assignments.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    11825 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/tasks.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8084 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/terms_of_service_user_statuses.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8106 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/terms_of_services.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5922 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/transfer.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8714 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/trashed_files.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     9580 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/trashed_folders.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     5921 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/trashed_items.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     7611 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/trashed_web_links.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    15382 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/uploads.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    16451 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/user_collaborations.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    29903 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/users.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    11821 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/web_links.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    14664 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/webhooks.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8623 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/workflows.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    10714 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/managers/zip_downloads.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-09 16:16:13.629000 box_sdk_gen-0.6.5/box_sdk_gen/networking/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      226 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/networking/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1090 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/networking/auth.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      773 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/networking/base_urls.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)    10114 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/networking/fetch.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     1586 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/networking/network.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       22 2024-05-09 16:16:02.000000 box_sdk_gen-0.6.5/box_sdk_gen/networking/version.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)   549900 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/schemas.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-09 16:16:13.629000 box_sdk_gen-0.6.5/box_sdk_gen/serialization/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       45 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/serialization/__init__.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-09 16:16:13.630000 box_sdk_gen-0.6.5/box_sdk_gen/serialization/json/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      112 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/serialization/json/__init__.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      337 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/serialization/json/json_data.py
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      712 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/box_sdk_gen/serialization/json/serializer.py
-drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-09 16:16:13.630000 box_sdk_gen-0.6.5/box_sdk_gen.egg-info/
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     8497 2024-05-09 16:16:13.000000 box_sdk_gen-0.6.5/box_sdk_gen.egg-info/PKG-INFO
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     3848 2024-05-09 16:16:13.000000 box_sdk_gen-0.6.5/box_sdk_gen.egg-info/SOURCES.txt
--rw-r--r--   0 container_jenkins  (3000) docker     (551)        1 2024-05-09 16:16:13.000000 box_sdk_gen-0.6.5/box_sdk_gen.egg-info/dependency_links.txt
--rw-r--r--   0 container_jenkins  (3000) docker     (551)      144 2024-05-09 16:16:13.000000 box_sdk_gen-0.6.5/box_sdk_gen.egg-info/requires.txt
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       12 2024-05-09 16:16:13.000000 box_sdk_gen-0.6.5/box_sdk_gen.egg-info/top_level.txt
--rw-r--r--   0 container_jenkins  (3000) docker     (551)       38 2024-05-09 16:16:13.633000 box_sdk_gen-0.6.5/setup.cfg
--rw-r--r--   0 container_jenkins  (3000) docker     (551)     2671 2024-05-09 16:04:31.000000 box_sdk_gen-0.6.5/setup.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-20 13:42:11.791052 box_sdk_gen-1.0.0/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9574 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/LICENSE
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9492 2024-05-20 13:42:11.790052 box_sdk_gen-1.0.0/PKG-INFO
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7555 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/README.md
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-20 13:42:11.687052 box_sdk_gen-1.0.0/box_sdk_gen/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      250 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/__init__.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-20 13:42:11.690052 box_sdk_gen-1.0.0/box_sdk_gen/box/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      251 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/box/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10135 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/box/ccg_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5784 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/box/developer_token_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3833 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/box/errors.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    18241 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/box/jwt_auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10577 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/box/oauth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2028 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/box/token_storage.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    16977 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/client.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-20 13:42:11.690052 box_sdk_gen-1.0.0/box_sdk_gen/internal/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       89 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/internal/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5352 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/internal/base_object.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7893 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/internal/utils.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-20 13:42:11.705052 box_sdk_gen-1.0.0/box_sdk_gen/managers/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3694 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7648 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/ai.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    18254 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/authorization.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5819 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/avatars.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    20700 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/chunked_uploads.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    26239 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/classifications.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8112 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/collaboration_allowlist_entries.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8243 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/collaboration_allowlist_exempt_targets.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6422 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/collections.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    13441 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/comments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6530 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/device_pinners.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4387 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/downloads.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5915 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/email_aliases.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    15861 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/events.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11421 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/file_classifications.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    14948 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/file_metadata.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    15388 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/file_requests.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5914 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/file_version_legal_holds.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6570 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/file_version_retentions.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    15190 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/file_versions.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6814 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/file_watermarks.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    26727 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/files.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11959 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/folder_classifications.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7212 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/folder_locks.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    15925 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/folder_metadata.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7218 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/folder_watermarks.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    36923 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/folders.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    18182 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/groups.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10735 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/integration_mappings.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6531 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/invites.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12548 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/legal_hold_policies.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    14157 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/legal_hold_policy_assignments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11690 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/list_collaborations.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    16546 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/memberships.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12563 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/metadata_cascade_policies.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    24428 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/metadata_templates.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3705 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/recent_items.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    19550 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/retention_policies.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    14757 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/retention_policy_assignments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    25856 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/search.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4321 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/session_termination.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    21113 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/shared_links_files.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    21280 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/shared_links_folders.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    19855 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/shared_links_web_links.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6760 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/shield_information_barrier_reports.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10841 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/shield_information_barrier_segment_members.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12555 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/shield_information_barrier_segment_restrictions.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10676 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/shield_information_barrier_segments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7963 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/shield_information_barriers.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    14808 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/sign_requests.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4253 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/sign_templates.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    15704 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/skills.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4983 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/storage_policies.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12847 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/storage_policy_assignments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10629 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/task_assignments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12106 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/tasks.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8178 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/terms_of_service_user_statuses.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8230 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/terms_of_services.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5951 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/transfer.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8849 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/trashed_files.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9640 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/trashed_folders.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5974 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/trashed_items.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7675 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/trashed_web_links.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    15439 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/uploads.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    16494 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/user_collaborations.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    30207 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/users.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11859 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/web_links.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    14714 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/webhooks.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8662 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/workflows.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10785 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/managers/zip_downloads.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-20 13:42:11.706052 box_sdk_gen-1.0.0/box_sdk_gen/networking/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      226 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/networking/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1103 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/networking/auth.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      765 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/networking/base_urls.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10114 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/networking/fetch.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1586 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/networking/network.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       22 2024-05-20 13:42:01.000000 box_sdk_gen-1.0.0/box_sdk_gen/networking/version.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-20 13:42:11.787052 box_sdk_gen-1.0.0/box_sdk_gen/schemas/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    11056 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2484 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/access_token.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1682 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/ai_ask.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      874 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/ai_response.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2830 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/ai_text_gen.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3678 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/classification.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9802 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/classification_template.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3121 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/client_error.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8594 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/collaboration.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1528 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/collaboration_allowlist_entries.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2791 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/collaboration_allowlist_entry.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2628 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/collaboration_allowlist_exempt_target.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1665 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/collaboration_allowlist_exempt_targets.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3008 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/collaborations.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2181 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/collaborator_variable.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1527 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/collection.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2972 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/collections.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2455 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/comment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      736 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/comment_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2466 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/comment_full.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2953 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/comments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1676 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/completion_rule_variable.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2786 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/conflict_error.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1113 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/device_pinner.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2227 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/device_pinners.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1144 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/email_alias.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      743 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/email_aliases.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      762 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/enterprise_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9798 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/event.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2005 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/event_source.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1126 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/events.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12544 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/file.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1321 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/file_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2025 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/file_conflict.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    25710 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/file_full.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2191 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/file_mini.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1214 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/file_or_folder_scope.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5281 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/file_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4247 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/file_request_copy_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3212 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/file_request_update_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2928 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/file_version.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      759 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/file_version_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3256 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/file_version_full.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1975 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/file_version_legal_hold.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1479 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/file_version_legal_holds.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1180 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/file_version_mini.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1968 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/file_version_retention.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1477 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/file_version_retentions.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3003 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/file_versions.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      712 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/files.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1400 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/files_on_hold.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1408 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/files_under_retention.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    14313 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/folder.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1359 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/folder_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    13960 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/folder_full.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2268 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/folder_lock.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1162 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/folder_locks.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1521 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/folder_mini.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        0 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/generic_source.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1593 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/group.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      666 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/group_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5543 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/group_full.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1850 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/group_membership.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3034 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/group_memberships.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1150 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/group_mini.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2929 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/groups.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4188 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/integration_mapping.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1096 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/integration_mapping_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      847 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/integration_mapping_box_item_slack.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2488 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/integration_mapping_mini.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1651 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/integration_mapping_partner_item_slack.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      855 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/integration_mapping_slack_create_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      762 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/integration_mapping_slack_options.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1210 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/integration_mappings.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2651 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/invite.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3119 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/items.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5016 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/keyword_skill_card.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1449 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/legal_hold_policies.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5436 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/legal_hold_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2246 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/legal_hold_policy_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      905 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/legal_hold_policy_assignment_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1517 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/legal_hold_policy_assignments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      809 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/legal_hold_policy_mini.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1493 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/metadata.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1992 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/metadata_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1485 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/metadata_cascade_policies.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4630 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/metadata_cascade_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1014 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/metadata_field_filter_date_range.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      954 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/metadata_field_filter_float_range.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3098 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/metadata_filter.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3126 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/metadata_full.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5532 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/metadata_query.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1931 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/metadata_query_index.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1490 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/metadata_query_results.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7253 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/metadata_template.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1451 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/metadata_templates.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      763 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/metadatas.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      666 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/o_auth_2_error.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1093 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/outcome.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      995 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/post_o_auth_2_revoke.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6885 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/post_o_auth_2_token.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1344 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/post_o_auth_2_token_refresh_access_token.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1627 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/realtime_server.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      770 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/realtime_servers.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1939 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/recent_item.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1415 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/recent_items.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1230 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/retention_policies.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8251 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/retention_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4548 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/retention_policy_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      934 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/retention_policy_assignment_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1254 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/retention_policy_assignments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      812 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/retention_policy_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2392 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/retention_policy_mini.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1463 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/role_variable.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1280 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/search_result_with_shared_link.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2233 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/search_results.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2406 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/search_results_with_shared_links.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      432 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/session_termination_message.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3231 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/shield_information_barrier.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      911 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/shield_information_barrier_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      497 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/shield_information_barrier_reference.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2668 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/shield_information_barrier_report.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      970 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/shield_information_barrier_report_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      725 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/shield_information_barrier_report_details.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1304 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/shield_information_barrier_reports.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2548 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/shield_information_barrier_segment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4037 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/shield_information_barrier_segment_member.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1094 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/shield_information_barrier_segment_member_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1157 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/shield_information_barrier_segment_member_mini.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1347 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/shield_information_barrier_segment_members.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3619 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/shield_information_barrier_segment_restriction.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1124 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/shield_information_barrier_segment_restriction_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4213 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/shield_information_barrier_segment_restriction_mini.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1384 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/shield_information_barrier_segment_restrictions.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1309 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/shield_information_barrier_segments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1255 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/shield_information_barriers.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10220 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/sign_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5468 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/sign_request_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6826 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/sign_request_create_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5444 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/sign_request_create_signer.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1192 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/sign_request_prefill_tag.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     8179 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/sign_request_signer.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2759 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/sign_request_signer_input.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1173 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/sign_requests.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10654 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/sign_template.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1423 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/sign_templates.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3822 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/skill_cards_metadata.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9282 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/skill_invocation.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5794 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/status_skill_card.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1435 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/storage_policies.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      894 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/storage_policy.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1704 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/storage_policy_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1495 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/storage_policy_assignments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      776 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/storage_policy_mini.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3216 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/task.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2958 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/task_assignment.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      782 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/task_assignments.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      872 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/tasks.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2275 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/template_signer.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5767 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/template_signer_input.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3353 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/terms_of_service.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      797 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/terms_of_service_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1926 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/terms_of_service_user_status.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      833 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/terms_of_service_user_statuses.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      774 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/terms_of_services.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6951 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/timeline_skill_card.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1050 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/tracking_code.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6380 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/transcript_skill_card.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7562 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/trash_file.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6330 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/trash_file_restored.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     7382 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/trash_folder.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6413 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/trash_folder_restored.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     6125 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/trash_web_link.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4859 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/trash_web_link_restored.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1383 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/upload_part.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      940 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/upload_part_mini.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3007 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/upload_parts.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3752 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/upload_session.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      756 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/upload_url.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      307 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/uploaded_part.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     5242 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/user.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1190 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/user_avatar.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      652 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/user_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1105 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/user_collaborations.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9397 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/user_full.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      966 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/user_integration_mappings.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      951 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/user_mini.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2917 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/users.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      943 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/watermark.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    10849 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/web_link.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      990 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/web_link_base.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1340 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/web_link_mini.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3817 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/webhook.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     3538 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/webhook_invocation.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1675 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/webhook_mini.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1412 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/webhooks.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9936 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/workflow.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2411 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/workflow_full.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1337 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/workflow_mini.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1401 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/workflows.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     4425 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/zip_download.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     1634 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/zip_download_request.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2197 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/schemas/zip_download_status.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-20 13:42:11.787052 box_sdk_gen-1.0.0/box_sdk_gen/serialization/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       45 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/serialization/__init__.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-20 13:42:11.788052 box_sdk_gen-1.0.0/box_sdk_gen/serialization/json/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      112 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/serialization/json/__init__.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      337 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/serialization/json/json_data.py
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      712 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/box_sdk_gen/serialization/json/serializer.py
+drwxr-xr-x   0 container_jenkins  (3000) docker     (551)        0 2024-05-20 13:42:11.788052 box_sdk_gen-1.0.0/box_sdk_gen.egg-info/
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     9492 2024-05-20 13:42:11.000000 box_sdk_gen-1.0.0/box_sdk_gen.egg-info/PKG-INFO
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)    12490 2024-05-20 13:42:11.000000 box_sdk_gen-1.0.0/box_sdk_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)        1 2024-05-20 13:42:11.000000 box_sdk_gen-1.0.0/box_sdk_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)      144 2024-05-20 13:42:11.000000 box_sdk_gen-1.0.0/box_sdk_gen.egg-info/requires.txt
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       12 2024-05-20 13:42:11.000000 box_sdk_gen-1.0.0/box_sdk_gen.egg-info/top_level.txt
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)       38 2024-05-20 13:42:11.791052 box_sdk_gen-1.0.0/setup.cfg
+-rw-r--r--   0 container_jenkins  (3000) docker     (551)     2671 2024-05-20 13:27:29.000000 box_sdk_gen-1.0.0/setup.py
```

### Comparing `box_sdk_gen-0.6.5/LICENSE` & `box_sdk_gen-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `box_sdk_gen-0.6.5/PKG-INFO` & `box_sdk_gen-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: box-sdk-gen
-Version: 0.6.5
+Version: 1.0.0
 Summary: [Box Platform](https://box.dev) provides functionality to provide access to content stored within [Box](https://box.com). It provides endpoints for basic manipulation of files and folders, management of users within an enterprise, as well as more complex topics such as legal holds and retention policies.
 Home-page: https://github.com/box/box-python-sdk-gen.git
 Author: Box
 Author-email: oss@box.com
 License: Apache-2.0, http://www.apache.org/licenses/LICENSE-2.0
 Keywords: box,sdk,api,rest,boxsdk
 Classifier: Development Status :: 4 - Beta
@@ -41,15 +41,22 @@
 
 <p align="center">
   <img src="https://github.com/box/sdks/blob/master/images/box-dev-logo.png" alt= “box-dev-logo” width="30%" height="50%">
 </p>
 
 # Box Python SDK GENERATED
 
-We are excited to introduce the latest generation (currently in Beta) of Box Python SDK, designed to elevate the developer experience and streamline your integration with the Box Content Cloud.
+[![Project Status](http://opensource.box.com/badges/active.svg)](http://opensource.box.com/badges)
+![build](https://github.com/box/box-python-sdk-gen/actions/workflows/build.yml/badge.svg)
+[![PyPI version](https://badge.fury.io/py/box-sdk-gen.svg)](https://badge.fury.io/py/box-sdk-gen)
+[![image](https://img.shields.io/pypi/dm/box-sdk-gen.svg)](https://pypi.python.org/pypi/box-sdk-gen)
+![Platform](https://img.shields.io/badge/python-3.8+-blue)
+[![Coverage](https://coveralls.io/repos/github/box/box-python-sdk-gen/badge.svg?branch=main)](https://coveralls.io/github/box/box-python-sdk-gen?branch=main)
+
+We are excited to introduce the stable release of the latest generation of Box Python SDK, designed to elevate the developer experience and streamline your integration with the Box Content Cloud.
 
 With this SDK, you’ll have access to:
 
 1. Full API Support: The new generation of Box SDKs empowers developers with complete coverage of the Box API ecosystem. You can now access all the latest features and functionalities offered by Box, allowing you to build even more sophisticated and feature-rich applications.
 2. Rapid API Updates: Say goodbye to waiting for new Box APIs to be incorporated into the SDK. With our new auto-generation development approach, we can now add new Box APIs to the SDK at a much faster pace (in a matter of days). This means you can leverage the most up-to-date features in your applications without delay.
 3. Embedded Documentation: We understand that easy access to information is crucial for developers. With our new approach, we have included comprehensive documentation for all objects and parameters directly in the source code of the SDK. This means you no longer need to look up this information on the developer portal, saving you time and streamlining your development process.
 4. Enhanced Convenience Methods: Our commitment to enhancing your development experience continues with the introduction of convenience methods. These methods cover various aspects such as chunk uploads, classification, and much more.
@@ -60,14 +67,16 @@
 # Table of contents
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
 - [Installing](#installing)
 - [Getting Started](#getting-started)
+- [Documentation](#documentation)
+- [Upgrades](#upgrades)
 - [Integration Tests](#integration-tests)
   - [Running integration tests locally](#running-integration-tests-locally)
     - [Create Custom Application](#create-custom-application)
     - [Export configuration](#export-configuration)
     - [Running tests](#running-tests)
 - [Questions, Bugs, and Feature Requests?](#questions-bugs-and-feature-requests)
 - [Copyright and License](#copyright-and-license)
@@ -76,15 +85,15 @@
 
 # Installing
 
 ```console
 pip install box-sdk-gen
 ```
 
-This is autogenerated Box SDK Beta version.
+This is autogenerated Box SDK version.
 Supported Python versions are Python 3.8 and above.
 
 To install also extra dependencies required for JWT authentication, use command:
 
 ```console
 pip install box-sdk-gen[jwt]
 ```
@@ -109,14 +118,22 @@
     for item in client.folders.get_folder_items('0').entries:
         print(item.name)
 
 if __name__ == '__main__':
     main('INSERT YOUR DEVELOPER TOKEN HERE')
 ```
 
+# Documentation
+
+Browse the [docs](docs/README.md) or see [API Reference](https://developer.box.com/reference/) for more information.
+
+# Upgrades
+
+Upgrading from our legacy SDKs to the new generation SDKs is a straightforward process. See our [migration guide](migration-guide.md) and [changelog](CHANGELOG.md) for more information.
+
 # Integration Tests
 
 ## Running integration tests locally
 
 ### Create Custom Application
 
 To run integration tests locally you will need a `Custom App` created in the [Box Developer
```

### Comparing `box_sdk_gen-0.6.5/README.md` & `box_sdk_gen-1.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 <p align="center">
   <img src="https://github.com/box/sdks/blob/master/images/box-dev-logo.png" alt= “box-dev-logo” width="30%" height="50%">
 </p>
 
 # Box Python SDK GENERATED
 
-We are excited to introduce the latest generation (currently in Beta) of Box Python SDK, designed to elevate the developer experience and streamline your integration with the Box Content Cloud.
+[![Project Status](http://opensource.box.com/badges/active.svg)](http://opensource.box.com/badges)
+![build](https://github.com/box/box-python-sdk-gen/actions/workflows/build.yml/badge.svg)
+[![PyPI version](https://badge.fury.io/py/box-sdk-gen.svg)](https://badge.fury.io/py/box-sdk-gen)
+[![image](https://img.shields.io/pypi/dm/box-sdk-gen.svg)](https://pypi.python.org/pypi/box-sdk-gen)
+![Platform](https://img.shields.io/badge/python-3.8+-blue)
+[![Coverage](https://coveralls.io/repos/github/box/box-python-sdk-gen/badge.svg?branch=main)](https://coveralls.io/github/box/box-python-sdk-gen?branch=main)
+
+We are excited to introduce the stable release of the latest generation of Box Python SDK, designed to elevate the developer experience and streamline your integration with the Box Content Cloud.
 
 With this SDK, you’ll have access to:
 
 1. Full API Support: The new generation of Box SDKs empowers developers with complete coverage of the Box API ecosystem. You can now access all the latest features and functionalities offered by Box, allowing you to build even more sophisticated and feature-rich applications.
 2. Rapid API Updates: Say goodbye to waiting for new Box APIs to be incorporated into the SDK. With our new auto-generation development approach, we can now add new Box APIs to the SDK at a much faster pace (in a matter of days). This means you can leverage the most up-to-date features in your applications without delay.
 3. Embedded Documentation: We understand that easy access to information is crucial for developers. With our new approach, we have included comprehensive documentation for all objects and parameters directly in the source code of the SDK. This means you no longer need to look up this information on the developer portal, saving you time and streamlining your development process.
 4. Enhanced Convenience Methods: Our commitment to enhancing your development experience continues with the introduction of convenience methods. These methods cover various aspects such as chunk uploads, classification, and much more.
@@ -19,14 +26,16 @@
 # Table of contents
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
 - [Installing](#installing)
 - [Getting Started](#getting-started)
+- [Documentation](#documentation)
+- [Upgrades](#upgrades)
 - [Integration Tests](#integration-tests)
   - [Running integration tests locally](#running-integration-tests-locally)
     - [Create Custom Application](#create-custom-application)
     - [Export configuration](#export-configuration)
     - [Running tests](#running-tests)
 - [Questions, Bugs, and Feature Requests?](#questions-bugs-and-feature-requests)
 - [Copyright and License](#copyright-and-license)
@@ -35,15 +44,15 @@
 
 # Installing
 
 ```console
 pip install box-sdk-gen
 ```
 
-This is autogenerated Box SDK Beta version.
+This is autogenerated Box SDK version.
 Supported Python versions are Python 3.8 and above.
 
 To install also extra dependencies required for JWT authentication, use command:
 
 ```console
 pip install box-sdk-gen[jwt]
 ```
@@ -68,14 +77,22 @@
     for item in client.folders.get_folder_items('0').entries:
         print(item.name)
 
 if __name__ == '__main__':
     main('INSERT YOUR DEVELOPER TOKEN HERE')
 ```
 
+# Documentation
+
+Browse the [docs](docs/README.md) or see [API Reference](https://developer.box.com/reference/) for more information.
+
+# Upgrades
+
+Upgrading from our legacy SDKs to the new generation SDKs is a straightforward process. See our [migration guide](migration-guide.md) and [changelog](CHANGELOG.md) for more information.
+
 # Integration Tests
 
 ## Running integration tests locally
 
 ### Create Custom Application
 
 To run integration tests locally you will need a `Custom App` created in the [Box Developer
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/box/ccg_auth.py` & `box_sdk_gen-1.0.0/box_sdk_gen/box/ccg_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Optional
 
 from typing import List
 
-from box_sdk_gen.schemas import PostOAuth2TokenGrantTypeField
+from box_sdk_gen.schemas.post_o_auth_2_token import PostOAuth2TokenGrantTypeField
 
-from box_sdk_gen.schemas import PostOAuth2TokenSubjectTokenTypeField
+from box_sdk_gen.schemas.post_o_auth_2_token import PostOAuth2TokenSubjectTokenTypeField
 
-from box_sdk_gen.schemas import AccessToken
+from box_sdk_gen.schemas.access_token import AccessToken
 
-from box_sdk_gen.schemas import PostOAuth2TokenBoxSubjectTypeField
+from box_sdk_gen.schemas.post_o_auth_2_token import PostOAuth2TokenBoxSubjectTypeField
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.box.token_storage import TokenStorage
 
 from box_sdk_gen.box.token_storage import InMemoryTokenStorage
 
 from box_sdk_gen.managers.authorization import AuthorizationManager
 
 from box_sdk_gen.box.errors import BoxSDKError
 
-from box_sdk_gen.schemas import PostOAuth2Token
+from box_sdk_gen.schemas.post_o_auth_2_token import PostOAuth2Token
 
-from box_sdk_gen.schemas import PostOAuth2Revoke
+from box_sdk_gen.schemas.post_o_auth_2_revoke import PostOAuth2Revoke
 
 
 class CCGConfig:
     def __init__(
         self,
         client_id: str,
         client_secret: str,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/box/developer_token_auth.py` & `box_sdk_gen-1.0.0/box_sdk_gen/box/developer_token_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from typing import Optional
 
 from typing import List
 
-from box_sdk_gen.schemas import PostOAuth2TokenGrantTypeField
+from box_sdk_gen.schemas.post_o_auth_2_token import PostOAuth2TokenGrantTypeField
 
-from box_sdk_gen.schemas import PostOAuth2TokenSubjectTokenTypeField
+from box_sdk_gen.schemas.post_o_auth_2_token import PostOAuth2TokenSubjectTokenTypeField
 
-from box_sdk_gen.schemas import AccessToken
+from box_sdk_gen.schemas.access_token import AccessToken
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.box.errors import BoxSDKError
 
 from box_sdk_gen.box.token_storage import TokenStorage
 
 from box_sdk_gen.box.token_storage import InMemoryTokenStorage
 
 from box_sdk_gen.managers.authorization import AuthorizationManager
 
-from box_sdk_gen.schemas import PostOAuth2Token
+from box_sdk_gen.schemas.post_o_auth_2_token import PostOAuth2Token
 
-from box_sdk_gen.schemas import PostOAuth2Revoke
+from box_sdk_gen.schemas.post_o_auth_2_revoke import PostOAuth2Revoke
 
 
 class DeveloperTokenConfig:
     def __init__(
         self, *, client_id: Optional[str] = None, client_secret: Optional[str] = None
     ):
         self.client_id = client_id
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/box/errors.py` & `box_sdk_gen-1.0.0/box_sdk_gen/box/errors.py`

 * *Files identical despite different names*

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/box/jwt_auth.py` & `box_sdk_gen-1.0.0/box_sdk_gen/box/jwt_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 
 from typing import Optional
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from typing import List
 
-from box_sdk_gen.schemas import PostOAuth2TokenGrantTypeField
+from box_sdk_gen.schemas.post_o_auth_2_token import PostOAuth2TokenGrantTypeField
 
-from box_sdk_gen.schemas import PostOAuth2TokenSubjectTokenTypeField
+from box_sdk_gen.schemas.post_o_auth_2_token import PostOAuth2TokenSubjectTokenTypeField
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
-from box_sdk_gen.schemas import AccessToken
+from box_sdk_gen.schemas.access_token import AccessToken
 
-from box_sdk_gen.schemas import PostOAuth2Token
+from box_sdk_gen.schemas.post_o_auth_2_token import PostOAuth2Token
 
-from box_sdk_gen.schemas import PostOAuth2Revoke
+from box_sdk_gen.schemas.post_o_auth_2_revoke import PostOAuth2Revoke
 
 from box_sdk_gen.box.token_storage import TokenStorage
 
 from box_sdk_gen.box.token_storage import InMemoryTokenStorage
 
 from box_sdk_gen.serialization.json.json_data import json_to_serialized_data
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/box/oauth.py` & `box_sdk_gen-1.0.0/box_sdk_gen/box/oauth.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 from typing import Dict
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
 from typing import List
 
-from box_sdk_gen.schemas import PostOAuth2TokenGrantTypeField
+from box_sdk_gen.schemas.post_o_auth_2_token import PostOAuth2TokenGrantTypeField
 
-from box_sdk_gen.schemas import PostOAuth2TokenSubjectTokenTypeField
+from box_sdk_gen.schemas.post_o_auth_2_token import PostOAuth2TokenSubjectTokenTypeField
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
-from box_sdk_gen.schemas import AccessToken
+from box_sdk_gen.schemas.access_token import AccessToken
 
-from box_sdk_gen.schemas import PostOAuth2Token
+from box_sdk_gen.schemas.post_o_auth_2_token import PostOAuth2Token
 
-from box_sdk_gen.schemas import PostOAuth2Revoke
+from box_sdk_gen.schemas.post_o_auth_2_revoke import PostOAuth2Revoke
 
 from box_sdk_gen.managers.authorization import AuthorizationManager
 
 from box_sdk_gen.box.token_storage import TokenStorage
 
 from box_sdk_gen.box.token_storage import InMemoryTokenStorage
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/box/token_storage.py` & `box_sdk_gen-1.0.0/box_sdk_gen/box/token_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import shelve
 from abc import abstractmethod
 from typing import Optional
 
-from ..schemas import AccessToken
+from ..schemas.access_token import AccessToken
 
 
 class TokenStorage:
     @abstractmethod
     def store(self, token: AccessToken) -> None:
         pass
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/client.py` & `box_sdk_gen-1.0.0/box_sdk_gen/client.py`

 * *Files identical despite different names*

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/internal/base_object.py` & `box_sdk_gen-1.0.0/box_sdk_gen/internal/base_object.py`

 * *Files identical despite different names*

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/internal/utils.py` & `box_sdk_gen-1.0.0/box_sdk_gen/internal/utils.py`

 * *Files identical despite different names*

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/__init__.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/ai.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/ai.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.internal.utils import DateTime
 
-from box_sdk_gen.schemas import AiResponse
+from box_sdk_gen.schemas.ai_response import AiResponse
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import AiAsk
+from box_sdk_gen.schemas.ai_ask import AiAsk
 
-from box_sdk_gen.schemas import AiTextGen
+from box_sdk_gen.schemas.ai_text_gen import AiTextGen
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -159,15 +159,15 @@
         :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         request_body: Dict = {'mode': mode, 'prompt': prompt, 'items': items}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/ai/ask']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/ai/ask']),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
                 auth=self.auth,
@@ -200,15 +200,15 @@
         request_body: Dict = {
             'prompt': prompt,
             'items': items,
             'dialogue_history': dialogue_history,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/ai/text_gen']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/ai/text_gen']),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
                 auth=self.auth,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/authorization.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/authorization.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,29 +6,31 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import PostOAuth2TokenGrantTypeField
+from box_sdk_gen.schemas.post_o_auth_2_token import PostOAuth2TokenGrantTypeField
 
-from box_sdk_gen.schemas import PostOAuth2TokenSubjectTokenTypeField
+from box_sdk_gen.schemas.post_o_auth_2_token import PostOAuth2TokenSubjectTokenTypeField
 
-from box_sdk_gen.schemas import PostOAuth2TokenBoxSubjectTypeField
+from box_sdk_gen.schemas.post_o_auth_2_token import PostOAuth2TokenBoxSubjectTypeField
 
-from box_sdk_gen.schemas import AccessToken
+from box_sdk_gen.schemas.access_token import AccessToken
 
-from box_sdk_gen.schemas import OAuth2Error
+from box_sdk_gen.schemas.o_auth_2_error import OAuth2Error
 
-from box_sdk_gen.schemas import PostOAuth2Token
+from box_sdk_gen.schemas.post_o_auth_2_token import PostOAuth2Token
 
-from box_sdk_gen.schemas import PostOAuth2TokenRefreshAccessToken
+from box_sdk_gen.schemas.post_o_auth_2_token_refresh_access_token import (
+    PostOAuth2TokenRefreshAccessToken,
+)
 
-from box_sdk_gen.schemas import PostOAuth2Revoke
+from box_sdk_gen.schemas.post_o_auth_2_revoke import PostOAuth2Revoke
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -317,15 +319,15 @@
             'resource': resource,
             'box_subject_type': box_subject_type,
             'box_subject_id': box_subject_id,
             'box_shared_link': box_shared_link,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join(['https://api.box.com/oauth2/token']),
+            ''.join([self.network_session.base_urls.base_url, '/oauth2/token']),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/x-www-form-urlencoded',
                 response_format='json',
                 auth=self.auth,
@@ -362,15 +364,15 @@
             'grant_type': grant_type,
             'client_id': client_id,
             'client_secret': client_secret,
             'refresh_token': refresh_token,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join(['https://api.box.com/oauth2/token#refresh']),
+            ''.join([self.network_session.base_urls.base_url, '/oauth2/token#refresh']),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/x-www-form-urlencoded',
                 response_format='json',
                 auth=self.auth,
@@ -408,15 +410,15 @@
         request_body: Dict = {
             'client_id': client_id,
             'client_secret': client_secret,
             'token': token,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join(['https://api.box.com/oauth2/revoke']),
+            ''.join([self.network_session.base_urls.base_url, '/oauth2/revoke']),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/x-www-form-urlencoded',
                 response_format=None,
                 auth=self.auth,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/avatars.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/avatars.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 from typing import Dict
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import UserAvatar
+from box_sdk_gen.schemas.user_avatar import UserAvatar
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -59,15 +59,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/users/',
+                    '/2.0/users/',
                     to_string(user_id),
                     '/avatar',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
@@ -107,15 +107,15 @@
             'pic_content_type': pic_content_type,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/users/',
+                    '/2.0/users/',
                     to_string(user_id),
                     '/avatar',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
@@ -152,15 +152,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/users/',
+                    '/2.0/users/',
                     to_string(user_id),
                     '/avatar',
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/chunked_uploads.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/chunked_uploads.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.internal.utils import Buffer
 
 from box_sdk_gen.internal.utils import HashName
 
-from box_sdk_gen.schemas import FileFull
+from box_sdk_gen.schemas.file_full import FileFull
 
 from box_sdk_gen.internal.utils import Iterator
 
-from box_sdk_gen.schemas import UploadSession
+from box_sdk_gen.schemas.upload_session import UploadSession
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import UploadedPart
+from box_sdk_gen.schemas.uploaded_part import UploadedPart
 
-from box_sdk_gen.schemas import UploadParts
+from box_sdk_gen.schemas.upload_parts import UploadParts
 
-from box_sdk_gen.schemas import Files
+from box_sdk_gen.schemas.files import Files
 
-from box_sdk_gen.schemas import UploadPart
+from box_sdk_gen.schemas.upload_part import UploadPart
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -61,15 +61,15 @@
 from box_sdk_gen.internal.utils import reduce_iterator
 
 from box_sdk_gen.internal.utils import Hash
 
 from box_sdk_gen.internal.utils import buffer_length
 
 
-class PartAccumulator:
+class _PartAccumulator:
     def __init__(
         self,
         last_index: int,
         parts: List[UploadPart],
         file_size: int,
         upload_session_id: str,
         file_hash: Hash,
@@ -118,15 +118,18 @@
             'folder_id': folder_id,
             'file_size': file_size,
             'file_name': file_name,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.upload_url, '/files/upload_sessions']
+                [
+                    self.network_session.base_urls.upload_url,
+                    '/2.0/files/upload_sessions',
+                ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
@@ -166,15 +169,15 @@
             extra_headers = {}
         request_body: Dict = {'file_size': file_size, 'file_name': file_name}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.upload_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/upload_sessions',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
@@ -204,15 +207,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.upload_url,
-                    '/files/upload_sessions/',
+                    '/2.0/files/upload_sessions/',
                     to_string(upload_session_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
@@ -276,15 +279,15 @@
                 **extra_headers,
             }
         )
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.upload_url,
-                    '/files/upload_sessions/',
+                    '/2.0/files/upload_sessions/',
                     to_string(upload_session_id),
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
                 file_stream=request_body,
@@ -316,15 +319,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.upload_url,
-                    '/files/upload_sessions/',
+                    '/2.0/files/upload_sessions/',
                     to_string(upload_session_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
@@ -367,15 +370,15 @@
             {'offset': to_string(offset), 'limit': to_string(limit)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.upload_url,
-                    '/files/upload_sessions/',
+                    '/2.0/files/upload_sessions/',
                     to_string(upload_session_id),
                     '/parts',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
@@ -444,15 +447,15 @@
                 **extra_headers,
             }
         )
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.upload_url,
-                    '/files/upload_sessions/',
+                    '/2.0/files/upload_sessions/',
                     to_string(upload_session_id),
                     '/commit',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
@@ -461,15 +464,15 @@
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
         return deserialize(response.data, Files)
 
-    def _reducer(self, acc: PartAccumulator, chunk: ByteStream) -> PartAccumulator:
+    def _reducer(self, acc: _PartAccumulator, chunk: ByteStream) -> _PartAccumulator:
         last_index: int = acc.last_index
         parts: List[UploadPart] = acc.parts
         chunk_buffer: Buffer = read_byte_stream(chunk)
         hash: Hash = Hash(algorithm=HashName.SHA1.value)
         hash.update_hash(chunk_buffer)
         sha_1: str = hash.digest_hash('base64')
         digest: str = ''.join(['sha=', sha_1])
@@ -494,15 +497,15 @@
         )
         part: UploadPart = uploaded_part.part
         part_sha_1: str = hex_to_base_64(part.sha_1)
         assert part_sha_1 == sha_1
         assert part.size == chunk_size
         assert part.offset == bytes_start
         acc.file_hash.update_hash(chunk_buffer)
-        return PartAccumulator(
+        return _PartAccumulator(
             last_index=bytes_end,
             parts=parts + [part],
             file_size=acc.file_size,
             upload_session_id=acc.upload_session_id,
             file_hash=acc.file_hash,
         )
 
@@ -526,18 +529,18 @@
         upload_session_id: str = upload_session.id
         part_size: int = upload_session.part_size
         total_parts: int = upload_session.total_parts
         assert part_size * total_parts >= file_size
         assert upload_session.num_parts_processed == 0
         file_hash: Hash = Hash(algorithm=HashName.SHA1.value)
         chunks_iterator: Iterator = iterate_chunks(file, part_size)
-        results: PartAccumulator = reduce_iterator(
+        results: _PartAccumulator = reduce_iterator(
             chunks_iterator,
             self._reducer,
-            PartAccumulator(
+            _PartAccumulator(
                 last_index=-1,
                 parts=[],
                 file_size=file_size,
                 upload_session_id=upload_session_id,
                 file_hash=file_hash,
             ),
         )
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/classifications.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/classifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 from typing import List
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import ClassificationTemplate
+from box_sdk_gen.schemas.classification_template import ClassificationTemplate
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -511,15 +511,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/metadata_templates/enterprise/securityClassification-6VMVochwUWo/schema',
+                    '/2.0/metadata_templates/enterprise/securityClassification-6VMVochwUWo/schema',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
@@ -556,15 +556,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/metadata_templates/enterprise/securityClassification-6VMVochwUWo/schema#add',
+                    '/2.0/metadata_templates/enterprise/securityClassification-6VMVochwUWo/schema#add',
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
@@ -603,15 +603,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/metadata_templates/enterprise/securityClassification-6VMVochwUWo/schema#update',
+                    '/2.0/metadata_templates/enterprise/securityClassification-6VMVochwUWo/schema#update',
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json-patch+json',
@@ -685,15 +685,15 @@
             'fields': fields,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/metadata_templates/schema#classifications',
+                    '/2.0/metadata_templates/schema#classifications',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/collaboration_allowlist_entries.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/collaboration_allowlist_entries.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,23 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import CollaborationAllowlistEntries
-
-from box_sdk_gen.schemas import ClientError
-
-from box_sdk_gen.schemas import CollaborationAllowlistEntry
+from box_sdk_gen.schemas.collaboration_allowlist_entries import (
+    CollaborationAllowlistEntries,
+)
+
+from box_sdk_gen.schemas.client_error import ClientError
+
+from box_sdk_gen.schemas.collaboration_allowlist_entry import (
+    CollaborationAllowlistEntry,
+)
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -83,15 +87,15 @@
             {'marker': to_string(marker), 'limit': to_string(limit)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/collaboration_whitelist_entries',
+                    '/2.0/collaboration_whitelist_entries',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
@@ -124,15 +128,15 @@
             extra_headers = {}
         request_body: Dict = {'domain': domain, 'direction': direction}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/collaboration_whitelist_entries',
+                    '/2.0/collaboration_whitelist_entries',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
@@ -163,15 +167,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/collaboration_whitelist_entries/',
+                    '/2.0/collaboration_whitelist_entries/',
                     to_string(collaboration_whitelist_entry_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
@@ -201,15 +205,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/collaboration_whitelist_entries/',
+                    '/2.0/collaboration_whitelist_entries/',
                     to_string(collaboration_whitelist_entry_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/collaboration_allowlist_exempt_targets.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/collaboration_allowlist_exempt_targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,23 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import CollaborationAllowlistExemptTargets
-
-from box_sdk_gen.schemas import ClientError
-
-from box_sdk_gen.schemas import CollaborationAllowlistExemptTarget
+from box_sdk_gen.schemas.collaboration_allowlist_exempt_targets import (
+    CollaborationAllowlistExemptTargets,
+)
+
+from box_sdk_gen.schemas.client_error import ClientError
+
+from box_sdk_gen.schemas.collaboration_allowlist_exempt_target import (
+    CollaborationAllowlistExemptTarget,
+)
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -87,15 +91,15 @@
             {'marker': to_string(marker), 'limit': to_string(limit)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/collaboration_whitelist_exempt_targets',
+                    '/2.0/collaboration_whitelist_exempt_targets',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
@@ -125,15 +129,15 @@
             extra_headers = {}
         request_body: Dict = {'user': user}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/collaboration_whitelist_exempt_targets',
+                    '/2.0/collaboration_whitelist_exempt_targets',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
@@ -164,15 +168,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/collaboration_whitelist_exempt_targets/',
+                    '/2.0/collaboration_whitelist_exempt_targets/',
                     to_string(collaboration_whitelist_exempt_target_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
@@ -202,15 +206,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/collaboration_whitelist_exempt_targets/',
+                    '/2.0/collaboration_whitelist_exempt_targets/',
                     to_string(collaboration_whitelist_exempt_target_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/collections.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 from typing import Dict
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import Collections
+from box_sdk_gen.schemas.collections import Collections
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import Items
+from box_sdk_gen.schemas.items import Items
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -91,15 +91,15 @@
                 'fields': to_string(fields),
                 'offset': to_string(offset),
                 'limit': to_string(limit),
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/collections']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/collections']),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
@@ -155,15 +155,15 @@
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/collections/',
+                    '/2.0/collections/',
                     to_string(collection_id),
                     '/items',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/comments.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/comments.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import Comments
+from box_sdk_gen.schemas.comments import Comments
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import CommentFull
+from box_sdk_gen.schemas.comment_full import CommentFull
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -124,15 +124,15 @@
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/comments',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
@@ -176,15 +176,15 @@
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/comments/',
+                    '/2.0/comments/',
                     to_string(comment_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
@@ -228,15 +228,15 @@
         request_body: Dict = {'message': message}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/comments/',
+                    '/2.0/comments/',
                     to_string(comment_id),
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 params=query_params_map,
                 headers=headers_map,
@@ -266,15 +266,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/comments/',
+                    '/2.0/comments/',
                     to_string(comment_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
@@ -336,15 +336,15 @@
             'message': message,
             'tagged_message': tagged_message,
             'item': item,
         }
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/comments']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/comments']),
             FetchOptions(
                 method='POST',
                 params=query_params_map,
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/device_pinners.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/device_pinners.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 from typing import Dict
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import DevicePinner
+from box_sdk_gen.schemas.device_pinner import DevicePinner
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import DevicePinners
+from box_sdk_gen.schemas.device_pinners import DevicePinners
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -69,15 +69,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/device_pinners/',
+                    '/2.0/device_pinners/',
                     to_string(device_pinner_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
@@ -104,15 +104,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/device_pinners/',
+                    '/2.0/device_pinners/',
                     to_string(device_pinner_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
@@ -165,15 +165,15 @@
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/enterprises/',
+                    '/2.0/enterprises/',
                     to_string(enterprise_id),
                     '/device_pinners',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/downloads.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/downloads.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 from typing import Dict
 
 from box_sdk_gen.internal.utils import to_string
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -90,15 +90,15 @@
         headers_map: Dict[str, str] = prepare_params(
             {'range': to_string(range), 'boxapi': to_string(boxapi), **extra_headers}
         )
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/content',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/email_aliases.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/email_aliases.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import EmailAliases
+from box_sdk_gen.schemas.email_aliases import EmailAliases
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import EmailAlias
+from box_sdk_gen.schemas.email_alias import EmailAlias
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -64,15 +64,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/users/',
+                    '/2.0/users/',
                     to_string(user_id),
                     '/email_aliases',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
@@ -110,15 +110,15 @@
             extra_headers = {}
         request_body: Dict = {'email': email}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/users/',
+                    '/2.0/users/',
                     to_string(user_id),
                     '/email_aliases',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
@@ -152,15 +152,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/users/',
+                    '/2.0/users/',
                     to_string(user_id),
                     '/email_aliases/',
                     to_string(email_alias_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/events.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 from typing import Dict
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import Events
+from box_sdk_gen.schemas.events import Events
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import RealtimeServers
+from box_sdk_gen.schemas.realtime_servers import RealtimeServers
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -285,15 +285,15 @@
                 'event_type': to_string(event_type),
                 'created_after': to_string(created_after),
                 'created_before': to_string(created_before),
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/events']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/events']),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
@@ -381,15 +381,15 @@
         :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
         :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/events']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/events']),
             FetchOptions(
                 method='OPTIONS',
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/file_classifications.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/file_classifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
 from typing import List
 
-from box_sdk_gen.schemas import Classification
+from box_sdk_gen.schemas.classification import Classification
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -120,15 +120,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/metadata/enterprise/securityClassification-6VMVochwUWo',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
@@ -185,15 +185,15 @@
             'Box__Security__Classification__Key': box_security_classification_key
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/metadata/enterprise/securityClassification-6VMVochwUWo',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
@@ -241,15 +241,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/metadata/enterprise/securityClassification-6VMVochwUWo',
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
@@ -291,15 +291,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/metadata/enterprise/securityClassification-6VMVochwUWo',
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/file_metadata.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/file_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
 from typing import List
 
-from box_sdk_gen.schemas import Metadatas
+from box_sdk_gen.schemas.metadatas import Metadatas
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import MetadataFull
+from box_sdk_gen.schemas.metadata_full import MetadataFull
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -155,15 +155,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/metadata',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
@@ -208,15 +208,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/metadata/',
                     to_string(scope),
                     '/',
                     to_string(template_key),
                 ]
             ),
@@ -273,15 +273,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/metadata/',
                     to_string(scope),
                     '/',
                     to_string(template_key),
                 ]
             ),
@@ -346,15 +346,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/metadata/',
                     to_string(scope),
                     '/',
                     to_string(template_key),
                 ]
             ),
@@ -401,15 +401,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/metadata/',
                     to_string(scope),
                     '/',
                     to_string(template_key),
                 ]
             ),
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/file_requests.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/file_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
 from box_sdk_gen.internal.utils import DateTime
 
-from box_sdk_gen.schemas import FileRequest
+from box_sdk_gen.schemas.file_request import FileRequest
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import FileRequestUpdateRequest
+from box_sdk_gen.schemas.file_request_update_request import FileRequestUpdateRequest
 
-from box_sdk_gen.schemas import FileRequestCopyRequest
+from box_sdk_gen.schemas.file_request_copy_request import FileRequestCopyRequest
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -114,15 +114,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/file_requests/',
+                    '/2.0/file_requests/',
                     to_string(file_request_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
@@ -226,15 +226,15 @@
         headers_map: Dict[str, str] = prepare_params(
             {'if-match': to_string(if_match), **extra_headers}
         )
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/file_requests/',
+                    '/2.0/file_requests/',
                     to_string(file_request_id),
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
                 data=serialize(request_body),
@@ -269,15 +269,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/file_requests/',
+                    '/2.0/file_requests/',
                     to_string(file_request_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
@@ -374,15 +374,15 @@
             'expires_at': expires_at,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/file_requests/',
+                    '/2.0/file_requests/',
                     to_string(file_request_id),
                     '/copy',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/file_version_legal_holds.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/file_version_legal_holds.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from typing import Dict
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import FileVersionLegalHold
+from box_sdk_gen.schemas.file_version_legal_hold import FileVersionLegalHold
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import FileVersionLegalHolds
+from box_sdk_gen.schemas.file_version_legal_holds import FileVersionLegalHolds
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -65,15 +65,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/file_version_legal_holds/',
+                    '/2.0/file_version_legal_holds/',
                     to_string(file_version_legal_hold_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
@@ -156,15 +156,18 @@
                 'marker': to_string(marker),
                 'limit': to_string(limit),
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/file_version_legal_holds']
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/file_version_legal_holds',
+                ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/file_version_retentions.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/file_version_retentions.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 from typing import Dict
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import FileVersionRetentions
+from box_sdk_gen.schemas.file_version_retentions import FileVersionRetentions
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import FileVersionRetention
+from box_sdk_gen.schemas.file_version_retention import FileVersionRetention
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -105,15 +105,18 @@
                 'limit': to_string(limit),
                 'marker': to_string(marker),
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/file_version_retentions']
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/file_version_retentions',
+                ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
@@ -139,15 +142,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/file_version_retentions/',
+                    '/2.0/file_version_retentions/',
                     to_string(file_version_retention_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/file_versions.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/file_versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import FileVersions
+from box_sdk_gen.schemas.file_versions import FileVersions
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import FileVersionFull
+from box_sdk_gen.schemas.file_version_full import FileVersionFull
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -112,15 +112,15 @@
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/versions',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
@@ -174,15 +174,15 @@
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/versions/',
                     to_string(file_version_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
@@ -236,15 +236,15 @@
             extra_headers = {}
         request_body: Dict = {'trashed_at': trashed_at}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/versions/',
                     to_string(file_version_id),
                 ]
             ),
             FetchOptions(
                 method='PUT',
@@ -299,15 +299,15 @@
         headers_map: Dict[str, str] = prepare_params(
             {'if-match': to_string(if_match), **extra_headers}
         )
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/versions/',
                     to_string(file_version_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
@@ -394,15 +394,15 @@
         request_body: Dict = {'id': id, 'type': type}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/versions/current',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 params=query_params_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/file_watermarks.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/folder_watermarks.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import Watermark
+from box_sdk_gen.schemas.watermark import Watermark
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -33,119 +33,128 @@
 from box_sdk_gen.networking.fetch import fetch
 
 from box_sdk_gen.serialization.json.json_data import sd_to_json
 
 from box_sdk_gen.serialization.json.json_data import SerializedData
 
 
-class UpdateFileWatermarkWatermarkImprintField(str, Enum):
+class UpdateFolderWatermarkWatermarkImprintField(str, Enum):
     DEFAULT = 'default'
 
 
-class UpdateFileWatermarkWatermark(BaseObject):
+class UpdateFolderWatermarkWatermark(BaseObject):
     def __init__(
         self,
         *,
-        imprint: UpdateFileWatermarkWatermarkImprintField = UpdateFileWatermarkWatermarkImprintField.DEFAULT.value,
+        imprint: UpdateFolderWatermarkWatermarkImprintField = UpdateFolderWatermarkWatermarkImprintField.DEFAULT.value,
         **kwargs
     ):
         """
                 :param imprint: The type of watermark to apply.
 
-        Currently only supports one option., defaults to UpdateFileWatermarkWatermarkImprintField.DEFAULT.value
-                :type imprint: UpdateFileWatermarkWatermarkImprintField, optional
+        Currently only supports one option., defaults to UpdateFolderWatermarkWatermarkImprintField.DEFAULT.value
+                :type imprint: UpdateFolderWatermarkWatermarkImprintField, optional
         """
         super().__init__(**kwargs)
         self.imprint = imprint
 
 
-class FileWatermarksManager:
+class FolderWatermarksManager:
     def __init__(
         self,
         *,
         auth: Optional[Authentication] = None,
         network_session: NetworkSession = None
     ):
         if network_session is None:
             network_session = NetworkSession()
         self.auth = auth
         self.network_session = network_session
 
-    def get_file_watermark(
-        self, file_id: str, *, extra_headers: Optional[Dict[str, Optional[str]]] = None
+    def get_folder_watermark(
+        self,
+        folder_id: str,
+        *,
+        extra_headers: Optional[Dict[str, Optional[str]]] = None
     ) -> Watermark:
         """
-                Retrieve the watermark for a file.
-                :param file_id: The unique identifier that represents a file.
+                Retrieve the watermark for a folder.
+                :param folder_id: The unique identifier that represent a folder.
 
-        The ID for any file can be determined
-        by visiting a file in the web application
+        The ID for any folder can be determined
+        by visiting this folder in the web application
         and copying the ID from the URL. For example,
-        for the URL `https://*.app.box.com/files/123`
-        the `file_id` is `123`.
+        for the URL `https://*.app.box.com/folder/123`
+        the `folder_id` is `123`.
+
+        The root folder of a Box account is
+        always represented by the ID `0`.
         Example: "12345"
-                :type file_id: str
+                :type folder_id: str
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
-                    to_string(file_id),
+                    '/2.0/folders/',
+                    to_string(folder_id),
                     '/watermark',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
         return deserialize(response.data, Watermark)
 
-    def update_file_watermark(
+    def update_folder_watermark(
         self,
-        file_id: str,
-        watermark: UpdateFileWatermarkWatermark,
+        folder_id: str,
+        watermark: UpdateFolderWatermarkWatermark,
         *,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
     ) -> Watermark:
         """
-                Applies or update a watermark on a file.
-                :param file_id: The unique identifier that represents a file.
+                Applies or update a watermark on a folder.
+                :param folder_id: The unique identifier that represent a folder.
 
-        The ID for any file can be determined
-        by visiting a file in the web application
+        The ID for any folder can be determined
+        by visiting this folder in the web application
         and copying the ID from the URL. For example,
-        for the URL `https://*.app.box.com/files/123`
-        the `file_id` is `123`.
+        for the URL `https://*.app.box.com/folder/123`
+        the `folder_id` is `123`.
+
+        The root folder of a Box account is
+        always represented by the ID `0`.
         Example: "12345"
-                :type file_id: str
-                :param watermark: The watermark to imprint on the file
-                :type watermark: UpdateFileWatermarkWatermark
+                :type folder_id: str
+                :param watermark: The watermark to imprint on the folder
+                :type watermark: UpdateFolderWatermarkWatermark
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         request_body: Dict = {'watermark': watermark}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
-                    to_string(file_id),
+                    '/2.0/folders/',
+                    to_string(folder_id),
                     '/watermark',
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
                 data=serialize(request_body),
@@ -153,40 +162,46 @@
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
         return deserialize(response.data, Watermark)
 
-    def delete_file_watermark(
-        self, file_id: str, *, extra_headers: Optional[Dict[str, Optional[str]]] = None
+    def delete_folder_watermark(
+        self,
+        folder_id: str,
+        *,
+        extra_headers: Optional[Dict[str, Optional[str]]] = None
     ) -> None:
         """
-                Removes the watermark from a file.
-                :param file_id: The unique identifier that represents a file.
+                Removes the watermark from a folder.
+                :param folder_id: The unique identifier that represent a folder.
 
-        The ID for any file can be determined
-        by visiting a file in the web application
+        The ID for any folder can be determined
+        by visiting this folder in the web application
         and copying the ID from the URL. For example,
-        for the URL `https://*.app.box.com/files/123`
-        the `file_id` is `123`.
+        for the URL `https://*.app.box.com/folder/123`
+        the `folder_id` is `123`.
+
+        The root folder of a Box account is
+        always represented by the ID `0`.
         Example: "12345"
-                :type file_id: str
+                :type folder_id: str
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
-                    to_string(file_id),
+                    '/2.0/folders/',
+                    to_string(folder_id),
                     '/watermark',
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/files.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import FileFull
+from box_sdk_gen.schemas.file_full import FileFull
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -302,15 +302,19 @@
                 'boxapi': to_string(boxapi),
                 'x-rep-hints': to_string(x_rep_hints),
                 **extra_headers,
             }
         )
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/files/', to_string(file_id)]
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/files/',
+                    to_string(file_id),
+                ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
@@ -426,15 +430,19 @@
         }
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params(
             {'if-match': to_string(if_match), **extra_headers}
         )
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/files/', to_string(file_id)]
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/files/',
+                    to_string(file_id),
+                ]
             ),
             FetchOptions(
                 method='PUT',
                 params=query_params_map,
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
@@ -486,15 +494,19 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params(
             {'if-match': to_string(if_match), **extra_headers}
         )
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/files/', to_string(file_id)]
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/files/',
+                    to_string(file_id),
+                ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
                 auth=self.auth,
                 network_session=self.network_session,
@@ -553,15 +565,15 @@
         request_body: Dict = {'name': name, 'version': version, 'parent': parent}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/copy',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 params=query_params_map,
@@ -640,15 +652,15 @@
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/thumbnail.',
                     to_string(extension),
                 ]
             ),
             FetchOptions(
                 method='GET',
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/folder_classifications.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/folder_classifications.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
 from typing import List
 
-from box_sdk_gen.schemas import Classification
+from box_sdk_gen.schemas.classification import Classification
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -126,15 +126,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                     '/metadata/enterprise/securityClassification-6VMVochwUWo',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
@@ -194,15 +194,15 @@
             'Box__Security__Classification__Key': box_security_classification_key
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                     '/metadata/enterprise/securityClassification-6VMVochwUWo',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
@@ -253,15 +253,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                     '/metadata/enterprise/securityClassification-6VMVochwUWo',
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
@@ -309,15 +309,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                     '/metadata/enterprise/securityClassification-6VMVochwUWo',
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/folder_locks.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/folder_locks.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import FolderLocks
+from box_sdk_gen.schemas.folder_locks import FolderLocks
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import FolderLock
+from box_sdk_gen.schemas.folder_lock import FolderLock
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -107,15 +107,15 @@
         if extra_headers is None:
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params(
             {'folder_id': to_string(folder_id)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/folder_locks']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/folder_locks']),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
@@ -151,15 +151,15 @@
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         request_body: Dict = {'locked_operations': locked_operations, 'folder': folder}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/folder_locks']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/folder_locks']),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
                 auth=self.auth,
@@ -191,15 +191,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folder_locks/',
+                    '/2.0/folder_locks/',
                     to_string(folder_lock_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/folder_metadata.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/folder_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
 from typing import List
 
-from box_sdk_gen.schemas import Metadatas
+from box_sdk_gen.schemas.metadatas import Metadatas
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import MetadataFull
+from box_sdk_gen.schemas.metadata_full import MetadataFull
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -164,15 +164,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                     '/metadata',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
@@ -220,15 +220,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                     '/metadata/',
                     to_string(scope),
                     '/',
                     to_string(template_key),
                 ]
             ),
@@ -297,15 +297,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                     '/metadata/',
                     to_string(scope),
                     '/',
                     to_string(template_key),
                 ]
             ),
@@ -373,15 +373,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                     '/metadata/',
                     to_string(scope),
                     '/',
                     to_string(template_key),
                 ]
             ),
@@ -431,15 +431,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                     '/metadata/',
                     to_string(scope),
                     '/',
                     to_string(template_key),
                 ]
             ),
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/folder_watermarks.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/file_watermarks.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import Watermark
+from box_sdk_gen.schemas.watermark import Watermark
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -33,128 +33,119 @@
 from box_sdk_gen.networking.fetch import fetch
 
 from box_sdk_gen.serialization.json.json_data import sd_to_json
 
 from box_sdk_gen.serialization.json.json_data import SerializedData
 
 
-class UpdateFolderWatermarkWatermarkImprintField(str, Enum):
+class UpdateFileWatermarkWatermarkImprintField(str, Enum):
     DEFAULT = 'default'
 
 
-class UpdateFolderWatermarkWatermark(BaseObject):
+class UpdateFileWatermarkWatermark(BaseObject):
     def __init__(
         self,
         *,
-        imprint: UpdateFolderWatermarkWatermarkImprintField = UpdateFolderWatermarkWatermarkImprintField.DEFAULT.value,
+        imprint: UpdateFileWatermarkWatermarkImprintField = UpdateFileWatermarkWatermarkImprintField.DEFAULT.value,
         **kwargs
     ):
         """
                 :param imprint: The type of watermark to apply.
 
-        Currently only supports one option., defaults to UpdateFolderWatermarkWatermarkImprintField.DEFAULT.value
-                :type imprint: UpdateFolderWatermarkWatermarkImprintField, optional
+        Currently only supports one option., defaults to UpdateFileWatermarkWatermarkImprintField.DEFAULT.value
+                :type imprint: UpdateFileWatermarkWatermarkImprintField, optional
         """
         super().__init__(**kwargs)
         self.imprint = imprint
 
 
-class FolderWatermarksManager:
+class FileWatermarksManager:
     def __init__(
         self,
         *,
         auth: Optional[Authentication] = None,
         network_session: NetworkSession = None
     ):
         if network_session is None:
             network_session = NetworkSession()
         self.auth = auth
         self.network_session = network_session
 
-    def get_folder_watermark(
-        self,
-        folder_id: str,
-        *,
-        extra_headers: Optional[Dict[str, Optional[str]]] = None
+    def get_file_watermark(
+        self, file_id: str, *, extra_headers: Optional[Dict[str, Optional[str]]] = None
     ) -> Watermark:
         """
-                Retrieve the watermark for a folder.
-                :param folder_id: The unique identifier that represent a folder.
+                Retrieve the watermark for a file.
+                :param file_id: The unique identifier that represents a file.
 
-        The ID for any folder can be determined
-        by visiting this folder in the web application
+        The ID for any file can be determined
+        by visiting a file in the web application
         and copying the ID from the URL. For example,
-        for the URL `https://*.app.box.com/folder/123`
-        the `folder_id` is `123`.
-
-        The root folder of a Box account is
-        always represented by the ID `0`.
+        for the URL `https://*.app.box.com/files/123`
+        the `file_id` is `123`.
         Example: "12345"
-                :type folder_id: str
+                :type file_id: str
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
-                    to_string(folder_id),
+                    '/2.0/files/',
+                    to_string(file_id),
                     '/watermark',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
         return deserialize(response.data, Watermark)
 
-    def update_folder_watermark(
+    def update_file_watermark(
         self,
-        folder_id: str,
-        watermark: UpdateFolderWatermarkWatermark,
+        file_id: str,
+        watermark: UpdateFileWatermarkWatermark,
         *,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
     ) -> Watermark:
         """
-                Applies or update a watermark on a folder.
-                :param folder_id: The unique identifier that represent a folder.
+                Applies or update a watermark on a file.
+                :param file_id: The unique identifier that represents a file.
 
-        The ID for any folder can be determined
-        by visiting this folder in the web application
+        The ID for any file can be determined
+        by visiting a file in the web application
         and copying the ID from the URL. For example,
-        for the URL `https://*.app.box.com/folder/123`
-        the `folder_id` is `123`.
-
-        The root folder of a Box account is
-        always represented by the ID `0`.
+        for the URL `https://*.app.box.com/files/123`
+        the `file_id` is `123`.
         Example: "12345"
-                :type folder_id: str
-                :param watermark: The watermark to imprint on the folder
-                :type watermark: UpdateFolderWatermarkWatermark
+                :type file_id: str
+                :param watermark: The watermark to imprint on the file
+                :type watermark: UpdateFileWatermarkWatermark
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         request_body: Dict = {'watermark': watermark}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
-                    to_string(folder_id),
+                    '/2.0/files/',
+                    to_string(file_id),
                     '/watermark',
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
                 data=serialize(request_body),
@@ -162,46 +153,40 @@
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
         return deserialize(response.data, Watermark)
 
-    def delete_folder_watermark(
-        self,
-        folder_id: str,
-        *,
-        extra_headers: Optional[Dict[str, Optional[str]]] = None
+    def delete_file_watermark(
+        self, file_id: str, *, extra_headers: Optional[Dict[str, Optional[str]]] = None
     ) -> None:
         """
-                Removes the watermark from a folder.
-                :param folder_id: The unique identifier that represent a folder.
+                Removes the watermark from a file.
+                :param file_id: The unique identifier that represents a file.
 
-        The ID for any folder can be determined
-        by visiting this folder in the web application
+        The ID for any file can be determined
+        by visiting a file in the web application
         and copying the ID from the URL. For example,
-        for the URL `https://*.app.box.com/folder/123`
-        the `folder_id` is `123`.
-
-        The root folder of a Box account is
-        always represented by the ID `0`.
+        for the URL `https://*.app.box.com/files/123`
+        the `file_id` is `123`.
         Example: "12345"
-                :type folder_id: str
+                :type file_id: str
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
-                    to_string(folder_id),
+                    '/2.0/files/',
+                    to_string(file_id),
                     '/watermark',
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/folders.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/folders.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import FolderFull
+from box_sdk_gen.schemas.folder_full import FolderFull
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import Items
+from box_sdk_gen.schemas.items import Items
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -411,15 +411,15 @@
                 **extra_headers,
             }
         )
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
@@ -556,15 +556,15 @@
         headers_map: Dict[str, str] = prepare_params(
             {'if-match': to_string(if_match), **extra_headers}
         )
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 params=query_params_map,
                 headers=headers_map,
@@ -624,15 +624,15 @@
         headers_map: Dict[str, str] = prepare_params(
             {'if-match': to_string(if_match), **extra_headers}
         )
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 params=query_params_map,
                 headers=headers_map,
@@ -778,15 +778,15 @@
         headers_map: Dict[str, str] = prepare_params(
             {'boxapi': to_string(boxapi), **extra_headers}
         )
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                     '/items',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
@@ -846,15 +846,15 @@
             'parent': parent,
             'folder_upload_email': folder_upload_email,
             'sync_state': sync_state,
         }
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/folders']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/folders']),
             FetchOptions(
                 method='POST',
                 params=query_params_map,
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
@@ -919,15 +919,15 @@
         request_body: Dict = {'name': name, 'parent': parent}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                     '/copy',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 params=query_params_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/groups.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import Groups
+from box_sdk_gen.schemas.groups import Groups
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import GroupFull
+from box_sdk_gen.schemas.group_full import GroupFull
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -121,15 +121,15 @@
                 'fields': to_string(fields),
                 'limit': to_string(limit),
                 'offset': to_string(offset),
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/groups']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/groups']),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
@@ -222,15 +222,15 @@
             'description': description,
             'invitability_level': invitability_level,
             'member_viewability_level': member_viewability_level,
         }
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/groups']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/groups']),
             FetchOptions(
                 method='POST',
                 params=query_params_map,
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
@@ -275,15 +275,15 @@
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/groups/',
+                    '/2.0/groups/',
                     to_string(group_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
@@ -391,15 +391,15 @@
         }
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/groups/',
+                    '/2.0/groups/',
                     to_string(group_id),
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 params=query_params_map,
                 headers=headers_map,
@@ -429,15 +429,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/groups/',
+                    '/2.0/groups/',
                     to_string(group_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/integration_mappings.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/integration_mappings.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,27 +6,35 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import IntegrationMappingPartnerItemSlack
+from box_sdk_gen.schemas.integration_mapping_partner_item_slack import (
+    IntegrationMappingPartnerItemSlack,
+)
 
-from box_sdk_gen.schemas import IntegrationMappings
+from box_sdk_gen.schemas.integration_mappings import IntegrationMappings
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import IntegrationMapping
+from box_sdk_gen.schemas.integration_mapping import IntegrationMapping
 
-from box_sdk_gen.schemas import IntegrationMappingSlackCreateRequest
+from box_sdk_gen.schemas.integration_mapping_slack_create_request import (
+    IntegrationMappingSlackCreateRequest,
+)
 
-from box_sdk_gen.schemas import IntegrationMappingBoxItemSlack
+from box_sdk_gen.schemas.integration_mapping_box_item_slack import (
+    IntegrationMappingBoxItemSlack,
+)
 
-from box_sdk_gen.schemas import IntegrationMappingSlackOptions
+from box_sdk_gen.schemas.integration_mapping_slack_options import (
+    IntegrationMappingSlackOptions,
+)
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -117,15 +125,18 @@
                 'box_item_type': to_string(box_item_type),
                 'is_manually_created': to_string(is_manually_created),
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/integration_mappings/slack']
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/integration_mappings/slack',
+                ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
@@ -162,15 +173,18 @@
             'partner_item': partner_item,
             'box_item': box_item,
             'options': options,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/integration_mappings/slack']
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/integration_mappings/slack',
+                ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
@@ -209,15 +223,15 @@
             extra_headers = {}
         request_body: Dict = {'box_item': box_item, 'options': options}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/integration_mappings/slack/',
+                    '/2.0/integration_mappings/slack/',
                     to_string(integration_mapping_id),
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
                 data=serialize(request_body),
@@ -252,15 +266,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/integration_mappings/slack/',
+                    '/2.0/integration_mappings/slack/',
                     to_string(integration_mapping_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/invites.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/invites.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import Invite
+from box_sdk_gen.schemas.invite import Invite
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -116,15 +116,15 @@
         """
         if extra_headers is None:
             extra_headers = {}
         request_body: Dict = {'enterprise': enterprise, 'actionable_by': actionable_by}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/invites']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/invites']),
             FetchOptions(
                 method='POST',
                 params=query_params_map,
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
@@ -163,15 +163,15 @@
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/invites/',
+                    '/2.0/invites/',
                     to_string(invite_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/legal_hold_policies.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/legal_hold_policies.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import LegalHoldPolicies
+from box_sdk_gen.schemas.legal_hold_policies import LegalHoldPolicies
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import LegalHoldPolicy
+from box_sdk_gen.schemas.legal_hold_policy import LegalHoldPolicy
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -96,15 +96,17 @@
                 'fields': to_string(fields),
                 'marker': to_string(marker),
                 'limit': to_string(limit),
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/legal_hold_policies']),
+            ''.join(
+                [self.network_session.base_urls.base_url, '/2.0/legal_hold_policies']
+            ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
@@ -171,15 +173,17 @@
             'description': description,
             'filter_started_at': filter_started_at,
             'filter_ended_at': filter_ended_at,
             'is_ongoing': is_ongoing,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/legal_hold_policies']),
+            ''.join(
+                [self.network_session.base_urls.base_url, '/2.0/legal_hold_policies']
+            ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
                 auth=self.auth,
@@ -205,15 +209,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/legal_hold_policies/',
+                    '/2.0/legal_hold_policies/',
                     to_string(legal_hold_policy_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
@@ -254,15 +258,15 @@
             'release_notes': release_notes,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/legal_hold_policies/',
+                    '/2.0/legal_hold_policies/',
                     to_string(legal_hold_policy_id),
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
                 data=serialize(request_body),
@@ -297,15 +301,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/legal_hold_policies/',
+                    '/2.0/legal_hold_policies/',
                     to_string(legal_hold_policy_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/legal_hold_policy_assignments.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/retention_policies.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from enum import Enum
 
-from box_sdk_gen.internal.base_object import BaseObject
-
 from typing import Optional
 
 from typing import List
 
 from typing import Dict
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import LegalHoldPolicyAssignments
+from box_sdk_gen.schemas.retention_policies import RetentionPolicies
+
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.retention_policy import RetentionPolicy
 
-from box_sdk_gen.schemas import LegalHoldPolicyAssignment
+from box_sdk_gen.schemas.user_mini import UserMini
 
-from box_sdk_gen.schemas import FileVersionLegalHolds
+from box_sdk_gen.schemas.user_base import UserBase
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -39,436 +39,397 @@
 from box_sdk_gen.networking.fetch import FetchResponse
 
 from box_sdk_gen.networking.fetch import fetch
 
 from box_sdk_gen.serialization.json.json_data import SerializedData
 
 
-class GetLegalHoldPolicyAssignmentsAssignToType(str, Enum):
-    FILE = 'file'
-    FILE_VERSION = 'file_version'
-    FOLDER = 'folder'
-    USER = 'user'
-
-
-class CreateLegalHoldPolicyAssignmentAssignToTypeField(str, Enum):
-    FILE = 'file'
-    FILE_VERSION = 'file_version'
-    FOLDER = 'folder'
-    USER = 'user'
+class GetRetentionPoliciesPolicyType(str, Enum):
+    FINITE = 'finite'
+    INDEFINITE = 'indefinite'
 
 
-class CreateLegalHoldPolicyAssignmentAssignTo(BaseObject):
-    _discriminator = 'type', {'file', 'file_version', 'folder', 'user'}
+class CreateRetentionPolicyPolicyType(str, Enum):
+    FINITE = 'finite'
+    INDEFINITE = 'indefinite'
 
-    def __init__(
-        self, type: CreateLegalHoldPolicyAssignmentAssignToTypeField, id: str, **kwargs
-    ):
-        """
-        :param type: The type of item to assign the policy to
-        :type type: CreateLegalHoldPolicyAssignmentAssignToTypeField
-        :param id: The ID of item to assign the policy to
-        :type id: str
-        """
-        super().__init__(**kwargs)
-        self.type = type
-        self.id = id
 
+class CreateRetentionPolicyDispositionAction(str, Enum):
+    PERMANENTLY_DELETE = 'permanently_delete'
+    REMOVE_RETENTION = 'remove_retention'
 
-class LegalHoldPolicyAssignmentsManager:
+
+class CreateRetentionPolicyRetentionType(str, Enum):
+    MODIFIABLE = 'modifiable'
+    NON_MODIFIABLE = 'non_modifiable'
+
+
+class RetentionPoliciesManager:
     def __init__(
         self,
         *,
         auth: Optional[Authentication] = None,
         network_session: NetworkSession = None
     ):
         if network_session is None:
             network_session = NetworkSession()
         self.auth = auth
         self.network_session = network_session
 
-    def get_legal_hold_policy_assignments(
+    def get_retention_policies(
         self,
-        policy_id: str,
         *,
-        assign_to_type: Optional[GetLegalHoldPolicyAssignmentsAssignToType] = None,
-        assign_to_id: Optional[str] = None,
-        marker: Optional[str] = None,
-        limit: Optional[int] = None,
+        policy_name: Optional[str] = None,
+        policy_type: Optional[GetRetentionPoliciesPolicyType] = None,
+        created_by_user_id: Optional[str] = None,
         fields: Optional[List[str]] = None,
+        limit: Optional[int] = None,
+        marker: Optional[str] = None,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> LegalHoldPolicyAssignments:
+    ) -> RetentionPolicies:
         """
-                Retrieves a list of items a legal hold policy has been assigned to.
-                :param policy_id: The ID of the legal hold policy
-                :type policy_id: str
-                :param assign_to_type: Filters the results by the type of item the
-        policy was applied to., defaults to None
-                :type assign_to_type: Optional[GetLegalHoldPolicyAssignmentsAssignToType], optional
-                :param assign_to_id: Filters the results by the ID of item the
-        policy was applied to., defaults to None
-                :type assign_to_id: Optional[str], optional
-                :param marker: Defines the position marker at which to begin returning results. This is
-        used when paginating using marker-based pagination.
-
-        This requires `usemarker` to be set to `true`., defaults to None
-                :type marker: Optional[str], optional
-                :param limit: The maximum number of items to return per page., defaults to None
-                :type limit: Optional[int], optional
+                Retrieves all of the retention policies for an enterprise.
+                :param policy_name: Filters results by a case sensitive prefix of the name of
+        retention policies., defaults to None
+                :type policy_name: Optional[str], optional
+                :param policy_type: Filters results by the type of retention policy., defaults to None
+                :type policy_type: Optional[GetRetentionPoliciesPolicyType], optional
+                :param created_by_user_id: Filters results by the ID of the user who created policy., defaults to None
+                :type created_by_user_id: Optional[str], optional
                 :param fields: A comma-separated list of attributes to include in the
         response. This can be used to request fields that are
         not normally returned in a standard response.
 
         Be aware that specifying this parameter will have the
         effect that none of the standard fields are returned in
         the response unless explicitly specified, instead only
         fields for the mini representation are returned, additional
         to the fields requested., defaults to None
                 :type fields: Optional[List[str]], optional
+                :param limit: The maximum number of items to return per page., defaults to None
+                :type limit: Optional[int], optional
+                :param marker: Defines the position marker at which to begin returning results. This is
+        used when paginating using marker-based pagination., defaults to None
+                :type marker: Optional[str], optional
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params(
             {
-                'policy_id': to_string(policy_id),
-                'assign_to_type': to_string(assign_to_type),
-                'assign_to_id': to_string(assign_to_id),
-                'marker': to_string(marker),
-                'limit': to_string(limit),
+                'policy_name': to_string(policy_name),
+                'policy_type': to_string(policy_type),
+                'created_by_user_id': to_string(created_by_user_id),
                 'fields': to_string(fields),
+                'limit': to_string(limit),
+                'marker': to_string(marker),
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [
-                    self.network_session.base_urls.base_url,
-                    '/legal_hold_policy_assignments',
-                ]
+                [self.network_session.base_urls.base_url, '/2.0/retention_policies']
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return deserialize(response.data, LegalHoldPolicyAssignments)
+        return deserialize(response.data, RetentionPolicies)
 
-    def create_legal_hold_policy_assignment(
+    def create_retention_policy(
         self,
-        policy_id: str,
-        assign_to: CreateLegalHoldPolicyAssignmentAssignTo,
+        policy_name: str,
+        policy_type: CreateRetentionPolicyPolicyType,
+        disposition_action: CreateRetentionPolicyDispositionAction,
         *,
+        description: Optional[str] = None,
+        retention_length: Optional[str] = None,
+        retention_type: Optional[CreateRetentionPolicyRetentionType] = None,
+        can_owner_extend_retention: Optional[bool] = None,
+        are_owners_notified: Optional[bool] = None,
+        custom_notification_recipients: Optional[List[UserMini]] = None,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> LegalHoldPolicyAssignment:
+    ) -> RetentionPolicy:
         """
-        Assign a legal hold to a file, file version, folder, or user.
-        :param policy_id: The ID of the policy to assign.
-        :type policy_id: str
-        :param assign_to: The item to assign the policy to
-        :type assign_to: CreateLegalHoldPolicyAssignmentAssignTo
-        :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
-        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+                Creates a retention policy.
+                :param policy_name: The name for the retention policy
+                :type policy_name: str
+                :param policy_type: The type of the retention policy. A retention
+        policy type can either be `finite`, where a
+        specific amount of time to retain the content is known
+        upfront, or `indefinite`, where the amount of time
+        to retain the content is still unknown.
+                :type policy_type: CreateRetentionPolicyPolicyType
+                :param disposition_action: The disposition action of the retention policy.
+        `permanently_delete` deletes the content
+        retained by the policy permanently.
+        `remove_retention` lifts retention policy
+        from the content, allowing it to be deleted
+        by users once the retention policy has expired.
+                :type disposition_action: CreateRetentionPolicyDispositionAction
+                :param description: The additional text description of the retention policy., defaults to None
+                :type description: Optional[str], optional
+                :param retention_length: The length of the retention policy. This value
+        specifies the duration in days that the retention
+        policy will be active for after being assigned to
+        content.  If the policy has a `policy_type` of
+        `indefinite`, the `retention_length` will also be
+        `indefinite`., defaults to None
+                :type retention_length: Optional[str], optional
+                :param retention_type: Specifies the retention type:
+
+        * `modifiable`: You can modify the retention policy. For example,
+        you can add or remove folders, shorten or lengthen
+        the policy duration, or delete the assignment.
+        Use this type if your retention policy
+        is not related to any regulatory purposes.
+
+        * `non_modifiable`: You can modify the retention policy
+        only in a limited way: add a folder, lengthen the duration,
+        retire the policy, change the disposition action
+        or notification settings. You cannot perform other actions,
+        such as deleting the assignment or shortening the
+        policy duration. Use this type to ensure
+        compliance with regulatory retention policies., defaults to None
+                :type retention_type: Optional[CreateRetentionPolicyRetentionType], optional
+                :param can_owner_extend_retention: Whether the owner of a file will be allowed to
+        extend the retention., defaults to None
+                :type can_owner_extend_retention: Optional[bool], optional
+                :param are_owners_notified: Whether owner and co-owners of a file are notified
+        when the policy nears expiration., defaults to None
+                :type are_owners_notified: Optional[bool], optional
+                :param custom_notification_recipients: A list of users notified when
+        the retention policy duration is about to end., defaults to None
+                :type custom_notification_recipients: Optional[List[UserMini]], optional
+                :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
+                :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
-        request_body: Dict = {'policy_id': policy_id, 'assign_to': assign_to}
+        request_body: Dict = {
+            'policy_name': policy_name,
+            'description': description,
+            'policy_type': policy_type,
+            'disposition_action': disposition_action,
+            'retention_length': retention_length,
+            'retention_type': retention_type,
+            'can_owner_extend_retention': can_owner_extend_retention,
+            'are_owners_notified': are_owners_notified,
+            'custom_notification_recipients': custom_notification_recipients,
+        }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [
-                    self.network_session.base_urls.base_url,
-                    '/legal_hold_policy_assignments',
-                ]
+                [self.network_session.base_urls.base_url, '/2.0/retention_policies']
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return deserialize(response.data, LegalHoldPolicyAssignment)
+        return deserialize(response.data, RetentionPolicy)
 
-    def get_legal_hold_policy_assignment_by_id(
+    def get_retention_policy_by_id(
         self,
-        legal_hold_policy_assignment_id: str,
+        retention_policy_id: str,
         *,
+        fields: Optional[List[str]] = None,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> LegalHoldPolicyAssignment:
+    ) -> RetentionPolicy:
         """
-                Retrieve a legal hold policy assignment.
-                :param legal_hold_policy_assignment_id: The ID of the legal hold policy assignment
-        Example: "753465"
-                :type legal_hold_policy_assignment_id: str
+                Retrieves a retention policy.
+                :param retention_policy_id: The ID of the retention policy.
+        Example: "982312"
+                :type retention_policy_id: str
+                :param fields: A comma-separated list of attributes to include in the
+        response. This can be used to request fields that are
+        not normally returned in a standard response.
+
+        Be aware that specifying this parameter will have the
+        effect that none of the standard fields are returned in
+        the response unless explicitly specified, instead only
+        fields for the mini representation are returned, additional
+        to the fields requested., defaults to None
+                :type fields: Optional[List[str]], optional
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
+        query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/legal_hold_policy_assignments/',
-                    to_string(legal_hold_policy_assignment_id),
+                    '/2.0/retention_policies/',
+                    to_string(retention_policy_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
+                params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return deserialize(response.data, LegalHoldPolicyAssignment)
+        return deserialize(response.data, RetentionPolicy)
 
-    def delete_legal_hold_policy_assignment_by_id(
+    def update_retention_policy_by_id(
         self,
-        legal_hold_policy_assignment_id: str,
+        retention_policy_id: str,
         *,
+        policy_name: Optional[str] = None,
+        description: Optional[str] = None,
+        disposition_action: Optional[str] = None,
+        retention_type: Optional[str] = None,
+        retention_length: Optional[str] = None,
+        status: Optional[str] = None,
+        can_owner_extend_retention: Optional[bool] = None,
+        are_owners_notified: Optional[bool] = None,
+        custom_notification_recipients: Optional[List[UserBase]] = None,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> None:
+    ) -> RetentionPolicy:
         """
-                Remove a legal hold from an item.
-
-                This is an asynchronous process. The policy will not be
-
-
-                fully removed yet when the response returns.
-
-                :param legal_hold_policy_assignment_id: The ID of the legal hold policy assignment
-        Example: "753465"
-                :type legal_hold_policy_assignment_id: str
-                :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
-                :type extra_headers: Optional[Dict[str, Optional[str]]], optional
-        """
-        if extra_headers is None:
-            extra_headers = {}
-        headers_map: Dict[str, str] = prepare_params({**extra_headers})
-        response: FetchResponse = fetch(
-            ''.join(
-                [
-                    self.network_session.base_urls.base_url,
-                    '/legal_hold_policy_assignments/',
-                    to_string(legal_hold_policy_assignment_id),
-                ]
-            ),
-            FetchOptions(
-                method='DELETE',
-                headers=headers_map,
-                response_format=None,
-                auth=self.auth,
-                network_session=self.network_session,
-            ),
-        )
-        return None
-
-    def get_legal_hold_policy_assignment_file_on_hold(
-        self,
-        legal_hold_policy_assignment_id: str,
-        *,
-        marker: Optional[str] = None,
-        limit: Optional[int] = None,
-        fields: Optional[List[str]] = None,
-        extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> FileVersionLegalHolds:
-        """
-                Get a list of current file versions for a legal hold
-
-                assignment.
-
-
-                In some cases you may want to get previous file versions instead. In these
-
-
-                cases, use the `GET  /legal_hold_policy_assignments/:id/file_versions_on_hold`
-
-
-                API instead to return any previous versions of a file for this legal hold
-
-
-                policy assignment.
-
-
-                Due to ongoing re-architecture efforts this API might not return all file
-
-
-                versions held for this policy ID. Instead, this API will only return the
-
-
-                latest file version held in the newly developed architecture. The `GET
-
-
-                /file_version_legal_holds` API can be used to fetch current and past versions
-
-
-                of files held within the legacy architecture.
-
-
-                The `GET /legal_hold_policy_assignments?policy_id={id}` API can be used to
-
-
-                find a list of policy assignments for a given policy ID.
-
-                :param legal_hold_policy_assignment_id: The ID of the legal hold policy assignment
-        Example: "753465"
-                :type legal_hold_policy_assignment_id: str
-                :param marker: Defines the position marker at which to begin returning results. This is
-        used when paginating using marker-based pagination.
-
-        This requires `usemarker` to be set to `true`., defaults to None
-                :type marker: Optional[str], optional
-                :param limit: The maximum number of items to return per page., defaults to None
-                :type limit: Optional[int], optional
-                :param fields: A comma-separated list of attributes to include in the
-        response. This can be used to request fields that are
-        not normally returned in a standard response.
-
-        Be aware that specifying this parameter will have the
-        effect that none of the standard fields are returned in
-        the response unless explicitly specified, instead only
-        fields for the mini representation are returned, additional
-        to the fields requested., defaults to None
-                :type fields: Optional[List[str]], optional
+                Updates a retention policy.
+                :param retention_policy_id: The ID of the retention policy.
+        Example: "982312"
+                :type retention_policy_id: str
+                :param policy_name: The name for the retention policy, defaults to None
+                :type policy_name: Optional[str], optional
+                :param description: The additional text description of the retention policy., defaults to None
+                :type description: Optional[str], optional
+                :param disposition_action: The disposition action of the retention policy.
+        This action can be `permanently_delete`, which
+        will cause the content retained by the policy
+        to be permanently deleted, or `remove_retention`,
+        which will lift the retention policy from the content,
+        allowing it to be deleted by users,
+        once the retention policy has expired.
+        You can use "null" if you don't want to change `disposition_action`., defaults to None
+                :type disposition_action: Optional[str], optional
+                :param retention_type: Specifies the retention type:
+
+        * `modifiable`: You can modify the retention policy. For example,
+        you can add or remove folders, shorten or lengthen
+        the policy duration, or delete the assignment.
+        Use this type if your retention policy
+        is not related to any regulatory purposes.
+        * `non-modifiable`: You can modify the retention policy
+        only in a limited way: add a folder, lengthen the duration,
+        retire the policy, change the disposition action
+        or notification settings. You cannot perform other actions,
+        such as deleting the assignment or shortening the
+        policy duration. Use this type to ensure
+        compliance with regulatory retention policies.
+
+        When updating a retention policy, you can use
+        `non-modifiable` type only. You can convert a
+        `modifiable` policy to `non-modifiable`, but
+        not the other way around., defaults to None
+                :type retention_type: Optional[str], optional
+                :param retention_length: The length of the retention policy. This value
+        specifies the duration in days that the retention
+        policy will be active for after being assigned to
+        content.  If the policy has a `policy_type` of
+        `indefinite`, the `retention_length` will also be
+        `indefinite`., defaults to None
+                :type retention_length: Optional[str], optional
+                :param status: Used to retire a retention policy.
+
+        If not retiring a policy, do not include this parameter
+        or set it to `null`., defaults to None
+                :type status: Optional[str], optional
+                :param can_owner_extend_retention: Determines if the owner of items under the policy
+        can extend the retention when the original retention
+        duration is about to end., defaults to None
+                :type can_owner_extend_retention: Optional[bool], optional
+                :param are_owners_notified: Determines if owners and co-owners of items
+        under the policy are notified when
+        the retention duration is about to end., defaults to None
+                :type are_owners_notified: Optional[bool], optional
+                :param custom_notification_recipients: A list of users notified when the retention duration is about to end., defaults to None
+                :type custom_notification_recipients: Optional[List[UserBase]], optional
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
-        query_params_map: Dict[str, str] = prepare_params(
-            {
-                'marker': to_string(marker),
-                'limit': to_string(limit),
-                'fields': to_string(fields),
-            }
-        )
+        request_body: Dict = {
+            'policy_name': policy_name,
+            'description': description,
+            'disposition_action': disposition_action,
+            'retention_type': retention_type,
+            'retention_length': retention_length,
+            'status': status,
+            'can_owner_extend_retention': can_owner_extend_retention,
+            'are_owners_notified': are_owners_notified,
+            'custom_notification_recipients': custom_notification_recipients,
+        }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/legal_hold_policy_assignments/',
-                    to_string(legal_hold_policy_assignment_id),
-                    '/files_on_hold',
+                    '/2.0/retention_policies/',
+                    to_string(retention_policy_id),
                 ]
             ),
             FetchOptions(
-                method='GET',
-                params=query_params_map,
+                method='PUT',
                 headers=headers_map,
+                data=serialize(request_body),
+                content_type='application/json',
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return deserialize(response.data, FileVersionLegalHolds)
+        return deserialize(response.data, RetentionPolicy)
 
-    def get_legal_hold_policy_assignment_file_version_on_hold(
+    def delete_retention_policy_by_id(
         self,
-        legal_hold_policy_assignment_id: str,
+        retention_policy_id: str,
         *,
-        marker: Optional[str] = None,
-        limit: Optional[int] = None,
-        fields: Optional[List[str]] = None,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> FileVersionLegalHolds:
+    ) -> None:
         """
-                Get a list of previous file versions for a legal hold
-
-                assignment.
-
-
-                In some cases you may only need the latest file versions instead. In these
-
-
-                cases, use the `GET  /legal_hold_policy_assignments/:id/files_on_hold` API
-
-
-                instead to return any current (latest) versions of a file for this legal hold
-
-
-                policy assignment.
-
-
-                Due to ongoing re-architecture efforts this API might not return all files
-
-
-                held for this policy ID. Instead, this API will only return past file versions
-
-
-                held in the newly developed architecture. The `GET /file_version_legal_holds`
-
-
-                API can be used to fetch current and past versions of files held within the
-
-
-                legacy architecture.
-
-
-                The `GET /legal_hold_policy_assignments?policy_id={id}` API can be used to
-
-
-                find a list of policy assignments for a given policy ID.
-
-                :param legal_hold_policy_assignment_id: The ID of the legal hold policy assignment
-        Example: "753465"
-                :type legal_hold_policy_assignment_id: str
-                :param marker: Defines the position marker at which to begin returning results. This is
-        used when paginating using marker-based pagination.
-
-        This requires `usemarker` to be set to `true`., defaults to None
-                :type marker: Optional[str], optional
-                :param limit: The maximum number of items to return per page., defaults to None
-                :type limit: Optional[int], optional
-                :param fields: A comma-separated list of attributes to include in the
-        response. This can be used to request fields that are
-        not normally returned in a standard response.
-
-        Be aware that specifying this parameter will have the
-        effect that none of the standard fields are returned in
-        the response unless explicitly specified, instead only
-        fields for the mini representation are returned, additional
-        to the fields requested., defaults to None
-                :type fields: Optional[List[str]], optional
+                Permanently deletes a retention policy.
+                :param retention_policy_id: The ID of the retention policy.
+        Example: "982312"
+                :type retention_policy_id: str
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
-        query_params_map: Dict[str, str] = prepare_params(
-            {
-                'marker': to_string(marker),
-                'limit': to_string(limit),
-                'fields': to_string(fields),
-            }
-        )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/legal_hold_policy_assignments/',
-                    to_string(legal_hold_policy_assignment_id),
-                    '/file_versions_on_hold',
+                    '/2.0/retention_policies/',
+                    to_string(retention_policy_id),
                 ]
             ),
             FetchOptions(
-                method='GET',
-                params=query_params_map,
+                method='DELETE',
                 headers=headers_map,
-                response_format='json',
+                response_format=None,
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return deserialize(response.data, FileVersionLegalHolds)
+        return None
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/list_collaborations.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/list_collaborations.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 from typing import Dict
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import Collaborations
+from box_sdk_gen.schemas.collaborations import Collaborations
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -107,15 +107,15 @@
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/collaborations',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
@@ -168,15 +168,15 @@
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                     '/collaborations',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
@@ -230,15 +230,15 @@
                 'fields': to_string(fields),
                 'offset': to_string(offset),
                 'limit': to_string(limit),
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/collaborations']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/collaborations']),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
@@ -285,15 +285,15 @@
             {'limit': to_string(limit), 'offset': to_string(offset)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/groups/',
+                    '/2.0/groups/',
                     to_string(group_id),
                     '/collaborations',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/memberships.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/memberships.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from typing import List
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import GroupMemberships
+from box_sdk_gen.schemas.group_memberships import GroupMemberships
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import GroupMembership
+from box_sdk_gen.schemas.group_membership import GroupMembership
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -119,15 +119,15 @@
             {'limit': to_string(limit), 'offset': to_string(offset)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/users/',
+                    '/2.0/users/',
                     to_string(user_id),
                     '/memberships',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
@@ -175,15 +175,15 @@
             {'limit': to_string(limit), 'offset': to_string(offset)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/groups/',
+                    '/2.0/groups/',
                     to_string(group_id),
                     '/memberships',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
@@ -247,15 +247,17 @@
             'group': group,
             'role': role,
             'configurable_permissions': configurable_permissions,
         }
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/group_memberships']),
+            ''.join(
+                [self.network_session.base_urls.base_url, '/2.0/group_memberships']
+            ),
             FetchOptions(
                 method='POST',
                 params=query_params_map,
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
@@ -300,15 +302,15 @@
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/group_memberships/',
+                    '/2.0/group_memberships/',
                     to_string(group_membership_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
@@ -373,15 +375,15 @@
         }
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/group_memberships/',
+                    '/2.0/group_memberships/',
                     to_string(group_membership_id),
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 params=query_params_map,
                 headers=headers_map,
@@ -417,15 +419,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/group_memberships/',
+                    '/2.0/group_memberships/',
                     to_string(group_membership_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/metadata_cascade_policies.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/metadata_cascade_policies.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import MetadataCascadePolicies
+from box_sdk_gen.schemas.metadata_cascade_policies import MetadataCascadePolicies
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import MetadataCascadePolicy
+from box_sdk_gen.schemas.metadata_cascade_policy import MetadataCascadePolicy
 
-from box_sdk_gen.schemas import ConflictError
+from box_sdk_gen.schemas.conflict_error import ConflictError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -108,15 +108,18 @@
                 'marker': to_string(marker),
                 'offset': to_string(offset),
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/metadata_cascade_policies']
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/metadata_cascade_policies',
+                ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
@@ -179,15 +182,18 @@
             'folder_id': folder_id,
             'scope': scope,
             'templateKey': template_key,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/metadata_cascade_policies']
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/metadata_cascade_policies',
+                ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
@@ -214,15 +220,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/metadata_cascade_policies/',
+                    '/2.0/metadata_cascade_policies/',
                     to_string(metadata_cascade_policy_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
@@ -249,15 +255,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/metadata_cascade_policies/',
+                    '/2.0/metadata_cascade_policies/',
                     to_string(metadata_cascade_policy_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
@@ -303,15 +309,15 @@
             extra_headers = {}
         request_body: Dict = {'conflict_resolution': conflict_resolution}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/metadata_cascade_policies/',
+                    '/2.0/metadata_cascade_policies/',
                     to_string(metadata_cascade_policy_id),
                     '/apply',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/metadata_templates.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/metadata_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import MetadataTemplates
+from box_sdk_gen.schemas.metadata_templates import MetadataTemplates
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import MetadataTemplate
+from box_sdk_gen.schemas.metadata_template import MetadataTemplate
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -247,15 +247,17 @@
         if extra_headers is None:
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params(
             {'metadata_instance_id': to_string(metadata_instance_id)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/metadata_templates']),
+            ''.join(
+                [self.network_session.base_urls.base_url, '/2.0/metadata_templates']
+            ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
@@ -290,15 +292,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/metadata_templates/',
+                    '/2.0/metadata_templates/',
                     to_string(scope),
                     '/',
                     to_string(template_key),
                     '/schema',
                 ]
             ),
             FetchOptions(
@@ -347,15 +349,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/metadata_templates/',
+                    '/2.0/metadata_templates/',
                     to_string(scope),
                     '/',
                     to_string(template_key),
                     '/schema',
                 ]
             ),
             FetchOptions(
@@ -394,15 +396,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/metadata_templates/',
+                    '/2.0/metadata_templates/',
                     to_string(scope),
                     '/',
                     to_string(template_key),
                     '/schema',
                 ]
             ),
             FetchOptions(
@@ -432,15 +434,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/metadata_templates/',
+                    '/2.0/metadata_templates/',
                     to_string(template_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
@@ -476,15 +478,18 @@
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params(
             {'marker': to_string(marker), 'limit': to_string(limit)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/metadata_templates/global']
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/metadata_templates/global',
+                ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
@@ -521,15 +526,15 @@
             {'marker': to_string(marker), 'limit': to_string(limit)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/metadata_templates/enterprise',
+                    '/2.0/metadata_templates/enterprise',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
@@ -594,15 +599,18 @@
             'hidden': hidden,
             'fields': fields,
             'copyInstanceOnItemCopy': copy_instance_on_item_copy,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/metadata_templates/schema']
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/metadata_templates/schema',
+                ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/recent_items.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/recent_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 from typing import Dict
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import RecentItems
+from box_sdk_gen.schemas.recent_items import RecentItems
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -88,15 +88,15 @@
                 'fields': to_string(fields),
                 'limit': to_string(limit),
                 'marker': to_string(marker),
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/recent_items']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/recent_items']),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/retention_policies.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/retention_policy_assignments.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from enum import Enum
 
 from typing import Optional
 
+from box_sdk_gen.internal.base_object import BaseObject
+
 from typing import List
 
 from typing import Dict
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import RetentionPolicies
-
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.retention_policy_assignments import RetentionPolicyAssignments
 
-from box_sdk_gen.schemas import RetentionPolicy
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import UserMini
+from box_sdk_gen.schemas.retention_policy_assignment import RetentionPolicyAssignment
 
-from box_sdk_gen.schemas import UserBase
+from box_sdk_gen.schemas.files_under_retention import FilesUnderRetention
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -39,218 +39,216 @@
 from box_sdk_gen.networking.fetch import FetchResponse
 
 from box_sdk_gen.networking.fetch import fetch
 
 from box_sdk_gen.serialization.json.json_data import SerializedData
 
 
-class GetRetentionPoliciesPolicyType(str, Enum):
-    FINITE = 'finite'
-    INDEFINITE = 'indefinite'
+class GetRetentionPolicyAssignmentsType(str, Enum):
+    FOLDER = 'folder'
+    ENTERPRISE = 'enterprise'
+    METADATA_TEMPLATE = 'metadata_template'
+
 
+class CreateRetentionPolicyAssignmentAssignToTypeField(str, Enum):
+    ENTERPRISE = 'enterprise'
+    FOLDER = 'folder'
+    METADATA_TEMPLATE = 'metadata_template'
 
-class CreateRetentionPolicyPolicyType(str, Enum):
-    FINITE = 'finite'
-    INDEFINITE = 'indefinite'
 
+class CreateRetentionPolicyAssignmentAssignTo(BaseObject):
+    _discriminator = 'type', {'enterprise', 'folder', 'metadata_template'}
 
-class CreateRetentionPolicyDispositionAction(str, Enum):
-    PERMANENTLY_DELETE = 'permanently_delete'
-    REMOVE_RETENTION = 'remove_retention'
+    def __init__(
+        self,
+        type: CreateRetentionPolicyAssignmentAssignToTypeField,
+        *,
+        id: Optional[str] = None,
+        **kwargs
+    ):
+        """
+                :param type: The type of item to assign the policy to.
+                :type type: CreateRetentionPolicyAssignmentAssignToTypeField
+                :param id: The ID of item to assign the policy to.
+        Set to `null` or omit when `type` is set to
+        `enterprise`., defaults to None
+                :type id: Optional[str], optional
+        """
+        super().__init__(**kwargs)
+        self.type = type
+        self.id = id
 
 
-class CreateRetentionPolicyRetentionType(str, Enum):
-    MODIFIABLE = 'modifiable'
-    NON_MODIFIABLE = 'non_modifiable'
+class CreateRetentionPolicyAssignmentFilterFields(BaseObject):
+    def __init__(
+        self, *, field: Optional[str] = None, value: Optional[str] = None, **kwargs
+    ):
+        """
+                :param field: The metadata attribute key id., defaults to None
+                :type field: Optional[str], optional
+                :param value: The metadata attribute field id. For value, only
+        enum and multiselect types are supported., defaults to None
+                :type value: Optional[str], optional
+        """
+        super().__init__(**kwargs)
+        self.field = field
+        self.value = value
 
 
-class RetentionPoliciesManager:
+class RetentionPolicyAssignmentsManager:
     def __init__(
         self,
         *,
         auth: Optional[Authentication] = None,
         network_session: NetworkSession = None
     ):
         if network_session is None:
             network_session = NetworkSession()
         self.auth = auth
         self.network_session = network_session
 
-    def get_retention_policies(
+    def get_retention_policy_assignments(
         self,
+        retention_policy_id: str,
         *,
-        policy_name: Optional[str] = None,
-        policy_type: Optional[GetRetentionPoliciesPolicyType] = None,
-        created_by_user_id: Optional[str] = None,
+        type: Optional[GetRetentionPolicyAssignmentsType] = None,
         fields: Optional[List[str]] = None,
-        limit: Optional[int] = None,
         marker: Optional[str] = None,
+        limit: Optional[int] = None,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> RetentionPolicies:
+    ) -> RetentionPolicyAssignments:
         """
-                Retrieves all of the retention policies for an enterprise.
-                :param policy_name: Filters results by a case sensitive prefix of the name of
-        retention policies., defaults to None
-                :type policy_name: Optional[str], optional
-                :param policy_type: Filters results by the type of retention policy., defaults to None
-                :type policy_type: Optional[GetRetentionPoliciesPolicyType], optional
-                :param created_by_user_id: Filters results by the ID of the user who created policy., defaults to None
-                :type created_by_user_id: Optional[str], optional
+                Returns a list of all retention policy assignments associated with a specified
+
+                retention policy.
+
+                :param retention_policy_id: The ID of the retention policy.
+        Example: "982312"
+                :type retention_policy_id: str
+                :param type: The type of the retention policy assignment to retrieve., defaults to None
+                :type type: Optional[GetRetentionPolicyAssignmentsType], optional
                 :param fields: A comma-separated list of attributes to include in the
         response. This can be used to request fields that are
         not normally returned in a standard response.
 
         Be aware that specifying this parameter will have the
         effect that none of the standard fields are returned in
         the response unless explicitly specified, instead only
         fields for the mini representation are returned, additional
         to the fields requested., defaults to None
                 :type fields: Optional[List[str]], optional
-                :param limit: The maximum number of items to return per page., defaults to None
-                :type limit: Optional[int], optional
                 :param marker: Defines the position marker at which to begin returning results. This is
         used when paginating using marker-based pagination., defaults to None
                 :type marker: Optional[str], optional
+                :param limit: The maximum number of items to return per page., defaults to None
+                :type limit: Optional[int], optional
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params(
             {
-                'policy_name': to_string(policy_name),
-                'policy_type': to_string(policy_type),
-                'created_by_user_id': to_string(created_by_user_id),
+                'type': to_string(type),
                 'fields': to_string(fields),
-                'limit': to_string(limit),
                 'marker': to_string(marker),
+                'limit': to_string(limit),
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/retention_policies']),
+            ''.join(
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/retention_policies/',
+                    to_string(retention_policy_id),
+                    '/assignments',
+                ]
+            ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return deserialize(response.data, RetentionPolicies)
+        return deserialize(response.data, RetentionPolicyAssignments)
 
-    def create_retention_policy(
+    def create_retention_policy_assignment(
         self,
-        policy_name: str,
-        policy_type: CreateRetentionPolicyPolicyType,
-        disposition_action: CreateRetentionPolicyDispositionAction,
+        policy_id: str,
+        assign_to: CreateRetentionPolicyAssignmentAssignTo,
         *,
-        description: Optional[str] = None,
-        retention_length: Optional[str] = None,
-        retention_type: Optional[CreateRetentionPolicyRetentionType] = None,
-        can_owner_extend_retention: Optional[bool] = None,
-        are_owners_notified: Optional[bool] = None,
-        custom_notification_recipients: Optional[List[UserMini]] = None,
+        filter_fields: Optional[
+            List[CreateRetentionPolicyAssignmentFilterFields]
+        ] = None,
+        start_date_field: Optional[str] = None,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> RetentionPolicy:
+    ) -> RetentionPolicyAssignment:
         """
-                Creates a retention policy.
-                :param policy_name: The name for the retention policy
-                :type policy_name: str
-                :param policy_type: The type of the retention policy. A retention
-        policy type can either be `finite`, where a
-        specific amount of time to retain the content is known
-        upfront, or `indefinite`, where the amount of time
-        to retain the content is still unknown.
-                :type policy_type: CreateRetentionPolicyPolicyType
-                :param disposition_action: The disposition action of the retention policy.
-        `permanently_delete` deletes the content
-        retained by the policy permanently.
-        `remove_retention` lifts retention policy
-        from the content, allowing it to be deleted
-        by users once the retention policy has expired.
-                :type disposition_action: CreateRetentionPolicyDispositionAction
-                :param description: The additional text description of the retention policy., defaults to None
-                :type description: Optional[str], optional
-                :param retention_length: The length of the retention policy. This value
-        specifies the duration in days that the retention
-        policy will be active for after being assigned to
-        content.  If the policy has a `policy_type` of
-        `indefinite`, the `retention_length` will also be
-        `indefinite`., defaults to None
-                :type retention_length: Optional[str], optional
-                :param retention_type: Specifies the retention type:
-
-        * `modifiable`: You can modify the retention policy. For example,
-        you can add or remove folders, shorten or lengthen
-        the policy duration, or delete the assignment.
-        Use this type if your retention policy
-        is not related to any regulatory purposes.
-
-        * `non_modifiable`: You can modify the retention policy
-        only in a limited way: add a folder, lengthen the duration,
-        retire the policy, change the disposition action
-        or notification settings. You cannot perform other actions,
-        such as deleting the assignment or shortening the
-        policy duration. Use this type to ensure
-        compliance with regulatory retention policies., defaults to None
-                :type retention_type: Optional[CreateRetentionPolicyRetentionType], optional
-                :param can_owner_extend_retention: Whether the owner of a file will be allowed to
-        extend the retention., defaults to None
-                :type can_owner_extend_retention: Optional[bool], optional
-                :param are_owners_notified: Whether owner and co-owners of a file are notified
-        when the policy nears expiration., defaults to None
-                :type are_owners_notified: Optional[bool], optional
-                :param custom_notification_recipients: A list of users notified when
-        the retention policy duration is about to end., defaults to None
-                :type custom_notification_recipients: Optional[List[UserMini]], optional
+                Assigns a retention policy to an item.
+                :param policy_id: The ID of the retention policy to assign
+                :type policy_id: str
+                :param assign_to: The item to assign the policy to
+                :type assign_to: CreateRetentionPolicyAssignmentAssignTo
+                :param filter_fields: If the `assign_to` type is `metadata_template`,
+        then optionally add the `filter_fields` parameter which will
+        require an array of objects with a field entry and a value entry.
+        Currently only one object of `field` and `value` is supported., defaults to None
+                :type filter_fields: Optional[List[CreateRetentionPolicyAssignmentFilterFields]], optional
+                :param start_date_field: The date the retention policy assignment begins.
+
+        If the `assigned_to` type is `metadata_template`,
+        this field can be a date field's metadata attribute key id., defaults to None
+                :type start_date_field: Optional[str], optional
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         request_body: Dict = {
-            'policy_name': policy_name,
-            'description': description,
-            'policy_type': policy_type,
-            'disposition_action': disposition_action,
-            'retention_length': retention_length,
-            'retention_type': retention_type,
-            'can_owner_extend_retention': can_owner_extend_retention,
-            'are_owners_notified': are_owners_notified,
-            'custom_notification_recipients': custom_notification_recipients,
+            'policy_id': policy_id,
+            'assign_to': assign_to,
+            'filter_fields': filter_fields,
+            'start_date_field': start_date_field,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/retention_policies']),
+            ''.join(
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/retention_policy_assignments',
+                ]
+            ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return deserialize(response.data, RetentionPolicy)
+        return deserialize(response.data, RetentionPolicyAssignment)
 
-    def get_retention_policy_by_id(
+    def get_retention_policy_assignment_by_id(
         self,
-        retention_policy_id: str,
+        retention_policy_assignment_id: str,
         *,
         fields: Optional[List[str]] = None,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> RetentionPolicy:
+    ) -> RetentionPolicyAssignment:
         """
-                Retrieves a retention policy.
-                :param retention_policy_id: The ID of the retention policy.
-        Example: "982312"
-                :type retention_policy_id: str
+                Retrieves a retention policy assignment
+                :param retention_policy_assignment_id: The ID of the retention policy assignment.
+        Example: "1233123"
+                :type retention_policy_assignment_id: str
                 :param fields: A comma-separated list of attributes to include in the
         response. This can be used to request fields that are
         not normally returned in a standard response.
 
         Be aware that specifying this parameter will have the
         effect that none of the standard fields are returned in
         the response unless explicitly specified, instead only
@@ -264,168 +262,108 @@
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/retention_policies/',
-                    to_string(retention_policy_id),
+                    '/2.0/retention_policy_assignments/',
+                    to_string(retention_policy_assignment_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return deserialize(response.data, RetentionPolicy)
+        return deserialize(response.data, RetentionPolicyAssignment)
 
-    def update_retention_policy_by_id(
+    def delete_retention_policy_assignment_by_id(
         self,
-        retention_policy_id: str,
+        retention_policy_assignment_id: str,
         *,
-        policy_name: Optional[str] = None,
-        description: Optional[str] = None,
-        disposition_action: Optional[str] = None,
-        retention_type: Optional[str] = None,
-        retention_length: Optional[str] = None,
-        status: Optional[str] = None,
-        can_owner_extend_retention: Optional[bool] = None,
-        are_owners_notified: Optional[bool] = None,
-        custom_notification_recipients: Optional[List[UserBase]] = None,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> RetentionPolicy:
+    ) -> None:
         """
-                Updates a retention policy.
-                :param retention_policy_id: The ID of the retention policy.
-        Example: "982312"
-                :type retention_policy_id: str
-                :param policy_name: The name for the retention policy, defaults to None
-                :type policy_name: Optional[str], optional
-                :param description: The additional text description of the retention policy., defaults to None
-                :type description: Optional[str], optional
-                :param disposition_action: The disposition action of the retention policy.
-        This action can be `permanently_delete`, which
-        will cause the content retained by the policy
-        to be permanently deleted, or `remove_retention`,
-        which will lift the retention policy from the content,
-        allowing it to be deleted by users,
-        once the retention policy has expired.
-        You can use "null" if you don't want to change `disposition_action`., defaults to None
-                :type disposition_action: Optional[str], optional
-                :param retention_type: Specifies the retention type:
-
-        * `modifiable`: You can modify the retention policy. For example,
-        you can add or remove folders, shorten or lengthen
-        the policy duration, or delete the assignment.
-        Use this type if your retention policy
-        is not related to any regulatory purposes.
-        * `non-modifiable`: You can modify the retention policy
-        only in a limited way: add a folder, lengthen the duration,
-        retire the policy, change the disposition action
-        or notification settings. You cannot perform other actions,
-        such as deleting the assignment or shortening the
-        policy duration. Use this type to ensure
-        compliance with regulatory retention policies.
-
-        When updating a retention policy, you can use
-        `non-modifiable` type only. You can convert a
-        `modifiable` policy to `non-modifiable`, but
-        not the other way around., defaults to None
-                :type retention_type: Optional[str], optional
-                :param retention_length: The length of the retention policy. This value
-        specifies the duration in days that the retention
-        policy will be active for after being assigned to
-        content.  If the policy has a `policy_type` of
-        `indefinite`, the `retention_length` will also be
-        `indefinite`., defaults to None
-                :type retention_length: Optional[str], optional
-                :param status: Used to retire a retention policy.
-
-        If not retiring a policy, do not include this parameter
-        or set it to `null`., defaults to None
-                :type status: Optional[str], optional
-                :param can_owner_extend_retention: Determines if the owner of items under the policy
-        can extend the retention when the original retention
-        duration is about to end., defaults to None
-                :type can_owner_extend_retention: Optional[bool], optional
-                :param are_owners_notified: Determines if owners and co-owners of items
-        under the policy are notified when
-        the retention duration is about to end., defaults to None
-                :type are_owners_notified: Optional[bool], optional
-                :param custom_notification_recipients: A list of users notified when the retention duration is about to end., defaults to None
-                :type custom_notification_recipients: Optional[List[UserBase]], optional
+                Removes a retention policy assignment
+
+                applied to content.
+
+                :param retention_policy_assignment_id: The ID of the retention policy assignment.
+        Example: "1233123"
+                :type retention_policy_assignment_id: str
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
-        request_body: Dict = {
-            'policy_name': policy_name,
-            'description': description,
-            'disposition_action': disposition_action,
-            'retention_type': retention_type,
-            'retention_length': retention_length,
-            'status': status,
-            'can_owner_extend_retention': can_owner_extend_retention,
-            'are_owners_notified': are_owners_notified,
-            'custom_notification_recipients': custom_notification_recipients,
-        }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/retention_policies/',
-                    to_string(retention_policy_id),
+                    '/2.0/retention_policy_assignments/',
+                    to_string(retention_policy_assignment_id),
                 ]
             ),
             FetchOptions(
-                method='PUT',
+                method='DELETE',
                 headers=headers_map,
-                data=serialize(request_body),
-                content_type='application/json',
-                response_format='json',
+                response_format=None,
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return deserialize(response.data, RetentionPolicy)
+        return None
 
-    def delete_retention_policy_by_id(
+    def get_files_under_retention_policy_assignment(
         self,
-        retention_policy_id: str,
+        retention_policy_assignment_id: str,
         *,
+        marker: Optional[str] = None,
+        limit: Optional[int] = None,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> None:
+    ) -> FilesUnderRetention:
         """
-                Permanently deletes a retention policy.
-                :param retention_policy_id: The ID of the retention policy.
-        Example: "982312"
-                :type retention_policy_id: str
+                Returns a list of files under retention for a retention policy assignment.
+                :param retention_policy_assignment_id: The ID of the retention policy assignment.
+        Example: "1233123"
+                :type retention_policy_assignment_id: str
+                :param marker: Defines the position marker at which to begin returning results. This is
+        used when paginating using marker-based pagination.
+
+        This requires `usemarker` to be set to `true`., defaults to None
+                :type marker: Optional[str], optional
+                :param limit: The maximum number of items to return per page., defaults to None
+                :type limit: Optional[int], optional
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
+        query_params_map: Dict[str, str] = prepare_params(
+            {'marker': to_string(marker), 'limit': to_string(limit)}
+        )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/retention_policies/',
-                    to_string(retention_policy_id),
+                    '/2.0/retention_policy_assignments/',
+                    to_string(retention_policy_assignment_id),
+                    '/files_under_retention',
                 ]
             ),
             FetchOptions(
-                method='DELETE',
+                method='GET',
+                params=query_params_map,
                 headers=headers_map,
-                response_format=None,
+                response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return None
+        return deserialize(response.data, FilesUnderRetention)
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/retention_policy_assignments.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/sign_requests.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,341 +1,195 @@
 from enum import Enum
 
 from typing import Optional
 
-from box_sdk_gen.internal.base_object import BaseObject
-
-from typing import List
-
 from typing import Dict
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
+from typing import List
+
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import RetentionPolicyAssignments
+from box_sdk_gen.schemas.file_base import FileBase
+
+from box_sdk_gen.schemas.sign_request_create_signer import SignRequestCreateSigner
+
+from box_sdk_gen.schemas.folder_mini import FolderMini
+
+from box_sdk_gen.schemas.sign_request_prefill_tag import SignRequestPrefillTag
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.sign_request import SignRequest
 
-from box_sdk_gen.schemas import RetentionPolicyAssignment
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import FilesUnderRetention
+from box_sdk_gen.schemas.sign_requests import SignRequests
+
+from box_sdk_gen.schemas.sign_request_create_request import SignRequestCreateRequest
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.internal.utils import ByteStream
 
-from box_sdk_gen.serialization.json.json_data import sd_to_json
-
 from box_sdk_gen.networking.fetch import FetchOptions
 
 from box_sdk_gen.networking.fetch import FetchResponse
 
 from box_sdk_gen.networking.fetch import fetch
 
-from box_sdk_gen.serialization.json.json_data import SerializedData
-
-
-class GetRetentionPolicyAssignmentsType(str, Enum):
-    FOLDER = 'folder'
-    ENTERPRISE = 'enterprise'
-    METADATA_TEMPLATE = 'metadata_template'
+from box_sdk_gen.serialization.json.json_data import sd_to_json
 
+from box_sdk_gen.serialization.json.json_data import SerializedData
 
-class CreateRetentionPolicyAssignmentAssignToTypeField(str, Enum):
-    ENTERPRISE = 'enterprise'
-    FOLDER = 'folder'
-    METADATA_TEMPLATE = 'metadata_template'
 
+class CreateSignRequestSignatureColor(str, Enum):
+    BLUE = 'blue'
+    BLACK = 'black'
+    RED = 'red'
 
-class CreateRetentionPolicyAssignmentAssignTo(BaseObject):
-    _discriminator = 'type', {'enterprise', 'folder', 'metadata_template'}
 
-    def __init__(
-        self,
-        type: CreateRetentionPolicyAssignmentAssignToTypeField,
-        *,
-        id: Optional[str] = None,
-        **kwargs
-    ):
-        """
-                :param type: The type of item to assign the policy to.
-                :type type: CreateRetentionPolicyAssignmentAssignToTypeField
-                :param id: The ID of item to assign the policy to.
-        Set to `null` or omit when `type` is set to
-        `enterprise`., defaults to None
-                :type id: Optional[str], optional
-        """
-        super().__init__(**kwargs)
-        self.type = type
-        self.id = id
-
-
-class CreateRetentionPolicyAssignmentFilterFields(BaseObject):
-    def __init__(
-        self, *, field: Optional[str] = None, value: Optional[str] = None, **kwargs
-    ):
-        """
-                :param field: The metadata attribute key id., defaults to None
-                :type field: Optional[str], optional
-                :param value: The metadata attribute field id. For value, only
-        enum and multiselect types are supported., defaults to None
-                :type value: Optional[str], optional
-        """
-        super().__init__(**kwargs)
-        self.field = field
-        self.value = value
-
-
-class RetentionPolicyAssignmentsManager:
+class SignRequestsManager:
     def __init__(
         self,
         *,
         auth: Optional[Authentication] = None,
         network_session: NetworkSession = None
     ):
         if network_session is None:
             network_session = NetworkSession()
         self.auth = auth
         self.network_session = network_session
 
-    def get_retention_policy_assignments(
+    def cancel_sign_request(
         self,
-        retention_policy_id: str,
+        sign_request_id: str,
         *,
-        type: Optional[GetRetentionPolicyAssignmentsType] = None,
-        fields: Optional[List[str]] = None,
-        marker: Optional[str] = None,
-        limit: Optional[int] = None,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> RetentionPolicyAssignments:
+    ) -> SignRequest:
         """
-                Returns a list of all retention policy assignments associated with a specified
-
-                retention policy.
-
-                :param retention_policy_id: The ID of the retention policy.
-        Example: "982312"
-                :type retention_policy_id: str
-                :param type: The type of the retention policy assignment to retrieve., defaults to None
-                :type type: Optional[GetRetentionPolicyAssignmentsType], optional
-                :param fields: A comma-separated list of attributes to include in the
-        response. This can be used to request fields that are
-        not normally returned in a standard response.
-
-        Be aware that specifying this parameter will have the
-        effect that none of the standard fields are returned in
-        the response unless explicitly specified, instead only
-        fields for the mini representation are returned, additional
-        to the fields requested., defaults to None
-                :type fields: Optional[List[str]], optional
-                :param marker: Defines the position marker at which to begin returning results. This is
-        used when paginating using marker-based pagination., defaults to None
-                :type marker: Optional[str], optional
-                :param limit: The maximum number of items to return per page., defaults to None
-                :type limit: Optional[int], optional
+                Cancels a sign request.
+                :param sign_request_id: The ID of the signature request
+        Example: "33243242"
+                :type sign_request_id: str
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
-        query_params_map: Dict[str, str] = prepare_params(
-            {
-                'type': to_string(type),
-                'fields': to_string(fields),
-                'marker': to_string(marker),
-                'limit': to_string(limit),
-            }
-        )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/retention_policies/',
-                    to_string(retention_policy_id),
-                    '/assignments',
+                    '/2.0/sign_requests/',
+                    to_string(sign_request_id),
+                    '/cancel',
                 ]
             ),
             FetchOptions(
-                method='GET',
-                params=query_params_map,
+                method='POST',
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return deserialize(response.data, RetentionPolicyAssignments)
+        return deserialize(response.data, SignRequest)
 
-    def create_retention_policy_assignment(
+    def resend_sign_request(
         self,
-        policy_id: str,
-        assign_to: CreateRetentionPolicyAssignmentAssignTo,
+        sign_request_id: str,
         *,
-        filter_fields: Optional[
-            List[CreateRetentionPolicyAssignmentFilterFields]
-        ] = None,
-        start_date_field: Optional[str] = None,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> RetentionPolicyAssignment:
+    ) -> None:
         """
-                Assigns a retention policy to an item.
-                :param policy_id: The ID of the retention policy to assign
-                :type policy_id: str
-                :param assign_to: The item to assign the policy to
-                :type assign_to: CreateRetentionPolicyAssignmentAssignTo
-                :param filter_fields: If the `assign_to` type is `metadata_template`,
-        then optionally add the `filter_fields` parameter which will
-        require an array of objects with a field entry and a value entry.
-        Currently only one object of `field` and `value` is supported., defaults to None
-                :type filter_fields: Optional[List[CreateRetentionPolicyAssignmentFilterFields]], optional
-                :param start_date_field: The date the retention policy assignment begins.
-
-        If the `assigned_to` type is `metadata_template`,
-        this field can be a date field's metadata attribute key id., defaults to None
-                :type start_date_field: Optional[str], optional
+                Resends a signature request email to all outstanding signers.
+                :param sign_request_id: The ID of the signature request
+        Example: "33243242"
+                :type sign_request_id: str
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
-        request_body: Dict = {
-            'policy_id': policy_id,
-            'assign_to': assign_to,
-            'filter_fields': filter_fields,
-            'start_date_field': start_date_field,
-        }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/retention_policy_assignments',
+                    '/2.0/sign_requests/',
+                    to_string(sign_request_id),
+                    '/resend',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
-                data=serialize(request_body),
-                content_type='application/json',
-                response_format='json',
+                response_format=None,
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return deserialize(response.data, RetentionPolicyAssignment)
+        return None
 
-    def get_retention_policy_assignment_by_id(
+    def get_sign_request_by_id(
         self,
-        retention_policy_assignment_id: str,
+        sign_request_id: str,
         *,
-        fields: Optional[List[str]] = None,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> RetentionPolicyAssignment:
+    ) -> SignRequest:
         """
-                Retrieves a retention policy assignment
-                :param retention_policy_assignment_id: The ID of the retention policy assignment.
-        Example: "1233123"
-                :type retention_policy_assignment_id: str
-                :param fields: A comma-separated list of attributes to include in the
-        response. This can be used to request fields that are
-        not normally returned in a standard response.
-
-        Be aware that specifying this parameter will have the
-        effect that none of the standard fields are returned in
-        the response unless explicitly specified, instead only
-        fields for the mini representation are returned, additional
-        to the fields requested., defaults to None
-                :type fields: Optional[List[str]], optional
+                Gets a sign request by ID.
+                :param sign_request_id: The ID of the signature request
+        Example: "33243242"
+                :type sign_request_id: str
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
-        query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/retention_policy_assignments/',
-                    to_string(retention_policy_assignment_id),
+                    '/2.0/sign_requests/',
+                    to_string(sign_request_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
-                params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return deserialize(response.data, RetentionPolicyAssignment)
+        return deserialize(response.data, SignRequest)
 
-    def delete_retention_policy_assignment_by_id(
+    def get_sign_requests(
         self,
-        retention_policy_assignment_id: str,
-        *,
-        extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> None:
-        """
-                Removes a retention policy assignment
-
-                applied to content.
-
-                :param retention_policy_assignment_id: The ID of the retention policy assignment.
-        Example: "1233123"
-                :type retention_policy_assignment_id: str
-                :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
-                :type extra_headers: Optional[Dict[str, Optional[str]]], optional
-        """
-        if extra_headers is None:
-            extra_headers = {}
-        headers_map: Dict[str, str] = prepare_params({**extra_headers})
-        response: FetchResponse = fetch(
-            ''.join(
-                [
-                    self.network_session.base_urls.base_url,
-                    '/retention_policy_assignments/',
-                    to_string(retention_policy_assignment_id),
-                ]
-            ),
-            FetchOptions(
-                method='DELETE',
-                headers=headers_map,
-                response_format=None,
-                auth=self.auth,
-                network_session=self.network_session,
-            ),
-        )
-        return None
-
-    def get_files_under_retention_policy_assignment(
-        self,
-        retention_policy_assignment_id: str,
         *,
         marker: Optional[str] = None,
         limit: Optional[int] = None,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> FilesUnderRetention:
+    ) -> SignRequests:
         """
-                Returns a list of files under retention for a retention policy assignment.
-                :param retention_policy_assignment_id: The ID of the retention policy assignment.
-        Example: "1233123"
-                :type retention_policy_assignment_id: str
+                Gets signature requests created by a user. If the `sign_files` and/or
+
+                `parent_folder` are deleted, the signature request will not return in the list.
+
                 :param marker: Defines the position marker at which to begin returning results. This is
         used when paginating using marker-based pagination.
 
         This requires `usemarker` to be set to `true`., defaults to None
                 :type marker: Optional[str], optional
                 :param limit: The maximum number of items to return per page., defaults to None
                 :type limit: Optional[int], optional
@@ -345,77 +199,120 @@
         if extra_headers is None:
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params(
             {'marker': to_string(marker), 'limit': to_string(limit)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join(
-                [
-                    self.network_session.base_urls.base_url,
-                    '/retention_policy_assignments/',
-                    to_string(retention_policy_assignment_id),
-                    '/files_under_retention',
-                ]
-            ),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/sign_requests']),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return deserialize(response.data, FilesUnderRetention)
+        return deserialize(response.data, SignRequests)
 
-    def get_file_versions_under_retention_policy_assignment(
+    def create_sign_request(
         self,
-        retention_policy_assignment_id: str,
+        signers: List[SignRequestCreateSigner],
         *,
-        marker: Optional[str] = None,
-        limit: Optional[int] = None,
+        source_files: Optional[List[FileBase]] = None,
+        signature_color: Optional[CreateSignRequestSignatureColor] = None,
+        parent_folder: Optional[FolderMini] = None,
+        is_document_preparation_needed: Optional[bool] = None,
+        redirect_url: Optional[str] = None,
+        declined_redirect_url: Optional[str] = None,
+        are_text_signatures_enabled: Optional[bool] = None,
+        email_subject: Optional[str] = None,
+        email_message: Optional[str] = None,
+        are_reminders_enabled: Optional[bool] = None,
+        name: Optional[str] = None,
+        prefill_tags: Optional[List[SignRequestPrefillTag]] = None,
+        days_valid: Optional[int] = None,
+        external_id: Optional[str] = None,
+        is_phone_verification_required_to_view: Optional[bool] = None,
+        template_id: Optional[str] = None,
+        external_system_name: Optional[str] = None,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> FilesUnderRetention:
+    ) -> SignRequest:
         """
-                Returns a list of file versions under retention for a retention policy
+        Creates a signature request. This involves preparing a document for signing and
 
-                assignment.
-
-                :param retention_policy_assignment_id: The ID of the retention policy assignment.
-        Example: "1233123"
-                :type retention_policy_assignment_id: str
-                :param marker: Defines the position marker at which to begin returning results. This is
-        used when paginating using marker-based pagination.
+        sending the signature request to signers.
 
-        This requires `usemarker` to be set to `true`., defaults to None
-                :type marker: Optional[str], optional
-                :param limit: The maximum number of items to return per page., defaults to None
-                :type limit: Optional[int], optional
-                :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
-                :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+        :param signers: Array of signers for the signature request. 35 is the max number of signers permitted.
+        :type signers: List[SignRequestCreateSigner]
+        :param source_files: List of files to create a signing document from. This is currently limited to ten files. Only the ID and type fields are required for each file., defaults to None
+        :type source_files: Optional[List[FileBase]], optional
+        :param signature_color: Force a specific color for the signature (blue, black, or red), defaults to None
+        :type signature_color: Optional[CreateSignRequestSignatureColor], optional
+        :param is_document_preparation_needed: Indicates if the sender should receive a `prepare_url` in the response to complete document preparation using the UI., defaults to None
+        :type is_document_preparation_needed: Optional[bool], optional
+        :param redirect_url: When specified, the signature request will be redirected to this url when a document is signed., defaults to None
+        :type redirect_url: Optional[str], optional
+        :param declined_redirect_url: The uri that a signer will be redirected to after declining to sign a document., defaults to None
+        :type declined_redirect_url: Optional[str], optional
+        :param are_text_signatures_enabled: Disables the usage of signatures generated by typing (text)., defaults to None
+        :type are_text_signatures_enabled: Optional[bool], optional
+        :param email_subject: Subject of sign request email. This is cleaned by sign request. If this field is not passed, a default subject will be used., defaults to None
+        :type email_subject: Optional[str], optional
+        :param email_message: Message to include in sign request email. The field is cleaned through sanitization of specific characters. However, some html tags are allowed. Links included in the message are also converted to hyperlinks in the email. The message may contain the following html tags including `a`, `abbr`, `acronym`, `b`, `blockquote`, `code`, `em`, `i`, `ul`, `li`, `ol`, and `strong`. Be aware that when the text to html ratio is too high, the email may end up in spam filters. Custom styles on these tags are not allowed. If this field is not passed, a default message will be used., defaults to None
+        :type email_message: Optional[str], optional
+        :param are_reminders_enabled: Reminds signers to sign a document on day 3, 8, 13 and 18. Reminders are only sent to outstanding signers., defaults to None
+        :type are_reminders_enabled: Optional[bool], optional
+        :param name: Name of the signature request., defaults to None
+        :type name: Optional[str], optional
+        :param prefill_tags: When a document contains sign-related tags in the content, you can prefill them using this `prefill_tags` by referencing the 'id' of the tag as the `external_id` field of the prefill tag., defaults to None
+        :type prefill_tags: Optional[List[SignRequestPrefillTag]], optional
+        :param days_valid: Set the number of days after which the created signature request will automatically expire if not completed. By default, we do not apply any expiration date on signature requests, and the signature request does not expire., defaults to None
+        :type days_valid: Optional[int], optional
+        :param external_id: This can be used to reference an ID in an external system that the sign request is related to., defaults to None
+        :type external_id: Optional[str], optional
+        :param is_phone_verification_required_to_view: Forces signers to verify a text message prior to viewing the document. You must specify the phone number of signers to have this setting apply to them., defaults to None
+        :type is_phone_verification_required_to_view: Optional[bool], optional
+        :param template_id: When a signature request is created from a template this field will indicate the id of that template., defaults to None
+        :type template_id: Optional[str], optional
+        :param external_system_name: Used as an optional system name to appear in the signature log next to the signers who have been assigned an `embed_url_external_id`, defaults to None
+        :type external_system_name: Optional[str], optional
+        :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
+        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
-        query_params_map: Dict[str, str] = prepare_params(
-            {'marker': to_string(marker), 'limit': to_string(limit)}
-        )
+        request_body: Dict = {
+            'source_files': source_files,
+            'signature_color': signature_color,
+            'signers': signers,
+            'parent_folder': parent_folder,
+            'is_document_preparation_needed': is_document_preparation_needed,
+            'redirect_url': redirect_url,
+            'declined_redirect_url': declined_redirect_url,
+            'are_text_signatures_enabled': are_text_signatures_enabled,
+            'email_subject': email_subject,
+            'email_message': email_message,
+            'are_reminders_enabled': are_reminders_enabled,
+            'name': name,
+            'prefill_tags': prefill_tags,
+            'days_valid': days_valid,
+            'external_id': external_id,
+            'is_phone_verification_required_to_view': is_phone_verification_required_to_view,
+            'template_id': template_id,
+            'external_system_name': external_system_name,
+        }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join(
-                [
-                    self.network_session.base_urls.base_url,
-                    '/retention_policy_assignments/',
-                    to_string(retention_policy_assignment_id),
-                    '/file_versions_under_retention',
-                ]
-            ),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/sign_requests']),
             FetchOptions(
-                method='GET',
-                params=query_params_map,
+                method='POST',
                 headers=headers_map,
+                data=serialize(request_body),
+                content_type='application/json',
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return deserialize(response.data, FilesUnderRetention)
+        return deserialize(response.data, SignRequest)
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/search.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,25 +12,27 @@
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.internal.utils import to_string
 
 from typing import Union
 
-from box_sdk_gen.schemas import MetadataQueryResults
+from box_sdk_gen.schemas.metadata_query_results import MetadataQueryResults
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import MetadataQuery
+from box_sdk_gen.schemas.metadata_query import MetadataQuery
 
-from box_sdk_gen.schemas import SearchResults
+from box_sdk_gen.schemas.search_results import SearchResults
 
-from box_sdk_gen.schemas import SearchResultsWithSharedLinks
+from box_sdk_gen.schemas.search_results_with_shared_links import (
+    SearchResultsWithSharedLinks,
+)
 
-from box_sdk_gen.schemas import MetadataFilter
+from box_sdk_gen.schemas.metadata_filter import MetadataFilter
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -221,15 +223,15 @@
             'fields': fields,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/metadata_queries/execute_read',
+                    '/2.0/metadata_queries/execute_read',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
@@ -426,15 +428,15 @@
         * `trashed_only` - Only searches for items currently in the trash
         * `non_trashed_only` - Only searches for items currently not in
           the trash
         * `all_items` - Searches for both trashed and non-trashed items., defaults to None
                 :type trash_content: Optional[SearchForContentTrashContent], optional
                 :param mdfilters: Limits the search results to any items for which the metadata matches the provided filter.
         This parameter is a list that specifies exactly **one** metadata template used to filter the search results.
-        It  unless the `query` parameter is provided., defaults to None
+        It is required unless the `query` parameter is provided., defaults to None
                 :type mdfilters: Optional[List[MetadataFilter]], optional
                 :param sort: Defines the order in which search results are returned. This API
         defaults to returning items by relevance unless this parameter is
         explicitly specified.
 
         * `relevance` (default) returns the results sorted by relevance to the
         query search term. The relevance is based on the occurrence of the search
@@ -537,15 +539,15 @@
                 'offset': to_string(offset),
                 'deleted_user_ids': to_string(deleted_user_ids),
                 'deleted_at_range': to_string(deleted_at_range),
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/search']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/search']),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/session_termination.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/session_termination.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 from typing import Dict
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import SessionTerminationMessage
+from box_sdk_gen.schemas.session_termination_message import SessionTerminationMessage
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -70,15 +70,18 @@
         """
         if extra_headers is None:
             extra_headers = {}
         request_body: Dict = {'user_ids': user_ids, 'user_logins': user_logins}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/users/terminate_sessions']
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/users/terminate_sessions',
+                ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
@@ -112,15 +115,18 @@
         """
         if extra_headers is None:
             extra_headers = {}
         request_body: Dict = {'group_ids': group_ids}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/groups/terminate_sessions']
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/groups/terminate_sessions',
+                ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/shared_links_files.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/shared_links_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import FileFull
+from box_sdk_gen.schemas.file_full import FileFull
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -300,15 +300,15 @@
             {
                 'if-none-match': to_string(if_none_match),
                 'boxapi': to_string(boxapi),
                 **extra_headers,
             }
         )
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/shared_items']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/shared_items']),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
@@ -344,15 +344,15 @@
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '#get_shared_link',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
@@ -398,15 +398,15 @@
         request_body: Dict = {'shared_link': shared_link}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '#add_shared_link',
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 params=query_params_map,
@@ -452,15 +452,15 @@
         request_body: Dict = {'shared_link': shared_link}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '#update_shared_link',
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 params=query_params_map,
@@ -507,15 +507,15 @@
         request_body: Dict = {'shared_link': shared_link}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '#remove_shared_link',
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 params=query_params_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/shared_links_folders.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/shared_links_folders.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import FolderFull
+from box_sdk_gen.schemas.folder_full import FolderFull
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -290,15 +290,17 @@
             {
                 'if-none-match': to_string(if_none_match),
                 'boxapi': to_string(boxapi),
                 **extra_headers,
             }
         )
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/shared_items#folders']),
+            ''.join(
+                [self.network_session.base_urls.base_url, '/2.0/shared_items#folders']
+            ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
@@ -337,15 +339,15 @@
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                     '#get_shared_link',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
@@ -395,15 +397,15 @@
         request_body: Dict = {'shared_link': shared_link}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                     '#add_shared_link',
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 params=query_params_map,
@@ -452,15 +454,15 @@
         request_body: Dict = {'shared_link': shared_link}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                     '#update_shared_link',
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 params=query_params_map,
@@ -510,15 +512,15 @@
         request_body: Dict = {'shared_link': shared_link}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                     '#remove_shared_link',
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 params=query_params_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/shared_links_web_links.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/shared_links_web_links.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import WebLink
+from box_sdk_gen.schemas.web_link import WebLink
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -289,15 +289,15 @@
                 'if-none-match': to_string(if_none_match),
                 'boxapi': to_string(boxapi),
                 **extra_headers,
             }
         )
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/shared_items#web_links']
+                [self.network_session.base_urls.base_url, '/2.0/shared_items#web_links']
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
@@ -328,15 +328,15 @@
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/web_links/',
+                    '/2.0/web_links/',
                     to_string(web_link_id),
                     '#get_shared_link',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
@@ -377,15 +377,15 @@
         request_body: Dict = {'shared_link': shared_link}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/web_links/',
+                    '/2.0/web_links/',
                     to_string(web_link_id),
                     '#add_shared_link',
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 params=query_params_map,
@@ -425,15 +425,15 @@
         request_body: Dict = {'shared_link': shared_link}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/web_links/',
+                    '/2.0/web_links/',
                     to_string(web_link_id),
                     '#update_shared_link',
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 params=query_params_map,
@@ -474,15 +474,15 @@
         request_body: Dict = {'shared_link': shared_link}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/web_links/',
+                    '/2.0/web_links/',
                     to_string(web_link_id),
                     '#remove_shared_link',
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 params=query_params_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/shield_information_barrier_reports.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/shield_information_barrier_reports.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,31 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import ShieldInformationBarrierBase
-
-from box_sdk_gen.schemas import ShieldInformationBarrierReports
-
-from box_sdk_gen.schemas import ClientError
-
-from box_sdk_gen.schemas import ShieldInformationBarrierReport
-
-from box_sdk_gen.schemas import ShieldInformationBarrierReference
+from box_sdk_gen.schemas.shield_information_barrier_base import (
+    ShieldInformationBarrierBase,
+)
+
+from box_sdk_gen.schemas.shield_information_barrier_reports import (
+    ShieldInformationBarrierReports,
+)
+
+from box_sdk_gen.schemas.client_error import ClientError
+
+from box_sdk_gen.schemas.shield_information_barrier_report import (
+    ShieldInformationBarrierReport,
+)
+
+from box_sdk_gen.schemas.shield_information_barrier_reference import (
+    ShieldInformationBarrierReference,
+)
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -85,15 +93,15 @@
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barrier_reports',
+                    '/2.0/shield_information_barrier_reports',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
@@ -118,15 +126,15 @@
             extra_headers = {}
         request_body: Dict = {'shield_information_barrier': shield_information_barrier}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barrier_reports',
+                    '/2.0/shield_information_barrier_reports',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
@@ -154,15 +162,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barrier_reports/',
+                    '/2.0/shield_information_barrier_reports/',
                     to_string(shield_information_barrier_report_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/shield_information_barrier_segment_members.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/shield_information_barrier_segment_members.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,23 +8,29 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import ShieldInformationBarrierSegmentMember
+from box_sdk_gen.schemas.shield_information_barrier_segment_member import (
+    ShieldInformationBarrierSegmentMember,
+)
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import ShieldInformationBarrierSegmentMembers
+from box_sdk_gen.schemas.shield_information_barrier_segment_members import (
+    ShieldInformationBarrierSegmentMembers,
+)
 
-from box_sdk_gen.schemas import ShieldInformationBarrierBase
+from box_sdk_gen.schemas.shield_information_barrier_base import (
+    ShieldInformationBarrierBase,
+)
 
-from box_sdk_gen.schemas import UserBase
+from box_sdk_gen.schemas.user_base import UserBase
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -113,15 +119,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barrier_segment_members/',
+                    '/2.0/shield_information_barrier_segment_members/',
                     to_string(shield_information_barrier_segment_member_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
@@ -151,15 +157,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barrier_segment_members/',
+                    '/2.0/shield_information_barrier_segment_members/',
                     to_string(shield_information_barrier_segment_member_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
@@ -206,15 +212,15 @@
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barrier_segment_members',
+                    '/2.0/shield_information_barrier_segment_members',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
@@ -254,15 +260,15 @@
             'user': user,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barrier_segment_members',
+                    '/2.0/shield_information_barrier_segment_members',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/shield_information_barrier_segment_restrictions.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/shield_information_barrier_segment_restrictions.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,21 +8,27 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import ShieldInformationBarrierSegmentRestriction
-
-from box_sdk_gen.schemas import ClientError
-
-from box_sdk_gen.schemas import ShieldInformationBarrierSegmentRestrictions
-
-from box_sdk_gen.schemas import ShieldInformationBarrierBase
+from box_sdk_gen.schemas.shield_information_barrier_segment_restriction import (
+    ShieldInformationBarrierSegmentRestriction,
+)
+
+from box_sdk_gen.schemas.client_error import ClientError
+
+from box_sdk_gen.schemas.shield_information_barrier_segment_restrictions import (
+    ShieldInformationBarrierSegmentRestrictions,
+)
+
+from box_sdk_gen.schemas.shield_information_barrier_base import (
+    ShieldInformationBarrierBase,
+)
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -142,15 +148,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barrier_segment_restrictions/',
+                    '/2.0/shield_information_barrier_segment_restrictions/',
                     to_string(shield_information_barrier_segment_restriction_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
@@ -180,15 +186,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barrier_segment_restrictions/',
+                    '/2.0/shield_information_barrier_segment_restrictions/',
                     to_string(shield_information_barrier_segment_restriction_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
@@ -235,15 +241,15 @@
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barrier_segment_restrictions',
+                    '/2.0/shield_information_barrier_segment_restrictions',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
@@ -288,15 +294,15 @@
             'restricted_segment': restricted_segment,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barrier_segment_restrictions',
+                    '/2.0/shield_information_barrier_segment_restrictions',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/shield_information_barrier_segments.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/shield_information_barrier_segments.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,27 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import ShieldInformationBarrierSegment
-
-from box_sdk_gen.schemas import ClientError
-
-from box_sdk_gen.schemas import ShieldInformationBarrierSegments
-
-from box_sdk_gen.schemas import ShieldInformationBarrierBase
+from box_sdk_gen.schemas.shield_information_barrier_segment import (
+    ShieldInformationBarrierSegment,
+)
+
+from box_sdk_gen.schemas.client_error import ClientError
+
+from box_sdk_gen.schemas.shield_information_barrier_segments import (
+    ShieldInformationBarrierSegments,
+)
+
+from box_sdk_gen.schemas.shield_information_barrier_base import (
+    ShieldInformationBarrierBase,
+)
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -66,15 +72,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barrier_segments/',
+                    '/2.0/shield_information_barrier_segments/',
                     to_string(shield_information_barrier_segment_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
@@ -109,15 +115,15 @@
             extra_headers = {}
         request_body: Dict = {'name': name, 'description': description}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barrier_segments/',
+                    '/2.0/shield_information_barrier_segments/',
                     to_string(shield_information_barrier_segment_id),
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
                 data=serialize(request_body),
@@ -149,15 +155,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barrier_segments/',
+                    '/2.0/shield_information_barrier_segments/',
                     to_string(shield_information_barrier_segment_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
@@ -204,15 +210,15 @@
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barrier_segments',
+                    '/2.0/shield_information_barrier_segments',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
@@ -247,15 +253,15 @@
             'description': description,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barrier_segments',
+                    '/2.0/shield_information_barrier_segments',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/shield_information_barriers.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/shield_information_barriers.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import ShieldInformationBarrier
+from box_sdk_gen.schemas.shield_information_barrier import ShieldInformationBarrier
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import ShieldInformationBarriers
+from box_sdk_gen.schemas.shield_information_barriers import ShieldInformationBarriers
 
-from box_sdk_gen.schemas import EnterpriseBase
+from box_sdk_gen.schemas.enterprise_base import EnterpriseBase
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -73,15 +73,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barriers/',
+                    '/2.0/shield_information_barriers/',
                     to_string(shield_information_barrier_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
@@ -111,15 +111,15 @@
             extra_headers = {}
         request_body: Dict = {'id': id, 'status': status}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barriers/change_status',
+                    '/2.0/shield_information_barriers/change_status',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
@@ -156,15 +156,15 @@
             {'marker': to_string(marker), 'limit': to_string(limit)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barriers',
+                    '/2.0/shield_information_barriers',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
@@ -197,15 +197,15 @@
             extra_headers = {}
         request_body: Dict = {'enterprise': enterprise}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/shield_information_barriers',
+                    '/2.0/shield_information_barriers',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/sign_requests.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/tasks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,26 @@
 from enum import Enum
 
 from typing import Optional
 
+from box_sdk_gen.internal.base_object import BaseObject
+
 from typing import Dict
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from typing import List
-
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import FileBase
-
-from box_sdk_gen.schemas import SignRequestCreateSigner
-
-from box_sdk_gen.schemas import FolderMini
-
-from box_sdk_gen.schemas import SignRequestPrefillTag
-
-from box_sdk_gen.schemas import SignRequest
+from box_sdk_gen.schemas.tasks import Tasks
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import SignRequests
-
-from box_sdk_gen.schemas import SignRequestCreateRequest
+from box_sdk_gen.schemas.task import Task
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -44,271 +34,303 @@
 
 from box_sdk_gen.networking.fetch import fetch
 
 from box_sdk_gen.serialization.json.json_data import sd_to_json
 
 from box_sdk_gen.serialization.json.json_data import SerializedData
 
+from box_sdk_gen.internal.utils import DateTime
+
+
+class CreateTaskItemTypeField(str, Enum):
+    FILE = 'file'
+
+
+class CreateTaskItem(BaseObject):
+    _discriminator = 'type', {'file'}
+
+    def __init__(
+        self,
+        *,
+        id: Optional[str] = None,
+        type: Optional[CreateTaskItemTypeField] = None,
+        **kwargs
+    ):
+        """
+        :param id: The ID of the file, defaults to None
+        :type id: Optional[str], optional
+        :param type: `file`, defaults to None
+        :type type: Optional[CreateTaskItemTypeField], optional
+        """
+        super().__init__(**kwargs)
+        self.id = id
+        self.type = type
+
+
+class CreateTaskAction(str, Enum):
+    REVIEW = 'review'
+    COMPLETE = 'complete'
+
 
-class CreateSignRequestSignatureColor(str, Enum):
-    BLUE = 'blue'
-    BLACK = 'black'
-    RED = 'red'
+class CreateTaskCompletionRule(str, Enum):
+    ALL_ASSIGNEES = 'all_assignees'
+    ANY_ASSIGNEE = 'any_assignee'
 
 
-class SignRequestsManager:
+class UpdateTaskByIdAction(str, Enum):
+    REVIEW = 'review'
+    COMPLETE = 'complete'
+
+
+class UpdateTaskByIdCompletionRule(str, Enum):
+    ALL_ASSIGNEES = 'all_assignees'
+    ANY_ASSIGNEE = 'any_assignee'
+
+
+class TasksManager:
     def __init__(
         self,
         *,
         auth: Optional[Authentication] = None,
         network_session: NetworkSession = None
     ):
         if network_session is None:
             network_session = NetworkSession()
         self.auth = auth
         self.network_session = network_session
 
-    def cancel_sign_request(
-        self,
-        sign_request_id: str,
-        *,
-        extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> SignRequest:
+    def get_file_tasks(
+        self, file_id: str, *, extra_headers: Optional[Dict[str, Optional[str]]] = None
+    ) -> Tasks:
         """
-                Cancels a sign request.
-                :param sign_request_id: The ID of the sign request
-        Example: "33243242"
-                :type sign_request_id: str
+                Retrieves a list of all the tasks for a file. This
+
+                endpoint does not support pagination.
+
+                :param file_id: The unique identifier that represents a file.
+
+        The ID for any file can be determined
+        by visiting a file in the web application
+        and copying the ID from the URL. For example,
+        for the URL `https://*.app.box.com/files/123`
+        the `file_id` is `123`.
+        Example: "12345"
+                :type file_id: str
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/sign_requests/',
-                    to_string(sign_request_id),
-                    '/cancel',
+                    '/2.0/files/',
+                    to_string(file_id),
+                    '/tasks',
                 ]
             ),
             FetchOptions(
-                method='POST',
+                method='GET',
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return deserialize(response.data, SignRequest)
+        return deserialize(response.data, Tasks)
 
-    def resend_sign_request(
+    def create_task(
         self,
-        sign_request_id: str,
+        item: CreateTaskItem,
         *,
+        action: Optional[CreateTaskAction] = None,
+        message: Optional[str] = None,
+        due_at: Optional[DateTime] = None,
+        completion_rule: Optional[CreateTaskCompletionRule] = None,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> None:
+    ) -> Task:
         """
-                Resends a sign request email to all outstanding signers.
-                :param sign_request_id: The ID of the sign request
-        Example: "33243242"
-                :type sign_request_id: str
+                Creates a single task on a file. This task is not assigned to any user and
+
+                will need to be assigned separately.
+
+                :param item: The file to attach the task to.
+                :type item: CreateTaskItem
+                :param action: The action the task assignee will be prompted to do. Must be
+
+        * `review` defines an approval task that can be approved or
+        rejected
+        * `complete` defines a general task which can be completed, defaults to None
+                :type action: Optional[CreateTaskAction], optional
+                :param message: An optional message to include with the task., defaults to None
+                :type message: Optional[str], optional
+                :param due_at: Defines when the task is due. Defaults to `null` if not
+        provided., defaults to None
+                :type due_at: Optional[DateTime], optional
+                :param completion_rule: Defines which assignees need to complete this task before the task
+        is considered completed.
+
+        * `all_assignees` (default) requires all assignees to review or
+        approve the the task in order for it to be considered completed.
+        * `any_assignee` accepts any one assignee to review or
+        approve the the task in order for it to be considered completed., defaults to None
+                :type completion_rule: Optional[CreateTaskCompletionRule], optional
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
+        request_body: Dict = {
+            'item': item,
+            'action': action,
+            'message': message,
+            'due_at': due_at,
+            'completion_rule': completion_rule,
+        }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join(
-                [
-                    self.network_session.base_urls.base_url,
-                    '/sign_requests/',
-                    to_string(sign_request_id),
-                    '/resend',
-                ]
-            ),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/tasks']),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
-                response_format=None,
+                data=serialize(request_body),
+                content_type='application/json',
+                response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return None
+        return deserialize(response.data, Task)
 
-    def get_sign_request_by_id(
-        self,
-        sign_request_id: str,
-        *,
-        extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> SignRequest:
+    def get_task_by_id(
+        self, task_id: str, *, extra_headers: Optional[Dict[str, Optional[str]]] = None
+    ) -> Task:
         """
-                Gets a sign request by ID.
-                :param sign_request_id: The ID of the sign request
-        Example: "33243242"
-                :type sign_request_id: str
+                Retrieves information about a specific task.
+                :param task_id: The ID of the task.
+        Example: "12345"
+                :type task_id: str
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/sign_requests/',
-                    to_string(sign_request_id),
+                    '/2.0/tasks/',
+                    to_string(task_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return deserialize(response.data, SignRequest)
+        return deserialize(response.data, Task)
 
-    def get_sign_requests(
+    def update_task_by_id(
         self,
+        task_id: str,
         *,
-        marker: Optional[str] = None,
-        limit: Optional[int] = None,
+        action: Optional[UpdateTaskByIdAction] = None,
+        message: Optional[str] = None,
+        due_at: Optional[DateTime] = None,
+        completion_rule: Optional[UpdateTaskByIdCompletionRule] = None,
         extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> SignRequests:
+    ) -> Task:
         """
-                Gets sign requests created by a user. If the `sign_files` and/or
+                Updates a task. This can be used to update a task's configuration, or to
 
-                `parent_folder` are deleted, the sign request will not return in the list.
+                update its completion state.
 
-                :param marker: Defines the position marker at which to begin returning results. This is
-        used when paginating using marker-based pagination.
-
-        This requires `usemarker` to be set to `true`., defaults to None
-                :type marker: Optional[str], optional
-                :param limit: The maximum number of items to return per page., defaults to None
-                :type limit: Optional[int], optional
+                :param task_id: The ID of the task.
+        Example: "12345"
+                :type task_id: str
+                :param action: The action the task assignee will be prompted to do. Must be
+
+        * `review` defines an approval task that can be approved or
+        rejected
+        * `complete` defines a general task which can be completed, defaults to None
+                :type action: Optional[UpdateTaskByIdAction], optional
+                :param message: The message included with the task., defaults to None
+                :type message: Optional[str], optional
+                :param due_at: When the task is due at., defaults to None
+                :type due_at: Optional[DateTime], optional
+                :param completion_rule: Defines which assignees need to complete this task before the task
+        is considered completed.
+
+        * `all_assignees` (default) requires all assignees to review or
+        approve the the task in order for it to be considered completed.
+        * `any_assignee` accepts any one assignee to review or
+        approve the the task in order for it to be considered completed., defaults to None
+                :type completion_rule: Optional[UpdateTaskByIdCompletionRule], optional
                 :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
-        query_params_map: Dict[str, str] = prepare_params(
-            {'marker': to_string(marker), 'limit': to_string(limit)}
-        )
+        request_body: Dict = {
+            'action': action,
+            'message': message,
+            'due_at': due_at,
+            'completion_rule': completion_rule,
+        }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/sign_requests']),
+            ''.join(
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/tasks/',
+                    to_string(task_id),
+                ]
+            ),
             FetchOptions(
-                method='GET',
-                params=query_params_map,
+                method='PUT',
                 headers=headers_map,
+                data=serialize(request_body),
+                content_type='application/json',
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return deserialize(response.data, SignRequests)
+        return deserialize(response.data, Task)
 
-    def create_sign_request(
-        self,
-        signers: List[SignRequestCreateSigner],
-        *,
-        source_files: Optional[List[FileBase]] = None,
-        signature_color: Optional[CreateSignRequestSignatureColor] = None,
-        parent_folder: Optional[FolderMini] = None,
-        is_document_preparation_needed: Optional[bool] = None,
-        redirect_url: Optional[str] = None,
-        declined_redirect_url: Optional[str] = None,
-        are_text_signatures_enabled: Optional[bool] = None,
-        email_subject: Optional[str] = None,
-        email_message: Optional[str] = None,
-        are_reminders_enabled: Optional[bool] = None,
-        name: Optional[str] = None,
-        prefill_tags: Optional[List[SignRequestPrefillTag]] = None,
-        days_valid: Optional[int] = None,
-        external_id: Optional[str] = None,
-        is_phone_verification_required_to_view: Optional[bool] = None,
-        template_id: Optional[str] = None,
-        extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> SignRequest:
+    def delete_task_by_id(
+        self, task_id: str, *, extra_headers: Optional[Dict[str, Optional[str]]] = None
+    ) -> None:
         """
-        Creates a sign request. This involves preparing a document for signing and
-
-        sending the sign request to signers.
-
-        :param signers: Array of signers for the sign request. 35 is the max number of signers permitted.
-        :type signers: List[SignRequestCreateSigner]
-        :param source_files: List of files to create a signing document from. This is currently limited to ten files. Only the ID and type fields are required for each file., defaults to None
-        :type source_files: Optional[List[FileBase]], optional
-        :param signature_color: Force a specific color for the signature (blue, black, or red), defaults to None
-        :type signature_color: Optional[CreateSignRequestSignatureColor], optional
-        :param is_document_preparation_needed: Indicates if the sender should receive a `prepare_url` in the response to complete document preparation via UI., defaults to None
-        :type is_document_preparation_needed: Optional[bool], optional
-        :param redirect_url: When specified, signature request will be redirected to this url when a document is signed., defaults to None
-        :type redirect_url: Optional[str], optional
-        :param declined_redirect_url: The uri that a signer will be redirected to after declining to sign a document., defaults to None
-        :type declined_redirect_url: Optional[str], optional
-        :param are_text_signatures_enabled: Disables the usage of signatures generated by typing (text)., defaults to None
-        :type are_text_signatures_enabled: Optional[bool], optional
-        :param email_subject: Subject of sign request email. This is cleaned by sign request. If this field is not passed, a default subject will be used., defaults to None
-        :type email_subject: Optional[str], optional
-        :param email_message: Message to include in sign request email. The field is cleaned through sanitization of specific characters. However, some html tags are allowed. Links included in the message are also converted to hyperlinks in the email. The message may contain the following html tags including `a`, `abbr`, `acronym`, `b`, `blockquote`, `code`, `em`, `i`, `ul`, `li`, `ol`, and `strong`. Be aware that when the text to html ratio is too high, the email may end up in spam filters. Custom styles on these tags are not allowed. If this field is not passed, a default message will be used., defaults to None
-        :type email_message: Optional[str], optional
-        :param are_reminders_enabled: Reminds signers to sign a document on day 3, 8, 13 and 18. Reminders are only sent to outstanding signers., defaults to None
-        :type are_reminders_enabled: Optional[bool], optional
-        :param name: Name of the sign request., defaults to None
-        :type name: Optional[str], optional
-        :param prefill_tags: When a document contains sign related tags in the content, you can prefill them using this `prefill_tags` by referencing the 'id' of the tag as the `external_id` field of the prefill tag., defaults to None
-        :type prefill_tags: Optional[List[SignRequestPrefillTag]], optional
-        :param days_valid: Set the number of days after which the created signature request will automatically expire if not completed. By default, we do not apply any expiration date on signature requests, and the signature request does not expire., defaults to None
-        :type days_valid: Optional[int], optional
-        :param external_id: This can be used to reference an ID in an external system that the sign request is related to., defaults to None
-        :type external_id: Optional[str], optional
-        :param is_phone_verification_required_to_view: Forces signers to verify a text message prior to viewing the document. You must specify the phone number of signers to have this setting apply to them., defaults to None
-        :type is_phone_verification_required_to_view: Optional[bool], optional
-        :param template_id: When a signature request is created from a template this field will indicate the id of that template., defaults to None
-        :type template_id: Optional[str], optional
-        :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
-        :type extra_headers: Optional[Dict[str, Optional[str]]], optional
+                Removes a task from a file.
+                :param task_id: The ID of the task.
+        Example: "12345"
+                :type task_id: str
+                :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
+                :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
-        request_body: Dict = {
-            'source_files': source_files,
-            'signature_color': signature_color,
-            'signers': signers,
-            'parent_folder': parent_folder,
-            'is_document_preparation_needed': is_document_preparation_needed,
-            'redirect_url': redirect_url,
-            'declined_redirect_url': declined_redirect_url,
-            'are_text_signatures_enabled': are_text_signatures_enabled,
-            'email_subject': email_subject,
-            'email_message': email_message,
-            'are_reminders_enabled': are_reminders_enabled,
-            'name': name,
-            'prefill_tags': prefill_tags,
-            'days_valid': days_valid,
-            'external_id': external_id,
-            'is_phone_verification_required_to_view': is_phone_verification_required_to_view,
-            'template_id': template_id,
-        }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/sign_requests']),
+            ''.join(
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/tasks/',
+                    to_string(task_id),
+                ]
+            ),
             FetchOptions(
-                method='POST',
+                method='DELETE',
                 headers=headers_map,
-                data=serialize(request_body),
-                content_type='application/json',
-                response_format='json',
+                response_format=None,
                 auth=self.auth,
                 network_session=self.network_session,
             ),
         )
-        return deserialize(response.data, SignRequest)
+        return None
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/sign_templates.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/sign_templates.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from typing import Dict
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import SignTemplates
+from box_sdk_gen.schemas.sign_templates import SignTemplates
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import SignTemplate
+from box_sdk_gen.schemas.sign_template import SignTemplate
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -67,15 +67,15 @@
         if extra_headers is None:
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params(
             {'marker': to_string(marker), 'limit': to_string(limit)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/sign_templates']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/sign_templates']),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
@@ -100,15 +100,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/sign_templates/',
+                    '/2.0/sign_templates/',
                     to_string(template_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/skills.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/skills.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import SkillCardsMetadata
+from box_sdk_gen.schemas.skill_cards_metadata import SkillCardsMetadata
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import KeywordSkillCard
+from box_sdk_gen.schemas.keyword_skill_card import KeywordSkillCard
 
-from box_sdk_gen.schemas import TimelineSkillCard
+from box_sdk_gen.schemas.timeline_skill_card import TimelineSkillCard
 
-from box_sdk_gen.schemas import TranscriptSkillCard
+from box_sdk_gen.schemas.transcript_skill_card import TranscriptSkillCard
 
-from box_sdk_gen.schemas import StatusSkillCard
+from box_sdk_gen.schemas.status_skill_card import StatusSkillCard
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -212,15 +212,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/metadata/global/boxSkillsCards',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
@@ -265,15 +265,15 @@
             extra_headers = {}
         request_body: Dict = {'cards': cards}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/metadata/global/boxSkillsCards',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
@@ -312,15 +312,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/metadata/global/boxSkillsCards',
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
@@ -353,15 +353,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/metadata/global/boxSkillsCards',
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
@@ -419,15 +419,15 @@
             'usage': usage,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/skill_invocations/',
+                    '/2.0/skill_invocations/',
                     to_string(skill_id),
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
                 data=serialize(request_body),
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/storage_policies.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/storage_policies.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 from typing import Dict
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import StoragePolicies
+from box_sdk_gen.schemas.storage_policies import StoragePolicies
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import StoragePolicy
+from box_sdk_gen.schemas.storage_policy import StoragePolicy
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -84,15 +84,15 @@
                 'fields': to_string(fields),
                 'marker': to_string(marker),
                 'limit': to_string(limit),
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/storage_policies']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/storage_policies']),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
@@ -117,15 +117,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/storage_policies/',
+                    '/2.0/storage_policies/',
                     to_string(storage_policy_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/storage_policy_assignments.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/storage_policy_assignments.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import StoragePolicyAssignments
+from box_sdk_gen.schemas.storage_policy_assignments import StoragePolicyAssignments
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import StoragePolicyAssignment
+from box_sdk_gen.schemas.storage_policy_assignment import StoragePolicyAssignment
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -158,15 +158,18 @@
                 'resolved_for_type': to_string(resolved_for_type),
                 'resolved_for_id': to_string(resolved_for_id),
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/storage_policy_assignments']
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/storage_policy_assignments',
+                ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
@@ -198,15 +201,18 @@
         request_body: Dict = {
             'storage_policy': storage_policy,
             'assigned_to': assigned_to,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/storage_policy_assignments']
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/storage_policy_assignments',
+                ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
@@ -233,15 +239,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/storage_policy_assignments/',
+                    '/2.0/storage_policy_assignments/',
                     to_string(storage_policy_assignment_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
@@ -273,15 +279,15 @@
             extra_headers = {}
         request_body: Dict = {'storage_policy': storage_policy}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/storage_policy_assignments/',
+                    '/2.0/storage_policy_assignments/',
                     to_string(storage_policy_assignment_id),
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
                 data=serialize(request_body),
@@ -325,15 +331,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/storage_policy_assignments/',
+                    '/2.0/storage_policy_assignments/',
                     to_string(storage_policy_assignment_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/task_assignments.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/task_assignments.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import TaskAssignments
+from box_sdk_gen.schemas.task_assignments import TaskAssignments
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import TaskAssignment
+from box_sdk_gen.schemas.task_assignment import TaskAssignment
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -117,15 +117,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/tasks/',
+                    '/2.0/tasks/',
                     to_string(task_id),
                     '/assignments',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
@@ -159,15 +159,15 @@
         :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         request_body: Dict = {'task': task, 'assign_to': assign_to}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/task_assignments']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/task_assignments']),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
                 auth=self.auth,
@@ -193,15 +193,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/task_assignments/',
+                    '/2.0/task_assignments/',
                     to_string(task_assignment_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
@@ -243,15 +243,15 @@
             extra_headers = {}
         request_body: Dict = {'message': message, 'resolution_state': resolution_state}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/task_assignments/',
+                    '/2.0/task_assignments/',
                     to_string(task_assignment_id),
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
                 data=serialize(request_body),
@@ -280,15 +280,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/task_assignments/',
+                    '/2.0/task_assignments/',
                     to_string(task_assignment_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/tasks.py` & `box_sdk_gen-1.0.0/box_sdk_gen/schemas/sign_request.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,324 +1,175 @@
 from enum import Enum
 
 from typing import Optional
 
-from box_sdk_gen.internal.base_object import BaseObject
-
-from typing import Dict
-
-from box_sdk_gen.internal.utils import to_string
-
-from box_sdk_gen.serialization.json.serializer import deserialize
-
-from box_sdk_gen.serialization.json.serializer import serialize
-
-from box_sdk_gen.schemas import Tasks
-
-from box_sdk_gen.schemas import ClientError
+from typing import List
 
-from box_sdk_gen.schemas import Task
-
-from box_sdk_gen.networking.auth import Authentication
-
-from box_sdk_gen.networking.network import NetworkSession
-
-from box_sdk_gen.internal.utils import prepare_params
-
-from box_sdk_gen.internal.utils import to_string
+from box_sdk_gen.internal.base_object import BaseObject
 
-from box_sdk_gen.internal.utils import ByteStream
+from box_sdk_gen.schemas.sign_request_prefill_tag import SignRequestPrefillTag
 
-from box_sdk_gen.networking.fetch import FetchOptions
+from box_sdk_gen.schemas.sign_request_base import SignRequestBase
 
-from box_sdk_gen.networking.fetch import FetchResponse
+from box_sdk_gen.schemas.file_base import FileBase
 
-from box_sdk_gen.networking.fetch import fetch
+from box_sdk_gen.schemas.sign_request_signer import SignRequestSigner
 
-from box_sdk_gen.serialization.json.json_data import sd_to_json
+from box_sdk_gen.schemas.file_mini import FileMini
 
-from box_sdk_gen.serialization.json.json_data import SerializedData
+from box_sdk_gen.schemas.folder_mini import FolderMini
 
 from box_sdk_gen.internal.utils import DateTime
 
 
-class CreateTaskItemTypeField(str, Enum):
-    FILE = 'file'
+class SignRequestTypeField(str, Enum):
+    SIGN_REQUEST = 'sign-request'
+
 
+class SignRequestStatusField(str, Enum):
+    CONVERTING = 'converting'
+    CREATED = 'created'
+    SENT = 'sent'
+    VIEWED = 'viewed'
+    SIGNED = 'signed'
+    CANCELLED = 'cancelled'
+    DECLINED = 'declined'
+    ERROR_CONVERTING = 'error_converting'
+    ERROR_SENDING = 'error_sending'
+    EXPIRED = 'expired'
+    FINALIZING = 'finalizing'
+    ERROR_FINALIZING = 'error_finalizing'
 
-class CreateTaskItem(BaseObject):
-    _discriminator = 'type', {'file'}
 
+class SignRequestSignFilesField(BaseObject):
     def __init__(
         self,
         *,
-        id: Optional[str] = None,
-        type: Optional[CreateTaskItemTypeField] = None,
+        files: Optional[List[FileMini]] = None,
+        is_ready_for_download: Optional[bool] = None,
         **kwargs
     ):
         """
-        :param id: The ID of the file, defaults to None
-        :type id: Optional[str], optional
-        :param type: `file`, defaults to None
-        :type type: Optional[CreateTaskItemTypeField], optional
+                :param is_ready_for_download: Indicates whether the `sign_files` documents are processing
+        and the PDFs may be out of date. A change to any document
+        requires processing on all `sign_files`. We
+        recommended waiting until processing is finished
+        (and this value is true) before downloading the PDFs., defaults to None
+                :type is_ready_for_download: Optional[bool], optional
         """
         super().__init__(**kwargs)
-        self.id = id
-        self.type = type
-
-
-class CreateTaskAction(str, Enum):
-    REVIEW = 'review'
-    COMPLETE = 'complete'
-
-
-class CreateTaskCompletionRule(str, Enum):
-    ALL_ASSIGNEES = 'all_assignees'
-    ANY_ASSIGNEE = 'any_assignee'
-
+        self.files = files
+        self.is_ready_for_download = is_ready_for_download
 
-class UpdateTaskByIdAction(str, Enum):
-    REVIEW = 'review'
-    COMPLETE = 'complete'
 
-
-class UpdateTaskByIdCompletionRule(str, Enum):
-    ALL_ASSIGNEES = 'all_assignees'
-    ANY_ASSIGNEE = 'any_assignee'
-
-
-class TasksManager:
+class SignRequest(SignRequestBase):
     def __init__(
         self,
         *,
-        auth: Optional[Authentication] = None,
-        network_session: NetworkSession = None
+        type: Optional[SignRequestTypeField] = None,
+        source_files: Optional[List[FileBase]] = None,
+        signers: Optional[List[SignRequestSigner]] = None,
+        signature_color: Optional[str] = None,
+        id: Optional[str] = None,
+        prepare_url: Optional[str] = None,
+        signing_log: Optional[FileMini] = None,
+        status: Optional[SignRequestStatusField] = None,
+        sign_files: Optional[SignRequestSignFilesField] = None,
+        auto_expire_at: Optional[DateTime] = None,
+        parent_folder: Optional[FolderMini] = None,
+        is_document_preparation_needed: Optional[bool] = None,
+        redirect_url: Optional[str] = None,
+        declined_redirect_url: Optional[str] = None,
+        are_text_signatures_enabled: Optional[bool] = None,
+        email_subject: Optional[str] = None,
+        email_message: Optional[str] = None,
+        are_reminders_enabled: Optional[bool] = None,
+        name: Optional[str] = None,
+        prefill_tags: Optional[List[SignRequestPrefillTag]] = None,
+        days_valid: Optional[int] = None,
+        external_id: Optional[str] = None,
+        is_phone_verification_required_to_view: Optional[bool] = None,
+        template_id: Optional[str] = None,
+        external_system_name: Optional[str] = None,
+        **kwargs
     ):
-        if network_session is None:
-            network_session = NetworkSession()
-        self.auth = auth
-        self.network_session = network_session
-
-    def get_file_tasks(
-        self, file_id: str, *, extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> Tasks:
-        """
-                Retrieves a list of all the tasks for a file. This
-
-                endpoint does not support pagination.
-
-                :param file_id: The unique identifier that represents a file.
-
-        The ID for any file can be determined
-        by visiting a file in the web application
-        and copying the ID from the URL. For example,
-        for the URL `https://*.app.box.com/files/123`
-        the `file_id` is `123`.
-        Example: "12345"
-                :type file_id: str
-                :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
-                :type extra_headers: Optional[Dict[str, Optional[str]]], optional
-        """
-        if extra_headers is None:
-            extra_headers = {}
-        headers_map: Dict[str, str] = prepare_params({**extra_headers})
-        response: FetchResponse = fetch(
-            ''.join(
-                [
-                    self.network_session.base_urls.base_url,
-                    '/files/',
-                    to_string(file_id),
-                    '/tasks',
-                ]
-            ),
-            FetchOptions(
-                method='GET',
-                headers=headers_map,
-                response_format='json',
-                auth=self.auth,
-                network_session=self.network_session,
-            ),
-        )
-        return deserialize(response.data, Tasks)
-
-    def create_task(
-        self,
-        item: CreateTaskItem,
-        *,
-        action: Optional[CreateTaskAction] = None,
-        message: Optional[str] = None,
-        due_at: Optional[DateTime] = None,
-        completion_rule: Optional[CreateTaskCompletionRule] = None,
-        extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> Task:
-        """
-                Creates a single task on a file. This task is not assigned to any user and
-
-                will need to be assigned separately.
-
-                :param item: The file to attach the task to.
-                :type item: CreateTaskItem
-                :param action: The action the task assignee will be prompted to do. Must be
-
-        * `review` defines an approval task that can be approved or
-        rejected
-        * `complete` defines a general task which can be completed, defaults to None
-                :type action: Optional[CreateTaskAction], optional
-                :param message: An optional message to include with the task., defaults to None
-                :type message: Optional[str], optional
-                :param due_at: Defines when the task is due. Defaults to `null` if not
-        provided., defaults to None
-                :type due_at: Optional[DateTime], optional
-                :param completion_rule: Defines which assignees need to complete this task before the task
-        is considered completed.
-
-        * `all_assignees` (default) requires all assignees to review or
-        approve the the task in order for it to be considered completed.
-        * `any_assignee` accepts any one assignee to review or
-        approve the the task in order for it to be considered completed., defaults to None
-                :type completion_rule: Optional[CreateTaskCompletionRule], optional
-                :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
-                :type extra_headers: Optional[Dict[str, Optional[str]]], optional
-        """
-        if extra_headers is None:
-            extra_headers = {}
-        request_body: Dict = {
-            'item': item,
-            'action': action,
-            'message': message,
-            'due_at': due_at,
-            'completion_rule': completion_rule,
-        }
-        headers_map: Dict[str, str] = prepare_params({**extra_headers})
-        response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/tasks']),
-            FetchOptions(
-                method='POST',
-                headers=headers_map,
-                data=serialize(request_body),
-                content_type='application/json',
-                response_format='json',
-                auth=self.auth,
-                network_session=self.network_session,
-            ),
-        )
-        return deserialize(response.data, Task)
-
-    def get_task_by_id(
-        self, task_id: str, *, extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> Task:
-        """
-                Retrieves information about a specific task.
-                :param task_id: The ID of the task.
-        Example: "12345"
-                :type task_id: str
-                :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
-                :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
-        if extra_headers is None:
-            extra_headers = {}
-        headers_map: Dict[str, str] = prepare_params({**extra_headers})
-        response: FetchResponse = fetch(
-            ''.join(
-                [self.network_session.base_urls.base_url, '/tasks/', to_string(task_id)]
-            ),
-            FetchOptions(
-                method='GET',
-                headers=headers_map,
-                response_format='json',
-                auth=self.auth,
-                network_session=self.network_session,
-            ),
+                :param type: object type, defaults to None
+                :type type: Optional[SignRequestTypeField], optional
+                :param source_files: List of files to create a signing document from. This is currently limited to ten files. Only the ID and type fields are required for each file., defaults to None
+                :type source_files: Optional[List[FileBase]], optional
+                :param signers: Array of signers for the signature request., defaults to None
+                :type signers: Optional[List[SignRequestSigner]], optional
+                :param signature_color: Force a specific color for the signature (blue, black, or red)., defaults to None
+                :type signature_color: Optional[str], optional
+                :param id: Box Sign request ID., defaults to None
+                :type id: Optional[str], optional
+                :param prepare_url: This URL is returned if `is_document_preparation_needed` is
+        set to `true` for Box Sign request. It is used to prepare a signature request
+        using the UI. The signature request is not sent until the preparation
+        phase is complete., defaults to None
+                :type prepare_url: Optional[str], optional
+                :param status: Describes the status of the signature request., defaults to None
+                :type status: Optional[SignRequestStatusField], optional
+                :param sign_files: List of files that will be signed, which are copies of the original
+        source files. A new version of these files are created as signers sign
+        and can be downloaded at any point in the signing process., defaults to None
+                :type sign_files: Optional[SignRequestSignFilesField], optional
+                :param auto_expire_at: Uses `days_valid` to calculate the date and time, in GMT, the sign request will expire if unsigned., defaults to None
+                :type auto_expire_at: Optional[DateTime], optional
+                :param is_document_preparation_needed: Indicates if the sender should receive a `prepare_url` in the response to complete document preparation using the UI., defaults to None
+                :type is_document_preparation_needed: Optional[bool], optional
+                :param redirect_url: When specified, the signature request will be redirected to this url when a document is signed., defaults to None
+                :type redirect_url: Optional[str], optional
+                :param declined_redirect_url: The uri that a signer will be redirected to after declining to sign a document., defaults to None
+                :type declined_redirect_url: Optional[str], optional
+                :param are_text_signatures_enabled: Disables the usage of signatures generated by typing (text)., defaults to None
+                :type are_text_signatures_enabled: Optional[bool], optional
+                :param email_subject: Subject of sign request email. This is cleaned by sign request. If this field is not passed, a default subject will be used., defaults to None
+                :type email_subject: Optional[str], optional
+                :param email_message: Message to include in sign request email. The field is cleaned through sanitization of specific characters. However, some html tags are allowed. Links included in the message are also converted to hyperlinks in the email. The message may contain the following html tags including `a`, `abbr`, `acronym`, `b`, `blockquote`, `code`, `em`, `i`, `ul`, `li`, `ol`, and `strong`. Be aware that when the text to html ratio is too high, the email may end up in spam filters. Custom styles on these tags are not allowed. If this field is not passed, a default message will be used., defaults to None
+                :type email_message: Optional[str], optional
+                :param are_reminders_enabled: Reminds signers to sign a document on day 3, 8, 13 and 18. Reminders are only sent to outstanding signers., defaults to None
+                :type are_reminders_enabled: Optional[bool], optional
+                :param name: Name of the signature request., defaults to None
+                :type name: Optional[str], optional
+                :param prefill_tags: When a document contains sign-related tags in the content, you can prefill them using this `prefill_tags` by referencing the 'id' of the tag as the `external_id` field of the prefill tag., defaults to None
+                :type prefill_tags: Optional[List[SignRequestPrefillTag]], optional
+                :param days_valid: Set the number of days after which the created signature request will automatically expire if not completed. By default, we do not apply any expiration date on signature requests, and the signature request does not expire., defaults to None
+                :type days_valid: Optional[int], optional
+                :param external_id: This can be used to reference an ID in an external system that the sign request is related to., defaults to None
+                :type external_id: Optional[str], optional
+                :param is_phone_verification_required_to_view: Forces signers to verify a text message prior to viewing the document. You must specify the phone number of signers to have this setting apply to them., defaults to None
+                :type is_phone_verification_required_to_view: Optional[bool], optional
+                :param template_id: When a signature request is created from a template this field will indicate the id of that template., defaults to None
+                :type template_id: Optional[str], optional
+                :param external_system_name: Used as an optional system name to appear in the signature log next to the signers who have been assigned an `embed_url_external_id`, defaults to None
+                :type external_system_name: Optional[str], optional
+        """
+        super().__init__(
+            is_document_preparation_needed=is_document_preparation_needed,
+            redirect_url=redirect_url,
+            declined_redirect_url=declined_redirect_url,
+            are_text_signatures_enabled=are_text_signatures_enabled,
+            email_subject=email_subject,
+            email_message=email_message,
+            are_reminders_enabled=are_reminders_enabled,
+            name=name,
+            prefill_tags=prefill_tags,
+            days_valid=days_valid,
+            external_id=external_id,
+            is_phone_verification_required_to_view=is_phone_verification_required_to_view,
+            template_id=template_id,
+            external_system_name=external_system_name,
+            **kwargs
         )
-        return deserialize(response.data, Task)
-
-    def update_task_by_id(
-        self,
-        task_id: str,
-        *,
-        action: Optional[UpdateTaskByIdAction] = None,
-        message: Optional[str] = None,
-        due_at: Optional[DateTime] = None,
-        completion_rule: Optional[UpdateTaskByIdCompletionRule] = None,
-        extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> Task:
-        """
-                Updates a task. This can be used to update a task's configuration, or to
-
-                update its completion state.
-
-                :param task_id: The ID of the task.
-        Example: "12345"
-                :type task_id: str
-                :param action: The action the task assignee will be prompted to do. Must be
-
-        * `review` defines an approval task that can be approved or
-        rejected
-        * `complete` defines a general task which can be completed, defaults to None
-                :type action: Optional[UpdateTaskByIdAction], optional
-                :param message: The message included with the task., defaults to None
-                :type message: Optional[str], optional
-                :param due_at: When the task is due at., defaults to None
-                :type due_at: Optional[DateTime], optional
-                :param completion_rule: Defines which assignees need to complete this task before the task
-        is considered completed.
-
-        * `all_assignees` (default) requires all assignees to review or
-        approve the the task in order for it to be considered completed.
-        * `any_assignee` accepts any one assignee to review or
-        approve the the task in order for it to be considered completed., defaults to None
-                :type completion_rule: Optional[UpdateTaskByIdCompletionRule], optional
-                :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
-                :type extra_headers: Optional[Dict[str, Optional[str]]], optional
-        """
-        if extra_headers is None:
-            extra_headers = {}
-        request_body: Dict = {
-            'action': action,
-            'message': message,
-            'due_at': due_at,
-            'completion_rule': completion_rule,
-        }
-        headers_map: Dict[str, str] = prepare_params({**extra_headers})
-        response: FetchResponse = fetch(
-            ''.join(
-                [self.network_session.base_urls.base_url, '/tasks/', to_string(task_id)]
-            ),
-            FetchOptions(
-                method='PUT',
-                headers=headers_map,
-                data=serialize(request_body),
-                content_type='application/json',
-                response_format='json',
-                auth=self.auth,
-                network_session=self.network_session,
-            ),
-        )
-        return deserialize(response.data, Task)
-
-    def delete_task_by_id(
-        self, task_id: str, *, extra_headers: Optional[Dict[str, Optional[str]]] = None
-    ) -> None:
-        """
-                Removes a task from a file.
-                :param task_id: The ID of the task.
-        Example: "12345"
-                :type task_id: str
-                :param extra_headers: Extra headers that will be included in the HTTP request., defaults to None
-                :type extra_headers: Optional[Dict[str, Optional[str]]], optional
-        """
-        if extra_headers is None:
-            extra_headers = {}
-        headers_map: Dict[str, str] = prepare_params({**extra_headers})
-        response: FetchResponse = fetch(
-            ''.join(
-                [self.network_session.base_urls.base_url, '/tasks/', to_string(task_id)]
-            ),
-            FetchOptions(
-                method='DELETE',
-                headers=headers_map,
-                response_format=None,
-                auth=self.auth,
-                network_session=self.network_session,
-            ),
-        )
-        return None
+        self.type = type
+        self.source_files = source_files
+        self.signers = signers
+        self.signature_color = signature_color
+        self.id = id
+        self.prepare_url = prepare_url
+        self.signing_log = signing_log
+        self.status = status
+        self.sign_files = sign_files
+        self.auto_expire_at = auto_expire_at
+        self.parent_folder = parent_folder
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/terms_of_service_user_statuses.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/terms_of_service_user_statuses.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import TermsOfServiceUserStatuses
+from box_sdk_gen.schemas.terms_of_service_user_statuses import (
+    TermsOfServiceUserStatuses,
+)
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import TermsOfServiceUserStatus
+from box_sdk_gen.schemas.terms_of_service_user_status import TermsOfServiceUserStatus
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -129,15 +131,15 @@
             {'tos_id': to_string(tos_id), 'user_id': to_string(user_id)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/terms_of_service_user_statuses',
+                    '/2.0/terms_of_service_user_statuses',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
@@ -170,15 +172,15 @@
             extra_headers = {}
         request_body: Dict = {'tos': tos, 'user': user, 'is_accepted': is_accepted}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/terms_of_service_user_statuses',
+                    '/2.0/terms_of_service_user_statuses',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
@@ -210,15 +212,15 @@
             extra_headers = {}
         request_body: Dict = {'is_accepted': is_accepted}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/terms_of_service_user_statuses/',
+                    '/2.0/terms_of_service_user_statuses/',
                     to_string(terms_of_service_user_status_id),
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
                 data=serialize(request_body),
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/terms_of_services.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/terms_of_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import TermsOfServices
+from box_sdk_gen.schemas.terms_of_services import TermsOfServices
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import TermsOfService
+from box_sdk_gen.schemas.terms_of_service import TermsOfService
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -88,15 +88,17 @@
         if extra_headers is None:
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params(
             {'tos_type': to_string(tos_type)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/terms_of_services']),
+            ''.join(
+                [self.network_session.base_urls.base_url, '/2.0/terms_of_services']
+            ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
@@ -130,15 +132,17 @@
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         request_body: Dict = {'status': status, 'tos_type': tos_type, 'text': text}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/terms_of_services']),
+            ''.join(
+                [self.network_session.base_urls.base_url, '/2.0/terms_of_services']
+            ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
                 auth=self.auth,
@@ -164,15 +168,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/terms_of_services/',
+                    '/2.0/terms_of_services/',
                     to_string(terms_of_service_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
@@ -208,15 +212,15 @@
             extra_headers = {}
         request_body: Dict = {'status': status, 'text': text}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/terms_of_services/',
+                    '/2.0/terms_of_services/',
                     to_string(terms_of_service_id),
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
                 data=serialize(request_body),
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/transfer.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import FolderFull
+from box_sdk_gen.schemas.folder_full import FolderFull
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -165,15 +165,15 @@
             {'fields': to_string(fields), 'notify': to_string(notify)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/users/',
+                    '/2.0/users/',
                     to_string(user_id),
                     '/folders/0',
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 params=query_params_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/trashed_files.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/trashed_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import TrashFileRestored
+from box_sdk_gen.schemas.trash_file_restored import TrashFileRestored
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import TrashFile
+from box_sdk_gen.schemas.trash_file import TrashFile
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -105,15 +105,19 @@
         if extra_headers is None:
             extra_headers = {}
         request_body: Dict = {'name': name, 'parent': parent}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/files/', to_string(file_id)]
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/files/',
+                    to_string(file_id),
+                ]
             ),
             FetchOptions(
                 method='POST',
                 params=query_params_map,
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
@@ -183,15 +187,15 @@
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/trash',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
@@ -226,15 +230,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/trash',
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/trashed_folders.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/trashed_folders.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import TrashFolderRestored
+from box_sdk_gen.schemas.trash_folder_restored import TrashFolderRestored
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import TrashFolder
+from box_sdk_gen.schemas.trash_folder import TrashFolder
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -128,15 +128,15 @@
         request_body: Dict = {'name': name, 'parent': parent}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                 ]
             ),
             FetchOptions(
                 method='POST',
                 params=query_params_map,
                 headers=headers_map,
@@ -211,15 +211,15 @@
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                     '/trash',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
@@ -260,15 +260,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/folders/',
+                    '/2.0/folders/',
                     to_string(folder_id),
                     '/trash',
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/trashed_items.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/trashed_items.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 from typing import Dict
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import Items
+from box_sdk_gen.schemas.items import Items
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -147,15 +147,17 @@
                 'marker': to_string(marker),
                 'direction': to_string(direction),
                 'sort': to_string(sort),
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/folders/trash/items']),
+            ''.join(
+                [self.network_session.base_urls.base_url, '/2.0/folders/trash/items']
+            ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/trashed_web_links.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/trashed_web_links.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import TrashWebLinkRestored
+from box_sdk_gen.schemas.trash_web_link_restored import TrashWebLinkRestored
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import TrashWebLink
+from box_sdk_gen.schemas.trash_web_link import TrashWebLink
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -101,15 +101,15 @@
         request_body: Dict = {'name': name, 'parent': parent}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/web_links/',
+                    '/2.0/web_links/',
                     to_string(web_link_id),
                 ]
             ),
             FetchOptions(
                 method='POST',
                 params=query_params_map,
                 headers=headers_map,
@@ -151,15 +151,15 @@
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/web_links/',
+                    '/2.0/web_links/',
                     to_string(web_link_id),
                     '/trash',
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
@@ -191,15 +191,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/web_links/',
+                    '/2.0/web_links/',
                     to_string(web_link_id),
                     '/trash',
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/uploads.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/uploads.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import Files
+from box_sdk_gen.schemas.files import Files
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import UploadUrl
+from box_sdk_gen.schemas.upload_url import UploadUrl
 
-from box_sdk_gen.schemas import ConflictError
+from box_sdk_gen.schemas.conflict_error import ConflictError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -233,15 +233,15 @@
                 **extra_headers,
             }
         )
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.upload_url,
-                    '/files/',
+                    '/2.0/files/',
                     to_string(file_id),
                     '/content',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 params=query_params_map,
@@ -346,15 +346,15 @@
             'file_content_type': file_content_type,
         }
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params(
             {'content-md5': to_string(content_md_5), **extra_headers}
         )
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.upload_url, '/files/content']),
+            ''.join([self.network_session.base_urls.upload_url, '/2.0/files/content']),
             FetchOptions(
                 method='POST',
                 params=query_params_map,
                 headers=headers_map,
                 multipart_data=[
                     MultipartItem(
                         part_name='attributes',
@@ -396,15 +396,15 @@
         :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         request_body: Dict = {'name': name, 'size': size, 'parent': parent}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/files/content']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/files/content']),
             FetchOptions(
                 method='OPTIONS',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
                 auth=self.auth,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/user_collaborations.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/user_collaborations.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import Collaboration
+from box_sdk_gen.schemas.collaboration import Collaboration
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -171,15 +171,15 @@
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/collaborations/',
+                    '/2.0/collaborations/',
                     to_string(collaboration_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
@@ -257,15 +257,15 @@
             'can_view_path': can_view_path,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/collaborations/',
+                    '/2.0/collaborations/',
                     to_string(collaboration_id),
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
                 data=serialize(request_body),
@@ -294,15 +294,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/collaborations/',
+                    '/2.0/collaborations/',
                     to_string(collaboration_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
@@ -420,15 +420,15 @@
             'expires_at': expires_at,
         }
         query_params_map: Dict[str, str] = prepare_params(
             {'fields': to_string(fields), 'notify': to_string(notify)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/collaborations']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/collaborations']),
             FetchOptions(
                 method='POST',
                 params=query_params_map,
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/users.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/users.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 
 from box_sdk_gen.internal.utils import to_string
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import Users
+from box_sdk_gen.schemas.users import Users
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import UserFull
+from box_sdk_gen.schemas.user_full import UserFull
 
-from box_sdk_gen.schemas import TrackingCode
+from box_sdk_gen.schemas.tracking_code import TrackingCode
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -196,15 +196,15 @@
                 'limit': to_string(limit),
                 'usemarker': to_string(usemarker),
                 'marker': to_string(marker),
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/users']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/users']),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
@@ -326,15 +326,15 @@
             'is_exempt_from_login_verification': is_exempt_from_login_verification,
             'status': status,
             'external_app_user_id': external_app_user_id,
         }
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/users']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/users']),
             FetchOptions(
                 method='POST',
                 params=query_params_map,
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
@@ -384,15 +384,15 @@
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/users/me']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/users/me']),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
@@ -451,15 +451,19 @@
         """
         if extra_headers is None:
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/users/', to_string(user_id)]
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/users/',
+                    to_string(user_id),
+                ]
             ),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
@@ -609,15 +613,19 @@
             'notification_email': notification_email,
             'external_app_user_id': external_app_user_id,
         }
         query_params_map: Dict[str, str] = prepare_params({'fields': to_string(fields)})
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/users/', to_string(user_id)]
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/users/',
+                    to_string(user_id),
+                ]
             ),
             FetchOptions(
                 method='PUT',
                 params=query_params_map,
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
@@ -663,15 +671,19 @@
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params(
             {'notify': to_string(notify), 'force': to_string(force)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
-                [self.network_session.base_urls.base_url, '/users/', to_string(user_id)]
+                [
+                    self.network_session.base_urls.base_url,
+                    '/2.0/users/',
+                    to_string(user_id),
+                ]
             ),
             FetchOptions(
                 method='DELETE',
                 params=query_params_map,
                 headers=headers_map,
                 response_format=None,
                 auth=self.auth,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/web_links.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/web_links.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from box_sdk_gen.internal.utils import to_string
 
-from box_sdk_gen.schemas import WebLink
+from box_sdk_gen.schemas.web_link import WebLink
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -157,15 +157,15 @@
             'url': url,
             'parent': parent,
             'name': name,
             'description': description,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/web_links']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/web_links']),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
                 auth=self.auth,
@@ -205,15 +205,15 @@
         headers_map: Dict[str, str] = prepare_params(
             {'boxapi': to_string(boxapi), **extra_headers}
         )
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/web_links/',
+                    '/2.0/web_links/',
                     to_string(web_link_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
@@ -261,15 +261,15 @@
             'shared_link': shared_link,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/web_links/',
+                    '/2.0/web_links/',
                     to_string(web_link_id),
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
                 data=serialize(request_body),
@@ -298,15 +298,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/web_links/',
+                    '/2.0/web_links/',
                     to_string(web_link_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/webhooks.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/webhooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from typing import List
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import Webhooks
+from box_sdk_gen.schemas.webhooks import Webhooks
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import Webhook
+from box_sdk_gen.schemas.webhook import Webhook
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -225,15 +225,15 @@
         if extra_headers is None:
             extra_headers = {}
         query_params_map: Dict[str, str] = prepare_params(
             {'marker': to_string(marker), 'limit': to_string(limit)}
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/webhooks']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/webhooks']),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
@@ -266,15 +266,15 @@
         request_body: Dict = {
             'target': target,
             'address': address,
             'triggers': triggers,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/webhooks']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/webhooks']),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
                 auth=self.auth,
@@ -300,15 +300,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/webhooks/',
+                    '/2.0/webhooks/',
                     to_string(webhook_id),
                 ]
             ),
             FetchOptions(
                 method='GET',
                 headers=headers_map,
                 response_format='json',
@@ -350,15 +350,15 @@
             'triggers': triggers,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/webhooks/',
+                    '/2.0/webhooks/',
                     to_string(webhook_id),
                 ]
             ),
             FetchOptions(
                 method='PUT',
                 headers=headers_map,
                 data=serialize(request_body),
@@ -387,15 +387,15 @@
         if extra_headers is None:
             extra_headers = {}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/webhooks/',
+                    '/2.0/webhooks/',
                     to_string(webhook_id),
                 ]
             ),
             FetchOptions(
                 method='DELETE',
                 headers=headers_map,
                 response_format=None,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/workflows.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/workflows.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
 from typing import List
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
-from box_sdk_gen.schemas import Workflows
+from box_sdk_gen.schemas.workflows import Workflows
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import Outcome
+from box_sdk_gen.schemas.outcome import Outcome
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -173,15 +173,15 @@
                 'trigger_type': to_string(trigger_type),
                 'limit': to_string(limit),
                 'marker': to_string(marker),
             }
         )
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/workflows']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/workflows']),
             FetchOptions(
                 method='GET',
                 params=query_params_map,
                 headers=headers_map,
                 response_format='json',
                 auth=self.auth,
                 network_session=self.network_session,
@@ -235,15 +235,15 @@
             'outcomes': outcomes,
         }
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
             ''.join(
                 [
                     self.network_session.base_urls.base_url,
-                    '/workflows/',
+                    '/2.0/workflows/',
                     to_string(workflow_id),
                     '/start',
                 ]
             ),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/managers/zip_downloads.py` & `box_sdk_gen-1.0.0/box_sdk_gen/managers/zip_downloads.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 from typing import Dict
 
 from box_sdk_gen.serialization.json.serializer import serialize
 
 from box_sdk_gen.serialization.json.serializer import deserialize
 
-from box_sdk_gen.schemas import ZipDownload
+from box_sdk_gen.schemas.zip_download import ZipDownload
 
-from box_sdk_gen.schemas import ClientError
+from box_sdk_gen.schemas.client_error import ClientError
 
-from box_sdk_gen.schemas import ZipDownloadRequest
+from box_sdk_gen.schemas.zip_download_request import ZipDownloadRequest
 
-from box_sdk_gen.schemas import ZipDownloadStatus
+from box_sdk_gen.schemas.zip_download_status import ZipDownloadStatus
 
 from box_sdk_gen.networking.auth import Authentication
 
 from box_sdk_gen.networking.network import NetworkSession
 
 from box_sdk_gen.internal.utils import prepare_params
 
@@ -153,15 +153,15 @@
                 :type extra_headers: Optional[Dict[str, Optional[str]]], optional
         """
         if extra_headers is None:
             extra_headers = {}
         request_body: Dict = {'items': items, 'download_file_name': download_file_name}
         headers_map: Dict[str, str] = prepare_params({**extra_headers})
         response: FetchResponse = fetch(
-            ''.join([self.network_session.base_urls.base_url, '/zip_downloads']),
+            ''.join([self.network_session.base_urls.base_url, '/2.0/zip_downloads']),
             FetchOptions(
                 method='POST',
                 headers=headers_map,
                 data=serialize(request_body),
                 content_type='application/json',
                 response_format='json',
                 auth=self.auth,
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/networking/auth.py` & `box_sdk_gen-1.0.0/box_sdk_gen/networking/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional
 
 from abc import abstractmethod
 
 from typing import List
 
-from box_sdk_gen.schemas import AccessToken
+from box_sdk_gen.schemas.access_token import AccessToken
 
 from box_sdk_gen.networking.network import NetworkSession
 
 
 class Authentication:
     def __init__(self):
         pass
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/networking/base_urls.py` & `box_sdk_gen-1.0.0/box_sdk_gen/networking/base_urls.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,16 +12,16 @@
         'oauth2_url': 'oauth_2_url',
         **BaseObject._json_to_fields_mapping,
     }
 
     def __init__(
         self,
         *,
-        base_url: str = 'https://api.box.com/2.0',
-        upload_url: str = 'https://upload.box.com/api/2.0',
+        base_url: str = 'https://api.box.com',
+        upload_url: str = 'https://upload.box.com/api',
         oauth_2_url: str = 'https://account.box.com/api/oauth2',
         **kwargs
     ):
         super().__init__(**kwargs)
         self.base_url = base_url
         self.upload_url = upload_url
         self.oauth_2_url = oauth_2_url
```

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/networking/fetch.py` & `box_sdk_gen-1.0.0/box_sdk_gen/networking/fetch.py`

 * *Files identical despite different names*

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/networking/network.py` & `box_sdk_gen-1.0.0/box_sdk_gen/networking/network.py`

 * *Files identical despite different names*

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen/serialization/json/serializer.py` & `box_sdk_gen-1.0.0/box_sdk_gen/serialization/json/serializer.py`

 * *Files identical despite different names*

### Comparing `box_sdk_gen-0.6.5/box_sdk_gen.egg-info/PKG-INFO` & `box_sdk_gen-1.0.0/box_sdk_gen.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: box-sdk-gen
-Version: 0.6.5
+Version: 1.0.0
 Summary: [Box Platform](https://box.dev) provides functionality to provide access to content stored within [Box](https://box.com). It provides endpoints for basic manipulation of files and folders, management of users within an enterprise, as well as more complex topics such as legal holds and retention policies.
 Home-page: https://github.com/box/box-python-sdk-gen.git
 Author: Box
 Author-email: oss@box.com
 License: Apache-2.0, http://www.apache.org/licenses/LICENSE-2.0
 Keywords: box,sdk,api,rest,boxsdk
 Classifier: Development Status :: 4 - Beta
@@ -41,15 +41,22 @@
 
 <p align="center">
   <img src="https://github.com/box/sdks/blob/master/images/box-dev-logo.png" alt= “box-dev-logo” width="30%" height="50%">
 </p>
 
 # Box Python SDK GENERATED
 
-We are excited to introduce the latest generation (currently in Beta) of Box Python SDK, designed to elevate the developer experience and streamline your integration with the Box Content Cloud.
+[![Project Status](http://opensource.box.com/badges/active.svg)](http://opensource.box.com/badges)
+![build](https://github.com/box/box-python-sdk-gen/actions/workflows/build.yml/badge.svg)
+[![PyPI version](https://badge.fury.io/py/box-sdk-gen.svg)](https://badge.fury.io/py/box-sdk-gen)
+[![image](https://img.shields.io/pypi/dm/box-sdk-gen.svg)](https://pypi.python.org/pypi/box-sdk-gen)
+![Platform](https://img.shields.io/badge/python-3.8+-blue)
+[![Coverage](https://coveralls.io/repos/github/box/box-python-sdk-gen/badge.svg?branch=main)](https://coveralls.io/github/box/box-python-sdk-gen?branch=main)
+
+We are excited to introduce the stable release of the latest generation of Box Python SDK, designed to elevate the developer experience and streamline your integration with the Box Content Cloud.
 
 With this SDK, you’ll have access to:
 
 1. Full API Support: The new generation of Box SDKs empowers developers with complete coverage of the Box API ecosystem. You can now access all the latest features and functionalities offered by Box, allowing you to build even more sophisticated and feature-rich applications.
 2. Rapid API Updates: Say goodbye to waiting for new Box APIs to be incorporated into the SDK. With our new auto-generation development approach, we can now add new Box APIs to the SDK at a much faster pace (in a matter of days). This means you can leverage the most up-to-date features in your applications without delay.
 3. Embedded Documentation: We understand that easy access to information is crucial for developers. With our new approach, we have included comprehensive documentation for all objects and parameters directly in the source code of the SDK. This means you no longer need to look up this information on the developer portal, saving you time and streamlining your development process.
 4. Enhanced Convenience Methods: Our commitment to enhancing your development experience continues with the introduction of convenience methods. These methods cover various aspects such as chunk uploads, classification, and much more.
@@ -60,14 +67,16 @@
 # Table of contents
 
 <!-- START doctoc generated TOC please keep comment here to allow auto update -->
 <!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
 
 - [Installing](#installing)
 - [Getting Started](#getting-started)
+- [Documentation](#documentation)
+- [Upgrades](#upgrades)
 - [Integration Tests](#integration-tests)
   - [Running integration tests locally](#running-integration-tests-locally)
     - [Create Custom Application](#create-custom-application)
     - [Export configuration](#export-configuration)
     - [Running tests](#running-tests)
 - [Questions, Bugs, and Feature Requests?](#questions-bugs-and-feature-requests)
 - [Copyright and License](#copyright-and-license)
@@ -76,15 +85,15 @@
 
 # Installing
 
 ```console
 pip install box-sdk-gen
 ```
 
-This is autogenerated Box SDK Beta version.
+This is autogenerated Box SDK version.
 Supported Python versions are Python 3.8 and above.
 
 To install also extra dependencies required for JWT authentication, use command:
 
 ```console
 pip install box-sdk-gen[jwt]
 ```
@@ -109,14 +118,22 @@
     for item in client.folders.get_folder_items('0').entries:
         print(item.name)
 
 if __name__ == '__main__':
     main('INSERT YOUR DEVELOPER TOKEN HERE')
 ```
 
+# Documentation
+
+Browse the [docs](docs/README.md) or see [API Reference](https://developer.box.com/reference/) for more information.
+
+# Upgrades
+
+Upgrading from our legacy SDKs to the new generation SDKs is a straightforward process. See our [migration guide](migration-guide.md) and [changelog](CHANGELOG.md) for more information.
+
 # Integration Tests
 
 ## Running integration tests locally
 
 ### Create Custom Application
 
 To run integration tests locally you will need a `Custom App` created in the [Box Developer
```

### Comparing `box_sdk_gen-0.6.5/setup.py` & `box_sdk_gen-1.0.0/setup.py`

 * *Files identical despite different names*

