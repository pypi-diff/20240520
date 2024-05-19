# Comparing `tmp/dvcx-0.79.0.tar.gz` & `tmp/dvcx-0.80.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.79.0.tar", last modified: Wed May 15 22:48:56 2024, max compression
+gzip compressed data, was "dvcx-0.80.0.tar", last modified: Sun May 19 23:11:58 2024, max compression
```

## Comparing `dvcx-0.79.0.tar` & `dvcx-0.80.0.tar`

### file list

```diff
@@ -1,254 +1,252 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.405135 dvcx-0.79.0/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-15 22:48:47.000000 dvcx-0.79.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-15 22:48:47.000000 dvcx-0.79.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.349135 dvcx-0.79.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.349135 dvcx-0.79.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-15 22:48:47.000000 dvcx-0.79.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-15 22:48:47.000000 dvcx-0.79.0/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-15 22:48:47.000000 dvcx-0.79.0/.github/ISSUE_TEMPLATE/epic-or-story.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-15 22:48:47.000000 dvcx-0.79.0/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-15 22:48:47.000000 dvcx-0.79.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.349135 dvcx-0.79.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-15 22:48:47.000000 dvcx-0.79.0/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-15 22:48:47.000000 dvcx-0.79.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-15 22:48:47.000000 dvcx-0.79.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-15 22:48:47.000000 dvcx-0.79.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-15 22:48:47.000000 dvcx-0.79.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-15 22:48:47.000000 dvcx-0.79.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.349135 dvcx-0.79.0/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-15 22:48:47.000000 dvcx-0.79.0/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-15 22:48:47.000000 dvcx-0.79.0/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-15 22:48:47.000000 dvcx-0.79.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-15 22:48:47.000000 dvcx-0.79.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-15 22:48:47.000000 dvcx-0.79.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.349135 dvcx-0.79.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-15 22:48:47.000000 dvcx-0.79.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-15 22:48:47.000000 dvcx-0.79.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-15 22:48:47.000000 dvcx-0.79.0/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-15 22:48:56.405135 dvcx-0.79.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-15 22:48:47.000000 dvcx-0.79.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.349135 dvcx-0.79.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-15 22:48:47.000000 dvcx-0.79.0/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.353135 dvcx-0.79.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/llm-claude-aggregate-query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/llm-claude-simple-query.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/llm-claude.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.353135 dvcx-0.79.0/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.357135 dvcx-0.79.0/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.357135 dvcx-0.79.0/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-15 22:48:47.000000 dvcx-0.79.0/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-15 22:48:47.000000 dvcx-0.79.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-05-15 22:48:47.000000 dvcx-0.79.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 22:48:56.405135 dvcx-0.79.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.345135 dvcx-0.79.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.361135 dvcx-0.79.0/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-15 22:48:56.000000 dvcx-0.79.0/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.361135 dvcx-0.79.0/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72958 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    14495 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/catalog/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    31032 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.365135 dvcx-0.79.0/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/client/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.365135 dvcx-0.79.0/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    45892 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/data_storage/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    30749 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    34870 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    17671 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.373135 dvcx-0.79.0/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)    16852 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/feature_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/tar_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/webdataset_laion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.377135 dvcx-0.79.0/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    60126 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/query/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/query/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.377135 dvcx-0.79.0/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.377135 dvcx-0.79.0/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.381135 dvcx-0.79.0/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.381135 dvcx-0.79.0/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/functions/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.381135 dvcx-0.79.0/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-15 22:48:47.000000 dvcx-0.79.0/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.397135 dvcx-0.79.0/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-15 22:48:56.000000 dvcx-0.79.0/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-15 22:48:56.000000 dvcx-0.79.0/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 22:48:56.000000 dvcx-0.79.0/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 22:48:56.000000 dvcx-0.79.0/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-15 22:48:56.000000 dvcx-0.79.0/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-15 22:48:56.000000 dvcx-0.79.0/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.385135 dvcx-0.79.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.385135 dvcx-0.79.0/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16205 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.389135 dvcx-0.79.0/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35731 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   113348 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    28867 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/func/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     7678 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/func/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.389135 dvcx-0.79.0/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/scripts/name_len_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/scripts/name_len_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/test_cli_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/test_query_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.393135 dvcx-0.79.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.397135 dvcx-0.79.0/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/test_cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/test_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/lib/test_webdataset_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.397135 dvcx-0.79.0/tests/unit/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:56.397135 dvcx-0.79.0/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/sql/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_catalog_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_catalog_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_dataset_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/unit/test_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-05-15 22:48:47.000000 dvcx-0.79.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.686604 dvcx-0.80.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-19 23:11:53.000000 dvcx-0.80.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-19 23:11:53.000000 dvcx-0.80.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.638604 dvcx-0.80.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.638604 dvcx-0.80.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-19 23:11:53.000000 dvcx-0.80.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-19 23:11:53.000000 dvcx-0.80.0/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-19 23:11:53.000000 dvcx-0.80.0/.github/ISSUE_TEMPLATE/epic-or-story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-19 23:11:53.000000 dvcx-0.80.0/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-19 23:11:53.000000 dvcx-0.80.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.638604 dvcx-0.80.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-19 23:11:53.000000 dvcx-0.80.0/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-19 23:11:53.000000 dvcx-0.80.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-19 23:11:53.000000 dvcx-0.80.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-19 23:11:53.000000 dvcx-0.80.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-19 23:11:53.000000 dvcx-0.80.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-19 23:11:53.000000 dvcx-0.80.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.638604 dvcx-0.80.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-19 23:11:53.000000 dvcx-0.80.0/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-19 23:11:53.000000 dvcx-0.80.0/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-19 23:11:53.000000 dvcx-0.80.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-19 23:11:53.000000 dvcx-0.80.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-19 23:11:53.000000 dvcx-0.80.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.638604 dvcx-0.80.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-19 23:11:53.000000 dvcx-0.80.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-19 23:11:53.000000 dvcx-0.80.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-19 23:11:53.000000 dvcx-0.80.0/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-19 23:11:58.686604 dvcx-0.80.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-19 23:11:53.000000 dvcx-0.80.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.638604 dvcx-0.80.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-19 23:11:53.000000 dvcx-0.80.0/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.642604 dvcx-0.80.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/llm-claude-aggregate-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/llm-claude-simple-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/llm-claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.646604 dvcx-0.80.0/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.646604 dvcx-0.80.0/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.646604 dvcx-0.80.0/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-19 23:11:53.000000 dvcx-0.80.0/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-19 23:11:53.000000 dvcx-0.80.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-19 23:11:53.000000 dvcx-0.80.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 23:11:58.686604 dvcx-0.80.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.630604 dvcx-0.80.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.650604 dvcx-0.80.0/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-19 23:11:58.000000 dvcx-0.80.0/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.650604 dvcx-0.80.0/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72656 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.654604 dvcx-0.80.0/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.654604 dvcx-0.80.0/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45892 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26305 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33673 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17671 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.658604 dvcx-0.80.0/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/feature_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/tar_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.662604 dvcx-0.80.0/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61484 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/query/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/query/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.662604 dvcx-0.80.0/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.662604 dvcx-0.80.0/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.662604 dvcx-0.80.0/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.666604 dvcx-0.80.0/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/sql/functions/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.666604 dvcx-0.80.0/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10468 2024-05-19 23:11:53.000000 dvcx-0.80.0/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.678604 dvcx-0.80.0/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-19 23:11:58.000000 dvcx-0.80.0/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-19 23:11:58.000000 dvcx-0.80.0/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 23:11:58.000000 dvcx-0.80.0/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-19 23:11:58.000000 dvcx-0.80.0/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-19 23:11:58.000000 dvcx-0.80.0/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-19 23:11:58.000000 dvcx-0.80.0/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.666604 dvcx-0.80.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.666604 dvcx-0.80.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16483 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.670604 dvcx-0.80.0/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35078 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113497 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28871 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/func/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.670604 dvcx-0.80.0/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/scripts/name_len_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/scripts/name_len_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/test_cli_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/test_query_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.674604 dvcx-0.80.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.674604 dvcx-0.80.0/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/lib/test_cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/lib/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/lib/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/lib/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.678604 dvcx-0.80.0/tests/unit/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:58.678604 dvcx-0.80.0/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/sql/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_dataset_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-19 23:11:53.000000 dvcx-0.80.0/tests/utils.py
```

### Comparing `dvcx-0.79.0/.cruft.json` & `dvcx-0.80.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/.github/ISSUE_TEMPLATE/bug_report.md` & `dvcx-0.80.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/.github/ISSUE_TEMPLATE/epic-or-story.md` & `dvcx-0.80.0/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/.github/workflows/benchmarks.yml` & `dvcx-0.80.0/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/.github/workflows/release.yml` & `dvcx-0.80.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/.github/workflows/tests.yml` & `dvcx-0.80.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/.gitignore` & `dvcx-0.80.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/.pre-commit-config.yaml` & `dvcx-0.80.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/CODE_OF_CONDUCT.rst` & `dvcx-0.80.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/CONTRIBUTING.rst` & `dvcx-0.80.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/LICENSE` & `dvcx-0.80.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/LICENSES/Apache-2.0.txt` & `dvcx-0.80.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/LICENSES/BSD-3-Clause.txt` & `dvcx-0.80.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/LICENSES/Python-2.0.txt` & `dvcx-0.80.0/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/PKG-INFO` & `dvcx-0.80.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.79.0
+Version: 0.80.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.79.0/README.rst` & `dvcx-0.80.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/docs/udfs.md` & `dvcx-0.80.0/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/blip2_image_desc_lib.py` & `dvcx-0.80.0/examples/blip2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/clip.py` & `dvcx-0.80.0/examples/clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/common_sql_functions.py` & `dvcx-0.80.0/examples/common_sql_functions.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/dir_expansion.py` & `dvcx-0.80.0/examples/dir_expansion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/hf_pipeline.py` & `dvcx-0.80.0/examples/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/llava2_image_desc_lib.py` & `dvcx-0.80.0/examples/llava2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/llm-claude-aggregate-query.py` & `dvcx-0.80.0/examples/llm-claude-aggregate-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/llm-claude-simple-query.py` & `dvcx-0.80.0/examples/llm-claude-simple-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/llm-claude.py` & `dvcx-0.80.0/examples/llm-claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/loader.py` & `dvcx-0.80.0/examples/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/neurips/README` & `dvcx-0.80.0/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/neurips/distance_to_query.py` & `dvcx-0.80.0/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/neurips/llm_chat.py` & `dvcx-0.80.0/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/neurips/single_query.py` & `dvcx-0.80.0/examples/neurips/single_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/neurips/text_loaders.py` & `dvcx-0.80.0/examples/neurips/text_loaders.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/openai_image_desc_lib.py` & `dvcx-0.80.0/examples/openai_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/openimage-detect.py` & `dvcx-0.80.0/examples/openimage-detect.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/pose_detection.py` & `dvcx-0.80.0/examples/pose_detection.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/torch-loader.py` & `dvcx-0.80.0/examples/torch-loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/udfs/batching.py` & `dvcx-0.80.0/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/udfs/image_transformation.py` & `dvcx-0.80.0/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/udfs/parallel.py` & `dvcx-0.80.0/examples/udfs/parallel.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/udfs/simple.py` & `dvcx-0.80.0/examples/udfs/simple.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/udfs/stateful.py` & `dvcx-0.80.0/examples/udfs/stateful.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/udfs/stateful_similarity.py` & `dvcx-0.80.0/examples/udfs/stateful_similarity.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/unstructured-text.py` & `dvcx-0.80.0/examples/unstructured-text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/wds.py` & `dvcx-0.80.0/examples/wds.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/wds_filtered.py` & `dvcx-0.80.0/examples/wds_filtered.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/wds_meta.py` & `dvcx-0.80.0/examples/wds_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/zalando/zalando_clip.py` & `dvcx-0.80.0/examples/zalando/zalando_clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.80.0/examples/zalando/zalando_dir_as_class.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/noxfile.py` & `dvcx-0.80.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/pyproject.toml` & `dvcx-0.80.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 where = ["src"]
 namespaces = false
 
 [tool.setuptools_scm]
 write_to = "src/dvcx/_version.py"
 
 [tool.pytest.ini_options]
-addopts = "-ra -m 'not benchmark'"
+addopts = "-rfEs -m 'not benchmark'"
 markers = [
   "benchmark: benchmarks.",
   "e2e: End-to-end tests"
 ]
 asyncio_mode = "auto"
 filterwarnings = [
   "ignore:Field name .* shadows an attribute in parent:UserWarning"  # dvcx.lib.feature
```

### Comparing `dvcx-0.79.0/src/dvcx/asyn.py` & `dvcx-0.80.0/src/dvcx/asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/cache.py` & `dvcx-0.80.0/src/dvcx/cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/catalog/catalog.py` & `dvcx-0.80.0/src/dvcx/catalog/catalog.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import ast
-import functools
 import io
 import json
 import logging
 import math
 import os
 import os.path
 import posixpath
@@ -12,15 +11,15 @@
 import time
 import traceback
 from ast import Attribute, Call, Expr, Import, Load, Name, alias
 from collections.abc import Iterable, Iterator, Mapping, Sequence
 from contextlib import contextmanager, nullcontext
 from copy import copy
 from dataclasses import dataclass
-from pathlib import Path
+from functools import cached_property, reduce
 from random import shuffle
 from threading import Thread
 from typing import (
     IO,
     TYPE_CHECKING,
     Any,
     Callable,
@@ -31,15 +30,14 @@
 )
 from uuid import uuid4
 
 import requests
 import sqlalchemy as sa
 import yaml
 from attrs import asdict
-from fsspec.implementations.local import LocalFileSystem
 from sqlalchemy import Column
 from tqdm import tqdm
 
 from dvcx.cache import DVCXCache
 from dvcx.client import Client
 from dvcx.config import get_remote_config, read_config
 from dvcx.data_storage.schema import DATASET_CORE_COLUMN_NAMES
@@ -55,15 +53,14 @@
 )
 from dvcx.dataset import Status as DatasetStatus
 from dvcx.error import (
     ClientError,
     DatasetInvalidVersionError,
     DatasetNotFoundError,
     DVCXError,
-    InconsistentSignalType,
     PendingIndexingError,
     QueryScriptCancelError,
     QueryScriptCompileError,
     QueryScriptDatasetNotFound,
     QueryScriptRunError,
 )
 from dvcx.listing import Listing
@@ -77,15 +74,14 @@
     chunk,
     dvcx_paths_join,
     import_object,
     parse_params_string,
 )
 
 from .datasource import DataSource
-from .formats import IndexingFormat, apply_processors
 
 if TYPE_CHECKING:
     from dvcx.data_storage import (
         AbstractIDGenerator,
         AbstractMetastore,
         AbstractWarehouse,
     )
@@ -571,26 +567,37 @@
         self,
         id_generator: "AbstractIDGenerator",
         metastore: "AbstractMetastore",
         warehouse: "AbstractWarehouse",
         cache_dir=None,
         tmp_dir=None,
         client_config: Optional[dict[str, Any]] = None,
+        warehouse_ready_callback: Optional[
+            Callable[["AbstractWarehouse"], None]
+        ] = None,
     ):
         dvcx_dir = DVCXDir(cache=cache_dir, tmp=tmp_dir)
         dvcx_dir.init()
         self.id_generator = id_generator
         self.metastore = metastore
-        self.warehouse = warehouse
+        self._warehouse = warehouse
         self.cache = DVCXCache(dvcx_dir.cache, dvcx_dir.tmp)
         self.client_config = client_config if client_config is not None else {}
         self._init_params = {
             "cache_dir": cache_dir,
             "tmp_dir": tmp_dir,
         }
+        self._warehouse_ready_callback = warehouse_ready_callback
+
+    @cached_property
+    def warehouse(self) -> "AbstractWarehouse":
+        if self._warehouse_ready_callback:
+            self._warehouse_ready_callback(self._warehouse)
+
+        return self._warehouse
 
     def get_init_params(self) -> dict[str, Any]:
         return {
             **self._init_params,
             "client_config": self.client_config,
         }
 
@@ -635,22 +642,14 @@
                 ]
                 code_ast.body[-1:] = new_expressions
             else:
                 raise Exception("Last line in a script was not an expression")
 
         return ast.unparse(code_ast)
 
-    def add_storage(self, source: str) -> None:
-        path = LocalFileSystem._strip_protocol(source)
-        if not os.path.isdir(path):
-            raise RuntimeError(f"{path} is not a directory")
-        uri = StorageURI(Path(path).resolve().as_uri())
-        print(f"Registering storage {uri}")
-        self.metastore.create_storage_if_not_registered(uri)
-
     def parse_url(self, uri: str, **config: Any) -> tuple[Client, str]:
         config = config or self.client_config
         return Client.parse_url(uri, self.metastore, self.cache, **config)
 
     def get_client(self, uri: StorageURI, **config: Any) -> Client:
         """
         Return the client corresponding to the given source `uri`.
@@ -662,15 +661,14 @@
     def enlist_source(
         self,
         source: str,
         ttl: int,
         force_update=False,
         skip_indexing=False,
         client_config=None,
-        index_processors: Optional[list[IndexingFormat]] = None,
     ) -> tuple[Listing, str]:
         if force_update and skip_indexing:
             raise ValueError(
                 "Both force_update and skip_indexing flags"
                 " cannot be True at the same time"
             )
 
@@ -741,37 +739,21 @@
         source_warehouse = self.warehouse.clone(uri=client.uri, partial_id=partial_id)
 
         lst = Listing(storage, source_metastore, source_warehouse, client)
 
         try:
             lst.fetch(prefix)
 
-            # Apply index processing before marking storage as indexed.
-            if index_processors:
-                apply_processors(lst, path, index_processors)
-
             source_metastore.mark_storage_indexed(
                 storage.uri,
                 Status.PARTIAL if prefix else Status.COMPLETE,
                 ttl,
                 prefix=prefix,
                 partial_id=partial_id,
             )
-        except InconsistentSignalType as e:
-            # handle all custom errors here which messages we want to show
-            # directly to the user (user mistake generated error)
-            source_metastore.mark_storage_indexed(
-                storage.uri,
-                Status.FAILED,
-                ttl,
-                prefix=prefix,
-                error_message=str(e),
-                error_stack=traceback.format_exc(),
-            )
-            raise
         except ClientError as e:
             # for handling cloud errors
             error_message = INDEX_INTERNAL_ERROR_MESSAGE
             if e.error_code in ["InvalidAccessKeyId", "SignatureDoesNotMatch"]:
                 error_message = "Invalid cloud credentials"
 
             source_metastore.mark_storage_indexed(
@@ -801,26 +783,24 @@
     def enlist_sources(
         self,
         sources: list[str],
         ttl: int,
         update: bool,
         skip_indexing=False,
         client_config=None,
-        index_processors: Optional[list[IndexingFormat]] = None,
         only_index=False,
     ) -> Optional[list["DataSource"]]:
         enlisted_sources = []
         for src in sources:  # Opt: parallel
             listing, file_path = self.enlist_source(
                 src,
                 ttl,
                 update,
                 skip_indexing=skip_indexing,
                 client_config=client_config or self.client_config,
-                index_processors=index_processors,
             )
             enlisted_sources.append((listing, file_path))
 
         if only_index:
             # sometimes we don't really need listing result (e.g on indexing process)
             # so this is to improve performance
             return None
@@ -1195,15 +1175,15 @@
                     client_config=client_config,
                     recursive=recursive,
                 )
 
             dataset_queries.append(dq)
 
         # create union of all dataset queries created from sources
-        dq = functools.reduce(lambda ds1, ds2: ds1.union(ds2), dataset_queries)
+        dq = reduce(lambda ds1, ds2: ds1.union(ds2), dataset_queries)
         try:
             dq.save(name)
         except Exception:
             ds = self.get_dataset(name)
             self.metastore.update_dataset_status(
                 ds,
                 DatasetStatus.FAILED,
@@ -1225,14 +1205,27 @@
             ds,
             ds.latest_version,
             sources="\n".join(sources),
         )
 
         return self.get_dataset(name)
 
+    def register_new_dataset(
+        self,
+        source_dataset: DatasetRecord,
+        source_version: int,
+        target_name: str,
+    ) -> DatasetRecord:
+        target_dataset = self.metastore.create_dataset(
+            target_name,
+            query_script=source_dataset.query_script,
+            custom_column_types=source_dataset.custom_column_types_serialized,
+        )
+        return self.register_dataset(source_dataset, source_version, target_dataset, 1)
+
     def register_dataset(
         self,
         dataset: DatasetRecord,
         version: int,
         target_dataset: DatasetRecord,
         target_version: Optional[int] = None,
     ) -> DatasetRecord:
@@ -1785,14 +1778,15 @@
 
     def query(
         self,
         query_script: str,
         envs: Optional[Mapping[str, str]] = None,
         python_executable: Optional[str] = None,
         save: bool = False,
+        save_as: Optional[str] = None,
         preview_limit: Optional[int] = 10,
         preview_offset: int = 0,
         preview_columns: Optional[list[str]] = None,
         capture_output: bool = True,
         output_hook: Callable[[str], None] = noop,
         params: Optional[dict[str, str]] = None,
     ) -> QueryResult:
@@ -1823,14 +1817,19 @@
         try:
             query_script_compiled = self.compile_query_script(query_script)
         except Exception as exc:
             raise QueryScriptCompileError(
                 f"Query script failed to compile, reason: {exc}"
             ) from exc
 
+        if save_as and save_as.startswith(QUERY_DATASET_PREFIX):
+            raise ValueError(
+                f"Cannot use {QUERY_DATASET_PREFIX} prefix for dataset name"
+            )
+
         r, w = os.pipe()
         if os.name == "nt":
             import msvcrt
 
             os.set_inheritable(w, True)
 
             startupinfo = subprocess.STARTUPINFO()  # type: ignore[attr-defined]
@@ -1849,14 +1848,15 @@
                     {
                         "limit": preview_limit,
                         "offset": preview_offset,
                         "columns": preview_columns,
                     }
                 ),
                 "DVCX_QUERY_SAVE": "1" if save else "",
+                "DVCX_QUERY_SAVE_AS": save_as or "",
                 "PYTHONUNBUFFERED": "1",
                 "DVCX_OUTPUT_FD": str(handle),
             },
         )
 
         python_executable = python_executable or sys.executable
         with subprocess.Popen(
@@ -1877,20 +1877,14 @@
             with ctx as lines, open(r) as f:
                 response_text = ""
                 while proc.poll() is None:
                     response_text += f.readline()
                     time.sleep(0.1)
                 response_text += f.readline()
 
-        try:
-            response = json.loads(response_text)
-        except ValueError:
-            response = {}
-        exec_result = ExecutionResult(**response)
-
         output = "".join(lines)
 
         if proc.returncode:
             if proc.returncode == QUERY_SCRIPT_CANCELED_EXIT_CODE:
                 raise QueryScriptCancelError(
                     "Query script was canceled by user",
                     return_code=proc.returncode,
@@ -1904,17 +1898,23 @@
                 )
             raise QueryScriptRunError(
                 f"Query script exited with error code {proc.returncode}",
                 return_code=proc.returncode,
                 output=output,
             )
 
-        dataset: Optional["DatasetRecord"] = None
+        try:
+            response = json.loads(response_text)
+        except ValueError:
+            response = {}
+        exec_result = ExecutionResult(**response)
+
+        dataset: Optional[DatasetRecord] = None
         version: Optional[int] = None
-        if save:
+        if save or save_as:
             if not exec_result.dataset:
                 raise QueryScriptDatasetNotFound(
                     "No dataset found after running Query script",
                     output=output,
                 )
             name, version = exec_result.dataset
             # finding returning dataset
@@ -1928,14 +1928,20 @@
                 ) from e
 
             dataset = self.update_dataset(
                 dataset,
                 script_output=output,
                 query_script=query_script,
             )
+            self.update_dataset_version_with_warehouse_info(
+                dataset,
+                version,
+                script_output=output,
+                query_script=query_script,
+            )
 
         return QueryResult(
             dataset=dataset,
             version=version,
             output=output,
             preview=exec_result.preview,
         )
@@ -2106,15 +2112,14 @@
     def index(
         self,
         sources,
         ttl=TTL_INT,
         update=False,
         *,
         client_config=None,
-        index_processors: Optional[Union[list[IndexingFormat], IndexingFormat]] = None,
     ) -> None:
         root_sources = [
             src for src in sources if Client.get_implementation(src).is_root_url(src)
         ]
         non_root_sources = [
             src
             for src in sources
@@ -2127,22 +2132,17 @@
         # saving them as storages, without further indexing in each bucket
         for source in root_sources:
             for bucket in Client.get_implementation(source).ls_buckets(**client_config):
                 client = self.get_client(bucket.uri, **client_config)
                 print(f"Registering storage {client.uri}")
                 self.metastore.create_storage_if_not_registered(client.uri)
 
-        if index_processors and not isinstance(index_processors, list):
-            processors = [index_processors]
-        else:
-            processors = index_processors  # type: ignore[assignment]
         self.enlist_sources(
             non_root_sources,
             ttl,
             update,
             client_config=client_config,
-            index_processors=processors,
             only_index=True,
         )
 
     def find_stale_storages(self) -> None:
         self.metastore.find_stale_storages()
```

### Comparing `dvcx-0.79.0/src/dvcx/catalog/datasource.py` & `dvcx-0.80.0/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/catalog/loader.py` & `dvcx-0.80.0/src/dvcx/catalog/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/cli.py` & `dvcx-0.80.0/src/dvcx/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 import shlex
 import sys
 import traceback
 from argparse import SUPPRESS, Action, ArgumentParser, ArgumentTypeError, Namespace
-from collections.abc import Iterable, Iterator, Mapping
+from collections.abc import Iterable, Iterator, Mapping, Sequence
 from itertools import chain
 from multiprocessing import freeze_support
 from typing import TYPE_CHECKING, Optional, Union
 
 import shtab
 
 from dvcx import __version__, utils
@@ -62,14 +62,43 @@
         "sources",
         type=str,
         nargs=nargs,
         help="Data sources - paths to cloud storage dirs",
     )
 
 
+def add_show_args(parser: ArgumentParser) -> None:
+    parser.add_argument(
+        "--limit",
+        action="store",
+        default=10,
+        type=int,
+        help="Number of rows to show",
+    )
+    parser.add_argument(
+        "--offset",
+        action="store",
+        default=0,
+        type=int,
+        help="Number of rows to offset",
+    )
+    parser.add_argument(
+        "--columns",
+        default=[],
+        action=CommaSeparatedArgs,
+        help="Columns to show",
+    )
+    parser.add_argument(
+        "--no-collapse",
+        action="store_true",
+        default=False,
+        help="Do not collapse the columns",
+    )
+
+
 def get_parser() -> ArgumentParser:  # noqa: PLR0915
     parser = ArgumentParser(description="DVCx: Data Query Language", prog="dvcx")
 
     parser.add_argument("-V", "--version", action="version", version=__version__)
     parser.add_argument("--internal-run-udf", action="store_true", help=SUPPRESS)
     parser.add_argument("--internal-run-udf-worker", action="store_true", help=SUPPRESS)
 
@@ -433,78 +462,61 @@
             f"Options are: {','.join(FIND_COLUMNS)} (Default: path)"
         ),
     )
 
     parse_index = subp.add_parser(
         "index", parents=[parent_parser], help="Index storage location"
     )
-    parse_index.add_argument(
-        "--format",
-        type=str,
-        default=None,
-        choices=["tar-files", "json-pair", "webdataset"],
-        help="Postprocessing step to apply, after indexing storage.",
-    )
     add_sources_arg(parse_index)
-    add_storage_parser = subp.add_parser(
-        "add-storage", parents=[parent_parser], help="Register local path as storage"
-    )
-    add_storage_parser.add_argument("uri", type=str, help="Source URI or path")
 
     subp.add_parser(
         "find-stale-storages",
         parents=[parent_parser],
         help="Finds and marks stale storages",
     )
+
+    show_parser = subp.add_parser(
+        "show",
+        parents=[parent_parser],
+        help="Create a new dataset with a query script",
+    )
+    show_parser.add_argument("name", type=str, help="Dataset name")
+    show_parser.add_argument(
+        "--version",
+        action="store",
+        default=None,
+        type=int,
+        help="Dataset version",
+    )
+    add_show_args(show_parser)
+
     query_parser = subp.add_parser(
         "query",
         parents=[parent_parser],
         help="Create a new dataset with a query script",
     )
     query_parser.add_argument(
-        "script", metavar="<script>", type=str, help="Filepath for script"
+        "script", metavar="<script.py>", type=str, help="Filepath for script"
+    )
+    query_parser.add_argument(
+        "dataset_name", nargs="?", type=str, help="Save result dataset as"
     )
     query_parser.add_argument(
         "--parallel",
         nargs="?",
         type=int,
         const=-1,
         default=None,
         metavar="N",
         help=(
             "Use multiprocessing to run any query script UDFs with N worker processes. "
             "N defaults to the CPU count."
         ),
     )
-    query_parser.add_argument(
-        "--limit",
-        action="store",
-        default=10,
-        type=int,
-        help="Number of rows to show",
-    )
-    query_parser.add_argument(
-        "--offset",
-        action="store",
-        default=0,
-        type=int,
-        help="Number of rows to offset",
-    )
-    query_parser.add_argument(
-        "--columns",
-        default=[],
-        action=CommaSeparatedArgs,
-        help="Columns to show",
-    )
-    query_parser.add_argument(
-        "--no-collapse",
-        action="store_true",
-        default=False,
-        help="Do not collapse the columns",
-    )
+    add_show_args(query_parser)
     query_parser.add_argument(
         "-p",
         "--param",
         metavar="param=value",
         nargs=1,
         action=KeyValueArgs,
         help="Query parameters",
@@ -787,29 +799,47 @@
         else:
             print(f"{utils.sizeof_fmt(size, si=si): >7} {path}")
 
 
 def index(
     catalog: "Catalog",
     sources,
-    indexer_format: Optional[str] = None,
     **kwargs,
 ):
-    fmt = None
-    if indexer_format:
-        from .catalog import indexer_formats
+    catalog.index(sources, **kwargs)
+
+
+def show(
+    catalog: "Catalog",
+    name: str,
+    version: Optional[int] = None,
+    limit: int = 10,
+    offset: int = 0,
+    columns: Sequence[str] = (),
+    no_collapse: bool = False,
+) -> None:
+    from dvcx.query import DatasetQuery
+    from dvcx.utils import show_records
 
-        fmt = indexer_formats.get(indexer_format)
-    catalog.index(sources, index_processors=fmt, **kwargs)
+    if columns:
+        columns = ("id", *columns)
+    query = (
+        DatasetQuery(name=name, version=version, catalog=catalog)
+        .select(*columns)
+        .limit(limit)
+        .offset(offset)
+    )
+    records = query.to_records()
+    show_records(records, collapse_columns=not no_collapse)
 
 
 def query(
     catalog: "Catalog",
     script: str,
-    dataset_name: str,
+    dataset_name: Optional[str] = None,
     parallel: Optional[int] = None,
     limit: int = 10,
     offset: int = 0,
     columns: Optional[list[str]] = None,
     no_collapse: bool = False,
     params: Optional[dict[str, str]] = None,
 ) -> None:
@@ -820,14 +850,15 @@
 
     if parallel is not None:
         # This also sets this environment variable for any subprocesses
         os.environ["DVCX_SETTINGS_PARALLEL"] = str(parallel)
 
     result = catalog.query(
         script_content,
+        save_as=dataset_name,
         preview_limit=limit,
         preview_offset=offset,
         preview_columns=columns,
         capture_output=False,
         params=params,
     )
     show_records(result.preview, collapse_columns=not no_collapse)
@@ -949,14 +980,24 @@
                 update=bool(args.update),
                 client_config=client_config,
             )
         elif args.command == "ls-datasets":
             ls_datasets(catalog)
         elif args.command == "ls-dataset-rows":
             ls_dataset_rows(catalog, args.name, args.version)
+        elif args.command == "show":
+            show(
+                catalog,
+                args.name,
+                args.version,
+                limit=args.limit,
+                offset=args.offset,
+                columns=args.columns,
+                no_collapse=args.no_collapse,
+            )
         elif args.command == "rm-dataset":
             rm_dataset(catalog, args.name, version=args.version, force=args.force)
         elif args.command == "dataset-stats":
             dataset_stats(
                 catalog,
                 args.name,
                 args.version,
@@ -993,28 +1034,26 @@
             if not results_found:
                 print("No results")
         elif args.command == "index":
             index(
                 catalog,
                 args.sources,
                 ttl=args.ttl,
-                indexer_format=args.format,
                 update=bool(args.update),
             )
-        elif args.command == "add-storage":
-            catalog.add_storage(args.uri)
         elif args.command == "completion":
             print(completion(args.shell))
         elif args.command == "find-stale-storages":
             catalog.find_stale_storages()
         elif args.command == "query":
             query(
                 catalog,
                 args.script,
-                args.parallel,
+                dataset_name=args.dataset_name,
+                parallel=args.parallel,
                 limit=args.limit,
                 offset=args.offset,
                 columns=args.columns,
                 no_collapse=args.no_collapse,
                 params=args.param,
             )
         elif args.command == "apply-udf":
```

### Comparing `dvcx-0.79.0/src/dvcx/cli_utils.py` & `dvcx-0.80.0/src/dvcx/cli_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/client/azure.py` & `dvcx-0.80.0/src/dvcx/client/azure.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/client/fileslice.py` & `dvcx-0.80.0/src/dvcx/client/fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/client/fsspec.py` & `dvcx-0.80.0/src/dvcx/client/fsspec.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     def parse_url(
         source: str,
         metastore: "AbstractMetastore",
         cache: DVCXCache,
         **kwargs,
     ) -> tuple["Client", str]:
         cls = Client.get_implementation(source)
-        storage_url, rel_path = cls.split_url(source, metastore)
+        storage_url, rel_path = cls.split_url(source)
         client = cls.from_name(storage_url, metastore, cache, kwargs)
         return client, rel_path
 
     @classmethod
     def create_fs(cls, **kwargs) -> "AbstractFileSystem":
         kwargs.setdefault("version_aware", True)
         fs = cls.FS_CLASS(**kwargs)
@@ -131,15 +131,15 @@
         return url == cls.PREFIX
 
     @property
     def uri(self) -> StorageURI:
         return StorageURI(f"{self.PREFIX}{self.name}")
 
     @classmethod
-    def split_url(cls, url: str, metastore: "AbstractMetastore") -> tuple[str, str]:
+    def split_url(cls, url: str) -> tuple[str, str]:
         fill_path = url[len(cls.PREFIX) :]
         path_split = fill_path.split("/", 1)
         bucket = path_split[0]
         path = path_split[1] if len(path_split) > 1 else ""
         return bucket, path
 
     def url(self, path: str, expires: int = 3600, **kwargs) -> str:
```

### Comparing `dvcx-0.79.0/src/dvcx/client/gcs.py` & `dvcx-0.80.0/src/dvcx/client/gcs.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/client/local.py` & `dvcx-0.80.0/src/dvcx/client/local.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import posixpath
 from datetime import datetime, timezone
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 from fsspec.implementations.local import LocalFileSystem
 
-from dvcx.error import StorageNotFoundError
 from dvcx.node import Entry
 from dvcx.storage import StorageURI
 
 from .fsspec import Client
 
 if TYPE_CHECKING:
     from dvcx.data_storage import AbstractMetastore
@@ -26,36 +25,56 @@
     ) -> None:
         super().__init__(name, fs, cache)
         self.use_symlinks = use_symlinks
 
     def url(self, path: str, expires: int = 3600, **kwargs) -> str:
         raise TypeError("Signed urls are not implemented for local file system")
 
+    @property
+    def uri(self) -> StorageURI:
+        """
+        This returns root of FS as uri, e.g
+            Linux & Mac : file:///
+            Windows: file:///C:/
+        """
+        return StorageURI(Path(self.name).as_uri())
+
+    @staticmethod
+    def root_dir() -> str:
+        """
+        Returns file system root path.
+        Linux &  MacOS: /
+        Windows: C:/
+        """
+        return Path.cwd().anchor.replace(os.sep, posixpath.sep)
+
+    @staticmethod
+    def root_path() -> Path:
+        return Path(FileClient.root_dir())
+
     @classmethod
     def ls_buckets(cls, **kwargs):
         return []
 
     @classmethod
-    def split_url(cls, url: str, metastore: "AbstractMetastore") -> tuple[str, str]:
-        def _storage_exists(uri: str) -> bool:
-            try:
-                metastore.get_storage(StorageURI(uri))
-            except StorageNotFoundError:
-                return False
-            return True
-
-        # lowercasing scheme just in case it's uppercase
+    def split_url(cls, url: str) -> tuple[str, str]:
+        """
+        Splits url into two components:
+            1. root of the FS which will later on become the name of the storage
+            2. path which will later on become partial path
+        Note that URL needs to be have file:/// protocol.
+        Examples:
+            file:///tmp/dir -> / + tmp/dir
+            file:///c:/windows/files -> c:/ + windows/files
+        """
+        # scheme / protocol is case insensitive
         scheme, rest = url.split(":", 1)
         url = f"{scheme.lower()}:{rest}"
-        if _storage_exists(url):
-            return LocalFileSystem._strip_protocol(url), ""
-        for pos in range(len(url) - 1, len(cls.PREFIX), -1):
-            if url[pos] == "/" and _storage_exists(url[:pos]):
-                return LocalFileSystem._strip_protocol(url[:pos]), url[pos + 1 :]
-        raise RuntimeError(f"Invalid file path '{url}'")
+
+        return cls.root_dir(), url.removeprefix(cls.root_path().as_uri())
 
     @classmethod
     def from_name(
         cls, name: str, metastore: "AbstractMetastore", cache, kwargs
     ) -> "FileClient":
         use_symlinks = kwargs.pop("use_symlinks", False)
         return cls(name, cls.create_fs(**kwargs), cache, use_symlinks=use_symlinks)
@@ -88,18 +107,14 @@
 
     async def ls_dir(self, path):
         return self.fs.ls(path, detail=True)
 
     def rel_path(self, path):
         return posixpath.relpath(path, self.name)
 
-    @property
-    def uri(self):
-        return Path(self.name).as_uri()
-
     def get_full_path(self, rel_path):
         full_path = Path(self.name, rel_path).as_uri()
         if rel_path.endswith("/") or not rel_path:
             full_path += "/"
         return full_path
 
     def convert_info(self, v: dict[str, Any], parent: str) -> Entry:
```

### Comparing `dvcx-0.79.0/src/dvcx/client/s3.py` & `dvcx-0.80.0/src/dvcx/client/s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/config.py` & `dvcx-0.80.0/src/dvcx/config.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/data_storage/db_engine.py` & `dvcx-0.80.0/src/dvcx/data_storage/db_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/data_storage/id_generator.py` & `dvcx-0.80.0/src/dvcx/data_storage/id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/data_storage/metastore.py` & `dvcx-0.80.0/src/dvcx/data_storage/metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/data_storage/schema.py` & `dvcx-0.80.0/src/dvcx/data_storage/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -373,28 +373,7 @@
     dataset_row_cls: type[DatasetRowT]
 
 
 class DefaultSchema(Schema[Node, DatasetRow]):
     def __init__(self):
         self.node_cls = Node
         self.dataset_row_cls = DatasetRow
-
-
-class SignalsTable(Table):
-    """A table for storing signals and annotations."""
-
-    def __init__(
-        self, name: str, cols: list[sa.Column], metadata: Optional["sa.MetaData"] = None
-    ):
-        self.cols = cols
-        super().__init__(name, metadata=metadata)
-
-    def get_table(self) -> "sa.Table":
-        table = self.metadata.tables.get(self.name)
-        if table is None:
-            return sa.Table(
-                self.name,
-                self.metadata,
-                sa.Column("id", sa.Integer, primary_key=True),
-                *self.cols,
-            )
-        return table
```

### Comparing `dvcx-0.79.0/src/dvcx/data_storage/serializer.py` & `dvcx-0.80.0/src/dvcx/data_storage/serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/data_storage/sqlite.py` & `dvcx-0.80.0/src/dvcx/data_storage/sqlite.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,32 +24,29 @@
 
 import dvcx.sql.sqlite
 from dvcx.data_storage import AbstractDBMetastore, AbstractWarehouse
 from dvcx.data_storage.db_engine import DatabaseEngine
 from dvcx.data_storage.id_generator import AbstractDBIDGenerator
 from dvcx.data_storage.schema import (
     DefaultSchema,
-    SignalsTable,
     convert_rows_custom_column_types,
 )
 from dvcx.dataset import DatasetRecord
-from dvcx.error import DVCXError, InconsistentSignalType
+from dvcx.error import DVCXError
 from dvcx.node import Entry
 from dvcx.sql.sqlite import create_user_defined_sql_functions, sqlite_dialect
 from dvcx.sql.types import SQLType
 from dvcx.storage import StorageURI
 from dvcx.utils import DVCXDir
 
 if TYPE_CHECKING:
     from sqlalchemy.schema import SchemaItem
     from sqlalchemy.sql.elements import ColumnClause, ColumnElement, TextClause
     from sqlalchemy.types import TypeEngine
 
-    from dvcx.data_storage import schema
-
 
 logger = logging.getLogger("dvcx")
 
 RETRY_START_SEC = 0.01
 RETRY_MAX_TIMES = 10
 RETRY_FACTOR = 2
 
@@ -730,123 +727,20 @@
                 self._col_python_type[col_type_cls] = col_type.type_engine(
                     sqlite_dialect
                 )
             col_type = self._col_python_type[col_type_cls]
 
         return col_type.python_type
 
-    def add_column(
-        self, table: Table, col_name: str, col_type: Union["TypeEngine", "SQLType"]
-    ):
-        """Adds a column to a table"""
-        # trying to find the same column in a table
-        table_col = table.c.get(col_name, None)
-
-        if isinstance(col_type, SQLType):
-            # converting our defined column types to dialect specific TypeEngine
-            col_type = col_type.type_engine(sqlite_dialect)
-
-        if table_col is not None and table_col.type.python_type != col_type.python_type:
-            raise InconsistentSignalType(
-                f"Column {col_name} already exists with a type:"
-                f" {table_col.type.python_type}"
-                f", but trying to create it with different type: {col_type.python_type}"
-            )
-        if table_col is not None:
-            # column with the same name and type already exist, nothing to do
-            return
-
-        table_name = quote_schema(table.name)
-        col_name_comp = quote(col_name)
-        col_type_comp = col_type.compile(dialect=sqlite_dialect)
-        q = f"ALTER TABLE {table_name} ADD COLUMN {col_name_comp} {col_type_comp}"
-        self.db.execute_str(q)
-
-        # reload the table to self.ddb.metadata so the table object
-        # self.ddb.metadata.tables[table.name] includes the new column
-        self._reflect_tables(filter_tables=lambda t, _: t == table.name)
-
     def dataset_table_export_file_names(
         self, dataset: DatasetRecord, version: int
     ) -> list[str]:
         raise NotImplementedError("Exporting dataset table not implemented for SQLite")
 
     def export_dataset_table(
         self,
         bucket_uri: str,
         dataset: DatasetRecord,
         version: int,
         client_config=None,
     ) -> list[str]:
         raise NotImplementedError("Exporting dataset table not implemented for SQLite")
-
-    #
-    # Signals
-    #
-
-    def create_signals_table(self) -> SignalsTable:
-        """
-        Create an empty signals table for storing signals entries.
-        """
-        tbl_name = self.signals_table_name(self.uri)
-        tbl = SignalsTable(tbl_name, [], self.db.metadata)
-        self.db.create_table(tbl.table, if_not_exists=True)
-        return tbl
-
-    def extend_index_with_signals(self, index: "schema.Table", signals: SignalsTable):
-        """
-        Extend a nodes table with a signals table.
-        This will result in the original index table being replaced
-        with a table that is a join between the signals table and the
-        index table (joining on the id column).
-        """
-
-        with self.db.transaction():
-            # Create temporary table.
-            join_tbl_name = self.TMP_TABLE_NAME_PREFIX + index.name
-
-            signal_columns = [c for c in signals.table.c if c.name != "id"]
-
-            join_tbl = self.schema.node_cls.new_table(
-                join_tbl_name,
-                [self.schema.node_cls.copy_signal_column(c) for c in signal_columns],
-                self.db.metadata,
-            )
-            try:
-                self.db.create_table(join_tbl, if_not_exists=True)
-
-                # Query joining original index table and signals table.
-                index_cols = {c.name for c in index.table.c}
-                duplicate_signal_cols = {
-                    c.name
-                    for c in signals.table.c
-                    if c.name in index_cols and c.name != "id"
-                }
-                select_cols = [
-                    # columns from index table
-                    *(c for c in index.table.c if c.name not in duplicate_signal_cols),
-                    # coalesce columns already in index table
-                    *(
-                        func.coalesce(*cc).label(cc[0].name)
-                        for cc in zip(
-                            [index.table.c[col] for col in duplicate_signal_cols],
-                            [signals.table.c[col] for col in duplicate_signal_cols],
-                        )
-                    ),
-                    # columns from signals table
-                    *(c for c in signal_columns if c.name not in duplicate_signal_cols),
-                ]
-                q = sqlalchemy.select(*select_cols).select_from(
-                    index.table.outerjoin(
-                        signals.table, index.c.id == signals.table.c.id
-                    )
-                )
-
-                cols = [c.name for c in select_cols]
-
-                # Write results of query to the new index table.
-                self.db.execute(sqlalchemy.insert(join_tbl).from_select(cols, q))
-                # Replace original table with extended one.
-                self.db.drop_table(index.table)
-                self.db.rename_table(join_tbl_name, index.name)
-            finally:
-                self.db.drop_table(join_tbl, if_exists=True)
```

### Comparing `dvcx-0.79.0/src/dvcx/data_storage/warehouse.py` & `dvcx-0.80.0/src/dvcx/data_storage/warehouse.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 
 import attrs
 import sqlalchemy as sa
 from sqlalchemy import Table, and_, case, select
 from sqlalchemy.sql import func
 from sqlalchemy.sql.expression import true
 
-from dvcx.data_storage.schema import DATASET_CORE_COLUMN_NAMES, SignalsTable
-from dvcx.data_storage.schema import Node as NodeTable
+from dvcx.data_storage.schema import DATASET_CORE_COLUMN_NAMES
 from dvcx.data_storage.serializer import Serializable
 from dvcx.dataset import DatasetRecord, DatasetRow
 from dvcx.node import DirTypeGroup, Entry, Node, NodeWithPath, get_path
 from dvcx.sql.types import Int, SQLType
 from dvcx.storage import StorageURI
 from dvcx.utils import GLOB_CHARS, sql_escape_like
 
@@ -59,15 +58,14 @@
 
     #
     # Constants, Initialization, and Tables
     #
 
     BUCKET_TABLE_NAME_PREFIX = "src_"
     DATASET_TABLE_PREFIX = "ds_"
-    SIGNALS_TABLE_PREFIX = "sg_"
     UDF_TABLE_NAME_PREFIX = "udf_"
     TMP_TABLE_NAME_PREFIX = "tmp_"
 
     id_generator: "AbstractIDGenerator"
     schema: "schema.Schema"
     db: "DatabaseEngine"
 
@@ -153,15 +151,15 @@
         """Initializes database tables for warehouse"""
 
     #
     # Query Tables
     #
 
     @abstractmethod
-    def is_ready(self, timeout: Optional[int]) -> bool: ...
+    def is_ready(self, timeout: Optional[int] = None) -> bool: ...
 
     @property
     def nodes(self):
         assert (
             self.current_bucket_table_name
         ), "Nodes can only be used if uri/current_bucket_table_name is set"
         if self._nodes is None:
@@ -265,18 +263,14 @@
         name = parsed.path if parsed.scheme == "file" else parsed.netloc
         return parsed.scheme, name
 
     def bucket_table_name(self, uri: str, version: int) -> str:
         scheme, name = self.uri_to_storage_info(uri)
         return f"{self.BUCKET_TABLE_NAME_PREFIX}{scheme}_{name}_{version}"
 
-    def signals_table_name(self, uri: str, version: int = 0) -> str:
-        parsed = urlparse(uri)
-        return f"{self.SIGNALS_TABLE_PREFIX}{parsed.scheme}_{parsed.netloc}_{version}"
-
     def dataset_table_name(self, dataset_name: str, version: int) -> str:
         return f"{self.DATASET_TABLE_PREFIX}{dataset_name}_{version}"
 
     @property
     def current_bucket_table_name(self) -> Optional[str]:
         if not self.uri:
             return None
@@ -506,18 +500,14 @@
     def get_table(self, name: str) -> sa.Table:
         """
         Returns a SQLAlchemy Table object by name. If table doesn't exist, it should
         create it
         """
 
     @abstractmethod
-    def add_column(self, table: Table, col_name: str, col_type: "TypeEngine") -> None:
-        """Adds a column with a name and type to a table"""
-
-    @abstractmethod
     def dataset_table_export_file_names(
         self, dataset: DatasetRecord, version: int
     ) -> list[str]:
         """
         Returns list of file names that will be created when user runs dataset export
         """
 
@@ -870,21 +860,14 @@
             n.select(*(getattr(n.c, f) for f in fields)),
             type,
             conds,
             order_by=order_by,
         )
         return self.db.execute(query)
 
-    def update_type(self, node_id: int, dir_type: int) -> None:
-        """Updates type of specific node in database"""
-        n = self.nodes
-        self.db.execute(
-            self.nodes.update().where(n.c.id == node_id).values(dir_type=dir_type)  # type: ignore [attr-defined]
-        )
-
     def update_node(self, node_id: int, values: dict[str, Any]) -> None:
         """Update entry of a specific node in the database."""
         n = self.nodes
         self.db.execute(self.nodes.update().values(**values).where(n.c.id == node_id))
 
     def storage_stats(
         self, uri: StorageURI, partial_id: Optional[int]
@@ -942,30 +925,14 @@
         ensure that they are cleaned up as soon as they are no longer
         needed. When running the same `DatasetQuery` multiple times we
         may use the same temporary table names.
         """
         for name in names:
             self.db.drop_table(Table(name, self.db.metadata), if_exists=True)
 
-    #
-    # Signals
-    #
-
-    @abstractmethod
-    def create_signals_table(self) -> SignalsTable:
-        """
-        Create an empty signals table for storing signals entries.
-        Signals columns will be added gradually as they are encountered during
-        data traversal
-        """
-
-    @abstractmethod
-    def extend_index_with_signals(self, index: NodeTable, signals: SignalsTable):
-        """Extend a nodes table with a signals table."""
-
     def subtract_query(
         self,
         source_query: sa.sql.selectable.Select,
         target_query: sa.sql.selectable.Select,
     ) -> sa.sql.selectable.Select:
         sq = source_query.alias("source_query")
         tq = target_query.alias("target_query")
```

### Comparing `dvcx-0.79.0/src/dvcx/dataset.py` & `dvcx-0.80.0/src/dvcx/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/error.py` & `dvcx-0.80.0/src/dvcx/error.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,13 +53,9 @@
 class ClientError(RuntimeError):
     def __init__(self, message, error_code=None):
         super().__init__(message)
         # error code from the cloud itself
         self.error_code = error_code
 
 
-class InconsistentSignalType(Exception):  # noqa: N818
-    pass
-
-
 class TableMissingError(DVCXError):
     pass
```

### Comparing `dvcx-0.79.0/src/dvcx/lib/cached_stream.py` & `dvcx-0.80.0/src/dvcx/lib/cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/claude.py` & `dvcx-0.80.0/src/dvcx/lib/claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/dataset.py` & `dvcx-0.80.0/src/dvcx/lib/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,26 +38,14 @@
 
     Each row in the DataFrame acts as a reference to a file (or specific elements within
     a file) and is associated with various file parameters, represented as columns.
     These columns typically include labels, embeddings, or auto-generated labels,
     providing a comprehensive view of the file's attributes.
     """
 
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def save(
-        self, name: Optional[str] = None, version: Optional[int] = None, **kwargs
-    ) -> "Dataset":
-        """Save and return a Dataset instead of a DatasetQuery."""
-        ds = super().save(name=name, version=version, **kwargs)
-        self.name = ds.name
-        self.version = ds.version
-        return self
-
     def apply(self, func, *args, **kwargs):
         return func(self, *args, **kwargs)
 
     def map(
         self,
         udf: Union[Callable, UDFBase],
         params=None,
```

### Comparing `dvcx-0.79.0/src/dvcx/lib/feature.py` & `dvcx-0.80.0/src/dvcx/lib/feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/feature_types.py` & `dvcx-0.80.0/src/dvcx/lib/feature_types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/feature_udf.py` & `dvcx-0.80.0/src/dvcx/lib/feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/file.py` & `dvcx-0.80.0/src/dvcx/lib/file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.80.0/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.80.0/src/dvcx/lib/hf_image_to_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.80.0/src/dvcx/lib/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/image.py` & `dvcx-0.80.0/src/dvcx/lib/image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/image_transform.py` & `dvcx-0.80.0/src/dvcx/lib/image_transform.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.80.0/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/pytorch.py` & `dvcx-0.80.0/src/dvcx/lib/pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/reader.py` & `dvcx-0.80.0/src/dvcx/lib/reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/tar_file.py` & `dvcx-0.80.0/src/dvcx/lib/tar_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/text.py` & `dvcx-0.80.0/src/dvcx/lib/text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/udf.py` & `dvcx-0.80.0/src/dvcx/lib/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/unstructured.py` & `dvcx-0.80.0/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/utils.py` & `dvcx-0.80.0/src/dvcx/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/webdataset.py` & `dvcx-0.80.0/src/dvcx/lib/webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/webdataset_laion.py` & `dvcx-0.80.0/src/dvcx/lib/webdataset_laion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.80.0/src/dvcx/lib/webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/listing.py` & `dvcx-0.80.0/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/node.py` & `dvcx-0.80.0/src/dvcx/node.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/nodes_fetcher.py` & `dvcx-0.80.0/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/nodes_thread_pool.py` & `dvcx-0.80.0/src/dvcx/nodes_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/progress.py` & `dvcx-0.80.0/src/dvcx/progress.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/query/batch.py` & `dvcx-0.80.0/src/dvcx/query/batch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/query/builtins.py` & `dvcx-0.80.0/src/dvcx/query/builtins.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/query/dataset.py` & `dvcx-0.80.0/src/dvcx/query/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import contextlib
+import datetime
 import inspect
 import json
 import logging
 import os
 import random
 import re
 import string
@@ -47,15 +48,15 @@
 )
 from dvcx.dataset import DatasetRow
 from dvcx.dataset import Status as DatasetStatus
 from dvcx.error import DatasetNotFoundError, QueryScriptCancelError
 from dvcx.sql.functions import rand
 from dvcx.sql.types import SQLType
 from dvcx.storage import StorageURI
-from dvcx.utils import JSONSerialize, chunk, determine_processes
+from dvcx.utils import chunk, determine_processes
 
 from .batch import DatasetRowsBatch
 from .schema import C, UDFParamSpec, normalize_param
 from .session import Session
 from .udf import UDFBase, UDFClassWrapper, UDFFactory, UDFType
 
 if TYPE_CHECKING:
@@ -1608,15 +1609,15 @@
                     version,
                     storage.uri,
                     storage.timestamp_str,
                 )
 
     def save(
         self, name: Optional[str] = None, version: Optional[int] = None, **kwargs
-    ) -> "DatasetQuery":
+    ) -> "Self":
         """Save the query as a dataset."""
         try:
             if name and version and self.catalog.get_dataset(name).has_version(version):
                 raise RuntimeError(f"Dataset {name} already has version {version}")
         except DatasetNotFoundError:
             pass
         if not name and version:
@@ -1681,16 +1682,15 @@
                 dataset, DatasetStatus.COMPLETE, version=version
             )
             self.catalog.update_dataset_version_with_warehouse_info(dataset, version)
 
             self._add_dependencies(dataset, version)  # type: ignore [arg-type]
         finally:
             self.cleanup()
-
-        return DatasetQuery(name=name, version=version, catalog=self.catalog)
+        return self.__class__(name=name, version=version, catalog=self.catalog)
 
 
 def _get_output_fd_for_write() -> Union[str, int]:
     handle = os.getenv("DVCX_OUTPUT_FD")
     if not handle:
         return os.devnull
 
@@ -1704,17 +1704,23 @@
 
 @attrs.define
 class ExecutionResult:
     preview: list[dict] = attrs.field(factory=list)
     dataset: Optional[tuple[str, int]] = None
 
 
-def _send_result(
-    dataset_query: DatasetQuery, dataset: Optional[tuple[str, int]] = None
-):
+def _send_result(dataset_query: DatasetQuery) -> None:
+    class JSONSerialize(json.JSONEncoder):
+        def default(self, obj):
+            if isinstance(obj, (datetime.datetime, datetime.date)):
+                return obj.isoformat()
+            if isinstance(obj, bytes):
+                return [f"{b:02x}" for b in obj[:1024]]
+            return super().default(obj)
+
     try:
         preview_args: dict[str, Any] = json.loads(
             os.getenv("DVCX_QUERY_PREVIEW_ARGS", "")
         )
     except ValueError:
         preview_args = {}
 
@@ -1724,14 +1730,20 @@
 
     preview_query = (
         dataset_query.select(*columns)
         .limit(preview_args.get("limit", 10))
         .offset(preview_args.get("offset", 0))
     )
 
+    dataset: Optional[tuple[str, int]] = None
+    if dataset_query.attached:
+        assert dataset_query.name, "Dataset name should be provided"
+        assert dataset_query.version, "Dataset version should be provided"
+        dataset = dataset_query.name, dataset_query.version
+
     preview = preview_query.to_records()
     result = ExecutionResult(preview, dataset)
     data = attrs.asdict(result)
 
     with open(_get_output_fd_for_write(), mode="w") as f:
         json.dump(data, f, cls=JSONSerialize)
 
@@ -1741,28 +1753,49 @@
     Wrapper function that wraps the last statement of user query script.
     Last statement MUST be instance of DatasetQuery, otherwise script exits with
     error code 10
     """
     if not isinstance(dataset_query, DatasetQuery):
         sys.exit(QUERY_SCRIPT_INVALID_LAST_STATEMENT_EXIT_CODE)
 
+    catalog = dataset_query.catalog
     save = bool(os.getenv("DVCX_QUERY_SAVE"))
-    dataset: Optional[tuple[str, int]] = None
-    if dataset_query.attached:
-        name = dataset_query.name
-        version = dataset_query.version
-        assert name
-        assert version
-        dataset = name, version
-    elif save:
-        name = dataset_query.catalog.generate_query_dataset_name()
-        dataset_query.save(name)
-        version = 1
-        dataset = name, version
-    _send_result(dataset_query, dataset=dataset)
+    save_as = os.getenv("DVCX_QUERY_SAVE_AS")
+
+    if save_as:
+        if dataset_query.attached:
+            dataset_name = dataset_query.name
+            version = dataset_query.version
+            assert dataset_name, "Dataset name should be provided in attached mode"
+            assert version, "Dataset version should be provided in attached mode"
+
+            dataset = catalog.get_dataset(dataset_name)
+
+            try:
+                target_dataset = catalog.get_dataset(save_as)
+            except DatasetNotFoundError:
+                target_dataset = None
+
+            if target_dataset:
+                dataset = catalog.register_dataset(dataset, version, target_dataset)
+            else:
+                dataset = catalog.register_new_dataset(dataset, version, save_as)
+
+            dataset_query = DatasetQuery(
+                name=dataset.name,
+                version=dataset.latest_version,
+                catalog=catalog,
+            )
+        else:
+            dataset_query = dataset_query.save(save_as)
+    elif save and not dataset_query.attached:
+        name = catalog.generate_query_dataset_name()
+        dataset_query = dataset_query.save(name)
+
+    _send_result(dataset_query)
     return dataset_query
 
 
 def _random_string(length: int) -> str:
     return "".join(
         random.choice(string.ascii_letters + string.digits)  # noqa: S311
         for i in range(length)
```

### Comparing `dvcx-0.79.0/src/dvcx/query/dispatch.py` & `dvcx-0.80.0/src/dvcx/query/dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/query/params.py` & `dvcx-0.80.0/src/dvcx/query/params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/query/schema.py` & `dvcx-0.80.0/src/dvcx/query/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/query/session.py` & `dvcx-0.80.0/src/dvcx/query/session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/query/udf.py` & `dvcx-0.80.0/src/dvcx/query/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/remote/studio.py` & `dvcx-0.80.0/src/dvcx/remote/studio.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/sql/default/base.py` & `dvcx-0.80.0/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/sql/functions/array.py` & `dvcx-0.80.0/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/sql/functions/path.py` & `dvcx-0.80.0/src/dvcx/sql/functions/path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/sql/selectable.py` & `dvcx-0.80.0/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/sql/sqlite/base.py` & `dvcx-0.80.0/src/dvcx/sql/sqlite/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/sql/sqlite/types.py` & `dvcx-0.80.0/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/sql/types.py` & `dvcx-0.80.0/src/dvcx/sql/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/sql/utils.py` & `dvcx-0.80.0/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/storage.py` & `dvcx-0.80.0/src/dvcx/storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx/utils.py` & `dvcx-0.80.0/src/dvcx/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.80.0/src/dvcx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.79.0
+Version: 0.80.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.79.0/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.80.0/src/dvcx.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,14 @@
 src/dvcx.egg-info/dependency_links.txt
 src/dvcx.egg-info/entry_points.txt
 src/dvcx.egg-info/requires.txt
 src/dvcx.egg-info/top_level.txt
 src/dvcx/catalog/__init__.py
 src/dvcx/catalog/catalog.py
 src/dvcx/catalog/datasource.py
-src/dvcx/catalog/formats.py
 src/dvcx/catalog/loader.py
 src/dvcx/client/__init__.py
 src/dvcx/client/azure.py
 src/dvcx/client/fileslice.py
 src/dvcx/client/fsspec.py
 src/dvcx/client/gcs.py
 src/dvcx/client/local.py
@@ -174,15 +173,14 @@
 tests/func/test_query.py
 tests/scripts/name_len_normal.py
 tests/scripts/name_len_slow.py
 tests/unit/__init__.py
 tests/unit/test_asyn.py
 tests/unit/test_cache.py
 tests/unit/test_catalog.py
-tests/unit/test_catalog_formats.py
 tests/unit/test_catalog_loader.py
 tests/unit/test_cli_parsing.py
 tests/unit/test_client.py
 tests/unit/test_client_s3.py
 tests/unit/test_data_storage.py
 tests/unit/test_database_engine.py
 tests/unit/test_dataset.py
```

### Comparing `dvcx-0.79.0/src/dvcx.egg-info/requires.txt` & `dvcx-0.80.0/src/dvcx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/benchmarks/conftest.py` & `dvcx-0.80.0/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/conftest.py` & `dvcx-0.80.0/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import pytest_servers.exceptions
 import sqlalchemy
 from pytest import MonkeyPatch, TempPathFactory
 from upath.implementations.cloud import CloudPath
 
 from dvcx.catalog import Catalog
 from dvcx.catalog.loader import get_id_generator, get_metastore, get_warehouse
+from dvcx.client.local import FileClient
 from dvcx.data_storage.sqlite import (
     SQLiteDatabaseEngine,
     SQLiteIDGenerator,
     SQLiteMetastore,
     SQLiteWarehouse,
 )
 from dvcx.dataset import DatasetRecord, DatasetRow
@@ -322,14 +323,27 @@
         return self.server.src
 
     @property
     def src_uri(self):
         return self.server.src_uri
 
     @property
+    def storage_uri(self):
+        if self.server.kind == "file":
+            return FileClient.root_path().as_uri()
+        return self.server.src_uri
+
+    @property
+    def partial_path(self):
+        if self.server.kind == "file":
+            _, rel_path = FileClient.split_url(self.src_uri)
+            return rel_path
+        return ""
+
+    @property
     def client_config(self):
         return self.server.client_config
 
 
 @pytest.fixture(scope="session", params=["file", "s3", "gcs", "azure"])
 def cloud_type(request):
     return request.param
@@ -399,20 +413,15 @@
         id_generator=id_generator,
         metastore=metastore,
         warehouse=warehouse,
         cache_dir=str(cache_dir),
         tmp_dir=str(tmpfile_dir),
         client_config=cloud_server.client_config,
     )
-    result = CloudTestCatalog(
-        server=cloud_server, working_dir=tmp_path, catalog=catalog
-    )
-    if cloud_server.kind == "file":
-        catalog.add_storage(f"{result.src_uri}")
-    return result
+    return CloudTestCatalog(server=cloud_server, working_dir=tmp_path, catalog=catalog)
 
 
 @pytest.fixture
 def cloud_test_catalog(
     cloud_server,
     cloud_server_credentials,
     tmp_path,
```

### Comparing `dvcx-0.79.0/tests/data.py` & `dvcx-0.80.0/tests/data.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/func/test_catalog.py` & `dvcx-0.80.0/tests/func/test_catalog.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,30 +4,29 @@
 from contextlib import suppress
 from pathlib import Path
 from textwrap import dedent
 from urllib.parse import urlparse
 
 import pytest
 import yaml
-from fsspec.implementations.local import LocalFileSystem
 
-from dvcx.catalog import indexer_formats, parse_edvcx_file
+from dvcx.catalog import parse_edvcx_file
 from dvcx.cli import garbage_collect
 from dvcx.error import (
     QueryScriptCompileError,
     QueryScriptDatasetNotFound,
     QueryScriptRunError,
     StorageNotFoundError,
 )
 from tests.data import ENTRIES
 from tests.utils import (
     DEFAULT_TREE,
     TARRED_TREE,
-    WEBFORMAT_TREE,
     assert_row_names,
+    create_tar_dataset,
     make_index,
     skip_if_not_sqlite,
     tree_from_path,
 )
 
 
 @pytest.fixture
@@ -168,25 +167,27 @@
         (True, True, False),
         (True, False, False),
         (True, False, True),
         (False, True, False),
         (False, False, False),
     ),
 )
-def test_cp_root(cloud_test_catalog, recursive, star, dir_exists):
+def test_cp_root(cloud_test_catalog, recursive, star, dir_exists, cloud_type):
     src_uri = cloud_test_catalog.src_uri
     working_dir = cloud_test_catalog.working_dir
     catalog = cloud_test_catalog.catalog
 
     dest = working_dir / "data"
 
     if star:
         src_path = f"{src_uri}/*"
     else:
         src_path = src_uri
+        if cloud_type == "file":
+            src_path += "/"
 
     if star:
         with pytest.raises(FileNotFoundError):
             catalog.cp([src_path], str(dest), recursive=recursive)
 
     if dir_exists or star:
         dest.mkdir()
@@ -213,15 +214,17 @@
     # Directories should never be saved
     assert "cats" not in files_by_name
     assert "dogs" not in files_by_name
     assert "others" not in files_by_name
     assert "dogs/others" not in files_by_name
 
     # Description is always copied (if anything is copied)
-    prefix = "" if star or (recursive and not dir_exists) else "/"
+    prefix = (
+        "" if star or (recursive and not dir_exists) or cloud_type == "file" else "/"
+    )
     assert files_by_name[f"{prefix}description"]["size"] == 13
 
     if recursive:
         assert tree_from_path(dest) == DEFAULT_TREE
         assert files_by_name[f"{prefix}cats/cat1"]["size"] == 4
         assert files_by_name[f"{prefix}cats/cat2"]["size"] == 4
         assert files_by_name[f"{prefix}dogs/dog1"]["size"] == 4
@@ -272,22 +275,23 @@
     }
 
 
 @pytest.mark.parametrize("tree", [TARRED_TREE], indirect=True)
 @pytest.mark.parametrize("suffix", ["/", "/*"])
 @pytest.mark.parametrize("recursive", [False, True])
 @pytest.mark.parametrize("dir_exists", [False, True])
+@pytest.mark.xfail(reason="Missing support for v-objects in cp")
 def test_cp_tar_root(cloud_test_catalog, suffix, recursive, dir_exists):
     ctc = cloud_test_catalog
     catalog = ctc.catalog
-    catalog.index([ctc.src_uri], index_processors=indexer_formats["tar-files"])
+    create_tar_dataset(catalog, ctc.src_uri, "tarred")
     dest = ctc.working_dir / "data"
     if dir_exists:
         dest.mkdir()
-    src = f"{ctc.src_uri}/animals.tar{suffix}"
+    src = f"ds://tarred/animals.tar{suffix}"
     dest_path = str(dest) + "/"
 
     if not dir_exists and suffix == "/*":
         with pytest.raises(FileNotFoundError):
             catalog.cp([src], dest_path, recursive=recursive, no_edvcx_file=True)
         return
 
@@ -303,21 +307,22 @@
                 if isinstance(expected[key], dict):
                     del expected[key]
 
     assert tree_from_path(dest) == expected
 
 
 @pytest.mark.parametrize("tree", [TARRED_TREE], indirect=True)
+@pytest.mark.xfail(reason="Missing support for v-objects in cp")
 def test_cp_full_tar(cloud_test_catalog):
     ctc = cloud_test_catalog
     catalog = ctc.catalog
-    catalog.index([ctc.src_uri], index_processors=indexer_formats["tar-files"])
+    create_tar_dataset(catalog, ctc.src_uri, "tarred")
     dest = ctc.working_dir / "data"
     dest.mkdir()
-    src = f"{ctc.src_uri}/"
+    src = "ds://tarred/"
     catalog.cp([src], str(dest), recursive=True, no_edvcx_file=True)
 
     assert tree_from_path(dest, binary=True) == TARRED_TREE
 
 
 @pytest.mark.parametrize(
     "recursive,star,slash,dir_exists",
@@ -401,22 +406,23 @@
 
 
 @pytest.mark.parametrize("tree", [TARRED_TREE], indirect=True)
 @pytest.mark.parametrize("path", ["*/dogs", "animals.tar/dogs"])
 @pytest.mark.parametrize("suffix", ["", "/", "/*"])
 @pytest.mark.parametrize("recursive", [False, True])
 @pytest.mark.parametrize("dir_exists", [False, True])
+@pytest.mark.xfail(reason="Missing support for v-objects in cp")
 def test_cp_tar_subdir(cloud_test_catalog, path, suffix, recursive, dir_exists):
     ctc = cloud_test_catalog
     catalog = ctc.catalog
-    catalog.index([ctc.src_uri], index_processors=indexer_formats["tar-files"])
+    create_tar_dataset(catalog, ctc.src_uri, "tarred")
     dest = ctc.working_dir / "data"
     if dir_exists:
         dest.mkdir()
-    src = f"{ctc.src_uri}/{path}{suffix}"
+    src = f"ds://tarred/{path}{suffix}"
 
     if not dir_exists and suffix == "/*":
         with pytest.raises(FileNotFoundError):
             catalog.cp([src], str(dest), recursive=recursive)
         return
 
     catalog.cp([src], str(dest), recursive=recursive)
@@ -854,78 +860,40 @@
 
 
 def clear_storages(catalog):
     ds = catalog.metastore
     ds.db.execute(ds._storages.delete())
 
 
-@pytest.mark.parametrize("cloud_type", ["file"], indirect=True)
-@pytest.mark.parametrize("use_path", [False, True])
-def test_add_storage(cloud_test_catalog, use_path):
-    catalog = cloud_test_catalog.catalog
-    src_uri = cloud_test_catalog.src_uri
-    clear_storages(catalog)
-    if use_path:
-        src = LocalFileSystem._strip_protocol(src_uri)
-        src = os.path.relpath(src)
-    else:
-        src = src_uri
-    with pytest.raises(RuntimeError):
-        catalog.index([src_uri])
-    catalog.add_storage(src)
-    catalog.index([src_uri])
-
-
-@pytest.mark.parametrize("tree", [TARRED_TREE], indirect=True)
-def test_tar_loader(cloud_test_catalog):
-    ctc = cloud_test_catalog
-    catalog = ctc.catalog
-    catalog.index([ctc.src_uri], index_processors=indexer_formats["tar-files"])
-
-
-@pytest.mark.parametrize("tree", [WEBFORMAT_TREE], indirect=True)
-def test_webformat_loader(cloud_test_catalog):
-    ctc = cloud_test_catalog
-    catalog = ctc.catalog
-    catalog.index([ctc.src_uri], index_processors=indexer_formats["json-pair"])
-
-
-def test_add_storage_error(cloud_test_catalog, cloud_type):
-    catalog = cloud_test_catalog.catalog
-    src_uri = cloud_test_catalog.src_uri
-    if cloud_type == "file":
-        src_uri += "/invalid"
-    with pytest.raises(RuntimeError):
-        catalog.add_storage(src_uri)
-
-
 @pytest.mark.parametrize("tree", [TARRED_TREE], indirect=True)
+@pytest.mark.xfail(reason="Missing support for datasets in ls")
 def test_ls_subobjects(cloud_test_catalog):
     ctc = cloud_test_catalog
     catalog = ctc.catalog
-    catalog.index([ctc.src_uri], index_processors=indexer_formats["tar-files"])
+    create_tar_dataset(catalog, ctc.src_uri, "tarred")
 
     def do_ls(target):
         ((_, results),) = list(catalog.ls([target], fields=["name"]))
         results = list(results)
         result_set = {x[0] for x in results}
         assert len(result_set) == len(results)
         return result_set
 
-    assert do_ls(ctc.src_uri) == {"animals.tar"}
-    assert do_ls(f"{ctc.src_uri}/animals.tar") == {"animals.tar"}
-    assert do_ls(f"{ctc.src_uri}/animals.tar/dogs") == {
+    ds = "ds://tarred"
+    assert do_ls(ds) == {"animals.tar"}
+    assert do_ls(f"{ds}/animals.tar") == {"animals.tar"}
+    assert do_ls(f"{ds}/animals.tar/dogs") == {
         "dog1",
         "dog2",
         "dog3",
         "others",
     }
-    assert do_ls(f"{ctc.src_uri}/animals.tar/") == {"description", "cats", "dogs"}
-    assert do_ls(f"{ctc.src_uri}/*.tar/") == {"description", "cats", "dogs"}
-    assert do_ls(f"{ctc.src_uri}/*.tar/desc*") == {"description"}
+    assert do_ls(f"{ds}/animals.tar/") == {"description", "cats", "dogs"}
+    assert do_ls(f"{ds}/*.tar/") == {"description", "cats", "dogs"}
+    assert do_ls(f"{ds}/*.tar/desc*") == {"description"}
 
 
 def test_index_error(cloud_test_catalog):
     protocol = cloud_test_catalog.src_uri.split("://", 1)[0]
     # XXX: different clients raise inconsistent exceptions
     with pytest.raises(Exception):  # noqa: B017
         cloud_test_catalog.catalog.index([f"{protocol}://does_not_exist"])
@@ -979,14 +947,29 @@
 
     query_script = "syntax error"
 
     with pytest.raises(QueryScriptCompileError):
         catalog.query(query_script)
 
 
+def test_query_fail_wrong_dataset_name(cloud_test_catalog):
+    catalog = cloud_test_catalog.catalog
+
+    query_script = """\
+    from dvcx.query import DatasetQuery
+    DatasetQuery("s3://bucket-name")
+    """
+    query_script = dedent(query_script)
+
+    with pytest.raises(
+        ValueError, match="Cannot use ds_query_ prefix for dataset name"
+    ):
+        catalog.query(query_script, save_as="ds_query_dataset")
+
+
 def test_query_subprocess_wrong_return_code(mock_popen, cloud_test_catalog):
     mock_popen.configure_mock(returncode=1)
     catalog = cloud_test_catalog.catalog
     src_uri = cloud_test_catalog.src_uri
 
     query_script = f"""
 from dvcx.query import DatasetQuery, C
@@ -1045,14 +1028,15 @@
     """
 
     with pytest.raises(QueryScriptDatasetNotFound) as e:
         catalog.query(query_script, save=True)
     assert e.value.output == "random str"
 
 
+@pytest.mark.parametrize("cloud_type", ["s3", "azure", "gcs"], indirect=True)
 def test_storage_stats(cloud_test_catalog):
     catalog = cloud_test_catalog.catalog
     src_uri = cloud_test_catalog.src_uri
 
     with pytest.raises(StorageNotFoundError):
         catalog.storage_stats(src_uri)
```

### Comparing `dvcx-0.79.0/tests/func/test_client.py` & `dvcx-0.80.0/tests/func/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/func/test_dataset_query.py` & `dvcx-0.80.0/tests/func/test_dataset_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import numpy as np
 import pytest
 import sqlalchemy
 from dateutil.parser import isoparse
 from sqlalchemy import tuple_
 
-from dvcx.catalog import QUERY_SCRIPT_CANCELED_EXIT_CODE, indexer_formats
+from dvcx.catalog import QUERY_SCRIPT_CANCELED_EXIT_CODE
 from dvcx.data_storage.schema import DATASET_CORE_COLUMN_NAMES
 from dvcx.data_storage.warehouse import RANDOM_BITS
 from dvcx.dataset import DatasetDependencyType
 from dvcx.dataset import Status as DatasetStatus
 from dvcx.error import DatasetInvalidVersionError, DatasetNotFoundError
 from dvcx.node import Node
 from dvcx.query import (
@@ -56,14 +56,15 @@
     DEFAULT_TREE,
     NUM_TREE,
     SIMPLE_DS_QUERY_RECORDS,
     TARRED_TREE,
     WEBFORMAT_TREE,
     adjusted_float_diff,
     assert_row_names,
+    create_tar_dataset,
     dataset_dependency_asdict,
     insert_nodes,
     text_embedding,
 )
 
 
 @pytest.fixture
@@ -2754,48 +2755,43 @@
     q = DatasetQuery(name="extracted", catalog=catalog).filter(C.parent.glob("*/cats*"))
     assert len(q.results()) == 2
 
     ds = q.extract(Object(to_str), "name")
     assert set(ds) == {("meow", "cat1"), ("mrow", "cat2")}
 
 
+@pytest.mark.parametrize("cloud_type", ["s3", "azure", "gcs"], indirect=True)
 @pytest.mark.parametrize("tree", [DEFAULT_TREE | TARRED_TREE], indirect=True)
 def test_simple_dataset_query(cloud_test_catalog):
     ctc = cloud_test_catalog
     catalog = ctc.catalog
     metastore = catalog.metastore
     warehouse = catalog.warehouse
-    catalog.index([ctc.src_uri], index_processors=indexer_formats["tar-files"])
-    catalog.create_dataset_from_sources("ds1", [ctc.src_uri], recursive=True)
-    DatasetQuery(ctc.src_uri, version=1, catalog=catalog).save("ds2")
-
-    partial_id = metastore.get_valid_partial_id(ctc.src_uri, "")
-    warehouse = warehouse.clone(ctc.src_uri, partial_id)
-    n = warehouse.nodes_table(ctc.src_uri, partial_id)
-    nq = n.dataset_query().order_by(n.c.parent, n.c.name)
-    ds_queries = [nq]
+    create_tar_dataset(catalog, ctc.src_uri, "ds1")
+    DatasetQuery(name="ds1", version=1, catalog=catalog).save("ds2")
+
+    ds_queries = []
     for ds_name in ("ds1", "ds2"):
         ds = metastore.get_dataset(ds_name)
         dr = warehouse.dataset_rows(ds)
         dq = dr.select().order_by(dr.c.parent, dr.c.name)
         ds_queries.append(dq)
 
     ignore_cols = ["id", "parent_id"]
-    node_ds, ds1, ds2 = (
+    ds1, ds2 = (
         [
             {k: v for k, v in zip(DATASET_CORE_COLUMN_NAMES, r) if k not in ignore_cols}
             for r in warehouse.db.execute(q)
         ]
         for q in ds_queries
     )
 
     # everything except the id field should match
-    assert ds1 == node_ds
-    assert ds2 == node_ds
-    assert [(r["parent"], r["name"]) for r in node_ds] == [
+    assert ds1 == ds2
+    assert [(r["parent"], r["name"]) for r in ds1] == [
         ("", "animals.tar"),
         ("", "description"),
         ("animals.tar", "description"),
         ("animals.tar/cats", "cat1"),
         ("animals.tar/cats", "cat2"),
         ("animals.tar/dogs", "dog1"),
         ("animals.tar/dogs", "dog2"),
@@ -2810,36 +2806,36 @@
     ]
 
 
 @pytest.mark.parametrize("tree", [DEFAULT_TREE | TARRED_TREE], indirect=True)
 def test_similarity_search(cloud_test_catalog):
     ctc = cloud_test_catalog
     catalog = ctc.catalog
-    catalog.index([ctc.src_uri], index_processors=indexer_formats["tar-files"])
+    create_tar_dataset(catalog, ctc.src_uri, "ds1")
 
     @udf(
         params=(Object(to_str),),
         output={"embedding": Array(Float32)},
         method="embedding",
     )
     class TextEmbeddingGenerator:
         def embedding(self, text):
             return (text_embedding(text),)
 
     target_embedding, source, parent, name = (
-        DatasetQuery(ctc.src_uri, catalog=catalog)
+        DatasetQuery(name="ds1", catalog=catalog)
         .filter(~C.name.glob("*.tar"))
         .order_by(C.source, C.parent, C.name)
         .limit(1)
         .add_signals(TextEmbeddingGenerator())
         .select(C.embedding, C.source, C.parent, C.name)
         .results()[0]
     )
     q = (
-        DatasetQuery(ctc.src_uri, catalog=catalog)
+        DatasetQuery(name="ds1", catalog=catalog)
         .filter(
             ~C.name.glob("*.tar"),
             tuple_(C.source, C.parent, C.name) != (source, parent, name),
         )
         .add_signals(TextEmbeddingGenerator())
         .mutate(
             cos_dist=cosine_distance(C.embedding, target_embedding),
@@ -2874,15 +2870,15 @@
         for (p1, n1, c1, e1), (p2, n2, c2, e2) in zip(result, expected)
     ]
     assert diffs == expected_diffs
 
 
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
-    [("s3", True)],
+    [("s3", True), ("file", False)],
     indirect=True,
 )
 def test_subtract(cloud_test_catalog):
     from dvcx.dataset import DatasetRow as Row
 
     @udf(("name",), {"name_len": Int})
     def name_len(name):
@@ -2997,15 +2993,15 @@
     assert q.count() == 4
     assert q.sum(C.size) == 15
     assert q.avg(C.size) == 15 / 4
     assert q.min(C.size) == 3
     assert q.max(C.size) == 4
 
 
-def test_group_by(cloud_test_catalog, dogs_dataset):
+def test_group_by(cloud_test_catalog, cloud_type, dogs_dataset):
     catalog = cloud_test_catalog.catalog
 
     q = (
         DatasetQuery(name=dogs_dataset.name, version=1, catalog=catalog)
         .group_by(C.parent)
         .select(
             C.parent,
@@ -3016,18 +3012,25 @@
             functions.max(C.size),
         )
     )
     result = q.results()
     assert len(result) == 2
 
     result_dict = {r[0]: r[1:] for r in result}
-    assert result_dict == {
-        "dogs": (3, 11, 11 / 3, 3, 4),
-        "dogs/others": (1, 4, 4, 4, 4),
-    }
+    if cloud_type == "file":
+        assert result_dict == {
+            f"{cloud_test_catalog.partial_path}/dogs": (3, 11, 11 / 3, 3, 4),
+            f"{cloud_test_catalog.partial_path}/dogs/others": (1, 4, 4, 4, 4),
+        }
+
+    else:
+        assert result_dict == {
+            "dogs": (3, 11, 11 / 3, 3, 4),
+            "dogs/others": (1, 4, 4, 4, 4),
+        }
 
 
 @pytest.mark.parametrize("tree", [WEBFORMAT_TREE], indirect=True)
 def test_json_loader(cloud_test_catalog):
     catalog = cloud_test_catalog.catalog
     dialect = catalog.warehouse.db.dialect
 
@@ -3247,15 +3250,15 @@
     assert (df == expected).all(axis=None)
 
 
 @pytest.mark.parametrize("method", ["to_records", "extract"])
 @pytest.mark.parametrize("save", [True, False])
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
-    [("s3", True)],
+    [("s3", True), ("file", False)],
     indirect=True,
 )
 def test_udf_after_union(cloud_test_catalog, save, method):
     catalog = cloud_test_catalog.catalog
     sources = [cloud_test_catalog.src_uri]
     globs = [s.rstrip("/") + "/*" for s in sources]
     catalog.index(sources)
@@ -3263,21 +3266,21 @@
 
     @udf(("name",), {"name_len": Int})
     def name_len(name):
         # A very simple udf.
         return (len(name),)
 
     ds_cats = DatasetQuery(name="animals", version=1, catalog=catalog).filter(
-        C.parent.glob("cats*")
+        C.parent.glob("*cats*")
     )
     if save:
         ds_cats.save("cats")
         ds_cats = DatasetQuery(name="cats", version=1, catalog=catalog)
     ds_dogs = DatasetQuery(name="animals", version=1, catalog=catalog).filter(
-        C.parent.glob("dogs*")
+        C.parent.glob("*dogs*")
     )
     if save:
         ds_dogs.save("dogs")
         ds_dogs = DatasetQuery(name="dogs", version=1, catalog=catalog)
 
     if method == "to_records":
 
@@ -3320,15 +3323,15 @@
         ("dog4", 4),
     ]
 
 
 @pytest.mark.parametrize("method", ["to_records", "extract"])
 @pytest.mark.parametrize(
     "cloud_type,version_aware",
-    [("s3", True)],
+    [("s3", True), ("file", False)],
     indirect=True,
 )
 def test_udf_after_union_same_rows_with_mutate(cloud_test_catalog, method):
     catalog = cloud_test_catalog.catalog
     sources = [cloud_test_catalog.src_uri]
     globs = [s.rstrip("/") + "/*" for s in sources]
     catalog.index(sources)
@@ -3336,15 +3339,15 @@
 
     @udf(("name",), {"name_len": Int})
     def name_len(name):
         # A very simple udf.
         return (len(name),)
 
     q_base = DatasetQuery(name="animals", version=1, catalog=catalog).filter(
-        C.parent.glob("dogs*")
+        C.parent.glob("*dogs*")
     )
     q1 = q_base.mutate(x=sqlalchemy.cast(C.name + "_1", String()))
     q2 = q_base.mutate(x=sqlalchemy.cast(C.name + "_2", String()))
 
     if method == "to_records":
 
         def get_result(query):
@@ -3390,15 +3393,15 @@
         ("dog4", "dog4_2", 4),
     ]
 
 
 @pytest.mark.parametrize("method", ["select", "extract"])
 @pytest.mark.parametrize(
     "cloud_type,version_aware,tree",
-    [("s3", True, NUM_TREE)],
+    [("s3", True, NUM_TREE), ("file", False, NUM_TREE)],
     indirect=True,
 )
 def test_udf_after_limit(cloud_test_catalog, method):
     catalog = cloud_test_catalog.catalog
     sources = [cloud_test_catalog.src_uri]
     globs = [s.rstrip("/") + "/*" for s in sources]
     catalog.index(sources)
@@ -3434,21 +3437,27 @@
     # incorrect results on clickhouse cloud.
     # See https://github.com/iterative/dvcx/issues/940
     assert get_result(ds.order_by("name")) == expected
     assert len(get_result(ds.order_by("random"))) == 100
     assert len(get_result(ds)) == 100
 
 
+@pytest.mark.parametrize(
+    "cloud_type,version_aware",
+    [("s3", True), ("file", False)],
+    indirect=True,
+)
 @pytest.mark.parametrize("indirect", [True, False])
 def test_dataset_dependencies_one_storage_as_dependency(
     cloud_test_catalog, listed_bucket, indirect
 ):
     ds_name = uuid.uuid4().hex
     catalog = cloud_test_catalog.catalog
-    storage = catalog.get_storage(cloud_test_catalog.src_uri)
+    storage = catalog.get_storage(cloud_test_catalog.storage_uri)
+
     path = f"{cloud_test_catalog.src_uri}/cats"
 
     DatasetQuery(path=path, catalog=catalog).save(ds_name)
 
     assert [
         dataset_dependency_asdict(d)
         for d in catalog.get_dataset_dependencies(ds_name, 1, indirect=indirect)
@@ -3466,15 +3475,15 @@
 
 @pytest.mark.parametrize("indirect", [True, False])
 def test_dataset_dependencies_one_registered_dataset_as_dependency(
     cloud_test_catalog, dogs_dataset, indirect
 ):
     ds_name = uuid.uuid4().hex
     catalog = cloud_test_catalog.catalog
-    storage = catalog.get_storage(cloud_test_catalog.src_uri)
+    storage = catalog.get_storage(cloud_test_catalog.storage_uri)
 
     DatasetQuery(name=dogs_dataset.name, catalog=catalog).save(ds_name)
 
     expected = [
         {
             "id": ANY,
             "type": DatasetDependencyType.DATASET,
@@ -3511,15 +3520,15 @@
 def test_dataset_dependencies_multiple_direct_dataset_dependencies(
     cloud_test_catalog, dogs_dataset, cats_dataset, method
 ):
     # multiple direct dataset dependencies can be achieved with methods that are
     # combining multiple DatasetQuery instances into new one like union or join
     ds_name = uuid.uuid4().hex
     catalog = cloud_test_catalog.catalog
-    storage = catalog.get_storage(cloud_test_catalog.src_uri)
+    storage = catalog.get_storage(cloud_test_catalog.storage_uri)
 
     dogs = DatasetQuery(name=dogs_dataset.name, version=1, catalog=catalog)
     cats = DatasetQuery(name=cats_dataset.name, version=1, catalog=catalog)
 
     if method == "union":
         dogs.union(cats).save(ds_name)
     else:
@@ -3580,15 +3589,15 @@
 
 
 def test_dataset_dependencies_multiple_union(
     cloud_test_catalog, dogs_dataset, cats_dataset
 ):
     ds_name = uuid.uuid4().hex
     catalog = cloud_test_catalog.catalog
-    storage = catalog.get_storage(cloud_test_catalog.src_uri)
+    storage = catalog.get_storage(cloud_test_catalog.storage_uri)
 
     dogs = DatasetQuery(name=dogs_dataset.name, version=1, catalog=catalog)
     cats = DatasetQuery(name=cats_dataset.name, version=1, catalog=catalog)
     dogs_other = DatasetQuery(name=dogs_dataset.name, version=1, catalog=catalog)
 
     dogs.union(cats).union(dogs_other).save(ds_name)
```

### Comparing `dvcx-0.79.0/tests/func/test_datasets.py` & `dvcx-0.80.0/tests/func/test_datasets.py`

 * *Files 0% similar despite different names*

```diff
@@ -926,15 +926,15 @@
 
 
 @pytest.mark.parametrize("indirect", [True, False])
 def test_dataset_dependencies_registered(
     listed_bucket, cloud_test_catalog, dogs_dataset, indirect
 ):
     catalog = cloud_test_catalog.catalog
-    storage = catalog.get_storage(cloud_test_catalog.src_uri)
+    storage = catalog.get_storage(cloud_test_catalog.storage_uri)
 
     assert [
         dataset_dependency_asdict(d)
         for d in catalog.get_dataset_dependencies(
             dogs_dataset.name, 1, indirect=indirect
         )
     ] == [
```

### Comparing `dvcx-0.79.0/tests/func/test_ls.py` & `dvcx-0.80.0/tests/func/test_ls.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,35 @@
 from typing import Any
 
 import msgpack
 import pytest
 from sqlalchemy import select
 
 from dvcx.cli import ls
+from dvcx.client.local import FileClient
 from tests.utils import uppercase_scheme
 
 
 def same_lines(lines1, lines2):
-    return sorted(lines1.split("\n")) == sorted(lines2.split("\n"))
+    def _split_lines(lines):
+        return [line.strip() for line in sorted(lines.split("\n"))]
 
+    return _split_lines(lines1) == _split_lines(lines2)
 
-def test_ls_no_args(cloud_test_catalog, capsys):
+
+def test_ls_no_args(cloud_test_catalog, cloud_type, capsys):
     src = cloud_test_catalog.src_uri
     catalog = cloud_test_catalog.catalog
     catalog.index([src])
     ls([], catalog=catalog)
     captured = capsys.readouterr()
-    assert captured.out == f"{src}\n"
+    if cloud_type == "file":
+        assert captured.out == FileClient.root_path().as_uri() + "\n"
+    else:
+        assert captured.out == f"{src}\n"
 
 
 def test_ls_root(cloud_test_catalog, cloud_type, capsys):
     src = cloud_test_catalog.src_uri
     root = src[: src.find("://") + 3]
     src_name = src.replace(root, "", 1)
     ls([root], catalog=cloud_test_catalog.catalog)
@@ -34,131 +41,173 @@
     if cloud_type == "file":
         assert not captured.out
     else:
         buckets = captured.out.split("\n")
         assert src_name in buckets
 
 
-ls_sources_output = """\
+def ls_sources_output(src, cloud_type):
+    if cloud_type == "file":
+        root_uri = FileClient.root_path().as_uri()
+        prefix = src[len(root_uri) :]
+        return f"""\
+{prefix}:
+cats/
+description
+dogs/
+
+{prefix}/dogs:
+dog1
+dog2
+dog3
+
+{prefix}/dogs/others:
+dog4
+    """
+
+    return """\
 cats/
 dogs/
 description
 
 dogs/others:
 dog4
 
 dogs:
 dog1
 dog2
 dog3
-"""
+    """
 
 
-def test_ls_sources(cloud_test_catalog, capsys):
+def test_ls_sources(cloud_test_catalog, cloud_type, capsys):
     src = cloud_test_catalog.src_uri
     ls([src, f"{src}/dogs/*"], catalog=cloud_test_catalog.catalog)
     captured = capsys.readouterr()
-    assert same_lines(captured.out, ls_sources_output)
+    assert same_lines(captured.out, ls_sources_output(src, cloud_type))
 
 
-def test_ls_sources_scheme_uppercased(cloud_test_catalog, capsys):
+def test_ls_sources_scheme_uppercased(cloud_test_catalog, cloud_type, capsys):
     src = uppercase_scheme(cloud_test_catalog.src_uri)
     ls([src, f"{src}/dogs/*"], catalog=cloud_test_catalog.catalog)
     captured = capsys.readouterr()
-    assert same_lines(captured.out, ls_sources_output)
+    assert same_lines(captured.out, ls_sources_output(src, cloud_type))
 
 
 def test_ls_not_found(cloud_test_catalog):
     src = cloud_test_catalog.src_uri
     with pytest.raises(FileNotFoundError):
         ls([src, f"{src}/cats/bogus*"], catalog=cloud_test_catalog.catalog)
 
 
 def test_ls_not_a_directory(cloud_test_catalog):
     src = cloud_test_catalog.src_uri
     with pytest.raises(FileNotFoundError):
         ls([src, f"{src}/description/"], catalog=cloud_test_catalog.catalog)
 
 
-ls_glob_output = """\
+def ls_glob_output(src, cloud_type):
+    if cloud_type == "file":
+        root_uri = FileClient.root_path().as_uri()
+        prefix = src[len(root_uri) :]
+        return f"""\
+{prefix}/dogs/others:
+dog4
+
+{prefix}/dogs:
+dog1
+dog2
+dog3
+    """
+
+    return """\
 dogs/others:
 dog4
 
 dogs:
 dog1
 dog2
 dog3
-"""
+    """
 
 
-def test_ls_glob_sub(cloud_test_catalog, capsys):
+def test_ls_glob_sub(cloud_test_catalog, cloud_type, capsys):
     src = cloud_test_catalog.src_uri
     ls([f"{src}/dogs/*"], catalog=cloud_test_catalog.catalog)
     captured = capsys.readouterr()
-    assert same_lines(captured.out, ls_glob_output)
+    assert same_lines(captured.out, ls_glob_output(src, cloud_type))
 
 
 def get_partial_indexed_paths(metastore):
     p = metastore._partials
     return [
         r[0] for r in metastore.db.execute(select(p.c.path_str).order_by(p.c.path_str))
     ]
 
 
-def test_ls_partial_indexing(cloud_test_catalog, capsys):
+def test_ls_partial_indexing(cloud_test_catalog, cloud_type, capsys):
     metastore = cloud_test_catalog.catalog.metastore
     src = cloud_test_catalog.src_uri
-    src_metastore = metastore.clone(src)
+    if cloud_type == "file":
+        src_metastore = metastore.clone(FileClient.root_path().as_uri())
+        root_uri = FileClient.root_path().as_uri()
+        prefix = src[len(root_uri) :] + "/"
+    else:
+        src_metastore = metastore.clone(src)
+        prefix = ""
 
     ls([f"{src}/dogs/others/"], catalog=cloud_test_catalog.catalog)
     # These sleep calls are here to ensure that capsys can fully capture the output
     # and to avoid any flaky tests due to multithreading generating output out of order
     sleep(0.05)
     captured = capsys.readouterr()
-    assert get_partial_indexed_paths(src_metastore) == ["dogs/others/"]
+    assert get_partial_indexed_paths(src_metastore) == [f"{prefix}dogs/others/"]
     assert "Listing" in captured.err
     assert captured.out == "dog4\n"
 
     ls([f"{src}/cats/"], catalog=cloud_test_catalog.catalog)
     sleep(0.05)
     captured = capsys.readouterr()
-    assert get_partial_indexed_paths(src_metastore) == ["cats/", "dogs/others/"]
+    assert get_partial_indexed_paths(src_metastore) == [
+        f"{prefix}cats/",
+        f"{prefix}dogs/others/",
+    ]
     assert "Listing" in captured.err
     assert same_lines("cat1\ncat2\n", captured.out)
 
     ls([f"{src}/dogs/"], catalog=cloud_test_catalog.catalog)
     sleep(0.05)
     captured = capsys.readouterr()
     assert get_partial_indexed_paths(src_metastore) == [
-        "cats/",
-        "dogs/",
-        "dogs/others/",
+        f"{prefix}cats/",
+        f"{prefix}dogs/",
+        f"{prefix}dogs/others/",
     ]
     assert "Listing" in captured.err
     assert same_lines("others/\ndog1\ndog2\ndog3\n", captured.out)
 
     ls([f"{src}/cats/"], catalog=cloud_test_catalog.catalog)
     sleep(0.05)
     captured = capsys.readouterr()
     assert get_partial_indexed_paths(src_metastore) == [
-        "cats/",
-        "dogs/",
-        "dogs/others/",
+        f"{prefix}cats/",
+        f"{prefix}dogs/",
+        f"{prefix}dogs/others/",
     ]
     assert "Listing" not in captured.err
     assert same_lines("cat1\ncat2\n", captured.out)
 
     ls([f"{src}/"], catalog=cloud_test_catalog.catalog)
     sleep(0.05)
     captured = capsys.readouterr()
     assert get_partial_indexed_paths(src_metastore) == [
-        "",
-        "cats/",
-        "dogs/",
-        "dogs/others/",
+        f"{prefix}",
+        f"{prefix}cats/",
+        f"{prefix}dogs/",
+        f"{prefix}dogs/others/",
     ]
     assert "Listing" in captured.err
     assert same_lines("cats/\ndogs/\ndescription\n", captured.out)
 
 
 class MockResponse:
     def __init__(self, content, ok=True):
```

### Comparing `dvcx-0.79.0/tests/func/test_pull.py` & `dvcx-0.80.0/tests/func/test_pull.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/func/test_pytorch.py` & `dvcx-0.80.0/tests/func/test_pytorch.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,39 +9,38 @@
 from dvcx.lib.pytorch import PytorchDataset
 from dvcx.sql.types import Int
 
 
 @pytest.fixture
 def fake_dataset(tmp_path):
     # Create fake images in labeled dirs
-    data_path = tmp_path / "data"
+    data_path = tmp_path / "data" / ""
     for i, (img, label) in enumerate(FakeData()):
         label = str(label)
         (data_path / label).mkdir(parents=True, exist_ok=True)
         img.save(data_path / label / f"{i}.jpg")
 
     # Create dataset from images
     uri = data_path.as_uri()
     catalog = get_catalog()
-    catalog.add_storage(uri)
 
     def extract_label(parent):
-        return (int(parent),)
+        return (int(parent.split("/")[-1]),)
 
     yield (
         Dataset(uri)
         .map(extract_label, params=("parent",), output={"label": Int})
         .save("fake")
     )
 
     catalog.remove_dataset("fake", version=1)
     catalog.id_generator.cleanup_for_tests()
 
 
-def test_pytorch_dataset(fake_dataset):
+def test_pytorch_dataset(tmp_path, fake_dataset):
     transform = v2.Compose([v2.ToTensor(), v2.Resize((64, 64))])
     pt_dataset = PytorchDataset(
         fr_classes=[ImageReader(), "label"],
         name=fake_dataset.name,
         version=fake_dataset.version,
         transform=transform,
     )
```

### Comparing `dvcx-0.79.0/tests/func/test_query.py` & `dvcx-0.80.0/tests/func/test_query.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from textwrap import dedent
 
 import dill
 import pytest
 
 from dvcx.catalog import QUERY_DATASET_PREFIX
 from dvcx.cli import query
+from dvcx.error import QueryScriptRunError
 from tests.utils import assert_row_names
 
 
 @pytest.fixture
 def catalog_info_filepath(cloud_test_catalog_tmpfile, tmp_path):
     catalog = cloud_test_catalog_tmpfile.catalog
 
@@ -81,31 +82,84 @@
     captured = capsys.readouterr()
 
     header, *rows = captured.out.splitlines()
     assert header.strip() == "name"
     name_rows = {row.split()[1] for row in rows}
     assert name_rows == {"cat1", "cat2", "description", "dog1", "dog2", "dog3", "dog4"}
 
+    assert catalog.get_dataset(ds_name)
 
-def test_query(cloud_test_catalog_tmpfile, tmp_path, catalog_info_filepath):
+
+def test_query_cli_no_dataset_returned(
+    cloud_test_catalog_tmpfile, tmp_path, catalog_info_filepath, capsys
+):
+    catalog = cloud_test_catalog_tmpfile.catalog
+
+    query_script = """\
+    from dvcx.query import DatasetQuery
+
+    DatasetQuery("test", catalog=catalog)
+
+    print("test")
+    """
+    query_script = setup_catalog(query_script, catalog_info_filepath)
+
+    filepath = tmp_path / "query_script.py"
+    filepath.write_text(query_script)
+
+    with pytest.raises(
+        QueryScriptRunError,
+        match="Last line in a script was not an instance of DatasetQuery",
+    ):
+        query(catalog, str(filepath), "my-dataset", columns=["name"])
+
+
+@pytest.mark.parametrize(
+    "save,save_as",
+    (
+        (True, None),
+        (None, "my-dataset"),
+        (True, "my-dataset"),
+    ),
+)
+@pytest.mark.parametrize("save_dataset", (None, "new-dataset"))
+def test_query(
+    save,
+    save_as,
+    save_dataset,
+    cloud_test_catalog_tmpfile,
+    tmp_path,
+    catalog_info_filepath,
+):
     catalog = cloud_test_catalog_tmpfile.catalog
     src_uri = cloud_test_catalog_tmpfile.src_uri
 
     query_script = f"""\
-    from dvcx.query import C, DatasetQuery
-
-    DatasetQuery({src_uri!r}, catalog=catalog)
+    from dvcx.query import DatasetQuery
+    ds = DatasetQuery({src_uri!r}, catalog=catalog)
+    if {save_dataset!r}:
+        ds = ds.save({save_dataset!r})
+    ds
     """
     query_script = setup_catalog(query_script, catalog_info_filepath)
 
-    dataset, version, output, _ = catalog.query(query_script, save=True)
-    assert dataset.name.startswith(QUERY_DATASET_PREFIX)
-    assert dataset.query_script == query_script
+    dataset, version, output, _ = catalog.query(
+        query_script, save=save, save_as=save_as
+    )
+    if save_as:
+        assert dataset.name == save_as
+        assert catalog.get_dataset(save_as)
+    elif save_dataset:
+        assert dataset.name == save_dataset
+        assert catalog.get_dataset(save_dataset)
+    else:
+        assert dataset.name.startswith(QUERY_DATASET_PREFIX)
     assert version == 1
     assert dataset.versions_values == [1]
+    assert dataset.query_script == query_script
     assert_row_names(
         catalog,
         dataset,
         version,
         {
             "cat1",
             "cat2",
```

### Comparing `dvcx-0.79.0/tests/scripts/name_len_normal.py` & `dvcx-0.80.0/tests/scripts/name_len_normal.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/scripts/name_len_slow.py` & `dvcx-0.80.0/tests/scripts/name_len_slow.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/test_cli_e2e.py` & `dvcx-0.80.0/tests/test_cli_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/test_query_e2e.py` & `dvcx-0.80.0/tests/test_query_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/lib/test_cached_stream.py` & `dvcx-0.80.0/tests/unit/lib/test_cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/lib/test_feature.py` & `dvcx-0.80.0/tests/unit/lib/test_feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/lib/test_feature_udf.py` & `dvcx-0.80.0/tests/unit/lib/test_feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/lib/test_file.py` & `dvcx-0.80.0/tests/unit/lib/test_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/lib/test_image.py` & `dvcx-0.80.0/tests/unit/lib/test_image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/lib/test_reader.py` & `dvcx-0.80.0/tests/unit/lib/test_reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/lib/test_text.py` & `dvcx-0.80.0/tests/unit/lib/test_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/lib/test_webdataset.py` & `dvcx-0.80.0/tests/unit/lib/test_webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/lib/test_webdataset_meta.py` & `dvcx-0.80.0/tests/unit/lib/test_webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/sql/test_array.py` & `dvcx-0.80.0/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/sql/test_conditional.py` & `dvcx-0.80.0/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/sql/test_path.py` & `dvcx-0.80.0/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/sql/test_selectable.py` & `dvcx-0.80.0/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/sql/test_string.py` & `dvcx-0.80.0/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_asyn.py` & `dvcx-0.80.0/tests/unit/test_asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_cache.py` & `dvcx-0.80.0/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_catalog_loader.py` & `dvcx-0.80.0/tests/unit/test_catalog_loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_cli_parsing.py` & `dvcx-0.80.0/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_client_s3.py` & `dvcx-0.80.0/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_database_engine.py` & `dvcx-0.80.0/tests/unit/test_database_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_dataset.py` & `dvcx-0.80.0/tests/unit/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_dataset_row.py` & `dvcx-0.80.0/tests/unit/test_dataset_row.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_dispatch.py` & `dvcx-0.80.0/tests/unit/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_fileslice.py` & `dvcx-0.80.0/tests/unit/test_fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_id_generator.py` & `dvcx-0.80.0/tests/unit/test_id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_listing.py` & `dvcx-0.80.0/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_metastore.py` & `dvcx-0.80.0/tests/unit/test_metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_query_params.py` & `dvcx-0.80.0/tests/unit/test_query_params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_serializer.py` & `dvcx-0.80.0/tests/unit/test_serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_session.py` & `dvcx-0.80.0/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_storage.py` & `dvcx-0.80.0/tests/unit/test_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -184,26 +184,33 @@
     assert storage.error_message == error_message
     assert storage.error_stack == error_stack
 
 
 def test_unlist_source(
     listed_bucket,
     cloud_test_catalog,
+    cloud_type,
 ):
     # TODO remove when https://github.com/iterative/dvcx/pull/868 is merged
     skip_if_not_sqlite()
     source_uri = cloud_test_catalog.src_uri
     catalog = cloud_test_catalog.catalog
-    partial_id = catalog.metastore.get_valid_partial_id(source_uri, "")
-    warehouse = catalog.warehouse.clone(source_uri, partial_id)
+    partial_id = catalog.metastore.get_valid_partial_id(
+        cloud_test_catalog.storage_uri, cloud_test_catalog.partial_path
+    )
+    warehouse = catalog.warehouse.clone(cloud_test_catalog.storage_uri, partial_id)
     dataset_name = warehouse.nodes.name
 
     # list source
-    storage = catalog.get_storage(source_uri)
-    assert storage.status == Status.COMPLETE
+    storage = catalog.get_storage(cloud_test_catalog.storage_uri)
+    if cloud_type == "file":
+        assert storage.status == Status.PARTIAL
+    else:
+        assert storage.status == Status.COMPLETE
+
     assert warehouse.db.has_table(dataset_name)
 
     # unlist source
     catalog.unlist_source(source_uri)
     with pytest.raises(StorageNotFoundError):
         catalog.get_storage(source_uri)
     # we preserve the table for dataset lineage
```

### Comparing `dvcx-0.79.0/tests/unit/test_udf.py` & `dvcx-0.80.0/tests/unit/test_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_utils.py` & `dvcx-0.80.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/unit/test_warehouse.py` & `dvcx-0.80.0/tests/unit/test_warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.79.0/tests/utils.py` & `dvcx-0.80.0/tests/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import pytest
 
 from dvcx.catalog.catalog import Catalog
 from dvcx.dataset import DatasetDependency, DatasetRecord
 from dvcx.node import Entry
 from dvcx.query import C, DatasetQuery
+from dvcx.query.builtins import index_tar
 from dvcx.storage import Status as StorageStatus
 
 
 def insert_nodes(warehouse, entries):
     """
     Takes a list of entries and inserts them synchronously.
 
@@ -122,14 +123,26 @@
             archive.addfile(info, io.BytesIO())
             write_tar(value, archive, name)
 
 
 TARRED_TREE: dict[str, Any] = {"animals.tar": make_tar(DEFAULT_TREE)}
 
 
+def create_tar_dataset(catalog, uri: str, ds_name: str) -> DatasetQuery:
+    """
+    Create a dataset from a storage location containing tar archives and other files.
+
+    The resulting dataset contains both the original files (as regular objects)
+    and the tar members (as v-objects).
+    """
+    ds1 = DatasetQuery(path=uri, catalog=catalog)
+    tar_entries = ds1.filter(C("name").glob("*.tar")).generate(index_tar)
+    return ds1.filter(~C("name").glob("*.tar")).union(tar_entries).save(ds_name)
+
+
 def skip_if_not_sqlite():
     if os.environ.get("DVCX_METASTORE") or os.environ.get("DVCX_WAREHOUSE"):
         pytest.skip("This test is not supported on other data storages")
 
 
 WEBFORMAT_TREE: dict[str, Any] = {
     "f1.raw": "raw data",
```

