# Comparing `tmp/kthcloud-0.3.0a0.tar.gz` & `tmp/kthcloud-0.4.0a0.tar.gz`

## Comparing `kthcloud-0.3.0a0.tar` & `kthcloud-0.4.0a0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
--rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/__init__.py
--rw-r--r--   0        0        0    64414 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_base_client.py
--rw-r--r--   0        0        0    17628 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_client.py
--rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_compat.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_constants.py
--rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_exceptions.py
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_files.py
--rw-r--r--   0        0        0    26096 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_models.py
--rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_qs.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_resource.py
--rw-r--r--   0        0        0    28489 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_response.py
--rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_streaming.py
--rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_types.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/py.typed
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_utils/__init__.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_utils/_logs.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_utils/_proxy.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_utils/_streams.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_utils/_sync.py
--rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_utils/_transform.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_utils/_typing.py
--rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_utils/_utils.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/lib/.keep
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/resources/__init__.py
--rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/resources/gpu_groups.py
--rw-r--r--   0        0        0    20320 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/resources/gpu_leases.py
--rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/resources/snapshots.py
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/resources/vm_actions.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/resources/vms/__init__.py
--rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/resources/vms/snapshot.py
--rw-r--r--   0        0        0    21148 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/resources/vms/vms.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/__init__.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/gpu_group.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/gpu_group_list_params.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/gpu_group_list_response.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_create_params.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_created.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_deleted.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_list_params.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_list_response.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_read.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_update_params.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_updated.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/snapshot_list_params.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/snapshot_list_response.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/vm_action_create_params.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/vm_action_created.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/vm_create_params.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/vm_created.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/vm_deleted.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/vm_list_params.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/vm_list_response.py
--rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/vm_read.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/vm_snapshot_created.py
--rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/vm_update_params.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/vm_updated.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/shared/__init__.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/shared/vm_snapshot_read.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/vms/__init__.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/vms/vm_snapshot_deleted.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/.gitignore
--rw-r--r--   0        0        0    11351 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/LICENSE
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/pyproject.toml
--rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 kthcloud-0.3.0a0/PKG-INFO
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v2/lib/.keep
+-rw-r--r--   0        0        0     2557 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/__init__.py
+-rw-r--r--   0        0        0    64414 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_base_client.py
+-rw-r--r--   0        0        0    17628 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_client.py
+-rw-r--r--   0        0        0     6389 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_compat.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_constants.py
+-rw-r--r--   0        0        0     3244 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_exceptions.py
+-rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_files.py
+-rw-r--r--   0        0        0    26876 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_models.py
+-rw-r--r--   0        0        0     4846 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_qs.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_resource.py
+-rw-r--r--   0        0        0    28489 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_response.py
+-rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_streaming.py
+-rw-r--r--   0        0        0     6142 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_types.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/py.typed
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/__init__.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_logs.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_proxy.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_streams.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_sync.py
+-rw-r--r--   0        0        0    12958 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_transform.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_typing.py
+-rw-r--r--   0        0        0    11497 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_utils.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/lib/.keep
+-rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/__init__.py
+-rw-r--r--   0        0        0     8641 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/gpu_groups.py
+-rw-r--r--   0        0        0    20320 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/gpu_leases.py
+-rw-r--r--   0        0        0     7678 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/snapshots.py
+-rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/vm_actions.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/vms/__init__.py
+-rw-r--r--   0        0        0     5200 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/vms/snapshot.py
+-rw-r--r--   0        0        0    21148 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/vms/vms.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/__init__.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_group.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_group_list_params.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_group_list_response.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_create_params.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_created.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_deleted.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_list_params.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_list_response.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_read.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_update_params.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_updated.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/snapshot_list_params.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/snapshot_list_response.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_action_create_params.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_action_created.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_create_params.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_created.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_deleted.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_list_params.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_list_response.py
+-rw-r--r--   0        0        0     3180 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_read.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_snapshot_created.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_update_params.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_updated.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/shared/__init__.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/shared/vm_snapshot_read.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vms/__init__.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vms/vm_snapshot_deleted.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/.gitignore
+-rw-r--r--   0        0        0    11351 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/LICENSE
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0    12680 2020-02-02 00:00:00.000000 kthcloud-0.4.0a0/PKG-INFO
```

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/__init__.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,16 +78,16 @@
 ]
 
 _setup_logging()
 
 # Update the __module__ attribute for exported symbols so that
 # error messages point to this module instead of the module
 # it was originally defined in, e.g.
-# kthcloud_go_deploy_v2._exceptions.NotFoundError -> kthcloud_go_deploy_v2.NotFoundError
+# kthcloud_go_deploy_v_._exceptions.NotFoundError -> kthcloud_go_deploy_v_.NotFoundError
 __locals = locals()
 for __name in __all__:
     if not __name.startswith("__"):
         try:
-            __locals[__name].__module__ = "kthcloud_go_deploy_v2"
+            __locals[__name].__module__ = "kthcloud_go_deploy_v_"
         except (TypeError, AttributeError):
             # Some of our exported symbols are builtins which we can't set attributes for.
             pass
```

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_base_client.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_base_client.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_client.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,16 +42,16 @@
     "AsyncKthcloudGoDeployV2",
     "Client",
     "AsyncClient",
 ]
 
 
 class KthcloudGoDeployV2(SyncAPIClient):
-    gpu_groups: resources.GpuGroupsResource
-    gpu_leases: resources.GpuLeasesResource
+    gpu_groups: resources.GPUGroupsResource
+    gpu_leases: resources.GPULeasesResource
     snapshots: resources.SnapshotsResource
     vm_actions: resources.VmActionsResource
     vms: resources.VmsResource
     with_raw_response: KthcloudGoDeployV2WithRawResponse
     with_streaming_response: KthcloudGoDeployV2WithStreamedResponse
 
     # client options
@@ -104,16 +104,16 @@
             timeout=timeout,
             http_client=http_client,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
-        self.gpu_groups = resources.GpuGroupsResource(self)
-        self.gpu_leases = resources.GpuLeasesResource(self)
+        self.gpu_groups = resources.GPUGroupsResource(self)
+        self.gpu_leases = resources.GPULeasesResource(self)
         self.snapshots = resources.SnapshotsResource(self)
         self.vm_actions = resources.VmActionsResource(self)
         self.vms = resources.VmsResource(self)
         self.with_raw_response = KthcloudGoDeployV2WithRawResponse(self)
         self.with_streaming_response = KthcloudGoDeployV2WithStreamedResponse(self)
 
     @property
@@ -218,16 +218,16 @@
 
         if response.status_code >= 500:
             return _exceptions.InternalServerError(err_msg, response=response, body=body)
         return APIStatusError(err_msg, response=response, body=body)
 
 
 class AsyncKthcloudGoDeployV2(AsyncAPIClient):
-    gpu_groups: resources.AsyncGpuGroupsResource
-    gpu_leases: resources.AsyncGpuLeasesResource
+    gpu_groups: resources.AsyncGPUGroupsResource
+    gpu_leases: resources.AsyncGPULeasesResource
     snapshots: resources.AsyncSnapshotsResource
     vm_actions: resources.AsyncVmActionsResource
     vms: resources.AsyncVmsResource
     with_raw_response: AsyncKthcloudGoDeployV2WithRawResponse
     with_streaming_response: AsyncKthcloudGoDeployV2WithStreamedResponse
 
     # client options
@@ -280,16 +280,16 @@
             timeout=timeout,
             http_client=http_client,
             custom_headers=default_headers,
             custom_query=default_query,
             _strict_response_validation=_strict_response_validation,
         )
 
-        self.gpu_groups = resources.AsyncGpuGroupsResource(self)
-        self.gpu_leases = resources.AsyncGpuLeasesResource(self)
+        self.gpu_groups = resources.AsyncGPUGroupsResource(self)
+        self.gpu_leases = resources.AsyncGPULeasesResource(self)
         self.snapshots = resources.AsyncSnapshotsResource(self)
         self.vm_actions = resources.AsyncVmActionsResource(self)
         self.vms = resources.AsyncVmsResource(self)
         self.with_raw_response = AsyncKthcloudGoDeployV2WithRawResponse(self)
         self.with_streaming_response = AsyncKthcloudGoDeployV2WithStreamedResponse(self)
 
     @property
@@ -395,43 +395,43 @@
         if response.status_code >= 500:
             return _exceptions.InternalServerError(err_msg, response=response, body=body)
         return APIStatusError(err_msg, response=response, body=body)
 
 
 class KthcloudGoDeployV2WithRawResponse:
     def __init__(self, client: KthcloudGoDeployV2) -> None:
-        self.gpu_groups = resources.GpuGroupsResourceWithRawResponse(client.gpu_groups)
-        self.gpu_leases = resources.GpuLeasesResourceWithRawResponse(client.gpu_leases)
+        self.gpu_groups = resources.GPUGroupsResourceWithRawResponse(client.gpu_groups)
+        self.gpu_leases = resources.GPULeasesResourceWithRawResponse(client.gpu_leases)
         self.snapshots = resources.SnapshotsResourceWithRawResponse(client.snapshots)
         self.vm_actions = resources.VmActionsResourceWithRawResponse(client.vm_actions)
         self.vms = resources.VmsResourceWithRawResponse(client.vms)
 
 
 class AsyncKthcloudGoDeployV2WithRawResponse:
     def __init__(self, client: AsyncKthcloudGoDeployV2) -> None:
-        self.gpu_groups = resources.AsyncGpuGroupsResourceWithRawResponse(client.gpu_groups)
-        self.gpu_leases = resources.AsyncGpuLeasesResourceWithRawResponse(client.gpu_leases)
+        self.gpu_groups = resources.AsyncGPUGroupsResourceWithRawResponse(client.gpu_groups)
+        self.gpu_leases = resources.AsyncGPULeasesResourceWithRawResponse(client.gpu_leases)
         self.snapshots = resources.AsyncSnapshotsResourceWithRawResponse(client.snapshots)
         self.vm_actions = resources.AsyncVmActionsResourceWithRawResponse(client.vm_actions)
         self.vms = resources.AsyncVmsResourceWithRawResponse(client.vms)
 
 
 class KthcloudGoDeployV2WithStreamedResponse:
     def __init__(self, client: KthcloudGoDeployV2) -> None:
-        self.gpu_groups = resources.GpuGroupsResourceWithStreamingResponse(client.gpu_groups)
-        self.gpu_leases = resources.GpuLeasesResourceWithStreamingResponse(client.gpu_leases)
+        self.gpu_groups = resources.GPUGroupsResourceWithStreamingResponse(client.gpu_groups)
+        self.gpu_leases = resources.GPULeasesResourceWithStreamingResponse(client.gpu_leases)
         self.snapshots = resources.SnapshotsResourceWithStreamingResponse(client.snapshots)
         self.vm_actions = resources.VmActionsResourceWithStreamingResponse(client.vm_actions)
         self.vms = resources.VmsResourceWithStreamingResponse(client.vms)
 
 
 class AsyncKthcloudGoDeployV2WithStreamedResponse:
     def __init__(self, client: AsyncKthcloudGoDeployV2) -> None:
-        self.gpu_groups = resources.AsyncGpuGroupsResourceWithStreamingResponse(client.gpu_groups)
-        self.gpu_leases = resources.AsyncGpuLeasesResourceWithStreamingResponse(client.gpu_leases)
+        self.gpu_groups = resources.AsyncGPUGroupsResourceWithStreamingResponse(client.gpu_groups)
+        self.gpu_leases = resources.AsyncGPULeasesResourceWithStreamingResponse(client.gpu_leases)
         self.snapshots = resources.AsyncSnapshotsResourceWithStreamingResponse(client.snapshots)
         self.vm_actions = resources.AsyncVmActionsResourceWithStreamingResponse(client.vm_actions)
         self.vms = resources.AsyncVmsResourceWithStreamingResponse(client.vms)
 
 
 Client = KthcloudGoDeployV2
```

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_compat.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_compat.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_exceptions.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_exceptions.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_files.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_files.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_models.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     get_model_config,
     get_model_fields,
     field_get_default,
 )
 from ._constants import RAW_RESPONSE_HEADER
 
 if TYPE_CHECKING:
-    from pydantic_core.core_schema import ModelField, ModelFieldsSchema
+    from pydantic_core.core_schema import ModelField, LiteralSchema, ModelFieldsSchema
 
 __all__ = ["BaseModel", "GenericModel"]
 
 _T = TypeVar("_T")
 
 
 @runtime_checkable
@@ -247,15 +247,17 @@
             include: IncEx = None,
             exclude: IncEx = None,
             by_alias: bool = False,
             exclude_unset: bool = False,
             exclude_defaults: bool = False,
             exclude_none: bool = False,
             round_trip: bool = False,
-            warnings: bool = True,
+            warnings: bool | Literal["none", "warn", "error"] = True,
+            context: dict[str, Any] | None = None,
+            serialize_as_any: bool = False,
         ) -> dict[str, Any]:
             """Usage docs: https://docs.pydantic.dev/2.4/concepts/serialization/#modelmodel_dump
 
             Generate a dictionary representation of the model, optionally specifying which fields to include or exclude.
 
             Args:
                 mode: The mode in which `to_python` should run.
@@ -275,14 +277,18 @@
             """
             if mode != "python":
                 raise ValueError("mode is only supported in Pydantic v2")
             if round_trip != False:
                 raise ValueError("round_trip is only supported in Pydantic v2")
             if warnings != True:
                 raise ValueError("warnings is only supported in Pydantic v2")
+            if context is not None:
+                raise ValueError("context is only supported in Pydantic v2")
+            if serialize_as_any != False:
+                raise ValueError("serialize_as_any is only supported in Pydantic v2")
             return super().dict(  # pyright: ignore[reportDeprecated]
                 include=include,
                 exclude=exclude,
                 by_alias=by_alias,
                 exclude_unset=exclude_unset,
                 exclude_defaults=exclude_defaults,
                 exclude_none=exclude_none,
@@ -296,15 +302,17 @@
             include: IncEx = None,
             exclude: IncEx = None,
             by_alias: bool = False,
             exclude_unset: bool = False,
             exclude_defaults: bool = False,
             exclude_none: bool = False,
             round_trip: bool = False,
-            warnings: bool = True,
+            warnings: bool | Literal["none", "warn", "error"] = True,
+            context: dict[str, Any] | None = None,
+            serialize_as_any: bool = False,
         ) -> str:
             """Usage docs: https://docs.pydantic.dev/2.4/concepts/serialization/#modelmodel_dump_json
 
             Generates a JSON representation of the model using Pydantic's `to_json` method.
 
             Args:
                 indent: Indentation to use in the JSON output. If None is passed, the output will be compact.
@@ -320,14 +328,18 @@
             Returns:
                 A JSON string representation of the model.
             """
             if round_trip != False:
                 raise ValueError("round_trip is only supported in Pydantic v2")
             if warnings != True:
                 raise ValueError("warnings is only supported in Pydantic v2")
+            if context is not None:
+                raise ValueError("context is only supported in Pydantic v2")
+            if serialize_as_any != False:
+                raise ValueError("serialize_as_any is only supported in Pydantic v2")
             return super().json(  # type: ignore[reportDeprecated]
                 indent=indent,
                 include=include,
                 exclude=exclude,
                 by_alias=by_alias,
                 exclude_unset=exclude_unset,
                 exclude_defaults=exclude_defaults,
@@ -546,15 +558,15 @@
 
                 # Note: if one variant defines an alias then they all should
                 discriminator_alias = field.get("serialization_alias")
 
                 field_schema = field["schema"]
 
                 if field_schema["type"] == "literal":
-                    for entry in field_schema["expected"]:
+                    for entry in cast("LiteralSchema", field_schema)["expected"]:
                         if isinstance(entry, str):
                             mapping[entry] = variant
             else:
                 field_info = cast("dict[str, FieldInfo]", variant.__fields__).get(discriminator_field_name)  # pyright: ignore[reportDeprecated, reportUnnecessaryCast]
                 if not field_info:
                     continue
```

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_qs.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_qs.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_resource.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_resource.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_response.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
             # as it would be easy to incorrectly construct the Response object due to the multitude of arguments.
             if cast_to != httpx.Response:
                 raise ValueError(f"Subclasses of httpx.Response cannot be passed to `cast_to`")
             return cast(R, response)
 
         if inspect.isclass(origin) and not issubclass(origin, BaseModel) and issubclass(origin, pydantic.BaseModel):
             raise TypeError(
-                "Pydantic models must subclass our base model type, e.g. `from kthcloud_go_deploy_v2 import BaseModel`"
+                "Pydantic models must subclass our base model type, e.g. `from kthcloud_go_deploy_v_ import BaseModel`"
             )
 
         if (
             cast_to is not object
             and not origin is list
             and not origin is dict
             and not origin is Union
@@ -269,15 +269,15 @@
 
         For lower-level control, see `.read()`, `.json()`, `.iter_bytes()`.
 
         You can customise the type that the response is parsed into through
         the `to` argument, e.g.
 
         ```py
-        from kthcloud_go_deploy_v2 import BaseModel
+        from kthcloud_go_deploy_v_ import BaseModel
 
 
         class MyModel(BaseModel):
             foo: str
 
 
         obj = response.parse(to=MyModel)
@@ -373,15 +373,15 @@
 
         For lower-level control, see `.read()`, `.json()`, `.iter_bytes()`.
 
         You can customise the type that the response is parsed into through
         the `to` argument, e.g.
 
         ```py
-        from kthcloud_go_deploy_v2 import BaseModel
+        from kthcloud_go_deploy_v_ import BaseModel
 
 
         class MyModel(BaseModel):
             foo: str
 
 
         obj = response.parse(to=MyModel)
@@ -544,15 +544,15 @@
             async for data in self.iter_bytes(chunk_size):
                 await f.write(data)
 
 
 class MissingStreamClassError(TypeError):
     def __init__(self) -> None:
         super().__init__(
-            "The `stream` argument was set to `True` but the `stream_cls` argument was not given. See `kthcloud_go_deploy_v2._streaming` for reference",
+            "The `stream` argument was set to `True` but the `stream_cls` argument was not given. See `kthcloud_go_deploy_v_._streaming` for reference",
         )
 
 
 class StreamAlreadyConsumed(KthcloudGoDeployV2Error):
     """
     Attempted to read or stream content, but the content has already
     been streamed.
```

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_streaming.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_streaming.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_types.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 # method that uses `ResponseT` which would lead to an unacceptable
 # amount of code duplication and make it unreadable. See _base_client.py
 # for example usage.
 #
 # This unfortunately means that you will either have
 # to import this type and pass it explicitly:
 #
-# from kthcloud_go_deploy_v2 import NoneType
+# from kthcloud_go_deploy_v_ import NoneType
 # client.get('/foo', cast_to=NoneType)
 #
 # or build it yourself:
 #
 # client.get('/foo', cast_to=type(None))
 if TYPE_CHECKING:
     NoneType: Type[None]
```

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_utils/__init__.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_utils/_logs.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_logs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import logging
 
-logger: logging.Logger = logging.getLogger("kthcloud_go_deploy_v2")
+logger: logging.Logger = logging.getLogger("kthcloud_go_deploy_v_")
 httpx_logger: logging.Logger = logging.getLogger("httpx")
 
 
 def _basic_config() -> None:
-    # e.g. [2023-10-05 14:12:26 - kthcloud_go_deploy_v2._base_client:818 - DEBUG] HTTP Request: POST http://127.0.0.1:4010/foo/bar "200 OK"
+    # e.g. [2023-10-05 14:12:26 - kthcloud_go_deploy_v_._base_client:818 - DEBUG] HTTP Request: POST http://127.0.0.1:4010/foo/bar "200 OK"
     logging.basicConfig(
         format="[%(asctime)s - %(name)s:%(lineno)d - %(levelname)s] %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
 
 
 def setup_logging() -> None:
```

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_utils/_proxy.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_proxy.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_utils/_sync.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_sync.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_utils/_transform.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_utils/_typing.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_typing.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/_utils/_utils.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/resources/__init__.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,51 +13,51 @@
     AsyncSnapshotsResource,
     SnapshotsResourceWithRawResponse,
     AsyncSnapshotsResourceWithRawResponse,
     SnapshotsResourceWithStreamingResponse,
     AsyncSnapshotsResourceWithStreamingResponse,
 )
 from .gpu_groups import (
-    GpuGroupsResource,
-    AsyncGpuGroupsResource,
-    GpuGroupsResourceWithRawResponse,
-    AsyncGpuGroupsResourceWithRawResponse,
-    GpuGroupsResourceWithStreamingResponse,
-    AsyncGpuGroupsResourceWithStreamingResponse,
+    GPUGroupsResource,
+    AsyncGPUGroupsResource,
+    GPUGroupsResourceWithRawResponse,
+    AsyncGPUGroupsResourceWithRawResponse,
+    GPUGroupsResourceWithStreamingResponse,
+    AsyncGPUGroupsResourceWithStreamingResponse,
 )
 from .gpu_leases import (
-    GpuLeasesResource,
-    AsyncGpuLeasesResource,
-    GpuLeasesResourceWithRawResponse,
-    AsyncGpuLeasesResourceWithRawResponse,
-    GpuLeasesResourceWithStreamingResponse,
-    AsyncGpuLeasesResourceWithStreamingResponse,
+    GPULeasesResource,
+    AsyncGPULeasesResource,
+    GPULeasesResourceWithRawResponse,
+    AsyncGPULeasesResourceWithRawResponse,
+    GPULeasesResourceWithStreamingResponse,
+    AsyncGPULeasesResourceWithStreamingResponse,
 )
 from .vm_actions import (
     VmActionsResource,
     AsyncVmActionsResource,
     VmActionsResourceWithRawResponse,
     AsyncVmActionsResourceWithRawResponse,
     VmActionsResourceWithStreamingResponse,
     AsyncVmActionsResourceWithStreamingResponse,
 )
 
 __all__ = [
-    "GpuGroupsResource",
-    "AsyncGpuGroupsResource",
-    "GpuGroupsResourceWithRawResponse",
-    "AsyncGpuGroupsResourceWithRawResponse",
-    "GpuGroupsResourceWithStreamingResponse",
-    "AsyncGpuGroupsResourceWithStreamingResponse",
-    "GpuLeasesResource",
-    "AsyncGpuLeasesResource",
-    "GpuLeasesResourceWithRawResponse",
-    "AsyncGpuLeasesResourceWithRawResponse",
-    "GpuLeasesResourceWithStreamingResponse",
-    "AsyncGpuLeasesResourceWithStreamingResponse",
+    "GPUGroupsResource",
+    "AsyncGPUGroupsResource",
+    "GPUGroupsResourceWithRawResponse",
+    "AsyncGPUGroupsResourceWithRawResponse",
+    "GPUGroupsResourceWithStreamingResponse",
+    "AsyncGPUGroupsResourceWithStreamingResponse",
+    "GPULeasesResource",
+    "AsyncGPULeasesResource",
+    "GPULeasesResourceWithRawResponse",
+    "AsyncGPULeasesResourceWithRawResponse",
+    "GPULeasesResourceWithStreamingResponse",
+    "AsyncGPULeasesResourceWithStreamingResponse",
     "SnapshotsResource",
     "AsyncSnapshotsResource",
     "SnapshotsResourceWithRawResponse",
     "AsyncSnapshotsResourceWithRawResponse",
     "SnapshotsResourceWithStreamingResponse",
     "AsyncSnapshotsResourceWithStreamingResponse",
     "VmActionsResource",
```

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/resources/gpu_groups.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/gpu_groups.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,40 +17,40 @@
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
 from .._base_client import (
     make_request_options,
 )
-from ..types.gpu_group import GpuGroup
-from ..types.gpu_group_list_response import GpuGroupListResponse
+from ..types.gpu_group import GPUGroup
+from ..types.gpu_group_list_response import GPUGroupListResponse
 
-__all__ = ["GpuGroupsResource", "AsyncGpuGroupsResource"]
+__all__ = ["GPUGroupsResource", "AsyncGPUGroupsResource"]
 
 
-class GpuGroupsResource(SyncAPIResource):
+class GPUGroupsResource(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> GpuGroupsResourceWithRawResponse:
-        return GpuGroupsResourceWithRawResponse(self)
+    def with_raw_response(self) -> GPUGroupsResourceWithRawResponse:
+        return GPUGroupsResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> GpuGroupsResourceWithStreamingResponse:
-        return GpuGroupsResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> GPUGroupsResourceWithStreamingResponse:
+        return GPUGroupsResourceWithStreamingResponse(self)
 
     def retrieve(
         self,
         gpu_group_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> GpuGroup:
+    ) -> GPUGroup:
         """
         Get GPU group
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -62,29 +62,29 @@
         if not gpu_group_id:
             raise ValueError(f"Expected a non-empty value for `gpu_group_id` but received {gpu_group_id!r}")
         return self._get(
             f"/v2/gpuGroups/{gpu_group_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=GpuGroup,
+            cast_to=GPUGroup,
         )
 
     def list(
         self,
         *,
         page: int | NotGiven = NOT_GIVEN,
         page_size: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> GpuGroupListResponse:
+    ) -> GPUGroupListResponse:
         """
         List GPU groups
 
         Args:
           page: Page number
 
           page_size: Number of items per page
@@ -105,41 +105,41 @@
                 extra_body=extra_body,
                 timeout=timeout,
                 query=maybe_transform(
                     {
                         "page": page,
                         "page_size": page_size,
                     },
-                    gpu_group_list_params.GpuGroupListParams,
+                    gpu_group_list_params.GPUGroupListParams,
                 ),
             ),
-            cast_to=GpuGroupListResponse,
+            cast_to=GPUGroupListResponse,
         )
 
 
-class AsyncGpuGroupsResource(AsyncAPIResource):
+class AsyncGPUGroupsResource(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncGpuGroupsResourceWithRawResponse:
-        return AsyncGpuGroupsResourceWithRawResponse(self)
+    def with_raw_response(self) -> AsyncGPUGroupsResourceWithRawResponse:
+        return AsyncGPUGroupsResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncGpuGroupsResourceWithStreamingResponse:
-        return AsyncGpuGroupsResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncGPUGroupsResourceWithStreamingResponse:
+        return AsyncGPUGroupsResourceWithStreamingResponse(self)
 
     async def retrieve(
         self,
         gpu_group_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> GpuGroup:
+    ) -> GPUGroup:
         """
         Get GPU group
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -151,29 +151,29 @@
         if not gpu_group_id:
             raise ValueError(f"Expected a non-empty value for `gpu_group_id` but received {gpu_group_id!r}")
         return await self._get(
             f"/v2/gpuGroups/{gpu_group_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=GpuGroup,
+            cast_to=GPUGroup,
         )
 
     async def list(
         self,
         *,
         page: int | NotGiven = NOT_GIVEN,
         page_size: int | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> GpuGroupListResponse:
+    ) -> GPUGroupListResponse:
         """
         List GPU groups
 
         Args:
           page: Page number
 
           page_size: Number of items per page
@@ -194,59 +194,59 @@
                 extra_body=extra_body,
                 timeout=timeout,
                 query=await async_maybe_transform(
                     {
                         "page": page,
                         "page_size": page_size,
                     },
-                    gpu_group_list_params.GpuGroupListParams,
+                    gpu_group_list_params.GPUGroupListParams,
                 ),
             ),
-            cast_to=GpuGroupListResponse,
+            cast_to=GPUGroupListResponse,
         )
 
 
-class GpuGroupsResourceWithRawResponse:
-    def __init__(self, gpu_groups: GpuGroupsResource) -> None:
+class GPUGroupsResourceWithRawResponse:
+    def __init__(self, gpu_groups: GPUGroupsResource) -> None:
         self._gpu_groups = gpu_groups
 
         self.retrieve = to_raw_response_wrapper(
             gpu_groups.retrieve,
         )
         self.list = to_raw_response_wrapper(
             gpu_groups.list,
         )
 
 
-class AsyncGpuGroupsResourceWithRawResponse:
-    def __init__(self, gpu_groups: AsyncGpuGroupsResource) -> None:
+class AsyncGPUGroupsResourceWithRawResponse:
+    def __init__(self, gpu_groups: AsyncGPUGroupsResource) -> None:
         self._gpu_groups = gpu_groups
 
         self.retrieve = async_to_raw_response_wrapper(
             gpu_groups.retrieve,
         )
         self.list = async_to_raw_response_wrapper(
             gpu_groups.list,
         )
 
 
-class GpuGroupsResourceWithStreamingResponse:
-    def __init__(self, gpu_groups: GpuGroupsResource) -> None:
+class GPUGroupsResourceWithStreamingResponse:
+    def __init__(self, gpu_groups: GPUGroupsResource) -> None:
         self._gpu_groups = gpu_groups
 
         self.retrieve = to_streamed_response_wrapper(
             gpu_groups.retrieve,
         )
         self.list = to_streamed_response_wrapper(
             gpu_groups.list,
         )
 
 
-class AsyncGpuGroupsResourceWithStreamingResponse:
-    def __init__(self, gpu_groups: AsyncGpuGroupsResource) -> None:
+class AsyncGPUGroupsResourceWithStreamingResponse:
+    def __init__(self, gpu_groups: AsyncGPUGroupsResource) -> None:
         self._gpu_groups = gpu_groups
 
         self.retrieve = async_to_streamed_response_wrapper(
             gpu_groups.retrieve,
         )
         self.list = async_to_streamed_response_wrapper(
             gpu_groups.list,
```

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/resources/gpu_leases.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/gpu_leases.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,44 +17,44 @@
     to_streamed_response_wrapper,
     async_to_raw_response_wrapper,
     async_to_streamed_response_wrapper,
 )
 from .._base_client import (
     make_request_options,
 )
-from ..types.gpu_lease_read import GpuLeaseRead
-from ..types.gpu_lease_created import GpuLeaseCreated
-from ..types.gpu_lease_deleted import GpuLeaseDeleted
-from ..types.gpu_lease_updated import GpuLeaseUpdated
-from ..types.gpu_lease_list_response import GpuLeaseListResponse
+from ..types.gpu_lease_read import GPULeaseRead
+from ..types.gpu_lease_created import GPULeaseCreated
+from ..types.gpu_lease_deleted import GPULeaseDeleted
+from ..types.gpu_lease_updated import GPULeaseUpdated
+from ..types.gpu_lease_list_response import GPULeaseListResponse
 
-__all__ = ["GpuLeasesResource", "AsyncGpuLeasesResource"]
+__all__ = ["GPULeasesResource", "AsyncGPULeasesResource"]
 
 
-class GpuLeasesResource(SyncAPIResource):
+class GPULeasesResource(SyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> GpuLeasesResourceWithRawResponse:
-        return GpuLeasesResourceWithRawResponse(self)
+    def with_raw_response(self) -> GPULeasesResourceWithRawResponse:
+        return GPULeasesResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> GpuLeasesResourceWithStreamingResponse:
-        return GpuLeasesResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> GPULeasesResourceWithStreamingResponse:
+        return GPULeasesResourceWithStreamingResponse(self)
 
     def create(
         self,
         *,
         gpu_group_id: str,
         lease_forever: bool | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> GpuLeaseCreated:
+    ) -> GPULeaseCreated:
         """
         Create GPU lease
 
         Args:
           gpu_group_id: GpuGroupID is used to specify the GPU to lease. As such, the lease does not
               specify which specific GPU to lease, but rather the type of GPU to lease.
 
@@ -71,33 +71,33 @@
         return self._post(
             "/v2/gpuLeases",
             body=maybe_transform(
                 {
                     "gpu_group_id": gpu_group_id,
                     "lease_forever": lease_forever,
                 },
-                gpu_lease_create_params.GpuLeaseCreateParams,
+                gpu_lease_create_params.GPULeaseCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=GpuLeaseCreated,
+            cast_to=GPULeaseCreated,
         )
 
     def retrieve(
         self,
         gpu_lease_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> GpuLeaseRead:
+    ) -> GPULeaseRead:
         """
         Get GPU lease
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -109,29 +109,29 @@
         if not gpu_lease_id:
             raise ValueError(f"Expected a non-empty value for `gpu_lease_id` but received {gpu_lease_id!r}")
         return self._get(
             f"/v2/gpuLeases/{gpu_lease_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=GpuLeaseRead,
+            cast_to=GPULeaseRead,
         )
 
     def update(
         self,
         gpu_lease_id: str,
         *,
         vm_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> GpuLeaseUpdated:
+    ) -> GPULeaseUpdated:
         """
         Update GPU lease
 
         Args:
           vm_id: VmID is used to specify the VM to attach the lease to.
 
               - If specified, the lease will be attached to the VM.
@@ -151,19 +151,19 @@
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         if not gpu_lease_id:
             raise ValueError(f"Expected a non-empty value for `gpu_lease_id` but received {gpu_lease_id!r}")
         return self._post(
             f"/v2/gpuLeases/{gpu_lease_id}",
-            body=maybe_transform({"vm_id": vm_id}, gpu_lease_update_params.GpuLeaseUpdateParams),
+            body=maybe_transform({"vm_id": vm_id}, gpu_lease_update_params.GPULeaseUpdateParams),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=GpuLeaseUpdated,
+            cast_to=GPULeaseUpdated,
         )
 
     def list(
         self,
         *,
         all: bool | NotGiven = NOT_GIVEN,
         page: int | NotGiven = NOT_GIVEN,
@@ -171,15 +171,15 @@
         vm_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> GpuLeaseListResponse:
+    ) -> GPULeaseListResponse:
         """
         List GPU leases
 
         Args:
           all: List all
 
           page: Page number
@@ -206,31 +206,31 @@
                 query=maybe_transform(
                     {
                         "all": all,
                         "page": page,
                         "page_size": page_size,
                         "vm_id": vm_id,
                     },
-                    gpu_lease_list_params.GpuLeaseListParams,
+                    gpu_lease_list_params.GPULeaseListParams,
                 ),
             ),
-            cast_to=GpuLeaseListResponse,
+            cast_to=GPULeaseListResponse,
         )
 
     def delete(
         self,
         gpu_lease_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> GpuLeaseDeleted:
+    ) -> GPULeaseDeleted:
         """
         Delete GPU lease
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -242,39 +242,39 @@
         if not gpu_lease_id:
             raise ValueError(f"Expected a non-empty value for `gpu_lease_id` but received {gpu_lease_id!r}")
         return self._delete(
             f"/v2/gpuLeases/{gpu_lease_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=GpuLeaseDeleted,
+            cast_to=GPULeaseDeleted,
         )
 
 
-class AsyncGpuLeasesResource(AsyncAPIResource):
+class AsyncGPULeasesResource(AsyncAPIResource):
     @cached_property
-    def with_raw_response(self) -> AsyncGpuLeasesResourceWithRawResponse:
-        return AsyncGpuLeasesResourceWithRawResponse(self)
+    def with_raw_response(self) -> AsyncGPULeasesResourceWithRawResponse:
+        return AsyncGPULeasesResourceWithRawResponse(self)
 
     @cached_property
-    def with_streaming_response(self) -> AsyncGpuLeasesResourceWithStreamingResponse:
-        return AsyncGpuLeasesResourceWithStreamingResponse(self)
+    def with_streaming_response(self) -> AsyncGPULeasesResourceWithStreamingResponse:
+        return AsyncGPULeasesResourceWithStreamingResponse(self)
 
     async def create(
         self,
         *,
         gpu_group_id: str,
         lease_forever: bool | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> GpuLeaseCreated:
+    ) -> GPULeaseCreated:
         """
         Create GPU lease
 
         Args:
           gpu_group_id: GpuGroupID is used to specify the GPU to lease. As such, the lease does not
               specify which specific GPU to lease, but rather the type of GPU to lease.
 
@@ -291,33 +291,33 @@
         return await self._post(
             "/v2/gpuLeases",
             body=await async_maybe_transform(
                 {
                     "gpu_group_id": gpu_group_id,
                     "lease_forever": lease_forever,
                 },
-                gpu_lease_create_params.GpuLeaseCreateParams,
+                gpu_lease_create_params.GPULeaseCreateParams,
             ),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=GpuLeaseCreated,
+            cast_to=GPULeaseCreated,
         )
 
     async def retrieve(
         self,
         gpu_lease_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> GpuLeaseRead:
+    ) -> GPULeaseRead:
         """
         Get GPU lease
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -329,29 +329,29 @@
         if not gpu_lease_id:
             raise ValueError(f"Expected a non-empty value for `gpu_lease_id` but received {gpu_lease_id!r}")
         return await self._get(
             f"/v2/gpuLeases/{gpu_lease_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=GpuLeaseRead,
+            cast_to=GPULeaseRead,
         )
 
     async def update(
         self,
         gpu_lease_id: str,
         *,
         vm_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> GpuLeaseUpdated:
+    ) -> GPULeaseUpdated:
         """
         Update GPU lease
 
         Args:
           vm_id: VmID is used to specify the VM to attach the lease to.
 
               - If specified, the lease will be attached to the VM.
@@ -371,19 +371,19 @@
 
           timeout: Override the client-level default timeout for this request, in seconds
         """
         if not gpu_lease_id:
             raise ValueError(f"Expected a non-empty value for `gpu_lease_id` but received {gpu_lease_id!r}")
         return await self._post(
             f"/v2/gpuLeases/{gpu_lease_id}",
-            body=await async_maybe_transform({"vm_id": vm_id}, gpu_lease_update_params.GpuLeaseUpdateParams),
+            body=await async_maybe_transform({"vm_id": vm_id}, gpu_lease_update_params.GPULeaseUpdateParams),
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=GpuLeaseUpdated,
+            cast_to=GPULeaseUpdated,
         )
 
     async def list(
         self,
         *,
         all: bool | NotGiven = NOT_GIVEN,
         page: int | NotGiven = NOT_GIVEN,
@@ -391,15 +391,15 @@
         vm_id: str | NotGiven = NOT_GIVEN,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> GpuLeaseListResponse:
+    ) -> GPULeaseListResponse:
         """
         List GPU leases
 
         Args:
           all: List all
 
           page: Page number
@@ -426,31 +426,31 @@
                 query=await async_maybe_transform(
                     {
                         "all": all,
                         "page": page,
                         "page_size": page_size,
                         "vm_id": vm_id,
                     },
-                    gpu_lease_list_params.GpuLeaseListParams,
+                    gpu_lease_list_params.GPULeaseListParams,
                 ),
             ),
-            cast_to=GpuLeaseListResponse,
+            cast_to=GPULeaseListResponse,
         )
 
     async def delete(
         self,
         gpu_lease_id: str,
         *,
         # Use the following arguments if you need to pass additional parameters to the API that aren't available via kwargs.
         # The extra values given here take precedence over values defined on the client or passed to this method.
         extra_headers: Headers | None = None,
         extra_query: Query | None = None,
         extra_body: Body | None = None,
         timeout: float | httpx.Timeout | None | NotGiven = NOT_GIVEN,
-    ) -> GpuLeaseDeleted:
+    ) -> GPULeaseDeleted:
         """
         Delete GPU lease
 
         Args:
           extra_headers: Send extra headers
 
           extra_query: Add additional query parameters to the request
@@ -462,20 +462,20 @@
         if not gpu_lease_id:
             raise ValueError(f"Expected a non-empty value for `gpu_lease_id` but received {gpu_lease_id!r}")
         return await self._delete(
             f"/v2/gpuLeases/{gpu_lease_id}",
             options=make_request_options(
                 extra_headers=extra_headers, extra_query=extra_query, extra_body=extra_body, timeout=timeout
             ),
-            cast_to=GpuLeaseDeleted,
+            cast_to=GPULeaseDeleted,
         )
 
 
-class GpuLeasesResourceWithRawResponse:
-    def __init__(self, gpu_leases: GpuLeasesResource) -> None:
+class GPULeasesResourceWithRawResponse:
+    def __init__(self, gpu_leases: GPULeasesResource) -> None:
         self._gpu_leases = gpu_leases
 
         self.create = to_raw_response_wrapper(
             gpu_leases.create,
         )
         self.retrieve = to_raw_response_wrapper(
             gpu_leases.retrieve,
@@ -487,16 +487,16 @@
             gpu_leases.list,
         )
         self.delete = to_raw_response_wrapper(
             gpu_leases.delete,
         )
 
 
-class AsyncGpuLeasesResourceWithRawResponse:
-    def __init__(self, gpu_leases: AsyncGpuLeasesResource) -> None:
+class AsyncGPULeasesResourceWithRawResponse:
+    def __init__(self, gpu_leases: AsyncGPULeasesResource) -> None:
         self._gpu_leases = gpu_leases
 
         self.create = async_to_raw_response_wrapper(
             gpu_leases.create,
         )
         self.retrieve = async_to_raw_response_wrapper(
             gpu_leases.retrieve,
@@ -508,16 +508,16 @@
             gpu_leases.list,
         )
         self.delete = async_to_raw_response_wrapper(
             gpu_leases.delete,
         )
 
 
-class GpuLeasesResourceWithStreamingResponse:
-    def __init__(self, gpu_leases: GpuLeasesResource) -> None:
+class GPULeasesResourceWithStreamingResponse:
+    def __init__(self, gpu_leases: GPULeasesResource) -> None:
         self._gpu_leases = gpu_leases
 
         self.create = to_streamed_response_wrapper(
             gpu_leases.create,
         )
         self.retrieve = to_streamed_response_wrapper(
             gpu_leases.retrieve,
@@ -529,16 +529,16 @@
             gpu_leases.list,
         )
         self.delete = to_streamed_response_wrapper(
             gpu_leases.delete,
         )
 
 
-class AsyncGpuLeasesResourceWithStreamingResponse:
-    def __init__(self, gpu_leases: AsyncGpuLeasesResource) -> None:
+class AsyncGPULeasesResourceWithStreamingResponse:
+    def __init__(self, gpu_leases: AsyncGPULeasesResource) -> None:
         self._gpu_leases = gpu_leases
 
         self.create = async_to_streamed_response_wrapper(
             gpu_leases.create,
         )
         self.retrieve = async_to_streamed_response_wrapper(
             gpu_leases.retrieve,
```

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/resources/snapshots.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/snapshots.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/resources/vm_actions.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/vm_actions.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/resources/vms/__init__.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/vms/__init__.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/resources/vms/snapshot.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/vms/snapshot.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/resources/vms/vms.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/resources/vms/vms.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/__init__.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # File generated from our OpenAPI spec by Stainless. See CONTRIBUTING.md for details.
 
 from __future__ import annotations
 
 from .shared import VmSnapshotRead as VmSnapshotRead
 from .vm_read import VmRead as VmRead
-from .gpu_group import GpuGroup as GpuGroup
+from .gpu_group import GPUGroup as GPUGroup
 from .vm_created import VmCreated as VmCreated
 from .vm_deleted import VmDeleted as VmDeleted
 from .vm_updated import VmUpdated as VmUpdated
-from .gpu_lease_read import GpuLeaseRead as GpuLeaseRead
+from .gpu_lease_read import GPULeaseRead as GPULeaseRead
 from .vm_list_params import VmListParams as VmListParams
 from .vm_create_params import VmCreateParams as VmCreateParams
 from .vm_list_response import VmListResponse as VmListResponse
 from .vm_update_params import VmUpdateParams as VmUpdateParams
-from .gpu_lease_created import GpuLeaseCreated as GpuLeaseCreated
-from .gpu_lease_deleted import GpuLeaseDeleted as GpuLeaseDeleted
-from .gpu_lease_updated import GpuLeaseUpdated as GpuLeaseUpdated
+from .gpu_lease_created import GPULeaseCreated as GPULeaseCreated
+from .gpu_lease_deleted import GPULeaseDeleted as GPULeaseDeleted
+from .gpu_lease_updated import GPULeaseUpdated as GPULeaseUpdated
 from .vm_action_created import VmActionCreated as VmActionCreated
 from .vm_snapshot_created import VmSnapshotCreated as VmSnapshotCreated
 from .snapshot_list_params import SnapshotListParams as SnapshotListParams
-from .gpu_group_list_params import GpuGroupListParams as GpuGroupListParams
-from .gpu_lease_list_params import GpuLeaseListParams as GpuLeaseListParams
+from .gpu_group_list_params import GPUGroupListParams as GPUGroupListParams
+from .gpu_lease_list_params import GPULeaseListParams as GPULeaseListParams
 from .snapshot_list_response import SnapshotListResponse as SnapshotListResponse
-from .gpu_group_list_response import GpuGroupListResponse as GpuGroupListResponse
-from .gpu_lease_create_params import GpuLeaseCreateParams as GpuLeaseCreateParams
-from .gpu_lease_list_response import GpuLeaseListResponse as GpuLeaseListResponse
-from .gpu_lease_update_params import GpuLeaseUpdateParams as GpuLeaseUpdateParams
+from .gpu_group_list_response import GPUGroupListResponse as GPUGroupListResponse
+from .gpu_lease_create_params import GPULeaseCreateParams as GPULeaseCreateParams
+from .gpu_lease_list_response import GPULeaseListResponse as GPULeaseListResponse
+from .gpu_lease_update_params import GPULeaseUpdateParams as GPULeaseUpdateParams
 from .vm_action_create_params import VmActionCreateParams as VmActionCreateParams
```

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/gpu_group.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from typing import Optional
 
 from pydantic import Field as FieldInfo
 
 from .._models import BaseModel
 
-__all__ = ["GpuGroup"]
+__all__ = ["GPUGroup"]
 
 
-class GpuGroup(BaseModel):
+class GPUGroup(BaseModel):
     id: Optional[str] = None
 
     available: Optional[int] = None
 
     display_name: Optional[str] = FieldInfo(alias="displayName", default=None)
 
     name: Optional[str] = None
```

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_create_params.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_create_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from __future__ import annotations
 
 from typing_extensions import Required, Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
-__all__ = ["GpuLeaseCreateParams"]
+__all__ = ["GPULeaseCreateParams"]
 
 
-class GpuLeaseCreateParams(TypedDict, total=False):
+class GPULeaseCreateParams(TypedDict, total=False):
     gpu_group_id: Required[Annotated[str, PropertyInfo(alias="gpuGroupId")]]
     """
     GpuGroupID is used to specify the GPU to lease. As such, the lease does not
     specify which specific GPU to lease, but rather the type of GPU to lease.
     """
 
     lease_forever: Annotated[bool, PropertyInfo(alias="leaseForever")]
```

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_list_params.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_list_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from __future__ import annotations
 
 from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
-__all__ = ["GpuLeaseListParams"]
+__all__ = ["GPULeaseListParams"]
 
 
-class GpuLeaseListParams(TypedDict, total=False):
+class GPULeaseListParams(TypedDict, total=False):
     all: bool
     """List all"""
 
     page: int
     """Page number"""
 
     page_size: Annotated[int, PropertyInfo(alias="pageSize")]
```

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_read.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from typing import Optional
 
 from pydantic import Field as FieldInfo
 
 from .._models import BaseModel
 
-__all__ = ["GpuLeaseRead"]
+__all__ = ["GPULeaseRead"]
 
 
-class GpuLeaseRead(BaseModel):
+class GPULeaseRead(BaseModel):
     id: Optional[str] = None
 
     activated_at: Optional[str] = FieldInfo(alias="activatedAt", default=None)
     """ActivatedAt specifies the time when the lease was activated.
 
     This is the time the user first attached the GPU or 1 day after the lease was
     created if the user did not attach the GPU.
```

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/gpu_lease_update_params.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/gpu_lease_update_params.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from __future__ import annotations
 
 from typing_extensions import Annotated, TypedDict
 
 from .._utils import PropertyInfo
 
-__all__ = ["GpuLeaseUpdateParams"]
+__all__ = ["GPULeaseUpdateParams"]
 
 
-class GpuLeaseUpdateParams(TypedDict, total=False):
+class GPULeaseUpdateParams(TypedDict, total=False):
     vm_id: Annotated[str, PropertyInfo(alias="vmId")]
     """VmID is used to specify the VM to attach the lease to.
 
     - If specified, the lease will be attached to the VM.
 
     - If the lease is already attached to a VM, it will be detached from the current
       VM and attached to the new VM.
```

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/vm_create_params.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_create_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/vm_list_params.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_list_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/vm_read.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from typing import List, Optional
 
 from pydantic import Field as FieldInfo
 
 from .._models import BaseModel
 
-__all__ = ["VmRead", "Gpu", "Port", "PortHTTPProxy", "PortHTTPProxyCustomDomain", "Specs"]
+__all__ = ["VmRead", "GPU", "Port", "PortHTTPProxy", "PortHTTPProxyCustomDomain", "Specs"]
 
 
-class Gpu(BaseModel):
+class GPU(BaseModel):
     id: Optional[str] = None
 
     activated_at: Optional[str] = FieldInfo(alias="activatedAt", default=None)
     """ActivatedAt specifies the time when the lease was activated.
 
     This is the time the user first attached the GPU or 1 day after the lease was
     created if the user did not attach the GPU.
@@ -80,15 +80,15 @@
 
 
 class VmRead(BaseModel):
     id: Optional[str] = None
 
     created_at: Optional[str] = FieldInfo(alias="createdAt", default=None)
 
-    gpu: Optional[Gpu] = None
+    gpu: Optional[GPU] = None
 
     host: Optional[str] = None
 
     internal_name: Optional[str] = FieldInfo(alias="internalName", default=None)
 
     name: Optional[str] = None
```

### Comparing `kthcloud-0.3.0a0/src/kthcloud_go_deploy_v2/types/vm_update_params.py` & `kthcloud-0.4.0a0/src/kthcloud_go_deploy_v_/types/vm_update_params.py`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/LICENSE` & `kthcloud-0.4.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `kthcloud-0.3.0a0/pyproject.toml` & `kthcloud-0.4.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "kthcloud"
-version = "0.3.0-alpha"
+version = "0.4.0-alpha"
 description = "The official Python library for the kthcloud-go-deploy-v2 API"
 dynamic = ["readme"]
 license = "Apache-2.0"
 authors = [
 { name = "Kthcloud Go Deploy V2", email = "dev@cloud.cbh.kth.se" },
 ]
 dependencies = [
@@ -80,28 +80,28 @@
 "fix:ruff" = "ruff --fix ."
 
 typecheck = { chain = [
   "typecheck:pyright",
   "typecheck:mypy"
 ]}
 "typecheck:pyright" = "pyright"
-"typecheck:verify-types" = "pyright --verifytypes kthcloud_go_deploy_v2 --ignoreexternal"
+"typecheck:verify-types" = "pyright --verifytypes kthcloud_go_deploy_v_ --ignoreexternal"
 "typecheck:mypy" = "mypy ."
 
 [build-system]
 requires = ["hatchling", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 include = [
   "src/*"
 ]
 
 [tool.hatch.build.targets.wheel]
-packages = ["src/kthcloud_go_deploy_v2"]
+packages = ["src/kthcloud_go_deploy_v_"]
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.md"
 
@@ -183,14 +183,14 @@
 "functools.lru_cache".msg = "This function does not retain type information for the wrapped function's arguments; The `lru_cache` function from `_utils` should be used instead"
 
 [tool.ruff.lint.isort]
 length-sort = true
 length-sort-straight = true
 combine-as-imports = true
 extra-standard-library = ["typing_extensions"]
-known-first-party = ["kthcloud_go_deploy_v2", "tests"]
+known-first-party = ["kthcloud_go_deploy_v_", "tests"]
 
 [tool.ruff.per-file-ignores]
 "bin/**.py" = ["T201", "T203"]
 "scripts/**.py" = ["T201", "T203"]
 "tests/**.py" = ["T201", "T203"]
 "examples/**.py" = ["T201", "T203"]
```

### Comparing `kthcloud-0.3.0a0/PKG-INFO` & `kthcloud-0.4.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kthcloud
-Version: 0.3.0a0
+Version: 0.4.0a0
 Summary: The official Python library for the kthcloud-go-deploy-v2 API
 Project-URL: Homepage, https://github.com/kthcloud/python-sdk
 Project-URL: Repository, https://github.com/kthcloud/python-sdk
 Author-email: Kthcloud Go Deploy V2 <dev@cloud.cbh.kth.se>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
@@ -54,15 +54,15 @@
 ```
 
 ## Usage
 
 The full API of this library can be found in [api.md](https://github.com/kthcloud/python-sdk/tree/main/api.md).
 
 ```python
-from kthcloud_go_deploy_v2 import KthcloudGoDeployV2
+from kthcloud_go_deploy_v_ import KthcloudGoDeployV2
 
 client = KthcloudGoDeployV2()
 
 vm_created = client.vms.create(
     cpu_cores=1,
     disk_size=10,
     name="xxx",
@@ -79,15 +79,15 @@
 
 ## Async usage
 
 Simply import `AsyncKthcloudGoDeployV2` instead of `KthcloudGoDeployV2` and use `await` with each API call:
 
 ```python
 import asyncio
-from kthcloud_go_deploy_v2 import AsyncKthcloudGoDeployV2
+from kthcloud_go_deploy_v_ import AsyncKthcloudGoDeployV2
 
 client = AsyncKthcloudGoDeployV2()
 
 
 async def main() -> None:
     vm_created = await client.vms.create(
         cpu_cores=1,
@@ -111,41 +111,41 @@
 - Serializing back into JSON, `model.to_json()`
 - Converting to a dictionary, `model.to_dict()`
 
 Typed requests and responses provide autocomplete and documentation within your editor. If you would like to see type errors in VS Code to help catch bugs earlier, set `python.analysis.typeCheckingMode` to `basic`.
 
 ## Handling errors
 
-When the library is unable to connect to the API (for example, due to network connection problems or a timeout), a subclass of `kthcloud_go_deploy_v2.APIConnectionError` is raised.
+When the library is unable to connect to the API (for example, due to network connection problems or a timeout), a subclass of `kthcloud_go_deploy_v_.APIConnectionError` is raised.
 
 When the API returns a non-success status code (that is, 4xx or 5xx
-response), a subclass of `kthcloud_go_deploy_v2.APIStatusError` is raised, containing `status_code` and `response` properties.
+response), a subclass of `kthcloud_go_deploy_v_.APIStatusError` is raised, containing `status_code` and `response` properties.
 
-All errors inherit from `kthcloud_go_deploy_v2.APIError`.
+All errors inherit from `kthcloud_go_deploy_v_.APIError`.
 
 ```python
-import kthcloud_go_deploy_v2
-from kthcloud_go_deploy_v2 import KthcloudGoDeployV2
+import kthcloud_go_deploy_v_
+from kthcloud_go_deploy_v_ import KthcloudGoDeployV2
 
 client = KthcloudGoDeployV2()
 
 try:
     client.vms.create(
         cpu_cores=1,
         disk_size=10,
         name="xxx",
         ram=1,
         ssh_public_key="string",
     )
-except kthcloud_go_deploy_v2.APIConnectionError as e:
+except kthcloud_go_deploy_v_.APIConnectionError as e:
     print("The server could not be reached")
     print(e.__cause__)  # an underlying Exception, likely raised within httpx.
-except kthcloud_go_deploy_v2.RateLimitError as e:
+except kthcloud_go_deploy_v_.RateLimitError as e:
     print("A 429 status code was received; we should back off a bit.")
-except kthcloud_go_deploy_v2.APIStatusError as e:
+except kthcloud_go_deploy_v_.APIStatusError as e:
     print("Another non-200-range status code was received")
     print(e.status_code)
     print(e.response)
 ```
 
 Error codes are as followed:
 
@@ -165,15 +165,15 @@
 Certain errors are automatically retried 2 times by default, with a short exponential backoff.
 Connection errors (for example, due to a network connectivity problem), 408 Request Timeout, 409 Conflict,
 429 Rate Limit, and >=500 Internal errors are all retried by default.
 
 You can use the `max_retries` option to configure or disable retry settings:
 
 ```python
-from kthcloud_go_deploy_v2 import KthcloudGoDeployV2
+from kthcloud_go_deploy_v_ import KthcloudGoDeployV2
 
 # Configure the default for all requests:
 client = KthcloudGoDeployV2(
     # default is 2
     max_retries=0,
 )
 
@@ -189,15 +189,15 @@
 
 ### Timeouts
 
 By default requests time out after 1 minute. You can configure this with a `timeout` option,
 which accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration) object:
 
 ```python
-from kthcloud_go_deploy_v2 import KthcloudGoDeployV2
+from kthcloud_go_deploy_v_ import KthcloudGoDeployV2
 
 # Configure the default for all requests:
 client = KthcloudGoDeployV2(
     # 20 seconds (default is 1 minute)
     timeout=20.0,
 )
 
@@ -245,15 +245,15 @@
 ```
 
 ### Accessing raw response data (e.g. headers)
 
 The "raw" Response object can be accessed by prefixing `.with_raw_response.` to any HTTP method call, e.g.,
 
 ```py
-from kthcloud_go_deploy_v2 import KthcloudGoDeployV2
+from kthcloud_go_deploy_v_ import KthcloudGoDeployV2
 
 client = KthcloudGoDeployV2()
 response = client.vms.with_raw_response.create(
     cpu_cores=1,
     disk_size=10,
     name="xxx",
     ram=1,
@@ -261,17 +261,17 @@
 )
 print(response.headers.get('X-My-Header'))
 
 vm = response.parse()  # get the object that `vms.create()` would have returned
 print(vm.id)
 ```
 
-These methods return an [`APIResponse`](https://github.com/kthcloud/python-sdk/tree/main/src/kthcloud_go_deploy_v2/_response.py) object.
+These methods return an [`APIResponse`](https://github.com/kthcloud/python-sdk/tree/main/src/kthcloud_go_deploy_v_/_response.py) object.
 
-The async client returns an [`AsyncAPIResponse`](https://github.com/kthcloud/python-sdk/tree/main/src/kthcloud_go_deploy_v2/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
+The async client returns an [`AsyncAPIResponse`](https://github.com/kthcloud/python-sdk/tree/main/src/kthcloud_go_deploy_v_/_response.py) with the same structure, the only difference being `await`able methods for reading the response content.
 
 #### `.with_streaming_response`
 
 The above interface eagerly reads the full response body when you make the request, which may not always be what you want.
 
 To stream the response body, use `.with_streaming_response` instead, which requires a context manager and only reads the response body once you call `.read()`, `.text()`, `.json()`, `.iter_bytes()`, `.iter_text()`, `.iter_lines()` or `.parse()`. In the async client, these are async methods.
 
@@ -331,15 +331,15 @@
 You can directly override the [httpx client](https://www.python-httpx.org/api/#client) to customize it for your use case, including:
 
 - Support for proxies
 - Custom transports
 - Additional [advanced](https://www.python-httpx.org/advanced/#client-instances) functionality
 
 ```python
-from kthcloud_go_deploy_v2 import KthcloudGoDeployV2, DefaultHttpxClient
+from kthcloud_go_deploy_v_ import KthcloudGoDeployV2, DefaultHttpxClient
 
 client = KthcloudGoDeployV2(
     # Or use the `KTHCLOUD_GO_DEPLOY_V2_BASE_URL` env var
     base_url="http://my.test.server.example.com:8083",
     http_client=DefaultHttpxClient(
         proxies="http://my.test.proxy.example.com",
         transport=httpx.HTTPTransport(local_address="0.0.0.0"),
```

