# Comparing `tmp/strongdm-8.3.0.zip` & `tmp/strongdm-8.4.0.zip`

## zipinfo {}

```diff
@@ -1,132 +1,132 @@
-Zip file size: 379424 bytes, number of entries: 130
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 15:52 strongdm-8.3.0/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 15:52 strongdm-8.3.0/strongdm.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 15:52 strongdm-8.3.0/strongdm/
--rw-r--r--  2.0 unx       38 b- defN 24-May-09 15:52 strongdm-8.3.0/setup.cfg
--rw-r--r--  2.0 unx    11342 b- defN 24-May-09 15:52 strongdm-8.3.0/LICENSE
--rw-r--r--  2.0 unx     3599 b- defN 24-May-09 15:52 strongdm-8.3.0/PKG-INFO
--rw-r--r--  2.0 unx     1908 b- defN 24-May-09 15:52 strongdm-8.3.0/setup.py
--rw-r--r--  2.0 unx     2875 b- defN 24-May-09 15:52 strongdm-8.3.0/README.md
--rw-r--r--  2.0 unx       50 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm.egg-info/requires.txt
--rw-r--r--  2.0 unx     4399 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx        9 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm.egg-info/top_level.txt
--rw-r--r--  2.0 unx     3599 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm.egg-info/PKG-INFO
--rw-r--r--  2.0 unx     8165 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/workflow_approvers_pb2_grpc.py
--rw-r--r--  2.0 unx    16079 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/workflow_roles_pb2.py
--rwxr-xr-x  2.0 unx    18845 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/constants.py
--rw-r--r--  2.0 unx     3417 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/access_requests_history_pb2_grpc.py
--rw-r--r--  2.0 unx    29031 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/accounts_pb2.py
--rw-r--r--  2.0 unx    19858 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/remote_identities_pb2.py
--rw-r--r--  2.0 unx     3434 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/account_resources_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3505 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/workflow_approvers_history_pb2_grpc.py
--rw-r--r--  2.0 unx     6598 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/control_panel_pb2_grpc.py
--rw-r--r--  2.0 unx     3420 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/queries_pb2_grpc.py
--rw-r--r--  2.0 unx     9416 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/approval_workflow_approvers_history_pb2.py
--rw-r--r--  2.0 unx     7980 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/account_grants_pb2_grpc.py
--rw-r--r--  2.0 unx     3361 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/replays_pb2_grpc.py
--rw-r--r--  2.0 unx     3561 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/remote_identity_groups_history_pb2_grpc.py
--rw-r--r--  2.0 unx      741 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/spec_pb2_grpc.py
--rw-r--r--  2.0 unx     3493 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/account_attachments_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3704 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py
--rw-r--r--  2.0 unx    16380 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/peering_group_nodes_pb2.py
--rw-r--r--  2.0 unx     8404 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/approval_workflow_steps_pb2_grpc.py
--rw-r--r--  2.0 unx     3322 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/secret_stores_history_pb2_grpc.py
--rw-r--r--  2.0 unx    15297 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/peering_groups_pb2.py
--rw-r--r--  2.0 unx     8901 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/account_attachments_history_pb2.py
--rw-r--r--  2.0 unx     8961 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/workflow_assignments_history_pb2.py
--rw-r--r--  2.0 unx     8138 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/accounts_history_pb2.py
--rw-r--r--  2.0 unx     9042 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/roles_pb2_grpc.py
--rw-r--r--  2.0 unx     5092 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/activities_pb2_grpc.py
--rw-r--r--  2.0 unx      741 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/options_pb2_grpc.py
--rw-r--r--  2.0 unx    18385 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/roles_pb2.py
--rw-r--r--  2.0 unx     8546 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/peering_group_resources_pb2_grpc.py
--rw-r--r--  2.0 unx    17204 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/workflow_approvers_pb2.py
--rw-r--r--  2.0 unx     8773 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/account_resources_history_pb2.py
--rw-r--r--  2.0 unx     3557 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/access_request_events_history_pb2_grpc.py
--rw-r--r--  2.0 unx    27237 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/client.py
--rw-r--r--  2.0 unx     4600 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/tags_pb2.py
--rw-r--r--  2.0 unx     9971 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/remote_identity_groups_pb2.py
--rw-r--r--  2.0 unx     8983 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/access_request_events_history_pb2.py
--rw-r--r--  2.0 unx     8792 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/approval_workflows_history_pb2.py
--rw-r--r--  2.0 unx    15576 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/access_requests_pb2.py
--rw-r--r--  2.0 unx      808 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/__init__.py
--rw-r--r--  2.0 unx    12455 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/resources_pb2_grpc.py
--rw-r--r--  2.0 unx     7932 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/peering_groups_pb2_grpc.py
--rw-r--r--  2.0 unx    22207 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/resources_pb2.py
--rw-r--r--  2.0 unx    15880 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/spec_pb2.py
--rw-r--r--  2.0 unx     3111 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/roles_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3479 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/workflow_assignments_pb2_grpc.py
--rw-r--r--  2.0 unx     2196 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/errors.py
--rw-r--r--  2.0 unx     3198 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/accounts_history_pb2_grpc.py
--rw-r--r--  2.0 unx    17214 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/secret_stores_pb2.py
--rw-r--r--  2.0 unx     8255 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/peering_group_nodes_pb2_grpc.py
--rw-r--r--  2.0 unx    17173 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/peering_group_resources_pb2.py
--rw-r--r--  2.0 unx   893989 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/drivers_pb2.py
--rw-r--r--  2.0 unx     9758 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/accounts_pb2_grpc.py
--rw-r--r--  2.0 unx     8412 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/secret_stores_history_pb2.py
--rw-r--r--  2.0 unx     3353 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/account_grants_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8708 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/approval_workflow_approvers_pb2_grpc.py
--rw-r--r--  2.0 unx     8808 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/workflow_approvers_history_pb2.py
--rw-r--r--  2.0 unx     7476 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/role_resources_pb2.py
--rw-r--r--  2.0 unx     8167 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/peering_group_peers_pb2_grpc.py
--rw-r--r--  2.0 unx     9665 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/workflows_pb2_grpc.py
--rw-r--r--  2.0 unx      741 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/secret_store_types_pb2_grpc.py
--rw-r--r--  2.0 unx     8071 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/workflow_roles_pb2_grpc.py
--rw-r--r--  2.0 unx     9113 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/approval_workflow_steps_history_pb2.py
--rw-r--r--  2.0 unx    16300 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/activities_pb2.py
--rw-r--r--  2.0 unx     8901 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/account_resources_pb2.py
--rw-r--r--  2.0 unx     8478 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/role_resources_history_pb2.py
--rw-r--r--  2.0 unx    17034 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/organization_history_pb2.py
--rw-r--r--  2.0 unx     9790 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/remote_identities_pb2_grpc.py
--rw-r--r--  2.0 unx     6849 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/secret_store_healths_pb2_grpc.py
--rw-r--r--  2.0 unx     3320 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/organization_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8396 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/account_permissions_pb2.py
--rw-r--r--  2.0 unx   202907 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/svc.py
--rw-r--r--  2.0 unx     9960 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/approval_workflows_pb2_grpc.py
--rw-r--r--  2.0 unx     3465 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/approval_workflows_history_pb2_grpc.py
--rw-r--r--  2.0 unx    29937 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/nodes_pb2.py
--rw-r--r--  2.0 unx     3592 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/approval_workflow_steps_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8650 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/remote_identities_history_pb2.py
--rw-r--r--  2.0 unx    16584 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/account_grants_pb2.py
--rw-r--r--  2.0 unx     3350 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/role_resources_history_pb2_grpc.py
--rw-r--r--  2.0 unx     8140 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/workflows_history_pb2.py
--rw-r--r--  2.0 unx    20009 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/approval_workflows_pb2.py
--rw-r--r--  2.0 unx    16005 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/secret_store_healths_pb2.py
--rw-r--r--  2.0 unx     3390 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/workflow_roles_history_pb2_grpc.py
--rw-r--r--  2.0 unx   439312 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/plumbing.py
--rw-r--r--  2.0 unx     8646 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/access_requests_history_pb2.py
--rw-r--r--  2.0 unx      741 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/tags_pb2_grpc.py
--rw-r--r--  2.0 unx    11611 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/control_panel_pb2.py
--rw-r--r--  2.0 unx     3470 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/account_permissions_pb2_grpc.py
--rw-r--r--  2.0 unx    19200 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/queries_pb2.py
--rw-r--r--  2.0 unx     3223 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/resources_history_pb2_grpc.py
--rw-r--r--  2.0 unx    17037 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/account_attachments_pb2.py
--rw-r--r--  2.0 unx     3561 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/workflow_assignments_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3259 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/workflows_history_pb2_grpc.py
--rw-r--r--  2.0 unx    20122 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/workflows_pb2.py
--rw-r--r--  2.0 unx     7340 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/workflow_assignments_pb2.py
--rw-r--r--  2.0 unx    17070 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/approval_workflow_steps_pb2.py
--rw-r--r--  2.0 unx     8102 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/account_attachments_pb2_grpc.py
--rw-r--r--  2.0 unx     9837 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/nodes_pb2_grpc.py
--rw-r--r--  2.0 unx   801091 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/models.py
--rw-r--r--  2.0 unx     9027 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/remote_identity_groups_history_pb2.py
--rw-r--r--  2.0 unx    16423 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/peering_group_peers_pb2.py
--rw-r--r--  2.0 unx    88491 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/secret_store_types_pb2.py
--rw-r--r--  2.0 unx     3388 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/account_resources_pb2_grpc.py
--rw-r--r--  2.0 unx     7818 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/roles_history_pb2.py
--rw-r--r--  2.0 unx     8320 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/replays_pb2.py
--rw-r--r--  2.0 unx      741 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/drivers_pb2_grpc.py
--rw-r--r--  2.0 unx     9376 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/secret_stores_pb2_grpc.py
--rw-r--r--  2.0 unx     8506 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/workflow_roles_history_pb2.py
--rw-r--r--  2.0 unx    18708 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/approval_workflow_approvers_pb2.py
--rw-r--r--  2.0 unx    14958 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/options_pb2.py
--rw-r--r--  2.0 unx     3180 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/access_requests_pb2_grpc.py
--rw-r--r--  2.0 unx     3424 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/remote_identities_history_pb2_grpc.py
--rw-r--r--  2.0 unx     3295 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/role_resources_pb2_grpc.py
--rw-r--r--  2.0 unx     7818 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/nodes_history_pb2.py
--rw-r--r--  2.0 unx     8550 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/account_grants_history_pb2.py
--rw-r--r--  2.0 unx     8132 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/resources_history_pb2.py
--rw-r--r--  2.0 unx     3111 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/nodes_history_pb2_grpc.py
--rw-r--r--  2.0 unx     6176 b- defN 24-May-09 15:52 strongdm-8.3.0/strongdm/remote_identity_groups_pb2_grpc.py
-130 files, 3486620 bytes uncompressed, 356984 bytes compressed:  89.8%
+Zip file size: 380118 bytes, number of entries: 130
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 21:52 strongdm-8.4.0/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 21:52 strongdm-8.4.0/strongdm/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-20 21:52 strongdm-8.4.0/strongdm.egg-info/
+-rw-r--r--  2.0 unx     1908 b- defN 24-May-20 21:52 strongdm-8.4.0/setup.py
+-rw-r--r--  2.0 unx     2875 b- defN 24-May-20 21:52 strongdm-8.4.0/README.md
+-rw-r--r--  2.0 unx    11342 b- defN 24-May-20 21:52 strongdm-8.4.0/LICENSE
+-rw-r--r--  2.0 unx     3599 b- defN 24-May-20 21:52 strongdm-8.4.0/PKG-INFO
+-rw-r--r--  2.0 unx       38 b- defN 24-May-20 21:52 strongdm-8.4.0/setup.cfg
+-rw-r--r--  2.0 unx     2196 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/errors.py
+-rw-r--r--  2.0 unx     8404 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/approval_workflow_steps_pb2_grpc.py
+-rw-r--r--  2.0 unx     3424 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/remote_identities_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    17204 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/workflow_approvers_pb2.py
+-rw-r--r--  2.0 unx   442205 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/plumbing.py
+-rw-r--r--  2.0 unx     8646 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/access_requests_history_pb2.py
+-rw-r--r--  2.0 unx     8983 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/access_request_events_history_pb2.py
+-rw-r--r--  2.0 unx     8773 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/account_resources_history_pb2.py
+-rw-r--r--  2.0 unx     3479 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/workflow_assignments_pb2_grpc.py
+-rw-r--r--  2.0 unx     7932 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/peering_groups_pb2_grpc.py
+-rw-r--r--  2.0 unx     8132 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/resources_history_pb2.py
+-rw-r--r--  2.0 unx     3320 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/organization_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    11611 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/control_panel_pb2.py
+-rw-r--r--  2.0 unx    17173 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/peering_group_resources_pb2.py
+-rw-r--r--  2.0 unx    16079 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/workflow_roles_pb2.py
+-rw-r--r--  2.0 unx    15576 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/access_requests_pb2.py
+-rw-r--r--  2.0 unx     3505 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/workflow_approvers_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     7818 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/roles_history_pb2.py
+-rw-r--r--  2.0 unx   893989 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/drivers_pb2.py
+-rw-r--r--  2.0 unx     9837 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/nodes_pb2_grpc.py
+-rw-r--r--  2.0 unx     5092 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/activities_pb2_grpc.py
+-rw-r--r--  2.0 unx    18385 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/roles_pb2.py
+-rw-r--r--  2.0 unx    19200 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/queries_pb2.py
+-rw-r--r--  2.0 unx     3198 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/accounts_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8650 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/remote_identities_history_pb2.py
+-rw-r--r--  2.0 unx    94807 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/secret_store_types_pb2.py
+-rw-r--r--  2.0 unx    22207 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/resources_pb2.py
+-rw-r--r--  2.0 unx     7818 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/nodes_history_pb2.py
+-rw-r--r--  2.0 unx    19858 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/remote_identities_pb2.py
+-rw-r--r--  2.0 unx     8550 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/account_grants_history_pb2.py
+-rw-r--r--  2.0 unx    29937 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/nodes_pb2.py
+-rw-r--r--  2.0 unx    14958 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/options_pb2.py
+-rw-r--r--  2.0 unx     3259 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/workflows_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8071 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/workflow_roles_pb2_grpc.py
+-rw-r--r--  2.0 unx     9042 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/roles_pb2_grpc.py
+-rw-r--r--  2.0 unx    20009 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/approval_workflows_pb2.py
+-rw-r--r--  2.0 unx     8808 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/workflow_approvers_history_pb2.py
+-rw-r--r--  2.0 unx     3465 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/approval_workflows_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8546 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/peering_group_resources_pb2_grpc.py
+-rw-r--r--  2.0 unx    16300 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/activities_pb2.py
+-rw-r--r--  2.0 unx      741 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/secret_store_types_pb2_grpc.py
+-rw-r--r--  2.0 unx     3557 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/access_request_events_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8320 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/replays_pb2.py
+-rw-r--r--  2.0 unx    17034 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/organization_history_pb2.py
+-rw-r--r--  2.0 unx      741 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/options_pb2_grpc.py
+-rw-r--r--  2.0 unx     3295 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/role_resources_pb2_grpc.py
+-rw-r--r--  2.0 unx    16005 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/secret_store_healths_pb2.py
+-rw-r--r--  2.0 unx      741 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/spec_pb2_grpc.py
+-rw-r--r--  2.0 unx    16584 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/account_grants_pb2.py
+-rw-r--r--  2.0 unx     9376 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/secret_stores_pb2_grpc.py
+-rw-r--r--  2.0 unx     3111 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/roles_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     9113 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/approval_workflow_steps_history_pb2.py
+-rw-r--r--  2.0 unx     8167 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/peering_group_peers_pb2_grpc.py
+-rw-r--r--  2.0 unx     9027 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/remote_identity_groups_history_pb2.py
+-rw-r--r--  2.0 unx     3417 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/access_requests_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8478 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/role_resources_history_pb2.py
+-rw-r--r--  2.0 unx     3111 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/nodes_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8901 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/account_resources_pb2.py
+-rw-r--r--  2.0 unx   202985 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/svc.py
+-rw-r--r--  2.0 unx     8412 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/secret_stores_history_pb2.py
+-rw-r--r--  2.0 unx     8901 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/account_attachments_history_pb2.py
+-rw-r--r--  2.0 unx    15880 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/spec_pb2.py
+-rw-r--r--  2.0 unx     3353 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/account_grants_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3361 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/replays_pb2_grpc.py
+-rw-r--r--  2.0 unx     8961 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/workflow_assignments_history_pb2.py
+-rwxr-xr-x  2.0 unx    18845 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/constants.py
+-rw-r--r--  2.0 unx     9960 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/approval_workflows_pb2_grpc.py
+-rw-r--r--  2.0 unx     9971 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/remote_identity_groups_pb2.py
+-rw-r--r--  2.0 unx     7340 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/workflow_assignments_pb2.py
+-rw-r--r--  2.0 unx     3434 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/account_resources_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8140 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/workflows_history_pb2.py
+-rw-r--r--  2.0 unx    20122 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/workflows_pb2.py
+-rw-r--r--  2.0 unx     3390 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/workflow_roles_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     9758 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/accounts_pb2_grpc.py
+-rw-r--r--  2.0 unx    27237 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/client.py
+-rw-r--r--  2.0 unx      808 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/__init__.py
+-rw-r--r--  2.0 unx     3420 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/queries_pb2_grpc.py
+-rw-r--r--  2.0 unx    17037 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/account_attachments_pb2.py
+-rw-r--r--  2.0 unx    12455 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/resources_pb2_grpc.py
+-rw-r--r--  2.0 unx    18708 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/approval_workflow_approvers_pb2.py
+-rw-r--r--  2.0 unx    16423 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/peering_group_peers_pb2.py
+-rw-r--r--  2.0 unx     8138 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/accounts_history_pb2.py
+-rw-r--r--  2.0 unx     3322 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/secret_stores_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3561 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/workflow_assignments_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8255 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/peering_group_nodes_pb2_grpc.py
+-rw-r--r--  2.0 unx     8708 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/approval_workflow_approvers_pb2_grpc.py
+-rw-r--r--  2.0 unx     3223 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/resources_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     6598 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/control_panel_pb2_grpc.py
+-rw-r--r--  2.0 unx     9416 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/approval_workflow_approvers_history_pb2.py
+-rw-r--r--  2.0 unx     3592 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/approval_workflow_steps_history_pb2_grpc.py
+-rw-r--r--  2.0 unx    15297 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/peering_groups_pb2.py
+-rw-r--r--  2.0 unx     8102 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/account_attachments_pb2_grpc.py
+-rw-r--r--  2.0 unx     3350 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/role_resources_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     4600 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/tags_pb2.py
+-rw-r--r--  2.0 unx     6849 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/secret_store_healths_pb2_grpc.py
+-rw-r--r--  2.0 unx     9665 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/workflows_pb2_grpc.py
+-rw-r--r--  2.0 unx     7476 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/role_resources_pb2.py
+-rw-r--r--  2.0 unx    17070 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/approval_workflow_steps_pb2.py
+-rw-r--r--  2.0 unx   805009 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/models.py
+-rw-r--r--  2.0 unx     9790 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/remote_identities_pb2_grpc.py
+-rw-r--r--  2.0 unx    29031 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/accounts_pb2.py
+-rw-r--r--  2.0 unx      741 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/drivers_pb2_grpc.py
+-rw-r--r--  2.0 unx     8792 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/approval_workflows_history_pb2.py
+-rw-r--r--  2.0 unx    17214 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/secret_stores_pb2.py
+-rw-r--r--  2.0 unx     8506 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/workflow_roles_history_pb2.py
+-rw-r--r--  2.0 unx    16380 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/peering_group_nodes_pb2.py
+-rw-r--r--  2.0 unx     7980 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/account_grants_pb2_grpc.py
+-rw-r--r--  2.0 unx      741 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/tags_pb2_grpc.py
+-rw-r--r--  2.0 unx     3493 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/account_attachments_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     8396 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/account_permissions_pb2.py
+-rw-r--r--  2.0 unx     6176 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/remote_identity_groups_pb2_grpc.py
+-rw-r--r--  2.0 unx     3180 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/access_requests_pb2_grpc.py
+-rw-r--r--  2.0 unx     8165 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/workflow_approvers_pb2_grpc.py
+-rw-r--r--  2.0 unx     3561 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/remote_identity_groups_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3704 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py
+-rw-r--r--  2.0 unx     3388 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/account_resources_pb2_grpc.py
+-rw-r--r--  2.0 unx     3470 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm/account_permissions_pb2_grpc.py
+-rw-r--r--  2.0 unx        1 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm.egg-info/top_level.txt
+-rw-r--r--  2.0 unx       50 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm.egg-info/requires.txt
+-rw-r--r--  2.0 unx     4399 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx     3599 b- defN 24-May-20 21:52 strongdm-8.4.0/strongdm.egg-info/PKG-INFO
+130 files, 3499825 bytes uncompressed, 357678 bytes compressed:  89.8%
```

## zipnote {}

```diff
@@ -1,391 +1,391 @@
-Filename: strongdm-8.3.0/
+Filename: strongdm-8.4.0/
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm.egg-info/
+Filename: strongdm-8.4.0/strongdm/
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/
+Filename: strongdm-8.4.0/strongdm.egg-info/
 Comment: 
 
-Filename: strongdm-8.3.0/setup.cfg
+Filename: strongdm-8.4.0/setup.py
 Comment: 
 
-Filename: strongdm-8.3.0/LICENSE
+Filename: strongdm-8.4.0/README.md
 Comment: 
 
-Filename: strongdm-8.3.0/PKG-INFO
+Filename: strongdm-8.4.0/LICENSE
 Comment: 
 
-Filename: strongdm-8.3.0/setup.py
+Filename: strongdm-8.4.0/PKG-INFO
 Comment: 
 
-Filename: strongdm-8.3.0/README.md
+Filename: strongdm-8.4.0/setup.cfg
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm.egg-info/requires.txt
+Filename: strongdm-8.4.0/strongdm/errors.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm.egg-info/SOURCES.txt
+Filename: strongdm-8.4.0/strongdm/approval_workflow_steps_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm.egg-info/dependency_links.txt
+Filename: strongdm-8.4.0/strongdm/remote_identities_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm.egg-info/top_level.txt
+Filename: strongdm-8.4.0/strongdm/workflow_approvers_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm.egg-info/PKG-INFO
+Filename: strongdm-8.4.0/strongdm/plumbing.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/workflow_approvers_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/access_requests_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/workflow_roles_pb2.py
+Filename: strongdm-8.4.0/strongdm/access_request_events_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/constants.py
+Filename: strongdm-8.4.0/strongdm/account_resources_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/access_requests_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/workflow_assignments_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/accounts_pb2.py
+Filename: strongdm-8.4.0/strongdm/peering_groups_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/remote_identities_pb2.py
+Filename: strongdm-8.4.0/strongdm/resources_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/account_resources_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/organization_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/workflow_approvers_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/control_panel_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/control_panel_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/peering_group_resources_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/queries_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/workflow_roles_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/approval_workflow_approvers_history_pb2.py
+Filename: strongdm-8.4.0/strongdm/access_requests_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/account_grants_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/workflow_approvers_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/replays_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/roles_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/remote_identity_groups_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/drivers_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/spec_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/nodes_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/account_attachments_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/activities_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/roles_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/peering_group_nodes_pb2.py
+Filename: strongdm-8.4.0/strongdm/queries_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/approval_workflow_steps_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/accounts_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/secret_stores_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/remote_identities_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/peering_groups_pb2.py
+Filename: strongdm-8.4.0/strongdm/secret_store_types_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/account_attachments_history_pb2.py
+Filename: strongdm-8.4.0/strongdm/resources_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/workflow_assignments_history_pb2.py
+Filename: strongdm-8.4.0/strongdm/nodes_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/accounts_history_pb2.py
+Filename: strongdm-8.4.0/strongdm/remote_identities_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/roles_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/account_grants_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/activities_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/nodes_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/options_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/options_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/roles_pb2.py
+Filename: strongdm-8.4.0/strongdm/workflows_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/peering_group_resources_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/workflow_roles_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/workflow_approvers_pb2.py
+Filename: strongdm-8.4.0/strongdm/roles_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/account_resources_history_pb2.py
+Filename: strongdm-8.4.0/strongdm/approval_workflows_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/access_request_events_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/workflow_approvers_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/client.py
+Filename: strongdm-8.4.0/strongdm/approval_workflows_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/tags_pb2.py
+Filename: strongdm-8.4.0/strongdm/peering_group_resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/remote_identity_groups_pb2.py
+Filename: strongdm-8.4.0/strongdm/activities_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/access_request_events_history_pb2.py
+Filename: strongdm-8.4.0/strongdm/secret_store_types_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/approval_workflows_history_pb2.py
+Filename: strongdm-8.4.0/strongdm/access_request_events_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/access_requests_pb2.py
+Filename: strongdm-8.4.0/strongdm/replays_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/__init__.py
+Filename: strongdm-8.4.0/strongdm/organization_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/resources_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/options_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/peering_groups_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/role_resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/resources_pb2.py
+Filename: strongdm-8.4.0/strongdm/secret_store_healths_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/spec_pb2.py
+Filename: strongdm-8.4.0/strongdm/spec_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/roles_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/account_grants_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/workflow_assignments_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/secret_stores_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/errors.py
+Filename: strongdm-8.4.0/strongdm/roles_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/accounts_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/approval_workflow_steps_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/secret_stores_pb2.py
+Filename: strongdm-8.4.0/strongdm/peering_group_peers_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/peering_group_nodes_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/remote_identity_groups_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/peering_group_resources_pb2.py
+Filename: strongdm-8.4.0/strongdm/access_requests_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/drivers_pb2.py
+Filename: strongdm-8.4.0/strongdm/role_resources_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/accounts_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/nodes_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/secret_stores_history_pb2.py
+Filename: strongdm-8.4.0/strongdm/account_resources_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/account_grants_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/svc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/approval_workflow_approvers_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/secret_stores_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/workflow_approvers_history_pb2.py
+Filename: strongdm-8.4.0/strongdm/account_attachments_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/role_resources_pb2.py
+Filename: strongdm-8.4.0/strongdm/spec_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/peering_group_peers_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/account_grants_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/workflows_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/replays_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/secret_store_types_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/workflow_assignments_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/workflow_roles_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/constants.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/approval_workflow_steps_history_pb2.py
+Filename: strongdm-8.4.0/strongdm/approval_workflows_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/activities_pb2.py
+Filename: strongdm-8.4.0/strongdm/remote_identity_groups_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/account_resources_pb2.py
+Filename: strongdm-8.4.0/strongdm/workflow_assignments_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/role_resources_history_pb2.py
+Filename: strongdm-8.4.0/strongdm/account_resources_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/organization_history_pb2.py
+Filename: strongdm-8.4.0/strongdm/workflows_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/remote_identities_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/workflows_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/secret_store_healths_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/workflow_roles_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/organization_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/accounts_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/account_permissions_pb2.py
+Filename: strongdm-8.4.0/strongdm/client.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/svc.py
+Filename: strongdm-8.4.0/strongdm/__init__.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/approval_workflows_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/queries_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/approval_workflows_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/account_attachments_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/nodes_pb2.py
+Filename: strongdm-8.4.0/strongdm/resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/approval_workflow_steps_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/approval_workflow_approvers_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/remote_identities_history_pb2.py
+Filename: strongdm-8.4.0/strongdm/peering_group_peers_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/account_grants_pb2.py
+Filename: strongdm-8.4.0/strongdm/accounts_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/role_resources_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/secret_stores_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/workflows_history_pb2.py
+Filename: strongdm-8.4.0/strongdm/workflow_assignments_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/approval_workflows_pb2.py
+Filename: strongdm-8.4.0/strongdm/peering_group_nodes_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/secret_store_healths_pb2.py
+Filename: strongdm-8.4.0/strongdm/approval_workflow_approvers_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/workflow_roles_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/resources_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/plumbing.py
+Filename: strongdm-8.4.0/strongdm/control_panel_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/access_requests_history_pb2.py
+Filename: strongdm-8.4.0/strongdm/approval_workflow_approvers_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/tags_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/approval_workflow_steps_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/control_panel_pb2.py
+Filename: strongdm-8.4.0/strongdm/peering_groups_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/account_permissions_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/account_attachments_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/queries_pb2.py
+Filename: strongdm-8.4.0/strongdm/role_resources_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/resources_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/tags_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/account_attachments_pb2.py
+Filename: strongdm-8.4.0/strongdm/secret_store_healths_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/workflow_assignments_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/workflows_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/workflows_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/role_resources_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/workflows_pb2.py
+Filename: strongdm-8.4.0/strongdm/approval_workflow_steps_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/workflow_assignments_pb2.py
+Filename: strongdm-8.4.0/strongdm/models.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/approval_workflow_steps_pb2.py
+Filename: strongdm-8.4.0/strongdm/remote_identities_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/account_attachments_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/accounts_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/nodes_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/drivers_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/models.py
+Filename: strongdm-8.4.0/strongdm/approval_workflows_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/remote_identity_groups_history_pb2.py
+Filename: strongdm-8.4.0/strongdm/secret_stores_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/peering_group_peers_pb2.py
+Filename: strongdm-8.4.0/strongdm/workflow_roles_history_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/secret_store_types_pb2.py
+Filename: strongdm-8.4.0/strongdm/peering_group_nodes_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/account_resources_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/account_grants_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/roles_history_pb2.py
+Filename: strongdm-8.4.0/strongdm/tags_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/replays_pb2.py
+Filename: strongdm-8.4.0/strongdm/account_attachments_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/drivers_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/account_permissions_pb2.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/secret_stores_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/remote_identity_groups_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/workflow_roles_history_pb2.py
+Filename: strongdm-8.4.0/strongdm/access_requests_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/approval_workflow_approvers_pb2.py
+Filename: strongdm-8.4.0/strongdm/workflow_approvers_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/options_pb2.py
+Filename: strongdm-8.4.0/strongdm/remote_identity_groups_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/access_requests_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/remote_identities_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/account_resources_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/role_resources_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm/account_permissions_pb2_grpc.py
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/nodes_history_pb2.py
+Filename: strongdm-8.4.0/strongdm.egg-info/dependency_links.txt
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/account_grants_history_pb2.py
+Filename: strongdm-8.4.0/strongdm.egg-info/top_level.txt
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/resources_history_pb2.py
+Filename: strongdm-8.4.0/strongdm.egg-info/requires.txt
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/nodes_history_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm.egg-info/SOURCES.txt
 Comment: 
 
-Filename: strongdm-8.3.0/strongdm/remote_identity_groups_pb2_grpc.py
+Filename: strongdm-8.4.0/strongdm.egg-info/PKG-INFO
 Comment: 
 
 Zip file comment:
```

## Comparing `strongdm-8.3.0/LICENSE` & `strongdm-8.4.0/LICENSE`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/PKG-INFO` & `strongdm-8.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: strongdm
-Version: 8.3.0
+Version: 8.4.0
 Summary: strongDM SDK for the Python programming language.
 Home-page: https://github.com/strongdm/strongdm-sdk-python
 Author: strongDM Team
 Author-email: sdk-feedback@strongdm.com
 License: apache-2.0
-Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v8.3.0.tar.gz
+Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v8.4.0.tar.gz
 Keywords: strongDM,sdm,api,automation,security,audit,database,server,ssh,rdp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `strongdm-8.3.0/setup.py` & `strongdm-8.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 from setuptools import setup
 setup(
     name='strongdm',
     packages=['strongdm'],
-    version='8.3.0',
+    version='8.4.0',
     license='apache-2.0',
     description='strongDM SDK for the Python programming language.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='strongDM Team',
     author_email='sdk-feedback@strongdm.com',
     url='https://github.com/strongdm/strongdm-sdk-python',
     download_url=
-    'https://github.com/strongdm/strongdm-sdk-python/archive/v8.3.0.tar.gz',
+    'https://github.com/strongdm/strongdm-sdk-python/archive/v8.4.0.tar.gz',
     keywords=[
         'strongDM', 'sdm', 'api', 'automation', 'security', 'audit',
         'database', 'server', 'ssh', 'rdp'
     ],
     install_requires=[
         'grpcio>=1.42.0',
         'googleapis-common-protos>1.56.2,<2',
```

## Comparing `strongdm-8.3.0/README.md` & `strongdm-8.4.0/README.md`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm.egg-info/SOURCES.txt` & `strongdm-8.4.0/strongdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm.egg-info/PKG-INFO` & `strongdm-8.4.0/strongdm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: strongdm
-Version: 8.3.0
+Version: 8.4.0
 Summary: strongDM SDK for the Python programming language.
 Home-page: https://github.com/strongdm/strongdm-sdk-python
 Author: strongDM Team
 Author-email: sdk-feedback@strongdm.com
 License: apache-2.0
-Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v8.3.0.tar.gz
+Download-URL: https://github.com/strongdm/strongdm-sdk-python/archive/v8.4.0.tar.gz
 Keywords: strongDM,sdm,api,automation,security,audit,database,server,ssh,rdp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `strongdm-8.3.0/strongdm/workflow_approvers_pb2_grpc.py` & `strongdm-8.4.0/strongdm/workflow_approvers_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/workflow_roles_pb2.py` & `strongdm-8.4.0/strongdm/workflow_roles_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/constants.py` & `strongdm-8.4.0/strongdm/constants.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/access_requests_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/access_requests_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/accounts_pb2.py` & `strongdm-8.4.0/strongdm/accounts_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/remote_identities_pb2.py` & `strongdm-8.4.0/strongdm/remote_identities_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/account_resources_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/account_resources_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/workflow_approvers_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/workflow_approvers_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/control_panel_pb2_grpc.py` & `strongdm-8.4.0/strongdm/control_panel_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/queries_pb2_grpc.py` & `strongdm-8.4.0/strongdm/queries_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/approval_workflow_approvers_history_pb2.py` & `strongdm-8.4.0/strongdm/approval_workflow_approvers_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/account_grants_pb2_grpc.py` & `strongdm-8.4.0/strongdm/account_grants_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/replays_pb2_grpc.py` & `strongdm-8.4.0/strongdm/replays_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/remote_identity_groups_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/remote_identity_groups_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/spec_pb2_grpc.py` & `strongdm-8.4.0/strongdm/secret_store_types_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/account_attachments_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/account_attachments_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/approval_workflow_approvers_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/peering_group_nodes_pb2.py` & `strongdm-8.4.0/strongdm/peering_group_nodes_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/approval_workflow_steps_pb2_grpc.py` & `strongdm-8.4.0/strongdm/approval_workflow_steps_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/secret_stores_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/secret_stores_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/peering_groups_pb2.py` & `strongdm-8.4.0/strongdm/peering_groups_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/account_attachments_history_pb2.py` & `strongdm-8.4.0/strongdm/account_attachments_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/workflow_assignments_history_pb2.py` & `strongdm-8.4.0/strongdm/workflow_assignments_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/accounts_history_pb2.py` & `strongdm-8.4.0/strongdm/accounts_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/roles_pb2_grpc.py` & `strongdm-8.4.0/strongdm/roles_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/activities_pb2_grpc.py` & `strongdm-8.4.0/strongdm/activities_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/options_pb2_grpc.py` & `strongdm-8.4.0/strongdm/options_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/roles_pb2.py` & `strongdm-8.4.0/strongdm/roles_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/peering_group_resources_pb2_grpc.py` & `strongdm-8.4.0/strongdm/peering_group_resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/workflow_approvers_pb2.py` & `strongdm-8.4.0/strongdm/workflow_approvers_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/account_resources_history_pb2.py` & `strongdm-8.4.0/strongdm/account_resources_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/access_request_events_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/access_request_events_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/client.py` & `strongdm-8.4.0/strongdm/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 # These defaults are taken from AWS. Customization of these values
 # is a future step in the API.
 DEFAULT_MAX_RETRIES = 3
 DEFAULT_BASE_RETRY_DELAY = 0.0030  # 30 ms
 DEFAULT_MAX_RETRY_DELAY = 300  # 300 seconds
 API_VERSION = '2024-03-28'
-USER_AGENT = 'strongdm-sdk-python/8.3.0'
+USER_AGENT = 'strongdm-sdk-python/8.4.0'
 
 
 class Client:
     '''Client interacts with the strongDM API.'''
     def __init__(self,
                  api_access_key,
                  api_secret,
```

## Comparing `strongdm-8.3.0/strongdm/tags_pb2.py` & `strongdm-8.4.0/strongdm/tags_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/remote_identity_groups_pb2.py` & `strongdm-8.4.0/strongdm/remote_identity_groups_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/access_request_events_history_pb2.py` & `strongdm-8.4.0/strongdm/access_request_events_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/approval_workflows_history_pb2.py` & `strongdm-8.4.0/strongdm/approval_workflows_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/access_requests_pb2.py` & `strongdm-8.4.0/strongdm/access_requests_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/__init__.py` & `strongdm-8.4.0/strongdm/__init__.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/resources_pb2_grpc.py` & `strongdm-8.4.0/strongdm/resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/peering_groups_pb2_grpc.py` & `strongdm-8.4.0/strongdm/peering_groups_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/resources_pb2.py` & `strongdm-8.4.0/strongdm/resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/spec_pb2.py` & `strongdm-8.4.0/strongdm/spec_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/roles_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/roles_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/workflow_assignments_pb2_grpc.py` & `strongdm-8.4.0/strongdm/workflow_assignments_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/errors.py` & `strongdm-8.4.0/strongdm/errors.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/accounts_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/accounts_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/secret_stores_pb2.py` & `strongdm-8.4.0/strongdm/secret_stores_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/peering_group_nodes_pb2_grpc.py` & `strongdm-8.4.0/strongdm/peering_group_nodes_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/peering_group_resources_pb2.py` & `strongdm-8.4.0/strongdm/peering_group_resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/drivers_pb2.py` & `strongdm-8.4.0/strongdm/drivers_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/accounts_pb2_grpc.py` & `strongdm-8.4.0/strongdm/accounts_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/secret_stores_history_pb2.py` & `strongdm-8.4.0/strongdm/secret_stores_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/account_grants_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/account_grants_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/approval_workflow_approvers_pb2_grpc.py` & `strongdm-8.4.0/strongdm/approval_workflow_approvers_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/workflow_approvers_history_pb2.py` & `strongdm-8.4.0/strongdm/workflow_approvers_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/role_resources_pb2.py` & `strongdm-8.4.0/strongdm/role_resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/peering_group_peers_pb2_grpc.py` & `strongdm-8.4.0/strongdm/peering_group_peers_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/workflows_pb2_grpc.py` & `strongdm-8.4.0/strongdm/workflows_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/secret_store_types_pb2_grpc.py` & `strongdm-8.4.0/strongdm/spec_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/workflow_roles_pb2_grpc.py` & `strongdm-8.4.0/strongdm/workflow_roles_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/approval_workflow_steps_history_pb2.py` & `strongdm-8.4.0/strongdm/approval_workflow_steps_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/activities_pb2.py` & `strongdm-8.4.0/strongdm/activities_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/account_resources_pb2.py` & `strongdm-8.4.0/strongdm/account_resources_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/role_resources_history_pb2.py` & `strongdm-8.4.0/strongdm/role_resources_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/organization_history_pb2.py` & `strongdm-8.4.0/strongdm/organization_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/remote_identities_pb2_grpc.py` & `strongdm-8.4.0/strongdm/remote_identities_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/secret_store_healths_pb2_grpc.py` & `strongdm-8.4.0/strongdm/secret_store_healths_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/organization_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/organization_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/account_permissions_pb2.py` & `strongdm-8.4.0/strongdm/account_permissions_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/svc.py` & `strongdm-8.4.0/strongdm/svc.py`

 * *Files 0% similar despite different names*

```diff
@@ -4313,14 +4313,16 @@
     `strongdm.models.GCPStore`
     `strongdm.models.GCPCertX509Store`
     `strongdm.models.KeyfactorSSHStore`
     `strongdm.models.KeyfactorX509Store`
     `strongdm.models.VaultAppRoleStore`
     `strongdm.models.VaultAppRoleCertSSHStore`
     `strongdm.models.VaultAppRoleCertX509Store`
+    `strongdm.models.VaultAWSEC2Store`
+    `strongdm.models.VaultAWSIAMStore`
     `strongdm.models.VaultTLSStore`
     `strongdm.models.VaultTLSCertSSHStore`
     `strongdm.models.VaultTLSCertX509Store`
     `strongdm.models.VaultTokenStore`
     `strongdm.models.VaultTokenCertSSHStore`
     `strongdm.models.VaultTokenCertX509Store`
     '''
```

## Comparing `strongdm-8.3.0/strongdm/approval_workflows_pb2_grpc.py` & `strongdm-8.4.0/strongdm/approval_workflows_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/approval_workflows_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/approval_workflows_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/nodes_pb2.py` & `strongdm-8.4.0/strongdm/nodes_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/approval_workflow_steps_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/approval_workflow_steps_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/remote_identities_history_pb2.py` & `strongdm-8.4.0/strongdm/remote_identities_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/account_grants_pb2.py` & `strongdm-8.4.0/strongdm/account_grants_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/role_resources_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/role_resources_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/workflows_history_pb2.py` & `strongdm-8.4.0/strongdm/workflows_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/approval_workflows_pb2.py` & `strongdm-8.4.0/strongdm/approval_workflows_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/secret_store_healths_pb2.py` & `strongdm-8.4.0/strongdm/secret_store_healths_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/workflow_roles_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/workflow_roles_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/plumbing.py` & `strongdm-8.4.0/strongdm/plumbing.py`

 * *Files 0% similar despite different names*

```diff
@@ -9778,14 +9778,20 @@
             convert_vault_app_role_store_to_plumbing(porcelain))
     if isinstance(porcelain, models.VaultAppRoleCertSSHStore):
         plumbing.vault_app_role_cert_ssh.CopyFrom(
             convert_vault_app_role_cert_ssh_store_to_plumbing(porcelain))
     if isinstance(porcelain, models.VaultAppRoleCertX509Store):
         plumbing.vault_app_role_cert_x_509.CopyFrom(
             convert_vault_app_role_cert_x_509_store_to_plumbing(porcelain))
+    if isinstance(porcelain, models.VaultAWSEC2Store):
+        plumbing.vault_awsec_2.CopyFrom(
+            convert_vault_awsec_2_store_to_plumbing(porcelain))
+    if isinstance(porcelain, models.VaultAWSIAMStore):
+        plumbing.vault_awsiam.CopyFrom(
+            convert_vault_awsiam_store_to_plumbing(porcelain))
     if isinstance(porcelain, models.VaultTLSStore):
         plumbing.vault_tls.CopyFrom(
             convert_vault_tls_store_to_plumbing(porcelain))
     if isinstance(porcelain, models.VaultTLSCertSSHStore):
         plumbing.vault_tls_cert_ssh.CopyFrom(
             convert_vault_tls_cert_ssh_store_to_plumbing(porcelain))
     if isinstance(porcelain, models.VaultTLSCertX509Store):
@@ -9841,14 +9847,18 @@
             plumbing.vault_app_role)
     if plumbing.HasField('vault_app_role_cert_ssh'):
         return convert_vault_app_role_cert_ssh_store_to_porcelain(
             plumbing.vault_app_role_cert_ssh)
     if plumbing.HasField('vault_app_role_cert_x_509'):
         return convert_vault_app_role_cert_x_509_store_to_porcelain(
             plumbing.vault_app_role_cert_x_509)
+    if plumbing.HasField('vault_awsec_2'):
+        return convert_vault_awsec_2_store_to_porcelain(plumbing.vault_awsec_2)
+    if plumbing.HasField('vault_awsiam'):
+        return convert_vault_awsiam_store_to_porcelain(plumbing.vault_awsiam)
     if plumbing.HasField('vault_tls'):
         return convert_vault_tls_store_to_porcelain(plumbing.vault_tls)
     if plumbing.HasField('vault_tls_cert_ssh'):
         return convert_vault_tls_cert_ssh_store_to_porcelain(
             plumbing.vault_tls_cert_ssh)
     if plumbing.HasField('vault_tls_cert_x_509'):
         return convert_vault_tls_cert_x_509_store_to_porcelain(
@@ -10702,14 +10712,90 @@
     return [convert_user_to_plumbing(porcelain) for porcelain in porcelains]
 
 
 def convert_repeated_user_to_porcelain(plumbings):
     return [convert_user_to_porcelain(plumbing) for plumbing in plumbings]
 
 
+def convert_vault_awsec_2_store_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.VaultAWSEC2Store()
+    porcelain.id = (plumbing.id)
+    porcelain.name = (plumbing.name)
+    porcelain.namespace = (plumbing.namespace)
+    porcelain.server_address = (plumbing.server_address)
+    porcelain.tags = convert_tags_to_porcelain(plumbing.tags)
+    return porcelain
+
+
+def convert_vault_awsec_2_store_to_plumbing(porcelain):
+    plumbing = VaultAWSEC2Store()
+    if porcelain is None:
+        return plumbing
+    plumbing.id = (porcelain.id)
+    plumbing.name = (porcelain.name)
+    plumbing.namespace = (porcelain.namespace)
+    plumbing.server_address = (porcelain.server_address)
+    plumbing.tags.CopyFrom(convert_tags_to_plumbing(porcelain.tags))
+    return plumbing
+
+
+def convert_repeated_vault_awsec_2_store_to_plumbing(porcelains):
+    return [
+        convert_vault_awsec_2_store_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_vault_awsec_2_store_to_porcelain(plumbings):
+    return [
+        convert_vault_awsec_2_store_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
+def convert_vault_awsiam_store_to_porcelain(plumbing):
+    if plumbing is None:
+        return None
+    porcelain = models.VaultAWSIAMStore()
+    porcelain.id = (plumbing.id)
+    porcelain.name = (plumbing.name)
+    porcelain.namespace = (plumbing.namespace)
+    porcelain.server_address = (plumbing.server_address)
+    porcelain.tags = convert_tags_to_porcelain(plumbing.tags)
+    return porcelain
+
+
+def convert_vault_awsiam_store_to_plumbing(porcelain):
+    plumbing = VaultAWSIAMStore()
+    if porcelain is None:
+        return plumbing
+    plumbing.id = (porcelain.id)
+    plumbing.name = (porcelain.name)
+    plumbing.namespace = (porcelain.namespace)
+    plumbing.server_address = (porcelain.server_address)
+    plumbing.tags.CopyFrom(convert_tags_to_plumbing(porcelain.tags))
+    return plumbing
+
+
+def convert_repeated_vault_awsiam_store_to_plumbing(porcelains):
+    return [
+        convert_vault_awsiam_store_to_plumbing(porcelain)
+        for porcelain in porcelains
+    ]
+
+
+def convert_repeated_vault_awsiam_store_to_porcelain(plumbings):
+    return [
+        convert_vault_awsiam_store_to_porcelain(plumbing)
+        for plumbing in plumbings
+    ]
+
+
 def convert_vault_app_role_cert_ssh_store_to_porcelain(plumbing):
     if plumbing is None:
         return None
     porcelain = models.VaultAppRoleCertSSHStore()
     porcelain.id = (plumbing.id)
     porcelain.issuedcertttlminutes = (plumbing.issuedCertTTLMinutes)
     porcelain.name = (plumbing.name)
```

## Comparing `strongdm-8.3.0/strongdm/access_requests_history_pb2.py` & `strongdm-8.4.0/strongdm/access_requests_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/tags_pb2_grpc.py` & `strongdm-8.4.0/strongdm/drivers_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/control_panel_pb2.py` & `strongdm-8.4.0/strongdm/control_panel_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/account_permissions_pb2_grpc.py` & `strongdm-8.4.0/strongdm/account_permissions_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/queries_pb2.py` & `strongdm-8.4.0/strongdm/queries_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/resources_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/resources_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/account_attachments_pb2.py` & `strongdm-8.4.0/strongdm/account_attachments_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/workflow_assignments_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/workflow_assignments_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/workflows_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/workflows_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/workflows_pb2.py` & `strongdm-8.4.0/strongdm/workflows_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/workflow_assignments_pb2.py` & `strongdm-8.4.0/strongdm/workflow_assignments_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/approval_workflow_steps_pb2.py` & `strongdm-8.4.0/strongdm/approval_workflow_steps_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/account_attachments_pb2_grpc.py` & `strongdm-8.4.0/strongdm/account_attachments_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/nodes_pb2_grpc.py` & `strongdm-8.4.0/strongdm/nodes_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/models.py` & `strongdm-8.4.0/strongdm/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -21511,14 +21511,156 @@
             managed_by=d.get('managed_by'),
             permission_level=d.get('permission_level'),
             suspended=d.get('suspended'),
             tags=d.get('tags'),
         )
 
 
+class VaultAWSEC2Store:
+    '''
+    VaultAWSEC2Store is currently unstable, and its API may change, or it may be removed,
+    without a major version bump.
+    '''
+    __slots__ = [
+        'id',
+        'name',
+        'namespace',
+        'server_address',
+        'tags',
+    ]
+
+    def __init__(
+        self,
+        id=None,
+        name=None,
+        namespace=None,
+        server_address=None,
+        tags=None,
+    ):
+        self.id = id if id is not None else ''
+        '''
+         Unique identifier of the SecretStore.
+        '''
+        self.name = name if name is not None else ''
+        '''
+         Unique human-readable name of the SecretStore.
+        '''
+        self.namespace = namespace if namespace is not None else ''
+        '''
+         The namespace to make requests within
+        '''
+        self.server_address = server_address if server_address is not None else ''
+        '''
+         The URL of the Vault to target
+        '''
+        self.tags = tags if tags is not None else _porcelain_zero_value_tags()
+        '''
+         Tags is a map of key, value pairs.
+        '''
+
+    def __repr__(self):
+        return '<sdm.VaultAWSEC2Store ' + \
+            'id: ' + repr(self.id) + ' ' +\
+            'name: ' + repr(self.name) + ' ' +\
+            'namespace: ' + repr(self.namespace) + ' ' +\
+            'server_address: ' + repr(self.server_address) + ' ' +\
+            'tags: ' + repr(self.tags) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'id': self.id,
+            'name': self.name,
+            'namespace': self.namespace,
+            'server_address': self.server_address,
+            'tags': self.tags,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            id=d.get('id'),
+            name=d.get('name'),
+            namespace=d.get('namespace'),
+            server_address=d.get('server_address'),
+            tags=d.get('tags'),
+        )
+
+
+class VaultAWSIAMStore:
+    '''
+    VaultAWSIAMStore is currently unstable, and its API may change, or it may be removed,
+    without a major version bump.
+    '''
+    __slots__ = [
+        'id',
+        'name',
+        'namespace',
+        'server_address',
+        'tags',
+    ]
+
+    def __init__(
+        self,
+        id=None,
+        name=None,
+        namespace=None,
+        server_address=None,
+        tags=None,
+    ):
+        self.id = id if id is not None else ''
+        '''
+         Unique identifier of the SecretStore.
+        '''
+        self.name = name if name is not None else ''
+        '''
+         Unique human-readable name of the SecretStore.
+        '''
+        self.namespace = namespace if namespace is not None else ''
+        '''
+         The namespace to make requests within
+        '''
+        self.server_address = server_address if server_address is not None else ''
+        '''
+         The URL of the Vault to target
+        '''
+        self.tags = tags if tags is not None else _porcelain_zero_value_tags()
+        '''
+         Tags is a map of key, value pairs.
+        '''
+
+    def __repr__(self):
+        return '<sdm.VaultAWSIAMStore ' + \
+            'id: ' + repr(self.id) + ' ' +\
+            'name: ' + repr(self.name) + ' ' +\
+            'namespace: ' + repr(self.namespace) + ' ' +\
+            'server_address: ' + repr(self.server_address) + ' ' +\
+            'tags: ' + repr(self.tags) + ' ' +\
+            '>'
+
+    def to_dict(self):
+        return {
+            'id': self.id,
+            'name': self.name,
+            'namespace': self.namespace,
+            'server_address': self.server_address,
+            'tags': self.tags,
+        }
+
+    @classmethod
+    def from_dict(cls, d):
+        return cls(
+            id=d.get('id'),
+            name=d.get('name'),
+            namespace=d.get('namespace'),
+            server_address=d.get('server_address'),
+            tags=d.get('tags'),
+        )
+
+
 class VaultAppRoleCertSSHStore:
     __slots__ = [
         'id',
         'issuedcertttlminutes',
         'name',
         'namespace',
         'server_address',
```

## Comparing `strongdm-8.3.0/strongdm/remote_identity_groups_history_pb2.py` & `strongdm-8.4.0/strongdm/remote_identity_groups_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/peering_group_peers_pb2.py` & `strongdm-8.4.0/strongdm/peering_group_peers_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/secret_store_types_pb2.py` & `strongdm-8.4.0/strongdm/secret_store_types_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from . import options_pb2 as options__pb2
 from . import tags_pb2 as tags__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18secret_store_types.proto\x12\x02v1\x1a\roptions.proto\x1a\ntags.proto\"\xfa\x11\n\x0bSecretStore\x12I\n\x03\x61ws\x18\x03 \x01(\x0b\x32\x0c.v1.AWSStoreB,\xf2\xf8\xb3\x07\x1d\xca\xf3\xb3\x07\x18\xc2\xf4\xb3\x07\x13\n\x0cjson_gateway\x12\x03\x61ws\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x64\n\x0e\x61ws_cert_x_509\x18\x1e \x01(\x0b\x32\x14.v1.AWSCertX509StoreB4\xf2\xf8\xb3\x07%\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0b\x61wsCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12o\n\x10\x61\x63tive_directory\x18\x9a\x05 \x01(\x0b\x32\x18.v1.ActiveDirectoryStoreB8\xf2\xf8\xb3\x07)\xca\xf3\xb3\x07$\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0f\x61\x63tiveDirectory\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12O\n\x05\x61zure\x18\x65 \x01(\x0b\x32\x0e.v1.AzureStoreB.\xf2\xf8\xb3\x07\x1f\xca\xf3\xb3\x07\x1a\xc2\xf4\xb3\x07\x15\n\x0cjson_gateway\x12\x05\x61zure\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12l\n\x0f\x63yberark_conjur\x18\xad\x02 \x01(\x0b\x32\x17.v1.CyberarkConjurStoreB7\xf2\xf8\xb3\x07(\xca\xf3\xb3\x07#\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63yberarkConjur\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x63\n\x0c\x63yberark_pam\x18\xaf\x02 \x01(\x0b\x32\x14.v1.CyberarkPAMStoreB4\xf2\xf8\xb3\x07%\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0b\x63yberarkPAM\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x88\x01\n\x19\x63yberark_pam_experimental\x18\xae\x02 \x01(\x0b\x32 .v1.CyberarkPAMExperimentalStoreB@\xf2\xf8\xb3\x07\x31\xca\xf3\xb3\x07,\xc2\xf4\xb3\x07\'\n\x0cjson_gateway\x12\x17\x63yberarkPAMExperimental\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12V\n\x07\x64\x65linea\x18\xd4\x16 \x01(\x0b\x32\x10.v1.DelineaStoreB0\xf2\xf8\xb3\x07!\xca\xf3\xb3\x07\x1c\xc2\xf4\xb3\x07\x17\n\x0cjson_gateway\x12\x07\x64\x65linea\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12J\n\x03gcp\x18\xc9\x01 \x01(\x0b\x32\x0c.v1.GCPStoreB,\xf2\xf8\xb3\x07\x1d\xca\xf3\xb3\x07\x18\xc2\xf4\xb3\x07\x13\n\x0cjson_gateway\x12\x03gcp\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x65\n\x0egcp_cert_x_509\x18\xca\x01 \x01(\x0b\x32\x14.v1.GCPCertX509StoreB4\xf2\xf8\xb3\x07%\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bgcpCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x66\n\rkeyfactor_ssh\x18\xd2\x01 \x01(\x0b\x32\x15.v1.KeyfactorSSHStoreB5\xf2\xf8\xb3\x07&\xca\xf3\xb3\x07!\xc2\xf4\xb3\x07\x1c\n\x0cjson_gateway\x12\x0ckeyfactorSSH\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12j\n\x0fkeyfactor_x_509\x18\xc8\x01 \x01(\x0b\x32\x16.v1.KeyfactorX509StoreB6\xf2\xf8\xb3\x07\'\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rkeyfactorX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x66\n\x0evault_app_role\x18\x04 \x01(\x0b\x32\x15.v1.VaultAppRoleStoreB5\xf2\xf8\xb3\x07&\xca\xf3\xb3\x07!\xc2\xf4\xb3\x07\x1c\n\x0cjson_gateway\x12\x0cvaultAppRole\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12}\n\x17vault_app_role_cert_ssh\x18^ \x01(\x0b\x32\x1c.v1.VaultAppRoleCertSSHStoreB<\xf2\xf8\xb3\x07-\xca\xf3\xb3\x07(\xc2\xf4\xb3\x07#\n\x0cjson_gateway\x12\x13vaultAppRoleCertSSH\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x81\x01\n\x19vault_app_role_cert_x_509\x18_ \x01(\x0b\x32\x1d.v1.VaultAppRoleCertX509StoreB=\xf2\xf8\xb3\x07.\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14vaultAppRoleCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12Y\n\tvault_tls\x18\x01 \x01(\x0b\x32\x11.v1.VaultTLSStoreB1\xf2\xf8\xb3\x07\"\xca\xf3\xb3\x07\x1d\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08vaultTLS\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12p\n\x12vault_tls_cert_ssh\x18\\ \x01(\x0b\x32\x18.v1.VaultTLSCertSSHStoreB8\xf2\xf8\xb3\x07)\xca\xf3\xb3\x07$\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0fvaultTLSCertSSH\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12t\n\x14vault_tls_cert_x_509\x18] \x01(\x0b\x32\x19.v1.VaultTLSCertX509StoreB9\xf2\xf8\xb3\x07*\xca\xf3\xb3\x07%\xc2\xf4\xb3\x07 \n\x0cjson_gateway\x12\x10vaultTLSCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12_\n\x0bvault_token\x18\x02 \x01(\x0b\x32\x13.v1.VaultTokenStoreB3\xf2\xf8\xb3\x07$\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\nvaultToken\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12v\n\x14vault_token_cert_ssh\x18Z \x01(\x0b\x32\x1a.v1.VaultTokenCertSSHStoreB:\xf2\xf8\xb3\x07+\xca\xf3\xb3\x07&\xc2\xf4\xb3\x07!\n\x0cjson_gateway\x12\x11vaultTokenCertSSH\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12z\n\x16vault_token_cert_x_509\x18[ \x01(\x0b\x32\x1b.v1.VaultTokenCertX509StoreB;\xf2\xf8\xb3\x07,\xca\xf3\xb3\x07\'\xc2\xf4\xb3\x07\"\n\x0cjson_gateway\x12\x12vaultTokenCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\x42,\n\x0csecret_store\x12\x1c\xaa\xf8\xb3\x07\t\xaa\xf8\xb3\x07\x04tags\xaa\xf8\xb3\x07\t\xaa\xf8\xb3\x07\x04name\"\xfc\x01\n\x08\x41WSStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12?\n\x06region\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06region\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:T\xfa\xf8\xb3\x07O\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x45\xc2\xf4\xb3\x07\n\n\x03\x63li\x12\x03\x61ws\xc2\xf4\xb3\x07\x13\n\x0cjson_gateway\x12\x03\x61ws\xc2\xf4\xb3\x07\x19\n\x12terraform-provider\x12\x03\x61ws\"\xe6\x04\n\x10\x41WSCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12=\n\x05\x63\x61\x41rn\x18\x05 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1a\xc2\xf4\xb3\x07\x15\n\x0cjson_gateway\x12\x05\x63\x61\x41rn\x12_\n\x16\x63\x65rtificateTemplateArn\x18\x07 \x01(\tB?\xf2\xf8\xb3\x07:\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07+\xc2\xf4\xb3\x07&\n\x0cjson_gateway\x12\x16\x63\x65rtificateTemplateArn\x12[\n\x14issuedCertTTLMinutes\x18\x08 \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12?\n\x06region\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06region\x12I\n\x0bsigningAlgo\x18\x06 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningAlgo\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:n\xfa\xf8\xb3\x07i\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07_\xc2\xf4\xb3\x07\x12\n\x03\x63li\x12\x0b\x61wsCertX509\xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0b\x61wsCertX509\xc2\xf4\xb3\x07#\n\x12terraform-provider\x12\raws_cert_x509\"\x93\x02\n\x14\x41\x63tiveDirectoryStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:N\xfa\xf8\xb3\x07I\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07?\xc2\xf4\xb3\x07\x16\n\x03\x63li\x12\x0f\x61\x63tiveDirectory\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0f\x61\x63tiveDirectory\"\xeb\x01\n\nAzureStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\tvault_uri\x18\x03 \x01(\tB1\xf2\xf8\xb3\x07,\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1d\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08vaultUri\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01::\xfa\xf8\xb3\x07\x35\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07+\xc2\xf4\xb3\x07\x0c\n\x03\x63li\x12\x05\x61zure\xc2\xf4\xb3\x07\x15\n\x0cjson_gateway\x12\x05\x61zure\"\xab\x02\n\x13\x43yberarkConjurStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12?\n\x06\x61ppURL\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06\x61ppUrl\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:v\xfa\xf8\xb3\x07q\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07g\xc2\xf4\xb3\x07\x15\n\x03\x63li\x12\x0e\x63yberarkConjur\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63yberarkConjur\xc2\xf4\xb3\x07%\n\x12terraform-provider\x12\x0f\x63yberark_conjur\"\x9f\x02\n\x10\x43yberarkPAMStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12?\n\x06\x61ppURL\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06\x61ppUrl\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:m\xfa\xf8\xb3\x07h\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07^\xc2\xf4\xb3\x07\x12\n\x03\x63li\x12\x0b\x63yberarkPAM\xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0b\x63yberarkPAM\xc2\xf4\xb3\x07\"\n\x12terraform-provider\x12\x0c\x63yberark_pam\"\xd8\x02\n\x1c\x43yberarkPAMExperimentalStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12?\n\x06\x61ppURL\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06\x61ppUrl\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x99\x01\xfa\xf8\xb3\x07\x93\x01\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x88\x01\x88\xf4\xb3\x07\x01\xc2\xf4\xb3\x07\x1e\n\x03\x63li\x12\x17\x63yberarkPAMExperimental\xc2\xf4\xb3\x07\'\n\x0cjson_gateway\x12\x17\x63yberarkPAMExperimental\xc2\xf4\xb3\x07/\n\x12terraform-provider\x12\x19\x63yberark_pam_experimental\"\xb3\x02\n\x0c\x44\x65lineaStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x41\n\nserver_url\x18\x03 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tserverUrl\x12\x43\n\x0btenant_name\x18\x04 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ntenantName\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:>\xfa\xf8\xb3\x07\x39\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07/\xc2\xf4\xb3\x07\x0e\n\x03\x63li\x12\x07\x64\x65linea\xc2\xf4\xb3\x07\x17\n\x0cjson_gateway\x12\x07\x64\x65linea\"\xe6\x01\n\x08GCPStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x45\n\tprojectID\x18\x03 \x01(\tB2\xf2\xf8\xb3\x07-\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tprojectId\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:6\xfa\xf8\xb3\x07\x31\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\'\xc2\xf4\xb3\x07\n\n\x03\x63li\x12\x03gcp\xc2\xf4\xb3\x07\x13\n\x0cjson_gateway\x12\x03gcp\"\x9d\x04\n\x10GCPCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x36\n\x04\x63\x61ID\x18\x06 \x01(\tB(\xf2\xf8\xb3\x07#\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x19\xc2\xf4\xb3\x07\x14\n\x0cjson_gateway\x12\x04\x63\x61Id\x12\x43\n\x08\x63\x61PoolID\x18\x05 \x01(\tB1\xf2\xf8\xb3\x07,\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1d\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08\x63\x61PoolId\x12[\n\x14issuedCertTTLMinutes\x18\x07 \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12\x43\n\x08location\x18\x04 \x01(\tB1\xf2\xf8\xb3\x07,\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1d\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08location\x12\x45\n\tprojectID\x18\x03 \x01(\tB2\xf2\xf8\xb3\x07-\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tprojectId\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:F\xfa\xf8\xb3\x07\x41\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x37\xc2\xf4\xb3\x07\x12\n\x03\x63li\x12\x0bgcpCertX509\xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bgcpCertX509\"\x8a\x08\n\x11KeyfactorSSHStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\x0c\x63\x61_file_path\x18\x06 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ncaFilePath\x12[\n\x15\x63\x65rtificate_file_path\x18\x04 \x01(\tB<\xf2\xf8\xb3\x07\x37\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07(\xc2\xf4\xb3\x07#\n\x0cjson_gateway\x12\x13\x63\x65rtificateFilePath\x12t\n\"default_certificate_authority_name\x18\n \x01(\tBH\xf2\xf8\xb3\x07\x43\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x34\xc2\xf4\xb3\x07/\n\x0cjson_gateway\x12\x1f\x64\x65\x66\x61ultCertificateAuthorityName\x12p\n default_certificate_profile_name\x18\x08 \x01(\tBF\xf2\xf8\xb3\x07\x41\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x32\xc2\xf4\xb3\x07-\n\x0cjson_gateway\x12\x1d\x64\x65\x66\x61ultCertificateProfileName\x12m\n\x1f\x64\x65\x66\x61ult_end_entity_profile_name\x18\t \x01(\tBD\xf2\xf8\xb3\x07?\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x30\xc2\xf4\xb3\x07+\n\x0cjson_gateway\x12\x1b\x64\x65\x66\x61ultEndEntityProfileName\x12Y\n\x17\x65nrollment_code_env_var\x18\x0c \x01(\tB8\xf2\xf8\xb3\x07\x33\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14\x65nrollmentCodeEnvVar\x12\x61\n\x1b\x65nrollment_username_env_var\x18\x0b \x01(\tB<\xf2\xf8\xb3\x07\x37\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07-\xc2\xf4\xb3\x07(\n\x0cjson_gateway\x12\x18\x65nrollmentUsernameEnvVar\x12\x46\n\rkey_file_path\x18\x05 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bkeyFilePath\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:H\xfa\xf8\xb3\x07\x43\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x39\xc2\xf4\xb3\x07\x13\n\x03\x63li\x12\x0ckeyfactorSSH\xc2\xf4\xb3\x07\x1c\n\x0cjson_gateway\x12\x0ckeyfactorSSH\"\x8d\x08\n\x12KeyfactorX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\x0c\x63\x61_file_path\x18\x06 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ncaFilePath\x12[\n\x15\x63\x65rtificate_file_path\x18\x04 \x01(\tB<\xf2\xf8\xb3\x07\x37\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07(\xc2\xf4\xb3\x07#\n\x0cjson_gateway\x12\x13\x63\x65rtificateFilePath\x12t\n\"default_certificate_authority_name\x18\n \x01(\tBH\xf2\xf8\xb3\x07\x43\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x34\xc2\xf4\xb3\x07/\n\x0cjson_gateway\x12\x1f\x64\x65\x66\x61ultCertificateAuthorityName\x12p\n default_certificate_profile_name\x18\x08 \x01(\tBF\xf2\xf8\xb3\x07\x41\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x32\xc2\xf4\xb3\x07-\n\x0cjson_gateway\x12\x1d\x64\x65\x66\x61ultCertificateProfileName\x12m\n\x1f\x64\x65\x66\x61ult_end_entity_profile_name\x18\t \x01(\tBD\xf2\xf8\xb3\x07?\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x30\xc2\xf4\xb3\x07+\n\x0cjson_gateway\x12\x1b\x64\x65\x66\x61ultEndEntityProfileName\x12Y\n\x17\x65nrollment_code_env_var\x18\x0c \x01(\tB8\xf2\xf8\xb3\x07\x33\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14\x65nrollmentCodeEnvVar\x12\x61\n\x1b\x65nrollment_username_env_var\x18\x0b \x01(\tB<\xf2\xf8\xb3\x07\x37\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07-\xc2\xf4\xb3\x07(\n\x0cjson_gateway\x12\x18\x65nrollmentUsernameEnvVar\x12\x46\n\rkey_file_path\x18\x05 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bkeyFilePath\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:J\xfa\xf8\xb3\x07\x45\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07;\xc2\xf4\xb3\x07\x14\n\x03\x63li\x12\rkeyfactorX509\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rkeyfactorX509\"\xf2\x02\n\x11VaultAppRoleStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12\"\n\x04tags\x18\x08 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:p\xfa\xf8\xb3\x07k\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x61\xc2\xf4\xb3\x07\x13\n\x03\x63li\x12\x0cvaultAppRole\xc2\xf4\xb3\x07\x1c\n\x0cjson_gateway\x12\x0cvaultAppRole\xc2\xf4\xb3\x07#\n\x12terraform-provider\x12\rvault_approle\"\x8c\x05\n\x18VaultAppRoleCertSSHStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12[\n\x14issuedCertTTLMinutes\x18\t \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\x07 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12O\n\x0fssh_mount_point\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rsshMountPoint\x12\"\n\x04tags\x18\x08 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x88\x01\xfa\xf8\xb3\x07\x82\x01\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07x\xc2\xf4\xb3\x07\x1a\n\x03\x63li\x12\x13vaultAppRoleCertSSH\xc2\xf4\xb3\x07#\n\x0cjson_gateway\x12\x13vaultAppRoleCertSSH\xc2\xf4\xb3\x07,\n\x12terraform-provider\x12\x16vault_approle_cert_ssh\"\x90\x05\n\x19VaultAppRoleCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12[\n\x14issuedCertTTLMinutes\x18\t \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12O\n\x0fpki_mount_point\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rpkiMountPoint\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\x07 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12\"\n\x04tags\x18\x08 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x8b\x01\xfa\xf8\xb3\x07\x85\x01\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07{\xc2\xf4\xb3\x07\x1b\n\x03\x63li\x12\x14vaultAppRoleCertX509\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14vaultAppRoleCertX509\xc2\xf4\xb3\x07-\n\x12terraform-provider\x12\x17vault_approle_cert_x509\"\xcc\x04\n\rVaultTLSStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\x0c\x43\x41_cert_path\x18\x04 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ncaCertPath\x12Q\n\x10\x63lient_cert_path\x18\x05 \x01(\tB7\xf2\xf8\xb3\x07\x32\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07#\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63lientCertPath\x12O\n\x0f\x63lient_key_path\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rclientKeyPath\x12@\n\tnamespace\x18\x08 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12\"\n\x04tags\x18\x07 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:d\xfa\xf8\xb3\x07_\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07U\xc2\xf4\xb3\x07\x0f\n\x03\x63li\x12\x08vaultTLS\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08vaultTLS\xc2\xf4\xb3\x07\x1f\n\x12terraform-provider\x12\tvault_tls\"\xe4\x06\n\x14VaultTLSCertSSHStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\x0c\x43\x41_cert_path\x18\x04 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ncaCertPath\x12Q\n\x10\x63lient_cert_path\x18\x05 \x01(\tB7\xf2\xf8\xb3\x07\x32\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07#\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63lientCertPath\x12O\n\x0f\x63lient_key_path\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rclientKeyPath\x12[\n\x14issuedCertTTLMinutes\x18\x0b \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x08 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\n \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12O\n\x0fssh_mount_point\x18\t \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rsshMountPoint\x12\"\n\x04tags\x18\x07 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:{\xfa\xf8\xb3\x07v\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07l\xc2\xf4\xb3\x07\x16\n\x03\x63li\x12\x0fvaultTLSCertSSH\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0fvaultTLSCertSSH\xc2\xf4\xb3\x07(\n\x12terraform-provider\x12\x12vault_tls_cert_ssh\"\xe8\x06\n\x15VaultTLSCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\x0c\x43\x41_cert_path\x18\x04 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ncaCertPath\x12Q\n\x10\x63lient_cert_path\x18\x05 \x01(\tB7\xf2\xf8\xb3\x07\x32\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07#\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63lientCertPath\x12O\n\x0f\x63lient_key_path\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rclientKeyPath\x12[\n\x14issuedCertTTLMinutes\x18\x0b \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x08 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12O\n\x0fpki_mount_point\x18\t \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rpkiMountPoint\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\n \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12\"\n\x04tags\x18\x07 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:~\xfa\xf8\xb3\x07y\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07o\xc2\xf4\xb3\x07\x17\n\x03\x63li\x12\x10vaultTLSCertX509\xc2\xf4\xb3\x07 \n\x0cjson_gateway\x12\x10vaultTLSCertX509\xc2\xf4\xb3\x07)\n\x12terraform-provider\x12\x13vault_tls_cert_x509\"\xea\x02\n\x0fVaultTokenStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:j\xfa\xf8\xb3\x07\x65\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07[\xc2\xf4\xb3\x07\x11\n\x03\x63li\x12\nvaultToken\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\nvaultToken\xc2\xf4\xb3\x07!\n\x12terraform-provider\x12\x0bvault_token\"\x83\x05\n\x16VaultTokenCertSSHStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12[\n\x14issuedCertTTLMinutes\x18\t \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\x07 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12O\n\x0fssh_mount_point\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rsshMountPoint\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x81\x01\xfa\xf8\xb3\x07|\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07r\xc2\xf4\xb3\x07\x18\n\x03\x63li\x12\x11vaultTokenCertSSH\xc2\xf4\xb3\x07!\n\x0cjson_gateway\x12\x11vaultTokenCertSSH\xc2\xf4\xb3\x07*\n\x12terraform-provider\x12\x14vault_token_cert_ssh\"\x87\x05\n\x17VaultTokenCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12[\n\x14issuedCertTTLMinutes\x18\x08 \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12O\n\x0fpki_mount_point\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rpkiMountPoint\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\x07 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x84\x01\xfa\xf8\xb3\x07\x7f\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07u\xc2\xf4\xb3\x07\x19\n\x03\x63li\x12\x12vaultTokenCertX509\xc2\xf4\xb3\x07\"\n\x0cjson_gateway\x12\x12vaultTokenCertX509\xc2\xf4\xb3\x07+\n\x12terraform-provider\x12\x15vault_token_cert_x509Bm\n\x19\x63om.strongdm.api.plumbingB\x19SecretStoresTypesPlumbingZ5github.com/strongdm/strongdm-sdk-go/v3/internal/v1;v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18secret_store_types.proto\x12\x02v1\x1a\roptions.proto\x1a\ntags.proto\"\xc3\x13\n\x0bSecretStore\x12I\n\x03\x61ws\x18\x03 \x01(\x0b\x32\x0c.v1.AWSStoreB,\xf2\xf8\xb3\x07\x1d\xca\xf3\xb3\x07\x18\xc2\xf4\xb3\x07\x13\n\x0cjson_gateway\x12\x03\x61ws\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x64\n\x0e\x61ws_cert_x_509\x18\x1e \x01(\x0b\x32\x14.v1.AWSCertX509StoreB4\xf2\xf8\xb3\x07%\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0b\x61wsCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12o\n\x10\x61\x63tive_directory\x18\x9a\x05 \x01(\x0b\x32\x18.v1.ActiveDirectoryStoreB8\xf2\xf8\xb3\x07)\xca\xf3\xb3\x07$\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0f\x61\x63tiveDirectory\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12O\n\x05\x61zure\x18\x65 \x01(\x0b\x32\x0e.v1.AzureStoreB.\xf2\xf8\xb3\x07\x1f\xca\xf3\xb3\x07\x1a\xc2\xf4\xb3\x07\x15\n\x0cjson_gateway\x12\x05\x61zure\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12l\n\x0f\x63yberark_conjur\x18\xad\x02 \x01(\x0b\x32\x17.v1.CyberarkConjurStoreB7\xf2\xf8\xb3\x07(\xca\xf3\xb3\x07#\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63yberarkConjur\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x63\n\x0c\x63yberark_pam\x18\xaf\x02 \x01(\x0b\x32\x14.v1.CyberarkPAMStoreB4\xf2\xf8\xb3\x07%\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0b\x63yberarkPAM\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x88\x01\n\x19\x63yberark_pam_experimental\x18\xae\x02 \x01(\x0b\x32 .v1.CyberarkPAMExperimentalStoreB@\xf2\xf8\xb3\x07\x31\xca\xf3\xb3\x07,\xc2\xf4\xb3\x07\'\n\x0cjson_gateway\x12\x17\x63yberarkPAMExperimental\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12V\n\x07\x64\x65linea\x18\xd4\x16 \x01(\x0b\x32\x10.v1.DelineaStoreB0\xf2\xf8\xb3\x07!\xca\xf3\xb3\x07\x1c\xc2\xf4\xb3\x07\x17\n\x0cjson_gateway\x12\x07\x64\x65linea\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12J\n\x03gcp\x18\xc9\x01 \x01(\x0b\x32\x0c.v1.GCPStoreB,\xf2\xf8\xb3\x07\x1d\xca\xf3\xb3\x07\x18\xc2\xf4\xb3\x07\x13\n\x0cjson_gateway\x12\x03gcp\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x65\n\x0egcp_cert_x_509\x18\xca\x01 \x01(\x0b\x32\x14.v1.GCPCertX509StoreB4\xf2\xf8\xb3\x07%\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bgcpCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x66\n\rkeyfactor_ssh\x18\xd2\x01 \x01(\x0b\x32\x15.v1.KeyfactorSSHStoreB5\xf2\xf8\xb3\x07&\xca\xf3\xb3\x07!\xc2\xf4\xb3\x07\x1c\n\x0cjson_gateway\x12\x0ckeyfactorSSH\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12j\n\x0fkeyfactor_x_509\x18\xc8\x01 \x01(\x0b\x32\x16.v1.KeyfactorX509StoreB6\xf2\xf8\xb3\x07\'\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rkeyfactorX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x63\n\rvault_awsec_2\x18\x61 \x01(\x0b\x32\x14.v1.VaultAWSEC2StoreB4\xf2\xf8\xb3\x07%\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bvaultAWSEC2\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x62\n\x0cvault_awsiam\x18` \x01(\x0b\x32\x14.v1.VaultAWSIAMStoreB4\xf2\xf8\xb3\x07%\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bvaultAWSIAM\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x66\n\x0evault_app_role\x18\x04 \x01(\x0b\x32\x15.v1.VaultAppRoleStoreB5\xf2\xf8\xb3\x07&\xca\xf3\xb3\x07!\xc2\xf4\xb3\x07\x1c\n\x0cjson_gateway\x12\x0cvaultAppRole\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12}\n\x17vault_app_role_cert_ssh\x18^ \x01(\x0b\x32\x1c.v1.VaultAppRoleCertSSHStoreB<\xf2\xf8\xb3\x07-\xca\xf3\xb3\x07(\xc2\xf4\xb3\x07#\n\x0cjson_gateway\x12\x13vaultAppRoleCertSSH\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12\x81\x01\n\x19vault_app_role_cert_x_509\x18_ \x01(\x0b\x32\x1d.v1.VaultAppRoleCertX509StoreB=\xf2\xf8\xb3\x07.\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14vaultAppRoleCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12Y\n\tvault_tls\x18\x01 \x01(\x0b\x32\x11.v1.VaultTLSStoreB1\xf2\xf8\xb3\x07\"\xca\xf3\xb3\x07\x1d\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08vaultTLS\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12p\n\x12vault_tls_cert_ssh\x18\\ \x01(\x0b\x32\x18.v1.VaultTLSCertSSHStoreB8\xf2\xf8\xb3\x07)\xca\xf3\xb3\x07$\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0fvaultTLSCertSSH\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12t\n\x14vault_tls_cert_x_509\x18] \x01(\x0b\x32\x19.v1.VaultTLSCertX509StoreB9\xf2\xf8\xb3\x07*\xca\xf3\xb3\x07%\xc2\xf4\xb3\x07 \n\x0cjson_gateway\x12\x10vaultTLSCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12_\n\x0bvault_token\x18\x02 \x01(\x0b\x32\x13.v1.VaultTokenStoreB3\xf2\xf8\xb3\x07$\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\nvaultToken\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12v\n\x14vault_token_cert_ssh\x18Z \x01(\x0b\x32\x1a.v1.VaultTokenCertSSHStoreB:\xf2\xf8\xb3\x07+\xca\xf3\xb3\x07&\xc2\xf4\xb3\x07!\n\x0cjson_gateway\x12\x11vaultTokenCertSSH\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00\x12z\n\x16vault_token_cert_x_509\x18[ \x01(\x0b\x32\x1b.v1.VaultTokenCertX509StoreB;\xf2\xf8\xb3\x07,\xca\xf3\xb3\x07\'\xc2\xf4\xb3\x07\"\n\x0cjson_gateway\x12\x12vaultTokenCertX509\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01H\x00:\n\xfa\xf8\xb3\x07\x05\xa8\xf3\xb3\x07\x01\x42,\n\x0csecret_store\x12\x1c\xaa\xf8\xb3\x07\t\xaa\xf8\xb3\x07\x04tags\xaa\xf8\xb3\x07\t\xaa\xf8\xb3\x07\x04name\"\xfc\x01\n\x08\x41WSStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12?\n\x06region\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06region\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:T\xfa\xf8\xb3\x07O\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x45\xc2\xf4\xb3\x07\n\n\x03\x63li\x12\x03\x61ws\xc2\xf4\xb3\x07\x13\n\x0cjson_gateway\x12\x03\x61ws\xc2\xf4\xb3\x07\x19\n\x12terraform-provider\x12\x03\x61ws\"\xe6\x04\n\x10\x41WSCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12=\n\x05\x63\x61\x41rn\x18\x05 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1a\xc2\xf4\xb3\x07\x15\n\x0cjson_gateway\x12\x05\x63\x61\x41rn\x12_\n\x16\x63\x65rtificateTemplateArn\x18\x07 \x01(\tB?\xf2\xf8\xb3\x07:\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07+\xc2\xf4\xb3\x07&\n\x0cjson_gateway\x12\x16\x63\x65rtificateTemplateArn\x12[\n\x14issuedCertTTLMinutes\x18\x08 \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12?\n\x06region\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06region\x12I\n\x0bsigningAlgo\x18\x06 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningAlgo\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:n\xfa\xf8\xb3\x07i\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07_\xc2\xf4\xb3\x07\x12\n\x03\x63li\x12\x0b\x61wsCertX509\xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0b\x61wsCertX509\xc2\xf4\xb3\x07#\n\x12terraform-provider\x12\raws_cert_x509\"\x93\x02\n\x14\x41\x63tiveDirectoryStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:N\xfa\xf8\xb3\x07I\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07?\xc2\xf4\xb3\x07\x16\n\x03\x63li\x12\x0f\x61\x63tiveDirectory\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0f\x61\x63tiveDirectory\"\xeb\x01\n\nAzureStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\tvault_uri\x18\x03 \x01(\tB1\xf2\xf8\xb3\x07,\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1d\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08vaultUri\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01::\xfa\xf8\xb3\x07\x35\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07+\xc2\xf4\xb3\x07\x0c\n\x03\x63li\x12\x05\x61zure\xc2\xf4\xb3\x07\x15\n\x0cjson_gateway\x12\x05\x61zure\"\xab\x02\n\x13\x43yberarkConjurStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12?\n\x06\x61ppURL\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06\x61ppUrl\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:v\xfa\xf8\xb3\x07q\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07g\xc2\xf4\xb3\x07\x15\n\x03\x63li\x12\x0e\x63yberarkConjur\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63yberarkConjur\xc2\xf4\xb3\x07%\n\x12terraform-provider\x12\x0f\x63yberark_conjur\"\x9f\x02\n\x10\x43yberarkPAMStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12?\n\x06\x61ppURL\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06\x61ppUrl\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:m\xfa\xf8\xb3\x07h\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07^\xc2\xf4\xb3\x07\x12\n\x03\x63li\x12\x0b\x63yberarkPAM\xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0b\x63yberarkPAM\xc2\xf4\xb3\x07\"\n\x12terraform-provider\x12\x0c\x63yberark_pam\"\xd8\x02\n\x1c\x43yberarkPAMExperimentalStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12?\n\x06\x61ppURL\x18\x03 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1b\xc2\xf4\xb3\x07\x16\n\x0cjson_gateway\x12\x06\x61ppUrl\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x99\x01\xfa\xf8\xb3\x07\x93\x01\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x88\x01\x88\xf4\xb3\x07\x01\xc2\xf4\xb3\x07\x1e\n\x03\x63li\x12\x17\x63yberarkPAMExperimental\xc2\xf4\xb3\x07\'\n\x0cjson_gateway\x12\x17\x63yberarkPAMExperimental\xc2\xf4\xb3\x07/\n\x12terraform-provider\x12\x19\x63yberark_pam_experimental\"\xb3\x02\n\x0c\x44\x65lineaStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x41\n\nserver_url\x18\x03 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tserverUrl\x12\x43\n\x0btenant_name\x18\x04 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ntenantName\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:>\xfa\xf8\xb3\x07\x39\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07/\xc2\xf4\xb3\x07\x0e\n\x03\x63li\x12\x07\x64\x65linea\xc2\xf4\xb3\x07\x17\n\x0cjson_gateway\x12\x07\x64\x65linea\"\xe6\x01\n\x08GCPStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x45\n\tprojectID\x18\x03 \x01(\tB2\xf2\xf8\xb3\x07-\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tprojectId\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:6\xfa\xf8\xb3\x07\x31\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\'\xc2\xf4\xb3\x07\n\n\x03\x63li\x12\x03gcp\xc2\xf4\xb3\x07\x13\n\x0cjson_gateway\x12\x03gcp\"\x9d\x04\n\x10GCPCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x36\n\x04\x63\x61ID\x18\x06 \x01(\tB(\xf2\xf8\xb3\x07#\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x19\xc2\xf4\xb3\x07\x14\n\x0cjson_gateway\x12\x04\x63\x61Id\x12\x43\n\x08\x63\x61PoolID\x18\x05 \x01(\tB1\xf2\xf8\xb3\x07,\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1d\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08\x63\x61PoolId\x12[\n\x14issuedCertTTLMinutes\x18\x07 \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12\x43\n\x08location\x18\x04 \x01(\tB1\xf2\xf8\xb3\x07,\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1d\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08location\x12\x45\n\tprojectID\x18\x03 \x01(\tB2\xf2\xf8\xb3\x07-\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tprojectId\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:F\xfa\xf8\xb3\x07\x41\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x37\xc2\xf4\xb3\x07\x12\n\x03\x63li\x12\x0bgcpCertX509\xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bgcpCertX509\"\x8a\x08\n\x11KeyfactorSSHStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\x0c\x63\x61_file_path\x18\x06 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ncaFilePath\x12[\n\x15\x63\x65rtificate_file_path\x18\x04 \x01(\tB<\xf2\xf8\xb3\x07\x37\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07(\xc2\xf4\xb3\x07#\n\x0cjson_gateway\x12\x13\x63\x65rtificateFilePath\x12t\n\"default_certificate_authority_name\x18\n \x01(\tBH\xf2\xf8\xb3\x07\x43\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x34\xc2\xf4\xb3\x07/\n\x0cjson_gateway\x12\x1f\x64\x65\x66\x61ultCertificateAuthorityName\x12p\n default_certificate_profile_name\x18\x08 \x01(\tBF\xf2\xf8\xb3\x07\x41\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x32\xc2\xf4\xb3\x07-\n\x0cjson_gateway\x12\x1d\x64\x65\x66\x61ultCertificateProfileName\x12m\n\x1f\x64\x65\x66\x61ult_end_entity_profile_name\x18\t \x01(\tBD\xf2\xf8\xb3\x07?\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x30\xc2\xf4\xb3\x07+\n\x0cjson_gateway\x12\x1b\x64\x65\x66\x61ultEndEntityProfileName\x12Y\n\x17\x65nrollment_code_env_var\x18\x0c \x01(\tB8\xf2\xf8\xb3\x07\x33\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14\x65nrollmentCodeEnvVar\x12\x61\n\x1b\x65nrollment_username_env_var\x18\x0b \x01(\tB<\xf2\xf8\xb3\x07\x37\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07-\xc2\xf4\xb3\x07(\n\x0cjson_gateway\x12\x18\x65nrollmentUsernameEnvVar\x12\x46\n\rkey_file_path\x18\x05 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bkeyFilePath\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:H\xfa\xf8\xb3\x07\x43\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x39\xc2\xf4\xb3\x07\x13\n\x03\x63li\x12\x0ckeyfactorSSH\xc2\xf4\xb3\x07\x1c\n\x0cjson_gateway\x12\x0ckeyfactorSSH\"\x8d\x08\n\x12KeyfactorX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\x0c\x63\x61_file_path\x18\x06 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ncaFilePath\x12[\n\x15\x63\x65rtificate_file_path\x18\x04 \x01(\tB<\xf2\xf8\xb3\x07\x37\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07(\xc2\xf4\xb3\x07#\n\x0cjson_gateway\x12\x13\x63\x65rtificateFilePath\x12t\n\"default_certificate_authority_name\x18\n \x01(\tBH\xf2\xf8\xb3\x07\x43\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x34\xc2\xf4\xb3\x07/\n\x0cjson_gateway\x12\x1f\x64\x65\x66\x61ultCertificateAuthorityName\x12p\n default_certificate_profile_name\x18\x08 \x01(\tBF\xf2\xf8\xb3\x07\x41\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x32\xc2\xf4\xb3\x07-\n\x0cjson_gateway\x12\x1d\x64\x65\x66\x61ultCertificateProfileName\x12m\n\x1f\x64\x65\x66\x61ult_end_entity_profile_name\x18\t \x01(\tBD\xf2\xf8\xb3\x07?\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x30\xc2\xf4\xb3\x07+\n\x0cjson_gateway\x12\x1b\x64\x65\x66\x61ultEndEntityProfileName\x12Y\n\x17\x65nrollment_code_env_var\x18\x0c \x01(\tB8\xf2\xf8\xb3\x07\x33\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14\x65nrollmentCodeEnvVar\x12\x61\n\x1b\x65nrollment_username_env_var\x18\x0b \x01(\tB<\xf2\xf8\xb3\x07\x37\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07-\xc2\xf4\xb3\x07(\n\x0cjson_gateway\x12\x18\x65nrollmentUsernameEnvVar\x12\x46\n\rkey_file_path\x18\x05 \x01(\tB/\xf2\xf8\xb3\x07*\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bkeyFilePath\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12$\n\x04tags\x18\x83\x80\x02 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:J\xfa\xf8\xb3\x07\x45\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07;\xc2\xf4\xb3\x07\x14\n\x03\x63li\x12\rkeyfactorX509\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rkeyfactorX509\"\xf4\x02\n\x10VaultAWSEC2Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12\"\n\x04tags\x18\x08 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:s\xfa\xf8\xb3\x07n\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x64\x88\xf4\xb3\x07\x01\xc2\xf4\xb3\x07\x12\n\x03\x63li\x12\x0bvaultAWSEC2\xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bvaultAWSEC2\xc2\xf4\xb3\x07#\n\x12terraform-provider\x12\rvault_aws_ec2\"\xf4\x02\n\x10VaultAWSIAMStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12\"\n\x04tags\x18\x08 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:s\xfa\xf8\xb3\x07n\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x64\x88\xf4\xb3\x07\x01\xc2\xf4\xb3\x07\x12\n\x03\x63li\x12\x0bvaultAWSIAM\xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bvaultAWSIAM\xc2\xf4\xb3\x07#\n\x12terraform-provider\x12\rvault_aws_iam\"\xf2\x02\n\x11VaultAppRoleStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12\"\n\x04tags\x18\x08 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:p\xfa\xf8\xb3\x07k\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x61\xc2\xf4\xb3\x07\x13\n\x03\x63li\x12\x0cvaultAppRole\xc2\xf4\xb3\x07\x1c\n\x0cjson_gateway\x12\x0cvaultAppRole\xc2\xf4\xb3\x07#\n\x12terraform-provider\x12\rvault_approle\"\x8c\x05\n\x18VaultAppRoleCertSSHStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12[\n\x14issuedCertTTLMinutes\x18\t \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\x07 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12O\n\x0fssh_mount_point\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rsshMountPoint\x12\"\n\x04tags\x18\x08 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x88\x01\xfa\xf8\xb3\x07\x82\x01\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07x\xc2\xf4\xb3\x07\x1a\n\x03\x63li\x12\x13vaultAppRoleCertSSH\xc2\xf4\xb3\x07#\n\x0cjson_gateway\x12\x13vaultAppRoleCertSSH\xc2\xf4\xb3\x07,\n\x12terraform-provider\x12\x16vault_approle_cert_ssh\"\x90\x05\n\x19VaultAppRoleCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12[\n\x14issuedCertTTLMinutes\x18\t \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12O\n\x0fpki_mount_point\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rpkiMountPoint\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\x07 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12\"\n\x04tags\x18\x08 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x8b\x01\xfa\xf8\xb3\x07\x85\x01\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07{\xc2\xf4\xb3\x07\x1b\n\x03\x63li\x12\x14vaultAppRoleCertX509\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14vaultAppRoleCertX509\xc2\xf4\xb3\x07-\n\x12terraform-provider\x12\x17vault_approle_cert_x509\"\xcc\x04\n\rVaultTLSStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\x0c\x43\x41_cert_path\x18\x04 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ncaCertPath\x12Q\n\x10\x63lient_cert_path\x18\x05 \x01(\tB7\xf2\xf8\xb3\x07\x32\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07#\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63lientCertPath\x12O\n\x0f\x63lient_key_path\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rclientKeyPath\x12@\n\tnamespace\x18\x08 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12\"\n\x04tags\x18\x07 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:d\xfa\xf8\xb3\x07_\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07U\xc2\xf4\xb3\x07\x0f\n\x03\x63li\x12\x08vaultTLS\xc2\xf4\xb3\x07\x18\n\x0cjson_gateway\x12\x08vaultTLS\xc2\xf4\xb3\x07\x1f\n\x12terraform-provider\x12\tvault_tls\"\xe4\x06\n\x14VaultTLSCertSSHStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\x0c\x43\x41_cert_path\x18\x04 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ncaCertPath\x12Q\n\x10\x63lient_cert_path\x18\x05 \x01(\tB7\xf2\xf8\xb3\x07\x32\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07#\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63lientCertPath\x12O\n\x0f\x63lient_key_path\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rclientKeyPath\x12[\n\x14issuedCertTTLMinutes\x18\x0b \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x08 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\n \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12O\n\x0fssh_mount_point\x18\t \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rsshMountPoint\x12\"\n\x04tags\x18\x07 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:{\xfa\xf8\xb3\x07v\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07l\xc2\xf4\xb3\x07\x16\n\x03\x63li\x12\x0fvaultTLSCertSSH\xc2\xf4\xb3\x07\x1f\n\x0cjson_gateway\x12\x0fvaultTLSCertSSH\xc2\xf4\xb3\x07(\n\x12terraform-provider\x12\x12vault_tls_cert_ssh\"\xe8\x06\n\x15VaultTLSCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12\x44\n\x0c\x43\x41_cert_path\x18\x04 \x01(\tB.\xf2\xf8\xb3\x07)\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1f\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\ncaCertPath\x12Q\n\x10\x63lient_cert_path\x18\x05 \x01(\tB7\xf2\xf8\xb3\x07\x32\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07#\xc2\xf4\xb3\x07\x1e\n\x0cjson_gateway\x12\x0e\x63lientCertPath\x12O\n\x0f\x63lient_key_path\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rclientKeyPath\x12[\n\x14issuedCertTTLMinutes\x18\x0b \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x08 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12O\n\x0fpki_mount_point\x18\t \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rpkiMountPoint\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\n \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12\"\n\x04tags\x18\x07 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:~\xfa\xf8\xb3\x07y\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07o\xc2\xf4\xb3\x07\x17\n\x03\x63li\x12\x10vaultTLSCertX509\xc2\xf4\xb3\x07 \n\x0cjson_gateway\x12\x10vaultTLSCertX509\xc2\xf4\xb3\x07)\n\x12terraform-provider\x12\x13vault_tls_cert_x509\"\xea\x02\n\x0fVaultTokenStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:j\xfa\xf8\xb3\x07\x65\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07[\xc2\xf4\xb3\x07\x11\n\x03\x63li\x12\nvaultToken\xc2\xf4\xb3\x07\x1a\n\x0cjson_gateway\x12\nvaultToken\xc2\xf4\xb3\x07!\n\x12terraform-provider\x12\x0bvault_token\"\x83\x05\n\x16VaultTokenCertSSHStore\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12[\n\x14issuedCertTTLMinutes\x18\t \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\x07 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12O\n\x0fssh_mount_point\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rsshMountPoint\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x81\x01\xfa\xf8\xb3\x07|\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07r\xc2\xf4\xb3\x07\x18\n\x03\x63li\x12\x11vaultTokenCertSSH\xc2\xf4\xb3\x07!\n\x0cjson_gateway\x12\x11vaultTokenCertSSH\xc2\xf4\xb3\x07*\n\x12terraform-provider\x12\x14vault_token_cert_ssh\"\x87\x05\n\x17VaultTokenCertX509Store\x12\x16\n\x02id\x18\x01 \x01(\tB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01\x12\x1d\n\x04name\x18\x02 \x01(\tB\x0f\xf2\xf8\xb3\x07\n\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\x12[\n\x14issuedCertTTLMinutes\x18\x08 \x01(\x05\x42=\xf2\xf8\xb3\x07\x38\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07)\xc2\xf4\xb3\x07$\n\x0cjson_gateway\x12\x14issuedCertTtlMinutes\x12@\n\tnamespace\x18\x05 \x01(\tB-\xf2\xf8\xb3\x07(\xb0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\x1e\xc2\xf4\xb3\x07\x19\n\x0cjson_gateway\x12\tnamespace\x12O\n\x0fpki_mount_point\x18\x06 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rpkiMountPoint\x12N\n\x0eserver_address\x18\x03 \x01(\tB6\xf2\xf8\xb3\x07\x31\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07\"\xc2\xf4\xb3\x07\x1d\n\x0cjson_gateway\x12\rserverAddress\x12J\n\x0csigning_role\x18\x07 \x01(\tB4\xf2\xf8\xb3\x07/\xb0\xf3\xb3\x07\x01\xc0\xf3\xb3\x07\x01\xca\xf3\xb3\x07 \xc2\xf4\xb3\x07\x1b\n\x0cjson_gateway\x12\x0bsigningRole\x12\"\n\x04tags\x18\x04 \x01(\x0b\x32\x08.v1.TagsB\n\xf2\xf8\xb3\x07\x05\xb0\xf3\xb3\x07\x01:\x84\x01\xfa\xf8\xb3\x07\x7f\xa8\xf3\xb3\x07\x01\xca\xf3\xb3\x07u\xc2\xf4\xb3\x07\x19\n\x03\x63li\x12\x12vaultTokenCertX509\xc2\xf4\xb3\x07\"\n\x0cjson_gateway\x12\x12vaultTokenCertX509\xc2\xf4\xb3\x07+\n\x12terraform-provider\x12\x15vault_token_cert_x509Bm\n\x19\x63om.strongdm.api.plumbingB\x19SecretStoresTypesPlumbingZ5github.com/strongdm/strongdm-sdk-go/v3/internal/v1;v1b\x06proto3')
 
 
 
 _SECRETSTORE = DESCRIPTOR.message_types_by_name['SecretStore']
 _AWSSTORE = DESCRIPTOR.message_types_by_name['AWSStore']
 _AWSCERTX509STORE = DESCRIPTOR.message_types_by_name['AWSCertX509Store']
 _ACTIVEDIRECTORYSTORE = DESCRIPTOR.message_types_by_name['ActiveDirectoryStore']
@@ -43,14 +43,16 @@
 _CYBERARKPAMSTORE = DESCRIPTOR.message_types_by_name['CyberarkPAMStore']
 _CYBERARKPAMEXPERIMENTALSTORE = DESCRIPTOR.message_types_by_name['CyberarkPAMExperimentalStore']
 _DELINEASTORE = DESCRIPTOR.message_types_by_name['DelineaStore']
 _GCPSTORE = DESCRIPTOR.message_types_by_name['GCPStore']
 _GCPCERTX509STORE = DESCRIPTOR.message_types_by_name['GCPCertX509Store']
 _KEYFACTORSSHSTORE = DESCRIPTOR.message_types_by_name['KeyfactorSSHStore']
 _KEYFACTORX509STORE = DESCRIPTOR.message_types_by_name['KeyfactorX509Store']
+_VAULTAWSEC2STORE = DESCRIPTOR.message_types_by_name['VaultAWSEC2Store']
+_VAULTAWSIAMSTORE = DESCRIPTOR.message_types_by_name['VaultAWSIAMStore']
 _VAULTAPPROLESTORE = DESCRIPTOR.message_types_by_name['VaultAppRoleStore']
 _VAULTAPPROLECERTSSHSTORE = DESCRIPTOR.message_types_by_name['VaultAppRoleCertSSHStore']
 _VAULTAPPROLECERTX509STORE = DESCRIPTOR.message_types_by_name['VaultAppRoleCertX509Store']
 _VAULTTLSSTORE = DESCRIPTOR.message_types_by_name['VaultTLSStore']
 _VAULTTLSCERTSSHSTORE = DESCRIPTOR.message_types_by_name['VaultTLSCertSSHStore']
 _VAULTTLSCERTX509STORE = DESCRIPTOR.message_types_by_name['VaultTLSCertX509Store']
 _VAULTTOKENSTORE = DESCRIPTOR.message_types_by_name['VaultTokenStore']
@@ -143,14 +145,28 @@
 KeyfactorX509Store = _reflection.GeneratedProtocolMessageType('KeyfactorX509Store', (_message.Message,), {
   'DESCRIPTOR' : _KEYFACTORX509STORE,
   '__module__' : 'secret_store_types_pb2'
   # @@protoc_insertion_point(class_scope:v1.KeyfactorX509Store)
   })
 _sym_db.RegisterMessage(KeyfactorX509Store)
 
+VaultAWSEC2Store = _reflection.GeneratedProtocolMessageType('VaultAWSEC2Store', (_message.Message,), {
+  'DESCRIPTOR' : _VAULTAWSEC2STORE,
+  '__module__' : 'secret_store_types_pb2'
+  # @@protoc_insertion_point(class_scope:v1.VaultAWSEC2Store)
+  })
+_sym_db.RegisterMessage(VaultAWSEC2Store)
+
+VaultAWSIAMStore = _reflection.GeneratedProtocolMessageType('VaultAWSIAMStore', (_message.Message,), {
+  'DESCRIPTOR' : _VAULTAWSIAMSTORE,
+  '__module__' : 'secret_store_types_pb2'
+  # @@protoc_insertion_point(class_scope:v1.VaultAWSIAMStore)
+  })
+_sym_db.RegisterMessage(VaultAWSIAMStore)
+
 VaultAppRoleStore = _reflection.GeneratedProtocolMessageType('VaultAppRoleStore', (_message.Message,), {
   'DESCRIPTOR' : _VAULTAPPROLESTORE,
   '__module__' : 'secret_store_types_pb2'
   # @@protoc_insertion_point(class_scope:v1.VaultAppRoleStore)
   })
 _sym_db.RegisterMessage(VaultAppRoleStore)
 
@@ -236,14 +252,18 @@
   _SECRETSTORE.fields_by_name['gcp']._serialized_options = b'\362\370\263\007\035\312\363\263\007\030\302\364\263\007\023\n\014json_gateway\022\003gcp\362\370\263\007\005\260\363\263\007\001'
   _SECRETSTORE.fields_by_name['gcp_cert_x_509']._options = None
   _SECRETSTORE.fields_by_name['gcp_cert_x_509']._serialized_options = b'\362\370\263\007%\312\363\263\007 \302\364\263\007\033\n\014json_gateway\022\013gcpCertX509\362\370\263\007\005\260\363\263\007\001'
   _SECRETSTORE.fields_by_name['keyfactor_ssh']._options = None
   _SECRETSTORE.fields_by_name['keyfactor_ssh']._serialized_options = b'\362\370\263\007&\312\363\263\007!\302\364\263\007\034\n\014json_gateway\022\014keyfactorSSH\362\370\263\007\005\260\363\263\007\001'
   _SECRETSTORE.fields_by_name['keyfactor_x_509']._options = None
   _SECRETSTORE.fields_by_name['keyfactor_x_509']._serialized_options = b'\362\370\263\007\'\312\363\263\007\"\302\364\263\007\035\n\014json_gateway\022\rkeyfactorX509\362\370\263\007\005\260\363\263\007\001'
+  _SECRETSTORE.fields_by_name['vault_awsec_2']._options = None
+  _SECRETSTORE.fields_by_name['vault_awsec_2']._serialized_options = b'\362\370\263\007%\312\363\263\007 \302\364\263\007\033\n\014json_gateway\022\013vaultAWSEC2\362\370\263\007\005\260\363\263\007\001'
+  _SECRETSTORE.fields_by_name['vault_awsiam']._options = None
+  _SECRETSTORE.fields_by_name['vault_awsiam']._serialized_options = b'\362\370\263\007%\312\363\263\007 \302\364\263\007\033\n\014json_gateway\022\013vaultAWSIAM\362\370\263\007\005\260\363\263\007\001'
   _SECRETSTORE.fields_by_name['vault_app_role']._options = None
   _SECRETSTORE.fields_by_name['vault_app_role']._serialized_options = b'\362\370\263\007&\312\363\263\007!\302\364\263\007\034\n\014json_gateway\022\014vaultAppRole\362\370\263\007\005\260\363\263\007\001'
   _SECRETSTORE.fields_by_name['vault_app_role_cert_ssh']._options = None
   _SECRETSTORE.fields_by_name['vault_app_role_cert_ssh']._serialized_options = b'\362\370\263\007-\312\363\263\007(\302\364\263\007#\n\014json_gateway\022\023vaultAppRoleCertSSH\362\370\263\007\005\260\363\263\007\001'
   _SECRETSTORE.fields_by_name['vault_app_role_cert_x_509']._options = None
   _SECRETSTORE.fields_by_name['vault_app_role_cert_x_509']._serialized_options = b'\362\370\263\007.\312\363\263\007)\302\364\263\007$\n\014json_gateway\022\024vaultAppRoleCertX509\362\370\263\007\005\260\363\263\007\001'
   _SECRETSTORE.fields_by_name['vault_tls']._options = None
@@ -426,14 +446,38 @@
   _KEYFACTORX509STORE.fields_by_name['key_file_path']._serialized_options = b'\362\370\263\007*\260\363\263\007\001\312\363\263\007 \302\364\263\007\033\n\014json_gateway\022\013keyFilePath'
   _KEYFACTORX509STORE.fields_by_name['server_address']._options = None
   _KEYFACTORX509STORE.fields_by_name['server_address']._serialized_options = b'\362\370\263\0071\260\363\263\007\001\300\363\263\007\001\312\363\263\007\"\302\364\263\007\035\n\014json_gateway\022\rserverAddress'
   _KEYFACTORX509STORE.fields_by_name['tags']._options = None
   _KEYFACTORX509STORE.fields_by_name['tags']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _KEYFACTORX509STORE._options = None
   _KEYFACTORX509STORE._serialized_options = b'\372\370\263\007E\250\363\263\007\001\312\363\263\007;\302\364\263\007\024\n\003cli\022\rkeyfactorX509\302\364\263\007\035\n\014json_gateway\022\rkeyfactorX509'
+  _VAULTAWSEC2STORE.fields_by_name['id']._options = None
+  _VAULTAWSEC2STORE.fields_by_name['id']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
+  _VAULTAWSEC2STORE.fields_by_name['name']._options = None
+  _VAULTAWSEC2STORE.fields_by_name['name']._serialized_options = b'\362\370\263\007\n\260\363\263\007\001\300\363\263\007\001'
+  _VAULTAWSEC2STORE.fields_by_name['namespace']._options = None
+  _VAULTAWSEC2STORE.fields_by_name['namespace']._serialized_options = b'\362\370\263\007(\260\363\263\007\001\312\363\263\007\036\302\364\263\007\031\n\014json_gateway\022\tnamespace'
+  _VAULTAWSEC2STORE.fields_by_name['server_address']._options = None
+  _VAULTAWSEC2STORE.fields_by_name['server_address']._serialized_options = b'\362\370\263\0071\260\363\263\007\001\300\363\263\007\001\312\363\263\007\"\302\364\263\007\035\n\014json_gateway\022\rserverAddress'
+  _VAULTAWSEC2STORE.fields_by_name['tags']._options = None
+  _VAULTAWSEC2STORE.fields_by_name['tags']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
+  _VAULTAWSEC2STORE._options = None
+  _VAULTAWSEC2STORE._serialized_options = b'\372\370\263\007n\250\363\263\007\001\312\363\263\007d\210\364\263\007\001\302\364\263\007\022\n\003cli\022\013vaultAWSEC2\302\364\263\007\033\n\014json_gateway\022\013vaultAWSEC2\302\364\263\007#\n\022terraform-provider\022\rvault_aws_ec2'
+  _VAULTAWSIAMSTORE.fields_by_name['id']._options = None
+  _VAULTAWSIAMSTORE.fields_by_name['id']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
+  _VAULTAWSIAMSTORE.fields_by_name['name']._options = None
+  _VAULTAWSIAMSTORE.fields_by_name['name']._serialized_options = b'\362\370\263\007\n\260\363\263\007\001\300\363\263\007\001'
+  _VAULTAWSIAMSTORE.fields_by_name['namespace']._options = None
+  _VAULTAWSIAMSTORE.fields_by_name['namespace']._serialized_options = b'\362\370\263\007(\260\363\263\007\001\312\363\263\007\036\302\364\263\007\031\n\014json_gateway\022\tnamespace'
+  _VAULTAWSIAMSTORE.fields_by_name['server_address']._options = None
+  _VAULTAWSIAMSTORE.fields_by_name['server_address']._serialized_options = b'\362\370\263\0071\260\363\263\007\001\300\363\263\007\001\312\363\263\007\"\302\364\263\007\035\n\014json_gateway\022\rserverAddress'
+  _VAULTAWSIAMSTORE.fields_by_name['tags']._options = None
+  _VAULTAWSIAMSTORE.fields_by_name['tags']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
+  _VAULTAWSIAMSTORE._options = None
+  _VAULTAWSIAMSTORE._serialized_options = b'\372\370\263\007n\250\363\263\007\001\312\363\263\007d\210\364\263\007\001\302\364\263\007\022\n\003cli\022\013vaultAWSIAM\302\364\263\007\033\n\014json_gateway\022\013vaultAWSIAM\302\364\263\007#\n\022terraform-provider\022\rvault_aws_iam'
   _VAULTAPPROLESTORE.fields_by_name['id']._options = None
   _VAULTAPPROLESTORE.fields_by_name['id']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _VAULTAPPROLESTORE.fields_by_name['name']._options = None
   _VAULTAPPROLESTORE.fields_by_name['name']._serialized_options = b'\362\370\263\007\n\260\363\263\007\001\300\363\263\007\001'
   _VAULTAPPROLESTORE.fields_by_name['namespace']._options = None
   _VAULTAPPROLESTORE.fields_by_name['namespace']._serialized_options = b'\362\370\263\007(\260\363\263\007\001\312\363\263\007\036\302\364\263\007\031\n\014json_gateway\022\tnamespace'
   _VAULTAPPROLESTORE.fields_by_name['server_address']._options = None
@@ -589,51 +633,55 @@
   _VAULTTOKENCERTX509STORE.fields_by_name['signing_role']._options = None
   _VAULTTOKENCERTX509STORE.fields_by_name['signing_role']._serialized_options = b'\362\370\263\007/\260\363\263\007\001\300\363\263\007\001\312\363\263\007 \302\364\263\007\033\n\014json_gateway\022\013signingRole'
   _VAULTTOKENCERTX509STORE.fields_by_name['tags']._options = None
   _VAULTTOKENCERTX509STORE.fields_by_name['tags']._serialized_options = b'\362\370\263\007\005\260\363\263\007\001'
   _VAULTTOKENCERTX509STORE._options = None
   _VAULTTOKENCERTX509STORE._serialized_options = b'\372\370\263\007\177\250\363\263\007\001\312\363\263\007u\302\364\263\007\031\n\003cli\022\022vaultTokenCertX509\302\364\263\007\"\n\014json_gateway\022\022vaultTokenCertX509\302\364\263\007+\n\022terraform-provider\022\025vault_token_cert_x509'
   _SECRETSTORE._serialized_start=60
-  _SECRETSTORE._serialized_end=2358
-  _AWSSTORE._serialized_start=2361
-  _AWSSTORE._serialized_end=2613
-  _AWSCERTX509STORE._serialized_start=2616
-  _AWSCERTX509STORE._serialized_end=3230
-  _ACTIVEDIRECTORYSTORE._serialized_start=3233
-  _ACTIVEDIRECTORYSTORE._serialized_end=3508
-  _AZURESTORE._serialized_start=3511
-  _AZURESTORE._serialized_end=3746
-  _CYBERARKCONJURSTORE._serialized_start=3749
-  _CYBERARKCONJURSTORE._serialized_end=4048
-  _CYBERARKPAMSTORE._serialized_start=4051
-  _CYBERARKPAMSTORE._serialized_end=4338
-  _CYBERARKPAMEXPERIMENTALSTORE._serialized_start=4341
-  _CYBERARKPAMEXPERIMENTALSTORE._serialized_end=4685
-  _DELINEASTORE._serialized_start=4688
-  _DELINEASTORE._serialized_end=4995
-  _GCPSTORE._serialized_start=4998
-  _GCPSTORE._serialized_end=5228
-  _GCPCERTX509STORE._serialized_start=5231
-  _GCPCERTX509STORE._serialized_end=5772
-  _KEYFACTORSSHSTORE._serialized_start=5775
-  _KEYFACTORSSHSTORE._serialized_end=6809
-  _KEYFACTORX509STORE._serialized_start=6812
-  _KEYFACTORX509STORE._serialized_end=7849
-  _VAULTAPPROLESTORE._serialized_start=7852
-  _VAULTAPPROLESTORE._serialized_end=8222
-  _VAULTAPPROLECERTSSHSTORE._serialized_start=8225
-  _VAULTAPPROLECERTSSHSTORE._serialized_end=8877
-  _VAULTAPPROLECERTX509STORE._serialized_start=8880
-  _VAULTAPPROLECERTX509STORE._serialized_end=9536
-  _VAULTTLSSTORE._serialized_start=9539
-  _VAULTTLSSTORE._serialized_end=10127
-  _VAULTTLSCERTSSHSTORE._serialized_start=10130
-  _VAULTTLSCERTSSHSTORE._serialized_end=10998
-  _VAULTTLSCERTX509STORE._serialized_start=11001
-  _VAULTTLSCERTX509STORE._serialized_end=11873
-  _VAULTTOKENSTORE._serialized_start=11876
-  _VAULTTOKENSTORE._serialized_end=12238
-  _VAULTTOKENCERTSSHSTORE._serialized_start=12241
-  _VAULTTOKENCERTSSHSTORE._serialized_end=12884
-  _VAULTTOKENCERTX509STORE._serialized_start=12887
-  _VAULTTOKENCERTX509STORE._serialized_end=13534
+  _SECRETSTORE._serialized_end=2559
+  _AWSSTORE._serialized_start=2562
+  _AWSSTORE._serialized_end=2814
+  _AWSCERTX509STORE._serialized_start=2817
+  _AWSCERTX509STORE._serialized_end=3431
+  _ACTIVEDIRECTORYSTORE._serialized_start=3434
+  _ACTIVEDIRECTORYSTORE._serialized_end=3709
+  _AZURESTORE._serialized_start=3712
+  _AZURESTORE._serialized_end=3947
+  _CYBERARKCONJURSTORE._serialized_start=3950
+  _CYBERARKCONJURSTORE._serialized_end=4249
+  _CYBERARKPAMSTORE._serialized_start=4252
+  _CYBERARKPAMSTORE._serialized_end=4539
+  _CYBERARKPAMEXPERIMENTALSTORE._serialized_start=4542
+  _CYBERARKPAMEXPERIMENTALSTORE._serialized_end=4886
+  _DELINEASTORE._serialized_start=4889
+  _DELINEASTORE._serialized_end=5196
+  _GCPSTORE._serialized_start=5199
+  _GCPSTORE._serialized_end=5429
+  _GCPCERTX509STORE._serialized_start=5432
+  _GCPCERTX509STORE._serialized_end=5973
+  _KEYFACTORSSHSTORE._serialized_start=5976
+  _KEYFACTORSSHSTORE._serialized_end=7010
+  _KEYFACTORX509STORE._serialized_start=7013
+  _KEYFACTORX509STORE._serialized_end=8050
+  _VAULTAWSEC2STORE._serialized_start=8053
+  _VAULTAWSEC2STORE._serialized_end=8425
+  _VAULTAWSIAMSTORE._serialized_start=8428
+  _VAULTAWSIAMSTORE._serialized_end=8800
+  _VAULTAPPROLESTORE._serialized_start=8803
+  _VAULTAPPROLESTORE._serialized_end=9173
+  _VAULTAPPROLECERTSSHSTORE._serialized_start=9176
+  _VAULTAPPROLECERTSSHSTORE._serialized_end=9828
+  _VAULTAPPROLECERTX509STORE._serialized_start=9831
+  _VAULTAPPROLECERTX509STORE._serialized_end=10487
+  _VAULTTLSSTORE._serialized_start=10490
+  _VAULTTLSSTORE._serialized_end=11078
+  _VAULTTLSCERTSSHSTORE._serialized_start=11081
+  _VAULTTLSCERTSSHSTORE._serialized_end=11949
+  _VAULTTLSCERTX509STORE._serialized_start=11952
+  _VAULTTLSCERTX509STORE._serialized_end=12824
+  _VAULTTOKENSTORE._serialized_start=12827
+  _VAULTTOKENSTORE._serialized_end=13189
+  _VAULTTOKENCERTSSHSTORE._serialized_start=13192
+  _VAULTTOKENCERTSSHSTORE._serialized_end=13835
+  _VAULTTOKENCERTX509STORE._serialized_start=13838
+  _VAULTTOKENCERTX509STORE._serialized_end=14485
 # @@protoc_insertion_point(module_scope)
```

## Comparing `strongdm-8.3.0/strongdm/account_resources_pb2_grpc.py` & `strongdm-8.4.0/strongdm/account_resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/roles_history_pb2.py` & `strongdm-8.4.0/strongdm/roles_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/replays_pb2.py` & `strongdm-8.4.0/strongdm/replays_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/drivers_pb2_grpc.py` & `strongdm-8.4.0/strongdm/tags_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/secret_stores_pb2_grpc.py` & `strongdm-8.4.0/strongdm/secret_stores_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/workflow_roles_history_pb2.py` & `strongdm-8.4.0/strongdm/workflow_roles_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/approval_workflow_approvers_pb2.py` & `strongdm-8.4.0/strongdm/approval_workflow_approvers_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/options_pb2.py` & `strongdm-8.4.0/strongdm/options_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/access_requests_pb2_grpc.py` & `strongdm-8.4.0/strongdm/access_requests_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/remote_identities_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/remote_identities_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/role_resources_pb2_grpc.py` & `strongdm-8.4.0/strongdm/role_resources_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/nodes_history_pb2.py` & `strongdm-8.4.0/strongdm/nodes_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/account_grants_history_pb2.py` & `strongdm-8.4.0/strongdm/account_grants_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/resources_history_pb2.py` & `strongdm-8.4.0/strongdm/resources_history_pb2.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/nodes_history_pb2_grpc.py` & `strongdm-8.4.0/strongdm/nodes_history_pb2_grpc.py`

 * *Files identical despite different names*

## Comparing `strongdm-8.3.0/strongdm/remote_identity_groups_pb2_grpc.py` & `strongdm-8.4.0/strongdm/remote_identity_groups_pb2_grpc.py`

 * *Files identical despite different names*

