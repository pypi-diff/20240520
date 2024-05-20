# Comparing `tmp/pulumiverse_exoscale-0.58.0.tar.gz` & `tmp/pulumiverse_exoscale-0.59.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_exoscale-0.58.0.tar", last modified: Sat May 11 23:09:10 2024, max compression
+gzip compressed data, was "pulumiverse_exoscale-0.59.0.tar", last modified: Mon May 20 11:43:11 2024, max compression
```

## Comparing `pulumiverse_exoscale-0.58.0.tar` & `pulumiverse_exoscale-0.59.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:09:10.432044 pulumiverse_exoscale-0.58.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-11 23:09:10.432044 pulumiverse_exoscale-0.58.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:09:10.432044 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    96537 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/affinity.py
--rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/anti_affinity_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    19241 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/block_storage_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    16739 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/block_storage_volume_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    59185 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    56907 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/compute_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:09:10.432044 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    44469 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    19830 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/domain_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    21132 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/elastic_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_affinity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_anti_affinity_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_block_storage_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_block_storage_volume_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute.py
--rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    20432 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute_instance_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_database_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_elastic_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_iam_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_iam_org_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_iam_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_iamapi_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    13769 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_instance_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_instance_pool_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_nlb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_nlb_service_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_private_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    21258 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_sks_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    19568 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_sks_cluster_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    21178 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_sks_nodepool.py
--rw-r--r--   0 runner    (1001) docker     (127)    19983 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_sks_nodepool_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)    16908 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iam_access_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iam_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iam_org_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    16323 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iam_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    10433 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iamapi_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    53589 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/instance_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    37861 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (127)    21070 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/nic.py
--rw-r--r--   0 runner    (1001) docker     (127)    16556 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/nlb.py
--rw-r--r--   0 runner    (1001) docker     (127)    26653 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/nlb_service.py
--rw-r--r--   0 runner    (1001) docker     (127)   149339 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19953 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/private_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/secondary_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (127)    11860 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    40734 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/security_group_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    14555 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/security_group_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    45580 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/sks_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    19086 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/sks_kubeconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)    47916 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/sks_nodepool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/ssh_keypair.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 23:09:10.432044 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/pulumiverse_exoscale.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 23:09:10.432044 pulumiverse_exoscale-0.58.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-11 23:09:10.000000 pulumiverse_exoscale-0.58.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:43:11.493063 pulumiverse_exoscale-0.59.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-20 11:43:11.493063 pulumiverse_exoscale-0.59.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:43:11.489063 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96537 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10715 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/affinity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8982 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/anti_affinity_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19185 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/block_storage_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16473 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/block_storage_volume_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59185 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56907 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/compute_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:43:11.493063 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44469 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19830 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21132 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/elastic_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_affinity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_anti_affinity_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_block_storage_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_block_storage_volume_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_compute.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_compute_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20432 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_compute_instance_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5442 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_compute_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_compute_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_database_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3224 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_elastic_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_iam_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_iam_org_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6023 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_iam_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_iamapi_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13769 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_instance_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_instance_pool_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5665 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6282 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_nlb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5824 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_nlb_service_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7815 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_private_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21258 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_sks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19568 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_sks_cluster_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21178 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_sks_nodepool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19983 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_sks_nodepool_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16908 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/iam_access_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/iam_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/iam_org_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16323 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/iam_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10433 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/iamapi_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53589 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/instance_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37861 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21070 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12211 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/nic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16556 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/nlb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26653 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/nlb_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)   149339 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19953 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/private_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/secondary_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11860 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40734 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/security_group_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14555 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/security_group_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45580 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/sks_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19086 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/sks_kubeconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47916 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/sks_nodepool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10691 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/ssh_keypair.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:43:11.493063 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/pulumiverse_exoscale.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 11:43:11.493063 pulumiverse_exoscale-0.59.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-20 11:43:11.000000 pulumiverse_exoscale-0.59.0/setup.py
```

### Comparing `pulumiverse_exoscale-0.58.0/PKG-INFO` & `pulumiverse_exoscale-0.59.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_exoscale
-Version: 0.58.0
+Version: 0.59.0
 Summary: A Pulumi package for creating and managing exoscale cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-exoscale
 Keywords: pulumi exoscale category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_exoscale-0.58.0/README.md` & `pulumiverse_exoscale-0.59.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/__init__.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/_inputs.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/_utilities.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/affinity.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/affinity.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/anti_affinity_group.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/anti_affinity_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/block_storage_volume.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/block_storage_volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
                  name: Optional[pulumi.Input[str]] = None,
                  size: Optional[pulumi.Input[int]] = None,
                  snapshot_target: Optional[pulumi.Input['BlockStorageVolumeSnapshotTargetArgs']] = None,
                  timeouts: Optional[pulumi.Input['BlockStorageVolumeTimeoutsArgs']] = None):
         """
         The set of arguments for constructing a BlockStorageVolume resource.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: ❗ Resource labels.
-        :param pulumi.Input[str] name: ❗ Volume name.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: Resource labels.
+        :param pulumi.Input[str] name: Volume name.
         :param pulumi.Input[int] size: Volume size in GB (default 10). If volume is attached, instance must be stopped to update this value. Volume can only grow, cannot be shrunk.
         :param pulumi.Input['BlockStorageVolumeSnapshotTargetArgs'] snapshot_target: Block storage snapshot to use when creating a volume. Read-only after creation.
         """
         pulumi.set(__self__, "zone", zone)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if name is not None:
@@ -54,27 +54,27 @@
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        ❗ Resource labels.
+        Resource labels.
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        ❗ Volume name.
+        Volume name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -124,16 +124,16 @@
                  state: Optional[pulumi.Input[str]] = None,
                  timeouts: Optional[pulumi.Input['BlockStorageVolumeTimeoutsArgs']] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering BlockStorageVolume resources.
         :param pulumi.Input[int] blocksize: Volume block size.
         :param pulumi.Input[str] created_at: Volume creation date.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: ❗ Resource labels.
-        :param pulumi.Input[str] name: ❗ Volume name.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: Resource labels.
+        :param pulumi.Input[str] name: Volume name.
         :param pulumi.Input[int] size: Volume size in GB (default 10). If volume is attached, instance must be stopped to update this value. Volume can only grow, cannot be shrunk.
         :param pulumi.Input['BlockStorageVolumeSnapshotTargetArgs'] snapshot_target: Block storage snapshot to use when creating a volume. Read-only after creation.
         :param pulumi.Input[str] state: Volume state.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if blocksize is not None:
             pulumi.set(__self__, "blocksize", blocksize)
@@ -178,27 +178,27 @@
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        ❗ Resource labels.
+        Resource labels.
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        ❗ Volume name.
+        Volume name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -275,16 +275,16 @@
         """
         Manage [Exoscale Block Storage](https://community.exoscale.com/documentation/block-storage/) Volume.
 
         Block Storage offers persistent externally attached volumes for your workloads.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: ❗ Resource labels.
-        :param pulumi.Input[str] name: ❗ Volume name.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: Resource labels.
+        :param pulumi.Input[str] name: Volume name.
         :param pulumi.Input[int] size: Volume size in GB (default 10). If volume is attached, instance must be stopped to update this value. Volume can only grow, cannot be shrunk.
         :param pulumi.Input[pulumi.InputType['BlockStorageVolumeSnapshotTargetArgs']] snapshot_target: Block storage snapshot to use when creating a volume. Read-only after creation.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
@@ -361,16 +361,16 @@
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[int] blocksize: Volume block size.
         :param pulumi.Input[str] created_at: Volume creation date.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: ❗ Resource labels.
-        :param pulumi.Input[str] name: ❗ Volume name.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: Resource labels.
+        :param pulumi.Input[str] name: Volume name.
         :param pulumi.Input[int] size: Volume size in GB (default 10). If volume is attached, instance must be stopped to update this value. Volume can only grow, cannot be shrunk.
         :param pulumi.Input[pulumi.InputType['BlockStorageVolumeSnapshotTargetArgs']] snapshot_target: Block storage snapshot to use when creating a volume. Read-only after creation.
         :param pulumi.Input[str] state: Volume state.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -403,23 +403,23 @@
         """
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter
     def labels(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        ❗ Resource labels.
+        Resource labels.
         """
         return pulumi.get(self, "labels")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        ❗ Volume name.
+        Volume name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def size(self) -> pulumi.Output[Optional[int]]:
         """
```

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/block_storage_volume_snapshot.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/block_storage_volume_snapshot.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,16 @@
                  labels: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  timeouts: Optional[pulumi.Input['BlockStorageVolumeSnapshotTimeoutsArgs']] = None):
         """
         The set of arguments for constructing a BlockStorageVolumeSnapshot resource.
         :param pulumi.Input['BlockStorageVolumeSnapshotVolumeArgs'] volume: Volume from which to create a snapshot.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: ❗ Resource labels. Not updateble after creation.
-        :param pulumi.Input[str] name: ❗ Volume snapshot name.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: Resource labels.
+        :param pulumi.Input[str] name: Volume snapshot name.
         """
         pulumi.set(__self__, "volume", volume)
         pulumi.set(__self__, "zone", zone)
         if labels is not None:
             pulumi.set(__self__, "labels", labels)
         if name is not None:
             pulumi.set(__self__, "name", name)
@@ -61,27 +61,27 @@
     def zone(self, value: pulumi.Input[str]):
         pulumi.set(self, "zone", value)
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        ❗ Resource labels. Not updateble after creation.
+        Resource labels.
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        ❗ Volume snapshot name.
+        Volume snapshot name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -105,16 +105,16 @@
                  state: Optional[pulumi.Input[str]] = None,
                  timeouts: Optional[pulumi.Input['BlockStorageVolumeSnapshotTimeoutsArgs']] = None,
                  volume: Optional[pulumi.Input['BlockStorageVolumeSnapshotVolumeArgs']] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering BlockStorageVolumeSnapshot resources.
         :param pulumi.Input[str] created_at: Snapshot creation date.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: ❗ Resource labels. Not updateble after creation.
-        :param pulumi.Input[str] name: ❗ Volume snapshot name.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: Resource labels.
+        :param pulumi.Input[str] name: Volume snapshot name.
         :param pulumi.Input[int] size: Snapshot size in GB.
         :param pulumi.Input[str] state: Snapshot state.
         :param pulumi.Input['BlockStorageVolumeSnapshotVolumeArgs'] volume: Volume from which to create a snapshot.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         if created_at is not None:
             pulumi.set(__self__, "created_at", created_at)
@@ -145,27 +145,27 @@
     def created_at(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "created_at", value)
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        ❗ Resource labels. Not updateble after creation.
+        Resource labels.
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        ❗ Volume snapshot name.
+        Volume snapshot name.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -241,16 +241,16 @@
         """
         Manage [Exoscale Block Storage](https://community.exoscale.com/documentation/block-storage/) Volume Snapshot.
 
         Block Storage offers persistent externally attached volumes for your workloads.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: ❗ Resource labels. Not updateble after creation.
-        :param pulumi.Input[str] name: ❗ Volume snapshot name.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: Resource labels.
+        :param pulumi.Input[str] name: Volume snapshot name.
         :param pulumi.Input[pulumi.InputType['BlockStorageVolumeSnapshotVolumeArgs']] volume: Volume from which to create a snapshot.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -324,16 +324,16 @@
         Get an existing BlockStorageVolumeSnapshot resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] created_at: Snapshot creation date.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: ❗ Resource labels. Not updateble after creation.
-        :param pulumi.Input[str] name: ❗ Volume snapshot name.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] labels: Resource labels.
+        :param pulumi.Input[str] name: Volume snapshot name.
         :param pulumi.Input[int] size: Snapshot size in GB.
         :param pulumi.Input[str] state: Snapshot state.
         :param pulumi.Input[pulumi.InputType['BlockStorageVolumeSnapshotVolumeArgs']] volume: Volume from which to create a snapshot.
         :param pulumi.Input[str] zone: ❗ The Exoscale [Zone](https://www.exoscale.com/datacenters/) name.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -357,23 +357,23 @@
         """
         return pulumi.get(self, "created_at")
 
     @property
     @pulumi.getter
     def labels(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        ❗ Resource labels. Not updateble after creation.
+        Resource labels.
         """
         return pulumi.get(self, "labels")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        ❗ Volume snapshot name.
+        Volume snapshot name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def size(self) -> pulumi.Output[int]:
         """
```

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/compute.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/compute.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/compute_instance.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/compute_instance.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/config/vars.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/database.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/database.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/domain.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/domain.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/domain_record.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/elastic_ip.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/elastic_ip.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_affinity.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_affinity.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_anti_affinity_group.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_anti_affinity_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_block_storage_volume.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_block_storage_volume.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_block_storage_volume_snapshot.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_block_storage_volume_snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_compute.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute_instance.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_compute_instance.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute_instance_list.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_compute_instance_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute_ip_address.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_compute_ip_address.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_compute_template.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_compute_template.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_database_uri.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_database_uri.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_domain.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_domain.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_domain_record.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_elastic_ip.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_elastic_ip.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_iam_api_key.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_iam_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_iam_org_policy.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_iam_org_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_iam_role.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_iam_role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_iamapi_key.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_iamapi_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_instance_pool.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_instance_pool.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_instance_pool_list.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_instance_pool_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_network.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_nlb.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_nlb.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_nlb_service_list.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_nlb_service_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_private_network.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_private_network.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_security_group.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_sks_cluster.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_sks_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_sks_cluster_list.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_sks_cluster_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_sks_nodepool.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_sks_nodepool.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_sks_nodepool_list.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_sks_nodepool_list.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_template.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_template.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/get_zones.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/get_zones.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iam_access_key.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/iam_access_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iam_api_key.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/iam_api_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iam_org_policy.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/iam_org_policy.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iam_role.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/iam_role.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/iamapi_key.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/iamapi_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/instance_pool.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/instance_pool.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/ip_address.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/ip_address.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/network.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/network.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/nic.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/nic.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/nlb.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/nlb.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/nlb_service.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/nlb_service.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/outputs.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/private_network.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/private_network.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/provider.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/secondary_ip_address.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/secondary_ip_address.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/security_group.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/security_group.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/security_group_rule.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/security_group_rule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/security_group_rules.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/security_group_rules.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/sks_cluster.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/sks_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/sks_kubeconfig.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/sks_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/sks_nodepool.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/sks_nodepool.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/ssh_key.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale/ssh_keypair.py` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale/ssh_keypair.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale.egg-info/PKG-INFO` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-exoscale
-Version: 0.58.0
+Version: 0.59.0
 Summary: A Pulumi package for creating and managing exoscale cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-exoscale
 Keywords: pulumi exoscale category/cloud
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_exoscale-0.58.0/pulumiverse_exoscale.egg-info/SOURCES.txt` & `pulumiverse_exoscale-0.59.0/pulumiverse_exoscale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_exoscale-0.58.0/setup.py` & `pulumiverse_exoscale-0.59.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.58.0"
+VERSION = "0.59.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "exoscale Pulumi Package - Development Version"
```

