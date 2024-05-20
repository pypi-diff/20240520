# Comparing `tmp/dcnum-0.18.0.tar.gz` & `tmp/dcnum-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcnum-0.18.0.tar", last modified: Wed May 15 14:44:20 2024, max compression
+gzip compressed data, was "dcnum-0.19.0.tar", last modified: Mon May 20 21:37:00 2024, max compression
```

## Comparing `dcnum-0.18.0.tar` & `dcnum-0.19.0.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.486162 dcnum-0.18.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.470162 dcnum-0.18.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.470162 dcnum-0.18.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-15 14:44:16.000000 dcnum-0.18.0/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-15 14:44:16.000000 dcnum-0.18.0/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-15 14:44:16.000000 dcnum-0.18.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-15 14:44:16.000000 dcnum-0.18.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11722 2024-05-15 14:44:16.000000 dcnum-0.18.0/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-15 14:44:16.000000 dcnum-0.18.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-15 14:44:20.486162 dcnum-0.18.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-15 14:44:16.000000 dcnum-0.18.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.470162 dcnum-0.18.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-15 14:44:16.000000 dcnum-0.18.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.474162 dcnum-0.18.0/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-15 14:44:16.000000 dcnum-0.18.0/docs/extensions/github_changelog.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-15 14:44:16.000000 dcnum-0.18.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-15 14:44:16.000000 dcnum-0.18.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-15 14:44:16.000000 dcnum-0.18.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:44:20.486162 dcnum-0.18.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.470162 dcnum-0.18.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.474162 dcnum-0.18.0/src/dcnum/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-15 14:44:20.000000 dcnum-0.18.0/src/dcnum/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.474162 dcnum-0.18.0/src/dcnum/feat/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/event_extractor_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.474162 dcnum-0.18.0/src/dcnum/feat/feat_background/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_background/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_background/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_background/bg_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13064 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_background/bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (127)    20705 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_background/bg_sparse_median.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.474162 dcnum-0.18.0/src/dcnum/feat/feat_brightness/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_brightness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_brightness/bright_all.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_brightness/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.474162 dcnum-0.18.0/src/dcnum/feat/feat_contour/
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_contour/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_contour/contour.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_contour/moments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_contour/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.474162 dcnum-0.18.0/src/dcnum/feat/feat_texture/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_texture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_texture/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/feat_texture/tex_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/gate.py
--rw-r--r--   0 runner    (1001) docker     (127)    15644 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/feat/queue_event_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.478162 dcnum-0.18.0/src/dcnum/logic/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27998 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/logic/ctrl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/logic/job.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/logic/json_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.478162 dcnum-0.18.0/src/dcnum/meta/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/meta/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/meta/ppid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.478162 dcnum-0.18.0/src/dcnum/read/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/read/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/read/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/read/hdf5_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/read/mapped.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.478162 dcnum-0.18.0/src/dcnum/segm/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/segm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/segm/segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (127)    12220 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/segm/segmenter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/segm/segmenter_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/segm/segmenter_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/segm/segmenter_manager_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.478162 dcnum-0.18.0/src/dcnum/write/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/write/deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    11906 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/write/queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-05-15 14:44:16.000000 dcnum-0.18.0/src/dcnum/write/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.486162 dcnum-0.18.0/src/dcnum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-15 14:44:20.000000 dcnum-0.18.0/src/dcnum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-15 14:44:20.000000 dcnum-0.18.0/src/dcnum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:44:20.000000 dcnum-0.18.0/src/dcnum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-15 14:44:20.000000 dcnum-0.18.0/src/dcnum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 14:44:20.000000 dcnum-0.18.0/src/dcnum.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.486162 dcnum-0.18.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:44:20.486162 dcnum-0.18.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip
--rw-r--r--   0 runner    (1001) docker     (127)   650653 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
--rw-r--r--   0 runner    (1001) docker     (127)   284743 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip
--rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/data/fmt-hdf5_shapein_empty.zip
--rw-r--r--   0 runner    (1001) docker     (127)   275920 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_background_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_background_bg_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_background_bg_roll_median.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_background_bg_sparsemed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_brightness.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_event_extractor_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_haralick.py
--rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_moments_based.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_moments_based_extended.py
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_feat_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_logic_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_logic_join.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_logic_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    24892 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_logic_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_meta_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)     4267 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_meta_ppid_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_meta_ppid_bg.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_meta_ppid_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_meta_ppid_feat.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_meta_ppid_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_meta_ppid_segm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_read_basin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_read_concat_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)    11118 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_read_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_read_hdf5_index_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_segm_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_segm_no_mask_proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_segm_thresh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_write_deque_writer_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_write_queue_collector_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)    12120 2024-05-15 14:44:16.000000 dcnum-0.18.0/tests/test_write_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.787156 dcnum-0.19.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.763157 dcnum-0.19.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.767156 dcnum-0.19.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-20 21:36:56.000000 dcnum-0.19.0/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-20 21:36:56.000000 dcnum-0.19.0/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-20 21:36:56.000000 dcnum-0.19.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-20 21:36:56.000000 dcnum-0.19.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11899 2024-05-20 21:36:56.000000 dcnum-0.19.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-20 21:36:56.000000 dcnum-0.19.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-20 21:37:00.787156 dcnum-0.19.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-20 21:36:56.000000 dcnum-0.19.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.771156 dcnum-0.19.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-20 21:36:56.000000 dcnum-0.19.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.771156 dcnum-0.19.0/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-20 21:36:56.000000 dcnum-0.19.0/docs/extensions/github_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-20 21:36:56.000000 dcnum-0.19.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 21:36:56.000000 dcnum-0.19.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-20 21:36:56.000000 dcnum-0.19.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 21:37:00.787156 dcnum-0.19.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.767156 dcnum-0.19.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.771156 dcnum-0.19.0/src/dcnum/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-20 21:37:00.000000 dcnum-0.19.0/src/dcnum/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.771156 dcnum-0.19.0/src/dcnum/feat/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7129 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/event_extractor_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.771156 dcnum-0.19.0/src/dcnum/feat/feat_background/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/feat_background/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7985 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/feat_background/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/feat_background/bg_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13173 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/feat_background/bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20705 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/feat_background/bg_sparse_median.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.771156 dcnum-0.19.0/src/dcnum/feat/feat_brightness/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/feat_brightness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/feat_brightness/bright_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/feat_brightness/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.775157 dcnum-0.19.0/src/dcnum/feat/feat_contour/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/feat_contour/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/feat_contour/contour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/feat_contour/moments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6639 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/feat_contour/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.775157 dcnum-0.19.0/src/dcnum/feat/feat_texture/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/feat_texture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/feat_texture/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/feat_texture/tex_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15644 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/feat/queue_event_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.775157 dcnum-0.19.0/src/dcnum/logic/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/logic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27956 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/logic/ctrl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/logic/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/logic/json_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.775157 dcnum-0.19.0/src/dcnum/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/meta/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/meta/ppid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.775157 dcnum-0.19.0/src/dcnum/read/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/read/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/read/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22112 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/read/hdf5_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/read/mapped.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.779157 dcnum-0.19.0/src/dcnum/segm/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/segm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/segm/segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12220 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/segm/segmenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/segm/segmenter_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/segm/segmenter_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5710 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/segm/segmenter_manager_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.779157 dcnum-0.19.0/src/dcnum/write/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/write/deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11906 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/write/queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-05-20 21:36:56.000000 dcnum-0.19.0/src/dcnum/write/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.787156 dcnum-0.19.0/src/dcnum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-20 21:37:00.000000 dcnum-0.19.0/src/dcnum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-20 21:37:00.000000 dcnum-0.19.0/src/dcnum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:37:00.000000 dcnum-0.19.0/src/dcnum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-20 21:37:00.000000 dcnum-0.19.0/src/dcnum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 21:37:00.000000 dcnum-0.19.0/src/dcnum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.783156 dcnum-0.19.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:37:00.787156 dcnum-0.19.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   650653 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   284743 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/data/fmt-hdf5_shapein_empty.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   275920 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_feat_background_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_feat_background_bg_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_feat_background_bg_roll_median.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9670 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_feat_background_bg_sparsemed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_feat_brightness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_feat_event_extractor_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_feat_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_feat_haralick.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_feat_moments_based.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_feat_moments_based_extended.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_feat_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_logic_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_logic_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_logic_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33551 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_logic_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_meta_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_meta_ppid_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_meta_ppid_bg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_meta_ppid_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_meta_ppid_feat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_meta_ppid_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_meta_ppid_segm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_read_basin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_read_concat_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11130 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_read_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_read_hdf5_index_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14336 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_segm_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_segm_no_mask_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_segm_thresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_write_deque_writer_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6100 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_write_queue_collector_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12120 2024-05-20 21:36:56.000000 dcnum-0.19.0/tests/test_write_writer.py
```

### Comparing `dcnum-0.18.0/.github/workflows/check.yml` & `dcnum-0.19.0/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/.github/workflows/deploy_pypi.yml` & `dcnum-0.19.0/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/.gitignore` & `dcnum-0.19.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/CHANGELOG` & `dcnum-0.19.0/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+0.19.0
+ - enh: elevate `HDF5Data`s `index_mapping` to pipeline identifier status
+   (this changes the pipeline identifier)
+ - enh: improve sanity checks for `BackgroundRollMed`
 0.18.0
  - BREAKING CHANGE: mask postprocessing did a morphological opening instead
    of a morphological closing, failing to remove spurious noise
  - BREAKING CHANGE: perform first fill_holes and then closing_disk in mask
    postprocessing
  - feat: allow to specify ranges when creating an HDF5Data instance to
    enable e.g. processing only a portion of an input file
```

### Comparing `dcnum-0.18.0/LICENSE` & `dcnum-0.19.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/PKG-INFO` & `dcnum-0.19.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.18.0
+Version: 0.19.0
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Maximilian Schlögel, Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.18.0/README.rst` & `dcnum-0.19.0/README.rst`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/docs/conf.py` & `dcnum-0.19.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/docs/extensions/github_changelog.py` & `dcnum-0.19.0/docs/extensions/github_changelog.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/pyproject.toml` & `dcnum-0.19.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/feat/event_extractor_manager_thread.py` & `dcnum-0.19.0/src/dcnum/feat/event_extractor_manager_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/feat/feat_background/base.py` & `dcnum-0.19.0/src/dcnum/feat/feat_background/base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/feat/feat_background/bg_copy.py` & `dcnum-0.19.0/src/dcnum/feat/feat_background/bg_copy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/feat/feat_background/bg_roll_median.py` & `dcnum-0.19.0/src/dcnum/feat/feat_background/bg_roll_median.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,28 +115,29 @@
     @staticmethod
     def check_user_kwargs(*,
                           kernel_size: int = 100,
                           batch_size: int = 10000):
         """Check user-defined properties of this class
 
         This method primarily exists so that the CLI knows which
-        keyword arguements can be passed to this class.
+        keyword arguments can be passed to this class.
 
         Parameters
         ----------
         kernel_size: int
             Kernel size for median computation. This is the number of
             events that are used to compute the median for each pixel.
         batch_size: int
             Number of events to process at the same time. Increasing this
             number much more than two orders of magnitude larger than
             `kernel_size` will not increase computation speed. Larger
             values lead to a higher memory consumption.
         """
-        assert kernel_size > 0
+        assert kernel_size > 0, "kernel size must be positive number"
+        assert kernel_size % 2 == 0, "kernel size must be even number"
         assert batch_size > kernel_size
 
     def get_slices_for_batch(self, batch_index=0):
         """Returns slices for getting the input and writing to output
 
         The input slice is `self.kernel_size` longer.
         """
```

### Comparing `dcnum-0.18.0/src/dcnum/feat/feat_background/bg_sparse_median.py` & `dcnum-0.19.0/src/dcnum/feat/feat_background/bg_sparse_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/feat/feat_brightness/bright_all.py` & `dcnum-0.19.0/src/dcnum/feat/feat_brightness/bright_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/feat/feat_contour/moments.py` & `dcnum-0.19.0/src/dcnum/feat/feat_contour/moments.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/feat/feat_contour/volume.py` & `dcnum-0.19.0/src/dcnum/feat/feat_contour/volume.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/feat/feat_texture/tex_all.py` & `dcnum-0.19.0/src/dcnum/feat/feat_texture/tex_all.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/feat/gate.py` & `dcnum-0.19.0/src/dcnum/feat/gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/feat/queue_event_extractor.py` & `dcnum-0.19.0/src/dcnum/feat/queue_event_extractor.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/logic/ctrl.py` & `dcnum-0.19.0/src/dcnum/logic/ctrl.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import collections
 import datetime
-import hashlib
 import json
 import logging
 from logging.handlers import QueueListener
 import multiprocessing as mp
-import numbers
 import os
 import pathlib
 import platform
 import socket
 import threading
 import time
 import traceback
 import uuid
 
 import h5py
-import numpy as np
 
 from ..feat.feat_background.base import get_available_background_methods
 from ..feat.queue_event_extractor import QueueEventExtractor
 from ..feat import gate
 from ..feat import EventExtractorManagerThread
 from ..segm import SegmenterManagerThread, get_available_segmenters
 from ..meta import ppid
@@ -309,15 +306,25 @@
         dathash = self.draw.h5.attrs.get("pipeline:dcnum hash", "0")
         # The number of events extracted in a potential previous pipeline run.
         evyield = self.draw.h5.attrs.get("pipeline:dcnum yield", -1)
         redo_sanity = (
             # Whether pipeline hash is invalid.
             ppid.compute_pipeline_hash(**datdict) != dathash
             # Whether the input file is the original output of the pipeline.
-            or len(self.draw) != evyield)
+            or len(self.draw) != evyield
+            # If index mapping is defined, then we always redo the pipeline.
+            # If the pipeline hashes are identical and index mapping is not
+            # None, then both pipelines were done with index mapping.
+            # But applying the same pipeline with index mapping in series
+            # will lead to a different result in the second run (e.g. 1st
+            # pipeline run: take every 2nd event; 2nd pipeline run: take
+            # every second event -> results in every 4th event in output of
+            # second pipeline run).
+            or self.draw.index_mapping is not None
+        )
         # Do we have to recompute the background data? In addition to the
         # hash sanity check above, check the generation, input data,
         # and background pipeline identifiers.
         redo_bg = (
             (datdict["gen_id"] != self.ppdict["gen_id"])
             or (datdict["dat_id"] != self.ppdict["dat_id"])
             or (datdict["bg_id"] != self.ppdict["bg_id"]))
@@ -383,29 +390,15 @@
             hw.h5.attrs["pipeline:dcnum segmenter"] = self.ppdict["seg_id"]
             hw.h5.attrs["pipeline:dcnum feature"] = self.ppdict["feat_id"]
             hw.h5.attrs["pipeline:dcnum gate"] = self.ppdict["gate_id"]
             hw.h5.attrs["pipeline:dcnum hash"] = self.pphash
             hw.h5.attrs["pipeline:dcnum yield"] = self.event_count
             # index mapping information
             im = self.job.kwargs["data_kwargs"].get("index_mapping", None)
-            if im is None:
-                dim = "0"
-            elif isinstance(im, numbers.Number):
-                dim = f"{im}"
-            elif isinstance(im, slice):
-                dim = (f"{im.start if im.start is not None else 'n'}"
-                       + f"-{im.stop if im.stop is not None else 'n'}"
-                       + f"-{im.step if im.step is not None else 'n'}"
-                       )
-            elif isinstance(im, (list, np.ndarray)):
-                idhash = hashlib.md5(
-                    np.array(im, dtype=np.uint32).tobytes()).hexdigest()
-                dim = f"h-{idhash[:8]}"
-            else:
-                dim = "unknown"
+            dim = HDF5Data.get_ppid_index_mapping(im)
             hw.h5.attrs["pipeline:dcnum mapping"] = dim
             # regular metadata
             hw.h5.attrs["experiment:event count"] = self.event_count
             hw.h5.attrs["imaging:pixel size"] = self.draw.pixel_size
             # Add job information to resulting .rtdc file
             hw.store_log(f"dcnum-job-{time_string}",
                          json.dumps({
```

### Comparing `dcnum-0.18.0/src/dcnum/logic/job.py` & `dcnum-0.19.0/src/dcnum/logic/job.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/logic/json_encoder.py` & `dcnum-0.19.0/src/dcnum/logic/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/meta/paths.py` & `dcnum-0.19.0/src/dcnum/meta/paths.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/meta/ppid.py` & `dcnum-0.19.0/src/dcnum/meta/ppid.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/read/cache.py` & `dcnum-0.19.0/src/dcnum/read/cache.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/read/hdf5_data.py` & `dcnum-0.19.0/src/dcnum/read/hdf5_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
+import hashlib
 import io
 import json
+import numbers
 import pathlib
 import tempfile
 from typing import Dict, BinaryIO, List
 import uuid
 import warnings
 
 import h5py
@@ -289,42 +291,78 @@
             if bn is not None:
                 bn.close()
         self._image_cache.clear()
         self._basin_data.clear()
         self.h5.close()
 
     def get_ppid(self):
-        return self.get_ppid_from_ppkw({"pixel_size": self.pixel_size})
+        return self.get_ppid_from_ppkw(
+            {"pixel_size": self.pixel_size,
+             "index_mapping": self.index_mapping})
 
     @classmethod
     def get_ppid_code(cls):
         return "hdf"
 
     @classmethod
     def get_ppid_from_ppkw(cls, kwargs):
         # Data does not really fit into the PPID scheme we use for the rest
         # of the pipeline. This implementation here is custom.
         code = cls.get_ppid_code()
+        # pixel size
         ppid_ps = f"{kwargs['pixel_size']:.8f}".rstrip("0")
-        kwid = "^".join([f"p={ppid_ps}"])
+        # index mapping
+        ppid_im = cls.get_ppid_index_mapping(kwargs.get("index_mapping", None))
+        kwid = "^".join([f"p={ppid_ps}", f"i={ppid_im}"])
         return ":".join([code, kwid])
 
     @staticmethod
+    def get_ppid_index_mapping(index_mapping):
+        """Return the pipeline identifier part for index mapping"""
+        im = index_mapping
+        if im is None:
+            dim = "0"
+        elif isinstance(im, numbers.Integral):
+            dim = f"{im}"
+        elif isinstance(im, slice):
+            dim = (f"{im.start if im.start is not None else 'n'}"
+                   + f"-{im.stop if im.stop is not None else 'n'}"
+                   + f"-{im.step if im.step is not None else 'n'}"
+                   )
+        elif isinstance(im, (list, np.ndarray)):
+            idhash = hashlib.md5(
+                np.array(im, dtype=np.uint32).tobytes()).hexdigest()
+            dim = f"h-{idhash[:8]}"
+        else:
+            dim = "unknown"
+        return dim
+
+    @staticmethod
     def get_ppkw_from_ppid(dat_ppid):
         # Data does not fit in the PPID scheme we use, but we still
         # would like to pass pixel_size to __init__ if we need it.
         code, kwargs_str = dat_ppid.split(":")
         if code != HDF5Data.get_ppid_code():
             raise ValueError(f"Could not find data method '{code}'!")
         kwitems = kwargs_str.split("^")
         kwargs = {}
         for item in kwitems:
             var, val = item.split("=")
             if var == "p":
                 kwargs["pixel_size"] = float(val)
+            elif var == "i":
+                if val.startswith("h-") or val == "unknown":
+                    raise ValueError(f"Cannot invert index mapping {val}")
+                elif val == "0":
+                    kwargs["index_mapping"] = None
+                elif val.count("-"):
+                    start, stop = [int(v) for v in val.split("-")]
+                    kwargs["index_mapping"] = slice(start, stop)
+                else:
+                    kwargs["index_mapping"] = int(val)
             else:
                 raise ValueError(f"Invalid parameter '{var}'!")
         return kwargs
 
     def get_basin_data(self, index):
         """Return HDF5Data info for a basin index in `self.basins`
```

### Comparing `dcnum-0.18.0/src/dcnum/read/mapped.py` & `dcnum-0.19.0/src/dcnum/read/mapped.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/segm/segm_thresh.py` & `dcnum-0.19.0/src/dcnum/segm/segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/segm/segmenter.py` & `dcnum-0.19.0/src/dcnum/segm/segmenter.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/segm/segmenter_cpu.py` & `dcnum-0.19.0/src/dcnum/segm/segmenter_cpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/segm/segmenter_gpu.py` & `dcnum-0.19.0/src/dcnum/segm/segmenter_gpu.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/segm/segmenter_manager_thread.py` & `dcnum-0.19.0/src/dcnum/segm/segmenter_manager_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/write/deque_writer_thread.py` & `dcnum-0.19.0/src/dcnum/write/deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/write/queue_collector_thread.py` & `dcnum-0.19.0/src/dcnum/write/queue_collector_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum/write/writer.py` & `dcnum-0.19.0/src/dcnum/write/writer.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/src/dcnum.egg-info/PKG-INFO` & `dcnum-0.19.0/src/dcnum.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcnum
-Version: 0.18.0
+Version: 0.19.0
 Summary: numerics toolbox for imaging deformability cytometry
 Author: Maximilian Schlögel, Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: MIT
 Project-URL: source, https://github.com/DC-Analysis/dcnum
 Project-URL: tracker, https://github.com/DC-Analysis/dcnum/issues
 Project-URL: documentation, https://dcnum.readthedocs.io/en/stable/
```

### Comparing `dcnum-0.18.0/src/dcnum.egg-info/SOURCES.txt` & `dcnum-0.19.0/src/dcnum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/conftest.py` & `dcnum-0.19.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip` & `dcnum-0.19.0/tests/data/fmt-hdf5_cytoshot_extended-moments-features.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip` & `dcnum-0.19.0/tests/data/fmt-hdf5_cytoshot_full-features_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip` & `dcnum-0.19.0/tests/data/fmt-hdf5_cytoshot_full-features_2024.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `dcnum-0.19.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/data/fmt-hdf5_shapein_empty.zip` & `dcnum-0.19.0/tests/data/fmt-hdf5_shapein_empty.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip` & `dcnum-0.19.0/tests/data/fmt-hdf5_shapein_raw-with-variable-length-logs.zip`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/helper_methods.py` & `dcnum-0.19.0/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_feat_background_base.py` & `dcnum-0.19.0/tests/test_feat_background_base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_feat_background_bg_copy.py` & `dcnum-0.19.0/tests/test_feat_background_bg_copy.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_feat_background_bg_roll_median.py` & `dcnum-0.19.0/tests/test_feat_background_bg_roll_median.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_feat_background_bg_sparsemed.py` & `dcnum-0.19.0/tests/test_feat_background_bg_sparsemed.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_feat_brightness.py` & `dcnum-0.19.0/tests/test_feat_brightness.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_feat_event_extractor_manager.py` & `dcnum-0.19.0/tests/test_feat_event_extractor_manager.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_feat_gate.py` & `dcnum-0.19.0/tests/test_feat_gate.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_feat_haralick.py` & `dcnum-0.19.0/tests/test_feat_haralick.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_feat_moments_based.py` & `dcnum-0.19.0/tests/test_feat_moments_based.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_feat_moments_based_extended.py` & `dcnum-0.19.0/tests/test_feat_moments_based_extended.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_feat_volume.py` & `dcnum-0.19.0/tests/test_feat_volume.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_logic_job.py` & `dcnum-0.19.0/tests/test_logic_job.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_logic_join.py` & `dcnum-0.19.0/tests/test_logic_join.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_logic_pipeline.py` & `dcnum-0.19.0/tests/test_logic_pipeline.py`

 * *Files 17% similar despite different names*

```diff
@@ -55,41 +55,35 @@
         assert "image" in h5["events"]
         assert "image_bg" in h5["events"]
         assert len(h5["events/deform"]) == 285
         assert h5.attrs["pipeline:dcnum background"] \
                == "sparsemed:k=250^s=1^t=0^f=0.8^o=1"
 
 
-@pytest.mark.parametrize("index_mapping,size,mapping_out", [
-    (None, 395, "0"),
-    (5, 11, "5"),
-    (slice(3, 5, None), 6, "3-5-n"),
-    ([3, 5, 6, 7], 7, "h-6e582938"),
-])
-def test_duplicate_pipeline(index_mapping, size, mapping_out):
+def test_duplicate_pipeline():
     """Test running the same pipeline twice
 
-    When the pipeline is run on a file with the same pipeline
-    identifier, data are just copied over. Nothing much fancy else.
+    When the pipeline is run on a file that has been run with the same
+    pipeline identifier, then we do not run the pipeline. Instead, we
+    copy the data from the first file.
     """
     path_orig = retrieve_data("fmt-hdf5_cytoshot_full-features_2023.zip")
     path = path_orig.with_name("input.rtdc")
     path2 = path.with_name("path_intermediate.rtdc")
     with read.concatenated_hdf5_data(5 * [path_orig], path_out=path):
         pass
     job = logic.DCNumPipelineJob(
         path_in=path,
         path_out=path2,
-        data_kwargs={"index_mapping": index_mapping},
         background_code="copy",
         segmenter_code="thresh",
         segmenter_kwargs={"thresh": -6,
                           "kwargs_mask": {"closing_disk": 0}},
         debug=True)
-    assert job.kwargs["data_kwargs"]["index_mapping"] == index_mapping
+    assert job.kwargs["data_kwargs"].get("index_mapping") is None
 
     # perform the initial pipeline
     with logic.DCNumJobRunner(job=job) as runner:
         runner.run()
     # Sanity checks for initial job
     with read.HDF5Data(job["path_out"]) as hd:
         # Check the logs
@@ -98,24 +92,20 @@
         assert "Finished background computation" in logdat
         assert "Starting segmentation and feature extraction" in logdat
         assert "Flushing data to disk" in logdat
         assert "Finished segmentation and feature extraction" in logdat
 
     # get the first image for reference
     with h5py.File(path) as h5:
-        if index_mapping is None:
-            idx0 = 0
-        else:
-            idx0 = read.get_mapping_indices(index_mapping)[0]
-        im0 = h5["/events/image"][idx0]
+        im0 = h5["/events/image"][0]
 
     # remove all logs just to be sure nothing interferes
     with h5py.File(path2, "a") as h5:
-        assert h5.attrs["pipeline:dcnum mapping"] == mapping_out
-        assert len(h5["events/deform"]) == size
+        assert h5.attrs["pipeline:dcnum mapping"] == "0"
+        assert len(h5["events/deform"]) == 395
         del h5["logs"]
 
     # now when we do everything again, not a thing should be done
     job2 = logic.DCNumPipelineJob(
         path_in=path2,
         path_out=path2.with_name("final_out.rtdc"),
         no_basins_in_output=True,
@@ -136,19 +126,235 @@
         assert "Flushing data to disk" not in logdat
         assert "Finished segmentation and feature extraction" not in logdat
 
     with h5py.File(job2["path_out"]) as h5:
         assert "deform" in h5["events"]
         assert "image" in h5["events"]
         assert "image_bg" in h5["events"]
-        assert len(h5["events/deform"]) == size
+        assert len(h5["events/deform"]) == 395
         assert h5.attrs["pipeline:dcnum mapping"] == "0"
         assert np.all(h5["events/image"][0] == im0)
 
 
+def test_duplicate_pipeline_redo_index_mapping():
+    """Test running the same pipeline twice
+
+    When the pipeline is run on a file that has been run with the same
+    pipeline identifier, then we do not run the pipeline. Instead, we
+    copy the data from the first file.
+
+    However, if something is odd, such as index mapping defined in the
+    pipeline then redo the computations.
+    This is the purpose of this test.
+    """
+    path_orig = retrieve_data("fmt-hdf5_cytoshot_full-features_2023.zip")
+    path = path_orig.with_name("input.rtdc")
+    path2 = path.with_name("path_intermediate.rtdc")
+    with read.concatenated_hdf5_data(5 * [path_orig], path_out=path):
+        pass
+    job = logic.DCNumPipelineJob(
+        path_in=path,
+        path_out=path2,
+        data_kwargs={"index_mapping": 10},
+        background_code="copy",
+        segmenter_code="thresh",
+        segmenter_kwargs={"thresh": -6,
+                          "kwargs_mask": {"closing_disk": 0}},
+        debug=True)
+    assert job.kwargs["data_kwargs"].get("index_mapping") == 10
+
+    # perform the initial pipeline
+    with logic.DCNumJobRunner(job=job) as runner:
+        runner.run()
+    # Sanity checks for initial job
+    with read.HDF5Data(job["path_out"]) as hd:
+        # Check the logs
+        logdat = " ".join(get_log(hd, time.strftime("dcnum-log-%Y")))
+        assert "Starting background computation" in logdat
+        assert "Finished background computation" in logdat
+        assert "Starting segmentation and feature extraction" in logdat
+        assert "Flushing data to disk" in logdat
+        assert "Finished segmentation and feature extraction" in logdat
+
+    with h5py.File(path2, "a") as h5:
+        # sanity checks
+        assert h5.attrs["pipeline:dcnum mapping"] == "10"
+        assert len(h5["events/deform"]) == 24
+        assert h5.attrs["pipeline:dcnum yield"] == 24
+        # remove all logs just to be sure nothing interferes
+        del h5["logs"]
+        # Modify the yield, triggering a new pipeline run
+        h5.attrs["pipeline:dcnum yield"] = 111111
+
+    # now when we do everything again, not a thing should be done
+    job2 = logic.DCNumPipelineJob(
+        path_in=path2,
+        path_out=path2.with_name("final_out.rtdc"),
+        no_basins_in_output=True,
+        data_kwargs={"index_mapping": 10},
+        background_code="copy",
+        segmenter_code="thresh",
+        segmenter_kwargs={"thresh": -6,
+                          "kwargs_mask": {"closing_disk": 0}},
+        debug=True)
+    with logic.DCNumJobRunner(job=job2) as runner2:
+        runner2.run()
+    # Real check for second run (not the `not`s [sic]!)
+    with read.HDF5Data(job2["path_out"]) as hd:
+        # Check the logs
+        logdat = " ".join(get_log(hd, time.strftime("dcnum-log-%Y")))
+        # Background computation is not repeated
+        assert "Starting background computation" not in logdat
+        assert "Finished background computation" not in logdat
+        # Segmentation is repeated
+        assert "Starting segmentation and feature extraction" in logdat
+        assert "Flushing data to disk" in logdat
+        assert "Finished segmentation and feature extraction" in logdat
+
+    with h5py.File(job2["path_out"]) as h5:
+        assert "deform" in h5["events"]
+        assert "image" in h5["events"]
+        assert "image_bg" in h5["events"]
+        # We have not 24 here, because the index mapping enumerates events,
+        # not frames.
+        assert len(h5["events/deform"]) == 11
+        assert h5.attrs["pipeline:dcnum mapping"] == "10"
+        assert h5.attrs["pipeline:dcnum yield"] == 11
+
+
+def test_duplicate_pipeline_redo_yield():
+    """Test running the same pipeline twice
+
+    When the pipeline is run on a file that has been run with the same
+    pipeline identifier, then we do not run the pipeline. Instead, we
+    copy the data from the first file.
+
+    However, if something is odd, such as the yield of the pipeline not
+    matching the data in the output file, then redo the computations.
+    This is the purpose of this test.
+    """
+    path_orig = retrieve_data("fmt-hdf5_cytoshot_full-features_2023.zip")
+    path = path_orig.with_name("input.rtdc")
+    path2 = path.with_name("path_intermediate.rtdc")
+    with read.concatenated_hdf5_data(5 * [path_orig], path_out=path):
+        pass
+    job = logic.DCNumPipelineJob(
+        path_in=path,
+        path_out=path2,
+        background_code="copy",
+        segmenter_code="thresh",
+        segmenter_kwargs={"thresh": -6,
+                          "kwargs_mask": {"closing_disk": 0}},
+        debug=True)
+    assert job.kwargs["data_kwargs"].get("index_mapping") is None
+
+    # perform the initial pipeline
+    with logic.DCNumJobRunner(job=job) as runner:
+        runner.run()
+    # Sanity checks for initial job
+    with read.HDF5Data(job["path_out"]) as hd:
+        # Check the logs
+        logdat = " ".join(get_log(hd, time.strftime("dcnum-log-%Y")))
+        assert "Starting background computation" in logdat
+        assert "Finished background computation" in logdat
+        assert "Starting segmentation and feature extraction" in logdat
+        assert "Flushing data to disk" in logdat
+        assert "Finished segmentation and feature extraction" in logdat
+
+    with h5py.File(path2, "a") as h5:
+        # sanity checks
+        assert h5.attrs["pipeline:dcnum mapping"] == "0"
+        assert len(h5["events/deform"]) == 395
+        assert h5.attrs["pipeline:dcnum yield"] == 395
+        # remove all logs just to be sure nothing interferes
+        del h5["logs"]
+        # Modify the yield, triggering a new pipeline run
+        h5.attrs["pipeline:dcnum yield"] = 111111
+
+    # now when we do everything again, not a thing should be done
+    job2 = logic.DCNumPipelineJob(
+        path_in=path2,
+        path_out=path2.with_name("final_out.rtdc"),
+        no_basins_in_output=True,
+        background_code="copy",
+        segmenter_code="thresh",
+        segmenter_kwargs={"thresh": -6,
+                          "kwargs_mask": {"closing_disk": 0}},
+        debug=True)
+    with logic.DCNumJobRunner(job=job2) as runner2:
+        runner2.run()
+    # Real check for second run (not the `not`s [sic]!)
+    with read.HDF5Data(job2["path_out"]) as hd:
+        # Check the logs
+        logdat = " ".join(get_log(hd, time.strftime("dcnum-log-%Y")))
+        # Background computation is not repeated
+        assert "Starting background computation" not in logdat
+        assert "Finished background computation" not in logdat
+        # Segmentation is repeated
+        assert "Starting segmentation and feature extraction" in logdat
+        assert "Flushing data to disk" in logdat
+        assert "Finished segmentation and feature extraction" in logdat
+
+    with h5py.File(job2["path_out"]) as h5:
+        assert "deform" in h5["events"]
+        assert "image" in h5["events"]
+        assert "image_bg" in h5["events"]
+        assert len(h5["events/deform"]) == 395
+        assert h5.attrs["pipeline:dcnum mapping"] == "0"
+        assert h5.attrs["pipeline:dcnum yield"] == 395
+
+
+@pytest.mark.parametrize("index_mapping,size,mapping_out", [
+    (5, 11, "5"),
+    (slice(3, 5, None), 6, "3-5-n"),
+    ([3, 5, 6, 7], 7, "h-6e582938"),
+])
+def test_index_mapping_pipeline(index_mapping, size, mapping_out):
+    """Test running the same pipeline twice
+
+    When the pipeline is run on a file with the same pipeline
+    identifier, data are just copied over. Nothing much fancy else.
+    """
+    path_orig = retrieve_data("fmt-hdf5_cytoshot_full-features_2023.zip")
+    path = path_orig.with_name("input.rtdc")
+    path2 = path.with_name("path_intermediate.rtdc")
+    with read.concatenated_hdf5_data(5 * [path_orig], path_out=path):
+        pass
+    job = logic.DCNumPipelineJob(
+        path_in=path,
+        path_out=path2,
+        data_kwargs={"index_mapping": index_mapping},
+        background_code="copy",
+        segmenter_code="thresh",
+        segmenter_kwargs={"thresh": -6,
+                          "kwargs_mask": {"closing_disk": 0}},
+        debug=True)
+    assert job.kwargs["data_kwargs"]["index_mapping"] == index_mapping
+
+    # perform the initial pipeline
+    with logic.DCNumJobRunner(job=job) as runner:
+        runner.run()
+    # Sanity checks for initial job
+    with read.HDF5Data(job["path_out"]) as hd:
+        # Check the logs
+        logdat = " ".join(get_log(hd, time.strftime("dcnum-log-%Y")))
+        assert "Starting background computation" in logdat
+        assert "Finished background computation" in logdat
+        assert "Starting segmentation and feature extraction" in logdat
+        assert "Flushing data to disk" in logdat
+        assert "Finished segmentation and feature extraction" in logdat
+
+    with h5py.File(job["path_out"]) as h5:
+        assert "deform" in h5["events"]
+        assert "image" in h5["events"]
+        assert "image_bg" in h5["events"]
+        assert len(h5["events/deform"]) == size
+        assert h5.attrs["pipeline:dcnum mapping"] == mapping_out
+
+
 def test_duplicate_transfer_basin_data():
     """task_transfer_basin_data should not copy basin data from input"""
     path_orig = retrieve_data("fmt-hdf5_cytoshot_full-features_2023.zip")
     path = path_orig.with_name("input.rtdc")
     path2 = path.with_name("path_intermediate.rtdc")
     with read.concatenated_hdf5_data(5 * [path_orig], path_out=path):
         pass
@@ -331,15 +537,15 @@
         pass
 
     with read.HDF5Data(path) as hd:
         assert len(hd) == 200, "sanity check"
 
     # this is the default pipeline
     gen_id = ppid.DCNUM_PPID_GENERATION
-    dat_id = "hdf:p=0.2645"
+    dat_id = "hdf:p=0.2645^i=0"
     bg_id = "sparsemed:k=200^s=1^t=0^f=0.8^o=1"
     seg_id = "thresh:t=-6:cle=1^f=1^clo=0"
     feat_id = "legacy:b=1^h=1^v=1"
     gate_id = "norm:o=0^s=10"
     jobid = "|".join([gen_id, dat_id, bg_id, seg_id, feat_id, gate_id])
 
     job = logic.DCNumPipelineJob(
@@ -398,15 +604,15 @@
         pass
 
     with read.HDF5Data(path) as hd:
         assert len(hd) == 200, "sanity check"
 
     # this is the default pipeline
     gen_id = ppid.DCNUM_PPID_GENERATION
-    dat_id = "hdf:p=0.2645"
+    dat_id = "hdf:p=0.2645^i=0"
     bg_id = "sparsemed:k=200^s=1^t=0^f=0.8^o=0"
     seg_id = "thresh:t=-6:cle=1^f=1^clo=0"
     feat_id = "legacy:b=1^h=1^v=1"
     gate_id = "norm:o=0^s=10"
     jobid = "|".join([gen_id, dat_id, bg_id, seg_id, feat_id, gate_id])
 
     job = logic.DCNumPipelineJob(
@@ -470,15 +676,15 @@
         runner.start()
         runner.join()
 
 
 @pytest.mark.parametrize("attr,oldval,newbg", [
     # Changes that trigger computation of new background
     ["pipeline:dcnum generation", "1", True],
-    ["pipeline:dcnum data", "hdf:p=0.2656", True],
+    ["pipeline:dcnum data", "hdf:p=0.2656^i=0", True],
     ["pipeline:dcnum background", "sparsemed:k=100^s=1^t=0^f=0.8^o=1", True],
     # Changes that don't trigger background computation
     ["pipeline:dcnum segmenter", "thresh:t=-1:cle=1^f=1^clo=2", False],
     ["pipeline:dcnum feature", "thresh:t=-1:cle=1^f=1^clo=2", False],
     ["pipeline:dcnum gate", "norm:o=0^s=5", False],
     ["pipeline:dcnum yield", 5000, False],
     ["pipeline:dcnum hash", "asdasd", False],
@@ -501,15 +707,15 @@
 
     with h5py.File(path, "a") as h5:
         # marker for identifying recomputation of background
         h5["events/image_bg"][:, 0, 0] = 200
 
         # Set the default values
         h5.attrs["pipeline:dcnum generation"] = ppid.DCNUM_PPID_GENERATION
-        h5.attrs["pipeline:dcnum data"] = "hdf:p=0.2645"
+        h5.attrs["pipeline:dcnum data"] = "hdf:p=0.2645^i=0"
         h5.attrs["pipeline:dcnum background"] = \
             "sparsemed:k=200^s=1^t=0^f=0.8^o=1"
         h5.attrs["pipeline:dcnum segmenter"] = "thresh:t=-6:cle=1^f=1^clo=2"
         h5.attrs["pipeline:dcnum feature"] = "legacy:b=1^h=1^v=1"
         h5.attrs["pipeline:dcnum gate"] = "norm:o=0^s=10"
         h5.attrs["pipeline:dcnum yield"] = h5["events/image"].shape[0]
 
@@ -549,15 +755,15 @@
 
     path = path_orig.with_name("input.rtdc")
     with read.concatenated_hdf5_data(5 * [path_orig], path_out=path):
         pass
 
     # this is the default pipeline
     gen_id = ppid.DCNUM_PPID_GENERATION
-    dat_id = "hdf:p=0.2645"
+    dat_id = "hdf:p=0.2645^i=0"
     bg_id = "sparsemed:k=200^s=1^t=0^f=0.8^o=1"
     seg_id = "thresh:t=-6:cle=1^f=1^clo=2"
     feat_id = "legacy:b=1^h=1^v=1"
     gate_id = "norm:o=0^s=10"
     jobid = "|".join([gen_id, dat_id, bg_id, seg_id, feat_id, gate_id])
 
     job = logic.DCNumPipelineJob(path_in=path, debug=True)
```

### Comparing `dcnum-0.18.0/tests/test_meta_paths.py` & `dcnum-0.19.0/tests/test_meta_paths.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_meta_ppid_base.py` & `dcnum-0.19.0/tests/test_meta_ppid_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,21 +28,21 @@
     def get_ppid_code(cls):
         return cls.__name__
 
 
 def test_compute_pipeline_hash():
     pp_hash = ppid.compute_pipeline_hash(
         gen_id="7",
-        dat_id="hdf:p=0.34",
+        dat_id="hdf:p=0.34^i=0",
         bg_id="sparsemed:k=200^s=1^t=0^f=0.8^o=1",
         seg_id="thresh:t=-3:cle=1^f=1^clo=2",
         feat_id="legacy:b=1^h=0^v=1",
         gate_id="norm:o=0^s=11",
     )
-    assert pp_hash == "2e56aa93fcb264381c90a8fd181b3fbc"
+    assert pp_hash == "4f3a850410b9801393ab5738afe69e9a"
 
 
 @pytest.mark.parametrize("in_list,out_list", [
     (["camera", "campus"],
      ["came", "camp"]),
     (["cole", "coleman"],
      ["cole", "colem"]),
```

### Comparing `dcnum-0.18.0/tests/test_meta_ppid_bg.py` & `dcnum-0.19.0/tests/test_meta_ppid_bg.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_meta_ppid_data.py` & `dcnum-0.19.0/tests/test_meta_ppid_gate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,24 @@
-from dcnum.read import HDF5Data
+from dcnum.feat.gate import Gate
 
 
-def test_ppid_decoding_dat_check_kwargs():
-    dat_ppid = "hdf:p=0.2658"
-    kwargs = HDF5Data.get_ppkw_from_ppid(dat_ppid)
-    assert kwargs["pixel_size"] == 0.2658
+def test_ppid_decoding_gate_check_kwargs():
+    gate_ppid = "norm:o=1^s=12"
+    kwargs = Gate.get_ppkw_from_ppid(gate_ppid)
+    assert kwargs["size_thresh_mask"] == 12
+    assert kwargs["online_gates"] is True
 
 
-def test_ppid_encoding_dat_check_kwargs():
-    kwargs = {"pixel_size": 0.34}
-    ppid = HDF5Data.get_ppid_from_ppkw(kwargs)
-    assert ppid == "hdf:p=0.34"
-
-
-def test_ppid_encoding_dat_check_kwargs_acc():
-    # accuracy for pixel_size is 8 digits after the decimal point
-    kwargs = {"pixel_size": 0.3400000036}
-    ppid = HDF5Data.get_ppid_from_ppkw(kwargs)
-    assert ppid == "hdf:p=0.34"
+def test_ppid_encoding_gate_check_kwargs():
+    kwargs = {"size_thresh_mask": 11, "online_gates": False}
+    ppid = Gate.get_ppid_from_ppkw(kwargs)
+    assert ppid == "norm:o=0^s=11"
 
 
 def test_ppid_required_method_definitions():
-    dat_code = "hdf"
-    dat_class = HDF5Data
-    assert hasattr(dat_class, "get_ppid")
-    assert hasattr(dat_class, "get_ppid_code")
-    assert hasattr(dat_class, "get_ppid_from_ppkw")
-    assert hasattr(dat_class, "get_ppkw_from_ppid")
-    assert dat_class.get_ppid_code() == dat_code
+    gate_code = "norm"
+    gate_class = Gate
+    assert hasattr(gate_class, "get_ppid")
+    assert hasattr(gate_class, "get_ppid_code")
+    assert hasattr(gate_class, "get_ppid_from_ppkw")
+    assert hasattr(gate_class, "get_ppkw_from_ppid")
+    assert gate_class.get_ppid_code() == gate_code
```

### Comparing `dcnum-0.18.0/tests/test_meta_ppid_feat.py` & `dcnum-0.19.0/tests/test_meta_ppid_feat.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_meta_ppid_segm.py` & `dcnum-0.19.0/tests/test_meta_ppid_segm.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_read_basin.py` & `dcnum-0.19.0/tests/test_read_basin.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_read_concat_hdf5.py` & `dcnum-0.19.0/tests/test_read_concat_hdf5.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_read_hdf5.py` & `dcnum-0.19.0/tests/test_read_hdf5.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,30 +45,30 @@
 
 
 def test_get_ppid():
     path = retrieve_data(
         "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
 
     with read.HDF5Data(path) as hd:
-        assert hd.get_ppid() == "hdf:p=0.2645"
+        assert hd.get_ppid() == "hdf:p=0.2645^i=0"
 
     with read.HDF5Data(path, pixel_size=0.49) as hd:
-        assert hd.get_ppid() == "hdf:p=0.49"
+        assert hd.get_ppid() == "hdf:p=0.49^i=0"
 
 
 def test_get_ppkw_from_ppid_error_bad_code():
     with pytest.raises(ValueError,
                        match="Could not find data method 'peter'"):
         read.HDF5Data.get_ppkw_from_ppid("peter:p=0.44")
 
 
 def test_get_ppkw_from_ppid_error_bad_parameter():
     with pytest.raises(ValueError,
                        match="Invalid parameter 'k'"):
-        read.HDF5Data.get_ppkw_from_ppid("hdf:k=0.44")
+        read.HDF5Data.get_ppkw_from_ppid("hdf:k=0.44^i=0")
 
 
 def test_get_ppkw_from_ppid_pixel_size():
     ppkw = read.HDF5Data.get_ppkw_from_ppid("hdf:p=0.44")
     assert np.allclose(ppkw["pixel_size"], 0.44)
     assert len(ppkw.keys()) == 1
```

### Comparing `dcnum-0.18.0/tests/test_read_hdf5_index_mapping.py` & `dcnum-0.19.0/tests/test_read_hdf5_index_mapping.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_segm_base.py` & `dcnum-0.19.0/tests/test_segm_base.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_segm_no_mask_proc.py` & `dcnum-0.19.0/tests/test_segm_no_mask_proc.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_segm_thresh.py` & `dcnum-0.19.0/tests/test_segm_thresh.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_write_deque_writer_thread.py` & `dcnum-0.19.0/tests/test_write_deque_writer_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_write_queue_collector_thread.py` & `dcnum-0.19.0/tests/test_write_queue_collector_thread.py`

 * *Files identical despite different names*

### Comparing `dcnum-0.18.0/tests/test_write_writer.py` & `dcnum-0.19.0/tests/test_write_writer.py`

 * *Files identical despite different names*

