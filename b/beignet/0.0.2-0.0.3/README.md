# Comparing `tmp/beignet-0.0.2.tar.gz` & `tmp/beignet-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beignet-0.0.2.tar", last modified: Wed Apr  3 15:47:41 2024, max compression
+gzip compressed data, was "beignet-0.0.3.tar", last modified: Mon May 20 13:40:10 2024, max compression
```

## Comparing `beignet-0.0.2.tar` & `beignet-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:47:41.221034 beignet-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:47:41.217034 beignet-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:47:41.217034 beignet-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-03 15:47:37.000000 beignet-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 15:47:37.000000 beignet-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-03 15:47:37.000000 beignet-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-03 15:47:41.221034 beignet-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 15:47:37.000000 beignet-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-03 15:47:37.000000 beignet-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:47:41.221034 beignet-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:47:41.217034 beignet-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:47:41.217034 beignet-0.0.2/src/beignet/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:47:37.000000 beignet-0.0.2/src/beignet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:47:41.221034 beignet-0.0.2/src/beignet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-03 15:47:41.000000 beignet-0.0.2/src/beignet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-03 15:47:41.000000 beignet-0.0.2/src/beignet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:47:41.000000 beignet-0.0.2/src/beignet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 15:47:41.000000 beignet-0.0.2/src/beignet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:10.556160 beignet-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:10.528160 beignet-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:10.532160 beignet-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 2024-05-20 13:40:05.000000 beignet-0.0.3/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-20 13:40:05.000000 beignet-0.0.3/.github/workflows/push_main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-20 13:40:05.000000 beignet-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-20 13:40:05.000000 beignet-0.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-20 13:40:05.000000 beignet-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-20 13:40:10.556160 beignet-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-20 13:40:05.000000 beignet-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:10.532160 beignet-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-20 13:40:05.000000 beignet-0.0.3/docs/beignet.datasets.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 13:40:05.000000 beignet-0.0.3/docs/beignet.features.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 13:40:05.000000 beignet-0.0.3/docs/beignet.io.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 13:40:05.000000 beignet-0.0.3/docs/beignet.transforms.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-20 13:40:05.000000 beignet-0.0.3/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:10.532160 beignet-0.0.3/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-20 13:40:05.000000 beignet-0.0.3/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-20 13:40:05.000000 beignet-0.0.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-20 13:40:05.000000 beignet-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:40:10.556160 beignet-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:10.528160 beignet-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:10.540160 beignet-0.0.3/src/beignet/
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_apply_euler_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_apply_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_apply_rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_apply_rotation_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_compose_euler_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_compose_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_compose_rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_compose_rotation_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_euler_angle_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_euler_angle_magnitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_euler_angle_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_euler_angle_to_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_euler_angle_to_rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_euler_angle_to_rotation_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_invert_euler_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_invert_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_invert_rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_invert_rotation_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_quaternion_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_quaternion_magnitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_quaternion_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_quaternion_slerp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_quaternion_to_euler_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_quaternion_to_rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_quaternion_to_rotation_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_random_euler_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_random_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_random_rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_random_rotation_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_rotation_matrix_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_rotation_matrix_magnitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_rotation_matrix_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_rotation_matrix_to_euler_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_rotation_matrix_to_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_rotation_matrix_to_rotation_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_rotation_vector_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_rotation_vector_magnitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_rotation_vector_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_rotation_vector_to_euler_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_rotation_vector_to_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_rotation_vector_to_rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/_translation_identity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:10.544160 beignet-0.0.3/src/beignet/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/datasets/__uni_ref_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/datasets/_fasta_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/datasets/_sequence_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/datasets/_sized_sequence_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/datasets/_uniref100_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/datasets/_uniref50_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/datasets/_uniref90_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:10.544160 beignet-0.0.3/src/beignet/features/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/features/_feature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:10.544160 beignet-0.0.3/src/beignet/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/io/_thread_safe_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:10.544160 beignet-0.0.3/src/beignet/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/transforms/_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-20 13:40:05.000000 beignet-0.0.3/src/beignet/transforms/_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:10.552160 beignet-0.0.3/src/beignet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-20 13:40:10.000000 beignet-0.0.3/src/beignet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4825 2024-05-20 13:40:10.000000 beignet-0.0.3/src/beignet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:40:10.000000 beignet-0.0.3/src/beignet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-20 13:40:10.000000 beignet-0.0.3/src/beignet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 13:40:10.000000 beignet-0.0.3/src/beignet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:10.532160 beignet-0.0.3/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:10.552160 beignet-0.0.3/tests/beignet/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:10.552160 beignet-0.0.3/tests/beignet/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/datasets/test__uniref_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:10.552160 beignet-0.0.3/tests/beignet/features/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/features/test__feature.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:10.552160 beignet-0.0.3/tests/beignet/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/io/test__thread_safe_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__apply_euler_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__apply_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__apply_rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__apply_rotation_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__compose_euler_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__compose_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__compose_rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__compose_rotation_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__euler_angle_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__euler_angle_magnitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__euler_angle_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__euler_angle_to_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__euler_angle_to_rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__euler_angle_to_rotation_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__invert_euler_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__invert_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__invert_rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__invert_rotation_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__quaternion_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__quaternion_magnitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__quaternion_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__quaternion_to_euler_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__quaternion_to_rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__quaternion_to_rotation_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__random_euler_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__random_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__random_rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__random_rotation_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__rotation_matrix_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__rotation_matrix_magnitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__rotation_matrix_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__rotation_matrix_to_euler_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__rotation_matrix_to_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__rotation_matrix_to_rotation_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__rotation_vector_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__rotation_vector_magnitude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__rotation_vector_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__rotation_vector_to_euler_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__rotation_vector_to_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__rotation_vector_to_rotation_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/test__slerp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:40:10.552160 beignet-0.0.3/tests/beignet/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-20 13:40:05.000000 beignet-0.0.3/tests/beignet/transforms/test__transform.py
```

### Comparing `beignet-0.0.2/.github/workflows/publish.yml` & `beignet-0.0.3/.github/workflows/push.yml`

 * *Files 6% similar despite different names*

```diff
@@ -10,32 +10,36 @@
           python-version: "3.x"
       - run: "python -m pip install --upgrade build"
       - run: "python -m build ."
       - uses: "actions/upload-artifact@v3"
         with:
           name: "python-package-distributions"
           path: "dist/"
-  test:
-    environment:
-      name: "test.pypi.org"
-      url: "https://test.pypi.org/project/beignet"
-    needs:
-      - "build"
-    permissions:
-      id-token: "write"
-    runs-on: "ubuntu-latest"
+  pytest:
+    strategy:
+      matrix:
+        platform:
+          - "macos-latest"
+          - "ubuntu-latest"
+          - "windows-latest"
+        python:
+          - "3.10"
+          - "3.11"
+    runs-on: ${{ matrix.platform }}
     steps:
-      - uses: "actions/download-artifact@v3"
+      - uses: "actions/checkout@v4"
+      - uses: "actions/setup-python@v5"
         with:
-          name: "python-package-distributions"
-          path: "dist/"
-      - uses: "pypa/gh-action-pypi-publish@release/v1"
-        with:
-          repository-url: "https://test.pypi.org/legacy/"
-  publish:
+          python-version: ${{ matrix.python }}
+      - run: "python -m pip install --editable '.[all]'"
+      - run: "python -m pytest"
+      - env:
+          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
+        uses: "codecov/codecov-action@v3"
+  pypi:
     environment:
       name: "pypi.org"
       url: "https://pypi.org/project/beignet"
     if: "startsWith(github.ref, 'refs/tags/')"
     needs:
       - "build"
     permissions:
@@ -45,15 +49,15 @@
       - uses: "actions/download-artifact@v3"
         with:
           name: "python-package-distributions"
           path: "dist/"
       - uses: "pypa/gh-action-pypi-publish@release/v1"
   release:
     needs:
-      - "publish"
+      - "pypi"
     permissions:
       contents: "write"
       id-token: "write"
     runs-on: "ubuntu-latest"
     steps:
       - uses: "actions/download-artifact@v3"
         with:
@@ -64,8 +68,33 @@
           inputs: "./dist/*.tar.gz ./dist/*.whl"
       - env:
           GITHUB_TOKEN: "${{ github.token }}"
         run: "gh release create '${{ github.ref_name }}' --notes '' --repo '${{ github.repository }}'"
       - env:
           GITHUB_TOKEN: "${{ github.token }}"
         run: "gh release upload '${{ github.ref_name }}' dist/** --repo '${{ github.repository }}'"
+  ruff:
+    runs-on: "ubuntu-latest"
+    steps:
+      - uses: "actions/checkout@v4"
+      - uses: "chartboost/ruff-action@v1"
+        with:
+          args: "format --check"
+  testpypi:
+    environment:
+      name: "test.pypi.org"
+      url: "https://test.pypi.org/project/beignet"
+    needs:
+      - "build"
+    permissions:
+      id-token: "write"
+    runs-on: "ubuntu-latest"
+    steps:
+      - uses: "actions/download-artifact@v3"
+        with:
+          name: "python-package-distributions"
+          path: "dist/"
+      - uses: "pypa/gh-action-pypi-publish@release/v1"
+        with:
+          repository-url: "https://test.pypi.org/legacy/"
+          skip-existing: true
 on: "push"
```

### Comparing `beignet-0.0.2/LICENSE` & `beignet-0.0.3/LICENSE`

 * *Files identical despite different names*

