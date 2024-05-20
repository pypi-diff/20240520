# Comparing `tmp/dkist-1.5.0rc1.tar.gz` & `tmp/dkist-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-1.5.0rc1.tar", last modified: Tue Apr  2 20:54:09 2024, max compression
+gzip compressed data, was "dkist-1.6.0.tar", last modified: Mon May 20 15:22:24 2024, max compression
```

## Comparing `dkist-1.5.0rc1.tar` & `dkist-1.6.0.tar`

### file list

```diff
@@ -1,249 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.110747 dkist-1.5.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.codespell-dict.txt
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.codespellrc
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.062747 dkist-1.5.0rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.074747 dkist-1.5.0rc1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.github/ISSUE_TEMPLATE/BUG_REPORT.md
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.github/ISSUE_TEMPLATE/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.074747 dkist-1.5.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.github/workflows/prepare-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.github/workflows/sub_package_update.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.rtd-environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/.ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)    23150 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-02 20:54:09.110747 dkist-1.5.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.074747 dkist-1.5.0rc1/changelog/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/changelog/309.bugfix.rst
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/changelog/344.trivial.rst
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/changelog/347.feature.rst
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/changelog/349.doc.rst
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/changelog/361.bugfix.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/changelog/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.074747 dkist-1.5.0rc1/dkist/
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-02 20:54:08.000000 dkist-1.5.0rc1/dkist/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.074747 dkist-1.5.0rc1/dkist/config/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12171 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.078747 dkist-1.5.0rc1/dkist/data/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/VISP_HEADER.hdr
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/api_search_values.json
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.082747 dkist-1.5.0rc1/dkist/data/test/
--rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/5d_gwcs.asdf
--rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/AGLKO-inv.ecsv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.086747 dkist-1.5.0rc1/dkist/data/test/EIT/
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.000010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.020010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.030011_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.040010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.050010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.060010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.080010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.090010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.100010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.110010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.120010_s.fits
--rw-r--r--   0 runner    (1001) docker     (127)    32769 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/EIT/eit_test_dataset.asdf
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    96407 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/eit_dataset-0.1.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    96552 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/eit_dataset-0.2.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    97195 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/eit_dataset-0.3.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    99686 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/eit_dataset-1.0.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    32741 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/eit_dataset-1.1.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    32769 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/eit_dataset-1.2.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/globus_operation_ls_response.json
--rw-r--r--   0 runner    (1001) docker     (127)    42219 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/globus_search_response.json
--rw-r--r--   0 runner    (1001) docker     (127)   136848 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/large_visp.asdf.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.086747 dkist-1.5.0rc1/dkist/data/test/small_visp/
--rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/small_visp/0.fits
--rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/small_visp/1.fits
--rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/small_visp/2.fits
--rw-r--r--   0 runner    (1001) docker     (127)   104749 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/small_visp/test_visp.asdf
--rw-r--r--   0 runner    (1001) docker     (127)    22098 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/test_old_wcs_BRMQY.asdf
--rw-r--r--   0 runner    (1001) docker     (127)   619185 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.0.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)   619217 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.1.0.asdf
--rw-r--r--   0 runner    (1001) docker     (127)   599267 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.2.0.asdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.086747 dkist-1.5.0rc1/dkist/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/dataset/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/tests/test_load_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/tests/test_tiled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/tiled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dataset/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/dkist.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/extern/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/io/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/io/asdf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/io/asdf/converters/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/converters/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/converters/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/converters/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/converters/tiled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2643 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/entry_points.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/io/asdf/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.090747 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-0.9.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-1.2.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-wcs-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-wcs-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-wcs-1.2.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.094747 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/asymmetric_mapping_model-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/coupled_compound_model-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-0.2.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-0.3.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-1.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/file_manager-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/ravel_model-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/tiled_dataset-0.1.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/tiled_dataset-1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/varying_celestial_transform-1.0.0.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.094747 dkist-1.5.0rc1/dkist/io/asdf/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/asdf/tests/test_tiled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/dask_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16928 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/level_1_dataset_schema.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.094747 dkist-1.5.0rc1/dkist/io/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10055 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/tests/test_file_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/io/tests/test_fits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.094747 dkist-1.5.0rc1/dkist/net/
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/attr_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13842 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/attrs_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.098747 dkist-1.5.0rc1/dkist/net/globus/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.098747 dkist-1.5.0rc1/dkist/net/globus/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/tests/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/tests/test_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/globus/transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.098747 dkist-1.5.0rc1/dkist/net/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/test_attr_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/test_attrs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/test_attrs_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/net/tests/test_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.098747 dkist-1.5.0rc1/dkist/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/tests/generate_aia_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/tests/generate_eit_test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/tests/generate_eit_tiled_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/tests/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/dkist/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/_model_to_graphviz.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/sysinfo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/dkist/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/tests/test_inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/utils/tests/test_sysinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/dkist/wcs/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/wcs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    26350 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/wcs/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/dkist/wcs/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/wcs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/wcs/tests/test_coupled_compound_model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24398 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/dkist/wcs/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.106747 dkist-1.5.0rc1/dkist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-02 20:54:09.000000 dkist-1.5.0rc1/dkist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-02 20:54:09.000000 dkist-1.5.0rc1/dkist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:54:09.000000 dkist-1.5.0rc1/dkist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-02 20:54:09.000000 dkist-1.5.0rc1/dkist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 20:54:08.000000 dkist-1.5.0rc1/dkist.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-02 20:54:09.000000 dkist-1.5.0rc1/dkist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 20:54:09.000000 dkist-1.5.0rc1/dkist.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/developer.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/docs/howto_guides/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/howto_guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/howto_guides/reproject_vbi_mosaic.md
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/docs/logo/
--rw-r--r--   0 runner    (1001) docker     (127)    72150 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/logo/icon_square.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/reference.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.102747 dkist-1.5.0rc1/docs/topic_guides/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/topic_guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/topic_guides/level1data.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/topic_guides/loading.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/topic_guides/net.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/topic_guides/usertools.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.106747 dkist-1.5.0rc1/docs/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/1_astropy_and_sunpy.md
--rw-r--r--   0 runner    (1001) docker     (127)     7855 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/1_astropy_and_sunpy_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/2_search_and_asdf_download.md
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/2_search_and_asdf_download_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/3_the_dataset.md
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/3_the_dataset_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/4_more_dataset.md
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/5_downloading_data.md
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/6_visualization.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/tutorial/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:09.106747 dkist-1.5.0rc1/docs/whatsnew/
--rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/whatsnew/1.0.rst
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/whatsnew/1.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/whatsnew/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/docs/whatsnew/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-02 20:54:09.110747 dkist-1.5.0rc1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       60 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-02 20:53:55.000000 dkist-1.5.0rc1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.481364 dkist-1.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-20 15:22:15.000000 dkist-1.6.0/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-20 15:22:15.000000 dkist-1.6.0/.codespell-dict.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-20 15:22:15.000000 dkist-1.6.0/.codespellrc
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-20 15:22:15.000000 dkist-1.6.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-20 15:22:15.000000 dkist-1.6.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-20 15:22:15.000000 dkist-1.6.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.441364 dkist-1.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.441364 dkist-1.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-20 15:22:15.000000 dkist-1.6.0/.github/ISSUE_TEMPLATE/BUG_REPORT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-20 15:22:15.000000 dkist-1.6.0/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-20 15:22:15.000000 dkist-1.6.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-20 15:22:15.000000 dkist-1.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.441364 dkist-1.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-20 15:22:15.000000 dkist-1.6.0/.github/workflows/codspeed.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-05-20 15:22:15.000000 dkist-1.6.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-05-20 15:22:15.000000 dkist-1.6.0/.github/workflows/prepare-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-20 15:22:15.000000 dkist-1.6.0/.github/workflows/sub_package_update.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-20 15:22:15.000000 dkist-1.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:15.000000 dkist-1.6.0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-20 15:22:15.000000 dkist-1.6.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-20 15:22:15.000000 dkist-1.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-20 15:22:15.000000 dkist-1.6.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-20 15:22:15.000000 dkist-1.6.0/.rtd-environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-05-20 15:22:15.000000 dkist-1.6.0/.ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    24880 2024-05-20 15:22:15.000000 dkist-1.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-20 15:22:15.000000 dkist-1.6.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-05-20 15:22:15.000000 dkist-1.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-20 15:22:15.000000 dkist-1.6.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-20 15:22:15.000000 dkist-1.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-20 15:22:24.481364 dkist-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-05-20 15:22:15.000000 dkist-1.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.441364 dkist-1.6.0/changelog/
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-20 15:22:15.000000 dkist-1.6.0/changelog/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-20 15:22:15.000000 dkist-1.6.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.441364 dkist-1.6.0/dkist/
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 15:22:24.000000 dkist-1.6.0/dkist/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.445364 dkist-1.6.0/dkist/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.445364 dkist-1.6.0/dkist/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/VISP_HEADER.hdr
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/api_search_values.json
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.453364 dkist-1.6.0/dkist/data/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     6393 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/5d_gwcs.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/AGLKO-inv.ecsv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.457364 dkist-1.6.0/dkist/data/test/EIT/
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/EIT/efz20040301.000010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/EIT/efz20040301.020010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/EIT/efz20040301.030011_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/EIT/efz20040301.040010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/EIT/efz20040301.050010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/EIT/efz20040301.060010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/EIT/efz20040301.080010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/EIT/efz20040301.090010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/EIT/efz20040301.100010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/EIT/efz20040301.110010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   141120 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/EIT/efz20040301.120010_s.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    32769 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/EIT/eit_test_dataset.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96407 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/eit_dataset-0.1.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    96552 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/eit_dataset-0.2.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    97195 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/eit_dataset-0.3.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    99686 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/eit_dataset-1.0.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    32741 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/eit_dataset-1.1.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    32769 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/eit_dataset-1.2.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/globus_operation_ls_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)    42219 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/globus_search_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)   136848 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/large_visp.asdf.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.457364 dkist-1.6.0/dkist/data/test/small_visp/
+-rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/small_visp/0.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/small_visp/1.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/small_visp/2.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   104749 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/small_visp/test_visp.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)    22098 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/test_old_wcs_BRMQY.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)   619185 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.0.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)   619217 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.1.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)   599267 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.2.0.asdf
+-rw-r--r--   0 runner    (1001) docker     (127)   280313 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/data/test/visp_no_headers.asdf.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.457364 dkist-1.6.0/dkist/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/dataset/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.457364 dkist-1.6.0/dkist/dataset/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/dataset/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/dataset/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/dataset/tests/test_load_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/dataset/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/dataset/tests/test_tiled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/dataset/tiled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5097 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/dataset/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/dkist.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.457364 dkist-1.6.0/dkist/extern/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.461364 dkist-1.6.0/dkist/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.461364 dkist-1.6.0/dkist/io/asdf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.461364 dkist-1.6.0/dkist/io/asdf/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/converters/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/converters/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/converters/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/converters/tiled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/entry_points.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.461364 dkist-1.6.0/dkist/io/asdf/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.461364 dkist-1.6.0/dkist/io/asdf/resources/manifests/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/manifests/dkist-0.9.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/manifests/dkist-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/manifests/dkist-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/manifests/dkist-1.2.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/manifests/dkist-wcs-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/manifests/dkist-wcs-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/manifests/dkist-wcs-1.2.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/manifests/dkist-wcs-1.3.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.465364 dkist-1.6.0/dkist/io/asdf/resources/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/schemas/asymmetric_mapping_model-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/schemas/asymmetric_mapping_model-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/schemas/coupled_compound_model-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/schemas/coupled_compound_model-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/schemas/dataset-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/schemas/dataset-0.2.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/schemas/dataset-0.3.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/schemas/dataset-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/schemas/dataset-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/schemas/file_manager-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/schemas/ravel_model-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/schemas/ravel_model-1.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/schemas/tiled_dataset-0.1.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/schemas/tiled_dataset-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/schemas/varying_celestial_transform-1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/resources/schemas/varying_celestial_transform-1.1.0.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.465364 dkist-1.6.0/dkist/io/asdf/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/asdf/tests/test_tiled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/dask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16928 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/level_1_dataset_schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.465364 dkist-1.6.0/dkist/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10055 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/tests/test_file_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/io/tests/test_fits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.469364 dkist-1.6.0/dkist/net/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/attr_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13842 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/attrs_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.469364 dkist-1.6.0/dkist/net/globus/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/globus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/globus/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/globus/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.469364 dkist-1.6.0/dkist/net/globus/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/globus/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/globus/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/globus/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/globus/tests/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/globus/tests/test_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12487 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/globus/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.469364 dkist-1.6.0/dkist/net/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/tests/test_attr_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/tests/test_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6237 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/tests/test_attrs_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9116 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/net/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.473364 dkist-1.6.0/dkist/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/tests/generate_aia_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/tests/generate_eit_test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/tests/generate_eit_tiled_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/tests/test_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.473364 dkist-1.6.0/dkist/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/utils/_model_to_graphviz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/utils/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/utils/sysinfo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.473364 dkist-1.6.0/dkist/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/utils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/utils/tests/test_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/utils/tests/test_sysinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.473364 dkist-1.6.0/dkist/wcs/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/wcs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29104 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/wcs/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.473364 dkist-1.6.0/dkist/wcs/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/wcs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/wcs/tests/test_coupled_compound_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24436 2024-05-20 15:22:15.000000 dkist-1.6.0/dkist/wcs/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.481364 dkist-1.6.0/dkist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-05-20 15:22:24.000000 dkist-1.6.0/dkist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-20 15:22:24.000000 dkist-1.6.0/dkist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:22:24.000000 dkist-1.6.0/dkist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-20 15:22:24.000000 dkist-1.6.0/dkist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 15:22:24.000000 dkist-1.6.0/dkist.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-20 15:22:24.000000 dkist-1.6.0/dkist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 15:22:24.000000 dkist-1.6.0/dkist.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.473364 dkist-1.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     6120 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/developer.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.477364 dkist-1.6.0/docs/howto_guides/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/howto_guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/howto_guides/reproject_vbi_mosaic.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.477364 dkist-1.6.0/docs/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)    72150 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/logo/icon_square.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/reference.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.477364 dkist-1.6.0/docs/topic_guides/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/topic_guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/topic_guides/level1data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6539 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/topic_guides/loading.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10253 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/topic_guides/net.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/topic_guides/usertools.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.477364 dkist-1.6.0/docs/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/tutorial/1_astropy_and_sunpy.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7855 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/tutorial/1_astropy_and_sunpy_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/tutorial/2_search_and_asdf_download.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/tutorial/2_search_and_asdf_download_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/tutorial/3_the_dataset.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/tutorial/3_the_dataset_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/tutorial/4_more_dataset.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/tutorial/5_downloading_data.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/tutorial/6_visualization.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/tutorial/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 15:22:24.477364 dkist-1.6.0/docs/whatsnew/
+-rw-r--r--   0 runner    (1001) docker     (127)     6966 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/whatsnew/1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/whatsnew/1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/whatsnew/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-20 15:22:15.000000 dkist-1.6.0/docs/whatsnew/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-20 15:22:15.000000 dkist-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-20 15:22:15.000000 dkist-1.6.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-20 15:22:24.481364 dkist-1.6.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       60 2024-05-20 15:22:15.000000 dkist-1.6.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3846 2024-05-20 15:22:15.000000 dkist-1.6.0/tox.ini
```

### Comparing `dkist-1.5.0rc1/.coveragerc` & `dkist-1.6.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/.cruft.json` & `dkist-1.6.0/.cruft.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'6d6729b22066ef890e70c37438da70cac33e03b4'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "ddc758c6a73ec074385ee0413253051ca15d7d8e",
+    "commit": "6d6729b22066ef890e70c37438da70cac33e03b4",
     "context": {
         "cookiecutter": {
             "_copy_without_render": [
                 "docs/_templates",
                 "docs/_static",
                 ".github/workflows/sub_package_update.yml"
             ],
```

### Comparing `dkist-1.5.0rc1/.flake8` & `dkist-1.6.0/.flake8`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/.github/ISSUE_TEMPLATE/BUG_REPORT.md` & `dkist-1.6.0/.github/ISSUE_TEMPLATE/BUG_REPORT.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md` & `dkist-1.6.0/.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/.github/workflows/main.yml` & `dkist-1.6.0/.github/workflows/main.yml`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,16 @@
       - 'prepare-v*'
     tags:
       - 'v*'
       - '!*dev*'
       - '!*pre*'
       - '!*post*'
   pull_request:
+  release:
+    types: [published]
   schedule:
     #        ┌───────── minute (0 - 59)
     #        │ ┌───────── hour (0 - 23)
     #        │ │ ┌───────── day of the month (1 - 31)
     #        │ │ │ ┌───────── month (1 - 12 or JAN-DEC)
     #        │ │ │ │ ┌───────── day of the week (0 - 6 or SUN-SAT)
     - cron: '0 9 * * 1'  # Every Monday at 0900 UTC
```

### Comparing `dkist-1.5.0rc1/.github/workflows/prepare-release.yml` & `dkist-1.6.0/.github/workflows/prepare-release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
       - name: Update attrs
         run: |
           python -c "from dkist.net.attrs_values import attempt_local_update; attempt_local_update(user_file='./dkist/data/api_search_values.json', silence_errors=False)"
 
       - name: Commit Attrs
         run: |
-          git update-index --refresh
+          git update-index --refresh || true
           git diff-index --quiet HEAD -- || git commit -m "Update attrs values before release [skip ci]" dkist/data/api_search_values.json
 
       - name: Install towncrier
         run: python -m pip install --upgrade towncrier pre-commit
 
       - name: Run towncrier in draft to capture the output
         run: towncrier build --draft --version ${{ inputs.version }} --yes > release-changelog.rst
```

### Comparing `dkist-1.5.0rc1/.github/workflows/sub_package_update.yml` & `dkist-1.6.0/.github/workflows/sub_package_update.yml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/.gitignore` & `dkist-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/.pre-commit-config.yaml` & `dkist-1.6.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         args: ["--fix"]
   - repo: https://github.com/PyCQA/isort
     rev: 5.13.2
     hooks:
       - id: isort
         exclude: ".*(.fits|.fts|.fit|.header|.txt|tca.*|extern.*|dkist/extern)$"
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-ast
       - id: check-case-conflict
       - id: trailing-whitespace
         exclude: ".*(.fits|.fts|.fit|.header|.txt|.hdr|.asdf)"
       - id: check-yaml
       - id: debug-statements
```

### Comparing `dkist-1.5.0rc1/.readthedocs.yaml` & `dkist-1.6.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/.ruff.toml` & `dkist-1.6.0/.ruff.toml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/CHANGELOG.rst` & `dkist-1.6.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,52 @@
+1.6.0 (2024-05-20)
+==================
+
+Features
+--------
+
+- Update ASDF schemas for upcoming ASDF standard 1.6.0. (`#324 <https://github.com/DKISTDC/dkist/pull/324>`_)
+- Improve performance of ``VaryingCelestialTransform`` classes by not creating a new transform for every set of parameters but instead update the parameters on a single model. (`#370 <https://github.com/DKISTDC/dkist/pull/370>`_)
+- Add GitHub workflow and dependencies for Codspeed, to benchmark PRs against main. (`#382 <https://github.com/DKISTDC/dkist/pull/382>`_)
+
+
+Trivial/Internal Changes
+------------------------
+
+- Run plotting benchmarks fewer times for more manageable CI, and add a benchmark for generate_celestial_transform. (`#383 <https://github.com/DKISTDC/dkist/pull/383>`_)
+
+
+1.5.0 (2024-04-03)
+==================
+
+Features
+--------
+
+- Our minimum Python version is now 3.10 inline with `SPEC-0 <https://scientific-python.org/specs/spec-0000/>`__. (`#347 <https://github.com/DKISTDC/dkist/pull/347>`_)
+
+
+Bug Fixes
+---------
+
+- Fix broadcasting issues during pixel -> world conversion for models with a Ravel component. (`#309 <https://github.com/DKISTDC/dkist/pull/309>`_)
+- Fix a performance regression when dask>=2024.2.1 is installed. (`#361 <https://github.com/DKISTDC/dkist/pull/361>`_)
+
+
+Improved Documentation
+----------------------
+
+- Add a how to guide describing how to reproject VBI data. Also migrate tutorial to the latest DDT datasets. (`#349 <https://github.com/DKISTDC/dkist/pull/349>`_)
+
+
+Trivial/Internal Changes
+------------------------
+
+- Refactor various subclasses of VaryingCelestialTransform to centralise the calculations in preparation for improving performance. (`#344 <https://github.com/DKISTDC/dkist/pull/344>`_)
+
+
 1.4.0 (2024-02-26)
 ==================
 
 Bug Fixes
 ---------
 
 - Correct Fido time searching to use `endTimeMin` and `startTimeMax` (in the correct order) so that searching returns any dataset with a partially or completely overlapping time range. (`#336 <https://github.com/DKISTDC/dkist/pull/336>`_)
```

### Comparing `dkist-1.5.0rc1/CONTRIBUTING.md` & `dkist-1.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/LICENSE.rst` & `dkist-1.6.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/PKG-INFO` & `dkist-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: dkist
-Version: 1.5.0rc1
+Version: 1.6.0
 Summary: DKIST User Tools
 Author-email: NSO / AURA <stuart@cadair.com>
 Project-URL: repository, https://github.com/DKISTDC/dkist
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: aiohttp>=3.8
 Requires-Dist: asdf>=2.11.2
 Requires-Dist: asdf-astropy>=0.2.0
 Requires-Dist: asdf-coordinates-schemas>=0.1.0
 Requires-Dist: asdf-standard>=1.0.3
 Requires-Dist: asdf-transform-schemas>=0.3.0
-Requires-Dist: asdf-unit-schemas>=0.1.0
 Requires-Dist: asdf-wcs-schemas>=0.3.0
 Requires-Dist: astropy>=5.3
 Requires-Dist: dask[array]>=2021.8.0
 Requires-Dist: globus-sdk>=3.0
 Requires-Dist: gwcs>=0.19.0
 Requires-Dist: matplotlib>=3.5
 Requires-Dist: ndcube[plotting,reproject]>=2.0
@@ -31,14 +30,16 @@
 Requires-Dist: pytest-doctestplus; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-remotedata; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: pytest-mpl; extra == "tests"
 Requires-Dist: pytest-httpserver; extra == "tests"
+Requires-Dist: pytest-filter-subpackage; extra == "tests"
+Requires-Dist: pytest-benchmark; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Requires-Dist: tox; extra == "tests"
 Requires-Dist: pydot; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-astropy; extra == "docs"
 Requires-Dist: sphinx-gallery; extra == "docs"
```

### Comparing `dkist-1.5.0rc1/README.rst` & `dkist-1.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/changelog/README.rst` & `dkist-1.6.0/changelog/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/__init__.py` & `dkist-1.6.0/dkist/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/conftest.py` & `dkist-1.6.0/dkist/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -303,24 +303,38 @@
 
     vispdir = Path(rootdir) / "small_visp"
     with asdf.open(vispdir / "test_visp.asdf") as f:
         return f.tree["dataset"]
 
 
 @pytest.fixture(scope="session")
-def large_visp_dataset(tmp_path_factory):
+def large_visp_dataset_file(tmp_path_factory):
+    vispdir = tmp_path_factory.mktemp("data")
+    with gzip.open(Path(rootdir) / "large_visp.asdf.gz", mode="rb") as gfo:
+        with open(vispdir / "test_visp.asdf", mode="wb") as afo:
+            afo.write(gfo.read())
+    return vispdir / "test_visp.asdf"
+
+
+@pytest.fixture(scope="session")
+def large_visp_dataset(large_visp_dataset_file):
     # This dataset was generated by the following code:
     # from dkist_data_simulator.spec214.visp import SimpleVISPDataset
     # from dkist_inventory.asdf_generator import dataset_from_fits
 
     # tmp_path = tmp_path_factory.mktemp("data")
     # vispdir = Path(tmp_path) / "large_visp"
     # ds = SimpleVISPDataset(n_maps=1, n_steps=20, n_stokes=4, time_delta=10,
     #                        linewave=500*u.nm, detector_shape=(50, 128))
     # ds.generate_files(vispdir)
     # dataset_from_fits(vispdir, "test_visp.asdf")
 
+    return load_dataset(large_visp_dataset_file)
+
+
+@pytest.fixture(scope="session")
+def visp_dataset_no_headers(tmp_path_factory):
     vispdir = tmp_path_factory.mktemp("data")
-    with gzip.open(Path(rootdir) / "large_visp.asdf.gz", mode="rb") as gfo:
-        with open(vispdir / "test_visp.asdf", mode="wb") as afo:
+    with gzip.open(Path(rootdir) / "visp_no_headers.asdf.gz", mode="rb") as gfo:
+        with open(vispdir / "test_visp_no_headers.asdf", mode="wb") as afo:
             afo.write(gfo.read())
-    return load_dataset(vispdir / "test_visp.asdf")
+    return load_dataset(vispdir / "test_visp_no_headers.asdf")
```

### Comparing `dkist-1.5.0rc1/dkist/data/VISP_HEADER.hdr` & `dkist-1.6.0/dkist/data/VISP_HEADER.hdr`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/api_search_values.json` & `dkist-1.6.0/dkist/data/api_search_values.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9832283077396062%*

 * *Differences: {"'parameterValues'": "{0: {'values': {'maxValue': '2024-05-02T18:36:22.864980'}}, 1: {'values': "*

 * *                      "{'maxValue': '2024-05-02T18:36:22.864980'}}, 2: {'values': {'maxValue': "*

 * *                      "'2024-04-24T21:02:32.111500'}}, 3: {'values': {'maxValue': "*

 * *                      "'2024-04-24T21:02:32.111500'}}, 7: {'values': {'minValue': "*

 * *                      "0.01695005847191685}}, 8: {'values': {'minValue': 0.01695005847191685}}, "*

 * *                      "11: {'values': {'maxValue': […]*

```diff
@@ -1,34 +1,34 @@
 {
     "parameterValues": [
         {
             "parameterName": "createDateMin",
             "values": {
-                "maxValue": "2024-01-27T16:18:31.564623",
+                "maxValue": "2024-05-02T18:36:22.864980",
                 "minValue": "2022-12-08T19:07:55.038280"
             }
         },
         {
             "parameterName": "createDateMax",
             "values": {
-                "maxValue": "2024-01-27T16:18:31.564623",
+                "maxValue": "2024-05-02T18:36:22.864980",
                 "minValue": "2022-12-08T19:07:55.038280"
             }
         },
         {
             "parameterName": "endTimeMin",
             "values": {
-                "maxValue": "2023-11-01T20:51:20.287000",
+                "maxValue": "2024-04-24T21:02:32.111500",
                 "minValue": "2022-02-23T20:48:55.393500"
             }
         },
         {
             "parameterName": "endTimeMax",
             "values": {
-                "maxValue": "2023-11-01T20:51:20.287000",
+                "maxValue": "2024-04-24T21:02:32.111500",
                 "minValue": "2022-02-23T20:48:55.393500"
             }
         },
         {
             "parameterName": "exposureTimeMin",
             "values": {
                 "maxValue": 1380.2332394366197,
@@ -51,22 +51,22 @@
                 ]
             }
         },
         {
             "parameterName": "qualityAverageFriedParameterMin",
             "values": {
                 "maxValue": 2.6520787500175156e+30,
-                "minValue": 0.027724481746640606
+                "minValue": 0.01695005847191685
             }
         },
         {
             "parameterName": "qualityAverageFriedParameterMax",
             "values": {
                 "maxValue": 2.6520787500175156e+30,
-                "minValue": 0.027724481746640606
+                "minValue": 0.01695005847191685
             }
         },
         {
             "parameterName": "qualityAveragePolarimetricAccuracyMin",
             "values": {
                 "maxValue": 1.3227079486518465,
                 "minValue": 0.7510039715379637
@@ -78,33 +78,35 @@
                 "maxValue": 1.3227079486518465,
                 "minValue": 0.7510039715379637
             }
         },
         {
             "parameterName": "startTimeMin",
             "values": {
-                "maxValue": "2023-11-01T19:53:02.868500",
+                "maxValue": "2024-04-24T20:38:33.709500",
                 "minValue": "2022-02-23T19:05:32.338002"
             }
         },
         {
             "parameterName": "startTimeMax",
             "values": {
-                "maxValue": "2023-11-01T19:53:02.868500",
+                "maxValue": "2024-04-24T20:38:33.709500",
                 "minValue": "2022-02-23T19:05:32.338002"
             }
         },
         {
             "parameterName": "targetTypes",
             "values": {
                 "categoricalValues": [
+                    "coronalhole",
+                    "sunspot",
                     "spicules",
                     "quietsun",
-                    "unknown",
-                    "sunspot"
+                    "plages",
+                    "unknown"
                 ]
             }
         },
         {
             "parameterName": "averageDatasetSpectralSamplingMin",
             "values": {
                 "maxValue": 0.002011144047143148,
@@ -146,25 +148,26 @@
                 "minValue": 9.139999999997528
             }
         },
         {
             "parameterName": "highLevelSoftwareVersion",
             "values": {
                 "categoricalValues": [
+                    "Alakai_11.1.0",
+                    "Alakai_6-0",
+                    "Alakai_8-0",
+                    "Alakai_10-0",
+                    "Alakai_7-0",
+                    "Pono_6.1.5",
                     "Pono_2.1.0",
                     "Pono_1.0.0",
                     "Alakai_5-1",
                     "Pono_3.1.0",
                     "Alakai_3-0",
-                    "Alakai_4-0",
-                    "Alakai_11.1.0",
-                    "Alakai_6-0",
-                    "Alakai_8-0",
-                    "Alakai_10-0",
-                    "Alakai_7-0"
+                    "Alakai_4-0"
                 ]
             }
         },
         {
             "parameterName": "workflowName",
             "values": {
                 "categoricalValues": [
@@ -173,62 +176,68 @@
                 ]
             }
         },
         {
             "parameterName": "workflowVersion",
             "values": {
                 "categoricalValues": [
-                    "1.4.11",
+                    "2.7.4",
+                    "2.10.3",
+                    "1.1.7",
+                    "0.16.0",
+                    "1.1.10",
+                    "2.7.2",
+                    "2.10.15",
+                    "2.7.0",
                     "2.10.1",
                     "2.0.2",
+                    "2.10.12",
                     "2.7.3",
-                    "1.4.1",
                     "1.1.5",
-                    "1.2.0",
-                    "2.10.2",
-                    "2.7.4",
                     "2.6.1",
                     "1.2.1",
+                    "2.10.13",
                     "2.7.5",
-                    "2.10.3",
-                    "1.1.7",
                     "2.0.1",
-                    "0.16.0",
                     "1.4.8",
+                    "1.8.2",
                     "2.9.0",
+                    "2.10.7",
                     "2.3.1",
                     "2.3.0",
                     "2.10.0",
-                    "1.1.10",
-                    "2.7.2",
                     "1.0.0",
-                    "2.7.0"
+                    "1.4.11",
+                    "1.4.1",
+                    "1.2.0",
+                    "2.10.2"
                 ]
             }
         },
         {
             "parameterName": "headerDataUnitCreationDateMin",
             "values": {
-                "maxValue": "2024-01-27T14:17:20.001000",
+                "maxValue": "2024-05-02T16:56:14.521000",
                 "minValue": "2022-12-08T17:25:51.965000"
             }
         },
         {
             "parameterName": "headerDataUnitCreationDateMax",
             "values": {
-                "maxValue": "2024-01-27T14:17:20.001000",
+                "maxValue": "2024-05-02T16:56:14.521000",
                 "minValue": "2022-12-08T17:25:51.965000"
             }
         },
         {
             "parameterName": "headerVersion",
             "values": {
                 "categoricalValues": [
                     "3.6.0",
                     "4.0.0",
+                    "4.1.1",
                     "3.3.0",
                     "3.0.0",
                     "3.4.0",
                     "3.9.0",
                     "3.5.0",
                     "3.7.1",
                     "3.8.1"
```

### Comparing `dkist-1.5.0rc1/dkist/data/test/5d_gwcs.asdf` & `dkist-1.6.0/dkist/data/test/5d_gwcs.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/AGLKO-inv.ecsv` & `dkist-1.6.0/dkist/data/test/AGLKO-inv.ecsv`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.000010_s.fits` & `dkist-1.6.0/dkist/data/test/EIT/efz20040301.000010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.020010_s.fits` & `dkist-1.6.0/dkist/data/test/EIT/efz20040301.020010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.030011_s.fits` & `dkist-1.6.0/dkist/data/test/EIT/efz20040301.030011_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.040010_s.fits` & `dkist-1.6.0/dkist/data/test/EIT/efz20040301.040010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.050010_s.fits` & `dkist-1.6.0/dkist/data/test/EIT/efz20040301.050010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.060010_s.fits` & `dkist-1.6.0/dkist/data/test/EIT/efz20040301.060010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.080010_s.fits` & `dkist-1.6.0/dkist/data/test/EIT/efz20040301.080010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.090010_s.fits` & `dkist-1.6.0/dkist/data/test/EIT/efz20040301.090010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.100010_s.fits` & `dkist-1.6.0/dkist/data/test/EIT/efz20040301.100010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.110010_s.fits` & `dkist-1.6.0/dkist/data/test/EIT/efz20040301.110010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/EIT/efz20040301.120010_s.fits` & `dkist-1.6.0/dkist/data/test/EIT/efz20040301.120010_s.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/EIT/eit_test_dataset.asdf` & `dkist-1.6.0/dkist/data/test/EIT/eit_test_dataset.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/eit_dataset-0.1.0.asdf` & `dkist-1.6.0/dkist/data/test/eit_dataset-0.1.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/eit_dataset-0.2.0.asdf` & `dkist-1.6.0/dkist/data/test/eit_dataset-0.2.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/eit_dataset-0.3.0.asdf` & `dkist-1.6.0/dkist/data/test/eit_dataset-0.3.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/eit_dataset-1.0.0.asdf` & `dkist-1.6.0/dkist/data/test/eit_dataset-1.0.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/eit_dataset-1.1.0.asdf` & `dkist-1.6.0/dkist/data/test/eit_dataset-1.1.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/eit_dataset-1.2.0.asdf` & `dkist-1.6.0/dkist/data/test/eit_dataset-1.2.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/globus_operation_ls_response.json` & `dkist-1.6.0/dkist/data/test/globus_operation_ls_response.json`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/globus_search_response.json` & `dkist-1.6.0/dkist/data/test/globus_search_response.json`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/large_visp.asdf.gz` & `dkist-1.6.0/dkist/data/test/large_visp.asdf.gz`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/small_visp/0.fits` & `dkist-1.6.0/dkist/data/test/small_visp/0.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/small_visp/1.fits` & `dkist-1.6.0/dkist/data/test/small_visp/1.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/small_visp/2.fits` & `dkist-1.6.0/dkist/data/test/small_visp/2.fits`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/small_visp/test_visp.asdf` & `dkist-1.6.0/dkist/data/test/small_visp/test_visp.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/test_old_wcs_BRMQY.asdf` & `dkist-1.6.0/dkist/data/test/test_old_wcs_BRMQY.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.0.0.asdf` & `dkist-1.6.0/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.0.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.1.0.asdf` & `dkist-1.6.0/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.1.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.2.0.asdf` & `dkist-1.6.0/dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.2.0.asdf`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/dataset/dataset.py` & `dkist-1.6.0/dkist/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/dataset/loader.py` & `dkist-1.6.0/dkist/dataset/loader.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/dataset/tests/test_dataset.py` & `dkist-1.6.0/dkist/dataset/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/dataset/tests/test_load_dataset.py` & `dkist-1.6.0/dkist/dataset/tests/test_load_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/dataset/tests/test_plotting.py` & `dkist-1.6.0/dkist/dataset/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/dataset/tests/test_tiled_dataset.py` & `dkist-1.6.0/dkist/dataset/tests/test_tiled_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/dataset/tiled_dataset.py` & `dkist-1.6.0/dkist/dataset/tiled_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/dataset/utils.py` & `dkist-1.6.0/dkist/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/converters/dataset.py` & `dkist-1.6.0/dkist/io/asdf/converters/dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/converters/file_manager.py` & `dkist-1.6.0/dkist/io/asdf/converters/file_manager.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/converters/models.py` & `dkist-1.6.0/dkist/io/asdf/converters/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import astropy.units as u
 from asdf_astropy.converters.transform.core import TransformConverterBase, parameter_to_value
 
 
 class VaryingCelestialConverter(TransformConverterBase):
     tags = [
-        "asdf://dkist.nso.edu/tags/varying_celestial_transform-1.1.0",
-        "asdf://dkist.nso.edu/tags/varying_celestial_transform-1.0.0",
-        "asdf://dkist.nso.edu/tags/inverse_varying_celestial_transform-1.1.0",
-        "asdf://dkist.nso.edu/tags/inverse_varying_celestial_transform-1.0.0",
+        "asdf://dkist.nso.edu/tags/varying_celestial_transform-*",
+        "asdf://dkist.nso.edu/tags/inverse_varying_celestial_transform-*",
         # Old slit tags must be kept so we can read old files, but not types as
         # we will not save slit classes any more
         "asdf://dkist.nso.edu/tags/varying_celestial_transform_slit-1.0.0",
         "asdf://dkist.nso.edu/tags/inverse_varying_celestial_transform_slit-1.0.0",
     ]
     types = [
         "dkist.wcs.models.VaryingCelestialTransform",
@@ -19,18 +17,21 @@
         "dkist.wcs.models.VaryingCelestialTransform2D",
         "dkist.wcs.models.InverseVaryingCelestialTransform2D",
         "dkist.wcs.models.VaryingCelestialTransform3D",
         "dkist.wcs.models.InverseVaryingCelestialTransform3D",
     ]
 
     def select_tag(self, obj, tags, ctx):
+        tag_pattern = "asdf://dkist.nso.edu/tags/varying_celestial_transform"
         if obj._is_inverse:
-            return "asdf://dkist.nso.edu/tags/inverse_varying_celestial_transform-1.1.0"
+            tag_pattern = "asdf://dkist.nso.edu/tags/inverse_varying_celestial_transform"
 
-        return "asdf://dkist.nso.edu/tags/varying_celestial_transform-1.1.0"
+        for tag in tags:
+            if tag.startswith(tag_pattern):
+                return tag
 
     def from_yaml_tree_transform(self, node, tag, ctx):
         from dkist.wcs.models import varying_celestial_transform_from_tables
 
         inverse = False
         if "inverse_varying_celestial_transform" in tag:
             inverse = True
@@ -70,15 +71,15 @@
 
 
 class CoupledCompoundConverter(TransformConverterBase):
     """
     ASDF serialization support for CompoundModel.
     """
     tags = [
-        "asdf://dkist.nso.edu/tags/coupled_compound_model-1.0.0",
+        "asdf://dkist.nso.edu/tags/coupled_compound_model-*",
     ]
 
     types = ["dkist.wcs.models.CoupledCompoundModel"]
 
     def to_yaml_tree_transform(self, model, tag, ctx):
         left = model.left
 
@@ -118,15 +119,15 @@
 
 class RavelConverter(TransformConverterBase):
     """
     ASDF serialization support for Ravel
     """
 
     tags  = [
-        "asdf://dkist.nso.edu/tags/ravel_model-1.0.0"
+        "asdf://dkist.nso.edu/tags/ravel_model-*"
     ]
 
     types = ["dkist.wcs.models.Ravel"]
 
     def to_yaml_tree_transform(self, model, tag, ctx):
         return {"array_shape": model.array_shape, "order": model.order}
 
@@ -138,15 +139,15 @@
 
 class AsymmetricMappingConverter(TransformConverterBase):
     """
     ASDF serialization support for Ravel
     """
 
     tags  = [
-        "asdf://dkist.nso.edu/tags/asymmetric_mapping_model-1.0.0"
+        "asdf://dkist.nso.edu/tags/asymmetric_mapping_model-*"
     ]
 
     types = ["dkist.wcs.models.AsymmetricMapping"]
 
     def to_yaml_tree_transform(self, model, tag, ctx):
         node = {
             "forward_mapping": model.forward_mapping,
```

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/converters/tiled_dataset.py` & `dkist-1.6.0/dkist/io/asdf/converters/tiled_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/entry_points.py` & `dkist-1.6.0/dkist/io/asdf/entry_points.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,16 @@
     return [
         ManifestExtension.from_uri("asdf://dkist.nso.edu/manifests/dkist-1.2.0",
                                    converters=dkist_converters),
         ManifestExtension.from_uri("asdf://dkist.nso.edu/manifests/dkist-1.1.0",
                                    converters=dkist_converters),
         ManifestExtension.from_uri("asdf://dkist.nso.edu/manifests/dkist-1.0.0",
                                    converters=dkist_converters),
+        ManifestExtension.from_uri("asdf://dkist.nso.edu/manifests/dkist-wcs-1.3.0",
+                                   converters=wcs_converters),
         ManifestExtension.from_uri("asdf://dkist.nso.edu/manifests/dkist-wcs-1.2.0",
                                    converters=wcs_converters),
         ManifestExtension.from_uri("asdf://dkist.nso.edu/manifests/dkist-wcs-1.1.0",
                                    converters=wcs_converters),
         ManifestExtension.from_uri("asdf://dkist.nso.edu/manifests/dkist-wcs-1.0.0",
                                    converters=wcs_converters),
         # This manifest handles all pre-refactor tags
```

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-0.9.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/manifests/dkist-0.9.0.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 %YAML 1.1
 ---
-id: asdf://dkist.nso.edu/dkist/manifests/dkist-0.9.0
+id: asdf://dkist.nso.edu/manifests/dkist-0.9.0
 extension_uri: asdf://dkist.nso.edu/dkist/extensions/dkist-0.9.0
 title: DKIST extension
 description: ASDF schemas and tags for pre-1.0 DKIST tags.
 
 tags:
   - schema_uri: "asdf://dkist.nso.edu/schemas/file_manager-1.0.0"
     tag_uri: "tag:dkist.nso.edu:dkist/array_container-0.2.0"
```

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-1.0.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/manifests/dkist-1.0.0.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 %YAML 1.1
 ---
-id: asdf://dkist.nso.edu/dkist/manifests/dkist-1.0.0
+id: asdf://dkist.nso.edu/manifests/dkist-1.0.0
 extension_uri: asdf://dkist.nso.edu/dkist/extensions/dkist-1.0.0
 title: DKIST extension
 description: ASDF schemas and tags for DKIST classes.
 
 tags:
   - schema_uri: "asdf://dkist.nso.edu/schemas/file_manager-1.0.0"
     tag_uri: "asdf://dkist.nso.edu/tags/file_manager-1.0.0"
```

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-1.1.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/manifests/dkist-1.1.0.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 %YAML 1.1
 ---
-id: asdf://dkist.nso.edu/dkist/manifests/dkist-1.1.0
-extension_uri: asdf://dkist.nso.edu/dkist/extensions/dkist-1.0.0
+id: asdf://dkist.nso.edu/manifests/dkist-1.1.0
+extension_uri: asdf://dkist.nso.edu/dkist/extensions/dkist-1.1.0
 title: DKIST extension
 description: ASDF schemas and tags for DKIST classes.
 
 tags:
   - schema_uri: "asdf://dkist.nso.edu/schemas/file_manager-1.0.0"
     tag_uri: "asdf://dkist.nso.edu/tags/file_manager-1.0.0"
   - schema_uri: "asdf://dkist.nso.edu/schemas/dataset-1.1.0"
```

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-1.2.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/manifests/dkist-1.2.0.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 %YAML 1.1
 ---
-id: asdf://dkist.nso.edu/dkist/manifests/dkist-1.2.0
-extension_uri: asdf://dkist.nso.edu/dkist/extensions/dkist-1.0.0
+id: asdf://dkist.nso.edu/manifests/dkist-1.2.0
+extension_uri: asdf://dkist.nso.edu/dkist/extensions/dkist-1.2.0
 title: DKIST extension
 description: ASDF schemas and tags for DKIST classes.
 
 tags:
   - schema_uri: "asdf://dkist.nso.edu/schemas/file_manager-1.0.0"
     tag_uri: "asdf://dkist.nso.edu/tags/file_manager-1.0.0"
   - schema_uri: "asdf://dkist.nso.edu/schemas/dataset-1.1.0"
```

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-wcs-1.0.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/manifests/dkist-wcs-1.1.0.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 %YAML 1.1
 ---
-id: asdf://dkist.nso.edu/dkist/manifests/dkist-wcs-1.0.0
-extension_uri: asdf://dkist.nso.edu/dkist/extensions/dkist-wcs-1.0.0
+id: asdf://dkist.nso.edu/manifests/dkist-wcs-1.1.0
+extension_uri: asdf://dkist.nso.edu/dkist/extensions/dkist-wcs-1.1.0
 title: DKIST WCS extension
 description: ASDF schemas and tags for models and WCS related classes.
 
 tags:
   - schema_uri: "asdf://dkist.nso.edu/schemas/varying_celestial_transform-1.0.0"
     tag_uri: "asdf://dkist.nso.edu/tags/varying_celestial_transform-1.0.0"
   - schema_uri: "asdf://dkist.nso.edu/schemas/varying_celestial_transform-1.0.0"
     tag_uri: "asdf://dkist.nso.edu/tags/inverse_varying_celestial_transform-1.0.0"
   - schema_uri: "asdf://dkist.nso.edu/schemas/coupled_compound_model-1.0.0"
     tag_uri: "asdf://dkist.nso.edu/tags/coupled_compound_model-1.0.0"
   - schema_uri: "asdf://dkist.nso.edu/schemas/varying_celestial_transform-1.0.0"
     tag_uri: "asdf://dkist.nso.edu/tags/varying_celestial_transform_slit-1.0.0"
   - schema_uri: "asdf://dkist.nso.edu/schemas/varying_celestial_transform-1.0.0"
     tag_uri: "asdf://dkist.nso.edu/tags/inverse_varying_celestial_transform_slit-1.0.0"
+  - schema_uri: "asdf://dkist.nso.edu/schemas/ravel_model-1.0.0"
+    tag_uri: "asdf://dkist.nso.edu/tags/ravel_model-1.0.0"
```

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-wcs-1.1.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/manifests/dkist-wcs-1.0.0.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 %YAML 1.1
 ---
-id: asdf://dkist.nso.edu/dkist/manifests/dkist-wcs-1.1.0
-extension_uri: asdf://dkist.nso.edu/dkist/extensions/dkist-wcs-1.1.0
+id: asdf://dkist.nso.edu/manifests/dkist-wcs-1.0.0
+extension_uri: asdf://dkist.nso.edu/dkist/extensions/dkist-wcs-1.0.0
 title: DKIST WCS extension
 description: ASDF schemas and tags for models and WCS related classes.
 
 tags:
   - schema_uri: "asdf://dkist.nso.edu/schemas/varying_celestial_transform-1.0.0"
     tag_uri: "asdf://dkist.nso.edu/tags/varying_celestial_transform-1.0.0"
   - schema_uri: "asdf://dkist.nso.edu/schemas/varying_celestial_transform-1.0.0"
     tag_uri: "asdf://dkist.nso.edu/tags/inverse_varying_celestial_transform-1.0.0"
   - schema_uri: "asdf://dkist.nso.edu/schemas/coupled_compound_model-1.0.0"
     tag_uri: "asdf://dkist.nso.edu/tags/coupled_compound_model-1.0.0"
   - schema_uri: "asdf://dkist.nso.edu/schemas/varying_celestial_transform-1.0.0"
     tag_uri: "asdf://dkist.nso.edu/tags/varying_celestial_transform_slit-1.0.0"
   - schema_uri: "asdf://dkist.nso.edu/schemas/varying_celestial_transform-1.0.0"
     tag_uri: "asdf://dkist.nso.edu/tags/inverse_varying_celestial_transform_slit-1.0.0"
-  - schema_uri: "asdf://dkist.nso.edu/schemas/ravel_model-1.0.0"
-    tag_uri: "asdf://dkist.nso.edu/tags/ravel_model-1.0.0"
```

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/manifests/dkist-wcs-1.2.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/manifests/dkist-wcs-1.2.0.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 %YAML 1.1
 ---
-id: asdf://dkist.nso.edu/dkist/manifests/dkist-wcs-1.2.0
+id: asdf://dkist.nso.edu/manifests/dkist-wcs-1.2.0
 extension_uri: asdf://dkist.nso.edu/dkist/extensions/dkist-wcs-1.2.0
 title: DKIST WCS extension
 description: ASDF schemas and tags for models and WCS related classes.
 
 tags:
   - schema_uri: "asdf://dkist.nso.edu/schemas/varying_celestial_transform-1.0.0"
     tag_uri: "asdf://dkist.nso.edu/tags/varying_celestial_transform-1.1.0"
```

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/asymmetric_mapping_model-1.0.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/schemas/asymmetric_mapping_model-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/coupled_compound_model-1.0.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/schemas/coupled_compound_model-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-0.1.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/schemas/dataset-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-0.2.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/schemas/dataset-0.2.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-0.3.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/schemas/dataset-0.3.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-1.0.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/schemas/dataset-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/dataset-1.1.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/schemas/dataset-1.1.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/file_manager-1.0.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/schemas/file_manager-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/ravel_model-1.0.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/schemas/ravel_model-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/tiled_dataset-0.1.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/schemas/tiled_dataset-0.1.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/tiled_dataset-1.0.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/schemas/tiled_dataset-1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/resources/schemas/varying_celestial_transform-1.0.0.yaml` & `dkist-1.6.0/dkist/io/asdf/resources/schemas/varying_celestial_transform-1.1.0.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 %YAML 1.1
 ---
 $schema: "http://stsci.edu/schemas/yaml-schema/draft-01"
-id: "asdf://dkist.nso.edu/schemas/varying_celestial_transform-1.0.0"
+id: "asdf://dkist.nso.edu/schemas/varying_celestial_transform-1.1.0"
 
 title: A varying FITS-like celestial transform.
 description:
   A model which represents a FITS-like celestial WCS transform which varies over a third pixel input.
 
 allOf:
-  - $ref: "http://stsci.edu/schemas/asdf/transform/transform-1.2.0"
+  - $ref: "http://stsci.edu/schemas/asdf/transform/transform-1.3.0"
   - properties:
       crpix:
         anyOf:
-          - tag: "core/ndarray-1.*"
+          - tag: "tag:stsci.edu:asdf/core/ndarray-1.*"
           - tag: "tag:stsci.edu:asdf/unit/quantity-1.*"
       cdelt:
         anyOf:
-          - tag: "core/ndarray-1.*"
+          - tag: "tag:stsci.edu:asdf/core/ndarray-1.*"
           - tag: "tag:stsci.edu:asdf/unit/quantity-1.*"
       lon_pole:
         anyOf:
           - type: number
           - tag: "tag:stsci.edu:asdf/unit/quantity-1.*"
       crval_table:
         anyOf:
-          - tag: "core/ndarray-1.*"
+          - tag: "tag:stsci.edu:asdf/core/ndarray-1.*"
           - tag: "tag:stsci.edu:asdf/unit/quantity-1.*"
       pc_table:
         anyOf:
-          - tag: "core/ndarray-1.*"
+          - tag: "tag:stsci.edu:asdf/core/ndarray-1.*"
           - tag: "tag:stsci.edu:asdf/unit/quantity-1.*"
       projection:
-        $ref: "http://stsci.edu/schemas/asdf/transform/transform-1.2.0"
+        $ref: "http://stsci.edu/schemas/asdf/transform/transform-1.3.0"
 
     required: [crpix, cdelt, lon_pole, crval_table, pc_table, projection]
     additionalProperties: true
 ...
```

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/tests/conftest.py` & `dkist-1.6.0/dkist/io/asdf/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/tests/test_dataset.py` & `dkist-1.6.0/dkist/io/asdf/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/tests/test_models.py` & `dkist-1.6.0/dkist/io/asdf/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/asdf/tests/test_tiled_dataset.py` & `dkist-1.6.0/dkist/io/asdf/tests/test_tiled_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/dask_utils.py` & `dkist-1.6.0/dkist/io/dask_utils.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/file_manager.py` & `dkist-1.6.0/dkist/io/file_manager.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/level_1_dataset_schema.yaml` & `dkist-1.6.0/dkist/io/level_1_dataset_schema.yaml`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/loaders.py` & `dkist-1.6.0/dkist/io/loaders.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/tests/test_file_manager.py` & `dkist-1.6.0/dkist/io/tests/test_file_manager.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/io/tests/test_fits.py` & `dkist-1.6.0/dkist/io/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/logger.py` & `dkist-1.6.0/dkist/logger.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/__init__.py` & `dkist-1.6.0/dkist/net/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/attr_walker.py` & `dkist-1.6.0/dkist/net/attr_walker.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/attrs.py` & `dkist-1.6.0/dkist/net/attrs.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/attrs_values.py` & `dkist-1.6.0/dkist/net/attrs_values.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/client.py` & `dkist-1.6.0/dkist/net/client.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/globus/auth.py` & `dkist-1.6.0/dkist/net/globus/auth.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/globus/endpoints.py` & `dkist-1.6.0/dkist/net/globus/endpoints.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/globus/tests/conftest.py` & `dkist-1.6.0/dkist/net/globus/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/globus/tests/test_auth.py` & `dkist-1.6.0/dkist/net/globus/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/globus/tests/test_endpoints.py` & `dkist-1.6.0/dkist/net/globus/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/globus/tests/test_transfer.py` & `dkist-1.6.0/dkist/net/globus/tests/test_transfer.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/globus/transfer.py` & `dkist-1.6.0/dkist/net/globus/transfer.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/helpers.py` & `dkist-1.6.0/dkist/net/helpers.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/tests/conftest.py` & `dkist-1.6.0/dkist/net/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/tests/strategies.py` & `dkist-1.6.0/dkist/net/tests/strategies.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/tests/test_attr_walker.py` & `dkist-1.6.0/dkist/net/tests/test_attr_walker.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/tests/test_attrs.py` & `dkist-1.6.0/dkist/net/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/tests/test_attrs_values.py` & `dkist-1.6.0/dkist/net/tests/test_attrs_values.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/tests/test_client.py` & `dkist-1.6.0/dkist/net/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/net/tests/test_helpers.py` & `dkist-1.6.0/dkist/net/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/tests/generate_aia_dataset.py` & `dkist-1.6.0/dkist/tests/generate_aia_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/tests/generate_eit_test_dataset.py` & `dkist-1.6.0/dkist/tests/generate_eit_test_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/tests/generate_eit_tiled_dataset.py` & `dkist-1.6.0/dkist/tests/generate_eit_tiled_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/tests/test_logger.py` & `dkist-1.6.0/dkist/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/utils/_model_to_graphviz.py` & `dkist-1.6.0/dkist/utils/_model_to_graphviz.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/utils/inventory.py` & `dkist-1.6.0/dkist/utils/inventory.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/utils/sysinfo.py` & `dkist-1.6.0/dkist/utils/sysinfo.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/utils/tests/test_inventory.py` & `dkist-1.6.0/dkist/utils/tests/test_inventory.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/version.py` & `dkist-1.6.0/dkist/version.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/wcs/models.py` & `dkist-1.6.0/dkist/wcs/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,21 +46,21 @@
     all must have units, if parameters are unitless they are assumed to be in
     degrees.
 
     Parameters
     ----------
     crpix
         The reference pixel (a length two array).
-    crval
-        The world coordinate at the reference pixel (a length two array).
     cdelt
         The sample interval along the pixel axis
     pc
         The rotation matrix for the affine transform. If specifying parameters
         with units this should have celestial (``u.deg``) units.
+    crval
+        The world coordinate at the reference pixel (a length two array).
     lon_pole
         The longitude of the celestial pole, defaults to 180 degrees.
     projection
         The map projection to use, defaults to ``TAN``.
 
     Notes
     -----
@@ -93,23 +93,71 @@
     shift = m.Shift(-crpix[0]) & m.Shift(-crpix[1])
     scale = m.Multiply(cdelt[0]) & m.Multiply(cdelt[1])
     rot = m.AffineTransformation2D(pc, translation=translation)
     skyrot = m.RotateNative2Celestial(crval[0], crval[1], lon_pole)
     return shift | rot | scale | projection | skyrot
 
 
+def update_celestial_transform_parameters(
+        transform,
+        crpix: Iterable[float] | u.Quantity,
+        cdelt: Iterable[float] | u.Quantity,
+        pc: ArrayLike | u.Quantity,
+        crval: Iterable[float] | u.Quantity,
+        lon_pole: float | u.Quantity,
+) -> CompoundModel:
+    """
+    Update an existing transform with new parameter values.
+
+    .. warning::
+        This assumes that the type (quantity vs not quantity) and units of the
+        new parameters are valid for the model.
+
+    Parameters
+    ----------
+    crpix
+        The reference pixel (a length two array).
+    cdelt
+        The sample interval along the pixel axis
+    pc
+        The rotation matrix for the affine transform. If specifying parameters
+        with units this should have celestial (``u.deg``) units.
+    crval
+        The world coordinate at the reference pixel (a length two array).
+    lon_pole
+        The longitude of the celestial pole, defaults to 180 degrees.
+    """
+    new_params = [
+        -crpix[0],
+        -crpix[1],
+        pc,
+        transform[2].translation.value,
+        cdelt[0],
+        cdelt[1],
+        crval[0],
+        crval[1],
+        lon_pole
+    ]
+
+    for name, val in zip(transform.param_names, new_params):
+        setattr(transform, name, val)
+
+    return transform
+
+
 class BaseVaryingCelestialTransform(Model, ABC):
     """
     Shared components between the forward and reverse varying celestial transforms.
     """
 
     # This prevents Model from broadcasting the parameters to the inputs
     standard_broadcasting = False
     _separable = False
     _input_units_allow_dimensionless = True
+    _input_units_strict = True
     _is_inverse = False
 
     crpix = Parameter()
     cdelt = Parameter()
     lon_pole = Parameter(default=180)
 
     n_outputs = 2
@@ -165,68 +213,110 @@
         else:
             self.inputs = ("x", "y", "z", "q", "m")[:self.n_inputs]
             self.outputs = ("lon", "lat")
 
         if len(self.table_shape) != self.n_inputs-2:
             raise ValueError(f"This model can only be constructed with a {self.n_inputs-2}-dimensional lookup table.")
 
+        self._transform = generate_celestial_transform(
+            crpix=[0, 0],
+            cdelt=[1, 1],
+            pc=np.identity(2),
+            crval=[0, 0],
+            lon_pole=180,
+            projection=projection,
+        )
+
     def transform_at_index(self, ind, crpix=None, cdelt=None, lon_pole=None):
         """
         Generate a spatial model based on an index for the pc and crval tables.
 
         Parameters
         ----------
         zind : int
-          The index to the lookup table.Q
+          The index to the lookup table.
 
         **kwargs
           The keyword arguments are optional and if not specified will be read
           from the parameters to this model.
 
         Returns
         -------
         `astropy.modeling.CompoundModel`
 
         """
-        # If we are being called from inside evaluate we can skip the lookup
-        crpix = crpix if crpix is not None else self.crpix
-        cdelt = cdelt if cdelt is not None else self.cdelt
-        lon_pole = lon_pole if lon_pole is not None else self.lon_pole
-
+        # If we are out of bounds of the lookup table return a constant model
         fill_val = np.nan
-        if isinstance(crpix, u.Quantity):
-            fill_val = np.nan * u.deg
         if (np.array(ind) > np.array(self.table_shape) - 1).any() or (np.array(ind) < 0).any():
             return m.Const1D(fill_val) & m.Const1D(fill_val)
 
-        return generate_celestial_transform(
+        # The self._transform is always unitless and always in degrees.
+        # So we need to strip down the parameters to be in the correct units
+
+        # If we are being called from inside evaluate we can skip the lookup
+        # but we have to handle both dimensionless and unitful parameters
+        if crpix is None:
+            if self.crpix.unit is not None:
+                crpix = u.Quantity(self.crpix)
+            else:
+                crpix = self.crpix.value
+        if cdelt is None:
+            if self.cdelt.unit is not None:
+                cdelt = u.Quantity(self.cdelt)
+            else:
+                cdelt = self.cdelt.value
+        if lon_pole is None:
+            if self.lon_pole.unit is not None:
+                lon_pole = u.Quantity(self.lon_pole)
+            else:
+                lon_pole = self.lon_pole.value
+
+        if isinstance(self.pc_table, u.Quantity):
+            pc = self.pc_table[ind].to_value(u.pix)
+        else:
+            pc = self.pc_table[ind]
+
+        if isinstance(self.crval_table, u.Quantity):
+            crval = self.crval_table[ind].to_value(u.deg)
+        else:
+            crval = self.crval_table[ind]
+
+        if isinstance(crpix, u.Quantity):
+            crpix = crpix.to_value(u.pix)
+
+        if isinstance(cdelt, u.Quantity):
+            cdelt = cdelt.to_value(u.deg / u.pix)
+
+        if isinstance(lon_pole, u.Quantity):
+            lon_pole = lon_pole.to_value(u.deg)
+
+        return update_celestial_transform_parameters(
+            self._transform,
             crpix=crpix,
             cdelt=cdelt,
-            pc=self.pc_table[ind],
-            crval=self.crval_table[ind],
+            pc=pc,
+            crval=crval,
             lon_pole=lon_pole,
-            projection=self.projection,
         )
 
-
     def _map_transform(self, *arrays, crpix, cdelt, lon_pole, inverse=False):
         # We need to broadcast the arrays together so they are all the same shape
         barrays = np.broadcast_arrays(*arrays, subok=True)
         # # Convert the z, q, and m coordinates where present into indices to the lookup tables
         inds = []
         for barray in barrays[2:]:
             inds.append(self.sanitize_index(barray))
 
-        # Generate output arrays (ignore units for simplicity)
         if isinstance(barrays[0], u.Quantity):
-            x_out = np.empty_like(barrays[0].value)
-            y_out = np.empty_like(barrays[1].value)
-        else:
-            x_out = np.empty_like(barrays[0])
-            y_out = np.empty_like(barrays[1])
+            # Because we have set input_units_strict to True we can assume that
+            # all inputs have the correct units for the transform
+            arrays = [arr.value for arr in barrays]
+
+        x_out = np.empty_like(arrays[0])
+        y_out = np.empty_like(arrays[1])
 
         # We now loop over every unique value of z and compute the transform.
         # This means we make the minimum number of calls possible to the transform.
         ranges = [np.unique(ind) for ind in inds]
         for ind in product(*ranges):
             # Scalar parameters are reshaped to be length one arrays by modeling
             sct = self.transform_at_index(ind, crpix=crpix[0], cdelt=cdelt[0], lon_pole=lon_pole[0])
@@ -234,27 +324,28 @@
             # Call this transform for all values of x, y where z == zind
             masks = [inds[i] == ind[i] for i in range(len(ind))]
             if len(masks) > 1:
                 mask = np.logical_and(*masks)
             else:
                 mask = masks[0]
             if inverse:
-                xx, yy = sct.inverse(barrays[0][mask], barrays[1][mask])
+                xx, yy = sct.inverse(arrays[0][mask], arrays[1][mask])
             else:
-                xx, yy = sct(barrays[0][mask], barrays[1][mask])
+                xx, yy = sct(arrays[0][mask], arrays[1][mask])
 
-            if isinstance(xx, u.Quantity):
-                x_out[mask], y_out[mask] = xx.value, yy.value
-            else:
-                x_out[mask], y_out[mask] = xx, yy
+            x_out[mask], y_out[mask] = xx, yy
 
-        # Put the units back
-        if isinstance(xx, u.Quantity):
-            x_out = x_out << xx.unit
-            y_out = y_out << yy.unit
+        # Put the units back if we started with some
+        if isinstance(barrays[0], u.Quantity):
+            if self._is_inverse:
+                x_out = x_out << u.pix
+                y_out = y_out << u.pix
+            else:
+                x_out = x_out << u.deg
+                y_out = y_out << u.deg
 
         return x_out, y_out
 
     def evaluate(self, *inputs):
         # This method has to be able to take an arbitrary number of arrays but also accept not being given kwargs
         # Fortunately we know how many arrays to expect from the number of inputs
         # Anything extra is therefore a kwarg
```

### Comparing `dkist-1.5.0rc1/dkist/wcs/tests/test_coupled_compound_model.py` & `dkist-1.6.0/dkist/wcs/tests/test_coupled_compound_model.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/dkist/wcs/tests/test_models.py` & `dkist-1.6.0/dkist/wcs/tests/test_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         crpix=(5, 5) * u.pix,
         cdelt=(1, 1) * u.arcsec/u.pix,
         crval_table=(0, 0) * u.arcsec,
         pc_table=varying_matrix_lt,
     )
     trans5 = vct.transform_at_index(5)
     assert isinstance(trans5, CompoundModel)
-    assert u.allclose(trans5.right.lon_pole, 180 * u.deg)
+    assert u.allclose(trans5.right.lon_pole, 180)
 
 
 def test_varying_transform_pc():
     varying_matrix_lt = [rotation_matrix(a)[:2, :2] for a in np.linspace(0, 90, 10)] * u.pix
 
     vct = VaryingCelestialTransform(
         crpix=(5, 5) * u.pix,
@@ -80,15 +80,15 @@
 
     trans5 = vct.transform_at_index(5)
     assert isinstance(trans5, CompoundModel)
 
     # Verify that we have the 5th matrix in the series
     affine = next(filter(lambda sm: isinstance(sm, m.AffineTransformation2D), trans5.traverse_postorder()))
     assert isinstance(affine, m.AffineTransformation2D)
-    assert u.allclose(affine.matrix, varying_matrix_lt[5])
+    assert u.allclose(affine.matrix, varying_matrix_lt[5].value)
     # x.shape=(1,), y.shape=(1,), z.shape=(1,)
     pixel = (0*u.pix, 0*u.pix, 5*u.pix)
     world = vct(*pixel)
     assert np.array(world[0]).shape == ()
     assert u.allclose(world, (359.99804329*u.deg, 0.00017119*u.deg))
     assert u.allclose(vct.inverse(*world, 5*u.pix), pixel[:2], atol=0.01*u.pix)
 
@@ -159,16 +159,16 @@
 
     trans2 = vct.transform_at_index(2)
     assert isinstance(trans2, CompoundModel)
 
     # Verify that we have the 2nd crval pair in the series
     crval1 = trans2.right.lon
     crval2 = trans2.right.lat
-    assert u.allclose(crval1, crval_table[2][0])
-    assert u.allclose(crval2, crval_table[2][1])
+    assert u.allclose(crval1, crval_table[2][0].to_value(u.deg))
+    assert u.allclose(crval2, crval_table[2][1].to_value(u.deg))
 
     pixel = (0*u.pix, 0*u.pix, 2*u.pix)
     world = vct(*pixel)
     assert u.allclose(world, (3.59999722e+02, 2.78325906e-13)*u.deg)
 
     assert u.allclose(vct.inverse(*world, 2*u.pix), pixel[:2], atol=0.01*u.pix)
 
@@ -270,15 +270,15 @@
 @pytest.mark.parametrize(("pixel", "lon_shape"), [
     ((*np.mgrid[0:5, 0:5] * u.pix, np.arange(5) * u.pix, 0 * u.pix), (5, 5)),
     (np.mgrid[0:10, 0:10, 0:5, 0:3] * u.pix, (10, 10, 5, 3)),
     ((2 * u.pix, 2 * u.pix, 0*u.pix, np.arange(3) * u.pix), (3,)),
     ((np.arange(10) * u.pix,
       np.arange(10) * u.pix,
       np.arange(5)[..., None] * u.pix,
-      np.arange(3)[..., None, None]), (3, 5, 10)),
+      np.arange(3)[..., None, None] * u.pix), (3, 5, 10)),
 ])
 def test_varying_transform_4d_pc_shapes(pixel, lon_shape):
     varying_matrix_lt = [rotation_matrix(a)[:2, :2] for a in np.linspace(0, 90, 15)] * u.pix
     varying_matrix_lt = varying_matrix_lt.reshape((5, 3, 2, 2))
 
     vct = VaryingCelestialTransform2D(
         crpix=(5, 5) * u.pix,
```

### Comparing `dkist-1.5.0rc1/dkist.egg-info/PKG-INFO` & `dkist-1.6.0/dkist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: dkist
-Version: 1.5.0rc1
+Version: 1.6.0
 Summary: DKIST User Tools
 Author-email: NSO / AURA <stuart@cadair.com>
 Project-URL: repository, https://github.com/DKISTDC/dkist
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE.rst
 Requires-Dist: aiohttp>=3.8
 Requires-Dist: asdf>=2.11.2
 Requires-Dist: asdf-astropy>=0.2.0
 Requires-Dist: asdf-coordinates-schemas>=0.1.0
 Requires-Dist: asdf-standard>=1.0.3
 Requires-Dist: asdf-transform-schemas>=0.3.0
-Requires-Dist: asdf-unit-schemas>=0.1.0
 Requires-Dist: asdf-wcs-schemas>=0.3.0
 Requires-Dist: astropy>=5.3
 Requires-Dist: dask[array]>=2021.8.0
 Requires-Dist: globus-sdk>=3.0
 Requires-Dist: gwcs>=0.19.0
 Requires-Dist: matplotlib>=3.5
 Requires-Dist: ndcube[plotting,reproject]>=2.0
@@ -31,14 +30,16 @@
 Requires-Dist: pytest-doctestplus; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-remotedata; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: pytest-mpl; extra == "tests"
 Requires-Dist: pytest-httpserver; extra == "tests"
+Requires-Dist: pytest-filter-subpackage; extra == "tests"
+Requires-Dist: pytest-benchmark; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Requires-Dist: tox; extra == "tests"
 Requires-Dist: pydot; extra == "tests"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-astropy; extra == "docs"
 Requires-Dist: sphinx-gallery; extra == "docs"
```

### Comparing `dkist-1.5.0rc1/dkist.egg-info/SOURCES.txt` & `dkist-1.6.0/dkist.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,25 +19,22 @@
 README.rst
 conftest.py
 pyproject.toml
 pytest.ini
 setup.cfg
 setup.py
 tox.ini
+.github/dependabot.yml
 .github/ISSUE_TEMPLATE/BUG_REPORT.md
 .github/ISSUE_TEMPLATE/FEATURE_REQUEST.md
 .github/ISSUE_TEMPLATE/config.yml
+.github/workflows/codspeed.yml
 .github/workflows/main.yml
 .github/workflows/prepare-release.yml
 .github/workflows/sub_package_update.yml
-changelog/309.bugfix.rst
-changelog/344.trivial.rst
-changelog/347.feature.rst
-changelog/349.doc.rst
-changelog/361.bugfix.rst
 changelog/README.rst
 dkist/__init__.py
 dkist/_version.py
 dkist/conftest.py
 dkist/dkist.cfg
 dkist/logger.py
 dkist/version.py
@@ -66,14 +63,15 @@
 dkist/data/test/globus_operation_ls_response.json
 dkist/data/test/globus_search_response.json
 dkist/data/test/large_visp.asdf.gz
 dkist/data/test/test_old_wcs_BRMQY.asdf
 dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.0.0.asdf
 dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.1.0.asdf
 dkist/data/test/test_tiled_dataset-1.0.0_dataset-1.2.0.asdf
+dkist/data/test/visp_no_headers.asdf.gz
 dkist/data/test/EIT/efz20040301.000010_s.fits
 dkist/data/test/EIT/efz20040301.020010_s.fits
 dkist/data/test/EIT/efz20040301.030011_s.fits
 dkist/data/test/EIT/efz20040301.040010_s.fits
 dkist/data/test/EIT/efz20040301.050010_s.fits
 dkist/data/test/EIT/efz20040301.060010_s.fits
 dkist/data/test/EIT/efz20040301.080010_s.fits
@@ -113,26 +111,31 @@
 dkist/io/asdf/resources/manifests/dkist-0.9.0.yaml
 dkist/io/asdf/resources/manifests/dkist-1.0.0.yaml
 dkist/io/asdf/resources/manifests/dkist-1.1.0.yaml
 dkist/io/asdf/resources/manifests/dkist-1.2.0.yaml
 dkist/io/asdf/resources/manifests/dkist-wcs-1.0.0.yaml
 dkist/io/asdf/resources/manifests/dkist-wcs-1.1.0.yaml
 dkist/io/asdf/resources/manifests/dkist-wcs-1.2.0.yaml
+dkist/io/asdf/resources/manifests/dkist-wcs-1.3.0.yaml
 dkist/io/asdf/resources/schemas/asymmetric_mapping_model-1.0.0.yaml
+dkist/io/asdf/resources/schemas/asymmetric_mapping_model-1.1.0.yaml
 dkist/io/asdf/resources/schemas/coupled_compound_model-1.0.0.yaml
+dkist/io/asdf/resources/schemas/coupled_compound_model-1.1.0.yaml
 dkist/io/asdf/resources/schemas/dataset-0.1.0.yaml
 dkist/io/asdf/resources/schemas/dataset-0.2.0.yaml
 dkist/io/asdf/resources/schemas/dataset-0.3.0.yaml
 dkist/io/asdf/resources/schemas/dataset-1.0.0.yaml
 dkist/io/asdf/resources/schemas/dataset-1.1.0.yaml
 dkist/io/asdf/resources/schemas/file_manager-1.0.0.yaml
 dkist/io/asdf/resources/schemas/ravel_model-1.0.0.yaml
+dkist/io/asdf/resources/schemas/ravel_model-1.1.0.yaml
 dkist/io/asdf/resources/schemas/tiled_dataset-0.1.0.yaml
 dkist/io/asdf/resources/schemas/tiled_dataset-1.0.0.yaml
 dkist/io/asdf/resources/schemas/varying_celestial_transform-1.0.0.yaml
+dkist/io/asdf/resources/schemas/varying_celestial_transform-1.1.0.yaml
 dkist/io/asdf/tests/__init__.py
 dkist/io/asdf/tests/conftest.py
 dkist/io/asdf/tests/test_dataset.py
 dkist/io/asdf/tests/test_models.py
 dkist/io/asdf/tests/test_tiled_dataset.py
 dkist/io/tests/__init__.py
 dkist/io/tests/test_file_manager.py
@@ -160,14 +163,15 @@
 dkist/net/tests/test_attrs_values.py
 dkist/net/tests/test_client.py
 dkist/net/tests/test_helpers.py
 dkist/tests/__init__.py
 dkist/tests/generate_aia_dataset.py
 dkist/tests/generate_eit_test_dataset.py
 dkist/tests/generate_eit_tiled_dataset.py
+dkist/tests/test_benchmarks.py
 dkist/tests/test_logger.py
 dkist/utils/__init__.py
 dkist/utils/_model_to_graphviz.py
 dkist/utils/decorators.py
 dkist/utils/exceptions.py
 dkist/utils/inventory.py
 dkist/utils/sysinfo.py
```

### Comparing `dkist-1.5.0rc1/docs/Makefile` & `dkist-1.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/conf.py` & `dkist-1.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/developer.rst` & `dkist-1.6.0/docs/developer.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/howto_guides/reproject_vbi_mosaic.md` & `dkist-1.6.0/docs/howto_guides/reproject_vbi_mosaic.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/index.rst` & `dkist-1.6.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/installation.rst` & `dkist-1.6.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/logo/icon_square.jpg` & `dkist-1.6.0/docs/logo/icon_square.jpg`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/make.bat` & `dkist-1.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/reference.rst` & `dkist-1.6.0/docs/reference.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/topic_guides/level1data.rst` & `dkist-1.6.0/docs/topic_guides/level1data.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/topic_guides/loading.rst` & `dkist-1.6.0/docs/topic_guides/loading.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/topic_guides/net.rst` & `dkist-1.6.0/docs/topic_guides/net.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/topic_guides/usertools.rst` & `dkist-1.6.0/docs/topic_guides/usertools.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/tutorial/1_astropy_and_sunpy.md` & `dkist-1.6.0/docs/tutorial/1_astropy_and_sunpy.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/tutorial/1_astropy_and_sunpy_NOTES.md` & `dkist-1.6.0/docs/tutorial/1_astropy_and_sunpy_NOTES.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/tutorial/2_search_and_asdf_download.md` & `dkist-1.6.0/docs/tutorial/2_search_and_asdf_download.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/tutorial/2_search_and_asdf_download_NOTES.md` & `dkist-1.6.0/docs/tutorial/2_search_and_asdf_download_NOTES.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/tutorial/3_the_dataset.md` & `dkist-1.6.0/docs/tutorial/3_the_dataset.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/tutorial/3_the_dataset_NOTES.md` & `dkist-1.6.0/docs/tutorial/3_the_dataset_NOTES.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/tutorial/4_more_dataset.md` & `dkist-1.6.0/docs/tutorial/4_more_dataset.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/tutorial/5_downloading_data.md` & `dkist-1.6.0/docs/tutorial/5_downloading_data.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/tutorial/6_visualization.md` & `dkist-1.6.0/docs/tutorial/6_visualization.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/tutorial/index.md` & `dkist-1.6.0/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/docs/whatsnew/1.0.rst` & `dkist-1.6.0/docs/whatsnew/1.0.rst`

 * *Files identical despite different names*

### Comparing `dkist-1.5.0rc1/pyproject.toml` & `dkist-1.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -18,20 +18,19 @@
   "aiohttp>=3.8",
   # Provide minimum deps for all asdf packages used to generate or read asdf
   # files so that we test with these minimums and also generate asdf's with
   # them
   # Some of these schema dependencies are minimums because we generated asdf
   # files with them unpinned so they are now required to read generated asdf
   # files.
-  "asdf>=2.11.2",  # Pick up jsonschema bug fix
+  "asdf>=2.11.2",
   "asdf-astropy>=0.2.0",
   "asdf-coordinates-schemas>=0.1.0",
   "asdf-standard>=1.0.3",
   "asdf-transform-schemas>=0.3.0",
-  "asdf-unit-schemas>=0.1.0",
   "asdf-wcs-schemas>=0.3.0",
   "astropy>=5.3",
   "dask[array]>=2021.8.0",
   "globus-sdk>=3.0",
   "gwcs>=0.19.0",
   "matplotlib>=3.5",
   "ndcube[plotting,reproject]>=2.0",
@@ -49,14 +48,16 @@
   "pytest-doctestplus",
   "pytest-cov",
   "pytest-remotedata",
   "pytest-cov",
   "pytest-mock",
   "pytest-mpl",
   "pytest-httpserver",
+  "pytest-filter-subpackage",
+  "pytest-benchmark",
   "hypothesis",
   "tox",
   "pydot",
 ]
 docs = [
   "sphinx",
   "sphinx-astropy",
```

### Comparing `dkist-1.5.0rc1/pytest.ini` & `dkist-1.6.0/pytest.ini`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 doctest_plus = enabled
 doctest_optionflags = NORMALIZE_WHITESPACE FLOAT_CMP ELLIPSIS
 text_file_format = rst
 addopts = --doctest-rst  -p no:unraisableexception -p no:threadexception
 markers =
     online: marks this test function as needing online connectivity.
     figure: marks this test function as using hash-based Matplotlib figure verification. This mark is not meant to be directly applied, but is instead automatically applied when a test function uses the @sunpy.tests.helpers.figure_test decorator.
+    benchmark: marks this test as a benchmark
 # Disable internet access for tests not marked remote_data
 remote_data_strict = True
 asdf_schema_root = dkist/io/asdf/resources/
 asdf_schema_tests_enabled = true
 filterwarnings =
     # Turn all warnings into errors so they do not pass silently.
     error
```

### Comparing `dkist-1.5.0rc1/tox.ini` & `dkist-1.6.0/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     tox-pypi-filter >= 0.14
 envlist =
     py{310,311,312}
     py312-devdeps
     py310-oldestdeps
     build_docs{,-notebooks}
     codestyle
+    benchmarks
 
 [testenv]
 pypi_filter = https://raw.githubusercontent.com/sunpy/sunpy/main/.test_package_pins.txt
 # Run the tests in a temporary directory to make sure that we don't import
 # the package from the source tree
 change_dir = .tmp/{envname}
 description =
@@ -30,15 +31,15 @@
     # If the user has set a LC override we should follow it
     LC_ALL
 set_env =
     MPLBACKEND = agg
     COLUMNS = 180
     devdeps: PIP_EXTRA_INDEX_URL = https://pypi.anaconda.org/astropy/simple https://pypi.anaconda.org/scientific-python-nightly-wheels/simple
     # Define the base test command here to allow us to add more flags for each tox factor
-    PYTEST_COMMAND = pytest -vvv -r fEs --pyargs dkist --cov-report=xml --cov=dkist --cov-config={toxinidir}/.coveragerc {toxinidir}/docs
+    PYTEST_COMMAND = pytest -vvv -r fEs --pyargs dkist --cov-report=xml --cov=dkist --cov-config={toxinidir}/.coveragerc {toxinidir}/docs --benchmark-skip
 deps =
     # For packages which publish nightly wheels this will pull the latest nightly
     devdeps: astropy>=0.0.dev0
     devdeps: numpy>=0.0.dev0
     devdeps: scipy>=0.0.dev0
     devdeps: matplotlib>=0.0.dev0
     devdeps: sunpy>=0.0.dev0
@@ -56,16 +57,20 @@
     oldestdeps: pip install -r requirements-min.txt cryptography<42 jsonschema==4.0.1
     pip freeze --all --no-input
 commands =
     # To run different commands for different factors exclude the factor from the default command like this
     # !online: {env:PYTEST_COMMAND} {posargs}
     # Then specify a specific one like this
     # online: {env:PYTEST_COMMAND} --remote-data=any {posargs}
-    !online: {env:PYTEST_COMMAND} {posargs}
-    online: {env:PYTEST_COMMAND} --remote-data=any {posargs}
+    {env:PYTEST_COMMAND} \
+    online: --remote-data=any \
+    # It's not possible to test the new schemas with the oldest dependencies
+    # as the new schemas require new dependent schemas
+    oldestdeps: -o asdf_schema_tests_enabled=false
+    {posargs}
 
 [testenv:codestyle]
 pypi_filter =
 skip_install = true
 description = Run all style and file checks with pre-commit
 deps =
     pre-commit
@@ -81,7 +86,12 @@
     docs
 commands =
     pip freeze --all --no-input
     # Disable parallel here due to https://github.com/astropy/astropy/issues/14916
     !notebooks: sphinx-build -j 1 --color -W --keep-going -b html -d _build/.doctrees . _build/html -D nb_execution_mode=off {posargs}
     notebooks: sphinx-build -j 1 --color -W --keep-going -b html -d _build/.doctrees . _build/html {posargs}
     python -c 'import pathlib; print("Documentation available under file://\{0\}".format(pathlib.Path(r"{toxinidir}") / "docs" / "_build" / "index.html"))'
+
+[testenv:benchmarks]
+description = Run benchmarks on PR and compare against main to ensure there are no performance regressions
+allowlist_externals=git
+commands = {env:PYTEST_COMMAND} -m benchmark --benchmark-autosave
```

