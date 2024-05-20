# Comparing `tmp/koku-nise-4.5.0.tar.gz` & `tmp/koku-nise-4.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koku-nise-4.5.0.tar", last modified: Fri May 17 17:09:29 2024, max compression
+gzip compressed data, was "koku-nise-4.5.1.tar", last modified: Mon May 20 19:31:59 2024, max compression
```

## Comparing `koku-nise-4.5.0.tar` & `koku-nise-4.5.1.tar`

### file list

```diff
@@ -1,111 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.068084 koku-nise-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-05-17 17:09:13.000000 koku-nise-4.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-17 17:09:13.000000 koku-nise-4.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-17 17:09:29.068084 koku-nise-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-05-17 17:09:13.000000 koku-nise-4.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.056084 koku-nise-4.5.0/koku_nise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-17 17:09:28.000000 koku-nise-4.5.0/koku_nise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-17 17:09:28.000000 koku-nise-4.5.0/koku_nise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 17:09:28.000000 koku-nise-4.5.0/koku_nise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-17 17:09:28.000000 koku-nise-4.5.0/koku_nise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 17:09:28.000000 koku-nise-4.5.0/koku_nise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-17 17:09:28.000000 koku-nise-4.5.0/koku_nise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-17 17:09:28.000000 koku-nise-4.5.0/koku_nise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.060084 koku-nise-4.5.0/nise/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28971 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/aws-template-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.060084 koku-nise-4.5.0/nise/generators/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.060084 koku-nise-4.5.0/nise/generators/aws/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/aws_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13560 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/aws_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/data_transfer_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/ebs_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/ec2_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/marketplace_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/rds_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/route53_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/s3_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/aws/vpc_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.064084 koku-nise-4.5.0/nise/generators/azure/
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16807 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/azure/azure_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/azure/bandwidth_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/azure/ccsp_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/azure/data_transfer_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/azure/sql_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/azure/storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/azure/virtual_machine_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/azure/virtual_network_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.064084 koku-nise-4.5.0/nise/generators/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/gcp/cloud_storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/gcp/compute_engine_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/gcp/gcp_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/gcp/gcp_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/gcp/gcp_network_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/gcp/hcs_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/gcp/project_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.064084 koku-nise-4.5.0/nise/generators/oci/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/oci/oci_block_storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/oci/oci_compute_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/oci/oci_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/oci/oci_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/oci/oci_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/oci/oci_network_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.064084 koku-nise-4.5.0/nise/generators/ocp/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/ocp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43084 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/generators/ocp/ocp_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    56209 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.064084 koku-nise-4.5.0/nise/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/util/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.064084 koku-nise-4.5.0/nise/yaml_generators/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.064084 koku-nise-4.5.0/nise/yaml_generators/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    71376 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/aws/ec2_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/aws/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/aws/rds_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/aws/regions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.068084 koku-nise-4.5.0/nise/yaml_generators/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/azure/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.068084 koku-nise-4.5.0/nise/yaml_generators/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/gcp/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.068084 koku-nise-4.5.0/nise/yaml_generators/oci/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/oci/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/oci/oci_yaml_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.068084 koku-nise-4.5.0/nise/yaml_generators/ocp/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/ocp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/ocp/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.068084 koku-nise-4.5.0/nise/yaml_generators/ocp_on_cloud/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/ocp_on_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/ocp_on_cloud/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 17:09:29.068084 koku-nise-4.5.0/nise/yaml_generators/static/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/aws_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/aws_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/azure_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/azure_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/gcp_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/gcp_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/oci_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/oci_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/ocp_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/ocp_on_cloud_options.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/static/ocp_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-17 17:09:13.000000 koku-nise-4.5.0/nise/yaml_generators/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 17:09:29.068084 koku-nise-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-17 17:09:13.000000 koku-nise-4.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:59.765807 koku-nise-4.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    34520 2024-05-20 19:31:44.000000 koku-nise-4.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-20 19:31:44.000000 koku-nise-4.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-20 19:31:59.765807 koku-nise-4.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9834 2024-05-20 19:31:44.000000 koku-nise-4.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:59.753807 koku-nise-4.5.1/koku_nise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-20 19:31:59.000000 koku-nise-4.5.1/koku_nise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3416 2024-05-20 19:31:59.000000 koku-nise-4.5.1/koku_nise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:31:59.000000 koku-nise-4.5.1/koku_nise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 19:31:59.000000 koku-nise-4.5.1/koku_nise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:31:59.000000 koku-nise-4.5.1/koku_nise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-20 19:31:59.000000 koku-nise-4.5.1/koku_nise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 19:31:59.000000 koku-nise-4.5.1/koku_nise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:59.757807 koku-nise-4.5.1/nise/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28971 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/aws-template-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5677 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:59.757807 koku-nise-4.5.1/nise/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:59.757807 koku-nise-4.5.1/nise/generators/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/aws/aws_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13560 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/aws/aws_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/aws/data_transfer_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/aws/ebs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7163 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/aws/ec2_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/aws/marketplace_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6495 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/aws/rds_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/aws/route53_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4009 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/aws/s3_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/aws/vpc_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:59.757807 koku-nise-4.5.1/nise/generators/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17226 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/azure/azure_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/azure/bandwidth_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/azure/ccsp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/azure/data_transfer_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/azure/managed_disk_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/azure/sql_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/azure/storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/azure/virtual_machine_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/azure/virtual_network_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:59.761807 koku-nise-4.5.1/nise/generators/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/gcp/cloud_storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9603 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/gcp/compute_engine_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/gcp/gcp_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11867 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/gcp/gcp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/gcp/gcp_network_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/gcp/hcs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/gcp/project_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:59.761807 koku-nise-4.5.1/nise/generators/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/oci/oci_block_storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/oci/oci_compute_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/oci/oci_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/oci/oci_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10817 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/oci/oci_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/oci/oci_network_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:59.761807 koku-nise-4.5.1/nise/generators/ocp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/ocp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43084 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/generators/ocp/ocp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56331 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:59.761807 koku-nise-4.5.1/nise/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/util/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:59.761807 koku-nise-4.5.1/nise/yaml_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:59.761807 koku-nise-4.5.1/nise/yaml_generators/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71376 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/aws/ec2_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/aws/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13953 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/aws/rds_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/aws/regions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:59.765807 koku-nise-4.5.1/nise/yaml_generators/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/azure/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:59.765807 koku-nise-4.5.1/nise/yaml_generators/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/gcp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:59.765807 koku-nise-4.5.1/nise/yaml_generators/oci/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/oci/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/oci/oci_yaml_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:59.765807 koku-nise-4.5.1/nise/yaml_generators/ocp/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/ocp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/ocp/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:59.765807 koku-nise-4.5.1/nise/yaml_generators/ocp_on_cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/ocp_on_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/ocp_on_cloud/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:31:59.765807 koku-nise-4.5.1/nise/yaml_generators/static/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/static/aws_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3423 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/static/aws_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/static/azure_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/static/azure_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/static/gcp_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/static/gcp_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/static/oci_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/static/oci_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/static/ocp_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/static/ocp_on_cloud_options.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/static/ocp_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-05-20 19:31:44.000000 koku-nise-4.5.1/nise/yaml_generators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:31:59.765807 koku-nise-4.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-05-20 19:31:44.000000 koku-nise-4.5.1/setup.py
```

### Comparing `koku-nise-4.5.0/LICENSE` & `koku-nise-4.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/README.md` & `koku-nise-4.5.1/README.md`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/koku_nise.egg-info/SOURCES.txt` & `koku-nise-4.5.1/koku_nise.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 nise/generators/aws/s3_generator.py
 nise/generators/aws/vpc_generator.py
 nise/generators/azure/__init__.py
 nise/generators/azure/azure_generator.py
 nise/generators/azure/bandwidth_generator.py
 nise/generators/azure/ccsp_generator.py
 nise/generators/azure/data_transfer_generator.py
+nise/generators/azure/managed_disk_generator.py
 nise/generators/azure/sql_database_generator.py
 nise/generators/azure/storage_generator.py
 nise/generators/azure/virtual_machine_generator.py
 nise/generators/azure/virtual_network_generator.py
 nise/generators/gcp/__init__.py
 nise/generators/gcp/cloud_storage_generator.py
 nise/generators/gcp/compute_engine_generator.py
```

### Comparing `koku-nise-4.5.0/nise/__main__.py` & `koku-nise-4.5.1/nise/__main__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/aws-template-manifest.json` & `koku-nise-4.5.1/nise/aws-template-manifest.json`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/copy.py` & `koku-nise-4.5.1/nise/copy.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/extract.py` & `koku-nise-4.5.1/nise/extract.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/aws/__init__.py` & `koku-nise-4.5.1/nise/generators/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/aws/aws_constants.py` & `koku-nise-4.5.1/nise/generators/aws/aws_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/aws/aws_generator.py` & `koku-nise-4.5.1/nise/generators/aws/aws_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/aws/data_transfer_generator.py` & `koku-nise-4.5.1/nise/generators/aws/data_transfer_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/aws/ebs_generator.py` & `koku-nise-4.5.1/nise/generators/aws/ebs_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/aws/ec2_generator.py` & `koku-nise-4.5.1/nise/generators/aws/ec2_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/aws/marketplace_generator.py` & `koku-nise-4.5.1/nise/generators/aws/marketplace_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/aws/rds_generator.py` & `koku-nise-4.5.1/nise/generators/aws/rds_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/aws/route53_generator.py` & `koku-nise-4.5.1/nise/generators/aws/route53_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/aws/s3_generator.py` & `koku-nise-4.5.1/nise/generators/aws/s3_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/aws/vpc_generator.py` & `koku-nise-4.5.1/nise/generators/aws/vpc_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/azure/__init__.py` & `koku-nise-4.5.1/nise/generators/azure/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,11 +17,12 @@
 """Module for azure data generators."""
 from nise.generators.azure.azure_generator import AZURE_COLUMNS  # noqa: F401
 from nise.generators.azure.azure_generator import AZURE_COLUMNS_V2  # noqa: F401
 from nise.generators.azure.azure_generator import AzureGenerator  # noqa: F401
 from nise.generators.azure.bandwidth_generator import BandwidthGenerator  # noqa: F401
 from nise.generators.azure.ccsp_generator import CCSPGenerator  # noqa: F401
 from nise.generators.azure.data_transfer_generator import DTGenerator  # noqa: F401
+from nise.generators.azure.managed_disk_generator import ManagedDiskGenerator  # noqa: F401
 from nise.generators.azure.sql_database_generator import SQLGenerator  # noqa: F401
 from nise.generators.azure.storage_generator import StorageGenerator  # noqa: F401
 from nise.generators.azure.virtual_machine_generator import VMGenerator  # noqa: F401
 from nise.generators.azure.virtual_network_generator import VNGenerator  # noqa: F401
```

### Comparing `koku-nise-4.5.0/nise/generators/azure/azure_generator.py` & `koku-nise-4.5.1/nise/generators/azure/azure_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 """Defines the abstract generator."""
 import calendar
 import datetime
 import json
+import uuid
 from random import choice
 from random import randint
 from random import uniform
 
 from nise.generators.generator import AbstractGenerator
 
 AZURE_COLUMNS = (
@@ -161,14 +162,27 @@
     )
 
     SERVICE_NAMES = ["SQL Database", "Storage", "Virtual Machines", "Virtual Network"]
     SERVICE_FAMILIES = ("Compute", "Storage", "Networking")
 
     INVOICE_SECTION_NAMES = ("IT Services",)
 
+    @property
+    def meter_id(self):
+        if self._meter_id is None:
+            self._meter_id = uuid.uuid4()
+        return self._meter_id
+
+    @property
+    def meter_name(self):
+        if self._meter_name is None:
+            _, _, meter_name, _ = self._get_cached_meter_values(self.meter_id, self.SERVICE_METER)
+            self._meter_name = meter_name
+        return self._meter_name
+
     def __init__(self, start_date, end_date, currency, account_info, attributes=None):  # noqa: C901
         """Initialize the generator."""
         self.azure_columns = AZURE_COLUMNS
         self.subscription_guid = account_info.get("subscription_guid")
         self.account_info = account_info
         self.usage_accounts = account_info.get("usage_accounts")
         self.attributes = attributes
@@ -351,16 +365,16 @@
             additional_info = ""
         if not service_info_2:
             service_info_2 = ""
 
         row["ResourceGroup"] = resource_group
         row["ResourceLocation"] = azure_region
         row["MeterCategory"] = self._service_name
-        row["MeterId"] = str(meter_id)
-        row["MeterName"] = meter_name
+        row["MeterId"] = str(self.meter_id)
+        row["MeterName"] = self.meter_name
         row["MeterRegion"] = meter_region
         row["ConsumedService"] = self._consumed
         row["OfferId"] = ""
         row["AdditionalInfo"] = json.dumps(additional_info)
         row["ServiceInfo1"] = ""
         row["ServiceInfo2"] = service_info_2
         row["UnitOfMeasure"] = units_of_measure
```

### Comparing `koku-nise-4.5.0/nise/generators/azure/bandwidth_generator.py` & `koku-nise-4.5.1/nise/generators/azure/bandwidth_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/azure/ccsp_generator.py` & `koku-nise-4.5.1/nise/generators/azure/ccsp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/azure/data_transfer_generator.py` & `koku-nise-4.5.1/nise/generators/azure/data_transfer_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/azure/sql_database_generator.py` & `koku-nise-4.5.1/nise/generators/azure/sql_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/azure/storage_generator.py` & `koku-nise-4.5.1/nise/generators/azure/storage_generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,17 +37,15 @@
         ("Storage - Bandwidth", "Bandwidth", "Geo-Replication v2 Data transfer", "100 GB"),
         ("Tables", "Tables", "GRS Batch Write Operations", "100000000"),
         ("Tables", "Tables", "Batch Write Operations", "100000000"),
         ("Tables", "Tables", "Write Operations", ""),
         ("Tables", "Tables", "Read Operations", "1000000"),
         ("Tables", "Tables", "LRS Data Stored", "100 GB/Month"),
         ("Tables", "Tables", "RA-GRS Data Stored", "100 GB/Month"),
-        ("Standard SSD Managed Disks", "Standard SSD Managed Disks", "E4 Disks", "1 /Month"),
         ("Standard SSD Managed Disks", "Standard SSD Managed Disks", "Disk Operations", "100000000"),
-        ("Premium SSD Managed Disks", "Premium SSD Managed Disks", "P10 Disks", ""),
         ("Premium SSD Managed Disks", "Premium SSD Managed Disks", "Disk Operations", ""),
         ("Standard Page Blob", "Standard Page Blob", "Disk Read Operations", "100000000"),
         ("Standard Page Blob", "Standard Page Blob", "Disk Write Operations", "100000000"),
         ("Standard Page Blob", "Standard Page Blob", "LRS Data Stored", "100 GB/Month"),
     )
     SERVICE_INFO_2 = [None]
     EXAMPLE_RESOURCE = (
```

### Comparing `koku-nise-4.5.0/nise/generators/azure/virtual_machine_generator.py` & `koku-nise-4.5.1/nise/generators/azure/virtual_machine_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/azure/virtual_network_generator.py` & `koku-nise-4.5.1/nise/generators/azure/virtual_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/gcp/__init__.py` & `koku-nise-4.5.1/nise/generators/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/gcp/cloud_storage_generator.py` & `koku-nise-4.5.1/nise/generators/gcp/cloud_storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/gcp/compute_engine_generator.py` & `koku-nise-4.5.1/nise/generators/gcp/compute_engine_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/gcp/gcp_database_generator.py` & `koku-nise-4.5.1/nise/generators/gcp/gcp_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/gcp/gcp_generator.py` & `koku-nise-4.5.1/nise/generators/gcp/gcp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/gcp/gcp_network_generator.py` & `koku-nise-4.5.1/nise/generators/gcp/gcp_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/gcp/hcs_generator.py` & `koku-nise-4.5.1/nise/generators/gcp/hcs_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/gcp/project_generator.py` & `koku-nise-4.5.1/nise/generators/gcp/project_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/generator.py` & `koku-nise-4.5.1/nise/generators/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/oci/__init__.py` & `koku-nise-4.5.1/nise/generators/oci/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/oci/oci_block_storage_generator.py` & `koku-nise-4.5.1/nise/generators/oci/oci_block_storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/oci/oci_compute_generator.py` & `koku-nise-4.5.1/nise/generators/oci/oci_compute_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/oci/oci_constants.py` & `koku-nise-4.5.1/nise/generators/oci/oci_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/oci/oci_database_generator.py` & `koku-nise-4.5.1/nise/generators/oci/oci_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/oci/oci_generator.py` & `koku-nise-4.5.1/nise/generators/oci/oci_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/oci/oci_network_generator.py` & `koku-nise-4.5.1/nise/generators/oci/oci_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/ocp/__init__.py` & `koku-nise-4.5.1/nise/generators/ocp/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/generators/ocp/ocp_generator.py` & `koku-nise-4.5.1/nise/generators/ocp/ocp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/manifest.py` & `koku-nise-4.5.1/nise/manifest.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/report.py` & `koku-nise-4.5.1/nise/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 from nise.generators.aws import RDSGenerator
 from nise.generators.aws import Route53Generator
 from nise.generators.aws import S3Generator
 from nise.generators.aws import VPCGenerator
 from nise.generators.azure import BandwidthGenerator
 from nise.generators.azure import CCSPGenerator
 from nise.generators.azure import DTGenerator
+from nise.generators.azure import ManagedDiskGenerator
 from nise.generators.azure import SQLGenerator
 from nise.generators.azure import StorageGenerator
 from nise.generators.azure import VMGenerator
 from nise.generators.azure import VNGenerator
 from nise.generators.gcp import CloudStorageGenerator
 from nise.generators.gcp import ComputeEngineGenerator
 from nise.generators.gcp import GCP_REPORT_COLUMNS
@@ -747,14 +748,15 @@
             {"generator": BandwidthGenerator, "attributes": {}},
             {"generator": CCSPGenerator, "attributes": {}},
             {"generator": SQLGenerator, "attributes": {}},
             {"generator": StorageGenerator, "attributes": {}},
             {"generator": VMGenerator, "attributes": {}},
             {"generator": VNGenerator, "attributes": {}},
             {"generator": DTGenerator, "attributes": {}},
+            {"generator": ManagedDiskGenerator, "attributes": {}},
         ]
         accounts_list = None
 
     months = _create_month_list(start_date, end_date)
 
     account_info = _generate_azure_account_info(accounts_list)
     currency = default_currency(options.get("currency"), account_info["currency_code"])
```

### Comparing `koku-nise-4.5.0/nise/upload.py` & `koku-nise-4.5.1/nise/upload.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/util/__init__.py` & `koku-nise-4.5.1/nise/util/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/util/log.py` & `koku-nise-4.5.1/nise/util/log.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_gen.py` & `koku-nise-4.5.1/nise/yaml_gen.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/aws/ec2_instance_types.py` & `koku-nise-4.5.1/nise/yaml_generators/aws/ec2_instance_types.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/aws/generator.py` & `koku-nise-4.5.1/nise/yaml_generators/aws/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/aws/rds_instance_types.py` & `koku-nise-4.5.1/nise/yaml_generators/aws/rds_instance_types.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/aws/regions.py` & `koku-nise-4.5.1/nise/yaml_generators/aws/regions.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/azure/generator.py` & `koku-nise-4.5.1/nise/yaml_generators/azure/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/gcp/generator.py` & `koku-nise-4.5.1/nise/yaml_generators/gcp/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/generator.py` & `koku-nise-4.5.1/nise/yaml_generators/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/oci/generator.py` & `koku-nise-4.5.1/nise/yaml_generators/oci/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/oci/oci_yaml_constants.py` & `koku-nise-4.5.1/nise/yaml_generators/oci/oci_yaml_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/ocp/generator.py` & `koku-nise-4.5.1/nise/yaml_generators/ocp/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/ocp_on_cloud/generator.py` & `koku-nise-4.5.1/nise/yaml_generators/ocp_on_cloud/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/static/aws_generator_config.yml` & `koku-nise-4.5.1/nise/yaml_generators/static/aws_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/static/aws_static_data.yml.j2` & `koku-nise-4.5.1/nise/yaml_generators/static/aws_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/static/azure_generator_config.yml` & `koku-nise-4.5.1/nise/yaml_generators/static/azure_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/static/azure_static_data.yml.j2` & `koku-nise-4.5.1/nise/yaml_generators/static/azure_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/static/gcp_static_data.yml.j2` & `koku-nise-4.5.1/nise/yaml_generators/static/gcp_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/static/oci_static_data.yml.j2` & `koku-nise-4.5.1/nise/yaml_generators/static/oci_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/static/ocp_generator_config.yml` & `koku-nise-4.5.1/nise/yaml_generators/static/ocp_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/static/ocp_on_cloud_options.yml` & `koku-nise-4.5.1/nise/yaml_generators/static/ocp_on_cloud_options.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/static/ocp_static_data.yml.j2` & `koku-nise-4.5.1/nise/yaml_generators/static/ocp_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/nise/yaml_generators/utils.py` & `koku-nise-4.5.1/nise/yaml_generators/utils.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.5.0/setup.py` & `koku-nise-4.5.1/setup.py`

 * *Files identical despite different names*

